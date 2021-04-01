## `nats:2-alpine`

```console
$ docker pull nats@sha256:ece4acb6a22288af4da0016e4af11c093f935d2d68ed74fd5b4b88869dd292c6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-alpine` - linux; amd64

```console
$ docker pull nats@sha256:faf06335ff05259553a7cd85c508540576e73735f878f991bdb316639c5beba8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7278367 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:baae0ba3d35d13f1ab017cea5d7a4c34e55d533b5f83ee0887f4e46b9df6169d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 31 Mar 2021 20:10:06 GMT
ADD file:7119167b56ff1228b2fb639c768955ce9db7a999cd947179240b216dfa5ccbb9 in / 
# Wed, 31 Mar 2021 20:10:06 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 14:29:19 GMT
ENV NATS_SERVER=2.2.0
# Thu, 01 Apr 2021 14:29:22 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='4dfcf480a32d9ba7098477387d96a657a036ef9ad495a008a83e06b22df63999' ;; 		armhf) natsArch='arm6'; sha256='b82fdb2c8f6e7c731254730043c145423b5c48a3b40e33ad6e32bce029a9f086' ;; 		armv7) natsArch='arm7'; sha256='cffc326c7faeb5ea0769d0f04787d9885d5b2baabd32000d3b18b1130742772e' ;; 		x86_64) natsArch='amd64'; sha256='764ee4a9761185f92904c21c3de204c8b898e9a6bad6afac8b1fe512ce887417' ;; 		x86) natsArch='386'; sha256='a8067d9f26007bed3df2a72eebd4a813035a473058db1451d615ef5e96b30577' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 01 Apr 2021 14:29:22 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 01 Apr 2021 14:29:22 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 01 Apr 2021 14:29:23 GMT
EXPOSE 4222 6222 8222
# Thu, 01 Apr 2021 14:29:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Apr 2021 14:29:23 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:ca3cd42a7c9525f6ce3d64c1a70982613a8235f0cc057ec9244052921853ef15`  
		Last Modified: Wed, 31 Mar 2021 20:10:46 GMT  
		Size: 2.8 MB (2811947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ada4cf180db02bbf5a645d367b3c999bd2d866adfb6969b459025ab3a5f5865d`  
		Last Modified: Thu, 01 Apr 2021 14:29:59 GMT  
		Size: 4.5 MB (4465448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5b817b47391bfd1cb047c312e74ba8c28ef3055a3f2610b6e1cac5fdb07d259`  
		Last Modified: Thu, 01 Apr 2021 14:29:59 GMT  
		Size: 559.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66852cd6a6ebc8a62018430b7b8048a2a6a6c95a33d89e73450ee3821b2eefb2`  
		Last Modified: Thu, 01 Apr 2021 14:29:58 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:176e8d0085b947261153305c1788facc818e70e077179cad7508f5f43bedf77e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6763895 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e9af42585046c70139fb1bb86197b2a6bb68b7a63929d91b30d560ef385d96fc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 31 Mar 2021 17:18:49 GMT
ADD file:988879d74f643b89539e5a0b6d74221621f19f4f87f722614addadc46ce47200 in / 
# Wed, 31 Mar 2021 17:18:50 GMT
CMD ["/bin/sh"]
# Wed, 31 Mar 2021 19:52:22 GMT
ENV NATS_SERVER=2.2.0
# Wed, 31 Mar 2021 19:52:28 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='4dfcf480a32d9ba7098477387d96a657a036ef9ad495a008a83e06b22df63999' ;; 		armhf) natsArch='arm6'; sha256='b82fdb2c8f6e7c731254730043c145423b5c48a3b40e33ad6e32bce029a9f086' ;; 		armv7) natsArch='arm7'; sha256='cffc326c7faeb5ea0769d0f04787d9885d5b2baabd32000d3b18b1130742772e' ;; 		x86_64) natsArch='amd64'; sha256='764ee4a9761185f92904c21c3de204c8b898e9a6bad6afac8b1fe512ce887417' ;; 		x86) natsArch='386'; sha256='a8067d9f26007bed3df2a72eebd4a813035a473058db1451d615ef5e96b30577' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 31 Mar 2021 19:52:29 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Wed, 31 Mar 2021 19:52:30 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 31 Mar 2021 19:52:30 GMT
EXPOSE 4222 6222 8222
# Wed, 31 Mar 2021 19:52:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 31 Mar 2021 19:52:33 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:bb87125c6ee1ce30c6b33d2c96a9fbe46da4a290f7cb1dd73fd62d4e06503699`  
		Last Modified: Wed, 31 Mar 2021 17:19:55 GMT  
		Size: 2.6 MB (2622116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82bb4a6b0c990fafb5aee813c8eb708a86505f095c25955d88163310817dc513`  
		Last Modified: Wed, 31 Mar 2021 19:53:15 GMT  
		Size: 4.1 MB (4140807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fcd67a5460afa2ecd7ff1f09dbffa0a3ee971b3c9211781b47f018dfb18604b`  
		Last Modified: Wed, 31 Mar 2021 19:53:14 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e265ad0375bb3e77396d2def17dfd4b28486975504690db16fe5e3379d72c149`  
		Last Modified: Wed, 31 Mar 2021 19:53:14 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:0d0d69075781a3105d70b4607557c74d2c13430f137da5d4ad9b893ff47bbcc1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6560058 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9fb0c3f1895fa95164aab25913ef37b6488bb4ef685b45fc7ea757d2028570cf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 31 Mar 2021 18:13:27 GMT
ADD file:56e92c06393237a87e0a1ff475e9c9dc80e897d69ec20f45359b587906da345b in / 
# Wed, 31 Mar 2021 18:13:31 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 09:52:30 GMT
ENV NATS_SERVER=2.2.0
# Thu, 01 Apr 2021 09:52:35 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='4dfcf480a32d9ba7098477387d96a657a036ef9ad495a008a83e06b22df63999' ;; 		armhf) natsArch='arm6'; sha256='b82fdb2c8f6e7c731254730043c145423b5c48a3b40e33ad6e32bce029a9f086' ;; 		armv7) natsArch='arm7'; sha256='cffc326c7faeb5ea0769d0f04787d9885d5b2baabd32000d3b18b1130742772e' ;; 		x86_64) natsArch='amd64'; sha256='764ee4a9761185f92904c21c3de204c8b898e9a6bad6afac8b1fe512ce887417' ;; 		x86) natsArch='386'; sha256='a8067d9f26007bed3df2a72eebd4a813035a473058db1451d615ef5e96b30577' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 01 Apr 2021 09:52:36 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 01 Apr 2021 09:52:36 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 01 Apr 2021 09:52:37 GMT
EXPOSE 4222 6222 8222
# Thu, 01 Apr 2021 09:52:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Apr 2021 09:52:39 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:07389e51ea05e1c9a3cb0ef92d31181f2afa1e445207ad99ffd8a94d6d6af295`  
		Last Modified: Wed, 31 Mar 2021 18:14:57 GMT  
		Size: 2.4 MB (2424108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2d72610fdeddca533a7fa8937e70712fae7aca0dcb07d6fbba1e43b20190fe8`  
		Last Modified: Thu, 01 Apr 2021 09:53:21 GMT  
		Size: 4.1 MB (4134981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e12af5140a82cb853be34ad036db9ac6e67f64654816fb140706e62e9c49dec4`  
		Last Modified: Thu, 01 Apr 2021 09:53:20 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56601effdbab268d5f96f091e3ab569209092f832637c2f53712cdd0c4cb06e9`  
		Last Modified: Thu, 01 Apr 2021 09:53:20 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:5e40ddf9a4d4f163f9f413a0a749d385b437a598d53ab8c462d21e6df734c97d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6822164 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fbbc27f239e9627f70c924bbb76c70b230bfabe5e49e3a7d9df731e4f38f39a7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 31 Mar 2021 17:21:21 GMT
ADD file:3b16ffee2b26d8af5db152fcc582aaccd9e1ec9e3343874e9969a205550fe07d in / 
# Wed, 31 Mar 2021 17:21:23 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 13:43:27 GMT
ENV NATS_SERVER=2.2.0
# Thu, 01 Apr 2021 13:43:32 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='4dfcf480a32d9ba7098477387d96a657a036ef9ad495a008a83e06b22df63999' ;; 		armhf) natsArch='arm6'; sha256='b82fdb2c8f6e7c731254730043c145423b5c48a3b40e33ad6e32bce029a9f086' ;; 		armv7) natsArch='arm7'; sha256='cffc326c7faeb5ea0769d0f04787d9885d5b2baabd32000d3b18b1130742772e' ;; 		x86_64) natsArch='amd64'; sha256='764ee4a9761185f92904c21c3de204c8b898e9a6bad6afac8b1fe512ce887417' ;; 		x86) natsArch='386'; sha256='a8067d9f26007bed3df2a72eebd4a813035a473058db1451d615ef5e96b30577' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 01 Apr 2021 13:43:33 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 01 Apr 2021 13:43:34 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 01 Apr 2021 13:43:34 GMT
EXPOSE 4222 6222 8222
# Thu, 01 Apr 2021 13:43:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Apr 2021 13:43:36 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:912815139b61c8926da31f7701f0a924e7964e3713052bf1a53193a4562157f6`  
		Last Modified: Wed, 31 Mar 2021 17:22:41 GMT  
		Size: 2.7 MB (2711920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7065a6411f04b75bef4097e4ddf4951d84ad0bfe9c9d9552a92bf75a42c77bd9`  
		Last Modified: Thu, 01 Apr 2021 13:48:40 GMT  
		Size: 4.1 MB (4109274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6db97b33cea8fa80f73c926008de131699a2fe7671dd699420d9c86a98a4c47a`  
		Last Modified: Thu, 01 Apr 2021 13:48:40 GMT  
		Size: 559.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c025cd8f41b22d6bda55a9235f10bf1751237ebff13e7ad89ed1325fbc9d86e2`  
		Last Modified: Thu, 01 Apr 2021 13:48:39 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
