## `nats:2-alpine`

```console
$ docker pull nats@sha256:755bdf0c9fea43659ef9485ff74a9303ac2595c1b02c807d92b53802baf808a6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-alpine` - linux; amd64

```console
$ docker pull nats@sha256:596442ede179d773ec7f08637e1347328ec3f12ed64568dd29bf8bd92259c84d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.6 MB (8589330 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:36a5b27103c778bd375b40b313ac2dd449b9123b78b3e1933ccf2c24bf0082bb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 09 Jan 2023 17:05:20 GMT
ADD file:e4d600fc4c9c293efe360be7b30ee96579925d1b4634c94332e2ec73f7d8eca1 in / 
# Mon, 09 Jan 2023 17:05:20 GMT
CMD ["/bin/sh"]
# Thu, 02 Feb 2023 21:32:50 GMT
ENV NATS_SERVER=2.9.12
# Thu, 02 Feb 2023 21:32:54 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='296075e7caa33684f0a23ac97c2a904c8f22dbc1d75da4ab443a81aa8b1b765b' ;; 		armhf) natsArch='arm6'; sha256='72af57a620de31e718131736b4ae123acd994295b2f81d1f847cdb9e1e686e63' ;; 		armv7) natsArch='arm7'; sha256='153d823e90b76457b6689cb6baa9f045b3a2152caaec787a0ad77162431949ed' ;; 		x86_64) natsArch='amd64'; sha256='cd05e53b3e1a535dd4e09a4cba3c1b0cd7c512e7f3d68d52ed8e8621dac8c925' ;; 		x86) natsArch='386'; sha256='103d89a231154708375a091dfb86ebe563f3de968a5e6ed14aba4c32e5c77925' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 02 Feb 2023 21:32:54 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 02 Feb 2023 21:32:54 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 02 Feb 2023 21:32:54 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Feb 2023 21:32:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 02 Feb 2023 21:32:54 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:8921db27df2831fa6eaa85321205a2470c669b855f3ec95d5a3c2b46de0442c9`  
		Last Modified: Mon, 09 Jan 2023 17:05:45 GMT  
		Size: 3.4 MB (3370628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90fc2d6058c164e7f06206d5ec77d1dc1a27fbde65facfb00c7be6ebd6c00c9a`  
		Last Modified: Thu, 02 Feb 2023 21:33:28 GMT  
		Size: 5.2 MB (5217701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c8da51ec4a12edfcbb65016c0ab6137e4261542c0806c198a7561573428f286`  
		Last Modified: Thu, 02 Feb 2023 21:33:28 GMT  
		Size: 588.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd8137ab539d1ca45399d4e83b217c0290e34a11f764287427ef7fa51ff209bf`  
		Last Modified: Thu, 02 Feb 2023 21:33:27 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:325775413795f10444c422d2b752494acbd407613fc1537a7cf84693283102a6
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.1 MB (8090427 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c037e626dfdaad2eb7338914f0db6020567bb99c48a7e0f01345484edfa0c7d9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 09 Jan 2023 17:04:54 GMT
ADD file:b15fd8e9f996815394e25f20c8459bfb4c2a8c4074592d6f4c75f4fe79ce537e in / 
# Mon, 09 Jan 2023 17:04:55 GMT
CMD ["/bin/sh"]
# Thu, 02 Feb 2023 21:49:33 GMT
ENV NATS_SERVER=2.9.12
# Thu, 02 Feb 2023 21:50:12 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='296075e7caa33684f0a23ac97c2a904c8f22dbc1d75da4ab443a81aa8b1b765b' ;; 		armhf) natsArch='arm6'; sha256='72af57a620de31e718131736b4ae123acd994295b2f81d1f847cdb9e1e686e63' ;; 		armv7) natsArch='arm7'; sha256='153d823e90b76457b6689cb6baa9f045b3a2152caaec787a0ad77162431949ed' ;; 		x86_64) natsArch='amd64'; sha256='cd05e53b3e1a535dd4e09a4cba3c1b0cd7c512e7f3d68d52ed8e8621dac8c925' ;; 		x86) natsArch='386'; sha256='103d89a231154708375a091dfb86ebe563f3de968a5e6ed14aba4c32e5c77925' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 02 Feb 2023 21:50:12 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 02 Feb 2023 21:50:12 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 02 Feb 2023 21:50:12 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Feb 2023 21:50:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 02 Feb 2023 21:50:13 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:0269c10e600f3a375f36ddabdbd264ce9503a455f0d0969ce8a00f24eaecc032`  
		Last Modified: Mon, 09 Jan 2023 17:05:45 GMT  
		Size: 3.1 MB (3107243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c06b18d184d344d8a89cb092274a39e8c3bf5646c1a8678e53519585c03292b`  
		Last Modified: Thu, 02 Feb 2023 21:51:28 GMT  
		Size: 5.0 MB (4982208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb35f9a15c3a5b93ea2a254cc9c9cc741a6e698dd58741a9f9af4936c2049f03`  
		Last Modified: Thu, 02 Feb 2023 21:51:27 GMT  
		Size: 561.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b92f0e4cdd97e7662fe9c94bd67aabac7172d0e0d97acf0b5c586de7b89f895`  
		Last Modified: Thu, 02 Feb 2023 21:51:27 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:6c2d2b789f9ed0c9edddd86e758373c2c2f76132958d3dec5c2a6d1e7336f9dc
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.8 MB (7841051 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d85fea070aff07d7750af4de5ce3ebb9b49a00738becb1eae53e9281e25aca5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 09 Jan 2023 17:06:27 GMT
ADD file:4696f25d0f019b27457c55b3b128b70bf153f38e3e4eb5bdfc21058543313e94 in / 
# Mon, 09 Jan 2023 17:06:27 GMT
CMD ["/bin/sh"]
# Thu, 02 Feb 2023 21:57:48 GMT
ENV NATS_SERVER=2.9.12
# Thu, 02 Feb 2023 21:57:51 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='296075e7caa33684f0a23ac97c2a904c8f22dbc1d75da4ab443a81aa8b1b765b' ;; 		armhf) natsArch='arm6'; sha256='72af57a620de31e718131736b4ae123acd994295b2f81d1f847cdb9e1e686e63' ;; 		armv7) natsArch='arm7'; sha256='153d823e90b76457b6689cb6baa9f045b3a2152caaec787a0ad77162431949ed' ;; 		x86_64) natsArch='amd64'; sha256='cd05e53b3e1a535dd4e09a4cba3c1b0cd7c512e7f3d68d52ed8e8621dac8c925' ;; 		x86) natsArch='386'; sha256='103d89a231154708375a091dfb86ebe563f3de968a5e6ed14aba4c32e5c77925' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 02 Feb 2023 21:57:51 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 02 Feb 2023 21:57:51 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 02 Feb 2023 21:57:51 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Feb 2023 21:57:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 02 Feb 2023 21:57:52 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:c527615e4ffa2d5b9b777fd469b3b5ba7c1b1e9201c065be2c43569de48a3754`  
		Last Modified: Mon, 09 Jan 2023 17:07:17 GMT  
		Size: 2.9 MB (2865208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54dcdcd84f34ebca9af1574488d3c29f20e5444ee61f4eb8688d3b5b9b1aa829`  
		Last Modified: Thu, 02 Feb 2023 21:59:11 GMT  
		Size: 5.0 MB (4974868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bebca7f9dc77dd081f1e8386b332902935be6eb718e5435056e6928dbdcded07`  
		Last Modified: Thu, 02 Feb 2023 21:59:10 GMT  
		Size: 561.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7247a73a46f57913d3042d8273753dc2524e2b7308a9b7c623043a9f83874df`  
		Last Modified: Thu, 02 Feb 2023 21:59:10 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:3b5d7a8ce580949f91c72ccb764cb0f808ca47f4a306cd2a64adef699b18c709
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.1 MB (8062087 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:72e93fab38c492847947f3360491ff675e9657ddad7fffcd6ddaf34818b3359e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 09 Jan 2023 17:04:48 GMT
ADD file:3080f19f39259a4b77cc53975de0184c78d4335ceb9ffb77a2838d0539ad6f85 in / 
# Mon, 09 Jan 2023 17:04:49 GMT
CMD ["/bin/sh"]
# Thu, 02 Feb 2023 21:47:31 GMT
ENV NATS_SERVER=2.9.12
# Thu, 02 Feb 2023 21:47:34 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='296075e7caa33684f0a23ac97c2a904c8f22dbc1d75da4ab443a81aa8b1b765b' ;; 		armhf) natsArch='arm6'; sha256='72af57a620de31e718131736b4ae123acd994295b2f81d1f847cdb9e1e686e63' ;; 		armv7) natsArch='arm7'; sha256='153d823e90b76457b6689cb6baa9f045b3a2152caaec787a0ad77162431949ed' ;; 		x86_64) natsArch='amd64'; sha256='cd05e53b3e1a535dd4e09a4cba3c1b0cd7c512e7f3d68d52ed8e8621dac8c925' ;; 		x86) natsArch='386'; sha256='103d89a231154708375a091dfb86ebe563f3de968a5e6ed14aba4c32e5c77925' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 02 Feb 2023 21:47:34 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 02 Feb 2023 21:47:34 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 02 Feb 2023 21:47:34 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Feb 2023 21:47:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 02 Feb 2023 21:47:34 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:a9eaa45ef418e883481a13c7d84fa9904f2ec56789c52a87ba5a9e6483f2b74f`  
		Last Modified: Mon, 09 Jan 2023 17:05:12 GMT  
		Size: 3.3 MB (3259241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf7882578303a0fa74c95f3a4d8ba43cb527ab5ae15db2e91420624139809c58`  
		Last Modified: Thu, 02 Feb 2023 21:48:06 GMT  
		Size: 4.8 MB (4801846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02c5fcf7cb836026cb1caf41222a5db286caad4181a1465fbc6a827e539d655f`  
		Last Modified: Thu, 02 Feb 2023 21:48:06 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c842168768b2663567de8311303dd5b2951b867f7c2228af37a24b50f24181ae`  
		Last Modified: Thu, 02 Feb 2023 21:48:05 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
