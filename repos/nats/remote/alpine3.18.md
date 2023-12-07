## `nats:alpine3.18`

```console
$ docker pull nats@sha256:497f324289e82824b3f7eefec5b9a6f639a32739bffe8bfd3394bf217098919f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:alpine3.18` - linux; amd64

```console
$ docker pull nats@sha256:e69ea3ea129b75663ef1fbf6f6b66c6065924b8648ceaff49fc1a6d243c07e62
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.5 MB (9513446 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b0ce66e0a46e1088055a51a8dae2234f13808213f4a7fae6f9c2475d3989849`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 30 Nov 2023 23:22:52 GMT
ADD file:fc714080c3bcbbce7ac746a10d7b4355ffa36293a8d435d62cd5359ea8eb8364 in / 
# Thu, 30 Nov 2023 23:22:52 GMT
CMD ["/bin/sh"]
# Thu, 07 Dec 2023 01:19:48 GMT
ENV NATS_SERVER=2.10.7
# Thu, 07 Dec 2023 01:19:50 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='9a88afab7b3805475ff7250649447d8807dd52262011252e7faedec926d01782' ;; 		armhf) natsArch='arm6'; sha256='37f8d913cdc69143edf8bd20bceced053b90dba26d1fa94e2e07b6fe17f9db2e' ;; 		armv7) natsArch='arm7'; sha256='d96042f12ecc0578d193d5353c362a572384c6ad9a46db73b7cb5f28cb6e4ad2' ;; 		x86_64) natsArch='amd64'; sha256='91f5b493ce3151baa0b15d8bf093279dc94106dd56a201704a20de567607bcf7' ;; 		x86) natsArch='386'; sha256='a5cddcac9f8debaf45e7b9ba3960778b1c786020c690991094ce31d033ec7649' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 07 Dec 2023 01:19:50 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 07 Dec 2023 01:19:50 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 07 Dec 2023 01:19:50 GMT
EXPOSE 4222 6222 8222
# Thu, 07 Dec 2023 01:19:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 07 Dec 2023 01:19:51 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:c926b61bad3b94ae7351bafd0c184c159ebf0643b085f7ef1d47ecdc7316833c`  
		Last Modified: Thu, 30 Nov 2023 23:23:28 GMT  
		Size: 3.4 MB (3402422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afd45941c5ec4c89954590450598e97bff29acdd357abb9550c2a4225bf2919b`  
		Last Modified: Thu, 07 Dec 2023 01:20:28 GMT  
		Size: 6.1 MB (6110026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f05a83670934c18d8eac79cf05ec48cb635976d0c5b05a80d36624b3ed45de0f`  
		Last Modified: Thu, 07 Dec 2023 01:20:26 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc87433b72bc5915d420aeb8d253e934c34c2cf9c799c6b7e284c51828d3d5bc`  
		Last Modified: Thu, 07 Dec 2023 01:20:26 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.18` - linux; arm variant v6

```console
$ docker pull nats@sha256:5646f5ce83a2cd0809dd62b9103aba3eff6bca2666965032ae01c1425f4c01c0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.0 MB (8975747 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c17c0157045551d25e73637159044fae84067bde183e05d0099b9b806299b456`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 30 Nov 2023 22:49:18 GMT
ADD file:dbf65487d049081dc2d39b3d99d2c64b6c89754e7e2996a46169d3512e59f32a in / 
# Thu, 30 Nov 2023 22:49:18 GMT
CMD ["/bin/sh"]
# Thu, 07 Dec 2023 00:49:19 GMT
ENV NATS_SERVER=2.10.7
# Thu, 07 Dec 2023 00:49:22 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='9a88afab7b3805475ff7250649447d8807dd52262011252e7faedec926d01782' ;; 		armhf) natsArch='arm6'; sha256='37f8d913cdc69143edf8bd20bceced053b90dba26d1fa94e2e07b6fe17f9db2e' ;; 		armv7) natsArch='arm7'; sha256='d96042f12ecc0578d193d5353c362a572384c6ad9a46db73b7cb5f28cb6e4ad2' ;; 		x86_64) natsArch='amd64'; sha256='91f5b493ce3151baa0b15d8bf093279dc94106dd56a201704a20de567607bcf7' ;; 		x86) natsArch='386'; sha256='a5cddcac9f8debaf45e7b9ba3960778b1c786020c690991094ce31d033ec7649' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 07 Dec 2023 00:49:22 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 07 Dec 2023 00:49:22 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 07 Dec 2023 00:49:22 GMT
EXPOSE 4222 6222 8222
# Thu, 07 Dec 2023 00:49:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 07 Dec 2023 00:49:23 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:85ae953f9e6740471d4e1440b27721679dc7a511e112eb73df467a4cde26e421`  
		Last Modified: Thu, 30 Nov 2023 22:49:40 GMT  
		Size: 3.1 MB (3146870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:733b743b5e93d5fde059f514131d51e22a1a4eef1fe4e71d4e42c7fdfc960da9`  
		Last Modified: Thu, 07 Dec 2023 00:49:56 GMT  
		Size: 5.8 MB (5827875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b3b83a38bf1009764f2673fbcfe66e38ba7d57492c7838790e767319e64c961`  
		Last Modified: Thu, 07 Dec 2023 00:49:54 GMT  
		Size: 589.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1b6d8395d698e101d9e4936dee08916549133753cd0672eceac8ddf1190193a`  
		Last Modified: Thu, 07 Dec 2023 00:49:54 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.18` - linux; arm variant v7

```console
$ docker pull nats@sha256:319339bfeb0f92227088c3f5cfd3e56981fa3b186d5116cfdf4226d2460a35fb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.7 MB (8720478 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d237f0362b1780eafc23b2167a400bc9263e907cee8681711608e8a81f74cd4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 30 Nov 2023 22:49:28 GMT
ADD file:dcb85d43d1fb96861612c42288878b13debfa9d0b956adea1f2472d0c50f0144 in / 
# Thu, 30 Nov 2023 22:49:29 GMT
CMD ["/bin/sh"]
# Thu, 07 Dec 2023 00:57:29 GMT
ENV NATS_SERVER=2.10.7
# Thu, 07 Dec 2023 00:57:32 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='9a88afab7b3805475ff7250649447d8807dd52262011252e7faedec926d01782' ;; 		armhf) natsArch='arm6'; sha256='37f8d913cdc69143edf8bd20bceced053b90dba26d1fa94e2e07b6fe17f9db2e' ;; 		armv7) natsArch='arm7'; sha256='d96042f12ecc0578d193d5353c362a572384c6ad9a46db73b7cb5f28cb6e4ad2' ;; 		x86_64) natsArch='amd64'; sha256='91f5b493ce3151baa0b15d8bf093279dc94106dd56a201704a20de567607bcf7' ;; 		x86) natsArch='386'; sha256='a5cddcac9f8debaf45e7b9ba3960778b1c786020c690991094ce31d033ec7649' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 07 Dec 2023 00:57:32 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 07 Dec 2023 00:57:32 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 07 Dec 2023 00:57:32 GMT
EXPOSE 4222 6222 8222
# Thu, 07 Dec 2023 00:57:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 07 Dec 2023 00:57:33 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:2387a44129d2147bd4e806bf369f3db92eb3ad3b6b8825c739db364b8baa4e26`  
		Last Modified: Thu, 30 Nov 2023 22:49:56 GMT  
		Size: 2.9 MB (2901006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:199d98699d8052dfaae7fe949909d4441e7ffa65f121292863ba744dcb835df5`  
		Last Modified: Thu, 07 Dec 2023 00:58:14 GMT  
		Size: 5.8 MB (5818474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5754b91893810a1324476d59ae9f561401be2dd7ae77503a7d84e5e7a5056f8d`  
		Last Modified: Thu, 07 Dec 2023 00:58:13 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4969653e0f6db6b3f49cb0add7efde0f957fd2bc0fdd0f1511497bdc1a319e5d`  
		Last Modified: Thu, 07 Dec 2023 00:58:13 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.18` - linux; arm64 variant v8

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
