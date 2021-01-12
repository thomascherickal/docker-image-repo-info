## `nats-streaming:alpine3.12`

```console
$ docker pull nats-streaming@sha256:8a523efff216bc402aa3cfbff2baa00cba890204bd3640ee99cfd9af9b71dc1f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:alpine3.12` - linux; amd64

```console
$ docker pull nats-streaming@sha256:f23e7901e6678f9427131aadcc75a95a91fb4c2ba46a005db8845ba1d5c7787f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.6 MB (9569779 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:67196f7de933f886026693bcb22ad853be6e6281c017c14733ad17f9339349c2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:41 GMT
ADD file:ec475c2abb2d46435286b5ae5efacf5b50b1a9e3b6293b69db3c0172b5b9658b in / 
# Thu, 17 Dec 2020 00:19:42 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 13:45:28 GMT
ENV NATS_STREAMING_SERVER=0.19.0
# Thu, 17 Dec 2020 13:45:33 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='d582023b8f9fe33b98f0faa6396aae8d5366ecade7e56cde912e21e5b93ea670' ;; 		armhf) natsArch='arm6'; sha256='f4af03e6cbb19f3ad9ea57217607dcf4b68018e1879859c847e2680917fc7139' ;; 		armv7) natsArch='arm7'; sha256='ec8c5ca693344e8b24de9ac955c38de757af8c5760658fc29ed2fbd804803fad' ;; 		x86_64) natsArch='amd64'; sha256='fc15530faec66b61de5140c2b99927c5839caff1c4c17f8bffbf4432fab83017' ;; 		x86) natsArch='386'; sha256='655f0f7cebf727317974006ad4a13ddacd3520f15266e854c2b01681e499bf80' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 17 Dec 2020 13:45:33 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Thu, 17 Dec 2020 13:45:33 GMT
EXPOSE 4222 8222
# Thu, 17 Dec 2020 13:45:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Dec 2020 13:45:34 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:801bfaa63ef2094d770c809815b9e2b9c1194728e5e754ef7bc764030e140cea`  
		Last Modified: Wed, 16 Dec 2020 19:34:50 GMT  
		Size: 2.8 MB (2799066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c64a51653d4053c34377310b5008de57d6224fbbb3065b8d39c2623ec0d79976`  
		Last Modified: Thu, 17 Dec 2020 13:46:30 GMT  
		Size: 6.8 MB (6770293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e070c7a0e34ad8644a164b7ddd81ba5780220bbf304ff6280e5386c323eb2ac0`  
		Last Modified: Thu, 17 Dec 2020 13:46:28 GMT  
		Size: 420.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine3.12` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:18fd3ddc15d5b65b6ad1171abf76e359cca31b60730750546e0dc0368a805750
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.3 MB (8330755 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0322ce6374b271fc98c0e0a12b42c00a722465006d75394c2ab41bbb47d50c46`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 16 Dec 2020 23:49:43 GMT
ADD file:0a16715e2d0e5811c3c578945d618db0e269847a799340248f9ba8d393c9eec2 in / 
# Wed, 16 Dec 2020 23:49:45 GMT
CMD ["/bin/sh"]
# Mon, 11 Jan 2021 23:53:38 GMT
ENV NATS_STREAMING_SERVER=0.20.0
# Mon, 11 Jan 2021 23:53:42 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='618008a4902916b6bdb26022343ab91313d4f7fc90b31d0c71ad9e75dc8299e4' ;; 		armhf) natsArch='arm6'; sha256='144b04f8f42793aee1b2deb3f6eb187648c37dcc32d526c607a0af99a847260d' ;; 		armv7) natsArch='arm7'; sha256='720f4a90d1dd536bc04639ae31c70ab46fb3e10556f0f261eb038fdce941f20c' ;; 		x86_64) natsArch='amd64'; sha256='098e2293cce5d457b92f3df35127789422562f1414427c406ffd03ea3bd687c9' ;; 		x86) natsArch='386'; sha256='322a290f4706f14d6ff8160ec437202bd282f61f0607741d0e4c38ef89b83451' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Mon, 11 Jan 2021 23:53:43 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Mon, 11 Jan 2021 23:53:44 GMT
EXPOSE 4222 8222
# Mon, 11 Jan 2021 23:53:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 11 Jan 2021 23:53:45 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:93247449aef3c56eb4f7ab7b3fed95743c974b823def6dd86ec84008126e7903`  
		Last Modified: Wed, 16 Dec 2020 23:50:24 GMT  
		Size: 2.6 MB (2604163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d54831e858eddfe2c245e8c154d4422ad61bc9a30c1cfe612ec35f7a12b1e529`  
		Last Modified: Mon, 11 Jan 2021 23:54:22 GMT  
		Size: 5.7 MB (5726171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:412a9e8bb4d16b7ddec81004c2205411fc7b8830d0d2a0f3054a2fe0dc4664cd`  
		Last Modified: Mon, 11 Jan 2021 23:54:20 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine3.12` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:327bffde98442421664114980572e9829a9b3d94d3d0ddd6f0454298c3b07035
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.7 MB (8732352 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6711b5f18d82236af21f862d8fcd2c2bfdcd38d5309184bd617c20b305ddd5f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 16 Dec 2020 23:58:14 GMT
ADD file:bd07f77a2b2741ca6bda80d9203be9c7274cf73145bff778cf000db0d8d4e903 in / 
# Wed, 16 Dec 2020 23:58:15 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 01:47:40 GMT
ENV NATS_STREAMING_SERVER=0.19.0
# Thu, 17 Dec 2020 01:47:45 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='d582023b8f9fe33b98f0faa6396aae8d5366ecade7e56cde912e21e5b93ea670' ;; 		armhf) natsArch='arm6'; sha256='f4af03e6cbb19f3ad9ea57217607dcf4b68018e1879859c847e2680917fc7139' ;; 		armv7) natsArch='arm7'; sha256='ec8c5ca693344e8b24de9ac955c38de757af8c5760658fc29ed2fbd804803fad' ;; 		x86_64) natsArch='amd64'; sha256='fc15530faec66b61de5140c2b99927c5839caff1c4c17f8bffbf4432fab83017' ;; 		x86) natsArch='386'; sha256='655f0f7cebf727317974006ad4a13ddacd3520f15266e854c2b01681e499bf80' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 17 Dec 2020 01:47:46 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Thu, 17 Dec 2020 01:47:47 GMT
EXPOSE 4222 8222
# Thu, 17 Dec 2020 01:47:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Dec 2020 01:47:48 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:c58e8a26a8407acc3ead776f6526efa889fda03270a8d05109208d9f59159420`  
		Last Modified: Wed, 16 Dec 2020 23:58:59 GMT  
		Size: 2.4 MB (2407555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4690136a7acc690baaa780fd5921752acda2b6fe1e6ec277bc354a6d4162b8ea`  
		Last Modified: Thu, 17 Dec 2020 01:48:23 GMT  
		Size: 6.3 MB (6324375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9de5ac561e04e3c2bd7c49b1cdcc1cb937c6f42db6a00b057f6b94617ae760b`  
		Last Modified: Thu, 17 Dec 2020 01:48:21 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine3.12` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:ae8f52346c3d26a49ae885bf56785f3952c14c8622a97e18288ae0abedd51660
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.4 MB (8377876 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5f79e7574653a33192a8af07510cf1a7f03f5c02a77b49072304e701cf514cf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 16 Dec 2020 23:40:26 GMT
ADD file:a4845c3840a3fd0e41e4635a179cce20c81afc6c02e34e3fd5bd2d535698918b in / 
# Wed, 16 Dec 2020 23:40:29 GMT
CMD ["/bin/sh"]
# Mon, 11 Jan 2021 23:47:10 GMT
ENV NATS_STREAMING_SERVER=0.20.0
# Mon, 11 Jan 2021 23:47:14 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='618008a4902916b6bdb26022343ab91313d4f7fc90b31d0c71ad9e75dc8299e4' ;; 		armhf) natsArch='arm6'; sha256='144b04f8f42793aee1b2deb3f6eb187648c37dcc32d526c607a0af99a847260d' ;; 		armv7) natsArch='arm7'; sha256='720f4a90d1dd536bc04639ae31c70ab46fb3e10556f0f261eb038fdce941f20c' ;; 		x86_64) natsArch='amd64'; sha256='098e2293cce5d457b92f3df35127789422562f1414427c406ffd03ea3bd687c9' ;; 		x86) natsArch='386'; sha256='322a290f4706f14d6ff8160ec437202bd282f61f0607741d0e4c38ef89b83451' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Mon, 11 Jan 2021 23:47:15 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Mon, 11 Jan 2021 23:47:15 GMT
EXPOSE 4222 8222
# Mon, 11 Jan 2021 23:47:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 11 Jan 2021 23:47:17 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:159e5727ea618dfe8b08811112e2c51f5bd2b9ae7db9eb214914a65249f70ca0`  
		Last Modified: Wed, 16 Dec 2020 23:41:08 GMT  
		Size: 2.7 MB (2709048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e424273d6cedd00225b67fa1b47e0dd8bf4b2abfa19fbc27f7763f096aeb138`  
		Last Modified: Mon, 11 Jan 2021 23:47:54 GMT  
		Size: 5.7 MB (5668408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33979e718e15555239006f224ba6d995cf9d6d044a7f25493196839d4d5aed73`  
		Last Modified: Mon, 11 Jan 2021 23:47:53 GMT  
		Size: 420.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
