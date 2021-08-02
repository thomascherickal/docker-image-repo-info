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
-	[`nats:2.3.3`](#nats233)
-	[`nats:2.3.3-alpine`](#nats233-alpine)
-	[`nats:2.3.3-alpine3.14`](#nats233-alpine314)
-	[`nats:2.3.3-linux`](#nats233-linux)
-	[`nats:2.3.3-nanoserver`](#nats233-nanoserver)
-	[`nats:2.3.3-nanoserver-1809`](#nats233-nanoserver-1809)
-	[`nats:2.3.3-scratch`](#nats233-scratch)
-	[`nats:2.3.3-windowsservercore`](#nats233-windowsservercore)
-	[`nats:2.3.3-windowsservercore-1809`](#nats233-windowsservercore-1809)
-	[`nats:2.3.3-windowsservercore-ltsc2016`](#nats233-windowsservercore-ltsc2016)
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
$ docker pull nats@sha256:35e8b0e22283402628389f80b8e9293ff1ecb777a0eb3483032017e387e086f9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.2061; amd64

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
$ docker pull nats@sha256:6e42eec5a210d9a5b6d95c179d5c55193b69846c76786a81908536eac2efbdc3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4173716 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31e1feb9bf2ac457664507fc7899f48e45d49df93dd60eacdea8b8a9cda8ec51`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 02 Aug 2021 21:17:15 GMT
COPY file:55e1c39fb6ec9785ddf1c189ad5438b9f306c3e1c2a355512f4efc73aa1aacf6 in /nats-server 
# Mon, 02 Aug 2021 21:17:15 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Mon, 02 Aug 2021 21:17:16 GMT
EXPOSE 4222 6222 8222
# Mon, 02 Aug 2021 21:17:16 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 02 Aug 2021 21:17:17 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:7f318c30554fccfe6a5ac8a63f4457a20876b88ede949510db6a8f1c5bcf1442`  
		Last Modified: Mon, 02 Aug 2021 21:19:37 GMT  
		Size: 4.2 MB (4173243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76c9419bcd494c007ef4d4f83649e535bb32d84c81337abb67e153ad75a1fb5f`  
		Last Modified: Mon, 02 Aug 2021 21:19:35 GMT  
		Size: 473.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - linux; arm variant v7

```console
$ docker pull nats@sha256:def02210305c7940addd2f5e26e8417017a2f2ae11116ee001b8f2a7bcb17bff
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.0 MB (3992886 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:20941bb671159cef8cb5d6b9047f5c6c298a495274b06f9c6d9278ea5f9e5a1f`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 07 Jul 2021 06:38:20 GMT
COPY file:a259b6f87cc2d22082524e5ba23201057e836734749f0d28676e8637d920d385 in /nats-server 
# Wed, 07 Jul 2021 06:38:21 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Wed, 07 Jul 2021 06:38:21 GMT
EXPOSE 4222 6222 8222
# Wed, 07 Jul 2021 06:38:22 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 07 Jul 2021 06:38:22 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:434fc0c4a6c5daa82c731102728bcac575b5a312862a89edf401b0305d2efc82`  
		Last Modified: Wed, 07 Jul 2021 06:40:42 GMT  
		Size: 4.0 MB (3992410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c195f08925b050ce566763c31c813f3d8c7e1ba40bc4ccdf0949cb87373c3a43`  
		Last Modified: Wed, 07 Jul 2021 06:40:39 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:7a367e1495e9df2cf9cc81af565194815e52b37c0ed1fd7e9f278d88311be5b4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.1 MB (4120338 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad1e0c5709f39238c0ff863c80e1595fb5da12e230643dc6fd4bd6b33cda4039`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 02 Aug 2021 21:06:28 GMT
COPY file:d94287ad868b49da5d590782f3102415d5dfd4ed2a775b4e4c10280c8ab25db3 in /nats-server 
# Mon, 02 Aug 2021 21:06:29 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Mon, 02 Aug 2021 21:06:29 GMT
EXPOSE 4222 6222 8222
# Mon, 02 Aug 2021 21:06:29 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 02 Aug 2021 21:06:29 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4ecc856c82596f8b8982843cac0e5ec138e9c881bfd322038cd7cf0f4942c9c9`  
		Last Modified: Mon, 02 Aug 2021 21:07:52 GMT  
		Size: 4.1 MB (4119864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68fa4df40d0356fc86fe0d6c780d2a447fe1b2c32b5572c65a3c7d2354961da4`  
		Last Modified: Mon, 02 Aug 2021 21:07:51 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - windows version 10.0.17763.2061; amd64

```console
$ docker pull nats@sha256:baf086eb51e7090cb2ef985758c034c882cbe1dd8d4b2a682a618d32b9215e35
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.3 MB (107296331 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d57bb9c1561692bbad5576428cd8e22189f1addf3a8b82e73e3f27e246bd485`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 06 Jul 2021 20:06:39 GMT
RUN Apply image 1809-amd64
# Wed, 14 Jul 2021 02:35:24 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Mon, 02 Aug 2021 21:17:05 GMT
RUN cmd /S /C #(nop) COPY file:359dd4a92709029cd62dc9620a8ff30527cb3494d6b89c9332ae019bae51b57b in C:\nats-server.exe 
# Mon, 02 Aug 2021 21:17:08 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Mon, 02 Aug 2021 21:17:10 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Mon, 02 Aug 2021 21:17:13 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Mon, 02 Aug 2021 21:17:16 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:29d43e56445c5279a6386c4dfe4d1ada3c7124ade9cb7b0f2757e58ffc7cd10b`  
		Size: 102.7 MB (102725622 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ec20c4c9f6fa5e782e09342d50033ef24c4049a9dad1befd33c96759b71da6de`  
		Last Modified: Wed, 14 Jul 2021 02:40:36 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab54ee8cb88b349708e6f2d10afe13c1d843b9c1ff995a70d40af5ca886eda42`  
		Last Modified: Mon, 02 Aug 2021 21:21:37 GMT  
		Size: 4.6 MB (4564319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27d161923a9b16db535efc5f78e4aedd08225387cc8377cedb826e7539fa9051`  
		Last Modified: Mon, 02 Aug 2021 21:21:36 GMT  
		Size: 1.8 KB (1766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e88c4ba846a11b45abc01afc7de665b15430ebfd4c6e585ba8cb11d896017cd`  
		Last Modified: Mon, 02 Aug 2021 21:21:36 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26ca1fda898c73546bdd8f1655f276fe9a0911a7c16f5a4054cdb40e996692c2`  
		Last Modified: Mon, 02 Aug 2021 21:21:36 GMT  
		Size: 1.2 KB (1180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:088b6cb05a147f4faf4e14f0fc1ecda8481f5ad0a8741dba786aebba4374207b`  
		Last Modified: Mon, 02 Aug 2021 21:21:36 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-alpine`

```console
$ docker pull nats@sha256:3ec525b1d139794286ecdb26410cff8ccf814eca88de9fe23c39a7d4b58479ef
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-alpine` - linux; amd64

```console
$ docker pull nats@sha256:b430407bf4008593c12a2cc85208f72e96b53fec98b30187c517b9d1958b657e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7601531 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:37a8e948168fcd8c0825a0cd425eb489bd313da994d65e73b5072d6ff6c8225a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 15 Jun 2021 22:19:37 GMT
ADD file:f278386b0cef68136129f5f58c52445590a417b624d62bca158d4dc926c340df in / 
# Tue, 15 Jun 2021 22:19:37 GMT
CMD ["/bin/sh"]
# Mon, 02 Aug 2021 21:22:41 GMT
ENV NATS_SERVER=2.3.3
# Mon, 02 Aug 2021 21:22:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f8e04470165fdfba062442cf5975f22668ab20fb12df7e299734e16a45370bef' ;; 		armhf) natsArch='arm6'; sha256='6396531f34e99cca903cdd461a79f1b8255d0cc219e5186ea15284b5b5e7e5e7' ;; 		armv7) natsArch='arm7'; sha256='4353de84d9e42b24b73ba98a4ed2a9eaa7c4f945bd68e1ddb4fbde885020ab30' ;; 		x86_64) natsArch='amd64'; sha256='66703b81de34d06060eb2198dfb5a1087547d45e680dee4da1214198a8073ce5' ;; 		x86) natsArch='386'; sha256='e38b9c9eda279bc4eee9cf6a3d4b2b25774b692450421a16e2ff6602977e6571' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Mon, 02 Aug 2021 21:22:44 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Mon, 02 Aug 2021 21:22:44 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 02 Aug 2021 21:22:44 GMT
EXPOSE 4222 6222 8222
# Mon, 02 Aug 2021 21:22:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 02 Aug 2021 21:22:45 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:5843afab387455b37944e709ee8c78d7520df80f8d01cf7f861aae63beeddb6b`  
		Last Modified: Tue, 15 Jun 2021 22:20:04 GMT  
		Size: 2.8 MB (2811478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03113b330e4f7fe35234354441a5bc0f8cabb61f7e7c02e1c2c7a9002be630c7`  
		Last Modified: Mon, 02 Aug 2021 21:23:32 GMT  
		Size: 4.8 MB (4789084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe9957a382ed4e85c0797d4c958c23eb4c68ab7e84a78c07a137bbf4bfd93c86`  
		Last Modified: Mon, 02 Aug 2021 21:23:31 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51734fe5b37d3390b972f615a9b12d4454a30ce0ed124f4a5d0f91a17d6ce6f8`  
		Last Modified: Mon, 02 Aug 2021 21:23:30 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:d5fc2c9df074891880beadedf530ee3dbf0761259a14619e946c1cefa842cac3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7079723 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f49351bac7a37d427b25fbdcc43daa3d1ea704fe96f3931802df83f01bf235c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 30 Jul 2021 17:49:42 GMT
ADD file:c80bc2b093cbc0fc466582ef21cbed377de9fa874aedbf320079525ddacd1200 in / 
# Fri, 30 Jul 2021 17:49:42 GMT
CMD ["/bin/sh"]
# Mon, 02 Aug 2021 21:16:47 GMT
ENV NATS_SERVER=2.3.3
# Mon, 02 Aug 2021 21:16:52 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f8e04470165fdfba062442cf5975f22668ab20fb12df7e299734e16a45370bef' ;; 		armhf) natsArch='arm6'; sha256='6396531f34e99cca903cdd461a79f1b8255d0cc219e5186ea15284b5b5e7e5e7' ;; 		armv7) natsArch='arm7'; sha256='4353de84d9e42b24b73ba98a4ed2a9eaa7c4f945bd68e1ddb4fbde885020ab30' ;; 		x86_64) natsArch='amd64'; sha256='66703b81de34d06060eb2198dfb5a1087547d45e680dee4da1214198a8073ce5' ;; 		x86) natsArch='386'; sha256='e38b9c9eda279bc4eee9cf6a3d4b2b25774b692450421a16e2ff6602977e6571' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Mon, 02 Aug 2021 21:16:52 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Mon, 02 Aug 2021 21:16:53 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 02 Aug 2021 21:16:53 GMT
EXPOSE 4222 6222 8222
# Mon, 02 Aug 2021 21:16:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 02 Aug 2021 21:16:54 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:b4c9a0924271af3466de27804af26420eb58da1466e7eaaba127d178b380fea3`  
		Last Modified: Tue, 15 Jun 2021 22:58:47 GMT  
		Size: 2.6 MB (2624382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e3313ef1b9ecd8d9e94997ae371b1c0aabda27773f0b2e12b4be7463517cf87`  
		Last Modified: Mon, 02 Aug 2021 21:18:59 GMT  
		Size: 4.5 MB (4454370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:785fbb490293d9c2f8cdaed64735e76ea2a0dc1c40e13814102053f6d9c4ddc3`  
		Last Modified: Mon, 02 Aug 2021 21:18:56 GMT  
		Size: 557.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ee9f0a3fdc78fe2942c2a3d6969418df884ad628f52adb50525f4022ed56ec2`  
		Last Modified: Mon, 02 Aug 2021 21:18:56 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:0cd94d122e5dd418d4d447257c6622e13c1d86149c0e7979057664951ab5a020
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.7 MB (6703143 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5635c4604b79a25fc3fdf3ccf6606d69eb347b3e8a3cb756dd261e2ca83e780`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 30 Jul 2021 18:36:19 GMT
ADD file:416a8b507abdc6bdcb22997a4be0a4170796c3f9f77e315b2dbff2b0a212bc68 in / 
# Fri, 30 Jul 2021 18:36:20 GMT
CMD ["/bin/sh"]
# Sat, 31 Jul 2021 03:13:57 GMT
ENV NATS_SERVER=2.3.2
# Sat, 31 Jul 2021 03:14:02 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='18a68cbef5c7a41052f5281bdfe9164b51cbeb60ce2dd31a7945c5adbcd39c2d' ;; 		armhf) natsArch='arm6'; sha256='a37949f8a1e24d5a8e47f57786e126205de7c3f6f8b3e5b849f33adbcfe8d2fb' ;; 		armv7) natsArch='arm7'; sha256='43a4820a57161b83fe721b81098d2ba9b1e2f42923be898f031bac40279f8f6e' ;; 		x86_64) natsArch='amd64'; sha256='6e6fdf781465fbf09cb024112b34ae6b2b432d94a5fc8b62f6ebf0da5fc3345d' ;; 		x86) natsArch='386'; sha256='c7c0ea9a5343925f0f5e2dda964946152382b0a3e0db96aa43c3f2ab17a37bf0' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Sat, 31 Jul 2021 03:14:03 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Sat, 31 Jul 2021 03:14:03 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Sat, 31 Jul 2021 03:14:04 GMT
EXPOSE 4222 6222 8222
# Sat, 31 Jul 2021 03:14:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 31 Jul 2021 03:14:05 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:136482bf81d1fa351b424ebb8c7e34d15f2c5ed3fc0b66b544b8312bda3d52d9`  
		Last Modified: Tue, 15 Jun 2021 23:16:40 GMT  
		Size: 2.4 MB (2427917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1a0b8bfe79fe7add5c0f3af812a506d01cc94a574cd58ba1f81146318d3638c`  
		Last Modified: Sat, 31 Jul 2021 03:16:43 GMT  
		Size: 4.3 MB (4274251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c35ac8f58b7f43ebc215a5713841cf5a94983b092019cf46da7ce8a3c9c84146`  
		Last Modified: Sat, 31 Jul 2021 03:16:40 GMT  
		Size: 560.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:735e5b5c342cb95f3f2eb33812321a4305479b159555d6fed062e4bb2880dc66`  
		Last Modified: Sat, 31 Jul 2021 03:16:40 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:f818c9007861b8440d5c89a859f8f20f483637ab3f3e7c7a7f89ef40afd23937
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7113993 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc01fa8c08e4612961dfe7cf6c422a1a58b99637fd0297f9c3d811b95a32c185`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 15 Jun 2021 21:44:56 GMT
ADD file:6797caacbfe41bfe44000b39ed017016c6fcc492b3d6557cdaba88536df6c876 in / 
# Tue, 15 Jun 2021 21:44:56 GMT
CMD ["/bin/sh"]
# Mon, 02 Aug 2021 21:06:09 GMT
ENV NATS_SERVER=2.3.3
# Mon, 02 Aug 2021 21:06:11 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f8e04470165fdfba062442cf5975f22668ab20fb12df7e299734e16a45370bef' ;; 		armhf) natsArch='arm6'; sha256='6396531f34e99cca903cdd461a79f1b8255d0cc219e5186ea15284b5b5e7e5e7' ;; 		armv7) natsArch='arm7'; sha256='4353de84d9e42b24b73ba98a4ed2a9eaa7c4f945bd68e1ddb4fbde885020ab30' ;; 		x86_64) natsArch='amd64'; sha256='66703b81de34d06060eb2198dfb5a1087547d45e680dee4da1214198a8073ce5' ;; 		x86) natsArch='386'; sha256='e38b9c9eda279bc4eee9cf6a3d4b2b25774b692450421a16e2ff6602977e6571' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Mon, 02 Aug 2021 21:06:11 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Mon, 02 Aug 2021 21:06:12 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 02 Aug 2021 21:06:12 GMT
EXPOSE 4222 6222 8222
# Mon, 02 Aug 2021 21:06:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 02 Aug 2021 21:06:12 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:58ab47519297212468320b23b8100fc1b2b96e8d342040806ae509a778a0a07a`  
		Last Modified: Tue, 15 Jun 2021 21:46:03 GMT  
		Size: 2.7 MB (2709626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0b71cb50e81b94a1183dec31a916ec92da12268c9d5c01358f63f093176829d`  
		Last Modified: Mon, 02 Aug 2021 21:07:22 GMT  
		Size: 4.4 MB (4403398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69e71c9cdab2ba7a29d11ef463c8173ea1cdc1f4a0a549ee1d8bdf0a21392641`  
		Last Modified: Mon, 02 Aug 2021 21:07:21 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17f4a027c87d570eda83fa005f1747518d8e6f172eaf1f5432d6073835418317`  
		Last Modified: Mon, 02 Aug 2021 21:07:21 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-alpine3.14`

```console
$ docker pull nats@sha256:3ec525b1d139794286ecdb26410cff8ccf814eca88de9fe23c39a7d4b58479ef
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-alpine3.14` - linux; amd64

```console
$ docker pull nats@sha256:b430407bf4008593c12a2cc85208f72e96b53fec98b30187c517b9d1958b657e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7601531 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:37a8e948168fcd8c0825a0cd425eb489bd313da994d65e73b5072d6ff6c8225a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 15 Jun 2021 22:19:37 GMT
ADD file:f278386b0cef68136129f5f58c52445590a417b624d62bca158d4dc926c340df in / 
# Tue, 15 Jun 2021 22:19:37 GMT
CMD ["/bin/sh"]
# Mon, 02 Aug 2021 21:22:41 GMT
ENV NATS_SERVER=2.3.3
# Mon, 02 Aug 2021 21:22:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f8e04470165fdfba062442cf5975f22668ab20fb12df7e299734e16a45370bef' ;; 		armhf) natsArch='arm6'; sha256='6396531f34e99cca903cdd461a79f1b8255d0cc219e5186ea15284b5b5e7e5e7' ;; 		armv7) natsArch='arm7'; sha256='4353de84d9e42b24b73ba98a4ed2a9eaa7c4f945bd68e1ddb4fbde885020ab30' ;; 		x86_64) natsArch='amd64'; sha256='66703b81de34d06060eb2198dfb5a1087547d45e680dee4da1214198a8073ce5' ;; 		x86) natsArch='386'; sha256='e38b9c9eda279bc4eee9cf6a3d4b2b25774b692450421a16e2ff6602977e6571' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Mon, 02 Aug 2021 21:22:44 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Mon, 02 Aug 2021 21:22:44 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 02 Aug 2021 21:22:44 GMT
EXPOSE 4222 6222 8222
# Mon, 02 Aug 2021 21:22:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 02 Aug 2021 21:22:45 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:5843afab387455b37944e709ee8c78d7520df80f8d01cf7f861aae63beeddb6b`  
		Last Modified: Tue, 15 Jun 2021 22:20:04 GMT  
		Size: 2.8 MB (2811478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03113b330e4f7fe35234354441a5bc0f8cabb61f7e7c02e1c2c7a9002be630c7`  
		Last Modified: Mon, 02 Aug 2021 21:23:32 GMT  
		Size: 4.8 MB (4789084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe9957a382ed4e85c0797d4c958c23eb4c68ab7e84a78c07a137bbf4bfd93c86`  
		Last Modified: Mon, 02 Aug 2021 21:23:31 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51734fe5b37d3390b972f615a9b12d4454a30ce0ed124f4a5d0f91a17d6ce6f8`  
		Last Modified: Mon, 02 Aug 2021 21:23:30 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.14` - linux; arm variant v6

```console
$ docker pull nats@sha256:d5fc2c9df074891880beadedf530ee3dbf0761259a14619e946c1cefa842cac3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7079723 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f49351bac7a37d427b25fbdcc43daa3d1ea704fe96f3931802df83f01bf235c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 30 Jul 2021 17:49:42 GMT
ADD file:c80bc2b093cbc0fc466582ef21cbed377de9fa874aedbf320079525ddacd1200 in / 
# Fri, 30 Jul 2021 17:49:42 GMT
CMD ["/bin/sh"]
# Mon, 02 Aug 2021 21:16:47 GMT
ENV NATS_SERVER=2.3.3
# Mon, 02 Aug 2021 21:16:52 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f8e04470165fdfba062442cf5975f22668ab20fb12df7e299734e16a45370bef' ;; 		armhf) natsArch='arm6'; sha256='6396531f34e99cca903cdd461a79f1b8255d0cc219e5186ea15284b5b5e7e5e7' ;; 		armv7) natsArch='arm7'; sha256='4353de84d9e42b24b73ba98a4ed2a9eaa7c4f945bd68e1ddb4fbde885020ab30' ;; 		x86_64) natsArch='amd64'; sha256='66703b81de34d06060eb2198dfb5a1087547d45e680dee4da1214198a8073ce5' ;; 		x86) natsArch='386'; sha256='e38b9c9eda279bc4eee9cf6a3d4b2b25774b692450421a16e2ff6602977e6571' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Mon, 02 Aug 2021 21:16:52 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Mon, 02 Aug 2021 21:16:53 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 02 Aug 2021 21:16:53 GMT
EXPOSE 4222 6222 8222
# Mon, 02 Aug 2021 21:16:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 02 Aug 2021 21:16:54 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:b4c9a0924271af3466de27804af26420eb58da1466e7eaaba127d178b380fea3`  
		Last Modified: Tue, 15 Jun 2021 22:58:47 GMT  
		Size: 2.6 MB (2624382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e3313ef1b9ecd8d9e94997ae371b1c0aabda27773f0b2e12b4be7463517cf87`  
		Last Modified: Mon, 02 Aug 2021 21:18:59 GMT  
		Size: 4.5 MB (4454370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:785fbb490293d9c2f8cdaed64735e76ea2a0dc1c40e13814102053f6d9c4ddc3`  
		Last Modified: Mon, 02 Aug 2021 21:18:56 GMT  
		Size: 557.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ee9f0a3fdc78fe2942c2a3d6969418df884ad628f52adb50525f4022ed56ec2`  
		Last Modified: Mon, 02 Aug 2021 21:18:56 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.14` - linux; arm variant v7

```console
$ docker pull nats@sha256:0cd94d122e5dd418d4d447257c6622e13c1d86149c0e7979057664951ab5a020
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.7 MB (6703143 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5635c4604b79a25fc3fdf3ccf6606d69eb347b3e8a3cb756dd261e2ca83e780`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 30 Jul 2021 18:36:19 GMT
ADD file:416a8b507abdc6bdcb22997a4be0a4170796c3f9f77e315b2dbff2b0a212bc68 in / 
# Fri, 30 Jul 2021 18:36:20 GMT
CMD ["/bin/sh"]
# Sat, 31 Jul 2021 03:13:57 GMT
ENV NATS_SERVER=2.3.2
# Sat, 31 Jul 2021 03:14:02 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='18a68cbef5c7a41052f5281bdfe9164b51cbeb60ce2dd31a7945c5adbcd39c2d' ;; 		armhf) natsArch='arm6'; sha256='a37949f8a1e24d5a8e47f57786e126205de7c3f6f8b3e5b849f33adbcfe8d2fb' ;; 		armv7) natsArch='arm7'; sha256='43a4820a57161b83fe721b81098d2ba9b1e2f42923be898f031bac40279f8f6e' ;; 		x86_64) natsArch='amd64'; sha256='6e6fdf781465fbf09cb024112b34ae6b2b432d94a5fc8b62f6ebf0da5fc3345d' ;; 		x86) natsArch='386'; sha256='c7c0ea9a5343925f0f5e2dda964946152382b0a3e0db96aa43c3f2ab17a37bf0' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Sat, 31 Jul 2021 03:14:03 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Sat, 31 Jul 2021 03:14:03 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Sat, 31 Jul 2021 03:14:04 GMT
EXPOSE 4222 6222 8222
# Sat, 31 Jul 2021 03:14:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 31 Jul 2021 03:14:05 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:136482bf81d1fa351b424ebb8c7e34d15f2c5ed3fc0b66b544b8312bda3d52d9`  
		Last Modified: Tue, 15 Jun 2021 23:16:40 GMT  
		Size: 2.4 MB (2427917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1a0b8bfe79fe7add5c0f3af812a506d01cc94a574cd58ba1f81146318d3638c`  
		Last Modified: Sat, 31 Jul 2021 03:16:43 GMT  
		Size: 4.3 MB (4274251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c35ac8f58b7f43ebc215a5713841cf5a94983b092019cf46da7ce8a3c9c84146`  
		Last Modified: Sat, 31 Jul 2021 03:16:40 GMT  
		Size: 560.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:735e5b5c342cb95f3f2eb33812321a4305479b159555d6fed062e4bb2880dc66`  
		Last Modified: Sat, 31 Jul 2021 03:16:40 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.14` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:f818c9007861b8440d5c89a859f8f20f483637ab3f3e7c7a7f89ef40afd23937
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7113993 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc01fa8c08e4612961dfe7cf6c422a1a58b99637fd0297f9c3d811b95a32c185`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 15 Jun 2021 21:44:56 GMT
ADD file:6797caacbfe41bfe44000b39ed017016c6fcc492b3d6557cdaba88536df6c876 in / 
# Tue, 15 Jun 2021 21:44:56 GMT
CMD ["/bin/sh"]
# Mon, 02 Aug 2021 21:06:09 GMT
ENV NATS_SERVER=2.3.3
# Mon, 02 Aug 2021 21:06:11 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f8e04470165fdfba062442cf5975f22668ab20fb12df7e299734e16a45370bef' ;; 		armhf) natsArch='arm6'; sha256='6396531f34e99cca903cdd461a79f1b8255d0cc219e5186ea15284b5b5e7e5e7' ;; 		armv7) natsArch='arm7'; sha256='4353de84d9e42b24b73ba98a4ed2a9eaa7c4f945bd68e1ddb4fbde885020ab30' ;; 		x86_64) natsArch='amd64'; sha256='66703b81de34d06060eb2198dfb5a1087547d45e680dee4da1214198a8073ce5' ;; 		x86) natsArch='386'; sha256='e38b9c9eda279bc4eee9cf6a3d4b2b25774b692450421a16e2ff6602977e6571' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Mon, 02 Aug 2021 21:06:11 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Mon, 02 Aug 2021 21:06:12 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 02 Aug 2021 21:06:12 GMT
EXPOSE 4222 6222 8222
# Mon, 02 Aug 2021 21:06:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 02 Aug 2021 21:06:12 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:58ab47519297212468320b23b8100fc1b2b96e8d342040806ae509a778a0a07a`  
		Last Modified: Tue, 15 Jun 2021 21:46:03 GMT  
		Size: 2.7 MB (2709626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0b71cb50e81b94a1183dec31a916ec92da12268c9d5c01358f63f093176829d`  
		Last Modified: Mon, 02 Aug 2021 21:07:22 GMT  
		Size: 4.4 MB (4403398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69e71c9cdab2ba7a29d11ef463c8173ea1cdc1f4a0a549ee1d8bdf0a21392641`  
		Last Modified: Mon, 02 Aug 2021 21:07:21 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17f4a027c87d570eda83fa005f1747518d8e6f172eaf1f5432d6073835418317`  
		Last Modified: Mon, 02 Aug 2021 21:07:21 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-linux`

```console
$ docker pull nats@sha256:111aefb3002e16ecc001abaa0bb5fc9aabf2510005be379d2cedc0373fa1e596
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-linux` - linux; amd64

```console
$ docker pull nats@sha256:4f6857e56d3555432c7bc830fb297d8c00cbe3b0522f81dfc8c84a4dacb54ed5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4505352 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23830fcc7f9834fd409d95d2bf9877f21b609b7b7392bfcd4b8b5e62e8be14fc`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 02 Aug 2021 21:23:05 GMT
COPY file:0b22daa17d88302a2606c64df249d26684c5926e82494be3f08d920922b75196 in /nats-server 
# Mon, 02 Aug 2021 21:23:05 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Mon, 02 Aug 2021 21:23:05 GMT
EXPOSE 4222 6222 8222
# Mon, 02 Aug 2021 21:23:05 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 02 Aug 2021 21:23:05 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:267760e6058167430070f7584ea1e5e18b4ddf538aec80d4b764ba1b9096b403`  
		Last Modified: Mon, 02 Aug 2021 21:23:56 GMT  
		Size: 4.5 MB (4504877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:612bea9c73fc6c5c02659a6bff01f1bcada2f4c47323021b03bee52a9ca1eba0`  
		Last Modified: Mon, 02 Aug 2021 21:23:55 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:6e42eec5a210d9a5b6d95c179d5c55193b69846c76786a81908536eac2efbdc3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4173716 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31e1feb9bf2ac457664507fc7899f48e45d49df93dd60eacdea8b8a9cda8ec51`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 02 Aug 2021 21:17:15 GMT
COPY file:55e1c39fb6ec9785ddf1c189ad5438b9f306c3e1c2a355512f4efc73aa1aacf6 in /nats-server 
# Mon, 02 Aug 2021 21:17:15 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Mon, 02 Aug 2021 21:17:16 GMT
EXPOSE 4222 6222 8222
# Mon, 02 Aug 2021 21:17:16 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 02 Aug 2021 21:17:17 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:7f318c30554fccfe6a5ac8a63f4457a20876b88ede949510db6a8f1c5bcf1442`  
		Last Modified: Mon, 02 Aug 2021 21:19:37 GMT  
		Size: 4.2 MB (4173243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76c9419bcd494c007ef4d4f83649e535bb32d84c81337abb67e153ad75a1fb5f`  
		Last Modified: Mon, 02 Aug 2021 21:19:35 GMT  
		Size: 473.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:def02210305c7940addd2f5e26e8417017a2f2ae11116ee001b8f2a7bcb17bff
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.0 MB (3992886 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:20941bb671159cef8cb5d6b9047f5c6c298a495274b06f9c6d9278ea5f9e5a1f`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 07 Jul 2021 06:38:20 GMT
COPY file:a259b6f87cc2d22082524e5ba23201057e836734749f0d28676e8637d920d385 in /nats-server 
# Wed, 07 Jul 2021 06:38:21 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Wed, 07 Jul 2021 06:38:21 GMT
EXPOSE 4222 6222 8222
# Wed, 07 Jul 2021 06:38:22 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 07 Jul 2021 06:38:22 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:434fc0c4a6c5daa82c731102728bcac575b5a312862a89edf401b0305d2efc82`  
		Last Modified: Wed, 07 Jul 2021 06:40:42 GMT  
		Size: 4.0 MB (3992410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c195f08925b050ce566763c31c813f3d8c7e1ba40bc4ccdf0949cb87373c3a43`  
		Last Modified: Wed, 07 Jul 2021 06:40:39 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:7a367e1495e9df2cf9cc81af565194815e52b37c0ed1fd7e9f278d88311be5b4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.1 MB (4120338 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad1e0c5709f39238c0ff863c80e1595fb5da12e230643dc6fd4bd6b33cda4039`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 02 Aug 2021 21:06:28 GMT
COPY file:d94287ad868b49da5d590782f3102415d5dfd4ed2a775b4e4c10280c8ab25db3 in /nats-server 
# Mon, 02 Aug 2021 21:06:29 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Mon, 02 Aug 2021 21:06:29 GMT
EXPOSE 4222 6222 8222
# Mon, 02 Aug 2021 21:06:29 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 02 Aug 2021 21:06:29 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4ecc856c82596f8b8982843cac0e5ec138e9c881bfd322038cd7cf0f4942c9c9`  
		Last Modified: Mon, 02 Aug 2021 21:07:52 GMT  
		Size: 4.1 MB (4119864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68fa4df40d0356fc86fe0d6c780d2a447fe1b2c32b5572c65a3c7d2354961da4`  
		Last Modified: Mon, 02 Aug 2021 21:07:51 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-nanoserver`

```console
$ docker pull nats@sha256:089f1003c28ef5e80a16a558155a581473b77e6d540a50934cc9d7fd5ca6a71b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2061; amd64

### `nats:2-nanoserver` - windows version 10.0.17763.2061; amd64

```console
$ docker pull nats@sha256:baf086eb51e7090cb2ef985758c034c882cbe1dd8d4b2a682a618d32b9215e35
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.3 MB (107296331 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d57bb9c1561692bbad5576428cd8e22189f1addf3a8b82e73e3f27e246bd485`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 06 Jul 2021 20:06:39 GMT
RUN Apply image 1809-amd64
# Wed, 14 Jul 2021 02:35:24 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Mon, 02 Aug 2021 21:17:05 GMT
RUN cmd /S /C #(nop) COPY file:359dd4a92709029cd62dc9620a8ff30527cb3494d6b89c9332ae019bae51b57b in C:\nats-server.exe 
# Mon, 02 Aug 2021 21:17:08 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Mon, 02 Aug 2021 21:17:10 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Mon, 02 Aug 2021 21:17:13 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Mon, 02 Aug 2021 21:17:16 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:29d43e56445c5279a6386c4dfe4d1ada3c7124ade9cb7b0f2757e58ffc7cd10b`  
		Size: 102.7 MB (102725622 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ec20c4c9f6fa5e782e09342d50033ef24c4049a9dad1befd33c96759b71da6de`  
		Last Modified: Wed, 14 Jul 2021 02:40:36 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab54ee8cb88b349708e6f2d10afe13c1d843b9c1ff995a70d40af5ca886eda42`  
		Last Modified: Mon, 02 Aug 2021 21:21:37 GMT  
		Size: 4.6 MB (4564319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27d161923a9b16db535efc5f78e4aedd08225387cc8377cedb826e7539fa9051`  
		Last Modified: Mon, 02 Aug 2021 21:21:36 GMT  
		Size: 1.8 KB (1766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e88c4ba846a11b45abc01afc7de665b15430ebfd4c6e585ba8cb11d896017cd`  
		Last Modified: Mon, 02 Aug 2021 21:21:36 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26ca1fda898c73546bdd8f1655f276fe9a0911a7c16f5a4054cdb40e996692c2`  
		Last Modified: Mon, 02 Aug 2021 21:21:36 GMT  
		Size: 1.2 KB (1180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:088b6cb05a147f4faf4e14f0fc1ecda8481f5ad0a8741dba786aebba4374207b`  
		Last Modified: Mon, 02 Aug 2021 21:21:36 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-nanoserver-1809`

```console
$ docker pull nats@sha256:089f1003c28ef5e80a16a558155a581473b77e6d540a50934cc9d7fd5ca6a71b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2061; amd64

### `nats:2-nanoserver-1809` - windows version 10.0.17763.2061; amd64

```console
$ docker pull nats@sha256:baf086eb51e7090cb2ef985758c034c882cbe1dd8d4b2a682a618d32b9215e35
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.3 MB (107296331 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d57bb9c1561692bbad5576428cd8e22189f1addf3a8b82e73e3f27e246bd485`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 06 Jul 2021 20:06:39 GMT
RUN Apply image 1809-amd64
# Wed, 14 Jul 2021 02:35:24 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Mon, 02 Aug 2021 21:17:05 GMT
RUN cmd /S /C #(nop) COPY file:359dd4a92709029cd62dc9620a8ff30527cb3494d6b89c9332ae019bae51b57b in C:\nats-server.exe 
# Mon, 02 Aug 2021 21:17:08 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Mon, 02 Aug 2021 21:17:10 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Mon, 02 Aug 2021 21:17:13 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Mon, 02 Aug 2021 21:17:16 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:29d43e56445c5279a6386c4dfe4d1ada3c7124ade9cb7b0f2757e58ffc7cd10b`  
		Size: 102.7 MB (102725622 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ec20c4c9f6fa5e782e09342d50033ef24c4049a9dad1befd33c96759b71da6de`  
		Last Modified: Wed, 14 Jul 2021 02:40:36 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab54ee8cb88b349708e6f2d10afe13c1d843b9c1ff995a70d40af5ca886eda42`  
		Last Modified: Mon, 02 Aug 2021 21:21:37 GMT  
		Size: 4.6 MB (4564319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27d161923a9b16db535efc5f78e4aedd08225387cc8377cedb826e7539fa9051`  
		Last Modified: Mon, 02 Aug 2021 21:21:36 GMT  
		Size: 1.8 KB (1766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e88c4ba846a11b45abc01afc7de665b15430ebfd4c6e585ba8cb11d896017cd`  
		Last Modified: Mon, 02 Aug 2021 21:21:36 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26ca1fda898c73546bdd8f1655f276fe9a0911a7c16f5a4054cdb40e996692c2`  
		Last Modified: Mon, 02 Aug 2021 21:21:36 GMT  
		Size: 1.2 KB (1180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:088b6cb05a147f4faf4e14f0fc1ecda8481f5ad0a8741dba786aebba4374207b`  
		Last Modified: Mon, 02 Aug 2021 21:21:36 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-scratch`

```console
$ docker pull nats@sha256:111aefb3002e16ecc001abaa0bb5fc9aabf2510005be379d2cedc0373fa1e596
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-scratch` - linux; amd64

```console
$ docker pull nats@sha256:4f6857e56d3555432c7bc830fb297d8c00cbe3b0522f81dfc8c84a4dacb54ed5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4505352 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23830fcc7f9834fd409d95d2bf9877f21b609b7b7392bfcd4b8b5e62e8be14fc`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 02 Aug 2021 21:23:05 GMT
COPY file:0b22daa17d88302a2606c64df249d26684c5926e82494be3f08d920922b75196 in /nats-server 
# Mon, 02 Aug 2021 21:23:05 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Mon, 02 Aug 2021 21:23:05 GMT
EXPOSE 4222 6222 8222
# Mon, 02 Aug 2021 21:23:05 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 02 Aug 2021 21:23:05 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:267760e6058167430070f7584ea1e5e18b4ddf538aec80d4b764ba1b9096b403`  
		Last Modified: Mon, 02 Aug 2021 21:23:56 GMT  
		Size: 4.5 MB (4504877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:612bea9c73fc6c5c02659a6bff01f1bcada2f4c47323021b03bee52a9ca1eba0`  
		Last Modified: Mon, 02 Aug 2021 21:23:55 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:6e42eec5a210d9a5b6d95c179d5c55193b69846c76786a81908536eac2efbdc3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4173716 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31e1feb9bf2ac457664507fc7899f48e45d49df93dd60eacdea8b8a9cda8ec51`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 02 Aug 2021 21:17:15 GMT
COPY file:55e1c39fb6ec9785ddf1c189ad5438b9f306c3e1c2a355512f4efc73aa1aacf6 in /nats-server 
# Mon, 02 Aug 2021 21:17:15 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Mon, 02 Aug 2021 21:17:16 GMT
EXPOSE 4222 6222 8222
# Mon, 02 Aug 2021 21:17:16 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 02 Aug 2021 21:17:17 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:7f318c30554fccfe6a5ac8a63f4457a20876b88ede949510db6a8f1c5bcf1442`  
		Last Modified: Mon, 02 Aug 2021 21:19:37 GMT  
		Size: 4.2 MB (4173243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76c9419bcd494c007ef4d4f83649e535bb32d84c81337abb67e153ad75a1fb5f`  
		Last Modified: Mon, 02 Aug 2021 21:19:35 GMT  
		Size: 473.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:def02210305c7940addd2f5e26e8417017a2f2ae11116ee001b8f2a7bcb17bff
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.0 MB (3992886 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:20941bb671159cef8cb5d6b9047f5c6c298a495274b06f9c6d9278ea5f9e5a1f`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 07 Jul 2021 06:38:20 GMT
COPY file:a259b6f87cc2d22082524e5ba23201057e836734749f0d28676e8637d920d385 in /nats-server 
# Wed, 07 Jul 2021 06:38:21 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Wed, 07 Jul 2021 06:38:21 GMT
EXPOSE 4222 6222 8222
# Wed, 07 Jul 2021 06:38:22 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 07 Jul 2021 06:38:22 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:434fc0c4a6c5daa82c731102728bcac575b5a312862a89edf401b0305d2efc82`  
		Last Modified: Wed, 07 Jul 2021 06:40:42 GMT  
		Size: 4.0 MB (3992410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c195f08925b050ce566763c31c813f3d8c7e1ba40bc4ccdf0949cb87373c3a43`  
		Last Modified: Wed, 07 Jul 2021 06:40:39 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:7a367e1495e9df2cf9cc81af565194815e52b37c0ed1fd7e9f278d88311be5b4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.1 MB (4120338 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad1e0c5709f39238c0ff863c80e1595fb5da12e230643dc6fd4bd6b33cda4039`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 02 Aug 2021 21:06:28 GMT
COPY file:d94287ad868b49da5d590782f3102415d5dfd4ed2a775b4e4c10280c8ab25db3 in /nats-server 
# Mon, 02 Aug 2021 21:06:29 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Mon, 02 Aug 2021 21:06:29 GMT
EXPOSE 4222 6222 8222
# Mon, 02 Aug 2021 21:06:29 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 02 Aug 2021 21:06:29 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4ecc856c82596f8b8982843cac0e5ec138e9c881bfd322038cd7cf0f4942c9c9`  
		Last Modified: Mon, 02 Aug 2021 21:07:52 GMT  
		Size: 4.1 MB (4119864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68fa4df40d0356fc86fe0d6c780d2a447fe1b2c32b5572c65a3c7d2354961da4`  
		Last Modified: Mon, 02 Aug 2021 21:07:51 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-windowsservercore`

```console
$ docker pull nats@sha256:d5e778d28d3d06f85d60c39772b380eb774d3f015b748c1491792a36c7a067f9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.2061; amd64
	-	windows version 10.0.14393.4530; amd64

### `nats:2-windowsservercore` - windows version 10.0.17763.2061; amd64

```console
$ docker pull nats@sha256:347fad05e489bf9e2c51d053e24efcce0d2031802c51a3feb8f4d2e7ab8765a9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2690730494 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1094808819e1865eaa575aa65800497b156f4e961675e37296ecd71758b68acf`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 06 Jul 2021 20:34:18 GMT
RUN Install update 1809-amd64
# Wed, 14 Jul 2021 01:07:27 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 14 Jul 2021 02:31:26 GMT
ENV NATS_DOCKERIZED=1
# Mon, 02 Aug 2021 21:14:23 GMT
ENV NATS_SERVER=2.3.3
# Mon, 02 Aug 2021 21:14:25 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.3.3/nats-server-v2.3.3-windows-amd64.zip
# Mon, 02 Aug 2021 21:14:28 GMT
ENV NATS_SERVER_SHASUM=dd14c9c104adb657de4a67a17bdf2fc7d7f55860e7a17ce0c6b9c117d9a50dde
# Mon, 02 Aug 2021 21:15:23 GMT
RUN Set-PSDebug -Trace 2
# Mon, 02 Aug 2021 21:16:45 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Mon, 02 Aug 2021 21:16:47 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Mon, 02 Aug 2021 21:16:49 GMT
EXPOSE 4222 6222 8222
# Mon, 02 Aug 2021 21:16:52 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Mon, 02 Aug 2021 21:16:54 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f143c6fed32d477c35b660b2e108ea62e3593c03e44bd9ced208ce52b26b0841`  
		Size: 967.1 MB (967113907 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:adcec6ff907307155c0652222cc9b95a0cc964d4c371e02767e72a5c90472192`  
		Last Modified: Wed, 14 Jul 2021 02:02:19 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f92bdc410321db22d4cf09322869bd9fb2495788c3725624c86d76a6ab3d95d3`  
		Last Modified: Wed, 14 Jul 2021 02:40:16 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c51291d3c5600cdb108e3ed994ab3d59042ca052eae615e136c35e3ac5f9bb6`  
		Last Modified: Mon, 02 Aug 2021 21:21:20 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:292fe7f01e91ae26c600f65e5c1f79e1cafd7d32145f63eda77265399a3c3804`  
		Last Modified: Mon, 02 Aug 2021 21:21:20 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17d5bb92d28832495b8124755df9034565b383dc7bc73be7f24838f425342d1a`  
		Last Modified: Mon, 02 Aug 2021 21:21:20 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8e0ae013ec15413637e098d44190826fe18ee0d434165a78f170bc86ce9c2fb`  
		Last Modified: Mon, 02 Aug 2021 21:21:20 GMT  
		Size: 364.2 KB (364232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4708b7da85335254f8c77a9656ef9c9034ed3d8d6df25e4621a4d1c0c4fce55e`  
		Last Modified: Mon, 02 Aug 2021 21:21:19 GMT  
		Size: 4.9 MB (4906167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88866e210b82ee16f0597e85bdb4ecfcfa4a4fb779acf4fac118727f77793da4`  
		Last Modified: Mon, 02 Aug 2021 21:21:17 GMT  
		Size: 2.0 KB (1963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b0d7cfeb38017cedd34bb386132d75c45a4680749166f4725a12ec569559074`  
		Last Modified: Mon, 02 Aug 2021 21:21:17 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:505a0140bcef7327375fc3aaaded24b5afac6d0507406776accf695315b15b45`  
		Last Modified: Mon, 02 Aug 2021 21:21:18 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:249b0508ccf09dee8b24a8f7319126a4e8aad55ba989a0d96252ad5e55bbcd2a`  
		Last Modified: Mon, 02 Aug 2021 21:21:17 GMT  
		Size: 1.4 KB (1356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-windowsservercore` - windows version 10.0.14393.4530; amd64

```console
$ docker pull nats@sha256:4d913e48d6a0ea2ed11c62cc9fff622727736be864fa3a7fe0f15c35fc4b7b6f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6274947967 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eff8abf4d3ed2a1c41241ff4223442903b563fe0a6d8be426bcaed438d42bbbf`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Fri, 09 Jul 2021 05:02:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 14 Jul 2021 01:14:25 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 14 Jul 2021 02:35:48 GMT
ENV NATS_DOCKERIZED=1
# Mon, 02 Aug 2021 21:17:24 GMT
ENV NATS_SERVER=2.3.3
# Mon, 02 Aug 2021 21:17:26 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.3.3/nats-server-v2.3.3-windows-amd64.zip
# Mon, 02 Aug 2021 21:17:28 GMT
ENV NATS_SERVER_SHASUM=dd14c9c104adb657de4a67a17bdf2fc7d7f55860e7a17ce0c6b9c117d9a50dde
# Mon, 02 Aug 2021 21:18:41 GMT
RUN Set-PSDebug -Trace 2
# Mon, 02 Aug 2021 21:20:28 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Mon, 02 Aug 2021 21:20:31 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Mon, 02 Aug 2021 21:20:33 GMT
EXPOSE 4222 6222 8222
# Mon, 02 Aug 2021 21:20:36 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Mon, 02 Aug 2021 21:20:38 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a567de41cc349380b25967f180fb1b6b2431bda61ccaaf69d78a33bc9523614a`  
		Size: 2.2 GB (2199646155 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:fed351b78c876c55ec9c7e75d3b9d1b146c5c5dfeb4b5480c0a7c384322df98c`  
		Last Modified: Wed, 14 Jul 2021 02:03:37 GMT  
		Size: 1.4 KB (1444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf08cae8b8db8f3f89e1a9192d393f2da55b44efce4e778fdb58debe2d608275`  
		Last Modified: Wed, 14 Jul 2021 02:40:57 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:278db267454aa76e00b506fdd53726da5583419a7844eaa96889ff07827a02b7`  
		Last Modified: Mon, 02 Aug 2021 21:21:56 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb231d65d7756b89dfbb667d5b24a7bf72ba86e6d5d9c111ab0d08e3e862dfeb`  
		Last Modified: Mon, 02 Aug 2021 21:21:56 GMT  
		Size: 1.4 KB (1371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfa0b0c97c4ebf872cafc434ce68ec59df2a3cc66e12e83e929b2d7264559729`  
		Last Modified: Mon, 02 Aug 2021 21:21:55 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fe01d11f12da0e487e1ccf3918b3f6a77405b4992df67bc7a092380599cb022`  
		Last Modified: Mon, 02 Aug 2021 21:21:56 GMT  
		Size: 364.5 KB (364483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5da4bfe4915750d7b0192abb4ef4e16913fc4d8746d369529feaead5f8ef2918`  
		Last Modified: Mon, 02 Aug 2021 21:21:59 GMT  
		Size: 4.9 MB (4938295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd26f2047cfc6ccce7d850ea9ec880c9890f783dd0fa4ea9102c561cfa2aa5b5`  
		Last Modified: Mon, 02 Aug 2021 21:21:53 GMT  
		Size: 2.0 KB (1962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce9a1c92d84c4bec202df1e1353e7ecaad58b85a2a2940a9297d14d4548d9e53`  
		Last Modified: Mon, 02 Aug 2021 21:21:53 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dda461d40f36bee8ad537d4225843e28f90f20e81aa8a552d3ada4ef4dbc9f7a`  
		Last Modified: Mon, 02 Aug 2021 21:21:53 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29bf964afbf31f7d4891dc65a1db75f1254d540945a2697c483cdb0375c9b825`  
		Last Modified: Mon, 02 Aug 2021 21:21:53 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-windowsservercore-1809`

```console
$ docker pull nats@sha256:1f0cbe04efcaa08eaf910fa921d81d21cc52ff521414b7b02ebbf2b5890f0763
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2061; amd64

### `nats:2-windowsservercore-1809` - windows version 10.0.17763.2061; amd64

```console
$ docker pull nats@sha256:347fad05e489bf9e2c51d053e24efcce0d2031802c51a3feb8f4d2e7ab8765a9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2690730494 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1094808819e1865eaa575aa65800497b156f4e961675e37296ecd71758b68acf`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 06 Jul 2021 20:34:18 GMT
RUN Install update 1809-amd64
# Wed, 14 Jul 2021 01:07:27 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 14 Jul 2021 02:31:26 GMT
ENV NATS_DOCKERIZED=1
# Mon, 02 Aug 2021 21:14:23 GMT
ENV NATS_SERVER=2.3.3
# Mon, 02 Aug 2021 21:14:25 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.3.3/nats-server-v2.3.3-windows-amd64.zip
# Mon, 02 Aug 2021 21:14:28 GMT
ENV NATS_SERVER_SHASUM=dd14c9c104adb657de4a67a17bdf2fc7d7f55860e7a17ce0c6b9c117d9a50dde
# Mon, 02 Aug 2021 21:15:23 GMT
RUN Set-PSDebug -Trace 2
# Mon, 02 Aug 2021 21:16:45 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Mon, 02 Aug 2021 21:16:47 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Mon, 02 Aug 2021 21:16:49 GMT
EXPOSE 4222 6222 8222
# Mon, 02 Aug 2021 21:16:52 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Mon, 02 Aug 2021 21:16:54 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f143c6fed32d477c35b660b2e108ea62e3593c03e44bd9ced208ce52b26b0841`  
		Size: 967.1 MB (967113907 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:adcec6ff907307155c0652222cc9b95a0cc964d4c371e02767e72a5c90472192`  
		Last Modified: Wed, 14 Jul 2021 02:02:19 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f92bdc410321db22d4cf09322869bd9fb2495788c3725624c86d76a6ab3d95d3`  
		Last Modified: Wed, 14 Jul 2021 02:40:16 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c51291d3c5600cdb108e3ed994ab3d59042ca052eae615e136c35e3ac5f9bb6`  
		Last Modified: Mon, 02 Aug 2021 21:21:20 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:292fe7f01e91ae26c600f65e5c1f79e1cafd7d32145f63eda77265399a3c3804`  
		Last Modified: Mon, 02 Aug 2021 21:21:20 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17d5bb92d28832495b8124755df9034565b383dc7bc73be7f24838f425342d1a`  
		Last Modified: Mon, 02 Aug 2021 21:21:20 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8e0ae013ec15413637e098d44190826fe18ee0d434165a78f170bc86ce9c2fb`  
		Last Modified: Mon, 02 Aug 2021 21:21:20 GMT  
		Size: 364.2 KB (364232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4708b7da85335254f8c77a9656ef9c9034ed3d8d6df25e4621a4d1c0c4fce55e`  
		Last Modified: Mon, 02 Aug 2021 21:21:19 GMT  
		Size: 4.9 MB (4906167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88866e210b82ee16f0597e85bdb4ecfcfa4a4fb779acf4fac118727f77793da4`  
		Last Modified: Mon, 02 Aug 2021 21:21:17 GMT  
		Size: 2.0 KB (1963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b0d7cfeb38017cedd34bb386132d75c45a4680749166f4725a12ec569559074`  
		Last Modified: Mon, 02 Aug 2021 21:21:17 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:505a0140bcef7327375fc3aaaded24b5afac6d0507406776accf695315b15b45`  
		Last Modified: Mon, 02 Aug 2021 21:21:18 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:249b0508ccf09dee8b24a8f7319126a4e8aad55ba989a0d96252ad5e55bbcd2a`  
		Last Modified: Mon, 02 Aug 2021 21:21:17 GMT  
		Size: 1.4 KB (1356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-windowsservercore-ltsc2016`

```console
$ docker pull nats@sha256:a9dd3bec26866787cd33035a57d380c31c2f13a9b85f2d6d34a1b8bc79f3f9ff
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.14393.4530; amd64

### `nats:2-windowsservercore-ltsc2016` - windows version 10.0.14393.4530; amd64

```console
$ docker pull nats@sha256:4d913e48d6a0ea2ed11c62cc9fff622727736be864fa3a7fe0f15c35fc4b7b6f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6274947967 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eff8abf4d3ed2a1c41241ff4223442903b563fe0a6d8be426bcaed438d42bbbf`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Fri, 09 Jul 2021 05:02:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 14 Jul 2021 01:14:25 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 14 Jul 2021 02:35:48 GMT
ENV NATS_DOCKERIZED=1
# Mon, 02 Aug 2021 21:17:24 GMT
ENV NATS_SERVER=2.3.3
# Mon, 02 Aug 2021 21:17:26 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.3.3/nats-server-v2.3.3-windows-amd64.zip
# Mon, 02 Aug 2021 21:17:28 GMT
ENV NATS_SERVER_SHASUM=dd14c9c104adb657de4a67a17bdf2fc7d7f55860e7a17ce0c6b9c117d9a50dde
# Mon, 02 Aug 2021 21:18:41 GMT
RUN Set-PSDebug -Trace 2
# Mon, 02 Aug 2021 21:20:28 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Mon, 02 Aug 2021 21:20:31 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Mon, 02 Aug 2021 21:20:33 GMT
EXPOSE 4222 6222 8222
# Mon, 02 Aug 2021 21:20:36 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Mon, 02 Aug 2021 21:20:38 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a567de41cc349380b25967f180fb1b6b2431bda61ccaaf69d78a33bc9523614a`  
		Size: 2.2 GB (2199646155 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:fed351b78c876c55ec9c7e75d3b9d1b146c5c5dfeb4b5480c0a7c384322df98c`  
		Last Modified: Wed, 14 Jul 2021 02:03:37 GMT  
		Size: 1.4 KB (1444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf08cae8b8db8f3f89e1a9192d393f2da55b44efce4e778fdb58debe2d608275`  
		Last Modified: Wed, 14 Jul 2021 02:40:57 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:278db267454aa76e00b506fdd53726da5583419a7844eaa96889ff07827a02b7`  
		Last Modified: Mon, 02 Aug 2021 21:21:56 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb231d65d7756b89dfbb667d5b24a7bf72ba86e6d5d9c111ab0d08e3e862dfeb`  
		Last Modified: Mon, 02 Aug 2021 21:21:56 GMT  
		Size: 1.4 KB (1371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfa0b0c97c4ebf872cafc434ce68ec59df2a3cc66e12e83e929b2d7264559729`  
		Last Modified: Mon, 02 Aug 2021 21:21:55 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fe01d11f12da0e487e1ccf3918b3f6a77405b4992df67bc7a092380599cb022`  
		Last Modified: Mon, 02 Aug 2021 21:21:56 GMT  
		Size: 364.5 KB (364483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5da4bfe4915750d7b0192abb4ef4e16913fc4d8746d369529feaead5f8ef2918`  
		Last Modified: Mon, 02 Aug 2021 21:21:59 GMT  
		Size: 4.9 MB (4938295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd26f2047cfc6ccce7d850ea9ec880c9890f783dd0fa4ea9102c561cfa2aa5b5`  
		Last Modified: Mon, 02 Aug 2021 21:21:53 GMT  
		Size: 2.0 KB (1962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce9a1c92d84c4bec202df1e1353e7ecaad58b85a2a2940a9297d14d4548d9e53`  
		Last Modified: Mon, 02 Aug 2021 21:21:53 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dda461d40f36bee8ad537d4225843e28f90f20e81aa8a552d3ada4ef4dbc9f7a`  
		Last Modified: Mon, 02 Aug 2021 21:21:53 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29bf964afbf31f7d4891dc65a1db75f1254d540945a2697c483cdb0375c9b825`  
		Last Modified: Mon, 02 Aug 2021 21:21:53 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.3`

```console
$ docker pull nats@sha256:6923c5f75f670dabe310c5dc2d3242e4f9ad4f1eabc625e18716358427ccd8d1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.2061; amd64

### `nats:2.3` - linux; amd64

```console
$ docker pull nats@sha256:4f6857e56d3555432c7bc830fb297d8c00cbe3b0522f81dfc8c84a4dacb54ed5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4505352 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23830fcc7f9834fd409d95d2bf9877f21b609b7b7392bfcd4b8b5e62e8be14fc`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 02 Aug 2021 21:23:05 GMT
COPY file:0b22daa17d88302a2606c64df249d26684c5926e82494be3f08d920922b75196 in /nats-server 
# Mon, 02 Aug 2021 21:23:05 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Mon, 02 Aug 2021 21:23:05 GMT
EXPOSE 4222 6222 8222
# Mon, 02 Aug 2021 21:23:05 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 02 Aug 2021 21:23:05 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:267760e6058167430070f7584ea1e5e18b4ddf538aec80d4b764ba1b9096b403`  
		Last Modified: Mon, 02 Aug 2021 21:23:56 GMT  
		Size: 4.5 MB (4504877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:612bea9c73fc6c5c02659a6bff01f1bcada2f4c47323021b03bee52a9ca1eba0`  
		Last Modified: Mon, 02 Aug 2021 21:23:55 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.3` - linux; arm variant v6

```console
$ docker pull nats@sha256:6e42eec5a210d9a5b6d95c179d5c55193b69846c76786a81908536eac2efbdc3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4173716 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31e1feb9bf2ac457664507fc7899f48e45d49df93dd60eacdea8b8a9cda8ec51`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 02 Aug 2021 21:17:15 GMT
COPY file:55e1c39fb6ec9785ddf1c189ad5438b9f306c3e1c2a355512f4efc73aa1aacf6 in /nats-server 
# Mon, 02 Aug 2021 21:17:15 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Mon, 02 Aug 2021 21:17:16 GMT
EXPOSE 4222 6222 8222
# Mon, 02 Aug 2021 21:17:16 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 02 Aug 2021 21:17:17 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:7f318c30554fccfe6a5ac8a63f4457a20876b88ede949510db6a8f1c5bcf1442`  
		Last Modified: Mon, 02 Aug 2021 21:19:37 GMT  
		Size: 4.2 MB (4173243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76c9419bcd494c007ef4d4f83649e535bb32d84c81337abb67e153ad75a1fb5f`  
		Last Modified: Mon, 02 Aug 2021 21:19:35 GMT  
		Size: 473.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.3` - linux; arm variant v7

```console
$ docker pull nats@sha256:def02210305c7940addd2f5e26e8417017a2f2ae11116ee001b8f2a7bcb17bff
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.0 MB (3992886 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:20941bb671159cef8cb5d6b9047f5c6c298a495274b06f9c6d9278ea5f9e5a1f`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 07 Jul 2021 06:38:20 GMT
COPY file:a259b6f87cc2d22082524e5ba23201057e836734749f0d28676e8637d920d385 in /nats-server 
# Wed, 07 Jul 2021 06:38:21 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Wed, 07 Jul 2021 06:38:21 GMT
EXPOSE 4222 6222 8222
# Wed, 07 Jul 2021 06:38:22 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 07 Jul 2021 06:38:22 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:434fc0c4a6c5daa82c731102728bcac575b5a312862a89edf401b0305d2efc82`  
		Last Modified: Wed, 07 Jul 2021 06:40:42 GMT  
		Size: 4.0 MB (3992410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c195f08925b050ce566763c31c813f3d8c7e1ba40bc4ccdf0949cb87373c3a43`  
		Last Modified: Wed, 07 Jul 2021 06:40:39 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.3` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:7a367e1495e9df2cf9cc81af565194815e52b37c0ed1fd7e9f278d88311be5b4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.1 MB (4120338 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad1e0c5709f39238c0ff863c80e1595fb5da12e230643dc6fd4bd6b33cda4039`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 02 Aug 2021 21:06:28 GMT
COPY file:d94287ad868b49da5d590782f3102415d5dfd4ed2a775b4e4c10280c8ab25db3 in /nats-server 
# Mon, 02 Aug 2021 21:06:29 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Mon, 02 Aug 2021 21:06:29 GMT
EXPOSE 4222 6222 8222
# Mon, 02 Aug 2021 21:06:29 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 02 Aug 2021 21:06:29 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4ecc856c82596f8b8982843cac0e5ec138e9c881bfd322038cd7cf0f4942c9c9`  
		Last Modified: Mon, 02 Aug 2021 21:07:52 GMT  
		Size: 4.1 MB (4119864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68fa4df40d0356fc86fe0d6c780d2a447fe1b2c32b5572c65a3c7d2354961da4`  
		Last Modified: Mon, 02 Aug 2021 21:07:51 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.3` - windows version 10.0.17763.2061; amd64

```console
$ docker pull nats@sha256:baf086eb51e7090cb2ef985758c034c882cbe1dd8d4b2a682a618d32b9215e35
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.3 MB (107296331 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d57bb9c1561692bbad5576428cd8e22189f1addf3a8b82e73e3f27e246bd485`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 06 Jul 2021 20:06:39 GMT
RUN Apply image 1809-amd64
# Wed, 14 Jul 2021 02:35:24 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Mon, 02 Aug 2021 21:17:05 GMT
RUN cmd /S /C #(nop) COPY file:359dd4a92709029cd62dc9620a8ff30527cb3494d6b89c9332ae019bae51b57b in C:\nats-server.exe 
# Mon, 02 Aug 2021 21:17:08 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Mon, 02 Aug 2021 21:17:10 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Mon, 02 Aug 2021 21:17:13 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Mon, 02 Aug 2021 21:17:16 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:29d43e56445c5279a6386c4dfe4d1ada3c7124ade9cb7b0f2757e58ffc7cd10b`  
		Size: 102.7 MB (102725622 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ec20c4c9f6fa5e782e09342d50033ef24c4049a9dad1befd33c96759b71da6de`  
		Last Modified: Wed, 14 Jul 2021 02:40:36 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab54ee8cb88b349708e6f2d10afe13c1d843b9c1ff995a70d40af5ca886eda42`  
		Last Modified: Mon, 02 Aug 2021 21:21:37 GMT  
		Size: 4.6 MB (4564319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27d161923a9b16db535efc5f78e4aedd08225387cc8377cedb826e7539fa9051`  
		Last Modified: Mon, 02 Aug 2021 21:21:36 GMT  
		Size: 1.8 KB (1766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e88c4ba846a11b45abc01afc7de665b15430ebfd4c6e585ba8cb11d896017cd`  
		Last Modified: Mon, 02 Aug 2021 21:21:36 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26ca1fda898c73546bdd8f1655f276fe9a0911a7c16f5a4054cdb40e996692c2`  
		Last Modified: Mon, 02 Aug 2021 21:21:36 GMT  
		Size: 1.2 KB (1180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:088b6cb05a147f4faf4e14f0fc1ecda8481f5ad0a8741dba786aebba4374207b`  
		Last Modified: Mon, 02 Aug 2021 21:21:36 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.3-alpine`

```console
$ docker pull nats@sha256:3ec525b1d139794286ecdb26410cff8ccf814eca88de9fe23c39a7d4b58479ef
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.3-alpine` - linux; amd64

```console
$ docker pull nats@sha256:b430407bf4008593c12a2cc85208f72e96b53fec98b30187c517b9d1958b657e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7601531 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:37a8e948168fcd8c0825a0cd425eb489bd313da994d65e73b5072d6ff6c8225a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 15 Jun 2021 22:19:37 GMT
ADD file:f278386b0cef68136129f5f58c52445590a417b624d62bca158d4dc926c340df in / 
# Tue, 15 Jun 2021 22:19:37 GMT
CMD ["/bin/sh"]
# Mon, 02 Aug 2021 21:22:41 GMT
ENV NATS_SERVER=2.3.3
# Mon, 02 Aug 2021 21:22:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f8e04470165fdfba062442cf5975f22668ab20fb12df7e299734e16a45370bef' ;; 		armhf) natsArch='arm6'; sha256='6396531f34e99cca903cdd461a79f1b8255d0cc219e5186ea15284b5b5e7e5e7' ;; 		armv7) natsArch='arm7'; sha256='4353de84d9e42b24b73ba98a4ed2a9eaa7c4f945bd68e1ddb4fbde885020ab30' ;; 		x86_64) natsArch='amd64'; sha256='66703b81de34d06060eb2198dfb5a1087547d45e680dee4da1214198a8073ce5' ;; 		x86) natsArch='386'; sha256='e38b9c9eda279bc4eee9cf6a3d4b2b25774b692450421a16e2ff6602977e6571' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Mon, 02 Aug 2021 21:22:44 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Mon, 02 Aug 2021 21:22:44 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 02 Aug 2021 21:22:44 GMT
EXPOSE 4222 6222 8222
# Mon, 02 Aug 2021 21:22:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 02 Aug 2021 21:22:45 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:5843afab387455b37944e709ee8c78d7520df80f8d01cf7f861aae63beeddb6b`  
		Last Modified: Tue, 15 Jun 2021 22:20:04 GMT  
		Size: 2.8 MB (2811478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03113b330e4f7fe35234354441a5bc0f8cabb61f7e7c02e1c2c7a9002be630c7`  
		Last Modified: Mon, 02 Aug 2021 21:23:32 GMT  
		Size: 4.8 MB (4789084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe9957a382ed4e85c0797d4c958c23eb4c68ab7e84a78c07a137bbf4bfd93c86`  
		Last Modified: Mon, 02 Aug 2021 21:23:31 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51734fe5b37d3390b972f615a9b12d4454a30ce0ed124f4a5d0f91a17d6ce6f8`  
		Last Modified: Mon, 02 Aug 2021 21:23:30 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.3-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:d5fc2c9df074891880beadedf530ee3dbf0761259a14619e946c1cefa842cac3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7079723 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f49351bac7a37d427b25fbdcc43daa3d1ea704fe96f3931802df83f01bf235c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 30 Jul 2021 17:49:42 GMT
ADD file:c80bc2b093cbc0fc466582ef21cbed377de9fa874aedbf320079525ddacd1200 in / 
# Fri, 30 Jul 2021 17:49:42 GMT
CMD ["/bin/sh"]
# Mon, 02 Aug 2021 21:16:47 GMT
ENV NATS_SERVER=2.3.3
# Mon, 02 Aug 2021 21:16:52 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f8e04470165fdfba062442cf5975f22668ab20fb12df7e299734e16a45370bef' ;; 		armhf) natsArch='arm6'; sha256='6396531f34e99cca903cdd461a79f1b8255d0cc219e5186ea15284b5b5e7e5e7' ;; 		armv7) natsArch='arm7'; sha256='4353de84d9e42b24b73ba98a4ed2a9eaa7c4f945bd68e1ddb4fbde885020ab30' ;; 		x86_64) natsArch='amd64'; sha256='66703b81de34d06060eb2198dfb5a1087547d45e680dee4da1214198a8073ce5' ;; 		x86) natsArch='386'; sha256='e38b9c9eda279bc4eee9cf6a3d4b2b25774b692450421a16e2ff6602977e6571' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Mon, 02 Aug 2021 21:16:52 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Mon, 02 Aug 2021 21:16:53 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 02 Aug 2021 21:16:53 GMT
EXPOSE 4222 6222 8222
# Mon, 02 Aug 2021 21:16:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 02 Aug 2021 21:16:54 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:b4c9a0924271af3466de27804af26420eb58da1466e7eaaba127d178b380fea3`  
		Last Modified: Tue, 15 Jun 2021 22:58:47 GMT  
		Size: 2.6 MB (2624382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e3313ef1b9ecd8d9e94997ae371b1c0aabda27773f0b2e12b4be7463517cf87`  
		Last Modified: Mon, 02 Aug 2021 21:18:59 GMT  
		Size: 4.5 MB (4454370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:785fbb490293d9c2f8cdaed64735e76ea2a0dc1c40e13814102053f6d9c4ddc3`  
		Last Modified: Mon, 02 Aug 2021 21:18:56 GMT  
		Size: 557.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ee9f0a3fdc78fe2942c2a3d6969418df884ad628f52adb50525f4022ed56ec2`  
		Last Modified: Mon, 02 Aug 2021 21:18:56 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.3-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:0cd94d122e5dd418d4d447257c6622e13c1d86149c0e7979057664951ab5a020
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.7 MB (6703143 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5635c4604b79a25fc3fdf3ccf6606d69eb347b3e8a3cb756dd261e2ca83e780`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 30 Jul 2021 18:36:19 GMT
ADD file:416a8b507abdc6bdcb22997a4be0a4170796c3f9f77e315b2dbff2b0a212bc68 in / 
# Fri, 30 Jul 2021 18:36:20 GMT
CMD ["/bin/sh"]
# Sat, 31 Jul 2021 03:13:57 GMT
ENV NATS_SERVER=2.3.2
# Sat, 31 Jul 2021 03:14:02 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='18a68cbef5c7a41052f5281bdfe9164b51cbeb60ce2dd31a7945c5adbcd39c2d' ;; 		armhf) natsArch='arm6'; sha256='a37949f8a1e24d5a8e47f57786e126205de7c3f6f8b3e5b849f33adbcfe8d2fb' ;; 		armv7) natsArch='arm7'; sha256='43a4820a57161b83fe721b81098d2ba9b1e2f42923be898f031bac40279f8f6e' ;; 		x86_64) natsArch='amd64'; sha256='6e6fdf781465fbf09cb024112b34ae6b2b432d94a5fc8b62f6ebf0da5fc3345d' ;; 		x86) natsArch='386'; sha256='c7c0ea9a5343925f0f5e2dda964946152382b0a3e0db96aa43c3f2ab17a37bf0' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Sat, 31 Jul 2021 03:14:03 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Sat, 31 Jul 2021 03:14:03 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Sat, 31 Jul 2021 03:14:04 GMT
EXPOSE 4222 6222 8222
# Sat, 31 Jul 2021 03:14:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 31 Jul 2021 03:14:05 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:136482bf81d1fa351b424ebb8c7e34d15f2c5ed3fc0b66b544b8312bda3d52d9`  
		Last Modified: Tue, 15 Jun 2021 23:16:40 GMT  
		Size: 2.4 MB (2427917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1a0b8bfe79fe7add5c0f3af812a506d01cc94a574cd58ba1f81146318d3638c`  
		Last Modified: Sat, 31 Jul 2021 03:16:43 GMT  
		Size: 4.3 MB (4274251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c35ac8f58b7f43ebc215a5713841cf5a94983b092019cf46da7ce8a3c9c84146`  
		Last Modified: Sat, 31 Jul 2021 03:16:40 GMT  
		Size: 560.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:735e5b5c342cb95f3f2eb33812321a4305479b159555d6fed062e4bb2880dc66`  
		Last Modified: Sat, 31 Jul 2021 03:16:40 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.3-alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:f818c9007861b8440d5c89a859f8f20f483637ab3f3e7c7a7f89ef40afd23937
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7113993 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc01fa8c08e4612961dfe7cf6c422a1a58b99637fd0297f9c3d811b95a32c185`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 15 Jun 2021 21:44:56 GMT
ADD file:6797caacbfe41bfe44000b39ed017016c6fcc492b3d6557cdaba88536df6c876 in / 
# Tue, 15 Jun 2021 21:44:56 GMT
CMD ["/bin/sh"]
# Mon, 02 Aug 2021 21:06:09 GMT
ENV NATS_SERVER=2.3.3
# Mon, 02 Aug 2021 21:06:11 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f8e04470165fdfba062442cf5975f22668ab20fb12df7e299734e16a45370bef' ;; 		armhf) natsArch='arm6'; sha256='6396531f34e99cca903cdd461a79f1b8255d0cc219e5186ea15284b5b5e7e5e7' ;; 		armv7) natsArch='arm7'; sha256='4353de84d9e42b24b73ba98a4ed2a9eaa7c4f945bd68e1ddb4fbde885020ab30' ;; 		x86_64) natsArch='amd64'; sha256='66703b81de34d06060eb2198dfb5a1087547d45e680dee4da1214198a8073ce5' ;; 		x86) natsArch='386'; sha256='e38b9c9eda279bc4eee9cf6a3d4b2b25774b692450421a16e2ff6602977e6571' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Mon, 02 Aug 2021 21:06:11 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Mon, 02 Aug 2021 21:06:12 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 02 Aug 2021 21:06:12 GMT
EXPOSE 4222 6222 8222
# Mon, 02 Aug 2021 21:06:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 02 Aug 2021 21:06:12 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:58ab47519297212468320b23b8100fc1b2b96e8d342040806ae509a778a0a07a`  
		Last Modified: Tue, 15 Jun 2021 21:46:03 GMT  
		Size: 2.7 MB (2709626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0b71cb50e81b94a1183dec31a916ec92da12268c9d5c01358f63f093176829d`  
		Last Modified: Mon, 02 Aug 2021 21:07:22 GMT  
		Size: 4.4 MB (4403398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69e71c9cdab2ba7a29d11ef463c8173ea1cdc1f4a0a549ee1d8bdf0a21392641`  
		Last Modified: Mon, 02 Aug 2021 21:07:21 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17f4a027c87d570eda83fa005f1747518d8e6f172eaf1f5432d6073835418317`  
		Last Modified: Mon, 02 Aug 2021 21:07:21 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.3-alpine3.14`

```console
$ docker pull nats@sha256:3ec525b1d139794286ecdb26410cff8ccf814eca88de9fe23c39a7d4b58479ef
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.3-alpine3.14` - linux; amd64

```console
$ docker pull nats@sha256:b430407bf4008593c12a2cc85208f72e96b53fec98b30187c517b9d1958b657e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7601531 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:37a8e948168fcd8c0825a0cd425eb489bd313da994d65e73b5072d6ff6c8225a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 15 Jun 2021 22:19:37 GMT
ADD file:f278386b0cef68136129f5f58c52445590a417b624d62bca158d4dc926c340df in / 
# Tue, 15 Jun 2021 22:19:37 GMT
CMD ["/bin/sh"]
# Mon, 02 Aug 2021 21:22:41 GMT
ENV NATS_SERVER=2.3.3
# Mon, 02 Aug 2021 21:22:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f8e04470165fdfba062442cf5975f22668ab20fb12df7e299734e16a45370bef' ;; 		armhf) natsArch='arm6'; sha256='6396531f34e99cca903cdd461a79f1b8255d0cc219e5186ea15284b5b5e7e5e7' ;; 		armv7) natsArch='arm7'; sha256='4353de84d9e42b24b73ba98a4ed2a9eaa7c4f945bd68e1ddb4fbde885020ab30' ;; 		x86_64) natsArch='amd64'; sha256='66703b81de34d06060eb2198dfb5a1087547d45e680dee4da1214198a8073ce5' ;; 		x86) natsArch='386'; sha256='e38b9c9eda279bc4eee9cf6a3d4b2b25774b692450421a16e2ff6602977e6571' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Mon, 02 Aug 2021 21:22:44 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Mon, 02 Aug 2021 21:22:44 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 02 Aug 2021 21:22:44 GMT
EXPOSE 4222 6222 8222
# Mon, 02 Aug 2021 21:22:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 02 Aug 2021 21:22:45 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:5843afab387455b37944e709ee8c78d7520df80f8d01cf7f861aae63beeddb6b`  
		Last Modified: Tue, 15 Jun 2021 22:20:04 GMT  
		Size: 2.8 MB (2811478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03113b330e4f7fe35234354441a5bc0f8cabb61f7e7c02e1c2c7a9002be630c7`  
		Last Modified: Mon, 02 Aug 2021 21:23:32 GMT  
		Size: 4.8 MB (4789084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe9957a382ed4e85c0797d4c958c23eb4c68ab7e84a78c07a137bbf4bfd93c86`  
		Last Modified: Mon, 02 Aug 2021 21:23:31 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51734fe5b37d3390b972f615a9b12d4454a30ce0ed124f4a5d0f91a17d6ce6f8`  
		Last Modified: Mon, 02 Aug 2021 21:23:30 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.3-alpine3.14` - linux; arm variant v6

```console
$ docker pull nats@sha256:d5fc2c9df074891880beadedf530ee3dbf0761259a14619e946c1cefa842cac3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7079723 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f49351bac7a37d427b25fbdcc43daa3d1ea704fe96f3931802df83f01bf235c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 30 Jul 2021 17:49:42 GMT
ADD file:c80bc2b093cbc0fc466582ef21cbed377de9fa874aedbf320079525ddacd1200 in / 
# Fri, 30 Jul 2021 17:49:42 GMT
CMD ["/bin/sh"]
# Mon, 02 Aug 2021 21:16:47 GMT
ENV NATS_SERVER=2.3.3
# Mon, 02 Aug 2021 21:16:52 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f8e04470165fdfba062442cf5975f22668ab20fb12df7e299734e16a45370bef' ;; 		armhf) natsArch='arm6'; sha256='6396531f34e99cca903cdd461a79f1b8255d0cc219e5186ea15284b5b5e7e5e7' ;; 		armv7) natsArch='arm7'; sha256='4353de84d9e42b24b73ba98a4ed2a9eaa7c4f945bd68e1ddb4fbde885020ab30' ;; 		x86_64) natsArch='amd64'; sha256='66703b81de34d06060eb2198dfb5a1087547d45e680dee4da1214198a8073ce5' ;; 		x86) natsArch='386'; sha256='e38b9c9eda279bc4eee9cf6a3d4b2b25774b692450421a16e2ff6602977e6571' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Mon, 02 Aug 2021 21:16:52 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Mon, 02 Aug 2021 21:16:53 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 02 Aug 2021 21:16:53 GMT
EXPOSE 4222 6222 8222
# Mon, 02 Aug 2021 21:16:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 02 Aug 2021 21:16:54 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:b4c9a0924271af3466de27804af26420eb58da1466e7eaaba127d178b380fea3`  
		Last Modified: Tue, 15 Jun 2021 22:58:47 GMT  
		Size: 2.6 MB (2624382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e3313ef1b9ecd8d9e94997ae371b1c0aabda27773f0b2e12b4be7463517cf87`  
		Last Modified: Mon, 02 Aug 2021 21:18:59 GMT  
		Size: 4.5 MB (4454370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:785fbb490293d9c2f8cdaed64735e76ea2a0dc1c40e13814102053f6d9c4ddc3`  
		Last Modified: Mon, 02 Aug 2021 21:18:56 GMT  
		Size: 557.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ee9f0a3fdc78fe2942c2a3d6969418df884ad628f52adb50525f4022ed56ec2`  
		Last Modified: Mon, 02 Aug 2021 21:18:56 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.3-alpine3.14` - linux; arm variant v7

```console
$ docker pull nats@sha256:0cd94d122e5dd418d4d447257c6622e13c1d86149c0e7979057664951ab5a020
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.7 MB (6703143 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5635c4604b79a25fc3fdf3ccf6606d69eb347b3e8a3cb756dd261e2ca83e780`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 30 Jul 2021 18:36:19 GMT
ADD file:416a8b507abdc6bdcb22997a4be0a4170796c3f9f77e315b2dbff2b0a212bc68 in / 
# Fri, 30 Jul 2021 18:36:20 GMT
CMD ["/bin/sh"]
# Sat, 31 Jul 2021 03:13:57 GMT
ENV NATS_SERVER=2.3.2
# Sat, 31 Jul 2021 03:14:02 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='18a68cbef5c7a41052f5281bdfe9164b51cbeb60ce2dd31a7945c5adbcd39c2d' ;; 		armhf) natsArch='arm6'; sha256='a37949f8a1e24d5a8e47f57786e126205de7c3f6f8b3e5b849f33adbcfe8d2fb' ;; 		armv7) natsArch='arm7'; sha256='43a4820a57161b83fe721b81098d2ba9b1e2f42923be898f031bac40279f8f6e' ;; 		x86_64) natsArch='amd64'; sha256='6e6fdf781465fbf09cb024112b34ae6b2b432d94a5fc8b62f6ebf0da5fc3345d' ;; 		x86) natsArch='386'; sha256='c7c0ea9a5343925f0f5e2dda964946152382b0a3e0db96aa43c3f2ab17a37bf0' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Sat, 31 Jul 2021 03:14:03 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Sat, 31 Jul 2021 03:14:03 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Sat, 31 Jul 2021 03:14:04 GMT
EXPOSE 4222 6222 8222
# Sat, 31 Jul 2021 03:14:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 31 Jul 2021 03:14:05 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:136482bf81d1fa351b424ebb8c7e34d15f2c5ed3fc0b66b544b8312bda3d52d9`  
		Last Modified: Tue, 15 Jun 2021 23:16:40 GMT  
		Size: 2.4 MB (2427917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1a0b8bfe79fe7add5c0f3af812a506d01cc94a574cd58ba1f81146318d3638c`  
		Last Modified: Sat, 31 Jul 2021 03:16:43 GMT  
		Size: 4.3 MB (4274251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c35ac8f58b7f43ebc215a5713841cf5a94983b092019cf46da7ce8a3c9c84146`  
		Last Modified: Sat, 31 Jul 2021 03:16:40 GMT  
		Size: 560.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:735e5b5c342cb95f3f2eb33812321a4305479b159555d6fed062e4bb2880dc66`  
		Last Modified: Sat, 31 Jul 2021 03:16:40 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.3-alpine3.14` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:f818c9007861b8440d5c89a859f8f20f483637ab3f3e7c7a7f89ef40afd23937
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7113993 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc01fa8c08e4612961dfe7cf6c422a1a58b99637fd0297f9c3d811b95a32c185`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 15 Jun 2021 21:44:56 GMT
ADD file:6797caacbfe41bfe44000b39ed017016c6fcc492b3d6557cdaba88536df6c876 in / 
# Tue, 15 Jun 2021 21:44:56 GMT
CMD ["/bin/sh"]
# Mon, 02 Aug 2021 21:06:09 GMT
ENV NATS_SERVER=2.3.3
# Mon, 02 Aug 2021 21:06:11 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f8e04470165fdfba062442cf5975f22668ab20fb12df7e299734e16a45370bef' ;; 		armhf) natsArch='arm6'; sha256='6396531f34e99cca903cdd461a79f1b8255d0cc219e5186ea15284b5b5e7e5e7' ;; 		armv7) natsArch='arm7'; sha256='4353de84d9e42b24b73ba98a4ed2a9eaa7c4f945bd68e1ddb4fbde885020ab30' ;; 		x86_64) natsArch='amd64'; sha256='66703b81de34d06060eb2198dfb5a1087547d45e680dee4da1214198a8073ce5' ;; 		x86) natsArch='386'; sha256='e38b9c9eda279bc4eee9cf6a3d4b2b25774b692450421a16e2ff6602977e6571' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Mon, 02 Aug 2021 21:06:11 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Mon, 02 Aug 2021 21:06:12 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 02 Aug 2021 21:06:12 GMT
EXPOSE 4222 6222 8222
# Mon, 02 Aug 2021 21:06:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 02 Aug 2021 21:06:12 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:58ab47519297212468320b23b8100fc1b2b96e8d342040806ae509a778a0a07a`  
		Last Modified: Tue, 15 Jun 2021 21:46:03 GMT  
		Size: 2.7 MB (2709626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0b71cb50e81b94a1183dec31a916ec92da12268c9d5c01358f63f093176829d`  
		Last Modified: Mon, 02 Aug 2021 21:07:22 GMT  
		Size: 4.4 MB (4403398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69e71c9cdab2ba7a29d11ef463c8173ea1cdc1f4a0a549ee1d8bdf0a21392641`  
		Last Modified: Mon, 02 Aug 2021 21:07:21 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17f4a027c87d570eda83fa005f1747518d8e6f172eaf1f5432d6073835418317`  
		Last Modified: Mon, 02 Aug 2021 21:07:21 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.3-linux`

```console
$ docker pull nats@sha256:111aefb3002e16ecc001abaa0bb5fc9aabf2510005be379d2cedc0373fa1e596
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.3-linux` - linux; amd64

```console
$ docker pull nats@sha256:4f6857e56d3555432c7bc830fb297d8c00cbe3b0522f81dfc8c84a4dacb54ed5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4505352 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23830fcc7f9834fd409d95d2bf9877f21b609b7b7392bfcd4b8b5e62e8be14fc`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 02 Aug 2021 21:23:05 GMT
COPY file:0b22daa17d88302a2606c64df249d26684c5926e82494be3f08d920922b75196 in /nats-server 
# Mon, 02 Aug 2021 21:23:05 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Mon, 02 Aug 2021 21:23:05 GMT
EXPOSE 4222 6222 8222
# Mon, 02 Aug 2021 21:23:05 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 02 Aug 2021 21:23:05 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:267760e6058167430070f7584ea1e5e18b4ddf538aec80d4b764ba1b9096b403`  
		Last Modified: Mon, 02 Aug 2021 21:23:56 GMT  
		Size: 4.5 MB (4504877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:612bea9c73fc6c5c02659a6bff01f1bcada2f4c47323021b03bee52a9ca1eba0`  
		Last Modified: Mon, 02 Aug 2021 21:23:55 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.3-linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:6e42eec5a210d9a5b6d95c179d5c55193b69846c76786a81908536eac2efbdc3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4173716 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31e1feb9bf2ac457664507fc7899f48e45d49df93dd60eacdea8b8a9cda8ec51`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 02 Aug 2021 21:17:15 GMT
COPY file:55e1c39fb6ec9785ddf1c189ad5438b9f306c3e1c2a355512f4efc73aa1aacf6 in /nats-server 
# Mon, 02 Aug 2021 21:17:15 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Mon, 02 Aug 2021 21:17:16 GMT
EXPOSE 4222 6222 8222
# Mon, 02 Aug 2021 21:17:16 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 02 Aug 2021 21:17:17 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:7f318c30554fccfe6a5ac8a63f4457a20876b88ede949510db6a8f1c5bcf1442`  
		Last Modified: Mon, 02 Aug 2021 21:19:37 GMT  
		Size: 4.2 MB (4173243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76c9419bcd494c007ef4d4f83649e535bb32d84c81337abb67e153ad75a1fb5f`  
		Last Modified: Mon, 02 Aug 2021 21:19:35 GMT  
		Size: 473.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.3-linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:def02210305c7940addd2f5e26e8417017a2f2ae11116ee001b8f2a7bcb17bff
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.0 MB (3992886 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:20941bb671159cef8cb5d6b9047f5c6c298a495274b06f9c6d9278ea5f9e5a1f`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 07 Jul 2021 06:38:20 GMT
COPY file:a259b6f87cc2d22082524e5ba23201057e836734749f0d28676e8637d920d385 in /nats-server 
# Wed, 07 Jul 2021 06:38:21 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Wed, 07 Jul 2021 06:38:21 GMT
EXPOSE 4222 6222 8222
# Wed, 07 Jul 2021 06:38:22 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 07 Jul 2021 06:38:22 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:434fc0c4a6c5daa82c731102728bcac575b5a312862a89edf401b0305d2efc82`  
		Last Modified: Wed, 07 Jul 2021 06:40:42 GMT  
		Size: 4.0 MB (3992410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c195f08925b050ce566763c31c813f3d8c7e1ba40bc4ccdf0949cb87373c3a43`  
		Last Modified: Wed, 07 Jul 2021 06:40:39 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.3-linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:7a367e1495e9df2cf9cc81af565194815e52b37c0ed1fd7e9f278d88311be5b4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.1 MB (4120338 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad1e0c5709f39238c0ff863c80e1595fb5da12e230643dc6fd4bd6b33cda4039`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 02 Aug 2021 21:06:28 GMT
COPY file:d94287ad868b49da5d590782f3102415d5dfd4ed2a775b4e4c10280c8ab25db3 in /nats-server 
# Mon, 02 Aug 2021 21:06:29 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Mon, 02 Aug 2021 21:06:29 GMT
EXPOSE 4222 6222 8222
# Mon, 02 Aug 2021 21:06:29 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 02 Aug 2021 21:06:29 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4ecc856c82596f8b8982843cac0e5ec138e9c881bfd322038cd7cf0f4942c9c9`  
		Last Modified: Mon, 02 Aug 2021 21:07:52 GMT  
		Size: 4.1 MB (4119864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68fa4df40d0356fc86fe0d6c780d2a447fe1b2c32b5572c65a3c7d2354961da4`  
		Last Modified: Mon, 02 Aug 2021 21:07:51 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.3-nanoserver`

```console
$ docker pull nats@sha256:089f1003c28ef5e80a16a558155a581473b77e6d540a50934cc9d7fd5ca6a71b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2061; amd64

### `nats:2.3-nanoserver` - windows version 10.0.17763.2061; amd64

```console
$ docker pull nats@sha256:baf086eb51e7090cb2ef985758c034c882cbe1dd8d4b2a682a618d32b9215e35
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.3 MB (107296331 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d57bb9c1561692bbad5576428cd8e22189f1addf3a8b82e73e3f27e246bd485`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 06 Jul 2021 20:06:39 GMT
RUN Apply image 1809-amd64
# Wed, 14 Jul 2021 02:35:24 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Mon, 02 Aug 2021 21:17:05 GMT
RUN cmd /S /C #(nop) COPY file:359dd4a92709029cd62dc9620a8ff30527cb3494d6b89c9332ae019bae51b57b in C:\nats-server.exe 
# Mon, 02 Aug 2021 21:17:08 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Mon, 02 Aug 2021 21:17:10 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Mon, 02 Aug 2021 21:17:13 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Mon, 02 Aug 2021 21:17:16 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:29d43e56445c5279a6386c4dfe4d1ada3c7124ade9cb7b0f2757e58ffc7cd10b`  
		Size: 102.7 MB (102725622 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ec20c4c9f6fa5e782e09342d50033ef24c4049a9dad1befd33c96759b71da6de`  
		Last Modified: Wed, 14 Jul 2021 02:40:36 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab54ee8cb88b349708e6f2d10afe13c1d843b9c1ff995a70d40af5ca886eda42`  
		Last Modified: Mon, 02 Aug 2021 21:21:37 GMT  
		Size: 4.6 MB (4564319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27d161923a9b16db535efc5f78e4aedd08225387cc8377cedb826e7539fa9051`  
		Last Modified: Mon, 02 Aug 2021 21:21:36 GMT  
		Size: 1.8 KB (1766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e88c4ba846a11b45abc01afc7de665b15430ebfd4c6e585ba8cb11d896017cd`  
		Last Modified: Mon, 02 Aug 2021 21:21:36 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26ca1fda898c73546bdd8f1655f276fe9a0911a7c16f5a4054cdb40e996692c2`  
		Last Modified: Mon, 02 Aug 2021 21:21:36 GMT  
		Size: 1.2 KB (1180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:088b6cb05a147f4faf4e14f0fc1ecda8481f5ad0a8741dba786aebba4374207b`  
		Last Modified: Mon, 02 Aug 2021 21:21:36 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.3-nanoserver-1809`

```console
$ docker pull nats@sha256:089f1003c28ef5e80a16a558155a581473b77e6d540a50934cc9d7fd5ca6a71b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2061; amd64

### `nats:2.3-nanoserver-1809` - windows version 10.0.17763.2061; amd64

```console
$ docker pull nats@sha256:baf086eb51e7090cb2ef985758c034c882cbe1dd8d4b2a682a618d32b9215e35
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.3 MB (107296331 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d57bb9c1561692bbad5576428cd8e22189f1addf3a8b82e73e3f27e246bd485`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 06 Jul 2021 20:06:39 GMT
RUN Apply image 1809-amd64
# Wed, 14 Jul 2021 02:35:24 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Mon, 02 Aug 2021 21:17:05 GMT
RUN cmd /S /C #(nop) COPY file:359dd4a92709029cd62dc9620a8ff30527cb3494d6b89c9332ae019bae51b57b in C:\nats-server.exe 
# Mon, 02 Aug 2021 21:17:08 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Mon, 02 Aug 2021 21:17:10 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Mon, 02 Aug 2021 21:17:13 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Mon, 02 Aug 2021 21:17:16 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:29d43e56445c5279a6386c4dfe4d1ada3c7124ade9cb7b0f2757e58ffc7cd10b`  
		Size: 102.7 MB (102725622 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ec20c4c9f6fa5e782e09342d50033ef24c4049a9dad1befd33c96759b71da6de`  
		Last Modified: Wed, 14 Jul 2021 02:40:36 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab54ee8cb88b349708e6f2d10afe13c1d843b9c1ff995a70d40af5ca886eda42`  
		Last Modified: Mon, 02 Aug 2021 21:21:37 GMT  
		Size: 4.6 MB (4564319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27d161923a9b16db535efc5f78e4aedd08225387cc8377cedb826e7539fa9051`  
		Last Modified: Mon, 02 Aug 2021 21:21:36 GMT  
		Size: 1.8 KB (1766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e88c4ba846a11b45abc01afc7de665b15430ebfd4c6e585ba8cb11d896017cd`  
		Last Modified: Mon, 02 Aug 2021 21:21:36 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26ca1fda898c73546bdd8f1655f276fe9a0911a7c16f5a4054cdb40e996692c2`  
		Last Modified: Mon, 02 Aug 2021 21:21:36 GMT  
		Size: 1.2 KB (1180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:088b6cb05a147f4faf4e14f0fc1ecda8481f5ad0a8741dba786aebba4374207b`  
		Last Modified: Mon, 02 Aug 2021 21:21:36 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.3-scratch`

```console
$ docker pull nats@sha256:111aefb3002e16ecc001abaa0bb5fc9aabf2510005be379d2cedc0373fa1e596
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.3-scratch` - linux; amd64

```console
$ docker pull nats@sha256:4f6857e56d3555432c7bc830fb297d8c00cbe3b0522f81dfc8c84a4dacb54ed5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4505352 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23830fcc7f9834fd409d95d2bf9877f21b609b7b7392bfcd4b8b5e62e8be14fc`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 02 Aug 2021 21:23:05 GMT
COPY file:0b22daa17d88302a2606c64df249d26684c5926e82494be3f08d920922b75196 in /nats-server 
# Mon, 02 Aug 2021 21:23:05 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Mon, 02 Aug 2021 21:23:05 GMT
EXPOSE 4222 6222 8222
# Mon, 02 Aug 2021 21:23:05 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 02 Aug 2021 21:23:05 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:267760e6058167430070f7584ea1e5e18b4ddf538aec80d4b764ba1b9096b403`  
		Last Modified: Mon, 02 Aug 2021 21:23:56 GMT  
		Size: 4.5 MB (4504877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:612bea9c73fc6c5c02659a6bff01f1bcada2f4c47323021b03bee52a9ca1eba0`  
		Last Modified: Mon, 02 Aug 2021 21:23:55 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.3-scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:6e42eec5a210d9a5b6d95c179d5c55193b69846c76786a81908536eac2efbdc3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4173716 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31e1feb9bf2ac457664507fc7899f48e45d49df93dd60eacdea8b8a9cda8ec51`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 02 Aug 2021 21:17:15 GMT
COPY file:55e1c39fb6ec9785ddf1c189ad5438b9f306c3e1c2a355512f4efc73aa1aacf6 in /nats-server 
# Mon, 02 Aug 2021 21:17:15 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Mon, 02 Aug 2021 21:17:16 GMT
EXPOSE 4222 6222 8222
# Mon, 02 Aug 2021 21:17:16 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 02 Aug 2021 21:17:17 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:7f318c30554fccfe6a5ac8a63f4457a20876b88ede949510db6a8f1c5bcf1442`  
		Last Modified: Mon, 02 Aug 2021 21:19:37 GMT  
		Size: 4.2 MB (4173243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76c9419bcd494c007ef4d4f83649e535bb32d84c81337abb67e153ad75a1fb5f`  
		Last Modified: Mon, 02 Aug 2021 21:19:35 GMT  
		Size: 473.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.3-scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:def02210305c7940addd2f5e26e8417017a2f2ae11116ee001b8f2a7bcb17bff
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.0 MB (3992886 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:20941bb671159cef8cb5d6b9047f5c6c298a495274b06f9c6d9278ea5f9e5a1f`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 07 Jul 2021 06:38:20 GMT
COPY file:a259b6f87cc2d22082524e5ba23201057e836734749f0d28676e8637d920d385 in /nats-server 
# Wed, 07 Jul 2021 06:38:21 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Wed, 07 Jul 2021 06:38:21 GMT
EXPOSE 4222 6222 8222
# Wed, 07 Jul 2021 06:38:22 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 07 Jul 2021 06:38:22 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:434fc0c4a6c5daa82c731102728bcac575b5a312862a89edf401b0305d2efc82`  
		Last Modified: Wed, 07 Jul 2021 06:40:42 GMT  
		Size: 4.0 MB (3992410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c195f08925b050ce566763c31c813f3d8c7e1ba40bc4ccdf0949cb87373c3a43`  
		Last Modified: Wed, 07 Jul 2021 06:40:39 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.3-scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:7a367e1495e9df2cf9cc81af565194815e52b37c0ed1fd7e9f278d88311be5b4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.1 MB (4120338 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad1e0c5709f39238c0ff863c80e1595fb5da12e230643dc6fd4bd6b33cda4039`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 02 Aug 2021 21:06:28 GMT
COPY file:d94287ad868b49da5d590782f3102415d5dfd4ed2a775b4e4c10280c8ab25db3 in /nats-server 
# Mon, 02 Aug 2021 21:06:29 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Mon, 02 Aug 2021 21:06:29 GMT
EXPOSE 4222 6222 8222
# Mon, 02 Aug 2021 21:06:29 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 02 Aug 2021 21:06:29 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4ecc856c82596f8b8982843cac0e5ec138e9c881bfd322038cd7cf0f4942c9c9`  
		Last Modified: Mon, 02 Aug 2021 21:07:52 GMT  
		Size: 4.1 MB (4119864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68fa4df40d0356fc86fe0d6c780d2a447fe1b2c32b5572c65a3c7d2354961da4`  
		Last Modified: Mon, 02 Aug 2021 21:07:51 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.3-windowsservercore`

```console
$ docker pull nats@sha256:d5e778d28d3d06f85d60c39772b380eb774d3f015b748c1491792a36c7a067f9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.2061; amd64
	-	windows version 10.0.14393.4530; amd64

### `nats:2.3-windowsservercore` - windows version 10.0.17763.2061; amd64

```console
$ docker pull nats@sha256:347fad05e489bf9e2c51d053e24efcce0d2031802c51a3feb8f4d2e7ab8765a9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2690730494 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1094808819e1865eaa575aa65800497b156f4e961675e37296ecd71758b68acf`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 06 Jul 2021 20:34:18 GMT
RUN Install update 1809-amd64
# Wed, 14 Jul 2021 01:07:27 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 14 Jul 2021 02:31:26 GMT
ENV NATS_DOCKERIZED=1
# Mon, 02 Aug 2021 21:14:23 GMT
ENV NATS_SERVER=2.3.3
# Mon, 02 Aug 2021 21:14:25 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.3.3/nats-server-v2.3.3-windows-amd64.zip
# Mon, 02 Aug 2021 21:14:28 GMT
ENV NATS_SERVER_SHASUM=dd14c9c104adb657de4a67a17bdf2fc7d7f55860e7a17ce0c6b9c117d9a50dde
# Mon, 02 Aug 2021 21:15:23 GMT
RUN Set-PSDebug -Trace 2
# Mon, 02 Aug 2021 21:16:45 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Mon, 02 Aug 2021 21:16:47 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Mon, 02 Aug 2021 21:16:49 GMT
EXPOSE 4222 6222 8222
# Mon, 02 Aug 2021 21:16:52 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Mon, 02 Aug 2021 21:16:54 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f143c6fed32d477c35b660b2e108ea62e3593c03e44bd9ced208ce52b26b0841`  
		Size: 967.1 MB (967113907 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:adcec6ff907307155c0652222cc9b95a0cc964d4c371e02767e72a5c90472192`  
		Last Modified: Wed, 14 Jul 2021 02:02:19 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f92bdc410321db22d4cf09322869bd9fb2495788c3725624c86d76a6ab3d95d3`  
		Last Modified: Wed, 14 Jul 2021 02:40:16 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c51291d3c5600cdb108e3ed994ab3d59042ca052eae615e136c35e3ac5f9bb6`  
		Last Modified: Mon, 02 Aug 2021 21:21:20 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:292fe7f01e91ae26c600f65e5c1f79e1cafd7d32145f63eda77265399a3c3804`  
		Last Modified: Mon, 02 Aug 2021 21:21:20 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17d5bb92d28832495b8124755df9034565b383dc7bc73be7f24838f425342d1a`  
		Last Modified: Mon, 02 Aug 2021 21:21:20 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8e0ae013ec15413637e098d44190826fe18ee0d434165a78f170bc86ce9c2fb`  
		Last Modified: Mon, 02 Aug 2021 21:21:20 GMT  
		Size: 364.2 KB (364232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4708b7da85335254f8c77a9656ef9c9034ed3d8d6df25e4621a4d1c0c4fce55e`  
		Last Modified: Mon, 02 Aug 2021 21:21:19 GMT  
		Size: 4.9 MB (4906167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88866e210b82ee16f0597e85bdb4ecfcfa4a4fb779acf4fac118727f77793da4`  
		Last Modified: Mon, 02 Aug 2021 21:21:17 GMT  
		Size: 2.0 KB (1963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b0d7cfeb38017cedd34bb386132d75c45a4680749166f4725a12ec569559074`  
		Last Modified: Mon, 02 Aug 2021 21:21:17 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:505a0140bcef7327375fc3aaaded24b5afac6d0507406776accf695315b15b45`  
		Last Modified: Mon, 02 Aug 2021 21:21:18 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:249b0508ccf09dee8b24a8f7319126a4e8aad55ba989a0d96252ad5e55bbcd2a`  
		Last Modified: Mon, 02 Aug 2021 21:21:17 GMT  
		Size: 1.4 KB (1356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.3-windowsservercore` - windows version 10.0.14393.4530; amd64

```console
$ docker pull nats@sha256:4d913e48d6a0ea2ed11c62cc9fff622727736be864fa3a7fe0f15c35fc4b7b6f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6274947967 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eff8abf4d3ed2a1c41241ff4223442903b563fe0a6d8be426bcaed438d42bbbf`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Fri, 09 Jul 2021 05:02:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 14 Jul 2021 01:14:25 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 14 Jul 2021 02:35:48 GMT
ENV NATS_DOCKERIZED=1
# Mon, 02 Aug 2021 21:17:24 GMT
ENV NATS_SERVER=2.3.3
# Mon, 02 Aug 2021 21:17:26 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.3.3/nats-server-v2.3.3-windows-amd64.zip
# Mon, 02 Aug 2021 21:17:28 GMT
ENV NATS_SERVER_SHASUM=dd14c9c104adb657de4a67a17bdf2fc7d7f55860e7a17ce0c6b9c117d9a50dde
# Mon, 02 Aug 2021 21:18:41 GMT
RUN Set-PSDebug -Trace 2
# Mon, 02 Aug 2021 21:20:28 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Mon, 02 Aug 2021 21:20:31 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Mon, 02 Aug 2021 21:20:33 GMT
EXPOSE 4222 6222 8222
# Mon, 02 Aug 2021 21:20:36 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Mon, 02 Aug 2021 21:20:38 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a567de41cc349380b25967f180fb1b6b2431bda61ccaaf69d78a33bc9523614a`  
		Size: 2.2 GB (2199646155 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:fed351b78c876c55ec9c7e75d3b9d1b146c5c5dfeb4b5480c0a7c384322df98c`  
		Last Modified: Wed, 14 Jul 2021 02:03:37 GMT  
		Size: 1.4 KB (1444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf08cae8b8db8f3f89e1a9192d393f2da55b44efce4e778fdb58debe2d608275`  
		Last Modified: Wed, 14 Jul 2021 02:40:57 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:278db267454aa76e00b506fdd53726da5583419a7844eaa96889ff07827a02b7`  
		Last Modified: Mon, 02 Aug 2021 21:21:56 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb231d65d7756b89dfbb667d5b24a7bf72ba86e6d5d9c111ab0d08e3e862dfeb`  
		Last Modified: Mon, 02 Aug 2021 21:21:56 GMT  
		Size: 1.4 KB (1371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfa0b0c97c4ebf872cafc434ce68ec59df2a3cc66e12e83e929b2d7264559729`  
		Last Modified: Mon, 02 Aug 2021 21:21:55 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fe01d11f12da0e487e1ccf3918b3f6a77405b4992df67bc7a092380599cb022`  
		Last Modified: Mon, 02 Aug 2021 21:21:56 GMT  
		Size: 364.5 KB (364483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5da4bfe4915750d7b0192abb4ef4e16913fc4d8746d369529feaead5f8ef2918`  
		Last Modified: Mon, 02 Aug 2021 21:21:59 GMT  
		Size: 4.9 MB (4938295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd26f2047cfc6ccce7d850ea9ec880c9890f783dd0fa4ea9102c561cfa2aa5b5`  
		Last Modified: Mon, 02 Aug 2021 21:21:53 GMT  
		Size: 2.0 KB (1962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce9a1c92d84c4bec202df1e1353e7ecaad58b85a2a2940a9297d14d4548d9e53`  
		Last Modified: Mon, 02 Aug 2021 21:21:53 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dda461d40f36bee8ad537d4225843e28f90f20e81aa8a552d3ada4ef4dbc9f7a`  
		Last Modified: Mon, 02 Aug 2021 21:21:53 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29bf964afbf31f7d4891dc65a1db75f1254d540945a2697c483cdb0375c9b825`  
		Last Modified: Mon, 02 Aug 2021 21:21:53 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.3-windowsservercore-1809`

```console
$ docker pull nats@sha256:1f0cbe04efcaa08eaf910fa921d81d21cc52ff521414b7b02ebbf2b5890f0763
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2061; amd64

### `nats:2.3-windowsservercore-1809` - windows version 10.0.17763.2061; amd64

```console
$ docker pull nats@sha256:347fad05e489bf9e2c51d053e24efcce0d2031802c51a3feb8f4d2e7ab8765a9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2690730494 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1094808819e1865eaa575aa65800497b156f4e961675e37296ecd71758b68acf`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 06 Jul 2021 20:34:18 GMT
RUN Install update 1809-amd64
# Wed, 14 Jul 2021 01:07:27 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 14 Jul 2021 02:31:26 GMT
ENV NATS_DOCKERIZED=1
# Mon, 02 Aug 2021 21:14:23 GMT
ENV NATS_SERVER=2.3.3
# Mon, 02 Aug 2021 21:14:25 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.3.3/nats-server-v2.3.3-windows-amd64.zip
# Mon, 02 Aug 2021 21:14:28 GMT
ENV NATS_SERVER_SHASUM=dd14c9c104adb657de4a67a17bdf2fc7d7f55860e7a17ce0c6b9c117d9a50dde
# Mon, 02 Aug 2021 21:15:23 GMT
RUN Set-PSDebug -Trace 2
# Mon, 02 Aug 2021 21:16:45 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Mon, 02 Aug 2021 21:16:47 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Mon, 02 Aug 2021 21:16:49 GMT
EXPOSE 4222 6222 8222
# Mon, 02 Aug 2021 21:16:52 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Mon, 02 Aug 2021 21:16:54 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f143c6fed32d477c35b660b2e108ea62e3593c03e44bd9ced208ce52b26b0841`  
		Size: 967.1 MB (967113907 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:adcec6ff907307155c0652222cc9b95a0cc964d4c371e02767e72a5c90472192`  
		Last Modified: Wed, 14 Jul 2021 02:02:19 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f92bdc410321db22d4cf09322869bd9fb2495788c3725624c86d76a6ab3d95d3`  
		Last Modified: Wed, 14 Jul 2021 02:40:16 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c51291d3c5600cdb108e3ed994ab3d59042ca052eae615e136c35e3ac5f9bb6`  
		Last Modified: Mon, 02 Aug 2021 21:21:20 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:292fe7f01e91ae26c600f65e5c1f79e1cafd7d32145f63eda77265399a3c3804`  
		Last Modified: Mon, 02 Aug 2021 21:21:20 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17d5bb92d28832495b8124755df9034565b383dc7bc73be7f24838f425342d1a`  
		Last Modified: Mon, 02 Aug 2021 21:21:20 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8e0ae013ec15413637e098d44190826fe18ee0d434165a78f170bc86ce9c2fb`  
		Last Modified: Mon, 02 Aug 2021 21:21:20 GMT  
		Size: 364.2 KB (364232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4708b7da85335254f8c77a9656ef9c9034ed3d8d6df25e4621a4d1c0c4fce55e`  
		Last Modified: Mon, 02 Aug 2021 21:21:19 GMT  
		Size: 4.9 MB (4906167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88866e210b82ee16f0597e85bdb4ecfcfa4a4fb779acf4fac118727f77793da4`  
		Last Modified: Mon, 02 Aug 2021 21:21:17 GMT  
		Size: 2.0 KB (1963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b0d7cfeb38017cedd34bb386132d75c45a4680749166f4725a12ec569559074`  
		Last Modified: Mon, 02 Aug 2021 21:21:17 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:505a0140bcef7327375fc3aaaded24b5afac6d0507406776accf695315b15b45`  
		Last Modified: Mon, 02 Aug 2021 21:21:18 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:249b0508ccf09dee8b24a8f7319126a4e8aad55ba989a0d96252ad5e55bbcd2a`  
		Last Modified: Mon, 02 Aug 2021 21:21:17 GMT  
		Size: 1.4 KB (1356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.3-windowsservercore-ltsc2016`

```console
$ docker pull nats@sha256:a9dd3bec26866787cd33035a57d380c31c2f13a9b85f2d6d34a1b8bc79f3f9ff
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.14393.4530; amd64

### `nats:2.3-windowsservercore-ltsc2016` - windows version 10.0.14393.4530; amd64

```console
$ docker pull nats@sha256:4d913e48d6a0ea2ed11c62cc9fff622727736be864fa3a7fe0f15c35fc4b7b6f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6274947967 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eff8abf4d3ed2a1c41241ff4223442903b563fe0a6d8be426bcaed438d42bbbf`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Fri, 09 Jul 2021 05:02:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 14 Jul 2021 01:14:25 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 14 Jul 2021 02:35:48 GMT
ENV NATS_DOCKERIZED=1
# Mon, 02 Aug 2021 21:17:24 GMT
ENV NATS_SERVER=2.3.3
# Mon, 02 Aug 2021 21:17:26 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.3.3/nats-server-v2.3.3-windows-amd64.zip
# Mon, 02 Aug 2021 21:17:28 GMT
ENV NATS_SERVER_SHASUM=dd14c9c104adb657de4a67a17bdf2fc7d7f55860e7a17ce0c6b9c117d9a50dde
# Mon, 02 Aug 2021 21:18:41 GMT
RUN Set-PSDebug -Trace 2
# Mon, 02 Aug 2021 21:20:28 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Mon, 02 Aug 2021 21:20:31 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Mon, 02 Aug 2021 21:20:33 GMT
EXPOSE 4222 6222 8222
# Mon, 02 Aug 2021 21:20:36 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Mon, 02 Aug 2021 21:20:38 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a567de41cc349380b25967f180fb1b6b2431bda61ccaaf69d78a33bc9523614a`  
		Size: 2.2 GB (2199646155 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:fed351b78c876c55ec9c7e75d3b9d1b146c5c5dfeb4b5480c0a7c384322df98c`  
		Last Modified: Wed, 14 Jul 2021 02:03:37 GMT  
		Size: 1.4 KB (1444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf08cae8b8db8f3f89e1a9192d393f2da55b44efce4e778fdb58debe2d608275`  
		Last Modified: Wed, 14 Jul 2021 02:40:57 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:278db267454aa76e00b506fdd53726da5583419a7844eaa96889ff07827a02b7`  
		Last Modified: Mon, 02 Aug 2021 21:21:56 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb231d65d7756b89dfbb667d5b24a7bf72ba86e6d5d9c111ab0d08e3e862dfeb`  
		Last Modified: Mon, 02 Aug 2021 21:21:56 GMT  
		Size: 1.4 KB (1371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfa0b0c97c4ebf872cafc434ce68ec59df2a3cc66e12e83e929b2d7264559729`  
		Last Modified: Mon, 02 Aug 2021 21:21:55 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fe01d11f12da0e487e1ccf3918b3f6a77405b4992df67bc7a092380599cb022`  
		Last Modified: Mon, 02 Aug 2021 21:21:56 GMT  
		Size: 364.5 KB (364483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5da4bfe4915750d7b0192abb4ef4e16913fc4d8746d369529feaead5f8ef2918`  
		Last Modified: Mon, 02 Aug 2021 21:21:59 GMT  
		Size: 4.9 MB (4938295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd26f2047cfc6ccce7d850ea9ec880c9890f783dd0fa4ea9102c561cfa2aa5b5`  
		Last Modified: Mon, 02 Aug 2021 21:21:53 GMT  
		Size: 2.0 KB (1962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce9a1c92d84c4bec202df1e1353e7ecaad58b85a2a2940a9297d14d4548d9e53`  
		Last Modified: Mon, 02 Aug 2021 21:21:53 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dda461d40f36bee8ad537d4225843e28f90f20e81aa8a552d3ada4ef4dbc9f7a`  
		Last Modified: Mon, 02 Aug 2021 21:21:53 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29bf964afbf31f7d4891dc65a1db75f1254d540945a2697c483cdb0375c9b825`  
		Last Modified: Mon, 02 Aug 2021 21:21:53 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.3.3`

```console
$ docker pull nats@sha256:264363b0f5b7a99322f96dc6786da7daa2b8073b27805a25cad9ce54d08c0679
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.2061; amd64

### `nats:2.3.3` - linux; amd64

```console
$ docker pull nats@sha256:4f6857e56d3555432c7bc830fb297d8c00cbe3b0522f81dfc8c84a4dacb54ed5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4505352 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23830fcc7f9834fd409d95d2bf9877f21b609b7b7392bfcd4b8b5e62e8be14fc`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 02 Aug 2021 21:23:05 GMT
COPY file:0b22daa17d88302a2606c64df249d26684c5926e82494be3f08d920922b75196 in /nats-server 
# Mon, 02 Aug 2021 21:23:05 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Mon, 02 Aug 2021 21:23:05 GMT
EXPOSE 4222 6222 8222
# Mon, 02 Aug 2021 21:23:05 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 02 Aug 2021 21:23:05 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:267760e6058167430070f7584ea1e5e18b4ddf538aec80d4b764ba1b9096b403`  
		Last Modified: Mon, 02 Aug 2021 21:23:56 GMT  
		Size: 4.5 MB (4504877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:612bea9c73fc6c5c02659a6bff01f1bcada2f4c47323021b03bee52a9ca1eba0`  
		Last Modified: Mon, 02 Aug 2021 21:23:55 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.3.3` - linux; arm variant v6

```console
$ docker pull nats@sha256:6e42eec5a210d9a5b6d95c179d5c55193b69846c76786a81908536eac2efbdc3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4173716 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31e1feb9bf2ac457664507fc7899f48e45d49df93dd60eacdea8b8a9cda8ec51`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 02 Aug 2021 21:17:15 GMT
COPY file:55e1c39fb6ec9785ddf1c189ad5438b9f306c3e1c2a355512f4efc73aa1aacf6 in /nats-server 
# Mon, 02 Aug 2021 21:17:15 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Mon, 02 Aug 2021 21:17:16 GMT
EXPOSE 4222 6222 8222
# Mon, 02 Aug 2021 21:17:16 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 02 Aug 2021 21:17:17 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:7f318c30554fccfe6a5ac8a63f4457a20876b88ede949510db6a8f1c5bcf1442`  
		Last Modified: Mon, 02 Aug 2021 21:19:37 GMT  
		Size: 4.2 MB (4173243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76c9419bcd494c007ef4d4f83649e535bb32d84c81337abb67e153ad75a1fb5f`  
		Last Modified: Mon, 02 Aug 2021 21:19:35 GMT  
		Size: 473.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.3.3` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:7a367e1495e9df2cf9cc81af565194815e52b37c0ed1fd7e9f278d88311be5b4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.1 MB (4120338 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad1e0c5709f39238c0ff863c80e1595fb5da12e230643dc6fd4bd6b33cda4039`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 02 Aug 2021 21:06:28 GMT
COPY file:d94287ad868b49da5d590782f3102415d5dfd4ed2a775b4e4c10280c8ab25db3 in /nats-server 
# Mon, 02 Aug 2021 21:06:29 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Mon, 02 Aug 2021 21:06:29 GMT
EXPOSE 4222 6222 8222
# Mon, 02 Aug 2021 21:06:29 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 02 Aug 2021 21:06:29 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4ecc856c82596f8b8982843cac0e5ec138e9c881bfd322038cd7cf0f4942c9c9`  
		Last Modified: Mon, 02 Aug 2021 21:07:52 GMT  
		Size: 4.1 MB (4119864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68fa4df40d0356fc86fe0d6c780d2a447fe1b2c32b5572c65a3c7d2354961da4`  
		Last Modified: Mon, 02 Aug 2021 21:07:51 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.3.3` - windows version 10.0.17763.2061; amd64

```console
$ docker pull nats@sha256:baf086eb51e7090cb2ef985758c034c882cbe1dd8d4b2a682a618d32b9215e35
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.3 MB (107296331 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d57bb9c1561692bbad5576428cd8e22189f1addf3a8b82e73e3f27e246bd485`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 06 Jul 2021 20:06:39 GMT
RUN Apply image 1809-amd64
# Wed, 14 Jul 2021 02:35:24 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Mon, 02 Aug 2021 21:17:05 GMT
RUN cmd /S /C #(nop) COPY file:359dd4a92709029cd62dc9620a8ff30527cb3494d6b89c9332ae019bae51b57b in C:\nats-server.exe 
# Mon, 02 Aug 2021 21:17:08 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Mon, 02 Aug 2021 21:17:10 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Mon, 02 Aug 2021 21:17:13 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Mon, 02 Aug 2021 21:17:16 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:29d43e56445c5279a6386c4dfe4d1ada3c7124ade9cb7b0f2757e58ffc7cd10b`  
		Size: 102.7 MB (102725622 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ec20c4c9f6fa5e782e09342d50033ef24c4049a9dad1befd33c96759b71da6de`  
		Last Modified: Wed, 14 Jul 2021 02:40:36 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab54ee8cb88b349708e6f2d10afe13c1d843b9c1ff995a70d40af5ca886eda42`  
		Last Modified: Mon, 02 Aug 2021 21:21:37 GMT  
		Size: 4.6 MB (4564319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27d161923a9b16db535efc5f78e4aedd08225387cc8377cedb826e7539fa9051`  
		Last Modified: Mon, 02 Aug 2021 21:21:36 GMT  
		Size: 1.8 KB (1766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e88c4ba846a11b45abc01afc7de665b15430ebfd4c6e585ba8cb11d896017cd`  
		Last Modified: Mon, 02 Aug 2021 21:21:36 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26ca1fda898c73546bdd8f1655f276fe9a0911a7c16f5a4054cdb40e996692c2`  
		Last Modified: Mon, 02 Aug 2021 21:21:36 GMT  
		Size: 1.2 KB (1180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:088b6cb05a147f4faf4e14f0fc1ecda8481f5ad0a8741dba786aebba4374207b`  
		Last Modified: Mon, 02 Aug 2021 21:21:36 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.3.3-alpine`

```console
$ docker pull nats@sha256:e01b2dbf146b1410a06f156b252199830350860133069ec035e14a9f2b940fe7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `nats:2.3.3-alpine` - linux; amd64

```console
$ docker pull nats@sha256:b430407bf4008593c12a2cc85208f72e96b53fec98b30187c517b9d1958b657e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7601531 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:37a8e948168fcd8c0825a0cd425eb489bd313da994d65e73b5072d6ff6c8225a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 15 Jun 2021 22:19:37 GMT
ADD file:f278386b0cef68136129f5f58c52445590a417b624d62bca158d4dc926c340df in / 
# Tue, 15 Jun 2021 22:19:37 GMT
CMD ["/bin/sh"]
# Mon, 02 Aug 2021 21:22:41 GMT
ENV NATS_SERVER=2.3.3
# Mon, 02 Aug 2021 21:22:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f8e04470165fdfba062442cf5975f22668ab20fb12df7e299734e16a45370bef' ;; 		armhf) natsArch='arm6'; sha256='6396531f34e99cca903cdd461a79f1b8255d0cc219e5186ea15284b5b5e7e5e7' ;; 		armv7) natsArch='arm7'; sha256='4353de84d9e42b24b73ba98a4ed2a9eaa7c4f945bd68e1ddb4fbde885020ab30' ;; 		x86_64) natsArch='amd64'; sha256='66703b81de34d06060eb2198dfb5a1087547d45e680dee4da1214198a8073ce5' ;; 		x86) natsArch='386'; sha256='e38b9c9eda279bc4eee9cf6a3d4b2b25774b692450421a16e2ff6602977e6571' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Mon, 02 Aug 2021 21:22:44 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Mon, 02 Aug 2021 21:22:44 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 02 Aug 2021 21:22:44 GMT
EXPOSE 4222 6222 8222
# Mon, 02 Aug 2021 21:22:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 02 Aug 2021 21:22:45 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:5843afab387455b37944e709ee8c78d7520df80f8d01cf7f861aae63beeddb6b`  
		Last Modified: Tue, 15 Jun 2021 22:20:04 GMT  
		Size: 2.8 MB (2811478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03113b330e4f7fe35234354441a5bc0f8cabb61f7e7c02e1c2c7a9002be630c7`  
		Last Modified: Mon, 02 Aug 2021 21:23:32 GMT  
		Size: 4.8 MB (4789084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe9957a382ed4e85c0797d4c958c23eb4c68ab7e84a78c07a137bbf4bfd93c86`  
		Last Modified: Mon, 02 Aug 2021 21:23:31 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51734fe5b37d3390b972f615a9b12d4454a30ce0ed124f4a5d0f91a17d6ce6f8`  
		Last Modified: Mon, 02 Aug 2021 21:23:30 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.3.3-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:d5fc2c9df074891880beadedf530ee3dbf0761259a14619e946c1cefa842cac3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7079723 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f49351bac7a37d427b25fbdcc43daa3d1ea704fe96f3931802df83f01bf235c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 30 Jul 2021 17:49:42 GMT
ADD file:c80bc2b093cbc0fc466582ef21cbed377de9fa874aedbf320079525ddacd1200 in / 
# Fri, 30 Jul 2021 17:49:42 GMT
CMD ["/bin/sh"]
# Mon, 02 Aug 2021 21:16:47 GMT
ENV NATS_SERVER=2.3.3
# Mon, 02 Aug 2021 21:16:52 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f8e04470165fdfba062442cf5975f22668ab20fb12df7e299734e16a45370bef' ;; 		armhf) natsArch='arm6'; sha256='6396531f34e99cca903cdd461a79f1b8255d0cc219e5186ea15284b5b5e7e5e7' ;; 		armv7) natsArch='arm7'; sha256='4353de84d9e42b24b73ba98a4ed2a9eaa7c4f945bd68e1ddb4fbde885020ab30' ;; 		x86_64) natsArch='amd64'; sha256='66703b81de34d06060eb2198dfb5a1087547d45e680dee4da1214198a8073ce5' ;; 		x86) natsArch='386'; sha256='e38b9c9eda279bc4eee9cf6a3d4b2b25774b692450421a16e2ff6602977e6571' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Mon, 02 Aug 2021 21:16:52 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Mon, 02 Aug 2021 21:16:53 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 02 Aug 2021 21:16:53 GMT
EXPOSE 4222 6222 8222
# Mon, 02 Aug 2021 21:16:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 02 Aug 2021 21:16:54 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:b4c9a0924271af3466de27804af26420eb58da1466e7eaaba127d178b380fea3`  
		Last Modified: Tue, 15 Jun 2021 22:58:47 GMT  
		Size: 2.6 MB (2624382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e3313ef1b9ecd8d9e94997ae371b1c0aabda27773f0b2e12b4be7463517cf87`  
		Last Modified: Mon, 02 Aug 2021 21:18:59 GMT  
		Size: 4.5 MB (4454370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:785fbb490293d9c2f8cdaed64735e76ea2a0dc1c40e13814102053f6d9c4ddc3`  
		Last Modified: Mon, 02 Aug 2021 21:18:56 GMT  
		Size: 557.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ee9f0a3fdc78fe2942c2a3d6969418df884ad628f52adb50525f4022ed56ec2`  
		Last Modified: Mon, 02 Aug 2021 21:18:56 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.3.3-alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:f818c9007861b8440d5c89a859f8f20f483637ab3f3e7c7a7f89ef40afd23937
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7113993 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc01fa8c08e4612961dfe7cf6c422a1a58b99637fd0297f9c3d811b95a32c185`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 15 Jun 2021 21:44:56 GMT
ADD file:6797caacbfe41bfe44000b39ed017016c6fcc492b3d6557cdaba88536df6c876 in / 
# Tue, 15 Jun 2021 21:44:56 GMT
CMD ["/bin/sh"]
# Mon, 02 Aug 2021 21:06:09 GMT
ENV NATS_SERVER=2.3.3
# Mon, 02 Aug 2021 21:06:11 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f8e04470165fdfba062442cf5975f22668ab20fb12df7e299734e16a45370bef' ;; 		armhf) natsArch='arm6'; sha256='6396531f34e99cca903cdd461a79f1b8255d0cc219e5186ea15284b5b5e7e5e7' ;; 		armv7) natsArch='arm7'; sha256='4353de84d9e42b24b73ba98a4ed2a9eaa7c4f945bd68e1ddb4fbde885020ab30' ;; 		x86_64) natsArch='amd64'; sha256='66703b81de34d06060eb2198dfb5a1087547d45e680dee4da1214198a8073ce5' ;; 		x86) natsArch='386'; sha256='e38b9c9eda279bc4eee9cf6a3d4b2b25774b692450421a16e2ff6602977e6571' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Mon, 02 Aug 2021 21:06:11 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Mon, 02 Aug 2021 21:06:12 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 02 Aug 2021 21:06:12 GMT
EXPOSE 4222 6222 8222
# Mon, 02 Aug 2021 21:06:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 02 Aug 2021 21:06:12 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:58ab47519297212468320b23b8100fc1b2b96e8d342040806ae509a778a0a07a`  
		Last Modified: Tue, 15 Jun 2021 21:46:03 GMT  
		Size: 2.7 MB (2709626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0b71cb50e81b94a1183dec31a916ec92da12268c9d5c01358f63f093176829d`  
		Last Modified: Mon, 02 Aug 2021 21:07:22 GMT  
		Size: 4.4 MB (4403398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69e71c9cdab2ba7a29d11ef463c8173ea1cdc1f4a0a549ee1d8bdf0a21392641`  
		Last Modified: Mon, 02 Aug 2021 21:07:21 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17f4a027c87d570eda83fa005f1747518d8e6f172eaf1f5432d6073835418317`  
		Last Modified: Mon, 02 Aug 2021 21:07:21 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.3.3-alpine3.14`

```console
$ docker pull nats@sha256:e01b2dbf146b1410a06f156b252199830350860133069ec035e14a9f2b940fe7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `nats:2.3.3-alpine3.14` - linux; amd64

```console
$ docker pull nats@sha256:b430407bf4008593c12a2cc85208f72e96b53fec98b30187c517b9d1958b657e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7601531 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:37a8e948168fcd8c0825a0cd425eb489bd313da994d65e73b5072d6ff6c8225a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 15 Jun 2021 22:19:37 GMT
ADD file:f278386b0cef68136129f5f58c52445590a417b624d62bca158d4dc926c340df in / 
# Tue, 15 Jun 2021 22:19:37 GMT
CMD ["/bin/sh"]
# Mon, 02 Aug 2021 21:22:41 GMT
ENV NATS_SERVER=2.3.3
# Mon, 02 Aug 2021 21:22:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f8e04470165fdfba062442cf5975f22668ab20fb12df7e299734e16a45370bef' ;; 		armhf) natsArch='arm6'; sha256='6396531f34e99cca903cdd461a79f1b8255d0cc219e5186ea15284b5b5e7e5e7' ;; 		armv7) natsArch='arm7'; sha256='4353de84d9e42b24b73ba98a4ed2a9eaa7c4f945bd68e1ddb4fbde885020ab30' ;; 		x86_64) natsArch='amd64'; sha256='66703b81de34d06060eb2198dfb5a1087547d45e680dee4da1214198a8073ce5' ;; 		x86) natsArch='386'; sha256='e38b9c9eda279bc4eee9cf6a3d4b2b25774b692450421a16e2ff6602977e6571' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Mon, 02 Aug 2021 21:22:44 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Mon, 02 Aug 2021 21:22:44 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 02 Aug 2021 21:22:44 GMT
EXPOSE 4222 6222 8222
# Mon, 02 Aug 2021 21:22:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 02 Aug 2021 21:22:45 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:5843afab387455b37944e709ee8c78d7520df80f8d01cf7f861aae63beeddb6b`  
		Last Modified: Tue, 15 Jun 2021 22:20:04 GMT  
		Size: 2.8 MB (2811478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03113b330e4f7fe35234354441a5bc0f8cabb61f7e7c02e1c2c7a9002be630c7`  
		Last Modified: Mon, 02 Aug 2021 21:23:32 GMT  
		Size: 4.8 MB (4789084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe9957a382ed4e85c0797d4c958c23eb4c68ab7e84a78c07a137bbf4bfd93c86`  
		Last Modified: Mon, 02 Aug 2021 21:23:31 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51734fe5b37d3390b972f615a9b12d4454a30ce0ed124f4a5d0f91a17d6ce6f8`  
		Last Modified: Mon, 02 Aug 2021 21:23:30 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.3.3-alpine3.14` - linux; arm variant v6

```console
$ docker pull nats@sha256:d5fc2c9df074891880beadedf530ee3dbf0761259a14619e946c1cefa842cac3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7079723 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f49351bac7a37d427b25fbdcc43daa3d1ea704fe96f3931802df83f01bf235c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 30 Jul 2021 17:49:42 GMT
ADD file:c80bc2b093cbc0fc466582ef21cbed377de9fa874aedbf320079525ddacd1200 in / 
# Fri, 30 Jul 2021 17:49:42 GMT
CMD ["/bin/sh"]
# Mon, 02 Aug 2021 21:16:47 GMT
ENV NATS_SERVER=2.3.3
# Mon, 02 Aug 2021 21:16:52 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f8e04470165fdfba062442cf5975f22668ab20fb12df7e299734e16a45370bef' ;; 		armhf) natsArch='arm6'; sha256='6396531f34e99cca903cdd461a79f1b8255d0cc219e5186ea15284b5b5e7e5e7' ;; 		armv7) natsArch='arm7'; sha256='4353de84d9e42b24b73ba98a4ed2a9eaa7c4f945bd68e1ddb4fbde885020ab30' ;; 		x86_64) natsArch='amd64'; sha256='66703b81de34d06060eb2198dfb5a1087547d45e680dee4da1214198a8073ce5' ;; 		x86) natsArch='386'; sha256='e38b9c9eda279bc4eee9cf6a3d4b2b25774b692450421a16e2ff6602977e6571' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Mon, 02 Aug 2021 21:16:52 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Mon, 02 Aug 2021 21:16:53 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 02 Aug 2021 21:16:53 GMT
EXPOSE 4222 6222 8222
# Mon, 02 Aug 2021 21:16:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 02 Aug 2021 21:16:54 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:b4c9a0924271af3466de27804af26420eb58da1466e7eaaba127d178b380fea3`  
		Last Modified: Tue, 15 Jun 2021 22:58:47 GMT  
		Size: 2.6 MB (2624382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e3313ef1b9ecd8d9e94997ae371b1c0aabda27773f0b2e12b4be7463517cf87`  
		Last Modified: Mon, 02 Aug 2021 21:18:59 GMT  
		Size: 4.5 MB (4454370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:785fbb490293d9c2f8cdaed64735e76ea2a0dc1c40e13814102053f6d9c4ddc3`  
		Last Modified: Mon, 02 Aug 2021 21:18:56 GMT  
		Size: 557.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ee9f0a3fdc78fe2942c2a3d6969418df884ad628f52adb50525f4022ed56ec2`  
		Last Modified: Mon, 02 Aug 2021 21:18:56 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.3.3-alpine3.14` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:f818c9007861b8440d5c89a859f8f20f483637ab3f3e7c7a7f89ef40afd23937
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7113993 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc01fa8c08e4612961dfe7cf6c422a1a58b99637fd0297f9c3d811b95a32c185`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 15 Jun 2021 21:44:56 GMT
ADD file:6797caacbfe41bfe44000b39ed017016c6fcc492b3d6557cdaba88536df6c876 in / 
# Tue, 15 Jun 2021 21:44:56 GMT
CMD ["/bin/sh"]
# Mon, 02 Aug 2021 21:06:09 GMT
ENV NATS_SERVER=2.3.3
# Mon, 02 Aug 2021 21:06:11 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f8e04470165fdfba062442cf5975f22668ab20fb12df7e299734e16a45370bef' ;; 		armhf) natsArch='arm6'; sha256='6396531f34e99cca903cdd461a79f1b8255d0cc219e5186ea15284b5b5e7e5e7' ;; 		armv7) natsArch='arm7'; sha256='4353de84d9e42b24b73ba98a4ed2a9eaa7c4f945bd68e1ddb4fbde885020ab30' ;; 		x86_64) natsArch='amd64'; sha256='66703b81de34d06060eb2198dfb5a1087547d45e680dee4da1214198a8073ce5' ;; 		x86) natsArch='386'; sha256='e38b9c9eda279bc4eee9cf6a3d4b2b25774b692450421a16e2ff6602977e6571' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Mon, 02 Aug 2021 21:06:11 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Mon, 02 Aug 2021 21:06:12 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 02 Aug 2021 21:06:12 GMT
EXPOSE 4222 6222 8222
# Mon, 02 Aug 2021 21:06:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 02 Aug 2021 21:06:12 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:58ab47519297212468320b23b8100fc1b2b96e8d342040806ae509a778a0a07a`  
		Last Modified: Tue, 15 Jun 2021 21:46:03 GMT  
		Size: 2.7 MB (2709626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0b71cb50e81b94a1183dec31a916ec92da12268c9d5c01358f63f093176829d`  
		Last Modified: Mon, 02 Aug 2021 21:07:22 GMT  
		Size: 4.4 MB (4403398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69e71c9cdab2ba7a29d11ef463c8173ea1cdc1f4a0a549ee1d8bdf0a21392641`  
		Last Modified: Mon, 02 Aug 2021 21:07:21 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17f4a027c87d570eda83fa005f1747518d8e6f172eaf1f5432d6073835418317`  
		Last Modified: Mon, 02 Aug 2021 21:07:21 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.3.3-linux`

```console
$ docker pull nats@sha256:00ee30146de79a4ebe96b9d4a07970bd71edd18342a0be7980b61def9ee330cb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `nats:2.3.3-linux` - linux; amd64

```console
$ docker pull nats@sha256:4f6857e56d3555432c7bc830fb297d8c00cbe3b0522f81dfc8c84a4dacb54ed5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4505352 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23830fcc7f9834fd409d95d2bf9877f21b609b7b7392bfcd4b8b5e62e8be14fc`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 02 Aug 2021 21:23:05 GMT
COPY file:0b22daa17d88302a2606c64df249d26684c5926e82494be3f08d920922b75196 in /nats-server 
# Mon, 02 Aug 2021 21:23:05 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Mon, 02 Aug 2021 21:23:05 GMT
EXPOSE 4222 6222 8222
# Mon, 02 Aug 2021 21:23:05 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 02 Aug 2021 21:23:05 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:267760e6058167430070f7584ea1e5e18b4ddf538aec80d4b764ba1b9096b403`  
		Last Modified: Mon, 02 Aug 2021 21:23:56 GMT  
		Size: 4.5 MB (4504877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:612bea9c73fc6c5c02659a6bff01f1bcada2f4c47323021b03bee52a9ca1eba0`  
		Last Modified: Mon, 02 Aug 2021 21:23:55 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.3.3-linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:6e42eec5a210d9a5b6d95c179d5c55193b69846c76786a81908536eac2efbdc3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4173716 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31e1feb9bf2ac457664507fc7899f48e45d49df93dd60eacdea8b8a9cda8ec51`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 02 Aug 2021 21:17:15 GMT
COPY file:55e1c39fb6ec9785ddf1c189ad5438b9f306c3e1c2a355512f4efc73aa1aacf6 in /nats-server 
# Mon, 02 Aug 2021 21:17:15 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Mon, 02 Aug 2021 21:17:16 GMT
EXPOSE 4222 6222 8222
# Mon, 02 Aug 2021 21:17:16 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 02 Aug 2021 21:17:17 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:7f318c30554fccfe6a5ac8a63f4457a20876b88ede949510db6a8f1c5bcf1442`  
		Last Modified: Mon, 02 Aug 2021 21:19:37 GMT  
		Size: 4.2 MB (4173243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76c9419bcd494c007ef4d4f83649e535bb32d84c81337abb67e153ad75a1fb5f`  
		Last Modified: Mon, 02 Aug 2021 21:19:35 GMT  
		Size: 473.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.3.3-linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:7a367e1495e9df2cf9cc81af565194815e52b37c0ed1fd7e9f278d88311be5b4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.1 MB (4120338 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad1e0c5709f39238c0ff863c80e1595fb5da12e230643dc6fd4bd6b33cda4039`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 02 Aug 2021 21:06:28 GMT
COPY file:d94287ad868b49da5d590782f3102415d5dfd4ed2a775b4e4c10280c8ab25db3 in /nats-server 
# Mon, 02 Aug 2021 21:06:29 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Mon, 02 Aug 2021 21:06:29 GMT
EXPOSE 4222 6222 8222
# Mon, 02 Aug 2021 21:06:29 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 02 Aug 2021 21:06:29 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4ecc856c82596f8b8982843cac0e5ec138e9c881bfd322038cd7cf0f4942c9c9`  
		Last Modified: Mon, 02 Aug 2021 21:07:52 GMT  
		Size: 4.1 MB (4119864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68fa4df40d0356fc86fe0d6c780d2a447fe1b2c32b5572c65a3c7d2354961da4`  
		Last Modified: Mon, 02 Aug 2021 21:07:51 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.3.3-nanoserver`

```console
$ docker pull nats@sha256:089f1003c28ef5e80a16a558155a581473b77e6d540a50934cc9d7fd5ca6a71b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2061; amd64

### `nats:2.3.3-nanoserver` - windows version 10.0.17763.2061; amd64

```console
$ docker pull nats@sha256:baf086eb51e7090cb2ef985758c034c882cbe1dd8d4b2a682a618d32b9215e35
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.3 MB (107296331 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d57bb9c1561692bbad5576428cd8e22189f1addf3a8b82e73e3f27e246bd485`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 06 Jul 2021 20:06:39 GMT
RUN Apply image 1809-amd64
# Wed, 14 Jul 2021 02:35:24 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Mon, 02 Aug 2021 21:17:05 GMT
RUN cmd /S /C #(nop) COPY file:359dd4a92709029cd62dc9620a8ff30527cb3494d6b89c9332ae019bae51b57b in C:\nats-server.exe 
# Mon, 02 Aug 2021 21:17:08 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Mon, 02 Aug 2021 21:17:10 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Mon, 02 Aug 2021 21:17:13 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Mon, 02 Aug 2021 21:17:16 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:29d43e56445c5279a6386c4dfe4d1ada3c7124ade9cb7b0f2757e58ffc7cd10b`  
		Size: 102.7 MB (102725622 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ec20c4c9f6fa5e782e09342d50033ef24c4049a9dad1befd33c96759b71da6de`  
		Last Modified: Wed, 14 Jul 2021 02:40:36 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab54ee8cb88b349708e6f2d10afe13c1d843b9c1ff995a70d40af5ca886eda42`  
		Last Modified: Mon, 02 Aug 2021 21:21:37 GMT  
		Size: 4.6 MB (4564319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27d161923a9b16db535efc5f78e4aedd08225387cc8377cedb826e7539fa9051`  
		Last Modified: Mon, 02 Aug 2021 21:21:36 GMT  
		Size: 1.8 KB (1766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e88c4ba846a11b45abc01afc7de665b15430ebfd4c6e585ba8cb11d896017cd`  
		Last Modified: Mon, 02 Aug 2021 21:21:36 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26ca1fda898c73546bdd8f1655f276fe9a0911a7c16f5a4054cdb40e996692c2`  
		Last Modified: Mon, 02 Aug 2021 21:21:36 GMT  
		Size: 1.2 KB (1180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:088b6cb05a147f4faf4e14f0fc1ecda8481f5ad0a8741dba786aebba4374207b`  
		Last Modified: Mon, 02 Aug 2021 21:21:36 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.3.3-nanoserver-1809`

```console
$ docker pull nats@sha256:089f1003c28ef5e80a16a558155a581473b77e6d540a50934cc9d7fd5ca6a71b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2061; amd64

### `nats:2.3.3-nanoserver-1809` - windows version 10.0.17763.2061; amd64

```console
$ docker pull nats@sha256:baf086eb51e7090cb2ef985758c034c882cbe1dd8d4b2a682a618d32b9215e35
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.3 MB (107296331 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d57bb9c1561692bbad5576428cd8e22189f1addf3a8b82e73e3f27e246bd485`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 06 Jul 2021 20:06:39 GMT
RUN Apply image 1809-amd64
# Wed, 14 Jul 2021 02:35:24 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Mon, 02 Aug 2021 21:17:05 GMT
RUN cmd /S /C #(nop) COPY file:359dd4a92709029cd62dc9620a8ff30527cb3494d6b89c9332ae019bae51b57b in C:\nats-server.exe 
# Mon, 02 Aug 2021 21:17:08 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Mon, 02 Aug 2021 21:17:10 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Mon, 02 Aug 2021 21:17:13 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Mon, 02 Aug 2021 21:17:16 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:29d43e56445c5279a6386c4dfe4d1ada3c7124ade9cb7b0f2757e58ffc7cd10b`  
		Size: 102.7 MB (102725622 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ec20c4c9f6fa5e782e09342d50033ef24c4049a9dad1befd33c96759b71da6de`  
		Last Modified: Wed, 14 Jul 2021 02:40:36 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab54ee8cb88b349708e6f2d10afe13c1d843b9c1ff995a70d40af5ca886eda42`  
		Last Modified: Mon, 02 Aug 2021 21:21:37 GMT  
		Size: 4.6 MB (4564319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27d161923a9b16db535efc5f78e4aedd08225387cc8377cedb826e7539fa9051`  
		Last Modified: Mon, 02 Aug 2021 21:21:36 GMT  
		Size: 1.8 KB (1766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e88c4ba846a11b45abc01afc7de665b15430ebfd4c6e585ba8cb11d896017cd`  
		Last Modified: Mon, 02 Aug 2021 21:21:36 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26ca1fda898c73546bdd8f1655f276fe9a0911a7c16f5a4054cdb40e996692c2`  
		Last Modified: Mon, 02 Aug 2021 21:21:36 GMT  
		Size: 1.2 KB (1180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:088b6cb05a147f4faf4e14f0fc1ecda8481f5ad0a8741dba786aebba4374207b`  
		Last Modified: Mon, 02 Aug 2021 21:21:36 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.3.3-scratch`

```console
$ docker pull nats@sha256:00ee30146de79a4ebe96b9d4a07970bd71edd18342a0be7980b61def9ee330cb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `nats:2.3.3-scratch` - linux; amd64

```console
$ docker pull nats@sha256:4f6857e56d3555432c7bc830fb297d8c00cbe3b0522f81dfc8c84a4dacb54ed5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4505352 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23830fcc7f9834fd409d95d2bf9877f21b609b7b7392bfcd4b8b5e62e8be14fc`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 02 Aug 2021 21:23:05 GMT
COPY file:0b22daa17d88302a2606c64df249d26684c5926e82494be3f08d920922b75196 in /nats-server 
# Mon, 02 Aug 2021 21:23:05 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Mon, 02 Aug 2021 21:23:05 GMT
EXPOSE 4222 6222 8222
# Mon, 02 Aug 2021 21:23:05 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 02 Aug 2021 21:23:05 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:267760e6058167430070f7584ea1e5e18b4ddf538aec80d4b764ba1b9096b403`  
		Last Modified: Mon, 02 Aug 2021 21:23:56 GMT  
		Size: 4.5 MB (4504877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:612bea9c73fc6c5c02659a6bff01f1bcada2f4c47323021b03bee52a9ca1eba0`  
		Last Modified: Mon, 02 Aug 2021 21:23:55 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.3.3-scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:6e42eec5a210d9a5b6d95c179d5c55193b69846c76786a81908536eac2efbdc3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4173716 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31e1feb9bf2ac457664507fc7899f48e45d49df93dd60eacdea8b8a9cda8ec51`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 02 Aug 2021 21:17:15 GMT
COPY file:55e1c39fb6ec9785ddf1c189ad5438b9f306c3e1c2a355512f4efc73aa1aacf6 in /nats-server 
# Mon, 02 Aug 2021 21:17:15 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Mon, 02 Aug 2021 21:17:16 GMT
EXPOSE 4222 6222 8222
# Mon, 02 Aug 2021 21:17:16 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 02 Aug 2021 21:17:17 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:7f318c30554fccfe6a5ac8a63f4457a20876b88ede949510db6a8f1c5bcf1442`  
		Last Modified: Mon, 02 Aug 2021 21:19:37 GMT  
		Size: 4.2 MB (4173243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76c9419bcd494c007ef4d4f83649e535bb32d84c81337abb67e153ad75a1fb5f`  
		Last Modified: Mon, 02 Aug 2021 21:19:35 GMT  
		Size: 473.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.3.3-scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:7a367e1495e9df2cf9cc81af565194815e52b37c0ed1fd7e9f278d88311be5b4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.1 MB (4120338 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad1e0c5709f39238c0ff863c80e1595fb5da12e230643dc6fd4bd6b33cda4039`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 02 Aug 2021 21:06:28 GMT
COPY file:d94287ad868b49da5d590782f3102415d5dfd4ed2a775b4e4c10280c8ab25db3 in /nats-server 
# Mon, 02 Aug 2021 21:06:29 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Mon, 02 Aug 2021 21:06:29 GMT
EXPOSE 4222 6222 8222
# Mon, 02 Aug 2021 21:06:29 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 02 Aug 2021 21:06:29 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4ecc856c82596f8b8982843cac0e5ec138e9c881bfd322038cd7cf0f4942c9c9`  
		Last Modified: Mon, 02 Aug 2021 21:07:52 GMT  
		Size: 4.1 MB (4119864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68fa4df40d0356fc86fe0d6c780d2a447fe1b2c32b5572c65a3c7d2354961da4`  
		Last Modified: Mon, 02 Aug 2021 21:07:51 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.3.3-windowsservercore`

```console
$ docker pull nats@sha256:d5e778d28d3d06f85d60c39772b380eb774d3f015b748c1491792a36c7a067f9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.2061; amd64
	-	windows version 10.0.14393.4530; amd64

### `nats:2.3.3-windowsservercore` - windows version 10.0.17763.2061; amd64

```console
$ docker pull nats@sha256:347fad05e489bf9e2c51d053e24efcce0d2031802c51a3feb8f4d2e7ab8765a9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2690730494 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1094808819e1865eaa575aa65800497b156f4e961675e37296ecd71758b68acf`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 06 Jul 2021 20:34:18 GMT
RUN Install update 1809-amd64
# Wed, 14 Jul 2021 01:07:27 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 14 Jul 2021 02:31:26 GMT
ENV NATS_DOCKERIZED=1
# Mon, 02 Aug 2021 21:14:23 GMT
ENV NATS_SERVER=2.3.3
# Mon, 02 Aug 2021 21:14:25 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.3.3/nats-server-v2.3.3-windows-amd64.zip
# Mon, 02 Aug 2021 21:14:28 GMT
ENV NATS_SERVER_SHASUM=dd14c9c104adb657de4a67a17bdf2fc7d7f55860e7a17ce0c6b9c117d9a50dde
# Mon, 02 Aug 2021 21:15:23 GMT
RUN Set-PSDebug -Trace 2
# Mon, 02 Aug 2021 21:16:45 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Mon, 02 Aug 2021 21:16:47 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Mon, 02 Aug 2021 21:16:49 GMT
EXPOSE 4222 6222 8222
# Mon, 02 Aug 2021 21:16:52 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Mon, 02 Aug 2021 21:16:54 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f143c6fed32d477c35b660b2e108ea62e3593c03e44bd9ced208ce52b26b0841`  
		Size: 967.1 MB (967113907 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:adcec6ff907307155c0652222cc9b95a0cc964d4c371e02767e72a5c90472192`  
		Last Modified: Wed, 14 Jul 2021 02:02:19 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f92bdc410321db22d4cf09322869bd9fb2495788c3725624c86d76a6ab3d95d3`  
		Last Modified: Wed, 14 Jul 2021 02:40:16 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c51291d3c5600cdb108e3ed994ab3d59042ca052eae615e136c35e3ac5f9bb6`  
		Last Modified: Mon, 02 Aug 2021 21:21:20 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:292fe7f01e91ae26c600f65e5c1f79e1cafd7d32145f63eda77265399a3c3804`  
		Last Modified: Mon, 02 Aug 2021 21:21:20 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17d5bb92d28832495b8124755df9034565b383dc7bc73be7f24838f425342d1a`  
		Last Modified: Mon, 02 Aug 2021 21:21:20 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8e0ae013ec15413637e098d44190826fe18ee0d434165a78f170bc86ce9c2fb`  
		Last Modified: Mon, 02 Aug 2021 21:21:20 GMT  
		Size: 364.2 KB (364232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4708b7da85335254f8c77a9656ef9c9034ed3d8d6df25e4621a4d1c0c4fce55e`  
		Last Modified: Mon, 02 Aug 2021 21:21:19 GMT  
		Size: 4.9 MB (4906167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88866e210b82ee16f0597e85bdb4ecfcfa4a4fb779acf4fac118727f77793da4`  
		Last Modified: Mon, 02 Aug 2021 21:21:17 GMT  
		Size: 2.0 KB (1963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b0d7cfeb38017cedd34bb386132d75c45a4680749166f4725a12ec569559074`  
		Last Modified: Mon, 02 Aug 2021 21:21:17 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:505a0140bcef7327375fc3aaaded24b5afac6d0507406776accf695315b15b45`  
		Last Modified: Mon, 02 Aug 2021 21:21:18 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:249b0508ccf09dee8b24a8f7319126a4e8aad55ba989a0d96252ad5e55bbcd2a`  
		Last Modified: Mon, 02 Aug 2021 21:21:17 GMT  
		Size: 1.4 KB (1356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.3.3-windowsservercore` - windows version 10.0.14393.4530; amd64

```console
$ docker pull nats@sha256:4d913e48d6a0ea2ed11c62cc9fff622727736be864fa3a7fe0f15c35fc4b7b6f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6274947967 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eff8abf4d3ed2a1c41241ff4223442903b563fe0a6d8be426bcaed438d42bbbf`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Fri, 09 Jul 2021 05:02:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 14 Jul 2021 01:14:25 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 14 Jul 2021 02:35:48 GMT
ENV NATS_DOCKERIZED=1
# Mon, 02 Aug 2021 21:17:24 GMT
ENV NATS_SERVER=2.3.3
# Mon, 02 Aug 2021 21:17:26 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.3.3/nats-server-v2.3.3-windows-amd64.zip
# Mon, 02 Aug 2021 21:17:28 GMT
ENV NATS_SERVER_SHASUM=dd14c9c104adb657de4a67a17bdf2fc7d7f55860e7a17ce0c6b9c117d9a50dde
# Mon, 02 Aug 2021 21:18:41 GMT
RUN Set-PSDebug -Trace 2
# Mon, 02 Aug 2021 21:20:28 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Mon, 02 Aug 2021 21:20:31 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Mon, 02 Aug 2021 21:20:33 GMT
EXPOSE 4222 6222 8222
# Mon, 02 Aug 2021 21:20:36 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Mon, 02 Aug 2021 21:20:38 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a567de41cc349380b25967f180fb1b6b2431bda61ccaaf69d78a33bc9523614a`  
		Size: 2.2 GB (2199646155 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:fed351b78c876c55ec9c7e75d3b9d1b146c5c5dfeb4b5480c0a7c384322df98c`  
		Last Modified: Wed, 14 Jul 2021 02:03:37 GMT  
		Size: 1.4 KB (1444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf08cae8b8db8f3f89e1a9192d393f2da55b44efce4e778fdb58debe2d608275`  
		Last Modified: Wed, 14 Jul 2021 02:40:57 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:278db267454aa76e00b506fdd53726da5583419a7844eaa96889ff07827a02b7`  
		Last Modified: Mon, 02 Aug 2021 21:21:56 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb231d65d7756b89dfbb667d5b24a7bf72ba86e6d5d9c111ab0d08e3e862dfeb`  
		Last Modified: Mon, 02 Aug 2021 21:21:56 GMT  
		Size: 1.4 KB (1371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfa0b0c97c4ebf872cafc434ce68ec59df2a3cc66e12e83e929b2d7264559729`  
		Last Modified: Mon, 02 Aug 2021 21:21:55 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fe01d11f12da0e487e1ccf3918b3f6a77405b4992df67bc7a092380599cb022`  
		Last Modified: Mon, 02 Aug 2021 21:21:56 GMT  
		Size: 364.5 KB (364483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5da4bfe4915750d7b0192abb4ef4e16913fc4d8746d369529feaead5f8ef2918`  
		Last Modified: Mon, 02 Aug 2021 21:21:59 GMT  
		Size: 4.9 MB (4938295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd26f2047cfc6ccce7d850ea9ec880c9890f783dd0fa4ea9102c561cfa2aa5b5`  
		Last Modified: Mon, 02 Aug 2021 21:21:53 GMT  
		Size: 2.0 KB (1962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce9a1c92d84c4bec202df1e1353e7ecaad58b85a2a2940a9297d14d4548d9e53`  
		Last Modified: Mon, 02 Aug 2021 21:21:53 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dda461d40f36bee8ad537d4225843e28f90f20e81aa8a552d3ada4ef4dbc9f7a`  
		Last Modified: Mon, 02 Aug 2021 21:21:53 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29bf964afbf31f7d4891dc65a1db75f1254d540945a2697c483cdb0375c9b825`  
		Last Modified: Mon, 02 Aug 2021 21:21:53 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.3.3-windowsservercore-1809`

```console
$ docker pull nats@sha256:1f0cbe04efcaa08eaf910fa921d81d21cc52ff521414b7b02ebbf2b5890f0763
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2061; amd64

### `nats:2.3.3-windowsservercore-1809` - windows version 10.0.17763.2061; amd64

```console
$ docker pull nats@sha256:347fad05e489bf9e2c51d053e24efcce0d2031802c51a3feb8f4d2e7ab8765a9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2690730494 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1094808819e1865eaa575aa65800497b156f4e961675e37296ecd71758b68acf`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 06 Jul 2021 20:34:18 GMT
RUN Install update 1809-amd64
# Wed, 14 Jul 2021 01:07:27 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 14 Jul 2021 02:31:26 GMT
ENV NATS_DOCKERIZED=1
# Mon, 02 Aug 2021 21:14:23 GMT
ENV NATS_SERVER=2.3.3
# Mon, 02 Aug 2021 21:14:25 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.3.3/nats-server-v2.3.3-windows-amd64.zip
# Mon, 02 Aug 2021 21:14:28 GMT
ENV NATS_SERVER_SHASUM=dd14c9c104adb657de4a67a17bdf2fc7d7f55860e7a17ce0c6b9c117d9a50dde
# Mon, 02 Aug 2021 21:15:23 GMT
RUN Set-PSDebug -Trace 2
# Mon, 02 Aug 2021 21:16:45 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Mon, 02 Aug 2021 21:16:47 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Mon, 02 Aug 2021 21:16:49 GMT
EXPOSE 4222 6222 8222
# Mon, 02 Aug 2021 21:16:52 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Mon, 02 Aug 2021 21:16:54 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f143c6fed32d477c35b660b2e108ea62e3593c03e44bd9ced208ce52b26b0841`  
		Size: 967.1 MB (967113907 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:adcec6ff907307155c0652222cc9b95a0cc964d4c371e02767e72a5c90472192`  
		Last Modified: Wed, 14 Jul 2021 02:02:19 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f92bdc410321db22d4cf09322869bd9fb2495788c3725624c86d76a6ab3d95d3`  
		Last Modified: Wed, 14 Jul 2021 02:40:16 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c51291d3c5600cdb108e3ed994ab3d59042ca052eae615e136c35e3ac5f9bb6`  
		Last Modified: Mon, 02 Aug 2021 21:21:20 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:292fe7f01e91ae26c600f65e5c1f79e1cafd7d32145f63eda77265399a3c3804`  
		Last Modified: Mon, 02 Aug 2021 21:21:20 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17d5bb92d28832495b8124755df9034565b383dc7bc73be7f24838f425342d1a`  
		Last Modified: Mon, 02 Aug 2021 21:21:20 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8e0ae013ec15413637e098d44190826fe18ee0d434165a78f170bc86ce9c2fb`  
		Last Modified: Mon, 02 Aug 2021 21:21:20 GMT  
		Size: 364.2 KB (364232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4708b7da85335254f8c77a9656ef9c9034ed3d8d6df25e4621a4d1c0c4fce55e`  
		Last Modified: Mon, 02 Aug 2021 21:21:19 GMT  
		Size: 4.9 MB (4906167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88866e210b82ee16f0597e85bdb4ecfcfa4a4fb779acf4fac118727f77793da4`  
		Last Modified: Mon, 02 Aug 2021 21:21:17 GMT  
		Size: 2.0 KB (1963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b0d7cfeb38017cedd34bb386132d75c45a4680749166f4725a12ec569559074`  
		Last Modified: Mon, 02 Aug 2021 21:21:17 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:505a0140bcef7327375fc3aaaded24b5afac6d0507406776accf695315b15b45`  
		Last Modified: Mon, 02 Aug 2021 21:21:18 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:249b0508ccf09dee8b24a8f7319126a4e8aad55ba989a0d96252ad5e55bbcd2a`  
		Last Modified: Mon, 02 Aug 2021 21:21:17 GMT  
		Size: 1.4 KB (1356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.3.3-windowsservercore-ltsc2016`

```console
$ docker pull nats@sha256:a9dd3bec26866787cd33035a57d380c31c2f13a9b85f2d6d34a1b8bc79f3f9ff
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.14393.4530; amd64

### `nats:2.3.3-windowsservercore-ltsc2016` - windows version 10.0.14393.4530; amd64

```console
$ docker pull nats@sha256:4d913e48d6a0ea2ed11c62cc9fff622727736be864fa3a7fe0f15c35fc4b7b6f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6274947967 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eff8abf4d3ed2a1c41241ff4223442903b563fe0a6d8be426bcaed438d42bbbf`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Fri, 09 Jul 2021 05:02:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 14 Jul 2021 01:14:25 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 14 Jul 2021 02:35:48 GMT
ENV NATS_DOCKERIZED=1
# Mon, 02 Aug 2021 21:17:24 GMT
ENV NATS_SERVER=2.3.3
# Mon, 02 Aug 2021 21:17:26 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.3.3/nats-server-v2.3.3-windows-amd64.zip
# Mon, 02 Aug 2021 21:17:28 GMT
ENV NATS_SERVER_SHASUM=dd14c9c104adb657de4a67a17bdf2fc7d7f55860e7a17ce0c6b9c117d9a50dde
# Mon, 02 Aug 2021 21:18:41 GMT
RUN Set-PSDebug -Trace 2
# Mon, 02 Aug 2021 21:20:28 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Mon, 02 Aug 2021 21:20:31 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Mon, 02 Aug 2021 21:20:33 GMT
EXPOSE 4222 6222 8222
# Mon, 02 Aug 2021 21:20:36 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Mon, 02 Aug 2021 21:20:38 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a567de41cc349380b25967f180fb1b6b2431bda61ccaaf69d78a33bc9523614a`  
		Size: 2.2 GB (2199646155 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:fed351b78c876c55ec9c7e75d3b9d1b146c5c5dfeb4b5480c0a7c384322df98c`  
		Last Modified: Wed, 14 Jul 2021 02:03:37 GMT  
		Size: 1.4 KB (1444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf08cae8b8db8f3f89e1a9192d393f2da55b44efce4e778fdb58debe2d608275`  
		Last Modified: Wed, 14 Jul 2021 02:40:57 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:278db267454aa76e00b506fdd53726da5583419a7844eaa96889ff07827a02b7`  
		Last Modified: Mon, 02 Aug 2021 21:21:56 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb231d65d7756b89dfbb667d5b24a7bf72ba86e6d5d9c111ab0d08e3e862dfeb`  
		Last Modified: Mon, 02 Aug 2021 21:21:56 GMT  
		Size: 1.4 KB (1371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfa0b0c97c4ebf872cafc434ce68ec59df2a3cc66e12e83e929b2d7264559729`  
		Last Modified: Mon, 02 Aug 2021 21:21:55 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fe01d11f12da0e487e1ccf3918b3f6a77405b4992df67bc7a092380599cb022`  
		Last Modified: Mon, 02 Aug 2021 21:21:56 GMT  
		Size: 364.5 KB (364483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5da4bfe4915750d7b0192abb4ef4e16913fc4d8746d369529feaead5f8ef2918`  
		Last Modified: Mon, 02 Aug 2021 21:21:59 GMT  
		Size: 4.9 MB (4938295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd26f2047cfc6ccce7d850ea9ec880c9890f783dd0fa4ea9102c561cfa2aa5b5`  
		Last Modified: Mon, 02 Aug 2021 21:21:53 GMT  
		Size: 2.0 KB (1962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce9a1c92d84c4bec202df1e1353e7ecaad58b85a2a2940a9297d14d4548d9e53`  
		Last Modified: Mon, 02 Aug 2021 21:21:53 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dda461d40f36bee8ad537d4225843e28f90f20e81aa8a552d3ada4ef4dbc9f7a`  
		Last Modified: Mon, 02 Aug 2021 21:21:53 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29bf964afbf31f7d4891dc65a1db75f1254d540945a2697c483cdb0375c9b825`  
		Last Modified: Mon, 02 Aug 2021 21:21:53 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:alpine`

```console
$ docker pull nats@sha256:3ec525b1d139794286ecdb26410cff8ccf814eca88de9fe23c39a7d4b58479ef
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:alpine` - linux; amd64

```console
$ docker pull nats@sha256:b430407bf4008593c12a2cc85208f72e96b53fec98b30187c517b9d1958b657e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7601531 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:37a8e948168fcd8c0825a0cd425eb489bd313da994d65e73b5072d6ff6c8225a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 15 Jun 2021 22:19:37 GMT
ADD file:f278386b0cef68136129f5f58c52445590a417b624d62bca158d4dc926c340df in / 
# Tue, 15 Jun 2021 22:19:37 GMT
CMD ["/bin/sh"]
# Mon, 02 Aug 2021 21:22:41 GMT
ENV NATS_SERVER=2.3.3
# Mon, 02 Aug 2021 21:22:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f8e04470165fdfba062442cf5975f22668ab20fb12df7e299734e16a45370bef' ;; 		armhf) natsArch='arm6'; sha256='6396531f34e99cca903cdd461a79f1b8255d0cc219e5186ea15284b5b5e7e5e7' ;; 		armv7) natsArch='arm7'; sha256='4353de84d9e42b24b73ba98a4ed2a9eaa7c4f945bd68e1ddb4fbde885020ab30' ;; 		x86_64) natsArch='amd64'; sha256='66703b81de34d06060eb2198dfb5a1087547d45e680dee4da1214198a8073ce5' ;; 		x86) natsArch='386'; sha256='e38b9c9eda279bc4eee9cf6a3d4b2b25774b692450421a16e2ff6602977e6571' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Mon, 02 Aug 2021 21:22:44 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Mon, 02 Aug 2021 21:22:44 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 02 Aug 2021 21:22:44 GMT
EXPOSE 4222 6222 8222
# Mon, 02 Aug 2021 21:22:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 02 Aug 2021 21:22:45 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:5843afab387455b37944e709ee8c78d7520df80f8d01cf7f861aae63beeddb6b`  
		Last Modified: Tue, 15 Jun 2021 22:20:04 GMT  
		Size: 2.8 MB (2811478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03113b330e4f7fe35234354441a5bc0f8cabb61f7e7c02e1c2c7a9002be630c7`  
		Last Modified: Mon, 02 Aug 2021 21:23:32 GMT  
		Size: 4.8 MB (4789084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe9957a382ed4e85c0797d4c958c23eb4c68ab7e84a78c07a137bbf4bfd93c86`  
		Last Modified: Mon, 02 Aug 2021 21:23:31 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51734fe5b37d3390b972f615a9b12d4454a30ce0ed124f4a5d0f91a17d6ce6f8`  
		Last Modified: Mon, 02 Aug 2021 21:23:30 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:d5fc2c9df074891880beadedf530ee3dbf0761259a14619e946c1cefa842cac3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7079723 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f49351bac7a37d427b25fbdcc43daa3d1ea704fe96f3931802df83f01bf235c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 30 Jul 2021 17:49:42 GMT
ADD file:c80bc2b093cbc0fc466582ef21cbed377de9fa874aedbf320079525ddacd1200 in / 
# Fri, 30 Jul 2021 17:49:42 GMT
CMD ["/bin/sh"]
# Mon, 02 Aug 2021 21:16:47 GMT
ENV NATS_SERVER=2.3.3
# Mon, 02 Aug 2021 21:16:52 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f8e04470165fdfba062442cf5975f22668ab20fb12df7e299734e16a45370bef' ;; 		armhf) natsArch='arm6'; sha256='6396531f34e99cca903cdd461a79f1b8255d0cc219e5186ea15284b5b5e7e5e7' ;; 		armv7) natsArch='arm7'; sha256='4353de84d9e42b24b73ba98a4ed2a9eaa7c4f945bd68e1ddb4fbde885020ab30' ;; 		x86_64) natsArch='amd64'; sha256='66703b81de34d06060eb2198dfb5a1087547d45e680dee4da1214198a8073ce5' ;; 		x86) natsArch='386'; sha256='e38b9c9eda279bc4eee9cf6a3d4b2b25774b692450421a16e2ff6602977e6571' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Mon, 02 Aug 2021 21:16:52 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Mon, 02 Aug 2021 21:16:53 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 02 Aug 2021 21:16:53 GMT
EXPOSE 4222 6222 8222
# Mon, 02 Aug 2021 21:16:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 02 Aug 2021 21:16:54 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:b4c9a0924271af3466de27804af26420eb58da1466e7eaaba127d178b380fea3`  
		Last Modified: Tue, 15 Jun 2021 22:58:47 GMT  
		Size: 2.6 MB (2624382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e3313ef1b9ecd8d9e94997ae371b1c0aabda27773f0b2e12b4be7463517cf87`  
		Last Modified: Mon, 02 Aug 2021 21:18:59 GMT  
		Size: 4.5 MB (4454370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:785fbb490293d9c2f8cdaed64735e76ea2a0dc1c40e13814102053f6d9c4ddc3`  
		Last Modified: Mon, 02 Aug 2021 21:18:56 GMT  
		Size: 557.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ee9f0a3fdc78fe2942c2a3d6969418df884ad628f52adb50525f4022ed56ec2`  
		Last Modified: Mon, 02 Aug 2021 21:18:56 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:0cd94d122e5dd418d4d447257c6622e13c1d86149c0e7979057664951ab5a020
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.7 MB (6703143 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5635c4604b79a25fc3fdf3ccf6606d69eb347b3e8a3cb756dd261e2ca83e780`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 30 Jul 2021 18:36:19 GMT
ADD file:416a8b507abdc6bdcb22997a4be0a4170796c3f9f77e315b2dbff2b0a212bc68 in / 
# Fri, 30 Jul 2021 18:36:20 GMT
CMD ["/bin/sh"]
# Sat, 31 Jul 2021 03:13:57 GMT
ENV NATS_SERVER=2.3.2
# Sat, 31 Jul 2021 03:14:02 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='18a68cbef5c7a41052f5281bdfe9164b51cbeb60ce2dd31a7945c5adbcd39c2d' ;; 		armhf) natsArch='arm6'; sha256='a37949f8a1e24d5a8e47f57786e126205de7c3f6f8b3e5b849f33adbcfe8d2fb' ;; 		armv7) natsArch='arm7'; sha256='43a4820a57161b83fe721b81098d2ba9b1e2f42923be898f031bac40279f8f6e' ;; 		x86_64) natsArch='amd64'; sha256='6e6fdf781465fbf09cb024112b34ae6b2b432d94a5fc8b62f6ebf0da5fc3345d' ;; 		x86) natsArch='386'; sha256='c7c0ea9a5343925f0f5e2dda964946152382b0a3e0db96aa43c3f2ab17a37bf0' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Sat, 31 Jul 2021 03:14:03 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Sat, 31 Jul 2021 03:14:03 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Sat, 31 Jul 2021 03:14:04 GMT
EXPOSE 4222 6222 8222
# Sat, 31 Jul 2021 03:14:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 31 Jul 2021 03:14:05 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:136482bf81d1fa351b424ebb8c7e34d15f2c5ed3fc0b66b544b8312bda3d52d9`  
		Last Modified: Tue, 15 Jun 2021 23:16:40 GMT  
		Size: 2.4 MB (2427917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1a0b8bfe79fe7add5c0f3af812a506d01cc94a574cd58ba1f81146318d3638c`  
		Last Modified: Sat, 31 Jul 2021 03:16:43 GMT  
		Size: 4.3 MB (4274251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c35ac8f58b7f43ebc215a5713841cf5a94983b092019cf46da7ce8a3c9c84146`  
		Last Modified: Sat, 31 Jul 2021 03:16:40 GMT  
		Size: 560.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:735e5b5c342cb95f3f2eb33812321a4305479b159555d6fed062e4bb2880dc66`  
		Last Modified: Sat, 31 Jul 2021 03:16:40 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:f818c9007861b8440d5c89a859f8f20f483637ab3f3e7c7a7f89ef40afd23937
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7113993 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc01fa8c08e4612961dfe7cf6c422a1a58b99637fd0297f9c3d811b95a32c185`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 15 Jun 2021 21:44:56 GMT
ADD file:6797caacbfe41bfe44000b39ed017016c6fcc492b3d6557cdaba88536df6c876 in / 
# Tue, 15 Jun 2021 21:44:56 GMT
CMD ["/bin/sh"]
# Mon, 02 Aug 2021 21:06:09 GMT
ENV NATS_SERVER=2.3.3
# Mon, 02 Aug 2021 21:06:11 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f8e04470165fdfba062442cf5975f22668ab20fb12df7e299734e16a45370bef' ;; 		armhf) natsArch='arm6'; sha256='6396531f34e99cca903cdd461a79f1b8255d0cc219e5186ea15284b5b5e7e5e7' ;; 		armv7) natsArch='arm7'; sha256='4353de84d9e42b24b73ba98a4ed2a9eaa7c4f945bd68e1ddb4fbde885020ab30' ;; 		x86_64) natsArch='amd64'; sha256='66703b81de34d06060eb2198dfb5a1087547d45e680dee4da1214198a8073ce5' ;; 		x86) natsArch='386'; sha256='e38b9c9eda279bc4eee9cf6a3d4b2b25774b692450421a16e2ff6602977e6571' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Mon, 02 Aug 2021 21:06:11 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Mon, 02 Aug 2021 21:06:12 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 02 Aug 2021 21:06:12 GMT
EXPOSE 4222 6222 8222
# Mon, 02 Aug 2021 21:06:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 02 Aug 2021 21:06:12 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:58ab47519297212468320b23b8100fc1b2b96e8d342040806ae509a778a0a07a`  
		Last Modified: Tue, 15 Jun 2021 21:46:03 GMT  
		Size: 2.7 MB (2709626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0b71cb50e81b94a1183dec31a916ec92da12268c9d5c01358f63f093176829d`  
		Last Modified: Mon, 02 Aug 2021 21:07:22 GMT  
		Size: 4.4 MB (4403398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69e71c9cdab2ba7a29d11ef463c8173ea1cdc1f4a0a549ee1d8bdf0a21392641`  
		Last Modified: Mon, 02 Aug 2021 21:07:21 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17f4a027c87d570eda83fa005f1747518d8e6f172eaf1f5432d6073835418317`  
		Last Modified: Mon, 02 Aug 2021 21:07:21 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:alpine3.14`

```console
$ docker pull nats@sha256:3ec525b1d139794286ecdb26410cff8ccf814eca88de9fe23c39a7d4b58479ef
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:alpine3.14` - linux; amd64

```console
$ docker pull nats@sha256:b430407bf4008593c12a2cc85208f72e96b53fec98b30187c517b9d1958b657e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7601531 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:37a8e948168fcd8c0825a0cd425eb489bd313da994d65e73b5072d6ff6c8225a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 15 Jun 2021 22:19:37 GMT
ADD file:f278386b0cef68136129f5f58c52445590a417b624d62bca158d4dc926c340df in / 
# Tue, 15 Jun 2021 22:19:37 GMT
CMD ["/bin/sh"]
# Mon, 02 Aug 2021 21:22:41 GMT
ENV NATS_SERVER=2.3.3
# Mon, 02 Aug 2021 21:22:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f8e04470165fdfba062442cf5975f22668ab20fb12df7e299734e16a45370bef' ;; 		armhf) natsArch='arm6'; sha256='6396531f34e99cca903cdd461a79f1b8255d0cc219e5186ea15284b5b5e7e5e7' ;; 		armv7) natsArch='arm7'; sha256='4353de84d9e42b24b73ba98a4ed2a9eaa7c4f945bd68e1ddb4fbde885020ab30' ;; 		x86_64) natsArch='amd64'; sha256='66703b81de34d06060eb2198dfb5a1087547d45e680dee4da1214198a8073ce5' ;; 		x86) natsArch='386'; sha256='e38b9c9eda279bc4eee9cf6a3d4b2b25774b692450421a16e2ff6602977e6571' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Mon, 02 Aug 2021 21:22:44 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Mon, 02 Aug 2021 21:22:44 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 02 Aug 2021 21:22:44 GMT
EXPOSE 4222 6222 8222
# Mon, 02 Aug 2021 21:22:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 02 Aug 2021 21:22:45 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:5843afab387455b37944e709ee8c78d7520df80f8d01cf7f861aae63beeddb6b`  
		Last Modified: Tue, 15 Jun 2021 22:20:04 GMT  
		Size: 2.8 MB (2811478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03113b330e4f7fe35234354441a5bc0f8cabb61f7e7c02e1c2c7a9002be630c7`  
		Last Modified: Mon, 02 Aug 2021 21:23:32 GMT  
		Size: 4.8 MB (4789084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe9957a382ed4e85c0797d4c958c23eb4c68ab7e84a78c07a137bbf4bfd93c86`  
		Last Modified: Mon, 02 Aug 2021 21:23:31 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51734fe5b37d3390b972f615a9b12d4454a30ce0ed124f4a5d0f91a17d6ce6f8`  
		Last Modified: Mon, 02 Aug 2021 21:23:30 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.14` - linux; arm variant v6

```console
$ docker pull nats@sha256:d5fc2c9df074891880beadedf530ee3dbf0761259a14619e946c1cefa842cac3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7079723 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f49351bac7a37d427b25fbdcc43daa3d1ea704fe96f3931802df83f01bf235c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 30 Jul 2021 17:49:42 GMT
ADD file:c80bc2b093cbc0fc466582ef21cbed377de9fa874aedbf320079525ddacd1200 in / 
# Fri, 30 Jul 2021 17:49:42 GMT
CMD ["/bin/sh"]
# Mon, 02 Aug 2021 21:16:47 GMT
ENV NATS_SERVER=2.3.3
# Mon, 02 Aug 2021 21:16:52 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f8e04470165fdfba062442cf5975f22668ab20fb12df7e299734e16a45370bef' ;; 		armhf) natsArch='arm6'; sha256='6396531f34e99cca903cdd461a79f1b8255d0cc219e5186ea15284b5b5e7e5e7' ;; 		armv7) natsArch='arm7'; sha256='4353de84d9e42b24b73ba98a4ed2a9eaa7c4f945bd68e1ddb4fbde885020ab30' ;; 		x86_64) natsArch='amd64'; sha256='66703b81de34d06060eb2198dfb5a1087547d45e680dee4da1214198a8073ce5' ;; 		x86) natsArch='386'; sha256='e38b9c9eda279bc4eee9cf6a3d4b2b25774b692450421a16e2ff6602977e6571' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Mon, 02 Aug 2021 21:16:52 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Mon, 02 Aug 2021 21:16:53 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 02 Aug 2021 21:16:53 GMT
EXPOSE 4222 6222 8222
# Mon, 02 Aug 2021 21:16:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 02 Aug 2021 21:16:54 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:b4c9a0924271af3466de27804af26420eb58da1466e7eaaba127d178b380fea3`  
		Last Modified: Tue, 15 Jun 2021 22:58:47 GMT  
		Size: 2.6 MB (2624382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e3313ef1b9ecd8d9e94997ae371b1c0aabda27773f0b2e12b4be7463517cf87`  
		Last Modified: Mon, 02 Aug 2021 21:18:59 GMT  
		Size: 4.5 MB (4454370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:785fbb490293d9c2f8cdaed64735e76ea2a0dc1c40e13814102053f6d9c4ddc3`  
		Last Modified: Mon, 02 Aug 2021 21:18:56 GMT  
		Size: 557.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ee9f0a3fdc78fe2942c2a3d6969418df884ad628f52adb50525f4022ed56ec2`  
		Last Modified: Mon, 02 Aug 2021 21:18:56 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.14` - linux; arm variant v7

```console
$ docker pull nats@sha256:0cd94d122e5dd418d4d447257c6622e13c1d86149c0e7979057664951ab5a020
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.7 MB (6703143 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5635c4604b79a25fc3fdf3ccf6606d69eb347b3e8a3cb756dd261e2ca83e780`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 30 Jul 2021 18:36:19 GMT
ADD file:416a8b507abdc6bdcb22997a4be0a4170796c3f9f77e315b2dbff2b0a212bc68 in / 
# Fri, 30 Jul 2021 18:36:20 GMT
CMD ["/bin/sh"]
# Sat, 31 Jul 2021 03:13:57 GMT
ENV NATS_SERVER=2.3.2
# Sat, 31 Jul 2021 03:14:02 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='18a68cbef5c7a41052f5281bdfe9164b51cbeb60ce2dd31a7945c5adbcd39c2d' ;; 		armhf) natsArch='arm6'; sha256='a37949f8a1e24d5a8e47f57786e126205de7c3f6f8b3e5b849f33adbcfe8d2fb' ;; 		armv7) natsArch='arm7'; sha256='43a4820a57161b83fe721b81098d2ba9b1e2f42923be898f031bac40279f8f6e' ;; 		x86_64) natsArch='amd64'; sha256='6e6fdf781465fbf09cb024112b34ae6b2b432d94a5fc8b62f6ebf0da5fc3345d' ;; 		x86) natsArch='386'; sha256='c7c0ea9a5343925f0f5e2dda964946152382b0a3e0db96aa43c3f2ab17a37bf0' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Sat, 31 Jul 2021 03:14:03 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Sat, 31 Jul 2021 03:14:03 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Sat, 31 Jul 2021 03:14:04 GMT
EXPOSE 4222 6222 8222
# Sat, 31 Jul 2021 03:14:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 31 Jul 2021 03:14:05 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:136482bf81d1fa351b424ebb8c7e34d15f2c5ed3fc0b66b544b8312bda3d52d9`  
		Last Modified: Tue, 15 Jun 2021 23:16:40 GMT  
		Size: 2.4 MB (2427917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1a0b8bfe79fe7add5c0f3af812a506d01cc94a574cd58ba1f81146318d3638c`  
		Last Modified: Sat, 31 Jul 2021 03:16:43 GMT  
		Size: 4.3 MB (4274251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c35ac8f58b7f43ebc215a5713841cf5a94983b092019cf46da7ce8a3c9c84146`  
		Last Modified: Sat, 31 Jul 2021 03:16:40 GMT  
		Size: 560.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:735e5b5c342cb95f3f2eb33812321a4305479b159555d6fed062e4bb2880dc66`  
		Last Modified: Sat, 31 Jul 2021 03:16:40 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.14` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:f818c9007861b8440d5c89a859f8f20f483637ab3f3e7c7a7f89ef40afd23937
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7113993 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc01fa8c08e4612961dfe7cf6c422a1a58b99637fd0297f9c3d811b95a32c185`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 15 Jun 2021 21:44:56 GMT
ADD file:6797caacbfe41bfe44000b39ed017016c6fcc492b3d6557cdaba88536df6c876 in / 
# Tue, 15 Jun 2021 21:44:56 GMT
CMD ["/bin/sh"]
# Mon, 02 Aug 2021 21:06:09 GMT
ENV NATS_SERVER=2.3.3
# Mon, 02 Aug 2021 21:06:11 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f8e04470165fdfba062442cf5975f22668ab20fb12df7e299734e16a45370bef' ;; 		armhf) natsArch='arm6'; sha256='6396531f34e99cca903cdd461a79f1b8255d0cc219e5186ea15284b5b5e7e5e7' ;; 		armv7) natsArch='arm7'; sha256='4353de84d9e42b24b73ba98a4ed2a9eaa7c4f945bd68e1ddb4fbde885020ab30' ;; 		x86_64) natsArch='amd64'; sha256='66703b81de34d06060eb2198dfb5a1087547d45e680dee4da1214198a8073ce5' ;; 		x86) natsArch='386'; sha256='e38b9c9eda279bc4eee9cf6a3d4b2b25774b692450421a16e2ff6602977e6571' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Mon, 02 Aug 2021 21:06:11 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Mon, 02 Aug 2021 21:06:12 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 02 Aug 2021 21:06:12 GMT
EXPOSE 4222 6222 8222
# Mon, 02 Aug 2021 21:06:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 02 Aug 2021 21:06:12 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:58ab47519297212468320b23b8100fc1b2b96e8d342040806ae509a778a0a07a`  
		Last Modified: Tue, 15 Jun 2021 21:46:03 GMT  
		Size: 2.7 MB (2709626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0b71cb50e81b94a1183dec31a916ec92da12268c9d5c01358f63f093176829d`  
		Last Modified: Mon, 02 Aug 2021 21:07:22 GMT  
		Size: 4.4 MB (4403398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69e71c9cdab2ba7a29d11ef463c8173ea1cdc1f4a0a549ee1d8bdf0a21392641`  
		Last Modified: Mon, 02 Aug 2021 21:07:21 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17f4a027c87d570eda83fa005f1747518d8e6f172eaf1f5432d6073835418317`  
		Last Modified: Mon, 02 Aug 2021 21:07:21 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:latest`

```console
$ docker pull nats@sha256:6923c5f75f670dabe310c5dc2d3242e4f9ad4f1eabc625e18716358427ccd8d1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.2061; amd64

### `nats:latest` - linux; amd64

```console
$ docker pull nats@sha256:4f6857e56d3555432c7bc830fb297d8c00cbe3b0522f81dfc8c84a4dacb54ed5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4505352 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23830fcc7f9834fd409d95d2bf9877f21b609b7b7392bfcd4b8b5e62e8be14fc`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 02 Aug 2021 21:23:05 GMT
COPY file:0b22daa17d88302a2606c64df249d26684c5926e82494be3f08d920922b75196 in /nats-server 
# Mon, 02 Aug 2021 21:23:05 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Mon, 02 Aug 2021 21:23:05 GMT
EXPOSE 4222 6222 8222
# Mon, 02 Aug 2021 21:23:05 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 02 Aug 2021 21:23:05 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:267760e6058167430070f7584ea1e5e18b4ddf538aec80d4b764ba1b9096b403`  
		Last Modified: Mon, 02 Aug 2021 21:23:56 GMT  
		Size: 4.5 MB (4504877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:612bea9c73fc6c5c02659a6bff01f1bcada2f4c47323021b03bee52a9ca1eba0`  
		Last Modified: Mon, 02 Aug 2021 21:23:55 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm variant v6

```console
$ docker pull nats@sha256:6e42eec5a210d9a5b6d95c179d5c55193b69846c76786a81908536eac2efbdc3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4173716 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31e1feb9bf2ac457664507fc7899f48e45d49df93dd60eacdea8b8a9cda8ec51`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 02 Aug 2021 21:17:15 GMT
COPY file:55e1c39fb6ec9785ddf1c189ad5438b9f306c3e1c2a355512f4efc73aa1aacf6 in /nats-server 
# Mon, 02 Aug 2021 21:17:15 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Mon, 02 Aug 2021 21:17:16 GMT
EXPOSE 4222 6222 8222
# Mon, 02 Aug 2021 21:17:16 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 02 Aug 2021 21:17:17 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:7f318c30554fccfe6a5ac8a63f4457a20876b88ede949510db6a8f1c5bcf1442`  
		Last Modified: Mon, 02 Aug 2021 21:19:37 GMT  
		Size: 4.2 MB (4173243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76c9419bcd494c007ef4d4f83649e535bb32d84c81337abb67e153ad75a1fb5f`  
		Last Modified: Mon, 02 Aug 2021 21:19:35 GMT  
		Size: 473.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm variant v7

```console
$ docker pull nats@sha256:def02210305c7940addd2f5e26e8417017a2f2ae11116ee001b8f2a7bcb17bff
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.0 MB (3992886 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:20941bb671159cef8cb5d6b9047f5c6c298a495274b06f9c6d9278ea5f9e5a1f`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 07 Jul 2021 06:38:20 GMT
COPY file:a259b6f87cc2d22082524e5ba23201057e836734749f0d28676e8637d920d385 in /nats-server 
# Wed, 07 Jul 2021 06:38:21 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Wed, 07 Jul 2021 06:38:21 GMT
EXPOSE 4222 6222 8222
# Wed, 07 Jul 2021 06:38:22 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 07 Jul 2021 06:38:22 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:434fc0c4a6c5daa82c731102728bcac575b5a312862a89edf401b0305d2efc82`  
		Last Modified: Wed, 07 Jul 2021 06:40:42 GMT  
		Size: 4.0 MB (3992410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c195f08925b050ce566763c31c813f3d8c7e1ba40bc4ccdf0949cb87373c3a43`  
		Last Modified: Wed, 07 Jul 2021 06:40:39 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:7a367e1495e9df2cf9cc81af565194815e52b37c0ed1fd7e9f278d88311be5b4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.1 MB (4120338 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad1e0c5709f39238c0ff863c80e1595fb5da12e230643dc6fd4bd6b33cda4039`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 02 Aug 2021 21:06:28 GMT
COPY file:d94287ad868b49da5d590782f3102415d5dfd4ed2a775b4e4c10280c8ab25db3 in /nats-server 
# Mon, 02 Aug 2021 21:06:29 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Mon, 02 Aug 2021 21:06:29 GMT
EXPOSE 4222 6222 8222
# Mon, 02 Aug 2021 21:06:29 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 02 Aug 2021 21:06:29 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4ecc856c82596f8b8982843cac0e5ec138e9c881bfd322038cd7cf0f4942c9c9`  
		Last Modified: Mon, 02 Aug 2021 21:07:52 GMT  
		Size: 4.1 MB (4119864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68fa4df40d0356fc86fe0d6c780d2a447fe1b2c32b5572c65a3c7d2354961da4`  
		Last Modified: Mon, 02 Aug 2021 21:07:51 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - windows version 10.0.17763.2061; amd64

```console
$ docker pull nats@sha256:baf086eb51e7090cb2ef985758c034c882cbe1dd8d4b2a682a618d32b9215e35
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.3 MB (107296331 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d57bb9c1561692bbad5576428cd8e22189f1addf3a8b82e73e3f27e246bd485`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 06 Jul 2021 20:06:39 GMT
RUN Apply image 1809-amd64
# Wed, 14 Jul 2021 02:35:24 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Mon, 02 Aug 2021 21:17:05 GMT
RUN cmd /S /C #(nop) COPY file:359dd4a92709029cd62dc9620a8ff30527cb3494d6b89c9332ae019bae51b57b in C:\nats-server.exe 
# Mon, 02 Aug 2021 21:17:08 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Mon, 02 Aug 2021 21:17:10 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Mon, 02 Aug 2021 21:17:13 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Mon, 02 Aug 2021 21:17:16 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:29d43e56445c5279a6386c4dfe4d1ada3c7124ade9cb7b0f2757e58ffc7cd10b`  
		Size: 102.7 MB (102725622 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ec20c4c9f6fa5e782e09342d50033ef24c4049a9dad1befd33c96759b71da6de`  
		Last Modified: Wed, 14 Jul 2021 02:40:36 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab54ee8cb88b349708e6f2d10afe13c1d843b9c1ff995a70d40af5ca886eda42`  
		Last Modified: Mon, 02 Aug 2021 21:21:37 GMT  
		Size: 4.6 MB (4564319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27d161923a9b16db535efc5f78e4aedd08225387cc8377cedb826e7539fa9051`  
		Last Modified: Mon, 02 Aug 2021 21:21:36 GMT  
		Size: 1.8 KB (1766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e88c4ba846a11b45abc01afc7de665b15430ebfd4c6e585ba8cb11d896017cd`  
		Last Modified: Mon, 02 Aug 2021 21:21:36 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26ca1fda898c73546bdd8f1655f276fe9a0911a7c16f5a4054cdb40e996692c2`  
		Last Modified: Mon, 02 Aug 2021 21:21:36 GMT  
		Size: 1.2 KB (1180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:088b6cb05a147f4faf4e14f0fc1ecda8481f5ad0a8741dba786aebba4374207b`  
		Last Modified: Mon, 02 Aug 2021 21:21:36 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:linux`

```console
$ docker pull nats@sha256:111aefb3002e16ecc001abaa0bb5fc9aabf2510005be379d2cedc0373fa1e596
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:linux` - linux; amd64

```console
$ docker pull nats@sha256:4f6857e56d3555432c7bc830fb297d8c00cbe3b0522f81dfc8c84a4dacb54ed5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4505352 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23830fcc7f9834fd409d95d2bf9877f21b609b7b7392bfcd4b8b5e62e8be14fc`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 02 Aug 2021 21:23:05 GMT
COPY file:0b22daa17d88302a2606c64df249d26684c5926e82494be3f08d920922b75196 in /nats-server 
# Mon, 02 Aug 2021 21:23:05 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Mon, 02 Aug 2021 21:23:05 GMT
EXPOSE 4222 6222 8222
# Mon, 02 Aug 2021 21:23:05 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 02 Aug 2021 21:23:05 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:267760e6058167430070f7584ea1e5e18b4ddf538aec80d4b764ba1b9096b403`  
		Last Modified: Mon, 02 Aug 2021 21:23:56 GMT  
		Size: 4.5 MB (4504877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:612bea9c73fc6c5c02659a6bff01f1bcada2f4c47323021b03bee52a9ca1eba0`  
		Last Modified: Mon, 02 Aug 2021 21:23:55 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:6e42eec5a210d9a5b6d95c179d5c55193b69846c76786a81908536eac2efbdc3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4173716 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31e1feb9bf2ac457664507fc7899f48e45d49df93dd60eacdea8b8a9cda8ec51`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 02 Aug 2021 21:17:15 GMT
COPY file:55e1c39fb6ec9785ddf1c189ad5438b9f306c3e1c2a355512f4efc73aa1aacf6 in /nats-server 
# Mon, 02 Aug 2021 21:17:15 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Mon, 02 Aug 2021 21:17:16 GMT
EXPOSE 4222 6222 8222
# Mon, 02 Aug 2021 21:17:16 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 02 Aug 2021 21:17:17 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:7f318c30554fccfe6a5ac8a63f4457a20876b88ede949510db6a8f1c5bcf1442`  
		Last Modified: Mon, 02 Aug 2021 21:19:37 GMT  
		Size: 4.2 MB (4173243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76c9419bcd494c007ef4d4f83649e535bb32d84c81337abb67e153ad75a1fb5f`  
		Last Modified: Mon, 02 Aug 2021 21:19:35 GMT  
		Size: 473.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:def02210305c7940addd2f5e26e8417017a2f2ae11116ee001b8f2a7bcb17bff
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.0 MB (3992886 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:20941bb671159cef8cb5d6b9047f5c6c298a495274b06f9c6d9278ea5f9e5a1f`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 07 Jul 2021 06:38:20 GMT
COPY file:a259b6f87cc2d22082524e5ba23201057e836734749f0d28676e8637d920d385 in /nats-server 
# Wed, 07 Jul 2021 06:38:21 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Wed, 07 Jul 2021 06:38:21 GMT
EXPOSE 4222 6222 8222
# Wed, 07 Jul 2021 06:38:22 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 07 Jul 2021 06:38:22 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:434fc0c4a6c5daa82c731102728bcac575b5a312862a89edf401b0305d2efc82`  
		Last Modified: Wed, 07 Jul 2021 06:40:42 GMT  
		Size: 4.0 MB (3992410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c195f08925b050ce566763c31c813f3d8c7e1ba40bc4ccdf0949cb87373c3a43`  
		Last Modified: Wed, 07 Jul 2021 06:40:39 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:7a367e1495e9df2cf9cc81af565194815e52b37c0ed1fd7e9f278d88311be5b4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.1 MB (4120338 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad1e0c5709f39238c0ff863c80e1595fb5da12e230643dc6fd4bd6b33cda4039`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 02 Aug 2021 21:06:28 GMT
COPY file:d94287ad868b49da5d590782f3102415d5dfd4ed2a775b4e4c10280c8ab25db3 in /nats-server 
# Mon, 02 Aug 2021 21:06:29 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Mon, 02 Aug 2021 21:06:29 GMT
EXPOSE 4222 6222 8222
# Mon, 02 Aug 2021 21:06:29 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 02 Aug 2021 21:06:29 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4ecc856c82596f8b8982843cac0e5ec138e9c881bfd322038cd7cf0f4942c9c9`  
		Last Modified: Mon, 02 Aug 2021 21:07:52 GMT  
		Size: 4.1 MB (4119864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68fa4df40d0356fc86fe0d6c780d2a447fe1b2c32b5572c65a3c7d2354961da4`  
		Last Modified: Mon, 02 Aug 2021 21:07:51 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:nanoserver`

```console
$ docker pull nats@sha256:089f1003c28ef5e80a16a558155a581473b77e6d540a50934cc9d7fd5ca6a71b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2061; amd64

### `nats:nanoserver` - windows version 10.0.17763.2061; amd64

```console
$ docker pull nats@sha256:baf086eb51e7090cb2ef985758c034c882cbe1dd8d4b2a682a618d32b9215e35
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.3 MB (107296331 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d57bb9c1561692bbad5576428cd8e22189f1addf3a8b82e73e3f27e246bd485`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 06 Jul 2021 20:06:39 GMT
RUN Apply image 1809-amd64
# Wed, 14 Jul 2021 02:35:24 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Mon, 02 Aug 2021 21:17:05 GMT
RUN cmd /S /C #(nop) COPY file:359dd4a92709029cd62dc9620a8ff30527cb3494d6b89c9332ae019bae51b57b in C:\nats-server.exe 
# Mon, 02 Aug 2021 21:17:08 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Mon, 02 Aug 2021 21:17:10 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Mon, 02 Aug 2021 21:17:13 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Mon, 02 Aug 2021 21:17:16 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:29d43e56445c5279a6386c4dfe4d1ada3c7124ade9cb7b0f2757e58ffc7cd10b`  
		Size: 102.7 MB (102725622 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ec20c4c9f6fa5e782e09342d50033ef24c4049a9dad1befd33c96759b71da6de`  
		Last Modified: Wed, 14 Jul 2021 02:40:36 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab54ee8cb88b349708e6f2d10afe13c1d843b9c1ff995a70d40af5ca886eda42`  
		Last Modified: Mon, 02 Aug 2021 21:21:37 GMT  
		Size: 4.6 MB (4564319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27d161923a9b16db535efc5f78e4aedd08225387cc8377cedb826e7539fa9051`  
		Last Modified: Mon, 02 Aug 2021 21:21:36 GMT  
		Size: 1.8 KB (1766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e88c4ba846a11b45abc01afc7de665b15430ebfd4c6e585ba8cb11d896017cd`  
		Last Modified: Mon, 02 Aug 2021 21:21:36 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26ca1fda898c73546bdd8f1655f276fe9a0911a7c16f5a4054cdb40e996692c2`  
		Last Modified: Mon, 02 Aug 2021 21:21:36 GMT  
		Size: 1.2 KB (1180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:088b6cb05a147f4faf4e14f0fc1ecda8481f5ad0a8741dba786aebba4374207b`  
		Last Modified: Mon, 02 Aug 2021 21:21:36 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:nanoserver-1809`

```console
$ docker pull nats@sha256:089f1003c28ef5e80a16a558155a581473b77e6d540a50934cc9d7fd5ca6a71b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2061; amd64

### `nats:nanoserver-1809` - windows version 10.0.17763.2061; amd64

```console
$ docker pull nats@sha256:baf086eb51e7090cb2ef985758c034c882cbe1dd8d4b2a682a618d32b9215e35
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.3 MB (107296331 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d57bb9c1561692bbad5576428cd8e22189f1addf3a8b82e73e3f27e246bd485`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 06 Jul 2021 20:06:39 GMT
RUN Apply image 1809-amd64
# Wed, 14 Jul 2021 02:35:24 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Mon, 02 Aug 2021 21:17:05 GMT
RUN cmd /S /C #(nop) COPY file:359dd4a92709029cd62dc9620a8ff30527cb3494d6b89c9332ae019bae51b57b in C:\nats-server.exe 
# Mon, 02 Aug 2021 21:17:08 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Mon, 02 Aug 2021 21:17:10 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Mon, 02 Aug 2021 21:17:13 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Mon, 02 Aug 2021 21:17:16 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:29d43e56445c5279a6386c4dfe4d1ada3c7124ade9cb7b0f2757e58ffc7cd10b`  
		Size: 102.7 MB (102725622 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ec20c4c9f6fa5e782e09342d50033ef24c4049a9dad1befd33c96759b71da6de`  
		Last Modified: Wed, 14 Jul 2021 02:40:36 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab54ee8cb88b349708e6f2d10afe13c1d843b9c1ff995a70d40af5ca886eda42`  
		Last Modified: Mon, 02 Aug 2021 21:21:37 GMT  
		Size: 4.6 MB (4564319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27d161923a9b16db535efc5f78e4aedd08225387cc8377cedb826e7539fa9051`  
		Last Modified: Mon, 02 Aug 2021 21:21:36 GMT  
		Size: 1.8 KB (1766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e88c4ba846a11b45abc01afc7de665b15430ebfd4c6e585ba8cb11d896017cd`  
		Last Modified: Mon, 02 Aug 2021 21:21:36 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26ca1fda898c73546bdd8f1655f276fe9a0911a7c16f5a4054cdb40e996692c2`  
		Last Modified: Mon, 02 Aug 2021 21:21:36 GMT  
		Size: 1.2 KB (1180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:088b6cb05a147f4faf4e14f0fc1ecda8481f5ad0a8741dba786aebba4374207b`  
		Last Modified: Mon, 02 Aug 2021 21:21:36 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:scratch`

```console
$ docker pull nats@sha256:111aefb3002e16ecc001abaa0bb5fc9aabf2510005be379d2cedc0373fa1e596
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:scratch` - linux; amd64

```console
$ docker pull nats@sha256:4f6857e56d3555432c7bc830fb297d8c00cbe3b0522f81dfc8c84a4dacb54ed5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4505352 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23830fcc7f9834fd409d95d2bf9877f21b609b7b7392bfcd4b8b5e62e8be14fc`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 02 Aug 2021 21:23:05 GMT
COPY file:0b22daa17d88302a2606c64df249d26684c5926e82494be3f08d920922b75196 in /nats-server 
# Mon, 02 Aug 2021 21:23:05 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Mon, 02 Aug 2021 21:23:05 GMT
EXPOSE 4222 6222 8222
# Mon, 02 Aug 2021 21:23:05 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 02 Aug 2021 21:23:05 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:267760e6058167430070f7584ea1e5e18b4ddf538aec80d4b764ba1b9096b403`  
		Last Modified: Mon, 02 Aug 2021 21:23:56 GMT  
		Size: 4.5 MB (4504877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:612bea9c73fc6c5c02659a6bff01f1bcada2f4c47323021b03bee52a9ca1eba0`  
		Last Modified: Mon, 02 Aug 2021 21:23:55 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:6e42eec5a210d9a5b6d95c179d5c55193b69846c76786a81908536eac2efbdc3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4173716 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31e1feb9bf2ac457664507fc7899f48e45d49df93dd60eacdea8b8a9cda8ec51`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 02 Aug 2021 21:17:15 GMT
COPY file:55e1c39fb6ec9785ddf1c189ad5438b9f306c3e1c2a355512f4efc73aa1aacf6 in /nats-server 
# Mon, 02 Aug 2021 21:17:15 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Mon, 02 Aug 2021 21:17:16 GMT
EXPOSE 4222 6222 8222
# Mon, 02 Aug 2021 21:17:16 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 02 Aug 2021 21:17:17 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:7f318c30554fccfe6a5ac8a63f4457a20876b88ede949510db6a8f1c5bcf1442`  
		Last Modified: Mon, 02 Aug 2021 21:19:37 GMT  
		Size: 4.2 MB (4173243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76c9419bcd494c007ef4d4f83649e535bb32d84c81337abb67e153ad75a1fb5f`  
		Last Modified: Mon, 02 Aug 2021 21:19:35 GMT  
		Size: 473.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:def02210305c7940addd2f5e26e8417017a2f2ae11116ee001b8f2a7bcb17bff
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.0 MB (3992886 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:20941bb671159cef8cb5d6b9047f5c6c298a495274b06f9c6d9278ea5f9e5a1f`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 07 Jul 2021 06:38:20 GMT
COPY file:a259b6f87cc2d22082524e5ba23201057e836734749f0d28676e8637d920d385 in /nats-server 
# Wed, 07 Jul 2021 06:38:21 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Wed, 07 Jul 2021 06:38:21 GMT
EXPOSE 4222 6222 8222
# Wed, 07 Jul 2021 06:38:22 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 07 Jul 2021 06:38:22 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:434fc0c4a6c5daa82c731102728bcac575b5a312862a89edf401b0305d2efc82`  
		Last Modified: Wed, 07 Jul 2021 06:40:42 GMT  
		Size: 4.0 MB (3992410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c195f08925b050ce566763c31c813f3d8c7e1ba40bc4ccdf0949cb87373c3a43`  
		Last Modified: Wed, 07 Jul 2021 06:40:39 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:7a367e1495e9df2cf9cc81af565194815e52b37c0ed1fd7e9f278d88311be5b4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.1 MB (4120338 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad1e0c5709f39238c0ff863c80e1595fb5da12e230643dc6fd4bd6b33cda4039`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 02 Aug 2021 21:06:28 GMT
COPY file:d94287ad868b49da5d590782f3102415d5dfd4ed2a775b4e4c10280c8ab25db3 in /nats-server 
# Mon, 02 Aug 2021 21:06:29 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Mon, 02 Aug 2021 21:06:29 GMT
EXPOSE 4222 6222 8222
# Mon, 02 Aug 2021 21:06:29 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 02 Aug 2021 21:06:29 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4ecc856c82596f8b8982843cac0e5ec138e9c881bfd322038cd7cf0f4942c9c9`  
		Last Modified: Mon, 02 Aug 2021 21:07:52 GMT  
		Size: 4.1 MB (4119864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68fa4df40d0356fc86fe0d6c780d2a447fe1b2c32b5572c65a3c7d2354961da4`  
		Last Modified: Mon, 02 Aug 2021 21:07:51 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:windowsservercore`

```console
$ docker pull nats@sha256:d5e778d28d3d06f85d60c39772b380eb774d3f015b748c1491792a36c7a067f9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.2061; amd64
	-	windows version 10.0.14393.4530; amd64

### `nats:windowsservercore` - windows version 10.0.17763.2061; amd64

```console
$ docker pull nats@sha256:347fad05e489bf9e2c51d053e24efcce0d2031802c51a3feb8f4d2e7ab8765a9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2690730494 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1094808819e1865eaa575aa65800497b156f4e961675e37296ecd71758b68acf`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 06 Jul 2021 20:34:18 GMT
RUN Install update 1809-amd64
# Wed, 14 Jul 2021 01:07:27 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 14 Jul 2021 02:31:26 GMT
ENV NATS_DOCKERIZED=1
# Mon, 02 Aug 2021 21:14:23 GMT
ENV NATS_SERVER=2.3.3
# Mon, 02 Aug 2021 21:14:25 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.3.3/nats-server-v2.3.3-windows-amd64.zip
# Mon, 02 Aug 2021 21:14:28 GMT
ENV NATS_SERVER_SHASUM=dd14c9c104adb657de4a67a17bdf2fc7d7f55860e7a17ce0c6b9c117d9a50dde
# Mon, 02 Aug 2021 21:15:23 GMT
RUN Set-PSDebug -Trace 2
# Mon, 02 Aug 2021 21:16:45 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Mon, 02 Aug 2021 21:16:47 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Mon, 02 Aug 2021 21:16:49 GMT
EXPOSE 4222 6222 8222
# Mon, 02 Aug 2021 21:16:52 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Mon, 02 Aug 2021 21:16:54 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f143c6fed32d477c35b660b2e108ea62e3593c03e44bd9ced208ce52b26b0841`  
		Size: 967.1 MB (967113907 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:adcec6ff907307155c0652222cc9b95a0cc964d4c371e02767e72a5c90472192`  
		Last Modified: Wed, 14 Jul 2021 02:02:19 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f92bdc410321db22d4cf09322869bd9fb2495788c3725624c86d76a6ab3d95d3`  
		Last Modified: Wed, 14 Jul 2021 02:40:16 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c51291d3c5600cdb108e3ed994ab3d59042ca052eae615e136c35e3ac5f9bb6`  
		Last Modified: Mon, 02 Aug 2021 21:21:20 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:292fe7f01e91ae26c600f65e5c1f79e1cafd7d32145f63eda77265399a3c3804`  
		Last Modified: Mon, 02 Aug 2021 21:21:20 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17d5bb92d28832495b8124755df9034565b383dc7bc73be7f24838f425342d1a`  
		Last Modified: Mon, 02 Aug 2021 21:21:20 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8e0ae013ec15413637e098d44190826fe18ee0d434165a78f170bc86ce9c2fb`  
		Last Modified: Mon, 02 Aug 2021 21:21:20 GMT  
		Size: 364.2 KB (364232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4708b7da85335254f8c77a9656ef9c9034ed3d8d6df25e4621a4d1c0c4fce55e`  
		Last Modified: Mon, 02 Aug 2021 21:21:19 GMT  
		Size: 4.9 MB (4906167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88866e210b82ee16f0597e85bdb4ecfcfa4a4fb779acf4fac118727f77793da4`  
		Last Modified: Mon, 02 Aug 2021 21:21:17 GMT  
		Size: 2.0 KB (1963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b0d7cfeb38017cedd34bb386132d75c45a4680749166f4725a12ec569559074`  
		Last Modified: Mon, 02 Aug 2021 21:21:17 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:505a0140bcef7327375fc3aaaded24b5afac6d0507406776accf695315b15b45`  
		Last Modified: Mon, 02 Aug 2021 21:21:18 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:249b0508ccf09dee8b24a8f7319126a4e8aad55ba989a0d96252ad5e55bbcd2a`  
		Last Modified: Mon, 02 Aug 2021 21:21:17 GMT  
		Size: 1.4 KB (1356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:windowsservercore` - windows version 10.0.14393.4530; amd64

```console
$ docker pull nats@sha256:4d913e48d6a0ea2ed11c62cc9fff622727736be864fa3a7fe0f15c35fc4b7b6f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6274947967 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eff8abf4d3ed2a1c41241ff4223442903b563fe0a6d8be426bcaed438d42bbbf`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Fri, 09 Jul 2021 05:02:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 14 Jul 2021 01:14:25 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 14 Jul 2021 02:35:48 GMT
ENV NATS_DOCKERIZED=1
# Mon, 02 Aug 2021 21:17:24 GMT
ENV NATS_SERVER=2.3.3
# Mon, 02 Aug 2021 21:17:26 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.3.3/nats-server-v2.3.3-windows-amd64.zip
# Mon, 02 Aug 2021 21:17:28 GMT
ENV NATS_SERVER_SHASUM=dd14c9c104adb657de4a67a17bdf2fc7d7f55860e7a17ce0c6b9c117d9a50dde
# Mon, 02 Aug 2021 21:18:41 GMT
RUN Set-PSDebug -Trace 2
# Mon, 02 Aug 2021 21:20:28 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Mon, 02 Aug 2021 21:20:31 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Mon, 02 Aug 2021 21:20:33 GMT
EXPOSE 4222 6222 8222
# Mon, 02 Aug 2021 21:20:36 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Mon, 02 Aug 2021 21:20:38 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a567de41cc349380b25967f180fb1b6b2431bda61ccaaf69d78a33bc9523614a`  
		Size: 2.2 GB (2199646155 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:fed351b78c876c55ec9c7e75d3b9d1b146c5c5dfeb4b5480c0a7c384322df98c`  
		Last Modified: Wed, 14 Jul 2021 02:03:37 GMT  
		Size: 1.4 KB (1444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf08cae8b8db8f3f89e1a9192d393f2da55b44efce4e778fdb58debe2d608275`  
		Last Modified: Wed, 14 Jul 2021 02:40:57 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:278db267454aa76e00b506fdd53726da5583419a7844eaa96889ff07827a02b7`  
		Last Modified: Mon, 02 Aug 2021 21:21:56 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb231d65d7756b89dfbb667d5b24a7bf72ba86e6d5d9c111ab0d08e3e862dfeb`  
		Last Modified: Mon, 02 Aug 2021 21:21:56 GMT  
		Size: 1.4 KB (1371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfa0b0c97c4ebf872cafc434ce68ec59df2a3cc66e12e83e929b2d7264559729`  
		Last Modified: Mon, 02 Aug 2021 21:21:55 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fe01d11f12da0e487e1ccf3918b3f6a77405b4992df67bc7a092380599cb022`  
		Last Modified: Mon, 02 Aug 2021 21:21:56 GMT  
		Size: 364.5 KB (364483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5da4bfe4915750d7b0192abb4ef4e16913fc4d8746d369529feaead5f8ef2918`  
		Last Modified: Mon, 02 Aug 2021 21:21:59 GMT  
		Size: 4.9 MB (4938295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd26f2047cfc6ccce7d850ea9ec880c9890f783dd0fa4ea9102c561cfa2aa5b5`  
		Last Modified: Mon, 02 Aug 2021 21:21:53 GMT  
		Size: 2.0 KB (1962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce9a1c92d84c4bec202df1e1353e7ecaad58b85a2a2940a9297d14d4548d9e53`  
		Last Modified: Mon, 02 Aug 2021 21:21:53 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dda461d40f36bee8ad537d4225843e28f90f20e81aa8a552d3ada4ef4dbc9f7a`  
		Last Modified: Mon, 02 Aug 2021 21:21:53 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29bf964afbf31f7d4891dc65a1db75f1254d540945a2697c483cdb0375c9b825`  
		Last Modified: Mon, 02 Aug 2021 21:21:53 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:windowsservercore-1809`

```console
$ docker pull nats@sha256:1f0cbe04efcaa08eaf910fa921d81d21cc52ff521414b7b02ebbf2b5890f0763
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2061; amd64

### `nats:windowsservercore-1809` - windows version 10.0.17763.2061; amd64

```console
$ docker pull nats@sha256:347fad05e489bf9e2c51d053e24efcce0d2031802c51a3feb8f4d2e7ab8765a9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2690730494 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1094808819e1865eaa575aa65800497b156f4e961675e37296ecd71758b68acf`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 06 Jul 2021 20:34:18 GMT
RUN Install update 1809-amd64
# Wed, 14 Jul 2021 01:07:27 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 14 Jul 2021 02:31:26 GMT
ENV NATS_DOCKERIZED=1
# Mon, 02 Aug 2021 21:14:23 GMT
ENV NATS_SERVER=2.3.3
# Mon, 02 Aug 2021 21:14:25 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.3.3/nats-server-v2.3.3-windows-amd64.zip
# Mon, 02 Aug 2021 21:14:28 GMT
ENV NATS_SERVER_SHASUM=dd14c9c104adb657de4a67a17bdf2fc7d7f55860e7a17ce0c6b9c117d9a50dde
# Mon, 02 Aug 2021 21:15:23 GMT
RUN Set-PSDebug -Trace 2
# Mon, 02 Aug 2021 21:16:45 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Mon, 02 Aug 2021 21:16:47 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Mon, 02 Aug 2021 21:16:49 GMT
EXPOSE 4222 6222 8222
# Mon, 02 Aug 2021 21:16:52 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Mon, 02 Aug 2021 21:16:54 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f143c6fed32d477c35b660b2e108ea62e3593c03e44bd9ced208ce52b26b0841`  
		Size: 967.1 MB (967113907 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:adcec6ff907307155c0652222cc9b95a0cc964d4c371e02767e72a5c90472192`  
		Last Modified: Wed, 14 Jul 2021 02:02:19 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f92bdc410321db22d4cf09322869bd9fb2495788c3725624c86d76a6ab3d95d3`  
		Last Modified: Wed, 14 Jul 2021 02:40:16 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c51291d3c5600cdb108e3ed994ab3d59042ca052eae615e136c35e3ac5f9bb6`  
		Last Modified: Mon, 02 Aug 2021 21:21:20 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:292fe7f01e91ae26c600f65e5c1f79e1cafd7d32145f63eda77265399a3c3804`  
		Last Modified: Mon, 02 Aug 2021 21:21:20 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17d5bb92d28832495b8124755df9034565b383dc7bc73be7f24838f425342d1a`  
		Last Modified: Mon, 02 Aug 2021 21:21:20 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8e0ae013ec15413637e098d44190826fe18ee0d434165a78f170bc86ce9c2fb`  
		Last Modified: Mon, 02 Aug 2021 21:21:20 GMT  
		Size: 364.2 KB (364232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4708b7da85335254f8c77a9656ef9c9034ed3d8d6df25e4621a4d1c0c4fce55e`  
		Last Modified: Mon, 02 Aug 2021 21:21:19 GMT  
		Size: 4.9 MB (4906167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88866e210b82ee16f0597e85bdb4ecfcfa4a4fb779acf4fac118727f77793da4`  
		Last Modified: Mon, 02 Aug 2021 21:21:17 GMT  
		Size: 2.0 KB (1963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b0d7cfeb38017cedd34bb386132d75c45a4680749166f4725a12ec569559074`  
		Last Modified: Mon, 02 Aug 2021 21:21:17 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:505a0140bcef7327375fc3aaaded24b5afac6d0507406776accf695315b15b45`  
		Last Modified: Mon, 02 Aug 2021 21:21:18 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:249b0508ccf09dee8b24a8f7319126a4e8aad55ba989a0d96252ad5e55bbcd2a`  
		Last Modified: Mon, 02 Aug 2021 21:21:17 GMT  
		Size: 1.4 KB (1356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:windowsservercore-ltsc2016`

```console
$ docker pull nats@sha256:a9dd3bec26866787cd33035a57d380c31c2f13a9b85f2d6d34a1b8bc79f3f9ff
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.14393.4530; amd64

### `nats:windowsservercore-ltsc2016` - windows version 10.0.14393.4530; amd64

```console
$ docker pull nats@sha256:4d913e48d6a0ea2ed11c62cc9fff622727736be864fa3a7fe0f15c35fc4b7b6f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6274947967 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eff8abf4d3ed2a1c41241ff4223442903b563fe0a6d8be426bcaed438d42bbbf`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Fri, 09 Jul 2021 05:02:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 14 Jul 2021 01:14:25 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 14 Jul 2021 02:35:48 GMT
ENV NATS_DOCKERIZED=1
# Mon, 02 Aug 2021 21:17:24 GMT
ENV NATS_SERVER=2.3.3
# Mon, 02 Aug 2021 21:17:26 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.3.3/nats-server-v2.3.3-windows-amd64.zip
# Mon, 02 Aug 2021 21:17:28 GMT
ENV NATS_SERVER_SHASUM=dd14c9c104adb657de4a67a17bdf2fc7d7f55860e7a17ce0c6b9c117d9a50dde
# Mon, 02 Aug 2021 21:18:41 GMT
RUN Set-PSDebug -Trace 2
# Mon, 02 Aug 2021 21:20:28 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Mon, 02 Aug 2021 21:20:31 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Mon, 02 Aug 2021 21:20:33 GMT
EXPOSE 4222 6222 8222
# Mon, 02 Aug 2021 21:20:36 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Mon, 02 Aug 2021 21:20:38 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a567de41cc349380b25967f180fb1b6b2431bda61ccaaf69d78a33bc9523614a`  
		Size: 2.2 GB (2199646155 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:fed351b78c876c55ec9c7e75d3b9d1b146c5c5dfeb4b5480c0a7c384322df98c`  
		Last Modified: Wed, 14 Jul 2021 02:03:37 GMT  
		Size: 1.4 KB (1444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf08cae8b8db8f3f89e1a9192d393f2da55b44efce4e778fdb58debe2d608275`  
		Last Modified: Wed, 14 Jul 2021 02:40:57 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:278db267454aa76e00b506fdd53726da5583419a7844eaa96889ff07827a02b7`  
		Last Modified: Mon, 02 Aug 2021 21:21:56 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb231d65d7756b89dfbb667d5b24a7bf72ba86e6d5d9c111ab0d08e3e862dfeb`  
		Last Modified: Mon, 02 Aug 2021 21:21:56 GMT  
		Size: 1.4 KB (1371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfa0b0c97c4ebf872cafc434ce68ec59df2a3cc66e12e83e929b2d7264559729`  
		Last Modified: Mon, 02 Aug 2021 21:21:55 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fe01d11f12da0e487e1ccf3918b3f6a77405b4992df67bc7a092380599cb022`  
		Last Modified: Mon, 02 Aug 2021 21:21:56 GMT  
		Size: 364.5 KB (364483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5da4bfe4915750d7b0192abb4ef4e16913fc4d8746d369529feaead5f8ef2918`  
		Last Modified: Mon, 02 Aug 2021 21:21:59 GMT  
		Size: 4.9 MB (4938295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd26f2047cfc6ccce7d850ea9ec880c9890f783dd0fa4ea9102c561cfa2aa5b5`  
		Last Modified: Mon, 02 Aug 2021 21:21:53 GMT  
		Size: 2.0 KB (1962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce9a1c92d84c4bec202df1e1353e7ecaad58b85a2a2940a9297d14d4548d9e53`  
		Last Modified: Mon, 02 Aug 2021 21:21:53 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dda461d40f36bee8ad537d4225843e28f90f20e81aa8a552d3ada4ef4dbc9f7a`  
		Last Modified: Mon, 02 Aug 2021 21:21:53 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29bf964afbf31f7d4891dc65a1db75f1254d540945a2697c483cdb0375c9b825`  
		Last Modified: Mon, 02 Aug 2021 21:21:53 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
