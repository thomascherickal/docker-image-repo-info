<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `nats`

-	[`nats:2`](#nats2)
-	[`nats:2-alpine`](#nats2-alpine)
-	[`nats:2-alpine3.14`](#nats2-alpine314)
-	[`nats:2-linux`](#nats2-linux)
-	[`nats:2-nanoserver`](#nats2-nanoserver)
-	[`nats:2-nanoserver-1809`](#nats2-nanoserver-1809)
-	[`nats:2-scratch`](#nats2-scratch)
-	[`nats:2-windowsservercore`](#nats2-windowsservercore)
-	[`nats:2-windowsservercore-1809`](#nats2-windowsservercore-1809)
-	[`nats:2-windowsservercore-ltsc2016`](#nats2-windowsservercore-ltsc2016)
-	[`nats:2.6`](#nats26)
-	[`nats:2.6-alpine`](#nats26-alpine)
-	[`nats:2.6-alpine3.14`](#nats26-alpine314)
-	[`nats:2.6-linux`](#nats26-linux)
-	[`nats:2.6-nanoserver`](#nats26-nanoserver)
-	[`nats:2.6-nanoserver-1809`](#nats26-nanoserver-1809)
-	[`nats:2.6-scratch`](#nats26-scratch)
-	[`nats:2.6-windowsservercore`](#nats26-windowsservercore)
-	[`nats:2.6-windowsservercore-1809`](#nats26-windowsservercore-1809)
-	[`nats:2.6-windowsservercore-ltsc2016`](#nats26-windowsservercore-ltsc2016)
-	[`nats:2.6.6`](#nats266)
-	[`nats:2.6.6-alpine`](#nats266-alpine)
-	[`nats:2.6.6-alpine3.14`](#nats266-alpine314)
-	[`nats:2.6.6-linux`](#nats266-linux)
-	[`nats:2.6.6-nanoserver`](#nats266-nanoserver)
-	[`nats:2.6.6-nanoserver-1809`](#nats266-nanoserver-1809)
-	[`nats:2.6.6-scratch`](#nats266-scratch)
-	[`nats:2.6.6-windowsservercore`](#nats266-windowsservercore)
-	[`nats:2.6.6-windowsservercore-1809`](#nats266-windowsservercore-1809)
-	[`nats:2.6.6-windowsservercore-ltsc2016`](#nats266-windowsservercore-ltsc2016)
-	[`nats:alpine`](#natsalpine)
-	[`nats:alpine3.14`](#natsalpine314)
-	[`nats:latest`](#natslatest)
-	[`nats:linux`](#natslinux)
-	[`nats:nanoserver`](#natsnanoserver)
-	[`nats:nanoserver-1809`](#natsnanoserver-1809)
-	[`nats:scratch`](#natsscratch)
-	[`nats:windowsservercore`](#natswindowsservercore)
-	[`nats:windowsservercore-1809`](#natswindowsservercore-1809)
-	[`nats:windowsservercore-ltsc2016`](#natswindowsservercore-ltsc2016)

## `nats:2`

```console
$ docker pull nats@sha256:9bd747193a9d316341136227475dbde257fe33d6209b7b43beaf16ae0a358865
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.2452; amd64

### `nats:2` - linux; amd64

```console
$ docker pull nats@sha256:dad4f69520337c2a80d2a9123963c971836f07f530cf4b7c56dde98a622e0a6b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4578170 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ba73da93bdda8525a9f473851ee3de9a2d23c21e1d0a51d7da118bc122df420`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 03 Dec 2021 21:23:03 GMT
COPY file:4070919cac43aa01e3ef5dd95589f24a9d649dcc7b4d6364927c764b1f90392e in /nats-server 
# Fri, 03 Dec 2021 21:23:04 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 03 Dec 2021 21:23:04 GMT
EXPOSE 4222 6222 8222
# Fri, 03 Dec 2021 21:23:04 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 03 Dec 2021 21:23:04 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:730cae3de796bb1fbb06f0f847317c2b738bf9af9d1233daafcf2f708eade5ec`  
		Last Modified: Fri, 03 Dec 2021 21:24:01 GMT  
		Size: 4.6 MB (4577696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39027e71725d02ee81938943fd0f3e980f01abbe21c5e8f8ea8219687aaae862`  
		Last Modified: Fri, 03 Dec 2021 21:24:00 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - linux; arm variant v6

```console
$ docker pull nats@sha256:54395301fd2f315191df081131cd6d142613d057970268d64480f4706bcaeda3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4241317 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c4851d5f7b19bc49c52879a43236bae3e26e03a8a0f035ec150eed9a723cca5`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 02 Dec 2021 22:50:02 GMT
COPY file:6036f30fae4132d78e941219bf965a4e4c3e6d898ac912ab22e7a0cc98adf5a5 in /nats-server 
# Thu, 02 Dec 2021 22:50:03 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 02 Dec 2021 22:50:03 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Dec 2021 22:50:04 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 02 Dec 2021 22:50:04 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:41ef8f0f5e4d1f0e1880325ac8c2ccde63d323e6ead77b97c1225e0ce1d226ce`  
		Last Modified: Thu, 02 Dec 2021 22:52:29 GMT  
		Size: 4.2 MB (4240841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e8f034153e28423592a04f327fe3b69d3d84721cb54631e3ea9dcae375ab0ef`  
		Last Modified: Thu, 02 Dec 2021 22:52:26 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - linux; arm variant v7

```console
$ docker pull nats@sha256:78ee1d57413d89c46e808dbb121ad895537b74af783c6e6189366afa07638b66
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4237689 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b3276dd6f6de73a2af8ca0c6bd2dc88c7f7ae0a0ce334bcae39c14047aab540`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 04 Dec 2021 07:52:28 GMT
COPY file:025e99b21a301a69c768cc2c72e67c371165b6314d59d0a5a95958216fd24eac in /nats-server 
# Sat, 04 Dec 2021 07:52:28 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Sat, 04 Dec 2021 07:52:29 GMT
EXPOSE 4222 6222 8222
# Sat, 04 Dec 2021 07:52:29 GMT
ENTRYPOINT ["/nats-server"]
# Sat, 04 Dec 2021 07:52:30 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:75a8e365d6e58c8d8f7fe944a206f76f3e800542aca1b53e849c4bffc78fd22d`  
		Last Modified: Sat, 04 Dec 2021 07:55:01 GMT  
		Size: 4.2 MB (4237211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc2920e0912e6a42ee2fd0b7b8b31c6cca01c6c99f16c760f904492422ff7cae`  
		Last Modified: Sat, 04 Dec 2021 07:54:58 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:8ecffb2097f683980b94450d536a99c79b3fe7654f8bc91fd1c45ad0825e6aae
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4189764 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90bb404fba49386fc48ceb05ee04604d317ff225da69f159d0bd4cc63a930c0e`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 03 Dec 2021 16:57:31 GMT
COPY file:b5f62686ba6debf89a42d2be7c4442db5f8735dba6b8932e6f01f315a2e63e27 in /nats-server 
# Fri, 03 Dec 2021 16:57:32 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 03 Dec 2021 16:57:32 GMT
EXPOSE 4222 6222 8222
# Fri, 03 Dec 2021 16:57:33 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 03 Dec 2021 16:57:34 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:44ff62bde832e2b2bca85708fd2fc86d7d6d1f4ca7c58b5d0e18e3d07c9c5bac`  
		Last Modified: Fri, 03 Dec 2021 16:58:50 GMT  
		Size: 4.2 MB (4189288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44dcbc70566b6f8312605c0214812444ccad7a55594fa2e7f0792c21af818ef0`  
		Last Modified: Fri, 03 Dec 2021 16:58:49 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - windows version 10.0.17763.2452; amd64

```console
$ docker pull nats@sha256:73596edd7d2bcfb546b2b6da26cbaf06733398e7cc550a610ed8e53c5c59021c
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.7 MB (107674705 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa5c572d20b69e54dca9ee7a24b26d6b489d4cd2be1d5931d9accce1dbb7e030`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 07 Jan 2022 22:25:06 GMT
RUN Apply image 1809-amd64
# Wed, 12 Jan 2022 15:13:42 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 12 Jan 2022 15:13:43 GMT
RUN cmd /S /C #(nop) COPY file:20c797e6dad00d7098dbf6d4d158c380fd073bc5fc24a80fd4f23205af77a338 in C:\nats-server.exe 
# Wed, 12 Jan 2022 15:13:44 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 12 Jan 2022 15:13:45 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 12 Jan 2022 15:13:46 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 12 Jan 2022 15:13:47 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3a78847ea829208edc2d7b320b7e602b9d12e47689499d5180a9cc7790dec4d7`  
		Size: 103.0 MB (103031066 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:db05d2e76671d91772a070867bf6f050343319070602a0f8239706d5d4d98387`  
		Last Modified: Wed, 12 Jan 2022 15:14:49 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6271ae84b48476b5c259495509975bd53d7f398555179642c1ef1d612099cb19`  
		Last Modified: Wed, 12 Jan 2022 15:14:48 GMT  
		Size: 4.6 MB (4637258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:178ab94841651126bd3f8a1478a504e44f389c2bf5abf59abafc16f163108f4c`  
		Last Modified: Wed, 12 Jan 2022 15:14:46 GMT  
		Size: 1.8 KB (1759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aa2ac290e2024e6f26c6fd076cc312a10b4842536f9c9daad8ac0e5ecced071`  
		Last Modified: Wed, 12 Jan 2022 15:14:46 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8cb0f84aeae0a7ea0020f00dd7b55f02b772c0bfaa74ea61e1fbd266eff8928`  
		Last Modified: Wed, 12 Jan 2022 15:14:46 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7238bcc9c911d52c987ca07602cb3204bf985a35ae993830fe3b54ea9563de43`  
		Last Modified: Wed, 12 Jan 2022 15:14:46 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-alpine`

```console
$ docker pull nats@sha256:8e2e34eb798631cd76f341277f529f78618a2366d81b59586d3b81f6cb839b25
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-alpine` - linux; amd64

```console
$ docker pull nats@sha256:687f39ecdab1eeda8a4eaa7b7210586d96698faa5e5e7e47aaf5ef8084d504e5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.7 MB (7689543 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c5dc2cfb512e016e62911eca35c050a2eb5ca4b783d5f2d413ba64c68c420bd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:44 GMT
ADD file:762c899ec0505d1a32930ee804c5b008825f41611161be104076cba33b7e5b2b in / 
# Fri, 12 Nov 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 03 Dec 2021 21:22:18 GMT
ENV NATS_SERVER=2.6.6
# Fri, 03 Dec 2021 21:22:21 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='70da0ad3694aebfc742f9aae919d3a4aa5b8c863946e99c5d332195fbbdad49c' ;; 		armhf) natsArch='arm6'; sha256='e2cc1e198d5d5c83e2f2c2dcb15fafb71601603e3740065682812afaa7dd443a' ;; 		armv7) natsArch='arm7'; sha256='f3698a4fb18c6664d477b920d5f07637141a6623cf2fa998900155fea0d97e61' ;; 		x86_64) natsArch='amd64'; sha256='2c2fc16322fb2bc0b166ee2a01e163d4beb2cf7b49d083cebcd36695dc05a381' ;; 		x86) natsArch='386'; sha256='1da03b0d163dc98209f010bf6efa5fc6c81a23b4bab7a98bebe142e19fc26bdc' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 03 Dec 2021 21:22:21 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 03 Dec 2021 21:22:22 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 03 Dec 2021 21:22:22 GMT
EXPOSE 4222 6222 8222
# Fri, 03 Dec 2021 21:22:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 03 Dec 2021 21:22:22 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:97518928ae5f3d52d4164b314a7e73654eb686ecd8aafa0b79acd980773a740d`  
		Last Modified: Fri, 12 Nov 2021 17:20:39 GMT  
		Size: 2.8 MB (2822981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daeb19d8d614f4a1df58ed04d3c72469fa9f7286c9d5482ee274405723b5e645`  
		Last Modified: Fri, 03 Dec 2021 21:23:37 GMT  
		Size: 4.9 MB (4865593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e51c3679390c1ab0c5f5e6786505ad9278d45683059fc7fac0298dcbb6dede86`  
		Last Modified: Fri, 03 Dec 2021 21:23:36 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b14f15cf01b25470e7340acc8ca0860eb4a00a7e1b5d5180bd7c23db1dd273af`  
		Last Modified: Fri, 03 Dec 2021 21:23:36 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:d42d25248435c99492dd0fbcd97688486c692c680069bc9a1eb8a7b1c85eebff
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7161537 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ae84a8c7e689bc4d7fd2915ef9aaf1fb624c094cb183af5863d4b20984f29cd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 12 Nov 2021 16:49:42 GMT
ADD file:6daf1fe862c00673bf9cf4d7e20b0bf253a56e7fb8ed5e730a4466ab9186e18a in / 
# Fri, 12 Nov 2021 16:49:44 GMT
CMD ["/bin/sh"]
# Thu, 02 Dec 2021 22:49:35 GMT
ENV NATS_SERVER=2.6.6
# Thu, 02 Dec 2021 22:49:39 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='70da0ad3694aebfc742f9aae919d3a4aa5b8c863946e99c5d332195fbbdad49c' ;; 		armhf) natsArch='arm6'; sha256='e2cc1e198d5d5c83e2f2c2dcb15fafb71601603e3740065682812afaa7dd443a' ;; 		armv7) natsArch='arm7'; sha256='f3698a4fb18c6664d477b920d5f07637141a6623cf2fa998900155fea0d97e61' ;; 		x86_64) natsArch='amd64'; sha256='2c2fc16322fb2bc0b166ee2a01e163d4beb2cf7b49d083cebcd36695dc05a381' ;; 		x86) natsArch='386'; sha256='1da03b0d163dc98209f010bf6efa5fc6c81a23b4bab7a98bebe142e19fc26bdc' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 02 Dec 2021 22:49:40 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 02 Dec 2021 22:49:40 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 02 Dec 2021 22:49:41 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Dec 2021 22:49:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 02 Dec 2021 22:49:42 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:56afcfda5d78cc243287acbaad250c5e8c0f47aae620dd7c51985b0d3c9b2728`  
		Last Modified: Fri, 12 Nov 2021 16:51:32 GMT  
		Size: 2.6 MB (2635392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3c7b89c441a056fc0e4d867cd4fd28308f188bd0f6b306e5feee96fee47cbdf`  
		Last Modified: Thu, 02 Dec 2021 22:51:52 GMT  
		Size: 4.5 MB (4525169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f67a5f3b97f233f2d6d30a90acd85b9e856cb9b98c298b71e2b5cbae3e0268cf`  
		Last Modified: Thu, 02 Dec 2021 22:51:50 GMT  
		Size: 561.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:706486ffe19b237b40203ebf10cb1110d7566cba5a3c10bf738be70173a1aa69`  
		Last Modified: Thu, 02 Dec 2021 22:51:50 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:dbc345345cfc225bd88b35e80f85f412483db712134bde3a0e4d959cb543350f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.0 MB (6958146 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6aaa47180fd5390c3f39b81e39db30c26897fc1b070c064d4677ebdd14c1f801`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 12 Nov 2021 16:57:35 GMT
ADD file:03e0720458c3475758bf4394afa56f2165198eb91e6e9581f7768e433744dd9b in / 
# Fri, 12 Nov 2021 16:57:36 GMT
CMD ["/bin/sh"]
# Sat, 04 Dec 2021 07:51:50 GMT
ENV NATS_SERVER=2.6.6
# Sat, 04 Dec 2021 07:51:54 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='70da0ad3694aebfc742f9aae919d3a4aa5b8c863946e99c5d332195fbbdad49c' ;; 		armhf) natsArch='arm6'; sha256='e2cc1e198d5d5c83e2f2c2dcb15fafb71601603e3740065682812afaa7dd443a' ;; 		armv7) natsArch='arm7'; sha256='f3698a4fb18c6664d477b920d5f07637141a6623cf2fa998900155fea0d97e61' ;; 		x86_64) natsArch='amd64'; sha256='2c2fc16322fb2bc0b166ee2a01e163d4beb2cf7b49d083cebcd36695dc05a381' ;; 		x86) natsArch='386'; sha256='1da03b0d163dc98209f010bf6efa5fc6c81a23b4bab7a98bebe142e19fc26bdc' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Sat, 04 Dec 2021 07:51:55 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Sat, 04 Dec 2021 07:51:55 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Sat, 04 Dec 2021 07:51:56 GMT
EXPOSE 4222 6222 8222
# Sat, 04 Dec 2021 07:51:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 04 Dec 2021 07:51:57 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:764d2e53e1a607f2d8261522185d5b9021ade3ec1a595664ee90308c00176899`  
		Last Modified: Fri, 12 Nov 2021 16:59:33 GMT  
		Size: 2.4 MB (2438618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:157eac698795baeacb3153cf2bbbc17f348e477e8062fa45b6728e97dd02e157`  
		Last Modified: Sat, 04 Dec 2021 07:54:19 GMT  
		Size: 4.5 MB (4518555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b5241fcba964a14f9c4681ebcc94815a476df86f68c628494f5759a3bee8514`  
		Last Modified: Sat, 04 Dec 2021 07:54:16 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36d02df08ee2f75a857120c105153a83b2b951337a87e902260e70e1de20dfd0`  
		Last Modified: Sat, 04 Dec 2021 07:54:16 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:f1e7262504ed73a185ee16f6a6da14c19c3a76120f2b22c51a051a0988ac3bdc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7193478 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55e483df89c189235b79aa4a9d2417378172236dba6fa85f6d5a0bb35756835f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 12 Nov 2021 16:39:58 GMT
ADD file:400c0466b29ccad54e0f6c0acef22542992828678c96693ef1f9f4d0551935d8 in / 
# Fri, 12 Nov 2021 16:39:58 GMT
CMD ["/bin/sh"]
# Fri, 03 Dec 2021 16:57:10 GMT
ENV NATS_SERVER=2.6.6
# Fri, 03 Dec 2021 16:57:13 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='70da0ad3694aebfc742f9aae919d3a4aa5b8c863946e99c5d332195fbbdad49c' ;; 		armhf) natsArch='arm6'; sha256='e2cc1e198d5d5c83e2f2c2dcb15fafb71601603e3740065682812afaa7dd443a' ;; 		armv7) natsArch='arm7'; sha256='f3698a4fb18c6664d477b920d5f07637141a6623cf2fa998900155fea0d97e61' ;; 		x86_64) natsArch='amd64'; sha256='2c2fc16322fb2bc0b166ee2a01e163d4beb2cf7b49d083cebcd36695dc05a381' ;; 		x86) natsArch='386'; sha256='1da03b0d163dc98209f010bf6efa5fc6c81a23b4bab7a98bebe142e19fc26bdc' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 03 Dec 2021 16:57:15 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 03 Dec 2021 16:57:16 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 03 Dec 2021 16:57:16 GMT
EXPOSE 4222 6222 8222
# Fri, 03 Dec 2021 16:57:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 03 Dec 2021 16:57:18 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:be307f383ecc62b27a29b599c3fc9d3129693a798e7fcce614f09174cfe2d354`  
		Last Modified: Fri, 12 Nov 2021 16:40:59 GMT  
		Size: 2.7 MB (2717700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdee3b2a5421d3ceb50b8101857ce4c0815c4532476e1f292867c63034c08f61`  
		Last Modified: Fri, 03 Dec 2021 16:58:22 GMT  
		Size: 4.5 MB (4474835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8a771880289bb86cd368ca8b39620b0cfe69694646e061ff6975f959ccfcd29`  
		Last Modified: Fri, 03 Dec 2021 16:58:21 GMT  
		Size: 528.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:438c5abdffd6599ac83fe661d26a9491552d63f48aeb9147609299ee11b78c78`  
		Last Modified: Fri, 03 Dec 2021 16:58:21 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-alpine3.14`

```console
$ docker pull nats@sha256:8e2e34eb798631cd76f341277f529f78618a2366d81b59586d3b81f6cb839b25
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-alpine3.14` - linux; amd64

```console
$ docker pull nats@sha256:687f39ecdab1eeda8a4eaa7b7210586d96698faa5e5e7e47aaf5ef8084d504e5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.7 MB (7689543 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c5dc2cfb512e016e62911eca35c050a2eb5ca4b783d5f2d413ba64c68c420bd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:44 GMT
ADD file:762c899ec0505d1a32930ee804c5b008825f41611161be104076cba33b7e5b2b in / 
# Fri, 12 Nov 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 03 Dec 2021 21:22:18 GMT
ENV NATS_SERVER=2.6.6
# Fri, 03 Dec 2021 21:22:21 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='70da0ad3694aebfc742f9aae919d3a4aa5b8c863946e99c5d332195fbbdad49c' ;; 		armhf) natsArch='arm6'; sha256='e2cc1e198d5d5c83e2f2c2dcb15fafb71601603e3740065682812afaa7dd443a' ;; 		armv7) natsArch='arm7'; sha256='f3698a4fb18c6664d477b920d5f07637141a6623cf2fa998900155fea0d97e61' ;; 		x86_64) natsArch='amd64'; sha256='2c2fc16322fb2bc0b166ee2a01e163d4beb2cf7b49d083cebcd36695dc05a381' ;; 		x86) natsArch='386'; sha256='1da03b0d163dc98209f010bf6efa5fc6c81a23b4bab7a98bebe142e19fc26bdc' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 03 Dec 2021 21:22:21 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 03 Dec 2021 21:22:22 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 03 Dec 2021 21:22:22 GMT
EXPOSE 4222 6222 8222
# Fri, 03 Dec 2021 21:22:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 03 Dec 2021 21:22:22 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:97518928ae5f3d52d4164b314a7e73654eb686ecd8aafa0b79acd980773a740d`  
		Last Modified: Fri, 12 Nov 2021 17:20:39 GMT  
		Size: 2.8 MB (2822981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daeb19d8d614f4a1df58ed04d3c72469fa9f7286c9d5482ee274405723b5e645`  
		Last Modified: Fri, 03 Dec 2021 21:23:37 GMT  
		Size: 4.9 MB (4865593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e51c3679390c1ab0c5f5e6786505ad9278d45683059fc7fac0298dcbb6dede86`  
		Last Modified: Fri, 03 Dec 2021 21:23:36 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b14f15cf01b25470e7340acc8ca0860eb4a00a7e1b5d5180bd7c23db1dd273af`  
		Last Modified: Fri, 03 Dec 2021 21:23:36 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.14` - linux; arm variant v6

```console
$ docker pull nats@sha256:d42d25248435c99492dd0fbcd97688486c692c680069bc9a1eb8a7b1c85eebff
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7161537 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ae84a8c7e689bc4d7fd2915ef9aaf1fb624c094cb183af5863d4b20984f29cd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 12 Nov 2021 16:49:42 GMT
ADD file:6daf1fe862c00673bf9cf4d7e20b0bf253a56e7fb8ed5e730a4466ab9186e18a in / 
# Fri, 12 Nov 2021 16:49:44 GMT
CMD ["/bin/sh"]
# Thu, 02 Dec 2021 22:49:35 GMT
ENV NATS_SERVER=2.6.6
# Thu, 02 Dec 2021 22:49:39 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='70da0ad3694aebfc742f9aae919d3a4aa5b8c863946e99c5d332195fbbdad49c' ;; 		armhf) natsArch='arm6'; sha256='e2cc1e198d5d5c83e2f2c2dcb15fafb71601603e3740065682812afaa7dd443a' ;; 		armv7) natsArch='arm7'; sha256='f3698a4fb18c6664d477b920d5f07637141a6623cf2fa998900155fea0d97e61' ;; 		x86_64) natsArch='amd64'; sha256='2c2fc16322fb2bc0b166ee2a01e163d4beb2cf7b49d083cebcd36695dc05a381' ;; 		x86) natsArch='386'; sha256='1da03b0d163dc98209f010bf6efa5fc6c81a23b4bab7a98bebe142e19fc26bdc' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 02 Dec 2021 22:49:40 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 02 Dec 2021 22:49:40 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 02 Dec 2021 22:49:41 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Dec 2021 22:49:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 02 Dec 2021 22:49:42 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:56afcfda5d78cc243287acbaad250c5e8c0f47aae620dd7c51985b0d3c9b2728`  
		Last Modified: Fri, 12 Nov 2021 16:51:32 GMT  
		Size: 2.6 MB (2635392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3c7b89c441a056fc0e4d867cd4fd28308f188bd0f6b306e5feee96fee47cbdf`  
		Last Modified: Thu, 02 Dec 2021 22:51:52 GMT  
		Size: 4.5 MB (4525169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f67a5f3b97f233f2d6d30a90acd85b9e856cb9b98c298b71e2b5cbae3e0268cf`  
		Last Modified: Thu, 02 Dec 2021 22:51:50 GMT  
		Size: 561.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:706486ffe19b237b40203ebf10cb1110d7566cba5a3c10bf738be70173a1aa69`  
		Last Modified: Thu, 02 Dec 2021 22:51:50 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.14` - linux; arm variant v7

```console
$ docker pull nats@sha256:dbc345345cfc225bd88b35e80f85f412483db712134bde3a0e4d959cb543350f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.0 MB (6958146 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6aaa47180fd5390c3f39b81e39db30c26897fc1b070c064d4677ebdd14c1f801`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 12 Nov 2021 16:57:35 GMT
ADD file:03e0720458c3475758bf4394afa56f2165198eb91e6e9581f7768e433744dd9b in / 
# Fri, 12 Nov 2021 16:57:36 GMT
CMD ["/bin/sh"]
# Sat, 04 Dec 2021 07:51:50 GMT
ENV NATS_SERVER=2.6.6
# Sat, 04 Dec 2021 07:51:54 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='70da0ad3694aebfc742f9aae919d3a4aa5b8c863946e99c5d332195fbbdad49c' ;; 		armhf) natsArch='arm6'; sha256='e2cc1e198d5d5c83e2f2c2dcb15fafb71601603e3740065682812afaa7dd443a' ;; 		armv7) natsArch='arm7'; sha256='f3698a4fb18c6664d477b920d5f07637141a6623cf2fa998900155fea0d97e61' ;; 		x86_64) natsArch='amd64'; sha256='2c2fc16322fb2bc0b166ee2a01e163d4beb2cf7b49d083cebcd36695dc05a381' ;; 		x86) natsArch='386'; sha256='1da03b0d163dc98209f010bf6efa5fc6c81a23b4bab7a98bebe142e19fc26bdc' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Sat, 04 Dec 2021 07:51:55 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Sat, 04 Dec 2021 07:51:55 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Sat, 04 Dec 2021 07:51:56 GMT
EXPOSE 4222 6222 8222
# Sat, 04 Dec 2021 07:51:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 04 Dec 2021 07:51:57 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:764d2e53e1a607f2d8261522185d5b9021ade3ec1a595664ee90308c00176899`  
		Last Modified: Fri, 12 Nov 2021 16:59:33 GMT  
		Size: 2.4 MB (2438618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:157eac698795baeacb3153cf2bbbc17f348e477e8062fa45b6728e97dd02e157`  
		Last Modified: Sat, 04 Dec 2021 07:54:19 GMT  
		Size: 4.5 MB (4518555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b5241fcba964a14f9c4681ebcc94815a476df86f68c628494f5759a3bee8514`  
		Last Modified: Sat, 04 Dec 2021 07:54:16 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36d02df08ee2f75a857120c105153a83b2b951337a87e902260e70e1de20dfd0`  
		Last Modified: Sat, 04 Dec 2021 07:54:16 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.14` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:f1e7262504ed73a185ee16f6a6da14c19c3a76120f2b22c51a051a0988ac3bdc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7193478 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55e483df89c189235b79aa4a9d2417378172236dba6fa85f6d5a0bb35756835f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 12 Nov 2021 16:39:58 GMT
ADD file:400c0466b29ccad54e0f6c0acef22542992828678c96693ef1f9f4d0551935d8 in / 
# Fri, 12 Nov 2021 16:39:58 GMT
CMD ["/bin/sh"]
# Fri, 03 Dec 2021 16:57:10 GMT
ENV NATS_SERVER=2.6.6
# Fri, 03 Dec 2021 16:57:13 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='70da0ad3694aebfc742f9aae919d3a4aa5b8c863946e99c5d332195fbbdad49c' ;; 		armhf) natsArch='arm6'; sha256='e2cc1e198d5d5c83e2f2c2dcb15fafb71601603e3740065682812afaa7dd443a' ;; 		armv7) natsArch='arm7'; sha256='f3698a4fb18c6664d477b920d5f07637141a6623cf2fa998900155fea0d97e61' ;; 		x86_64) natsArch='amd64'; sha256='2c2fc16322fb2bc0b166ee2a01e163d4beb2cf7b49d083cebcd36695dc05a381' ;; 		x86) natsArch='386'; sha256='1da03b0d163dc98209f010bf6efa5fc6c81a23b4bab7a98bebe142e19fc26bdc' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 03 Dec 2021 16:57:15 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 03 Dec 2021 16:57:16 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 03 Dec 2021 16:57:16 GMT
EXPOSE 4222 6222 8222
# Fri, 03 Dec 2021 16:57:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 03 Dec 2021 16:57:18 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:be307f383ecc62b27a29b599c3fc9d3129693a798e7fcce614f09174cfe2d354`  
		Last Modified: Fri, 12 Nov 2021 16:40:59 GMT  
		Size: 2.7 MB (2717700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdee3b2a5421d3ceb50b8101857ce4c0815c4532476e1f292867c63034c08f61`  
		Last Modified: Fri, 03 Dec 2021 16:58:22 GMT  
		Size: 4.5 MB (4474835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8a771880289bb86cd368ca8b39620b0cfe69694646e061ff6975f959ccfcd29`  
		Last Modified: Fri, 03 Dec 2021 16:58:21 GMT  
		Size: 528.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:438c5abdffd6599ac83fe661d26a9491552d63f48aeb9147609299ee11b78c78`  
		Last Modified: Fri, 03 Dec 2021 16:58:21 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-linux`

```console
$ docker pull nats@sha256:5d130fed2ad109f922a3a52e45c0b87c0d5a674ad432024cb3d45f898cf425b8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-linux` - linux; amd64

```console
$ docker pull nats@sha256:dad4f69520337c2a80d2a9123963c971836f07f530cf4b7c56dde98a622e0a6b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4578170 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ba73da93bdda8525a9f473851ee3de9a2d23c21e1d0a51d7da118bc122df420`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 03 Dec 2021 21:23:03 GMT
COPY file:4070919cac43aa01e3ef5dd95589f24a9d649dcc7b4d6364927c764b1f90392e in /nats-server 
# Fri, 03 Dec 2021 21:23:04 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 03 Dec 2021 21:23:04 GMT
EXPOSE 4222 6222 8222
# Fri, 03 Dec 2021 21:23:04 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 03 Dec 2021 21:23:04 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:730cae3de796bb1fbb06f0f847317c2b738bf9af9d1233daafcf2f708eade5ec`  
		Last Modified: Fri, 03 Dec 2021 21:24:01 GMT  
		Size: 4.6 MB (4577696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39027e71725d02ee81938943fd0f3e980f01abbe21c5e8f8ea8219687aaae862`  
		Last Modified: Fri, 03 Dec 2021 21:24:00 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:54395301fd2f315191df081131cd6d142613d057970268d64480f4706bcaeda3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4241317 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c4851d5f7b19bc49c52879a43236bae3e26e03a8a0f035ec150eed9a723cca5`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 02 Dec 2021 22:50:02 GMT
COPY file:6036f30fae4132d78e941219bf965a4e4c3e6d898ac912ab22e7a0cc98adf5a5 in /nats-server 
# Thu, 02 Dec 2021 22:50:03 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 02 Dec 2021 22:50:03 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Dec 2021 22:50:04 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 02 Dec 2021 22:50:04 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:41ef8f0f5e4d1f0e1880325ac8c2ccde63d323e6ead77b97c1225e0ce1d226ce`  
		Last Modified: Thu, 02 Dec 2021 22:52:29 GMT  
		Size: 4.2 MB (4240841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e8f034153e28423592a04f327fe3b69d3d84721cb54631e3ea9dcae375ab0ef`  
		Last Modified: Thu, 02 Dec 2021 22:52:26 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:78ee1d57413d89c46e808dbb121ad895537b74af783c6e6189366afa07638b66
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4237689 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b3276dd6f6de73a2af8ca0c6bd2dc88c7f7ae0a0ce334bcae39c14047aab540`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 04 Dec 2021 07:52:28 GMT
COPY file:025e99b21a301a69c768cc2c72e67c371165b6314d59d0a5a95958216fd24eac in /nats-server 
# Sat, 04 Dec 2021 07:52:28 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Sat, 04 Dec 2021 07:52:29 GMT
EXPOSE 4222 6222 8222
# Sat, 04 Dec 2021 07:52:29 GMT
ENTRYPOINT ["/nats-server"]
# Sat, 04 Dec 2021 07:52:30 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:75a8e365d6e58c8d8f7fe944a206f76f3e800542aca1b53e849c4bffc78fd22d`  
		Last Modified: Sat, 04 Dec 2021 07:55:01 GMT  
		Size: 4.2 MB (4237211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc2920e0912e6a42ee2fd0b7b8b31c6cca01c6c99f16c760f904492422ff7cae`  
		Last Modified: Sat, 04 Dec 2021 07:54:58 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:8ecffb2097f683980b94450d536a99c79b3fe7654f8bc91fd1c45ad0825e6aae
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4189764 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90bb404fba49386fc48ceb05ee04604d317ff225da69f159d0bd4cc63a930c0e`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 03 Dec 2021 16:57:31 GMT
COPY file:b5f62686ba6debf89a42d2be7c4442db5f8735dba6b8932e6f01f315a2e63e27 in /nats-server 
# Fri, 03 Dec 2021 16:57:32 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 03 Dec 2021 16:57:32 GMT
EXPOSE 4222 6222 8222
# Fri, 03 Dec 2021 16:57:33 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 03 Dec 2021 16:57:34 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:44ff62bde832e2b2bca85708fd2fc86d7d6d1f4ca7c58b5d0e18e3d07c9c5bac`  
		Last Modified: Fri, 03 Dec 2021 16:58:50 GMT  
		Size: 4.2 MB (4189288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44dcbc70566b6f8312605c0214812444ccad7a55594fa2e7f0792c21af818ef0`  
		Last Modified: Fri, 03 Dec 2021 16:58:49 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-nanoserver`

```console
$ docker pull nats@sha256:0b2895172f1057f6c9b6bfeb7502714c3bfee379610222e16e17a226fc537354
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2452; amd64

### `nats:2-nanoserver` - windows version 10.0.17763.2452; amd64

```console
$ docker pull nats@sha256:73596edd7d2bcfb546b2b6da26cbaf06733398e7cc550a610ed8e53c5c59021c
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.7 MB (107674705 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa5c572d20b69e54dca9ee7a24b26d6b489d4cd2be1d5931d9accce1dbb7e030`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 07 Jan 2022 22:25:06 GMT
RUN Apply image 1809-amd64
# Wed, 12 Jan 2022 15:13:42 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 12 Jan 2022 15:13:43 GMT
RUN cmd /S /C #(nop) COPY file:20c797e6dad00d7098dbf6d4d158c380fd073bc5fc24a80fd4f23205af77a338 in C:\nats-server.exe 
# Wed, 12 Jan 2022 15:13:44 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 12 Jan 2022 15:13:45 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 12 Jan 2022 15:13:46 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 12 Jan 2022 15:13:47 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3a78847ea829208edc2d7b320b7e602b9d12e47689499d5180a9cc7790dec4d7`  
		Size: 103.0 MB (103031066 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:db05d2e76671d91772a070867bf6f050343319070602a0f8239706d5d4d98387`  
		Last Modified: Wed, 12 Jan 2022 15:14:49 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6271ae84b48476b5c259495509975bd53d7f398555179642c1ef1d612099cb19`  
		Last Modified: Wed, 12 Jan 2022 15:14:48 GMT  
		Size: 4.6 MB (4637258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:178ab94841651126bd3f8a1478a504e44f389c2bf5abf59abafc16f163108f4c`  
		Last Modified: Wed, 12 Jan 2022 15:14:46 GMT  
		Size: 1.8 KB (1759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aa2ac290e2024e6f26c6fd076cc312a10b4842536f9c9daad8ac0e5ecced071`  
		Last Modified: Wed, 12 Jan 2022 15:14:46 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8cb0f84aeae0a7ea0020f00dd7b55f02b772c0bfaa74ea61e1fbd266eff8928`  
		Last Modified: Wed, 12 Jan 2022 15:14:46 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7238bcc9c911d52c987ca07602cb3204bf985a35ae993830fe3b54ea9563de43`  
		Last Modified: Wed, 12 Jan 2022 15:14:46 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-nanoserver-1809`

```console
$ docker pull nats@sha256:0b2895172f1057f6c9b6bfeb7502714c3bfee379610222e16e17a226fc537354
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2452; amd64

### `nats:2-nanoserver-1809` - windows version 10.0.17763.2452; amd64

```console
$ docker pull nats@sha256:73596edd7d2bcfb546b2b6da26cbaf06733398e7cc550a610ed8e53c5c59021c
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.7 MB (107674705 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa5c572d20b69e54dca9ee7a24b26d6b489d4cd2be1d5931d9accce1dbb7e030`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 07 Jan 2022 22:25:06 GMT
RUN Apply image 1809-amd64
# Wed, 12 Jan 2022 15:13:42 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 12 Jan 2022 15:13:43 GMT
RUN cmd /S /C #(nop) COPY file:20c797e6dad00d7098dbf6d4d158c380fd073bc5fc24a80fd4f23205af77a338 in C:\nats-server.exe 
# Wed, 12 Jan 2022 15:13:44 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 12 Jan 2022 15:13:45 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 12 Jan 2022 15:13:46 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 12 Jan 2022 15:13:47 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3a78847ea829208edc2d7b320b7e602b9d12e47689499d5180a9cc7790dec4d7`  
		Size: 103.0 MB (103031066 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:db05d2e76671d91772a070867bf6f050343319070602a0f8239706d5d4d98387`  
		Last Modified: Wed, 12 Jan 2022 15:14:49 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6271ae84b48476b5c259495509975bd53d7f398555179642c1ef1d612099cb19`  
		Last Modified: Wed, 12 Jan 2022 15:14:48 GMT  
		Size: 4.6 MB (4637258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:178ab94841651126bd3f8a1478a504e44f389c2bf5abf59abafc16f163108f4c`  
		Last Modified: Wed, 12 Jan 2022 15:14:46 GMT  
		Size: 1.8 KB (1759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aa2ac290e2024e6f26c6fd076cc312a10b4842536f9c9daad8ac0e5ecced071`  
		Last Modified: Wed, 12 Jan 2022 15:14:46 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8cb0f84aeae0a7ea0020f00dd7b55f02b772c0bfaa74ea61e1fbd266eff8928`  
		Last Modified: Wed, 12 Jan 2022 15:14:46 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7238bcc9c911d52c987ca07602cb3204bf985a35ae993830fe3b54ea9563de43`  
		Last Modified: Wed, 12 Jan 2022 15:14:46 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-scratch`

```console
$ docker pull nats@sha256:5d130fed2ad109f922a3a52e45c0b87c0d5a674ad432024cb3d45f898cf425b8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-scratch` - linux; amd64

```console
$ docker pull nats@sha256:dad4f69520337c2a80d2a9123963c971836f07f530cf4b7c56dde98a622e0a6b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4578170 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ba73da93bdda8525a9f473851ee3de9a2d23c21e1d0a51d7da118bc122df420`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 03 Dec 2021 21:23:03 GMT
COPY file:4070919cac43aa01e3ef5dd95589f24a9d649dcc7b4d6364927c764b1f90392e in /nats-server 
# Fri, 03 Dec 2021 21:23:04 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 03 Dec 2021 21:23:04 GMT
EXPOSE 4222 6222 8222
# Fri, 03 Dec 2021 21:23:04 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 03 Dec 2021 21:23:04 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:730cae3de796bb1fbb06f0f847317c2b738bf9af9d1233daafcf2f708eade5ec`  
		Last Modified: Fri, 03 Dec 2021 21:24:01 GMT  
		Size: 4.6 MB (4577696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39027e71725d02ee81938943fd0f3e980f01abbe21c5e8f8ea8219687aaae862`  
		Last Modified: Fri, 03 Dec 2021 21:24:00 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:54395301fd2f315191df081131cd6d142613d057970268d64480f4706bcaeda3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4241317 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c4851d5f7b19bc49c52879a43236bae3e26e03a8a0f035ec150eed9a723cca5`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 02 Dec 2021 22:50:02 GMT
COPY file:6036f30fae4132d78e941219bf965a4e4c3e6d898ac912ab22e7a0cc98adf5a5 in /nats-server 
# Thu, 02 Dec 2021 22:50:03 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 02 Dec 2021 22:50:03 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Dec 2021 22:50:04 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 02 Dec 2021 22:50:04 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:41ef8f0f5e4d1f0e1880325ac8c2ccde63d323e6ead77b97c1225e0ce1d226ce`  
		Last Modified: Thu, 02 Dec 2021 22:52:29 GMT  
		Size: 4.2 MB (4240841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e8f034153e28423592a04f327fe3b69d3d84721cb54631e3ea9dcae375ab0ef`  
		Last Modified: Thu, 02 Dec 2021 22:52:26 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:78ee1d57413d89c46e808dbb121ad895537b74af783c6e6189366afa07638b66
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4237689 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b3276dd6f6de73a2af8ca0c6bd2dc88c7f7ae0a0ce334bcae39c14047aab540`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 04 Dec 2021 07:52:28 GMT
COPY file:025e99b21a301a69c768cc2c72e67c371165b6314d59d0a5a95958216fd24eac in /nats-server 
# Sat, 04 Dec 2021 07:52:28 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Sat, 04 Dec 2021 07:52:29 GMT
EXPOSE 4222 6222 8222
# Sat, 04 Dec 2021 07:52:29 GMT
ENTRYPOINT ["/nats-server"]
# Sat, 04 Dec 2021 07:52:30 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:75a8e365d6e58c8d8f7fe944a206f76f3e800542aca1b53e849c4bffc78fd22d`  
		Last Modified: Sat, 04 Dec 2021 07:55:01 GMT  
		Size: 4.2 MB (4237211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc2920e0912e6a42ee2fd0b7b8b31c6cca01c6c99f16c760f904492422ff7cae`  
		Last Modified: Sat, 04 Dec 2021 07:54:58 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:8ecffb2097f683980b94450d536a99c79b3fe7654f8bc91fd1c45ad0825e6aae
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4189764 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90bb404fba49386fc48ceb05ee04604d317ff225da69f159d0bd4cc63a930c0e`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 03 Dec 2021 16:57:31 GMT
COPY file:b5f62686ba6debf89a42d2be7c4442db5f8735dba6b8932e6f01f315a2e63e27 in /nats-server 
# Fri, 03 Dec 2021 16:57:32 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 03 Dec 2021 16:57:32 GMT
EXPOSE 4222 6222 8222
# Fri, 03 Dec 2021 16:57:33 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 03 Dec 2021 16:57:34 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:44ff62bde832e2b2bca85708fd2fc86d7d6d1f4ca7c58b5d0e18e3d07c9c5bac`  
		Last Modified: Fri, 03 Dec 2021 16:58:50 GMT  
		Size: 4.2 MB (4189288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44dcbc70566b6f8312605c0214812444ccad7a55594fa2e7f0792c21af818ef0`  
		Last Modified: Fri, 03 Dec 2021 16:58:49 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-windowsservercore`

```console
$ docker pull nats@sha256:24e44e15d62a911e94d6ff5b7e22accfe329f699b42ade9ebb1a5caa3197f373
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.2452; amd64
	-	windows version 10.0.14393.4886; amd64

### `nats:2-windowsservercore` - windows version 10.0.17763.2452; amd64

```console
$ docker pull nats@sha256:7f3bfcdbda90968d69223b48664ee1ec937a82bce7365c82135785fe353ba699
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2717536770 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4622435affd612664c15aa4fd83b1e45ba56de92d3c7e6dd3dd924adf28111bf`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 07 Jan 2022 22:48:13 GMT
RUN Install update 1809-amd64
# Wed, 12 Jan 2022 13:54:17 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 Jan 2022 15:10:29 GMT
ENV NATS_DOCKERIZED=1
# Wed, 12 Jan 2022 15:10:30 GMT
ENV NATS_SERVER=2.6.6
# Wed, 12 Jan 2022 15:10:32 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.6.6/nats-server-v2.6.6-windows-amd64.zip
# Wed, 12 Jan 2022 15:10:33 GMT
ENV NATS_SERVER_SHASUM=9730ea401beed7ac40aeada0a8dccfb70207bb234202035aad5644e93ec657da
# Wed, 12 Jan 2022 15:11:32 GMT
RUN Set-PSDebug -Trace 2
# Wed, 12 Jan 2022 15:13:24 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 12 Jan 2022 15:13:26 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 12 Jan 2022 15:13:27 GMT
EXPOSE 4222 6222 8222
# Wed, 12 Jan 2022 15:13:28 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 12 Jan 2022 15:13:29 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:635f15ebd5b486e8a00bf217a0574a29550e5bbf08c1d021e1e308100b2e49b5`  
		Size: 993.9 MB (993898043 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:537828534783cff318d36854dbda0683aef7263e437c7c669de4092e1778959c`  
		Last Modified: Wed, 12 Jan 2022 15:14:30 GMT  
		Size: 1.3 KB (1296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9576e7772519d67febb0ceb94d8f22531ea99f0c60c36e67a4f5a497c384f5e0`  
		Last Modified: Wed, 12 Jan 2022 15:14:30 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaf1f761c394ef0da3c3fef1865f52e977d392f3f0b6c0575c3d1341da6cd7e9`  
		Last Modified: Wed, 12 Jan 2022 15:14:28 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e647346313038e022d4394703013d0963bc45ad0782bcf984166dd279d475c5d`  
		Last Modified: Wed, 12 Jan 2022 15:14:27 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fb56fc761a44bdcdde0f2cfaa2a75932b2ac8fe3c78177727284b0f58037fb0`  
		Last Modified: Wed, 12 Jan 2022 15:14:28 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5797262702f20651c9e1f79f4fbfbe22a260dc9bb7408bf5820eb186b3063f4d`  
		Last Modified: Wed, 12 Jan 2022 15:14:27 GMT  
		Size: 338.2 KB (338250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24cad06e122fd976b54af5acb5a3ba1d1299d61be733e7c2eadeb185aca82942`  
		Last Modified: Wed, 12 Jan 2022 15:14:31 GMT  
		Size: 5.0 MB (4954480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:886cf217b75c847a9ef63c4cc6093d9aa9c783f67b2c999fb7b23249e80b6e6c`  
		Last Modified: Wed, 12 Jan 2022 15:14:25 GMT  
		Size: 1.9 KB (1941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f1f92fb92be2d3b29fc1f42015a4d47bb112ae53db5fab9fa63f432838b7747`  
		Last Modified: Wed, 12 Jan 2022 15:14:25 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:099a82c04f8e6eee73daaccc93d0ad74009ffb4c94eb7d9c8a6a52b4e6bdf2fd`  
		Last Modified: Wed, 12 Jan 2022 15:14:25 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:507bd2ef766612deffd70102b577c1242165b07a8464313f8454713360560c86`  
		Last Modified: Wed, 12 Jan 2022 15:14:25 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-windowsservercore` - windows version 10.0.14393.4886; amd64

```console
$ docker pull nats@sha256:e476d11dde611fc9b39eb6a45798c2e503fa1bfa4ece59509826bfaed6a4cbe1
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6283541821 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:084594550a22f2aa624e5b2e740a29366a6846c2e1f194854e6e32270f5f0edb`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Thu, 06 Jan 2022 14:33:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 11 Jan 2022 19:57:39 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Tue, 11 Jan 2022 19:57:40 GMT
ENV NATS_DOCKERIZED=1
# Tue, 11 Jan 2022 21:15:53 GMT
ENV NATS_SERVER=2.6.6
# Tue, 11 Jan 2022 21:15:55 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.6.6/nats-server-v2.6.6-windows-amd64.zip
# Tue, 11 Jan 2022 21:15:56 GMT
ENV NATS_SERVER_SHASUM=9730ea401beed7ac40aeada0a8dccfb70207bb234202035aad5644e93ec657da
# Tue, 11 Jan 2022 21:16:48 GMT
RUN Set-PSDebug -Trace 2
# Tue, 11 Jan 2022 21:18:24 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Tue, 11 Jan 2022 21:18:25 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Tue, 11 Jan 2022 21:18:26 GMT
EXPOSE 4222 6222 8222
# Tue, 11 Jan 2022 21:18:28 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 11 Jan 2022 21:18:29 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8428508ffd63b4af1ba690ec41e82a116f10ec6c3fb70962348f5448d42e5835`  
		Size: 2.2 GB (2208216859 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:25aec0a6b64c784bf7521344203ee5def4d38eedfdd68f4b452d3250b5b9ddcf`  
		Last Modified: Tue, 11 Jan 2022 21:19:46 GMT  
		Size: 1.3 KB (1327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3fffdd310a93f98578e45ffbf8e22c031b37efefcc042f21d2a63c2a77c4ee3`  
		Last Modified: Tue, 11 Jan 2022 21:19:45 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15052497c858a1a8b4a8159d05850fbf43551aad161e61ae0fd6880c46eb4556`  
		Last Modified: Tue, 11 Jan 2022 21:19:44 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:080911a4b1ac40e1f062d68ed70319860e88ecb9abec2aef41d0bc3bae89098d`  
		Last Modified: Tue, 11 Jan 2022 21:19:44 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e79cea19a92f33c59acbcc8f501e9acdb5985bbad5b03ccd1190848ae1b4cf1`  
		Last Modified: Tue, 11 Jan 2022 21:19:44 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae0544e04ecd7b6afc6366924310fd892736faf1983ea2ee9e40efd31a0ec502`  
		Last Modified: Tue, 11 Jan 2022 21:19:44 GMT  
		Size: 337.0 KB (337010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8906d4ca25b04680081cc6af81b8eec86a9756abb72e21ed2785f82372ba7c58`  
		Last Modified: Tue, 11 Jan 2022 21:19:43 GMT  
		Size: 5.0 MB (4988964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99a01b43c4c8c06f528a3080b9f4d396d196ff851a603ac22c9ce560c3d5b082`  
		Last Modified: Tue, 11 Jan 2022 21:19:42 GMT  
		Size: 2.0 KB (1973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e156e4bebcfed633295afa0f9dacd6146736cb7de973581f01931fdf6d5f5ae`  
		Last Modified: Tue, 11 Jan 2022 21:19:41 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf3ee9fcf4be90533587d2a54238465fc8f6bad0744784041f675b2e97a93bb9`  
		Last Modified: Tue, 11 Jan 2022 21:19:42 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6e44c694323da6f62bebd7b52b659731c89b1e15c15e5c345ec43e24cba28f7`  
		Last Modified: Tue, 11 Jan 2022 21:19:41 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-windowsservercore-1809`

```console
$ docker pull nats@sha256:688fa8edbb0b5931af887d0ab00ed77da3f9e8505225dc1eccf15672638fd7a7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2452; amd64

### `nats:2-windowsservercore-1809` - windows version 10.0.17763.2452; amd64

```console
$ docker pull nats@sha256:7f3bfcdbda90968d69223b48664ee1ec937a82bce7365c82135785fe353ba699
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2717536770 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4622435affd612664c15aa4fd83b1e45ba56de92d3c7e6dd3dd924adf28111bf`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 07 Jan 2022 22:48:13 GMT
RUN Install update 1809-amd64
# Wed, 12 Jan 2022 13:54:17 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 Jan 2022 15:10:29 GMT
ENV NATS_DOCKERIZED=1
# Wed, 12 Jan 2022 15:10:30 GMT
ENV NATS_SERVER=2.6.6
# Wed, 12 Jan 2022 15:10:32 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.6.6/nats-server-v2.6.6-windows-amd64.zip
# Wed, 12 Jan 2022 15:10:33 GMT
ENV NATS_SERVER_SHASUM=9730ea401beed7ac40aeada0a8dccfb70207bb234202035aad5644e93ec657da
# Wed, 12 Jan 2022 15:11:32 GMT
RUN Set-PSDebug -Trace 2
# Wed, 12 Jan 2022 15:13:24 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 12 Jan 2022 15:13:26 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 12 Jan 2022 15:13:27 GMT
EXPOSE 4222 6222 8222
# Wed, 12 Jan 2022 15:13:28 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 12 Jan 2022 15:13:29 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:635f15ebd5b486e8a00bf217a0574a29550e5bbf08c1d021e1e308100b2e49b5`  
		Size: 993.9 MB (993898043 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:537828534783cff318d36854dbda0683aef7263e437c7c669de4092e1778959c`  
		Last Modified: Wed, 12 Jan 2022 15:14:30 GMT  
		Size: 1.3 KB (1296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9576e7772519d67febb0ceb94d8f22531ea99f0c60c36e67a4f5a497c384f5e0`  
		Last Modified: Wed, 12 Jan 2022 15:14:30 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaf1f761c394ef0da3c3fef1865f52e977d392f3f0b6c0575c3d1341da6cd7e9`  
		Last Modified: Wed, 12 Jan 2022 15:14:28 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e647346313038e022d4394703013d0963bc45ad0782bcf984166dd279d475c5d`  
		Last Modified: Wed, 12 Jan 2022 15:14:27 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fb56fc761a44bdcdde0f2cfaa2a75932b2ac8fe3c78177727284b0f58037fb0`  
		Last Modified: Wed, 12 Jan 2022 15:14:28 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5797262702f20651c9e1f79f4fbfbe22a260dc9bb7408bf5820eb186b3063f4d`  
		Last Modified: Wed, 12 Jan 2022 15:14:27 GMT  
		Size: 338.2 KB (338250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24cad06e122fd976b54af5acb5a3ba1d1299d61be733e7c2eadeb185aca82942`  
		Last Modified: Wed, 12 Jan 2022 15:14:31 GMT  
		Size: 5.0 MB (4954480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:886cf217b75c847a9ef63c4cc6093d9aa9c783f67b2c999fb7b23249e80b6e6c`  
		Last Modified: Wed, 12 Jan 2022 15:14:25 GMT  
		Size: 1.9 KB (1941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f1f92fb92be2d3b29fc1f42015a4d47bb112ae53db5fab9fa63f432838b7747`  
		Last Modified: Wed, 12 Jan 2022 15:14:25 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:099a82c04f8e6eee73daaccc93d0ad74009ffb4c94eb7d9c8a6a52b4e6bdf2fd`  
		Last Modified: Wed, 12 Jan 2022 15:14:25 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:507bd2ef766612deffd70102b577c1242165b07a8464313f8454713360560c86`  
		Last Modified: Wed, 12 Jan 2022 15:14:25 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-windowsservercore-ltsc2016`

```console
$ docker pull nats@sha256:3d337d85e45c503e13f57109f85de0e1c916fc6781cf7bbd3f40ccffd0fb664b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.14393.4886; amd64

### `nats:2-windowsservercore-ltsc2016` - windows version 10.0.14393.4886; amd64

```console
$ docker pull nats@sha256:e476d11dde611fc9b39eb6a45798c2e503fa1bfa4ece59509826bfaed6a4cbe1
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6283541821 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:084594550a22f2aa624e5b2e740a29366a6846c2e1f194854e6e32270f5f0edb`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Thu, 06 Jan 2022 14:33:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 11 Jan 2022 19:57:39 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Tue, 11 Jan 2022 19:57:40 GMT
ENV NATS_DOCKERIZED=1
# Tue, 11 Jan 2022 21:15:53 GMT
ENV NATS_SERVER=2.6.6
# Tue, 11 Jan 2022 21:15:55 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.6.6/nats-server-v2.6.6-windows-amd64.zip
# Tue, 11 Jan 2022 21:15:56 GMT
ENV NATS_SERVER_SHASUM=9730ea401beed7ac40aeada0a8dccfb70207bb234202035aad5644e93ec657da
# Tue, 11 Jan 2022 21:16:48 GMT
RUN Set-PSDebug -Trace 2
# Tue, 11 Jan 2022 21:18:24 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Tue, 11 Jan 2022 21:18:25 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Tue, 11 Jan 2022 21:18:26 GMT
EXPOSE 4222 6222 8222
# Tue, 11 Jan 2022 21:18:28 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 11 Jan 2022 21:18:29 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8428508ffd63b4af1ba690ec41e82a116f10ec6c3fb70962348f5448d42e5835`  
		Size: 2.2 GB (2208216859 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:25aec0a6b64c784bf7521344203ee5def4d38eedfdd68f4b452d3250b5b9ddcf`  
		Last Modified: Tue, 11 Jan 2022 21:19:46 GMT  
		Size: 1.3 KB (1327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3fffdd310a93f98578e45ffbf8e22c031b37efefcc042f21d2a63c2a77c4ee3`  
		Last Modified: Tue, 11 Jan 2022 21:19:45 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15052497c858a1a8b4a8159d05850fbf43551aad161e61ae0fd6880c46eb4556`  
		Last Modified: Tue, 11 Jan 2022 21:19:44 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:080911a4b1ac40e1f062d68ed70319860e88ecb9abec2aef41d0bc3bae89098d`  
		Last Modified: Tue, 11 Jan 2022 21:19:44 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e79cea19a92f33c59acbcc8f501e9acdb5985bbad5b03ccd1190848ae1b4cf1`  
		Last Modified: Tue, 11 Jan 2022 21:19:44 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae0544e04ecd7b6afc6366924310fd892736faf1983ea2ee9e40efd31a0ec502`  
		Last Modified: Tue, 11 Jan 2022 21:19:44 GMT  
		Size: 337.0 KB (337010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8906d4ca25b04680081cc6af81b8eec86a9756abb72e21ed2785f82372ba7c58`  
		Last Modified: Tue, 11 Jan 2022 21:19:43 GMT  
		Size: 5.0 MB (4988964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99a01b43c4c8c06f528a3080b9f4d396d196ff851a603ac22c9ce560c3d5b082`  
		Last Modified: Tue, 11 Jan 2022 21:19:42 GMT  
		Size: 2.0 KB (1973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e156e4bebcfed633295afa0f9dacd6146736cb7de973581f01931fdf6d5f5ae`  
		Last Modified: Tue, 11 Jan 2022 21:19:41 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf3ee9fcf4be90533587d2a54238465fc8f6bad0744784041f675b2e97a93bb9`  
		Last Modified: Tue, 11 Jan 2022 21:19:42 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6e44c694323da6f62bebd7b52b659731c89b1e15c15e5c345ec43e24cba28f7`  
		Last Modified: Tue, 11 Jan 2022 21:19:41 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.6`

```console
$ docker pull nats@sha256:9bd747193a9d316341136227475dbde257fe33d6209b7b43beaf16ae0a358865
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.2452; amd64

### `nats:2.6` - linux; amd64

```console
$ docker pull nats@sha256:dad4f69520337c2a80d2a9123963c971836f07f530cf4b7c56dde98a622e0a6b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4578170 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ba73da93bdda8525a9f473851ee3de9a2d23c21e1d0a51d7da118bc122df420`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 03 Dec 2021 21:23:03 GMT
COPY file:4070919cac43aa01e3ef5dd95589f24a9d649dcc7b4d6364927c764b1f90392e in /nats-server 
# Fri, 03 Dec 2021 21:23:04 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 03 Dec 2021 21:23:04 GMT
EXPOSE 4222 6222 8222
# Fri, 03 Dec 2021 21:23:04 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 03 Dec 2021 21:23:04 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:730cae3de796bb1fbb06f0f847317c2b738bf9af9d1233daafcf2f708eade5ec`  
		Last Modified: Fri, 03 Dec 2021 21:24:01 GMT  
		Size: 4.6 MB (4577696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39027e71725d02ee81938943fd0f3e980f01abbe21c5e8f8ea8219687aaae862`  
		Last Modified: Fri, 03 Dec 2021 21:24:00 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.6` - linux; arm variant v6

```console
$ docker pull nats@sha256:54395301fd2f315191df081131cd6d142613d057970268d64480f4706bcaeda3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4241317 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c4851d5f7b19bc49c52879a43236bae3e26e03a8a0f035ec150eed9a723cca5`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 02 Dec 2021 22:50:02 GMT
COPY file:6036f30fae4132d78e941219bf965a4e4c3e6d898ac912ab22e7a0cc98adf5a5 in /nats-server 
# Thu, 02 Dec 2021 22:50:03 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 02 Dec 2021 22:50:03 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Dec 2021 22:50:04 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 02 Dec 2021 22:50:04 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:41ef8f0f5e4d1f0e1880325ac8c2ccde63d323e6ead77b97c1225e0ce1d226ce`  
		Last Modified: Thu, 02 Dec 2021 22:52:29 GMT  
		Size: 4.2 MB (4240841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e8f034153e28423592a04f327fe3b69d3d84721cb54631e3ea9dcae375ab0ef`  
		Last Modified: Thu, 02 Dec 2021 22:52:26 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.6` - linux; arm variant v7

```console
$ docker pull nats@sha256:78ee1d57413d89c46e808dbb121ad895537b74af783c6e6189366afa07638b66
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4237689 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b3276dd6f6de73a2af8ca0c6bd2dc88c7f7ae0a0ce334bcae39c14047aab540`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 04 Dec 2021 07:52:28 GMT
COPY file:025e99b21a301a69c768cc2c72e67c371165b6314d59d0a5a95958216fd24eac in /nats-server 
# Sat, 04 Dec 2021 07:52:28 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Sat, 04 Dec 2021 07:52:29 GMT
EXPOSE 4222 6222 8222
# Sat, 04 Dec 2021 07:52:29 GMT
ENTRYPOINT ["/nats-server"]
# Sat, 04 Dec 2021 07:52:30 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:75a8e365d6e58c8d8f7fe944a206f76f3e800542aca1b53e849c4bffc78fd22d`  
		Last Modified: Sat, 04 Dec 2021 07:55:01 GMT  
		Size: 4.2 MB (4237211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc2920e0912e6a42ee2fd0b7b8b31c6cca01c6c99f16c760f904492422ff7cae`  
		Last Modified: Sat, 04 Dec 2021 07:54:58 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.6` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:8ecffb2097f683980b94450d536a99c79b3fe7654f8bc91fd1c45ad0825e6aae
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4189764 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90bb404fba49386fc48ceb05ee04604d317ff225da69f159d0bd4cc63a930c0e`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 03 Dec 2021 16:57:31 GMT
COPY file:b5f62686ba6debf89a42d2be7c4442db5f8735dba6b8932e6f01f315a2e63e27 in /nats-server 
# Fri, 03 Dec 2021 16:57:32 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 03 Dec 2021 16:57:32 GMT
EXPOSE 4222 6222 8222
# Fri, 03 Dec 2021 16:57:33 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 03 Dec 2021 16:57:34 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:44ff62bde832e2b2bca85708fd2fc86d7d6d1f4ca7c58b5d0e18e3d07c9c5bac`  
		Last Modified: Fri, 03 Dec 2021 16:58:50 GMT  
		Size: 4.2 MB (4189288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44dcbc70566b6f8312605c0214812444ccad7a55594fa2e7f0792c21af818ef0`  
		Last Modified: Fri, 03 Dec 2021 16:58:49 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.6` - windows version 10.0.17763.2452; amd64

```console
$ docker pull nats@sha256:73596edd7d2bcfb546b2b6da26cbaf06733398e7cc550a610ed8e53c5c59021c
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.7 MB (107674705 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa5c572d20b69e54dca9ee7a24b26d6b489d4cd2be1d5931d9accce1dbb7e030`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 07 Jan 2022 22:25:06 GMT
RUN Apply image 1809-amd64
# Wed, 12 Jan 2022 15:13:42 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 12 Jan 2022 15:13:43 GMT
RUN cmd /S /C #(nop) COPY file:20c797e6dad00d7098dbf6d4d158c380fd073bc5fc24a80fd4f23205af77a338 in C:\nats-server.exe 
# Wed, 12 Jan 2022 15:13:44 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 12 Jan 2022 15:13:45 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 12 Jan 2022 15:13:46 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 12 Jan 2022 15:13:47 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3a78847ea829208edc2d7b320b7e602b9d12e47689499d5180a9cc7790dec4d7`  
		Size: 103.0 MB (103031066 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:db05d2e76671d91772a070867bf6f050343319070602a0f8239706d5d4d98387`  
		Last Modified: Wed, 12 Jan 2022 15:14:49 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6271ae84b48476b5c259495509975bd53d7f398555179642c1ef1d612099cb19`  
		Last Modified: Wed, 12 Jan 2022 15:14:48 GMT  
		Size: 4.6 MB (4637258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:178ab94841651126bd3f8a1478a504e44f389c2bf5abf59abafc16f163108f4c`  
		Last Modified: Wed, 12 Jan 2022 15:14:46 GMT  
		Size: 1.8 KB (1759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aa2ac290e2024e6f26c6fd076cc312a10b4842536f9c9daad8ac0e5ecced071`  
		Last Modified: Wed, 12 Jan 2022 15:14:46 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8cb0f84aeae0a7ea0020f00dd7b55f02b772c0bfaa74ea61e1fbd266eff8928`  
		Last Modified: Wed, 12 Jan 2022 15:14:46 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7238bcc9c911d52c987ca07602cb3204bf985a35ae993830fe3b54ea9563de43`  
		Last Modified: Wed, 12 Jan 2022 15:14:46 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.6-alpine`

```console
$ docker pull nats@sha256:8e2e34eb798631cd76f341277f529f78618a2366d81b59586d3b81f6cb839b25
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.6-alpine` - linux; amd64

```console
$ docker pull nats@sha256:687f39ecdab1eeda8a4eaa7b7210586d96698faa5e5e7e47aaf5ef8084d504e5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.7 MB (7689543 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c5dc2cfb512e016e62911eca35c050a2eb5ca4b783d5f2d413ba64c68c420bd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:44 GMT
ADD file:762c899ec0505d1a32930ee804c5b008825f41611161be104076cba33b7e5b2b in / 
# Fri, 12 Nov 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 03 Dec 2021 21:22:18 GMT
ENV NATS_SERVER=2.6.6
# Fri, 03 Dec 2021 21:22:21 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='70da0ad3694aebfc742f9aae919d3a4aa5b8c863946e99c5d332195fbbdad49c' ;; 		armhf) natsArch='arm6'; sha256='e2cc1e198d5d5c83e2f2c2dcb15fafb71601603e3740065682812afaa7dd443a' ;; 		armv7) natsArch='arm7'; sha256='f3698a4fb18c6664d477b920d5f07637141a6623cf2fa998900155fea0d97e61' ;; 		x86_64) natsArch='amd64'; sha256='2c2fc16322fb2bc0b166ee2a01e163d4beb2cf7b49d083cebcd36695dc05a381' ;; 		x86) natsArch='386'; sha256='1da03b0d163dc98209f010bf6efa5fc6c81a23b4bab7a98bebe142e19fc26bdc' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 03 Dec 2021 21:22:21 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 03 Dec 2021 21:22:22 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 03 Dec 2021 21:22:22 GMT
EXPOSE 4222 6222 8222
# Fri, 03 Dec 2021 21:22:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 03 Dec 2021 21:22:22 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:97518928ae5f3d52d4164b314a7e73654eb686ecd8aafa0b79acd980773a740d`  
		Last Modified: Fri, 12 Nov 2021 17:20:39 GMT  
		Size: 2.8 MB (2822981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daeb19d8d614f4a1df58ed04d3c72469fa9f7286c9d5482ee274405723b5e645`  
		Last Modified: Fri, 03 Dec 2021 21:23:37 GMT  
		Size: 4.9 MB (4865593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e51c3679390c1ab0c5f5e6786505ad9278d45683059fc7fac0298dcbb6dede86`  
		Last Modified: Fri, 03 Dec 2021 21:23:36 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b14f15cf01b25470e7340acc8ca0860eb4a00a7e1b5d5180bd7c23db1dd273af`  
		Last Modified: Fri, 03 Dec 2021 21:23:36 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.6-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:d42d25248435c99492dd0fbcd97688486c692c680069bc9a1eb8a7b1c85eebff
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7161537 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ae84a8c7e689bc4d7fd2915ef9aaf1fb624c094cb183af5863d4b20984f29cd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 12 Nov 2021 16:49:42 GMT
ADD file:6daf1fe862c00673bf9cf4d7e20b0bf253a56e7fb8ed5e730a4466ab9186e18a in / 
# Fri, 12 Nov 2021 16:49:44 GMT
CMD ["/bin/sh"]
# Thu, 02 Dec 2021 22:49:35 GMT
ENV NATS_SERVER=2.6.6
# Thu, 02 Dec 2021 22:49:39 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='70da0ad3694aebfc742f9aae919d3a4aa5b8c863946e99c5d332195fbbdad49c' ;; 		armhf) natsArch='arm6'; sha256='e2cc1e198d5d5c83e2f2c2dcb15fafb71601603e3740065682812afaa7dd443a' ;; 		armv7) natsArch='arm7'; sha256='f3698a4fb18c6664d477b920d5f07637141a6623cf2fa998900155fea0d97e61' ;; 		x86_64) natsArch='amd64'; sha256='2c2fc16322fb2bc0b166ee2a01e163d4beb2cf7b49d083cebcd36695dc05a381' ;; 		x86) natsArch='386'; sha256='1da03b0d163dc98209f010bf6efa5fc6c81a23b4bab7a98bebe142e19fc26bdc' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 02 Dec 2021 22:49:40 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 02 Dec 2021 22:49:40 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 02 Dec 2021 22:49:41 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Dec 2021 22:49:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 02 Dec 2021 22:49:42 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:56afcfda5d78cc243287acbaad250c5e8c0f47aae620dd7c51985b0d3c9b2728`  
		Last Modified: Fri, 12 Nov 2021 16:51:32 GMT  
		Size: 2.6 MB (2635392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3c7b89c441a056fc0e4d867cd4fd28308f188bd0f6b306e5feee96fee47cbdf`  
		Last Modified: Thu, 02 Dec 2021 22:51:52 GMT  
		Size: 4.5 MB (4525169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f67a5f3b97f233f2d6d30a90acd85b9e856cb9b98c298b71e2b5cbae3e0268cf`  
		Last Modified: Thu, 02 Dec 2021 22:51:50 GMT  
		Size: 561.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:706486ffe19b237b40203ebf10cb1110d7566cba5a3c10bf738be70173a1aa69`  
		Last Modified: Thu, 02 Dec 2021 22:51:50 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.6-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:dbc345345cfc225bd88b35e80f85f412483db712134bde3a0e4d959cb543350f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.0 MB (6958146 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6aaa47180fd5390c3f39b81e39db30c26897fc1b070c064d4677ebdd14c1f801`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 12 Nov 2021 16:57:35 GMT
ADD file:03e0720458c3475758bf4394afa56f2165198eb91e6e9581f7768e433744dd9b in / 
# Fri, 12 Nov 2021 16:57:36 GMT
CMD ["/bin/sh"]
# Sat, 04 Dec 2021 07:51:50 GMT
ENV NATS_SERVER=2.6.6
# Sat, 04 Dec 2021 07:51:54 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='70da0ad3694aebfc742f9aae919d3a4aa5b8c863946e99c5d332195fbbdad49c' ;; 		armhf) natsArch='arm6'; sha256='e2cc1e198d5d5c83e2f2c2dcb15fafb71601603e3740065682812afaa7dd443a' ;; 		armv7) natsArch='arm7'; sha256='f3698a4fb18c6664d477b920d5f07637141a6623cf2fa998900155fea0d97e61' ;; 		x86_64) natsArch='amd64'; sha256='2c2fc16322fb2bc0b166ee2a01e163d4beb2cf7b49d083cebcd36695dc05a381' ;; 		x86) natsArch='386'; sha256='1da03b0d163dc98209f010bf6efa5fc6c81a23b4bab7a98bebe142e19fc26bdc' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Sat, 04 Dec 2021 07:51:55 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Sat, 04 Dec 2021 07:51:55 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Sat, 04 Dec 2021 07:51:56 GMT
EXPOSE 4222 6222 8222
# Sat, 04 Dec 2021 07:51:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 04 Dec 2021 07:51:57 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:764d2e53e1a607f2d8261522185d5b9021ade3ec1a595664ee90308c00176899`  
		Last Modified: Fri, 12 Nov 2021 16:59:33 GMT  
		Size: 2.4 MB (2438618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:157eac698795baeacb3153cf2bbbc17f348e477e8062fa45b6728e97dd02e157`  
		Last Modified: Sat, 04 Dec 2021 07:54:19 GMT  
		Size: 4.5 MB (4518555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b5241fcba964a14f9c4681ebcc94815a476df86f68c628494f5759a3bee8514`  
		Last Modified: Sat, 04 Dec 2021 07:54:16 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36d02df08ee2f75a857120c105153a83b2b951337a87e902260e70e1de20dfd0`  
		Last Modified: Sat, 04 Dec 2021 07:54:16 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.6-alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:f1e7262504ed73a185ee16f6a6da14c19c3a76120f2b22c51a051a0988ac3bdc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7193478 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55e483df89c189235b79aa4a9d2417378172236dba6fa85f6d5a0bb35756835f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 12 Nov 2021 16:39:58 GMT
ADD file:400c0466b29ccad54e0f6c0acef22542992828678c96693ef1f9f4d0551935d8 in / 
# Fri, 12 Nov 2021 16:39:58 GMT
CMD ["/bin/sh"]
# Fri, 03 Dec 2021 16:57:10 GMT
ENV NATS_SERVER=2.6.6
# Fri, 03 Dec 2021 16:57:13 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='70da0ad3694aebfc742f9aae919d3a4aa5b8c863946e99c5d332195fbbdad49c' ;; 		armhf) natsArch='arm6'; sha256='e2cc1e198d5d5c83e2f2c2dcb15fafb71601603e3740065682812afaa7dd443a' ;; 		armv7) natsArch='arm7'; sha256='f3698a4fb18c6664d477b920d5f07637141a6623cf2fa998900155fea0d97e61' ;; 		x86_64) natsArch='amd64'; sha256='2c2fc16322fb2bc0b166ee2a01e163d4beb2cf7b49d083cebcd36695dc05a381' ;; 		x86) natsArch='386'; sha256='1da03b0d163dc98209f010bf6efa5fc6c81a23b4bab7a98bebe142e19fc26bdc' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 03 Dec 2021 16:57:15 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 03 Dec 2021 16:57:16 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 03 Dec 2021 16:57:16 GMT
EXPOSE 4222 6222 8222
# Fri, 03 Dec 2021 16:57:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 03 Dec 2021 16:57:18 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:be307f383ecc62b27a29b599c3fc9d3129693a798e7fcce614f09174cfe2d354`  
		Last Modified: Fri, 12 Nov 2021 16:40:59 GMT  
		Size: 2.7 MB (2717700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdee3b2a5421d3ceb50b8101857ce4c0815c4532476e1f292867c63034c08f61`  
		Last Modified: Fri, 03 Dec 2021 16:58:22 GMT  
		Size: 4.5 MB (4474835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8a771880289bb86cd368ca8b39620b0cfe69694646e061ff6975f959ccfcd29`  
		Last Modified: Fri, 03 Dec 2021 16:58:21 GMT  
		Size: 528.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:438c5abdffd6599ac83fe661d26a9491552d63f48aeb9147609299ee11b78c78`  
		Last Modified: Fri, 03 Dec 2021 16:58:21 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.6-alpine3.14`

```console
$ docker pull nats@sha256:8e2e34eb798631cd76f341277f529f78618a2366d81b59586d3b81f6cb839b25
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.6-alpine3.14` - linux; amd64

```console
$ docker pull nats@sha256:687f39ecdab1eeda8a4eaa7b7210586d96698faa5e5e7e47aaf5ef8084d504e5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.7 MB (7689543 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c5dc2cfb512e016e62911eca35c050a2eb5ca4b783d5f2d413ba64c68c420bd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:44 GMT
ADD file:762c899ec0505d1a32930ee804c5b008825f41611161be104076cba33b7e5b2b in / 
# Fri, 12 Nov 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 03 Dec 2021 21:22:18 GMT
ENV NATS_SERVER=2.6.6
# Fri, 03 Dec 2021 21:22:21 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='70da0ad3694aebfc742f9aae919d3a4aa5b8c863946e99c5d332195fbbdad49c' ;; 		armhf) natsArch='arm6'; sha256='e2cc1e198d5d5c83e2f2c2dcb15fafb71601603e3740065682812afaa7dd443a' ;; 		armv7) natsArch='arm7'; sha256='f3698a4fb18c6664d477b920d5f07637141a6623cf2fa998900155fea0d97e61' ;; 		x86_64) natsArch='amd64'; sha256='2c2fc16322fb2bc0b166ee2a01e163d4beb2cf7b49d083cebcd36695dc05a381' ;; 		x86) natsArch='386'; sha256='1da03b0d163dc98209f010bf6efa5fc6c81a23b4bab7a98bebe142e19fc26bdc' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 03 Dec 2021 21:22:21 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 03 Dec 2021 21:22:22 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 03 Dec 2021 21:22:22 GMT
EXPOSE 4222 6222 8222
# Fri, 03 Dec 2021 21:22:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 03 Dec 2021 21:22:22 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:97518928ae5f3d52d4164b314a7e73654eb686ecd8aafa0b79acd980773a740d`  
		Last Modified: Fri, 12 Nov 2021 17:20:39 GMT  
		Size: 2.8 MB (2822981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daeb19d8d614f4a1df58ed04d3c72469fa9f7286c9d5482ee274405723b5e645`  
		Last Modified: Fri, 03 Dec 2021 21:23:37 GMT  
		Size: 4.9 MB (4865593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e51c3679390c1ab0c5f5e6786505ad9278d45683059fc7fac0298dcbb6dede86`  
		Last Modified: Fri, 03 Dec 2021 21:23:36 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b14f15cf01b25470e7340acc8ca0860eb4a00a7e1b5d5180bd7c23db1dd273af`  
		Last Modified: Fri, 03 Dec 2021 21:23:36 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.6-alpine3.14` - linux; arm variant v6

```console
$ docker pull nats@sha256:d42d25248435c99492dd0fbcd97688486c692c680069bc9a1eb8a7b1c85eebff
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7161537 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ae84a8c7e689bc4d7fd2915ef9aaf1fb624c094cb183af5863d4b20984f29cd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 12 Nov 2021 16:49:42 GMT
ADD file:6daf1fe862c00673bf9cf4d7e20b0bf253a56e7fb8ed5e730a4466ab9186e18a in / 
# Fri, 12 Nov 2021 16:49:44 GMT
CMD ["/bin/sh"]
# Thu, 02 Dec 2021 22:49:35 GMT
ENV NATS_SERVER=2.6.6
# Thu, 02 Dec 2021 22:49:39 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='70da0ad3694aebfc742f9aae919d3a4aa5b8c863946e99c5d332195fbbdad49c' ;; 		armhf) natsArch='arm6'; sha256='e2cc1e198d5d5c83e2f2c2dcb15fafb71601603e3740065682812afaa7dd443a' ;; 		armv7) natsArch='arm7'; sha256='f3698a4fb18c6664d477b920d5f07637141a6623cf2fa998900155fea0d97e61' ;; 		x86_64) natsArch='amd64'; sha256='2c2fc16322fb2bc0b166ee2a01e163d4beb2cf7b49d083cebcd36695dc05a381' ;; 		x86) natsArch='386'; sha256='1da03b0d163dc98209f010bf6efa5fc6c81a23b4bab7a98bebe142e19fc26bdc' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 02 Dec 2021 22:49:40 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 02 Dec 2021 22:49:40 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 02 Dec 2021 22:49:41 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Dec 2021 22:49:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 02 Dec 2021 22:49:42 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:56afcfda5d78cc243287acbaad250c5e8c0f47aae620dd7c51985b0d3c9b2728`  
		Last Modified: Fri, 12 Nov 2021 16:51:32 GMT  
		Size: 2.6 MB (2635392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3c7b89c441a056fc0e4d867cd4fd28308f188bd0f6b306e5feee96fee47cbdf`  
		Last Modified: Thu, 02 Dec 2021 22:51:52 GMT  
		Size: 4.5 MB (4525169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f67a5f3b97f233f2d6d30a90acd85b9e856cb9b98c298b71e2b5cbae3e0268cf`  
		Last Modified: Thu, 02 Dec 2021 22:51:50 GMT  
		Size: 561.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:706486ffe19b237b40203ebf10cb1110d7566cba5a3c10bf738be70173a1aa69`  
		Last Modified: Thu, 02 Dec 2021 22:51:50 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.6-alpine3.14` - linux; arm variant v7

```console
$ docker pull nats@sha256:dbc345345cfc225bd88b35e80f85f412483db712134bde3a0e4d959cb543350f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.0 MB (6958146 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6aaa47180fd5390c3f39b81e39db30c26897fc1b070c064d4677ebdd14c1f801`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 12 Nov 2021 16:57:35 GMT
ADD file:03e0720458c3475758bf4394afa56f2165198eb91e6e9581f7768e433744dd9b in / 
# Fri, 12 Nov 2021 16:57:36 GMT
CMD ["/bin/sh"]
# Sat, 04 Dec 2021 07:51:50 GMT
ENV NATS_SERVER=2.6.6
# Sat, 04 Dec 2021 07:51:54 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='70da0ad3694aebfc742f9aae919d3a4aa5b8c863946e99c5d332195fbbdad49c' ;; 		armhf) natsArch='arm6'; sha256='e2cc1e198d5d5c83e2f2c2dcb15fafb71601603e3740065682812afaa7dd443a' ;; 		armv7) natsArch='arm7'; sha256='f3698a4fb18c6664d477b920d5f07637141a6623cf2fa998900155fea0d97e61' ;; 		x86_64) natsArch='amd64'; sha256='2c2fc16322fb2bc0b166ee2a01e163d4beb2cf7b49d083cebcd36695dc05a381' ;; 		x86) natsArch='386'; sha256='1da03b0d163dc98209f010bf6efa5fc6c81a23b4bab7a98bebe142e19fc26bdc' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Sat, 04 Dec 2021 07:51:55 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Sat, 04 Dec 2021 07:51:55 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Sat, 04 Dec 2021 07:51:56 GMT
EXPOSE 4222 6222 8222
# Sat, 04 Dec 2021 07:51:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 04 Dec 2021 07:51:57 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:764d2e53e1a607f2d8261522185d5b9021ade3ec1a595664ee90308c00176899`  
		Last Modified: Fri, 12 Nov 2021 16:59:33 GMT  
		Size: 2.4 MB (2438618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:157eac698795baeacb3153cf2bbbc17f348e477e8062fa45b6728e97dd02e157`  
		Last Modified: Sat, 04 Dec 2021 07:54:19 GMT  
		Size: 4.5 MB (4518555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b5241fcba964a14f9c4681ebcc94815a476df86f68c628494f5759a3bee8514`  
		Last Modified: Sat, 04 Dec 2021 07:54:16 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36d02df08ee2f75a857120c105153a83b2b951337a87e902260e70e1de20dfd0`  
		Last Modified: Sat, 04 Dec 2021 07:54:16 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.6-alpine3.14` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:f1e7262504ed73a185ee16f6a6da14c19c3a76120f2b22c51a051a0988ac3bdc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7193478 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55e483df89c189235b79aa4a9d2417378172236dba6fa85f6d5a0bb35756835f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 12 Nov 2021 16:39:58 GMT
ADD file:400c0466b29ccad54e0f6c0acef22542992828678c96693ef1f9f4d0551935d8 in / 
# Fri, 12 Nov 2021 16:39:58 GMT
CMD ["/bin/sh"]
# Fri, 03 Dec 2021 16:57:10 GMT
ENV NATS_SERVER=2.6.6
# Fri, 03 Dec 2021 16:57:13 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='70da0ad3694aebfc742f9aae919d3a4aa5b8c863946e99c5d332195fbbdad49c' ;; 		armhf) natsArch='arm6'; sha256='e2cc1e198d5d5c83e2f2c2dcb15fafb71601603e3740065682812afaa7dd443a' ;; 		armv7) natsArch='arm7'; sha256='f3698a4fb18c6664d477b920d5f07637141a6623cf2fa998900155fea0d97e61' ;; 		x86_64) natsArch='amd64'; sha256='2c2fc16322fb2bc0b166ee2a01e163d4beb2cf7b49d083cebcd36695dc05a381' ;; 		x86) natsArch='386'; sha256='1da03b0d163dc98209f010bf6efa5fc6c81a23b4bab7a98bebe142e19fc26bdc' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 03 Dec 2021 16:57:15 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 03 Dec 2021 16:57:16 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 03 Dec 2021 16:57:16 GMT
EXPOSE 4222 6222 8222
# Fri, 03 Dec 2021 16:57:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 03 Dec 2021 16:57:18 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:be307f383ecc62b27a29b599c3fc9d3129693a798e7fcce614f09174cfe2d354`  
		Last Modified: Fri, 12 Nov 2021 16:40:59 GMT  
		Size: 2.7 MB (2717700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdee3b2a5421d3ceb50b8101857ce4c0815c4532476e1f292867c63034c08f61`  
		Last Modified: Fri, 03 Dec 2021 16:58:22 GMT  
		Size: 4.5 MB (4474835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8a771880289bb86cd368ca8b39620b0cfe69694646e061ff6975f959ccfcd29`  
		Last Modified: Fri, 03 Dec 2021 16:58:21 GMT  
		Size: 528.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:438c5abdffd6599ac83fe661d26a9491552d63f48aeb9147609299ee11b78c78`  
		Last Modified: Fri, 03 Dec 2021 16:58:21 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.6-linux`

```console
$ docker pull nats@sha256:5d130fed2ad109f922a3a52e45c0b87c0d5a674ad432024cb3d45f898cf425b8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.6-linux` - linux; amd64

```console
$ docker pull nats@sha256:dad4f69520337c2a80d2a9123963c971836f07f530cf4b7c56dde98a622e0a6b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4578170 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ba73da93bdda8525a9f473851ee3de9a2d23c21e1d0a51d7da118bc122df420`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 03 Dec 2021 21:23:03 GMT
COPY file:4070919cac43aa01e3ef5dd95589f24a9d649dcc7b4d6364927c764b1f90392e in /nats-server 
# Fri, 03 Dec 2021 21:23:04 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 03 Dec 2021 21:23:04 GMT
EXPOSE 4222 6222 8222
# Fri, 03 Dec 2021 21:23:04 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 03 Dec 2021 21:23:04 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:730cae3de796bb1fbb06f0f847317c2b738bf9af9d1233daafcf2f708eade5ec`  
		Last Modified: Fri, 03 Dec 2021 21:24:01 GMT  
		Size: 4.6 MB (4577696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39027e71725d02ee81938943fd0f3e980f01abbe21c5e8f8ea8219687aaae862`  
		Last Modified: Fri, 03 Dec 2021 21:24:00 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.6-linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:54395301fd2f315191df081131cd6d142613d057970268d64480f4706bcaeda3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4241317 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c4851d5f7b19bc49c52879a43236bae3e26e03a8a0f035ec150eed9a723cca5`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 02 Dec 2021 22:50:02 GMT
COPY file:6036f30fae4132d78e941219bf965a4e4c3e6d898ac912ab22e7a0cc98adf5a5 in /nats-server 
# Thu, 02 Dec 2021 22:50:03 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 02 Dec 2021 22:50:03 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Dec 2021 22:50:04 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 02 Dec 2021 22:50:04 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:41ef8f0f5e4d1f0e1880325ac8c2ccde63d323e6ead77b97c1225e0ce1d226ce`  
		Last Modified: Thu, 02 Dec 2021 22:52:29 GMT  
		Size: 4.2 MB (4240841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e8f034153e28423592a04f327fe3b69d3d84721cb54631e3ea9dcae375ab0ef`  
		Last Modified: Thu, 02 Dec 2021 22:52:26 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.6-linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:78ee1d57413d89c46e808dbb121ad895537b74af783c6e6189366afa07638b66
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4237689 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b3276dd6f6de73a2af8ca0c6bd2dc88c7f7ae0a0ce334bcae39c14047aab540`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 04 Dec 2021 07:52:28 GMT
COPY file:025e99b21a301a69c768cc2c72e67c371165b6314d59d0a5a95958216fd24eac in /nats-server 
# Sat, 04 Dec 2021 07:52:28 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Sat, 04 Dec 2021 07:52:29 GMT
EXPOSE 4222 6222 8222
# Sat, 04 Dec 2021 07:52:29 GMT
ENTRYPOINT ["/nats-server"]
# Sat, 04 Dec 2021 07:52:30 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:75a8e365d6e58c8d8f7fe944a206f76f3e800542aca1b53e849c4bffc78fd22d`  
		Last Modified: Sat, 04 Dec 2021 07:55:01 GMT  
		Size: 4.2 MB (4237211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc2920e0912e6a42ee2fd0b7b8b31c6cca01c6c99f16c760f904492422ff7cae`  
		Last Modified: Sat, 04 Dec 2021 07:54:58 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.6-linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:8ecffb2097f683980b94450d536a99c79b3fe7654f8bc91fd1c45ad0825e6aae
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4189764 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90bb404fba49386fc48ceb05ee04604d317ff225da69f159d0bd4cc63a930c0e`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 03 Dec 2021 16:57:31 GMT
COPY file:b5f62686ba6debf89a42d2be7c4442db5f8735dba6b8932e6f01f315a2e63e27 in /nats-server 
# Fri, 03 Dec 2021 16:57:32 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 03 Dec 2021 16:57:32 GMT
EXPOSE 4222 6222 8222
# Fri, 03 Dec 2021 16:57:33 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 03 Dec 2021 16:57:34 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:44ff62bde832e2b2bca85708fd2fc86d7d6d1f4ca7c58b5d0e18e3d07c9c5bac`  
		Last Modified: Fri, 03 Dec 2021 16:58:50 GMT  
		Size: 4.2 MB (4189288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44dcbc70566b6f8312605c0214812444ccad7a55594fa2e7f0792c21af818ef0`  
		Last Modified: Fri, 03 Dec 2021 16:58:49 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.6-nanoserver`

```console
$ docker pull nats@sha256:0b2895172f1057f6c9b6bfeb7502714c3bfee379610222e16e17a226fc537354
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2452; amd64

### `nats:2.6-nanoserver` - windows version 10.0.17763.2452; amd64

```console
$ docker pull nats@sha256:73596edd7d2bcfb546b2b6da26cbaf06733398e7cc550a610ed8e53c5c59021c
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.7 MB (107674705 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa5c572d20b69e54dca9ee7a24b26d6b489d4cd2be1d5931d9accce1dbb7e030`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 07 Jan 2022 22:25:06 GMT
RUN Apply image 1809-amd64
# Wed, 12 Jan 2022 15:13:42 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 12 Jan 2022 15:13:43 GMT
RUN cmd /S /C #(nop) COPY file:20c797e6dad00d7098dbf6d4d158c380fd073bc5fc24a80fd4f23205af77a338 in C:\nats-server.exe 
# Wed, 12 Jan 2022 15:13:44 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 12 Jan 2022 15:13:45 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 12 Jan 2022 15:13:46 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 12 Jan 2022 15:13:47 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3a78847ea829208edc2d7b320b7e602b9d12e47689499d5180a9cc7790dec4d7`  
		Size: 103.0 MB (103031066 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:db05d2e76671d91772a070867bf6f050343319070602a0f8239706d5d4d98387`  
		Last Modified: Wed, 12 Jan 2022 15:14:49 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6271ae84b48476b5c259495509975bd53d7f398555179642c1ef1d612099cb19`  
		Last Modified: Wed, 12 Jan 2022 15:14:48 GMT  
		Size: 4.6 MB (4637258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:178ab94841651126bd3f8a1478a504e44f389c2bf5abf59abafc16f163108f4c`  
		Last Modified: Wed, 12 Jan 2022 15:14:46 GMT  
		Size: 1.8 KB (1759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aa2ac290e2024e6f26c6fd076cc312a10b4842536f9c9daad8ac0e5ecced071`  
		Last Modified: Wed, 12 Jan 2022 15:14:46 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8cb0f84aeae0a7ea0020f00dd7b55f02b772c0bfaa74ea61e1fbd266eff8928`  
		Last Modified: Wed, 12 Jan 2022 15:14:46 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7238bcc9c911d52c987ca07602cb3204bf985a35ae993830fe3b54ea9563de43`  
		Last Modified: Wed, 12 Jan 2022 15:14:46 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.6-nanoserver-1809`

```console
$ docker pull nats@sha256:0b2895172f1057f6c9b6bfeb7502714c3bfee379610222e16e17a226fc537354
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2452; amd64

### `nats:2.6-nanoserver-1809` - windows version 10.0.17763.2452; amd64

```console
$ docker pull nats@sha256:73596edd7d2bcfb546b2b6da26cbaf06733398e7cc550a610ed8e53c5c59021c
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.7 MB (107674705 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa5c572d20b69e54dca9ee7a24b26d6b489d4cd2be1d5931d9accce1dbb7e030`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 07 Jan 2022 22:25:06 GMT
RUN Apply image 1809-amd64
# Wed, 12 Jan 2022 15:13:42 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 12 Jan 2022 15:13:43 GMT
RUN cmd /S /C #(nop) COPY file:20c797e6dad00d7098dbf6d4d158c380fd073bc5fc24a80fd4f23205af77a338 in C:\nats-server.exe 
# Wed, 12 Jan 2022 15:13:44 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 12 Jan 2022 15:13:45 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 12 Jan 2022 15:13:46 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 12 Jan 2022 15:13:47 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3a78847ea829208edc2d7b320b7e602b9d12e47689499d5180a9cc7790dec4d7`  
		Size: 103.0 MB (103031066 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:db05d2e76671d91772a070867bf6f050343319070602a0f8239706d5d4d98387`  
		Last Modified: Wed, 12 Jan 2022 15:14:49 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6271ae84b48476b5c259495509975bd53d7f398555179642c1ef1d612099cb19`  
		Last Modified: Wed, 12 Jan 2022 15:14:48 GMT  
		Size: 4.6 MB (4637258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:178ab94841651126bd3f8a1478a504e44f389c2bf5abf59abafc16f163108f4c`  
		Last Modified: Wed, 12 Jan 2022 15:14:46 GMT  
		Size: 1.8 KB (1759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aa2ac290e2024e6f26c6fd076cc312a10b4842536f9c9daad8ac0e5ecced071`  
		Last Modified: Wed, 12 Jan 2022 15:14:46 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8cb0f84aeae0a7ea0020f00dd7b55f02b772c0bfaa74ea61e1fbd266eff8928`  
		Last Modified: Wed, 12 Jan 2022 15:14:46 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7238bcc9c911d52c987ca07602cb3204bf985a35ae993830fe3b54ea9563de43`  
		Last Modified: Wed, 12 Jan 2022 15:14:46 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.6-scratch`

```console
$ docker pull nats@sha256:5d130fed2ad109f922a3a52e45c0b87c0d5a674ad432024cb3d45f898cf425b8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.6-scratch` - linux; amd64

```console
$ docker pull nats@sha256:dad4f69520337c2a80d2a9123963c971836f07f530cf4b7c56dde98a622e0a6b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4578170 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ba73da93bdda8525a9f473851ee3de9a2d23c21e1d0a51d7da118bc122df420`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 03 Dec 2021 21:23:03 GMT
COPY file:4070919cac43aa01e3ef5dd95589f24a9d649dcc7b4d6364927c764b1f90392e in /nats-server 
# Fri, 03 Dec 2021 21:23:04 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 03 Dec 2021 21:23:04 GMT
EXPOSE 4222 6222 8222
# Fri, 03 Dec 2021 21:23:04 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 03 Dec 2021 21:23:04 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:730cae3de796bb1fbb06f0f847317c2b738bf9af9d1233daafcf2f708eade5ec`  
		Last Modified: Fri, 03 Dec 2021 21:24:01 GMT  
		Size: 4.6 MB (4577696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39027e71725d02ee81938943fd0f3e980f01abbe21c5e8f8ea8219687aaae862`  
		Last Modified: Fri, 03 Dec 2021 21:24:00 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.6-scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:54395301fd2f315191df081131cd6d142613d057970268d64480f4706bcaeda3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4241317 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c4851d5f7b19bc49c52879a43236bae3e26e03a8a0f035ec150eed9a723cca5`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 02 Dec 2021 22:50:02 GMT
COPY file:6036f30fae4132d78e941219bf965a4e4c3e6d898ac912ab22e7a0cc98adf5a5 in /nats-server 
# Thu, 02 Dec 2021 22:50:03 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 02 Dec 2021 22:50:03 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Dec 2021 22:50:04 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 02 Dec 2021 22:50:04 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:41ef8f0f5e4d1f0e1880325ac8c2ccde63d323e6ead77b97c1225e0ce1d226ce`  
		Last Modified: Thu, 02 Dec 2021 22:52:29 GMT  
		Size: 4.2 MB (4240841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e8f034153e28423592a04f327fe3b69d3d84721cb54631e3ea9dcae375ab0ef`  
		Last Modified: Thu, 02 Dec 2021 22:52:26 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.6-scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:78ee1d57413d89c46e808dbb121ad895537b74af783c6e6189366afa07638b66
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4237689 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b3276dd6f6de73a2af8ca0c6bd2dc88c7f7ae0a0ce334bcae39c14047aab540`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 04 Dec 2021 07:52:28 GMT
COPY file:025e99b21a301a69c768cc2c72e67c371165b6314d59d0a5a95958216fd24eac in /nats-server 
# Sat, 04 Dec 2021 07:52:28 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Sat, 04 Dec 2021 07:52:29 GMT
EXPOSE 4222 6222 8222
# Sat, 04 Dec 2021 07:52:29 GMT
ENTRYPOINT ["/nats-server"]
# Sat, 04 Dec 2021 07:52:30 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:75a8e365d6e58c8d8f7fe944a206f76f3e800542aca1b53e849c4bffc78fd22d`  
		Last Modified: Sat, 04 Dec 2021 07:55:01 GMT  
		Size: 4.2 MB (4237211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc2920e0912e6a42ee2fd0b7b8b31c6cca01c6c99f16c760f904492422ff7cae`  
		Last Modified: Sat, 04 Dec 2021 07:54:58 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.6-scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:8ecffb2097f683980b94450d536a99c79b3fe7654f8bc91fd1c45ad0825e6aae
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4189764 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90bb404fba49386fc48ceb05ee04604d317ff225da69f159d0bd4cc63a930c0e`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 03 Dec 2021 16:57:31 GMT
COPY file:b5f62686ba6debf89a42d2be7c4442db5f8735dba6b8932e6f01f315a2e63e27 in /nats-server 
# Fri, 03 Dec 2021 16:57:32 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 03 Dec 2021 16:57:32 GMT
EXPOSE 4222 6222 8222
# Fri, 03 Dec 2021 16:57:33 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 03 Dec 2021 16:57:34 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:44ff62bde832e2b2bca85708fd2fc86d7d6d1f4ca7c58b5d0e18e3d07c9c5bac`  
		Last Modified: Fri, 03 Dec 2021 16:58:50 GMT  
		Size: 4.2 MB (4189288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44dcbc70566b6f8312605c0214812444ccad7a55594fa2e7f0792c21af818ef0`  
		Last Modified: Fri, 03 Dec 2021 16:58:49 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.6-windowsservercore`

```console
$ docker pull nats@sha256:24e44e15d62a911e94d6ff5b7e22accfe329f699b42ade9ebb1a5caa3197f373
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.2452; amd64
	-	windows version 10.0.14393.4886; amd64

### `nats:2.6-windowsservercore` - windows version 10.0.17763.2452; amd64

```console
$ docker pull nats@sha256:7f3bfcdbda90968d69223b48664ee1ec937a82bce7365c82135785fe353ba699
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2717536770 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4622435affd612664c15aa4fd83b1e45ba56de92d3c7e6dd3dd924adf28111bf`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 07 Jan 2022 22:48:13 GMT
RUN Install update 1809-amd64
# Wed, 12 Jan 2022 13:54:17 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 Jan 2022 15:10:29 GMT
ENV NATS_DOCKERIZED=1
# Wed, 12 Jan 2022 15:10:30 GMT
ENV NATS_SERVER=2.6.6
# Wed, 12 Jan 2022 15:10:32 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.6.6/nats-server-v2.6.6-windows-amd64.zip
# Wed, 12 Jan 2022 15:10:33 GMT
ENV NATS_SERVER_SHASUM=9730ea401beed7ac40aeada0a8dccfb70207bb234202035aad5644e93ec657da
# Wed, 12 Jan 2022 15:11:32 GMT
RUN Set-PSDebug -Trace 2
# Wed, 12 Jan 2022 15:13:24 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 12 Jan 2022 15:13:26 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 12 Jan 2022 15:13:27 GMT
EXPOSE 4222 6222 8222
# Wed, 12 Jan 2022 15:13:28 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 12 Jan 2022 15:13:29 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:635f15ebd5b486e8a00bf217a0574a29550e5bbf08c1d021e1e308100b2e49b5`  
		Size: 993.9 MB (993898043 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:537828534783cff318d36854dbda0683aef7263e437c7c669de4092e1778959c`  
		Last Modified: Wed, 12 Jan 2022 15:14:30 GMT  
		Size: 1.3 KB (1296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9576e7772519d67febb0ceb94d8f22531ea99f0c60c36e67a4f5a497c384f5e0`  
		Last Modified: Wed, 12 Jan 2022 15:14:30 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaf1f761c394ef0da3c3fef1865f52e977d392f3f0b6c0575c3d1341da6cd7e9`  
		Last Modified: Wed, 12 Jan 2022 15:14:28 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e647346313038e022d4394703013d0963bc45ad0782bcf984166dd279d475c5d`  
		Last Modified: Wed, 12 Jan 2022 15:14:27 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fb56fc761a44bdcdde0f2cfaa2a75932b2ac8fe3c78177727284b0f58037fb0`  
		Last Modified: Wed, 12 Jan 2022 15:14:28 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5797262702f20651c9e1f79f4fbfbe22a260dc9bb7408bf5820eb186b3063f4d`  
		Last Modified: Wed, 12 Jan 2022 15:14:27 GMT  
		Size: 338.2 KB (338250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24cad06e122fd976b54af5acb5a3ba1d1299d61be733e7c2eadeb185aca82942`  
		Last Modified: Wed, 12 Jan 2022 15:14:31 GMT  
		Size: 5.0 MB (4954480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:886cf217b75c847a9ef63c4cc6093d9aa9c783f67b2c999fb7b23249e80b6e6c`  
		Last Modified: Wed, 12 Jan 2022 15:14:25 GMT  
		Size: 1.9 KB (1941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f1f92fb92be2d3b29fc1f42015a4d47bb112ae53db5fab9fa63f432838b7747`  
		Last Modified: Wed, 12 Jan 2022 15:14:25 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:099a82c04f8e6eee73daaccc93d0ad74009ffb4c94eb7d9c8a6a52b4e6bdf2fd`  
		Last Modified: Wed, 12 Jan 2022 15:14:25 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:507bd2ef766612deffd70102b577c1242165b07a8464313f8454713360560c86`  
		Last Modified: Wed, 12 Jan 2022 15:14:25 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.6-windowsservercore` - windows version 10.0.14393.4886; amd64

```console
$ docker pull nats@sha256:e476d11dde611fc9b39eb6a45798c2e503fa1bfa4ece59509826bfaed6a4cbe1
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6283541821 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:084594550a22f2aa624e5b2e740a29366a6846c2e1f194854e6e32270f5f0edb`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Thu, 06 Jan 2022 14:33:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 11 Jan 2022 19:57:39 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Tue, 11 Jan 2022 19:57:40 GMT
ENV NATS_DOCKERIZED=1
# Tue, 11 Jan 2022 21:15:53 GMT
ENV NATS_SERVER=2.6.6
# Tue, 11 Jan 2022 21:15:55 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.6.6/nats-server-v2.6.6-windows-amd64.zip
# Tue, 11 Jan 2022 21:15:56 GMT
ENV NATS_SERVER_SHASUM=9730ea401beed7ac40aeada0a8dccfb70207bb234202035aad5644e93ec657da
# Tue, 11 Jan 2022 21:16:48 GMT
RUN Set-PSDebug -Trace 2
# Tue, 11 Jan 2022 21:18:24 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Tue, 11 Jan 2022 21:18:25 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Tue, 11 Jan 2022 21:18:26 GMT
EXPOSE 4222 6222 8222
# Tue, 11 Jan 2022 21:18:28 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 11 Jan 2022 21:18:29 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8428508ffd63b4af1ba690ec41e82a116f10ec6c3fb70962348f5448d42e5835`  
		Size: 2.2 GB (2208216859 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:25aec0a6b64c784bf7521344203ee5def4d38eedfdd68f4b452d3250b5b9ddcf`  
		Last Modified: Tue, 11 Jan 2022 21:19:46 GMT  
		Size: 1.3 KB (1327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3fffdd310a93f98578e45ffbf8e22c031b37efefcc042f21d2a63c2a77c4ee3`  
		Last Modified: Tue, 11 Jan 2022 21:19:45 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15052497c858a1a8b4a8159d05850fbf43551aad161e61ae0fd6880c46eb4556`  
		Last Modified: Tue, 11 Jan 2022 21:19:44 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:080911a4b1ac40e1f062d68ed70319860e88ecb9abec2aef41d0bc3bae89098d`  
		Last Modified: Tue, 11 Jan 2022 21:19:44 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e79cea19a92f33c59acbcc8f501e9acdb5985bbad5b03ccd1190848ae1b4cf1`  
		Last Modified: Tue, 11 Jan 2022 21:19:44 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae0544e04ecd7b6afc6366924310fd892736faf1983ea2ee9e40efd31a0ec502`  
		Last Modified: Tue, 11 Jan 2022 21:19:44 GMT  
		Size: 337.0 KB (337010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8906d4ca25b04680081cc6af81b8eec86a9756abb72e21ed2785f82372ba7c58`  
		Last Modified: Tue, 11 Jan 2022 21:19:43 GMT  
		Size: 5.0 MB (4988964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99a01b43c4c8c06f528a3080b9f4d396d196ff851a603ac22c9ce560c3d5b082`  
		Last Modified: Tue, 11 Jan 2022 21:19:42 GMT  
		Size: 2.0 KB (1973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e156e4bebcfed633295afa0f9dacd6146736cb7de973581f01931fdf6d5f5ae`  
		Last Modified: Tue, 11 Jan 2022 21:19:41 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf3ee9fcf4be90533587d2a54238465fc8f6bad0744784041f675b2e97a93bb9`  
		Last Modified: Tue, 11 Jan 2022 21:19:42 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6e44c694323da6f62bebd7b52b659731c89b1e15c15e5c345ec43e24cba28f7`  
		Last Modified: Tue, 11 Jan 2022 21:19:41 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.6-windowsservercore-1809`

```console
$ docker pull nats@sha256:688fa8edbb0b5931af887d0ab00ed77da3f9e8505225dc1eccf15672638fd7a7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2452; amd64

### `nats:2.6-windowsservercore-1809` - windows version 10.0.17763.2452; amd64

```console
$ docker pull nats@sha256:7f3bfcdbda90968d69223b48664ee1ec937a82bce7365c82135785fe353ba699
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2717536770 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4622435affd612664c15aa4fd83b1e45ba56de92d3c7e6dd3dd924adf28111bf`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 07 Jan 2022 22:48:13 GMT
RUN Install update 1809-amd64
# Wed, 12 Jan 2022 13:54:17 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 Jan 2022 15:10:29 GMT
ENV NATS_DOCKERIZED=1
# Wed, 12 Jan 2022 15:10:30 GMT
ENV NATS_SERVER=2.6.6
# Wed, 12 Jan 2022 15:10:32 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.6.6/nats-server-v2.6.6-windows-amd64.zip
# Wed, 12 Jan 2022 15:10:33 GMT
ENV NATS_SERVER_SHASUM=9730ea401beed7ac40aeada0a8dccfb70207bb234202035aad5644e93ec657da
# Wed, 12 Jan 2022 15:11:32 GMT
RUN Set-PSDebug -Trace 2
# Wed, 12 Jan 2022 15:13:24 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 12 Jan 2022 15:13:26 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 12 Jan 2022 15:13:27 GMT
EXPOSE 4222 6222 8222
# Wed, 12 Jan 2022 15:13:28 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 12 Jan 2022 15:13:29 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:635f15ebd5b486e8a00bf217a0574a29550e5bbf08c1d021e1e308100b2e49b5`  
		Size: 993.9 MB (993898043 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:537828534783cff318d36854dbda0683aef7263e437c7c669de4092e1778959c`  
		Last Modified: Wed, 12 Jan 2022 15:14:30 GMT  
		Size: 1.3 KB (1296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9576e7772519d67febb0ceb94d8f22531ea99f0c60c36e67a4f5a497c384f5e0`  
		Last Modified: Wed, 12 Jan 2022 15:14:30 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaf1f761c394ef0da3c3fef1865f52e977d392f3f0b6c0575c3d1341da6cd7e9`  
		Last Modified: Wed, 12 Jan 2022 15:14:28 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e647346313038e022d4394703013d0963bc45ad0782bcf984166dd279d475c5d`  
		Last Modified: Wed, 12 Jan 2022 15:14:27 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fb56fc761a44bdcdde0f2cfaa2a75932b2ac8fe3c78177727284b0f58037fb0`  
		Last Modified: Wed, 12 Jan 2022 15:14:28 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5797262702f20651c9e1f79f4fbfbe22a260dc9bb7408bf5820eb186b3063f4d`  
		Last Modified: Wed, 12 Jan 2022 15:14:27 GMT  
		Size: 338.2 KB (338250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24cad06e122fd976b54af5acb5a3ba1d1299d61be733e7c2eadeb185aca82942`  
		Last Modified: Wed, 12 Jan 2022 15:14:31 GMT  
		Size: 5.0 MB (4954480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:886cf217b75c847a9ef63c4cc6093d9aa9c783f67b2c999fb7b23249e80b6e6c`  
		Last Modified: Wed, 12 Jan 2022 15:14:25 GMT  
		Size: 1.9 KB (1941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f1f92fb92be2d3b29fc1f42015a4d47bb112ae53db5fab9fa63f432838b7747`  
		Last Modified: Wed, 12 Jan 2022 15:14:25 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:099a82c04f8e6eee73daaccc93d0ad74009ffb4c94eb7d9c8a6a52b4e6bdf2fd`  
		Last Modified: Wed, 12 Jan 2022 15:14:25 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:507bd2ef766612deffd70102b577c1242165b07a8464313f8454713360560c86`  
		Last Modified: Wed, 12 Jan 2022 15:14:25 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.6-windowsservercore-ltsc2016`

```console
$ docker pull nats@sha256:3d337d85e45c503e13f57109f85de0e1c916fc6781cf7bbd3f40ccffd0fb664b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.14393.4886; amd64

### `nats:2.6-windowsservercore-ltsc2016` - windows version 10.0.14393.4886; amd64

```console
$ docker pull nats@sha256:e476d11dde611fc9b39eb6a45798c2e503fa1bfa4ece59509826bfaed6a4cbe1
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6283541821 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:084594550a22f2aa624e5b2e740a29366a6846c2e1f194854e6e32270f5f0edb`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Thu, 06 Jan 2022 14:33:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 11 Jan 2022 19:57:39 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Tue, 11 Jan 2022 19:57:40 GMT
ENV NATS_DOCKERIZED=1
# Tue, 11 Jan 2022 21:15:53 GMT
ENV NATS_SERVER=2.6.6
# Tue, 11 Jan 2022 21:15:55 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.6.6/nats-server-v2.6.6-windows-amd64.zip
# Tue, 11 Jan 2022 21:15:56 GMT
ENV NATS_SERVER_SHASUM=9730ea401beed7ac40aeada0a8dccfb70207bb234202035aad5644e93ec657da
# Tue, 11 Jan 2022 21:16:48 GMT
RUN Set-PSDebug -Trace 2
# Tue, 11 Jan 2022 21:18:24 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Tue, 11 Jan 2022 21:18:25 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Tue, 11 Jan 2022 21:18:26 GMT
EXPOSE 4222 6222 8222
# Tue, 11 Jan 2022 21:18:28 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 11 Jan 2022 21:18:29 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8428508ffd63b4af1ba690ec41e82a116f10ec6c3fb70962348f5448d42e5835`  
		Size: 2.2 GB (2208216859 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:25aec0a6b64c784bf7521344203ee5def4d38eedfdd68f4b452d3250b5b9ddcf`  
		Last Modified: Tue, 11 Jan 2022 21:19:46 GMT  
		Size: 1.3 KB (1327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3fffdd310a93f98578e45ffbf8e22c031b37efefcc042f21d2a63c2a77c4ee3`  
		Last Modified: Tue, 11 Jan 2022 21:19:45 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15052497c858a1a8b4a8159d05850fbf43551aad161e61ae0fd6880c46eb4556`  
		Last Modified: Tue, 11 Jan 2022 21:19:44 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:080911a4b1ac40e1f062d68ed70319860e88ecb9abec2aef41d0bc3bae89098d`  
		Last Modified: Tue, 11 Jan 2022 21:19:44 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e79cea19a92f33c59acbcc8f501e9acdb5985bbad5b03ccd1190848ae1b4cf1`  
		Last Modified: Tue, 11 Jan 2022 21:19:44 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae0544e04ecd7b6afc6366924310fd892736faf1983ea2ee9e40efd31a0ec502`  
		Last Modified: Tue, 11 Jan 2022 21:19:44 GMT  
		Size: 337.0 KB (337010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8906d4ca25b04680081cc6af81b8eec86a9756abb72e21ed2785f82372ba7c58`  
		Last Modified: Tue, 11 Jan 2022 21:19:43 GMT  
		Size: 5.0 MB (4988964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99a01b43c4c8c06f528a3080b9f4d396d196ff851a603ac22c9ce560c3d5b082`  
		Last Modified: Tue, 11 Jan 2022 21:19:42 GMT  
		Size: 2.0 KB (1973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e156e4bebcfed633295afa0f9dacd6146736cb7de973581f01931fdf6d5f5ae`  
		Last Modified: Tue, 11 Jan 2022 21:19:41 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf3ee9fcf4be90533587d2a54238465fc8f6bad0744784041f675b2e97a93bb9`  
		Last Modified: Tue, 11 Jan 2022 21:19:42 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6e44c694323da6f62bebd7b52b659731c89b1e15c15e5c345ec43e24cba28f7`  
		Last Modified: Tue, 11 Jan 2022 21:19:41 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.6.6`

```console
$ docker pull nats@sha256:9bd747193a9d316341136227475dbde257fe33d6209b7b43beaf16ae0a358865
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.2452; amd64

### `nats:2.6.6` - linux; amd64

```console
$ docker pull nats@sha256:dad4f69520337c2a80d2a9123963c971836f07f530cf4b7c56dde98a622e0a6b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4578170 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ba73da93bdda8525a9f473851ee3de9a2d23c21e1d0a51d7da118bc122df420`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 03 Dec 2021 21:23:03 GMT
COPY file:4070919cac43aa01e3ef5dd95589f24a9d649dcc7b4d6364927c764b1f90392e in /nats-server 
# Fri, 03 Dec 2021 21:23:04 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 03 Dec 2021 21:23:04 GMT
EXPOSE 4222 6222 8222
# Fri, 03 Dec 2021 21:23:04 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 03 Dec 2021 21:23:04 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:730cae3de796bb1fbb06f0f847317c2b738bf9af9d1233daafcf2f708eade5ec`  
		Last Modified: Fri, 03 Dec 2021 21:24:01 GMT  
		Size: 4.6 MB (4577696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39027e71725d02ee81938943fd0f3e980f01abbe21c5e8f8ea8219687aaae862`  
		Last Modified: Fri, 03 Dec 2021 21:24:00 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.6.6` - linux; arm variant v6

```console
$ docker pull nats@sha256:54395301fd2f315191df081131cd6d142613d057970268d64480f4706bcaeda3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4241317 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c4851d5f7b19bc49c52879a43236bae3e26e03a8a0f035ec150eed9a723cca5`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 02 Dec 2021 22:50:02 GMT
COPY file:6036f30fae4132d78e941219bf965a4e4c3e6d898ac912ab22e7a0cc98adf5a5 in /nats-server 
# Thu, 02 Dec 2021 22:50:03 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 02 Dec 2021 22:50:03 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Dec 2021 22:50:04 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 02 Dec 2021 22:50:04 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:41ef8f0f5e4d1f0e1880325ac8c2ccde63d323e6ead77b97c1225e0ce1d226ce`  
		Last Modified: Thu, 02 Dec 2021 22:52:29 GMT  
		Size: 4.2 MB (4240841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e8f034153e28423592a04f327fe3b69d3d84721cb54631e3ea9dcae375ab0ef`  
		Last Modified: Thu, 02 Dec 2021 22:52:26 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.6.6` - linux; arm variant v7

```console
$ docker pull nats@sha256:78ee1d57413d89c46e808dbb121ad895537b74af783c6e6189366afa07638b66
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4237689 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b3276dd6f6de73a2af8ca0c6bd2dc88c7f7ae0a0ce334bcae39c14047aab540`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 04 Dec 2021 07:52:28 GMT
COPY file:025e99b21a301a69c768cc2c72e67c371165b6314d59d0a5a95958216fd24eac in /nats-server 
# Sat, 04 Dec 2021 07:52:28 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Sat, 04 Dec 2021 07:52:29 GMT
EXPOSE 4222 6222 8222
# Sat, 04 Dec 2021 07:52:29 GMT
ENTRYPOINT ["/nats-server"]
# Sat, 04 Dec 2021 07:52:30 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:75a8e365d6e58c8d8f7fe944a206f76f3e800542aca1b53e849c4bffc78fd22d`  
		Last Modified: Sat, 04 Dec 2021 07:55:01 GMT  
		Size: 4.2 MB (4237211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc2920e0912e6a42ee2fd0b7b8b31c6cca01c6c99f16c760f904492422ff7cae`  
		Last Modified: Sat, 04 Dec 2021 07:54:58 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.6.6` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:8ecffb2097f683980b94450d536a99c79b3fe7654f8bc91fd1c45ad0825e6aae
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4189764 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90bb404fba49386fc48ceb05ee04604d317ff225da69f159d0bd4cc63a930c0e`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 03 Dec 2021 16:57:31 GMT
COPY file:b5f62686ba6debf89a42d2be7c4442db5f8735dba6b8932e6f01f315a2e63e27 in /nats-server 
# Fri, 03 Dec 2021 16:57:32 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 03 Dec 2021 16:57:32 GMT
EXPOSE 4222 6222 8222
# Fri, 03 Dec 2021 16:57:33 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 03 Dec 2021 16:57:34 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:44ff62bde832e2b2bca85708fd2fc86d7d6d1f4ca7c58b5d0e18e3d07c9c5bac`  
		Last Modified: Fri, 03 Dec 2021 16:58:50 GMT  
		Size: 4.2 MB (4189288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44dcbc70566b6f8312605c0214812444ccad7a55594fa2e7f0792c21af818ef0`  
		Last Modified: Fri, 03 Dec 2021 16:58:49 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.6.6` - windows version 10.0.17763.2452; amd64

```console
$ docker pull nats@sha256:73596edd7d2bcfb546b2b6da26cbaf06733398e7cc550a610ed8e53c5c59021c
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.7 MB (107674705 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa5c572d20b69e54dca9ee7a24b26d6b489d4cd2be1d5931d9accce1dbb7e030`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 07 Jan 2022 22:25:06 GMT
RUN Apply image 1809-amd64
# Wed, 12 Jan 2022 15:13:42 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 12 Jan 2022 15:13:43 GMT
RUN cmd /S /C #(nop) COPY file:20c797e6dad00d7098dbf6d4d158c380fd073bc5fc24a80fd4f23205af77a338 in C:\nats-server.exe 
# Wed, 12 Jan 2022 15:13:44 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 12 Jan 2022 15:13:45 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 12 Jan 2022 15:13:46 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 12 Jan 2022 15:13:47 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3a78847ea829208edc2d7b320b7e602b9d12e47689499d5180a9cc7790dec4d7`  
		Size: 103.0 MB (103031066 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:db05d2e76671d91772a070867bf6f050343319070602a0f8239706d5d4d98387`  
		Last Modified: Wed, 12 Jan 2022 15:14:49 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6271ae84b48476b5c259495509975bd53d7f398555179642c1ef1d612099cb19`  
		Last Modified: Wed, 12 Jan 2022 15:14:48 GMT  
		Size: 4.6 MB (4637258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:178ab94841651126bd3f8a1478a504e44f389c2bf5abf59abafc16f163108f4c`  
		Last Modified: Wed, 12 Jan 2022 15:14:46 GMT  
		Size: 1.8 KB (1759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aa2ac290e2024e6f26c6fd076cc312a10b4842536f9c9daad8ac0e5ecced071`  
		Last Modified: Wed, 12 Jan 2022 15:14:46 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8cb0f84aeae0a7ea0020f00dd7b55f02b772c0bfaa74ea61e1fbd266eff8928`  
		Last Modified: Wed, 12 Jan 2022 15:14:46 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7238bcc9c911d52c987ca07602cb3204bf985a35ae993830fe3b54ea9563de43`  
		Last Modified: Wed, 12 Jan 2022 15:14:46 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.6.6-alpine`

```console
$ docker pull nats@sha256:8e2e34eb798631cd76f341277f529f78618a2366d81b59586d3b81f6cb839b25
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.6.6-alpine` - linux; amd64

```console
$ docker pull nats@sha256:687f39ecdab1eeda8a4eaa7b7210586d96698faa5e5e7e47aaf5ef8084d504e5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.7 MB (7689543 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c5dc2cfb512e016e62911eca35c050a2eb5ca4b783d5f2d413ba64c68c420bd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:44 GMT
ADD file:762c899ec0505d1a32930ee804c5b008825f41611161be104076cba33b7e5b2b in / 
# Fri, 12 Nov 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 03 Dec 2021 21:22:18 GMT
ENV NATS_SERVER=2.6.6
# Fri, 03 Dec 2021 21:22:21 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='70da0ad3694aebfc742f9aae919d3a4aa5b8c863946e99c5d332195fbbdad49c' ;; 		armhf) natsArch='arm6'; sha256='e2cc1e198d5d5c83e2f2c2dcb15fafb71601603e3740065682812afaa7dd443a' ;; 		armv7) natsArch='arm7'; sha256='f3698a4fb18c6664d477b920d5f07637141a6623cf2fa998900155fea0d97e61' ;; 		x86_64) natsArch='amd64'; sha256='2c2fc16322fb2bc0b166ee2a01e163d4beb2cf7b49d083cebcd36695dc05a381' ;; 		x86) natsArch='386'; sha256='1da03b0d163dc98209f010bf6efa5fc6c81a23b4bab7a98bebe142e19fc26bdc' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 03 Dec 2021 21:22:21 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 03 Dec 2021 21:22:22 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 03 Dec 2021 21:22:22 GMT
EXPOSE 4222 6222 8222
# Fri, 03 Dec 2021 21:22:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 03 Dec 2021 21:22:22 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:97518928ae5f3d52d4164b314a7e73654eb686ecd8aafa0b79acd980773a740d`  
		Last Modified: Fri, 12 Nov 2021 17:20:39 GMT  
		Size: 2.8 MB (2822981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daeb19d8d614f4a1df58ed04d3c72469fa9f7286c9d5482ee274405723b5e645`  
		Last Modified: Fri, 03 Dec 2021 21:23:37 GMT  
		Size: 4.9 MB (4865593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e51c3679390c1ab0c5f5e6786505ad9278d45683059fc7fac0298dcbb6dede86`  
		Last Modified: Fri, 03 Dec 2021 21:23:36 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b14f15cf01b25470e7340acc8ca0860eb4a00a7e1b5d5180bd7c23db1dd273af`  
		Last Modified: Fri, 03 Dec 2021 21:23:36 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.6.6-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:d42d25248435c99492dd0fbcd97688486c692c680069bc9a1eb8a7b1c85eebff
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7161537 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ae84a8c7e689bc4d7fd2915ef9aaf1fb624c094cb183af5863d4b20984f29cd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 12 Nov 2021 16:49:42 GMT
ADD file:6daf1fe862c00673bf9cf4d7e20b0bf253a56e7fb8ed5e730a4466ab9186e18a in / 
# Fri, 12 Nov 2021 16:49:44 GMT
CMD ["/bin/sh"]
# Thu, 02 Dec 2021 22:49:35 GMT
ENV NATS_SERVER=2.6.6
# Thu, 02 Dec 2021 22:49:39 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='70da0ad3694aebfc742f9aae919d3a4aa5b8c863946e99c5d332195fbbdad49c' ;; 		armhf) natsArch='arm6'; sha256='e2cc1e198d5d5c83e2f2c2dcb15fafb71601603e3740065682812afaa7dd443a' ;; 		armv7) natsArch='arm7'; sha256='f3698a4fb18c6664d477b920d5f07637141a6623cf2fa998900155fea0d97e61' ;; 		x86_64) natsArch='amd64'; sha256='2c2fc16322fb2bc0b166ee2a01e163d4beb2cf7b49d083cebcd36695dc05a381' ;; 		x86) natsArch='386'; sha256='1da03b0d163dc98209f010bf6efa5fc6c81a23b4bab7a98bebe142e19fc26bdc' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 02 Dec 2021 22:49:40 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 02 Dec 2021 22:49:40 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 02 Dec 2021 22:49:41 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Dec 2021 22:49:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 02 Dec 2021 22:49:42 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:56afcfda5d78cc243287acbaad250c5e8c0f47aae620dd7c51985b0d3c9b2728`  
		Last Modified: Fri, 12 Nov 2021 16:51:32 GMT  
		Size: 2.6 MB (2635392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3c7b89c441a056fc0e4d867cd4fd28308f188bd0f6b306e5feee96fee47cbdf`  
		Last Modified: Thu, 02 Dec 2021 22:51:52 GMT  
		Size: 4.5 MB (4525169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f67a5f3b97f233f2d6d30a90acd85b9e856cb9b98c298b71e2b5cbae3e0268cf`  
		Last Modified: Thu, 02 Dec 2021 22:51:50 GMT  
		Size: 561.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:706486ffe19b237b40203ebf10cb1110d7566cba5a3c10bf738be70173a1aa69`  
		Last Modified: Thu, 02 Dec 2021 22:51:50 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.6.6-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:dbc345345cfc225bd88b35e80f85f412483db712134bde3a0e4d959cb543350f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.0 MB (6958146 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6aaa47180fd5390c3f39b81e39db30c26897fc1b070c064d4677ebdd14c1f801`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 12 Nov 2021 16:57:35 GMT
ADD file:03e0720458c3475758bf4394afa56f2165198eb91e6e9581f7768e433744dd9b in / 
# Fri, 12 Nov 2021 16:57:36 GMT
CMD ["/bin/sh"]
# Sat, 04 Dec 2021 07:51:50 GMT
ENV NATS_SERVER=2.6.6
# Sat, 04 Dec 2021 07:51:54 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='70da0ad3694aebfc742f9aae919d3a4aa5b8c863946e99c5d332195fbbdad49c' ;; 		armhf) natsArch='arm6'; sha256='e2cc1e198d5d5c83e2f2c2dcb15fafb71601603e3740065682812afaa7dd443a' ;; 		armv7) natsArch='arm7'; sha256='f3698a4fb18c6664d477b920d5f07637141a6623cf2fa998900155fea0d97e61' ;; 		x86_64) natsArch='amd64'; sha256='2c2fc16322fb2bc0b166ee2a01e163d4beb2cf7b49d083cebcd36695dc05a381' ;; 		x86) natsArch='386'; sha256='1da03b0d163dc98209f010bf6efa5fc6c81a23b4bab7a98bebe142e19fc26bdc' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Sat, 04 Dec 2021 07:51:55 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Sat, 04 Dec 2021 07:51:55 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Sat, 04 Dec 2021 07:51:56 GMT
EXPOSE 4222 6222 8222
# Sat, 04 Dec 2021 07:51:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 04 Dec 2021 07:51:57 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:764d2e53e1a607f2d8261522185d5b9021ade3ec1a595664ee90308c00176899`  
		Last Modified: Fri, 12 Nov 2021 16:59:33 GMT  
		Size: 2.4 MB (2438618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:157eac698795baeacb3153cf2bbbc17f348e477e8062fa45b6728e97dd02e157`  
		Last Modified: Sat, 04 Dec 2021 07:54:19 GMT  
		Size: 4.5 MB (4518555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b5241fcba964a14f9c4681ebcc94815a476df86f68c628494f5759a3bee8514`  
		Last Modified: Sat, 04 Dec 2021 07:54:16 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36d02df08ee2f75a857120c105153a83b2b951337a87e902260e70e1de20dfd0`  
		Last Modified: Sat, 04 Dec 2021 07:54:16 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.6.6-alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:f1e7262504ed73a185ee16f6a6da14c19c3a76120f2b22c51a051a0988ac3bdc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7193478 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55e483df89c189235b79aa4a9d2417378172236dba6fa85f6d5a0bb35756835f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 12 Nov 2021 16:39:58 GMT
ADD file:400c0466b29ccad54e0f6c0acef22542992828678c96693ef1f9f4d0551935d8 in / 
# Fri, 12 Nov 2021 16:39:58 GMT
CMD ["/bin/sh"]
# Fri, 03 Dec 2021 16:57:10 GMT
ENV NATS_SERVER=2.6.6
# Fri, 03 Dec 2021 16:57:13 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='70da0ad3694aebfc742f9aae919d3a4aa5b8c863946e99c5d332195fbbdad49c' ;; 		armhf) natsArch='arm6'; sha256='e2cc1e198d5d5c83e2f2c2dcb15fafb71601603e3740065682812afaa7dd443a' ;; 		armv7) natsArch='arm7'; sha256='f3698a4fb18c6664d477b920d5f07637141a6623cf2fa998900155fea0d97e61' ;; 		x86_64) natsArch='amd64'; sha256='2c2fc16322fb2bc0b166ee2a01e163d4beb2cf7b49d083cebcd36695dc05a381' ;; 		x86) natsArch='386'; sha256='1da03b0d163dc98209f010bf6efa5fc6c81a23b4bab7a98bebe142e19fc26bdc' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 03 Dec 2021 16:57:15 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 03 Dec 2021 16:57:16 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 03 Dec 2021 16:57:16 GMT
EXPOSE 4222 6222 8222
# Fri, 03 Dec 2021 16:57:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 03 Dec 2021 16:57:18 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:be307f383ecc62b27a29b599c3fc9d3129693a798e7fcce614f09174cfe2d354`  
		Last Modified: Fri, 12 Nov 2021 16:40:59 GMT  
		Size: 2.7 MB (2717700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdee3b2a5421d3ceb50b8101857ce4c0815c4532476e1f292867c63034c08f61`  
		Last Modified: Fri, 03 Dec 2021 16:58:22 GMT  
		Size: 4.5 MB (4474835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8a771880289bb86cd368ca8b39620b0cfe69694646e061ff6975f959ccfcd29`  
		Last Modified: Fri, 03 Dec 2021 16:58:21 GMT  
		Size: 528.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:438c5abdffd6599ac83fe661d26a9491552d63f48aeb9147609299ee11b78c78`  
		Last Modified: Fri, 03 Dec 2021 16:58:21 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.6.6-alpine3.14`

```console
$ docker pull nats@sha256:8e2e34eb798631cd76f341277f529f78618a2366d81b59586d3b81f6cb839b25
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.6.6-alpine3.14` - linux; amd64

```console
$ docker pull nats@sha256:687f39ecdab1eeda8a4eaa7b7210586d96698faa5e5e7e47aaf5ef8084d504e5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.7 MB (7689543 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c5dc2cfb512e016e62911eca35c050a2eb5ca4b783d5f2d413ba64c68c420bd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:44 GMT
ADD file:762c899ec0505d1a32930ee804c5b008825f41611161be104076cba33b7e5b2b in / 
# Fri, 12 Nov 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 03 Dec 2021 21:22:18 GMT
ENV NATS_SERVER=2.6.6
# Fri, 03 Dec 2021 21:22:21 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='70da0ad3694aebfc742f9aae919d3a4aa5b8c863946e99c5d332195fbbdad49c' ;; 		armhf) natsArch='arm6'; sha256='e2cc1e198d5d5c83e2f2c2dcb15fafb71601603e3740065682812afaa7dd443a' ;; 		armv7) natsArch='arm7'; sha256='f3698a4fb18c6664d477b920d5f07637141a6623cf2fa998900155fea0d97e61' ;; 		x86_64) natsArch='amd64'; sha256='2c2fc16322fb2bc0b166ee2a01e163d4beb2cf7b49d083cebcd36695dc05a381' ;; 		x86) natsArch='386'; sha256='1da03b0d163dc98209f010bf6efa5fc6c81a23b4bab7a98bebe142e19fc26bdc' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 03 Dec 2021 21:22:21 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 03 Dec 2021 21:22:22 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 03 Dec 2021 21:22:22 GMT
EXPOSE 4222 6222 8222
# Fri, 03 Dec 2021 21:22:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 03 Dec 2021 21:22:22 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:97518928ae5f3d52d4164b314a7e73654eb686ecd8aafa0b79acd980773a740d`  
		Last Modified: Fri, 12 Nov 2021 17:20:39 GMT  
		Size: 2.8 MB (2822981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daeb19d8d614f4a1df58ed04d3c72469fa9f7286c9d5482ee274405723b5e645`  
		Last Modified: Fri, 03 Dec 2021 21:23:37 GMT  
		Size: 4.9 MB (4865593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e51c3679390c1ab0c5f5e6786505ad9278d45683059fc7fac0298dcbb6dede86`  
		Last Modified: Fri, 03 Dec 2021 21:23:36 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b14f15cf01b25470e7340acc8ca0860eb4a00a7e1b5d5180bd7c23db1dd273af`  
		Last Modified: Fri, 03 Dec 2021 21:23:36 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.6.6-alpine3.14` - linux; arm variant v6

```console
$ docker pull nats@sha256:d42d25248435c99492dd0fbcd97688486c692c680069bc9a1eb8a7b1c85eebff
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7161537 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ae84a8c7e689bc4d7fd2915ef9aaf1fb624c094cb183af5863d4b20984f29cd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 12 Nov 2021 16:49:42 GMT
ADD file:6daf1fe862c00673bf9cf4d7e20b0bf253a56e7fb8ed5e730a4466ab9186e18a in / 
# Fri, 12 Nov 2021 16:49:44 GMT
CMD ["/bin/sh"]
# Thu, 02 Dec 2021 22:49:35 GMT
ENV NATS_SERVER=2.6.6
# Thu, 02 Dec 2021 22:49:39 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='70da0ad3694aebfc742f9aae919d3a4aa5b8c863946e99c5d332195fbbdad49c' ;; 		armhf) natsArch='arm6'; sha256='e2cc1e198d5d5c83e2f2c2dcb15fafb71601603e3740065682812afaa7dd443a' ;; 		armv7) natsArch='arm7'; sha256='f3698a4fb18c6664d477b920d5f07637141a6623cf2fa998900155fea0d97e61' ;; 		x86_64) natsArch='amd64'; sha256='2c2fc16322fb2bc0b166ee2a01e163d4beb2cf7b49d083cebcd36695dc05a381' ;; 		x86) natsArch='386'; sha256='1da03b0d163dc98209f010bf6efa5fc6c81a23b4bab7a98bebe142e19fc26bdc' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 02 Dec 2021 22:49:40 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 02 Dec 2021 22:49:40 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 02 Dec 2021 22:49:41 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Dec 2021 22:49:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 02 Dec 2021 22:49:42 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:56afcfda5d78cc243287acbaad250c5e8c0f47aae620dd7c51985b0d3c9b2728`  
		Last Modified: Fri, 12 Nov 2021 16:51:32 GMT  
		Size: 2.6 MB (2635392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3c7b89c441a056fc0e4d867cd4fd28308f188bd0f6b306e5feee96fee47cbdf`  
		Last Modified: Thu, 02 Dec 2021 22:51:52 GMT  
		Size: 4.5 MB (4525169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f67a5f3b97f233f2d6d30a90acd85b9e856cb9b98c298b71e2b5cbae3e0268cf`  
		Last Modified: Thu, 02 Dec 2021 22:51:50 GMT  
		Size: 561.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:706486ffe19b237b40203ebf10cb1110d7566cba5a3c10bf738be70173a1aa69`  
		Last Modified: Thu, 02 Dec 2021 22:51:50 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.6.6-alpine3.14` - linux; arm variant v7

```console
$ docker pull nats@sha256:dbc345345cfc225bd88b35e80f85f412483db712134bde3a0e4d959cb543350f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.0 MB (6958146 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6aaa47180fd5390c3f39b81e39db30c26897fc1b070c064d4677ebdd14c1f801`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 12 Nov 2021 16:57:35 GMT
ADD file:03e0720458c3475758bf4394afa56f2165198eb91e6e9581f7768e433744dd9b in / 
# Fri, 12 Nov 2021 16:57:36 GMT
CMD ["/bin/sh"]
# Sat, 04 Dec 2021 07:51:50 GMT
ENV NATS_SERVER=2.6.6
# Sat, 04 Dec 2021 07:51:54 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='70da0ad3694aebfc742f9aae919d3a4aa5b8c863946e99c5d332195fbbdad49c' ;; 		armhf) natsArch='arm6'; sha256='e2cc1e198d5d5c83e2f2c2dcb15fafb71601603e3740065682812afaa7dd443a' ;; 		armv7) natsArch='arm7'; sha256='f3698a4fb18c6664d477b920d5f07637141a6623cf2fa998900155fea0d97e61' ;; 		x86_64) natsArch='amd64'; sha256='2c2fc16322fb2bc0b166ee2a01e163d4beb2cf7b49d083cebcd36695dc05a381' ;; 		x86) natsArch='386'; sha256='1da03b0d163dc98209f010bf6efa5fc6c81a23b4bab7a98bebe142e19fc26bdc' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Sat, 04 Dec 2021 07:51:55 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Sat, 04 Dec 2021 07:51:55 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Sat, 04 Dec 2021 07:51:56 GMT
EXPOSE 4222 6222 8222
# Sat, 04 Dec 2021 07:51:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 04 Dec 2021 07:51:57 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:764d2e53e1a607f2d8261522185d5b9021ade3ec1a595664ee90308c00176899`  
		Last Modified: Fri, 12 Nov 2021 16:59:33 GMT  
		Size: 2.4 MB (2438618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:157eac698795baeacb3153cf2bbbc17f348e477e8062fa45b6728e97dd02e157`  
		Last Modified: Sat, 04 Dec 2021 07:54:19 GMT  
		Size: 4.5 MB (4518555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b5241fcba964a14f9c4681ebcc94815a476df86f68c628494f5759a3bee8514`  
		Last Modified: Sat, 04 Dec 2021 07:54:16 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36d02df08ee2f75a857120c105153a83b2b951337a87e902260e70e1de20dfd0`  
		Last Modified: Sat, 04 Dec 2021 07:54:16 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.6.6-alpine3.14` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:f1e7262504ed73a185ee16f6a6da14c19c3a76120f2b22c51a051a0988ac3bdc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7193478 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55e483df89c189235b79aa4a9d2417378172236dba6fa85f6d5a0bb35756835f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 12 Nov 2021 16:39:58 GMT
ADD file:400c0466b29ccad54e0f6c0acef22542992828678c96693ef1f9f4d0551935d8 in / 
# Fri, 12 Nov 2021 16:39:58 GMT
CMD ["/bin/sh"]
# Fri, 03 Dec 2021 16:57:10 GMT
ENV NATS_SERVER=2.6.6
# Fri, 03 Dec 2021 16:57:13 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='70da0ad3694aebfc742f9aae919d3a4aa5b8c863946e99c5d332195fbbdad49c' ;; 		armhf) natsArch='arm6'; sha256='e2cc1e198d5d5c83e2f2c2dcb15fafb71601603e3740065682812afaa7dd443a' ;; 		armv7) natsArch='arm7'; sha256='f3698a4fb18c6664d477b920d5f07637141a6623cf2fa998900155fea0d97e61' ;; 		x86_64) natsArch='amd64'; sha256='2c2fc16322fb2bc0b166ee2a01e163d4beb2cf7b49d083cebcd36695dc05a381' ;; 		x86) natsArch='386'; sha256='1da03b0d163dc98209f010bf6efa5fc6c81a23b4bab7a98bebe142e19fc26bdc' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 03 Dec 2021 16:57:15 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 03 Dec 2021 16:57:16 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 03 Dec 2021 16:57:16 GMT
EXPOSE 4222 6222 8222
# Fri, 03 Dec 2021 16:57:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 03 Dec 2021 16:57:18 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:be307f383ecc62b27a29b599c3fc9d3129693a798e7fcce614f09174cfe2d354`  
		Last Modified: Fri, 12 Nov 2021 16:40:59 GMT  
		Size: 2.7 MB (2717700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdee3b2a5421d3ceb50b8101857ce4c0815c4532476e1f292867c63034c08f61`  
		Last Modified: Fri, 03 Dec 2021 16:58:22 GMT  
		Size: 4.5 MB (4474835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8a771880289bb86cd368ca8b39620b0cfe69694646e061ff6975f959ccfcd29`  
		Last Modified: Fri, 03 Dec 2021 16:58:21 GMT  
		Size: 528.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:438c5abdffd6599ac83fe661d26a9491552d63f48aeb9147609299ee11b78c78`  
		Last Modified: Fri, 03 Dec 2021 16:58:21 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.6.6-linux`

```console
$ docker pull nats@sha256:5d130fed2ad109f922a3a52e45c0b87c0d5a674ad432024cb3d45f898cf425b8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.6.6-linux` - linux; amd64

```console
$ docker pull nats@sha256:dad4f69520337c2a80d2a9123963c971836f07f530cf4b7c56dde98a622e0a6b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4578170 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ba73da93bdda8525a9f473851ee3de9a2d23c21e1d0a51d7da118bc122df420`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 03 Dec 2021 21:23:03 GMT
COPY file:4070919cac43aa01e3ef5dd95589f24a9d649dcc7b4d6364927c764b1f90392e in /nats-server 
# Fri, 03 Dec 2021 21:23:04 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 03 Dec 2021 21:23:04 GMT
EXPOSE 4222 6222 8222
# Fri, 03 Dec 2021 21:23:04 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 03 Dec 2021 21:23:04 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:730cae3de796bb1fbb06f0f847317c2b738bf9af9d1233daafcf2f708eade5ec`  
		Last Modified: Fri, 03 Dec 2021 21:24:01 GMT  
		Size: 4.6 MB (4577696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39027e71725d02ee81938943fd0f3e980f01abbe21c5e8f8ea8219687aaae862`  
		Last Modified: Fri, 03 Dec 2021 21:24:00 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.6.6-linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:54395301fd2f315191df081131cd6d142613d057970268d64480f4706bcaeda3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4241317 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c4851d5f7b19bc49c52879a43236bae3e26e03a8a0f035ec150eed9a723cca5`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 02 Dec 2021 22:50:02 GMT
COPY file:6036f30fae4132d78e941219bf965a4e4c3e6d898ac912ab22e7a0cc98adf5a5 in /nats-server 
# Thu, 02 Dec 2021 22:50:03 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 02 Dec 2021 22:50:03 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Dec 2021 22:50:04 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 02 Dec 2021 22:50:04 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:41ef8f0f5e4d1f0e1880325ac8c2ccde63d323e6ead77b97c1225e0ce1d226ce`  
		Last Modified: Thu, 02 Dec 2021 22:52:29 GMT  
		Size: 4.2 MB (4240841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e8f034153e28423592a04f327fe3b69d3d84721cb54631e3ea9dcae375ab0ef`  
		Last Modified: Thu, 02 Dec 2021 22:52:26 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.6.6-linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:78ee1d57413d89c46e808dbb121ad895537b74af783c6e6189366afa07638b66
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4237689 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b3276dd6f6de73a2af8ca0c6bd2dc88c7f7ae0a0ce334bcae39c14047aab540`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 04 Dec 2021 07:52:28 GMT
COPY file:025e99b21a301a69c768cc2c72e67c371165b6314d59d0a5a95958216fd24eac in /nats-server 
# Sat, 04 Dec 2021 07:52:28 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Sat, 04 Dec 2021 07:52:29 GMT
EXPOSE 4222 6222 8222
# Sat, 04 Dec 2021 07:52:29 GMT
ENTRYPOINT ["/nats-server"]
# Sat, 04 Dec 2021 07:52:30 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:75a8e365d6e58c8d8f7fe944a206f76f3e800542aca1b53e849c4bffc78fd22d`  
		Last Modified: Sat, 04 Dec 2021 07:55:01 GMT  
		Size: 4.2 MB (4237211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc2920e0912e6a42ee2fd0b7b8b31c6cca01c6c99f16c760f904492422ff7cae`  
		Last Modified: Sat, 04 Dec 2021 07:54:58 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.6.6-linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:8ecffb2097f683980b94450d536a99c79b3fe7654f8bc91fd1c45ad0825e6aae
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4189764 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90bb404fba49386fc48ceb05ee04604d317ff225da69f159d0bd4cc63a930c0e`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 03 Dec 2021 16:57:31 GMT
COPY file:b5f62686ba6debf89a42d2be7c4442db5f8735dba6b8932e6f01f315a2e63e27 in /nats-server 
# Fri, 03 Dec 2021 16:57:32 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 03 Dec 2021 16:57:32 GMT
EXPOSE 4222 6222 8222
# Fri, 03 Dec 2021 16:57:33 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 03 Dec 2021 16:57:34 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:44ff62bde832e2b2bca85708fd2fc86d7d6d1f4ca7c58b5d0e18e3d07c9c5bac`  
		Last Modified: Fri, 03 Dec 2021 16:58:50 GMT  
		Size: 4.2 MB (4189288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44dcbc70566b6f8312605c0214812444ccad7a55594fa2e7f0792c21af818ef0`  
		Last Modified: Fri, 03 Dec 2021 16:58:49 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.6.6-nanoserver`

```console
$ docker pull nats@sha256:0b2895172f1057f6c9b6bfeb7502714c3bfee379610222e16e17a226fc537354
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2452; amd64

### `nats:2.6.6-nanoserver` - windows version 10.0.17763.2452; amd64

```console
$ docker pull nats@sha256:73596edd7d2bcfb546b2b6da26cbaf06733398e7cc550a610ed8e53c5c59021c
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.7 MB (107674705 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa5c572d20b69e54dca9ee7a24b26d6b489d4cd2be1d5931d9accce1dbb7e030`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 07 Jan 2022 22:25:06 GMT
RUN Apply image 1809-amd64
# Wed, 12 Jan 2022 15:13:42 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 12 Jan 2022 15:13:43 GMT
RUN cmd /S /C #(nop) COPY file:20c797e6dad00d7098dbf6d4d158c380fd073bc5fc24a80fd4f23205af77a338 in C:\nats-server.exe 
# Wed, 12 Jan 2022 15:13:44 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 12 Jan 2022 15:13:45 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 12 Jan 2022 15:13:46 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 12 Jan 2022 15:13:47 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3a78847ea829208edc2d7b320b7e602b9d12e47689499d5180a9cc7790dec4d7`  
		Size: 103.0 MB (103031066 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:db05d2e76671d91772a070867bf6f050343319070602a0f8239706d5d4d98387`  
		Last Modified: Wed, 12 Jan 2022 15:14:49 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6271ae84b48476b5c259495509975bd53d7f398555179642c1ef1d612099cb19`  
		Last Modified: Wed, 12 Jan 2022 15:14:48 GMT  
		Size: 4.6 MB (4637258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:178ab94841651126bd3f8a1478a504e44f389c2bf5abf59abafc16f163108f4c`  
		Last Modified: Wed, 12 Jan 2022 15:14:46 GMT  
		Size: 1.8 KB (1759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aa2ac290e2024e6f26c6fd076cc312a10b4842536f9c9daad8ac0e5ecced071`  
		Last Modified: Wed, 12 Jan 2022 15:14:46 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8cb0f84aeae0a7ea0020f00dd7b55f02b772c0bfaa74ea61e1fbd266eff8928`  
		Last Modified: Wed, 12 Jan 2022 15:14:46 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7238bcc9c911d52c987ca07602cb3204bf985a35ae993830fe3b54ea9563de43`  
		Last Modified: Wed, 12 Jan 2022 15:14:46 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.6.6-nanoserver-1809`

```console
$ docker pull nats@sha256:0b2895172f1057f6c9b6bfeb7502714c3bfee379610222e16e17a226fc537354
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2452; amd64

### `nats:2.6.6-nanoserver-1809` - windows version 10.0.17763.2452; amd64

```console
$ docker pull nats@sha256:73596edd7d2bcfb546b2b6da26cbaf06733398e7cc550a610ed8e53c5c59021c
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.7 MB (107674705 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa5c572d20b69e54dca9ee7a24b26d6b489d4cd2be1d5931d9accce1dbb7e030`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 07 Jan 2022 22:25:06 GMT
RUN Apply image 1809-amd64
# Wed, 12 Jan 2022 15:13:42 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 12 Jan 2022 15:13:43 GMT
RUN cmd /S /C #(nop) COPY file:20c797e6dad00d7098dbf6d4d158c380fd073bc5fc24a80fd4f23205af77a338 in C:\nats-server.exe 
# Wed, 12 Jan 2022 15:13:44 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 12 Jan 2022 15:13:45 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 12 Jan 2022 15:13:46 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 12 Jan 2022 15:13:47 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3a78847ea829208edc2d7b320b7e602b9d12e47689499d5180a9cc7790dec4d7`  
		Size: 103.0 MB (103031066 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:db05d2e76671d91772a070867bf6f050343319070602a0f8239706d5d4d98387`  
		Last Modified: Wed, 12 Jan 2022 15:14:49 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6271ae84b48476b5c259495509975bd53d7f398555179642c1ef1d612099cb19`  
		Last Modified: Wed, 12 Jan 2022 15:14:48 GMT  
		Size: 4.6 MB (4637258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:178ab94841651126bd3f8a1478a504e44f389c2bf5abf59abafc16f163108f4c`  
		Last Modified: Wed, 12 Jan 2022 15:14:46 GMT  
		Size: 1.8 KB (1759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aa2ac290e2024e6f26c6fd076cc312a10b4842536f9c9daad8ac0e5ecced071`  
		Last Modified: Wed, 12 Jan 2022 15:14:46 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8cb0f84aeae0a7ea0020f00dd7b55f02b772c0bfaa74ea61e1fbd266eff8928`  
		Last Modified: Wed, 12 Jan 2022 15:14:46 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7238bcc9c911d52c987ca07602cb3204bf985a35ae993830fe3b54ea9563de43`  
		Last Modified: Wed, 12 Jan 2022 15:14:46 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.6.6-scratch`

```console
$ docker pull nats@sha256:5d130fed2ad109f922a3a52e45c0b87c0d5a674ad432024cb3d45f898cf425b8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.6.6-scratch` - linux; amd64

```console
$ docker pull nats@sha256:dad4f69520337c2a80d2a9123963c971836f07f530cf4b7c56dde98a622e0a6b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4578170 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ba73da93bdda8525a9f473851ee3de9a2d23c21e1d0a51d7da118bc122df420`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 03 Dec 2021 21:23:03 GMT
COPY file:4070919cac43aa01e3ef5dd95589f24a9d649dcc7b4d6364927c764b1f90392e in /nats-server 
# Fri, 03 Dec 2021 21:23:04 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 03 Dec 2021 21:23:04 GMT
EXPOSE 4222 6222 8222
# Fri, 03 Dec 2021 21:23:04 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 03 Dec 2021 21:23:04 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:730cae3de796bb1fbb06f0f847317c2b738bf9af9d1233daafcf2f708eade5ec`  
		Last Modified: Fri, 03 Dec 2021 21:24:01 GMT  
		Size: 4.6 MB (4577696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39027e71725d02ee81938943fd0f3e980f01abbe21c5e8f8ea8219687aaae862`  
		Last Modified: Fri, 03 Dec 2021 21:24:00 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.6.6-scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:54395301fd2f315191df081131cd6d142613d057970268d64480f4706bcaeda3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4241317 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c4851d5f7b19bc49c52879a43236bae3e26e03a8a0f035ec150eed9a723cca5`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 02 Dec 2021 22:50:02 GMT
COPY file:6036f30fae4132d78e941219bf965a4e4c3e6d898ac912ab22e7a0cc98adf5a5 in /nats-server 
# Thu, 02 Dec 2021 22:50:03 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 02 Dec 2021 22:50:03 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Dec 2021 22:50:04 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 02 Dec 2021 22:50:04 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:41ef8f0f5e4d1f0e1880325ac8c2ccde63d323e6ead77b97c1225e0ce1d226ce`  
		Last Modified: Thu, 02 Dec 2021 22:52:29 GMT  
		Size: 4.2 MB (4240841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e8f034153e28423592a04f327fe3b69d3d84721cb54631e3ea9dcae375ab0ef`  
		Last Modified: Thu, 02 Dec 2021 22:52:26 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.6.6-scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:78ee1d57413d89c46e808dbb121ad895537b74af783c6e6189366afa07638b66
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4237689 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b3276dd6f6de73a2af8ca0c6bd2dc88c7f7ae0a0ce334bcae39c14047aab540`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 04 Dec 2021 07:52:28 GMT
COPY file:025e99b21a301a69c768cc2c72e67c371165b6314d59d0a5a95958216fd24eac in /nats-server 
# Sat, 04 Dec 2021 07:52:28 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Sat, 04 Dec 2021 07:52:29 GMT
EXPOSE 4222 6222 8222
# Sat, 04 Dec 2021 07:52:29 GMT
ENTRYPOINT ["/nats-server"]
# Sat, 04 Dec 2021 07:52:30 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:75a8e365d6e58c8d8f7fe944a206f76f3e800542aca1b53e849c4bffc78fd22d`  
		Last Modified: Sat, 04 Dec 2021 07:55:01 GMT  
		Size: 4.2 MB (4237211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc2920e0912e6a42ee2fd0b7b8b31c6cca01c6c99f16c760f904492422ff7cae`  
		Last Modified: Sat, 04 Dec 2021 07:54:58 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.6.6-scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:8ecffb2097f683980b94450d536a99c79b3fe7654f8bc91fd1c45ad0825e6aae
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4189764 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90bb404fba49386fc48ceb05ee04604d317ff225da69f159d0bd4cc63a930c0e`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 03 Dec 2021 16:57:31 GMT
COPY file:b5f62686ba6debf89a42d2be7c4442db5f8735dba6b8932e6f01f315a2e63e27 in /nats-server 
# Fri, 03 Dec 2021 16:57:32 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 03 Dec 2021 16:57:32 GMT
EXPOSE 4222 6222 8222
# Fri, 03 Dec 2021 16:57:33 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 03 Dec 2021 16:57:34 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:44ff62bde832e2b2bca85708fd2fc86d7d6d1f4ca7c58b5d0e18e3d07c9c5bac`  
		Last Modified: Fri, 03 Dec 2021 16:58:50 GMT  
		Size: 4.2 MB (4189288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44dcbc70566b6f8312605c0214812444ccad7a55594fa2e7f0792c21af818ef0`  
		Last Modified: Fri, 03 Dec 2021 16:58:49 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.6.6-windowsservercore`

```console
$ docker pull nats@sha256:24e44e15d62a911e94d6ff5b7e22accfe329f699b42ade9ebb1a5caa3197f373
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.2452; amd64
	-	windows version 10.0.14393.4886; amd64

### `nats:2.6.6-windowsservercore` - windows version 10.0.17763.2452; amd64

```console
$ docker pull nats@sha256:7f3bfcdbda90968d69223b48664ee1ec937a82bce7365c82135785fe353ba699
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2717536770 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4622435affd612664c15aa4fd83b1e45ba56de92d3c7e6dd3dd924adf28111bf`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 07 Jan 2022 22:48:13 GMT
RUN Install update 1809-amd64
# Wed, 12 Jan 2022 13:54:17 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 Jan 2022 15:10:29 GMT
ENV NATS_DOCKERIZED=1
# Wed, 12 Jan 2022 15:10:30 GMT
ENV NATS_SERVER=2.6.6
# Wed, 12 Jan 2022 15:10:32 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.6.6/nats-server-v2.6.6-windows-amd64.zip
# Wed, 12 Jan 2022 15:10:33 GMT
ENV NATS_SERVER_SHASUM=9730ea401beed7ac40aeada0a8dccfb70207bb234202035aad5644e93ec657da
# Wed, 12 Jan 2022 15:11:32 GMT
RUN Set-PSDebug -Trace 2
# Wed, 12 Jan 2022 15:13:24 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 12 Jan 2022 15:13:26 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 12 Jan 2022 15:13:27 GMT
EXPOSE 4222 6222 8222
# Wed, 12 Jan 2022 15:13:28 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 12 Jan 2022 15:13:29 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:635f15ebd5b486e8a00bf217a0574a29550e5bbf08c1d021e1e308100b2e49b5`  
		Size: 993.9 MB (993898043 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:537828534783cff318d36854dbda0683aef7263e437c7c669de4092e1778959c`  
		Last Modified: Wed, 12 Jan 2022 15:14:30 GMT  
		Size: 1.3 KB (1296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9576e7772519d67febb0ceb94d8f22531ea99f0c60c36e67a4f5a497c384f5e0`  
		Last Modified: Wed, 12 Jan 2022 15:14:30 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaf1f761c394ef0da3c3fef1865f52e977d392f3f0b6c0575c3d1341da6cd7e9`  
		Last Modified: Wed, 12 Jan 2022 15:14:28 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e647346313038e022d4394703013d0963bc45ad0782bcf984166dd279d475c5d`  
		Last Modified: Wed, 12 Jan 2022 15:14:27 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fb56fc761a44bdcdde0f2cfaa2a75932b2ac8fe3c78177727284b0f58037fb0`  
		Last Modified: Wed, 12 Jan 2022 15:14:28 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5797262702f20651c9e1f79f4fbfbe22a260dc9bb7408bf5820eb186b3063f4d`  
		Last Modified: Wed, 12 Jan 2022 15:14:27 GMT  
		Size: 338.2 KB (338250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24cad06e122fd976b54af5acb5a3ba1d1299d61be733e7c2eadeb185aca82942`  
		Last Modified: Wed, 12 Jan 2022 15:14:31 GMT  
		Size: 5.0 MB (4954480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:886cf217b75c847a9ef63c4cc6093d9aa9c783f67b2c999fb7b23249e80b6e6c`  
		Last Modified: Wed, 12 Jan 2022 15:14:25 GMT  
		Size: 1.9 KB (1941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f1f92fb92be2d3b29fc1f42015a4d47bb112ae53db5fab9fa63f432838b7747`  
		Last Modified: Wed, 12 Jan 2022 15:14:25 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:099a82c04f8e6eee73daaccc93d0ad74009ffb4c94eb7d9c8a6a52b4e6bdf2fd`  
		Last Modified: Wed, 12 Jan 2022 15:14:25 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:507bd2ef766612deffd70102b577c1242165b07a8464313f8454713360560c86`  
		Last Modified: Wed, 12 Jan 2022 15:14:25 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.6.6-windowsservercore` - windows version 10.0.14393.4886; amd64

```console
$ docker pull nats@sha256:e476d11dde611fc9b39eb6a45798c2e503fa1bfa4ece59509826bfaed6a4cbe1
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6283541821 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:084594550a22f2aa624e5b2e740a29366a6846c2e1f194854e6e32270f5f0edb`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Thu, 06 Jan 2022 14:33:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 11 Jan 2022 19:57:39 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Tue, 11 Jan 2022 19:57:40 GMT
ENV NATS_DOCKERIZED=1
# Tue, 11 Jan 2022 21:15:53 GMT
ENV NATS_SERVER=2.6.6
# Tue, 11 Jan 2022 21:15:55 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.6.6/nats-server-v2.6.6-windows-amd64.zip
# Tue, 11 Jan 2022 21:15:56 GMT
ENV NATS_SERVER_SHASUM=9730ea401beed7ac40aeada0a8dccfb70207bb234202035aad5644e93ec657da
# Tue, 11 Jan 2022 21:16:48 GMT
RUN Set-PSDebug -Trace 2
# Tue, 11 Jan 2022 21:18:24 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Tue, 11 Jan 2022 21:18:25 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Tue, 11 Jan 2022 21:18:26 GMT
EXPOSE 4222 6222 8222
# Tue, 11 Jan 2022 21:18:28 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 11 Jan 2022 21:18:29 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8428508ffd63b4af1ba690ec41e82a116f10ec6c3fb70962348f5448d42e5835`  
		Size: 2.2 GB (2208216859 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:25aec0a6b64c784bf7521344203ee5def4d38eedfdd68f4b452d3250b5b9ddcf`  
		Last Modified: Tue, 11 Jan 2022 21:19:46 GMT  
		Size: 1.3 KB (1327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3fffdd310a93f98578e45ffbf8e22c031b37efefcc042f21d2a63c2a77c4ee3`  
		Last Modified: Tue, 11 Jan 2022 21:19:45 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15052497c858a1a8b4a8159d05850fbf43551aad161e61ae0fd6880c46eb4556`  
		Last Modified: Tue, 11 Jan 2022 21:19:44 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:080911a4b1ac40e1f062d68ed70319860e88ecb9abec2aef41d0bc3bae89098d`  
		Last Modified: Tue, 11 Jan 2022 21:19:44 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e79cea19a92f33c59acbcc8f501e9acdb5985bbad5b03ccd1190848ae1b4cf1`  
		Last Modified: Tue, 11 Jan 2022 21:19:44 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae0544e04ecd7b6afc6366924310fd892736faf1983ea2ee9e40efd31a0ec502`  
		Last Modified: Tue, 11 Jan 2022 21:19:44 GMT  
		Size: 337.0 KB (337010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8906d4ca25b04680081cc6af81b8eec86a9756abb72e21ed2785f82372ba7c58`  
		Last Modified: Tue, 11 Jan 2022 21:19:43 GMT  
		Size: 5.0 MB (4988964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99a01b43c4c8c06f528a3080b9f4d396d196ff851a603ac22c9ce560c3d5b082`  
		Last Modified: Tue, 11 Jan 2022 21:19:42 GMT  
		Size: 2.0 KB (1973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e156e4bebcfed633295afa0f9dacd6146736cb7de973581f01931fdf6d5f5ae`  
		Last Modified: Tue, 11 Jan 2022 21:19:41 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf3ee9fcf4be90533587d2a54238465fc8f6bad0744784041f675b2e97a93bb9`  
		Last Modified: Tue, 11 Jan 2022 21:19:42 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6e44c694323da6f62bebd7b52b659731c89b1e15c15e5c345ec43e24cba28f7`  
		Last Modified: Tue, 11 Jan 2022 21:19:41 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.6.6-windowsservercore-1809`

```console
$ docker pull nats@sha256:688fa8edbb0b5931af887d0ab00ed77da3f9e8505225dc1eccf15672638fd7a7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2452; amd64

### `nats:2.6.6-windowsservercore-1809` - windows version 10.0.17763.2452; amd64

```console
$ docker pull nats@sha256:7f3bfcdbda90968d69223b48664ee1ec937a82bce7365c82135785fe353ba699
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2717536770 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4622435affd612664c15aa4fd83b1e45ba56de92d3c7e6dd3dd924adf28111bf`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 07 Jan 2022 22:48:13 GMT
RUN Install update 1809-amd64
# Wed, 12 Jan 2022 13:54:17 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 Jan 2022 15:10:29 GMT
ENV NATS_DOCKERIZED=1
# Wed, 12 Jan 2022 15:10:30 GMT
ENV NATS_SERVER=2.6.6
# Wed, 12 Jan 2022 15:10:32 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.6.6/nats-server-v2.6.6-windows-amd64.zip
# Wed, 12 Jan 2022 15:10:33 GMT
ENV NATS_SERVER_SHASUM=9730ea401beed7ac40aeada0a8dccfb70207bb234202035aad5644e93ec657da
# Wed, 12 Jan 2022 15:11:32 GMT
RUN Set-PSDebug -Trace 2
# Wed, 12 Jan 2022 15:13:24 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 12 Jan 2022 15:13:26 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 12 Jan 2022 15:13:27 GMT
EXPOSE 4222 6222 8222
# Wed, 12 Jan 2022 15:13:28 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 12 Jan 2022 15:13:29 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:635f15ebd5b486e8a00bf217a0574a29550e5bbf08c1d021e1e308100b2e49b5`  
		Size: 993.9 MB (993898043 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:537828534783cff318d36854dbda0683aef7263e437c7c669de4092e1778959c`  
		Last Modified: Wed, 12 Jan 2022 15:14:30 GMT  
		Size: 1.3 KB (1296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9576e7772519d67febb0ceb94d8f22531ea99f0c60c36e67a4f5a497c384f5e0`  
		Last Modified: Wed, 12 Jan 2022 15:14:30 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaf1f761c394ef0da3c3fef1865f52e977d392f3f0b6c0575c3d1341da6cd7e9`  
		Last Modified: Wed, 12 Jan 2022 15:14:28 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e647346313038e022d4394703013d0963bc45ad0782bcf984166dd279d475c5d`  
		Last Modified: Wed, 12 Jan 2022 15:14:27 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fb56fc761a44bdcdde0f2cfaa2a75932b2ac8fe3c78177727284b0f58037fb0`  
		Last Modified: Wed, 12 Jan 2022 15:14:28 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5797262702f20651c9e1f79f4fbfbe22a260dc9bb7408bf5820eb186b3063f4d`  
		Last Modified: Wed, 12 Jan 2022 15:14:27 GMT  
		Size: 338.2 KB (338250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24cad06e122fd976b54af5acb5a3ba1d1299d61be733e7c2eadeb185aca82942`  
		Last Modified: Wed, 12 Jan 2022 15:14:31 GMT  
		Size: 5.0 MB (4954480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:886cf217b75c847a9ef63c4cc6093d9aa9c783f67b2c999fb7b23249e80b6e6c`  
		Last Modified: Wed, 12 Jan 2022 15:14:25 GMT  
		Size: 1.9 KB (1941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f1f92fb92be2d3b29fc1f42015a4d47bb112ae53db5fab9fa63f432838b7747`  
		Last Modified: Wed, 12 Jan 2022 15:14:25 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:099a82c04f8e6eee73daaccc93d0ad74009ffb4c94eb7d9c8a6a52b4e6bdf2fd`  
		Last Modified: Wed, 12 Jan 2022 15:14:25 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:507bd2ef766612deffd70102b577c1242165b07a8464313f8454713360560c86`  
		Last Modified: Wed, 12 Jan 2022 15:14:25 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.6.6-windowsservercore-ltsc2016`

```console
$ docker pull nats@sha256:3d337d85e45c503e13f57109f85de0e1c916fc6781cf7bbd3f40ccffd0fb664b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.14393.4886; amd64

### `nats:2.6.6-windowsservercore-ltsc2016` - windows version 10.0.14393.4886; amd64

```console
$ docker pull nats@sha256:e476d11dde611fc9b39eb6a45798c2e503fa1bfa4ece59509826bfaed6a4cbe1
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6283541821 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:084594550a22f2aa624e5b2e740a29366a6846c2e1f194854e6e32270f5f0edb`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Thu, 06 Jan 2022 14:33:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 11 Jan 2022 19:57:39 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Tue, 11 Jan 2022 19:57:40 GMT
ENV NATS_DOCKERIZED=1
# Tue, 11 Jan 2022 21:15:53 GMT
ENV NATS_SERVER=2.6.6
# Tue, 11 Jan 2022 21:15:55 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.6.6/nats-server-v2.6.6-windows-amd64.zip
# Tue, 11 Jan 2022 21:15:56 GMT
ENV NATS_SERVER_SHASUM=9730ea401beed7ac40aeada0a8dccfb70207bb234202035aad5644e93ec657da
# Tue, 11 Jan 2022 21:16:48 GMT
RUN Set-PSDebug -Trace 2
# Tue, 11 Jan 2022 21:18:24 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Tue, 11 Jan 2022 21:18:25 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Tue, 11 Jan 2022 21:18:26 GMT
EXPOSE 4222 6222 8222
# Tue, 11 Jan 2022 21:18:28 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 11 Jan 2022 21:18:29 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8428508ffd63b4af1ba690ec41e82a116f10ec6c3fb70962348f5448d42e5835`  
		Size: 2.2 GB (2208216859 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:25aec0a6b64c784bf7521344203ee5def4d38eedfdd68f4b452d3250b5b9ddcf`  
		Last Modified: Tue, 11 Jan 2022 21:19:46 GMT  
		Size: 1.3 KB (1327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3fffdd310a93f98578e45ffbf8e22c031b37efefcc042f21d2a63c2a77c4ee3`  
		Last Modified: Tue, 11 Jan 2022 21:19:45 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15052497c858a1a8b4a8159d05850fbf43551aad161e61ae0fd6880c46eb4556`  
		Last Modified: Tue, 11 Jan 2022 21:19:44 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:080911a4b1ac40e1f062d68ed70319860e88ecb9abec2aef41d0bc3bae89098d`  
		Last Modified: Tue, 11 Jan 2022 21:19:44 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e79cea19a92f33c59acbcc8f501e9acdb5985bbad5b03ccd1190848ae1b4cf1`  
		Last Modified: Tue, 11 Jan 2022 21:19:44 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae0544e04ecd7b6afc6366924310fd892736faf1983ea2ee9e40efd31a0ec502`  
		Last Modified: Tue, 11 Jan 2022 21:19:44 GMT  
		Size: 337.0 KB (337010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8906d4ca25b04680081cc6af81b8eec86a9756abb72e21ed2785f82372ba7c58`  
		Last Modified: Tue, 11 Jan 2022 21:19:43 GMT  
		Size: 5.0 MB (4988964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99a01b43c4c8c06f528a3080b9f4d396d196ff851a603ac22c9ce560c3d5b082`  
		Last Modified: Tue, 11 Jan 2022 21:19:42 GMT  
		Size: 2.0 KB (1973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e156e4bebcfed633295afa0f9dacd6146736cb7de973581f01931fdf6d5f5ae`  
		Last Modified: Tue, 11 Jan 2022 21:19:41 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf3ee9fcf4be90533587d2a54238465fc8f6bad0744784041f675b2e97a93bb9`  
		Last Modified: Tue, 11 Jan 2022 21:19:42 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6e44c694323da6f62bebd7b52b659731c89b1e15c15e5c345ec43e24cba28f7`  
		Last Modified: Tue, 11 Jan 2022 21:19:41 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:alpine`

```console
$ docker pull nats@sha256:8e2e34eb798631cd76f341277f529f78618a2366d81b59586d3b81f6cb839b25
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:alpine` - linux; amd64

```console
$ docker pull nats@sha256:687f39ecdab1eeda8a4eaa7b7210586d96698faa5e5e7e47aaf5ef8084d504e5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.7 MB (7689543 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c5dc2cfb512e016e62911eca35c050a2eb5ca4b783d5f2d413ba64c68c420bd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:44 GMT
ADD file:762c899ec0505d1a32930ee804c5b008825f41611161be104076cba33b7e5b2b in / 
# Fri, 12 Nov 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 03 Dec 2021 21:22:18 GMT
ENV NATS_SERVER=2.6.6
# Fri, 03 Dec 2021 21:22:21 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='70da0ad3694aebfc742f9aae919d3a4aa5b8c863946e99c5d332195fbbdad49c' ;; 		armhf) natsArch='arm6'; sha256='e2cc1e198d5d5c83e2f2c2dcb15fafb71601603e3740065682812afaa7dd443a' ;; 		armv7) natsArch='arm7'; sha256='f3698a4fb18c6664d477b920d5f07637141a6623cf2fa998900155fea0d97e61' ;; 		x86_64) natsArch='amd64'; sha256='2c2fc16322fb2bc0b166ee2a01e163d4beb2cf7b49d083cebcd36695dc05a381' ;; 		x86) natsArch='386'; sha256='1da03b0d163dc98209f010bf6efa5fc6c81a23b4bab7a98bebe142e19fc26bdc' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 03 Dec 2021 21:22:21 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 03 Dec 2021 21:22:22 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 03 Dec 2021 21:22:22 GMT
EXPOSE 4222 6222 8222
# Fri, 03 Dec 2021 21:22:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 03 Dec 2021 21:22:22 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:97518928ae5f3d52d4164b314a7e73654eb686ecd8aafa0b79acd980773a740d`  
		Last Modified: Fri, 12 Nov 2021 17:20:39 GMT  
		Size: 2.8 MB (2822981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daeb19d8d614f4a1df58ed04d3c72469fa9f7286c9d5482ee274405723b5e645`  
		Last Modified: Fri, 03 Dec 2021 21:23:37 GMT  
		Size: 4.9 MB (4865593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e51c3679390c1ab0c5f5e6786505ad9278d45683059fc7fac0298dcbb6dede86`  
		Last Modified: Fri, 03 Dec 2021 21:23:36 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b14f15cf01b25470e7340acc8ca0860eb4a00a7e1b5d5180bd7c23db1dd273af`  
		Last Modified: Fri, 03 Dec 2021 21:23:36 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:d42d25248435c99492dd0fbcd97688486c692c680069bc9a1eb8a7b1c85eebff
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7161537 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ae84a8c7e689bc4d7fd2915ef9aaf1fb624c094cb183af5863d4b20984f29cd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 12 Nov 2021 16:49:42 GMT
ADD file:6daf1fe862c00673bf9cf4d7e20b0bf253a56e7fb8ed5e730a4466ab9186e18a in / 
# Fri, 12 Nov 2021 16:49:44 GMT
CMD ["/bin/sh"]
# Thu, 02 Dec 2021 22:49:35 GMT
ENV NATS_SERVER=2.6.6
# Thu, 02 Dec 2021 22:49:39 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='70da0ad3694aebfc742f9aae919d3a4aa5b8c863946e99c5d332195fbbdad49c' ;; 		armhf) natsArch='arm6'; sha256='e2cc1e198d5d5c83e2f2c2dcb15fafb71601603e3740065682812afaa7dd443a' ;; 		armv7) natsArch='arm7'; sha256='f3698a4fb18c6664d477b920d5f07637141a6623cf2fa998900155fea0d97e61' ;; 		x86_64) natsArch='amd64'; sha256='2c2fc16322fb2bc0b166ee2a01e163d4beb2cf7b49d083cebcd36695dc05a381' ;; 		x86) natsArch='386'; sha256='1da03b0d163dc98209f010bf6efa5fc6c81a23b4bab7a98bebe142e19fc26bdc' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 02 Dec 2021 22:49:40 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 02 Dec 2021 22:49:40 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 02 Dec 2021 22:49:41 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Dec 2021 22:49:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 02 Dec 2021 22:49:42 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:56afcfda5d78cc243287acbaad250c5e8c0f47aae620dd7c51985b0d3c9b2728`  
		Last Modified: Fri, 12 Nov 2021 16:51:32 GMT  
		Size: 2.6 MB (2635392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3c7b89c441a056fc0e4d867cd4fd28308f188bd0f6b306e5feee96fee47cbdf`  
		Last Modified: Thu, 02 Dec 2021 22:51:52 GMT  
		Size: 4.5 MB (4525169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f67a5f3b97f233f2d6d30a90acd85b9e856cb9b98c298b71e2b5cbae3e0268cf`  
		Last Modified: Thu, 02 Dec 2021 22:51:50 GMT  
		Size: 561.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:706486ffe19b237b40203ebf10cb1110d7566cba5a3c10bf738be70173a1aa69`  
		Last Modified: Thu, 02 Dec 2021 22:51:50 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:dbc345345cfc225bd88b35e80f85f412483db712134bde3a0e4d959cb543350f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.0 MB (6958146 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6aaa47180fd5390c3f39b81e39db30c26897fc1b070c064d4677ebdd14c1f801`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 12 Nov 2021 16:57:35 GMT
ADD file:03e0720458c3475758bf4394afa56f2165198eb91e6e9581f7768e433744dd9b in / 
# Fri, 12 Nov 2021 16:57:36 GMT
CMD ["/bin/sh"]
# Sat, 04 Dec 2021 07:51:50 GMT
ENV NATS_SERVER=2.6.6
# Sat, 04 Dec 2021 07:51:54 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='70da0ad3694aebfc742f9aae919d3a4aa5b8c863946e99c5d332195fbbdad49c' ;; 		armhf) natsArch='arm6'; sha256='e2cc1e198d5d5c83e2f2c2dcb15fafb71601603e3740065682812afaa7dd443a' ;; 		armv7) natsArch='arm7'; sha256='f3698a4fb18c6664d477b920d5f07637141a6623cf2fa998900155fea0d97e61' ;; 		x86_64) natsArch='amd64'; sha256='2c2fc16322fb2bc0b166ee2a01e163d4beb2cf7b49d083cebcd36695dc05a381' ;; 		x86) natsArch='386'; sha256='1da03b0d163dc98209f010bf6efa5fc6c81a23b4bab7a98bebe142e19fc26bdc' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Sat, 04 Dec 2021 07:51:55 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Sat, 04 Dec 2021 07:51:55 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Sat, 04 Dec 2021 07:51:56 GMT
EXPOSE 4222 6222 8222
# Sat, 04 Dec 2021 07:51:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 04 Dec 2021 07:51:57 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:764d2e53e1a607f2d8261522185d5b9021ade3ec1a595664ee90308c00176899`  
		Last Modified: Fri, 12 Nov 2021 16:59:33 GMT  
		Size: 2.4 MB (2438618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:157eac698795baeacb3153cf2bbbc17f348e477e8062fa45b6728e97dd02e157`  
		Last Modified: Sat, 04 Dec 2021 07:54:19 GMT  
		Size: 4.5 MB (4518555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b5241fcba964a14f9c4681ebcc94815a476df86f68c628494f5759a3bee8514`  
		Last Modified: Sat, 04 Dec 2021 07:54:16 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36d02df08ee2f75a857120c105153a83b2b951337a87e902260e70e1de20dfd0`  
		Last Modified: Sat, 04 Dec 2021 07:54:16 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:f1e7262504ed73a185ee16f6a6da14c19c3a76120f2b22c51a051a0988ac3bdc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7193478 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55e483df89c189235b79aa4a9d2417378172236dba6fa85f6d5a0bb35756835f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 12 Nov 2021 16:39:58 GMT
ADD file:400c0466b29ccad54e0f6c0acef22542992828678c96693ef1f9f4d0551935d8 in / 
# Fri, 12 Nov 2021 16:39:58 GMT
CMD ["/bin/sh"]
# Fri, 03 Dec 2021 16:57:10 GMT
ENV NATS_SERVER=2.6.6
# Fri, 03 Dec 2021 16:57:13 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='70da0ad3694aebfc742f9aae919d3a4aa5b8c863946e99c5d332195fbbdad49c' ;; 		armhf) natsArch='arm6'; sha256='e2cc1e198d5d5c83e2f2c2dcb15fafb71601603e3740065682812afaa7dd443a' ;; 		armv7) natsArch='arm7'; sha256='f3698a4fb18c6664d477b920d5f07637141a6623cf2fa998900155fea0d97e61' ;; 		x86_64) natsArch='amd64'; sha256='2c2fc16322fb2bc0b166ee2a01e163d4beb2cf7b49d083cebcd36695dc05a381' ;; 		x86) natsArch='386'; sha256='1da03b0d163dc98209f010bf6efa5fc6c81a23b4bab7a98bebe142e19fc26bdc' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 03 Dec 2021 16:57:15 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 03 Dec 2021 16:57:16 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 03 Dec 2021 16:57:16 GMT
EXPOSE 4222 6222 8222
# Fri, 03 Dec 2021 16:57:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 03 Dec 2021 16:57:18 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:be307f383ecc62b27a29b599c3fc9d3129693a798e7fcce614f09174cfe2d354`  
		Last Modified: Fri, 12 Nov 2021 16:40:59 GMT  
		Size: 2.7 MB (2717700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdee3b2a5421d3ceb50b8101857ce4c0815c4532476e1f292867c63034c08f61`  
		Last Modified: Fri, 03 Dec 2021 16:58:22 GMT  
		Size: 4.5 MB (4474835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8a771880289bb86cd368ca8b39620b0cfe69694646e061ff6975f959ccfcd29`  
		Last Modified: Fri, 03 Dec 2021 16:58:21 GMT  
		Size: 528.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:438c5abdffd6599ac83fe661d26a9491552d63f48aeb9147609299ee11b78c78`  
		Last Modified: Fri, 03 Dec 2021 16:58:21 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:alpine3.14`

```console
$ docker pull nats@sha256:8e2e34eb798631cd76f341277f529f78618a2366d81b59586d3b81f6cb839b25
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:alpine3.14` - linux; amd64

```console
$ docker pull nats@sha256:687f39ecdab1eeda8a4eaa7b7210586d96698faa5e5e7e47aaf5ef8084d504e5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.7 MB (7689543 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c5dc2cfb512e016e62911eca35c050a2eb5ca4b783d5f2d413ba64c68c420bd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:44 GMT
ADD file:762c899ec0505d1a32930ee804c5b008825f41611161be104076cba33b7e5b2b in / 
# Fri, 12 Nov 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 03 Dec 2021 21:22:18 GMT
ENV NATS_SERVER=2.6.6
# Fri, 03 Dec 2021 21:22:21 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='70da0ad3694aebfc742f9aae919d3a4aa5b8c863946e99c5d332195fbbdad49c' ;; 		armhf) natsArch='arm6'; sha256='e2cc1e198d5d5c83e2f2c2dcb15fafb71601603e3740065682812afaa7dd443a' ;; 		armv7) natsArch='arm7'; sha256='f3698a4fb18c6664d477b920d5f07637141a6623cf2fa998900155fea0d97e61' ;; 		x86_64) natsArch='amd64'; sha256='2c2fc16322fb2bc0b166ee2a01e163d4beb2cf7b49d083cebcd36695dc05a381' ;; 		x86) natsArch='386'; sha256='1da03b0d163dc98209f010bf6efa5fc6c81a23b4bab7a98bebe142e19fc26bdc' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 03 Dec 2021 21:22:21 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 03 Dec 2021 21:22:22 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 03 Dec 2021 21:22:22 GMT
EXPOSE 4222 6222 8222
# Fri, 03 Dec 2021 21:22:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 03 Dec 2021 21:22:22 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:97518928ae5f3d52d4164b314a7e73654eb686ecd8aafa0b79acd980773a740d`  
		Last Modified: Fri, 12 Nov 2021 17:20:39 GMT  
		Size: 2.8 MB (2822981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daeb19d8d614f4a1df58ed04d3c72469fa9f7286c9d5482ee274405723b5e645`  
		Last Modified: Fri, 03 Dec 2021 21:23:37 GMT  
		Size: 4.9 MB (4865593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e51c3679390c1ab0c5f5e6786505ad9278d45683059fc7fac0298dcbb6dede86`  
		Last Modified: Fri, 03 Dec 2021 21:23:36 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b14f15cf01b25470e7340acc8ca0860eb4a00a7e1b5d5180bd7c23db1dd273af`  
		Last Modified: Fri, 03 Dec 2021 21:23:36 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.14` - linux; arm variant v6

```console
$ docker pull nats@sha256:d42d25248435c99492dd0fbcd97688486c692c680069bc9a1eb8a7b1c85eebff
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7161537 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ae84a8c7e689bc4d7fd2915ef9aaf1fb624c094cb183af5863d4b20984f29cd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 12 Nov 2021 16:49:42 GMT
ADD file:6daf1fe862c00673bf9cf4d7e20b0bf253a56e7fb8ed5e730a4466ab9186e18a in / 
# Fri, 12 Nov 2021 16:49:44 GMT
CMD ["/bin/sh"]
# Thu, 02 Dec 2021 22:49:35 GMT
ENV NATS_SERVER=2.6.6
# Thu, 02 Dec 2021 22:49:39 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='70da0ad3694aebfc742f9aae919d3a4aa5b8c863946e99c5d332195fbbdad49c' ;; 		armhf) natsArch='arm6'; sha256='e2cc1e198d5d5c83e2f2c2dcb15fafb71601603e3740065682812afaa7dd443a' ;; 		armv7) natsArch='arm7'; sha256='f3698a4fb18c6664d477b920d5f07637141a6623cf2fa998900155fea0d97e61' ;; 		x86_64) natsArch='amd64'; sha256='2c2fc16322fb2bc0b166ee2a01e163d4beb2cf7b49d083cebcd36695dc05a381' ;; 		x86) natsArch='386'; sha256='1da03b0d163dc98209f010bf6efa5fc6c81a23b4bab7a98bebe142e19fc26bdc' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 02 Dec 2021 22:49:40 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 02 Dec 2021 22:49:40 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 02 Dec 2021 22:49:41 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Dec 2021 22:49:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 02 Dec 2021 22:49:42 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:56afcfda5d78cc243287acbaad250c5e8c0f47aae620dd7c51985b0d3c9b2728`  
		Last Modified: Fri, 12 Nov 2021 16:51:32 GMT  
		Size: 2.6 MB (2635392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3c7b89c441a056fc0e4d867cd4fd28308f188bd0f6b306e5feee96fee47cbdf`  
		Last Modified: Thu, 02 Dec 2021 22:51:52 GMT  
		Size: 4.5 MB (4525169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f67a5f3b97f233f2d6d30a90acd85b9e856cb9b98c298b71e2b5cbae3e0268cf`  
		Last Modified: Thu, 02 Dec 2021 22:51:50 GMT  
		Size: 561.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:706486ffe19b237b40203ebf10cb1110d7566cba5a3c10bf738be70173a1aa69`  
		Last Modified: Thu, 02 Dec 2021 22:51:50 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.14` - linux; arm variant v7

```console
$ docker pull nats@sha256:dbc345345cfc225bd88b35e80f85f412483db712134bde3a0e4d959cb543350f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.0 MB (6958146 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6aaa47180fd5390c3f39b81e39db30c26897fc1b070c064d4677ebdd14c1f801`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 12 Nov 2021 16:57:35 GMT
ADD file:03e0720458c3475758bf4394afa56f2165198eb91e6e9581f7768e433744dd9b in / 
# Fri, 12 Nov 2021 16:57:36 GMT
CMD ["/bin/sh"]
# Sat, 04 Dec 2021 07:51:50 GMT
ENV NATS_SERVER=2.6.6
# Sat, 04 Dec 2021 07:51:54 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='70da0ad3694aebfc742f9aae919d3a4aa5b8c863946e99c5d332195fbbdad49c' ;; 		armhf) natsArch='arm6'; sha256='e2cc1e198d5d5c83e2f2c2dcb15fafb71601603e3740065682812afaa7dd443a' ;; 		armv7) natsArch='arm7'; sha256='f3698a4fb18c6664d477b920d5f07637141a6623cf2fa998900155fea0d97e61' ;; 		x86_64) natsArch='amd64'; sha256='2c2fc16322fb2bc0b166ee2a01e163d4beb2cf7b49d083cebcd36695dc05a381' ;; 		x86) natsArch='386'; sha256='1da03b0d163dc98209f010bf6efa5fc6c81a23b4bab7a98bebe142e19fc26bdc' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Sat, 04 Dec 2021 07:51:55 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Sat, 04 Dec 2021 07:51:55 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Sat, 04 Dec 2021 07:51:56 GMT
EXPOSE 4222 6222 8222
# Sat, 04 Dec 2021 07:51:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 04 Dec 2021 07:51:57 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:764d2e53e1a607f2d8261522185d5b9021ade3ec1a595664ee90308c00176899`  
		Last Modified: Fri, 12 Nov 2021 16:59:33 GMT  
		Size: 2.4 MB (2438618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:157eac698795baeacb3153cf2bbbc17f348e477e8062fa45b6728e97dd02e157`  
		Last Modified: Sat, 04 Dec 2021 07:54:19 GMT  
		Size: 4.5 MB (4518555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b5241fcba964a14f9c4681ebcc94815a476df86f68c628494f5759a3bee8514`  
		Last Modified: Sat, 04 Dec 2021 07:54:16 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36d02df08ee2f75a857120c105153a83b2b951337a87e902260e70e1de20dfd0`  
		Last Modified: Sat, 04 Dec 2021 07:54:16 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.14` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:f1e7262504ed73a185ee16f6a6da14c19c3a76120f2b22c51a051a0988ac3bdc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7193478 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55e483df89c189235b79aa4a9d2417378172236dba6fa85f6d5a0bb35756835f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 12 Nov 2021 16:39:58 GMT
ADD file:400c0466b29ccad54e0f6c0acef22542992828678c96693ef1f9f4d0551935d8 in / 
# Fri, 12 Nov 2021 16:39:58 GMT
CMD ["/bin/sh"]
# Fri, 03 Dec 2021 16:57:10 GMT
ENV NATS_SERVER=2.6.6
# Fri, 03 Dec 2021 16:57:13 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='70da0ad3694aebfc742f9aae919d3a4aa5b8c863946e99c5d332195fbbdad49c' ;; 		armhf) natsArch='arm6'; sha256='e2cc1e198d5d5c83e2f2c2dcb15fafb71601603e3740065682812afaa7dd443a' ;; 		armv7) natsArch='arm7'; sha256='f3698a4fb18c6664d477b920d5f07637141a6623cf2fa998900155fea0d97e61' ;; 		x86_64) natsArch='amd64'; sha256='2c2fc16322fb2bc0b166ee2a01e163d4beb2cf7b49d083cebcd36695dc05a381' ;; 		x86) natsArch='386'; sha256='1da03b0d163dc98209f010bf6efa5fc6c81a23b4bab7a98bebe142e19fc26bdc' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 03 Dec 2021 16:57:15 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 03 Dec 2021 16:57:16 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 03 Dec 2021 16:57:16 GMT
EXPOSE 4222 6222 8222
# Fri, 03 Dec 2021 16:57:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 03 Dec 2021 16:57:18 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:be307f383ecc62b27a29b599c3fc9d3129693a798e7fcce614f09174cfe2d354`  
		Last Modified: Fri, 12 Nov 2021 16:40:59 GMT  
		Size: 2.7 MB (2717700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdee3b2a5421d3ceb50b8101857ce4c0815c4532476e1f292867c63034c08f61`  
		Last Modified: Fri, 03 Dec 2021 16:58:22 GMT  
		Size: 4.5 MB (4474835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8a771880289bb86cd368ca8b39620b0cfe69694646e061ff6975f959ccfcd29`  
		Last Modified: Fri, 03 Dec 2021 16:58:21 GMT  
		Size: 528.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:438c5abdffd6599ac83fe661d26a9491552d63f48aeb9147609299ee11b78c78`  
		Last Modified: Fri, 03 Dec 2021 16:58:21 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:latest`

```console
$ docker pull nats@sha256:9bd747193a9d316341136227475dbde257fe33d6209b7b43beaf16ae0a358865
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.2452; amd64

### `nats:latest` - linux; amd64

```console
$ docker pull nats@sha256:dad4f69520337c2a80d2a9123963c971836f07f530cf4b7c56dde98a622e0a6b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4578170 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ba73da93bdda8525a9f473851ee3de9a2d23c21e1d0a51d7da118bc122df420`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 03 Dec 2021 21:23:03 GMT
COPY file:4070919cac43aa01e3ef5dd95589f24a9d649dcc7b4d6364927c764b1f90392e in /nats-server 
# Fri, 03 Dec 2021 21:23:04 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 03 Dec 2021 21:23:04 GMT
EXPOSE 4222 6222 8222
# Fri, 03 Dec 2021 21:23:04 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 03 Dec 2021 21:23:04 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:730cae3de796bb1fbb06f0f847317c2b738bf9af9d1233daafcf2f708eade5ec`  
		Last Modified: Fri, 03 Dec 2021 21:24:01 GMT  
		Size: 4.6 MB (4577696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39027e71725d02ee81938943fd0f3e980f01abbe21c5e8f8ea8219687aaae862`  
		Last Modified: Fri, 03 Dec 2021 21:24:00 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm variant v6

```console
$ docker pull nats@sha256:54395301fd2f315191df081131cd6d142613d057970268d64480f4706bcaeda3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4241317 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c4851d5f7b19bc49c52879a43236bae3e26e03a8a0f035ec150eed9a723cca5`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 02 Dec 2021 22:50:02 GMT
COPY file:6036f30fae4132d78e941219bf965a4e4c3e6d898ac912ab22e7a0cc98adf5a5 in /nats-server 
# Thu, 02 Dec 2021 22:50:03 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 02 Dec 2021 22:50:03 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Dec 2021 22:50:04 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 02 Dec 2021 22:50:04 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:41ef8f0f5e4d1f0e1880325ac8c2ccde63d323e6ead77b97c1225e0ce1d226ce`  
		Last Modified: Thu, 02 Dec 2021 22:52:29 GMT  
		Size: 4.2 MB (4240841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e8f034153e28423592a04f327fe3b69d3d84721cb54631e3ea9dcae375ab0ef`  
		Last Modified: Thu, 02 Dec 2021 22:52:26 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm variant v7

```console
$ docker pull nats@sha256:78ee1d57413d89c46e808dbb121ad895537b74af783c6e6189366afa07638b66
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4237689 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b3276dd6f6de73a2af8ca0c6bd2dc88c7f7ae0a0ce334bcae39c14047aab540`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 04 Dec 2021 07:52:28 GMT
COPY file:025e99b21a301a69c768cc2c72e67c371165b6314d59d0a5a95958216fd24eac in /nats-server 
# Sat, 04 Dec 2021 07:52:28 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Sat, 04 Dec 2021 07:52:29 GMT
EXPOSE 4222 6222 8222
# Sat, 04 Dec 2021 07:52:29 GMT
ENTRYPOINT ["/nats-server"]
# Sat, 04 Dec 2021 07:52:30 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:75a8e365d6e58c8d8f7fe944a206f76f3e800542aca1b53e849c4bffc78fd22d`  
		Last Modified: Sat, 04 Dec 2021 07:55:01 GMT  
		Size: 4.2 MB (4237211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc2920e0912e6a42ee2fd0b7b8b31c6cca01c6c99f16c760f904492422ff7cae`  
		Last Modified: Sat, 04 Dec 2021 07:54:58 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:8ecffb2097f683980b94450d536a99c79b3fe7654f8bc91fd1c45ad0825e6aae
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4189764 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90bb404fba49386fc48ceb05ee04604d317ff225da69f159d0bd4cc63a930c0e`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 03 Dec 2021 16:57:31 GMT
COPY file:b5f62686ba6debf89a42d2be7c4442db5f8735dba6b8932e6f01f315a2e63e27 in /nats-server 
# Fri, 03 Dec 2021 16:57:32 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 03 Dec 2021 16:57:32 GMT
EXPOSE 4222 6222 8222
# Fri, 03 Dec 2021 16:57:33 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 03 Dec 2021 16:57:34 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:44ff62bde832e2b2bca85708fd2fc86d7d6d1f4ca7c58b5d0e18e3d07c9c5bac`  
		Last Modified: Fri, 03 Dec 2021 16:58:50 GMT  
		Size: 4.2 MB (4189288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44dcbc70566b6f8312605c0214812444ccad7a55594fa2e7f0792c21af818ef0`  
		Last Modified: Fri, 03 Dec 2021 16:58:49 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - windows version 10.0.17763.2452; amd64

```console
$ docker pull nats@sha256:73596edd7d2bcfb546b2b6da26cbaf06733398e7cc550a610ed8e53c5c59021c
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.7 MB (107674705 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa5c572d20b69e54dca9ee7a24b26d6b489d4cd2be1d5931d9accce1dbb7e030`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 07 Jan 2022 22:25:06 GMT
RUN Apply image 1809-amd64
# Wed, 12 Jan 2022 15:13:42 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 12 Jan 2022 15:13:43 GMT
RUN cmd /S /C #(nop) COPY file:20c797e6dad00d7098dbf6d4d158c380fd073bc5fc24a80fd4f23205af77a338 in C:\nats-server.exe 
# Wed, 12 Jan 2022 15:13:44 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 12 Jan 2022 15:13:45 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 12 Jan 2022 15:13:46 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 12 Jan 2022 15:13:47 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3a78847ea829208edc2d7b320b7e602b9d12e47689499d5180a9cc7790dec4d7`  
		Size: 103.0 MB (103031066 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:db05d2e76671d91772a070867bf6f050343319070602a0f8239706d5d4d98387`  
		Last Modified: Wed, 12 Jan 2022 15:14:49 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6271ae84b48476b5c259495509975bd53d7f398555179642c1ef1d612099cb19`  
		Last Modified: Wed, 12 Jan 2022 15:14:48 GMT  
		Size: 4.6 MB (4637258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:178ab94841651126bd3f8a1478a504e44f389c2bf5abf59abafc16f163108f4c`  
		Last Modified: Wed, 12 Jan 2022 15:14:46 GMT  
		Size: 1.8 KB (1759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aa2ac290e2024e6f26c6fd076cc312a10b4842536f9c9daad8ac0e5ecced071`  
		Last Modified: Wed, 12 Jan 2022 15:14:46 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8cb0f84aeae0a7ea0020f00dd7b55f02b772c0bfaa74ea61e1fbd266eff8928`  
		Last Modified: Wed, 12 Jan 2022 15:14:46 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7238bcc9c911d52c987ca07602cb3204bf985a35ae993830fe3b54ea9563de43`  
		Last Modified: Wed, 12 Jan 2022 15:14:46 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:linux`

```console
$ docker pull nats@sha256:5d130fed2ad109f922a3a52e45c0b87c0d5a674ad432024cb3d45f898cf425b8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:linux` - linux; amd64

```console
$ docker pull nats@sha256:dad4f69520337c2a80d2a9123963c971836f07f530cf4b7c56dde98a622e0a6b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4578170 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ba73da93bdda8525a9f473851ee3de9a2d23c21e1d0a51d7da118bc122df420`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 03 Dec 2021 21:23:03 GMT
COPY file:4070919cac43aa01e3ef5dd95589f24a9d649dcc7b4d6364927c764b1f90392e in /nats-server 
# Fri, 03 Dec 2021 21:23:04 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 03 Dec 2021 21:23:04 GMT
EXPOSE 4222 6222 8222
# Fri, 03 Dec 2021 21:23:04 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 03 Dec 2021 21:23:04 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:730cae3de796bb1fbb06f0f847317c2b738bf9af9d1233daafcf2f708eade5ec`  
		Last Modified: Fri, 03 Dec 2021 21:24:01 GMT  
		Size: 4.6 MB (4577696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39027e71725d02ee81938943fd0f3e980f01abbe21c5e8f8ea8219687aaae862`  
		Last Modified: Fri, 03 Dec 2021 21:24:00 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:54395301fd2f315191df081131cd6d142613d057970268d64480f4706bcaeda3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4241317 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c4851d5f7b19bc49c52879a43236bae3e26e03a8a0f035ec150eed9a723cca5`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 02 Dec 2021 22:50:02 GMT
COPY file:6036f30fae4132d78e941219bf965a4e4c3e6d898ac912ab22e7a0cc98adf5a5 in /nats-server 
# Thu, 02 Dec 2021 22:50:03 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 02 Dec 2021 22:50:03 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Dec 2021 22:50:04 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 02 Dec 2021 22:50:04 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:41ef8f0f5e4d1f0e1880325ac8c2ccde63d323e6ead77b97c1225e0ce1d226ce`  
		Last Modified: Thu, 02 Dec 2021 22:52:29 GMT  
		Size: 4.2 MB (4240841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e8f034153e28423592a04f327fe3b69d3d84721cb54631e3ea9dcae375ab0ef`  
		Last Modified: Thu, 02 Dec 2021 22:52:26 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:78ee1d57413d89c46e808dbb121ad895537b74af783c6e6189366afa07638b66
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4237689 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b3276dd6f6de73a2af8ca0c6bd2dc88c7f7ae0a0ce334bcae39c14047aab540`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 04 Dec 2021 07:52:28 GMT
COPY file:025e99b21a301a69c768cc2c72e67c371165b6314d59d0a5a95958216fd24eac in /nats-server 
# Sat, 04 Dec 2021 07:52:28 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Sat, 04 Dec 2021 07:52:29 GMT
EXPOSE 4222 6222 8222
# Sat, 04 Dec 2021 07:52:29 GMT
ENTRYPOINT ["/nats-server"]
# Sat, 04 Dec 2021 07:52:30 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:75a8e365d6e58c8d8f7fe944a206f76f3e800542aca1b53e849c4bffc78fd22d`  
		Last Modified: Sat, 04 Dec 2021 07:55:01 GMT  
		Size: 4.2 MB (4237211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc2920e0912e6a42ee2fd0b7b8b31c6cca01c6c99f16c760f904492422ff7cae`  
		Last Modified: Sat, 04 Dec 2021 07:54:58 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:8ecffb2097f683980b94450d536a99c79b3fe7654f8bc91fd1c45ad0825e6aae
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4189764 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90bb404fba49386fc48ceb05ee04604d317ff225da69f159d0bd4cc63a930c0e`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 03 Dec 2021 16:57:31 GMT
COPY file:b5f62686ba6debf89a42d2be7c4442db5f8735dba6b8932e6f01f315a2e63e27 in /nats-server 
# Fri, 03 Dec 2021 16:57:32 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 03 Dec 2021 16:57:32 GMT
EXPOSE 4222 6222 8222
# Fri, 03 Dec 2021 16:57:33 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 03 Dec 2021 16:57:34 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:44ff62bde832e2b2bca85708fd2fc86d7d6d1f4ca7c58b5d0e18e3d07c9c5bac`  
		Last Modified: Fri, 03 Dec 2021 16:58:50 GMT  
		Size: 4.2 MB (4189288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44dcbc70566b6f8312605c0214812444ccad7a55594fa2e7f0792c21af818ef0`  
		Last Modified: Fri, 03 Dec 2021 16:58:49 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:nanoserver`

```console
$ docker pull nats@sha256:0b2895172f1057f6c9b6bfeb7502714c3bfee379610222e16e17a226fc537354
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2452; amd64

### `nats:nanoserver` - windows version 10.0.17763.2452; amd64

```console
$ docker pull nats@sha256:73596edd7d2bcfb546b2b6da26cbaf06733398e7cc550a610ed8e53c5c59021c
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.7 MB (107674705 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa5c572d20b69e54dca9ee7a24b26d6b489d4cd2be1d5931d9accce1dbb7e030`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 07 Jan 2022 22:25:06 GMT
RUN Apply image 1809-amd64
# Wed, 12 Jan 2022 15:13:42 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 12 Jan 2022 15:13:43 GMT
RUN cmd /S /C #(nop) COPY file:20c797e6dad00d7098dbf6d4d158c380fd073bc5fc24a80fd4f23205af77a338 in C:\nats-server.exe 
# Wed, 12 Jan 2022 15:13:44 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 12 Jan 2022 15:13:45 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 12 Jan 2022 15:13:46 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 12 Jan 2022 15:13:47 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3a78847ea829208edc2d7b320b7e602b9d12e47689499d5180a9cc7790dec4d7`  
		Size: 103.0 MB (103031066 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:db05d2e76671d91772a070867bf6f050343319070602a0f8239706d5d4d98387`  
		Last Modified: Wed, 12 Jan 2022 15:14:49 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6271ae84b48476b5c259495509975bd53d7f398555179642c1ef1d612099cb19`  
		Last Modified: Wed, 12 Jan 2022 15:14:48 GMT  
		Size: 4.6 MB (4637258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:178ab94841651126bd3f8a1478a504e44f389c2bf5abf59abafc16f163108f4c`  
		Last Modified: Wed, 12 Jan 2022 15:14:46 GMT  
		Size: 1.8 KB (1759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aa2ac290e2024e6f26c6fd076cc312a10b4842536f9c9daad8ac0e5ecced071`  
		Last Modified: Wed, 12 Jan 2022 15:14:46 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8cb0f84aeae0a7ea0020f00dd7b55f02b772c0bfaa74ea61e1fbd266eff8928`  
		Last Modified: Wed, 12 Jan 2022 15:14:46 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7238bcc9c911d52c987ca07602cb3204bf985a35ae993830fe3b54ea9563de43`  
		Last Modified: Wed, 12 Jan 2022 15:14:46 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:nanoserver-1809`

```console
$ docker pull nats@sha256:0b2895172f1057f6c9b6bfeb7502714c3bfee379610222e16e17a226fc537354
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2452; amd64

### `nats:nanoserver-1809` - windows version 10.0.17763.2452; amd64

```console
$ docker pull nats@sha256:73596edd7d2bcfb546b2b6da26cbaf06733398e7cc550a610ed8e53c5c59021c
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.7 MB (107674705 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa5c572d20b69e54dca9ee7a24b26d6b489d4cd2be1d5931d9accce1dbb7e030`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 07 Jan 2022 22:25:06 GMT
RUN Apply image 1809-amd64
# Wed, 12 Jan 2022 15:13:42 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 12 Jan 2022 15:13:43 GMT
RUN cmd /S /C #(nop) COPY file:20c797e6dad00d7098dbf6d4d158c380fd073bc5fc24a80fd4f23205af77a338 in C:\nats-server.exe 
# Wed, 12 Jan 2022 15:13:44 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 12 Jan 2022 15:13:45 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 12 Jan 2022 15:13:46 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 12 Jan 2022 15:13:47 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3a78847ea829208edc2d7b320b7e602b9d12e47689499d5180a9cc7790dec4d7`  
		Size: 103.0 MB (103031066 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:db05d2e76671d91772a070867bf6f050343319070602a0f8239706d5d4d98387`  
		Last Modified: Wed, 12 Jan 2022 15:14:49 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6271ae84b48476b5c259495509975bd53d7f398555179642c1ef1d612099cb19`  
		Last Modified: Wed, 12 Jan 2022 15:14:48 GMT  
		Size: 4.6 MB (4637258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:178ab94841651126bd3f8a1478a504e44f389c2bf5abf59abafc16f163108f4c`  
		Last Modified: Wed, 12 Jan 2022 15:14:46 GMT  
		Size: 1.8 KB (1759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aa2ac290e2024e6f26c6fd076cc312a10b4842536f9c9daad8ac0e5ecced071`  
		Last Modified: Wed, 12 Jan 2022 15:14:46 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8cb0f84aeae0a7ea0020f00dd7b55f02b772c0bfaa74ea61e1fbd266eff8928`  
		Last Modified: Wed, 12 Jan 2022 15:14:46 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7238bcc9c911d52c987ca07602cb3204bf985a35ae993830fe3b54ea9563de43`  
		Last Modified: Wed, 12 Jan 2022 15:14:46 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:scratch`

```console
$ docker pull nats@sha256:5d130fed2ad109f922a3a52e45c0b87c0d5a674ad432024cb3d45f898cf425b8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:scratch` - linux; amd64

```console
$ docker pull nats@sha256:dad4f69520337c2a80d2a9123963c971836f07f530cf4b7c56dde98a622e0a6b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4578170 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ba73da93bdda8525a9f473851ee3de9a2d23c21e1d0a51d7da118bc122df420`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 03 Dec 2021 21:23:03 GMT
COPY file:4070919cac43aa01e3ef5dd95589f24a9d649dcc7b4d6364927c764b1f90392e in /nats-server 
# Fri, 03 Dec 2021 21:23:04 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 03 Dec 2021 21:23:04 GMT
EXPOSE 4222 6222 8222
# Fri, 03 Dec 2021 21:23:04 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 03 Dec 2021 21:23:04 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:730cae3de796bb1fbb06f0f847317c2b738bf9af9d1233daafcf2f708eade5ec`  
		Last Modified: Fri, 03 Dec 2021 21:24:01 GMT  
		Size: 4.6 MB (4577696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39027e71725d02ee81938943fd0f3e980f01abbe21c5e8f8ea8219687aaae862`  
		Last Modified: Fri, 03 Dec 2021 21:24:00 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:54395301fd2f315191df081131cd6d142613d057970268d64480f4706bcaeda3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4241317 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c4851d5f7b19bc49c52879a43236bae3e26e03a8a0f035ec150eed9a723cca5`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 02 Dec 2021 22:50:02 GMT
COPY file:6036f30fae4132d78e941219bf965a4e4c3e6d898ac912ab22e7a0cc98adf5a5 in /nats-server 
# Thu, 02 Dec 2021 22:50:03 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 02 Dec 2021 22:50:03 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Dec 2021 22:50:04 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 02 Dec 2021 22:50:04 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:41ef8f0f5e4d1f0e1880325ac8c2ccde63d323e6ead77b97c1225e0ce1d226ce`  
		Last Modified: Thu, 02 Dec 2021 22:52:29 GMT  
		Size: 4.2 MB (4240841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e8f034153e28423592a04f327fe3b69d3d84721cb54631e3ea9dcae375ab0ef`  
		Last Modified: Thu, 02 Dec 2021 22:52:26 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:78ee1d57413d89c46e808dbb121ad895537b74af783c6e6189366afa07638b66
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4237689 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b3276dd6f6de73a2af8ca0c6bd2dc88c7f7ae0a0ce334bcae39c14047aab540`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 04 Dec 2021 07:52:28 GMT
COPY file:025e99b21a301a69c768cc2c72e67c371165b6314d59d0a5a95958216fd24eac in /nats-server 
# Sat, 04 Dec 2021 07:52:28 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Sat, 04 Dec 2021 07:52:29 GMT
EXPOSE 4222 6222 8222
# Sat, 04 Dec 2021 07:52:29 GMT
ENTRYPOINT ["/nats-server"]
# Sat, 04 Dec 2021 07:52:30 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:75a8e365d6e58c8d8f7fe944a206f76f3e800542aca1b53e849c4bffc78fd22d`  
		Last Modified: Sat, 04 Dec 2021 07:55:01 GMT  
		Size: 4.2 MB (4237211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc2920e0912e6a42ee2fd0b7b8b31c6cca01c6c99f16c760f904492422ff7cae`  
		Last Modified: Sat, 04 Dec 2021 07:54:58 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:8ecffb2097f683980b94450d536a99c79b3fe7654f8bc91fd1c45ad0825e6aae
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4189764 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90bb404fba49386fc48ceb05ee04604d317ff225da69f159d0bd4cc63a930c0e`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 03 Dec 2021 16:57:31 GMT
COPY file:b5f62686ba6debf89a42d2be7c4442db5f8735dba6b8932e6f01f315a2e63e27 in /nats-server 
# Fri, 03 Dec 2021 16:57:32 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 03 Dec 2021 16:57:32 GMT
EXPOSE 4222 6222 8222
# Fri, 03 Dec 2021 16:57:33 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 03 Dec 2021 16:57:34 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:44ff62bde832e2b2bca85708fd2fc86d7d6d1f4ca7c58b5d0e18e3d07c9c5bac`  
		Last Modified: Fri, 03 Dec 2021 16:58:50 GMT  
		Size: 4.2 MB (4189288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44dcbc70566b6f8312605c0214812444ccad7a55594fa2e7f0792c21af818ef0`  
		Last Modified: Fri, 03 Dec 2021 16:58:49 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:windowsservercore`

```console
$ docker pull nats@sha256:24e44e15d62a911e94d6ff5b7e22accfe329f699b42ade9ebb1a5caa3197f373
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.2452; amd64
	-	windows version 10.0.14393.4886; amd64

### `nats:windowsservercore` - windows version 10.0.17763.2452; amd64

```console
$ docker pull nats@sha256:7f3bfcdbda90968d69223b48664ee1ec937a82bce7365c82135785fe353ba699
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2717536770 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4622435affd612664c15aa4fd83b1e45ba56de92d3c7e6dd3dd924adf28111bf`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 07 Jan 2022 22:48:13 GMT
RUN Install update 1809-amd64
# Wed, 12 Jan 2022 13:54:17 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 Jan 2022 15:10:29 GMT
ENV NATS_DOCKERIZED=1
# Wed, 12 Jan 2022 15:10:30 GMT
ENV NATS_SERVER=2.6.6
# Wed, 12 Jan 2022 15:10:32 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.6.6/nats-server-v2.6.6-windows-amd64.zip
# Wed, 12 Jan 2022 15:10:33 GMT
ENV NATS_SERVER_SHASUM=9730ea401beed7ac40aeada0a8dccfb70207bb234202035aad5644e93ec657da
# Wed, 12 Jan 2022 15:11:32 GMT
RUN Set-PSDebug -Trace 2
# Wed, 12 Jan 2022 15:13:24 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 12 Jan 2022 15:13:26 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 12 Jan 2022 15:13:27 GMT
EXPOSE 4222 6222 8222
# Wed, 12 Jan 2022 15:13:28 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 12 Jan 2022 15:13:29 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:635f15ebd5b486e8a00bf217a0574a29550e5bbf08c1d021e1e308100b2e49b5`  
		Size: 993.9 MB (993898043 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:537828534783cff318d36854dbda0683aef7263e437c7c669de4092e1778959c`  
		Last Modified: Wed, 12 Jan 2022 15:14:30 GMT  
		Size: 1.3 KB (1296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9576e7772519d67febb0ceb94d8f22531ea99f0c60c36e67a4f5a497c384f5e0`  
		Last Modified: Wed, 12 Jan 2022 15:14:30 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaf1f761c394ef0da3c3fef1865f52e977d392f3f0b6c0575c3d1341da6cd7e9`  
		Last Modified: Wed, 12 Jan 2022 15:14:28 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e647346313038e022d4394703013d0963bc45ad0782bcf984166dd279d475c5d`  
		Last Modified: Wed, 12 Jan 2022 15:14:27 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fb56fc761a44bdcdde0f2cfaa2a75932b2ac8fe3c78177727284b0f58037fb0`  
		Last Modified: Wed, 12 Jan 2022 15:14:28 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5797262702f20651c9e1f79f4fbfbe22a260dc9bb7408bf5820eb186b3063f4d`  
		Last Modified: Wed, 12 Jan 2022 15:14:27 GMT  
		Size: 338.2 KB (338250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24cad06e122fd976b54af5acb5a3ba1d1299d61be733e7c2eadeb185aca82942`  
		Last Modified: Wed, 12 Jan 2022 15:14:31 GMT  
		Size: 5.0 MB (4954480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:886cf217b75c847a9ef63c4cc6093d9aa9c783f67b2c999fb7b23249e80b6e6c`  
		Last Modified: Wed, 12 Jan 2022 15:14:25 GMT  
		Size: 1.9 KB (1941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f1f92fb92be2d3b29fc1f42015a4d47bb112ae53db5fab9fa63f432838b7747`  
		Last Modified: Wed, 12 Jan 2022 15:14:25 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:099a82c04f8e6eee73daaccc93d0ad74009ffb4c94eb7d9c8a6a52b4e6bdf2fd`  
		Last Modified: Wed, 12 Jan 2022 15:14:25 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:507bd2ef766612deffd70102b577c1242165b07a8464313f8454713360560c86`  
		Last Modified: Wed, 12 Jan 2022 15:14:25 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:windowsservercore` - windows version 10.0.14393.4886; amd64

```console
$ docker pull nats@sha256:e476d11dde611fc9b39eb6a45798c2e503fa1bfa4ece59509826bfaed6a4cbe1
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6283541821 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:084594550a22f2aa624e5b2e740a29366a6846c2e1f194854e6e32270f5f0edb`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Thu, 06 Jan 2022 14:33:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 11 Jan 2022 19:57:39 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Tue, 11 Jan 2022 19:57:40 GMT
ENV NATS_DOCKERIZED=1
# Tue, 11 Jan 2022 21:15:53 GMT
ENV NATS_SERVER=2.6.6
# Tue, 11 Jan 2022 21:15:55 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.6.6/nats-server-v2.6.6-windows-amd64.zip
# Tue, 11 Jan 2022 21:15:56 GMT
ENV NATS_SERVER_SHASUM=9730ea401beed7ac40aeada0a8dccfb70207bb234202035aad5644e93ec657da
# Tue, 11 Jan 2022 21:16:48 GMT
RUN Set-PSDebug -Trace 2
# Tue, 11 Jan 2022 21:18:24 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Tue, 11 Jan 2022 21:18:25 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Tue, 11 Jan 2022 21:18:26 GMT
EXPOSE 4222 6222 8222
# Tue, 11 Jan 2022 21:18:28 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 11 Jan 2022 21:18:29 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8428508ffd63b4af1ba690ec41e82a116f10ec6c3fb70962348f5448d42e5835`  
		Size: 2.2 GB (2208216859 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:25aec0a6b64c784bf7521344203ee5def4d38eedfdd68f4b452d3250b5b9ddcf`  
		Last Modified: Tue, 11 Jan 2022 21:19:46 GMT  
		Size: 1.3 KB (1327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3fffdd310a93f98578e45ffbf8e22c031b37efefcc042f21d2a63c2a77c4ee3`  
		Last Modified: Tue, 11 Jan 2022 21:19:45 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15052497c858a1a8b4a8159d05850fbf43551aad161e61ae0fd6880c46eb4556`  
		Last Modified: Tue, 11 Jan 2022 21:19:44 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:080911a4b1ac40e1f062d68ed70319860e88ecb9abec2aef41d0bc3bae89098d`  
		Last Modified: Tue, 11 Jan 2022 21:19:44 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e79cea19a92f33c59acbcc8f501e9acdb5985bbad5b03ccd1190848ae1b4cf1`  
		Last Modified: Tue, 11 Jan 2022 21:19:44 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae0544e04ecd7b6afc6366924310fd892736faf1983ea2ee9e40efd31a0ec502`  
		Last Modified: Tue, 11 Jan 2022 21:19:44 GMT  
		Size: 337.0 KB (337010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8906d4ca25b04680081cc6af81b8eec86a9756abb72e21ed2785f82372ba7c58`  
		Last Modified: Tue, 11 Jan 2022 21:19:43 GMT  
		Size: 5.0 MB (4988964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99a01b43c4c8c06f528a3080b9f4d396d196ff851a603ac22c9ce560c3d5b082`  
		Last Modified: Tue, 11 Jan 2022 21:19:42 GMT  
		Size: 2.0 KB (1973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e156e4bebcfed633295afa0f9dacd6146736cb7de973581f01931fdf6d5f5ae`  
		Last Modified: Tue, 11 Jan 2022 21:19:41 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf3ee9fcf4be90533587d2a54238465fc8f6bad0744784041f675b2e97a93bb9`  
		Last Modified: Tue, 11 Jan 2022 21:19:42 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6e44c694323da6f62bebd7b52b659731c89b1e15c15e5c345ec43e24cba28f7`  
		Last Modified: Tue, 11 Jan 2022 21:19:41 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:windowsservercore-1809`

```console
$ docker pull nats@sha256:688fa8edbb0b5931af887d0ab00ed77da3f9e8505225dc1eccf15672638fd7a7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2452; amd64

### `nats:windowsservercore-1809` - windows version 10.0.17763.2452; amd64

```console
$ docker pull nats@sha256:7f3bfcdbda90968d69223b48664ee1ec937a82bce7365c82135785fe353ba699
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2717536770 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4622435affd612664c15aa4fd83b1e45ba56de92d3c7e6dd3dd924adf28111bf`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 07 Jan 2022 22:48:13 GMT
RUN Install update 1809-amd64
# Wed, 12 Jan 2022 13:54:17 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 Jan 2022 15:10:29 GMT
ENV NATS_DOCKERIZED=1
# Wed, 12 Jan 2022 15:10:30 GMT
ENV NATS_SERVER=2.6.6
# Wed, 12 Jan 2022 15:10:32 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.6.6/nats-server-v2.6.6-windows-amd64.zip
# Wed, 12 Jan 2022 15:10:33 GMT
ENV NATS_SERVER_SHASUM=9730ea401beed7ac40aeada0a8dccfb70207bb234202035aad5644e93ec657da
# Wed, 12 Jan 2022 15:11:32 GMT
RUN Set-PSDebug -Trace 2
# Wed, 12 Jan 2022 15:13:24 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 12 Jan 2022 15:13:26 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 12 Jan 2022 15:13:27 GMT
EXPOSE 4222 6222 8222
# Wed, 12 Jan 2022 15:13:28 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 12 Jan 2022 15:13:29 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:635f15ebd5b486e8a00bf217a0574a29550e5bbf08c1d021e1e308100b2e49b5`  
		Size: 993.9 MB (993898043 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:537828534783cff318d36854dbda0683aef7263e437c7c669de4092e1778959c`  
		Last Modified: Wed, 12 Jan 2022 15:14:30 GMT  
		Size: 1.3 KB (1296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9576e7772519d67febb0ceb94d8f22531ea99f0c60c36e67a4f5a497c384f5e0`  
		Last Modified: Wed, 12 Jan 2022 15:14:30 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaf1f761c394ef0da3c3fef1865f52e977d392f3f0b6c0575c3d1341da6cd7e9`  
		Last Modified: Wed, 12 Jan 2022 15:14:28 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e647346313038e022d4394703013d0963bc45ad0782bcf984166dd279d475c5d`  
		Last Modified: Wed, 12 Jan 2022 15:14:27 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fb56fc761a44bdcdde0f2cfaa2a75932b2ac8fe3c78177727284b0f58037fb0`  
		Last Modified: Wed, 12 Jan 2022 15:14:28 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5797262702f20651c9e1f79f4fbfbe22a260dc9bb7408bf5820eb186b3063f4d`  
		Last Modified: Wed, 12 Jan 2022 15:14:27 GMT  
		Size: 338.2 KB (338250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24cad06e122fd976b54af5acb5a3ba1d1299d61be733e7c2eadeb185aca82942`  
		Last Modified: Wed, 12 Jan 2022 15:14:31 GMT  
		Size: 5.0 MB (4954480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:886cf217b75c847a9ef63c4cc6093d9aa9c783f67b2c999fb7b23249e80b6e6c`  
		Last Modified: Wed, 12 Jan 2022 15:14:25 GMT  
		Size: 1.9 KB (1941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f1f92fb92be2d3b29fc1f42015a4d47bb112ae53db5fab9fa63f432838b7747`  
		Last Modified: Wed, 12 Jan 2022 15:14:25 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:099a82c04f8e6eee73daaccc93d0ad74009ffb4c94eb7d9c8a6a52b4e6bdf2fd`  
		Last Modified: Wed, 12 Jan 2022 15:14:25 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:507bd2ef766612deffd70102b577c1242165b07a8464313f8454713360560c86`  
		Last Modified: Wed, 12 Jan 2022 15:14:25 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:windowsservercore-ltsc2016`

```console
$ docker pull nats@sha256:3d337d85e45c503e13f57109f85de0e1c916fc6781cf7bbd3f40ccffd0fb664b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.14393.4886; amd64

### `nats:windowsservercore-ltsc2016` - windows version 10.0.14393.4886; amd64

```console
$ docker pull nats@sha256:e476d11dde611fc9b39eb6a45798c2e503fa1bfa4ece59509826bfaed6a4cbe1
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6283541821 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:084594550a22f2aa624e5b2e740a29366a6846c2e1f194854e6e32270f5f0edb`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Thu, 06 Jan 2022 14:33:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 11 Jan 2022 19:57:39 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Tue, 11 Jan 2022 19:57:40 GMT
ENV NATS_DOCKERIZED=1
# Tue, 11 Jan 2022 21:15:53 GMT
ENV NATS_SERVER=2.6.6
# Tue, 11 Jan 2022 21:15:55 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.6.6/nats-server-v2.6.6-windows-amd64.zip
# Tue, 11 Jan 2022 21:15:56 GMT
ENV NATS_SERVER_SHASUM=9730ea401beed7ac40aeada0a8dccfb70207bb234202035aad5644e93ec657da
# Tue, 11 Jan 2022 21:16:48 GMT
RUN Set-PSDebug -Trace 2
# Tue, 11 Jan 2022 21:18:24 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Tue, 11 Jan 2022 21:18:25 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Tue, 11 Jan 2022 21:18:26 GMT
EXPOSE 4222 6222 8222
# Tue, 11 Jan 2022 21:18:28 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 11 Jan 2022 21:18:29 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8428508ffd63b4af1ba690ec41e82a116f10ec6c3fb70962348f5448d42e5835`  
		Size: 2.2 GB (2208216859 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:25aec0a6b64c784bf7521344203ee5def4d38eedfdd68f4b452d3250b5b9ddcf`  
		Last Modified: Tue, 11 Jan 2022 21:19:46 GMT  
		Size: 1.3 KB (1327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3fffdd310a93f98578e45ffbf8e22c031b37efefcc042f21d2a63c2a77c4ee3`  
		Last Modified: Tue, 11 Jan 2022 21:19:45 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15052497c858a1a8b4a8159d05850fbf43551aad161e61ae0fd6880c46eb4556`  
		Last Modified: Tue, 11 Jan 2022 21:19:44 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:080911a4b1ac40e1f062d68ed70319860e88ecb9abec2aef41d0bc3bae89098d`  
		Last Modified: Tue, 11 Jan 2022 21:19:44 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e79cea19a92f33c59acbcc8f501e9acdb5985bbad5b03ccd1190848ae1b4cf1`  
		Last Modified: Tue, 11 Jan 2022 21:19:44 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae0544e04ecd7b6afc6366924310fd892736faf1983ea2ee9e40efd31a0ec502`  
		Last Modified: Tue, 11 Jan 2022 21:19:44 GMT  
		Size: 337.0 KB (337010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8906d4ca25b04680081cc6af81b8eec86a9756abb72e21ed2785f82372ba7c58`  
		Last Modified: Tue, 11 Jan 2022 21:19:43 GMT  
		Size: 5.0 MB (4988964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99a01b43c4c8c06f528a3080b9f4d396d196ff851a603ac22c9ce560c3d5b082`  
		Last Modified: Tue, 11 Jan 2022 21:19:42 GMT  
		Size: 2.0 KB (1973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e156e4bebcfed633295afa0f9dacd6146736cb7de973581f01931fdf6d5f5ae`  
		Last Modified: Tue, 11 Jan 2022 21:19:41 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf3ee9fcf4be90533587d2a54238465fc8f6bad0744784041f675b2e97a93bb9`  
		Last Modified: Tue, 11 Jan 2022 21:19:42 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6e44c694323da6f62bebd7b52b659731c89b1e15c15e5c345ec43e24cba28f7`  
		Last Modified: Tue, 11 Jan 2022 21:19:41 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
