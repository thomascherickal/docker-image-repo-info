## `nats:2-alpine3.16`

```console
$ docker pull nats@sha256:e5a371efe6187d5965b819b9152fbad9583f1750370a76961665837cfc97407f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-alpine3.16` - linux; arm variant v6

```console
$ docker pull nats@sha256:085e2d3603a5ffeb96a5e784f11532c03a4f0840b6d68974c49981ff00ae2403
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7567312 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9cc82d17b5c2168901fc2938dbcf28eb4107996ab8bc9eb7f577b8561f959058`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:22 GMT
ADD file:e8733e8cc0a81e15ca4041760b6e27392c34171512d34405a9b262b1fff5c687 in / 
# Tue, 09 Aug 2022 17:49:22 GMT
CMD ["/bin/sh"]
# Mon, 12 Sep 2022 18:49:32 GMT
ENV NATS_SERVER=2.9.0
# Mon, 12 Sep 2022 18:49:34 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='b82c2910819bbf9350a5040ba2145b5e17d0faf8fca502505a4845ce1dcba441' ;; 		armhf) natsArch='arm6'; sha256='4f5f02bd8e06e83d685f7cba76620ae76cdfb7bd94f89e3aea323bbd0bf6ab3b' ;; 		armv7) natsArch='arm7'; sha256='0af9e816fb4a47274d2f7b1d1ebebd13568f0b70d466feefdd04cf1f14a0195f' ;; 		x86_64) natsArch='amd64'; sha256='e2c678de6900dfd126ce181a1103201ac6fb4e63f7112d320932a011db64d4e0' ;; 		x86) natsArch='386'; sha256='a617f94da82e2518549d2192d336be1da09674498553d117a95e167c4f3425ca' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 12 Sep 2022 18:49:35 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 12 Sep 2022 18:49:35 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 12 Sep 2022 18:49:35 GMT
EXPOSE 4222 6222 8222
# Mon, 12 Sep 2022 18:49:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 12 Sep 2022 18:49:35 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9506b835437abb4d8ba1683e00c500b8f77e1975e930b356fbb72f2dbdc274d9`  
		Last Modified: Tue, 09 Aug 2022 17:50:33 GMT  
		Size: 2.6 MB (2613965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00fddff5163e8c58a7497154f421e89aff54a43caec19e95069cc494375041aa`  
		Last Modified: Mon, 12 Sep 2022 18:50:45 GMT  
		Size: 5.0 MB (4952345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8019ab673b790b4ed63a97187571f3d0e5f4eb16dfa17399f6a243d11ff5722b`  
		Last Modified: Mon, 12 Sep 2022 18:50:44 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5ceaa398303883b9d5e592ce9aeaccbcf4b34b99a27a67d1578a0d6de4e69d3`  
		Last Modified: Mon, 12 Sep 2022 18:50:44 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.16` - linux; arm variant v7

```console
$ docker pull nats@sha256:b95fa7ad87668f84962e4ef5abed9890fb57640ad479112b7f8c119bfa45dfda
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.4 MB (7363700 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b06933b06c17a95c6cd21d33dc823a06314c6b8517ebbfaf5b76c3b3cf11b155`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 16:57:44 GMT
ADD file:75521fe16320b193092588f6f31052c85e736965ceb11673de18bd14965a45e6 in / 
# Tue, 09 Aug 2022 16:57:44 GMT
CMD ["/bin/sh"]
# Mon, 12 Sep 2022 19:03:51 GMT
ENV NATS_SERVER=2.9.0
# Mon, 12 Sep 2022 19:03:54 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='b82c2910819bbf9350a5040ba2145b5e17d0faf8fca502505a4845ce1dcba441' ;; 		armhf) natsArch='arm6'; sha256='4f5f02bd8e06e83d685f7cba76620ae76cdfb7bd94f89e3aea323bbd0bf6ab3b' ;; 		armv7) natsArch='arm7'; sha256='0af9e816fb4a47274d2f7b1d1ebebd13568f0b70d466feefdd04cf1f14a0195f' ;; 		x86_64) natsArch='amd64'; sha256='e2c678de6900dfd126ce181a1103201ac6fb4e63f7112d320932a011db64d4e0' ;; 		x86) natsArch='386'; sha256='a617f94da82e2518549d2192d336be1da09674498553d117a95e167c4f3425ca' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 12 Sep 2022 19:03:54 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 12 Sep 2022 19:03:54 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 12 Sep 2022 19:03:54 GMT
EXPOSE 4222 6222 8222
# Mon, 12 Sep 2022 19:03:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 12 Sep 2022 19:03:55 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:c6556b3b6858c6fa1e328377cc2c4becdc9cd1bc3e7302aa7299936522cf93ba`  
		Last Modified: Tue, 09 Aug 2022 16:58:55 GMT  
		Size: 2.4 MB (2417065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3571a588810a8fe42813cdd7bcdc3e7b0be7bfc9084e38508f050f9826bba19`  
		Last Modified: Mon, 12 Sep 2022 19:05:22 GMT  
		Size: 4.9 MB (4945636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b1bcd898e16c2896f273f1b98e85da9bae6f599fb25e92fcdb2cab7ba63d64d`  
		Last Modified: Mon, 12 Sep 2022 19:05:20 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21cdba5340addabedb9b0801b2c8d51c4b04c684965b7e4f9b25e8b44573fb78`  
		Last Modified: Mon, 12 Sep 2022 19:05:20 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.16` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:7869a7f7498ee46895e9948a102087841874c9ee049696fe96edc9c4c5f7b17c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.5 MB (7482302 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e7cded970df3ac075d6833bcc805ee1cd39b6de8728ce00785f95016a231117`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Mon, 12 Sep 2022 18:50:02 GMT
ENV NATS_SERVER=2.9.0
# Mon, 12 Sep 2022 18:50:04 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='b82c2910819bbf9350a5040ba2145b5e17d0faf8fca502505a4845ce1dcba441' ;; 		armhf) natsArch='arm6'; sha256='4f5f02bd8e06e83d685f7cba76620ae76cdfb7bd94f89e3aea323bbd0bf6ab3b' ;; 		armv7) natsArch='arm7'; sha256='0af9e816fb4a47274d2f7b1d1ebebd13568f0b70d466feefdd04cf1f14a0195f' ;; 		x86_64) natsArch='amd64'; sha256='e2c678de6900dfd126ce181a1103201ac6fb4e63f7112d320932a011db64d4e0' ;; 		x86) natsArch='386'; sha256='a617f94da82e2518549d2192d336be1da09674498553d117a95e167c4f3425ca' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 12 Sep 2022 18:50:06 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 12 Sep 2022 18:50:07 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 12 Sep 2022 18:50:07 GMT
EXPOSE 4222 6222 8222
# Mon, 12 Sep 2022 18:50:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 12 Sep 2022 18:50:09 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f13b8dbdcf7252f528110cd3097a32511e40b830a0e7690d5d3c7c544cbbace`  
		Last Modified: Mon, 12 Sep 2022 18:51:12 GMT  
		Size: 4.8 MB (4773665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27cb8435ac86def6a8973b25db155dbd8c3f0c407542046937eb1ab78b99276e`  
		Last Modified: Mon, 12 Sep 2022 18:51:11 GMT  
		Size: 561.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a47359896823731079e2553b7cf975eba66a0095c51b1ccffbe582b732a6d41b`  
		Last Modified: Mon, 12 Sep 2022 18:51:11 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
