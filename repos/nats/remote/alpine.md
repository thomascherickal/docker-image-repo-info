## `nats:alpine`

```console
$ docker pull nats@sha256:51e3a0879d09c1a00f1deea0c824367e5b30339f1cf92066e7f28cb466119b43
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:alpine` - linux; amd64

```console
$ docker pull nats@sha256:23dc685e3c08196e1b7e062a062a0e297da560197192316ba846db109c8c9085
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.5 MB (9509686 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9beb0f33b937617e04a3bece66962a00cd4f8a2e4da8fd6723e2af3135ec6531`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 30 Nov 2023 23:22:52 GMT
ADD file:fc714080c3bcbbce7ac746a10d7b4355ffa36293a8d435d62cd5359ea8eb8364 in / 
# Thu, 30 Nov 2023 23:22:52 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 07:09:33 GMT
ENV NATS_SERVER=2.10.5
# Fri, 01 Dec 2023 07:09:35 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='de560b8863ddceac5d765b1f99d4b8f0becf8488890253beafffb7cb730f1aa8' ;; 		armhf) natsArch='arm6'; sha256='b0ca5676f1b65a60dd7feb0b1be5b7ae35977a978ba21451d0165492c984a93f' ;; 		armv7) natsArch='arm7'; sha256='0b0695e6f4e90012021e5ef59b71d6a4e0a19df0c5852c83494d7e9776dc5085' ;; 		x86_64) natsArch='amd64'; sha256='33e9796344fcde53d1d9ab5fc3e2393d1f558aec53f5ea51f769827602a20225' ;; 		x86) natsArch='386'; sha256='f8d4facfc3735ea46ccaecc1e7815f2b755dd0697b0b7f7d83cff568e2ebd77c' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 01 Dec 2023 07:09:35 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 01 Dec 2023 07:09:35 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 01 Dec 2023 07:09:35 GMT
EXPOSE 4222 6222 8222
# Fri, 01 Dec 2023 07:09:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 01 Dec 2023 07:09:35 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:c926b61bad3b94ae7351bafd0c184c159ebf0643b085f7ef1d47ecdc7316833c`  
		Last Modified: Thu, 30 Nov 2023 23:23:28 GMT  
		Size: 3.4 MB (3402422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a214d6eab35932b2be0106225c564b689dab8bf0c4f2d2657c63e48b2247b6fc`  
		Last Modified: Fri, 01 Dec 2023 07:10:15 GMT  
		Size: 6.1 MB (6106263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f423ec088dc856b962a5dd89c31ab09416457de0a5994922f51bef46d1945f5`  
		Last Modified: Fri, 01 Dec 2023 07:10:14 GMT  
		Size: 588.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e93563c51811f1dc92fe243bd5b8721f10cf5060cfd617ed40a18ed8a840ab3a`  
		Last Modified: Fri, 01 Dec 2023 07:10:14 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:f9a012265e9ab4e95584f7ea9f4f78234e048366873dcef81b1b46359e22d9f5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.0 MB (8975414 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ce4db94168c70869897e9c0941e0567f3ce732d60f92f80ef605d765d9c9686`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 30 Nov 2023 22:49:18 GMT
ADD file:dbf65487d049081dc2d39b3d99d2c64b6c89754e7e2996a46169d3512e59f32a in / 
# Thu, 30 Nov 2023 22:49:18 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 21:49:22 GMT
ENV NATS_SERVER=2.10.6
# Fri, 01 Dec 2023 21:49:25 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='89eade997286bf889cbbd40bd52e4952d318eb85d66387162d3539124c8ec5d5' ;; 		armhf) natsArch='arm6'; sha256='2ebbdca481127ada62c5fc814ca4fea06ce18f0bdfc658769b589e1936b93566' ;; 		armv7) natsArch='arm7'; sha256='c5c0532ff6c5c32674932fa97dee462020ce5e30401d7a089ce3a5c52c259d9d' ;; 		x86_64) natsArch='amd64'; sha256='07a687d38ce737961adae346df8023ec5dc3a74e541931b911ec5e21491f6c2e' ;; 		x86) natsArch='386'; sha256='921180ca022af2316db3dc0e00689a104771a5438ecf0f6db27e92f78a17509d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 01 Dec 2023 21:49:25 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 01 Dec 2023 21:49:25 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 01 Dec 2023 21:49:25 GMT
EXPOSE 4222 6222 8222
# Fri, 01 Dec 2023 21:49:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 01 Dec 2023 21:49:25 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:85ae953f9e6740471d4e1440b27721679dc7a511e112eb73df467a4cde26e421`  
		Last Modified: Thu, 30 Nov 2023 22:49:40 GMT  
		Size: 3.1 MB (3146870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9345d2089731ee6f2e92bf32245d1665e8357fecf55c50e9a428966a109c4ed`  
		Last Modified: Fri, 01 Dec 2023 21:50:01 GMT  
		Size: 5.8 MB (5827544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:569cb676c86b2aeb776ffd80a904ac5e9bdcda8bea7c0684872fba5efc4b8007`  
		Last Modified: Fri, 01 Dec 2023 21:50:00 GMT  
		Size: 588.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23edb8dc9637ca24330de881d8e57e7f369ebd6b7b100db2dbae3aff15d50f29`  
		Last Modified: Fri, 01 Dec 2023 21:50:00 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:d6be8cbc263e2393e2d5f07d4b579c143dada13fe2dd8966097c11e9a1ddc178
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.7 MB (8720293 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c00554cdbce58cc9a6a11ca1b37f5b90932f2c7bc9b55f096f26b93ba240a4a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 30 Nov 2023 22:49:28 GMT
ADD file:dcb85d43d1fb96861612c42288878b13debfa9d0b956adea1f2472d0c50f0144 in / 
# Thu, 30 Nov 2023 22:49:29 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 21:57:27 GMT
ENV NATS_SERVER=2.10.6
# Fri, 01 Dec 2023 21:57:30 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='89eade997286bf889cbbd40bd52e4952d318eb85d66387162d3539124c8ec5d5' ;; 		armhf) natsArch='arm6'; sha256='2ebbdca481127ada62c5fc814ca4fea06ce18f0bdfc658769b589e1936b93566' ;; 		armv7) natsArch='arm7'; sha256='c5c0532ff6c5c32674932fa97dee462020ce5e30401d7a089ce3a5c52c259d9d' ;; 		x86_64) natsArch='amd64'; sha256='07a687d38ce737961adae346df8023ec5dc3a74e541931b911ec5e21491f6c2e' ;; 		x86) natsArch='386'; sha256='921180ca022af2316db3dc0e00689a104771a5438ecf0f6db27e92f78a17509d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 01 Dec 2023 21:57:30 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 01 Dec 2023 21:57:30 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 01 Dec 2023 21:57:30 GMT
EXPOSE 4222 6222 8222
# Fri, 01 Dec 2023 21:57:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 01 Dec 2023 21:57:30 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:2387a44129d2147bd4e806bf369f3db92eb3ad3b6b8825c739db364b8baa4e26`  
		Last Modified: Thu, 30 Nov 2023 22:49:56 GMT  
		Size: 2.9 MB (2901006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6f8756919eccb97dc6990af357a87c8ba743e3a3ee7ad6d8c8c3dc108620e3c`  
		Last Modified: Fri, 01 Dec 2023 21:58:16 GMT  
		Size: 5.8 MB (5818288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55307c3335ece26e2e60bb611f614f94af63814be706d6b3394d9691f55e7f82`  
		Last Modified: Fri, 01 Dec 2023 21:58:15 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f7195a7938dcaa9bf7c4b89602950f827640c5bbecbb4a4f858b6a846f6719b`  
		Last Modified: Fri, 01 Dec 2023 21:58:16 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:ecd307e2f9675cf866313820a53a82b1a1459cf04a50da39b145b79360877119
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.0 MB (9018304 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f0e350d93fb277376b154a1cc0e44e75d36e34a479bea66c1186b2ef6ce5ec9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 30 Nov 2023 23:11:03 GMT
ADD file:d8a30995bbcd627f084912c728fda5483b6ba486de25af588a0956069d0bd7ad in / 
# Thu, 30 Nov 2023 23:11:03 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 21:39:48 GMT
ENV NATS_SERVER=2.10.6
# Fri, 01 Dec 2023 21:39:50 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='89eade997286bf889cbbd40bd52e4952d318eb85d66387162d3539124c8ec5d5' ;; 		armhf) natsArch='arm6'; sha256='2ebbdca481127ada62c5fc814ca4fea06ce18f0bdfc658769b589e1936b93566' ;; 		armv7) natsArch='arm7'; sha256='c5c0532ff6c5c32674932fa97dee462020ce5e30401d7a089ce3a5c52c259d9d' ;; 		x86_64) natsArch='amd64'; sha256='07a687d38ce737961adae346df8023ec5dc3a74e541931b911ec5e21491f6c2e' ;; 		x86) natsArch='386'; sha256='921180ca022af2316db3dc0e00689a104771a5438ecf0f6db27e92f78a17509d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 01 Dec 2023 21:39:50 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 01 Dec 2023 21:39:50 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 01 Dec 2023 21:39:50 GMT
EXPOSE 4222 6222 8222
# Fri, 01 Dec 2023 21:39:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 01 Dec 2023 21:39:50 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:2c03dbb20264f09924f9eab176da44e5421e74a78b09531d3c63448a7baa7c59`  
		Last Modified: Thu, 30 Nov 2023 23:11:32 GMT  
		Size: 3.3 MB (3333033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:099335ae91609137f74432a77e75ffc1877279b74582260fc094104662cc3707`  
		Last Modified: Fri, 01 Dec 2023 21:40:50 GMT  
		Size: 5.7 MB (5684273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a10e033372c9ea54711e4453250cd168911b0b43394e197c03164fcab8331f7`  
		Last Modified: Fri, 01 Dec 2023 21:40:49 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a9486420e5d0bd9ffaf1e3828a6eec84d98d97415b6fe70f65534ff451b2c61`  
		Last Modified: Fri, 01 Dec 2023 21:40:49 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
