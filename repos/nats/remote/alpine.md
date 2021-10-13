## `nats:alpine`

```console
$ docker pull nats@sha256:8ffeb310d3ca33f5c5cad8f2a1cb6f971ddfc3fa264c05f46daa26cc09190eb7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:alpine` - linux; amd64

```console
$ docker pull nats@sha256:14cc6a656f138d1e3e707e88c18ef88452b29ccb72af4176b8f5f78d23748030
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.7 MB (7655041 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f5d1cad0ce15a4e94e87f82b966b73e25ba0d4629eb29c09178beb3f5af0b43`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 24 Sep 2021 18:20:14 GMT
ENV NATS_SERVER=2.6.1
# Fri, 24 Sep 2021 18:20:17 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='4354bdc411f63fa1528479b39b9312de1e1c23531136d88c6b58978dcbf1ec29' ;; 		armhf) natsArch='arm6'; sha256='65473af9ff2f0c75b65609722ad8eb37ee495b382a16697b0168a02abd7bf0f9' ;; 		armv7) natsArch='arm7'; sha256='c95287f62472566bbe30941b57dc4df6547ea5d6219615c3666ae4d5f3acd9d9' ;; 		x86_64) natsArch='amd64'; sha256='9168ba515d68cce426874096d0be2510d9846de66c74c7ab3ecbdc2a27e9c114' ;; 		x86) natsArch='386'; sha256='8f83456101181c7a0a59e83be03c4ec54d6a34737609d97575e2a4f47a08aa24' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 24 Sep 2021 18:20:18 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 24 Sep 2021 18:20:18 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 24 Sep 2021 18:20:18 GMT
EXPOSE 4222 6222 8222
# Fri, 24 Sep 2021 18:20:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Sep 2021 18:20:18 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb318bc128d118ab570ff784f370b12bba9799d4b8ead06996ddb459d55ba9f4`  
		Last Modified: Fri, 24 Sep 2021 18:21:22 GMT  
		Size: 4.8 MB (4839621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9abea9d20040e530947975d310bc6504f29c3518f07ca9320cf04a81b0372d03`  
		Last Modified: Fri, 24 Sep 2021 18:21:21 GMT  
		Size: 561.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f787462ffd44dbb2ccc478572962380ecf84219b3f54034a8244cab789596707`  
		Last Modified: Fri, 24 Sep 2021 18:21:21 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:b66e17fed81f78bfbade4b7df09380660a6116411d67d0f35c45bc9052371006
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7137044 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c74f19d7e07b4a0f3fa0b0ba0130868922801363e4bde23047bbc98550870e5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:49:29 GMT
ADD file:1c1c4520d49cb6e8f795f3b953d1ed3c3c77868b98b53a455169c254fcec5acd in / 
# Fri, 27 Aug 2021 17:49:30 GMT
CMD ["/bin/sh"]
# Tue, 12 Oct 2021 23:49:34 GMT
ENV NATS_SERVER=2.6.2
# Tue, 12 Oct 2021 23:49:39 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='040b4fbd896240d91dfec258d159731fa98eac0a8329a0009c65dee8a875d1a0' ;; 		armhf) natsArch='arm6'; sha256='1bba8a38b61bc4f95bc89a4038b34c7dadbd5e05ca93e4a28d0b98cc11b1c101' ;; 		armv7) natsArch='arm7'; sha256='ef0a719476e5e84f173c7abcf379c7a2ae8b1472ad397fd9e72909362f426679' ;; 		x86_64) natsArch='amd64'; sha256='cc6c6b737e8ecadbba2480518897c5a9fd2168fdd8115664a734f582d4c8c759' ;; 		x86) natsArch='386'; sha256='785539ec342ca08ebbfff72871ec570b19c3eee29dc357c0047af33aa387dadb' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Tue, 12 Oct 2021 23:49:39 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Tue, 12 Oct 2021 23:49:40 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 12 Oct 2021 23:49:40 GMT
EXPOSE 4222 6222 8222
# Tue, 12 Oct 2021 23:49:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 12 Oct 2021 23:49:41 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:2e78c0f86ba9a1fed30df20cb48c9cc73e9626399f12749d36b892ff99c0ecf5`  
		Last Modified: Fri, 27 Aug 2021 17:50:55 GMT  
		Size: 2.6 MB (2627447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:004dac4814d8a10e132980bc0c9fc26f1b132815155952b39410b19de4bdfffb`  
		Last Modified: Tue, 12 Oct 2021 23:51:48 GMT  
		Size: 4.5 MB (4508626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfc1ac7d223637b9928337142770c52955d5340766ff58dcf405505f154442eb`  
		Last Modified: Tue, 12 Oct 2021 23:51:45 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5ddd7eaa459a35633b8f07a40f5f36fa5f9666c49347b9341a0ca30f502dbb3`  
		Last Modified: Tue, 12 Oct 2021 23:51:45 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:d9fc63779407554a8674633e5732621f680292866c780da9f007ce29d75542e1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.9 MB (6927152 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1e1c6d9848dce815735e333708e9e35533486997ca7f3031b655d4c398a92b2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:57:31 GMT
ADD file:a7da7992ccea54d3295231027614f138aa45c4d4a25ea6ec9bf7b316b9f67d95 in / 
# Fri, 27 Aug 2021 17:57:32 GMT
CMD ["/bin/sh"]
# Thu, 30 Sep 2021 19:47:23 GMT
ENV NATS_SERVER=2.6.1
# Thu, 30 Sep 2021 19:47:28 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='4354bdc411f63fa1528479b39b9312de1e1c23531136d88c6b58978dcbf1ec29' ;; 		armhf) natsArch='arm6'; sha256='65473af9ff2f0c75b65609722ad8eb37ee495b382a16697b0168a02abd7bf0f9' ;; 		armv7) natsArch='arm7'; sha256='c95287f62472566bbe30941b57dc4df6547ea5d6219615c3666ae4d5f3acd9d9' ;; 		x86_64) natsArch='amd64'; sha256='9168ba515d68cce426874096d0be2510d9846de66c74c7ab3ecbdc2a27e9c114' ;; 		x86) natsArch='386'; sha256='8f83456101181c7a0a59e83be03c4ec54d6a34737609d97575e2a4f47a08aa24' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 30 Sep 2021 19:47:28 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 30 Sep 2021 19:47:29 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 30 Sep 2021 19:47:29 GMT
EXPOSE 4222 6222 8222
# Thu, 30 Sep 2021 19:47:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Sep 2021 19:47:30 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:a14774a5a62e0f454febaec7cb603e18a6a8e25ef9da4a4da85b155bdd5e5a7a`  
		Last Modified: Fri, 27 Aug 2021 17:59:00 GMT  
		Size: 2.4 MB (2430419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d00126b6dca785aa0a1a05eae3f9dca609d9677a0b164c6f686ab687589b5a3a`  
		Last Modified: Thu, 30 Sep 2021 19:49:42 GMT  
		Size: 4.5 MB (4495760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d70fb5271d804ff6a23c62bea2d0df5fe9b68466315efe98ab09239efa418c9`  
		Last Modified: Thu, 30 Sep 2021 19:49:38 GMT  
		Size: 559.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b47f9daa3ced3fd472321b155a7206875a5603a287f70b05bdd184ffbd55c647`  
		Last Modified: Thu, 30 Sep 2021 19:49:38 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:38888e1c67f76b7edbb92804a050b5de8e4e4f6ae8a980f919d17de7f1fcd4f3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7162092 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:700188dc91cf1626d6b15bb088a273301826130510c19b4dcc9fa42a7f8592ae`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Fri, 24 Sep 2021 17:40:05 GMT
ENV NATS_SERVER=2.6.1
# Fri, 24 Sep 2021 17:40:08 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='4354bdc411f63fa1528479b39b9312de1e1c23531136d88c6b58978dcbf1ec29' ;; 		armhf) natsArch='arm6'; sha256='65473af9ff2f0c75b65609722ad8eb37ee495b382a16697b0168a02abd7bf0f9' ;; 		armv7) natsArch='arm7'; sha256='c95287f62472566bbe30941b57dc4df6547ea5d6219615c3666ae4d5f3acd9d9' ;; 		x86_64) natsArch='amd64'; sha256='9168ba515d68cce426874096d0be2510d9846de66c74c7ab3ecbdc2a27e9c114' ;; 		x86) natsArch='386'; sha256='8f83456101181c7a0a59e83be03c4ec54d6a34737609d97575e2a4f47a08aa24' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 24 Sep 2021 17:40:08 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 24 Sep 2021 17:40:08 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 24 Sep 2021 17:40:08 GMT
EXPOSE 4222 6222 8222
# Fri, 24 Sep 2021 17:40:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Sep 2021 17:40:09 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:552d1f2373af9bfe12033568ebbfb0ccbb0de11279f9a415a29207e264d7f4d9`  
		Last Modified: Fri, 27 Aug 2021 17:40:18 GMT  
		Size: 2.7 MB (2711827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1047b8662a09fdfa7dea8086cf9e2a632d09dd8f2848de9a500d15ae3c2bf7a9`  
		Last Modified: Fri, 24 Sep 2021 17:41:28 GMT  
		Size: 4.4 MB (4449294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84477e5068504078a4d643a66ae31db7aead8076162df1016404ea7f6ec479f9`  
		Last Modified: Fri, 24 Sep 2021 17:41:27 GMT  
		Size: 557.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4c94a831ef4c3b67a6834a3a36c58f4d6c60d52de703d7780d6d7ef071673bd`  
		Last Modified: Fri, 24 Sep 2021 17:41:27 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
