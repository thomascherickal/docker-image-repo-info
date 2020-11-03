## `nats:2-alpine`

```console
$ docker pull nats@sha256:4e1350061030e0de15fd0528877b26cc28d429361e50b48a8f4a32df24f7224e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-alpine` - linux; amd64

```console
$ docker pull nats@sha256:a6f914658a5f8a7a82c9005a3a36863628d331cb2cd4c0c0a3653e7e8a7c0d95
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7208222 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:96815e17bf1191cbfa7a1745a82f87b8fcc43fbd793da4d66c9fd175c136dd27`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:03 GMT
ADD file:b91adb67b670d3a6ff9463e48b7def903ed516be66fc4282d22c53e41512be49 in / 
# Fri, 24 Apr 2020 01:05:03 GMT
CMD ["/bin/sh"]
# Fri, 04 Sep 2020 19:23:32 GMT
ENV NATS_SERVER=2.1.8
# Fri, 04 Sep 2020 19:23:34 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='567d5c7f80305b8876230204b993f0cf213411d006d931a036b26dd2288ac81b' ;; 		armhf) natsArch='arm6'; sha256='d76c1ed6f660e13faaa8b1c058723981aa59436ce7d4d4e208ae486395db458f' ;; 		armv7) natsArch='arm7'; sha256='e26f0eba9b065f9537986f88233f279f44c01487aacffe65d4d7440129a5d0a2' ;; 		x86_64) natsArch='amd64'; sha256='8ec25475ef1d49bf5e721de38deb11d689d1a9b2fa588540af78d56cbea2b49d' ;; 		x86) natsArch='386'; sha256='e8535179805573e9d684cc8aa6f79551ab9fcfacd45643d7ba2174e176997d9e' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 04 Sep 2020 19:23:34 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 04 Sep 2020 19:23:34 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 04 Sep 2020 19:23:35 GMT
EXPOSE 4222 6222 8222
# Fri, 04 Sep 2020 19:23:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 04 Sep 2020 19:23:35 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:cbdbe7a5bc2a134ca8ec91be58565ec07d037386d1f1d8385412d224deafca08`  
		Last Modified: Thu, 23 Apr 2020 14:07:19 GMT  
		Size: 2.8 MB (2813316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7f9fca7275bd535bd4680297f95f240c9b48d96d0b9b7f17dd38b73917d2b99`  
		Last Modified: Fri, 04 Sep 2020 19:24:56 GMT  
		Size: 4.4 MB (4393961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6905e1079d9ad73fb2f14b529adb1378cfaa4fcabf48ee0a819af4a49842a3a4`  
		Last Modified: Fri, 04 Sep 2020 19:24:55 GMT  
		Size: 530.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a148278ed7ad77a22a36b3ea6e6cdbcaa397edc556440f575992b8bbd8abfc9b`  
		Last Modified: Fri, 04 Sep 2020 19:24:55 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:9e48df44aebb727f47d0dcba60b78c28a0ef104e36ff33080ecc8aace4f7b268
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.7 MB (6702104 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19529e739baf0662c8730673c66c4b5fd30e95cf209a9aa4c92aeee96f944d22`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 22 Oct 2020 02:01:09 GMT
ADD file:dec4d3b6cf21c59820d1d74a554d0a193b5f4859e00b932f31ffe73f554d5afb in / 
# Thu, 22 Oct 2020 02:01:12 GMT
CMD ["/bin/sh"]
# Mon, 02 Nov 2020 23:53:12 GMT
ENV NATS_SERVER=2.1.9
# Mon, 02 Nov 2020 23:53:15 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='22659ec3653a2db53294427c8ec939a3b9d207a36ea54daf945b9fa43477434d' ;; 		armhf) natsArch='arm6'; sha256='761d1062303e9637196ab3b329d01609ea907d297e6c10f6932212b62ff9b1b4' ;; 		armv7) natsArch='arm7'; sha256='0a000c41c5031969f7b855cf4c65d5e6b1d6cd2230857f728a190a6ee128828c' ;; 		x86_64) natsArch='amd64'; sha256='c9538f4a47ffe75d11f3c5ce1e1c9a3c6ae1e26e26f7a1428ca5dda6b1b476d1' ;; 		x86) natsArch='386'; sha256='079cbfc5f42ebbe2b696fdc88c75ffdebd3b9f34e88d61a829ced064ab48a749' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Mon, 02 Nov 2020 23:53:16 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Mon, 02 Nov 2020 23:53:17 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 02 Nov 2020 23:53:17 GMT
EXPOSE 4222 6222 8222
# Mon, 02 Nov 2020 23:53:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 02 Nov 2020 23:53:18 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:bad30e7b45c14f784ef29a828b5fc69db0ebdefebcde6a7c98f4f77ffc93a546`  
		Last Modified: Thu, 22 Oct 2020 02:01:42 GMT  
		Size: 2.6 MB (2601912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3160b7583dbd74fb51d0252fa0081efe742be228ffce0f8a8376b5fd40406c0d`  
		Last Modified: Mon, 02 Nov 2020 23:53:59 GMT  
		Size: 4.1 MB (4099220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3aaddabf5d9ffe7bfcbfdf91dcc457fa4df2b23ac4092c8fdaaafcaac17c1cf7`  
		Last Modified: Mon, 02 Nov 2020 23:53:58 GMT  
		Size: 559.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a0f36eeef476b5d018b5a4d45c3faa40dfd23693bdbd60011f9c55f808d9c70`  
		Last Modified: Mon, 02 Nov 2020 23:53:58 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:57a1feff0b8a1d875b723f8610882b4a440c5743b412ec85ef067d1ccba969c1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 MB (6501277 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:023d468e0ee5d5f12746ec4d791b447385a9ba784869e5d72cd799b98569b839`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 22 Oct 2020 01:58:13 GMT
ADD file:46f89172426e9f5b1d669a2ca7ab218fc2deaef1caeeab88f2b5bd443ac9773d in / 
# Thu, 22 Oct 2020 01:58:14 GMT
CMD ["/bin/sh"]
# Tue, 03 Nov 2020 00:03:16 GMT
ENV NATS_SERVER=2.1.9
# Tue, 03 Nov 2020 00:03:19 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='22659ec3653a2db53294427c8ec939a3b9d207a36ea54daf945b9fa43477434d' ;; 		armhf) natsArch='arm6'; sha256='761d1062303e9637196ab3b329d01609ea907d297e6c10f6932212b62ff9b1b4' ;; 		armv7) natsArch='arm7'; sha256='0a000c41c5031969f7b855cf4c65d5e6b1d6cd2230857f728a190a6ee128828c' ;; 		x86_64) natsArch='amd64'; sha256='c9538f4a47ffe75d11f3c5ce1e1c9a3c6ae1e26e26f7a1428ca5dda6b1b476d1' ;; 		x86) natsArch='386'; sha256='079cbfc5f42ebbe2b696fdc88c75ffdebd3b9f34e88d61a829ced064ab48a749' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Tue, 03 Nov 2020 00:03:20 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Tue, 03 Nov 2020 00:03:21 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 03 Nov 2020 00:03:21 GMT
EXPOSE 4222 6222 8222
# Tue, 03 Nov 2020 00:03:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 03 Nov 2020 00:03:23 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:5f2023fd85a4e68f37fe41421fd89f30e69b98a645613521c57c01317561eee3`  
		Last Modified: Thu, 22 Oct 2020 01:58:45 GMT  
		Size: 2.4 MB (2405675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dfce6983e3f7c06d074642c9b764d3233981dca2919b8d28e1239ffdde794d9`  
		Last Modified: Tue, 03 Nov 2020 00:04:17 GMT  
		Size: 4.1 MB (4094632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f7049631684363461d086d36dd5cab857aa52e898ffcddb6da26ccd8eaf27b4`  
		Last Modified: Tue, 03 Nov 2020 00:04:16 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbfa4e9bce9726a8a6a7e2a357bc9012a2c3f6078047c5e30d7ff9f2d56358e4`  
		Last Modified: Tue, 03 Nov 2020 00:04:17 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:700235b690efc969452c359aa31b2b636e1001730ac02e9d67aec2f035b23370
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6819487 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7c44b6c5226c848ac88f68fb752a7650eec2ef1ebd3b91fba0e525f5903f7ee3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 24 Apr 2020 00:14:18 GMT
ADD file:85ae77bc1e43353ff14e6fe1658be1ed4ecbf4330212ac3d7ab7462add32dd39 in / 
# Fri, 24 Apr 2020 00:14:21 GMT
CMD ["/bin/sh"]
# Fri, 04 Sep 2020 19:40:30 GMT
ENV NATS_SERVER=2.1.8
# Fri, 04 Sep 2020 19:40:34 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='567d5c7f80305b8876230204b993f0cf213411d006d931a036b26dd2288ac81b' ;; 		armhf) natsArch='arm6'; sha256='d76c1ed6f660e13faaa8b1c058723981aa59436ce7d4d4e208ae486395db458f' ;; 		armv7) natsArch='arm7'; sha256='e26f0eba9b065f9537986f88233f279f44c01487aacffe65d4d7440129a5d0a2' ;; 		x86_64) natsArch='amd64'; sha256='8ec25475ef1d49bf5e721de38deb11d689d1a9b2fa588540af78d56cbea2b49d' ;; 		x86) natsArch='386'; sha256='e8535179805573e9d684cc8aa6f79551ab9fcfacd45643d7ba2174e176997d9e' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 04 Sep 2020 19:40:35 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 04 Sep 2020 19:40:35 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 04 Sep 2020 19:40:36 GMT
EXPOSE 4222 6222 8222
# Fri, 04 Sep 2020 19:40:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 04 Sep 2020 19:40:37 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:29e5d40040c18c692ed73df24511071725b74956ca1a61fe6056a651d86a13bd`  
		Last Modified: Fri, 24 Apr 2020 00:15:41 GMT  
		Size: 2.7 MB (2724424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d3d1d8b6792cec2b145ec7c0c1b6107e3712804cbd65a93c4d6bc4f5a540ce2`  
		Last Modified: Fri, 04 Sep 2020 19:51:31 GMT  
		Size: 4.1 MB (4094087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c256e59f9e1973a41cd6c2d2af211bfb10c5534b990b63e9c81790cd3c1bdbf3`  
		Last Modified: Fri, 04 Sep 2020 19:51:29 GMT  
		Size: 561.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71ea7fd4055fec9b7d9f52d74d616f372dbd367262c3cec827ce3ddc633e3efc`  
		Last Modified: Fri, 04 Sep 2020 19:51:29 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
