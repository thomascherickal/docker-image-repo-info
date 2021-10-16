## `nats-streaming:alpine`

```console
$ docker pull nats-streaming@sha256:2a7a810a5bb19349a2e43fcb4f4cf22f83374b98aff961745b3d2b4cd6ebba92
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:alpine` - linux; amd64

```console
$ docker pull nats-streaming@sha256:9d1a14ec8294f02ad61859abbae261ed58e52656ca742e506fc959664b834904
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.4 MB (10380582 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d15d33fcb55af1db00c97fe142efd0d2b9474767a61be57bf2c04f7d245c8e71`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 15 Oct 2021 23:32:18 GMT
ENV NATS_STREAMING_SERVER=0.23.0
# Fri, 15 Oct 2021 23:32:21 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='997b1235349360c46d37588047f5b1b64e7a8603b84478edf153124f3a0b6fbf' ;; 		armhf) natsArch='arm6'; sha256='127e953a64ba7d88039cf7d688a29f968cadcac2a65e43bf2c93e4055665358f' ;; 		armv7) natsArch='arm7'; sha256='d5f9bf496419f4874c2a10a668d04a858d269aec1b31306e1289ccb12b03217e' ;; 		x86_64) natsArch='amd64'; sha256='4695eca8dbc09c1e363b5e2725eada3a1412a3a71f002ce1208aaab91c03e3d1' ;; 		x86) natsArch='386'; sha256='b6c06a9b1edf69cfa764bc499302d27127212787bbc107045f814ad378eaed49' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 15 Oct 2021 23:32:22 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Fri, 15 Oct 2021 23:32:22 GMT
EXPOSE 4222 8222
# Fri, 15 Oct 2021 23:32:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 15 Oct 2021 23:32:22 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9d98635b1c67ba74edd1c339053b799e81535f34ede771018aa3d1acd660b1b`  
		Last Modified: Fri, 15 Oct 2021 23:33:11 GMT  
		Size: 7.6 MB (7565714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22ad9a9bb37a13d2b80423d6893b9217cc45bfc227b6084ac664d6edb1cda628`  
		Last Modified: Fri, 15 Oct 2021 23:33:09 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:94e32218185bce38079a89646554af12973d9c1a66ffc9f423be40fa5e7f5e48
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.7 MB (9667646 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c2a4a22be20ed6a78d3dc32468da4408ee3ad94d70127fb08162e8c8746a554`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 27 Aug 2021 17:49:29 GMT
ADD file:1c1c4520d49cb6e8f795f3b953d1ed3c3c77868b98b53a455169c254fcec5acd in / 
# Fri, 27 Aug 2021 17:49:30 GMT
CMD ["/bin/sh"]
# Sat, 16 Oct 2021 00:09:49 GMT
ENV NATS_STREAMING_SERVER=0.23.0
# Sat, 16 Oct 2021 00:09:54 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='997b1235349360c46d37588047f5b1b64e7a8603b84478edf153124f3a0b6fbf' ;; 		armhf) natsArch='arm6'; sha256='127e953a64ba7d88039cf7d688a29f968cadcac2a65e43bf2c93e4055665358f' ;; 		armv7) natsArch='arm7'; sha256='d5f9bf496419f4874c2a10a668d04a858d269aec1b31306e1289ccb12b03217e' ;; 		x86_64) natsArch='amd64'; sha256='4695eca8dbc09c1e363b5e2725eada3a1412a3a71f002ce1208aaab91c03e3d1' ;; 		x86) natsArch='386'; sha256='b6c06a9b1edf69cfa764bc499302d27127212787bbc107045f814ad378eaed49' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Sat, 16 Oct 2021 00:09:55 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Sat, 16 Oct 2021 00:09:55 GMT
EXPOSE 4222 8222
# Sat, 16 Oct 2021 00:09:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 16 Oct 2021 00:09:56 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:2e78c0f86ba9a1fed30df20cb48c9cc73e9626399f12749d36b892ff99c0ecf5`  
		Last Modified: Fri, 27 Aug 2021 17:50:55 GMT  
		Size: 2.6 MB (2627447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecfda0054989a71c89a82b1f380260d3777cc5519f77c1bf34125a4b3463ed9b`  
		Last Modified: Sat, 16 Oct 2021 00:11:39 GMT  
		Size: 7.0 MB (7039777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06b9a84c28137138f528f26f1146a1cec8d0a0c5ceb5ab4dc89fe5758c96ec55`  
		Last Modified: Sat, 16 Oct 2021 00:11:34 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:709bf964baa04bed21788daab878aaf76613f67b25782dfa91f68dac883c1e96
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.4 MB (9352403 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:120c9c54d0d41980417a67786d13b07474948f1a4fe697b1bfe029344e8b5d55`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 27 Aug 2021 17:57:31 GMT
ADD file:a7da7992ccea54d3295231027614f138aa45c4d4a25ea6ec9bf7b316b9f67d95 in / 
# Fri, 27 Aug 2021 17:57:32 GMT
CMD ["/bin/sh"]
# Fri, 27 Aug 2021 21:15:57 GMT
ENV NATS_STREAMING_SERVER=0.22.1
# Fri, 27 Aug 2021 21:16:03 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='581698d248a19ecae64e4048d153bc1021744a3da6284680a339f9f82a53a9cf' ;; 		armhf) natsArch='arm6'; sha256='438a89221bb0608e40d21e73ca27a4b70b8560730726942c0ade94a6b6013d6f' ;; 		armv7) natsArch='arm7'; sha256='4164baadd201d1374f7654d3e54a24d81ceb87a385867e31a82c1d1a69e3b1ae' ;; 		x86_64) natsArch='amd64'; sha256='f29e87ac9ff998c928aa8ebc8cf0c4d04d34a3d95b9900d92fd7dafab2bec8cc' ;; 		x86) natsArch='386'; sha256='0ca68e57babb8901d7afeb7569042730904887e718ddf860ef3ee54278753505' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 27 Aug 2021 21:16:03 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Fri, 27 Aug 2021 21:16:04 GMT
EXPOSE 4222 8222
# Fri, 27 Aug 2021 21:16:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 Aug 2021 21:16:05 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:a14774a5a62e0f454febaec7cb603e18a6a8e25ef9da4a4da85b155bdd5e5a7a`  
		Last Modified: Fri, 27 Aug 2021 17:59:00 GMT  
		Size: 2.4 MB (2430419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7d0e8657e131875280f89b03741d9c7b5b154791cef8ce515fe711e4185a32d`  
		Last Modified: Fri, 27 Aug 2021 21:17:51 GMT  
		Size: 6.9 MB (6921563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20506d2b8361ef74d3f9c4e5dc7489f829d0181c070aca1b163eb8f540762e4c`  
		Last Modified: Fri, 27 Aug 2021 21:17:47 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:c62bf392316ddd25875ed160e0dbd43b3eb58f79e2b216d210959498f48551cf
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.6 MB (9644840 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3719e8038a8fa3be083d1e31199895ce43c32a2b70a6f244e8f36b05e0b091d7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Sat, 16 Oct 2021 00:03:02 GMT
ENV NATS_STREAMING_SERVER=0.23.0
# Sat, 16 Oct 2021 00:03:05 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='997b1235349360c46d37588047f5b1b64e7a8603b84478edf153124f3a0b6fbf' ;; 		armhf) natsArch='arm6'; sha256='127e953a64ba7d88039cf7d688a29f968cadcac2a65e43bf2c93e4055665358f' ;; 		armv7) natsArch='arm7'; sha256='d5f9bf496419f4874c2a10a668d04a858d269aec1b31306e1289ccb12b03217e' ;; 		x86_64) natsArch='amd64'; sha256='4695eca8dbc09c1e363b5e2725eada3a1412a3a71f002ce1208aaab91c03e3d1' ;; 		x86) natsArch='386'; sha256='b6c06a9b1edf69cfa764bc499302d27127212787bbc107045f814ad378eaed49' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Sat, 16 Oct 2021 00:03:07 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Sat, 16 Oct 2021 00:03:07 GMT
EXPOSE 4222 8222
# Sat, 16 Oct 2021 00:03:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 16 Oct 2021 00:03:09 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:552d1f2373af9bfe12033568ebbfb0ccbb0de11279f9a415a29207e264d7f4d9`  
		Last Modified: Fri, 27 Aug 2021 17:40:18 GMT  
		Size: 2.7 MB (2711827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9016e5cac797bd165a69dd41ff1d64e5fa2949672aa9281e36d865b6404e0b5d`  
		Last Modified: Sat, 16 Oct 2021 00:03:58 GMT  
		Size: 6.9 MB (6932593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac73239a7164496d5fc076e03bf08e5438d03208201b539b5adf840f49296215`  
		Last Modified: Sat, 16 Oct 2021 00:03:56 GMT  
		Size: 420.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
