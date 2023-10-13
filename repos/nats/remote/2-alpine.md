## `nats:2-alpine`

```console
$ docker pull nats@sha256:da1eb7478d24a313509338be67dd17478870881a21eb30d0246d6a82e91266d4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-alpine` - linux; amd64

```console
$ docker pull nats@sha256:2cceb1f3fa7b15611e166ed479dd90d3e43b8d46cb776d08f64e05deb200be68
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.5 MB (9498416 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a57a41cbb09fe1a60b56fd7522328ad6c507b968b2837855dba4d6661e84806`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 28 Sep 2023 21:19:27 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Thu, 28 Sep 2023 21:19:27 GMT
CMD ["/bin/sh"]
# Fri, 13 Oct 2023 20:20:05 GMT
ENV NATS_SERVER=2.10.3
# Fri, 13 Oct 2023 20:20:08 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='924a92491f549be8e8d51d56fc0cd211e8326933b9e7c2bbd31af0fdc7f15240' ;; 		armhf) natsArch='arm6'; sha256='dc8cfc756af14cda3c754ebfbe942616f7e3e65b8d846e7a34f5de2c55612a9d' ;; 		armv7) natsArch='arm7'; sha256='f8e4cf88d50800650b0fed026e776d8ca7eace6b0cbc4762beca7d0f3590ba00' ;; 		x86_64) natsArch='amd64'; sha256='a5587b04062a9cf117ec13aea5cb60cf4cd2e644be8c44628d85b5f4dfc19ab6' ;; 		x86) natsArch='386'; sha256='e8a1a521aeeef68abf2b1bd3baf3f359a073c25cef4f87aa505a49c1b0920e90' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 13 Oct 2023 20:20:08 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 13 Oct 2023 20:20:08 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 13 Oct 2023 20:20:08 GMT
EXPOSE 4222 6222 8222
# Fri, 13 Oct 2023 20:20:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 13 Oct 2023 20:20:08 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2ad1a616f2a37d0761343518ccdc80755abd01cb3c30a49c3a328adc0d7024c`  
		Last Modified: Fri, 13 Oct 2023 20:21:25 GMT  
		Size: 6.1 MB (6095446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b3ded5aac5d1e1475aec9d0629cd78f96b816735bada84e67b6ee7abeafcaa7`  
		Last Modified: Fri, 13 Oct 2023 20:21:23 GMT  
		Size: 589.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f5407fa2efd19d981d3f8ffcc0cde53637fa5fcd5cccbba08976c8db248aee5`  
		Last Modified: Fri, 13 Oct 2023 20:21:23 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:c396810cff0b8e5d376956733815f1821a74b6c5a32758a3b7f4814afa54f660
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.0 MB (8959561 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:457fab83639c9d351944ed83d25e70d9fdecda349419acd221d702f136e514a8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 28 Sep 2023 20:49:16 GMT
ADD file:2222b03381ff0fce22edd647f5c60529ec6a72202f8d3cb1d6e4648ebcd19a1e in / 
# Thu, 28 Sep 2023 20:49:16 GMT
CMD ["/bin/sh"]
# Fri, 13 Oct 2023 20:49:23 GMT
ENV NATS_SERVER=2.10.3
# Fri, 13 Oct 2023 20:49:26 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='924a92491f549be8e8d51d56fc0cd211e8326933b9e7c2bbd31af0fdc7f15240' ;; 		armhf) natsArch='arm6'; sha256='dc8cfc756af14cda3c754ebfbe942616f7e3e65b8d846e7a34f5de2c55612a9d' ;; 		armv7) natsArch='arm7'; sha256='f8e4cf88d50800650b0fed026e776d8ca7eace6b0cbc4762beca7d0f3590ba00' ;; 		x86_64) natsArch='amd64'; sha256='a5587b04062a9cf117ec13aea5cb60cf4cd2e644be8c44628d85b5f4dfc19ab6' ;; 		x86) natsArch='386'; sha256='e8a1a521aeeef68abf2b1bd3baf3f359a073c25cef4f87aa505a49c1b0920e90' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 13 Oct 2023 20:49:26 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 13 Oct 2023 20:49:26 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 13 Oct 2023 20:49:26 GMT
EXPOSE 4222 6222 8222
# Fri, 13 Oct 2023 20:49:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 13 Oct 2023 20:49:26 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:91cb83b91ee16f1ee0d588fccef56ab5dbb5689a64e5373caf33d7e4fe52ceb4`  
		Last Modified: Thu, 28 Sep 2023 20:51:25 GMT  
		Size: 3.1 MB (3145291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61241071cebda9cba981b7b82f393e119b961bd9159bf55dcdba1c4624e45917`  
		Last Modified: Fri, 13 Oct 2023 20:50:04 GMT  
		Size: 5.8 MB (5813268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a337d1a669a446adc02d1d8002392edf0fe2d8138ef94a0e50ee7530ec685fe4`  
		Last Modified: Fri, 13 Oct 2023 20:50:02 GMT  
		Size: 585.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77b037061c6ffd9f106c296b4de2e1020665e9f20af8504311b688fbf579ec44`  
		Last Modified: Fri, 13 Oct 2023 20:50:02 GMT  
		Size: 417.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:17c05176e65bf9d0e1491927694e3044a595cb8b8e4bb2dea59ebcca6604a15f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.7 MB (8704649 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d36339c31362689fb85865c6dd5463c41fbc8316ead741ca7cf2bd7aa7d31e7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 28 Sep 2023 20:59:24 GMT
ADD file:61f54a318ad79861c6177783bb4c604412b5d952f45a9aa12ff97f4dccba7f73 in / 
# Thu, 28 Sep 2023 20:59:24 GMT
CMD ["/bin/sh"]
# Fri, 13 Oct 2023 20:57:28 GMT
ENV NATS_SERVER=2.10.3
# Fri, 13 Oct 2023 20:57:31 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='924a92491f549be8e8d51d56fc0cd211e8326933b9e7c2bbd31af0fdc7f15240' ;; 		armhf) natsArch='arm6'; sha256='dc8cfc756af14cda3c754ebfbe942616f7e3e65b8d846e7a34f5de2c55612a9d' ;; 		armv7) natsArch='arm7'; sha256='f8e4cf88d50800650b0fed026e776d8ca7eace6b0cbc4762beca7d0f3590ba00' ;; 		x86_64) natsArch='amd64'; sha256='a5587b04062a9cf117ec13aea5cb60cf4cd2e644be8c44628d85b5f4dfc19ab6' ;; 		x86) natsArch='386'; sha256='e8a1a521aeeef68abf2b1bd3baf3f359a073c25cef4f87aa505a49c1b0920e90' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 13 Oct 2023 20:57:31 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 13 Oct 2023 20:57:31 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 13 Oct 2023 20:57:31 GMT
EXPOSE 4222 6222 8222
# Fri, 13 Oct 2023 20:57:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 13 Oct 2023 20:57:31 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:622a0779436eb93ceea635e910268f867c2eba47d4f62f0bd45f0bd165af3572`  
		Last Modified: Thu, 28 Sep 2023 21:00:50 GMT  
		Size: 2.9 MB (2899905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88d4d62a2fc0e535870d4eb68884f7c44422fac7850ed219352cb3b6f323195a`  
		Last Modified: Fri, 13 Oct 2023 20:58:30 GMT  
		Size: 5.8 MB (5803745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba1309051fb0c589da4d478edb5890d87ec73851f7d22b94f676eb80a98eece7`  
		Last Modified: Fri, 13 Oct 2023 20:58:28 GMT  
		Size: 585.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e4f9000751a913e3d4861bb2e51a86d81df3a1822e8439e3c67216216ca29cb`  
		Last Modified: Fri, 13 Oct 2023 20:58:28 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:10622e60a928a676f6bd678c05fd8146ec12e0ce1a02063af044dcbb6983b55e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.0 MB (9002000 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea617ccf0da02c9e88f244b2dccd65610b1b4fd6b7344bb61b01de68426f539d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 28 Sep 2023 20:39:33 GMT
ADD file:ff3112828967e8004a3264d7ece3f81c88e6a1d44d360b9b5613caab15b41717 in / 
# Thu, 28 Sep 2023 20:39:34 GMT
CMD ["/bin/sh"]
# Fri, 13 Oct 2023 20:39:43 GMT
ENV NATS_SERVER=2.10.3
# Fri, 13 Oct 2023 20:39:46 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='924a92491f549be8e8d51d56fc0cd211e8326933b9e7c2bbd31af0fdc7f15240' ;; 		armhf) natsArch='arm6'; sha256='dc8cfc756af14cda3c754ebfbe942616f7e3e65b8d846e7a34f5de2c55612a9d' ;; 		armv7) natsArch='arm7'; sha256='f8e4cf88d50800650b0fed026e776d8ca7eace6b0cbc4762beca7d0f3590ba00' ;; 		x86_64) natsArch='amd64'; sha256='a5587b04062a9cf117ec13aea5cb60cf4cd2e644be8c44628d85b5f4dfc19ab6' ;; 		x86) natsArch='386'; sha256='e8a1a521aeeef68abf2b1bd3baf3f359a073c25cef4f87aa505a49c1b0920e90' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 13 Oct 2023 20:39:46 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 13 Oct 2023 20:39:46 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 13 Oct 2023 20:39:46 GMT
EXPOSE 4222 6222 8222
# Fri, 13 Oct 2023 20:39:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 13 Oct 2023 20:39:46 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:579b34f0a95bb83b3acd6b3249ddc52c3d80f5c84b13c944e9e324feb86dd329`  
		Last Modified: Thu, 28 Sep 2023 20:40:08 GMT  
		Size: 3.3 MB (3331831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b89779f99904600f0b8257e364b4b34fbc2dfada2a75d6ef94cb9202a0b63b2f`  
		Last Modified: Fri, 13 Oct 2023 20:41:03 GMT  
		Size: 5.7 MB (5669169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97b37a3e5cd62562515d46192516aa3e3c3549500a7962fa65c0a37d0e143e2f`  
		Last Modified: Fri, 13 Oct 2023 20:41:02 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2f4fb413d4d2c0b6f57336bc01227dfe8bbef8a217d95c5d06496241c8c3d84`  
		Last Modified: Fri, 13 Oct 2023 20:41:02 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
