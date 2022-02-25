## `nats:alpine3.15`

```console
$ docker pull nats@sha256:6944283c7d430ef4d5e23afb87b2a2d9faf963793bcd94b0461bc12def6c74c2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:alpine3.15` - linux; amd64

```console
$ docker pull nats@sha256:6f8d631c068a9d37845ebee434d2c37606757634b9d8950e8de1035dc68842b4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7591453 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:775ec723ebf4c964b880457f54f66782e850e7121d3264c851da7d58cddb64bc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 24 Nov 2021 20:19:40 GMT
ADD file:9233f6f2237d79659a9521f7e390df217cec49f1a8aa3a12147bbca1956acdb9 in / 
# Wed, 24 Nov 2021 20:19:40 GMT
CMD ["/bin/sh"]
# Fri, 25 Feb 2022 02:21:01 GMT
ENV NATS_SERVER=2.7.3
# Fri, 25 Feb 2022 02:21:04 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='c895169ab34bc21442121f6c885905a254a9351a098402f319b3fbfd1e6225c9' ;; 		armhf) natsArch='arm6'; sha256='1b7e1c5835131825c4007766befd0c96a60edbcc3bc336a6739de5c8affea0c4' ;; 		armv7) natsArch='arm7'; sha256='723290467bc7e95b59ca7238a818932b199b00a21d4e3d7eb0e826b7aba2e0ea' ;; 		x86_64) natsArch='amd64'; sha256='2186c7660cd1d9774421614f6724ad32d7cec2389e39858f227a7991be41b1a7' ;; 		x86) natsArch='386'; sha256='3e8e2841921d555d06c67b1e33fc9bd934e4afec4748f7ddf27c67d707fafea4' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 25 Feb 2022 02:21:04 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 25 Feb 2022 02:21:04 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 25 Feb 2022 02:21:04 GMT
EXPOSE 4222 6222 8222
# Fri, 25 Feb 2022 02:21:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Feb 2022 02:21:05 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:59bf1c3509f33515622619af21ed55bbe26d24913cedbca106468a5fb37a50c3`  
		Last Modified: Wed, 24 Nov 2021 20:20:05 GMT  
		Size: 2.8 MB (2818413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfad251bce41e482876302125c33ef603e0ca99f33d1d274a09af07e1acd1be6`  
		Last Modified: Fri, 25 Feb 2022 02:21:40 GMT  
		Size: 4.8 MB (4772040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8c6f8e0dbab2106f703f51433a684cef43840e5e7443402b474f3c09144a4fe`  
		Last Modified: Fri, 25 Feb 2022 02:21:39 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0d8341c3c348e685617552e338228d15dd937ca0708bd7ab85c3c1b273ed88c`  
		Last Modified: Fri, 25 Feb 2022 02:21:39 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.15` - linux; arm variant v6

```console
$ docker pull nats@sha256:d6f43ae04309c6115c32d1c71469973712b3e817088a449ce37a9e8cb6b86bf9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7071601 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:846b4c8922b69a90d198633a7b622da89348aa9e3f7f11f58a294e2c4b112a33`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 24 Nov 2021 21:08:16 GMT
ADD file:61137e0aa49ba06f57ac69466fe2fb116f580b5e6159d56f846b1d72c4a3c814 in / 
# Wed, 24 Nov 2021 21:08:16 GMT
CMD ["/bin/sh"]
# Fri, 25 Feb 2022 02:49:34 GMT
ENV NATS_SERVER=2.7.3
# Fri, 25 Feb 2022 02:49:38 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='c895169ab34bc21442121f6c885905a254a9351a098402f319b3fbfd1e6225c9' ;; 		armhf) natsArch='arm6'; sha256='1b7e1c5835131825c4007766befd0c96a60edbcc3bc336a6739de5c8affea0c4' ;; 		armv7) natsArch='arm7'; sha256='723290467bc7e95b59ca7238a818932b199b00a21d4e3d7eb0e826b7aba2e0ea' ;; 		x86_64) natsArch='amd64'; sha256='2186c7660cd1d9774421614f6724ad32d7cec2389e39858f227a7991be41b1a7' ;; 		x86) natsArch='386'; sha256='3e8e2841921d555d06c67b1e33fc9bd934e4afec4748f7ddf27c67d707fafea4' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 25 Feb 2022 02:49:38 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 25 Feb 2022 02:49:39 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 25 Feb 2022 02:49:39 GMT
EXPOSE 4222 6222 8222
# Fri, 25 Feb 2022 02:49:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Feb 2022 02:49:40 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:e4a43de54da9e309482f6762f0c11f5f547cd8fd61a49c5f158453066162023e`  
		Last Modified: Wed, 24 Nov 2021 21:09:46 GMT  
		Size: 2.6 MB (2631421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ecb484648e454aaf42c41938db64a0715cb509a90811b5912192d2e66a2f7fb`  
		Last Modified: Fri, 25 Feb 2022 02:51:52 GMT  
		Size: 4.4 MB (4439176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdd675987846849cf3247fbc41b25505410823bffd30e841e7f663936458e553`  
		Last Modified: Fri, 25 Feb 2022 02:51:49 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ae450e4bdcdcad0dc3e04a43f8855409627f6c7fdecd22f661dbfe3a99530d2`  
		Last Modified: Fri, 25 Feb 2022 02:51:49 GMT  
		Size: 417.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.15` - linux; arm variant v7

```console
$ docker pull nats@sha256:665c6221a3c009747c340953834a8e1c6e38008d728f3a9d4d4eaab76e8e640d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.9 MB (6865015 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f23f21c3235ba9d61b53aeb161021b62412dc690dd81727439de14a1f9b902eb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 24 Nov 2021 21:42:11 GMT
ADD file:ca436da5b0bfc9c0e2fc685533c6628918000c8fff109fe9a8da625b9a798002 in / 
# Wed, 24 Nov 2021 21:42:11 GMT
CMD ["/bin/sh"]
# Fri, 25 Feb 2022 02:57:52 GMT
ENV NATS_SERVER=2.7.3
# Fri, 25 Feb 2022 02:57:56 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='c895169ab34bc21442121f6c885905a254a9351a098402f319b3fbfd1e6225c9' ;; 		armhf) natsArch='arm6'; sha256='1b7e1c5835131825c4007766befd0c96a60edbcc3bc336a6739de5c8affea0c4' ;; 		armv7) natsArch='arm7'; sha256='723290467bc7e95b59ca7238a818932b199b00a21d4e3d7eb0e826b7aba2e0ea' ;; 		x86_64) natsArch='amd64'; sha256='2186c7660cd1d9774421614f6724ad32d7cec2389e39858f227a7991be41b1a7' ;; 		x86) natsArch='386'; sha256='3e8e2841921d555d06c67b1e33fc9bd934e4afec4748f7ddf27c67d707fafea4' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 25 Feb 2022 02:57:57 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 25 Feb 2022 02:57:57 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 25 Feb 2022 02:57:58 GMT
EXPOSE 4222 6222 8222
# Fri, 25 Feb 2022 02:57:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Feb 2022 02:57:58 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:5480d2ca1740c20ce17652e01ed2265cdc914458acd41256a2b1ccff28f2762c`  
		Last Modified: Wed, 24 Nov 2021 21:43:40 GMT  
		Size: 2.4 MB (2434764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fafd4ba596baa033665a46ce765df0c4a928784832ecc5645944032cfcd9295`  
		Last Modified: Fri, 25 Feb 2022 03:00:20 GMT  
		Size: 4.4 MB (4429250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abb2edff52bc9250fdec4032d39728784d4495539ef65cceed401a8968ec2df5`  
		Last Modified: Fri, 25 Feb 2022 03:00:18 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1047f2aa448d4163e2995aed662d6890fdd3954289a1ff2908edc894450b3d78`  
		Last Modified: Fri, 25 Feb 2022 03:00:18 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.15` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:8f79d8af0b084884d2cc9641a33a1274022fc51b99e955d3f13d9c45f47cf6b4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7132810 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e50bb490b2ac0a89152a29fc28e269300b6b83d2a85c0ce5ebe74635c34cdb0d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 24 Nov 2021 20:39:20 GMT
ADD file:df53811312284306901fdaaff0a357a4bf40d631e662fe9ce6d342442e494b6c in / 
# Wed, 24 Nov 2021 20:39:20 GMT
CMD ["/bin/sh"]
# Fri, 25 Feb 2022 03:01:24 GMT
ENV NATS_SERVER=2.7.3
# Fri, 25 Feb 2022 03:01:26 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='c895169ab34bc21442121f6c885905a254a9351a098402f319b3fbfd1e6225c9' ;; 		armhf) natsArch='arm6'; sha256='1b7e1c5835131825c4007766befd0c96a60edbcc3bc336a6739de5c8affea0c4' ;; 		armv7) natsArch='arm7'; sha256='723290467bc7e95b59ca7238a818932b199b00a21d4e3d7eb0e826b7aba2e0ea' ;; 		x86_64) natsArch='amd64'; sha256='2186c7660cd1d9774421614f6724ad32d7cec2389e39858f227a7991be41b1a7' ;; 		x86) natsArch='386'; sha256='3e8e2841921d555d06c67b1e33fc9bd934e4afec4748f7ddf27c67d707fafea4' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 25 Feb 2022 03:01:28 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 25 Feb 2022 03:01:29 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 25 Feb 2022 03:01:29 GMT
EXPOSE 4222 6222 8222
# Fri, 25 Feb 2022 03:01:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Feb 2022 03:01:31 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9b3977197b4f2147bdd31e1271f811319dcd5c2fc595f14e81f5351ab6275b99`  
		Last Modified: Wed, 24 Nov 2021 20:39:59 GMT  
		Size: 2.7 MB (2715434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c75ed4d21bde940c8f5b4d0d82b44c31489bd5a37d46b1f197b7d1baed0b6e8`  
		Last Modified: Fri, 25 Feb 2022 03:02:31 GMT  
		Size: 4.4 MB (4416403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f7dd0d82f2c731b21df156c69326c651274a35eb010b23b5150397309110717`  
		Last Modified: Fri, 25 Feb 2022 03:02:30 GMT  
		Size: 559.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f29d0f81d7bbfb90bc5607be41aabbd3e970b1e74e19a069c23e863092772ba`  
		Last Modified: Fri, 25 Feb 2022 03:02:30 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
