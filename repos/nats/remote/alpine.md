## `nats:alpine`

```console
$ docker pull nats@sha256:cc2bde1fe965db9ac2011073b071010691ebdb1904c7933922ad2a107a5a7a34
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:alpine` - linux; amd64

```console
$ docker pull nats@sha256:9d2f79cec13b773e5677cec0f3272e52e55be44210e9f5b4917c623166394f34
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7345153 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:491da5634208d92e0c0a052128e76069f3d086b42582b2a07515f1b2284e1b62`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Tue, 25 May 2021 01:38:13 GMT
ENV NATS_SERVER=2.2.6
# Tue, 25 May 2021 01:38:16 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='779d7f363fb0244071e67bf146c7169a8e3c35af2746c0a01323a3c5fd12bf31' ;; 		armhf) natsArch='arm6'; sha256='ed7211f56fa3928e3664ed92df632b0e7480bd1b4a91c239cb26a0f55831c815' ;; 		armv7) natsArch='arm7'; sha256='a55335b1329248912e80d8e68b5dd6b6a48c4742de089c4226f503d7e8357f2c' ;; 		x86_64) natsArch='amd64'; sha256='fc67ce0b4c748fa16ff92414c7d6be18a9285824c21d9629684c0093cf074f77' ;; 		x86) natsArch='386'; sha256='386811034531cea6e794e4764fdd70b0b948fdf7212064e8c176663992c46f2e' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Tue, 25 May 2021 01:38:16 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Tue, 25 May 2021 01:38:16 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 25 May 2021 01:38:16 GMT
EXPOSE 4222 6222 8222
# Tue, 25 May 2021 01:38:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 25 May 2021 01:38:17 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9cf50b10150a20d88392a1085f9599e8af8f5a3018685f039e7c0e5dd7288d4`  
		Last Modified: Tue, 25 May 2021 01:39:00 GMT  
		Size: 4.5 MB (4532213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09ee7d5e3ce0eae646fccf205b9550e978ab7664d6926dbb673199ef0f8835fd`  
		Last Modified: Tue, 25 May 2021 01:38:59 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54a7f22a12d626460f4a81bc8142154fd148479c9c6d9c9513863790fc54ec43`  
		Last Modified: Tue, 25 May 2021 01:38:59 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:b9aeba4df029d36ef4a1dee985b4378d5d85c43e66b8bb16ca6bf9a9fe324247
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6821208 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d25e733bd4a006fa768f685d0a46df5974265e6076c77e6fbc77ec11d80256b1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Apr 2021 18:49:39 GMT
ADD file:4479f0a51530e039edf231d87201896dcff908aa542a613cdccb015f93dda8a3 in / 
# Wed, 14 Apr 2021 18:49:40 GMT
CMD ["/bin/sh"]
# Wed, 26 May 2021 18:22:42 GMT
ENV NATS_SERVER=2.2.6
# Wed, 26 May 2021 18:22:45 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='779d7f363fb0244071e67bf146c7169a8e3c35af2746c0a01323a3c5fd12bf31' ;; 		armhf) natsArch='arm6'; sha256='ed7211f56fa3928e3664ed92df632b0e7480bd1b4a91c239cb26a0f55831c815' ;; 		armv7) natsArch='arm7'; sha256='a55335b1329248912e80d8e68b5dd6b6a48c4742de089c4226f503d7e8357f2c' ;; 		x86_64) natsArch='amd64'; sha256='fc67ce0b4c748fa16ff92414c7d6be18a9285824c21d9629684c0093cf074f77' ;; 		x86) natsArch='386'; sha256='386811034531cea6e794e4764fdd70b0b948fdf7212064e8c176663992c46f2e' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 26 May 2021 18:22:45 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Wed, 26 May 2021 18:22:46 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 26 May 2021 18:22:46 GMT
EXPOSE 4222 6222 8222
# Wed, 26 May 2021 18:22:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 May 2021 18:22:46 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:740c950346cf39c85b52576998695c9b909c24a58a8bb1b64cce91fda3ef1d3a`  
		Last Modified: Wed, 14 Apr 2021 18:50:30 GMT  
		Size: 2.6 MB (2622131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d3a57d0cfca764ba6dced768ca03ad14dc28ff512a35ee518f7b976236776e1`  
		Last Modified: Wed, 26 May 2021 18:24:16 GMT  
		Size: 4.2 MB (4198107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca2401e323dd0f68908e5aacc989cadeff54eeaf0d59eb407c281796d59e8a64`  
		Last Modified: Wed, 26 May 2021 18:24:16 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddba5a5f87ca0d8782a46b9c4e4aeb6fc684c4b3e78792a8b7c8ee233d9e0bc2`  
		Last Modified: Wed, 26 May 2021 18:24:16 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:91d2dbf930b400b44b948361b60920659e74b28370d38b384bda56985d7d172c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6617719 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:02dc5ea95004c286602940e81b2950f498ef35217e01e1da4e372194c8a65d45`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Apr 2021 18:57:39 GMT
ADD file:028c5b473d862250586e174c5dd19b37f8fc3bffbc02d888e72df30f32fd6129 in / 
# Wed, 14 Apr 2021 18:57:39 GMT
CMD ["/bin/sh"]
# Tue, 25 May 2021 22:22:45 GMT
ENV NATS_SERVER=2.2.6
# Tue, 25 May 2021 22:22:48 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='779d7f363fb0244071e67bf146c7169a8e3c35af2746c0a01323a3c5fd12bf31' ;; 		armhf) natsArch='arm6'; sha256='ed7211f56fa3928e3664ed92df632b0e7480bd1b4a91c239cb26a0f55831c815' ;; 		armv7) natsArch='arm7'; sha256='a55335b1329248912e80d8e68b5dd6b6a48c4742de089c4226f503d7e8357f2c' ;; 		x86_64) natsArch='amd64'; sha256='fc67ce0b4c748fa16ff92414c7d6be18a9285824c21d9629684c0093cf074f77' ;; 		x86) natsArch='386'; sha256='386811034531cea6e794e4764fdd70b0b948fdf7212064e8c176663992c46f2e' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Tue, 25 May 2021 22:22:48 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Tue, 25 May 2021 22:22:49 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 25 May 2021 22:22:49 GMT
EXPOSE 4222 6222 8222
# Tue, 25 May 2021 22:22:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 25 May 2021 22:22:49 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:e160e00eb35d5bc2373770873fbc9c8f5706045b0b06bfd1c364fcf69f02e9fe`  
		Last Modified: Wed, 14 Apr 2021 18:58:36 GMT  
		Size: 2.4 MB (2424145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee8fd93bac31720120ec97ee8f514ace788f281711084b9532b4d152e8fa3514`  
		Last Modified: Tue, 25 May 2021 22:24:21 GMT  
		Size: 4.2 MB (4192604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f240e54fb35db3d43766365af298a4fcd1eaab7acbfda0fd141a242fc1feaeb5`  
		Last Modified: Tue, 25 May 2021 22:24:21 GMT  
		Size: 557.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfddeffbc3b0f30d139487df21b514ec7bc915cbca61e31ee793eed0d9472e16`  
		Last Modified: Tue, 25 May 2021 22:24:20 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:5246e11d8205a6ffbbec46aa7b095539b03c36404be14eb0b0860a3049c4251a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.9 MB (6884738 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:76e8898b79510f35f89fb68e130151b491a24a9a1bd2d3913e82a3893a7b5d65`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 15 Jun 2021 21:45:03 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Tue, 15 Jun 2021 21:45:04 GMT
CMD ["/bin/sh"]
# Wed, 16 Jun 2021 01:08:34 GMT
ENV NATS_SERVER=2.2.6
# Wed, 16 Jun 2021 01:08:37 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='779d7f363fb0244071e67bf146c7169a8e3c35af2746c0a01323a3c5fd12bf31' ;; 		armhf) natsArch='arm6'; sha256='ed7211f56fa3928e3664ed92df632b0e7480bd1b4a91c239cb26a0f55831c815' ;; 		armv7) natsArch='arm7'; sha256='a55335b1329248912e80d8e68b5dd6b6a48c4742de089c4226f503d7e8357f2c' ;; 		x86_64) natsArch='amd64'; sha256='fc67ce0b4c748fa16ff92414c7d6be18a9285824c21d9629684c0093cf074f77' ;; 		x86) natsArch='386'; sha256='386811034531cea6e794e4764fdd70b0b948fdf7212064e8c176663992c46f2e' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 16 Jun 2021 01:08:37 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Wed, 16 Jun 2021 01:08:37 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 16 Jun 2021 01:08:37 GMT
EXPOSE 4222 6222 8222
# Wed, 16 Jun 2021 01:08:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Jun 2021 01:08:38 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f040d63fb2ddd057295cc71251ca3d1cb1c42ffe30dba29380ea25ccfbd29a7`  
		Last Modified: Wed, 16 Jun 2021 01:09:38 GMT  
		Size: 4.2 MB (4171741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d1ad8eacdaba56c63bd09d368c8a9368c754fbdd1bc80bb5258a43f0534f941`  
		Last Modified: Wed, 16 Jun 2021 01:09:37 GMT  
		Size: 557.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76b762266ffc9192790141facce5309e7d94fa3c1c9a35d8d32c0ba21662b9d1`  
		Last Modified: Wed, 16 Jun 2021 01:09:38 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
