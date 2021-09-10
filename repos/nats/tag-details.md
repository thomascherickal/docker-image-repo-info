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
-	[`nats:2.5`](#nats25)
-	[`nats:2.5-alpine`](#nats25-alpine)
-	[`nats:2.5-alpine3.14`](#nats25-alpine314)
-	[`nats:2.5-linux`](#nats25-linux)
-	[`nats:2.5-nanoserver`](#nats25-nanoserver)
-	[`nats:2.5-nanoserver-1809`](#nats25-nanoserver-1809)
-	[`nats:2.5-scratch`](#nats25-scratch)
-	[`nats:2.5-windowsservercore`](#nats25-windowsservercore)
-	[`nats:2.5-windowsservercore-1809`](#nats25-windowsservercore-1809)
-	[`nats:2.5-windowsservercore-ltsc2016`](#nats25-windowsservercore-ltsc2016)
-	[`nats:2.5.0`](#nats250)
-	[`nats:2.5.0-alpine`](#nats250-alpine)
-	[`nats:2.5.0-alpine3.14`](#nats250-alpine314)
-	[`nats:2.5.0-linux`](#nats250-linux)
-	[`nats:2.5.0-nanoserver`](#nats250-nanoserver)
-	[`nats:2.5.0-nanoserver-1809`](#nats250-nanoserver-1809)
-	[`nats:2.5.0-scratch`](#nats250-scratch)
-	[`nats:2.5.0-windowsservercore`](#nats250-windowsservercore)
-	[`nats:2.5.0-windowsservercore-1809`](#nats250-windowsservercore-1809)
-	[`nats:2.5.0-windowsservercore-ltsc2016`](#nats250-windowsservercore-ltsc2016)
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
$ docker pull nats@sha256:c812e8c75705b49bfc4694743b59428590372ff6689425c86ea3ddd682fd8c58
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
$ docker pull nats@sha256:01dbe57fde6a40eecbd53edc6a418f3c9b1ddd85f03dd17e73ecef98a3b15318
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4546051 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80fcdf2bfe0f4a11267c9e8d06e5e52dce7dd9b41267e1a51d5e9df22c76bf9c`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 10 Sep 2021 00:20:41 GMT
COPY file:0b180121e1ef70970b020901a4b61990a8673ac9db99b94c348c5321333884ea in /nats-server 
# Fri, 10 Sep 2021 00:20:41 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 10 Sep 2021 00:20:41 GMT
EXPOSE 4222 6222 8222
# Fri, 10 Sep 2021 00:20:41 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 10 Sep 2021 00:20:42 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:9cee557b7d3312d12996f8c4338bf9ea02657256657ef77d46510c729d9be195`  
		Last Modified: Fri, 10 Sep 2021 00:21:32 GMT  
		Size: 4.5 MB (4545577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb24b942a0d168497adac7ad3190098a6f8dfa34ad2ef37932150fbce9336c9a`  
		Last Modified: Fri, 10 Sep 2021 00:21:31 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - linux; arm variant v6

```console
$ docker pull nats@sha256:b21057f1f945b501d03cf3c5c2d530f7961e1a3198e00bb297b7f69a849cc0e9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4210290 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:865dcd8a77138e8339293c7089adeee440305e68331df5533186ea36b8132f84`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 09 Sep 2021 23:50:15 GMT
COPY file:a60049eef2da0cbda1255e229e5e5c6377e3c3445b0cd16ce13a272139c7ce85 in /nats-server 
# Thu, 09 Sep 2021 23:50:16 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 09 Sep 2021 23:50:17 GMT
EXPOSE 4222 6222 8222
# Thu, 09 Sep 2021 23:50:17 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 09 Sep 2021 23:50:18 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b95232e9c9c31dfba5a6124fb74b4abc750a3fd6d5f89a13438a0b051430299e`  
		Last Modified: Thu, 09 Sep 2021 23:52:42 GMT  
		Size: 4.2 MB (4209813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2c01128246ad2a36efed9386a5ed63a01f73f3f56e54d059834ac17a2f64a48`  
		Last Modified: Thu, 09 Sep 2021 23:52:38 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - linux; arm variant v7

```console
$ docker pull nats@sha256:aafbb0b5e1b7412f9d0e71ddd6c3948c7080697882dd40ae20578b855ca40c1f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4206272 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:79f5a4fb5f9254997b2d7e573f24316740a167eb829bb23952ba05ff8304ddc1`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 10 Sep 2021 00:59:05 GMT
COPY file:7043dd814cd92048127f9905d58e9204d2968d9c03bbb7feba592c45a87e9963 in /nats-server 
# Fri, 10 Sep 2021 00:59:06 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 10 Sep 2021 00:59:06 GMT
EXPOSE 4222 6222 8222
# Fri, 10 Sep 2021 00:59:07 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 10 Sep 2021 00:59:07 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:8ae70a7ddee0b3bc3819ff86ee31d3295a37b10282b7ee0d14d3dd3c8dcb16c7`  
		Last Modified: Fri, 10 Sep 2021 01:01:28 GMT  
		Size: 4.2 MB (4205795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbbfbfa45875dc8bff20ba3a989407cf3ab8018f98f4277411dd068510c071c6`  
		Last Modified: Fri, 10 Sep 2021 01:01:25 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:24f192937e7bc371f7c2631055e49a51d489659d28f55b4fdf2eb5a19843a5ae
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4158958 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2cd8bb7e96599c9badd4424f86ef2d5f8561cfa0c4a4322057847c002da643a9`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 09 Sep 2021 23:40:25 GMT
COPY file:eda8ae8779fbfb7d34c95bc93fc8ce409cbd298cb302284f61ee4ebf6ac10b0e in /nats-server 
# Thu, 09 Sep 2021 23:40:26 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 09 Sep 2021 23:40:26 GMT
EXPOSE 4222 6222 8222
# Thu, 09 Sep 2021 23:40:26 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 09 Sep 2021 23:40:26 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:0c0083faeb4bd1e89eefb7cbc2a5556eb056acaba6107a833c271a1ca7cd8633`  
		Last Modified: Thu, 09 Sep 2021 23:41:48 GMT  
		Size: 4.2 MB (4158481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4227e148c1053ae9735f2dcc2ab35b83566aab7b85aa3d50395ec15be4630e26`  
		Last Modified: Thu, 09 Sep 2021 23:41:47 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - windows version 10.0.17763.2114; amd64

```console
$ docker pull nats@sha256:da56a6dd1f9556f706d9086ed48947ac745a5b9dd1e3bc0d988581858828c23c
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.4 MB (107351558 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:780da6fbe38cee622e2d2e69123219af601b417dada779a198cef0514370203e`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 05 Aug 2021 19:15:20 GMT
RUN Apply image 1809-amd64
# Wed, 25 Aug 2021 16:07:56 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 10 Sep 2021 00:16:45 GMT
RUN cmd /S /C #(nop) COPY file:13fac1899b72f2f26df9bd8ce320e46a5f7736306d7abf82ea7d657c16444fb9 in C:\nats-server.exe 
# Fri, 10 Sep 2021 00:16:46 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 10 Sep 2021 00:16:47 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Fri, 10 Sep 2021 00:16:47 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 10 Sep 2021 00:16:48 GMT
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
	-	`sha256:55bd340c78387be49377457ea8e39875e7be9b3799bdac42ff35c749d67b3940`  
		Last Modified: Fri, 10 Sep 2021 00:20:25 GMT  
		Size: 4.6 MB (4604102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76e6782c003b15abdb2161dc360ffef0eeb967b34fc78186d8d6085aacfc85fa`  
		Last Modified: Fri, 10 Sep 2021 00:20:20 GMT  
		Size: 1.8 KB (1777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf24d35e2c525beccaa7b227eda13492b401302f8ecc528e2a35118220e3f760`  
		Last Modified: Fri, 10 Sep 2021 00:20:20 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71603cdad9bbdd669dd86cda1c010a6f91d1a58de21eac052a29279f77bd247f`  
		Last Modified: Fri, 10 Sep 2021 00:20:20 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01477f3ed16729139c6a0a856de33336e03c4fb127df26c6e42b8157eaf1801b`  
		Last Modified: Fri, 10 Sep 2021 00:20:20 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-alpine`

```console
$ docker pull nats@sha256:52a8fe18f5c85cdd5cf0304eadb4e4a6a4208db9183fabc36140ff9ed7a813a3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-alpine` - linux; amd64

```console
$ docker pull nats@sha256:f6b2376c122defe213696fdbf87c7f365bdbbd60a6068fe88b1ab8aee27987d2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7647076 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b59fdb5895884cf160a5cabba5411b4a328b11aa2798042d794fe41e69fe8165`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 10 Sep 2021 00:20:12 GMT
ENV NATS_SERVER=2.5.0
# Fri, 10 Sep 2021 00:20:15 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='93f64cd14f04b4e7f6c3a2c10d09888be653406b7bc1a41f399ae44746388a5c' ;; 		armhf) natsArch='arm6'; sha256='12f38f6881cdcf27c0faebb7ab6580b40253c36dc1531d499a29c4998a009494' ;; 		armv7) natsArch='arm7'; sha256='fb3611b57a932f5c75310dee66597057ab65b442eb84d73b2c5fd9389eb6e518' ;; 		x86_64) natsArch='amd64'; sha256='4d2f4abb15b45618ce772659c9f3eca60f25266dfc976f0354430ad67c8fd886' ;; 		x86) natsArch='386'; sha256='776aecc77c33146d88e6b3cb1787097f9817122182f49f7243c0ea3fd62ad029' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 10 Sep 2021 00:20:15 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 10 Sep 2021 00:20:15 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 10 Sep 2021 00:20:15 GMT
EXPOSE 4222 6222 8222
# Fri, 10 Sep 2021 00:20:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 10 Sep 2021 00:20:16 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59a9809baa02715a6c4ccdb1ebc94edaf948058be9f97cea623426ca670b426e`  
		Last Modified: Fri, 10 Sep 2021 00:21:08 GMT  
		Size: 4.8 MB (4831663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68c0794b9b379d130866e40babeef9f4557514bcc2c88194e89b90081ef7ad12`  
		Last Modified: Fri, 10 Sep 2021 00:21:08 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:240551b5739b209d882cd7b4f76138b9188aac1a497ff32a469526302056dd98`  
		Last Modified: Fri, 10 Sep 2021 00:21:07 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:c516621cb4dc61ad9db1927cdcec7210328be6d7b813acb688016584d61be212
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7121422 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c48580010dc9af32e7a019914f078134ae513ef77280b7877fe7fd47665426b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:49:29 GMT
ADD file:1c1c4520d49cb6e8f795f3b953d1ed3c3c77868b98b53a455169c254fcec5acd in / 
# Fri, 27 Aug 2021 17:49:30 GMT
CMD ["/bin/sh"]
# Thu, 09 Sep 2021 23:49:46 GMT
ENV NATS_SERVER=2.5.0
# Thu, 09 Sep 2021 23:49:51 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='93f64cd14f04b4e7f6c3a2c10d09888be653406b7bc1a41f399ae44746388a5c' ;; 		armhf) natsArch='arm6'; sha256='12f38f6881cdcf27c0faebb7ab6580b40253c36dc1531d499a29c4998a009494' ;; 		armv7) natsArch='arm7'; sha256='fb3611b57a932f5c75310dee66597057ab65b442eb84d73b2c5fd9389eb6e518' ;; 		x86_64) natsArch='amd64'; sha256='4d2f4abb15b45618ce772659c9f3eca60f25266dfc976f0354430ad67c8fd886' ;; 		x86) natsArch='386'; sha256='776aecc77c33146d88e6b3cb1787097f9817122182f49f7243c0ea3fd62ad029' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 09 Sep 2021 23:49:51 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 09 Sep 2021 23:49:52 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 09 Sep 2021 23:49:52 GMT
EXPOSE 4222 6222 8222
# Thu, 09 Sep 2021 23:49:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 09 Sep 2021 23:49:53 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:2e78c0f86ba9a1fed30df20cb48c9cc73e9626399f12749d36b892ff99c0ecf5`  
		Last Modified: Fri, 27 Aug 2021 17:50:55 GMT  
		Size: 2.6 MB (2627447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75b214a44f07577985e2f01798e9acf02be903c28022f74d244b22418b31e815`  
		Last Modified: Thu, 09 Sep 2021 23:52:03 GMT  
		Size: 4.5 MB (4493006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d232ac6d6c1f822be800be02acbb341f7abe35b05bd13a0857df02fd1cc600a6`  
		Last Modified: Thu, 09 Sep 2021 23:52:01 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e364400828db299d750b3bcc80b1e3b1df2f7abe62c5d6293f3c7e22d93e20a`  
		Last Modified: Thu, 09 Sep 2021 23:52:00 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:c5a16f99958e4ae6f318a577619242a7d168fc47e07883d8adbc1701faa36ab4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.9 MB (6918058 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b6128ceec7a63c74e316f6b3bda400e98def18ed14e046a0177a1095946dd8e2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:57:31 GMT
ADD file:a7da7992ccea54d3295231027614f138aa45c4d4a25ea6ec9bf7b316b9f67d95 in / 
# Fri, 27 Aug 2021 17:57:32 GMT
CMD ["/bin/sh"]
# Fri, 10 Sep 2021 00:58:26 GMT
ENV NATS_SERVER=2.5.0
# Fri, 10 Sep 2021 00:58:31 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='93f64cd14f04b4e7f6c3a2c10d09888be653406b7bc1a41f399ae44746388a5c' ;; 		armhf) natsArch='arm6'; sha256='12f38f6881cdcf27c0faebb7ab6580b40253c36dc1531d499a29c4998a009494' ;; 		armv7) natsArch='arm7'; sha256='fb3611b57a932f5c75310dee66597057ab65b442eb84d73b2c5fd9389eb6e518' ;; 		x86_64) natsArch='amd64'; sha256='4d2f4abb15b45618ce772659c9f3eca60f25266dfc976f0354430ad67c8fd886' ;; 		x86) natsArch='386'; sha256='776aecc77c33146d88e6b3cb1787097f9817122182f49f7243c0ea3fd62ad029' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 10 Sep 2021 00:58:32 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 10 Sep 2021 00:58:32 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 10 Sep 2021 00:58:33 GMT
EXPOSE 4222 6222 8222
# Fri, 10 Sep 2021 00:58:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 10 Sep 2021 00:58:34 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:a14774a5a62e0f454febaec7cb603e18a6a8e25ef9da4a4da85b155bdd5e5a7a`  
		Last Modified: Fri, 27 Aug 2021 17:59:00 GMT  
		Size: 2.4 MB (2430419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2edd63df5776202ac2717836b8350736f3e046021c53b49e6e872ef9f4a960a9`  
		Last Modified: Fri, 10 Sep 2021 01:00:49 GMT  
		Size: 4.5 MB (4486667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d073c5b9595fcde55c46ccb0f54148caba30c630427ffcdfe9f03a4e84be10ec`  
		Last Modified: Fri, 10 Sep 2021 01:00:46 GMT  
		Size: 559.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15f66a2a44784b8ce7529a34b470376f9a52740980b2b05baf8525ec5f4a39f2`  
		Last Modified: Fri, 10 Sep 2021 01:00:46 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:88b4d8f2f54f207d5400e8d3e9037d55ca8d2969b126e07d833c6d3464f93300
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7156798 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f803b2b0ed9b56df4cac8c3a03dfd789e480a622c1f3a282ecee5fd0f937d9e5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Thu, 09 Sep 2021 23:40:02 GMT
ENV NATS_SERVER=2.5.0
# Thu, 09 Sep 2021 23:40:05 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='93f64cd14f04b4e7f6c3a2c10d09888be653406b7bc1a41f399ae44746388a5c' ;; 		armhf) natsArch='arm6'; sha256='12f38f6881cdcf27c0faebb7ab6580b40253c36dc1531d499a29c4998a009494' ;; 		armv7) natsArch='arm7'; sha256='fb3611b57a932f5c75310dee66597057ab65b442eb84d73b2c5fd9389eb6e518' ;; 		x86_64) natsArch='amd64'; sha256='4d2f4abb15b45618ce772659c9f3eca60f25266dfc976f0354430ad67c8fd886' ;; 		x86) natsArch='386'; sha256='776aecc77c33146d88e6b3cb1787097f9817122182f49f7243c0ea3fd62ad029' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 09 Sep 2021 23:40:05 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 09 Sep 2021 23:40:05 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 09 Sep 2021 23:40:05 GMT
EXPOSE 4222 6222 8222
# Thu, 09 Sep 2021 23:40:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 09 Sep 2021 23:40:06 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:552d1f2373af9bfe12033568ebbfb0ccbb0de11279f9a415a29207e264d7f4d9`  
		Last Modified: Fri, 27 Aug 2021 17:40:18 GMT  
		Size: 2.7 MB (2711827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49450e2f2462d1e207a865d4a084154f6a3c5edc2b3b4954d34d4e1ce75d38f2`  
		Last Modified: Thu, 09 Sep 2021 23:41:18 GMT  
		Size: 4.4 MB (4444005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edeb0b05b16add9a16e4a8bc8c1eced6c1f60f58ac669216dbbf93cb9bce40d2`  
		Last Modified: Thu, 09 Sep 2021 23:41:18 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67be552e94a6cfc686543e5bfa0c1a6bca72bc9dce939fb9f3e43c4a77f5e6e3`  
		Last Modified: Thu, 09 Sep 2021 23:41:18 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-alpine3.14`

```console
$ docker pull nats@sha256:52a8fe18f5c85cdd5cf0304eadb4e4a6a4208db9183fabc36140ff9ed7a813a3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-alpine3.14` - linux; amd64

```console
$ docker pull nats@sha256:f6b2376c122defe213696fdbf87c7f365bdbbd60a6068fe88b1ab8aee27987d2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7647076 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b59fdb5895884cf160a5cabba5411b4a328b11aa2798042d794fe41e69fe8165`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 10 Sep 2021 00:20:12 GMT
ENV NATS_SERVER=2.5.0
# Fri, 10 Sep 2021 00:20:15 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='93f64cd14f04b4e7f6c3a2c10d09888be653406b7bc1a41f399ae44746388a5c' ;; 		armhf) natsArch='arm6'; sha256='12f38f6881cdcf27c0faebb7ab6580b40253c36dc1531d499a29c4998a009494' ;; 		armv7) natsArch='arm7'; sha256='fb3611b57a932f5c75310dee66597057ab65b442eb84d73b2c5fd9389eb6e518' ;; 		x86_64) natsArch='amd64'; sha256='4d2f4abb15b45618ce772659c9f3eca60f25266dfc976f0354430ad67c8fd886' ;; 		x86) natsArch='386'; sha256='776aecc77c33146d88e6b3cb1787097f9817122182f49f7243c0ea3fd62ad029' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 10 Sep 2021 00:20:15 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 10 Sep 2021 00:20:15 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 10 Sep 2021 00:20:15 GMT
EXPOSE 4222 6222 8222
# Fri, 10 Sep 2021 00:20:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 10 Sep 2021 00:20:16 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59a9809baa02715a6c4ccdb1ebc94edaf948058be9f97cea623426ca670b426e`  
		Last Modified: Fri, 10 Sep 2021 00:21:08 GMT  
		Size: 4.8 MB (4831663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68c0794b9b379d130866e40babeef9f4557514bcc2c88194e89b90081ef7ad12`  
		Last Modified: Fri, 10 Sep 2021 00:21:08 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:240551b5739b209d882cd7b4f76138b9188aac1a497ff32a469526302056dd98`  
		Last Modified: Fri, 10 Sep 2021 00:21:07 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.14` - linux; arm variant v6

```console
$ docker pull nats@sha256:c516621cb4dc61ad9db1927cdcec7210328be6d7b813acb688016584d61be212
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7121422 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c48580010dc9af32e7a019914f078134ae513ef77280b7877fe7fd47665426b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:49:29 GMT
ADD file:1c1c4520d49cb6e8f795f3b953d1ed3c3c77868b98b53a455169c254fcec5acd in / 
# Fri, 27 Aug 2021 17:49:30 GMT
CMD ["/bin/sh"]
# Thu, 09 Sep 2021 23:49:46 GMT
ENV NATS_SERVER=2.5.0
# Thu, 09 Sep 2021 23:49:51 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='93f64cd14f04b4e7f6c3a2c10d09888be653406b7bc1a41f399ae44746388a5c' ;; 		armhf) natsArch='arm6'; sha256='12f38f6881cdcf27c0faebb7ab6580b40253c36dc1531d499a29c4998a009494' ;; 		armv7) natsArch='arm7'; sha256='fb3611b57a932f5c75310dee66597057ab65b442eb84d73b2c5fd9389eb6e518' ;; 		x86_64) natsArch='amd64'; sha256='4d2f4abb15b45618ce772659c9f3eca60f25266dfc976f0354430ad67c8fd886' ;; 		x86) natsArch='386'; sha256='776aecc77c33146d88e6b3cb1787097f9817122182f49f7243c0ea3fd62ad029' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 09 Sep 2021 23:49:51 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 09 Sep 2021 23:49:52 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 09 Sep 2021 23:49:52 GMT
EXPOSE 4222 6222 8222
# Thu, 09 Sep 2021 23:49:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 09 Sep 2021 23:49:53 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:2e78c0f86ba9a1fed30df20cb48c9cc73e9626399f12749d36b892ff99c0ecf5`  
		Last Modified: Fri, 27 Aug 2021 17:50:55 GMT  
		Size: 2.6 MB (2627447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75b214a44f07577985e2f01798e9acf02be903c28022f74d244b22418b31e815`  
		Last Modified: Thu, 09 Sep 2021 23:52:03 GMT  
		Size: 4.5 MB (4493006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d232ac6d6c1f822be800be02acbb341f7abe35b05bd13a0857df02fd1cc600a6`  
		Last Modified: Thu, 09 Sep 2021 23:52:01 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e364400828db299d750b3bcc80b1e3b1df2f7abe62c5d6293f3c7e22d93e20a`  
		Last Modified: Thu, 09 Sep 2021 23:52:00 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.14` - linux; arm variant v7

```console
$ docker pull nats@sha256:c5a16f99958e4ae6f318a577619242a7d168fc47e07883d8adbc1701faa36ab4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.9 MB (6918058 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b6128ceec7a63c74e316f6b3bda400e98def18ed14e046a0177a1095946dd8e2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:57:31 GMT
ADD file:a7da7992ccea54d3295231027614f138aa45c4d4a25ea6ec9bf7b316b9f67d95 in / 
# Fri, 27 Aug 2021 17:57:32 GMT
CMD ["/bin/sh"]
# Fri, 10 Sep 2021 00:58:26 GMT
ENV NATS_SERVER=2.5.0
# Fri, 10 Sep 2021 00:58:31 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='93f64cd14f04b4e7f6c3a2c10d09888be653406b7bc1a41f399ae44746388a5c' ;; 		armhf) natsArch='arm6'; sha256='12f38f6881cdcf27c0faebb7ab6580b40253c36dc1531d499a29c4998a009494' ;; 		armv7) natsArch='arm7'; sha256='fb3611b57a932f5c75310dee66597057ab65b442eb84d73b2c5fd9389eb6e518' ;; 		x86_64) natsArch='amd64'; sha256='4d2f4abb15b45618ce772659c9f3eca60f25266dfc976f0354430ad67c8fd886' ;; 		x86) natsArch='386'; sha256='776aecc77c33146d88e6b3cb1787097f9817122182f49f7243c0ea3fd62ad029' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 10 Sep 2021 00:58:32 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 10 Sep 2021 00:58:32 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 10 Sep 2021 00:58:33 GMT
EXPOSE 4222 6222 8222
# Fri, 10 Sep 2021 00:58:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 10 Sep 2021 00:58:34 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:a14774a5a62e0f454febaec7cb603e18a6a8e25ef9da4a4da85b155bdd5e5a7a`  
		Last Modified: Fri, 27 Aug 2021 17:59:00 GMT  
		Size: 2.4 MB (2430419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2edd63df5776202ac2717836b8350736f3e046021c53b49e6e872ef9f4a960a9`  
		Last Modified: Fri, 10 Sep 2021 01:00:49 GMT  
		Size: 4.5 MB (4486667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d073c5b9595fcde55c46ccb0f54148caba30c630427ffcdfe9f03a4e84be10ec`  
		Last Modified: Fri, 10 Sep 2021 01:00:46 GMT  
		Size: 559.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15f66a2a44784b8ce7529a34b470376f9a52740980b2b05baf8525ec5f4a39f2`  
		Last Modified: Fri, 10 Sep 2021 01:00:46 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.14` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:88b4d8f2f54f207d5400e8d3e9037d55ca8d2969b126e07d833c6d3464f93300
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7156798 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f803b2b0ed9b56df4cac8c3a03dfd789e480a622c1f3a282ecee5fd0f937d9e5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Thu, 09 Sep 2021 23:40:02 GMT
ENV NATS_SERVER=2.5.0
# Thu, 09 Sep 2021 23:40:05 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='93f64cd14f04b4e7f6c3a2c10d09888be653406b7bc1a41f399ae44746388a5c' ;; 		armhf) natsArch='arm6'; sha256='12f38f6881cdcf27c0faebb7ab6580b40253c36dc1531d499a29c4998a009494' ;; 		armv7) natsArch='arm7'; sha256='fb3611b57a932f5c75310dee66597057ab65b442eb84d73b2c5fd9389eb6e518' ;; 		x86_64) natsArch='amd64'; sha256='4d2f4abb15b45618ce772659c9f3eca60f25266dfc976f0354430ad67c8fd886' ;; 		x86) natsArch='386'; sha256='776aecc77c33146d88e6b3cb1787097f9817122182f49f7243c0ea3fd62ad029' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 09 Sep 2021 23:40:05 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 09 Sep 2021 23:40:05 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 09 Sep 2021 23:40:05 GMT
EXPOSE 4222 6222 8222
# Thu, 09 Sep 2021 23:40:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 09 Sep 2021 23:40:06 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:552d1f2373af9bfe12033568ebbfb0ccbb0de11279f9a415a29207e264d7f4d9`  
		Last Modified: Fri, 27 Aug 2021 17:40:18 GMT  
		Size: 2.7 MB (2711827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49450e2f2462d1e207a865d4a084154f6a3c5edc2b3b4954d34d4e1ce75d38f2`  
		Last Modified: Thu, 09 Sep 2021 23:41:18 GMT  
		Size: 4.4 MB (4444005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edeb0b05b16add9a16e4a8bc8c1eced6c1f60f58ac669216dbbf93cb9bce40d2`  
		Last Modified: Thu, 09 Sep 2021 23:41:18 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67be552e94a6cfc686543e5bfa0c1a6bca72bc9dce939fb9f3e43c4a77f5e6e3`  
		Last Modified: Thu, 09 Sep 2021 23:41:18 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-linux`

```console
$ docker pull nats@sha256:6808dfb3132c301916bbeb4241ae1f3c0be5dca763a6c0be6180ca1bd6da298a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-linux` - linux; amd64

```console
$ docker pull nats@sha256:01dbe57fde6a40eecbd53edc6a418f3c9b1ddd85f03dd17e73ecef98a3b15318
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4546051 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80fcdf2bfe0f4a11267c9e8d06e5e52dce7dd9b41267e1a51d5e9df22c76bf9c`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 10 Sep 2021 00:20:41 GMT
COPY file:0b180121e1ef70970b020901a4b61990a8673ac9db99b94c348c5321333884ea in /nats-server 
# Fri, 10 Sep 2021 00:20:41 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 10 Sep 2021 00:20:41 GMT
EXPOSE 4222 6222 8222
# Fri, 10 Sep 2021 00:20:41 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 10 Sep 2021 00:20:42 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:9cee557b7d3312d12996f8c4338bf9ea02657256657ef77d46510c729d9be195`  
		Last Modified: Fri, 10 Sep 2021 00:21:32 GMT  
		Size: 4.5 MB (4545577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb24b942a0d168497adac7ad3190098a6f8dfa34ad2ef37932150fbce9336c9a`  
		Last Modified: Fri, 10 Sep 2021 00:21:31 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:b21057f1f945b501d03cf3c5c2d530f7961e1a3198e00bb297b7f69a849cc0e9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4210290 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:865dcd8a77138e8339293c7089adeee440305e68331df5533186ea36b8132f84`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 09 Sep 2021 23:50:15 GMT
COPY file:a60049eef2da0cbda1255e229e5e5c6377e3c3445b0cd16ce13a272139c7ce85 in /nats-server 
# Thu, 09 Sep 2021 23:50:16 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 09 Sep 2021 23:50:17 GMT
EXPOSE 4222 6222 8222
# Thu, 09 Sep 2021 23:50:17 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 09 Sep 2021 23:50:18 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b95232e9c9c31dfba5a6124fb74b4abc750a3fd6d5f89a13438a0b051430299e`  
		Last Modified: Thu, 09 Sep 2021 23:52:42 GMT  
		Size: 4.2 MB (4209813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2c01128246ad2a36efed9386a5ed63a01f73f3f56e54d059834ac17a2f64a48`  
		Last Modified: Thu, 09 Sep 2021 23:52:38 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:aafbb0b5e1b7412f9d0e71ddd6c3948c7080697882dd40ae20578b855ca40c1f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4206272 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:79f5a4fb5f9254997b2d7e573f24316740a167eb829bb23952ba05ff8304ddc1`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 10 Sep 2021 00:59:05 GMT
COPY file:7043dd814cd92048127f9905d58e9204d2968d9c03bbb7feba592c45a87e9963 in /nats-server 
# Fri, 10 Sep 2021 00:59:06 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 10 Sep 2021 00:59:06 GMT
EXPOSE 4222 6222 8222
# Fri, 10 Sep 2021 00:59:07 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 10 Sep 2021 00:59:07 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:8ae70a7ddee0b3bc3819ff86ee31d3295a37b10282b7ee0d14d3dd3c8dcb16c7`  
		Last Modified: Fri, 10 Sep 2021 01:01:28 GMT  
		Size: 4.2 MB (4205795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbbfbfa45875dc8bff20ba3a989407cf3ab8018f98f4277411dd068510c071c6`  
		Last Modified: Fri, 10 Sep 2021 01:01:25 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:24f192937e7bc371f7c2631055e49a51d489659d28f55b4fdf2eb5a19843a5ae
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4158958 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2cd8bb7e96599c9badd4424f86ef2d5f8561cfa0c4a4322057847c002da643a9`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 09 Sep 2021 23:40:25 GMT
COPY file:eda8ae8779fbfb7d34c95bc93fc8ce409cbd298cb302284f61ee4ebf6ac10b0e in /nats-server 
# Thu, 09 Sep 2021 23:40:26 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 09 Sep 2021 23:40:26 GMT
EXPOSE 4222 6222 8222
# Thu, 09 Sep 2021 23:40:26 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 09 Sep 2021 23:40:26 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:0c0083faeb4bd1e89eefb7cbc2a5556eb056acaba6107a833c271a1ca7cd8633`  
		Last Modified: Thu, 09 Sep 2021 23:41:48 GMT  
		Size: 4.2 MB (4158481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4227e148c1053ae9735f2dcc2ab35b83566aab7b85aa3d50395ec15be4630e26`  
		Last Modified: Thu, 09 Sep 2021 23:41:47 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-nanoserver`

```console
$ docker pull nats@sha256:5b8ea050ee708eb4017db4e1cb913456e468e82c227eb67a070974651446cfd9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2114; amd64

### `nats:2-nanoserver` - windows version 10.0.17763.2114; amd64

```console
$ docker pull nats@sha256:da56a6dd1f9556f706d9086ed48947ac745a5b9dd1e3bc0d988581858828c23c
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.4 MB (107351558 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:780da6fbe38cee622e2d2e69123219af601b417dada779a198cef0514370203e`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 05 Aug 2021 19:15:20 GMT
RUN Apply image 1809-amd64
# Wed, 25 Aug 2021 16:07:56 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 10 Sep 2021 00:16:45 GMT
RUN cmd /S /C #(nop) COPY file:13fac1899b72f2f26df9bd8ce320e46a5f7736306d7abf82ea7d657c16444fb9 in C:\nats-server.exe 
# Fri, 10 Sep 2021 00:16:46 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 10 Sep 2021 00:16:47 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Fri, 10 Sep 2021 00:16:47 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 10 Sep 2021 00:16:48 GMT
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
	-	`sha256:55bd340c78387be49377457ea8e39875e7be9b3799bdac42ff35c749d67b3940`  
		Last Modified: Fri, 10 Sep 2021 00:20:25 GMT  
		Size: 4.6 MB (4604102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76e6782c003b15abdb2161dc360ffef0eeb967b34fc78186d8d6085aacfc85fa`  
		Last Modified: Fri, 10 Sep 2021 00:20:20 GMT  
		Size: 1.8 KB (1777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf24d35e2c525beccaa7b227eda13492b401302f8ecc528e2a35118220e3f760`  
		Last Modified: Fri, 10 Sep 2021 00:20:20 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71603cdad9bbdd669dd86cda1c010a6f91d1a58de21eac052a29279f77bd247f`  
		Last Modified: Fri, 10 Sep 2021 00:20:20 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01477f3ed16729139c6a0a856de33336e03c4fb127df26c6e42b8157eaf1801b`  
		Last Modified: Fri, 10 Sep 2021 00:20:20 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-nanoserver-1809`

```console
$ docker pull nats@sha256:5b8ea050ee708eb4017db4e1cb913456e468e82c227eb67a070974651446cfd9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2114; amd64

### `nats:2-nanoserver-1809` - windows version 10.0.17763.2114; amd64

```console
$ docker pull nats@sha256:da56a6dd1f9556f706d9086ed48947ac745a5b9dd1e3bc0d988581858828c23c
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.4 MB (107351558 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:780da6fbe38cee622e2d2e69123219af601b417dada779a198cef0514370203e`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 05 Aug 2021 19:15:20 GMT
RUN Apply image 1809-amd64
# Wed, 25 Aug 2021 16:07:56 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 10 Sep 2021 00:16:45 GMT
RUN cmd /S /C #(nop) COPY file:13fac1899b72f2f26df9bd8ce320e46a5f7736306d7abf82ea7d657c16444fb9 in C:\nats-server.exe 
# Fri, 10 Sep 2021 00:16:46 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 10 Sep 2021 00:16:47 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Fri, 10 Sep 2021 00:16:47 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 10 Sep 2021 00:16:48 GMT
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
	-	`sha256:55bd340c78387be49377457ea8e39875e7be9b3799bdac42ff35c749d67b3940`  
		Last Modified: Fri, 10 Sep 2021 00:20:25 GMT  
		Size: 4.6 MB (4604102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76e6782c003b15abdb2161dc360ffef0eeb967b34fc78186d8d6085aacfc85fa`  
		Last Modified: Fri, 10 Sep 2021 00:20:20 GMT  
		Size: 1.8 KB (1777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf24d35e2c525beccaa7b227eda13492b401302f8ecc528e2a35118220e3f760`  
		Last Modified: Fri, 10 Sep 2021 00:20:20 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71603cdad9bbdd669dd86cda1c010a6f91d1a58de21eac052a29279f77bd247f`  
		Last Modified: Fri, 10 Sep 2021 00:20:20 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01477f3ed16729139c6a0a856de33336e03c4fb127df26c6e42b8157eaf1801b`  
		Last Modified: Fri, 10 Sep 2021 00:20:20 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-scratch`

```console
$ docker pull nats@sha256:6808dfb3132c301916bbeb4241ae1f3c0be5dca763a6c0be6180ca1bd6da298a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-scratch` - linux; amd64

```console
$ docker pull nats@sha256:01dbe57fde6a40eecbd53edc6a418f3c9b1ddd85f03dd17e73ecef98a3b15318
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4546051 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80fcdf2bfe0f4a11267c9e8d06e5e52dce7dd9b41267e1a51d5e9df22c76bf9c`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 10 Sep 2021 00:20:41 GMT
COPY file:0b180121e1ef70970b020901a4b61990a8673ac9db99b94c348c5321333884ea in /nats-server 
# Fri, 10 Sep 2021 00:20:41 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 10 Sep 2021 00:20:41 GMT
EXPOSE 4222 6222 8222
# Fri, 10 Sep 2021 00:20:41 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 10 Sep 2021 00:20:42 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:9cee557b7d3312d12996f8c4338bf9ea02657256657ef77d46510c729d9be195`  
		Last Modified: Fri, 10 Sep 2021 00:21:32 GMT  
		Size: 4.5 MB (4545577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb24b942a0d168497adac7ad3190098a6f8dfa34ad2ef37932150fbce9336c9a`  
		Last Modified: Fri, 10 Sep 2021 00:21:31 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:b21057f1f945b501d03cf3c5c2d530f7961e1a3198e00bb297b7f69a849cc0e9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4210290 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:865dcd8a77138e8339293c7089adeee440305e68331df5533186ea36b8132f84`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 09 Sep 2021 23:50:15 GMT
COPY file:a60049eef2da0cbda1255e229e5e5c6377e3c3445b0cd16ce13a272139c7ce85 in /nats-server 
# Thu, 09 Sep 2021 23:50:16 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 09 Sep 2021 23:50:17 GMT
EXPOSE 4222 6222 8222
# Thu, 09 Sep 2021 23:50:17 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 09 Sep 2021 23:50:18 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b95232e9c9c31dfba5a6124fb74b4abc750a3fd6d5f89a13438a0b051430299e`  
		Last Modified: Thu, 09 Sep 2021 23:52:42 GMT  
		Size: 4.2 MB (4209813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2c01128246ad2a36efed9386a5ed63a01f73f3f56e54d059834ac17a2f64a48`  
		Last Modified: Thu, 09 Sep 2021 23:52:38 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:aafbb0b5e1b7412f9d0e71ddd6c3948c7080697882dd40ae20578b855ca40c1f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4206272 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:79f5a4fb5f9254997b2d7e573f24316740a167eb829bb23952ba05ff8304ddc1`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 10 Sep 2021 00:59:05 GMT
COPY file:7043dd814cd92048127f9905d58e9204d2968d9c03bbb7feba592c45a87e9963 in /nats-server 
# Fri, 10 Sep 2021 00:59:06 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 10 Sep 2021 00:59:06 GMT
EXPOSE 4222 6222 8222
# Fri, 10 Sep 2021 00:59:07 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 10 Sep 2021 00:59:07 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:8ae70a7ddee0b3bc3819ff86ee31d3295a37b10282b7ee0d14d3dd3c8dcb16c7`  
		Last Modified: Fri, 10 Sep 2021 01:01:28 GMT  
		Size: 4.2 MB (4205795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbbfbfa45875dc8bff20ba3a989407cf3ab8018f98f4277411dd068510c071c6`  
		Last Modified: Fri, 10 Sep 2021 01:01:25 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:24f192937e7bc371f7c2631055e49a51d489659d28f55b4fdf2eb5a19843a5ae
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4158958 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2cd8bb7e96599c9badd4424f86ef2d5f8561cfa0c4a4322057847c002da643a9`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 09 Sep 2021 23:40:25 GMT
COPY file:eda8ae8779fbfb7d34c95bc93fc8ce409cbd298cb302284f61ee4ebf6ac10b0e in /nats-server 
# Thu, 09 Sep 2021 23:40:26 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 09 Sep 2021 23:40:26 GMT
EXPOSE 4222 6222 8222
# Thu, 09 Sep 2021 23:40:26 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 09 Sep 2021 23:40:26 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:0c0083faeb4bd1e89eefb7cbc2a5556eb056acaba6107a833c271a1ca7cd8633`  
		Last Modified: Thu, 09 Sep 2021 23:41:48 GMT  
		Size: 4.2 MB (4158481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4227e148c1053ae9735f2dcc2ab35b83566aab7b85aa3d50395ec15be4630e26`  
		Last Modified: Thu, 09 Sep 2021 23:41:47 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-windowsservercore`

```console
$ docker pull nats@sha256:fc4b18ccf5f4b0e559c7deb1e5c01e21f0ba9699b9a6966fce5548faec1f5dfb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.2114; amd64
	-	windows version 10.0.14393.4583; amd64

### `nats:2-windowsservercore` - windows version 10.0.17763.2114; amd64

```console
$ docker pull nats@sha256:ea5bd03ca8c905a9bb8df9bcefe1c70aada9fce64c82d90932dfaf570332087a
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2691339003 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce14639524af68868fed35dda40295ffe16c35eb58b5038f43989d7d60f7059d`
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
# Fri, 10 Sep 2021 00:14:04 GMT
ENV NATS_SERVER=2.5.0
# Fri, 10 Sep 2021 00:14:05 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.5.0/nats-server-v2.5.0-windows-amd64.zip
# Fri, 10 Sep 2021 00:14:06 GMT
ENV NATS_SERVER_SHASUM=0eae96ad4555f5060b0b6325ba972566b404cd8930b3168b9c0ffe911d15c5d8
# Fri, 10 Sep 2021 00:15:08 GMT
RUN Set-PSDebug -Trace 2
# Fri, 10 Sep 2021 00:16:32 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 10 Sep 2021 00:16:33 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 10 Sep 2021 00:16:34 GMT
EXPOSE 4222 6222 8222
# Fri, 10 Sep 2021 00:16:34 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 10 Sep 2021 00:16:35 GMT
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
	-	`sha256:4c32056c4535002b64e42d1424edb3a7ac778c308d2d9109f33d738d59c85454`  
		Last Modified: Fri, 10 Sep 2021 00:20:02 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb115761571c4ba7b8b719d8ee1587c8898f7e13246d1a92ee2283c0f929a1b1`  
		Last Modified: Fri, 10 Sep 2021 00:20:01 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd93d02cef774a55aa7c6f566b3b5718436cbdae64582cc888ef3b1efe452735`  
		Last Modified: Fri, 10 Sep 2021 00:20:01 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f28336574033153776b7149c4d079b46a95608a291563bc581fc8b029d9399c`  
		Last Modified: Fri, 10 Sep 2021 00:20:02 GMT  
		Size: 372.4 KB (372418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcce3c7fbad71cacb4533bac881f55d312123c387549ca7840f402aa108fb59d`  
		Last Modified: Fri, 10 Sep 2021 00:20:05 GMT  
		Size: 5.0 MB (4955556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0d387c2eda58f8b5f8c3889645ec5e1a977b681cb17de77c04de1c643341b18`  
		Last Modified: Fri, 10 Sep 2021 00:19:59 GMT  
		Size: 1.9 KB (1944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f70bbbc8ecda378ae0099ea8e49350ba7d78be681cd5defc71e6f624abca5d7`  
		Last Modified: Fri, 10 Sep 2021 00:19:59 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76b0025f319f789e7c26483abcf5ca7944dc5a1f0a071023d2415526aa310d40`  
		Last Modified: Fri, 10 Sep 2021 00:19:59 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99ff7344cf8ed7957719594d8f9fe4d78b0ef7acc3755bb1962febcf166ac4ce`  
		Last Modified: Fri, 10 Sep 2021 00:19:59 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-windowsservercore` - windows version 10.0.14393.4583; amd64

```console
$ docker pull nats@sha256:7f318bb6bf586d9b74b6b8e8097ffabf3b4d16c43c5b9b2dd62d532713aa0305
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6276274196 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5716654340a54076fb48e8d797d45b91a2e56551a534fb6d800d7d6c61262257`
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
# Fri, 10 Sep 2021 00:16:55 GMT
ENV NATS_SERVER=2.5.0
# Fri, 10 Sep 2021 00:16:56 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.5.0/nats-server-v2.5.0-windows-amd64.zip
# Fri, 10 Sep 2021 00:16:57 GMT
ENV NATS_SERVER_SHASUM=0eae96ad4555f5060b0b6325ba972566b404cd8930b3168b9c0ffe911d15c5d8
# Fri, 10 Sep 2021 00:17:43 GMT
RUN Set-PSDebug -Trace 2
# Fri, 10 Sep 2021 00:19:14 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 10 Sep 2021 00:19:15 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 10 Sep 2021 00:19:16 GMT
EXPOSE 4222 6222 8222
# Fri, 10 Sep 2021 00:19:17 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 10 Sep 2021 00:19:18 GMT
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
	-	`sha256:786675b79153c67ad039b6b8a55171a8167b2ff8c8186ccb7c5cab0b01f47767`  
		Last Modified: Fri, 10 Sep 2021 00:20:42 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65445b8a1c334a2efce7d34289af9fa682427cba808180c96ce46f39f765e9b5`  
		Last Modified: Fri, 10 Sep 2021 00:20:42 GMT  
		Size: 1.4 KB (1358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08647f69046830b98e59118ace63049f027ad1786cc2aaad037990a4e7a87344`  
		Last Modified: Fri, 10 Sep 2021 00:20:42 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b50cf5c744e8952689c263dbc9800bbe4a032fb4c8df3c8e5028092bdb2a5c9c`  
		Last Modified: Fri, 10 Sep 2021 00:20:42 GMT  
		Size: 338.0 KB (337964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:459c701464a835b4d39cc3183fff454248a3045bb433c26b0430f06e91acf1bb`  
		Last Modified: Fri, 10 Sep 2021 00:20:41 GMT  
		Size: 5.0 MB (4957179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cb2fb143896bcefca1d8ad8640f3146b771f5b284f01be2b849a048d9ac9eeb`  
		Last Modified: Fri, 10 Sep 2021 00:20:40 GMT  
		Size: 1.9 KB (1938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d9f7d515a8e73d005392fc0bccc42761025b86ab370cffe210a552fe53d1cbe`  
		Last Modified: Fri, 10 Sep 2021 00:20:40 GMT  
		Size: 1.4 KB (1380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d68902a6dec2675ab57a60716c10ce8a85e58fe54d7abea307bc340452e882a`  
		Last Modified: Fri, 10 Sep 2021 00:20:39 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37e0389f87abc858cef1a365e6b548d7d7762be571608840bc715ef352c41084`  
		Last Modified: Fri, 10 Sep 2021 00:20:39 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-windowsservercore-1809`

```console
$ docker pull nats@sha256:4e912b79015d0859d5b6c675d055f80bd7628c8e368d96466b6ab6d9c7a51f7b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2114; amd64

### `nats:2-windowsservercore-1809` - windows version 10.0.17763.2114; amd64

```console
$ docker pull nats@sha256:ea5bd03ca8c905a9bb8df9bcefe1c70aada9fce64c82d90932dfaf570332087a
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2691339003 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce14639524af68868fed35dda40295ffe16c35eb58b5038f43989d7d60f7059d`
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
# Fri, 10 Sep 2021 00:14:04 GMT
ENV NATS_SERVER=2.5.0
# Fri, 10 Sep 2021 00:14:05 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.5.0/nats-server-v2.5.0-windows-amd64.zip
# Fri, 10 Sep 2021 00:14:06 GMT
ENV NATS_SERVER_SHASUM=0eae96ad4555f5060b0b6325ba972566b404cd8930b3168b9c0ffe911d15c5d8
# Fri, 10 Sep 2021 00:15:08 GMT
RUN Set-PSDebug -Trace 2
# Fri, 10 Sep 2021 00:16:32 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 10 Sep 2021 00:16:33 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 10 Sep 2021 00:16:34 GMT
EXPOSE 4222 6222 8222
# Fri, 10 Sep 2021 00:16:34 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 10 Sep 2021 00:16:35 GMT
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
	-	`sha256:4c32056c4535002b64e42d1424edb3a7ac778c308d2d9109f33d738d59c85454`  
		Last Modified: Fri, 10 Sep 2021 00:20:02 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb115761571c4ba7b8b719d8ee1587c8898f7e13246d1a92ee2283c0f929a1b1`  
		Last Modified: Fri, 10 Sep 2021 00:20:01 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd93d02cef774a55aa7c6f566b3b5718436cbdae64582cc888ef3b1efe452735`  
		Last Modified: Fri, 10 Sep 2021 00:20:01 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f28336574033153776b7149c4d079b46a95608a291563bc581fc8b029d9399c`  
		Last Modified: Fri, 10 Sep 2021 00:20:02 GMT  
		Size: 372.4 KB (372418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcce3c7fbad71cacb4533bac881f55d312123c387549ca7840f402aa108fb59d`  
		Last Modified: Fri, 10 Sep 2021 00:20:05 GMT  
		Size: 5.0 MB (4955556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0d387c2eda58f8b5f8c3889645ec5e1a977b681cb17de77c04de1c643341b18`  
		Last Modified: Fri, 10 Sep 2021 00:19:59 GMT  
		Size: 1.9 KB (1944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f70bbbc8ecda378ae0099ea8e49350ba7d78be681cd5defc71e6f624abca5d7`  
		Last Modified: Fri, 10 Sep 2021 00:19:59 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76b0025f319f789e7c26483abcf5ca7944dc5a1f0a071023d2415526aa310d40`  
		Last Modified: Fri, 10 Sep 2021 00:19:59 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99ff7344cf8ed7957719594d8f9fe4d78b0ef7acc3755bb1962febcf166ac4ce`  
		Last Modified: Fri, 10 Sep 2021 00:19:59 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-windowsservercore-ltsc2016`

```console
$ docker pull nats@sha256:521575d35d4f87b16aa1482f712733b1273962ba4f75353d07327cfc4e324cee
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.14393.4583; amd64

### `nats:2-windowsservercore-ltsc2016` - windows version 10.0.14393.4583; amd64

```console
$ docker pull nats@sha256:7f318bb6bf586d9b74b6b8e8097ffabf3b4d16c43c5b9b2dd62d532713aa0305
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6276274196 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5716654340a54076fb48e8d797d45b91a2e56551a534fb6d800d7d6c61262257`
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
# Fri, 10 Sep 2021 00:16:55 GMT
ENV NATS_SERVER=2.5.0
# Fri, 10 Sep 2021 00:16:56 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.5.0/nats-server-v2.5.0-windows-amd64.zip
# Fri, 10 Sep 2021 00:16:57 GMT
ENV NATS_SERVER_SHASUM=0eae96ad4555f5060b0b6325ba972566b404cd8930b3168b9c0ffe911d15c5d8
# Fri, 10 Sep 2021 00:17:43 GMT
RUN Set-PSDebug -Trace 2
# Fri, 10 Sep 2021 00:19:14 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 10 Sep 2021 00:19:15 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 10 Sep 2021 00:19:16 GMT
EXPOSE 4222 6222 8222
# Fri, 10 Sep 2021 00:19:17 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 10 Sep 2021 00:19:18 GMT
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
	-	`sha256:786675b79153c67ad039b6b8a55171a8167b2ff8c8186ccb7c5cab0b01f47767`  
		Last Modified: Fri, 10 Sep 2021 00:20:42 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65445b8a1c334a2efce7d34289af9fa682427cba808180c96ce46f39f765e9b5`  
		Last Modified: Fri, 10 Sep 2021 00:20:42 GMT  
		Size: 1.4 KB (1358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08647f69046830b98e59118ace63049f027ad1786cc2aaad037990a4e7a87344`  
		Last Modified: Fri, 10 Sep 2021 00:20:42 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b50cf5c744e8952689c263dbc9800bbe4a032fb4c8df3c8e5028092bdb2a5c9c`  
		Last Modified: Fri, 10 Sep 2021 00:20:42 GMT  
		Size: 338.0 KB (337964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:459c701464a835b4d39cc3183fff454248a3045bb433c26b0430f06e91acf1bb`  
		Last Modified: Fri, 10 Sep 2021 00:20:41 GMT  
		Size: 5.0 MB (4957179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cb2fb143896bcefca1d8ad8640f3146b771f5b284f01be2b849a048d9ac9eeb`  
		Last Modified: Fri, 10 Sep 2021 00:20:40 GMT  
		Size: 1.9 KB (1938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d9f7d515a8e73d005392fc0bccc42761025b86ab370cffe210a552fe53d1cbe`  
		Last Modified: Fri, 10 Sep 2021 00:20:40 GMT  
		Size: 1.4 KB (1380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d68902a6dec2675ab57a60716c10ce8a85e58fe54d7abea307bc340452e882a`  
		Last Modified: Fri, 10 Sep 2021 00:20:39 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37e0389f87abc858cef1a365e6b548d7d7762be571608840bc715ef352c41084`  
		Last Modified: Fri, 10 Sep 2021 00:20:39 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.5`

```console
$ docker pull nats@sha256:c812e8c75705b49bfc4694743b59428590372ff6689425c86ea3ddd682fd8c58
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.2114; amd64

### `nats:2.5` - linux; amd64

```console
$ docker pull nats@sha256:01dbe57fde6a40eecbd53edc6a418f3c9b1ddd85f03dd17e73ecef98a3b15318
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4546051 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80fcdf2bfe0f4a11267c9e8d06e5e52dce7dd9b41267e1a51d5e9df22c76bf9c`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 10 Sep 2021 00:20:41 GMT
COPY file:0b180121e1ef70970b020901a4b61990a8673ac9db99b94c348c5321333884ea in /nats-server 
# Fri, 10 Sep 2021 00:20:41 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 10 Sep 2021 00:20:41 GMT
EXPOSE 4222 6222 8222
# Fri, 10 Sep 2021 00:20:41 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 10 Sep 2021 00:20:42 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:9cee557b7d3312d12996f8c4338bf9ea02657256657ef77d46510c729d9be195`  
		Last Modified: Fri, 10 Sep 2021 00:21:32 GMT  
		Size: 4.5 MB (4545577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb24b942a0d168497adac7ad3190098a6f8dfa34ad2ef37932150fbce9336c9a`  
		Last Modified: Fri, 10 Sep 2021 00:21:31 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.5` - linux; arm variant v6

```console
$ docker pull nats@sha256:b21057f1f945b501d03cf3c5c2d530f7961e1a3198e00bb297b7f69a849cc0e9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4210290 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:865dcd8a77138e8339293c7089adeee440305e68331df5533186ea36b8132f84`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 09 Sep 2021 23:50:15 GMT
COPY file:a60049eef2da0cbda1255e229e5e5c6377e3c3445b0cd16ce13a272139c7ce85 in /nats-server 
# Thu, 09 Sep 2021 23:50:16 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 09 Sep 2021 23:50:17 GMT
EXPOSE 4222 6222 8222
# Thu, 09 Sep 2021 23:50:17 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 09 Sep 2021 23:50:18 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b95232e9c9c31dfba5a6124fb74b4abc750a3fd6d5f89a13438a0b051430299e`  
		Last Modified: Thu, 09 Sep 2021 23:52:42 GMT  
		Size: 4.2 MB (4209813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2c01128246ad2a36efed9386a5ed63a01f73f3f56e54d059834ac17a2f64a48`  
		Last Modified: Thu, 09 Sep 2021 23:52:38 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.5` - linux; arm variant v7

```console
$ docker pull nats@sha256:aafbb0b5e1b7412f9d0e71ddd6c3948c7080697882dd40ae20578b855ca40c1f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4206272 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:79f5a4fb5f9254997b2d7e573f24316740a167eb829bb23952ba05ff8304ddc1`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 10 Sep 2021 00:59:05 GMT
COPY file:7043dd814cd92048127f9905d58e9204d2968d9c03bbb7feba592c45a87e9963 in /nats-server 
# Fri, 10 Sep 2021 00:59:06 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 10 Sep 2021 00:59:06 GMT
EXPOSE 4222 6222 8222
# Fri, 10 Sep 2021 00:59:07 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 10 Sep 2021 00:59:07 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:8ae70a7ddee0b3bc3819ff86ee31d3295a37b10282b7ee0d14d3dd3c8dcb16c7`  
		Last Modified: Fri, 10 Sep 2021 01:01:28 GMT  
		Size: 4.2 MB (4205795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbbfbfa45875dc8bff20ba3a989407cf3ab8018f98f4277411dd068510c071c6`  
		Last Modified: Fri, 10 Sep 2021 01:01:25 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.5` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:24f192937e7bc371f7c2631055e49a51d489659d28f55b4fdf2eb5a19843a5ae
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4158958 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2cd8bb7e96599c9badd4424f86ef2d5f8561cfa0c4a4322057847c002da643a9`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 09 Sep 2021 23:40:25 GMT
COPY file:eda8ae8779fbfb7d34c95bc93fc8ce409cbd298cb302284f61ee4ebf6ac10b0e in /nats-server 
# Thu, 09 Sep 2021 23:40:26 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 09 Sep 2021 23:40:26 GMT
EXPOSE 4222 6222 8222
# Thu, 09 Sep 2021 23:40:26 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 09 Sep 2021 23:40:26 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:0c0083faeb4bd1e89eefb7cbc2a5556eb056acaba6107a833c271a1ca7cd8633`  
		Last Modified: Thu, 09 Sep 2021 23:41:48 GMT  
		Size: 4.2 MB (4158481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4227e148c1053ae9735f2dcc2ab35b83566aab7b85aa3d50395ec15be4630e26`  
		Last Modified: Thu, 09 Sep 2021 23:41:47 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.5` - windows version 10.0.17763.2114; amd64

```console
$ docker pull nats@sha256:da56a6dd1f9556f706d9086ed48947ac745a5b9dd1e3bc0d988581858828c23c
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.4 MB (107351558 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:780da6fbe38cee622e2d2e69123219af601b417dada779a198cef0514370203e`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 05 Aug 2021 19:15:20 GMT
RUN Apply image 1809-amd64
# Wed, 25 Aug 2021 16:07:56 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 10 Sep 2021 00:16:45 GMT
RUN cmd /S /C #(nop) COPY file:13fac1899b72f2f26df9bd8ce320e46a5f7736306d7abf82ea7d657c16444fb9 in C:\nats-server.exe 
# Fri, 10 Sep 2021 00:16:46 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 10 Sep 2021 00:16:47 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Fri, 10 Sep 2021 00:16:47 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 10 Sep 2021 00:16:48 GMT
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
	-	`sha256:55bd340c78387be49377457ea8e39875e7be9b3799bdac42ff35c749d67b3940`  
		Last Modified: Fri, 10 Sep 2021 00:20:25 GMT  
		Size: 4.6 MB (4604102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76e6782c003b15abdb2161dc360ffef0eeb967b34fc78186d8d6085aacfc85fa`  
		Last Modified: Fri, 10 Sep 2021 00:20:20 GMT  
		Size: 1.8 KB (1777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf24d35e2c525beccaa7b227eda13492b401302f8ecc528e2a35118220e3f760`  
		Last Modified: Fri, 10 Sep 2021 00:20:20 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71603cdad9bbdd669dd86cda1c010a6f91d1a58de21eac052a29279f77bd247f`  
		Last Modified: Fri, 10 Sep 2021 00:20:20 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01477f3ed16729139c6a0a856de33336e03c4fb127df26c6e42b8157eaf1801b`  
		Last Modified: Fri, 10 Sep 2021 00:20:20 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.5-alpine`

```console
$ docker pull nats@sha256:52a8fe18f5c85cdd5cf0304eadb4e4a6a4208db9183fabc36140ff9ed7a813a3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.5-alpine` - linux; amd64

```console
$ docker pull nats@sha256:f6b2376c122defe213696fdbf87c7f365bdbbd60a6068fe88b1ab8aee27987d2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7647076 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b59fdb5895884cf160a5cabba5411b4a328b11aa2798042d794fe41e69fe8165`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 10 Sep 2021 00:20:12 GMT
ENV NATS_SERVER=2.5.0
# Fri, 10 Sep 2021 00:20:15 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='93f64cd14f04b4e7f6c3a2c10d09888be653406b7bc1a41f399ae44746388a5c' ;; 		armhf) natsArch='arm6'; sha256='12f38f6881cdcf27c0faebb7ab6580b40253c36dc1531d499a29c4998a009494' ;; 		armv7) natsArch='arm7'; sha256='fb3611b57a932f5c75310dee66597057ab65b442eb84d73b2c5fd9389eb6e518' ;; 		x86_64) natsArch='amd64'; sha256='4d2f4abb15b45618ce772659c9f3eca60f25266dfc976f0354430ad67c8fd886' ;; 		x86) natsArch='386'; sha256='776aecc77c33146d88e6b3cb1787097f9817122182f49f7243c0ea3fd62ad029' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 10 Sep 2021 00:20:15 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 10 Sep 2021 00:20:15 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 10 Sep 2021 00:20:15 GMT
EXPOSE 4222 6222 8222
# Fri, 10 Sep 2021 00:20:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 10 Sep 2021 00:20:16 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59a9809baa02715a6c4ccdb1ebc94edaf948058be9f97cea623426ca670b426e`  
		Last Modified: Fri, 10 Sep 2021 00:21:08 GMT  
		Size: 4.8 MB (4831663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68c0794b9b379d130866e40babeef9f4557514bcc2c88194e89b90081ef7ad12`  
		Last Modified: Fri, 10 Sep 2021 00:21:08 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:240551b5739b209d882cd7b4f76138b9188aac1a497ff32a469526302056dd98`  
		Last Modified: Fri, 10 Sep 2021 00:21:07 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.5-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:c516621cb4dc61ad9db1927cdcec7210328be6d7b813acb688016584d61be212
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7121422 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c48580010dc9af32e7a019914f078134ae513ef77280b7877fe7fd47665426b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:49:29 GMT
ADD file:1c1c4520d49cb6e8f795f3b953d1ed3c3c77868b98b53a455169c254fcec5acd in / 
# Fri, 27 Aug 2021 17:49:30 GMT
CMD ["/bin/sh"]
# Thu, 09 Sep 2021 23:49:46 GMT
ENV NATS_SERVER=2.5.0
# Thu, 09 Sep 2021 23:49:51 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='93f64cd14f04b4e7f6c3a2c10d09888be653406b7bc1a41f399ae44746388a5c' ;; 		armhf) natsArch='arm6'; sha256='12f38f6881cdcf27c0faebb7ab6580b40253c36dc1531d499a29c4998a009494' ;; 		armv7) natsArch='arm7'; sha256='fb3611b57a932f5c75310dee66597057ab65b442eb84d73b2c5fd9389eb6e518' ;; 		x86_64) natsArch='amd64'; sha256='4d2f4abb15b45618ce772659c9f3eca60f25266dfc976f0354430ad67c8fd886' ;; 		x86) natsArch='386'; sha256='776aecc77c33146d88e6b3cb1787097f9817122182f49f7243c0ea3fd62ad029' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 09 Sep 2021 23:49:51 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 09 Sep 2021 23:49:52 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 09 Sep 2021 23:49:52 GMT
EXPOSE 4222 6222 8222
# Thu, 09 Sep 2021 23:49:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 09 Sep 2021 23:49:53 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:2e78c0f86ba9a1fed30df20cb48c9cc73e9626399f12749d36b892ff99c0ecf5`  
		Last Modified: Fri, 27 Aug 2021 17:50:55 GMT  
		Size: 2.6 MB (2627447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75b214a44f07577985e2f01798e9acf02be903c28022f74d244b22418b31e815`  
		Last Modified: Thu, 09 Sep 2021 23:52:03 GMT  
		Size: 4.5 MB (4493006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d232ac6d6c1f822be800be02acbb341f7abe35b05bd13a0857df02fd1cc600a6`  
		Last Modified: Thu, 09 Sep 2021 23:52:01 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e364400828db299d750b3bcc80b1e3b1df2f7abe62c5d6293f3c7e22d93e20a`  
		Last Modified: Thu, 09 Sep 2021 23:52:00 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.5-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:c5a16f99958e4ae6f318a577619242a7d168fc47e07883d8adbc1701faa36ab4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.9 MB (6918058 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b6128ceec7a63c74e316f6b3bda400e98def18ed14e046a0177a1095946dd8e2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:57:31 GMT
ADD file:a7da7992ccea54d3295231027614f138aa45c4d4a25ea6ec9bf7b316b9f67d95 in / 
# Fri, 27 Aug 2021 17:57:32 GMT
CMD ["/bin/sh"]
# Fri, 10 Sep 2021 00:58:26 GMT
ENV NATS_SERVER=2.5.0
# Fri, 10 Sep 2021 00:58:31 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='93f64cd14f04b4e7f6c3a2c10d09888be653406b7bc1a41f399ae44746388a5c' ;; 		armhf) natsArch='arm6'; sha256='12f38f6881cdcf27c0faebb7ab6580b40253c36dc1531d499a29c4998a009494' ;; 		armv7) natsArch='arm7'; sha256='fb3611b57a932f5c75310dee66597057ab65b442eb84d73b2c5fd9389eb6e518' ;; 		x86_64) natsArch='amd64'; sha256='4d2f4abb15b45618ce772659c9f3eca60f25266dfc976f0354430ad67c8fd886' ;; 		x86) natsArch='386'; sha256='776aecc77c33146d88e6b3cb1787097f9817122182f49f7243c0ea3fd62ad029' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 10 Sep 2021 00:58:32 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 10 Sep 2021 00:58:32 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 10 Sep 2021 00:58:33 GMT
EXPOSE 4222 6222 8222
# Fri, 10 Sep 2021 00:58:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 10 Sep 2021 00:58:34 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:a14774a5a62e0f454febaec7cb603e18a6a8e25ef9da4a4da85b155bdd5e5a7a`  
		Last Modified: Fri, 27 Aug 2021 17:59:00 GMT  
		Size: 2.4 MB (2430419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2edd63df5776202ac2717836b8350736f3e046021c53b49e6e872ef9f4a960a9`  
		Last Modified: Fri, 10 Sep 2021 01:00:49 GMT  
		Size: 4.5 MB (4486667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d073c5b9595fcde55c46ccb0f54148caba30c630427ffcdfe9f03a4e84be10ec`  
		Last Modified: Fri, 10 Sep 2021 01:00:46 GMT  
		Size: 559.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15f66a2a44784b8ce7529a34b470376f9a52740980b2b05baf8525ec5f4a39f2`  
		Last Modified: Fri, 10 Sep 2021 01:00:46 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.5-alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:88b4d8f2f54f207d5400e8d3e9037d55ca8d2969b126e07d833c6d3464f93300
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7156798 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f803b2b0ed9b56df4cac8c3a03dfd789e480a622c1f3a282ecee5fd0f937d9e5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Thu, 09 Sep 2021 23:40:02 GMT
ENV NATS_SERVER=2.5.0
# Thu, 09 Sep 2021 23:40:05 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='93f64cd14f04b4e7f6c3a2c10d09888be653406b7bc1a41f399ae44746388a5c' ;; 		armhf) natsArch='arm6'; sha256='12f38f6881cdcf27c0faebb7ab6580b40253c36dc1531d499a29c4998a009494' ;; 		armv7) natsArch='arm7'; sha256='fb3611b57a932f5c75310dee66597057ab65b442eb84d73b2c5fd9389eb6e518' ;; 		x86_64) natsArch='amd64'; sha256='4d2f4abb15b45618ce772659c9f3eca60f25266dfc976f0354430ad67c8fd886' ;; 		x86) natsArch='386'; sha256='776aecc77c33146d88e6b3cb1787097f9817122182f49f7243c0ea3fd62ad029' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 09 Sep 2021 23:40:05 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 09 Sep 2021 23:40:05 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 09 Sep 2021 23:40:05 GMT
EXPOSE 4222 6222 8222
# Thu, 09 Sep 2021 23:40:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 09 Sep 2021 23:40:06 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:552d1f2373af9bfe12033568ebbfb0ccbb0de11279f9a415a29207e264d7f4d9`  
		Last Modified: Fri, 27 Aug 2021 17:40:18 GMT  
		Size: 2.7 MB (2711827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49450e2f2462d1e207a865d4a084154f6a3c5edc2b3b4954d34d4e1ce75d38f2`  
		Last Modified: Thu, 09 Sep 2021 23:41:18 GMT  
		Size: 4.4 MB (4444005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edeb0b05b16add9a16e4a8bc8c1eced6c1f60f58ac669216dbbf93cb9bce40d2`  
		Last Modified: Thu, 09 Sep 2021 23:41:18 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67be552e94a6cfc686543e5bfa0c1a6bca72bc9dce939fb9f3e43c4a77f5e6e3`  
		Last Modified: Thu, 09 Sep 2021 23:41:18 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.5-alpine3.14`

```console
$ docker pull nats@sha256:52a8fe18f5c85cdd5cf0304eadb4e4a6a4208db9183fabc36140ff9ed7a813a3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.5-alpine3.14` - linux; amd64

```console
$ docker pull nats@sha256:f6b2376c122defe213696fdbf87c7f365bdbbd60a6068fe88b1ab8aee27987d2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7647076 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b59fdb5895884cf160a5cabba5411b4a328b11aa2798042d794fe41e69fe8165`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 10 Sep 2021 00:20:12 GMT
ENV NATS_SERVER=2.5.0
# Fri, 10 Sep 2021 00:20:15 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='93f64cd14f04b4e7f6c3a2c10d09888be653406b7bc1a41f399ae44746388a5c' ;; 		armhf) natsArch='arm6'; sha256='12f38f6881cdcf27c0faebb7ab6580b40253c36dc1531d499a29c4998a009494' ;; 		armv7) natsArch='arm7'; sha256='fb3611b57a932f5c75310dee66597057ab65b442eb84d73b2c5fd9389eb6e518' ;; 		x86_64) natsArch='amd64'; sha256='4d2f4abb15b45618ce772659c9f3eca60f25266dfc976f0354430ad67c8fd886' ;; 		x86) natsArch='386'; sha256='776aecc77c33146d88e6b3cb1787097f9817122182f49f7243c0ea3fd62ad029' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 10 Sep 2021 00:20:15 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 10 Sep 2021 00:20:15 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 10 Sep 2021 00:20:15 GMT
EXPOSE 4222 6222 8222
# Fri, 10 Sep 2021 00:20:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 10 Sep 2021 00:20:16 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59a9809baa02715a6c4ccdb1ebc94edaf948058be9f97cea623426ca670b426e`  
		Last Modified: Fri, 10 Sep 2021 00:21:08 GMT  
		Size: 4.8 MB (4831663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68c0794b9b379d130866e40babeef9f4557514bcc2c88194e89b90081ef7ad12`  
		Last Modified: Fri, 10 Sep 2021 00:21:08 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:240551b5739b209d882cd7b4f76138b9188aac1a497ff32a469526302056dd98`  
		Last Modified: Fri, 10 Sep 2021 00:21:07 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.5-alpine3.14` - linux; arm variant v6

```console
$ docker pull nats@sha256:c516621cb4dc61ad9db1927cdcec7210328be6d7b813acb688016584d61be212
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7121422 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c48580010dc9af32e7a019914f078134ae513ef77280b7877fe7fd47665426b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:49:29 GMT
ADD file:1c1c4520d49cb6e8f795f3b953d1ed3c3c77868b98b53a455169c254fcec5acd in / 
# Fri, 27 Aug 2021 17:49:30 GMT
CMD ["/bin/sh"]
# Thu, 09 Sep 2021 23:49:46 GMT
ENV NATS_SERVER=2.5.0
# Thu, 09 Sep 2021 23:49:51 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='93f64cd14f04b4e7f6c3a2c10d09888be653406b7bc1a41f399ae44746388a5c' ;; 		armhf) natsArch='arm6'; sha256='12f38f6881cdcf27c0faebb7ab6580b40253c36dc1531d499a29c4998a009494' ;; 		armv7) natsArch='arm7'; sha256='fb3611b57a932f5c75310dee66597057ab65b442eb84d73b2c5fd9389eb6e518' ;; 		x86_64) natsArch='amd64'; sha256='4d2f4abb15b45618ce772659c9f3eca60f25266dfc976f0354430ad67c8fd886' ;; 		x86) natsArch='386'; sha256='776aecc77c33146d88e6b3cb1787097f9817122182f49f7243c0ea3fd62ad029' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 09 Sep 2021 23:49:51 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 09 Sep 2021 23:49:52 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 09 Sep 2021 23:49:52 GMT
EXPOSE 4222 6222 8222
# Thu, 09 Sep 2021 23:49:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 09 Sep 2021 23:49:53 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:2e78c0f86ba9a1fed30df20cb48c9cc73e9626399f12749d36b892ff99c0ecf5`  
		Last Modified: Fri, 27 Aug 2021 17:50:55 GMT  
		Size: 2.6 MB (2627447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75b214a44f07577985e2f01798e9acf02be903c28022f74d244b22418b31e815`  
		Last Modified: Thu, 09 Sep 2021 23:52:03 GMT  
		Size: 4.5 MB (4493006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d232ac6d6c1f822be800be02acbb341f7abe35b05bd13a0857df02fd1cc600a6`  
		Last Modified: Thu, 09 Sep 2021 23:52:01 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e364400828db299d750b3bcc80b1e3b1df2f7abe62c5d6293f3c7e22d93e20a`  
		Last Modified: Thu, 09 Sep 2021 23:52:00 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.5-alpine3.14` - linux; arm variant v7

```console
$ docker pull nats@sha256:c5a16f99958e4ae6f318a577619242a7d168fc47e07883d8adbc1701faa36ab4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.9 MB (6918058 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b6128ceec7a63c74e316f6b3bda400e98def18ed14e046a0177a1095946dd8e2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:57:31 GMT
ADD file:a7da7992ccea54d3295231027614f138aa45c4d4a25ea6ec9bf7b316b9f67d95 in / 
# Fri, 27 Aug 2021 17:57:32 GMT
CMD ["/bin/sh"]
# Fri, 10 Sep 2021 00:58:26 GMT
ENV NATS_SERVER=2.5.0
# Fri, 10 Sep 2021 00:58:31 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='93f64cd14f04b4e7f6c3a2c10d09888be653406b7bc1a41f399ae44746388a5c' ;; 		armhf) natsArch='arm6'; sha256='12f38f6881cdcf27c0faebb7ab6580b40253c36dc1531d499a29c4998a009494' ;; 		armv7) natsArch='arm7'; sha256='fb3611b57a932f5c75310dee66597057ab65b442eb84d73b2c5fd9389eb6e518' ;; 		x86_64) natsArch='amd64'; sha256='4d2f4abb15b45618ce772659c9f3eca60f25266dfc976f0354430ad67c8fd886' ;; 		x86) natsArch='386'; sha256='776aecc77c33146d88e6b3cb1787097f9817122182f49f7243c0ea3fd62ad029' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 10 Sep 2021 00:58:32 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 10 Sep 2021 00:58:32 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 10 Sep 2021 00:58:33 GMT
EXPOSE 4222 6222 8222
# Fri, 10 Sep 2021 00:58:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 10 Sep 2021 00:58:34 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:a14774a5a62e0f454febaec7cb603e18a6a8e25ef9da4a4da85b155bdd5e5a7a`  
		Last Modified: Fri, 27 Aug 2021 17:59:00 GMT  
		Size: 2.4 MB (2430419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2edd63df5776202ac2717836b8350736f3e046021c53b49e6e872ef9f4a960a9`  
		Last Modified: Fri, 10 Sep 2021 01:00:49 GMT  
		Size: 4.5 MB (4486667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d073c5b9595fcde55c46ccb0f54148caba30c630427ffcdfe9f03a4e84be10ec`  
		Last Modified: Fri, 10 Sep 2021 01:00:46 GMT  
		Size: 559.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15f66a2a44784b8ce7529a34b470376f9a52740980b2b05baf8525ec5f4a39f2`  
		Last Modified: Fri, 10 Sep 2021 01:00:46 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.5-alpine3.14` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:88b4d8f2f54f207d5400e8d3e9037d55ca8d2969b126e07d833c6d3464f93300
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7156798 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f803b2b0ed9b56df4cac8c3a03dfd789e480a622c1f3a282ecee5fd0f937d9e5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Thu, 09 Sep 2021 23:40:02 GMT
ENV NATS_SERVER=2.5.0
# Thu, 09 Sep 2021 23:40:05 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='93f64cd14f04b4e7f6c3a2c10d09888be653406b7bc1a41f399ae44746388a5c' ;; 		armhf) natsArch='arm6'; sha256='12f38f6881cdcf27c0faebb7ab6580b40253c36dc1531d499a29c4998a009494' ;; 		armv7) natsArch='arm7'; sha256='fb3611b57a932f5c75310dee66597057ab65b442eb84d73b2c5fd9389eb6e518' ;; 		x86_64) natsArch='amd64'; sha256='4d2f4abb15b45618ce772659c9f3eca60f25266dfc976f0354430ad67c8fd886' ;; 		x86) natsArch='386'; sha256='776aecc77c33146d88e6b3cb1787097f9817122182f49f7243c0ea3fd62ad029' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 09 Sep 2021 23:40:05 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 09 Sep 2021 23:40:05 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 09 Sep 2021 23:40:05 GMT
EXPOSE 4222 6222 8222
# Thu, 09 Sep 2021 23:40:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 09 Sep 2021 23:40:06 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:552d1f2373af9bfe12033568ebbfb0ccbb0de11279f9a415a29207e264d7f4d9`  
		Last Modified: Fri, 27 Aug 2021 17:40:18 GMT  
		Size: 2.7 MB (2711827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49450e2f2462d1e207a865d4a084154f6a3c5edc2b3b4954d34d4e1ce75d38f2`  
		Last Modified: Thu, 09 Sep 2021 23:41:18 GMT  
		Size: 4.4 MB (4444005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edeb0b05b16add9a16e4a8bc8c1eced6c1f60f58ac669216dbbf93cb9bce40d2`  
		Last Modified: Thu, 09 Sep 2021 23:41:18 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67be552e94a6cfc686543e5bfa0c1a6bca72bc9dce939fb9f3e43c4a77f5e6e3`  
		Last Modified: Thu, 09 Sep 2021 23:41:18 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.5-linux`

```console
$ docker pull nats@sha256:6808dfb3132c301916bbeb4241ae1f3c0be5dca763a6c0be6180ca1bd6da298a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.5-linux` - linux; amd64

```console
$ docker pull nats@sha256:01dbe57fde6a40eecbd53edc6a418f3c9b1ddd85f03dd17e73ecef98a3b15318
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4546051 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80fcdf2bfe0f4a11267c9e8d06e5e52dce7dd9b41267e1a51d5e9df22c76bf9c`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 10 Sep 2021 00:20:41 GMT
COPY file:0b180121e1ef70970b020901a4b61990a8673ac9db99b94c348c5321333884ea in /nats-server 
# Fri, 10 Sep 2021 00:20:41 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 10 Sep 2021 00:20:41 GMT
EXPOSE 4222 6222 8222
# Fri, 10 Sep 2021 00:20:41 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 10 Sep 2021 00:20:42 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:9cee557b7d3312d12996f8c4338bf9ea02657256657ef77d46510c729d9be195`  
		Last Modified: Fri, 10 Sep 2021 00:21:32 GMT  
		Size: 4.5 MB (4545577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb24b942a0d168497adac7ad3190098a6f8dfa34ad2ef37932150fbce9336c9a`  
		Last Modified: Fri, 10 Sep 2021 00:21:31 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.5-linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:b21057f1f945b501d03cf3c5c2d530f7961e1a3198e00bb297b7f69a849cc0e9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4210290 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:865dcd8a77138e8339293c7089adeee440305e68331df5533186ea36b8132f84`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 09 Sep 2021 23:50:15 GMT
COPY file:a60049eef2da0cbda1255e229e5e5c6377e3c3445b0cd16ce13a272139c7ce85 in /nats-server 
# Thu, 09 Sep 2021 23:50:16 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 09 Sep 2021 23:50:17 GMT
EXPOSE 4222 6222 8222
# Thu, 09 Sep 2021 23:50:17 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 09 Sep 2021 23:50:18 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b95232e9c9c31dfba5a6124fb74b4abc750a3fd6d5f89a13438a0b051430299e`  
		Last Modified: Thu, 09 Sep 2021 23:52:42 GMT  
		Size: 4.2 MB (4209813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2c01128246ad2a36efed9386a5ed63a01f73f3f56e54d059834ac17a2f64a48`  
		Last Modified: Thu, 09 Sep 2021 23:52:38 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.5-linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:aafbb0b5e1b7412f9d0e71ddd6c3948c7080697882dd40ae20578b855ca40c1f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4206272 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:79f5a4fb5f9254997b2d7e573f24316740a167eb829bb23952ba05ff8304ddc1`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 10 Sep 2021 00:59:05 GMT
COPY file:7043dd814cd92048127f9905d58e9204d2968d9c03bbb7feba592c45a87e9963 in /nats-server 
# Fri, 10 Sep 2021 00:59:06 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 10 Sep 2021 00:59:06 GMT
EXPOSE 4222 6222 8222
# Fri, 10 Sep 2021 00:59:07 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 10 Sep 2021 00:59:07 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:8ae70a7ddee0b3bc3819ff86ee31d3295a37b10282b7ee0d14d3dd3c8dcb16c7`  
		Last Modified: Fri, 10 Sep 2021 01:01:28 GMT  
		Size: 4.2 MB (4205795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbbfbfa45875dc8bff20ba3a989407cf3ab8018f98f4277411dd068510c071c6`  
		Last Modified: Fri, 10 Sep 2021 01:01:25 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.5-linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:24f192937e7bc371f7c2631055e49a51d489659d28f55b4fdf2eb5a19843a5ae
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4158958 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2cd8bb7e96599c9badd4424f86ef2d5f8561cfa0c4a4322057847c002da643a9`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 09 Sep 2021 23:40:25 GMT
COPY file:eda8ae8779fbfb7d34c95bc93fc8ce409cbd298cb302284f61ee4ebf6ac10b0e in /nats-server 
# Thu, 09 Sep 2021 23:40:26 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 09 Sep 2021 23:40:26 GMT
EXPOSE 4222 6222 8222
# Thu, 09 Sep 2021 23:40:26 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 09 Sep 2021 23:40:26 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:0c0083faeb4bd1e89eefb7cbc2a5556eb056acaba6107a833c271a1ca7cd8633`  
		Last Modified: Thu, 09 Sep 2021 23:41:48 GMT  
		Size: 4.2 MB (4158481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4227e148c1053ae9735f2dcc2ab35b83566aab7b85aa3d50395ec15be4630e26`  
		Last Modified: Thu, 09 Sep 2021 23:41:47 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.5-nanoserver`

```console
$ docker pull nats@sha256:5b8ea050ee708eb4017db4e1cb913456e468e82c227eb67a070974651446cfd9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2114; amd64

### `nats:2.5-nanoserver` - windows version 10.0.17763.2114; amd64

```console
$ docker pull nats@sha256:da56a6dd1f9556f706d9086ed48947ac745a5b9dd1e3bc0d988581858828c23c
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.4 MB (107351558 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:780da6fbe38cee622e2d2e69123219af601b417dada779a198cef0514370203e`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 05 Aug 2021 19:15:20 GMT
RUN Apply image 1809-amd64
# Wed, 25 Aug 2021 16:07:56 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 10 Sep 2021 00:16:45 GMT
RUN cmd /S /C #(nop) COPY file:13fac1899b72f2f26df9bd8ce320e46a5f7736306d7abf82ea7d657c16444fb9 in C:\nats-server.exe 
# Fri, 10 Sep 2021 00:16:46 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 10 Sep 2021 00:16:47 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Fri, 10 Sep 2021 00:16:47 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 10 Sep 2021 00:16:48 GMT
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
	-	`sha256:55bd340c78387be49377457ea8e39875e7be9b3799bdac42ff35c749d67b3940`  
		Last Modified: Fri, 10 Sep 2021 00:20:25 GMT  
		Size: 4.6 MB (4604102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76e6782c003b15abdb2161dc360ffef0eeb967b34fc78186d8d6085aacfc85fa`  
		Last Modified: Fri, 10 Sep 2021 00:20:20 GMT  
		Size: 1.8 KB (1777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf24d35e2c525beccaa7b227eda13492b401302f8ecc528e2a35118220e3f760`  
		Last Modified: Fri, 10 Sep 2021 00:20:20 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71603cdad9bbdd669dd86cda1c010a6f91d1a58de21eac052a29279f77bd247f`  
		Last Modified: Fri, 10 Sep 2021 00:20:20 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01477f3ed16729139c6a0a856de33336e03c4fb127df26c6e42b8157eaf1801b`  
		Last Modified: Fri, 10 Sep 2021 00:20:20 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.5-nanoserver-1809`

```console
$ docker pull nats@sha256:5b8ea050ee708eb4017db4e1cb913456e468e82c227eb67a070974651446cfd9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2114; amd64

### `nats:2.5-nanoserver-1809` - windows version 10.0.17763.2114; amd64

```console
$ docker pull nats@sha256:da56a6dd1f9556f706d9086ed48947ac745a5b9dd1e3bc0d988581858828c23c
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.4 MB (107351558 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:780da6fbe38cee622e2d2e69123219af601b417dada779a198cef0514370203e`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 05 Aug 2021 19:15:20 GMT
RUN Apply image 1809-amd64
# Wed, 25 Aug 2021 16:07:56 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 10 Sep 2021 00:16:45 GMT
RUN cmd /S /C #(nop) COPY file:13fac1899b72f2f26df9bd8ce320e46a5f7736306d7abf82ea7d657c16444fb9 in C:\nats-server.exe 
# Fri, 10 Sep 2021 00:16:46 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 10 Sep 2021 00:16:47 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Fri, 10 Sep 2021 00:16:47 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 10 Sep 2021 00:16:48 GMT
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
	-	`sha256:55bd340c78387be49377457ea8e39875e7be9b3799bdac42ff35c749d67b3940`  
		Last Modified: Fri, 10 Sep 2021 00:20:25 GMT  
		Size: 4.6 MB (4604102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76e6782c003b15abdb2161dc360ffef0eeb967b34fc78186d8d6085aacfc85fa`  
		Last Modified: Fri, 10 Sep 2021 00:20:20 GMT  
		Size: 1.8 KB (1777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf24d35e2c525beccaa7b227eda13492b401302f8ecc528e2a35118220e3f760`  
		Last Modified: Fri, 10 Sep 2021 00:20:20 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71603cdad9bbdd669dd86cda1c010a6f91d1a58de21eac052a29279f77bd247f`  
		Last Modified: Fri, 10 Sep 2021 00:20:20 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01477f3ed16729139c6a0a856de33336e03c4fb127df26c6e42b8157eaf1801b`  
		Last Modified: Fri, 10 Sep 2021 00:20:20 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.5-scratch`

```console
$ docker pull nats@sha256:6808dfb3132c301916bbeb4241ae1f3c0be5dca763a6c0be6180ca1bd6da298a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.5-scratch` - linux; amd64

```console
$ docker pull nats@sha256:01dbe57fde6a40eecbd53edc6a418f3c9b1ddd85f03dd17e73ecef98a3b15318
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4546051 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80fcdf2bfe0f4a11267c9e8d06e5e52dce7dd9b41267e1a51d5e9df22c76bf9c`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 10 Sep 2021 00:20:41 GMT
COPY file:0b180121e1ef70970b020901a4b61990a8673ac9db99b94c348c5321333884ea in /nats-server 
# Fri, 10 Sep 2021 00:20:41 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 10 Sep 2021 00:20:41 GMT
EXPOSE 4222 6222 8222
# Fri, 10 Sep 2021 00:20:41 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 10 Sep 2021 00:20:42 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:9cee557b7d3312d12996f8c4338bf9ea02657256657ef77d46510c729d9be195`  
		Last Modified: Fri, 10 Sep 2021 00:21:32 GMT  
		Size: 4.5 MB (4545577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb24b942a0d168497adac7ad3190098a6f8dfa34ad2ef37932150fbce9336c9a`  
		Last Modified: Fri, 10 Sep 2021 00:21:31 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.5-scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:b21057f1f945b501d03cf3c5c2d530f7961e1a3198e00bb297b7f69a849cc0e9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4210290 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:865dcd8a77138e8339293c7089adeee440305e68331df5533186ea36b8132f84`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 09 Sep 2021 23:50:15 GMT
COPY file:a60049eef2da0cbda1255e229e5e5c6377e3c3445b0cd16ce13a272139c7ce85 in /nats-server 
# Thu, 09 Sep 2021 23:50:16 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 09 Sep 2021 23:50:17 GMT
EXPOSE 4222 6222 8222
# Thu, 09 Sep 2021 23:50:17 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 09 Sep 2021 23:50:18 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b95232e9c9c31dfba5a6124fb74b4abc750a3fd6d5f89a13438a0b051430299e`  
		Last Modified: Thu, 09 Sep 2021 23:52:42 GMT  
		Size: 4.2 MB (4209813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2c01128246ad2a36efed9386a5ed63a01f73f3f56e54d059834ac17a2f64a48`  
		Last Modified: Thu, 09 Sep 2021 23:52:38 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.5-scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:aafbb0b5e1b7412f9d0e71ddd6c3948c7080697882dd40ae20578b855ca40c1f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4206272 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:79f5a4fb5f9254997b2d7e573f24316740a167eb829bb23952ba05ff8304ddc1`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 10 Sep 2021 00:59:05 GMT
COPY file:7043dd814cd92048127f9905d58e9204d2968d9c03bbb7feba592c45a87e9963 in /nats-server 
# Fri, 10 Sep 2021 00:59:06 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 10 Sep 2021 00:59:06 GMT
EXPOSE 4222 6222 8222
# Fri, 10 Sep 2021 00:59:07 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 10 Sep 2021 00:59:07 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:8ae70a7ddee0b3bc3819ff86ee31d3295a37b10282b7ee0d14d3dd3c8dcb16c7`  
		Last Modified: Fri, 10 Sep 2021 01:01:28 GMT  
		Size: 4.2 MB (4205795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbbfbfa45875dc8bff20ba3a989407cf3ab8018f98f4277411dd068510c071c6`  
		Last Modified: Fri, 10 Sep 2021 01:01:25 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.5-scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:24f192937e7bc371f7c2631055e49a51d489659d28f55b4fdf2eb5a19843a5ae
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4158958 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2cd8bb7e96599c9badd4424f86ef2d5f8561cfa0c4a4322057847c002da643a9`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 09 Sep 2021 23:40:25 GMT
COPY file:eda8ae8779fbfb7d34c95bc93fc8ce409cbd298cb302284f61ee4ebf6ac10b0e in /nats-server 
# Thu, 09 Sep 2021 23:40:26 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 09 Sep 2021 23:40:26 GMT
EXPOSE 4222 6222 8222
# Thu, 09 Sep 2021 23:40:26 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 09 Sep 2021 23:40:26 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:0c0083faeb4bd1e89eefb7cbc2a5556eb056acaba6107a833c271a1ca7cd8633`  
		Last Modified: Thu, 09 Sep 2021 23:41:48 GMT  
		Size: 4.2 MB (4158481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4227e148c1053ae9735f2dcc2ab35b83566aab7b85aa3d50395ec15be4630e26`  
		Last Modified: Thu, 09 Sep 2021 23:41:47 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.5-windowsservercore`

```console
$ docker pull nats@sha256:fc4b18ccf5f4b0e559c7deb1e5c01e21f0ba9699b9a6966fce5548faec1f5dfb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.2114; amd64
	-	windows version 10.0.14393.4583; amd64

### `nats:2.5-windowsservercore` - windows version 10.0.17763.2114; amd64

```console
$ docker pull nats@sha256:ea5bd03ca8c905a9bb8df9bcefe1c70aada9fce64c82d90932dfaf570332087a
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2691339003 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce14639524af68868fed35dda40295ffe16c35eb58b5038f43989d7d60f7059d`
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
# Fri, 10 Sep 2021 00:14:04 GMT
ENV NATS_SERVER=2.5.0
# Fri, 10 Sep 2021 00:14:05 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.5.0/nats-server-v2.5.0-windows-amd64.zip
# Fri, 10 Sep 2021 00:14:06 GMT
ENV NATS_SERVER_SHASUM=0eae96ad4555f5060b0b6325ba972566b404cd8930b3168b9c0ffe911d15c5d8
# Fri, 10 Sep 2021 00:15:08 GMT
RUN Set-PSDebug -Trace 2
# Fri, 10 Sep 2021 00:16:32 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 10 Sep 2021 00:16:33 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 10 Sep 2021 00:16:34 GMT
EXPOSE 4222 6222 8222
# Fri, 10 Sep 2021 00:16:34 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 10 Sep 2021 00:16:35 GMT
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
	-	`sha256:4c32056c4535002b64e42d1424edb3a7ac778c308d2d9109f33d738d59c85454`  
		Last Modified: Fri, 10 Sep 2021 00:20:02 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb115761571c4ba7b8b719d8ee1587c8898f7e13246d1a92ee2283c0f929a1b1`  
		Last Modified: Fri, 10 Sep 2021 00:20:01 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd93d02cef774a55aa7c6f566b3b5718436cbdae64582cc888ef3b1efe452735`  
		Last Modified: Fri, 10 Sep 2021 00:20:01 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f28336574033153776b7149c4d079b46a95608a291563bc581fc8b029d9399c`  
		Last Modified: Fri, 10 Sep 2021 00:20:02 GMT  
		Size: 372.4 KB (372418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcce3c7fbad71cacb4533bac881f55d312123c387549ca7840f402aa108fb59d`  
		Last Modified: Fri, 10 Sep 2021 00:20:05 GMT  
		Size: 5.0 MB (4955556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0d387c2eda58f8b5f8c3889645ec5e1a977b681cb17de77c04de1c643341b18`  
		Last Modified: Fri, 10 Sep 2021 00:19:59 GMT  
		Size: 1.9 KB (1944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f70bbbc8ecda378ae0099ea8e49350ba7d78be681cd5defc71e6f624abca5d7`  
		Last Modified: Fri, 10 Sep 2021 00:19:59 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76b0025f319f789e7c26483abcf5ca7944dc5a1f0a071023d2415526aa310d40`  
		Last Modified: Fri, 10 Sep 2021 00:19:59 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99ff7344cf8ed7957719594d8f9fe4d78b0ef7acc3755bb1962febcf166ac4ce`  
		Last Modified: Fri, 10 Sep 2021 00:19:59 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.5-windowsservercore` - windows version 10.0.14393.4583; amd64

```console
$ docker pull nats@sha256:7f318bb6bf586d9b74b6b8e8097ffabf3b4d16c43c5b9b2dd62d532713aa0305
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6276274196 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5716654340a54076fb48e8d797d45b91a2e56551a534fb6d800d7d6c61262257`
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
# Fri, 10 Sep 2021 00:16:55 GMT
ENV NATS_SERVER=2.5.0
# Fri, 10 Sep 2021 00:16:56 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.5.0/nats-server-v2.5.0-windows-amd64.zip
# Fri, 10 Sep 2021 00:16:57 GMT
ENV NATS_SERVER_SHASUM=0eae96ad4555f5060b0b6325ba972566b404cd8930b3168b9c0ffe911d15c5d8
# Fri, 10 Sep 2021 00:17:43 GMT
RUN Set-PSDebug -Trace 2
# Fri, 10 Sep 2021 00:19:14 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 10 Sep 2021 00:19:15 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 10 Sep 2021 00:19:16 GMT
EXPOSE 4222 6222 8222
# Fri, 10 Sep 2021 00:19:17 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 10 Sep 2021 00:19:18 GMT
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
	-	`sha256:786675b79153c67ad039b6b8a55171a8167b2ff8c8186ccb7c5cab0b01f47767`  
		Last Modified: Fri, 10 Sep 2021 00:20:42 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65445b8a1c334a2efce7d34289af9fa682427cba808180c96ce46f39f765e9b5`  
		Last Modified: Fri, 10 Sep 2021 00:20:42 GMT  
		Size: 1.4 KB (1358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08647f69046830b98e59118ace63049f027ad1786cc2aaad037990a4e7a87344`  
		Last Modified: Fri, 10 Sep 2021 00:20:42 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b50cf5c744e8952689c263dbc9800bbe4a032fb4c8df3c8e5028092bdb2a5c9c`  
		Last Modified: Fri, 10 Sep 2021 00:20:42 GMT  
		Size: 338.0 KB (337964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:459c701464a835b4d39cc3183fff454248a3045bb433c26b0430f06e91acf1bb`  
		Last Modified: Fri, 10 Sep 2021 00:20:41 GMT  
		Size: 5.0 MB (4957179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cb2fb143896bcefca1d8ad8640f3146b771f5b284f01be2b849a048d9ac9eeb`  
		Last Modified: Fri, 10 Sep 2021 00:20:40 GMT  
		Size: 1.9 KB (1938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d9f7d515a8e73d005392fc0bccc42761025b86ab370cffe210a552fe53d1cbe`  
		Last Modified: Fri, 10 Sep 2021 00:20:40 GMT  
		Size: 1.4 KB (1380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d68902a6dec2675ab57a60716c10ce8a85e58fe54d7abea307bc340452e882a`  
		Last Modified: Fri, 10 Sep 2021 00:20:39 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37e0389f87abc858cef1a365e6b548d7d7762be571608840bc715ef352c41084`  
		Last Modified: Fri, 10 Sep 2021 00:20:39 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.5-windowsservercore-1809`

```console
$ docker pull nats@sha256:4e912b79015d0859d5b6c675d055f80bd7628c8e368d96466b6ab6d9c7a51f7b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2114; amd64

### `nats:2.5-windowsservercore-1809` - windows version 10.0.17763.2114; amd64

```console
$ docker pull nats@sha256:ea5bd03ca8c905a9bb8df9bcefe1c70aada9fce64c82d90932dfaf570332087a
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2691339003 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce14639524af68868fed35dda40295ffe16c35eb58b5038f43989d7d60f7059d`
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
# Fri, 10 Sep 2021 00:14:04 GMT
ENV NATS_SERVER=2.5.0
# Fri, 10 Sep 2021 00:14:05 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.5.0/nats-server-v2.5.0-windows-amd64.zip
# Fri, 10 Sep 2021 00:14:06 GMT
ENV NATS_SERVER_SHASUM=0eae96ad4555f5060b0b6325ba972566b404cd8930b3168b9c0ffe911d15c5d8
# Fri, 10 Sep 2021 00:15:08 GMT
RUN Set-PSDebug -Trace 2
# Fri, 10 Sep 2021 00:16:32 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 10 Sep 2021 00:16:33 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 10 Sep 2021 00:16:34 GMT
EXPOSE 4222 6222 8222
# Fri, 10 Sep 2021 00:16:34 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 10 Sep 2021 00:16:35 GMT
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
	-	`sha256:4c32056c4535002b64e42d1424edb3a7ac778c308d2d9109f33d738d59c85454`  
		Last Modified: Fri, 10 Sep 2021 00:20:02 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb115761571c4ba7b8b719d8ee1587c8898f7e13246d1a92ee2283c0f929a1b1`  
		Last Modified: Fri, 10 Sep 2021 00:20:01 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd93d02cef774a55aa7c6f566b3b5718436cbdae64582cc888ef3b1efe452735`  
		Last Modified: Fri, 10 Sep 2021 00:20:01 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f28336574033153776b7149c4d079b46a95608a291563bc581fc8b029d9399c`  
		Last Modified: Fri, 10 Sep 2021 00:20:02 GMT  
		Size: 372.4 KB (372418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcce3c7fbad71cacb4533bac881f55d312123c387549ca7840f402aa108fb59d`  
		Last Modified: Fri, 10 Sep 2021 00:20:05 GMT  
		Size: 5.0 MB (4955556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0d387c2eda58f8b5f8c3889645ec5e1a977b681cb17de77c04de1c643341b18`  
		Last Modified: Fri, 10 Sep 2021 00:19:59 GMT  
		Size: 1.9 KB (1944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f70bbbc8ecda378ae0099ea8e49350ba7d78be681cd5defc71e6f624abca5d7`  
		Last Modified: Fri, 10 Sep 2021 00:19:59 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76b0025f319f789e7c26483abcf5ca7944dc5a1f0a071023d2415526aa310d40`  
		Last Modified: Fri, 10 Sep 2021 00:19:59 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99ff7344cf8ed7957719594d8f9fe4d78b0ef7acc3755bb1962febcf166ac4ce`  
		Last Modified: Fri, 10 Sep 2021 00:19:59 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.5-windowsservercore-ltsc2016`

```console
$ docker pull nats@sha256:521575d35d4f87b16aa1482f712733b1273962ba4f75353d07327cfc4e324cee
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.14393.4583; amd64

### `nats:2.5-windowsservercore-ltsc2016` - windows version 10.0.14393.4583; amd64

```console
$ docker pull nats@sha256:7f318bb6bf586d9b74b6b8e8097ffabf3b4d16c43c5b9b2dd62d532713aa0305
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6276274196 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5716654340a54076fb48e8d797d45b91a2e56551a534fb6d800d7d6c61262257`
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
# Fri, 10 Sep 2021 00:16:55 GMT
ENV NATS_SERVER=2.5.0
# Fri, 10 Sep 2021 00:16:56 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.5.0/nats-server-v2.5.0-windows-amd64.zip
# Fri, 10 Sep 2021 00:16:57 GMT
ENV NATS_SERVER_SHASUM=0eae96ad4555f5060b0b6325ba972566b404cd8930b3168b9c0ffe911d15c5d8
# Fri, 10 Sep 2021 00:17:43 GMT
RUN Set-PSDebug -Trace 2
# Fri, 10 Sep 2021 00:19:14 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 10 Sep 2021 00:19:15 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 10 Sep 2021 00:19:16 GMT
EXPOSE 4222 6222 8222
# Fri, 10 Sep 2021 00:19:17 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 10 Sep 2021 00:19:18 GMT
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
	-	`sha256:786675b79153c67ad039b6b8a55171a8167b2ff8c8186ccb7c5cab0b01f47767`  
		Last Modified: Fri, 10 Sep 2021 00:20:42 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65445b8a1c334a2efce7d34289af9fa682427cba808180c96ce46f39f765e9b5`  
		Last Modified: Fri, 10 Sep 2021 00:20:42 GMT  
		Size: 1.4 KB (1358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08647f69046830b98e59118ace63049f027ad1786cc2aaad037990a4e7a87344`  
		Last Modified: Fri, 10 Sep 2021 00:20:42 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b50cf5c744e8952689c263dbc9800bbe4a032fb4c8df3c8e5028092bdb2a5c9c`  
		Last Modified: Fri, 10 Sep 2021 00:20:42 GMT  
		Size: 338.0 KB (337964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:459c701464a835b4d39cc3183fff454248a3045bb433c26b0430f06e91acf1bb`  
		Last Modified: Fri, 10 Sep 2021 00:20:41 GMT  
		Size: 5.0 MB (4957179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cb2fb143896bcefca1d8ad8640f3146b771f5b284f01be2b849a048d9ac9eeb`  
		Last Modified: Fri, 10 Sep 2021 00:20:40 GMT  
		Size: 1.9 KB (1938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d9f7d515a8e73d005392fc0bccc42761025b86ab370cffe210a552fe53d1cbe`  
		Last Modified: Fri, 10 Sep 2021 00:20:40 GMT  
		Size: 1.4 KB (1380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d68902a6dec2675ab57a60716c10ce8a85e58fe54d7abea307bc340452e882a`  
		Last Modified: Fri, 10 Sep 2021 00:20:39 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37e0389f87abc858cef1a365e6b548d7d7762be571608840bc715ef352c41084`  
		Last Modified: Fri, 10 Sep 2021 00:20:39 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.5.0`

```console
$ docker pull nats@sha256:c812e8c75705b49bfc4694743b59428590372ff6689425c86ea3ddd682fd8c58
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.2114; amd64

### `nats:2.5.0` - linux; amd64

```console
$ docker pull nats@sha256:01dbe57fde6a40eecbd53edc6a418f3c9b1ddd85f03dd17e73ecef98a3b15318
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4546051 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80fcdf2bfe0f4a11267c9e8d06e5e52dce7dd9b41267e1a51d5e9df22c76bf9c`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 10 Sep 2021 00:20:41 GMT
COPY file:0b180121e1ef70970b020901a4b61990a8673ac9db99b94c348c5321333884ea in /nats-server 
# Fri, 10 Sep 2021 00:20:41 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 10 Sep 2021 00:20:41 GMT
EXPOSE 4222 6222 8222
# Fri, 10 Sep 2021 00:20:41 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 10 Sep 2021 00:20:42 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:9cee557b7d3312d12996f8c4338bf9ea02657256657ef77d46510c729d9be195`  
		Last Modified: Fri, 10 Sep 2021 00:21:32 GMT  
		Size: 4.5 MB (4545577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb24b942a0d168497adac7ad3190098a6f8dfa34ad2ef37932150fbce9336c9a`  
		Last Modified: Fri, 10 Sep 2021 00:21:31 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.5.0` - linux; arm variant v6

```console
$ docker pull nats@sha256:b21057f1f945b501d03cf3c5c2d530f7961e1a3198e00bb297b7f69a849cc0e9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4210290 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:865dcd8a77138e8339293c7089adeee440305e68331df5533186ea36b8132f84`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 09 Sep 2021 23:50:15 GMT
COPY file:a60049eef2da0cbda1255e229e5e5c6377e3c3445b0cd16ce13a272139c7ce85 in /nats-server 
# Thu, 09 Sep 2021 23:50:16 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 09 Sep 2021 23:50:17 GMT
EXPOSE 4222 6222 8222
# Thu, 09 Sep 2021 23:50:17 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 09 Sep 2021 23:50:18 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b95232e9c9c31dfba5a6124fb74b4abc750a3fd6d5f89a13438a0b051430299e`  
		Last Modified: Thu, 09 Sep 2021 23:52:42 GMT  
		Size: 4.2 MB (4209813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2c01128246ad2a36efed9386a5ed63a01f73f3f56e54d059834ac17a2f64a48`  
		Last Modified: Thu, 09 Sep 2021 23:52:38 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.5.0` - linux; arm variant v7

```console
$ docker pull nats@sha256:aafbb0b5e1b7412f9d0e71ddd6c3948c7080697882dd40ae20578b855ca40c1f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4206272 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:79f5a4fb5f9254997b2d7e573f24316740a167eb829bb23952ba05ff8304ddc1`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 10 Sep 2021 00:59:05 GMT
COPY file:7043dd814cd92048127f9905d58e9204d2968d9c03bbb7feba592c45a87e9963 in /nats-server 
# Fri, 10 Sep 2021 00:59:06 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 10 Sep 2021 00:59:06 GMT
EXPOSE 4222 6222 8222
# Fri, 10 Sep 2021 00:59:07 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 10 Sep 2021 00:59:07 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:8ae70a7ddee0b3bc3819ff86ee31d3295a37b10282b7ee0d14d3dd3c8dcb16c7`  
		Last Modified: Fri, 10 Sep 2021 01:01:28 GMT  
		Size: 4.2 MB (4205795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbbfbfa45875dc8bff20ba3a989407cf3ab8018f98f4277411dd068510c071c6`  
		Last Modified: Fri, 10 Sep 2021 01:01:25 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.5.0` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:24f192937e7bc371f7c2631055e49a51d489659d28f55b4fdf2eb5a19843a5ae
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4158958 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2cd8bb7e96599c9badd4424f86ef2d5f8561cfa0c4a4322057847c002da643a9`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 09 Sep 2021 23:40:25 GMT
COPY file:eda8ae8779fbfb7d34c95bc93fc8ce409cbd298cb302284f61ee4ebf6ac10b0e in /nats-server 
# Thu, 09 Sep 2021 23:40:26 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 09 Sep 2021 23:40:26 GMT
EXPOSE 4222 6222 8222
# Thu, 09 Sep 2021 23:40:26 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 09 Sep 2021 23:40:26 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:0c0083faeb4bd1e89eefb7cbc2a5556eb056acaba6107a833c271a1ca7cd8633`  
		Last Modified: Thu, 09 Sep 2021 23:41:48 GMT  
		Size: 4.2 MB (4158481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4227e148c1053ae9735f2dcc2ab35b83566aab7b85aa3d50395ec15be4630e26`  
		Last Modified: Thu, 09 Sep 2021 23:41:47 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.5.0` - windows version 10.0.17763.2114; amd64

```console
$ docker pull nats@sha256:da56a6dd1f9556f706d9086ed48947ac745a5b9dd1e3bc0d988581858828c23c
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.4 MB (107351558 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:780da6fbe38cee622e2d2e69123219af601b417dada779a198cef0514370203e`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 05 Aug 2021 19:15:20 GMT
RUN Apply image 1809-amd64
# Wed, 25 Aug 2021 16:07:56 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 10 Sep 2021 00:16:45 GMT
RUN cmd /S /C #(nop) COPY file:13fac1899b72f2f26df9bd8ce320e46a5f7736306d7abf82ea7d657c16444fb9 in C:\nats-server.exe 
# Fri, 10 Sep 2021 00:16:46 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 10 Sep 2021 00:16:47 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Fri, 10 Sep 2021 00:16:47 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 10 Sep 2021 00:16:48 GMT
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
	-	`sha256:55bd340c78387be49377457ea8e39875e7be9b3799bdac42ff35c749d67b3940`  
		Last Modified: Fri, 10 Sep 2021 00:20:25 GMT  
		Size: 4.6 MB (4604102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76e6782c003b15abdb2161dc360ffef0eeb967b34fc78186d8d6085aacfc85fa`  
		Last Modified: Fri, 10 Sep 2021 00:20:20 GMT  
		Size: 1.8 KB (1777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf24d35e2c525beccaa7b227eda13492b401302f8ecc528e2a35118220e3f760`  
		Last Modified: Fri, 10 Sep 2021 00:20:20 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71603cdad9bbdd669dd86cda1c010a6f91d1a58de21eac052a29279f77bd247f`  
		Last Modified: Fri, 10 Sep 2021 00:20:20 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01477f3ed16729139c6a0a856de33336e03c4fb127df26c6e42b8157eaf1801b`  
		Last Modified: Fri, 10 Sep 2021 00:20:20 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.5.0-alpine`

```console
$ docker pull nats@sha256:52a8fe18f5c85cdd5cf0304eadb4e4a6a4208db9183fabc36140ff9ed7a813a3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.5.0-alpine` - linux; amd64

```console
$ docker pull nats@sha256:f6b2376c122defe213696fdbf87c7f365bdbbd60a6068fe88b1ab8aee27987d2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7647076 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b59fdb5895884cf160a5cabba5411b4a328b11aa2798042d794fe41e69fe8165`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 10 Sep 2021 00:20:12 GMT
ENV NATS_SERVER=2.5.0
# Fri, 10 Sep 2021 00:20:15 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='93f64cd14f04b4e7f6c3a2c10d09888be653406b7bc1a41f399ae44746388a5c' ;; 		armhf) natsArch='arm6'; sha256='12f38f6881cdcf27c0faebb7ab6580b40253c36dc1531d499a29c4998a009494' ;; 		armv7) natsArch='arm7'; sha256='fb3611b57a932f5c75310dee66597057ab65b442eb84d73b2c5fd9389eb6e518' ;; 		x86_64) natsArch='amd64'; sha256='4d2f4abb15b45618ce772659c9f3eca60f25266dfc976f0354430ad67c8fd886' ;; 		x86) natsArch='386'; sha256='776aecc77c33146d88e6b3cb1787097f9817122182f49f7243c0ea3fd62ad029' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 10 Sep 2021 00:20:15 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 10 Sep 2021 00:20:15 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 10 Sep 2021 00:20:15 GMT
EXPOSE 4222 6222 8222
# Fri, 10 Sep 2021 00:20:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 10 Sep 2021 00:20:16 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59a9809baa02715a6c4ccdb1ebc94edaf948058be9f97cea623426ca670b426e`  
		Last Modified: Fri, 10 Sep 2021 00:21:08 GMT  
		Size: 4.8 MB (4831663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68c0794b9b379d130866e40babeef9f4557514bcc2c88194e89b90081ef7ad12`  
		Last Modified: Fri, 10 Sep 2021 00:21:08 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:240551b5739b209d882cd7b4f76138b9188aac1a497ff32a469526302056dd98`  
		Last Modified: Fri, 10 Sep 2021 00:21:07 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.5.0-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:c516621cb4dc61ad9db1927cdcec7210328be6d7b813acb688016584d61be212
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7121422 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c48580010dc9af32e7a019914f078134ae513ef77280b7877fe7fd47665426b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:49:29 GMT
ADD file:1c1c4520d49cb6e8f795f3b953d1ed3c3c77868b98b53a455169c254fcec5acd in / 
# Fri, 27 Aug 2021 17:49:30 GMT
CMD ["/bin/sh"]
# Thu, 09 Sep 2021 23:49:46 GMT
ENV NATS_SERVER=2.5.0
# Thu, 09 Sep 2021 23:49:51 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='93f64cd14f04b4e7f6c3a2c10d09888be653406b7bc1a41f399ae44746388a5c' ;; 		armhf) natsArch='arm6'; sha256='12f38f6881cdcf27c0faebb7ab6580b40253c36dc1531d499a29c4998a009494' ;; 		armv7) natsArch='arm7'; sha256='fb3611b57a932f5c75310dee66597057ab65b442eb84d73b2c5fd9389eb6e518' ;; 		x86_64) natsArch='amd64'; sha256='4d2f4abb15b45618ce772659c9f3eca60f25266dfc976f0354430ad67c8fd886' ;; 		x86) natsArch='386'; sha256='776aecc77c33146d88e6b3cb1787097f9817122182f49f7243c0ea3fd62ad029' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 09 Sep 2021 23:49:51 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 09 Sep 2021 23:49:52 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 09 Sep 2021 23:49:52 GMT
EXPOSE 4222 6222 8222
# Thu, 09 Sep 2021 23:49:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 09 Sep 2021 23:49:53 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:2e78c0f86ba9a1fed30df20cb48c9cc73e9626399f12749d36b892ff99c0ecf5`  
		Last Modified: Fri, 27 Aug 2021 17:50:55 GMT  
		Size: 2.6 MB (2627447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75b214a44f07577985e2f01798e9acf02be903c28022f74d244b22418b31e815`  
		Last Modified: Thu, 09 Sep 2021 23:52:03 GMT  
		Size: 4.5 MB (4493006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d232ac6d6c1f822be800be02acbb341f7abe35b05bd13a0857df02fd1cc600a6`  
		Last Modified: Thu, 09 Sep 2021 23:52:01 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e364400828db299d750b3bcc80b1e3b1df2f7abe62c5d6293f3c7e22d93e20a`  
		Last Modified: Thu, 09 Sep 2021 23:52:00 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.5.0-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:c5a16f99958e4ae6f318a577619242a7d168fc47e07883d8adbc1701faa36ab4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.9 MB (6918058 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b6128ceec7a63c74e316f6b3bda400e98def18ed14e046a0177a1095946dd8e2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:57:31 GMT
ADD file:a7da7992ccea54d3295231027614f138aa45c4d4a25ea6ec9bf7b316b9f67d95 in / 
# Fri, 27 Aug 2021 17:57:32 GMT
CMD ["/bin/sh"]
# Fri, 10 Sep 2021 00:58:26 GMT
ENV NATS_SERVER=2.5.0
# Fri, 10 Sep 2021 00:58:31 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='93f64cd14f04b4e7f6c3a2c10d09888be653406b7bc1a41f399ae44746388a5c' ;; 		armhf) natsArch='arm6'; sha256='12f38f6881cdcf27c0faebb7ab6580b40253c36dc1531d499a29c4998a009494' ;; 		armv7) natsArch='arm7'; sha256='fb3611b57a932f5c75310dee66597057ab65b442eb84d73b2c5fd9389eb6e518' ;; 		x86_64) natsArch='amd64'; sha256='4d2f4abb15b45618ce772659c9f3eca60f25266dfc976f0354430ad67c8fd886' ;; 		x86) natsArch='386'; sha256='776aecc77c33146d88e6b3cb1787097f9817122182f49f7243c0ea3fd62ad029' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 10 Sep 2021 00:58:32 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 10 Sep 2021 00:58:32 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 10 Sep 2021 00:58:33 GMT
EXPOSE 4222 6222 8222
# Fri, 10 Sep 2021 00:58:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 10 Sep 2021 00:58:34 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:a14774a5a62e0f454febaec7cb603e18a6a8e25ef9da4a4da85b155bdd5e5a7a`  
		Last Modified: Fri, 27 Aug 2021 17:59:00 GMT  
		Size: 2.4 MB (2430419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2edd63df5776202ac2717836b8350736f3e046021c53b49e6e872ef9f4a960a9`  
		Last Modified: Fri, 10 Sep 2021 01:00:49 GMT  
		Size: 4.5 MB (4486667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d073c5b9595fcde55c46ccb0f54148caba30c630427ffcdfe9f03a4e84be10ec`  
		Last Modified: Fri, 10 Sep 2021 01:00:46 GMT  
		Size: 559.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15f66a2a44784b8ce7529a34b470376f9a52740980b2b05baf8525ec5f4a39f2`  
		Last Modified: Fri, 10 Sep 2021 01:00:46 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.5.0-alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:88b4d8f2f54f207d5400e8d3e9037d55ca8d2969b126e07d833c6d3464f93300
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7156798 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f803b2b0ed9b56df4cac8c3a03dfd789e480a622c1f3a282ecee5fd0f937d9e5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Thu, 09 Sep 2021 23:40:02 GMT
ENV NATS_SERVER=2.5.0
# Thu, 09 Sep 2021 23:40:05 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='93f64cd14f04b4e7f6c3a2c10d09888be653406b7bc1a41f399ae44746388a5c' ;; 		armhf) natsArch='arm6'; sha256='12f38f6881cdcf27c0faebb7ab6580b40253c36dc1531d499a29c4998a009494' ;; 		armv7) natsArch='arm7'; sha256='fb3611b57a932f5c75310dee66597057ab65b442eb84d73b2c5fd9389eb6e518' ;; 		x86_64) natsArch='amd64'; sha256='4d2f4abb15b45618ce772659c9f3eca60f25266dfc976f0354430ad67c8fd886' ;; 		x86) natsArch='386'; sha256='776aecc77c33146d88e6b3cb1787097f9817122182f49f7243c0ea3fd62ad029' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 09 Sep 2021 23:40:05 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 09 Sep 2021 23:40:05 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 09 Sep 2021 23:40:05 GMT
EXPOSE 4222 6222 8222
# Thu, 09 Sep 2021 23:40:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 09 Sep 2021 23:40:06 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:552d1f2373af9bfe12033568ebbfb0ccbb0de11279f9a415a29207e264d7f4d9`  
		Last Modified: Fri, 27 Aug 2021 17:40:18 GMT  
		Size: 2.7 MB (2711827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49450e2f2462d1e207a865d4a084154f6a3c5edc2b3b4954d34d4e1ce75d38f2`  
		Last Modified: Thu, 09 Sep 2021 23:41:18 GMT  
		Size: 4.4 MB (4444005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edeb0b05b16add9a16e4a8bc8c1eced6c1f60f58ac669216dbbf93cb9bce40d2`  
		Last Modified: Thu, 09 Sep 2021 23:41:18 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67be552e94a6cfc686543e5bfa0c1a6bca72bc9dce939fb9f3e43c4a77f5e6e3`  
		Last Modified: Thu, 09 Sep 2021 23:41:18 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.5.0-alpine3.14`

```console
$ docker pull nats@sha256:52a8fe18f5c85cdd5cf0304eadb4e4a6a4208db9183fabc36140ff9ed7a813a3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.5.0-alpine3.14` - linux; amd64

```console
$ docker pull nats@sha256:f6b2376c122defe213696fdbf87c7f365bdbbd60a6068fe88b1ab8aee27987d2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7647076 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b59fdb5895884cf160a5cabba5411b4a328b11aa2798042d794fe41e69fe8165`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 10 Sep 2021 00:20:12 GMT
ENV NATS_SERVER=2.5.0
# Fri, 10 Sep 2021 00:20:15 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='93f64cd14f04b4e7f6c3a2c10d09888be653406b7bc1a41f399ae44746388a5c' ;; 		armhf) natsArch='arm6'; sha256='12f38f6881cdcf27c0faebb7ab6580b40253c36dc1531d499a29c4998a009494' ;; 		armv7) natsArch='arm7'; sha256='fb3611b57a932f5c75310dee66597057ab65b442eb84d73b2c5fd9389eb6e518' ;; 		x86_64) natsArch='amd64'; sha256='4d2f4abb15b45618ce772659c9f3eca60f25266dfc976f0354430ad67c8fd886' ;; 		x86) natsArch='386'; sha256='776aecc77c33146d88e6b3cb1787097f9817122182f49f7243c0ea3fd62ad029' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 10 Sep 2021 00:20:15 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 10 Sep 2021 00:20:15 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 10 Sep 2021 00:20:15 GMT
EXPOSE 4222 6222 8222
# Fri, 10 Sep 2021 00:20:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 10 Sep 2021 00:20:16 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59a9809baa02715a6c4ccdb1ebc94edaf948058be9f97cea623426ca670b426e`  
		Last Modified: Fri, 10 Sep 2021 00:21:08 GMT  
		Size: 4.8 MB (4831663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68c0794b9b379d130866e40babeef9f4557514bcc2c88194e89b90081ef7ad12`  
		Last Modified: Fri, 10 Sep 2021 00:21:08 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:240551b5739b209d882cd7b4f76138b9188aac1a497ff32a469526302056dd98`  
		Last Modified: Fri, 10 Sep 2021 00:21:07 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.5.0-alpine3.14` - linux; arm variant v6

```console
$ docker pull nats@sha256:c516621cb4dc61ad9db1927cdcec7210328be6d7b813acb688016584d61be212
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7121422 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c48580010dc9af32e7a019914f078134ae513ef77280b7877fe7fd47665426b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:49:29 GMT
ADD file:1c1c4520d49cb6e8f795f3b953d1ed3c3c77868b98b53a455169c254fcec5acd in / 
# Fri, 27 Aug 2021 17:49:30 GMT
CMD ["/bin/sh"]
# Thu, 09 Sep 2021 23:49:46 GMT
ENV NATS_SERVER=2.5.0
# Thu, 09 Sep 2021 23:49:51 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='93f64cd14f04b4e7f6c3a2c10d09888be653406b7bc1a41f399ae44746388a5c' ;; 		armhf) natsArch='arm6'; sha256='12f38f6881cdcf27c0faebb7ab6580b40253c36dc1531d499a29c4998a009494' ;; 		armv7) natsArch='arm7'; sha256='fb3611b57a932f5c75310dee66597057ab65b442eb84d73b2c5fd9389eb6e518' ;; 		x86_64) natsArch='amd64'; sha256='4d2f4abb15b45618ce772659c9f3eca60f25266dfc976f0354430ad67c8fd886' ;; 		x86) natsArch='386'; sha256='776aecc77c33146d88e6b3cb1787097f9817122182f49f7243c0ea3fd62ad029' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 09 Sep 2021 23:49:51 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 09 Sep 2021 23:49:52 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 09 Sep 2021 23:49:52 GMT
EXPOSE 4222 6222 8222
# Thu, 09 Sep 2021 23:49:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 09 Sep 2021 23:49:53 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:2e78c0f86ba9a1fed30df20cb48c9cc73e9626399f12749d36b892ff99c0ecf5`  
		Last Modified: Fri, 27 Aug 2021 17:50:55 GMT  
		Size: 2.6 MB (2627447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75b214a44f07577985e2f01798e9acf02be903c28022f74d244b22418b31e815`  
		Last Modified: Thu, 09 Sep 2021 23:52:03 GMT  
		Size: 4.5 MB (4493006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d232ac6d6c1f822be800be02acbb341f7abe35b05bd13a0857df02fd1cc600a6`  
		Last Modified: Thu, 09 Sep 2021 23:52:01 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e364400828db299d750b3bcc80b1e3b1df2f7abe62c5d6293f3c7e22d93e20a`  
		Last Modified: Thu, 09 Sep 2021 23:52:00 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.5.0-alpine3.14` - linux; arm variant v7

```console
$ docker pull nats@sha256:c5a16f99958e4ae6f318a577619242a7d168fc47e07883d8adbc1701faa36ab4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.9 MB (6918058 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b6128ceec7a63c74e316f6b3bda400e98def18ed14e046a0177a1095946dd8e2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:57:31 GMT
ADD file:a7da7992ccea54d3295231027614f138aa45c4d4a25ea6ec9bf7b316b9f67d95 in / 
# Fri, 27 Aug 2021 17:57:32 GMT
CMD ["/bin/sh"]
# Fri, 10 Sep 2021 00:58:26 GMT
ENV NATS_SERVER=2.5.0
# Fri, 10 Sep 2021 00:58:31 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='93f64cd14f04b4e7f6c3a2c10d09888be653406b7bc1a41f399ae44746388a5c' ;; 		armhf) natsArch='arm6'; sha256='12f38f6881cdcf27c0faebb7ab6580b40253c36dc1531d499a29c4998a009494' ;; 		armv7) natsArch='arm7'; sha256='fb3611b57a932f5c75310dee66597057ab65b442eb84d73b2c5fd9389eb6e518' ;; 		x86_64) natsArch='amd64'; sha256='4d2f4abb15b45618ce772659c9f3eca60f25266dfc976f0354430ad67c8fd886' ;; 		x86) natsArch='386'; sha256='776aecc77c33146d88e6b3cb1787097f9817122182f49f7243c0ea3fd62ad029' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 10 Sep 2021 00:58:32 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 10 Sep 2021 00:58:32 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 10 Sep 2021 00:58:33 GMT
EXPOSE 4222 6222 8222
# Fri, 10 Sep 2021 00:58:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 10 Sep 2021 00:58:34 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:a14774a5a62e0f454febaec7cb603e18a6a8e25ef9da4a4da85b155bdd5e5a7a`  
		Last Modified: Fri, 27 Aug 2021 17:59:00 GMT  
		Size: 2.4 MB (2430419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2edd63df5776202ac2717836b8350736f3e046021c53b49e6e872ef9f4a960a9`  
		Last Modified: Fri, 10 Sep 2021 01:00:49 GMT  
		Size: 4.5 MB (4486667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d073c5b9595fcde55c46ccb0f54148caba30c630427ffcdfe9f03a4e84be10ec`  
		Last Modified: Fri, 10 Sep 2021 01:00:46 GMT  
		Size: 559.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15f66a2a44784b8ce7529a34b470376f9a52740980b2b05baf8525ec5f4a39f2`  
		Last Modified: Fri, 10 Sep 2021 01:00:46 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.5.0-alpine3.14` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:88b4d8f2f54f207d5400e8d3e9037d55ca8d2969b126e07d833c6d3464f93300
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7156798 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f803b2b0ed9b56df4cac8c3a03dfd789e480a622c1f3a282ecee5fd0f937d9e5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Thu, 09 Sep 2021 23:40:02 GMT
ENV NATS_SERVER=2.5.0
# Thu, 09 Sep 2021 23:40:05 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='93f64cd14f04b4e7f6c3a2c10d09888be653406b7bc1a41f399ae44746388a5c' ;; 		armhf) natsArch='arm6'; sha256='12f38f6881cdcf27c0faebb7ab6580b40253c36dc1531d499a29c4998a009494' ;; 		armv7) natsArch='arm7'; sha256='fb3611b57a932f5c75310dee66597057ab65b442eb84d73b2c5fd9389eb6e518' ;; 		x86_64) natsArch='amd64'; sha256='4d2f4abb15b45618ce772659c9f3eca60f25266dfc976f0354430ad67c8fd886' ;; 		x86) natsArch='386'; sha256='776aecc77c33146d88e6b3cb1787097f9817122182f49f7243c0ea3fd62ad029' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 09 Sep 2021 23:40:05 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 09 Sep 2021 23:40:05 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 09 Sep 2021 23:40:05 GMT
EXPOSE 4222 6222 8222
# Thu, 09 Sep 2021 23:40:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 09 Sep 2021 23:40:06 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:552d1f2373af9bfe12033568ebbfb0ccbb0de11279f9a415a29207e264d7f4d9`  
		Last Modified: Fri, 27 Aug 2021 17:40:18 GMT  
		Size: 2.7 MB (2711827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49450e2f2462d1e207a865d4a084154f6a3c5edc2b3b4954d34d4e1ce75d38f2`  
		Last Modified: Thu, 09 Sep 2021 23:41:18 GMT  
		Size: 4.4 MB (4444005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edeb0b05b16add9a16e4a8bc8c1eced6c1f60f58ac669216dbbf93cb9bce40d2`  
		Last Modified: Thu, 09 Sep 2021 23:41:18 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67be552e94a6cfc686543e5bfa0c1a6bca72bc9dce939fb9f3e43c4a77f5e6e3`  
		Last Modified: Thu, 09 Sep 2021 23:41:18 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.5.0-linux`

```console
$ docker pull nats@sha256:6808dfb3132c301916bbeb4241ae1f3c0be5dca763a6c0be6180ca1bd6da298a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.5.0-linux` - linux; amd64

```console
$ docker pull nats@sha256:01dbe57fde6a40eecbd53edc6a418f3c9b1ddd85f03dd17e73ecef98a3b15318
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4546051 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80fcdf2bfe0f4a11267c9e8d06e5e52dce7dd9b41267e1a51d5e9df22c76bf9c`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 10 Sep 2021 00:20:41 GMT
COPY file:0b180121e1ef70970b020901a4b61990a8673ac9db99b94c348c5321333884ea in /nats-server 
# Fri, 10 Sep 2021 00:20:41 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 10 Sep 2021 00:20:41 GMT
EXPOSE 4222 6222 8222
# Fri, 10 Sep 2021 00:20:41 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 10 Sep 2021 00:20:42 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:9cee557b7d3312d12996f8c4338bf9ea02657256657ef77d46510c729d9be195`  
		Last Modified: Fri, 10 Sep 2021 00:21:32 GMT  
		Size: 4.5 MB (4545577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb24b942a0d168497adac7ad3190098a6f8dfa34ad2ef37932150fbce9336c9a`  
		Last Modified: Fri, 10 Sep 2021 00:21:31 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.5.0-linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:b21057f1f945b501d03cf3c5c2d530f7961e1a3198e00bb297b7f69a849cc0e9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4210290 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:865dcd8a77138e8339293c7089adeee440305e68331df5533186ea36b8132f84`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 09 Sep 2021 23:50:15 GMT
COPY file:a60049eef2da0cbda1255e229e5e5c6377e3c3445b0cd16ce13a272139c7ce85 in /nats-server 
# Thu, 09 Sep 2021 23:50:16 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 09 Sep 2021 23:50:17 GMT
EXPOSE 4222 6222 8222
# Thu, 09 Sep 2021 23:50:17 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 09 Sep 2021 23:50:18 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b95232e9c9c31dfba5a6124fb74b4abc750a3fd6d5f89a13438a0b051430299e`  
		Last Modified: Thu, 09 Sep 2021 23:52:42 GMT  
		Size: 4.2 MB (4209813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2c01128246ad2a36efed9386a5ed63a01f73f3f56e54d059834ac17a2f64a48`  
		Last Modified: Thu, 09 Sep 2021 23:52:38 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.5.0-linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:aafbb0b5e1b7412f9d0e71ddd6c3948c7080697882dd40ae20578b855ca40c1f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4206272 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:79f5a4fb5f9254997b2d7e573f24316740a167eb829bb23952ba05ff8304ddc1`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 10 Sep 2021 00:59:05 GMT
COPY file:7043dd814cd92048127f9905d58e9204d2968d9c03bbb7feba592c45a87e9963 in /nats-server 
# Fri, 10 Sep 2021 00:59:06 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 10 Sep 2021 00:59:06 GMT
EXPOSE 4222 6222 8222
# Fri, 10 Sep 2021 00:59:07 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 10 Sep 2021 00:59:07 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:8ae70a7ddee0b3bc3819ff86ee31d3295a37b10282b7ee0d14d3dd3c8dcb16c7`  
		Last Modified: Fri, 10 Sep 2021 01:01:28 GMT  
		Size: 4.2 MB (4205795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbbfbfa45875dc8bff20ba3a989407cf3ab8018f98f4277411dd068510c071c6`  
		Last Modified: Fri, 10 Sep 2021 01:01:25 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.5.0-linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:24f192937e7bc371f7c2631055e49a51d489659d28f55b4fdf2eb5a19843a5ae
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4158958 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2cd8bb7e96599c9badd4424f86ef2d5f8561cfa0c4a4322057847c002da643a9`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 09 Sep 2021 23:40:25 GMT
COPY file:eda8ae8779fbfb7d34c95bc93fc8ce409cbd298cb302284f61ee4ebf6ac10b0e in /nats-server 
# Thu, 09 Sep 2021 23:40:26 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 09 Sep 2021 23:40:26 GMT
EXPOSE 4222 6222 8222
# Thu, 09 Sep 2021 23:40:26 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 09 Sep 2021 23:40:26 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:0c0083faeb4bd1e89eefb7cbc2a5556eb056acaba6107a833c271a1ca7cd8633`  
		Last Modified: Thu, 09 Sep 2021 23:41:48 GMT  
		Size: 4.2 MB (4158481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4227e148c1053ae9735f2dcc2ab35b83566aab7b85aa3d50395ec15be4630e26`  
		Last Modified: Thu, 09 Sep 2021 23:41:47 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.5.0-nanoserver`

```console
$ docker pull nats@sha256:5b8ea050ee708eb4017db4e1cb913456e468e82c227eb67a070974651446cfd9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2114; amd64

### `nats:2.5.0-nanoserver` - windows version 10.0.17763.2114; amd64

```console
$ docker pull nats@sha256:da56a6dd1f9556f706d9086ed48947ac745a5b9dd1e3bc0d988581858828c23c
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.4 MB (107351558 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:780da6fbe38cee622e2d2e69123219af601b417dada779a198cef0514370203e`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 05 Aug 2021 19:15:20 GMT
RUN Apply image 1809-amd64
# Wed, 25 Aug 2021 16:07:56 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 10 Sep 2021 00:16:45 GMT
RUN cmd /S /C #(nop) COPY file:13fac1899b72f2f26df9bd8ce320e46a5f7736306d7abf82ea7d657c16444fb9 in C:\nats-server.exe 
# Fri, 10 Sep 2021 00:16:46 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 10 Sep 2021 00:16:47 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Fri, 10 Sep 2021 00:16:47 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 10 Sep 2021 00:16:48 GMT
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
	-	`sha256:55bd340c78387be49377457ea8e39875e7be9b3799bdac42ff35c749d67b3940`  
		Last Modified: Fri, 10 Sep 2021 00:20:25 GMT  
		Size: 4.6 MB (4604102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76e6782c003b15abdb2161dc360ffef0eeb967b34fc78186d8d6085aacfc85fa`  
		Last Modified: Fri, 10 Sep 2021 00:20:20 GMT  
		Size: 1.8 KB (1777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf24d35e2c525beccaa7b227eda13492b401302f8ecc528e2a35118220e3f760`  
		Last Modified: Fri, 10 Sep 2021 00:20:20 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71603cdad9bbdd669dd86cda1c010a6f91d1a58de21eac052a29279f77bd247f`  
		Last Modified: Fri, 10 Sep 2021 00:20:20 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01477f3ed16729139c6a0a856de33336e03c4fb127df26c6e42b8157eaf1801b`  
		Last Modified: Fri, 10 Sep 2021 00:20:20 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.5.0-nanoserver-1809`

```console
$ docker pull nats@sha256:5b8ea050ee708eb4017db4e1cb913456e468e82c227eb67a070974651446cfd9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2114; amd64

### `nats:2.5.0-nanoserver-1809` - windows version 10.0.17763.2114; amd64

```console
$ docker pull nats@sha256:da56a6dd1f9556f706d9086ed48947ac745a5b9dd1e3bc0d988581858828c23c
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.4 MB (107351558 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:780da6fbe38cee622e2d2e69123219af601b417dada779a198cef0514370203e`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 05 Aug 2021 19:15:20 GMT
RUN Apply image 1809-amd64
# Wed, 25 Aug 2021 16:07:56 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 10 Sep 2021 00:16:45 GMT
RUN cmd /S /C #(nop) COPY file:13fac1899b72f2f26df9bd8ce320e46a5f7736306d7abf82ea7d657c16444fb9 in C:\nats-server.exe 
# Fri, 10 Sep 2021 00:16:46 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 10 Sep 2021 00:16:47 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Fri, 10 Sep 2021 00:16:47 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 10 Sep 2021 00:16:48 GMT
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
	-	`sha256:55bd340c78387be49377457ea8e39875e7be9b3799bdac42ff35c749d67b3940`  
		Last Modified: Fri, 10 Sep 2021 00:20:25 GMT  
		Size: 4.6 MB (4604102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76e6782c003b15abdb2161dc360ffef0eeb967b34fc78186d8d6085aacfc85fa`  
		Last Modified: Fri, 10 Sep 2021 00:20:20 GMT  
		Size: 1.8 KB (1777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf24d35e2c525beccaa7b227eda13492b401302f8ecc528e2a35118220e3f760`  
		Last Modified: Fri, 10 Sep 2021 00:20:20 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71603cdad9bbdd669dd86cda1c010a6f91d1a58de21eac052a29279f77bd247f`  
		Last Modified: Fri, 10 Sep 2021 00:20:20 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01477f3ed16729139c6a0a856de33336e03c4fb127df26c6e42b8157eaf1801b`  
		Last Modified: Fri, 10 Sep 2021 00:20:20 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.5.0-scratch`

```console
$ docker pull nats@sha256:6808dfb3132c301916bbeb4241ae1f3c0be5dca763a6c0be6180ca1bd6da298a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.5.0-scratch` - linux; amd64

```console
$ docker pull nats@sha256:01dbe57fde6a40eecbd53edc6a418f3c9b1ddd85f03dd17e73ecef98a3b15318
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4546051 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80fcdf2bfe0f4a11267c9e8d06e5e52dce7dd9b41267e1a51d5e9df22c76bf9c`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 10 Sep 2021 00:20:41 GMT
COPY file:0b180121e1ef70970b020901a4b61990a8673ac9db99b94c348c5321333884ea in /nats-server 
# Fri, 10 Sep 2021 00:20:41 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 10 Sep 2021 00:20:41 GMT
EXPOSE 4222 6222 8222
# Fri, 10 Sep 2021 00:20:41 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 10 Sep 2021 00:20:42 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:9cee557b7d3312d12996f8c4338bf9ea02657256657ef77d46510c729d9be195`  
		Last Modified: Fri, 10 Sep 2021 00:21:32 GMT  
		Size: 4.5 MB (4545577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb24b942a0d168497adac7ad3190098a6f8dfa34ad2ef37932150fbce9336c9a`  
		Last Modified: Fri, 10 Sep 2021 00:21:31 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.5.0-scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:b21057f1f945b501d03cf3c5c2d530f7961e1a3198e00bb297b7f69a849cc0e9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4210290 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:865dcd8a77138e8339293c7089adeee440305e68331df5533186ea36b8132f84`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 09 Sep 2021 23:50:15 GMT
COPY file:a60049eef2da0cbda1255e229e5e5c6377e3c3445b0cd16ce13a272139c7ce85 in /nats-server 
# Thu, 09 Sep 2021 23:50:16 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 09 Sep 2021 23:50:17 GMT
EXPOSE 4222 6222 8222
# Thu, 09 Sep 2021 23:50:17 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 09 Sep 2021 23:50:18 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b95232e9c9c31dfba5a6124fb74b4abc750a3fd6d5f89a13438a0b051430299e`  
		Last Modified: Thu, 09 Sep 2021 23:52:42 GMT  
		Size: 4.2 MB (4209813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2c01128246ad2a36efed9386a5ed63a01f73f3f56e54d059834ac17a2f64a48`  
		Last Modified: Thu, 09 Sep 2021 23:52:38 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.5.0-scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:aafbb0b5e1b7412f9d0e71ddd6c3948c7080697882dd40ae20578b855ca40c1f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4206272 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:79f5a4fb5f9254997b2d7e573f24316740a167eb829bb23952ba05ff8304ddc1`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 10 Sep 2021 00:59:05 GMT
COPY file:7043dd814cd92048127f9905d58e9204d2968d9c03bbb7feba592c45a87e9963 in /nats-server 
# Fri, 10 Sep 2021 00:59:06 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 10 Sep 2021 00:59:06 GMT
EXPOSE 4222 6222 8222
# Fri, 10 Sep 2021 00:59:07 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 10 Sep 2021 00:59:07 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:8ae70a7ddee0b3bc3819ff86ee31d3295a37b10282b7ee0d14d3dd3c8dcb16c7`  
		Last Modified: Fri, 10 Sep 2021 01:01:28 GMT  
		Size: 4.2 MB (4205795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbbfbfa45875dc8bff20ba3a989407cf3ab8018f98f4277411dd068510c071c6`  
		Last Modified: Fri, 10 Sep 2021 01:01:25 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.5.0-scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:24f192937e7bc371f7c2631055e49a51d489659d28f55b4fdf2eb5a19843a5ae
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4158958 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2cd8bb7e96599c9badd4424f86ef2d5f8561cfa0c4a4322057847c002da643a9`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 09 Sep 2021 23:40:25 GMT
COPY file:eda8ae8779fbfb7d34c95bc93fc8ce409cbd298cb302284f61ee4ebf6ac10b0e in /nats-server 
# Thu, 09 Sep 2021 23:40:26 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 09 Sep 2021 23:40:26 GMT
EXPOSE 4222 6222 8222
# Thu, 09 Sep 2021 23:40:26 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 09 Sep 2021 23:40:26 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:0c0083faeb4bd1e89eefb7cbc2a5556eb056acaba6107a833c271a1ca7cd8633`  
		Last Modified: Thu, 09 Sep 2021 23:41:48 GMT  
		Size: 4.2 MB (4158481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4227e148c1053ae9735f2dcc2ab35b83566aab7b85aa3d50395ec15be4630e26`  
		Last Modified: Thu, 09 Sep 2021 23:41:47 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.5.0-windowsservercore`

```console
$ docker pull nats@sha256:fc4b18ccf5f4b0e559c7deb1e5c01e21f0ba9699b9a6966fce5548faec1f5dfb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.2114; amd64
	-	windows version 10.0.14393.4583; amd64

### `nats:2.5.0-windowsservercore` - windows version 10.0.17763.2114; amd64

```console
$ docker pull nats@sha256:ea5bd03ca8c905a9bb8df9bcefe1c70aada9fce64c82d90932dfaf570332087a
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2691339003 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce14639524af68868fed35dda40295ffe16c35eb58b5038f43989d7d60f7059d`
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
# Fri, 10 Sep 2021 00:14:04 GMT
ENV NATS_SERVER=2.5.0
# Fri, 10 Sep 2021 00:14:05 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.5.0/nats-server-v2.5.0-windows-amd64.zip
# Fri, 10 Sep 2021 00:14:06 GMT
ENV NATS_SERVER_SHASUM=0eae96ad4555f5060b0b6325ba972566b404cd8930b3168b9c0ffe911d15c5d8
# Fri, 10 Sep 2021 00:15:08 GMT
RUN Set-PSDebug -Trace 2
# Fri, 10 Sep 2021 00:16:32 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 10 Sep 2021 00:16:33 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 10 Sep 2021 00:16:34 GMT
EXPOSE 4222 6222 8222
# Fri, 10 Sep 2021 00:16:34 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 10 Sep 2021 00:16:35 GMT
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
	-	`sha256:4c32056c4535002b64e42d1424edb3a7ac778c308d2d9109f33d738d59c85454`  
		Last Modified: Fri, 10 Sep 2021 00:20:02 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb115761571c4ba7b8b719d8ee1587c8898f7e13246d1a92ee2283c0f929a1b1`  
		Last Modified: Fri, 10 Sep 2021 00:20:01 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd93d02cef774a55aa7c6f566b3b5718436cbdae64582cc888ef3b1efe452735`  
		Last Modified: Fri, 10 Sep 2021 00:20:01 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f28336574033153776b7149c4d079b46a95608a291563bc581fc8b029d9399c`  
		Last Modified: Fri, 10 Sep 2021 00:20:02 GMT  
		Size: 372.4 KB (372418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcce3c7fbad71cacb4533bac881f55d312123c387549ca7840f402aa108fb59d`  
		Last Modified: Fri, 10 Sep 2021 00:20:05 GMT  
		Size: 5.0 MB (4955556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0d387c2eda58f8b5f8c3889645ec5e1a977b681cb17de77c04de1c643341b18`  
		Last Modified: Fri, 10 Sep 2021 00:19:59 GMT  
		Size: 1.9 KB (1944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f70bbbc8ecda378ae0099ea8e49350ba7d78be681cd5defc71e6f624abca5d7`  
		Last Modified: Fri, 10 Sep 2021 00:19:59 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76b0025f319f789e7c26483abcf5ca7944dc5a1f0a071023d2415526aa310d40`  
		Last Modified: Fri, 10 Sep 2021 00:19:59 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99ff7344cf8ed7957719594d8f9fe4d78b0ef7acc3755bb1962febcf166ac4ce`  
		Last Modified: Fri, 10 Sep 2021 00:19:59 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.5.0-windowsservercore` - windows version 10.0.14393.4583; amd64

```console
$ docker pull nats@sha256:7f318bb6bf586d9b74b6b8e8097ffabf3b4d16c43c5b9b2dd62d532713aa0305
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6276274196 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5716654340a54076fb48e8d797d45b91a2e56551a534fb6d800d7d6c61262257`
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
# Fri, 10 Sep 2021 00:16:55 GMT
ENV NATS_SERVER=2.5.0
# Fri, 10 Sep 2021 00:16:56 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.5.0/nats-server-v2.5.0-windows-amd64.zip
# Fri, 10 Sep 2021 00:16:57 GMT
ENV NATS_SERVER_SHASUM=0eae96ad4555f5060b0b6325ba972566b404cd8930b3168b9c0ffe911d15c5d8
# Fri, 10 Sep 2021 00:17:43 GMT
RUN Set-PSDebug -Trace 2
# Fri, 10 Sep 2021 00:19:14 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 10 Sep 2021 00:19:15 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 10 Sep 2021 00:19:16 GMT
EXPOSE 4222 6222 8222
# Fri, 10 Sep 2021 00:19:17 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 10 Sep 2021 00:19:18 GMT
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
	-	`sha256:786675b79153c67ad039b6b8a55171a8167b2ff8c8186ccb7c5cab0b01f47767`  
		Last Modified: Fri, 10 Sep 2021 00:20:42 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65445b8a1c334a2efce7d34289af9fa682427cba808180c96ce46f39f765e9b5`  
		Last Modified: Fri, 10 Sep 2021 00:20:42 GMT  
		Size: 1.4 KB (1358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08647f69046830b98e59118ace63049f027ad1786cc2aaad037990a4e7a87344`  
		Last Modified: Fri, 10 Sep 2021 00:20:42 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b50cf5c744e8952689c263dbc9800bbe4a032fb4c8df3c8e5028092bdb2a5c9c`  
		Last Modified: Fri, 10 Sep 2021 00:20:42 GMT  
		Size: 338.0 KB (337964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:459c701464a835b4d39cc3183fff454248a3045bb433c26b0430f06e91acf1bb`  
		Last Modified: Fri, 10 Sep 2021 00:20:41 GMT  
		Size: 5.0 MB (4957179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cb2fb143896bcefca1d8ad8640f3146b771f5b284f01be2b849a048d9ac9eeb`  
		Last Modified: Fri, 10 Sep 2021 00:20:40 GMT  
		Size: 1.9 KB (1938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d9f7d515a8e73d005392fc0bccc42761025b86ab370cffe210a552fe53d1cbe`  
		Last Modified: Fri, 10 Sep 2021 00:20:40 GMT  
		Size: 1.4 KB (1380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d68902a6dec2675ab57a60716c10ce8a85e58fe54d7abea307bc340452e882a`  
		Last Modified: Fri, 10 Sep 2021 00:20:39 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37e0389f87abc858cef1a365e6b548d7d7762be571608840bc715ef352c41084`  
		Last Modified: Fri, 10 Sep 2021 00:20:39 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.5.0-windowsservercore-1809`

```console
$ docker pull nats@sha256:4e912b79015d0859d5b6c675d055f80bd7628c8e368d96466b6ab6d9c7a51f7b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2114; amd64

### `nats:2.5.0-windowsservercore-1809` - windows version 10.0.17763.2114; amd64

```console
$ docker pull nats@sha256:ea5bd03ca8c905a9bb8df9bcefe1c70aada9fce64c82d90932dfaf570332087a
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2691339003 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce14639524af68868fed35dda40295ffe16c35eb58b5038f43989d7d60f7059d`
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
# Fri, 10 Sep 2021 00:14:04 GMT
ENV NATS_SERVER=2.5.0
# Fri, 10 Sep 2021 00:14:05 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.5.0/nats-server-v2.5.0-windows-amd64.zip
# Fri, 10 Sep 2021 00:14:06 GMT
ENV NATS_SERVER_SHASUM=0eae96ad4555f5060b0b6325ba972566b404cd8930b3168b9c0ffe911d15c5d8
# Fri, 10 Sep 2021 00:15:08 GMT
RUN Set-PSDebug -Trace 2
# Fri, 10 Sep 2021 00:16:32 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 10 Sep 2021 00:16:33 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 10 Sep 2021 00:16:34 GMT
EXPOSE 4222 6222 8222
# Fri, 10 Sep 2021 00:16:34 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 10 Sep 2021 00:16:35 GMT
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
	-	`sha256:4c32056c4535002b64e42d1424edb3a7ac778c308d2d9109f33d738d59c85454`  
		Last Modified: Fri, 10 Sep 2021 00:20:02 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb115761571c4ba7b8b719d8ee1587c8898f7e13246d1a92ee2283c0f929a1b1`  
		Last Modified: Fri, 10 Sep 2021 00:20:01 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd93d02cef774a55aa7c6f566b3b5718436cbdae64582cc888ef3b1efe452735`  
		Last Modified: Fri, 10 Sep 2021 00:20:01 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f28336574033153776b7149c4d079b46a95608a291563bc581fc8b029d9399c`  
		Last Modified: Fri, 10 Sep 2021 00:20:02 GMT  
		Size: 372.4 KB (372418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcce3c7fbad71cacb4533bac881f55d312123c387549ca7840f402aa108fb59d`  
		Last Modified: Fri, 10 Sep 2021 00:20:05 GMT  
		Size: 5.0 MB (4955556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0d387c2eda58f8b5f8c3889645ec5e1a977b681cb17de77c04de1c643341b18`  
		Last Modified: Fri, 10 Sep 2021 00:19:59 GMT  
		Size: 1.9 KB (1944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f70bbbc8ecda378ae0099ea8e49350ba7d78be681cd5defc71e6f624abca5d7`  
		Last Modified: Fri, 10 Sep 2021 00:19:59 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76b0025f319f789e7c26483abcf5ca7944dc5a1f0a071023d2415526aa310d40`  
		Last Modified: Fri, 10 Sep 2021 00:19:59 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99ff7344cf8ed7957719594d8f9fe4d78b0ef7acc3755bb1962febcf166ac4ce`  
		Last Modified: Fri, 10 Sep 2021 00:19:59 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.5.0-windowsservercore-ltsc2016`

```console
$ docker pull nats@sha256:521575d35d4f87b16aa1482f712733b1273962ba4f75353d07327cfc4e324cee
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.14393.4583; amd64

### `nats:2.5.0-windowsservercore-ltsc2016` - windows version 10.0.14393.4583; amd64

```console
$ docker pull nats@sha256:7f318bb6bf586d9b74b6b8e8097ffabf3b4d16c43c5b9b2dd62d532713aa0305
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6276274196 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5716654340a54076fb48e8d797d45b91a2e56551a534fb6d800d7d6c61262257`
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
# Fri, 10 Sep 2021 00:16:55 GMT
ENV NATS_SERVER=2.5.0
# Fri, 10 Sep 2021 00:16:56 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.5.0/nats-server-v2.5.0-windows-amd64.zip
# Fri, 10 Sep 2021 00:16:57 GMT
ENV NATS_SERVER_SHASUM=0eae96ad4555f5060b0b6325ba972566b404cd8930b3168b9c0ffe911d15c5d8
# Fri, 10 Sep 2021 00:17:43 GMT
RUN Set-PSDebug -Trace 2
# Fri, 10 Sep 2021 00:19:14 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 10 Sep 2021 00:19:15 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 10 Sep 2021 00:19:16 GMT
EXPOSE 4222 6222 8222
# Fri, 10 Sep 2021 00:19:17 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 10 Sep 2021 00:19:18 GMT
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
	-	`sha256:786675b79153c67ad039b6b8a55171a8167b2ff8c8186ccb7c5cab0b01f47767`  
		Last Modified: Fri, 10 Sep 2021 00:20:42 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65445b8a1c334a2efce7d34289af9fa682427cba808180c96ce46f39f765e9b5`  
		Last Modified: Fri, 10 Sep 2021 00:20:42 GMT  
		Size: 1.4 KB (1358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08647f69046830b98e59118ace63049f027ad1786cc2aaad037990a4e7a87344`  
		Last Modified: Fri, 10 Sep 2021 00:20:42 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b50cf5c744e8952689c263dbc9800bbe4a032fb4c8df3c8e5028092bdb2a5c9c`  
		Last Modified: Fri, 10 Sep 2021 00:20:42 GMT  
		Size: 338.0 KB (337964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:459c701464a835b4d39cc3183fff454248a3045bb433c26b0430f06e91acf1bb`  
		Last Modified: Fri, 10 Sep 2021 00:20:41 GMT  
		Size: 5.0 MB (4957179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cb2fb143896bcefca1d8ad8640f3146b771f5b284f01be2b849a048d9ac9eeb`  
		Last Modified: Fri, 10 Sep 2021 00:20:40 GMT  
		Size: 1.9 KB (1938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d9f7d515a8e73d005392fc0bccc42761025b86ab370cffe210a552fe53d1cbe`  
		Last Modified: Fri, 10 Sep 2021 00:20:40 GMT  
		Size: 1.4 KB (1380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d68902a6dec2675ab57a60716c10ce8a85e58fe54d7abea307bc340452e882a`  
		Last Modified: Fri, 10 Sep 2021 00:20:39 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37e0389f87abc858cef1a365e6b548d7d7762be571608840bc715ef352c41084`  
		Last Modified: Fri, 10 Sep 2021 00:20:39 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:alpine`

```console
$ docker pull nats@sha256:52a8fe18f5c85cdd5cf0304eadb4e4a6a4208db9183fabc36140ff9ed7a813a3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:alpine` - linux; amd64

```console
$ docker pull nats@sha256:f6b2376c122defe213696fdbf87c7f365bdbbd60a6068fe88b1ab8aee27987d2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7647076 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b59fdb5895884cf160a5cabba5411b4a328b11aa2798042d794fe41e69fe8165`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 10 Sep 2021 00:20:12 GMT
ENV NATS_SERVER=2.5.0
# Fri, 10 Sep 2021 00:20:15 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='93f64cd14f04b4e7f6c3a2c10d09888be653406b7bc1a41f399ae44746388a5c' ;; 		armhf) natsArch='arm6'; sha256='12f38f6881cdcf27c0faebb7ab6580b40253c36dc1531d499a29c4998a009494' ;; 		armv7) natsArch='arm7'; sha256='fb3611b57a932f5c75310dee66597057ab65b442eb84d73b2c5fd9389eb6e518' ;; 		x86_64) natsArch='amd64'; sha256='4d2f4abb15b45618ce772659c9f3eca60f25266dfc976f0354430ad67c8fd886' ;; 		x86) natsArch='386'; sha256='776aecc77c33146d88e6b3cb1787097f9817122182f49f7243c0ea3fd62ad029' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 10 Sep 2021 00:20:15 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 10 Sep 2021 00:20:15 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 10 Sep 2021 00:20:15 GMT
EXPOSE 4222 6222 8222
# Fri, 10 Sep 2021 00:20:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 10 Sep 2021 00:20:16 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59a9809baa02715a6c4ccdb1ebc94edaf948058be9f97cea623426ca670b426e`  
		Last Modified: Fri, 10 Sep 2021 00:21:08 GMT  
		Size: 4.8 MB (4831663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68c0794b9b379d130866e40babeef9f4557514bcc2c88194e89b90081ef7ad12`  
		Last Modified: Fri, 10 Sep 2021 00:21:08 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:240551b5739b209d882cd7b4f76138b9188aac1a497ff32a469526302056dd98`  
		Last Modified: Fri, 10 Sep 2021 00:21:07 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:c516621cb4dc61ad9db1927cdcec7210328be6d7b813acb688016584d61be212
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7121422 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c48580010dc9af32e7a019914f078134ae513ef77280b7877fe7fd47665426b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:49:29 GMT
ADD file:1c1c4520d49cb6e8f795f3b953d1ed3c3c77868b98b53a455169c254fcec5acd in / 
# Fri, 27 Aug 2021 17:49:30 GMT
CMD ["/bin/sh"]
# Thu, 09 Sep 2021 23:49:46 GMT
ENV NATS_SERVER=2.5.0
# Thu, 09 Sep 2021 23:49:51 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='93f64cd14f04b4e7f6c3a2c10d09888be653406b7bc1a41f399ae44746388a5c' ;; 		armhf) natsArch='arm6'; sha256='12f38f6881cdcf27c0faebb7ab6580b40253c36dc1531d499a29c4998a009494' ;; 		armv7) natsArch='arm7'; sha256='fb3611b57a932f5c75310dee66597057ab65b442eb84d73b2c5fd9389eb6e518' ;; 		x86_64) natsArch='amd64'; sha256='4d2f4abb15b45618ce772659c9f3eca60f25266dfc976f0354430ad67c8fd886' ;; 		x86) natsArch='386'; sha256='776aecc77c33146d88e6b3cb1787097f9817122182f49f7243c0ea3fd62ad029' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 09 Sep 2021 23:49:51 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 09 Sep 2021 23:49:52 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 09 Sep 2021 23:49:52 GMT
EXPOSE 4222 6222 8222
# Thu, 09 Sep 2021 23:49:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 09 Sep 2021 23:49:53 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:2e78c0f86ba9a1fed30df20cb48c9cc73e9626399f12749d36b892ff99c0ecf5`  
		Last Modified: Fri, 27 Aug 2021 17:50:55 GMT  
		Size: 2.6 MB (2627447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75b214a44f07577985e2f01798e9acf02be903c28022f74d244b22418b31e815`  
		Last Modified: Thu, 09 Sep 2021 23:52:03 GMT  
		Size: 4.5 MB (4493006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d232ac6d6c1f822be800be02acbb341f7abe35b05bd13a0857df02fd1cc600a6`  
		Last Modified: Thu, 09 Sep 2021 23:52:01 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e364400828db299d750b3bcc80b1e3b1df2f7abe62c5d6293f3c7e22d93e20a`  
		Last Modified: Thu, 09 Sep 2021 23:52:00 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:c5a16f99958e4ae6f318a577619242a7d168fc47e07883d8adbc1701faa36ab4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.9 MB (6918058 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b6128ceec7a63c74e316f6b3bda400e98def18ed14e046a0177a1095946dd8e2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:57:31 GMT
ADD file:a7da7992ccea54d3295231027614f138aa45c4d4a25ea6ec9bf7b316b9f67d95 in / 
# Fri, 27 Aug 2021 17:57:32 GMT
CMD ["/bin/sh"]
# Fri, 10 Sep 2021 00:58:26 GMT
ENV NATS_SERVER=2.5.0
# Fri, 10 Sep 2021 00:58:31 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='93f64cd14f04b4e7f6c3a2c10d09888be653406b7bc1a41f399ae44746388a5c' ;; 		armhf) natsArch='arm6'; sha256='12f38f6881cdcf27c0faebb7ab6580b40253c36dc1531d499a29c4998a009494' ;; 		armv7) natsArch='arm7'; sha256='fb3611b57a932f5c75310dee66597057ab65b442eb84d73b2c5fd9389eb6e518' ;; 		x86_64) natsArch='amd64'; sha256='4d2f4abb15b45618ce772659c9f3eca60f25266dfc976f0354430ad67c8fd886' ;; 		x86) natsArch='386'; sha256='776aecc77c33146d88e6b3cb1787097f9817122182f49f7243c0ea3fd62ad029' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 10 Sep 2021 00:58:32 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 10 Sep 2021 00:58:32 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 10 Sep 2021 00:58:33 GMT
EXPOSE 4222 6222 8222
# Fri, 10 Sep 2021 00:58:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 10 Sep 2021 00:58:34 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:a14774a5a62e0f454febaec7cb603e18a6a8e25ef9da4a4da85b155bdd5e5a7a`  
		Last Modified: Fri, 27 Aug 2021 17:59:00 GMT  
		Size: 2.4 MB (2430419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2edd63df5776202ac2717836b8350736f3e046021c53b49e6e872ef9f4a960a9`  
		Last Modified: Fri, 10 Sep 2021 01:00:49 GMT  
		Size: 4.5 MB (4486667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d073c5b9595fcde55c46ccb0f54148caba30c630427ffcdfe9f03a4e84be10ec`  
		Last Modified: Fri, 10 Sep 2021 01:00:46 GMT  
		Size: 559.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15f66a2a44784b8ce7529a34b470376f9a52740980b2b05baf8525ec5f4a39f2`  
		Last Modified: Fri, 10 Sep 2021 01:00:46 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:88b4d8f2f54f207d5400e8d3e9037d55ca8d2969b126e07d833c6d3464f93300
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7156798 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f803b2b0ed9b56df4cac8c3a03dfd789e480a622c1f3a282ecee5fd0f937d9e5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Thu, 09 Sep 2021 23:40:02 GMT
ENV NATS_SERVER=2.5.0
# Thu, 09 Sep 2021 23:40:05 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='93f64cd14f04b4e7f6c3a2c10d09888be653406b7bc1a41f399ae44746388a5c' ;; 		armhf) natsArch='arm6'; sha256='12f38f6881cdcf27c0faebb7ab6580b40253c36dc1531d499a29c4998a009494' ;; 		armv7) natsArch='arm7'; sha256='fb3611b57a932f5c75310dee66597057ab65b442eb84d73b2c5fd9389eb6e518' ;; 		x86_64) natsArch='amd64'; sha256='4d2f4abb15b45618ce772659c9f3eca60f25266dfc976f0354430ad67c8fd886' ;; 		x86) natsArch='386'; sha256='776aecc77c33146d88e6b3cb1787097f9817122182f49f7243c0ea3fd62ad029' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 09 Sep 2021 23:40:05 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 09 Sep 2021 23:40:05 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 09 Sep 2021 23:40:05 GMT
EXPOSE 4222 6222 8222
# Thu, 09 Sep 2021 23:40:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 09 Sep 2021 23:40:06 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:552d1f2373af9bfe12033568ebbfb0ccbb0de11279f9a415a29207e264d7f4d9`  
		Last Modified: Fri, 27 Aug 2021 17:40:18 GMT  
		Size: 2.7 MB (2711827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49450e2f2462d1e207a865d4a084154f6a3c5edc2b3b4954d34d4e1ce75d38f2`  
		Last Modified: Thu, 09 Sep 2021 23:41:18 GMT  
		Size: 4.4 MB (4444005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edeb0b05b16add9a16e4a8bc8c1eced6c1f60f58ac669216dbbf93cb9bce40d2`  
		Last Modified: Thu, 09 Sep 2021 23:41:18 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67be552e94a6cfc686543e5bfa0c1a6bca72bc9dce939fb9f3e43c4a77f5e6e3`  
		Last Modified: Thu, 09 Sep 2021 23:41:18 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:alpine3.14`

```console
$ docker pull nats@sha256:52a8fe18f5c85cdd5cf0304eadb4e4a6a4208db9183fabc36140ff9ed7a813a3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:alpine3.14` - linux; amd64

```console
$ docker pull nats@sha256:f6b2376c122defe213696fdbf87c7f365bdbbd60a6068fe88b1ab8aee27987d2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7647076 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b59fdb5895884cf160a5cabba5411b4a328b11aa2798042d794fe41e69fe8165`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 10 Sep 2021 00:20:12 GMT
ENV NATS_SERVER=2.5.0
# Fri, 10 Sep 2021 00:20:15 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='93f64cd14f04b4e7f6c3a2c10d09888be653406b7bc1a41f399ae44746388a5c' ;; 		armhf) natsArch='arm6'; sha256='12f38f6881cdcf27c0faebb7ab6580b40253c36dc1531d499a29c4998a009494' ;; 		armv7) natsArch='arm7'; sha256='fb3611b57a932f5c75310dee66597057ab65b442eb84d73b2c5fd9389eb6e518' ;; 		x86_64) natsArch='amd64'; sha256='4d2f4abb15b45618ce772659c9f3eca60f25266dfc976f0354430ad67c8fd886' ;; 		x86) natsArch='386'; sha256='776aecc77c33146d88e6b3cb1787097f9817122182f49f7243c0ea3fd62ad029' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 10 Sep 2021 00:20:15 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 10 Sep 2021 00:20:15 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 10 Sep 2021 00:20:15 GMT
EXPOSE 4222 6222 8222
# Fri, 10 Sep 2021 00:20:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 10 Sep 2021 00:20:16 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59a9809baa02715a6c4ccdb1ebc94edaf948058be9f97cea623426ca670b426e`  
		Last Modified: Fri, 10 Sep 2021 00:21:08 GMT  
		Size: 4.8 MB (4831663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68c0794b9b379d130866e40babeef9f4557514bcc2c88194e89b90081ef7ad12`  
		Last Modified: Fri, 10 Sep 2021 00:21:08 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:240551b5739b209d882cd7b4f76138b9188aac1a497ff32a469526302056dd98`  
		Last Modified: Fri, 10 Sep 2021 00:21:07 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.14` - linux; arm variant v6

```console
$ docker pull nats@sha256:c516621cb4dc61ad9db1927cdcec7210328be6d7b813acb688016584d61be212
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7121422 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c48580010dc9af32e7a019914f078134ae513ef77280b7877fe7fd47665426b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:49:29 GMT
ADD file:1c1c4520d49cb6e8f795f3b953d1ed3c3c77868b98b53a455169c254fcec5acd in / 
# Fri, 27 Aug 2021 17:49:30 GMT
CMD ["/bin/sh"]
# Thu, 09 Sep 2021 23:49:46 GMT
ENV NATS_SERVER=2.5.0
# Thu, 09 Sep 2021 23:49:51 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='93f64cd14f04b4e7f6c3a2c10d09888be653406b7bc1a41f399ae44746388a5c' ;; 		armhf) natsArch='arm6'; sha256='12f38f6881cdcf27c0faebb7ab6580b40253c36dc1531d499a29c4998a009494' ;; 		armv7) natsArch='arm7'; sha256='fb3611b57a932f5c75310dee66597057ab65b442eb84d73b2c5fd9389eb6e518' ;; 		x86_64) natsArch='amd64'; sha256='4d2f4abb15b45618ce772659c9f3eca60f25266dfc976f0354430ad67c8fd886' ;; 		x86) natsArch='386'; sha256='776aecc77c33146d88e6b3cb1787097f9817122182f49f7243c0ea3fd62ad029' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 09 Sep 2021 23:49:51 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 09 Sep 2021 23:49:52 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 09 Sep 2021 23:49:52 GMT
EXPOSE 4222 6222 8222
# Thu, 09 Sep 2021 23:49:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 09 Sep 2021 23:49:53 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:2e78c0f86ba9a1fed30df20cb48c9cc73e9626399f12749d36b892ff99c0ecf5`  
		Last Modified: Fri, 27 Aug 2021 17:50:55 GMT  
		Size: 2.6 MB (2627447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75b214a44f07577985e2f01798e9acf02be903c28022f74d244b22418b31e815`  
		Last Modified: Thu, 09 Sep 2021 23:52:03 GMT  
		Size: 4.5 MB (4493006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d232ac6d6c1f822be800be02acbb341f7abe35b05bd13a0857df02fd1cc600a6`  
		Last Modified: Thu, 09 Sep 2021 23:52:01 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e364400828db299d750b3bcc80b1e3b1df2f7abe62c5d6293f3c7e22d93e20a`  
		Last Modified: Thu, 09 Sep 2021 23:52:00 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.14` - linux; arm variant v7

```console
$ docker pull nats@sha256:c5a16f99958e4ae6f318a577619242a7d168fc47e07883d8adbc1701faa36ab4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.9 MB (6918058 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b6128ceec7a63c74e316f6b3bda400e98def18ed14e046a0177a1095946dd8e2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:57:31 GMT
ADD file:a7da7992ccea54d3295231027614f138aa45c4d4a25ea6ec9bf7b316b9f67d95 in / 
# Fri, 27 Aug 2021 17:57:32 GMT
CMD ["/bin/sh"]
# Fri, 10 Sep 2021 00:58:26 GMT
ENV NATS_SERVER=2.5.0
# Fri, 10 Sep 2021 00:58:31 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='93f64cd14f04b4e7f6c3a2c10d09888be653406b7bc1a41f399ae44746388a5c' ;; 		armhf) natsArch='arm6'; sha256='12f38f6881cdcf27c0faebb7ab6580b40253c36dc1531d499a29c4998a009494' ;; 		armv7) natsArch='arm7'; sha256='fb3611b57a932f5c75310dee66597057ab65b442eb84d73b2c5fd9389eb6e518' ;; 		x86_64) natsArch='amd64'; sha256='4d2f4abb15b45618ce772659c9f3eca60f25266dfc976f0354430ad67c8fd886' ;; 		x86) natsArch='386'; sha256='776aecc77c33146d88e6b3cb1787097f9817122182f49f7243c0ea3fd62ad029' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 10 Sep 2021 00:58:32 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 10 Sep 2021 00:58:32 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 10 Sep 2021 00:58:33 GMT
EXPOSE 4222 6222 8222
# Fri, 10 Sep 2021 00:58:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 10 Sep 2021 00:58:34 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:a14774a5a62e0f454febaec7cb603e18a6a8e25ef9da4a4da85b155bdd5e5a7a`  
		Last Modified: Fri, 27 Aug 2021 17:59:00 GMT  
		Size: 2.4 MB (2430419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2edd63df5776202ac2717836b8350736f3e046021c53b49e6e872ef9f4a960a9`  
		Last Modified: Fri, 10 Sep 2021 01:00:49 GMT  
		Size: 4.5 MB (4486667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d073c5b9595fcde55c46ccb0f54148caba30c630427ffcdfe9f03a4e84be10ec`  
		Last Modified: Fri, 10 Sep 2021 01:00:46 GMT  
		Size: 559.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15f66a2a44784b8ce7529a34b470376f9a52740980b2b05baf8525ec5f4a39f2`  
		Last Modified: Fri, 10 Sep 2021 01:00:46 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.14` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:88b4d8f2f54f207d5400e8d3e9037d55ca8d2969b126e07d833c6d3464f93300
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7156798 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f803b2b0ed9b56df4cac8c3a03dfd789e480a622c1f3a282ecee5fd0f937d9e5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Thu, 09 Sep 2021 23:40:02 GMT
ENV NATS_SERVER=2.5.0
# Thu, 09 Sep 2021 23:40:05 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='93f64cd14f04b4e7f6c3a2c10d09888be653406b7bc1a41f399ae44746388a5c' ;; 		armhf) natsArch='arm6'; sha256='12f38f6881cdcf27c0faebb7ab6580b40253c36dc1531d499a29c4998a009494' ;; 		armv7) natsArch='arm7'; sha256='fb3611b57a932f5c75310dee66597057ab65b442eb84d73b2c5fd9389eb6e518' ;; 		x86_64) natsArch='amd64'; sha256='4d2f4abb15b45618ce772659c9f3eca60f25266dfc976f0354430ad67c8fd886' ;; 		x86) natsArch='386'; sha256='776aecc77c33146d88e6b3cb1787097f9817122182f49f7243c0ea3fd62ad029' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 09 Sep 2021 23:40:05 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 09 Sep 2021 23:40:05 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 09 Sep 2021 23:40:05 GMT
EXPOSE 4222 6222 8222
# Thu, 09 Sep 2021 23:40:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 09 Sep 2021 23:40:06 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:552d1f2373af9bfe12033568ebbfb0ccbb0de11279f9a415a29207e264d7f4d9`  
		Last Modified: Fri, 27 Aug 2021 17:40:18 GMT  
		Size: 2.7 MB (2711827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49450e2f2462d1e207a865d4a084154f6a3c5edc2b3b4954d34d4e1ce75d38f2`  
		Last Modified: Thu, 09 Sep 2021 23:41:18 GMT  
		Size: 4.4 MB (4444005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edeb0b05b16add9a16e4a8bc8c1eced6c1f60f58ac669216dbbf93cb9bce40d2`  
		Last Modified: Thu, 09 Sep 2021 23:41:18 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67be552e94a6cfc686543e5bfa0c1a6bca72bc9dce939fb9f3e43c4a77f5e6e3`  
		Last Modified: Thu, 09 Sep 2021 23:41:18 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:latest`

```console
$ docker pull nats@sha256:c812e8c75705b49bfc4694743b59428590372ff6689425c86ea3ddd682fd8c58
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
$ docker pull nats@sha256:01dbe57fde6a40eecbd53edc6a418f3c9b1ddd85f03dd17e73ecef98a3b15318
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4546051 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80fcdf2bfe0f4a11267c9e8d06e5e52dce7dd9b41267e1a51d5e9df22c76bf9c`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 10 Sep 2021 00:20:41 GMT
COPY file:0b180121e1ef70970b020901a4b61990a8673ac9db99b94c348c5321333884ea in /nats-server 
# Fri, 10 Sep 2021 00:20:41 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 10 Sep 2021 00:20:41 GMT
EXPOSE 4222 6222 8222
# Fri, 10 Sep 2021 00:20:41 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 10 Sep 2021 00:20:42 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:9cee557b7d3312d12996f8c4338bf9ea02657256657ef77d46510c729d9be195`  
		Last Modified: Fri, 10 Sep 2021 00:21:32 GMT  
		Size: 4.5 MB (4545577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb24b942a0d168497adac7ad3190098a6f8dfa34ad2ef37932150fbce9336c9a`  
		Last Modified: Fri, 10 Sep 2021 00:21:31 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm variant v6

```console
$ docker pull nats@sha256:b21057f1f945b501d03cf3c5c2d530f7961e1a3198e00bb297b7f69a849cc0e9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4210290 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:865dcd8a77138e8339293c7089adeee440305e68331df5533186ea36b8132f84`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 09 Sep 2021 23:50:15 GMT
COPY file:a60049eef2da0cbda1255e229e5e5c6377e3c3445b0cd16ce13a272139c7ce85 in /nats-server 
# Thu, 09 Sep 2021 23:50:16 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 09 Sep 2021 23:50:17 GMT
EXPOSE 4222 6222 8222
# Thu, 09 Sep 2021 23:50:17 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 09 Sep 2021 23:50:18 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b95232e9c9c31dfba5a6124fb74b4abc750a3fd6d5f89a13438a0b051430299e`  
		Last Modified: Thu, 09 Sep 2021 23:52:42 GMT  
		Size: 4.2 MB (4209813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2c01128246ad2a36efed9386a5ed63a01f73f3f56e54d059834ac17a2f64a48`  
		Last Modified: Thu, 09 Sep 2021 23:52:38 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm variant v7

```console
$ docker pull nats@sha256:aafbb0b5e1b7412f9d0e71ddd6c3948c7080697882dd40ae20578b855ca40c1f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4206272 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:79f5a4fb5f9254997b2d7e573f24316740a167eb829bb23952ba05ff8304ddc1`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 10 Sep 2021 00:59:05 GMT
COPY file:7043dd814cd92048127f9905d58e9204d2968d9c03bbb7feba592c45a87e9963 in /nats-server 
# Fri, 10 Sep 2021 00:59:06 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 10 Sep 2021 00:59:06 GMT
EXPOSE 4222 6222 8222
# Fri, 10 Sep 2021 00:59:07 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 10 Sep 2021 00:59:07 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:8ae70a7ddee0b3bc3819ff86ee31d3295a37b10282b7ee0d14d3dd3c8dcb16c7`  
		Last Modified: Fri, 10 Sep 2021 01:01:28 GMT  
		Size: 4.2 MB (4205795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbbfbfa45875dc8bff20ba3a989407cf3ab8018f98f4277411dd068510c071c6`  
		Last Modified: Fri, 10 Sep 2021 01:01:25 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:24f192937e7bc371f7c2631055e49a51d489659d28f55b4fdf2eb5a19843a5ae
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4158958 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2cd8bb7e96599c9badd4424f86ef2d5f8561cfa0c4a4322057847c002da643a9`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 09 Sep 2021 23:40:25 GMT
COPY file:eda8ae8779fbfb7d34c95bc93fc8ce409cbd298cb302284f61ee4ebf6ac10b0e in /nats-server 
# Thu, 09 Sep 2021 23:40:26 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 09 Sep 2021 23:40:26 GMT
EXPOSE 4222 6222 8222
# Thu, 09 Sep 2021 23:40:26 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 09 Sep 2021 23:40:26 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:0c0083faeb4bd1e89eefb7cbc2a5556eb056acaba6107a833c271a1ca7cd8633`  
		Last Modified: Thu, 09 Sep 2021 23:41:48 GMT  
		Size: 4.2 MB (4158481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4227e148c1053ae9735f2dcc2ab35b83566aab7b85aa3d50395ec15be4630e26`  
		Last Modified: Thu, 09 Sep 2021 23:41:47 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - windows version 10.0.17763.2114; amd64

```console
$ docker pull nats@sha256:da56a6dd1f9556f706d9086ed48947ac745a5b9dd1e3bc0d988581858828c23c
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.4 MB (107351558 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:780da6fbe38cee622e2d2e69123219af601b417dada779a198cef0514370203e`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 05 Aug 2021 19:15:20 GMT
RUN Apply image 1809-amd64
# Wed, 25 Aug 2021 16:07:56 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 10 Sep 2021 00:16:45 GMT
RUN cmd /S /C #(nop) COPY file:13fac1899b72f2f26df9bd8ce320e46a5f7736306d7abf82ea7d657c16444fb9 in C:\nats-server.exe 
# Fri, 10 Sep 2021 00:16:46 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 10 Sep 2021 00:16:47 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Fri, 10 Sep 2021 00:16:47 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 10 Sep 2021 00:16:48 GMT
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
	-	`sha256:55bd340c78387be49377457ea8e39875e7be9b3799bdac42ff35c749d67b3940`  
		Last Modified: Fri, 10 Sep 2021 00:20:25 GMT  
		Size: 4.6 MB (4604102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76e6782c003b15abdb2161dc360ffef0eeb967b34fc78186d8d6085aacfc85fa`  
		Last Modified: Fri, 10 Sep 2021 00:20:20 GMT  
		Size: 1.8 KB (1777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf24d35e2c525beccaa7b227eda13492b401302f8ecc528e2a35118220e3f760`  
		Last Modified: Fri, 10 Sep 2021 00:20:20 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71603cdad9bbdd669dd86cda1c010a6f91d1a58de21eac052a29279f77bd247f`  
		Last Modified: Fri, 10 Sep 2021 00:20:20 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01477f3ed16729139c6a0a856de33336e03c4fb127df26c6e42b8157eaf1801b`  
		Last Modified: Fri, 10 Sep 2021 00:20:20 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:linux`

```console
$ docker pull nats@sha256:6808dfb3132c301916bbeb4241ae1f3c0be5dca763a6c0be6180ca1bd6da298a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:linux` - linux; amd64

```console
$ docker pull nats@sha256:01dbe57fde6a40eecbd53edc6a418f3c9b1ddd85f03dd17e73ecef98a3b15318
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4546051 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80fcdf2bfe0f4a11267c9e8d06e5e52dce7dd9b41267e1a51d5e9df22c76bf9c`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 10 Sep 2021 00:20:41 GMT
COPY file:0b180121e1ef70970b020901a4b61990a8673ac9db99b94c348c5321333884ea in /nats-server 
# Fri, 10 Sep 2021 00:20:41 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 10 Sep 2021 00:20:41 GMT
EXPOSE 4222 6222 8222
# Fri, 10 Sep 2021 00:20:41 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 10 Sep 2021 00:20:42 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:9cee557b7d3312d12996f8c4338bf9ea02657256657ef77d46510c729d9be195`  
		Last Modified: Fri, 10 Sep 2021 00:21:32 GMT  
		Size: 4.5 MB (4545577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb24b942a0d168497adac7ad3190098a6f8dfa34ad2ef37932150fbce9336c9a`  
		Last Modified: Fri, 10 Sep 2021 00:21:31 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:b21057f1f945b501d03cf3c5c2d530f7961e1a3198e00bb297b7f69a849cc0e9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4210290 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:865dcd8a77138e8339293c7089adeee440305e68331df5533186ea36b8132f84`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 09 Sep 2021 23:50:15 GMT
COPY file:a60049eef2da0cbda1255e229e5e5c6377e3c3445b0cd16ce13a272139c7ce85 in /nats-server 
# Thu, 09 Sep 2021 23:50:16 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 09 Sep 2021 23:50:17 GMT
EXPOSE 4222 6222 8222
# Thu, 09 Sep 2021 23:50:17 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 09 Sep 2021 23:50:18 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b95232e9c9c31dfba5a6124fb74b4abc750a3fd6d5f89a13438a0b051430299e`  
		Last Modified: Thu, 09 Sep 2021 23:52:42 GMT  
		Size: 4.2 MB (4209813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2c01128246ad2a36efed9386a5ed63a01f73f3f56e54d059834ac17a2f64a48`  
		Last Modified: Thu, 09 Sep 2021 23:52:38 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:aafbb0b5e1b7412f9d0e71ddd6c3948c7080697882dd40ae20578b855ca40c1f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4206272 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:79f5a4fb5f9254997b2d7e573f24316740a167eb829bb23952ba05ff8304ddc1`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 10 Sep 2021 00:59:05 GMT
COPY file:7043dd814cd92048127f9905d58e9204d2968d9c03bbb7feba592c45a87e9963 in /nats-server 
# Fri, 10 Sep 2021 00:59:06 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 10 Sep 2021 00:59:06 GMT
EXPOSE 4222 6222 8222
# Fri, 10 Sep 2021 00:59:07 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 10 Sep 2021 00:59:07 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:8ae70a7ddee0b3bc3819ff86ee31d3295a37b10282b7ee0d14d3dd3c8dcb16c7`  
		Last Modified: Fri, 10 Sep 2021 01:01:28 GMT  
		Size: 4.2 MB (4205795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbbfbfa45875dc8bff20ba3a989407cf3ab8018f98f4277411dd068510c071c6`  
		Last Modified: Fri, 10 Sep 2021 01:01:25 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:24f192937e7bc371f7c2631055e49a51d489659d28f55b4fdf2eb5a19843a5ae
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4158958 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2cd8bb7e96599c9badd4424f86ef2d5f8561cfa0c4a4322057847c002da643a9`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 09 Sep 2021 23:40:25 GMT
COPY file:eda8ae8779fbfb7d34c95bc93fc8ce409cbd298cb302284f61ee4ebf6ac10b0e in /nats-server 
# Thu, 09 Sep 2021 23:40:26 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 09 Sep 2021 23:40:26 GMT
EXPOSE 4222 6222 8222
# Thu, 09 Sep 2021 23:40:26 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 09 Sep 2021 23:40:26 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:0c0083faeb4bd1e89eefb7cbc2a5556eb056acaba6107a833c271a1ca7cd8633`  
		Last Modified: Thu, 09 Sep 2021 23:41:48 GMT  
		Size: 4.2 MB (4158481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4227e148c1053ae9735f2dcc2ab35b83566aab7b85aa3d50395ec15be4630e26`  
		Last Modified: Thu, 09 Sep 2021 23:41:47 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:nanoserver`

```console
$ docker pull nats@sha256:5b8ea050ee708eb4017db4e1cb913456e468e82c227eb67a070974651446cfd9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2114; amd64

### `nats:nanoserver` - windows version 10.0.17763.2114; amd64

```console
$ docker pull nats@sha256:da56a6dd1f9556f706d9086ed48947ac745a5b9dd1e3bc0d988581858828c23c
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.4 MB (107351558 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:780da6fbe38cee622e2d2e69123219af601b417dada779a198cef0514370203e`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 05 Aug 2021 19:15:20 GMT
RUN Apply image 1809-amd64
# Wed, 25 Aug 2021 16:07:56 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 10 Sep 2021 00:16:45 GMT
RUN cmd /S /C #(nop) COPY file:13fac1899b72f2f26df9bd8ce320e46a5f7736306d7abf82ea7d657c16444fb9 in C:\nats-server.exe 
# Fri, 10 Sep 2021 00:16:46 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 10 Sep 2021 00:16:47 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Fri, 10 Sep 2021 00:16:47 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 10 Sep 2021 00:16:48 GMT
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
	-	`sha256:55bd340c78387be49377457ea8e39875e7be9b3799bdac42ff35c749d67b3940`  
		Last Modified: Fri, 10 Sep 2021 00:20:25 GMT  
		Size: 4.6 MB (4604102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76e6782c003b15abdb2161dc360ffef0eeb967b34fc78186d8d6085aacfc85fa`  
		Last Modified: Fri, 10 Sep 2021 00:20:20 GMT  
		Size: 1.8 KB (1777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf24d35e2c525beccaa7b227eda13492b401302f8ecc528e2a35118220e3f760`  
		Last Modified: Fri, 10 Sep 2021 00:20:20 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71603cdad9bbdd669dd86cda1c010a6f91d1a58de21eac052a29279f77bd247f`  
		Last Modified: Fri, 10 Sep 2021 00:20:20 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01477f3ed16729139c6a0a856de33336e03c4fb127df26c6e42b8157eaf1801b`  
		Last Modified: Fri, 10 Sep 2021 00:20:20 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:nanoserver-1809`

```console
$ docker pull nats@sha256:5b8ea050ee708eb4017db4e1cb913456e468e82c227eb67a070974651446cfd9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2114; amd64

### `nats:nanoserver-1809` - windows version 10.0.17763.2114; amd64

```console
$ docker pull nats@sha256:da56a6dd1f9556f706d9086ed48947ac745a5b9dd1e3bc0d988581858828c23c
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.4 MB (107351558 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:780da6fbe38cee622e2d2e69123219af601b417dada779a198cef0514370203e`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 05 Aug 2021 19:15:20 GMT
RUN Apply image 1809-amd64
# Wed, 25 Aug 2021 16:07:56 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 10 Sep 2021 00:16:45 GMT
RUN cmd /S /C #(nop) COPY file:13fac1899b72f2f26df9bd8ce320e46a5f7736306d7abf82ea7d657c16444fb9 in C:\nats-server.exe 
# Fri, 10 Sep 2021 00:16:46 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 10 Sep 2021 00:16:47 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Fri, 10 Sep 2021 00:16:47 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 10 Sep 2021 00:16:48 GMT
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
	-	`sha256:55bd340c78387be49377457ea8e39875e7be9b3799bdac42ff35c749d67b3940`  
		Last Modified: Fri, 10 Sep 2021 00:20:25 GMT  
		Size: 4.6 MB (4604102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76e6782c003b15abdb2161dc360ffef0eeb967b34fc78186d8d6085aacfc85fa`  
		Last Modified: Fri, 10 Sep 2021 00:20:20 GMT  
		Size: 1.8 KB (1777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf24d35e2c525beccaa7b227eda13492b401302f8ecc528e2a35118220e3f760`  
		Last Modified: Fri, 10 Sep 2021 00:20:20 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71603cdad9bbdd669dd86cda1c010a6f91d1a58de21eac052a29279f77bd247f`  
		Last Modified: Fri, 10 Sep 2021 00:20:20 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01477f3ed16729139c6a0a856de33336e03c4fb127df26c6e42b8157eaf1801b`  
		Last Modified: Fri, 10 Sep 2021 00:20:20 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:scratch`

```console
$ docker pull nats@sha256:6808dfb3132c301916bbeb4241ae1f3c0be5dca763a6c0be6180ca1bd6da298a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:scratch` - linux; amd64

```console
$ docker pull nats@sha256:01dbe57fde6a40eecbd53edc6a418f3c9b1ddd85f03dd17e73ecef98a3b15318
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4546051 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80fcdf2bfe0f4a11267c9e8d06e5e52dce7dd9b41267e1a51d5e9df22c76bf9c`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 10 Sep 2021 00:20:41 GMT
COPY file:0b180121e1ef70970b020901a4b61990a8673ac9db99b94c348c5321333884ea in /nats-server 
# Fri, 10 Sep 2021 00:20:41 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 10 Sep 2021 00:20:41 GMT
EXPOSE 4222 6222 8222
# Fri, 10 Sep 2021 00:20:41 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 10 Sep 2021 00:20:42 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:9cee557b7d3312d12996f8c4338bf9ea02657256657ef77d46510c729d9be195`  
		Last Modified: Fri, 10 Sep 2021 00:21:32 GMT  
		Size: 4.5 MB (4545577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb24b942a0d168497adac7ad3190098a6f8dfa34ad2ef37932150fbce9336c9a`  
		Last Modified: Fri, 10 Sep 2021 00:21:31 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:b21057f1f945b501d03cf3c5c2d530f7961e1a3198e00bb297b7f69a849cc0e9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4210290 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:865dcd8a77138e8339293c7089adeee440305e68331df5533186ea36b8132f84`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 09 Sep 2021 23:50:15 GMT
COPY file:a60049eef2da0cbda1255e229e5e5c6377e3c3445b0cd16ce13a272139c7ce85 in /nats-server 
# Thu, 09 Sep 2021 23:50:16 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 09 Sep 2021 23:50:17 GMT
EXPOSE 4222 6222 8222
# Thu, 09 Sep 2021 23:50:17 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 09 Sep 2021 23:50:18 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b95232e9c9c31dfba5a6124fb74b4abc750a3fd6d5f89a13438a0b051430299e`  
		Last Modified: Thu, 09 Sep 2021 23:52:42 GMT  
		Size: 4.2 MB (4209813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2c01128246ad2a36efed9386a5ed63a01f73f3f56e54d059834ac17a2f64a48`  
		Last Modified: Thu, 09 Sep 2021 23:52:38 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:aafbb0b5e1b7412f9d0e71ddd6c3948c7080697882dd40ae20578b855ca40c1f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4206272 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:79f5a4fb5f9254997b2d7e573f24316740a167eb829bb23952ba05ff8304ddc1`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 10 Sep 2021 00:59:05 GMT
COPY file:7043dd814cd92048127f9905d58e9204d2968d9c03bbb7feba592c45a87e9963 in /nats-server 
# Fri, 10 Sep 2021 00:59:06 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 10 Sep 2021 00:59:06 GMT
EXPOSE 4222 6222 8222
# Fri, 10 Sep 2021 00:59:07 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 10 Sep 2021 00:59:07 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:8ae70a7ddee0b3bc3819ff86ee31d3295a37b10282b7ee0d14d3dd3c8dcb16c7`  
		Last Modified: Fri, 10 Sep 2021 01:01:28 GMT  
		Size: 4.2 MB (4205795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbbfbfa45875dc8bff20ba3a989407cf3ab8018f98f4277411dd068510c071c6`  
		Last Modified: Fri, 10 Sep 2021 01:01:25 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:24f192937e7bc371f7c2631055e49a51d489659d28f55b4fdf2eb5a19843a5ae
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4158958 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2cd8bb7e96599c9badd4424f86ef2d5f8561cfa0c4a4322057847c002da643a9`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 09 Sep 2021 23:40:25 GMT
COPY file:eda8ae8779fbfb7d34c95bc93fc8ce409cbd298cb302284f61ee4ebf6ac10b0e in /nats-server 
# Thu, 09 Sep 2021 23:40:26 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 09 Sep 2021 23:40:26 GMT
EXPOSE 4222 6222 8222
# Thu, 09 Sep 2021 23:40:26 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 09 Sep 2021 23:40:26 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:0c0083faeb4bd1e89eefb7cbc2a5556eb056acaba6107a833c271a1ca7cd8633`  
		Last Modified: Thu, 09 Sep 2021 23:41:48 GMT  
		Size: 4.2 MB (4158481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4227e148c1053ae9735f2dcc2ab35b83566aab7b85aa3d50395ec15be4630e26`  
		Last Modified: Thu, 09 Sep 2021 23:41:47 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:windowsservercore`

```console
$ docker pull nats@sha256:fc4b18ccf5f4b0e559c7deb1e5c01e21f0ba9699b9a6966fce5548faec1f5dfb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.2114; amd64
	-	windows version 10.0.14393.4583; amd64

### `nats:windowsservercore` - windows version 10.0.17763.2114; amd64

```console
$ docker pull nats@sha256:ea5bd03ca8c905a9bb8df9bcefe1c70aada9fce64c82d90932dfaf570332087a
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2691339003 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce14639524af68868fed35dda40295ffe16c35eb58b5038f43989d7d60f7059d`
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
# Fri, 10 Sep 2021 00:14:04 GMT
ENV NATS_SERVER=2.5.0
# Fri, 10 Sep 2021 00:14:05 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.5.0/nats-server-v2.5.0-windows-amd64.zip
# Fri, 10 Sep 2021 00:14:06 GMT
ENV NATS_SERVER_SHASUM=0eae96ad4555f5060b0b6325ba972566b404cd8930b3168b9c0ffe911d15c5d8
# Fri, 10 Sep 2021 00:15:08 GMT
RUN Set-PSDebug -Trace 2
# Fri, 10 Sep 2021 00:16:32 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 10 Sep 2021 00:16:33 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 10 Sep 2021 00:16:34 GMT
EXPOSE 4222 6222 8222
# Fri, 10 Sep 2021 00:16:34 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 10 Sep 2021 00:16:35 GMT
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
	-	`sha256:4c32056c4535002b64e42d1424edb3a7ac778c308d2d9109f33d738d59c85454`  
		Last Modified: Fri, 10 Sep 2021 00:20:02 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb115761571c4ba7b8b719d8ee1587c8898f7e13246d1a92ee2283c0f929a1b1`  
		Last Modified: Fri, 10 Sep 2021 00:20:01 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd93d02cef774a55aa7c6f566b3b5718436cbdae64582cc888ef3b1efe452735`  
		Last Modified: Fri, 10 Sep 2021 00:20:01 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f28336574033153776b7149c4d079b46a95608a291563bc581fc8b029d9399c`  
		Last Modified: Fri, 10 Sep 2021 00:20:02 GMT  
		Size: 372.4 KB (372418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcce3c7fbad71cacb4533bac881f55d312123c387549ca7840f402aa108fb59d`  
		Last Modified: Fri, 10 Sep 2021 00:20:05 GMT  
		Size: 5.0 MB (4955556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0d387c2eda58f8b5f8c3889645ec5e1a977b681cb17de77c04de1c643341b18`  
		Last Modified: Fri, 10 Sep 2021 00:19:59 GMT  
		Size: 1.9 KB (1944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f70bbbc8ecda378ae0099ea8e49350ba7d78be681cd5defc71e6f624abca5d7`  
		Last Modified: Fri, 10 Sep 2021 00:19:59 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76b0025f319f789e7c26483abcf5ca7944dc5a1f0a071023d2415526aa310d40`  
		Last Modified: Fri, 10 Sep 2021 00:19:59 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99ff7344cf8ed7957719594d8f9fe4d78b0ef7acc3755bb1962febcf166ac4ce`  
		Last Modified: Fri, 10 Sep 2021 00:19:59 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:windowsservercore` - windows version 10.0.14393.4583; amd64

```console
$ docker pull nats@sha256:7f318bb6bf586d9b74b6b8e8097ffabf3b4d16c43c5b9b2dd62d532713aa0305
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6276274196 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5716654340a54076fb48e8d797d45b91a2e56551a534fb6d800d7d6c61262257`
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
# Fri, 10 Sep 2021 00:16:55 GMT
ENV NATS_SERVER=2.5.0
# Fri, 10 Sep 2021 00:16:56 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.5.0/nats-server-v2.5.0-windows-amd64.zip
# Fri, 10 Sep 2021 00:16:57 GMT
ENV NATS_SERVER_SHASUM=0eae96ad4555f5060b0b6325ba972566b404cd8930b3168b9c0ffe911d15c5d8
# Fri, 10 Sep 2021 00:17:43 GMT
RUN Set-PSDebug -Trace 2
# Fri, 10 Sep 2021 00:19:14 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 10 Sep 2021 00:19:15 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 10 Sep 2021 00:19:16 GMT
EXPOSE 4222 6222 8222
# Fri, 10 Sep 2021 00:19:17 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 10 Sep 2021 00:19:18 GMT
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
	-	`sha256:786675b79153c67ad039b6b8a55171a8167b2ff8c8186ccb7c5cab0b01f47767`  
		Last Modified: Fri, 10 Sep 2021 00:20:42 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65445b8a1c334a2efce7d34289af9fa682427cba808180c96ce46f39f765e9b5`  
		Last Modified: Fri, 10 Sep 2021 00:20:42 GMT  
		Size: 1.4 KB (1358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08647f69046830b98e59118ace63049f027ad1786cc2aaad037990a4e7a87344`  
		Last Modified: Fri, 10 Sep 2021 00:20:42 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b50cf5c744e8952689c263dbc9800bbe4a032fb4c8df3c8e5028092bdb2a5c9c`  
		Last Modified: Fri, 10 Sep 2021 00:20:42 GMT  
		Size: 338.0 KB (337964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:459c701464a835b4d39cc3183fff454248a3045bb433c26b0430f06e91acf1bb`  
		Last Modified: Fri, 10 Sep 2021 00:20:41 GMT  
		Size: 5.0 MB (4957179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cb2fb143896bcefca1d8ad8640f3146b771f5b284f01be2b849a048d9ac9eeb`  
		Last Modified: Fri, 10 Sep 2021 00:20:40 GMT  
		Size: 1.9 KB (1938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d9f7d515a8e73d005392fc0bccc42761025b86ab370cffe210a552fe53d1cbe`  
		Last Modified: Fri, 10 Sep 2021 00:20:40 GMT  
		Size: 1.4 KB (1380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d68902a6dec2675ab57a60716c10ce8a85e58fe54d7abea307bc340452e882a`  
		Last Modified: Fri, 10 Sep 2021 00:20:39 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37e0389f87abc858cef1a365e6b548d7d7762be571608840bc715ef352c41084`  
		Last Modified: Fri, 10 Sep 2021 00:20:39 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:windowsservercore-1809`

```console
$ docker pull nats@sha256:4e912b79015d0859d5b6c675d055f80bd7628c8e368d96466b6ab6d9c7a51f7b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2114; amd64

### `nats:windowsservercore-1809` - windows version 10.0.17763.2114; amd64

```console
$ docker pull nats@sha256:ea5bd03ca8c905a9bb8df9bcefe1c70aada9fce64c82d90932dfaf570332087a
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2691339003 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce14639524af68868fed35dda40295ffe16c35eb58b5038f43989d7d60f7059d`
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
# Fri, 10 Sep 2021 00:14:04 GMT
ENV NATS_SERVER=2.5.0
# Fri, 10 Sep 2021 00:14:05 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.5.0/nats-server-v2.5.0-windows-amd64.zip
# Fri, 10 Sep 2021 00:14:06 GMT
ENV NATS_SERVER_SHASUM=0eae96ad4555f5060b0b6325ba972566b404cd8930b3168b9c0ffe911d15c5d8
# Fri, 10 Sep 2021 00:15:08 GMT
RUN Set-PSDebug -Trace 2
# Fri, 10 Sep 2021 00:16:32 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 10 Sep 2021 00:16:33 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 10 Sep 2021 00:16:34 GMT
EXPOSE 4222 6222 8222
# Fri, 10 Sep 2021 00:16:34 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 10 Sep 2021 00:16:35 GMT
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
	-	`sha256:4c32056c4535002b64e42d1424edb3a7ac778c308d2d9109f33d738d59c85454`  
		Last Modified: Fri, 10 Sep 2021 00:20:02 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb115761571c4ba7b8b719d8ee1587c8898f7e13246d1a92ee2283c0f929a1b1`  
		Last Modified: Fri, 10 Sep 2021 00:20:01 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd93d02cef774a55aa7c6f566b3b5718436cbdae64582cc888ef3b1efe452735`  
		Last Modified: Fri, 10 Sep 2021 00:20:01 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f28336574033153776b7149c4d079b46a95608a291563bc581fc8b029d9399c`  
		Last Modified: Fri, 10 Sep 2021 00:20:02 GMT  
		Size: 372.4 KB (372418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcce3c7fbad71cacb4533bac881f55d312123c387549ca7840f402aa108fb59d`  
		Last Modified: Fri, 10 Sep 2021 00:20:05 GMT  
		Size: 5.0 MB (4955556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0d387c2eda58f8b5f8c3889645ec5e1a977b681cb17de77c04de1c643341b18`  
		Last Modified: Fri, 10 Sep 2021 00:19:59 GMT  
		Size: 1.9 KB (1944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f70bbbc8ecda378ae0099ea8e49350ba7d78be681cd5defc71e6f624abca5d7`  
		Last Modified: Fri, 10 Sep 2021 00:19:59 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76b0025f319f789e7c26483abcf5ca7944dc5a1f0a071023d2415526aa310d40`  
		Last Modified: Fri, 10 Sep 2021 00:19:59 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99ff7344cf8ed7957719594d8f9fe4d78b0ef7acc3755bb1962febcf166ac4ce`  
		Last Modified: Fri, 10 Sep 2021 00:19:59 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:windowsservercore-ltsc2016`

```console
$ docker pull nats@sha256:521575d35d4f87b16aa1482f712733b1273962ba4f75353d07327cfc4e324cee
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.14393.4583; amd64

### `nats:windowsservercore-ltsc2016` - windows version 10.0.14393.4583; amd64

```console
$ docker pull nats@sha256:7f318bb6bf586d9b74b6b8e8097ffabf3b4d16c43c5b9b2dd62d532713aa0305
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6276274196 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5716654340a54076fb48e8d797d45b91a2e56551a534fb6d800d7d6c61262257`
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
# Fri, 10 Sep 2021 00:16:55 GMT
ENV NATS_SERVER=2.5.0
# Fri, 10 Sep 2021 00:16:56 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.5.0/nats-server-v2.5.0-windows-amd64.zip
# Fri, 10 Sep 2021 00:16:57 GMT
ENV NATS_SERVER_SHASUM=0eae96ad4555f5060b0b6325ba972566b404cd8930b3168b9c0ffe911d15c5d8
# Fri, 10 Sep 2021 00:17:43 GMT
RUN Set-PSDebug -Trace 2
# Fri, 10 Sep 2021 00:19:14 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 10 Sep 2021 00:19:15 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 10 Sep 2021 00:19:16 GMT
EXPOSE 4222 6222 8222
# Fri, 10 Sep 2021 00:19:17 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 10 Sep 2021 00:19:18 GMT
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
	-	`sha256:786675b79153c67ad039b6b8a55171a8167b2ff8c8186ccb7c5cab0b01f47767`  
		Last Modified: Fri, 10 Sep 2021 00:20:42 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65445b8a1c334a2efce7d34289af9fa682427cba808180c96ce46f39f765e9b5`  
		Last Modified: Fri, 10 Sep 2021 00:20:42 GMT  
		Size: 1.4 KB (1358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08647f69046830b98e59118ace63049f027ad1786cc2aaad037990a4e7a87344`  
		Last Modified: Fri, 10 Sep 2021 00:20:42 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b50cf5c744e8952689c263dbc9800bbe4a032fb4c8df3c8e5028092bdb2a5c9c`  
		Last Modified: Fri, 10 Sep 2021 00:20:42 GMT  
		Size: 338.0 KB (337964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:459c701464a835b4d39cc3183fff454248a3045bb433c26b0430f06e91acf1bb`  
		Last Modified: Fri, 10 Sep 2021 00:20:41 GMT  
		Size: 5.0 MB (4957179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cb2fb143896bcefca1d8ad8640f3146b771f5b284f01be2b849a048d9ac9eeb`  
		Last Modified: Fri, 10 Sep 2021 00:20:40 GMT  
		Size: 1.9 KB (1938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d9f7d515a8e73d005392fc0bccc42761025b86ab370cffe210a552fe53d1cbe`  
		Last Modified: Fri, 10 Sep 2021 00:20:40 GMT  
		Size: 1.4 KB (1380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d68902a6dec2675ab57a60716c10ce8a85e58fe54d7abea307bc340452e882a`  
		Last Modified: Fri, 10 Sep 2021 00:20:39 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37e0389f87abc858cef1a365e6b548d7d7762be571608840bc715ef352c41084`  
		Last Modified: Fri, 10 Sep 2021 00:20:39 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
