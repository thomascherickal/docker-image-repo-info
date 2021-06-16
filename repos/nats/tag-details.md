<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `nats`

-	[`nats:2`](#nats2)
-	[`nats:2-alpine`](#nats2-alpine)
-	[`nats:2-alpine3.13`](#nats2-alpine313)
-	[`nats:2-linux`](#nats2-linux)
-	[`nats:2-nanoserver`](#nats2-nanoserver)
-	[`nats:2-nanoserver-1809`](#nats2-nanoserver-1809)
-	[`nats:2-scratch`](#nats2-scratch)
-	[`nats:2-windowsservercore`](#nats2-windowsservercore)
-	[`nats:2-windowsservercore-1809`](#nats2-windowsservercore-1809)
-	[`nats:2-windowsservercore-ltsc2016`](#nats2-windowsservercore-ltsc2016)
-	[`nats:2.2`](#nats22)
-	[`nats:2.2-alpine`](#nats22-alpine)
-	[`nats:2.2-alpine3.13`](#nats22-alpine313)
-	[`nats:2.2-linux`](#nats22-linux)
-	[`nats:2.2-nanoserver`](#nats22-nanoserver)
-	[`nats:2.2-nanoserver-1809`](#nats22-nanoserver-1809)
-	[`nats:2.2-scratch`](#nats22-scratch)
-	[`nats:2.2-windowsservercore`](#nats22-windowsservercore)
-	[`nats:2.2-windowsservercore-1809`](#nats22-windowsservercore-1809)
-	[`nats:2.2-windowsservercore-ltsc2016`](#nats22-windowsservercore-ltsc2016)
-	[`nats:2.2.6`](#nats226)
-	[`nats:2.2.6-alpine`](#nats226-alpine)
-	[`nats:2.2.6-alpine3.13`](#nats226-alpine313)
-	[`nats:2.2.6-linux`](#nats226-linux)
-	[`nats:2.2.6-nanoserver`](#nats226-nanoserver)
-	[`nats:2.2.6-nanoserver-1809`](#nats226-nanoserver-1809)
-	[`nats:2.2.6-scratch`](#nats226-scratch)
-	[`nats:2.2.6-windowsservercore`](#nats226-windowsservercore)
-	[`nats:2.2.6-windowsservercore-1809`](#nats226-windowsservercore-1809)
-	[`nats:2.2.6-windowsservercore-ltsc2016`](#nats226-windowsservercore-ltsc2016)
-	[`nats:alpine`](#natsalpine)
-	[`nats:alpine3.13`](#natsalpine313)
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
$ docker pull nats@sha256:ed66dfeef8f3c691f17ac8920b46054de09796a3b7a5bd3e96cb234a87915523
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.1999; amd64

### `nats:2` - linux; amd64

```console
$ docker pull nats@sha256:bad1b98cb238be899761405ed9a084eb4cee1e4982c4082414a49e1e47d83993
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4249359 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3903d09e582715d83e8da5706ee14109824854452c0ebf177eb55dfb789e311`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 25 May 2021 01:38:34 GMT
COPY file:6d5e77e6be5bafda9b9e03a4f397b21f9432694e3c3c3b5cd6e621b4c3ec3018 in /nats-server 
# Tue, 25 May 2021 01:38:34 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Tue, 25 May 2021 01:38:34 GMT
EXPOSE 4222 6222 8222
# Tue, 25 May 2021 01:38:34 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 25 May 2021 01:38:35 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:bf9e6d973acc267c8b0f05973d840142eec057566b36d0ae18177113f1fdadda`  
		Last Modified: Tue, 25 May 2021 01:39:26 GMT  
		Size: 4.2 MB (4248883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14a60a1c8cdedd7b360929beb64e25bbab3d679ba8134844479aaa6169d73595`  
		Last Modified: Tue, 25 May 2021 01:39:25 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - linux; arm variant v6

```console
$ docker pull nats@sha256:f98c4fa99482edcc01991046e5e9b2650e6181ec78b070d6601adef0afbbc3d9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3916550 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:573ae66ceb9d5149762ca1a8585b9f794bc0c0372ce18f73beefebb086f898c1`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 26 May 2021 18:22:59 GMT
COPY file:09c6eee4fb87ec105cf70b09816e278a49955f5e23576db600bfdb2fff0d6633 in /nats-server 
# Wed, 26 May 2021 18:23:00 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Wed, 26 May 2021 18:23:00 GMT
EXPOSE 4222 6222 8222
# Wed, 26 May 2021 18:23:00 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 26 May 2021 18:23:00 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:069976a4471c1abc4ad7dc33e5d7ed35c51e717ae622a055b7e925dd0bbe2ccb`  
		Last Modified: Wed, 26 May 2021 18:24:53 GMT  
		Size: 3.9 MB (3916076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4094f904541e138a0436baf31ea6b5ed4b91aee4871a54fce1650f2d63d2da2`  
		Last Modified: Wed, 26 May 2021 18:24:52 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - linux; arm variant v7

```console
$ docker pull nats@sha256:593e1b418f3e55050730f63b1d5da6e5f6f9c990c66e15bb9cd6659ea836279f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3914539 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4093ac9e36206435159f30858c34c7ed656e69e8dcbe1aaa6fbd40099701ade7`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 25 May 2021 22:23:02 GMT
COPY file:1ccce8553c778be1204380469e7248fd9ee472bdec35db0b7dd150122ae7c37d in /nats-server 
# Tue, 25 May 2021 22:23:02 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Tue, 25 May 2021 22:23:03 GMT
EXPOSE 4222 6222 8222
# Tue, 25 May 2021 22:23:03 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 25 May 2021 22:23:03 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a459b50ce258c1a3884cfc6f671ebabe9d05421a39962966809134623f3b9979`  
		Last Modified: Tue, 25 May 2021 22:24:59 GMT  
		Size: 3.9 MB (3914063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1808b616cb182b07285cb2e4b7d289755ccf8fa8575a8bc73a20ae46f8f253a`  
		Last Modified: Tue, 25 May 2021 22:24:58 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:8d8addd19d02a411d04db404a43383648e6a39e5a6686d5c2870bd5a0b80c546
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3889451 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b2ba9cf0b70339a1dd0b4bc93c1c83f00d829cd27d85adabe9b5ef7fdfefc69`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 26 May 2021 23:34:44 GMT
COPY file:312f19d8ade34bbf7590dddfdd3664f3152040117d8296ec0a54e9a9f7f42ae7 in /nats-server 
# Wed, 26 May 2021 23:34:45 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Wed, 26 May 2021 23:34:45 GMT
EXPOSE 4222 6222 8222
# Wed, 26 May 2021 23:34:45 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 26 May 2021 23:34:45 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:529a1438983ee1d8a2fdcab2846023465327ab9d8b15f0a7ed6ce61ff67fb8e8`  
		Last Modified: Wed, 26 May 2021 23:36:07 GMT  
		Size: 3.9 MB (3888976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:411d0165541f17c63026ae51d40e5a1f09909f0ab49fdadc7c2c7d904a4a3cb9`  
		Last Modified: Wed, 26 May 2021 23:36:06 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - windows version 10.0.17763.1999; amd64

```console
$ docker pull nats@sha256:7305d7bf57da3e44ce9e5b368d294f4d9a6f86908ee0522b2e3af953bbfeaeb8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.0 MB (106983364 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:448497fc5d2a9aa4a4fe1404fa1f9cbd4a6cabcc2593a935a7e18d9ca49f7743`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sun, 06 Jun 2021 04:04:04 GMT
RUN Apply image 1809-amd64
# Wed, 09 Jun 2021 15:55:07 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 09 Jun 2021 15:55:09 GMT
RUN cmd /S /C #(nop) COPY file:a13acc0f2f64f12c4304c7730a47bebb73f06865d8dee680ec7a370c77d69e10 in C:\nats-server.exe 
# Wed, 09 Jun 2021 15:55:12 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 09 Jun 2021 15:55:14 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 09 Jun 2021 15:55:17 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 09 Jun 2021 15:55:19 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:e4800203e906d49fbdaf1eeab4de72f28796d5b9a1ea44f8d7461001cfa56614`  
		Size: 102.7 MB (102671454 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:80d93ce19113bbf944b699f12e59395e0eabeb00ccd1fd5dc7df46bb115eba2f`  
		Last Modified: Wed, 09 Jun 2021 15:59:58 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02a2af79aa85193c9d59672eaa3d7792de702370a62c15d646ca3d6e9805a4e3`  
		Last Modified: Wed, 09 Jun 2021 15:59:57 GMT  
		Size: 4.3 MB (4305480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9e0f71986494c926842ef864b29a5d7f3467a0415538fa78ad7850693a7b9d2`  
		Last Modified: Wed, 09 Jun 2021 15:59:56 GMT  
		Size: 1.8 KB (1752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74462c7c877f0c6efdd4131bf6b4ddf0ab34ceaa3aaeec8ca8d0b9f3fe614731`  
		Last Modified: Wed, 09 Jun 2021 15:59:56 GMT  
		Size: 1.2 KB (1192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cff02dcbfcaa11d91acbf9f579c2dc701b2c0a8057cb1b98b85a60bdeac38ba`  
		Last Modified: Wed, 09 Jun 2021 15:59:55 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56f9ea8a05c1d3919aab5e228736bf5b7f7dfd2493d7450e95724e6a41aab47b`  
		Last Modified: Wed, 09 Jun 2021 15:59:56 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-alpine`

```console
$ docker pull nats@sha256:cc2bde1fe965db9ac2011073b071010691ebdb1904c7933922ad2a107a5a7a34
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-alpine` - linux; amd64

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

### `nats:2-alpine` - linux; arm variant v6

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

### `nats:2-alpine` - linux; arm variant v7

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

### `nats:2-alpine` - linux; arm64 variant v8

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

## `nats:2-alpine3.13`

```console
$ docker pull nats@sha256:cc2bde1fe965db9ac2011073b071010691ebdb1904c7933922ad2a107a5a7a34
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-alpine3.13` - linux; amd64

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

### `nats:2-alpine3.13` - linux; arm variant v6

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

### `nats:2-alpine3.13` - linux; arm variant v7

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

### `nats:2-alpine3.13` - linux; arm64 variant v8

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

## `nats:2-linux`

```console
$ docker pull nats@sha256:8aceb3b18cc40ba1aa1d88ac3d22108e02e7a43cae6d2b66910dcfa80d437885
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-linux` - linux; amd64

```console
$ docker pull nats@sha256:bad1b98cb238be899761405ed9a084eb4cee1e4982c4082414a49e1e47d83993
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4249359 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3903d09e582715d83e8da5706ee14109824854452c0ebf177eb55dfb789e311`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 25 May 2021 01:38:34 GMT
COPY file:6d5e77e6be5bafda9b9e03a4f397b21f9432694e3c3c3b5cd6e621b4c3ec3018 in /nats-server 
# Tue, 25 May 2021 01:38:34 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Tue, 25 May 2021 01:38:34 GMT
EXPOSE 4222 6222 8222
# Tue, 25 May 2021 01:38:34 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 25 May 2021 01:38:35 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:bf9e6d973acc267c8b0f05973d840142eec057566b36d0ae18177113f1fdadda`  
		Last Modified: Tue, 25 May 2021 01:39:26 GMT  
		Size: 4.2 MB (4248883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14a60a1c8cdedd7b360929beb64e25bbab3d679ba8134844479aaa6169d73595`  
		Last Modified: Tue, 25 May 2021 01:39:25 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:f98c4fa99482edcc01991046e5e9b2650e6181ec78b070d6601adef0afbbc3d9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3916550 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:573ae66ceb9d5149762ca1a8585b9f794bc0c0372ce18f73beefebb086f898c1`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 26 May 2021 18:22:59 GMT
COPY file:09c6eee4fb87ec105cf70b09816e278a49955f5e23576db600bfdb2fff0d6633 in /nats-server 
# Wed, 26 May 2021 18:23:00 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Wed, 26 May 2021 18:23:00 GMT
EXPOSE 4222 6222 8222
# Wed, 26 May 2021 18:23:00 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 26 May 2021 18:23:00 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:069976a4471c1abc4ad7dc33e5d7ed35c51e717ae622a055b7e925dd0bbe2ccb`  
		Last Modified: Wed, 26 May 2021 18:24:53 GMT  
		Size: 3.9 MB (3916076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4094f904541e138a0436baf31ea6b5ed4b91aee4871a54fce1650f2d63d2da2`  
		Last Modified: Wed, 26 May 2021 18:24:52 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:593e1b418f3e55050730f63b1d5da6e5f6f9c990c66e15bb9cd6659ea836279f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3914539 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4093ac9e36206435159f30858c34c7ed656e69e8dcbe1aaa6fbd40099701ade7`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 25 May 2021 22:23:02 GMT
COPY file:1ccce8553c778be1204380469e7248fd9ee472bdec35db0b7dd150122ae7c37d in /nats-server 
# Tue, 25 May 2021 22:23:02 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Tue, 25 May 2021 22:23:03 GMT
EXPOSE 4222 6222 8222
# Tue, 25 May 2021 22:23:03 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 25 May 2021 22:23:03 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a459b50ce258c1a3884cfc6f671ebabe9d05421a39962966809134623f3b9979`  
		Last Modified: Tue, 25 May 2021 22:24:59 GMT  
		Size: 3.9 MB (3914063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1808b616cb182b07285cb2e4b7d289755ccf8fa8575a8bc73a20ae46f8f253a`  
		Last Modified: Tue, 25 May 2021 22:24:58 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:8d8addd19d02a411d04db404a43383648e6a39e5a6686d5c2870bd5a0b80c546
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3889451 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b2ba9cf0b70339a1dd0b4bc93c1c83f00d829cd27d85adabe9b5ef7fdfefc69`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 26 May 2021 23:34:44 GMT
COPY file:312f19d8ade34bbf7590dddfdd3664f3152040117d8296ec0a54e9a9f7f42ae7 in /nats-server 
# Wed, 26 May 2021 23:34:45 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Wed, 26 May 2021 23:34:45 GMT
EXPOSE 4222 6222 8222
# Wed, 26 May 2021 23:34:45 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 26 May 2021 23:34:45 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:529a1438983ee1d8a2fdcab2846023465327ab9d8b15f0a7ed6ce61ff67fb8e8`  
		Last Modified: Wed, 26 May 2021 23:36:07 GMT  
		Size: 3.9 MB (3888976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:411d0165541f17c63026ae51d40e5a1f09909f0ab49fdadc7c2c7d904a4a3cb9`  
		Last Modified: Wed, 26 May 2021 23:36:06 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-nanoserver`

```console
$ docker pull nats@sha256:a0aacfbc002543c9a2dac717593b25e60fe52c18ec1033479d2a8fd25bab8391
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1999; amd64

### `nats:2-nanoserver` - windows version 10.0.17763.1999; amd64

```console
$ docker pull nats@sha256:7305d7bf57da3e44ce9e5b368d294f4d9a6f86908ee0522b2e3af953bbfeaeb8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.0 MB (106983364 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:448497fc5d2a9aa4a4fe1404fa1f9cbd4a6cabcc2593a935a7e18d9ca49f7743`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sun, 06 Jun 2021 04:04:04 GMT
RUN Apply image 1809-amd64
# Wed, 09 Jun 2021 15:55:07 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 09 Jun 2021 15:55:09 GMT
RUN cmd /S /C #(nop) COPY file:a13acc0f2f64f12c4304c7730a47bebb73f06865d8dee680ec7a370c77d69e10 in C:\nats-server.exe 
# Wed, 09 Jun 2021 15:55:12 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 09 Jun 2021 15:55:14 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 09 Jun 2021 15:55:17 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 09 Jun 2021 15:55:19 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:e4800203e906d49fbdaf1eeab4de72f28796d5b9a1ea44f8d7461001cfa56614`  
		Size: 102.7 MB (102671454 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:80d93ce19113bbf944b699f12e59395e0eabeb00ccd1fd5dc7df46bb115eba2f`  
		Last Modified: Wed, 09 Jun 2021 15:59:58 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02a2af79aa85193c9d59672eaa3d7792de702370a62c15d646ca3d6e9805a4e3`  
		Last Modified: Wed, 09 Jun 2021 15:59:57 GMT  
		Size: 4.3 MB (4305480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9e0f71986494c926842ef864b29a5d7f3467a0415538fa78ad7850693a7b9d2`  
		Last Modified: Wed, 09 Jun 2021 15:59:56 GMT  
		Size: 1.8 KB (1752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74462c7c877f0c6efdd4131bf6b4ddf0ab34ceaa3aaeec8ca8d0b9f3fe614731`  
		Last Modified: Wed, 09 Jun 2021 15:59:56 GMT  
		Size: 1.2 KB (1192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cff02dcbfcaa11d91acbf9f579c2dc701b2c0a8057cb1b98b85a60bdeac38ba`  
		Last Modified: Wed, 09 Jun 2021 15:59:55 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56f9ea8a05c1d3919aab5e228736bf5b7f7dfd2493d7450e95724e6a41aab47b`  
		Last Modified: Wed, 09 Jun 2021 15:59:56 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-nanoserver-1809`

```console
$ docker pull nats@sha256:a0aacfbc002543c9a2dac717593b25e60fe52c18ec1033479d2a8fd25bab8391
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1999; amd64

### `nats:2-nanoserver-1809` - windows version 10.0.17763.1999; amd64

```console
$ docker pull nats@sha256:7305d7bf57da3e44ce9e5b368d294f4d9a6f86908ee0522b2e3af953bbfeaeb8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.0 MB (106983364 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:448497fc5d2a9aa4a4fe1404fa1f9cbd4a6cabcc2593a935a7e18d9ca49f7743`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sun, 06 Jun 2021 04:04:04 GMT
RUN Apply image 1809-amd64
# Wed, 09 Jun 2021 15:55:07 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 09 Jun 2021 15:55:09 GMT
RUN cmd /S /C #(nop) COPY file:a13acc0f2f64f12c4304c7730a47bebb73f06865d8dee680ec7a370c77d69e10 in C:\nats-server.exe 
# Wed, 09 Jun 2021 15:55:12 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 09 Jun 2021 15:55:14 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 09 Jun 2021 15:55:17 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 09 Jun 2021 15:55:19 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:e4800203e906d49fbdaf1eeab4de72f28796d5b9a1ea44f8d7461001cfa56614`  
		Size: 102.7 MB (102671454 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:80d93ce19113bbf944b699f12e59395e0eabeb00ccd1fd5dc7df46bb115eba2f`  
		Last Modified: Wed, 09 Jun 2021 15:59:58 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02a2af79aa85193c9d59672eaa3d7792de702370a62c15d646ca3d6e9805a4e3`  
		Last Modified: Wed, 09 Jun 2021 15:59:57 GMT  
		Size: 4.3 MB (4305480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9e0f71986494c926842ef864b29a5d7f3467a0415538fa78ad7850693a7b9d2`  
		Last Modified: Wed, 09 Jun 2021 15:59:56 GMT  
		Size: 1.8 KB (1752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74462c7c877f0c6efdd4131bf6b4ddf0ab34ceaa3aaeec8ca8d0b9f3fe614731`  
		Last Modified: Wed, 09 Jun 2021 15:59:56 GMT  
		Size: 1.2 KB (1192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cff02dcbfcaa11d91acbf9f579c2dc701b2c0a8057cb1b98b85a60bdeac38ba`  
		Last Modified: Wed, 09 Jun 2021 15:59:55 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56f9ea8a05c1d3919aab5e228736bf5b7f7dfd2493d7450e95724e6a41aab47b`  
		Last Modified: Wed, 09 Jun 2021 15:59:56 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-scratch`

```console
$ docker pull nats@sha256:8aceb3b18cc40ba1aa1d88ac3d22108e02e7a43cae6d2b66910dcfa80d437885
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-scratch` - linux; amd64

```console
$ docker pull nats@sha256:bad1b98cb238be899761405ed9a084eb4cee1e4982c4082414a49e1e47d83993
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4249359 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3903d09e582715d83e8da5706ee14109824854452c0ebf177eb55dfb789e311`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 25 May 2021 01:38:34 GMT
COPY file:6d5e77e6be5bafda9b9e03a4f397b21f9432694e3c3c3b5cd6e621b4c3ec3018 in /nats-server 
# Tue, 25 May 2021 01:38:34 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Tue, 25 May 2021 01:38:34 GMT
EXPOSE 4222 6222 8222
# Tue, 25 May 2021 01:38:34 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 25 May 2021 01:38:35 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:bf9e6d973acc267c8b0f05973d840142eec057566b36d0ae18177113f1fdadda`  
		Last Modified: Tue, 25 May 2021 01:39:26 GMT  
		Size: 4.2 MB (4248883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14a60a1c8cdedd7b360929beb64e25bbab3d679ba8134844479aaa6169d73595`  
		Last Modified: Tue, 25 May 2021 01:39:25 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:f98c4fa99482edcc01991046e5e9b2650e6181ec78b070d6601adef0afbbc3d9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3916550 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:573ae66ceb9d5149762ca1a8585b9f794bc0c0372ce18f73beefebb086f898c1`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 26 May 2021 18:22:59 GMT
COPY file:09c6eee4fb87ec105cf70b09816e278a49955f5e23576db600bfdb2fff0d6633 in /nats-server 
# Wed, 26 May 2021 18:23:00 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Wed, 26 May 2021 18:23:00 GMT
EXPOSE 4222 6222 8222
# Wed, 26 May 2021 18:23:00 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 26 May 2021 18:23:00 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:069976a4471c1abc4ad7dc33e5d7ed35c51e717ae622a055b7e925dd0bbe2ccb`  
		Last Modified: Wed, 26 May 2021 18:24:53 GMT  
		Size: 3.9 MB (3916076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4094f904541e138a0436baf31ea6b5ed4b91aee4871a54fce1650f2d63d2da2`  
		Last Modified: Wed, 26 May 2021 18:24:52 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:593e1b418f3e55050730f63b1d5da6e5f6f9c990c66e15bb9cd6659ea836279f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3914539 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4093ac9e36206435159f30858c34c7ed656e69e8dcbe1aaa6fbd40099701ade7`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 25 May 2021 22:23:02 GMT
COPY file:1ccce8553c778be1204380469e7248fd9ee472bdec35db0b7dd150122ae7c37d in /nats-server 
# Tue, 25 May 2021 22:23:02 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Tue, 25 May 2021 22:23:03 GMT
EXPOSE 4222 6222 8222
# Tue, 25 May 2021 22:23:03 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 25 May 2021 22:23:03 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a459b50ce258c1a3884cfc6f671ebabe9d05421a39962966809134623f3b9979`  
		Last Modified: Tue, 25 May 2021 22:24:59 GMT  
		Size: 3.9 MB (3914063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1808b616cb182b07285cb2e4b7d289755ccf8fa8575a8bc73a20ae46f8f253a`  
		Last Modified: Tue, 25 May 2021 22:24:58 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:8d8addd19d02a411d04db404a43383648e6a39e5a6686d5c2870bd5a0b80c546
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3889451 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b2ba9cf0b70339a1dd0b4bc93c1c83f00d829cd27d85adabe9b5ef7fdfefc69`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 26 May 2021 23:34:44 GMT
COPY file:312f19d8ade34bbf7590dddfdd3664f3152040117d8296ec0a54e9a9f7f42ae7 in /nats-server 
# Wed, 26 May 2021 23:34:45 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Wed, 26 May 2021 23:34:45 GMT
EXPOSE 4222 6222 8222
# Wed, 26 May 2021 23:34:45 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 26 May 2021 23:34:45 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:529a1438983ee1d8a2fdcab2846023465327ab9d8b15f0a7ed6ce61ff67fb8e8`  
		Last Modified: Wed, 26 May 2021 23:36:07 GMT  
		Size: 3.9 MB (3888976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:411d0165541f17c63026ae51d40e5a1f09909f0ab49fdadc7c2c7d904a4a3cb9`  
		Last Modified: Wed, 26 May 2021 23:36:06 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-windowsservercore`

```console
$ docker pull nats@sha256:334a5bbe37d543b1a8fcbd110923b8ac58c7095ba41eace53d0005932cd0899e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1999; amd64
	-	windows version 10.0.14393.4467; amd64

### `nats:2-windowsservercore` - windows version 10.0.17763.1999; amd64

```console
$ docker pull nats@sha256:b02d0fddc42e8f50f6dccf56bc6da2c299fa6ca12dac2a91142f5ea6f3c3b4d2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2646572446 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec0469d99bdcdeb93ecb4cd714c002dc5344cdd980081af67522abd90cb61f56`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sun, 06 Jun 2021 04:28:43 GMT
RUN Install update 1809-amd64
# Wed, 09 Jun 2021 13:15:43 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Jun 2021 15:52:54 GMT
ENV NATS_DOCKERIZED=1
# Wed, 09 Jun 2021 15:52:57 GMT
ENV NATS_SERVER=2.2.6
# Wed, 09 Jun 2021 15:52:59 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.2.6/nats-server-v2.2.6-windows-amd64.zip
# Wed, 09 Jun 2021 15:53:01 GMT
ENV GIT_DOWNLOAD_SHA256=c1712f41e4e811027701a036b6ff67b1f09fb298b0674098b26f875d37e709b2
# Wed, 09 Jun 2021 15:53:32 GMT
RUN Set-PSDebug -Trace 2
# Wed, 09 Jun 2021 15:54:42 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 09 Jun 2021 15:54:44 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 09 Jun 2021 15:54:47 GMT
EXPOSE 4222 6222 8222
# Wed, 09 Jun 2021 15:54:49 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 09 Jun 2021 15:54:51 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:639bb6bb2beb4cfdcacb9f0844344448fe26494665d5fe78a494419f86fbb18f`  
		Size: 923.3 MB (923252167 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ae7d2dc4b590128efeafd375d02122e65a2525623ac2be100c1a390caf8a4b49`  
		Last Modified: Wed, 09 Jun 2021 15:28:02 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:507a90d55d261855b42c7b5905599cdc274ca135ad962fffffe1fa6246c9bba7`  
		Last Modified: Wed, 09 Jun 2021 15:59:38 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58a0385e3ae1d1d8c00cf0ca66edc248c97d96c91e476559b29c6c52c46d3fe8`  
		Last Modified: Wed, 09 Jun 2021 15:59:37 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4e1c1a9e404ff727f004e12aef5245aa88eb270ce9e3f73be3e85f2df635f3f`  
		Last Modified: Wed, 09 Jun 2021 15:59:37 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a88b6cac0f81b699f58105a6102b27018ddf36099cc8cf069fa44ad96e2fa0b`  
		Last Modified: Wed, 09 Jun 2021 15:59:37 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dda44751dc046b037f6feced0dd9d70b6acfe04fc9099997ee322d8207cbe35c`  
		Last Modified: Wed, 09 Jun 2021 15:59:37 GMT  
		Size: 343.2 KB (343169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7df0a3f2eb0c7743406c39664c54d6dce8e83061bfa9d6fdc98ddb08231f479`  
		Last Modified: Wed, 09 Jun 2021 15:59:36 GMT  
		Size: 4.6 MB (4630934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ebd05a6c49ff1da6167088c0efd1b8272094cd2930c4d10b9c4423900006425`  
		Last Modified: Wed, 09 Jun 2021 15:59:34 GMT  
		Size: 2.0 KB (1976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:017fad8ec54342ed6819d801e462a0d9586120616b12bdac050efd3b2b3f10ed`  
		Last Modified: Wed, 09 Jun 2021 15:59:34 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4498408c64a82cbf1b4299f721bce414f88e9db0c6fdd6ec622145e162095d7a`  
		Last Modified: Wed, 09 Jun 2021 15:59:34 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11779cb16754ca0392b14675af366dbb6f10875912082da0e4faaad270fedc8b`  
		Last Modified: Wed, 09 Jun 2021 15:59:34 GMT  
		Size: 1.4 KB (1443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-windowsservercore` - windows version 10.0.14393.4467; amd64

```console
$ docker pull nats@sha256:6e91913decc2a4bf6631d6c1ed5778e84342adc058acd2d9d9e9087b094da085
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6275203768 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe3a6d5b045a5442f1b6cafb40ecfb21592694d830e3dcf02806137974a5bc94`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Sun, 06 Jun 2021 15:37:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 09 Jun 2021 13:26:15 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Jun 2021 15:55:27 GMT
ENV NATS_DOCKERIZED=1
# Wed, 09 Jun 2021 15:55:30 GMT
ENV NATS_SERVER=2.2.6
# Wed, 09 Jun 2021 15:55:32 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.2.6/nats-server-v2.2.6-windows-amd64.zip
# Wed, 09 Jun 2021 15:55:34 GMT
ENV GIT_DOWNLOAD_SHA256=c1712f41e4e811027701a036b6ff67b1f09fb298b0674098b26f875d37e709b2
# Wed, 09 Jun 2021 15:56:47 GMT
RUN Set-PSDebug -Trace 2
# Wed, 09 Jun 2021 15:58:51 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 09 Jun 2021 15:58:53 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 09 Jun 2021 15:58:55 GMT
EXPOSE 4222 6222 8222
# Wed, 09 Jun 2021 15:58:58 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 09 Jun 2021 15:59:00 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2f52abeee6d6f4a925ad418b5e6200d4fca9bf92834ffc918b8bbaccd34251db`  
		Size: 2.2 GB (2195741359 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:fa4e6085e5538e957ef06561fe1e62dff898da7f4bb577e81da74323aecab2d7`  
		Last Modified: Wed, 09 Jun 2021 15:28:27 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7db57f94547be7109ad927e2f9d04a0501a2a5f0cb91ad8c4385eb32758f86b9`  
		Last Modified: Wed, 09 Jun 2021 16:00:21 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbc5017d27bf2f39955e298905f004a5999d929508e8b509e647d3432f8149ae`  
		Last Modified: Wed, 09 Jun 2021 16:00:18 GMT  
		Size: 1.4 KB (1379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad9d2c3aac632d05fde125d210746bf905438eeb4275fd89897ced5a1e237610`  
		Last Modified: Wed, 09 Jun 2021 16:00:18 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:defd74399fc019d7b0578a6724c0ac2c0eed04a8ae798590dcc568f83ffe3e67`  
		Last Modified: Wed, 09 Jun 2021 16:00:18 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76a97163f551fdbf75334ad37f6d16e6fe2d77ece5522d279046cd346d153b42`  
		Last Modified: Wed, 09 Jun 2021 16:00:18 GMT  
		Size: 341.5 KB (341515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecac4038087ee903af4019f7607dfc1e6850bfcd85c0b5e05c3132918b35dd90`  
		Last Modified: Wed, 09 Jun 2021 16:00:27 GMT  
		Size: 9.1 MB (9121804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f76428eff7b847a4fe7562a4795f520e7c7784527bb82c3074f2364b06f8cf69`  
		Last Modified: Wed, 09 Jun 2021 16:00:16 GMT  
		Size: 1.9 KB (1937 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4da349fd26102b808fd3307d65d0fe3c971879a8b7dad5b2e4ff228e1236614`  
		Last Modified: Wed, 09 Jun 2021 16:00:16 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8855b9c66052a7932dd8f755b14dbcc1581a824febee8a011b90f4213b2a3242`  
		Last Modified: Wed, 09 Jun 2021 16:00:16 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f1a11333ba3d20e4c4e4312c4d3840fdb58724a21cc62f43e8ded134e7b3682`  
		Last Modified: Wed, 09 Jun 2021 16:00:16 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-windowsservercore-1809`

```console
$ docker pull nats@sha256:e86cdc0cb1ce27e7d790872f30cdcbcefbe40bb9cc7a818e4dac93051c9f3e18
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1999; amd64

### `nats:2-windowsservercore-1809` - windows version 10.0.17763.1999; amd64

```console
$ docker pull nats@sha256:b02d0fddc42e8f50f6dccf56bc6da2c299fa6ca12dac2a91142f5ea6f3c3b4d2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2646572446 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec0469d99bdcdeb93ecb4cd714c002dc5344cdd980081af67522abd90cb61f56`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sun, 06 Jun 2021 04:28:43 GMT
RUN Install update 1809-amd64
# Wed, 09 Jun 2021 13:15:43 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Jun 2021 15:52:54 GMT
ENV NATS_DOCKERIZED=1
# Wed, 09 Jun 2021 15:52:57 GMT
ENV NATS_SERVER=2.2.6
# Wed, 09 Jun 2021 15:52:59 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.2.6/nats-server-v2.2.6-windows-amd64.zip
# Wed, 09 Jun 2021 15:53:01 GMT
ENV GIT_DOWNLOAD_SHA256=c1712f41e4e811027701a036b6ff67b1f09fb298b0674098b26f875d37e709b2
# Wed, 09 Jun 2021 15:53:32 GMT
RUN Set-PSDebug -Trace 2
# Wed, 09 Jun 2021 15:54:42 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 09 Jun 2021 15:54:44 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 09 Jun 2021 15:54:47 GMT
EXPOSE 4222 6222 8222
# Wed, 09 Jun 2021 15:54:49 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 09 Jun 2021 15:54:51 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:639bb6bb2beb4cfdcacb9f0844344448fe26494665d5fe78a494419f86fbb18f`  
		Size: 923.3 MB (923252167 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ae7d2dc4b590128efeafd375d02122e65a2525623ac2be100c1a390caf8a4b49`  
		Last Modified: Wed, 09 Jun 2021 15:28:02 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:507a90d55d261855b42c7b5905599cdc274ca135ad962fffffe1fa6246c9bba7`  
		Last Modified: Wed, 09 Jun 2021 15:59:38 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58a0385e3ae1d1d8c00cf0ca66edc248c97d96c91e476559b29c6c52c46d3fe8`  
		Last Modified: Wed, 09 Jun 2021 15:59:37 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4e1c1a9e404ff727f004e12aef5245aa88eb270ce9e3f73be3e85f2df635f3f`  
		Last Modified: Wed, 09 Jun 2021 15:59:37 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a88b6cac0f81b699f58105a6102b27018ddf36099cc8cf069fa44ad96e2fa0b`  
		Last Modified: Wed, 09 Jun 2021 15:59:37 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dda44751dc046b037f6feced0dd9d70b6acfe04fc9099997ee322d8207cbe35c`  
		Last Modified: Wed, 09 Jun 2021 15:59:37 GMT  
		Size: 343.2 KB (343169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7df0a3f2eb0c7743406c39664c54d6dce8e83061bfa9d6fdc98ddb08231f479`  
		Last Modified: Wed, 09 Jun 2021 15:59:36 GMT  
		Size: 4.6 MB (4630934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ebd05a6c49ff1da6167088c0efd1b8272094cd2930c4d10b9c4423900006425`  
		Last Modified: Wed, 09 Jun 2021 15:59:34 GMT  
		Size: 2.0 KB (1976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:017fad8ec54342ed6819d801e462a0d9586120616b12bdac050efd3b2b3f10ed`  
		Last Modified: Wed, 09 Jun 2021 15:59:34 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4498408c64a82cbf1b4299f721bce414f88e9db0c6fdd6ec622145e162095d7a`  
		Last Modified: Wed, 09 Jun 2021 15:59:34 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11779cb16754ca0392b14675af366dbb6f10875912082da0e4faaad270fedc8b`  
		Last Modified: Wed, 09 Jun 2021 15:59:34 GMT  
		Size: 1.4 KB (1443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-windowsservercore-ltsc2016`

```console
$ docker pull nats@sha256:aa8b74dbfe213c84911b8c47dac74da599ad57326e421c97b17e1b61bae86e51
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4467; amd64

### `nats:2-windowsservercore-ltsc2016` - windows version 10.0.14393.4467; amd64

```console
$ docker pull nats@sha256:6e91913decc2a4bf6631d6c1ed5778e84342adc058acd2d9d9e9087b094da085
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6275203768 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe3a6d5b045a5442f1b6cafb40ecfb21592694d830e3dcf02806137974a5bc94`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Sun, 06 Jun 2021 15:37:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 09 Jun 2021 13:26:15 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Jun 2021 15:55:27 GMT
ENV NATS_DOCKERIZED=1
# Wed, 09 Jun 2021 15:55:30 GMT
ENV NATS_SERVER=2.2.6
# Wed, 09 Jun 2021 15:55:32 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.2.6/nats-server-v2.2.6-windows-amd64.zip
# Wed, 09 Jun 2021 15:55:34 GMT
ENV GIT_DOWNLOAD_SHA256=c1712f41e4e811027701a036b6ff67b1f09fb298b0674098b26f875d37e709b2
# Wed, 09 Jun 2021 15:56:47 GMT
RUN Set-PSDebug -Trace 2
# Wed, 09 Jun 2021 15:58:51 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 09 Jun 2021 15:58:53 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 09 Jun 2021 15:58:55 GMT
EXPOSE 4222 6222 8222
# Wed, 09 Jun 2021 15:58:58 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 09 Jun 2021 15:59:00 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2f52abeee6d6f4a925ad418b5e6200d4fca9bf92834ffc918b8bbaccd34251db`  
		Size: 2.2 GB (2195741359 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:fa4e6085e5538e957ef06561fe1e62dff898da7f4bb577e81da74323aecab2d7`  
		Last Modified: Wed, 09 Jun 2021 15:28:27 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7db57f94547be7109ad927e2f9d04a0501a2a5f0cb91ad8c4385eb32758f86b9`  
		Last Modified: Wed, 09 Jun 2021 16:00:21 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbc5017d27bf2f39955e298905f004a5999d929508e8b509e647d3432f8149ae`  
		Last Modified: Wed, 09 Jun 2021 16:00:18 GMT  
		Size: 1.4 KB (1379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad9d2c3aac632d05fde125d210746bf905438eeb4275fd89897ced5a1e237610`  
		Last Modified: Wed, 09 Jun 2021 16:00:18 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:defd74399fc019d7b0578a6724c0ac2c0eed04a8ae798590dcc568f83ffe3e67`  
		Last Modified: Wed, 09 Jun 2021 16:00:18 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76a97163f551fdbf75334ad37f6d16e6fe2d77ece5522d279046cd346d153b42`  
		Last Modified: Wed, 09 Jun 2021 16:00:18 GMT  
		Size: 341.5 KB (341515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecac4038087ee903af4019f7607dfc1e6850bfcd85c0b5e05c3132918b35dd90`  
		Last Modified: Wed, 09 Jun 2021 16:00:27 GMT  
		Size: 9.1 MB (9121804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f76428eff7b847a4fe7562a4795f520e7c7784527bb82c3074f2364b06f8cf69`  
		Last Modified: Wed, 09 Jun 2021 16:00:16 GMT  
		Size: 1.9 KB (1937 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4da349fd26102b808fd3307d65d0fe3c971879a8b7dad5b2e4ff228e1236614`  
		Last Modified: Wed, 09 Jun 2021 16:00:16 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8855b9c66052a7932dd8f755b14dbcc1581a824febee8a011b90f4213b2a3242`  
		Last Modified: Wed, 09 Jun 2021 16:00:16 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f1a11333ba3d20e4c4e4312c4d3840fdb58724a21cc62f43e8ded134e7b3682`  
		Last Modified: Wed, 09 Jun 2021 16:00:16 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.2`

```console
$ docker pull nats@sha256:ed66dfeef8f3c691f17ac8920b46054de09796a3b7a5bd3e96cb234a87915523
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.1999; amd64

### `nats:2.2` - linux; amd64

```console
$ docker pull nats@sha256:bad1b98cb238be899761405ed9a084eb4cee1e4982c4082414a49e1e47d83993
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4249359 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3903d09e582715d83e8da5706ee14109824854452c0ebf177eb55dfb789e311`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 25 May 2021 01:38:34 GMT
COPY file:6d5e77e6be5bafda9b9e03a4f397b21f9432694e3c3c3b5cd6e621b4c3ec3018 in /nats-server 
# Tue, 25 May 2021 01:38:34 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Tue, 25 May 2021 01:38:34 GMT
EXPOSE 4222 6222 8222
# Tue, 25 May 2021 01:38:34 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 25 May 2021 01:38:35 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:bf9e6d973acc267c8b0f05973d840142eec057566b36d0ae18177113f1fdadda`  
		Last Modified: Tue, 25 May 2021 01:39:26 GMT  
		Size: 4.2 MB (4248883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14a60a1c8cdedd7b360929beb64e25bbab3d679ba8134844479aaa6169d73595`  
		Last Modified: Tue, 25 May 2021 01:39:25 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2` - linux; arm variant v6

```console
$ docker pull nats@sha256:f98c4fa99482edcc01991046e5e9b2650e6181ec78b070d6601adef0afbbc3d9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3916550 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:573ae66ceb9d5149762ca1a8585b9f794bc0c0372ce18f73beefebb086f898c1`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 26 May 2021 18:22:59 GMT
COPY file:09c6eee4fb87ec105cf70b09816e278a49955f5e23576db600bfdb2fff0d6633 in /nats-server 
# Wed, 26 May 2021 18:23:00 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Wed, 26 May 2021 18:23:00 GMT
EXPOSE 4222 6222 8222
# Wed, 26 May 2021 18:23:00 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 26 May 2021 18:23:00 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:069976a4471c1abc4ad7dc33e5d7ed35c51e717ae622a055b7e925dd0bbe2ccb`  
		Last Modified: Wed, 26 May 2021 18:24:53 GMT  
		Size: 3.9 MB (3916076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4094f904541e138a0436baf31ea6b5ed4b91aee4871a54fce1650f2d63d2da2`  
		Last Modified: Wed, 26 May 2021 18:24:52 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2` - linux; arm variant v7

```console
$ docker pull nats@sha256:593e1b418f3e55050730f63b1d5da6e5f6f9c990c66e15bb9cd6659ea836279f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3914539 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4093ac9e36206435159f30858c34c7ed656e69e8dcbe1aaa6fbd40099701ade7`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 25 May 2021 22:23:02 GMT
COPY file:1ccce8553c778be1204380469e7248fd9ee472bdec35db0b7dd150122ae7c37d in /nats-server 
# Tue, 25 May 2021 22:23:02 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Tue, 25 May 2021 22:23:03 GMT
EXPOSE 4222 6222 8222
# Tue, 25 May 2021 22:23:03 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 25 May 2021 22:23:03 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a459b50ce258c1a3884cfc6f671ebabe9d05421a39962966809134623f3b9979`  
		Last Modified: Tue, 25 May 2021 22:24:59 GMT  
		Size: 3.9 MB (3914063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1808b616cb182b07285cb2e4b7d289755ccf8fa8575a8bc73a20ae46f8f253a`  
		Last Modified: Tue, 25 May 2021 22:24:58 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:8d8addd19d02a411d04db404a43383648e6a39e5a6686d5c2870bd5a0b80c546
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3889451 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b2ba9cf0b70339a1dd0b4bc93c1c83f00d829cd27d85adabe9b5ef7fdfefc69`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 26 May 2021 23:34:44 GMT
COPY file:312f19d8ade34bbf7590dddfdd3664f3152040117d8296ec0a54e9a9f7f42ae7 in /nats-server 
# Wed, 26 May 2021 23:34:45 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Wed, 26 May 2021 23:34:45 GMT
EXPOSE 4222 6222 8222
# Wed, 26 May 2021 23:34:45 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 26 May 2021 23:34:45 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:529a1438983ee1d8a2fdcab2846023465327ab9d8b15f0a7ed6ce61ff67fb8e8`  
		Last Modified: Wed, 26 May 2021 23:36:07 GMT  
		Size: 3.9 MB (3888976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:411d0165541f17c63026ae51d40e5a1f09909f0ab49fdadc7c2c7d904a4a3cb9`  
		Last Modified: Wed, 26 May 2021 23:36:06 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2` - windows version 10.0.17763.1999; amd64

```console
$ docker pull nats@sha256:7305d7bf57da3e44ce9e5b368d294f4d9a6f86908ee0522b2e3af953bbfeaeb8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.0 MB (106983364 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:448497fc5d2a9aa4a4fe1404fa1f9cbd4a6cabcc2593a935a7e18d9ca49f7743`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sun, 06 Jun 2021 04:04:04 GMT
RUN Apply image 1809-amd64
# Wed, 09 Jun 2021 15:55:07 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 09 Jun 2021 15:55:09 GMT
RUN cmd /S /C #(nop) COPY file:a13acc0f2f64f12c4304c7730a47bebb73f06865d8dee680ec7a370c77d69e10 in C:\nats-server.exe 
# Wed, 09 Jun 2021 15:55:12 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 09 Jun 2021 15:55:14 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 09 Jun 2021 15:55:17 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 09 Jun 2021 15:55:19 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:e4800203e906d49fbdaf1eeab4de72f28796d5b9a1ea44f8d7461001cfa56614`  
		Size: 102.7 MB (102671454 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:80d93ce19113bbf944b699f12e59395e0eabeb00ccd1fd5dc7df46bb115eba2f`  
		Last Modified: Wed, 09 Jun 2021 15:59:58 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02a2af79aa85193c9d59672eaa3d7792de702370a62c15d646ca3d6e9805a4e3`  
		Last Modified: Wed, 09 Jun 2021 15:59:57 GMT  
		Size: 4.3 MB (4305480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9e0f71986494c926842ef864b29a5d7f3467a0415538fa78ad7850693a7b9d2`  
		Last Modified: Wed, 09 Jun 2021 15:59:56 GMT  
		Size: 1.8 KB (1752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74462c7c877f0c6efdd4131bf6b4ddf0ab34ceaa3aaeec8ca8d0b9f3fe614731`  
		Last Modified: Wed, 09 Jun 2021 15:59:56 GMT  
		Size: 1.2 KB (1192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cff02dcbfcaa11d91acbf9f579c2dc701b2c0a8057cb1b98b85a60bdeac38ba`  
		Last Modified: Wed, 09 Jun 2021 15:59:55 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56f9ea8a05c1d3919aab5e228736bf5b7f7dfd2493d7450e95724e6a41aab47b`  
		Last Modified: Wed, 09 Jun 2021 15:59:56 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.2-alpine`

```console
$ docker pull nats@sha256:cc2bde1fe965db9ac2011073b071010691ebdb1904c7933922ad2a107a5a7a34
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.2-alpine` - linux; amd64

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

### `nats:2.2-alpine` - linux; arm variant v6

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

### `nats:2.2-alpine` - linux; arm variant v7

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

### `nats:2.2-alpine` - linux; arm64 variant v8

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

## `nats:2.2-alpine3.13`

```console
$ docker pull nats@sha256:cc2bde1fe965db9ac2011073b071010691ebdb1904c7933922ad2a107a5a7a34
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.2-alpine3.13` - linux; amd64

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

### `nats:2.2-alpine3.13` - linux; arm variant v6

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

### `nats:2.2-alpine3.13` - linux; arm variant v7

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

### `nats:2.2-alpine3.13` - linux; arm64 variant v8

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

## `nats:2.2-linux`

```console
$ docker pull nats@sha256:8aceb3b18cc40ba1aa1d88ac3d22108e02e7a43cae6d2b66910dcfa80d437885
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.2-linux` - linux; amd64

```console
$ docker pull nats@sha256:bad1b98cb238be899761405ed9a084eb4cee1e4982c4082414a49e1e47d83993
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4249359 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3903d09e582715d83e8da5706ee14109824854452c0ebf177eb55dfb789e311`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 25 May 2021 01:38:34 GMT
COPY file:6d5e77e6be5bafda9b9e03a4f397b21f9432694e3c3c3b5cd6e621b4c3ec3018 in /nats-server 
# Tue, 25 May 2021 01:38:34 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Tue, 25 May 2021 01:38:34 GMT
EXPOSE 4222 6222 8222
# Tue, 25 May 2021 01:38:34 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 25 May 2021 01:38:35 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:bf9e6d973acc267c8b0f05973d840142eec057566b36d0ae18177113f1fdadda`  
		Last Modified: Tue, 25 May 2021 01:39:26 GMT  
		Size: 4.2 MB (4248883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14a60a1c8cdedd7b360929beb64e25bbab3d679ba8134844479aaa6169d73595`  
		Last Modified: Tue, 25 May 2021 01:39:25 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2-linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:f98c4fa99482edcc01991046e5e9b2650e6181ec78b070d6601adef0afbbc3d9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3916550 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:573ae66ceb9d5149762ca1a8585b9f794bc0c0372ce18f73beefebb086f898c1`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 26 May 2021 18:22:59 GMT
COPY file:09c6eee4fb87ec105cf70b09816e278a49955f5e23576db600bfdb2fff0d6633 in /nats-server 
# Wed, 26 May 2021 18:23:00 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Wed, 26 May 2021 18:23:00 GMT
EXPOSE 4222 6222 8222
# Wed, 26 May 2021 18:23:00 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 26 May 2021 18:23:00 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:069976a4471c1abc4ad7dc33e5d7ed35c51e717ae622a055b7e925dd0bbe2ccb`  
		Last Modified: Wed, 26 May 2021 18:24:53 GMT  
		Size: 3.9 MB (3916076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4094f904541e138a0436baf31ea6b5ed4b91aee4871a54fce1650f2d63d2da2`  
		Last Modified: Wed, 26 May 2021 18:24:52 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2-linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:593e1b418f3e55050730f63b1d5da6e5f6f9c990c66e15bb9cd6659ea836279f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3914539 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4093ac9e36206435159f30858c34c7ed656e69e8dcbe1aaa6fbd40099701ade7`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 25 May 2021 22:23:02 GMT
COPY file:1ccce8553c778be1204380469e7248fd9ee472bdec35db0b7dd150122ae7c37d in /nats-server 
# Tue, 25 May 2021 22:23:02 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Tue, 25 May 2021 22:23:03 GMT
EXPOSE 4222 6222 8222
# Tue, 25 May 2021 22:23:03 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 25 May 2021 22:23:03 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a459b50ce258c1a3884cfc6f671ebabe9d05421a39962966809134623f3b9979`  
		Last Modified: Tue, 25 May 2021 22:24:59 GMT  
		Size: 3.9 MB (3914063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1808b616cb182b07285cb2e4b7d289755ccf8fa8575a8bc73a20ae46f8f253a`  
		Last Modified: Tue, 25 May 2021 22:24:58 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2-linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:8d8addd19d02a411d04db404a43383648e6a39e5a6686d5c2870bd5a0b80c546
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3889451 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b2ba9cf0b70339a1dd0b4bc93c1c83f00d829cd27d85adabe9b5ef7fdfefc69`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 26 May 2021 23:34:44 GMT
COPY file:312f19d8ade34bbf7590dddfdd3664f3152040117d8296ec0a54e9a9f7f42ae7 in /nats-server 
# Wed, 26 May 2021 23:34:45 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Wed, 26 May 2021 23:34:45 GMT
EXPOSE 4222 6222 8222
# Wed, 26 May 2021 23:34:45 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 26 May 2021 23:34:45 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:529a1438983ee1d8a2fdcab2846023465327ab9d8b15f0a7ed6ce61ff67fb8e8`  
		Last Modified: Wed, 26 May 2021 23:36:07 GMT  
		Size: 3.9 MB (3888976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:411d0165541f17c63026ae51d40e5a1f09909f0ab49fdadc7c2c7d904a4a3cb9`  
		Last Modified: Wed, 26 May 2021 23:36:06 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.2-nanoserver`

```console
$ docker pull nats@sha256:a0aacfbc002543c9a2dac717593b25e60fe52c18ec1033479d2a8fd25bab8391
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1999; amd64

### `nats:2.2-nanoserver` - windows version 10.0.17763.1999; amd64

```console
$ docker pull nats@sha256:7305d7bf57da3e44ce9e5b368d294f4d9a6f86908ee0522b2e3af953bbfeaeb8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.0 MB (106983364 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:448497fc5d2a9aa4a4fe1404fa1f9cbd4a6cabcc2593a935a7e18d9ca49f7743`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sun, 06 Jun 2021 04:04:04 GMT
RUN Apply image 1809-amd64
# Wed, 09 Jun 2021 15:55:07 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 09 Jun 2021 15:55:09 GMT
RUN cmd /S /C #(nop) COPY file:a13acc0f2f64f12c4304c7730a47bebb73f06865d8dee680ec7a370c77d69e10 in C:\nats-server.exe 
# Wed, 09 Jun 2021 15:55:12 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 09 Jun 2021 15:55:14 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 09 Jun 2021 15:55:17 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 09 Jun 2021 15:55:19 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:e4800203e906d49fbdaf1eeab4de72f28796d5b9a1ea44f8d7461001cfa56614`  
		Size: 102.7 MB (102671454 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:80d93ce19113bbf944b699f12e59395e0eabeb00ccd1fd5dc7df46bb115eba2f`  
		Last Modified: Wed, 09 Jun 2021 15:59:58 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02a2af79aa85193c9d59672eaa3d7792de702370a62c15d646ca3d6e9805a4e3`  
		Last Modified: Wed, 09 Jun 2021 15:59:57 GMT  
		Size: 4.3 MB (4305480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9e0f71986494c926842ef864b29a5d7f3467a0415538fa78ad7850693a7b9d2`  
		Last Modified: Wed, 09 Jun 2021 15:59:56 GMT  
		Size: 1.8 KB (1752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74462c7c877f0c6efdd4131bf6b4ddf0ab34ceaa3aaeec8ca8d0b9f3fe614731`  
		Last Modified: Wed, 09 Jun 2021 15:59:56 GMT  
		Size: 1.2 KB (1192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cff02dcbfcaa11d91acbf9f579c2dc701b2c0a8057cb1b98b85a60bdeac38ba`  
		Last Modified: Wed, 09 Jun 2021 15:59:55 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56f9ea8a05c1d3919aab5e228736bf5b7f7dfd2493d7450e95724e6a41aab47b`  
		Last Modified: Wed, 09 Jun 2021 15:59:56 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.2-nanoserver-1809`

```console
$ docker pull nats@sha256:a0aacfbc002543c9a2dac717593b25e60fe52c18ec1033479d2a8fd25bab8391
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1999; amd64

### `nats:2.2-nanoserver-1809` - windows version 10.0.17763.1999; amd64

```console
$ docker pull nats@sha256:7305d7bf57da3e44ce9e5b368d294f4d9a6f86908ee0522b2e3af953bbfeaeb8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.0 MB (106983364 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:448497fc5d2a9aa4a4fe1404fa1f9cbd4a6cabcc2593a935a7e18d9ca49f7743`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sun, 06 Jun 2021 04:04:04 GMT
RUN Apply image 1809-amd64
# Wed, 09 Jun 2021 15:55:07 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 09 Jun 2021 15:55:09 GMT
RUN cmd /S /C #(nop) COPY file:a13acc0f2f64f12c4304c7730a47bebb73f06865d8dee680ec7a370c77d69e10 in C:\nats-server.exe 
# Wed, 09 Jun 2021 15:55:12 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 09 Jun 2021 15:55:14 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 09 Jun 2021 15:55:17 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 09 Jun 2021 15:55:19 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:e4800203e906d49fbdaf1eeab4de72f28796d5b9a1ea44f8d7461001cfa56614`  
		Size: 102.7 MB (102671454 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:80d93ce19113bbf944b699f12e59395e0eabeb00ccd1fd5dc7df46bb115eba2f`  
		Last Modified: Wed, 09 Jun 2021 15:59:58 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02a2af79aa85193c9d59672eaa3d7792de702370a62c15d646ca3d6e9805a4e3`  
		Last Modified: Wed, 09 Jun 2021 15:59:57 GMT  
		Size: 4.3 MB (4305480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9e0f71986494c926842ef864b29a5d7f3467a0415538fa78ad7850693a7b9d2`  
		Last Modified: Wed, 09 Jun 2021 15:59:56 GMT  
		Size: 1.8 KB (1752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74462c7c877f0c6efdd4131bf6b4ddf0ab34ceaa3aaeec8ca8d0b9f3fe614731`  
		Last Modified: Wed, 09 Jun 2021 15:59:56 GMT  
		Size: 1.2 KB (1192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cff02dcbfcaa11d91acbf9f579c2dc701b2c0a8057cb1b98b85a60bdeac38ba`  
		Last Modified: Wed, 09 Jun 2021 15:59:55 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56f9ea8a05c1d3919aab5e228736bf5b7f7dfd2493d7450e95724e6a41aab47b`  
		Last Modified: Wed, 09 Jun 2021 15:59:56 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.2-scratch`

```console
$ docker pull nats@sha256:8aceb3b18cc40ba1aa1d88ac3d22108e02e7a43cae6d2b66910dcfa80d437885
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.2-scratch` - linux; amd64

```console
$ docker pull nats@sha256:bad1b98cb238be899761405ed9a084eb4cee1e4982c4082414a49e1e47d83993
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4249359 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3903d09e582715d83e8da5706ee14109824854452c0ebf177eb55dfb789e311`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 25 May 2021 01:38:34 GMT
COPY file:6d5e77e6be5bafda9b9e03a4f397b21f9432694e3c3c3b5cd6e621b4c3ec3018 in /nats-server 
# Tue, 25 May 2021 01:38:34 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Tue, 25 May 2021 01:38:34 GMT
EXPOSE 4222 6222 8222
# Tue, 25 May 2021 01:38:34 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 25 May 2021 01:38:35 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:bf9e6d973acc267c8b0f05973d840142eec057566b36d0ae18177113f1fdadda`  
		Last Modified: Tue, 25 May 2021 01:39:26 GMT  
		Size: 4.2 MB (4248883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14a60a1c8cdedd7b360929beb64e25bbab3d679ba8134844479aaa6169d73595`  
		Last Modified: Tue, 25 May 2021 01:39:25 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2-scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:f98c4fa99482edcc01991046e5e9b2650e6181ec78b070d6601adef0afbbc3d9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3916550 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:573ae66ceb9d5149762ca1a8585b9f794bc0c0372ce18f73beefebb086f898c1`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 26 May 2021 18:22:59 GMT
COPY file:09c6eee4fb87ec105cf70b09816e278a49955f5e23576db600bfdb2fff0d6633 in /nats-server 
# Wed, 26 May 2021 18:23:00 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Wed, 26 May 2021 18:23:00 GMT
EXPOSE 4222 6222 8222
# Wed, 26 May 2021 18:23:00 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 26 May 2021 18:23:00 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:069976a4471c1abc4ad7dc33e5d7ed35c51e717ae622a055b7e925dd0bbe2ccb`  
		Last Modified: Wed, 26 May 2021 18:24:53 GMT  
		Size: 3.9 MB (3916076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4094f904541e138a0436baf31ea6b5ed4b91aee4871a54fce1650f2d63d2da2`  
		Last Modified: Wed, 26 May 2021 18:24:52 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2-scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:593e1b418f3e55050730f63b1d5da6e5f6f9c990c66e15bb9cd6659ea836279f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3914539 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4093ac9e36206435159f30858c34c7ed656e69e8dcbe1aaa6fbd40099701ade7`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 25 May 2021 22:23:02 GMT
COPY file:1ccce8553c778be1204380469e7248fd9ee472bdec35db0b7dd150122ae7c37d in /nats-server 
# Tue, 25 May 2021 22:23:02 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Tue, 25 May 2021 22:23:03 GMT
EXPOSE 4222 6222 8222
# Tue, 25 May 2021 22:23:03 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 25 May 2021 22:23:03 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a459b50ce258c1a3884cfc6f671ebabe9d05421a39962966809134623f3b9979`  
		Last Modified: Tue, 25 May 2021 22:24:59 GMT  
		Size: 3.9 MB (3914063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1808b616cb182b07285cb2e4b7d289755ccf8fa8575a8bc73a20ae46f8f253a`  
		Last Modified: Tue, 25 May 2021 22:24:58 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2-scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:8d8addd19d02a411d04db404a43383648e6a39e5a6686d5c2870bd5a0b80c546
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3889451 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b2ba9cf0b70339a1dd0b4bc93c1c83f00d829cd27d85adabe9b5ef7fdfefc69`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 26 May 2021 23:34:44 GMT
COPY file:312f19d8ade34bbf7590dddfdd3664f3152040117d8296ec0a54e9a9f7f42ae7 in /nats-server 
# Wed, 26 May 2021 23:34:45 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Wed, 26 May 2021 23:34:45 GMT
EXPOSE 4222 6222 8222
# Wed, 26 May 2021 23:34:45 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 26 May 2021 23:34:45 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:529a1438983ee1d8a2fdcab2846023465327ab9d8b15f0a7ed6ce61ff67fb8e8`  
		Last Modified: Wed, 26 May 2021 23:36:07 GMT  
		Size: 3.9 MB (3888976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:411d0165541f17c63026ae51d40e5a1f09909f0ab49fdadc7c2c7d904a4a3cb9`  
		Last Modified: Wed, 26 May 2021 23:36:06 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.2-windowsservercore`

```console
$ docker pull nats@sha256:334a5bbe37d543b1a8fcbd110923b8ac58c7095ba41eace53d0005932cd0899e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1999; amd64
	-	windows version 10.0.14393.4467; amd64

### `nats:2.2-windowsservercore` - windows version 10.0.17763.1999; amd64

```console
$ docker pull nats@sha256:b02d0fddc42e8f50f6dccf56bc6da2c299fa6ca12dac2a91142f5ea6f3c3b4d2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2646572446 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec0469d99bdcdeb93ecb4cd714c002dc5344cdd980081af67522abd90cb61f56`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sun, 06 Jun 2021 04:28:43 GMT
RUN Install update 1809-amd64
# Wed, 09 Jun 2021 13:15:43 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Jun 2021 15:52:54 GMT
ENV NATS_DOCKERIZED=1
# Wed, 09 Jun 2021 15:52:57 GMT
ENV NATS_SERVER=2.2.6
# Wed, 09 Jun 2021 15:52:59 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.2.6/nats-server-v2.2.6-windows-amd64.zip
# Wed, 09 Jun 2021 15:53:01 GMT
ENV GIT_DOWNLOAD_SHA256=c1712f41e4e811027701a036b6ff67b1f09fb298b0674098b26f875d37e709b2
# Wed, 09 Jun 2021 15:53:32 GMT
RUN Set-PSDebug -Trace 2
# Wed, 09 Jun 2021 15:54:42 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 09 Jun 2021 15:54:44 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 09 Jun 2021 15:54:47 GMT
EXPOSE 4222 6222 8222
# Wed, 09 Jun 2021 15:54:49 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 09 Jun 2021 15:54:51 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:639bb6bb2beb4cfdcacb9f0844344448fe26494665d5fe78a494419f86fbb18f`  
		Size: 923.3 MB (923252167 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ae7d2dc4b590128efeafd375d02122e65a2525623ac2be100c1a390caf8a4b49`  
		Last Modified: Wed, 09 Jun 2021 15:28:02 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:507a90d55d261855b42c7b5905599cdc274ca135ad962fffffe1fa6246c9bba7`  
		Last Modified: Wed, 09 Jun 2021 15:59:38 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58a0385e3ae1d1d8c00cf0ca66edc248c97d96c91e476559b29c6c52c46d3fe8`  
		Last Modified: Wed, 09 Jun 2021 15:59:37 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4e1c1a9e404ff727f004e12aef5245aa88eb270ce9e3f73be3e85f2df635f3f`  
		Last Modified: Wed, 09 Jun 2021 15:59:37 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a88b6cac0f81b699f58105a6102b27018ddf36099cc8cf069fa44ad96e2fa0b`  
		Last Modified: Wed, 09 Jun 2021 15:59:37 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dda44751dc046b037f6feced0dd9d70b6acfe04fc9099997ee322d8207cbe35c`  
		Last Modified: Wed, 09 Jun 2021 15:59:37 GMT  
		Size: 343.2 KB (343169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7df0a3f2eb0c7743406c39664c54d6dce8e83061bfa9d6fdc98ddb08231f479`  
		Last Modified: Wed, 09 Jun 2021 15:59:36 GMT  
		Size: 4.6 MB (4630934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ebd05a6c49ff1da6167088c0efd1b8272094cd2930c4d10b9c4423900006425`  
		Last Modified: Wed, 09 Jun 2021 15:59:34 GMT  
		Size: 2.0 KB (1976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:017fad8ec54342ed6819d801e462a0d9586120616b12bdac050efd3b2b3f10ed`  
		Last Modified: Wed, 09 Jun 2021 15:59:34 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4498408c64a82cbf1b4299f721bce414f88e9db0c6fdd6ec622145e162095d7a`  
		Last Modified: Wed, 09 Jun 2021 15:59:34 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11779cb16754ca0392b14675af366dbb6f10875912082da0e4faaad270fedc8b`  
		Last Modified: Wed, 09 Jun 2021 15:59:34 GMT  
		Size: 1.4 KB (1443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2-windowsservercore` - windows version 10.0.14393.4467; amd64

```console
$ docker pull nats@sha256:6e91913decc2a4bf6631d6c1ed5778e84342adc058acd2d9d9e9087b094da085
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6275203768 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe3a6d5b045a5442f1b6cafb40ecfb21592694d830e3dcf02806137974a5bc94`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Sun, 06 Jun 2021 15:37:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 09 Jun 2021 13:26:15 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Jun 2021 15:55:27 GMT
ENV NATS_DOCKERIZED=1
# Wed, 09 Jun 2021 15:55:30 GMT
ENV NATS_SERVER=2.2.6
# Wed, 09 Jun 2021 15:55:32 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.2.6/nats-server-v2.2.6-windows-amd64.zip
# Wed, 09 Jun 2021 15:55:34 GMT
ENV GIT_DOWNLOAD_SHA256=c1712f41e4e811027701a036b6ff67b1f09fb298b0674098b26f875d37e709b2
# Wed, 09 Jun 2021 15:56:47 GMT
RUN Set-PSDebug -Trace 2
# Wed, 09 Jun 2021 15:58:51 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 09 Jun 2021 15:58:53 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 09 Jun 2021 15:58:55 GMT
EXPOSE 4222 6222 8222
# Wed, 09 Jun 2021 15:58:58 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 09 Jun 2021 15:59:00 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2f52abeee6d6f4a925ad418b5e6200d4fca9bf92834ffc918b8bbaccd34251db`  
		Size: 2.2 GB (2195741359 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:fa4e6085e5538e957ef06561fe1e62dff898da7f4bb577e81da74323aecab2d7`  
		Last Modified: Wed, 09 Jun 2021 15:28:27 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7db57f94547be7109ad927e2f9d04a0501a2a5f0cb91ad8c4385eb32758f86b9`  
		Last Modified: Wed, 09 Jun 2021 16:00:21 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbc5017d27bf2f39955e298905f004a5999d929508e8b509e647d3432f8149ae`  
		Last Modified: Wed, 09 Jun 2021 16:00:18 GMT  
		Size: 1.4 KB (1379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad9d2c3aac632d05fde125d210746bf905438eeb4275fd89897ced5a1e237610`  
		Last Modified: Wed, 09 Jun 2021 16:00:18 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:defd74399fc019d7b0578a6724c0ac2c0eed04a8ae798590dcc568f83ffe3e67`  
		Last Modified: Wed, 09 Jun 2021 16:00:18 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76a97163f551fdbf75334ad37f6d16e6fe2d77ece5522d279046cd346d153b42`  
		Last Modified: Wed, 09 Jun 2021 16:00:18 GMT  
		Size: 341.5 KB (341515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecac4038087ee903af4019f7607dfc1e6850bfcd85c0b5e05c3132918b35dd90`  
		Last Modified: Wed, 09 Jun 2021 16:00:27 GMT  
		Size: 9.1 MB (9121804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f76428eff7b847a4fe7562a4795f520e7c7784527bb82c3074f2364b06f8cf69`  
		Last Modified: Wed, 09 Jun 2021 16:00:16 GMT  
		Size: 1.9 KB (1937 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4da349fd26102b808fd3307d65d0fe3c971879a8b7dad5b2e4ff228e1236614`  
		Last Modified: Wed, 09 Jun 2021 16:00:16 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8855b9c66052a7932dd8f755b14dbcc1581a824febee8a011b90f4213b2a3242`  
		Last Modified: Wed, 09 Jun 2021 16:00:16 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f1a11333ba3d20e4c4e4312c4d3840fdb58724a21cc62f43e8ded134e7b3682`  
		Last Modified: Wed, 09 Jun 2021 16:00:16 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.2-windowsservercore-1809`

```console
$ docker pull nats@sha256:e86cdc0cb1ce27e7d790872f30cdcbcefbe40bb9cc7a818e4dac93051c9f3e18
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1999; amd64

### `nats:2.2-windowsservercore-1809` - windows version 10.0.17763.1999; amd64

```console
$ docker pull nats@sha256:b02d0fddc42e8f50f6dccf56bc6da2c299fa6ca12dac2a91142f5ea6f3c3b4d2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2646572446 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec0469d99bdcdeb93ecb4cd714c002dc5344cdd980081af67522abd90cb61f56`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sun, 06 Jun 2021 04:28:43 GMT
RUN Install update 1809-amd64
# Wed, 09 Jun 2021 13:15:43 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Jun 2021 15:52:54 GMT
ENV NATS_DOCKERIZED=1
# Wed, 09 Jun 2021 15:52:57 GMT
ENV NATS_SERVER=2.2.6
# Wed, 09 Jun 2021 15:52:59 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.2.6/nats-server-v2.2.6-windows-amd64.zip
# Wed, 09 Jun 2021 15:53:01 GMT
ENV GIT_DOWNLOAD_SHA256=c1712f41e4e811027701a036b6ff67b1f09fb298b0674098b26f875d37e709b2
# Wed, 09 Jun 2021 15:53:32 GMT
RUN Set-PSDebug -Trace 2
# Wed, 09 Jun 2021 15:54:42 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 09 Jun 2021 15:54:44 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 09 Jun 2021 15:54:47 GMT
EXPOSE 4222 6222 8222
# Wed, 09 Jun 2021 15:54:49 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 09 Jun 2021 15:54:51 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:639bb6bb2beb4cfdcacb9f0844344448fe26494665d5fe78a494419f86fbb18f`  
		Size: 923.3 MB (923252167 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ae7d2dc4b590128efeafd375d02122e65a2525623ac2be100c1a390caf8a4b49`  
		Last Modified: Wed, 09 Jun 2021 15:28:02 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:507a90d55d261855b42c7b5905599cdc274ca135ad962fffffe1fa6246c9bba7`  
		Last Modified: Wed, 09 Jun 2021 15:59:38 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58a0385e3ae1d1d8c00cf0ca66edc248c97d96c91e476559b29c6c52c46d3fe8`  
		Last Modified: Wed, 09 Jun 2021 15:59:37 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4e1c1a9e404ff727f004e12aef5245aa88eb270ce9e3f73be3e85f2df635f3f`  
		Last Modified: Wed, 09 Jun 2021 15:59:37 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a88b6cac0f81b699f58105a6102b27018ddf36099cc8cf069fa44ad96e2fa0b`  
		Last Modified: Wed, 09 Jun 2021 15:59:37 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dda44751dc046b037f6feced0dd9d70b6acfe04fc9099997ee322d8207cbe35c`  
		Last Modified: Wed, 09 Jun 2021 15:59:37 GMT  
		Size: 343.2 KB (343169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7df0a3f2eb0c7743406c39664c54d6dce8e83061bfa9d6fdc98ddb08231f479`  
		Last Modified: Wed, 09 Jun 2021 15:59:36 GMT  
		Size: 4.6 MB (4630934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ebd05a6c49ff1da6167088c0efd1b8272094cd2930c4d10b9c4423900006425`  
		Last Modified: Wed, 09 Jun 2021 15:59:34 GMT  
		Size: 2.0 KB (1976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:017fad8ec54342ed6819d801e462a0d9586120616b12bdac050efd3b2b3f10ed`  
		Last Modified: Wed, 09 Jun 2021 15:59:34 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4498408c64a82cbf1b4299f721bce414f88e9db0c6fdd6ec622145e162095d7a`  
		Last Modified: Wed, 09 Jun 2021 15:59:34 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11779cb16754ca0392b14675af366dbb6f10875912082da0e4faaad270fedc8b`  
		Last Modified: Wed, 09 Jun 2021 15:59:34 GMT  
		Size: 1.4 KB (1443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.2-windowsservercore-ltsc2016`

```console
$ docker pull nats@sha256:aa8b74dbfe213c84911b8c47dac74da599ad57326e421c97b17e1b61bae86e51
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4467; amd64

### `nats:2.2-windowsservercore-ltsc2016` - windows version 10.0.14393.4467; amd64

```console
$ docker pull nats@sha256:6e91913decc2a4bf6631d6c1ed5778e84342adc058acd2d9d9e9087b094da085
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6275203768 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe3a6d5b045a5442f1b6cafb40ecfb21592694d830e3dcf02806137974a5bc94`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Sun, 06 Jun 2021 15:37:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 09 Jun 2021 13:26:15 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Jun 2021 15:55:27 GMT
ENV NATS_DOCKERIZED=1
# Wed, 09 Jun 2021 15:55:30 GMT
ENV NATS_SERVER=2.2.6
# Wed, 09 Jun 2021 15:55:32 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.2.6/nats-server-v2.2.6-windows-amd64.zip
# Wed, 09 Jun 2021 15:55:34 GMT
ENV GIT_DOWNLOAD_SHA256=c1712f41e4e811027701a036b6ff67b1f09fb298b0674098b26f875d37e709b2
# Wed, 09 Jun 2021 15:56:47 GMT
RUN Set-PSDebug -Trace 2
# Wed, 09 Jun 2021 15:58:51 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 09 Jun 2021 15:58:53 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 09 Jun 2021 15:58:55 GMT
EXPOSE 4222 6222 8222
# Wed, 09 Jun 2021 15:58:58 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 09 Jun 2021 15:59:00 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2f52abeee6d6f4a925ad418b5e6200d4fca9bf92834ffc918b8bbaccd34251db`  
		Size: 2.2 GB (2195741359 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:fa4e6085e5538e957ef06561fe1e62dff898da7f4bb577e81da74323aecab2d7`  
		Last Modified: Wed, 09 Jun 2021 15:28:27 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7db57f94547be7109ad927e2f9d04a0501a2a5f0cb91ad8c4385eb32758f86b9`  
		Last Modified: Wed, 09 Jun 2021 16:00:21 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbc5017d27bf2f39955e298905f004a5999d929508e8b509e647d3432f8149ae`  
		Last Modified: Wed, 09 Jun 2021 16:00:18 GMT  
		Size: 1.4 KB (1379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad9d2c3aac632d05fde125d210746bf905438eeb4275fd89897ced5a1e237610`  
		Last Modified: Wed, 09 Jun 2021 16:00:18 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:defd74399fc019d7b0578a6724c0ac2c0eed04a8ae798590dcc568f83ffe3e67`  
		Last Modified: Wed, 09 Jun 2021 16:00:18 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76a97163f551fdbf75334ad37f6d16e6fe2d77ece5522d279046cd346d153b42`  
		Last Modified: Wed, 09 Jun 2021 16:00:18 GMT  
		Size: 341.5 KB (341515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecac4038087ee903af4019f7607dfc1e6850bfcd85c0b5e05c3132918b35dd90`  
		Last Modified: Wed, 09 Jun 2021 16:00:27 GMT  
		Size: 9.1 MB (9121804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f76428eff7b847a4fe7562a4795f520e7c7784527bb82c3074f2364b06f8cf69`  
		Last Modified: Wed, 09 Jun 2021 16:00:16 GMT  
		Size: 1.9 KB (1937 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4da349fd26102b808fd3307d65d0fe3c971879a8b7dad5b2e4ff228e1236614`  
		Last Modified: Wed, 09 Jun 2021 16:00:16 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8855b9c66052a7932dd8f755b14dbcc1581a824febee8a011b90f4213b2a3242`  
		Last Modified: Wed, 09 Jun 2021 16:00:16 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f1a11333ba3d20e4c4e4312c4d3840fdb58724a21cc62f43e8ded134e7b3682`  
		Last Modified: Wed, 09 Jun 2021 16:00:16 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.2.6`

```console
$ docker pull nats@sha256:ed66dfeef8f3c691f17ac8920b46054de09796a3b7a5bd3e96cb234a87915523
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.1999; amd64

### `nats:2.2.6` - linux; amd64

```console
$ docker pull nats@sha256:bad1b98cb238be899761405ed9a084eb4cee1e4982c4082414a49e1e47d83993
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4249359 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3903d09e582715d83e8da5706ee14109824854452c0ebf177eb55dfb789e311`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 25 May 2021 01:38:34 GMT
COPY file:6d5e77e6be5bafda9b9e03a4f397b21f9432694e3c3c3b5cd6e621b4c3ec3018 in /nats-server 
# Tue, 25 May 2021 01:38:34 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Tue, 25 May 2021 01:38:34 GMT
EXPOSE 4222 6222 8222
# Tue, 25 May 2021 01:38:34 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 25 May 2021 01:38:35 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:bf9e6d973acc267c8b0f05973d840142eec057566b36d0ae18177113f1fdadda`  
		Last Modified: Tue, 25 May 2021 01:39:26 GMT  
		Size: 4.2 MB (4248883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14a60a1c8cdedd7b360929beb64e25bbab3d679ba8134844479aaa6169d73595`  
		Last Modified: Tue, 25 May 2021 01:39:25 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2.6` - linux; arm variant v6

```console
$ docker pull nats@sha256:f98c4fa99482edcc01991046e5e9b2650e6181ec78b070d6601adef0afbbc3d9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3916550 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:573ae66ceb9d5149762ca1a8585b9f794bc0c0372ce18f73beefebb086f898c1`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 26 May 2021 18:22:59 GMT
COPY file:09c6eee4fb87ec105cf70b09816e278a49955f5e23576db600bfdb2fff0d6633 in /nats-server 
# Wed, 26 May 2021 18:23:00 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Wed, 26 May 2021 18:23:00 GMT
EXPOSE 4222 6222 8222
# Wed, 26 May 2021 18:23:00 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 26 May 2021 18:23:00 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:069976a4471c1abc4ad7dc33e5d7ed35c51e717ae622a055b7e925dd0bbe2ccb`  
		Last Modified: Wed, 26 May 2021 18:24:53 GMT  
		Size: 3.9 MB (3916076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4094f904541e138a0436baf31ea6b5ed4b91aee4871a54fce1650f2d63d2da2`  
		Last Modified: Wed, 26 May 2021 18:24:52 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2.6` - linux; arm variant v7

```console
$ docker pull nats@sha256:593e1b418f3e55050730f63b1d5da6e5f6f9c990c66e15bb9cd6659ea836279f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3914539 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4093ac9e36206435159f30858c34c7ed656e69e8dcbe1aaa6fbd40099701ade7`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 25 May 2021 22:23:02 GMT
COPY file:1ccce8553c778be1204380469e7248fd9ee472bdec35db0b7dd150122ae7c37d in /nats-server 
# Tue, 25 May 2021 22:23:02 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Tue, 25 May 2021 22:23:03 GMT
EXPOSE 4222 6222 8222
# Tue, 25 May 2021 22:23:03 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 25 May 2021 22:23:03 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a459b50ce258c1a3884cfc6f671ebabe9d05421a39962966809134623f3b9979`  
		Last Modified: Tue, 25 May 2021 22:24:59 GMT  
		Size: 3.9 MB (3914063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1808b616cb182b07285cb2e4b7d289755ccf8fa8575a8bc73a20ae46f8f253a`  
		Last Modified: Tue, 25 May 2021 22:24:58 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2.6` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:8d8addd19d02a411d04db404a43383648e6a39e5a6686d5c2870bd5a0b80c546
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3889451 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b2ba9cf0b70339a1dd0b4bc93c1c83f00d829cd27d85adabe9b5ef7fdfefc69`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 26 May 2021 23:34:44 GMT
COPY file:312f19d8ade34bbf7590dddfdd3664f3152040117d8296ec0a54e9a9f7f42ae7 in /nats-server 
# Wed, 26 May 2021 23:34:45 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Wed, 26 May 2021 23:34:45 GMT
EXPOSE 4222 6222 8222
# Wed, 26 May 2021 23:34:45 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 26 May 2021 23:34:45 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:529a1438983ee1d8a2fdcab2846023465327ab9d8b15f0a7ed6ce61ff67fb8e8`  
		Last Modified: Wed, 26 May 2021 23:36:07 GMT  
		Size: 3.9 MB (3888976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:411d0165541f17c63026ae51d40e5a1f09909f0ab49fdadc7c2c7d904a4a3cb9`  
		Last Modified: Wed, 26 May 2021 23:36:06 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2.6` - windows version 10.0.17763.1999; amd64

```console
$ docker pull nats@sha256:7305d7bf57da3e44ce9e5b368d294f4d9a6f86908ee0522b2e3af953bbfeaeb8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.0 MB (106983364 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:448497fc5d2a9aa4a4fe1404fa1f9cbd4a6cabcc2593a935a7e18d9ca49f7743`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sun, 06 Jun 2021 04:04:04 GMT
RUN Apply image 1809-amd64
# Wed, 09 Jun 2021 15:55:07 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 09 Jun 2021 15:55:09 GMT
RUN cmd /S /C #(nop) COPY file:a13acc0f2f64f12c4304c7730a47bebb73f06865d8dee680ec7a370c77d69e10 in C:\nats-server.exe 
# Wed, 09 Jun 2021 15:55:12 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 09 Jun 2021 15:55:14 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 09 Jun 2021 15:55:17 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 09 Jun 2021 15:55:19 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:e4800203e906d49fbdaf1eeab4de72f28796d5b9a1ea44f8d7461001cfa56614`  
		Size: 102.7 MB (102671454 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:80d93ce19113bbf944b699f12e59395e0eabeb00ccd1fd5dc7df46bb115eba2f`  
		Last Modified: Wed, 09 Jun 2021 15:59:58 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02a2af79aa85193c9d59672eaa3d7792de702370a62c15d646ca3d6e9805a4e3`  
		Last Modified: Wed, 09 Jun 2021 15:59:57 GMT  
		Size: 4.3 MB (4305480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9e0f71986494c926842ef864b29a5d7f3467a0415538fa78ad7850693a7b9d2`  
		Last Modified: Wed, 09 Jun 2021 15:59:56 GMT  
		Size: 1.8 KB (1752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74462c7c877f0c6efdd4131bf6b4ddf0ab34ceaa3aaeec8ca8d0b9f3fe614731`  
		Last Modified: Wed, 09 Jun 2021 15:59:56 GMT  
		Size: 1.2 KB (1192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cff02dcbfcaa11d91acbf9f579c2dc701b2c0a8057cb1b98b85a60bdeac38ba`  
		Last Modified: Wed, 09 Jun 2021 15:59:55 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56f9ea8a05c1d3919aab5e228736bf5b7f7dfd2493d7450e95724e6a41aab47b`  
		Last Modified: Wed, 09 Jun 2021 15:59:56 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.2.6-alpine`

```console
$ docker pull nats@sha256:cc2bde1fe965db9ac2011073b071010691ebdb1904c7933922ad2a107a5a7a34
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.2.6-alpine` - linux; amd64

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

### `nats:2.2.6-alpine` - linux; arm variant v6

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

### `nats:2.2.6-alpine` - linux; arm variant v7

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

### `nats:2.2.6-alpine` - linux; arm64 variant v8

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

## `nats:2.2.6-alpine3.13`

```console
$ docker pull nats@sha256:cc2bde1fe965db9ac2011073b071010691ebdb1904c7933922ad2a107a5a7a34
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.2.6-alpine3.13` - linux; amd64

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

### `nats:2.2.6-alpine3.13` - linux; arm variant v6

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

### `nats:2.2.6-alpine3.13` - linux; arm variant v7

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

### `nats:2.2.6-alpine3.13` - linux; arm64 variant v8

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

## `nats:2.2.6-linux`

```console
$ docker pull nats@sha256:8aceb3b18cc40ba1aa1d88ac3d22108e02e7a43cae6d2b66910dcfa80d437885
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.2.6-linux` - linux; amd64

```console
$ docker pull nats@sha256:bad1b98cb238be899761405ed9a084eb4cee1e4982c4082414a49e1e47d83993
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4249359 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3903d09e582715d83e8da5706ee14109824854452c0ebf177eb55dfb789e311`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 25 May 2021 01:38:34 GMT
COPY file:6d5e77e6be5bafda9b9e03a4f397b21f9432694e3c3c3b5cd6e621b4c3ec3018 in /nats-server 
# Tue, 25 May 2021 01:38:34 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Tue, 25 May 2021 01:38:34 GMT
EXPOSE 4222 6222 8222
# Tue, 25 May 2021 01:38:34 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 25 May 2021 01:38:35 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:bf9e6d973acc267c8b0f05973d840142eec057566b36d0ae18177113f1fdadda`  
		Last Modified: Tue, 25 May 2021 01:39:26 GMT  
		Size: 4.2 MB (4248883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14a60a1c8cdedd7b360929beb64e25bbab3d679ba8134844479aaa6169d73595`  
		Last Modified: Tue, 25 May 2021 01:39:25 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2.6-linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:f98c4fa99482edcc01991046e5e9b2650e6181ec78b070d6601adef0afbbc3d9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3916550 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:573ae66ceb9d5149762ca1a8585b9f794bc0c0372ce18f73beefebb086f898c1`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 26 May 2021 18:22:59 GMT
COPY file:09c6eee4fb87ec105cf70b09816e278a49955f5e23576db600bfdb2fff0d6633 in /nats-server 
# Wed, 26 May 2021 18:23:00 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Wed, 26 May 2021 18:23:00 GMT
EXPOSE 4222 6222 8222
# Wed, 26 May 2021 18:23:00 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 26 May 2021 18:23:00 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:069976a4471c1abc4ad7dc33e5d7ed35c51e717ae622a055b7e925dd0bbe2ccb`  
		Last Modified: Wed, 26 May 2021 18:24:53 GMT  
		Size: 3.9 MB (3916076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4094f904541e138a0436baf31ea6b5ed4b91aee4871a54fce1650f2d63d2da2`  
		Last Modified: Wed, 26 May 2021 18:24:52 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2.6-linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:593e1b418f3e55050730f63b1d5da6e5f6f9c990c66e15bb9cd6659ea836279f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3914539 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4093ac9e36206435159f30858c34c7ed656e69e8dcbe1aaa6fbd40099701ade7`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 25 May 2021 22:23:02 GMT
COPY file:1ccce8553c778be1204380469e7248fd9ee472bdec35db0b7dd150122ae7c37d in /nats-server 
# Tue, 25 May 2021 22:23:02 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Tue, 25 May 2021 22:23:03 GMT
EXPOSE 4222 6222 8222
# Tue, 25 May 2021 22:23:03 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 25 May 2021 22:23:03 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a459b50ce258c1a3884cfc6f671ebabe9d05421a39962966809134623f3b9979`  
		Last Modified: Tue, 25 May 2021 22:24:59 GMT  
		Size: 3.9 MB (3914063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1808b616cb182b07285cb2e4b7d289755ccf8fa8575a8bc73a20ae46f8f253a`  
		Last Modified: Tue, 25 May 2021 22:24:58 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2.6-linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:8d8addd19d02a411d04db404a43383648e6a39e5a6686d5c2870bd5a0b80c546
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3889451 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b2ba9cf0b70339a1dd0b4bc93c1c83f00d829cd27d85adabe9b5ef7fdfefc69`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 26 May 2021 23:34:44 GMT
COPY file:312f19d8ade34bbf7590dddfdd3664f3152040117d8296ec0a54e9a9f7f42ae7 in /nats-server 
# Wed, 26 May 2021 23:34:45 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Wed, 26 May 2021 23:34:45 GMT
EXPOSE 4222 6222 8222
# Wed, 26 May 2021 23:34:45 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 26 May 2021 23:34:45 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:529a1438983ee1d8a2fdcab2846023465327ab9d8b15f0a7ed6ce61ff67fb8e8`  
		Last Modified: Wed, 26 May 2021 23:36:07 GMT  
		Size: 3.9 MB (3888976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:411d0165541f17c63026ae51d40e5a1f09909f0ab49fdadc7c2c7d904a4a3cb9`  
		Last Modified: Wed, 26 May 2021 23:36:06 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.2.6-nanoserver`

```console
$ docker pull nats@sha256:a0aacfbc002543c9a2dac717593b25e60fe52c18ec1033479d2a8fd25bab8391
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1999; amd64

### `nats:2.2.6-nanoserver` - windows version 10.0.17763.1999; amd64

```console
$ docker pull nats@sha256:7305d7bf57da3e44ce9e5b368d294f4d9a6f86908ee0522b2e3af953bbfeaeb8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.0 MB (106983364 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:448497fc5d2a9aa4a4fe1404fa1f9cbd4a6cabcc2593a935a7e18d9ca49f7743`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sun, 06 Jun 2021 04:04:04 GMT
RUN Apply image 1809-amd64
# Wed, 09 Jun 2021 15:55:07 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 09 Jun 2021 15:55:09 GMT
RUN cmd /S /C #(nop) COPY file:a13acc0f2f64f12c4304c7730a47bebb73f06865d8dee680ec7a370c77d69e10 in C:\nats-server.exe 
# Wed, 09 Jun 2021 15:55:12 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 09 Jun 2021 15:55:14 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 09 Jun 2021 15:55:17 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 09 Jun 2021 15:55:19 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:e4800203e906d49fbdaf1eeab4de72f28796d5b9a1ea44f8d7461001cfa56614`  
		Size: 102.7 MB (102671454 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:80d93ce19113bbf944b699f12e59395e0eabeb00ccd1fd5dc7df46bb115eba2f`  
		Last Modified: Wed, 09 Jun 2021 15:59:58 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02a2af79aa85193c9d59672eaa3d7792de702370a62c15d646ca3d6e9805a4e3`  
		Last Modified: Wed, 09 Jun 2021 15:59:57 GMT  
		Size: 4.3 MB (4305480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9e0f71986494c926842ef864b29a5d7f3467a0415538fa78ad7850693a7b9d2`  
		Last Modified: Wed, 09 Jun 2021 15:59:56 GMT  
		Size: 1.8 KB (1752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74462c7c877f0c6efdd4131bf6b4ddf0ab34ceaa3aaeec8ca8d0b9f3fe614731`  
		Last Modified: Wed, 09 Jun 2021 15:59:56 GMT  
		Size: 1.2 KB (1192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cff02dcbfcaa11d91acbf9f579c2dc701b2c0a8057cb1b98b85a60bdeac38ba`  
		Last Modified: Wed, 09 Jun 2021 15:59:55 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56f9ea8a05c1d3919aab5e228736bf5b7f7dfd2493d7450e95724e6a41aab47b`  
		Last Modified: Wed, 09 Jun 2021 15:59:56 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.2.6-nanoserver-1809`

```console
$ docker pull nats@sha256:a0aacfbc002543c9a2dac717593b25e60fe52c18ec1033479d2a8fd25bab8391
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1999; amd64

### `nats:2.2.6-nanoserver-1809` - windows version 10.0.17763.1999; amd64

```console
$ docker pull nats@sha256:7305d7bf57da3e44ce9e5b368d294f4d9a6f86908ee0522b2e3af953bbfeaeb8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.0 MB (106983364 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:448497fc5d2a9aa4a4fe1404fa1f9cbd4a6cabcc2593a935a7e18d9ca49f7743`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sun, 06 Jun 2021 04:04:04 GMT
RUN Apply image 1809-amd64
# Wed, 09 Jun 2021 15:55:07 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 09 Jun 2021 15:55:09 GMT
RUN cmd /S /C #(nop) COPY file:a13acc0f2f64f12c4304c7730a47bebb73f06865d8dee680ec7a370c77d69e10 in C:\nats-server.exe 
# Wed, 09 Jun 2021 15:55:12 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 09 Jun 2021 15:55:14 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 09 Jun 2021 15:55:17 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 09 Jun 2021 15:55:19 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:e4800203e906d49fbdaf1eeab4de72f28796d5b9a1ea44f8d7461001cfa56614`  
		Size: 102.7 MB (102671454 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:80d93ce19113bbf944b699f12e59395e0eabeb00ccd1fd5dc7df46bb115eba2f`  
		Last Modified: Wed, 09 Jun 2021 15:59:58 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02a2af79aa85193c9d59672eaa3d7792de702370a62c15d646ca3d6e9805a4e3`  
		Last Modified: Wed, 09 Jun 2021 15:59:57 GMT  
		Size: 4.3 MB (4305480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9e0f71986494c926842ef864b29a5d7f3467a0415538fa78ad7850693a7b9d2`  
		Last Modified: Wed, 09 Jun 2021 15:59:56 GMT  
		Size: 1.8 KB (1752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74462c7c877f0c6efdd4131bf6b4ddf0ab34ceaa3aaeec8ca8d0b9f3fe614731`  
		Last Modified: Wed, 09 Jun 2021 15:59:56 GMT  
		Size: 1.2 KB (1192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cff02dcbfcaa11d91acbf9f579c2dc701b2c0a8057cb1b98b85a60bdeac38ba`  
		Last Modified: Wed, 09 Jun 2021 15:59:55 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56f9ea8a05c1d3919aab5e228736bf5b7f7dfd2493d7450e95724e6a41aab47b`  
		Last Modified: Wed, 09 Jun 2021 15:59:56 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.2.6-scratch`

```console
$ docker pull nats@sha256:8aceb3b18cc40ba1aa1d88ac3d22108e02e7a43cae6d2b66910dcfa80d437885
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.2.6-scratch` - linux; amd64

```console
$ docker pull nats@sha256:bad1b98cb238be899761405ed9a084eb4cee1e4982c4082414a49e1e47d83993
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4249359 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3903d09e582715d83e8da5706ee14109824854452c0ebf177eb55dfb789e311`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 25 May 2021 01:38:34 GMT
COPY file:6d5e77e6be5bafda9b9e03a4f397b21f9432694e3c3c3b5cd6e621b4c3ec3018 in /nats-server 
# Tue, 25 May 2021 01:38:34 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Tue, 25 May 2021 01:38:34 GMT
EXPOSE 4222 6222 8222
# Tue, 25 May 2021 01:38:34 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 25 May 2021 01:38:35 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:bf9e6d973acc267c8b0f05973d840142eec057566b36d0ae18177113f1fdadda`  
		Last Modified: Tue, 25 May 2021 01:39:26 GMT  
		Size: 4.2 MB (4248883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14a60a1c8cdedd7b360929beb64e25bbab3d679ba8134844479aaa6169d73595`  
		Last Modified: Tue, 25 May 2021 01:39:25 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2.6-scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:f98c4fa99482edcc01991046e5e9b2650e6181ec78b070d6601adef0afbbc3d9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3916550 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:573ae66ceb9d5149762ca1a8585b9f794bc0c0372ce18f73beefebb086f898c1`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 26 May 2021 18:22:59 GMT
COPY file:09c6eee4fb87ec105cf70b09816e278a49955f5e23576db600bfdb2fff0d6633 in /nats-server 
# Wed, 26 May 2021 18:23:00 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Wed, 26 May 2021 18:23:00 GMT
EXPOSE 4222 6222 8222
# Wed, 26 May 2021 18:23:00 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 26 May 2021 18:23:00 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:069976a4471c1abc4ad7dc33e5d7ed35c51e717ae622a055b7e925dd0bbe2ccb`  
		Last Modified: Wed, 26 May 2021 18:24:53 GMT  
		Size: 3.9 MB (3916076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4094f904541e138a0436baf31ea6b5ed4b91aee4871a54fce1650f2d63d2da2`  
		Last Modified: Wed, 26 May 2021 18:24:52 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2.6-scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:593e1b418f3e55050730f63b1d5da6e5f6f9c990c66e15bb9cd6659ea836279f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3914539 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4093ac9e36206435159f30858c34c7ed656e69e8dcbe1aaa6fbd40099701ade7`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 25 May 2021 22:23:02 GMT
COPY file:1ccce8553c778be1204380469e7248fd9ee472bdec35db0b7dd150122ae7c37d in /nats-server 
# Tue, 25 May 2021 22:23:02 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Tue, 25 May 2021 22:23:03 GMT
EXPOSE 4222 6222 8222
# Tue, 25 May 2021 22:23:03 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 25 May 2021 22:23:03 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a459b50ce258c1a3884cfc6f671ebabe9d05421a39962966809134623f3b9979`  
		Last Modified: Tue, 25 May 2021 22:24:59 GMT  
		Size: 3.9 MB (3914063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1808b616cb182b07285cb2e4b7d289755ccf8fa8575a8bc73a20ae46f8f253a`  
		Last Modified: Tue, 25 May 2021 22:24:58 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2.6-scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:8d8addd19d02a411d04db404a43383648e6a39e5a6686d5c2870bd5a0b80c546
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3889451 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b2ba9cf0b70339a1dd0b4bc93c1c83f00d829cd27d85adabe9b5ef7fdfefc69`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 26 May 2021 23:34:44 GMT
COPY file:312f19d8ade34bbf7590dddfdd3664f3152040117d8296ec0a54e9a9f7f42ae7 in /nats-server 
# Wed, 26 May 2021 23:34:45 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Wed, 26 May 2021 23:34:45 GMT
EXPOSE 4222 6222 8222
# Wed, 26 May 2021 23:34:45 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 26 May 2021 23:34:45 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:529a1438983ee1d8a2fdcab2846023465327ab9d8b15f0a7ed6ce61ff67fb8e8`  
		Last Modified: Wed, 26 May 2021 23:36:07 GMT  
		Size: 3.9 MB (3888976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:411d0165541f17c63026ae51d40e5a1f09909f0ab49fdadc7c2c7d904a4a3cb9`  
		Last Modified: Wed, 26 May 2021 23:36:06 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.2.6-windowsservercore`

```console
$ docker pull nats@sha256:334a5bbe37d543b1a8fcbd110923b8ac58c7095ba41eace53d0005932cd0899e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1999; amd64
	-	windows version 10.0.14393.4467; amd64

### `nats:2.2.6-windowsservercore` - windows version 10.0.17763.1999; amd64

```console
$ docker pull nats@sha256:b02d0fddc42e8f50f6dccf56bc6da2c299fa6ca12dac2a91142f5ea6f3c3b4d2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2646572446 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec0469d99bdcdeb93ecb4cd714c002dc5344cdd980081af67522abd90cb61f56`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sun, 06 Jun 2021 04:28:43 GMT
RUN Install update 1809-amd64
# Wed, 09 Jun 2021 13:15:43 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Jun 2021 15:52:54 GMT
ENV NATS_DOCKERIZED=1
# Wed, 09 Jun 2021 15:52:57 GMT
ENV NATS_SERVER=2.2.6
# Wed, 09 Jun 2021 15:52:59 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.2.6/nats-server-v2.2.6-windows-amd64.zip
# Wed, 09 Jun 2021 15:53:01 GMT
ENV GIT_DOWNLOAD_SHA256=c1712f41e4e811027701a036b6ff67b1f09fb298b0674098b26f875d37e709b2
# Wed, 09 Jun 2021 15:53:32 GMT
RUN Set-PSDebug -Trace 2
# Wed, 09 Jun 2021 15:54:42 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 09 Jun 2021 15:54:44 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 09 Jun 2021 15:54:47 GMT
EXPOSE 4222 6222 8222
# Wed, 09 Jun 2021 15:54:49 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 09 Jun 2021 15:54:51 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:639bb6bb2beb4cfdcacb9f0844344448fe26494665d5fe78a494419f86fbb18f`  
		Size: 923.3 MB (923252167 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ae7d2dc4b590128efeafd375d02122e65a2525623ac2be100c1a390caf8a4b49`  
		Last Modified: Wed, 09 Jun 2021 15:28:02 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:507a90d55d261855b42c7b5905599cdc274ca135ad962fffffe1fa6246c9bba7`  
		Last Modified: Wed, 09 Jun 2021 15:59:38 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58a0385e3ae1d1d8c00cf0ca66edc248c97d96c91e476559b29c6c52c46d3fe8`  
		Last Modified: Wed, 09 Jun 2021 15:59:37 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4e1c1a9e404ff727f004e12aef5245aa88eb270ce9e3f73be3e85f2df635f3f`  
		Last Modified: Wed, 09 Jun 2021 15:59:37 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a88b6cac0f81b699f58105a6102b27018ddf36099cc8cf069fa44ad96e2fa0b`  
		Last Modified: Wed, 09 Jun 2021 15:59:37 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dda44751dc046b037f6feced0dd9d70b6acfe04fc9099997ee322d8207cbe35c`  
		Last Modified: Wed, 09 Jun 2021 15:59:37 GMT  
		Size: 343.2 KB (343169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7df0a3f2eb0c7743406c39664c54d6dce8e83061bfa9d6fdc98ddb08231f479`  
		Last Modified: Wed, 09 Jun 2021 15:59:36 GMT  
		Size: 4.6 MB (4630934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ebd05a6c49ff1da6167088c0efd1b8272094cd2930c4d10b9c4423900006425`  
		Last Modified: Wed, 09 Jun 2021 15:59:34 GMT  
		Size: 2.0 KB (1976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:017fad8ec54342ed6819d801e462a0d9586120616b12bdac050efd3b2b3f10ed`  
		Last Modified: Wed, 09 Jun 2021 15:59:34 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4498408c64a82cbf1b4299f721bce414f88e9db0c6fdd6ec622145e162095d7a`  
		Last Modified: Wed, 09 Jun 2021 15:59:34 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11779cb16754ca0392b14675af366dbb6f10875912082da0e4faaad270fedc8b`  
		Last Modified: Wed, 09 Jun 2021 15:59:34 GMT  
		Size: 1.4 KB (1443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2.6-windowsservercore` - windows version 10.0.14393.4467; amd64

```console
$ docker pull nats@sha256:6e91913decc2a4bf6631d6c1ed5778e84342adc058acd2d9d9e9087b094da085
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6275203768 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe3a6d5b045a5442f1b6cafb40ecfb21592694d830e3dcf02806137974a5bc94`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Sun, 06 Jun 2021 15:37:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 09 Jun 2021 13:26:15 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Jun 2021 15:55:27 GMT
ENV NATS_DOCKERIZED=1
# Wed, 09 Jun 2021 15:55:30 GMT
ENV NATS_SERVER=2.2.6
# Wed, 09 Jun 2021 15:55:32 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.2.6/nats-server-v2.2.6-windows-amd64.zip
# Wed, 09 Jun 2021 15:55:34 GMT
ENV GIT_DOWNLOAD_SHA256=c1712f41e4e811027701a036b6ff67b1f09fb298b0674098b26f875d37e709b2
# Wed, 09 Jun 2021 15:56:47 GMT
RUN Set-PSDebug -Trace 2
# Wed, 09 Jun 2021 15:58:51 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 09 Jun 2021 15:58:53 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 09 Jun 2021 15:58:55 GMT
EXPOSE 4222 6222 8222
# Wed, 09 Jun 2021 15:58:58 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 09 Jun 2021 15:59:00 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2f52abeee6d6f4a925ad418b5e6200d4fca9bf92834ffc918b8bbaccd34251db`  
		Size: 2.2 GB (2195741359 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:fa4e6085e5538e957ef06561fe1e62dff898da7f4bb577e81da74323aecab2d7`  
		Last Modified: Wed, 09 Jun 2021 15:28:27 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7db57f94547be7109ad927e2f9d04a0501a2a5f0cb91ad8c4385eb32758f86b9`  
		Last Modified: Wed, 09 Jun 2021 16:00:21 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbc5017d27bf2f39955e298905f004a5999d929508e8b509e647d3432f8149ae`  
		Last Modified: Wed, 09 Jun 2021 16:00:18 GMT  
		Size: 1.4 KB (1379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad9d2c3aac632d05fde125d210746bf905438eeb4275fd89897ced5a1e237610`  
		Last Modified: Wed, 09 Jun 2021 16:00:18 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:defd74399fc019d7b0578a6724c0ac2c0eed04a8ae798590dcc568f83ffe3e67`  
		Last Modified: Wed, 09 Jun 2021 16:00:18 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76a97163f551fdbf75334ad37f6d16e6fe2d77ece5522d279046cd346d153b42`  
		Last Modified: Wed, 09 Jun 2021 16:00:18 GMT  
		Size: 341.5 KB (341515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecac4038087ee903af4019f7607dfc1e6850bfcd85c0b5e05c3132918b35dd90`  
		Last Modified: Wed, 09 Jun 2021 16:00:27 GMT  
		Size: 9.1 MB (9121804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f76428eff7b847a4fe7562a4795f520e7c7784527bb82c3074f2364b06f8cf69`  
		Last Modified: Wed, 09 Jun 2021 16:00:16 GMT  
		Size: 1.9 KB (1937 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4da349fd26102b808fd3307d65d0fe3c971879a8b7dad5b2e4ff228e1236614`  
		Last Modified: Wed, 09 Jun 2021 16:00:16 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8855b9c66052a7932dd8f755b14dbcc1581a824febee8a011b90f4213b2a3242`  
		Last Modified: Wed, 09 Jun 2021 16:00:16 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f1a11333ba3d20e4c4e4312c4d3840fdb58724a21cc62f43e8ded134e7b3682`  
		Last Modified: Wed, 09 Jun 2021 16:00:16 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.2.6-windowsservercore-1809`

```console
$ docker pull nats@sha256:e86cdc0cb1ce27e7d790872f30cdcbcefbe40bb9cc7a818e4dac93051c9f3e18
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1999; amd64

### `nats:2.2.6-windowsservercore-1809` - windows version 10.0.17763.1999; amd64

```console
$ docker pull nats@sha256:b02d0fddc42e8f50f6dccf56bc6da2c299fa6ca12dac2a91142f5ea6f3c3b4d2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2646572446 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec0469d99bdcdeb93ecb4cd714c002dc5344cdd980081af67522abd90cb61f56`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sun, 06 Jun 2021 04:28:43 GMT
RUN Install update 1809-amd64
# Wed, 09 Jun 2021 13:15:43 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Jun 2021 15:52:54 GMT
ENV NATS_DOCKERIZED=1
# Wed, 09 Jun 2021 15:52:57 GMT
ENV NATS_SERVER=2.2.6
# Wed, 09 Jun 2021 15:52:59 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.2.6/nats-server-v2.2.6-windows-amd64.zip
# Wed, 09 Jun 2021 15:53:01 GMT
ENV GIT_DOWNLOAD_SHA256=c1712f41e4e811027701a036b6ff67b1f09fb298b0674098b26f875d37e709b2
# Wed, 09 Jun 2021 15:53:32 GMT
RUN Set-PSDebug -Trace 2
# Wed, 09 Jun 2021 15:54:42 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 09 Jun 2021 15:54:44 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 09 Jun 2021 15:54:47 GMT
EXPOSE 4222 6222 8222
# Wed, 09 Jun 2021 15:54:49 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 09 Jun 2021 15:54:51 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:639bb6bb2beb4cfdcacb9f0844344448fe26494665d5fe78a494419f86fbb18f`  
		Size: 923.3 MB (923252167 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ae7d2dc4b590128efeafd375d02122e65a2525623ac2be100c1a390caf8a4b49`  
		Last Modified: Wed, 09 Jun 2021 15:28:02 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:507a90d55d261855b42c7b5905599cdc274ca135ad962fffffe1fa6246c9bba7`  
		Last Modified: Wed, 09 Jun 2021 15:59:38 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58a0385e3ae1d1d8c00cf0ca66edc248c97d96c91e476559b29c6c52c46d3fe8`  
		Last Modified: Wed, 09 Jun 2021 15:59:37 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4e1c1a9e404ff727f004e12aef5245aa88eb270ce9e3f73be3e85f2df635f3f`  
		Last Modified: Wed, 09 Jun 2021 15:59:37 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a88b6cac0f81b699f58105a6102b27018ddf36099cc8cf069fa44ad96e2fa0b`  
		Last Modified: Wed, 09 Jun 2021 15:59:37 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dda44751dc046b037f6feced0dd9d70b6acfe04fc9099997ee322d8207cbe35c`  
		Last Modified: Wed, 09 Jun 2021 15:59:37 GMT  
		Size: 343.2 KB (343169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7df0a3f2eb0c7743406c39664c54d6dce8e83061bfa9d6fdc98ddb08231f479`  
		Last Modified: Wed, 09 Jun 2021 15:59:36 GMT  
		Size: 4.6 MB (4630934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ebd05a6c49ff1da6167088c0efd1b8272094cd2930c4d10b9c4423900006425`  
		Last Modified: Wed, 09 Jun 2021 15:59:34 GMT  
		Size: 2.0 KB (1976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:017fad8ec54342ed6819d801e462a0d9586120616b12bdac050efd3b2b3f10ed`  
		Last Modified: Wed, 09 Jun 2021 15:59:34 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4498408c64a82cbf1b4299f721bce414f88e9db0c6fdd6ec622145e162095d7a`  
		Last Modified: Wed, 09 Jun 2021 15:59:34 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11779cb16754ca0392b14675af366dbb6f10875912082da0e4faaad270fedc8b`  
		Last Modified: Wed, 09 Jun 2021 15:59:34 GMT  
		Size: 1.4 KB (1443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.2.6-windowsservercore-ltsc2016`

```console
$ docker pull nats@sha256:aa8b74dbfe213c84911b8c47dac74da599ad57326e421c97b17e1b61bae86e51
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4467; amd64

### `nats:2.2.6-windowsservercore-ltsc2016` - windows version 10.0.14393.4467; amd64

```console
$ docker pull nats@sha256:6e91913decc2a4bf6631d6c1ed5778e84342adc058acd2d9d9e9087b094da085
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6275203768 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe3a6d5b045a5442f1b6cafb40ecfb21592694d830e3dcf02806137974a5bc94`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Sun, 06 Jun 2021 15:37:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 09 Jun 2021 13:26:15 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Jun 2021 15:55:27 GMT
ENV NATS_DOCKERIZED=1
# Wed, 09 Jun 2021 15:55:30 GMT
ENV NATS_SERVER=2.2.6
# Wed, 09 Jun 2021 15:55:32 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.2.6/nats-server-v2.2.6-windows-amd64.zip
# Wed, 09 Jun 2021 15:55:34 GMT
ENV GIT_DOWNLOAD_SHA256=c1712f41e4e811027701a036b6ff67b1f09fb298b0674098b26f875d37e709b2
# Wed, 09 Jun 2021 15:56:47 GMT
RUN Set-PSDebug -Trace 2
# Wed, 09 Jun 2021 15:58:51 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 09 Jun 2021 15:58:53 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 09 Jun 2021 15:58:55 GMT
EXPOSE 4222 6222 8222
# Wed, 09 Jun 2021 15:58:58 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 09 Jun 2021 15:59:00 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2f52abeee6d6f4a925ad418b5e6200d4fca9bf92834ffc918b8bbaccd34251db`  
		Size: 2.2 GB (2195741359 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:fa4e6085e5538e957ef06561fe1e62dff898da7f4bb577e81da74323aecab2d7`  
		Last Modified: Wed, 09 Jun 2021 15:28:27 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7db57f94547be7109ad927e2f9d04a0501a2a5f0cb91ad8c4385eb32758f86b9`  
		Last Modified: Wed, 09 Jun 2021 16:00:21 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbc5017d27bf2f39955e298905f004a5999d929508e8b509e647d3432f8149ae`  
		Last Modified: Wed, 09 Jun 2021 16:00:18 GMT  
		Size: 1.4 KB (1379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad9d2c3aac632d05fde125d210746bf905438eeb4275fd89897ced5a1e237610`  
		Last Modified: Wed, 09 Jun 2021 16:00:18 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:defd74399fc019d7b0578a6724c0ac2c0eed04a8ae798590dcc568f83ffe3e67`  
		Last Modified: Wed, 09 Jun 2021 16:00:18 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76a97163f551fdbf75334ad37f6d16e6fe2d77ece5522d279046cd346d153b42`  
		Last Modified: Wed, 09 Jun 2021 16:00:18 GMT  
		Size: 341.5 KB (341515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecac4038087ee903af4019f7607dfc1e6850bfcd85c0b5e05c3132918b35dd90`  
		Last Modified: Wed, 09 Jun 2021 16:00:27 GMT  
		Size: 9.1 MB (9121804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f76428eff7b847a4fe7562a4795f520e7c7784527bb82c3074f2364b06f8cf69`  
		Last Modified: Wed, 09 Jun 2021 16:00:16 GMT  
		Size: 1.9 KB (1937 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4da349fd26102b808fd3307d65d0fe3c971879a8b7dad5b2e4ff228e1236614`  
		Last Modified: Wed, 09 Jun 2021 16:00:16 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8855b9c66052a7932dd8f755b14dbcc1581a824febee8a011b90f4213b2a3242`  
		Last Modified: Wed, 09 Jun 2021 16:00:16 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f1a11333ba3d20e4c4e4312c4d3840fdb58724a21cc62f43e8ded134e7b3682`  
		Last Modified: Wed, 09 Jun 2021 16:00:16 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

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

## `nats:alpine3.13`

```console
$ docker pull nats@sha256:cc2bde1fe965db9ac2011073b071010691ebdb1904c7933922ad2a107a5a7a34
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:alpine3.13` - linux; amd64

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

### `nats:alpine3.13` - linux; arm variant v6

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

### `nats:alpine3.13` - linux; arm variant v7

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

### `nats:alpine3.13` - linux; arm64 variant v8

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

## `nats:latest`

```console
$ docker pull nats@sha256:ed66dfeef8f3c691f17ac8920b46054de09796a3b7a5bd3e96cb234a87915523
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.1999; amd64

### `nats:latest` - linux; amd64

```console
$ docker pull nats@sha256:bad1b98cb238be899761405ed9a084eb4cee1e4982c4082414a49e1e47d83993
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4249359 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3903d09e582715d83e8da5706ee14109824854452c0ebf177eb55dfb789e311`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 25 May 2021 01:38:34 GMT
COPY file:6d5e77e6be5bafda9b9e03a4f397b21f9432694e3c3c3b5cd6e621b4c3ec3018 in /nats-server 
# Tue, 25 May 2021 01:38:34 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Tue, 25 May 2021 01:38:34 GMT
EXPOSE 4222 6222 8222
# Tue, 25 May 2021 01:38:34 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 25 May 2021 01:38:35 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:bf9e6d973acc267c8b0f05973d840142eec057566b36d0ae18177113f1fdadda`  
		Last Modified: Tue, 25 May 2021 01:39:26 GMT  
		Size: 4.2 MB (4248883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14a60a1c8cdedd7b360929beb64e25bbab3d679ba8134844479aaa6169d73595`  
		Last Modified: Tue, 25 May 2021 01:39:25 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm variant v6

```console
$ docker pull nats@sha256:f98c4fa99482edcc01991046e5e9b2650e6181ec78b070d6601adef0afbbc3d9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3916550 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:573ae66ceb9d5149762ca1a8585b9f794bc0c0372ce18f73beefebb086f898c1`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 26 May 2021 18:22:59 GMT
COPY file:09c6eee4fb87ec105cf70b09816e278a49955f5e23576db600bfdb2fff0d6633 in /nats-server 
# Wed, 26 May 2021 18:23:00 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Wed, 26 May 2021 18:23:00 GMT
EXPOSE 4222 6222 8222
# Wed, 26 May 2021 18:23:00 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 26 May 2021 18:23:00 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:069976a4471c1abc4ad7dc33e5d7ed35c51e717ae622a055b7e925dd0bbe2ccb`  
		Last Modified: Wed, 26 May 2021 18:24:53 GMT  
		Size: 3.9 MB (3916076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4094f904541e138a0436baf31ea6b5ed4b91aee4871a54fce1650f2d63d2da2`  
		Last Modified: Wed, 26 May 2021 18:24:52 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm variant v7

```console
$ docker pull nats@sha256:593e1b418f3e55050730f63b1d5da6e5f6f9c990c66e15bb9cd6659ea836279f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3914539 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4093ac9e36206435159f30858c34c7ed656e69e8dcbe1aaa6fbd40099701ade7`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 25 May 2021 22:23:02 GMT
COPY file:1ccce8553c778be1204380469e7248fd9ee472bdec35db0b7dd150122ae7c37d in /nats-server 
# Tue, 25 May 2021 22:23:02 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Tue, 25 May 2021 22:23:03 GMT
EXPOSE 4222 6222 8222
# Tue, 25 May 2021 22:23:03 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 25 May 2021 22:23:03 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a459b50ce258c1a3884cfc6f671ebabe9d05421a39962966809134623f3b9979`  
		Last Modified: Tue, 25 May 2021 22:24:59 GMT  
		Size: 3.9 MB (3914063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1808b616cb182b07285cb2e4b7d289755ccf8fa8575a8bc73a20ae46f8f253a`  
		Last Modified: Tue, 25 May 2021 22:24:58 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:8d8addd19d02a411d04db404a43383648e6a39e5a6686d5c2870bd5a0b80c546
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3889451 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b2ba9cf0b70339a1dd0b4bc93c1c83f00d829cd27d85adabe9b5ef7fdfefc69`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 26 May 2021 23:34:44 GMT
COPY file:312f19d8ade34bbf7590dddfdd3664f3152040117d8296ec0a54e9a9f7f42ae7 in /nats-server 
# Wed, 26 May 2021 23:34:45 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Wed, 26 May 2021 23:34:45 GMT
EXPOSE 4222 6222 8222
# Wed, 26 May 2021 23:34:45 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 26 May 2021 23:34:45 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:529a1438983ee1d8a2fdcab2846023465327ab9d8b15f0a7ed6ce61ff67fb8e8`  
		Last Modified: Wed, 26 May 2021 23:36:07 GMT  
		Size: 3.9 MB (3888976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:411d0165541f17c63026ae51d40e5a1f09909f0ab49fdadc7c2c7d904a4a3cb9`  
		Last Modified: Wed, 26 May 2021 23:36:06 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - windows version 10.0.17763.1999; amd64

```console
$ docker pull nats@sha256:7305d7bf57da3e44ce9e5b368d294f4d9a6f86908ee0522b2e3af953bbfeaeb8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.0 MB (106983364 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:448497fc5d2a9aa4a4fe1404fa1f9cbd4a6cabcc2593a935a7e18d9ca49f7743`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sun, 06 Jun 2021 04:04:04 GMT
RUN Apply image 1809-amd64
# Wed, 09 Jun 2021 15:55:07 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 09 Jun 2021 15:55:09 GMT
RUN cmd /S /C #(nop) COPY file:a13acc0f2f64f12c4304c7730a47bebb73f06865d8dee680ec7a370c77d69e10 in C:\nats-server.exe 
# Wed, 09 Jun 2021 15:55:12 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 09 Jun 2021 15:55:14 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 09 Jun 2021 15:55:17 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 09 Jun 2021 15:55:19 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:e4800203e906d49fbdaf1eeab4de72f28796d5b9a1ea44f8d7461001cfa56614`  
		Size: 102.7 MB (102671454 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:80d93ce19113bbf944b699f12e59395e0eabeb00ccd1fd5dc7df46bb115eba2f`  
		Last Modified: Wed, 09 Jun 2021 15:59:58 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02a2af79aa85193c9d59672eaa3d7792de702370a62c15d646ca3d6e9805a4e3`  
		Last Modified: Wed, 09 Jun 2021 15:59:57 GMT  
		Size: 4.3 MB (4305480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9e0f71986494c926842ef864b29a5d7f3467a0415538fa78ad7850693a7b9d2`  
		Last Modified: Wed, 09 Jun 2021 15:59:56 GMT  
		Size: 1.8 KB (1752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74462c7c877f0c6efdd4131bf6b4ddf0ab34ceaa3aaeec8ca8d0b9f3fe614731`  
		Last Modified: Wed, 09 Jun 2021 15:59:56 GMT  
		Size: 1.2 KB (1192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cff02dcbfcaa11d91acbf9f579c2dc701b2c0a8057cb1b98b85a60bdeac38ba`  
		Last Modified: Wed, 09 Jun 2021 15:59:55 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56f9ea8a05c1d3919aab5e228736bf5b7f7dfd2493d7450e95724e6a41aab47b`  
		Last Modified: Wed, 09 Jun 2021 15:59:56 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:linux`

```console
$ docker pull nats@sha256:8aceb3b18cc40ba1aa1d88ac3d22108e02e7a43cae6d2b66910dcfa80d437885
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:linux` - linux; amd64

```console
$ docker pull nats@sha256:bad1b98cb238be899761405ed9a084eb4cee1e4982c4082414a49e1e47d83993
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4249359 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3903d09e582715d83e8da5706ee14109824854452c0ebf177eb55dfb789e311`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 25 May 2021 01:38:34 GMT
COPY file:6d5e77e6be5bafda9b9e03a4f397b21f9432694e3c3c3b5cd6e621b4c3ec3018 in /nats-server 
# Tue, 25 May 2021 01:38:34 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Tue, 25 May 2021 01:38:34 GMT
EXPOSE 4222 6222 8222
# Tue, 25 May 2021 01:38:34 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 25 May 2021 01:38:35 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:bf9e6d973acc267c8b0f05973d840142eec057566b36d0ae18177113f1fdadda`  
		Last Modified: Tue, 25 May 2021 01:39:26 GMT  
		Size: 4.2 MB (4248883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14a60a1c8cdedd7b360929beb64e25bbab3d679ba8134844479aaa6169d73595`  
		Last Modified: Tue, 25 May 2021 01:39:25 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:f98c4fa99482edcc01991046e5e9b2650e6181ec78b070d6601adef0afbbc3d9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3916550 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:573ae66ceb9d5149762ca1a8585b9f794bc0c0372ce18f73beefebb086f898c1`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 26 May 2021 18:22:59 GMT
COPY file:09c6eee4fb87ec105cf70b09816e278a49955f5e23576db600bfdb2fff0d6633 in /nats-server 
# Wed, 26 May 2021 18:23:00 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Wed, 26 May 2021 18:23:00 GMT
EXPOSE 4222 6222 8222
# Wed, 26 May 2021 18:23:00 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 26 May 2021 18:23:00 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:069976a4471c1abc4ad7dc33e5d7ed35c51e717ae622a055b7e925dd0bbe2ccb`  
		Last Modified: Wed, 26 May 2021 18:24:53 GMT  
		Size: 3.9 MB (3916076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4094f904541e138a0436baf31ea6b5ed4b91aee4871a54fce1650f2d63d2da2`  
		Last Modified: Wed, 26 May 2021 18:24:52 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:593e1b418f3e55050730f63b1d5da6e5f6f9c990c66e15bb9cd6659ea836279f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3914539 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4093ac9e36206435159f30858c34c7ed656e69e8dcbe1aaa6fbd40099701ade7`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 25 May 2021 22:23:02 GMT
COPY file:1ccce8553c778be1204380469e7248fd9ee472bdec35db0b7dd150122ae7c37d in /nats-server 
# Tue, 25 May 2021 22:23:02 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Tue, 25 May 2021 22:23:03 GMT
EXPOSE 4222 6222 8222
# Tue, 25 May 2021 22:23:03 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 25 May 2021 22:23:03 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a459b50ce258c1a3884cfc6f671ebabe9d05421a39962966809134623f3b9979`  
		Last Modified: Tue, 25 May 2021 22:24:59 GMT  
		Size: 3.9 MB (3914063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1808b616cb182b07285cb2e4b7d289755ccf8fa8575a8bc73a20ae46f8f253a`  
		Last Modified: Tue, 25 May 2021 22:24:58 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:8d8addd19d02a411d04db404a43383648e6a39e5a6686d5c2870bd5a0b80c546
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3889451 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b2ba9cf0b70339a1dd0b4bc93c1c83f00d829cd27d85adabe9b5ef7fdfefc69`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 26 May 2021 23:34:44 GMT
COPY file:312f19d8ade34bbf7590dddfdd3664f3152040117d8296ec0a54e9a9f7f42ae7 in /nats-server 
# Wed, 26 May 2021 23:34:45 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Wed, 26 May 2021 23:34:45 GMT
EXPOSE 4222 6222 8222
# Wed, 26 May 2021 23:34:45 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 26 May 2021 23:34:45 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:529a1438983ee1d8a2fdcab2846023465327ab9d8b15f0a7ed6ce61ff67fb8e8`  
		Last Modified: Wed, 26 May 2021 23:36:07 GMT  
		Size: 3.9 MB (3888976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:411d0165541f17c63026ae51d40e5a1f09909f0ab49fdadc7c2c7d904a4a3cb9`  
		Last Modified: Wed, 26 May 2021 23:36:06 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:nanoserver`

```console
$ docker pull nats@sha256:a0aacfbc002543c9a2dac717593b25e60fe52c18ec1033479d2a8fd25bab8391
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1999; amd64

### `nats:nanoserver` - windows version 10.0.17763.1999; amd64

```console
$ docker pull nats@sha256:7305d7bf57da3e44ce9e5b368d294f4d9a6f86908ee0522b2e3af953bbfeaeb8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.0 MB (106983364 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:448497fc5d2a9aa4a4fe1404fa1f9cbd4a6cabcc2593a935a7e18d9ca49f7743`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sun, 06 Jun 2021 04:04:04 GMT
RUN Apply image 1809-amd64
# Wed, 09 Jun 2021 15:55:07 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 09 Jun 2021 15:55:09 GMT
RUN cmd /S /C #(nop) COPY file:a13acc0f2f64f12c4304c7730a47bebb73f06865d8dee680ec7a370c77d69e10 in C:\nats-server.exe 
# Wed, 09 Jun 2021 15:55:12 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 09 Jun 2021 15:55:14 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 09 Jun 2021 15:55:17 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 09 Jun 2021 15:55:19 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:e4800203e906d49fbdaf1eeab4de72f28796d5b9a1ea44f8d7461001cfa56614`  
		Size: 102.7 MB (102671454 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:80d93ce19113bbf944b699f12e59395e0eabeb00ccd1fd5dc7df46bb115eba2f`  
		Last Modified: Wed, 09 Jun 2021 15:59:58 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02a2af79aa85193c9d59672eaa3d7792de702370a62c15d646ca3d6e9805a4e3`  
		Last Modified: Wed, 09 Jun 2021 15:59:57 GMT  
		Size: 4.3 MB (4305480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9e0f71986494c926842ef864b29a5d7f3467a0415538fa78ad7850693a7b9d2`  
		Last Modified: Wed, 09 Jun 2021 15:59:56 GMT  
		Size: 1.8 KB (1752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74462c7c877f0c6efdd4131bf6b4ddf0ab34ceaa3aaeec8ca8d0b9f3fe614731`  
		Last Modified: Wed, 09 Jun 2021 15:59:56 GMT  
		Size: 1.2 KB (1192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cff02dcbfcaa11d91acbf9f579c2dc701b2c0a8057cb1b98b85a60bdeac38ba`  
		Last Modified: Wed, 09 Jun 2021 15:59:55 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56f9ea8a05c1d3919aab5e228736bf5b7f7dfd2493d7450e95724e6a41aab47b`  
		Last Modified: Wed, 09 Jun 2021 15:59:56 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:nanoserver-1809`

```console
$ docker pull nats@sha256:a0aacfbc002543c9a2dac717593b25e60fe52c18ec1033479d2a8fd25bab8391
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1999; amd64

### `nats:nanoserver-1809` - windows version 10.0.17763.1999; amd64

```console
$ docker pull nats@sha256:7305d7bf57da3e44ce9e5b368d294f4d9a6f86908ee0522b2e3af953bbfeaeb8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.0 MB (106983364 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:448497fc5d2a9aa4a4fe1404fa1f9cbd4a6cabcc2593a935a7e18d9ca49f7743`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sun, 06 Jun 2021 04:04:04 GMT
RUN Apply image 1809-amd64
# Wed, 09 Jun 2021 15:55:07 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 09 Jun 2021 15:55:09 GMT
RUN cmd /S /C #(nop) COPY file:a13acc0f2f64f12c4304c7730a47bebb73f06865d8dee680ec7a370c77d69e10 in C:\nats-server.exe 
# Wed, 09 Jun 2021 15:55:12 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 09 Jun 2021 15:55:14 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 09 Jun 2021 15:55:17 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 09 Jun 2021 15:55:19 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:e4800203e906d49fbdaf1eeab4de72f28796d5b9a1ea44f8d7461001cfa56614`  
		Size: 102.7 MB (102671454 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:80d93ce19113bbf944b699f12e59395e0eabeb00ccd1fd5dc7df46bb115eba2f`  
		Last Modified: Wed, 09 Jun 2021 15:59:58 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02a2af79aa85193c9d59672eaa3d7792de702370a62c15d646ca3d6e9805a4e3`  
		Last Modified: Wed, 09 Jun 2021 15:59:57 GMT  
		Size: 4.3 MB (4305480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9e0f71986494c926842ef864b29a5d7f3467a0415538fa78ad7850693a7b9d2`  
		Last Modified: Wed, 09 Jun 2021 15:59:56 GMT  
		Size: 1.8 KB (1752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74462c7c877f0c6efdd4131bf6b4ddf0ab34ceaa3aaeec8ca8d0b9f3fe614731`  
		Last Modified: Wed, 09 Jun 2021 15:59:56 GMT  
		Size: 1.2 KB (1192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cff02dcbfcaa11d91acbf9f579c2dc701b2c0a8057cb1b98b85a60bdeac38ba`  
		Last Modified: Wed, 09 Jun 2021 15:59:55 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56f9ea8a05c1d3919aab5e228736bf5b7f7dfd2493d7450e95724e6a41aab47b`  
		Last Modified: Wed, 09 Jun 2021 15:59:56 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:scratch`

```console
$ docker pull nats@sha256:8aceb3b18cc40ba1aa1d88ac3d22108e02e7a43cae6d2b66910dcfa80d437885
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:scratch` - linux; amd64

```console
$ docker pull nats@sha256:bad1b98cb238be899761405ed9a084eb4cee1e4982c4082414a49e1e47d83993
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4249359 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3903d09e582715d83e8da5706ee14109824854452c0ebf177eb55dfb789e311`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 25 May 2021 01:38:34 GMT
COPY file:6d5e77e6be5bafda9b9e03a4f397b21f9432694e3c3c3b5cd6e621b4c3ec3018 in /nats-server 
# Tue, 25 May 2021 01:38:34 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Tue, 25 May 2021 01:38:34 GMT
EXPOSE 4222 6222 8222
# Tue, 25 May 2021 01:38:34 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 25 May 2021 01:38:35 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:bf9e6d973acc267c8b0f05973d840142eec057566b36d0ae18177113f1fdadda`  
		Last Modified: Tue, 25 May 2021 01:39:26 GMT  
		Size: 4.2 MB (4248883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14a60a1c8cdedd7b360929beb64e25bbab3d679ba8134844479aaa6169d73595`  
		Last Modified: Tue, 25 May 2021 01:39:25 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:f98c4fa99482edcc01991046e5e9b2650e6181ec78b070d6601adef0afbbc3d9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3916550 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:573ae66ceb9d5149762ca1a8585b9f794bc0c0372ce18f73beefebb086f898c1`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 26 May 2021 18:22:59 GMT
COPY file:09c6eee4fb87ec105cf70b09816e278a49955f5e23576db600bfdb2fff0d6633 in /nats-server 
# Wed, 26 May 2021 18:23:00 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Wed, 26 May 2021 18:23:00 GMT
EXPOSE 4222 6222 8222
# Wed, 26 May 2021 18:23:00 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 26 May 2021 18:23:00 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:069976a4471c1abc4ad7dc33e5d7ed35c51e717ae622a055b7e925dd0bbe2ccb`  
		Last Modified: Wed, 26 May 2021 18:24:53 GMT  
		Size: 3.9 MB (3916076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4094f904541e138a0436baf31ea6b5ed4b91aee4871a54fce1650f2d63d2da2`  
		Last Modified: Wed, 26 May 2021 18:24:52 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:593e1b418f3e55050730f63b1d5da6e5f6f9c990c66e15bb9cd6659ea836279f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3914539 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4093ac9e36206435159f30858c34c7ed656e69e8dcbe1aaa6fbd40099701ade7`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 25 May 2021 22:23:02 GMT
COPY file:1ccce8553c778be1204380469e7248fd9ee472bdec35db0b7dd150122ae7c37d in /nats-server 
# Tue, 25 May 2021 22:23:02 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Tue, 25 May 2021 22:23:03 GMT
EXPOSE 4222 6222 8222
# Tue, 25 May 2021 22:23:03 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 25 May 2021 22:23:03 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a459b50ce258c1a3884cfc6f671ebabe9d05421a39962966809134623f3b9979`  
		Last Modified: Tue, 25 May 2021 22:24:59 GMT  
		Size: 3.9 MB (3914063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1808b616cb182b07285cb2e4b7d289755ccf8fa8575a8bc73a20ae46f8f253a`  
		Last Modified: Tue, 25 May 2021 22:24:58 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:8d8addd19d02a411d04db404a43383648e6a39e5a6686d5c2870bd5a0b80c546
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3889451 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b2ba9cf0b70339a1dd0b4bc93c1c83f00d829cd27d85adabe9b5ef7fdfefc69`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 26 May 2021 23:34:44 GMT
COPY file:312f19d8ade34bbf7590dddfdd3664f3152040117d8296ec0a54e9a9f7f42ae7 in /nats-server 
# Wed, 26 May 2021 23:34:45 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Wed, 26 May 2021 23:34:45 GMT
EXPOSE 4222 6222 8222
# Wed, 26 May 2021 23:34:45 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 26 May 2021 23:34:45 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:529a1438983ee1d8a2fdcab2846023465327ab9d8b15f0a7ed6ce61ff67fb8e8`  
		Last Modified: Wed, 26 May 2021 23:36:07 GMT  
		Size: 3.9 MB (3888976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:411d0165541f17c63026ae51d40e5a1f09909f0ab49fdadc7c2c7d904a4a3cb9`  
		Last Modified: Wed, 26 May 2021 23:36:06 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:windowsservercore`

```console
$ docker pull nats@sha256:334a5bbe37d543b1a8fcbd110923b8ac58c7095ba41eace53d0005932cd0899e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1999; amd64
	-	windows version 10.0.14393.4467; amd64

### `nats:windowsservercore` - windows version 10.0.17763.1999; amd64

```console
$ docker pull nats@sha256:b02d0fddc42e8f50f6dccf56bc6da2c299fa6ca12dac2a91142f5ea6f3c3b4d2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2646572446 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec0469d99bdcdeb93ecb4cd714c002dc5344cdd980081af67522abd90cb61f56`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sun, 06 Jun 2021 04:28:43 GMT
RUN Install update 1809-amd64
# Wed, 09 Jun 2021 13:15:43 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Jun 2021 15:52:54 GMT
ENV NATS_DOCKERIZED=1
# Wed, 09 Jun 2021 15:52:57 GMT
ENV NATS_SERVER=2.2.6
# Wed, 09 Jun 2021 15:52:59 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.2.6/nats-server-v2.2.6-windows-amd64.zip
# Wed, 09 Jun 2021 15:53:01 GMT
ENV GIT_DOWNLOAD_SHA256=c1712f41e4e811027701a036b6ff67b1f09fb298b0674098b26f875d37e709b2
# Wed, 09 Jun 2021 15:53:32 GMT
RUN Set-PSDebug -Trace 2
# Wed, 09 Jun 2021 15:54:42 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 09 Jun 2021 15:54:44 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 09 Jun 2021 15:54:47 GMT
EXPOSE 4222 6222 8222
# Wed, 09 Jun 2021 15:54:49 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 09 Jun 2021 15:54:51 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:639bb6bb2beb4cfdcacb9f0844344448fe26494665d5fe78a494419f86fbb18f`  
		Size: 923.3 MB (923252167 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ae7d2dc4b590128efeafd375d02122e65a2525623ac2be100c1a390caf8a4b49`  
		Last Modified: Wed, 09 Jun 2021 15:28:02 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:507a90d55d261855b42c7b5905599cdc274ca135ad962fffffe1fa6246c9bba7`  
		Last Modified: Wed, 09 Jun 2021 15:59:38 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58a0385e3ae1d1d8c00cf0ca66edc248c97d96c91e476559b29c6c52c46d3fe8`  
		Last Modified: Wed, 09 Jun 2021 15:59:37 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4e1c1a9e404ff727f004e12aef5245aa88eb270ce9e3f73be3e85f2df635f3f`  
		Last Modified: Wed, 09 Jun 2021 15:59:37 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a88b6cac0f81b699f58105a6102b27018ddf36099cc8cf069fa44ad96e2fa0b`  
		Last Modified: Wed, 09 Jun 2021 15:59:37 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dda44751dc046b037f6feced0dd9d70b6acfe04fc9099997ee322d8207cbe35c`  
		Last Modified: Wed, 09 Jun 2021 15:59:37 GMT  
		Size: 343.2 KB (343169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7df0a3f2eb0c7743406c39664c54d6dce8e83061bfa9d6fdc98ddb08231f479`  
		Last Modified: Wed, 09 Jun 2021 15:59:36 GMT  
		Size: 4.6 MB (4630934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ebd05a6c49ff1da6167088c0efd1b8272094cd2930c4d10b9c4423900006425`  
		Last Modified: Wed, 09 Jun 2021 15:59:34 GMT  
		Size: 2.0 KB (1976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:017fad8ec54342ed6819d801e462a0d9586120616b12bdac050efd3b2b3f10ed`  
		Last Modified: Wed, 09 Jun 2021 15:59:34 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4498408c64a82cbf1b4299f721bce414f88e9db0c6fdd6ec622145e162095d7a`  
		Last Modified: Wed, 09 Jun 2021 15:59:34 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11779cb16754ca0392b14675af366dbb6f10875912082da0e4faaad270fedc8b`  
		Last Modified: Wed, 09 Jun 2021 15:59:34 GMT  
		Size: 1.4 KB (1443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:windowsservercore` - windows version 10.0.14393.4467; amd64

```console
$ docker pull nats@sha256:6e91913decc2a4bf6631d6c1ed5778e84342adc058acd2d9d9e9087b094da085
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6275203768 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe3a6d5b045a5442f1b6cafb40ecfb21592694d830e3dcf02806137974a5bc94`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Sun, 06 Jun 2021 15:37:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 09 Jun 2021 13:26:15 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Jun 2021 15:55:27 GMT
ENV NATS_DOCKERIZED=1
# Wed, 09 Jun 2021 15:55:30 GMT
ENV NATS_SERVER=2.2.6
# Wed, 09 Jun 2021 15:55:32 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.2.6/nats-server-v2.2.6-windows-amd64.zip
# Wed, 09 Jun 2021 15:55:34 GMT
ENV GIT_DOWNLOAD_SHA256=c1712f41e4e811027701a036b6ff67b1f09fb298b0674098b26f875d37e709b2
# Wed, 09 Jun 2021 15:56:47 GMT
RUN Set-PSDebug -Trace 2
# Wed, 09 Jun 2021 15:58:51 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 09 Jun 2021 15:58:53 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 09 Jun 2021 15:58:55 GMT
EXPOSE 4222 6222 8222
# Wed, 09 Jun 2021 15:58:58 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 09 Jun 2021 15:59:00 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2f52abeee6d6f4a925ad418b5e6200d4fca9bf92834ffc918b8bbaccd34251db`  
		Size: 2.2 GB (2195741359 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:fa4e6085e5538e957ef06561fe1e62dff898da7f4bb577e81da74323aecab2d7`  
		Last Modified: Wed, 09 Jun 2021 15:28:27 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7db57f94547be7109ad927e2f9d04a0501a2a5f0cb91ad8c4385eb32758f86b9`  
		Last Modified: Wed, 09 Jun 2021 16:00:21 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbc5017d27bf2f39955e298905f004a5999d929508e8b509e647d3432f8149ae`  
		Last Modified: Wed, 09 Jun 2021 16:00:18 GMT  
		Size: 1.4 KB (1379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad9d2c3aac632d05fde125d210746bf905438eeb4275fd89897ced5a1e237610`  
		Last Modified: Wed, 09 Jun 2021 16:00:18 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:defd74399fc019d7b0578a6724c0ac2c0eed04a8ae798590dcc568f83ffe3e67`  
		Last Modified: Wed, 09 Jun 2021 16:00:18 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76a97163f551fdbf75334ad37f6d16e6fe2d77ece5522d279046cd346d153b42`  
		Last Modified: Wed, 09 Jun 2021 16:00:18 GMT  
		Size: 341.5 KB (341515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecac4038087ee903af4019f7607dfc1e6850bfcd85c0b5e05c3132918b35dd90`  
		Last Modified: Wed, 09 Jun 2021 16:00:27 GMT  
		Size: 9.1 MB (9121804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f76428eff7b847a4fe7562a4795f520e7c7784527bb82c3074f2364b06f8cf69`  
		Last Modified: Wed, 09 Jun 2021 16:00:16 GMT  
		Size: 1.9 KB (1937 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4da349fd26102b808fd3307d65d0fe3c971879a8b7dad5b2e4ff228e1236614`  
		Last Modified: Wed, 09 Jun 2021 16:00:16 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8855b9c66052a7932dd8f755b14dbcc1581a824febee8a011b90f4213b2a3242`  
		Last Modified: Wed, 09 Jun 2021 16:00:16 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f1a11333ba3d20e4c4e4312c4d3840fdb58724a21cc62f43e8ded134e7b3682`  
		Last Modified: Wed, 09 Jun 2021 16:00:16 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:windowsservercore-1809`

```console
$ docker pull nats@sha256:e86cdc0cb1ce27e7d790872f30cdcbcefbe40bb9cc7a818e4dac93051c9f3e18
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1999; amd64

### `nats:windowsservercore-1809` - windows version 10.0.17763.1999; amd64

```console
$ docker pull nats@sha256:b02d0fddc42e8f50f6dccf56bc6da2c299fa6ca12dac2a91142f5ea6f3c3b4d2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2646572446 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec0469d99bdcdeb93ecb4cd714c002dc5344cdd980081af67522abd90cb61f56`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sun, 06 Jun 2021 04:28:43 GMT
RUN Install update 1809-amd64
# Wed, 09 Jun 2021 13:15:43 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Jun 2021 15:52:54 GMT
ENV NATS_DOCKERIZED=1
# Wed, 09 Jun 2021 15:52:57 GMT
ENV NATS_SERVER=2.2.6
# Wed, 09 Jun 2021 15:52:59 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.2.6/nats-server-v2.2.6-windows-amd64.zip
# Wed, 09 Jun 2021 15:53:01 GMT
ENV GIT_DOWNLOAD_SHA256=c1712f41e4e811027701a036b6ff67b1f09fb298b0674098b26f875d37e709b2
# Wed, 09 Jun 2021 15:53:32 GMT
RUN Set-PSDebug -Trace 2
# Wed, 09 Jun 2021 15:54:42 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 09 Jun 2021 15:54:44 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 09 Jun 2021 15:54:47 GMT
EXPOSE 4222 6222 8222
# Wed, 09 Jun 2021 15:54:49 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 09 Jun 2021 15:54:51 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:639bb6bb2beb4cfdcacb9f0844344448fe26494665d5fe78a494419f86fbb18f`  
		Size: 923.3 MB (923252167 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ae7d2dc4b590128efeafd375d02122e65a2525623ac2be100c1a390caf8a4b49`  
		Last Modified: Wed, 09 Jun 2021 15:28:02 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:507a90d55d261855b42c7b5905599cdc274ca135ad962fffffe1fa6246c9bba7`  
		Last Modified: Wed, 09 Jun 2021 15:59:38 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58a0385e3ae1d1d8c00cf0ca66edc248c97d96c91e476559b29c6c52c46d3fe8`  
		Last Modified: Wed, 09 Jun 2021 15:59:37 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4e1c1a9e404ff727f004e12aef5245aa88eb270ce9e3f73be3e85f2df635f3f`  
		Last Modified: Wed, 09 Jun 2021 15:59:37 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a88b6cac0f81b699f58105a6102b27018ddf36099cc8cf069fa44ad96e2fa0b`  
		Last Modified: Wed, 09 Jun 2021 15:59:37 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dda44751dc046b037f6feced0dd9d70b6acfe04fc9099997ee322d8207cbe35c`  
		Last Modified: Wed, 09 Jun 2021 15:59:37 GMT  
		Size: 343.2 KB (343169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7df0a3f2eb0c7743406c39664c54d6dce8e83061bfa9d6fdc98ddb08231f479`  
		Last Modified: Wed, 09 Jun 2021 15:59:36 GMT  
		Size: 4.6 MB (4630934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ebd05a6c49ff1da6167088c0efd1b8272094cd2930c4d10b9c4423900006425`  
		Last Modified: Wed, 09 Jun 2021 15:59:34 GMT  
		Size: 2.0 KB (1976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:017fad8ec54342ed6819d801e462a0d9586120616b12bdac050efd3b2b3f10ed`  
		Last Modified: Wed, 09 Jun 2021 15:59:34 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4498408c64a82cbf1b4299f721bce414f88e9db0c6fdd6ec622145e162095d7a`  
		Last Modified: Wed, 09 Jun 2021 15:59:34 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11779cb16754ca0392b14675af366dbb6f10875912082da0e4faaad270fedc8b`  
		Last Modified: Wed, 09 Jun 2021 15:59:34 GMT  
		Size: 1.4 KB (1443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:windowsservercore-ltsc2016`

```console
$ docker pull nats@sha256:aa8b74dbfe213c84911b8c47dac74da599ad57326e421c97b17e1b61bae86e51
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4467; amd64

### `nats:windowsservercore-ltsc2016` - windows version 10.0.14393.4467; amd64

```console
$ docker pull nats@sha256:6e91913decc2a4bf6631d6c1ed5778e84342adc058acd2d9d9e9087b094da085
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6275203768 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe3a6d5b045a5442f1b6cafb40ecfb21592694d830e3dcf02806137974a5bc94`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Sun, 06 Jun 2021 15:37:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 09 Jun 2021 13:26:15 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Jun 2021 15:55:27 GMT
ENV NATS_DOCKERIZED=1
# Wed, 09 Jun 2021 15:55:30 GMT
ENV NATS_SERVER=2.2.6
# Wed, 09 Jun 2021 15:55:32 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.2.6/nats-server-v2.2.6-windows-amd64.zip
# Wed, 09 Jun 2021 15:55:34 GMT
ENV GIT_DOWNLOAD_SHA256=c1712f41e4e811027701a036b6ff67b1f09fb298b0674098b26f875d37e709b2
# Wed, 09 Jun 2021 15:56:47 GMT
RUN Set-PSDebug -Trace 2
# Wed, 09 Jun 2021 15:58:51 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 09 Jun 2021 15:58:53 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 09 Jun 2021 15:58:55 GMT
EXPOSE 4222 6222 8222
# Wed, 09 Jun 2021 15:58:58 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 09 Jun 2021 15:59:00 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2f52abeee6d6f4a925ad418b5e6200d4fca9bf92834ffc918b8bbaccd34251db`  
		Size: 2.2 GB (2195741359 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:fa4e6085e5538e957ef06561fe1e62dff898da7f4bb577e81da74323aecab2d7`  
		Last Modified: Wed, 09 Jun 2021 15:28:27 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7db57f94547be7109ad927e2f9d04a0501a2a5f0cb91ad8c4385eb32758f86b9`  
		Last Modified: Wed, 09 Jun 2021 16:00:21 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbc5017d27bf2f39955e298905f004a5999d929508e8b509e647d3432f8149ae`  
		Last Modified: Wed, 09 Jun 2021 16:00:18 GMT  
		Size: 1.4 KB (1379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad9d2c3aac632d05fde125d210746bf905438eeb4275fd89897ced5a1e237610`  
		Last Modified: Wed, 09 Jun 2021 16:00:18 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:defd74399fc019d7b0578a6724c0ac2c0eed04a8ae798590dcc568f83ffe3e67`  
		Last Modified: Wed, 09 Jun 2021 16:00:18 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76a97163f551fdbf75334ad37f6d16e6fe2d77ece5522d279046cd346d153b42`  
		Last Modified: Wed, 09 Jun 2021 16:00:18 GMT  
		Size: 341.5 KB (341515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecac4038087ee903af4019f7607dfc1e6850bfcd85c0b5e05c3132918b35dd90`  
		Last Modified: Wed, 09 Jun 2021 16:00:27 GMT  
		Size: 9.1 MB (9121804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f76428eff7b847a4fe7562a4795f520e7c7784527bb82c3074f2364b06f8cf69`  
		Last Modified: Wed, 09 Jun 2021 16:00:16 GMT  
		Size: 1.9 KB (1937 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4da349fd26102b808fd3307d65d0fe3c971879a8b7dad5b2e4ff228e1236614`  
		Last Modified: Wed, 09 Jun 2021 16:00:16 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8855b9c66052a7932dd8f755b14dbcc1581a824febee8a011b90f4213b2a3242`  
		Last Modified: Wed, 09 Jun 2021 16:00:16 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f1a11333ba3d20e4c4e4312c4d3840fdb58724a21cc62f43e8ded134e7b3682`  
		Last Modified: Wed, 09 Jun 2021 16:00:16 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
