## `nats:alpine3.13`

```console
$ docker pull nats@sha256:04056aae6c6ae545f8a1e126c8a861e9b9533ed7f14949e4fe9e9769821dd073
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:alpine3.13` - linux; amd64

```console
$ docker pull nats@sha256:0588bdd49eff9fbe5a97b3e59d8be059b2a3e28fc10028e5acc783c04168af62
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7278086 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d54139de8fa56bbc2ccf30efcab4bf2ac3d8fbd197fafdb1227536ec200fbd28`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 17 Feb 2021 21:19:54 GMT
ADD file:80bf8bd014071345b1c0364eeb0a5e48f3fb0d87f9c31cb990e57caa652b59b8 in / 
# Wed, 17 Feb 2021 21:19:54 GMT
CMD ["/bin/sh"]
# Mon, 15 Mar 2021 20:38:02 GMT
ENV NATS_SERVER=2.2.0
# Mon, 15 Mar 2021 20:38:05 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='4dfcf480a32d9ba7098477387d96a657a036ef9ad495a008a83e06b22df63999' ;; 		armhf) natsArch='arm6'; sha256='b82fdb2c8f6e7c731254730043c145423b5c48a3b40e33ad6e32bce029a9f086' ;; 		armv7) natsArch='arm7'; sha256='cffc326c7faeb5ea0769d0f04787d9885d5b2baabd32000d3b18b1130742772e' ;; 		x86_64) natsArch='amd64'; sha256='764ee4a9761185f92904c21c3de204c8b898e9a6bad6afac8b1fe512ce887417' ;; 		x86) natsArch='386'; sha256='a8067d9f26007bed3df2a72eebd4a813035a473058db1451d615ef5e96b30577' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Mon, 15 Mar 2021 20:38:06 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Mon, 15 Mar 2021 20:38:06 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 15 Mar 2021 20:38:06 GMT
EXPOSE 4222 6222 8222
# Mon, 15 Mar 2021 20:38:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 15 Mar 2021 20:38:06 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:ba3557a56b150f9b813f9d02274d62914fd8fce120dd374d9ee17b87cf1d277d`  
		Last Modified: Wed, 17 Feb 2021 21:20:25 GMT  
		Size: 2.8 MB (2811657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6de6c88bd8bb61feb100dc546a639f394479b63ab77b85b204b919c037e3561c`  
		Last Modified: Mon, 15 Mar 2021 20:38:45 GMT  
		Size: 4.5 MB (4465460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:441c16ca1333387827028b48699ebf7705fec9cba68418e481f6844a7a5ce84a`  
		Last Modified: Mon, 15 Mar 2021 20:38:44 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:363cd9ab055c3a7affd93e67333d1bbba811b592ec3c1dc8a0b449d14392ffcd`  
		Last Modified: Mon, 15 Mar 2021 20:38:44 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.13` - linux; arm variant v6

```console
$ docker pull nats@sha256:3b09aaa49e9ec674f064d69adde7ff3746fac00a4dfcd49c74bbde754a6486a3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6763843 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6bf1914719a1adcdac67b8cf15e7cf6f3c3f520405439a53770af13c049b7966`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 17 Feb 2021 20:49:32 GMT
ADD file:c04fbd3b039001c592cfa14f8388f8934ed4223ccf274dbb926e75039e172af4 in / 
# Wed, 17 Feb 2021 20:49:33 GMT
CMD ["/bin/sh"]
# Mon, 15 Mar 2021 21:15:53 GMT
ENV NATS_SERVER=2.2.0
# Mon, 15 Mar 2021 21:15:58 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='4dfcf480a32d9ba7098477387d96a657a036ef9ad495a008a83e06b22df63999' ;; 		armhf) natsArch='arm6'; sha256='b82fdb2c8f6e7c731254730043c145423b5c48a3b40e33ad6e32bce029a9f086' ;; 		armv7) natsArch='arm7'; sha256='cffc326c7faeb5ea0769d0f04787d9885d5b2baabd32000d3b18b1130742772e' ;; 		x86_64) natsArch='amd64'; sha256='764ee4a9761185f92904c21c3de204c8b898e9a6bad6afac8b1fe512ce887417' ;; 		x86) natsArch='386'; sha256='a8067d9f26007bed3df2a72eebd4a813035a473058db1451d615ef5e96b30577' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Mon, 15 Mar 2021 21:15:59 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Mon, 15 Mar 2021 21:15:59 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 15 Mar 2021 21:16:00 GMT
EXPOSE 4222 6222 8222
# Mon, 15 Mar 2021 21:16:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 15 Mar 2021 21:16:02 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:1353527ebe111f9bb1e271264a3c182e909e4b36463f80d7dbde1be0713eb892`  
		Last Modified: Wed, 17 Feb 2021 20:50:06 GMT  
		Size: 2.6 MB (2622039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7303c38c75c792b3baa6a38dd076a2776c8f9fded9e8b2d7922b82e65463b66e`  
		Last Modified: Mon, 15 Mar 2021 21:17:35 GMT  
		Size: 4.1 MB (4140833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:822378818180c446dcc1dbaf6cf750ce747aa292fd991f1844e83b23249db84f`  
		Last Modified: Mon, 15 Mar 2021 21:17:33 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7dbd40dab87b34d2855c1f53815d15407c9e80ae40ab94d258c4c88d1271c00`  
		Last Modified: Mon, 15 Mar 2021 21:17:33 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.13` - linux; arm variant v7

```console
$ docker pull nats@sha256:b864b2dd1d22aa7b79f42ac9e76d8a2cf236482a1a80366dd63d147cfd836c11
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6559845 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:362b7a041a42201c7f0f1e90623dd37ab077b5c5acb6596403e36ab6abadedf7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 17 Feb 2021 20:57:36 GMT
ADD file:efdd39e5243eaf378f12ad5a85d2222b44930850a90263e5f17e8a6b5e9bc9b8 in / 
# Wed, 17 Feb 2021 20:57:37 GMT
CMD ["/bin/sh"]
# Mon, 15 Mar 2021 21:20:49 GMT
ENV NATS_SERVER=2.2.0
# Mon, 15 Mar 2021 21:20:54 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='4dfcf480a32d9ba7098477387d96a657a036ef9ad495a008a83e06b22df63999' ;; 		armhf) natsArch='arm6'; sha256='b82fdb2c8f6e7c731254730043c145423b5c48a3b40e33ad6e32bce029a9f086' ;; 		armv7) natsArch='arm7'; sha256='cffc326c7faeb5ea0769d0f04787d9885d5b2baabd32000d3b18b1130742772e' ;; 		x86_64) natsArch='amd64'; sha256='764ee4a9761185f92904c21c3de204c8b898e9a6bad6afac8b1fe512ce887417' ;; 		x86) natsArch='386'; sha256='a8067d9f26007bed3df2a72eebd4a813035a473058db1451d615ef5e96b30577' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Mon, 15 Mar 2021 21:20:55 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Mon, 15 Mar 2021 21:20:56 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 15 Mar 2021 21:20:57 GMT
EXPOSE 4222 6222 8222
# Mon, 15 Mar 2021 21:20:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 15 Mar 2021 21:21:00 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:f55b840e27d3dbe27e44497103a4397f043749f933eb0433d29e2f104b3435ef`  
		Last Modified: Wed, 17 Feb 2021 20:58:14 GMT  
		Size: 2.4 MB (2423892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d27d2f1024ee6f137f679cc66d38363972f76824d87b5f16e4a751e6845f297b`  
		Last Modified: Mon, 15 Mar 2021 21:25:31 GMT  
		Size: 4.1 MB (4134980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:661d8a6cd44e4d001074e3f9da0ff480efb9de0846813635dba6b267eff76177`  
		Last Modified: Mon, 15 Mar 2021 21:25:30 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3426dd5b3f09fb5c0e8e720c12de50ab3890f37d36deb9198f5e5680232ac4e8`  
		Last Modified: Mon, 15 Mar 2021 21:25:31 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.13` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:ba5427cdb73e45d940e785bc123b0ecc0fe7aacb57e7222a188b75f29c54adf1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6821717 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:034dc01fad63fe260a0f644d8dda705c2c7658723244366989f4b8e17d23c0b9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 17 Feb 2021 20:39:29 GMT
ADD file:3bf1497bd250cf7c73c12231dc4ebe3a3a67f2cd99e35bce47ef6674683aeb1d in / 
# Wed, 17 Feb 2021 20:39:30 GMT
CMD ["/bin/sh"]
# Mon, 15 Mar 2021 22:09:42 GMT
ENV NATS_SERVER=2.2.0
# Mon, 15 Mar 2021 22:09:47 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='4dfcf480a32d9ba7098477387d96a657a036ef9ad495a008a83e06b22df63999' ;; 		armhf) natsArch='arm6'; sha256='b82fdb2c8f6e7c731254730043c145423b5c48a3b40e33ad6e32bce029a9f086' ;; 		armv7) natsArch='arm7'; sha256='cffc326c7faeb5ea0769d0f04787d9885d5b2baabd32000d3b18b1130742772e' ;; 		x86_64) natsArch='amd64'; sha256='764ee4a9761185f92904c21c3de204c8b898e9a6bad6afac8b1fe512ce887417' ;; 		x86) natsArch='386'; sha256='a8067d9f26007bed3df2a72eebd4a813035a473058db1451d615ef5e96b30577' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Mon, 15 Mar 2021 22:09:48 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Mon, 15 Mar 2021 22:09:49 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 15 Mar 2021 22:09:50 GMT
EXPOSE 4222 6222 8222
# Mon, 15 Mar 2021 22:09:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 15 Mar 2021 22:09:52 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:069a56d6d07f6b186fbb82e4486616b9be9a37ce32a63013af6cddcb65898182`  
		Last Modified: Wed, 17 Feb 2021 20:40:04 GMT  
		Size: 2.7 MB (2711572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df47184a8d6e652e9c3893688cadcfaac678dd9bba677246459c0451b14a53bd`  
		Last Modified: Mon, 15 Mar 2021 22:16:07 GMT  
		Size: 4.1 MB (4109175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d65589fd772e58c1aa03b1b49be83fa3909c9db60a4b8b10670b8ae85292e884`  
		Last Modified: Mon, 15 Mar 2021 22:16:07 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bd62fd1ff9c979fd53e99f28463065043c4cf0dc1091e2d7490bcca2e646eb3`  
		Last Modified: Mon, 15 Mar 2021 22:16:06 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
