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
-	[`nats:2.2.1`](#nats221)
-	[`nats:2.2.1-alpine`](#nats221-alpine)
-	[`nats:2.2.1-alpine3.13`](#nats221-alpine313)
-	[`nats:2.2.1-linux`](#nats221-linux)
-	[`nats:2.2.1-nanoserver`](#nats221-nanoserver)
-	[`nats:2.2.1-nanoserver-1809`](#nats221-nanoserver-1809)
-	[`nats:2.2.1-scratch`](#nats221-scratch)
-	[`nats:2.2.1-windowsservercore`](#nats221-windowsservercore)
-	[`nats:2.2.1-windowsservercore-1809`](#nats221-windowsservercore-1809)
-	[`nats:2.2.1-windowsservercore-ltsc2016`](#nats221-windowsservercore-ltsc2016)
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
$ docker pull nats@sha256:5958ba516eb8f221dc01b26d0afece5f9a48f7f0e978c889d19d1e788a02531e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.1817; amd64

### `nats:2` - linux; amd64

```console
$ docker pull nats@sha256:3bd24b6508d68c6d8835ecf42066a66f01b9e58d55c7a82d99eb3f1d9041fe15
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4208708 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f68fc0ca6306424854628406a234c7c5f76f2a13d658233ecefdb59a3de4ec89`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 03 Apr 2021 03:02:40 GMT
COPY file:494bfb1615387aa8aa24059641c501c246cffbb47653109c93d498a68ccce32a in /nats-server 
# Sat, 03 Apr 2021 03:02:41 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Sat, 03 Apr 2021 03:02:41 GMT
EXPOSE 4222 6222 8222
# Sat, 03 Apr 2021 03:02:41 GMT
ENTRYPOINT ["/nats-server"]
# Sat, 03 Apr 2021 03:02:41 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:832634cbfed021f934fff287987e6acb75f23228af46328d3f79d812b6462c57`  
		Last Modified: Sat, 03 Apr 2021 03:03:31 GMT  
		Size: 4.2 MB (4208232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91f381d2349aa770a85b4fde9e5c7794fe38c878aea8784f679b3f09728534a4`  
		Last Modified: Sat, 03 Apr 2021 03:03:30 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - linux; arm variant v6

```console
$ docker pull nats@sha256:0c1db0c5e32501c283742665116d2ae34168be99f1f0298a17fe6a1a0c3c9cb1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3882437 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dadccf67b2f681485255da8d75647104535e861fb3ee82f610f6d42281a07300`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 03 Apr 2021 01:02:37 GMT
COPY file:54bee7857c6b5cc9e3287e28fd1ffbbd529d72e791a1746d90d0b66346698246 in /nats-server 
# Sat, 03 Apr 2021 01:02:38 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Sat, 03 Apr 2021 01:02:38 GMT
EXPOSE 4222 6222 8222
# Sat, 03 Apr 2021 01:02:39 GMT
ENTRYPOINT ["/nats-server"]
# Sat, 03 Apr 2021 01:02:40 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:91cca6fbde65445d7c75ad5de8204fd8356fa76f2dd2983a53b2c0d9b7255bd9`  
		Last Modified: Sat, 03 Apr 2021 01:03:23 GMT  
		Size: 3.9 MB (3881961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b8d6f093021c26c95a4df34d728495a189d358902c6fed301d6bc06e93f4e85`  
		Last Modified: Sat, 03 Apr 2021 01:03:22 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - linux; arm variant v7

```console
$ docker pull nats@sha256:61dade57dcce93e1f3ea3e01779c4d2f1bf4ff21415290e42dfe72cba333f7d1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3877449 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64ad61fe367441505f4bdd49177124c6f6fbb5d9e212c6b871aec402ea6c4122`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 03 Apr 2021 01:45:33 GMT
COPY file:d95e297af0c7798d74c045b7143a48199a8e32ca5c5aa0b8d7c967a602bc1cfe in /nats-server 
# Sat, 03 Apr 2021 01:45:34 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Sat, 03 Apr 2021 01:45:35 GMT
EXPOSE 4222 6222 8222
# Sat, 03 Apr 2021 01:45:36 GMT
ENTRYPOINT ["/nats-server"]
# Sat, 03 Apr 2021 01:45:37 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:7919165d0b190df92f81ef4af9a0a2fef8a2da95dac86e567498a9364b0be069`  
		Last Modified: Sat, 03 Apr 2021 01:46:21 GMT  
		Size: 3.9 MB (3876974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdfa2b4e61cc1a65501d2feea740d0f932e2bf901c202226b24a7d787c0f4dff`  
		Last Modified: Sat, 03 Apr 2021 01:46:20 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:13c34571ac946007679eb9333b30ca2fc5225ea3afdeb3ec3082bf4e5befe284
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3850749 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9d8fa2c7d5a8fb8a3e96f92707cd39a3107455acd96b42415d60cf31cae334d`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 03 Apr 2021 03:48:01 GMT
COPY file:4d714e3c520aa8a1f5935c65806500f01ea25ace84372fd7f3aa0a06f1f626c9 in /nats-server 
# Sat, 03 Apr 2021 03:48:02 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Sat, 03 Apr 2021 03:48:03 GMT
EXPOSE 4222 6222 8222
# Sat, 03 Apr 2021 03:48:04 GMT
ENTRYPOINT ["/nats-server"]
# Sat, 03 Apr 2021 03:48:05 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:310f293639061b27b8965c8683cf2bffb7d9b58bdb924635525fa7d990f2f3fb`  
		Last Modified: Sat, 03 Apr 2021 03:48:48 GMT  
		Size: 3.9 MB (3850270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e64370dd792941a18253408636a97ab34ef2f6ea706da1fe18ae7e008a3b13e`  
		Last Modified: Sat, 03 Apr 2021 03:48:47 GMT  
		Size: 479.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - windows version 10.0.17763.1817; amd64

```console
$ docker pull nats@sha256:7400f49e711ad398f8708d78498cb89250765f194fcad4bfb28b0811dddce228
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.7 MB (105658317 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d32a24884d574cc6457ee6540f906dc735846c9ed2cd1b15cb1b79c0f0df8fd`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 26 Feb 2021 16:47:31 GMT
RUN Apply image 1809-amd64
# Wed, 10 Mar 2021 16:56:55 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Sat, 03 Apr 2021 01:17:28 GMT
RUN cmd /S /C #(nop) COPY file:428a7e80db4313301a46326a9a79832e9cbe7d78c94e749b5c295e813e484f21 in C:\nats-server.exe 
# Sat, 03 Apr 2021 01:17:29 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Sat, 03 Apr 2021 01:17:30 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Sat, 03 Apr 2021 01:17:30 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Sat, 03 Apr 2021 01:17:32 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a11c4ca8f1ba16b6e1395d4523be2215bd0871c2e3e4695b9f2b87bd7472be52`  
		Size: 101.4 MB (101389964 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f49969195f32b7e40a81e3d189259fec7ebf52ee0ec5dafd5f3f288715354fed`  
		Last Modified: Wed, 10 Mar 2021 17:01:57 GMT  
		Size: 1.0 KB (1047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b78be9ec55bfa99633688cc4d73e47268a005880724f5c31af765df173fe522b`  
		Last Modified: Sat, 03 Apr 2021 01:22:27 GMT  
		Size: 4.3 MB (4262100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93286c3879edf77d449ceff1ed34a72becb3264fead3b488a3f05415c4bb62ec`  
		Last Modified: Sat, 03 Apr 2021 01:22:26 GMT  
		Size: 1.8 KB (1761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a913d40db4af4450743a872058165885095d790cda716fcd48634e3d7f4143f`  
		Last Modified: Sat, 03 Apr 2021 01:22:26 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67f64ab62ffafadee29cddb026c057f47c1d88836cf8c2e1da91189a1289fafd`  
		Last Modified: Sat, 03 Apr 2021 01:22:26 GMT  
		Size: 1.1 KB (1102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f1de1af4e095d547a9e171edf595e46d67d5687074985d261582ae4618438fb`  
		Last Modified: Sat, 03 Apr 2021 01:22:26 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-alpine`

```console
$ docker pull nats@sha256:786039ea5743e66f92097f4c98419cdb7755824388806faae9ca893626cda20f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-alpine` - linux; amd64

```console
$ docker pull nats@sha256:11a99e623a9df5677bdcbcff33bd032975aabdc9c226e00410997607a5398ad0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7303859 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f56ceabe89d18dd0b0c58d97b018484ed43d818791b7a1d9e5e8a09123c6cbd5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 31 Mar 2021 20:10:06 GMT
ADD file:7119167b56ff1228b2fb639c768955ce9db7a999cd947179240b216dfa5ccbb9 in / 
# Wed, 31 Mar 2021 20:10:06 GMT
CMD ["/bin/sh"]
# Sat, 03 Apr 2021 03:02:20 GMT
ENV NATS_SERVER=2.2.1
# Sat, 03 Apr 2021 03:02:23 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='0123d924907282265190258662edf8ad4351055083b5040e3bdf59117bd1c51c' ;; 		armhf) natsArch='arm6'; sha256='da719b07fd57137f85bfa6cffc7d00841a9c1fb4cdf7ca9a537bfc3f99b71f36' ;; 		armv7) natsArch='arm7'; sha256='cf6e8d9a9cc5d05f7320fb4be8fc9239cb87b91c6600a61ce7a2fb63e2f29f5a' ;; 		x86_64) natsArch='amd64'; sha256='70cb40d78b82ea6c0ca926c31ef98d2e1c885cfe2f73f34883e4ca448366c2dd' ;; 		x86) natsArch='386'; sha256='da54d129f8a52c048ded61e3b62e946037a9464d02cf818e568bbf1e385ce6be' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Sat, 03 Apr 2021 03:02:23 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Sat, 03 Apr 2021 03:02:24 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Sat, 03 Apr 2021 03:02:24 GMT
EXPOSE 4222 6222 8222
# Sat, 03 Apr 2021 03:02:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 03 Apr 2021 03:02:24 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:ca3cd42a7c9525f6ce3d64c1a70982613a8235f0cc057ec9244052921853ef15`  
		Last Modified: Wed, 31 Mar 2021 20:10:46 GMT  
		Size: 2.8 MB (2811947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0ab87484469466c6eeb084bcbe5538907a8cca9e02c6c00ffc4e03bd68d4563`  
		Last Modified: Sat, 03 Apr 2021 03:03:06 GMT  
		Size: 4.5 MB (4490943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63537464a64606bc6b408c793c1b726d40b4b1a540a829516859d3405c203e37`  
		Last Modified: Sat, 03 Apr 2021 03:03:05 GMT  
		Size: 557.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:843bbc65e4b41319d487b9ba5eb3a58b709e795448cc632d75fb8f54d76868d9`  
		Last Modified: Sat, 03 Apr 2021 03:03:05 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:5980c4f84be539fd1b559624db6fa63ee409f825e4a93fa441598e93115d4b15
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6784924 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8f97d97f7e09aa5c9f936e0377789f200b06c8aabe846ce2591ebff76f7db8b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 31 Mar 2021 17:18:49 GMT
ADD file:988879d74f643b89539e5a0b6d74221621f19f4f87f722614addadc46ce47200 in / 
# Wed, 31 Mar 2021 17:18:50 GMT
CMD ["/bin/sh"]
# Sat, 03 Apr 2021 01:02:19 GMT
ENV NATS_SERVER=2.2.1
# Sat, 03 Apr 2021 01:02:24 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='0123d924907282265190258662edf8ad4351055083b5040e3bdf59117bd1c51c' ;; 		armhf) natsArch='arm6'; sha256='da719b07fd57137f85bfa6cffc7d00841a9c1fb4cdf7ca9a537bfc3f99b71f36' ;; 		armv7) natsArch='arm7'; sha256='cf6e8d9a9cc5d05f7320fb4be8fc9239cb87b91c6600a61ce7a2fb63e2f29f5a' ;; 		x86_64) natsArch='amd64'; sha256='70cb40d78b82ea6c0ca926c31ef98d2e1c885cfe2f73f34883e4ca448366c2dd' ;; 		x86) natsArch='386'; sha256='da54d129f8a52c048ded61e3b62e946037a9464d02cf818e568bbf1e385ce6be' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Sat, 03 Apr 2021 01:02:25 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Sat, 03 Apr 2021 01:02:26 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Sat, 03 Apr 2021 01:02:26 GMT
EXPOSE 4222 6222 8222
# Sat, 03 Apr 2021 01:02:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 03 Apr 2021 01:02:28 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:bb87125c6ee1ce30c6b33d2c96a9fbe46da4a290f7cb1dd73fd62d4e06503699`  
		Last Modified: Wed, 31 Mar 2021 17:19:55 GMT  
		Size: 2.6 MB (2622116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8d4b6ba6b297e822b0c0fe254f2d6b5afda81265eaf2481116af687cf66235c`  
		Last Modified: Sat, 03 Apr 2021 01:03:09 GMT  
		Size: 4.2 MB (4161834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ae0dfcf0132d6f11bd4762e4d1ec0b73f5ee36875a95dc78731673415f9de05`  
		Last Modified: Sat, 03 Apr 2021 01:03:07 GMT  
		Size: 561.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4f6ffd2be76e6334bd04318e19b02428d71b315b61ae8bb68ade8b07279ccff`  
		Last Modified: Sat, 03 Apr 2021 01:03:07 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:8e048143304eabc1fad2f149b2761e661ebe261c60e0ecb4cd0f58818ca12090
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6583142 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:04ad730346110f756c4e29df7ebe6e02cb97db3770b8fdda258f5f4def7c2f88`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 31 Mar 2021 18:13:27 GMT
ADD file:56e92c06393237a87e0a1ff475e9c9dc80e897d69ec20f45359b587906da345b in / 
# Wed, 31 Mar 2021 18:13:31 GMT
CMD ["/bin/sh"]
# Sat, 03 Apr 2021 01:45:11 GMT
ENV NATS_SERVER=2.2.1
# Sat, 03 Apr 2021 01:45:16 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='0123d924907282265190258662edf8ad4351055083b5040e3bdf59117bd1c51c' ;; 		armhf) natsArch='arm6'; sha256='da719b07fd57137f85bfa6cffc7d00841a9c1fb4cdf7ca9a537bfc3f99b71f36' ;; 		armv7) natsArch='arm7'; sha256='cf6e8d9a9cc5d05f7320fb4be8fc9239cb87b91c6600a61ce7a2fb63e2f29f5a' ;; 		x86_64) natsArch='amd64'; sha256='70cb40d78b82ea6c0ca926c31ef98d2e1c885cfe2f73f34883e4ca448366c2dd' ;; 		x86) natsArch='386'; sha256='da54d129f8a52c048ded61e3b62e946037a9464d02cf818e568bbf1e385ce6be' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Sat, 03 Apr 2021 01:45:17 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Sat, 03 Apr 2021 01:45:18 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Sat, 03 Apr 2021 01:45:19 GMT
EXPOSE 4222 6222 8222
# Sat, 03 Apr 2021 01:45:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 03 Apr 2021 01:45:21 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:07389e51ea05e1c9a3cb0ef92d31181f2afa1e445207ad99ffd8a94d6d6af295`  
		Last Modified: Wed, 31 Mar 2021 18:14:57 GMT  
		Size: 2.4 MB (2424108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7331da30076f2eba452960efaf8df4620f03624062670e29e8e3fb97823756b3`  
		Last Modified: Sat, 03 Apr 2021 01:46:03 GMT  
		Size: 4.2 MB (4158064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abd26a9a6149ca00bb0a5e94ae858765a0b787564c99ea0ba4ec23d5cd7a8bd9`  
		Last Modified: Sat, 03 Apr 2021 01:46:02 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96a5a7410fa6228e048f75c6327720948ad9d6dd06db4b594d43165c1f6cab1c`  
		Last Modified: Sat, 03 Apr 2021 01:46:01 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:980841965bacdff61fc62145784092e89a8c0db1f125fccc5e9d240f60f94e93
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6844304 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99075b219d76c9593adb6b735cc906569e0124a6761312332407ee8de31e6382`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 31 Mar 2021 17:21:21 GMT
ADD file:3b16ffee2b26d8af5db152fcc582aaccd9e1ec9e3343874e9969a205550fe07d in / 
# Wed, 31 Mar 2021 17:21:23 GMT
CMD ["/bin/sh"]
# Sat, 03 Apr 2021 03:47:42 GMT
ENV NATS_SERVER=2.2.1
# Sat, 03 Apr 2021 03:47:46 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='0123d924907282265190258662edf8ad4351055083b5040e3bdf59117bd1c51c' ;; 		armhf) natsArch='arm6'; sha256='da719b07fd57137f85bfa6cffc7d00841a9c1fb4cdf7ca9a537bfc3f99b71f36' ;; 		armv7) natsArch='arm7'; sha256='cf6e8d9a9cc5d05f7320fb4be8fc9239cb87b91c6600a61ce7a2fb63e2f29f5a' ;; 		x86_64) natsArch='amd64'; sha256='70cb40d78b82ea6c0ca926c31ef98d2e1c885cfe2f73f34883e4ca448366c2dd' ;; 		x86) natsArch='386'; sha256='da54d129f8a52c048ded61e3b62e946037a9464d02cf818e568bbf1e385ce6be' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Sat, 03 Apr 2021 03:47:47 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Sat, 03 Apr 2021 03:47:48 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Sat, 03 Apr 2021 03:47:49 GMT
EXPOSE 4222 6222 8222
# Sat, 03 Apr 2021 03:47:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 03 Apr 2021 03:47:51 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:912815139b61c8926da31f7701f0a924e7964e3713052bf1a53193a4562157f6`  
		Last Modified: Wed, 31 Mar 2021 17:22:41 GMT  
		Size: 2.7 MB (2711920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9228d7a2d7ff547081c5c823de18c8fa62bb6200cee9f820f437c3004e90f309`  
		Last Modified: Sat, 03 Apr 2021 03:48:31 GMT  
		Size: 4.1 MB (4131414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ec0c89cac556aea8879a9beeefc7c2f8528b16539e3765c11de3c76e564e6f6`  
		Last Modified: Sat, 03 Apr 2021 03:48:30 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08fc29c470aa8216b46da0c00b30283b238b812f9d1395be3920045c367005af`  
		Last Modified: Sat, 03 Apr 2021 03:48:30 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-alpine3.13`

```console
$ docker pull nats@sha256:786039ea5743e66f92097f4c98419cdb7755824388806faae9ca893626cda20f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-alpine3.13` - linux; amd64

```console
$ docker pull nats@sha256:11a99e623a9df5677bdcbcff33bd032975aabdc9c226e00410997607a5398ad0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7303859 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f56ceabe89d18dd0b0c58d97b018484ed43d818791b7a1d9e5e8a09123c6cbd5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 31 Mar 2021 20:10:06 GMT
ADD file:7119167b56ff1228b2fb639c768955ce9db7a999cd947179240b216dfa5ccbb9 in / 
# Wed, 31 Mar 2021 20:10:06 GMT
CMD ["/bin/sh"]
# Sat, 03 Apr 2021 03:02:20 GMT
ENV NATS_SERVER=2.2.1
# Sat, 03 Apr 2021 03:02:23 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='0123d924907282265190258662edf8ad4351055083b5040e3bdf59117bd1c51c' ;; 		armhf) natsArch='arm6'; sha256='da719b07fd57137f85bfa6cffc7d00841a9c1fb4cdf7ca9a537bfc3f99b71f36' ;; 		armv7) natsArch='arm7'; sha256='cf6e8d9a9cc5d05f7320fb4be8fc9239cb87b91c6600a61ce7a2fb63e2f29f5a' ;; 		x86_64) natsArch='amd64'; sha256='70cb40d78b82ea6c0ca926c31ef98d2e1c885cfe2f73f34883e4ca448366c2dd' ;; 		x86) natsArch='386'; sha256='da54d129f8a52c048ded61e3b62e946037a9464d02cf818e568bbf1e385ce6be' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Sat, 03 Apr 2021 03:02:23 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Sat, 03 Apr 2021 03:02:24 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Sat, 03 Apr 2021 03:02:24 GMT
EXPOSE 4222 6222 8222
# Sat, 03 Apr 2021 03:02:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 03 Apr 2021 03:02:24 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:ca3cd42a7c9525f6ce3d64c1a70982613a8235f0cc057ec9244052921853ef15`  
		Last Modified: Wed, 31 Mar 2021 20:10:46 GMT  
		Size: 2.8 MB (2811947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0ab87484469466c6eeb084bcbe5538907a8cca9e02c6c00ffc4e03bd68d4563`  
		Last Modified: Sat, 03 Apr 2021 03:03:06 GMT  
		Size: 4.5 MB (4490943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63537464a64606bc6b408c793c1b726d40b4b1a540a829516859d3405c203e37`  
		Last Modified: Sat, 03 Apr 2021 03:03:05 GMT  
		Size: 557.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:843bbc65e4b41319d487b9ba5eb3a58b709e795448cc632d75fb8f54d76868d9`  
		Last Modified: Sat, 03 Apr 2021 03:03:05 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.13` - linux; arm variant v6

```console
$ docker pull nats@sha256:5980c4f84be539fd1b559624db6fa63ee409f825e4a93fa441598e93115d4b15
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6784924 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8f97d97f7e09aa5c9f936e0377789f200b06c8aabe846ce2591ebff76f7db8b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 31 Mar 2021 17:18:49 GMT
ADD file:988879d74f643b89539e5a0b6d74221621f19f4f87f722614addadc46ce47200 in / 
# Wed, 31 Mar 2021 17:18:50 GMT
CMD ["/bin/sh"]
# Sat, 03 Apr 2021 01:02:19 GMT
ENV NATS_SERVER=2.2.1
# Sat, 03 Apr 2021 01:02:24 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='0123d924907282265190258662edf8ad4351055083b5040e3bdf59117bd1c51c' ;; 		armhf) natsArch='arm6'; sha256='da719b07fd57137f85bfa6cffc7d00841a9c1fb4cdf7ca9a537bfc3f99b71f36' ;; 		armv7) natsArch='arm7'; sha256='cf6e8d9a9cc5d05f7320fb4be8fc9239cb87b91c6600a61ce7a2fb63e2f29f5a' ;; 		x86_64) natsArch='amd64'; sha256='70cb40d78b82ea6c0ca926c31ef98d2e1c885cfe2f73f34883e4ca448366c2dd' ;; 		x86) natsArch='386'; sha256='da54d129f8a52c048ded61e3b62e946037a9464d02cf818e568bbf1e385ce6be' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Sat, 03 Apr 2021 01:02:25 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Sat, 03 Apr 2021 01:02:26 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Sat, 03 Apr 2021 01:02:26 GMT
EXPOSE 4222 6222 8222
# Sat, 03 Apr 2021 01:02:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 03 Apr 2021 01:02:28 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:bb87125c6ee1ce30c6b33d2c96a9fbe46da4a290f7cb1dd73fd62d4e06503699`  
		Last Modified: Wed, 31 Mar 2021 17:19:55 GMT  
		Size: 2.6 MB (2622116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8d4b6ba6b297e822b0c0fe254f2d6b5afda81265eaf2481116af687cf66235c`  
		Last Modified: Sat, 03 Apr 2021 01:03:09 GMT  
		Size: 4.2 MB (4161834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ae0dfcf0132d6f11bd4762e4d1ec0b73f5ee36875a95dc78731673415f9de05`  
		Last Modified: Sat, 03 Apr 2021 01:03:07 GMT  
		Size: 561.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4f6ffd2be76e6334bd04318e19b02428d71b315b61ae8bb68ade8b07279ccff`  
		Last Modified: Sat, 03 Apr 2021 01:03:07 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.13` - linux; arm variant v7

```console
$ docker pull nats@sha256:8e048143304eabc1fad2f149b2761e661ebe261c60e0ecb4cd0f58818ca12090
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6583142 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:04ad730346110f756c4e29df7ebe6e02cb97db3770b8fdda258f5f4def7c2f88`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 31 Mar 2021 18:13:27 GMT
ADD file:56e92c06393237a87e0a1ff475e9c9dc80e897d69ec20f45359b587906da345b in / 
# Wed, 31 Mar 2021 18:13:31 GMT
CMD ["/bin/sh"]
# Sat, 03 Apr 2021 01:45:11 GMT
ENV NATS_SERVER=2.2.1
# Sat, 03 Apr 2021 01:45:16 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='0123d924907282265190258662edf8ad4351055083b5040e3bdf59117bd1c51c' ;; 		armhf) natsArch='arm6'; sha256='da719b07fd57137f85bfa6cffc7d00841a9c1fb4cdf7ca9a537bfc3f99b71f36' ;; 		armv7) natsArch='arm7'; sha256='cf6e8d9a9cc5d05f7320fb4be8fc9239cb87b91c6600a61ce7a2fb63e2f29f5a' ;; 		x86_64) natsArch='amd64'; sha256='70cb40d78b82ea6c0ca926c31ef98d2e1c885cfe2f73f34883e4ca448366c2dd' ;; 		x86) natsArch='386'; sha256='da54d129f8a52c048ded61e3b62e946037a9464d02cf818e568bbf1e385ce6be' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Sat, 03 Apr 2021 01:45:17 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Sat, 03 Apr 2021 01:45:18 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Sat, 03 Apr 2021 01:45:19 GMT
EXPOSE 4222 6222 8222
# Sat, 03 Apr 2021 01:45:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 03 Apr 2021 01:45:21 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:07389e51ea05e1c9a3cb0ef92d31181f2afa1e445207ad99ffd8a94d6d6af295`  
		Last Modified: Wed, 31 Mar 2021 18:14:57 GMT  
		Size: 2.4 MB (2424108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7331da30076f2eba452960efaf8df4620f03624062670e29e8e3fb97823756b3`  
		Last Modified: Sat, 03 Apr 2021 01:46:03 GMT  
		Size: 4.2 MB (4158064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abd26a9a6149ca00bb0a5e94ae858765a0b787564c99ea0ba4ec23d5cd7a8bd9`  
		Last Modified: Sat, 03 Apr 2021 01:46:02 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96a5a7410fa6228e048f75c6327720948ad9d6dd06db4b594d43165c1f6cab1c`  
		Last Modified: Sat, 03 Apr 2021 01:46:01 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.13` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:980841965bacdff61fc62145784092e89a8c0db1f125fccc5e9d240f60f94e93
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6844304 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99075b219d76c9593adb6b735cc906569e0124a6761312332407ee8de31e6382`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 31 Mar 2021 17:21:21 GMT
ADD file:3b16ffee2b26d8af5db152fcc582aaccd9e1ec9e3343874e9969a205550fe07d in / 
# Wed, 31 Mar 2021 17:21:23 GMT
CMD ["/bin/sh"]
# Sat, 03 Apr 2021 03:47:42 GMT
ENV NATS_SERVER=2.2.1
# Sat, 03 Apr 2021 03:47:46 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='0123d924907282265190258662edf8ad4351055083b5040e3bdf59117bd1c51c' ;; 		armhf) natsArch='arm6'; sha256='da719b07fd57137f85bfa6cffc7d00841a9c1fb4cdf7ca9a537bfc3f99b71f36' ;; 		armv7) natsArch='arm7'; sha256='cf6e8d9a9cc5d05f7320fb4be8fc9239cb87b91c6600a61ce7a2fb63e2f29f5a' ;; 		x86_64) natsArch='amd64'; sha256='70cb40d78b82ea6c0ca926c31ef98d2e1c885cfe2f73f34883e4ca448366c2dd' ;; 		x86) natsArch='386'; sha256='da54d129f8a52c048ded61e3b62e946037a9464d02cf818e568bbf1e385ce6be' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Sat, 03 Apr 2021 03:47:47 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Sat, 03 Apr 2021 03:47:48 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Sat, 03 Apr 2021 03:47:49 GMT
EXPOSE 4222 6222 8222
# Sat, 03 Apr 2021 03:47:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 03 Apr 2021 03:47:51 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:912815139b61c8926da31f7701f0a924e7964e3713052bf1a53193a4562157f6`  
		Last Modified: Wed, 31 Mar 2021 17:22:41 GMT  
		Size: 2.7 MB (2711920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9228d7a2d7ff547081c5c823de18c8fa62bb6200cee9f820f437c3004e90f309`  
		Last Modified: Sat, 03 Apr 2021 03:48:31 GMT  
		Size: 4.1 MB (4131414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ec0c89cac556aea8879a9beeefc7c2f8528b16539e3765c11de3c76e564e6f6`  
		Last Modified: Sat, 03 Apr 2021 03:48:30 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08fc29c470aa8216b46da0c00b30283b238b812f9d1395be3920045c367005af`  
		Last Modified: Sat, 03 Apr 2021 03:48:30 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-linux`

```console
$ docker pull nats@sha256:f116a903fd14977153dc2ae74e3b0437762ee2a6c7858807246d6501b2a9af54
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-linux` - linux; amd64

```console
$ docker pull nats@sha256:3bd24b6508d68c6d8835ecf42066a66f01b9e58d55c7a82d99eb3f1d9041fe15
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4208708 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f68fc0ca6306424854628406a234c7c5f76f2a13d658233ecefdb59a3de4ec89`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 03 Apr 2021 03:02:40 GMT
COPY file:494bfb1615387aa8aa24059641c501c246cffbb47653109c93d498a68ccce32a in /nats-server 
# Sat, 03 Apr 2021 03:02:41 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Sat, 03 Apr 2021 03:02:41 GMT
EXPOSE 4222 6222 8222
# Sat, 03 Apr 2021 03:02:41 GMT
ENTRYPOINT ["/nats-server"]
# Sat, 03 Apr 2021 03:02:41 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:832634cbfed021f934fff287987e6acb75f23228af46328d3f79d812b6462c57`  
		Last Modified: Sat, 03 Apr 2021 03:03:31 GMT  
		Size: 4.2 MB (4208232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91f381d2349aa770a85b4fde9e5c7794fe38c878aea8784f679b3f09728534a4`  
		Last Modified: Sat, 03 Apr 2021 03:03:30 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:0c1db0c5e32501c283742665116d2ae34168be99f1f0298a17fe6a1a0c3c9cb1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3882437 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dadccf67b2f681485255da8d75647104535e861fb3ee82f610f6d42281a07300`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 03 Apr 2021 01:02:37 GMT
COPY file:54bee7857c6b5cc9e3287e28fd1ffbbd529d72e791a1746d90d0b66346698246 in /nats-server 
# Sat, 03 Apr 2021 01:02:38 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Sat, 03 Apr 2021 01:02:38 GMT
EXPOSE 4222 6222 8222
# Sat, 03 Apr 2021 01:02:39 GMT
ENTRYPOINT ["/nats-server"]
# Sat, 03 Apr 2021 01:02:40 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:91cca6fbde65445d7c75ad5de8204fd8356fa76f2dd2983a53b2c0d9b7255bd9`  
		Last Modified: Sat, 03 Apr 2021 01:03:23 GMT  
		Size: 3.9 MB (3881961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b8d6f093021c26c95a4df34d728495a189d358902c6fed301d6bc06e93f4e85`  
		Last Modified: Sat, 03 Apr 2021 01:03:22 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:61dade57dcce93e1f3ea3e01779c4d2f1bf4ff21415290e42dfe72cba333f7d1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3877449 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64ad61fe367441505f4bdd49177124c6f6fbb5d9e212c6b871aec402ea6c4122`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 03 Apr 2021 01:45:33 GMT
COPY file:d95e297af0c7798d74c045b7143a48199a8e32ca5c5aa0b8d7c967a602bc1cfe in /nats-server 
# Sat, 03 Apr 2021 01:45:34 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Sat, 03 Apr 2021 01:45:35 GMT
EXPOSE 4222 6222 8222
# Sat, 03 Apr 2021 01:45:36 GMT
ENTRYPOINT ["/nats-server"]
# Sat, 03 Apr 2021 01:45:37 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:7919165d0b190df92f81ef4af9a0a2fef8a2da95dac86e567498a9364b0be069`  
		Last Modified: Sat, 03 Apr 2021 01:46:21 GMT  
		Size: 3.9 MB (3876974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdfa2b4e61cc1a65501d2feea740d0f932e2bf901c202226b24a7d787c0f4dff`  
		Last Modified: Sat, 03 Apr 2021 01:46:20 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:13c34571ac946007679eb9333b30ca2fc5225ea3afdeb3ec3082bf4e5befe284
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3850749 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9d8fa2c7d5a8fb8a3e96f92707cd39a3107455acd96b42415d60cf31cae334d`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 03 Apr 2021 03:48:01 GMT
COPY file:4d714e3c520aa8a1f5935c65806500f01ea25ace84372fd7f3aa0a06f1f626c9 in /nats-server 
# Sat, 03 Apr 2021 03:48:02 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Sat, 03 Apr 2021 03:48:03 GMT
EXPOSE 4222 6222 8222
# Sat, 03 Apr 2021 03:48:04 GMT
ENTRYPOINT ["/nats-server"]
# Sat, 03 Apr 2021 03:48:05 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:310f293639061b27b8965c8683cf2bffb7d9b58bdb924635525fa7d990f2f3fb`  
		Last Modified: Sat, 03 Apr 2021 03:48:48 GMT  
		Size: 3.9 MB (3850270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e64370dd792941a18253408636a97ab34ef2f6ea706da1fe18ae7e008a3b13e`  
		Last Modified: Sat, 03 Apr 2021 03:48:47 GMT  
		Size: 479.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-nanoserver`

```console
$ docker pull nats@sha256:795115a3a3b1b5f4cbc7c017ddd52f46848199b694cff7aafbcb0c7d464925e5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1817; amd64

### `nats:2-nanoserver` - windows version 10.0.17763.1817; amd64

```console
$ docker pull nats@sha256:7400f49e711ad398f8708d78498cb89250765f194fcad4bfb28b0811dddce228
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.7 MB (105658317 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d32a24884d574cc6457ee6540f906dc735846c9ed2cd1b15cb1b79c0f0df8fd`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 26 Feb 2021 16:47:31 GMT
RUN Apply image 1809-amd64
# Wed, 10 Mar 2021 16:56:55 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Sat, 03 Apr 2021 01:17:28 GMT
RUN cmd /S /C #(nop) COPY file:428a7e80db4313301a46326a9a79832e9cbe7d78c94e749b5c295e813e484f21 in C:\nats-server.exe 
# Sat, 03 Apr 2021 01:17:29 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Sat, 03 Apr 2021 01:17:30 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Sat, 03 Apr 2021 01:17:30 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Sat, 03 Apr 2021 01:17:32 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a11c4ca8f1ba16b6e1395d4523be2215bd0871c2e3e4695b9f2b87bd7472be52`  
		Size: 101.4 MB (101389964 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f49969195f32b7e40a81e3d189259fec7ebf52ee0ec5dafd5f3f288715354fed`  
		Last Modified: Wed, 10 Mar 2021 17:01:57 GMT  
		Size: 1.0 KB (1047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b78be9ec55bfa99633688cc4d73e47268a005880724f5c31af765df173fe522b`  
		Last Modified: Sat, 03 Apr 2021 01:22:27 GMT  
		Size: 4.3 MB (4262100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93286c3879edf77d449ceff1ed34a72becb3264fead3b488a3f05415c4bb62ec`  
		Last Modified: Sat, 03 Apr 2021 01:22:26 GMT  
		Size: 1.8 KB (1761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a913d40db4af4450743a872058165885095d790cda716fcd48634e3d7f4143f`  
		Last Modified: Sat, 03 Apr 2021 01:22:26 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67f64ab62ffafadee29cddb026c057f47c1d88836cf8c2e1da91189a1289fafd`  
		Last Modified: Sat, 03 Apr 2021 01:22:26 GMT  
		Size: 1.1 KB (1102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f1de1af4e095d547a9e171edf595e46d67d5687074985d261582ae4618438fb`  
		Last Modified: Sat, 03 Apr 2021 01:22:26 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-nanoserver-1809`

```console
$ docker pull nats@sha256:795115a3a3b1b5f4cbc7c017ddd52f46848199b694cff7aafbcb0c7d464925e5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1817; amd64

### `nats:2-nanoserver-1809` - windows version 10.0.17763.1817; amd64

```console
$ docker pull nats@sha256:7400f49e711ad398f8708d78498cb89250765f194fcad4bfb28b0811dddce228
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.7 MB (105658317 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d32a24884d574cc6457ee6540f906dc735846c9ed2cd1b15cb1b79c0f0df8fd`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 26 Feb 2021 16:47:31 GMT
RUN Apply image 1809-amd64
# Wed, 10 Mar 2021 16:56:55 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Sat, 03 Apr 2021 01:17:28 GMT
RUN cmd /S /C #(nop) COPY file:428a7e80db4313301a46326a9a79832e9cbe7d78c94e749b5c295e813e484f21 in C:\nats-server.exe 
# Sat, 03 Apr 2021 01:17:29 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Sat, 03 Apr 2021 01:17:30 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Sat, 03 Apr 2021 01:17:30 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Sat, 03 Apr 2021 01:17:32 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a11c4ca8f1ba16b6e1395d4523be2215bd0871c2e3e4695b9f2b87bd7472be52`  
		Size: 101.4 MB (101389964 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f49969195f32b7e40a81e3d189259fec7ebf52ee0ec5dafd5f3f288715354fed`  
		Last Modified: Wed, 10 Mar 2021 17:01:57 GMT  
		Size: 1.0 KB (1047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b78be9ec55bfa99633688cc4d73e47268a005880724f5c31af765df173fe522b`  
		Last Modified: Sat, 03 Apr 2021 01:22:27 GMT  
		Size: 4.3 MB (4262100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93286c3879edf77d449ceff1ed34a72becb3264fead3b488a3f05415c4bb62ec`  
		Last Modified: Sat, 03 Apr 2021 01:22:26 GMT  
		Size: 1.8 KB (1761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a913d40db4af4450743a872058165885095d790cda716fcd48634e3d7f4143f`  
		Last Modified: Sat, 03 Apr 2021 01:22:26 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67f64ab62ffafadee29cddb026c057f47c1d88836cf8c2e1da91189a1289fafd`  
		Last Modified: Sat, 03 Apr 2021 01:22:26 GMT  
		Size: 1.1 KB (1102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f1de1af4e095d547a9e171edf595e46d67d5687074985d261582ae4618438fb`  
		Last Modified: Sat, 03 Apr 2021 01:22:26 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-scratch`

```console
$ docker pull nats@sha256:f116a903fd14977153dc2ae74e3b0437762ee2a6c7858807246d6501b2a9af54
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-scratch` - linux; amd64

```console
$ docker pull nats@sha256:3bd24b6508d68c6d8835ecf42066a66f01b9e58d55c7a82d99eb3f1d9041fe15
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4208708 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f68fc0ca6306424854628406a234c7c5f76f2a13d658233ecefdb59a3de4ec89`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 03 Apr 2021 03:02:40 GMT
COPY file:494bfb1615387aa8aa24059641c501c246cffbb47653109c93d498a68ccce32a in /nats-server 
# Sat, 03 Apr 2021 03:02:41 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Sat, 03 Apr 2021 03:02:41 GMT
EXPOSE 4222 6222 8222
# Sat, 03 Apr 2021 03:02:41 GMT
ENTRYPOINT ["/nats-server"]
# Sat, 03 Apr 2021 03:02:41 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:832634cbfed021f934fff287987e6acb75f23228af46328d3f79d812b6462c57`  
		Last Modified: Sat, 03 Apr 2021 03:03:31 GMT  
		Size: 4.2 MB (4208232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91f381d2349aa770a85b4fde9e5c7794fe38c878aea8784f679b3f09728534a4`  
		Last Modified: Sat, 03 Apr 2021 03:03:30 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:0c1db0c5e32501c283742665116d2ae34168be99f1f0298a17fe6a1a0c3c9cb1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3882437 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dadccf67b2f681485255da8d75647104535e861fb3ee82f610f6d42281a07300`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 03 Apr 2021 01:02:37 GMT
COPY file:54bee7857c6b5cc9e3287e28fd1ffbbd529d72e791a1746d90d0b66346698246 in /nats-server 
# Sat, 03 Apr 2021 01:02:38 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Sat, 03 Apr 2021 01:02:38 GMT
EXPOSE 4222 6222 8222
# Sat, 03 Apr 2021 01:02:39 GMT
ENTRYPOINT ["/nats-server"]
# Sat, 03 Apr 2021 01:02:40 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:91cca6fbde65445d7c75ad5de8204fd8356fa76f2dd2983a53b2c0d9b7255bd9`  
		Last Modified: Sat, 03 Apr 2021 01:03:23 GMT  
		Size: 3.9 MB (3881961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b8d6f093021c26c95a4df34d728495a189d358902c6fed301d6bc06e93f4e85`  
		Last Modified: Sat, 03 Apr 2021 01:03:22 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:61dade57dcce93e1f3ea3e01779c4d2f1bf4ff21415290e42dfe72cba333f7d1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3877449 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64ad61fe367441505f4bdd49177124c6f6fbb5d9e212c6b871aec402ea6c4122`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 03 Apr 2021 01:45:33 GMT
COPY file:d95e297af0c7798d74c045b7143a48199a8e32ca5c5aa0b8d7c967a602bc1cfe in /nats-server 
# Sat, 03 Apr 2021 01:45:34 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Sat, 03 Apr 2021 01:45:35 GMT
EXPOSE 4222 6222 8222
# Sat, 03 Apr 2021 01:45:36 GMT
ENTRYPOINT ["/nats-server"]
# Sat, 03 Apr 2021 01:45:37 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:7919165d0b190df92f81ef4af9a0a2fef8a2da95dac86e567498a9364b0be069`  
		Last Modified: Sat, 03 Apr 2021 01:46:21 GMT  
		Size: 3.9 MB (3876974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdfa2b4e61cc1a65501d2feea740d0f932e2bf901c202226b24a7d787c0f4dff`  
		Last Modified: Sat, 03 Apr 2021 01:46:20 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:13c34571ac946007679eb9333b30ca2fc5225ea3afdeb3ec3082bf4e5befe284
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3850749 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9d8fa2c7d5a8fb8a3e96f92707cd39a3107455acd96b42415d60cf31cae334d`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 03 Apr 2021 03:48:01 GMT
COPY file:4d714e3c520aa8a1f5935c65806500f01ea25ace84372fd7f3aa0a06f1f626c9 in /nats-server 
# Sat, 03 Apr 2021 03:48:02 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Sat, 03 Apr 2021 03:48:03 GMT
EXPOSE 4222 6222 8222
# Sat, 03 Apr 2021 03:48:04 GMT
ENTRYPOINT ["/nats-server"]
# Sat, 03 Apr 2021 03:48:05 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:310f293639061b27b8965c8683cf2bffb7d9b58bdb924635525fa7d990f2f3fb`  
		Last Modified: Sat, 03 Apr 2021 03:48:48 GMT  
		Size: 3.9 MB (3850270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e64370dd792941a18253408636a97ab34ef2f6ea706da1fe18ae7e008a3b13e`  
		Last Modified: Sat, 03 Apr 2021 03:48:47 GMT  
		Size: 479.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-windowsservercore`

```console
$ docker pull nats@sha256:91810bbcbf606b0cf379000443d302c7b5d928cc7309c63da19917ca3ff0525f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1817; amd64
	-	windows version 10.0.14393.4283; amd64

### `nats:2-windowsservercore` - windows version 10.0.17763.1817; amd64

```console
$ docker pull nats@sha256:79eefa8948e2758f0659fb934899c37b05b67eb96c38b0e8c67c1a0974992423
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2480294595 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3875d7d95dfdb0356da902eee6142a19a85e38ae7ddde3bbf34b06e18765ecd7`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 27 Feb 2021 09:32:06 GMT
RUN Install update 1809-amd64
# Wed, 10 Mar 2021 14:15:30 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Mar 2021 16:54:55 GMT
ENV NATS_DOCKERIZED=1
# Sat, 03 Apr 2021 01:15:14 GMT
ENV NATS_SERVER=2.2.1
# Sat, 03 Apr 2021 01:15:16 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.2.1/nats-server-v2.2.1-windows-amd64.zip
# Sat, 03 Apr 2021 01:15:17 GMT
ENV GIT_DOWNLOAD_SHA256=1f0d48a7ba9200e2572016a9f3e1ec7e630f0518cc0b40950c14ff3a5d900924
# Sat, 03 Apr 2021 01:15:50 GMT
RUN Set-PSDebug -Trace 2
# Sat, 03 Apr 2021 01:17:04 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Sat, 03 Apr 2021 01:17:06 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Sat, 03 Apr 2021 01:17:07 GMT
EXPOSE 4222 6222 8222
# Sat, 03 Apr 2021 01:17:08 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Sat, 03 Apr 2021 01:17:09 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5ff1512f88ecd4ff0a91ade34d43733c48834433e35f062f80e6e70d706f8d73`  
		Size: 743.2 MB (743201590 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:31ae1fcdffac4071930a0d98172fc515a43c93aa55870e4b6cc8c789b9444e73`  
		Last Modified: Wed, 10 Mar 2021 16:22:41 GMT  
		Size: 1.3 KB (1305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cfde5dabd6353190a5343286e79ed9ad72f47f48ca9197e594b9771b5039e7d`  
		Last Modified: Wed, 10 Mar 2021 17:01:37 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4eb0ea2b178ae862896fca7bda0c5c677fd82870ca007ebe695e42f058831af`  
		Last Modified: Sat, 03 Apr 2021 01:22:03 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8c9d68c9aa9d29abd0c09f2016e9fcfc53bd185a7403989cec09108f661a977`  
		Last Modified: Sat, 03 Apr 2021 01:22:03 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b05ed1fd68964dcfc103f5452b7ee8528749d538e395dd36d17158cab031fdf`  
		Last Modified: Sat, 03 Apr 2021 01:22:03 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3994ed7efdb8fb7c71541583ff656c6c8e54e722284ec414d3ef00145cb43efa`  
		Last Modified: Sat, 03 Apr 2021 01:22:09 GMT  
		Size: 5.1 MB (5064967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0c3e4f395cd1bacff8cb6c6a451cfe4d56b4a054cfc15dd1a8b04a9e56240fa`  
		Last Modified: Sat, 03 Apr 2021 01:22:03 GMT  
		Size: 13.7 MB (13681925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bc88971a96126558018ca2f17f084db054369de555c8cb84a508c7a1394236e`  
		Last Modified: Sat, 03 Apr 2021 01:22:00 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66fa36b1a5dd3f83c94c4e1597659532cb557cd8f9cd414bb81f1049f39924af`  
		Last Modified: Sat, 03 Apr 2021 01:22:00 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4147b1dd2e59f8f133ab83ace94bf75ef78c0f9f261d49d65b7cc0b84d49438e`  
		Last Modified: Sat, 03 Apr 2021 01:22:00 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49b9455ff088b797d1cff54432e7f275092555cd8485bbf6b4aa926b88077f94`  
		Last Modified: Sat, 03 Apr 2021 01:22:00 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-windowsservercore` - windows version 10.0.14393.4283; amd64

```console
$ docker pull nats@sha256:ea694b06746523df91b7d824d0fc9030b282cc666bf34e937103b72b280d8a09
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5817027558 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:265f2ee0b7a998cc6ce663873648377be2b81226575d11ed5d1537b35a4118bf`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 03 Mar 2021 18:02:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Mar 2021 14:25:01 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Mar 2021 16:57:09 GMT
ENV NATS_DOCKERIZED=1
# Sat, 03 Apr 2021 01:17:41 GMT
ENV NATS_SERVER=2.2.1
# Sat, 03 Apr 2021 01:17:42 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.2.1/nats-server-v2.2.1-windows-amd64.zip
# Sat, 03 Apr 2021 01:17:43 GMT
ENV GIT_DOWNLOAD_SHA256=1f0d48a7ba9200e2572016a9f3e1ec7e630f0518cc0b40950c14ff3a5d900924
# Sat, 03 Apr 2021 01:19:05 GMT
RUN Set-PSDebug -Trace 2
# Sat, 03 Apr 2021 01:21:10 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Sat, 03 Apr 2021 01:21:11 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Sat, 03 Apr 2021 01:21:12 GMT
EXPOSE 4222 6222 8222
# Sat, 03 Apr 2021 01:21:13 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Sat, 03 Apr 2021 01:21:14 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:30bda99601c5cbd3b2118409f401852ea648e2319bd81518723e476b28d764c5`  
		Size: 1.7 GB (1726924885 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5205e01a19ce3835a7f1caba14b71dbbcae05a77274c60358d9794ee0e2a3e65`  
		Last Modified: Wed, 10 Mar 2021 16:23:35 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4390a91a59ec3760f5740301d69b960d0f0b7fb212a8bc2201b27b93b24d4054`  
		Last Modified: Wed, 10 Mar 2021 17:02:23 GMT  
		Size: 1.3 KB (1305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdf068626801ee0e0c0bd2b1a1f9e05e2d16d27757653ade2a5cc0d971764f50`  
		Last Modified: Sat, 03 Apr 2021 01:22:47 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36e3dd9e9e868f213575a6d17e3fda275a2d47d15e2f9d13ad6d206a0f8567a7`  
		Last Modified: Sat, 03 Apr 2021 01:22:47 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:657647c528aa33d6da248e5aeeb7babe0f7976361e1654d5920cdb0b6c4848b9`  
		Last Modified: Sat, 03 Apr 2021 01:22:47 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:389f475c113034c3ad6f5619cf1bc1b11fdad81b5e5e009ba573539909b23423`  
		Last Modified: Sat, 03 Apr 2021 01:22:48 GMT  
		Size: 5.7 MB (5656062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd7a05da95e65b18383e1ae5b037f3b75a628a6af2949313789b364e70c3e7dc`  
		Last Modified: Sat, 03 Apr 2021 01:22:48 GMT  
		Size: 14.4 MB (14447531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55d02d4cabb443df53f1d6f7a6f93f8f9dda642d034916077f4fab20c5632675`  
		Last Modified: Sat, 03 Apr 2021 01:22:44 GMT  
		Size: 2.0 KB (1974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06b93a0d4c513ec838b27546bad996f092605e9c8399ad016f78b8b4cb96a900`  
		Last Modified: Sat, 03 Apr 2021 01:22:44 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8317ff85679d749fdf54c66f1b278c9f16aa11a116c5c0d288bc4f8debe41262`  
		Last Modified: Sat, 03 Apr 2021 01:22:44 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b8b1e736261cff8c3afa409fd73d85b78d6610a610e3b8eb3412798d3a18348`  
		Last Modified: Sat, 03 Apr 2021 01:22:44 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-windowsservercore-1809`

```console
$ docker pull nats@sha256:f8a4f8888f531755c5711af4f90423afca2a36de1890ddd11b74df0dad4bd18c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1817; amd64

### `nats:2-windowsservercore-1809` - windows version 10.0.17763.1817; amd64

```console
$ docker pull nats@sha256:79eefa8948e2758f0659fb934899c37b05b67eb96c38b0e8c67c1a0974992423
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2480294595 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3875d7d95dfdb0356da902eee6142a19a85e38ae7ddde3bbf34b06e18765ecd7`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 27 Feb 2021 09:32:06 GMT
RUN Install update 1809-amd64
# Wed, 10 Mar 2021 14:15:30 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Mar 2021 16:54:55 GMT
ENV NATS_DOCKERIZED=1
# Sat, 03 Apr 2021 01:15:14 GMT
ENV NATS_SERVER=2.2.1
# Sat, 03 Apr 2021 01:15:16 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.2.1/nats-server-v2.2.1-windows-amd64.zip
# Sat, 03 Apr 2021 01:15:17 GMT
ENV GIT_DOWNLOAD_SHA256=1f0d48a7ba9200e2572016a9f3e1ec7e630f0518cc0b40950c14ff3a5d900924
# Sat, 03 Apr 2021 01:15:50 GMT
RUN Set-PSDebug -Trace 2
# Sat, 03 Apr 2021 01:17:04 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Sat, 03 Apr 2021 01:17:06 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Sat, 03 Apr 2021 01:17:07 GMT
EXPOSE 4222 6222 8222
# Sat, 03 Apr 2021 01:17:08 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Sat, 03 Apr 2021 01:17:09 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5ff1512f88ecd4ff0a91ade34d43733c48834433e35f062f80e6e70d706f8d73`  
		Size: 743.2 MB (743201590 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:31ae1fcdffac4071930a0d98172fc515a43c93aa55870e4b6cc8c789b9444e73`  
		Last Modified: Wed, 10 Mar 2021 16:22:41 GMT  
		Size: 1.3 KB (1305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cfde5dabd6353190a5343286e79ed9ad72f47f48ca9197e594b9771b5039e7d`  
		Last Modified: Wed, 10 Mar 2021 17:01:37 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4eb0ea2b178ae862896fca7bda0c5c677fd82870ca007ebe695e42f058831af`  
		Last Modified: Sat, 03 Apr 2021 01:22:03 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8c9d68c9aa9d29abd0c09f2016e9fcfc53bd185a7403989cec09108f661a977`  
		Last Modified: Sat, 03 Apr 2021 01:22:03 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b05ed1fd68964dcfc103f5452b7ee8528749d538e395dd36d17158cab031fdf`  
		Last Modified: Sat, 03 Apr 2021 01:22:03 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3994ed7efdb8fb7c71541583ff656c6c8e54e722284ec414d3ef00145cb43efa`  
		Last Modified: Sat, 03 Apr 2021 01:22:09 GMT  
		Size: 5.1 MB (5064967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0c3e4f395cd1bacff8cb6c6a451cfe4d56b4a054cfc15dd1a8b04a9e56240fa`  
		Last Modified: Sat, 03 Apr 2021 01:22:03 GMT  
		Size: 13.7 MB (13681925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bc88971a96126558018ca2f17f084db054369de555c8cb84a508c7a1394236e`  
		Last Modified: Sat, 03 Apr 2021 01:22:00 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66fa36b1a5dd3f83c94c4e1597659532cb557cd8f9cd414bb81f1049f39924af`  
		Last Modified: Sat, 03 Apr 2021 01:22:00 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4147b1dd2e59f8f133ab83ace94bf75ef78c0f9f261d49d65b7cc0b84d49438e`  
		Last Modified: Sat, 03 Apr 2021 01:22:00 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49b9455ff088b797d1cff54432e7f275092555cd8485bbf6b4aa926b88077f94`  
		Last Modified: Sat, 03 Apr 2021 01:22:00 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-windowsservercore-ltsc2016`

```console
$ docker pull nats@sha256:a29981e9b9b26371bed2856c6ac2b18e78e0ec9db3aeb251d0d8b281501c7196
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4283; amd64

### `nats:2-windowsservercore-ltsc2016` - windows version 10.0.14393.4283; amd64

```console
$ docker pull nats@sha256:ea694b06746523df91b7d824d0fc9030b282cc666bf34e937103b72b280d8a09
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5817027558 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:265f2ee0b7a998cc6ce663873648377be2b81226575d11ed5d1537b35a4118bf`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 03 Mar 2021 18:02:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Mar 2021 14:25:01 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Mar 2021 16:57:09 GMT
ENV NATS_DOCKERIZED=1
# Sat, 03 Apr 2021 01:17:41 GMT
ENV NATS_SERVER=2.2.1
# Sat, 03 Apr 2021 01:17:42 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.2.1/nats-server-v2.2.1-windows-amd64.zip
# Sat, 03 Apr 2021 01:17:43 GMT
ENV GIT_DOWNLOAD_SHA256=1f0d48a7ba9200e2572016a9f3e1ec7e630f0518cc0b40950c14ff3a5d900924
# Sat, 03 Apr 2021 01:19:05 GMT
RUN Set-PSDebug -Trace 2
# Sat, 03 Apr 2021 01:21:10 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Sat, 03 Apr 2021 01:21:11 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Sat, 03 Apr 2021 01:21:12 GMT
EXPOSE 4222 6222 8222
# Sat, 03 Apr 2021 01:21:13 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Sat, 03 Apr 2021 01:21:14 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:30bda99601c5cbd3b2118409f401852ea648e2319bd81518723e476b28d764c5`  
		Size: 1.7 GB (1726924885 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5205e01a19ce3835a7f1caba14b71dbbcae05a77274c60358d9794ee0e2a3e65`  
		Last Modified: Wed, 10 Mar 2021 16:23:35 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4390a91a59ec3760f5740301d69b960d0f0b7fb212a8bc2201b27b93b24d4054`  
		Last Modified: Wed, 10 Mar 2021 17:02:23 GMT  
		Size: 1.3 KB (1305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdf068626801ee0e0c0bd2b1a1f9e05e2d16d27757653ade2a5cc0d971764f50`  
		Last Modified: Sat, 03 Apr 2021 01:22:47 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36e3dd9e9e868f213575a6d17e3fda275a2d47d15e2f9d13ad6d206a0f8567a7`  
		Last Modified: Sat, 03 Apr 2021 01:22:47 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:657647c528aa33d6da248e5aeeb7babe0f7976361e1654d5920cdb0b6c4848b9`  
		Last Modified: Sat, 03 Apr 2021 01:22:47 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:389f475c113034c3ad6f5619cf1bc1b11fdad81b5e5e009ba573539909b23423`  
		Last Modified: Sat, 03 Apr 2021 01:22:48 GMT  
		Size: 5.7 MB (5656062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd7a05da95e65b18383e1ae5b037f3b75a628a6af2949313789b364e70c3e7dc`  
		Last Modified: Sat, 03 Apr 2021 01:22:48 GMT  
		Size: 14.4 MB (14447531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55d02d4cabb443df53f1d6f7a6f93f8f9dda642d034916077f4fab20c5632675`  
		Last Modified: Sat, 03 Apr 2021 01:22:44 GMT  
		Size: 2.0 KB (1974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06b93a0d4c513ec838b27546bad996f092605e9c8399ad016f78b8b4cb96a900`  
		Last Modified: Sat, 03 Apr 2021 01:22:44 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8317ff85679d749fdf54c66f1b278c9f16aa11a116c5c0d288bc4f8debe41262`  
		Last Modified: Sat, 03 Apr 2021 01:22:44 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b8b1e736261cff8c3afa409fd73d85b78d6610a610e3b8eb3412798d3a18348`  
		Last Modified: Sat, 03 Apr 2021 01:22:44 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.2`

```console
$ docker pull nats@sha256:5958ba516eb8f221dc01b26d0afece5f9a48f7f0e978c889d19d1e788a02531e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.1817; amd64

### `nats:2.2` - linux; amd64

```console
$ docker pull nats@sha256:3bd24b6508d68c6d8835ecf42066a66f01b9e58d55c7a82d99eb3f1d9041fe15
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4208708 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f68fc0ca6306424854628406a234c7c5f76f2a13d658233ecefdb59a3de4ec89`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 03 Apr 2021 03:02:40 GMT
COPY file:494bfb1615387aa8aa24059641c501c246cffbb47653109c93d498a68ccce32a in /nats-server 
# Sat, 03 Apr 2021 03:02:41 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Sat, 03 Apr 2021 03:02:41 GMT
EXPOSE 4222 6222 8222
# Sat, 03 Apr 2021 03:02:41 GMT
ENTRYPOINT ["/nats-server"]
# Sat, 03 Apr 2021 03:02:41 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:832634cbfed021f934fff287987e6acb75f23228af46328d3f79d812b6462c57`  
		Last Modified: Sat, 03 Apr 2021 03:03:31 GMT  
		Size: 4.2 MB (4208232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91f381d2349aa770a85b4fde9e5c7794fe38c878aea8784f679b3f09728534a4`  
		Last Modified: Sat, 03 Apr 2021 03:03:30 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2` - linux; arm variant v6

```console
$ docker pull nats@sha256:0c1db0c5e32501c283742665116d2ae34168be99f1f0298a17fe6a1a0c3c9cb1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3882437 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dadccf67b2f681485255da8d75647104535e861fb3ee82f610f6d42281a07300`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 03 Apr 2021 01:02:37 GMT
COPY file:54bee7857c6b5cc9e3287e28fd1ffbbd529d72e791a1746d90d0b66346698246 in /nats-server 
# Sat, 03 Apr 2021 01:02:38 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Sat, 03 Apr 2021 01:02:38 GMT
EXPOSE 4222 6222 8222
# Sat, 03 Apr 2021 01:02:39 GMT
ENTRYPOINT ["/nats-server"]
# Sat, 03 Apr 2021 01:02:40 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:91cca6fbde65445d7c75ad5de8204fd8356fa76f2dd2983a53b2c0d9b7255bd9`  
		Last Modified: Sat, 03 Apr 2021 01:03:23 GMT  
		Size: 3.9 MB (3881961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b8d6f093021c26c95a4df34d728495a189d358902c6fed301d6bc06e93f4e85`  
		Last Modified: Sat, 03 Apr 2021 01:03:22 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2` - linux; arm variant v7

```console
$ docker pull nats@sha256:61dade57dcce93e1f3ea3e01779c4d2f1bf4ff21415290e42dfe72cba333f7d1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3877449 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64ad61fe367441505f4bdd49177124c6f6fbb5d9e212c6b871aec402ea6c4122`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 03 Apr 2021 01:45:33 GMT
COPY file:d95e297af0c7798d74c045b7143a48199a8e32ca5c5aa0b8d7c967a602bc1cfe in /nats-server 
# Sat, 03 Apr 2021 01:45:34 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Sat, 03 Apr 2021 01:45:35 GMT
EXPOSE 4222 6222 8222
# Sat, 03 Apr 2021 01:45:36 GMT
ENTRYPOINT ["/nats-server"]
# Sat, 03 Apr 2021 01:45:37 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:7919165d0b190df92f81ef4af9a0a2fef8a2da95dac86e567498a9364b0be069`  
		Last Modified: Sat, 03 Apr 2021 01:46:21 GMT  
		Size: 3.9 MB (3876974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdfa2b4e61cc1a65501d2feea740d0f932e2bf901c202226b24a7d787c0f4dff`  
		Last Modified: Sat, 03 Apr 2021 01:46:20 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:13c34571ac946007679eb9333b30ca2fc5225ea3afdeb3ec3082bf4e5befe284
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3850749 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9d8fa2c7d5a8fb8a3e96f92707cd39a3107455acd96b42415d60cf31cae334d`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 03 Apr 2021 03:48:01 GMT
COPY file:4d714e3c520aa8a1f5935c65806500f01ea25ace84372fd7f3aa0a06f1f626c9 in /nats-server 
# Sat, 03 Apr 2021 03:48:02 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Sat, 03 Apr 2021 03:48:03 GMT
EXPOSE 4222 6222 8222
# Sat, 03 Apr 2021 03:48:04 GMT
ENTRYPOINT ["/nats-server"]
# Sat, 03 Apr 2021 03:48:05 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:310f293639061b27b8965c8683cf2bffb7d9b58bdb924635525fa7d990f2f3fb`  
		Last Modified: Sat, 03 Apr 2021 03:48:48 GMT  
		Size: 3.9 MB (3850270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e64370dd792941a18253408636a97ab34ef2f6ea706da1fe18ae7e008a3b13e`  
		Last Modified: Sat, 03 Apr 2021 03:48:47 GMT  
		Size: 479.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2` - windows version 10.0.17763.1817; amd64

```console
$ docker pull nats@sha256:7400f49e711ad398f8708d78498cb89250765f194fcad4bfb28b0811dddce228
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.7 MB (105658317 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d32a24884d574cc6457ee6540f906dc735846c9ed2cd1b15cb1b79c0f0df8fd`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 26 Feb 2021 16:47:31 GMT
RUN Apply image 1809-amd64
# Wed, 10 Mar 2021 16:56:55 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Sat, 03 Apr 2021 01:17:28 GMT
RUN cmd /S /C #(nop) COPY file:428a7e80db4313301a46326a9a79832e9cbe7d78c94e749b5c295e813e484f21 in C:\nats-server.exe 
# Sat, 03 Apr 2021 01:17:29 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Sat, 03 Apr 2021 01:17:30 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Sat, 03 Apr 2021 01:17:30 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Sat, 03 Apr 2021 01:17:32 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a11c4ca8f1ba16b6e1395d4523be2215bd0871c2e3e4695b9f2b87bd7472be52`  
		Size: 101.4 MB (101389964 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f49969195f32b7e40a81e3d189259fec7ebf52ee0ec5dafd5f3f288715354fed`  
		Last Modified: Wed, 10 Mar 2021 17:01:57 GMT  
		Size: 1.0 KB (1047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b78be9ec55bfa99633688cc4d73e47268a005880724f5c31af765df173fe522b`  
		Last Modified: Sat, 03 Apr 2021 01:22:27 GMT  
		Size: 4.3 MB (4262100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93286c3879edf77d449ceff1ed34a72becb3264fead3b488a3f05415c4bb62ec`  
		Last Modified: Sat, 03 Apr 2021 01:22:26 GMT  
		Size: 1.8 KB (1761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a913d40db4af4450743a872058165885095d790cda716fcd48634e3d7f4143f`  
		Last Modified: Sat, 03 Apr 2021 01:22:26 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67f64ab62ffafadee29cddb026c057f47c1d88836cf8c2e1da91189a1289fafd`  
		Last Modified: Sat, 03 Apr 2021 01:22:26 GMT  
		Size: 1.1 KB (1102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f1de1af4e095d547a9e171edf595e46d67d5687074985d261582ae4618438fb`  
		Last Modified: Sat, 03 Apr 2021 01:22:26 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.2-alpine`

```console
$ docker pull nats@sha256:786039ea5743e66f92097f4c98419cdb7755824388806faae9ca893626cda20f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.2-alpine` - linux; amd64

```console
$ docker pull nats@sha256:11a99e623a9df5677bdcbcff33bd032975aabdc9c226e00410997607a5398ad0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7303859 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f56ceabe89d18dd0b0c58d97b018484ed43d818791b7a1d9e5e8a09123c6cbd5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 31 Mar 2021 20:10:06 GMT
ADD file:7119167b56ff1228b2fb639c768955ce9db7a999cd947179240b216dfa5ccbb9 in / 
# Wed, 31 Mar 2021 20:10:06 GMT
CMD ["/bin/sh"]
# Sat, 03 Apr 2021 03:02:20 GMT
ENV NATS_SERVER=2.2.1
# Sat, 03 Apr 2021 03:02:23 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='0123d924907282265190258662edf8ad4351055083b5040e3bdf59117bd1c51c' ;; 		armhf) natsArch='arm6'; sha256='da719b07fd57137f85bfa6cffc7d00841a9c1fb4cdf7ca9a537bfc3f99b71f36' ;; 		armv7) natsArch='arm7'; sha256='cf6e8d9a9cc5d05f7320fb4be8fc9239cb87b91c6600a61ce7a2fb63e2f29f5a' ;; 		x86_64) natsArch='amd64'; sha256='70cb40d78b82ea6c0ca926c31ef98d2e1c885cfe2f73f34883e4ca448366c2dd' ;; 		x86) natsArch='386'; sha256='da54d129f8a52c048ded61e3b62e946037a9464d02cf818e568bbf1e385ce6be' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Sat, 03 Apr 2021 03:02:23 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Sat, 03 Apr 2021 03:02:24 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Sat, 03 Apr 2021 03:02:24 GMT
EXPOSE 4222 6222 8222
# Sat, 03 Apr 2021 03:02:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 03 Apr 2021 03:02:24 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:ca3cd42a7c9525f6ce3d64c1a70982613a8235f0cc057ec9244052921853ef15`  
		Last Modified: Wed, 31 Mar 2021 20:10:46 GMT  
		Size: 2.8 MB (2811947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0ab87484469466c6eeb084bcbe5538907a8cca9e02c6c00ffc4e03bd68d4563`  
		Last Modified: Sat, 03 Apr 2021 03:03:06 GMT  
		Size: 4.5 MB (4490943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63537464a64606bc6b408c793c1b726d40b4b1a540a829516859d3405c203e37`  
		Last Modified: Sat, 03 Apr 2021 03:03:05 GMT  
		Size: 557.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:843bbc65e4b41319d487b9ba5eb3a58b709e795448cc632d75fb8f54d76868d9`  
		Last Modified: Sat, 03 Apr 2021 03:03:05 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:5980c4f84be539fd1b559624db6fa63ee409f825e4a93fa441598e93115d4b15
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6784924 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8f97d97f7e09aa5c9f936e0377789f200b06c8aabe846ce2591ebff76f7db8b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 31 Mar 2021 17:18:49 GMT
ADD file:988879d74f643b89539e5a0b6d74221621f19f4f87f722614addadc46ce47200 in / 
# Wed, 31 Mar 2021 17:18:50 GMT
CMD ["/bin/sh"]
# Sat, 03 Apr 2021 01:02:19 GMT
ENV NATS_SERVER=2.2.1
# Sat, 03 Apr 2021 01:02:24 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='0123d924907282265190258662edf8ad4351055083b5040e3bdf59117bd1c51c' ;; 		armhf) natsArch='arm6'; sha256='da719b07fd57137f85bfa6cffc7d00841a9c1fb4cdf7ca9a537bfc3f99b71f36' ;; 		armv7) natsArch='arm7'; sha256='cf6e8d9a9cc5d05f7320fb4be8fc9239cb87b91c6600a61ce7a2fb63e2f29f5a' ;; 		x86_64) natsArch='amd64'; sha256='70cb40d78b82ea6c0ca926c31ef98d2e1c885cfe2f73f34883e4ca448366c2dd' ;; 		x86) natsArch='386'; sha256='da54d129f8a52c048ded61e3b62e946037a9464d02cf818e568bbf1e385ce6be' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Sat, 03 Apr 2021 01:02:25 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Sat, 03 Apr 2021 01:02:26 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Sat, 03 Apr 2021 01:02:26 GMT
EXPOSE 4222 6222 8222
# Sat, 03 Apr 2021 01:02:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 03 Apr 2021 01:02:28 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:bb87125c6ee1ce30c6b33d2c96a9fbe46da4a290f7cb1dd73fd62d4e06503699`  
		Last Modified: Wed, 31 Mar 2021 17:19:55 GMT  
		Size: 2.6 MB (2622116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8d4b6ba6b297e822b0c0fe254f2d6b5afda81265eaf2481116af687cf66235c`  
		Last Modified: Sat, 03 Apr 2021 01:03:09 GMT  
		Size: 4.2 MB (4161834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ae0dfcf0132d6f11bd4762e4d1ec0b73f5ee36875a95dc78731673415f9de05`  
		Last Modified: Sat, 03 Apr 2021 01:03:07 GMT  
		Size: 561.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4f6ffd2be76e6334bd04318e19b02428d71b315b61ae8bb68ade8b07279ccff`  
		Last Modified: Sat, 03 Apr 2021 01:03:07 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:8e048143304eabc1fad2f149b2761e661ebe261c60e0ecb4cd0f58818ca12090
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6583142 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:04ad730346110f756c4e29df7ebe6e02cb97db3770b8fdda258f5f4def7c2f88`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 31 Mar 2021 18:13:27 GMT
ADD file:56e92c06393237a87e0a1ff475e9c9dc80e897d69ec20f45359b587906da345b in / 
# Wed, 31 Mar 2021 18:13:31 GMT
CMD ["/bin/sh"]
# Sat, 03 Apr 2021 01:45:11 GMT
ENV NATS_SERVER=2.2.1
# Sat, 03 Apr 2021 01:45:16 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='0123d924907282265190258662edf8ad4351055083b5040e3bdf59117bd1c51c' ;; 		armhf) natsArch='arm6'; sha256='da719b07fd57137f85bfa6cffc7d00841a9c1fb4cdf7ca9a537bfc3f99b71f36' ;; 		armv7) natsArch='arm7'; sha256='cf6e8d9a9cc5d05f7320fb4be8fc9239cb87b91c6600a61ce7a2fb63e2f29f5a' ;; 		x86_64) natsArch='amd64'; sha256='70cb40d78b82ea6c0ca926c31ef98d2e1c885cfe2f73f34883e4ca448366c2dd' ;; 		x86) natsArch='386'; sha256='da54d129f8a52c048ded61e3b62e946037a9464d02cf818e568bbf1e385ce6be' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Sat, 03 Apr 2021 01:45:17 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Sat, 03 Apr 2021 01:45:18 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Sat, 03 Apr 2021 01:45:19 GMT
EXPOSE 4222 6222 8222
# Sat, 03 Apr 2021 01:45:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 03 Apr 2021 01:45:21 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:07389e51ea05e1c9a3cb0ef92d31181f2afa1e445207ad99ffd8a94d6d6af295`  
		Last Modified: Wed, 31 Mar 2021 18:14:57 GMT  
		Size: 2.4 MB (2424108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7331da30076f2eba452960efaf8df4620f03624062670e29e8e3fb97823756b3`  
		Last Modified: Sat, 03 Apr 2021 01:46:03 GMT  
		Size: 4.2 MB (4158064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abd26a9a6149ca00bb0a5e94ae858765a0b787564c99ea0ba4ec23d5cd7a8bd9`  
		Last Modified: Sat, 03 Apr 2021 01:46:02 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96a5a7410fa6228e048f75c6327720948ad9d6dd06db4b594d43165c1f6cab1c`  
		Last Modified: Sat, 03 Apr 2021 01:46:01 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2-alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:980841965bacdff61fc62145784092e89a8c0db1f125fccc5e9d240f60f94e93
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6844304 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99075b219d76c9593adb6b735cc906569e0124a6761312332407ee8de31e6382`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 31 Mar 2021 17:21:21 GMT
ADD file:3b16ffee2b26d8af5db152fcc582aaccd9e1ec9e3343874e9969a205550fe07d in / 
# Wed, 31 Mar 2021 17:21:23 GMT
CMD ["/bin/sh"]
# Sat, 03 Apr 2021 03:47:42 GMT
ENV NATS_SERVER=2.2.1
# Sat, 03 Apr 2021 03:47:46 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='0123d924907282265190258662edf8ad4351055083b5040e3bdf59117bd1c51c' ;; 		armhf) natsArch='arm6'; sha256='da719b07fd57137f85bfa6cffc7d00841a9c1fb4cdf7ca9a537bfc3f99b71f36' ;; 		armv7) natsArch='arm7'; sha256='cf6e8d9a9cc5d05f7320fb4be8fc9239cb87b91c6600a61ce7a2fb63e2f29f5a' ;; 		x86_64) natsArch='amd64'; sha256='70cb40d78b82ea6c0ca926c31ef98d2e1c885cfe2f73f34883e4ca448366c2dd' ;; 		x86) natsArch='386'; sha256='da54d129f8a52c048ded61e3b62e946037a9464d02cf818e568bbf1e385ce6be' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Sat, 03 Apr 2021 03:47:47 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Sat, 03 Apr 2021 03:47:48 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Sat, 03 Apr 2021 03:47:49 GMT
EXPOSE 4222 6222 8222
# Sat, 03 Apr 2021 03:47:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 03 Apr 2021 03:47:51 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:912815139b61c8926da31f7701f0a924e7964e3713052bf1a53193a4562157f6`  
		Last Modified: Wed, 31 Mar 2021 17:22:41 GMT  
		Size: 2.7 MB (2711920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9228d7a2d7ff547081c5c823de18c8fa62bb6200cee9f820f437c3004e90f309`  
		Last Modified: Sat, 03 Apr 2021 03:48:31 GMT  
		Size: 4.1 MB (4131414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ec0c89cac556aea8879a9beeefc7c2f8528b16539e3765c11de3c76e564e6f6`  
		Last Modified: Sat, 03 Apr 2021 03:48:30 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08fc29c470aa8216b46da0c00b30283b238b812f9d1395be3920045c367005af`  
		Last Modified: Sat, 03 Apr 2021 03:48:30 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.2-alpine3.13`

```console
$ docker pull nats@sha256:786039ea5743e66f92097f4c98419cdb7755824388806faae9ca893626cda20f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.2-alpine3.13` - linux; amd64

```console
$ docker pull nats@sha256:11a99e623a9df5677bdcbcff33bd032975aabdc9c226e00410997607a5398ad0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7303859 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f56ceabe89d18dd0b0c58d97b018484ed43d818791b7a1d9e5e8a09123c6cbd5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 31 Mar 2021 20:10:06 GMT
ADD file:7119167b56ff1228b2fb639c768955ce9db7a999cd947179240b216dfa5ccbb9 in / 
# Wed, 31 Mar 2021 20:10:06 GMT
CMD ["/bin/sh"]
# Sat, 03 Apr 2021 03:02:20 GMT
ENV NATS_SERVER=2.2.1
# Sat, 03 Apr 2021 03:02:23 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='0123d924907282265190258662edf8ad4351055083b5040e3bdf59117bd1c51c' ;; 		armhf) natsArch='arm6'; sha256='da719b07fd57137f85bfa6cffc7d00841a9c1fb4cdf7ca9a537bfc3f99b71f36' ;; 		armv7) natsArch='arm7'; sha256='cf6e8d9a9cc5d05f7320fb4be8fc9239cb87b91c6600a61ce7a2fb63e2f29f5a' ;; 		x86_64) natsArch='amd64'; sha256='70cb40d78b82ea6c0ca926c31ef98d2e1c885cfe2f73f34883e4ca448366c2dd' ;; 		x86) natsArch='386'; sha256='da54d129f8a52c048ded61e3b62e946037a9464d02cf818e568bbf1e385ce6be' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Sat, 03 Apr 2021 03:02:23 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Sat, 03 Apr 2021 03:02:24 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Sat, 03 Apr 2021 03:02:24 GMT
EXPOSE 4222 6222 8222
# Sat, 03 Apr 2021 03:02:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 03 Apr 2021 03:02:24 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:ca3cd42a7c9525f6ce3d64c1a70982613a8235f0cc057ec9244052921853ef15`  
		Last Modified: Wed, 31 Mar 2021 20:10:46 GMT  
		Size: 2.8 MB (2811947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0ab87484469466c6eeb084bcbe5538907a8cca9e02c6c00ffc4e03bd68d4563`  
		Last Modified: Sat, 03 Apr 2021 03:03:06 GMT  
		Size: 4.5 MB (4490943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63537464a64606bc6b408c793c1b726d40b4b1a540a829516859d3405c203e37`  
		Last Modified: Sat, 03 Apr 2021 03:03:05 GMT  
		Size: 557.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:843bbc65e4b41319d487b9ba5eb3a58b709e795448cc632d75fb8f54d76868d9`  
		Last Modified: Sat, 03 Apr 2021 03:03:05 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2-alpine3.13` - linux; arm variant v6

```console
$ docker pull nats@sha256:5980c4f84be539fd1b559624db6fa63ee409f825e4a93fa441598e93115d4b15
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6784924 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8f97d97f7e09aa5c9f936e0377789f200b06c8aabe846ce2591ebff76f7db8b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 31 Mar 2021 17:18:49 GMT
ADD file:988879d74f643b89539e5a0b6d74221621f19f4f87f722614addadc46ce47200 in / 
# Wed, 31 Mar 2021 17:18:50 GMT
CMD ["/bin/sh"]
# Sat, 03 Apr 2021 01:02:19 GMT
ENV NATS_SERVER=2.2.1
# Sat, 03 Apr 2021 01:02:24 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='0123d924907282265190258662edf8ad4351055083b5040e3bdf59117bd1c51c' ;; 		armhf) natsArch='arm6'; sha256='da719b07fd57137f85bfa6cffc7d00841a9c1fb4cdf7ca9a537bfc3f99b71f36' ;; 		armv7) natsArch='arm7'; sha256='cf6e8d9a9cc5d05f7320fb4be8fc9239cb87b91c6600a61ce7a2fb63e2f29f5a' ;; 		x86_64) natsArch='amd64'; sha256='70cb40d78b82ea6c0ca926c31ef98d2e1c885cfe2f73f34883e4ca448366c2dd' ;; 		x86) natsArch='386'; sha256='da54d129f8a52c048ded61e3b62e946037a9464d02cf818e568bbf1e385ce6be' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Sat, 03 Apr 2021 01:02:25 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Sat, 03 Apr 2021 01:02:26 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Sat, 03 Apr 2021 01:02:26 GMT
EXPOSE 4222 6222 8222
# Sat, 03 Apr 2021 01:02:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 03 Apr 2021 01:02:28 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:bb87125c6ee1ce30c6b33d2c96a9fbe46da4a290f7cb1dd73fd62d4e06503699`  
		Last Modified: Wed, 31 Mar 2021 17:19:55 GMT  
		Size: 2.6 MB (2622116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8d4b6ba6b297e822b0c0fe254f2d6b5afda81265eaf2481116af687cf66235c`  
		Last Modified: Sat, 03 Apr 2021 01:03:09 GMT  
		Size: 4.2 MB (4161834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ae0dfcf0132d6f11bd4762e4d1ec0b73f5ee36875a95dc78731673415f9de05`  
		Last Modified: Sat, 03 Apr 2021 01:03:07 GMT  
		Size: 561.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4f6ffd2be76e6334bd04318e19b02428d71b315b61ae8bb68ade8b07279ccff`  
		Last Modified: Sat, 03 Apr 2021 01:03:07 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2-alpine3.13` - linux; arm variant v7

```console
$ docker pull nats@sha256:8e048143304eabc1fad2f149b2761e661ebe261c60e0ecb4cd0f58818ca12090
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6583142 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:04ad730346110f756c4e29df7ebe6e02cb97db3770b8fdda258f5f4def7c2f88`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 31 Mar 2021 18:13:27 GMT
ADD file:56e92c06393237a87e0a1ff475e9c9dc80e897d69ec20f45359b587906da345b in / 
# Wed, 31 Mar 2021 18:13:31 GMT
CMD ["/bin/sh"]
# Sat, 03 Apr 2021 01:45:11 GMT
ENV NATS_SERVER=2.2.1
# Sat, 03 Apr 2021 01:45:16 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='0123d924907282265190258662edf8ad4351055083b5040e3bdf59117bd1c51c' ;; 		armhf) natsArch='arm6'; sha256='da719b07fd57137f85bfa6cffc7d00841a9c1fb4cdf7ca9a537bfc3f99b71f36' ;; 		armv7) natsArch='arm7'; sha256='cf6e8d9a9cc5d05f7320fb4be8fc9239cb87b91c6600a61ce7a2fb63e2f29f5a' ;; 		x86_64) natsArch='amd64'; sha256='70cb40d78b82ea6c0ca926c31ef98d2e1c885cfe2f73f34883e4ca448366c2dd' ;; 		x86) natsArch='386'; sha256='da54d129f8a52c048ded61e3b62e946037a9464d02cf818e568bbf1e385ce6be' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Sat, 03 Apr 2021 01:45:17 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Sat, 03 Apr 2021 01:45:18 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Sat, 03 Apr 2021 01:45:19 GMT
EXPOSE 4222 6222 8222
# Sat, 03 Apr 2021 01:45:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 03 Apr 2021 01:45:21 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:07389e51ea05e1c9a3cb0ef92d31181f2afa1e445207ad99ffd8a94d6d6af295`  
		Last Modified: Wed, 31 Mar 2021 18:14:57 GMT  
		Size: 2.4 MB (2424108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7331da30076f2eba452960efaf8df4620f03624062670e29e8e3fb97823756b3`  
		Last Modified: Sat, 03 Apr 2021 01:46:03 GMT  
		Size: 4.2 MB (4158064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abd26a9a6149ca00bb0a5e94ae858765a0b787564c99ea0ba4ec23d5cd7a8bd9`  
		Last Modified: Sat, 03 Apr 2021 01:46:02 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96a5a7410fa6228e048f75c6327720948ad9d6dd06db4b594d43165c1f6cab1c`  
		Last Modified: Sat, 03 Apr 2021 01:46:01 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2-alpine3.13` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:980841965bacdff61fc62145784092e89a8c0db1f125fccc5e9d240f60f94e93
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6844304 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99075b219d76c9593adb6b735cc906569e0124a6761312332407ee8de31e6382`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 31 Mar 2021 17:21:21 GMT
ADD file:3b16ffee2b26d8af5db152fcc582aaccd9e1ec9e3343874e9969a205550fe07d in / 
# Wed, 31 Mar 2021 17:21:23 GMT
CMD ["/bin/sh"]
# Sat, 03 Apr 2021 03:47:42 GMT
ENV NATS_SERVER=2.2.1
# Sat, 03 Apr 2021 03:47:46 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='0123d924907282265190258662edf8ad4351055083b5040e3bdf59117bd1c51c' ;; 		armhf) natsArch='arm6'; sha256='da719b07fd57137f85bfa6cffc7d00841a9c1fb4cdf7ca9a537bfc3f99b71f36' ;; 		armv7) natsArch='arm7'; sha256='cf6e8d9a9cc5d05f7320fb4be8fc9239cb87b91c6600a61ce7a2fb63e2f29f5a' ;; 		x86_64) natsArch='amd64'; sha256='70cb40d78b82ea6c0ca926c31ef98d2e1c885cfe2f73f34883e4ca448366c2dd' ;; 		x86) natsArch='386'; sha256='da54d129f8a52c048ded61e3b62e946037a9464d02cf818e568bbf1e385ce6be' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Sat, 03 Apr 2021 03:47:47 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Sat, 03 Apr 2021 03:47:48 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Sat, 03 Apr 2021 03:47:49 GMT
EXPOSE 4222 6222 8222
# Sat, 03 Apr 2021 03:47:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 03 Apr 2021 03:47:51 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:912815139b61c8926da31f7701f0a924e7964e3713052bf1a53193a4562157f6`  
		Last Modified: Wed, 31 Mar 2021 17:22:41 GMT  
		Size: 2.7 MB (2711920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9228d7a2d7ff547081c5c823de18c8fa62bb6200cee9f820f437c3004e90f309`  
		Last Modified: Sat, 03 Apr 2021 03:48:31 GMT  
		Size: 4.1 MB (4131414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ec0c89cac556aea8879a9beeefc7c2f8528b16539e3765c11de3c76e564e6f6`  
		Last Modified: Sat, 03 Apr 2021 03:48:30 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08fc29c470aa8216b46da0c00b30283b238b812f9d1395be3920045c367005af`  
		Last Modified: Sat, 03 Apr 2021 03:48:30 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.2-linux`

```console
$ docker pull nats@sha256:f116a903fd14977153dc2ae74e3b0437762ee2a6c7858807246d6501b2a9af54
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.2-linux` - linux; amd64

```console
$ docker pull nats@sha256:3bd24b6508d68c6d8835ecf42066a66f01b9e58d55c7a82d99eb3f1d9041fe15
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4208708 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f68fc0ca6306424854628406a234c7c5f76f2a13d658233ecefdb59a3de4ec89`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 03 Apr 2021 03:02:40 GMT
COPY file:494bfb1615387aa8aa24059641c501c246cffbb47653109c93d498a68ccce32a in /nats-server 
# Sat, 03 Apr 2021 03:02:41 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Sat, 03 Apr 2021 03:02:41 GMT
EXPOSE 4222 6222 8222
# Sat, 03 Apr 2021 03:02:41 GMT
ENTRYPOINT ["/nats-server"]
# Sat, 03 Apr 2021 03:02:41 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:832634cbfed021f934fff287987e6acb75f23228af46328d3f79d812b6462c57`  
		Last Modified: Sat, 03 Apr 2021 03:03:31 GMT  
		Size: 4.2 MB (4208232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91f381d2349aa770a85b4fde9e5c7794fe38c878aea8784f679b3f09728534a4`  
		Last Modified: Sat, 03 Apr 2021 03:03:30 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2-linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:0c1db0c5e32501c283742665116d2ae34168be99f1f0298a17fe6a1a0c3c9cb1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3882437 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dadccf67b2f681485255da8d75647104535e861fb3ee82f610f6d42281a07300`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 03 Apr 2021 01:02:37 GMT
COPY file:54bee7857c6b5cc9e3287e28fd1ffbbd529d72e791a1746d90d0b66346698246 in /nats-server 
# Sat, 03 Apr 2021 01:02:38 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Sat, 03 Apr 2021 01:02:38 GMT
EXPOSE 4222 6222 8222
# Sat, 03 Apr 2021 01:02:39 GMT
ENTRYPOINT ["/nats-server"]
# Sat, 03 Apr 2021 01:02:40 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:91cca6fbde65445d7c75ad5de8204fd8356fa76f2dd2983a53b2c0d9b7255bd9`  
		Last Modified: Sat, 03 Apr 2021 01:03:23 GMT  
		Size: 3.9 MB (3881961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b8d6f093021c26c95a4df34d728495a189d358902c6fed301d6bc06e93f4e85`  
		Last Modified: Sat, 03 Apr 2021 01:03:22 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2-linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:61dade57dcce93e1f3ea3e01779c4d2f1bf4ff21415290e42dfe72cba333f7d1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3877449 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64ad61fe367441505f4bdd49177124c6f6fbb5d9e212c6b871aec402ea6c4122`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 03 Apr 2021 01:45:33 GMT
COPY file:d95e297af0c7798d74c045b7143a48199a8e32ca5c5aa0b8d7c967a602bc1cfe in /nats-server 
# Sat, 03 Apr 2021 01:45:34 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Sat, 03 Apr 2021 01:45:35 GMT
EXPOSE 4222 6222 8222
# Sat, 03 Apr 2021 01:45:36 GMT
ENTRYPOINT ["/nats-server"]
# Sat, 03 Apr 2021 01:45:37 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:7919165d0b190df92f81ef4af9a0a2fef8a2da95dac86e567498a9364b0be069`  
		Last Modified: Sat, 03 Apr 2021 01:46:21 GMT  
		Size: 3.9 MB (3876974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdfa2b4e61cc1a65501d2feea740d0f932e2bf901c202226b24a7d787c0f4dff`  
		Last Modified: Sat, 03 Apr 2021 01:46:20 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2-linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:13c34571ac946007679eb9333b30ca2fc5225ea3afdeb3ec3082bf4e5befe284
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3850749 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9d8fa2c7d5a8fb8a3e96f92707cd39a3107455acd96b42415d60cf31cae334d`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 03 Apr 2021 03:48:01 GMT
COPY file:4d714e3c520aa8a1f5935c65806500f01ea25ace84372fd7f3aa0a06f1f626c9 in /nats-server 
# Sat, 03 Apr 2021 03:48:02 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Sat, 03 Apr 2021 03:48:03 GMT
EXPOSE 4222 6222 8222
# Sat, 03 Apr 2021 03:48:04 GMT
ENTRYPOINT ["/nats-server"]
# Sat, 03 Apr 2021 03:48:05 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:310f293639061b27b8965c8683cf2bffb7d9b58bdb924635525fa7d990f2f3fb`  
		Last Modified: Sat, 03 Apr 2021 03:48:48 GMT  
		Size: 3.9 MB (3850270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e64370dd792941a18253408636a97ab34ef2f6ea706da1fe18ae7e008a3b13e`  
		Last Modified: Sat, 03 Apr 2021 03:48:47 GMT  
		Size: 479.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.2-nanoserver`

```console
$ docker pull nats@sha256:795115a3a3b1b5f4cbc7c017ddd52f46848199b694cff7aafbcb0c7d464925e5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1817; amd64

### `nats:2.2-nanoserver` - windows version 10.0.17763.1817; amd64

```console
$ docker pull nats@sha256:7400f49e711ad398f8708d78498cb89250765f194fcad4bfb28b0811dddce228
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.7 MB (105658317 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d32a24884d574cc6457ee6540f906dc735846c9ed2cd1b15cb1b79c0f0df8fd`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 26 Feb 2021 16:47:31 GMT
RUN Apply image 1809-amd64
# Wed, 10 Mar 2021 16:56:55 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Sat, 03 Apr 2021 01:17:28 GMT
RUN cmd /S /C #(nop) COPY file:428a7e80db4313301a46326a9a79832e9cbe7d78c94e749b5c295e813e484f21 in C:\nats-server.exe 
# Sat, 03 Apr 2021 01:17:29 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Sat, 03 Apr 2021 01:17:30 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Sat, 03 Apr 2021 01:17:30 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Sat, 03 Apr 2021 01:17:32 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a11c4ca8f1ba16b6e1395d4523be2215bd0871c2e3e4695b9f2b87bd7472be52`  
		Size: 101.4 MB (101389964 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f49969195f32b7e40a81e3d189259fec7ebf52ee0ec5dafd5f3f288715354fed`  
		Last Modified: Wed, 10 Mar 2021 17:01:57 GMT  
		Size: 1.0 KB (1047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b78be9ec55bfa99633688cc4d73e47268a005880724f5c31af765df173fe522b`  
		Last Modified: Sat, 03 Apr 2021 01:22:27 GMT  
		Size: 4.3 MB (4262100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93286c3879edf77d449ceff1ed34a72becb3264fead3b488a3f05415c4bb62ec`  
		Last Modified: Sat, 03 Apr 2021 01:22:26 GMT  
		Size: 1.8 KB (1761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a913d40db4af4450743a872058165885095d790cda716fcd48634e3d7f4143f`  
		Last Modified: Sat, 03 Apr 2021 01:22:26 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67f64ab62ffafadee29cddb026c057f47c1d88836cf8c2e1da91189a1289fafd`  
		Last Modified: Sat, 03 Apr 2021 01:22:26 GMT  
		Size: 1.1 KB (1102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f1de1af4e095d547a9e171edf595e46d67d5687074985d261582ae4618438fb`  
		Last Modified: Sat, 03 Apr 2021 01:22:26 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.2-nanoserver-1809`

```console
$ docker pull nats@sha256:795115a3a3b1b5f4cbc7c017ddd52f46848199b694cff7aafbcb0c7d464925e5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1817; amd64

### `nats:2.2-nanoserver-1809` - windows version 10.0.17763.1817; amd64

```console
$ docker pull nats@sha256:7400f49e711ad398f8708d78498cb89250765f194fcad4bfb28b0811dddce228
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.7 MB (105658317 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d32a24884d574cc6457ee6540f906dc735846c9ed2cd1b15cb1b79c0f0df8fd`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 26 Feb 2021 16:47:31 GMT
RUN Apply image 1809-amd64
# Wed, 10 Mar 2021 16:56:55 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Sat, 03 Apr 2021 01:17:28 GMT
RUN cmd /S /C #(nop) COPY file:428a7e80db4313301a46326a9a79832e9cbe7d78c94e749b5c295e813e484f21 in C:\nats-server.exe 
# Sat, 03 Apr 2021 01:17:29 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Sat, 03 Apr 2021 01:17:30 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Sat, 03 Apr 2021 01:17:30 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Sat, 03 Apr 2021 01:17:32 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a11c4ca8f1ba16b6e1395d4523be2215bd0871c2e3e4695b9f2b87bd7472be52`  
		Size: 101.4 MB (101389964 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f49969195f32b7e40a81e3d189259fec7ebf52ee0ec5dafd5f3f288715354fed`  
		Last Modified: Wed, 10 Mar 2021 17:01:57 GMT  
		Size: 1.0 KB (1047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b78be9ec55bfa99633688cc4d73e47268a005880724f5c31af765df173fe522b`  
		Last Modified: Sat, 03 Apr 2021 01:22:27 GMT  
		Size: 4.3 MB (4262100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93286c3879edf77d449ceff1ed34a72becb3264fead3b488a3f05415c4bb62ec`  
		Last Modified: Sat, 03 Apr 2021 01:22:26 GMT  
		Size: 1.8 KB (1761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a913d40db4af4450743a872058165885095d790cda716fcd48634e3d7f4143f`  
		Last Modified: Sat, 03 Apr 2021 01:22:26 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67f64ab62ffafadee29cddb026c057f47c1d88836cf8c2e1da91189a1289fafd`  
		Last Modified: Sat, 03 Apr 2021 01:22:26 GMT  
		Size: 1.1 KB (1102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f1de1af4e095d547a9e171edf595e46d67d5687074985d261582ae4618438fb`  
		Last Modified: Sat, 03 Apr 2021 01:22:26 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.2-scratch`

```console
$ docker pull nats@sha256:f116a903fd14977153dc2ae74e3b0437762ee2a6c7858807246d6501b2a9af54
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.2-scratch` - linux; amd64

```console
$ docker pull nats@sha256:3bd24b6508d68c6d8835ecf42066a66f01b9e58d55c7a82d99eb3f1d9041fe15
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4208708 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f68fc0ca6306424854628406a234c7c5f76f2a13d658233ecefdb59a3de4ec89`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 03 Apr 2021 03:02:40 GMT
COPY file:494bfb1615387aa8aa24059641c501c246cffbb47653109c93d498a68ccce32a in /nats-server 
# Sat, 03 Apr 2021 03:02:41 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Sat, 03 Apr 2021 03:02:41 GMT
EXPOSE 4222 6222 8222
# Sat, 03 Apr 2021 03:02:41 GMT
ENTRYPOINT ["/nats-server"]
# Sat, 03 Apr 2021 03:02:41 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:832634cbfed021f934fff287987e6acb75f23228af46328d3f79d812b6462c57`  
		Last Modified: Sat, 03 Apr 2021 03:03:31 GMT  
		Size: 4.2 MB (4208232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91f381d2349aa770a85b4fde9e5c7794fe38c878aea8784f679b3f09728534a4`  
		Last Modified: Sat, 03 Apr 2021 03:03:30 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2-scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:0c1db0c5e32501c283742665116d2ae34168be99f1f0298a17fe6a1a0c3c9cb1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3882437 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dadccf67b2f681485255da8d75647104535e861fb3ee82f610f6d42281a07300`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 03 Apr 2021 01:02:37 GMT
COPY file:54bee7857c6b5cc9e3287e28fd1ffbbd529d72e791a1746d90d0b66346698246 in /nats-server 
# Sat, 03 Apr 2021 01:02:38 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Sat, 03 Apr 2021 01:02:38 GMT
EXPOSE 4222 6222 8222
# Sat, 03 Apr 2021 01:02:39 GMT
ENTRYPOINT ["/nats-server"]
# Sat, 03 Apr 2021 01:02:40 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:91cca6fbde65445d7c75ad5de8204fd8356fa76f2dd2983a53b2c0d9b7255bd9`  
		Last Modified: Sat, 03 Apr 2021 01:03:23 GMT  
		Size: 3.9 MB (3881961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b8d6f093021c26c95a4df34d728495a189d358902c6fed301d6bc06e93f4e85`  
		Last Modified: Sat, 03 Apr 2021 01:03:22 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2-scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:61dade57dcce93e1f3ea3e01779c4d2f1bf4ff21415290e42dfe72cba333f7d1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3877449 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64ad61fe367441505f4bdd49177124c6f6fbb5d9e212c6b871aec402ea6c4122`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 03 Apr 2021 01:45:33 GMT
COPY file:d95e297af0c7798d74c045b7143a48199a8e32ca5c5aa0b8d7c967a602bc1cfe in /nats-server 
# Sat, 03 Apr 2021 01:45:34 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Sat, 03 Apr 2021 01:45:35 GMT
EXPOSE 4222 6222 8222
# Sat, 03 Apr 2021 01:45:36 GMT
ENTRYPOINT ["/nats-server"]
# Sat, 03 Apr 2021 01:45:37 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:7919165d0b190df92f81ef4af9a0a2fef8a2da95dac86e567498a9364b0be069`  
		Last Modified: Sat, 03 Apr 2021 01:46:21 GMT  
		Size: 3.9 MB (3876974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdfa2b4e61cc1a65501d2feea740d0f932e2bf901c202226b24a7d787c0f4dff`  
		Last Modified: Sat, 03 Apr 2021 01:46:20 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2-scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:13c34571ac946007679eb9333b30ca2fc5225ea3afdeb3ec3082bf4e5befe284
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3850749 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9d8fa2c7d5a8fb8a3e96f92707cd39a3107455acd96b42415d60cf31cae334d`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 03 Apr 2021 03:48:01 GMT
COPY file:4d714e3c520aa8a1f5935c65806500f01ea25ace84372fd7f3aa0a06f1f626c9 in /nats-server 
# Sat, 03 Apr 2021 03:48:02 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Sat, 03 Apr 2021 03:48:03 GMT
EXPOSE 4222 6222 8222
# Sat, 03 Apr 2021 03:48:04 GMT
ENTRYPOINT ["/nats-server"]
# Sat, 03 Apr 2021 03:48:05 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:310f293639061b27b8965c8683cf2bffb7d9b58bdb924635525fa7d990f2f3fb`  
		Last Modified: Sat, 03 Apr 2021 03:48:48 GMT  
		Size: 3.9 MB (3850270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e64370dd792941a18253408636a97ab34ef2f6ea706da1fe18ae7e008a3b13e`  
		Last Modified: Sat, 03 Apr 2021 03:48:47 GMT  
		Size: 479.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.2-windowsservercore`

```console
$ docker pull nats@sha256:91810bbcbf606b0cf379000443d302c7b5d928cc7309c63da19917ca3ff0525f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1817; amd64
	-	windows version 10.0.14393.4283; amd64

### `nats:2.2-windowsservercore` - windows version 10.0.17763.1817; amd64

```console
$ docker pull nats@sha256:79eefa8948e2758f0659fb934899c37b05b67eb96c38b0e8c67c1a0974992423
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2480294595 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3875d7d95dfdb0356da902eee6142a19a85e38ae7ddde3bbf34b06e18765ecd7`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 27 Feb 2021 09:32:06 GMT
RUN Install update 1809-amd64
# Wed, 10 Mar 2021 14:15:30 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Mar 2021 16:54:55 GMT
ENV NATS_DOCKERIZED=1
# Sat, 03 Apr 2021 01:15:14 GMT
ENV NATS_SERVER=2.2.1
# Sat, 03 Apr 2021 01:15:16 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.2.1/nats-server-v2.2.1-windows-amd64.zip
# Sat, 03 Apr 2021 01:15:17 GMT
ENV GIT_DOWNLOAD_SHA256=1f0d48a7ba9200e2572016a9f3e1ec7e630f0518cc0b40950c14ff3a5d900924
# Sat, 03 Apr 2021 01:15:50 GMT
RUN Set-PSDebug -Trace 2
# Sat, 03 Apr 2021 01:17:04 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Sat, 03 Apr 2021 01:17:06 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Sat, 03 Apr 2021 01:17:07 GMT
EXPOSE 4222 6222 8222
# Sat, 03 Apr 2021 01:17:08 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Sat, 03 Apr 2021 01:17:09 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5ff1512f88ecd4ff0a91ade34d43733c48834433e35f062f80e6e70d706f8d73`  
		Size: 743.2 MB (743201590 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:31ae1fcdffac4071930a0d98172fc515a43c93aa55870e4b6cc8c789b9444e73`  
		Last Modified: Wed, 10 Mar 2021 16:22:41 GMT  
		Size: 1.3 KB (1305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cfde5dabd6353190a5343286e79ed9ad72f47f48ca9197e594b9771b5039e7d`  
		Last Modified: Wed, 10 Mar 2021 17:01:37 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4eb0ea2b178ae862896fca7bda0c5c677fd82870ca007ebe695e42f058831af`  
		Last Modified: Sat, 03 Apr 2021 01:22:03 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8c9d68c9aa9d29abd0c09f2016e9fcfc53bd185a7403989cec09108f661a977`  
		Last Modified: Sat, 03 Apr 2021 01:22:03 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b05ed1fd68964dcfc103f5452b7ee8528749d538e395dd36d17158cab031fdf`  
		Last Modified: Sat, 03 Apr 2021 01:22:03 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3994ed7efdb8fb7c71541583ff656c6c8e54e722284ec414d3ef00145cb43efa`  
		Last Modified: Sat, 03 Apr 2021 01:22:09 GMT  
		Size: 5.1 MB (5064967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0c3e4f395cd1bacff8cb6c6a451cfe4d56b4a054cfc15dd1a8b04a9e56240fa`  
		Last Modified: Sat, 03 Apr 2021 01:22:03 GMT  
		Size: 13.7 MB (13681925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bc88971a96126558018ca2f17f084db054369de555c8cb84a508c7a1394236e`  
		Last Modified: Sat, 03 Apr 2021 01:22:00 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66fa36b1a5dd3f83c94c4e1597659532cb557cd8f9cd414bb81f1049f39924af`  
		Last Modified: Sat, 03 Apr 2021 01:22:00 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4147b1dd2e59f8f133ab83ace94bf75ef78c0f9f261d49d65b7cc0b84d49438e`  
		Last Modified: Sat, 03 Apr 2021 01:22:00 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49b9455ff088b797d1cff54432e7f275092555cd8485bbf6b4aa926b88077f94`  
		Last Modified: Sat, 03 Apr 2021 01:22:00 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2-windowsservercore` - windows version 10.0.14393.4283; amd64

```console
$ docker pull nats@sha256:ea694b06746523df91b7d824d0fc9030b282cc666bf34e937103b72b280d8a09
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5817027558 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:265f2ee0b7a998cc6ce663873648377be2b81226575d11ed5d1537b35a4118bf`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 03 Mar 2021 18:02:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Mar 2021 14:25:01 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Mar 2021 16:57:09 GMT
ENV NATS_DOCKERIZED=1
# Sat, 03 Apr 2021 01:17:41 GMT
ENV NATS_SERVER=2.2.1
# Sat, 03 Apr 2021 01:17:42 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.2.1/nats-server-v2.2.1-windows-amd64.zip
# Sat, 03 Apr 2021 01:17:43 GMT
ENV GIT_DOWNLOAD_SHA256=1f0d48a7ba9200e2572016a9f3e1ec7e630f0518cc0b40950c14ff3a5d900924
# Sat, 03 Apr 2021 01:19:05 GMT
RUN Set-PSDebug -Trace 2
# Sat, 03 Apr 2021 01:21:10 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Sat, 03 Apr 2021 01:21:11 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Sat, 03 Apr 2021 01:21:12 GMT
EXPOSE 4222 6222 8222
# Sat, 03 Apr 2021 01:21:13 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Sat, 03 Apr 2021 01:21:14 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:30bda99601c5cbd3b2118409f401852ea648e2319bd81518723e476b28d764c5`  
		Size: 1.7 GB (1726924885 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5205e01a19ce3835a7f1caba14b71dbbcae05a77274c60358d9794ee0e2a3e65`  
		Last Modified: Wed, 10 Mar 2021 16:23:35 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4390a91a59ec3760f5740301d69b960d0f0b7fb212a8bc2201b27b93b24d4054`  
		Last Modified: Wed, 10 Mar 2021 17:02:23 GMT  
		Size: 1.3 KB (1305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdf068626801ee0e0c0bd2b1a1f9e05e2d16d27757653ade2a5cc0d971764f50`  
		Last Modified: Sat, 03 Apr 2021 01:22:47 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36e3dd9e9e868f213575a6d17e3fda275a2d47d15e2f9d13ad6d206a0f8567a7`  
		Last Modified: Sat, 03 Apr 2021 01:22:47 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:657647c528aa33d6da248e5aeeb7babe0f7976361e1654d5920cdb0b6c4848b9`  
		Last Modified: Sat, 03 Apr 2021 01:22:47 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:389f475c113034c3ad6f5619cf1bc1b11fdad81b5e5e009ba573539909b23423`  
		Last Modified: Sat, 03 Apr 2021 01:22:48 GMT  
		Size: 5.7 MB (5656062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd7a05da95e65b18383e1ae5b037f3b75a628a6af2949313789b364e70c3e7dc`  
		Last Modified: Sat, 03 Apr 2021 01:22:48 GMT  
		Size: 14.4 MB (14447531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55d02d4cabb443df53f1d6f7a6f93f8f9dda642d034916077f4fab20c5632675`  
		Last Modified: Sat, 03 Apr 2021 01:22:44 GMT  
		Size: 2.0 KB (1974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06b93a0d4c513ec838b27546bad996f092605e9c8399ad016f78b8b4cb96a900`  
		Last Modified: Sat, 03 Apr 2021 01:22:44 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8317ff85679d749fdf54c66f1b278c9f16aa11a116c5c0d288bc4f8debe41262`  
		Last Modified: Sat, 03 Apr 2021 01:22:44 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b8b1e736261cff8c3afa409fd73d85b78d6610a610e3b8eb3412798d3a18348`  
		Last Modified: Sat, 03 Apr 2021 01:22:44 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.2-windowsservercore-1809`

```console
$ docker pull nats@sha256:f8a4f8888f531755c5711af4f90423afca2a36de1890ddd11b74df0dad4bd18c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1817; amd64

### `nats:2.2-windowsservercore-1809` - windows version 10.0.17763.1817; amd64

```console
$ docker pull nats@sha256:79eefa8948e2758f0659fb934899c37b05b67eb96c38b0e8c67c1a0974992423
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2480294595 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3875d7d95dfdb0356da902eee6142a19a85e38ae7ddde3bbf34b06e18765ecd7`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 27 Feb 2021 09:32:06 GMT
RUN Install update 1809-amd64
# Wed, 10 Mar 2021 14:15:30 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Mar 2021 16:54:55 GMT
ENV NATS_DOCKERIZED=1
# Sat, 03 Apr 2021 01:15:14 GMT
ENV NATS_SERVER=2.2.1
# Sat, 03 Apr 2021 01:15:16 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.2.1/nats-server-v2.2.1-windows-amd64.zip
# Sat, 03 Apr 2021 01:15:17 GMT
ENV GIT_DOWNLOAD_SHA256=1f0d48a7ba9200e2572016a9f3e1ec7e630f0518cc0b40950c14ff3a5d900924
# Sat, 03 Apr 2021 01:15:50 GMT
RUN Set-PSDebug -Trace 2
# Sat, 03 Apr 2021 01:17:04 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Sat, 03 Apr 2021 01:17:06 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Sat, 03 Apr 2021 01:17:07 GMT
EXPOSE 4222 6222 8222
# Sat, 03 Apr 2021 01:17:08 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Sat, 03 Apr 2021 01:17:09 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5ff1512f88ecd4ff0a91ade34d43733c48834433e35f062f80e6e70d706f8d73`  
		Size: 743.2 MB (743201590 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:31ae1fcdffac4071930a0d98172fc515a43c93aa55870e4b6cc8c789b9444e73`  
		Last Modified: Wed, 10 Mar 2021 16:22:41 GMT  
		Size: 1.3 KB (1305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cfde5dabd6353190a5343286e79ed9ad72f47f48ca9197e594b9771b5039e7d`  
		Last Modified: Wed, 10 Mar 2021 17:01:37 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4eb0ea2b178ae862896fca7bda0c5c677fd82870ca007ebe695e42f058831af`  
		Last Modified: Sat, 03 Apr 2021 01:22:03 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8c9d68c9aa9d29abd0c09f2016e9fcfc53bd185a7403989cec09108f661a977`  
		Last Modified: Sat, 03 Apr 2021 01:22:03 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b05ed1fd68964dcfc103f5452b7ee8528749d538e395dd36d17158cab031fdf`  
		Last Modified: Sat, 03 Apr 2021 01:22:03 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3994ed7efdb8fb7c71541583ff656c6c8e54e722284ec414d3ef00145cb43efa`  
		Last Modified: Sat, 03 Apr 2021 01:22:09 GMT  
		Size: 5.1 MB (5064967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0c3e4f395cd1bacff8cb6c6a451cfe4d56b4a054cfc15dd1a8b04a9e56240fa`  
		Last Modified: Sat, 03 Apr 2021 01:22:03 GMT  
		Size: 13.7 MB (13681925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bc88971a96126558018ca2f17f084db054369de555c8cb84a508c7a1394236e`  
		Last Modified: Sat, 03 Apr 2021 01:22:00 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66fa36b1a5dd3f83c94c4e1597659532cb557cd8f9cd414bb81f1049f39924af`  
		Last Modified: Sat, 03 Apr 2021 01:22:00 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4147b1dd2e59f8f133ab83ace94bf75ef78c0f9f261d49d65b7cc0b84d49438e`  
		Last Modified: Sat, 03 Apr 2021 01:22:00 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49b9455ff088b797d1cff54432e7f275092555cd8485bbf6b4aa926b88077f94`  
		Last Modified: Sat, 03 Apr 2021 01:22:00 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.2-windowsservercore-ltsc2016`

```console
$ docker pull nats@sha256:a29981e9b9b26371bed2856c6ac2b18e78e0ec9db3aeb251d0d8b281501c7196
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4283; amd64

### `nats:2.2-windowsservercore-ltsc2016` - windows version 10.0.14393.4283; amd64

```console
$ docker pull nats@sha256:ea694b06746523df91b7d824d0fc9030b282cc666bf34e937103b72b280d8a09
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5817027558 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:265f2ee0b7a998cc6ce663873648377be2b81226575d11ed5d1537b35a4118bf`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 03 Mar 2021 18:02:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Mar 2021 14:25:01 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Mar 2021 16:57:09 GMT
ENV NATS_DOCKERIZED=1
# Sat, 03 Apr 2021 01:17:41 GMT
ENV NATS_SERVER=2.2.1
# Sat, 03 Apr 2021 01:17:42 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.2.1/nats-server-v2.2.1-windows-amd64.zip
# Sat, 03 Apr 2021 01:17:43 GMT
ENV GIT_DOWNLOAD_SHA256=1f0d48a7ba9200e2572016a9f3e1ec7e630f0518cc0b40950c14ff3a5d900924
# Sat, 03 Apr 2021 01:19:05 GMT
RUN Set-PSDebug -Trace 2
# Sat, 03 Apr 2021 01:21:10 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Sat, 03 Apr 2021 01:21:11 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Sat, 03 Apr 2021 01:21:12 GMT
EXPOSE 4222 6222 8222
# Sat, 03 Apr 2021 01:21:13 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Sat, 03 Apr 2021 01:21:14 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:30bda99601c5cbd3b2118409f401852ea648e2319bd81518723e476b28d764c5`  
		Size: 1.7 GB (1726924885 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5205e01a19ce3835a7f1caba14b71dbbcae05a77274c60358d9794ee0e2a3e65`  
		Last Modified: Wed, 10 Mar 2021 16:23:35 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4390a91a59ec3760f5740301d69b960d0f0b7fb212a8bc2201b27b93b24d4054`  
		Last Modified: Wed, 10 Mar 2021 17:02:23 GMT  
		Size: 1.3 KB (1305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdf068626801ee0e0c0bd2b1a1f9e05e2d16d27757653ade2a5cc0d971764f50`  
		Last Modified: Sat, 03 Apr 2021 01:22:47 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36e3dd9e9e868f213575a6d17e3fda275a2d47d15e2f9d13ad6d206a0f8567a7`  
		Last Modified: Sat, 03 Apr 2021 01:22:47 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:657647c528aa33d6da248e5aeeb7babe0f7976361e1654d5920cdb0b6c4848b9`  
		Last Modified: Sat, 03 Apr 2021 01:22:47 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:389f475c113034c3ad6f5619cf1bc1b11fdad81b5e5e009ba573539909b23423`  
		Last Modified: Sat, 03 Apr 2021 01:22:48 GMT  
		Size: 5.7 MB (5656062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd7a05da95e65b18383e1ae5b037f3b75a628a6af2949313789b364e70c3e7dc`  
		Last Modified: Sat, 03 Apr 2021 01:22:48 GMT  
		Size: 14.4 MB (14447531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55d02d4cabb443df53f1d6f7a6f93f8f9dda642d034916077f4fab20c5632675`  
		Last Modified: Sat, 03 Apr 2021 01:22:44 GMT  
		Size: 2.0 KB (1974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06b93a0d4c513ec838b27546bad996f092605e9c8399ad016f78b8b4cb96a900`  
		Last Modified: Sat, 03 Apr 2021 01:22:44 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8317ff85679d749fdf54c66f1b278c9f16aa11a116c5c0d288bc4f8debe41262`  
		Last Modified: Sat, 03 Apr 2021 01:22:44 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b8b1e736261cff8c3afa409fd73d85b78d6610a610e3b8eb3412798d3a18348`  
		Last Modified: Sat, 03 Apr 2021 01:22:44 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.2.1`

```console
$ docker pull nats@sha256:5958ba516eb8f221dc01b26d0afece5f9a48f7f0e978c889d19d1e788a02531e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.1817; amd64

### `nats:2.2.1` - linux; amd64

```console
$ docker pull nats@sha256:3bd24b6508d68c6d8835ecf42066a66f01b9e58d55c7a82d99eb3f1d9041fe15
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4208708 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f68fc0ca6306424854628406a234c7c5f76f2a13d658233ecefdb59a3de4ec89`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 03 Apr 2021 03:02:40 GMT
COPY file:494bfb1615387aa8aa24059641c501c246cffbb47653109c93d498a68ccce32a in /nats-server 
# Sat, 03 Apr 2021 03:02:41 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Sat, 03 Apr 2021 03:02:41 GMT
EXPOSE 4222 6222 8222
# Sat, 03 Apr 2021 03:02:41 GMT
ENTRYPOINT ["/nats-server"]
# Sat, 03 Apr 2021 03:02:41 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:832634cbfed021f934fff287987e6acb75f23228af46328d3f79d812b6462c57`  
		Last Modified: Sat, 03 Apr 2021 03:03:31 GMT  
		Size: 4.2 MB (4208232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91f381d2349aa770a85b4fde9e5c7794fe38c878aea8784f679b3f09728534a4`  
		Last Modified: Sat, 03 Apr 2021 03:03:30 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2.1` - linux; arm variant v6

```console
$ docker pull nats@sha256:0c1db0c5e32501c283742665116d2ae34168be99f1f0298a17fe6a1a0c3c9cb1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3882437 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dadccf67b2f681485255da8d75647104535e861fb3ee82f610f6d42281a07300`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 03 Apr 2021 01:02:37 GMT
COPY file:54bee7857c6b5cc9e3287e28fd1ffbbd529d72e791a1746d90d0b66346698246 in /nats-server 
# Sat, 03 Apr 2021 01:02:38 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Sat, 03 Apr 2021 01:02:38 GMT
EXPOSE 4222 6222 8222
# Sat, 03 Apr 2021 01:02:39 GMT
ENTRYPOINT ["/nats-server"]
# Sat, 03 Apr 2021 01:02:40 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:91cca6fbde65445d7c75ad5de8204fd8356fa76f2dd2983a53b2c0d9b7255bd9`  
		Last Modified: Sat, 03 Apr 2021 01:03:23 GMT  
		Size: 3.9 MB (3881961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b8d6f093021c26c95a4df34d728495a189d358902c6fed301d6bc06e93f4e85`  
		Last Modified: Sat, 03 Apr 2021 01:03:22 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2.1` - linux; arm variant v7

```console
$ docker pull nats@sha256:61dade57dcce93e1f3ea3e01779c4d2f1bf4ff21415290e42dfe72cba333f7d1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3877449 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64ad61fe367441505f4bdd49177124c6f6fbb5d9e212c6b871aec402ea6c4122`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 03 Apr 2021 01:45:33 GMT
COPY file:d95e297af0c7798d74c045b7143a48199a8e32ca5c5aa0b8d7c967a602bc1cfe in /nats-server 
# Sat, 03 Apr 2021 01:45:34 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Sat, 03 Apr 2021 01:45:35 GMT
EXPOSE 4222 6222 8222
# Sat, 03 Apr 2021 01:45:36 GMT
ENTRYPOINT ["/nats-server"]
# Sat, 03 Apr 2021 01:45:37 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:7919165d0b190df92f81ef4af9a0a2fef8a2da95dac86e567498a9364b0be069`  
		Last Modified: Sat, 03 Apr 2021 01:46:21 GMT  
		Size: 3.9 MB (3876974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdfa2b4e61cc1a65501d2feea740d0f932e2bf901c202226b24a7d787c0f4dff`  
		Last Modified: Sat, 03 Apr 2021 01:46:20 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2.1` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:13c34571ac946007679eb9333b30ca2fc5225ea3afdeb3ec3082bf4e5befe284
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3850749 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9d8fa2c7d5a8fb8a3e96f92707cd39a3107455acd96b42415d60cf31cae334d`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 03 Apr 2021 03:48:01 GMT
COPY file:4d714e3c520aa8a1f5935c65806500f01ea25ace84372fd7f3aa0a06f1f626c9 in /nats-server 
# Sat, 03 Apr 2021 03:48:02 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Sat, 03 Apr 2021 03:48:03 GMT
EXPOSE 4222 6222 8222
# Sat, 03 Apr 2021 03:48:04 GMT
ENTRYPOINT ["/nats-server"]
# Sat, 03 Apr 2021 03:48:05 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:310f293639061b27b8965c8683cf2bffb7d9b58bdb924635525fa7d990f2f3fb`  
		Last Modified: Sat, 03 Apr 2021 03:48:48 GMT  
		Size: 3.9 MB (3850270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e64370dd792941a18253408636a97ab34ef2f6ea706da1fe18ae7e008a3b13e`  
		Last Modified: Sat, 03 Apr 2021 03:48:47 GMT  
		Size: 479.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2.1` - windows version 10.0.17763.1817; amd64

```console
$ docker pull nats@sha256:7400f49e711ad398f8708d78498cb89250765f194fcad4bfb28b0811dddce228
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.7 MB (105658317 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d32a24884d574cc6457ee6540f906dc735846c9ed2cd1b15cb1b79c0f0df8fd`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 26 Feb 2021 16:47:31 GMT
RUN Apply image 1809-amd64
# Wed, 10 Mar 2021 16:56:55 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Sat, 03 Apr 2021 01:17:28 GMT
RUN cmd /S /C #(nop) COPY file:428a7e80db4313301a46326a9a79832e9cbe7d78c94e749b5c295e813e484f21 in C:\nats-server.exe 
# Sat, 03 Apr 2021 01:17:29 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Sat, 03 Apr 2021 01:17:30 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Sat, 03 Apr 2021 01:17:30 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Sat, 03 Apr 2021 01:17:32 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a11c4ca8f1ba16b6e1395d4523be2215bd0871c2e3e4695b9f2b87bd7472be52`  
		Size: 101.4 MB (101389964 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f49969195f32b7e40a81e3d189259fec7ebf52ee0ec5dafd5f3f288715354fed`  
		Last Modified: Wed, 10 Mar 2021 17:01:57 GMT  
		Size: 1.0 KB (1047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b78be9ec55bfa99633688cc4d73e47268a005880724f5c31af765df173fe522b`  
		Last Modified: Sat, 03 Apr 2021 01:22:27 GMT  
		Size: 4.3 MB (4262100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93286c3879edf77d449ceff1ed34a72becb3264fead3b488a3f05415c4bb62ec`  
		Last Modified: Sat, 03 Apr 2021 01:22:26 GMT  
		Size: 1.8 KB (1761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a913d40db4af4450743a872058165885095d790cda716fcd48634e3d7f4143f`  
		Last Modified: Sat, 03 Apr 2021 01:22:26 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67f64ab62ffafadee29cddb026c057f47c1d88836cf8c2e1da91189a1289fafd`  
		Last Modified: Sat, 03 Apr 2021 01:22:26 GMT  
		Size: 1.1 KB (1102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f1de1af4e095d547a9e171edf595e46d67d5687074985d261582ae4618438fb`  
		Last Modified: Sat, 03 Apr 2021 01:22:26 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.2.1-alpine`

```console
$ docker pull nats@sha256:786039ea5743e66f92097f4c98419cdb7755824388806faae9ca893626cda20f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.2.1-alpine` - linux; amd64

```console
$ docker pull nats@sha256:11a99e623a9df5677bdcbcff33bd032975aabdc9c226e00410997607a5398ad0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7303859 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f56ceabe89d18dd0b0c58d97b018484ed43d818791b7a1d9e5e8a09123c6cbd5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 31 Mar 2021 20:10:06 GMT
ADD file:7119167b56ff1228b2fb639c768955ce9db7a999cd947179240b216dfa5ccbb9 in / 
# Wed, 31 Mar 2021 20:10:06 GMT
CMD ["/bin/sh"]
# Sat, 03 Apr 2021 03:02:20 GMT
ENV NATS_SERVER=2.2.1
# Sat, 03 Apr 2021 03:02:23 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='0123d924907282265190258662edf8ad4351055083b5040e3bdf59117bd1c51c' ;; 		armhf) natsArch='arm6'; sha256='da719b07fd57137f85bfa6cffc7d00841a9c1fb4cdf7ca9a537bfc3f99b71f36' ;; 		armv7) natsArch='arm7'; sha256='cf6e8d9a9cc5d05f7320fb4be8fc9239cb87b91c6600a61ce7a2fb63e2f29f5a' ;; 		x86_64) natsArch='amd64'; sha256='70cb40d78b82ea6c0ca926c31ef98d2e1c885cfe2f73f34883e4ca448366c2dd' ;; 		x86) natsArch='386'; sha256='da54d129f8a52c048ded61e3b62e946037a9464d02cf818e568bbf1e385ce6be' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Sat, 03 Apr 2021 03:02:23 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Sat, 03 Apr 2021 03:02:24 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Sat, 03 Apr 2021 03:02:24 GMT
EXPOSE 4222 6222 8222
# Sat, 03 Apr 2021 03:02:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 03 Apr 2021 03:02:24 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:ca3cd42a7c9525f6ce3d64c1a70982613a8235f0cc057ec9244052921853ef15`  
		Last Modified: Wed, 31 Mar 2021 20:10:46 GMT  
		Size: 2.8 MB (2811947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0ab87484469466c6eeb084bcbe5538907a8cca9e02c6c00ffc4e03bd68d4563`  
		Last Modified: Sat, 03 Apr 2021 03:03:06 GMT  
		Size: 4.5 MB (4490943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63537464a64606bc6b408c793c1b726d40b4b1a540a829516859d3405c203e37`  
		Last Modified: Sat, 03 Apr 2021 03:03:05 GMT  
		Size: 557.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:843bbc65e4b41319d487b9ba5eb3a58b709e795448cc632d75fb8f54d76868d9`  
		Last Modified: Sat, 03 Apr 2021 03:03:05 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2.1-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:5980c4f84be539fd1b559624db6fa63ee409f825e4a93fa441598e93115d4b15
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6784924 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8f97d97f7e09aa5c9f936e0377789f200b06c8aabe846ce2591ebff76f7db8b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 31 Mar 2021 17:18:49 GMT
ADD file:988879d74f643b89539e5a0b6d74221621f19f4f87f722614addadc46ce47200 in / 
# Wed, 31 Mar 2021 17:18:50 GMT
CMD ["/bin/sh"]
# Sat, 03 Apr 2021 01:02:19 GMT
ENV NATS_SERVER=2.2.1
# Sat, 03 Apr 2021 01:02:24 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='0123d924907282265190258662edf8ad4351055083b5040e3bdf59117bd1c51c' ;; 		armhf) natsArch='arm6'; sha256='da719b07fd57137f85bfa6cffc7d00841a9c1fb4cdf7ca9a537bfc3f99b71f36' ;; 		armv7) natsArch='arm7'; sha256='cf6e8d9a9cc5d05f7320fb4be8fc9239cb87b91c6600a61ce7a2fb63e2f29f5a' ;; 		x86_64) natsArch='amd64'; sha256='70cb40d78b82ea6c0ca926c31ef98d2e1c885cfe2f73f34883e4ca448366c2dd' ;; 		x86) natsArch='386'; sha256='da54d129f8a52c048ded61e3b62e946037a9464d02cf818e568bbf1e385ce6be' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Sat, 03 Apr 2021 01:02:25 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Sat, 03 Apr 2021 01:02:26 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Sat, 03 Apr 2021 01:02:26 GMT
EXPOSE 4222 6222 8222
# Sat, 03 Apr 2021 01:02:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 03 Apr 2021 01:02:28 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:bb87125c6ee1ce30c6b33d2c96a9fbe46da4a290f7cb1dd73fd62d4e06503699`  
		Last Modified: Wed, 31 Mar 2021 17:19:55 GMT  
		Size: 2.6 MB (2622116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8d4b6ba6b297e822b0c0fe254f2d6b5afda81265eaf2481116af687cf66235c`  
		Last Modified: Sat, 03 Apr 2021 01:03:09 GMT  
		Size: 4.2 MB (4161834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ae0dfcf0132d6f11bd4762e4d1ec0b73f5ee36875a95dc78731673415f9de05`  
		Last Modified: Sat, 03 Apr 2021 01:03:07 GMT  
		Size: 561.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4f6ffd2be76e6334bd04318e19b02428d71b315b61ae8bb68ade8b07279ccff`  
		Last Modified: Sat, 03 Apr 2021 01:03:07 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2.1-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:8e048143304eabc1fad2f149b2761e661ebe261c60e0ecb4cd0f58818ca12090
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6583142 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:04ad730346110f756c4e29df7ebe6e02cb97db3770b8fdda258f5f4def7c2f88`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 31 Mar 2021 18:13:27 GMT
ADD file:56e92c06393237a87e0a1ff475e9c9dc80e897d69ec20f45359b587906da345b in / 
# Wed, 31 Mar 2021 18:13:31 GMT
CMD ["/bin/sh"]
# Sat, 03 Apr 2021 01:45:11 GMT
ENV NATS_SERVER=2.2.1
# Sat, 03 Apr 2021 01:45:16 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='0123d924907282265190258662edf8ad4351055083b5040e3bdf59117bd1c51c' ;; 		armhf) natsArch='arm6'; sha256='da719b07fd57137f85bfa6cffc7d00841a9c1fb4cdf7ca9a537bfc3f99b71f36' ;; 		armv7) natsArch='arm7'; sha256='cf6e8d9a9cc5d05f7320fb4be8fc9239cb87b91c6600a61ce7a2fb63e2f29f5a' ;; 		x86_64) natsArch='amd64'; sha256='70cb40d78b82ea6c0ca926c31ef98d2e1c885cfe2f73f34883e4ca448366c2dd' ;; 		x86) natsArch='386'; sha256='da54d129f8a52c048ded61e3b62e946037a9464d02cf818e568bbf1e385ce6be' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Sat, 03 Apr 2021 01:45:17 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Sat, 03 Apr 2021 01:45:18 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Sat, 03 Apr 2021 01:45:19 GMT
EXPOSE 4222 6222 8222
# Sat, 03 Apr 2021 01:45:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 03 Apr 2021 01:45:21 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:07389e51ea05e1c9a3cb0ef92d31181f2afa1e445207ad99ffd8a94d6d6af295`  
		Last Modified: Wed, 31 Mar 2021 18:14:57 GMT  
		Size: 2.4 MB (2424108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7331da30076f2eba452960efaf8df4620f03624062670e29e8e3fb97823756b3`  
		Last Modified: Sat, 03 Apr 2021 01:46:03 GMT  
		Size: 4.2 MB (4158064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abd26a9a6149ca00bb0a5e94ae858765a0b787564c99ea0ba4ec23d5cd7a8bd9`  
		Last Modified: Sat, 03 Apr 2021 01:46:02 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96a5a7410fa6228e048f75c6327720948ad9d6dd06db4b594d43165c1f6cab1c`  
		Last Modified: Sat, 03 Apr 2021 01:46:01 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2.1-alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:980841965bacdff61fc62145784092e89a8c0db1f125fccc5e9d240f60f94e93
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6844304 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99075b219d76c9593adb6b735cc906569e0124a6761312332407ee8de31e6382`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 31 Mar 2021 17:21:21 GMT
ADD file:3b16ffee2b26d8af5db152fcc582aaccd9e1ec9e3343874e9969a205550fe07d in / 
# Wed, 31 Mar 2021 17:21:23 GMT
CMD ["/bin/sh"]
# Sat, 03 Apr 2021 03:47:42 GMT
ENV NATS_SERVER=2.2.1
# Sat, 03 Apr 2021 03:47:46 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='0123d924907282265190258662edf8ad4351055083b5040e3bdf59117bd1c51c' ;; 		armhf) natsArch='arm6'; sha256='da719b07fd57137f85bfa6cffc7d00841a9c1fb4cdf7ca9a537bfc3f99b71f36' ;; 		armv7) natsArch='arm7'; sha256='cf6e8d9a9cc5d05f7320fb4be8fc9239cb87b91c6600a61ce7a2fb63e2f29f5a' ;; 		x86_64) natsArch='amd64'; sha256='70cb40d78b82ea6c0ca926c31ef98d2e1c885cfe2f73f34883e4ca448366c2dd' ;; 		x86) natsArch='386'; sha256='da54d129f8a52c048ded61e3b62e946037a9464d02cf818e568bbf1e385ce6be' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Sat, 03 Apr 2021 03:47:47 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Sat, 03 Apr 2021 03:47:48 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Sat, 03 Apr 2021 03:47:49 GMT
EXPOSE 4222 6222 8222
# Sat, 03 Apr 2021 03:47:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 03 Apr 2021 03:47:51 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:912815139b61c8926da31f7701f0a924e7964e3713052bf1a53193a4562157f6`  
		Last Modified: Wed, 31 Mar 2021 17:22:41 GMT  
		Size: 2.7 MB (2711920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9228d7a2d7ff547081c5c823de18c8fa62bb6200cee9f820f437c3004e90f309`  
		Last Modified: Sat, 03 Apr 2021 03:48:31 GMT  
		Size: 4.1 MB (4131414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ec0c89cac556aea8879a9beeefc7c2f8528b16539e3765c11de3c76e564e6f6`  
		Last Modified: Sat, 03 Apr 2021 03:48:30 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08fc29c470aa8216b46da0c00b30283b238b812f9d1395be3920045c367005af`  
		Last Modified: Sat, 03 Apr 2021 03:48:30 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.2.1-alpine3.13`

```console
$ docker pull nats@sha256:786039ea5743e66f92097f4c98419cdb7755824388806faae9ca893626cda20f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.2.1-alpine3.13` - linux; amd64

```console
$ docker pull nats@sha256:11a99e623a9df5677bdcbcff33bd032975aabdc9c226e00410997607a5398ad0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7303859 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f56ceabe89d18dd0b0c58d97b018484ed43d818791b7a1d9e5e8a09123c6cbd5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 31 Mar 2021 20:10:06 GMT
ADD file:7119167b56ff1228b2fb639c768955ce9db7a999cd947179240b216dfa5ccbb9 in / 
# Wed, 31 Mar 2021 20:10:06 GMT
CMD ["/bin/sh"]
# Sat, 03 Apr 2021 03:02:20 GMT
ENV NATS_SERVER=2.2.1
# Sat, 03 Apr 2021 03:02:23 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='0123d924907282265190258662edf8ad4351055083b5040e3bdf59117bd1c51c' ;; 		armhf) natsArch='arm6'; sha256='da719b07fd57137f85bfa6cffc7d00841a9c1fb4cdf7ca9a537bfc3f99b71f36' ;; 		armv7) natsArch='arm7'; sha256='cf6e8d9a9cc5d05f7320fb4be8fc9239cb87b91c6600a61ce7a2fb63e2f29f5a' ;; 		x86_64) natsArch='amd64'; sha256='70cb40d78b82ea6c0ca926c31ef98d2e1c885cfe2f73f34883e4ca448366c2dd' ;; 		x86) natsArch='386'; sha256='da54d129f8a52c048ded61e3b62e946037a9464d02cf818e568bbf1e385ce6be' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Sat, 03 Apr 2021 03:02:23 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Sat, 03 Apr 2021 03:02:24 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Sat, 03 Apr 2021 03:02:24 GMT
EXPOSE 4222 6222 8222
# Sat, 03 Apr 2021 03:02:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 03 Apr 2021 03:02:24 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:ca3cd42a7c9525f6ce3d64c1a70982613a8235f0cc057ec9244052921853ef15`  
		Last Modified: Wed, 31 Mar 2021 20:10:46 GMT  
		Size: 2.8 MB (2811947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0ab87484469466c6eeb084bcbe5538907a8cca9e02c6c00ffc4e03bd68d4563`  
		Last Modified: Sat, 03 Apr 2021 03:03:06 GMT  
		Size: 4.5 MB (4490943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63537464a64606bc6b408c793c1b726d40b4b1a540a829516859d3405c203e37`  
		Last Modified: Sat, 03 Apr 2021 03:03:05 GMT  
		Size: 557.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:843bbc65e4b41319d487b9ba5eb3a58b709e795448cc632d75fb8f54d76868d9`  
		Last Modified: Sat, 03 Apr 2021 03:03:05 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2.1-alpine3.13` - linux; arm variant v6

```console
$ docker pull nats@sha256:5980c4f84be539fd1b559624db6fa63ee409f825e4a93fa441598e93115d4b15
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6784924 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8f97d97f7e09aa5c9f936e0377789f200b06c8aabe846ce2591ebff76f7db8b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 31 Mar 2021 17:18:49 GMT
ADD file:988879d74f643b89539e5a0b6d74221621f19f4f87f722614addadc46ce47200 in / 
# Wed, 31 Mar 2021 17:18:50 GMT
CMD ["/bin/sh"]
# Sat, 03 Apr 2021 01:02:19 GMT
ENV NATS_SERVER=2.2.1
# Sat, 03 Apr 2021 01:02:24 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='0123d924907282265190258662edf8ad4351055083b5040e3bdf59117bd1c51c' ;; 		armhf) natsArch='arm6'; sha256='da719b07fd57137f85bfa6cffc7d00841a9c1fb4cdf7ca9a537bfc3f99b71f36' ;; 		armv7) natsArch='arm7'; sha256='cf6e8d9a9cc5d05f7320fb4be8fc9239cb87b91c6600a61ce7a2fb63e2f29f5a' ;; 		x86_64) natsArch='amd64'; sha256='70cb40d78b82ea6c0ca926c31ef98d2e1c885cfe2f73f34883e4ca448366c2dd' ;; 		x86) natsArch='386'; sha256='da54d129f8a52c048ded61e3b62e946037a9464d02cf818e568bbf1e385ce6be' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Sat, 03 Apr 2021 01:02:25 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Sat, 03 Apr 2021 01:02:26 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Sat, 03 Apr 2021 01:02:26 GMT
EXPOSE 4222 6222 8222
# Sat, 03 Apr 2021 01:02:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 03 Apr 2021 01:02:28 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:bb87125c6ee1ce30c6b33d2c96a9fbe46da4a290f7cb1dd73fd62d4e06503699`  
		Last Modified: Wed, 31 Mar 2021 17:19:55 GMT  
		Size: 2.6 MB (2622116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8d4b6ba6b297e822b0c0fe254f2d6b5afda81265eaf2481116af687cf66235c`  
		Last Modified: Sat, 03 Apr 2021 01:03:09 GMT  
		Size: 4.2 MB (4161834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ae0dfcf0132d6f11bd4762e4d1ec0b73f5ee36875a95dc78731673415f9de05`  
		Last Modified: Sat, 03 Apr 2021 01:03:07 GMT  
		Size: 561.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4f6ffd2be76e6334bd04318e19b02428d71b315b61ae8bb68ade8b07279ccff`  
		Last Modified: Sat, 03 Apr 2021 01:03:07 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2.1-alpine3.13` - linux; arm variant v7

```console
$ docker pull nats@sha256:8e048143304eabc1fad2f149b2761e661ebe261c60e0ecb4cd0f58818ca12090
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6583142 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:04ad730346110f756c4e29df7ebe6e02cb97db3770b8fdda258f5f4def7c2f88`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 31 Mar 2021 18:13:27 GMT
ADD file:56e92c06393237a87e0a1ff475e9c9dc80e897d69ec20f45359b587906da345b in / 
# Wed, 31 Mar 2021 18:13:31 GMT
CMD ["/bin/sh"]
# Sat, 03 Apr 2021 01:45:11 GMT
ENV NATS_SERVER=2.2.1
# Sat, 03 Apr 2021 01:45:16 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='0123d924907282265190258662edf8ad4351055083b5040e3bdf59117bd1c51c' ;; 		armhf) natsArch='arm6'; sha256='da719b07fd57137f85bfa6cffc7d00841a9c1fb4cdf7ca9a537bfc3f99b71f36' ;; 		armv7) natsArch='arm7'; sha256='cf6e8d9a9cc5d05f7320fb4be8fc9239cb87b91c6600a61ce7a2fb63e2f29f5a' ;; 		x86_64) natsArch='amd64'; sha256='70cb40d78b82ea6c0ca926c31ef98d2e1c885cfe2f73f34883e4ca448366c2dd' ;; 		x86) natsArch='386'; sha256='da54d129f8a52c048ded61e3b62e946037a9464d02cf818e568bbf1e385ce6be' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Sat, 03 Apr 2021 01:45:17 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Sat, 03 Apr 2021 01:45:18 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Sat, 03 Apr 2021 01:45:19 GMT
EXPOSE 4222 6222 8222
# Sat, 03 Apr 2021 01:45:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 03 Apr 2021 01:45:21 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:07389e51ea05e1c9a3cb0ef92d31181f2afa1e445207ad99ffd8a94d6d6af295`  
		Last Modified: Wed, 31 Mar 2021 18:14:57 GMT  
		Size: 2.4 MB (2424108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7331da30076f2eba452960efaf8df4620f03624062670e29e8e3fb97823756b3`  
		Last Modified: Sat, 03 Apr 2021 01:46:03 GMT  
		Size: 4.2 MB (4158064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abd26a9a6149ca00bb0a5e94ae858765a0b787564c99ea0ba4ec23d5cd7a8bd9`  
		Last Modified: Sat, 03 Apr 2021 01:46:02 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96a5a7410fa6228e048f75c6327720948ad9d6dd06db4b594d43165c1f6cab1c`  
		Last Modified: Sat, 03 Apr 2021 01:46:01 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2.1-alpine3.13` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:980841965bacdff61fc62145784092e89a8c0db1f125fccc5e9d240f60f94e93
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6844304 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99075b219d76c9593adb6b735cc906569e0124a6761312332407ee8de31e6382`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 31 Mar 2021 17:21:21 GMT
ADD file:3b16ffee2b26d8af5db152fcc582aaccd9e1ec9e3343874e9969a205550fe07d in / 
# Wed, 31 Mar 2021 17:21:23 GMT
CMD ["/bin/sh"]
# Sat, 03 Apr 2021 03:47:42 GMT
ENV NATS_SERVER=2.2.1
# Sat, 03 Apr 2021 03:47:46 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='0123d924907282265190258662edf8ad4351055083b5040e3bdf59117bd1c51c' ;; 		armhf) natsArch='arm6'; sha256='da719b07fd57137f85bfa6cffc7d00841a9c1fb4cdf7ca9a537bfc3f99b71f36' ;; 		armv7) natsArch='arm7'; sha256='cf6e8d9a9cc5d05f7320fb4be8fc9239cb87b91c6600a61ce7a2fb63e2f29f5a' ;; 		x86_64) natsArch='amd64'; sha256='70cb40d78b82ea6c0ca926c31ef98d2e1c885cfe2f73f34883e4ca448366c2dd' ;; 		x86) natsArch='386'; sha256='da54d129f8a52c048ded61e3b62e946037a9464d02cf818e568bbf1e385ce6be' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Sat, 03 Apr 2021 03:47:47 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Sat, 03 Apr 2021 03:47:48 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Sat, 03 Apr 2021 03:47:49 GMT
EXPOSE 4222 6222 8222
# Sat, 03 Apr 2021 03:47:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 03 Apr 2021 03:47:51 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:912815139b61c8926da31f7701f0a924e7964e3713052bf1a53193a4562157f6`  
		Last Modified: Wed, 31 Mar 2021 17:22:41 GMT  
		Size: 2.7 MB (2711920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9228d7a2d7ff547081c5c823de18c8fa62bb6200cee9f820f437c3004e90f309`  
		Last Modified: Sat, 03 Apr 2021 03:48:31 GMT  
		Size: 4.1 MB (4131414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ec0c89cac556aea8879a9beeefc7c2f8528b16539e3765c11de3c76e564e6f6`  
		Last Modified: Sat, 03 Apr 2021 03:48:30 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08fc29c470aa8216b46da0c00b30283b238b812f9d1395be3920045c367005af`  
		Last Modified: Sat, 03 Apr 2021 03:48:30 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.2.1-linux`

```console
$ docker pull nats@sha256:f116a903fd14977153dc2ae74e3b0437762ee2a6c7858807246d6501b2a9af54
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.2.1-linux` - linux; amd64

```console
$ docker pull nats@sha256:3bd24b6508d68c6d8835ecf42066a66f01b9e58d55c7a82d99eb3f1d9041fe15
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4208708 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f68fc0ca6306424854628406a234c7c5f76f2a13d658233ecefdb59a3de4ec89`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 03 Apr 2021 03:02:40 GMT
COPY file:494bfb1615387aa8aa24059641c501c246cffbb47653109c93d498a68ccce32a in /nats-server 
# Sat, 03 Apr 2021 03:02:41 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Sat, 03 Apr 2021 03:02:41 GMT
EXPOSE 4222 6222 8222
# Sat, 03 Apr 2021 03:02:41 GMT
ENTRYPOINT ["/nats-server"]
# Sat, 03 Apr 2021 03:02:41 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:832634cbfed021f934fff287987e6acb75f23228af46328d3f79d812b6462c57`  
		Last Modified: Sat, 03 Apr 2021 03:03:31 GMT  
		Size: 4.2 MB (4208232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91f381d2349aa770a85b4fde9e5c7794fe38c878aea8784f679b3f09728534a4`  
		Last Modified: Sat, 03 Apr 2021 03:03:30 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2.1-linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:0c1db0c5e32501c283742665116d2ae34168be99f1f0298a17fe6a1a0c3c9cb1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3882437 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dadccf67b2f681485255da8d75647104535e861fb3ee82f610f6d42281a07300`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 03 Apr 2021 01:02:37 GMT
COPY file:54bee7857c6b5cc9e3287e28fd1ffbbd529d72e791a1746d90d0b66346698246 in /nats-server 
# Sat, 03 Apr 2021 01:02:38 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Sat, 03 Apr 2021 01:02:38 GMT
EXPOSE 4222 6222 8222
# Sat, 03 Apr 2021 01:02:39 GMT
ENTRYPOINT ["/nats-server"]
# Sat, 03 Apr 2021 01:02:40 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:91cca6fbde65445d7c75ad5de8204fd8356fa76f2dd2983a53b2c0d9b7255bd9`  
		Last Modified: Sat, 03 Apr 2021 01:03:23 GMT  
		Size: 3.9 MB (3881961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b8d6f093021c26c95a4df34d728495a189d358902c6fed301d6bc06e93f4e85`  
		Last Modified: Sat, 03 Apr 2021 01:03:22 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2.1-linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:61dade57dcce93e1f3ea3e01779c4d2f1bf4ff21415290e42dfe72cba333f7d1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3877449 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64ad61fe367441505f4bdd49177124c6f6fbb5d9e212c6b871aec402ea6c4122`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 03 Apr 2021 01:45:33 GMT
COPY file:d95e297af0c7798d74c045b7143a48199a8e32ca5c5aa0b8d7c967a602bc1cfe in /nats-server 
# Sat, 03 Apr 2021 01:45:34 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Sat, 03 Apr 2021 01:45:35 GMT
EXPOSE 4222 6222 8222
# Sat, 03 Apr 2021 01:45:36 GMT
ENTRYPOINT ["/nats-server"]
# Sat, 03 Apr 2021 01:45:37 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:7919165d0b190df92f81ef4af9a0a2fef8a2da95dac86e567498a9364b0be069`  
		Last Modified: Sat, 03 Apr 2021 01:46:21 GMT  
		Size: 3.9 MB (3876974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdfa2b4e61cc1a65501d2feea740d0f932e2bf901c202226b24a7d787c0f4dff`  
		Last Modified: Sat, 03 Apr 2021 01:46:20 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2.1-linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:13c34571ac946007679eb9333b30ca2fc5225ea3afdeb3ec3082bf4e5befe284
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3850749 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9d8fa2c7d5a8fb8a3e96f92707cd39a3107455acd96b42415d60cf31cae334d`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 03 Apr 2021 03:48:01 GMT
COPY file:4d714e3c520aa8a1f5935c65806500f01ea25ace84372fd7f3aa0a06f1f626c9 in /nats-server 
# Sat, 03 Apr 2021 03:48:02 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Sat, 03 Apr 2021 03:48:03 GMT
EXPOSE 4222 6222 8222
# Sat, 03 Apr 2021 03:48:04 GMT
ENTRYPOINT ["/nats-server"]
# Sat, 03 Apr 2021 03:48:05 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:310f293639061b27b8965c8683cf2bffb7d9b58bdb924635525fa7d990f2f3fb`  
		Last Modified: Sat, 03 Apr 2021 03:48:48 GMT  
		Size: 3.9 MB (3850270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e64370dd792941a18253408636a97ab34ef2f6ea706da1fe18ae7e008a3b13e`  
		Last Modified: Sat, 03 Apr 2021 03:48:47 GMT  
		Size: 479.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.2.1-nanoserver`

```console
$ docker pull nats@sha256:795115a3a3b1b5f4cbc7c017ddd52f46848199b694cff7aafbcb0c7d464925e5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1817; amd64

### `nats:2.2.1-nanoserver` - windows version 10.0.17763.1817; amd64

```console
$ docker pull nats@sha256:7400f49e711ad398f8708d78498cb89250765f194fcad4bfb28b0811dddce228
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.7 MB (105658317 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d32a24884d574cc6457ee6540f906dc735846c9ed2cd1b15cb1b79c0f0df8fd`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 26 Feb 2021 16:47:31 GMT
RUN Apply image 1809-amd64
# Wed, 10 Mar 2021 16:56:55 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Sat, 03 Apr 2021 01:17:28 GMT
RUN cmd /S /C #(nop) COPY file:428a7e80db4313301a46326a9a79832e9cbe7d78c94e749b5c295e813e484f21 in C:\nats-server.exe 
# Sat, 03 Apr 2021 01:17:29 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Sat, 03 Apr 2021 01:17:30 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Sat, 03 Apr 2021 01:17:30 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Sat, 03 Apr 2021 01:17:32 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a11c4ca8f1ba16b6e1395d4523be2215bd0871c2e3e4695b9f2b87bd7472be52`  
		Size: 101.4 MB (101389964 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f49969195f32b7e40a81e3d189259fec7ebf52ee0ec5dafd5f3f288715354fed`  
		Last Modified: Wed, 10 Mar 2021 17:01:57 GMT  
		Size: 1.0 KB (1047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b78be9ec55bfa99633688cc4d73e47268a005880724f5c31af765df173fe522b`  
		Last Modified: Sat, 03 Apr 2021 01:22:27 GMT  
		Size: 4.3 MB (4262100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93286c3879edf77d449ceff1ed34a72becb3264fead3b488a3f05415c4bb62ec`  
		Last Modified: Sat, 03 Apr 2021 01:22:26 GMT  
		Size: 1.8 KB (1761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a913d40db4af4450743a872058165885095d790cda716fcd48634e3d7f4143f`  
		Last Modified: Sat, 03 Apr 2021 01:22:26 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67f64ab62ffafadee29cddb026c057f47c1d88836cf8c2e1da91189a1289fafd`  
		Last Modified: Sat, 03 Apr 2021 01:22:26 GMT  
		Size: 1.1 KB (1102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f1de1af4e095d547a9e171edf595e46d67d5687074985d261582ae4618438fb`  
		Last Modified: Sat, 03 Apr 2021 01:22:26 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.2.1-nanoserver-1809`

```console
$ docker pull nats@sha256:795115a3a3b1b5f4cbc7c017ddd52f46848199b694cff7aafbcb0c7d464925e5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1817; amd64

### `nats:2.2.1-nanoserver-1809` - windows version 10.0.17763.1817; amd64

```console
$ docker pull nats@sha256:7400f49e711ad398f8708d78498cb89250765f194fcad4bfb28b0811dddce228
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.7 MB (105658317 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d32a24884d574cc6457ee6540f906dc735846c9ed2cd1b15cb1b79c0f0df8fd`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 26 Feb 2021 16:47:31 GMT
RUN Apply image 1809-amd64
# Wed, 10 Mar 2021 16:56:55 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Sat, 03 Apr 2021 01:17:28 GMT
RUN cmd /S /C #(nop) COPY file:428a7e80db4313301a46326a9a79832e9cbe7d78c94e749b5c295e813e484f21 in C:\nats-server.exe 
# Sat, 03 Apr 2021 01:17:29 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Sat, 03 Apr 2021 01:17:30 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Sat, 03 Apr 2021 01:17:30 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Sat, 03 Apr 2021 01:17:32 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a11c4ca8f1ba16b6e1395d4523be2215bd0871c2e3e4695b9f2b87bd7472be52`  
		Size: 101.4 MB (101389964 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f49969195f32b7e40a81e3d189259fec7ebf52ee0ec5dafd5f3f288715354fed`  
		Last Modified: Wed, 10 Mar 2021 17:01:57 GMT  
		Size: 1.0 KB (1047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b78be9ec55bfa99633688cc4d73e47268a005880724f5c31af765df173fe522b`  
		Last Modified: Sat, 03 Apr 2021 01:22:27 GMT  
		Size: 4.3 MB (4262100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93286c3879edf77d449ceff1ed34a72becb3264fead3b488a3f05415c4bb62ec`  
		Last Modified: Sat, 03 Apr 2021 01:22:26 GMT  
		Size: 1.8 KB (1761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a913d40db4af4450743a872058165885095d790cda716fcd48634e3d7f4143f`  
		Last Modified: Sat, 03 Apr 2021 01:22:26 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67f64ab62ffafadee29cddb026c057f47c1d88836cf8c2e1da91189a1289fafd`  
		Last Modified: Sat, 03 Apr 2021 01:22:26 GMT  
		Size: 1.1 KB (1102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f1de1af4e095d547a9e171edf595e46d67d5687074985d261582ae4618438fb`  
		Last Modified: Sat, 03 Apr 2021 01:22:26 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.2.1-scratch`

```console
$ docker pull nats@sha256:f116a903fd14977153dc2ae74e3b0437762ee2a6c7858807246d6501b2a9af54
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.2.1-scratch` - linux; amd64

```console
$ docker pull nats@sha256:3bd24b6508d68c6d8835ecf42066a66f01b9e58d55c7a82d99eb3f1d9041fe15
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4208708 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f68fc0ca6306424854628406a234c7c5f76f2a13d658233ecefdb59a3de4ec89`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 03 Apr 2021 03:02:40 GMT
COPY file:494bfb1615387aa8aa24059641c501c246cffbb47653109c93d498a68ccce32a in /nats-server 
# Sat, 03 Apr 2021 03:02:41 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Sat, 03 Apr 2021 03:02:41 GMT
EXPOSE 4222 6222 8222
# Sat, 03 Apr 2021 03:02:41 GMT
ENTRYPOINT ["/nats-server"]
# Sat, 03 Apr 2021 03:02:41 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:832634cbfed021f934fff287987e6acb75f23228af46328d3f79d812b6462c57`  
		Last Modified: Sat, 03 Apr 2021 03:03:31 GMT  
		Size: 4.2 MB (4208232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91f381d2349aa770a85b4fde9e5c7794fe38c878aea8784f679b3f09728534a4`  
		Last Modified: Sat, 03 Apr 2021 03:03:30 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2.1-scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:0c1db0c5e32501c283742665116d2ae34168be99f1f0298a17fe6a1a0c3c9cb1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3882437 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dadccf67b2f681485255da8d75647104535e861fb3ee82f610f6d42281a07300`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 03 Apr 2021 01:02:37 GMT
COPY file:54bee7857c6b5cc9e3287e28fd1ffbbd529d72e791a1746d90d0b66346698246 in /nats-server 
# Sat, 03 Apr 2021 01:02:38 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Sat, 03 Apr 2021 01:02:38 GMT
EXPOSE 4222 6222 8222
# Sat, 03 Apr 2021 01:02:39 GMT
ENTRYPOINT ["/nats-server"]
# Sat, 03 Apr 2021 01:02:40 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:91cca6fbde65445d7c75ad5de8204fd8356fa76f2dd2983a53b2c0d9b7255bd9`  
		Last Modified: Sat, 03 Apr 2021 01:03:23 GMT  
		Size: 3.9 MB (3881961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b8d6f093021c26c95a4df34d728495a189d358902c6fed301d6bc06e93f4e85`  
		Last Modified: Sat, 03 Apr 2021 01:03:22 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2.1-scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:61dade57dcce93e1f3ea3e01779c4d2f1bf4ff21415290e42dfe72cba333f7d1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3877449 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64ad61fe367441505f4bdd49177124c6f6fbb5d9e212c6b871aec402ea6c4122`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 03 Apr 2021 01:45:33 GMT
COPY file:d95e297af0c7798d74c045b7143a48199a8e32ca5c5aa0b8d7c967a602bc1cfe in /nats-server 
# Sat, 03 Apr 2021 01:45:34 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Sat, 03 Apr 2021 01:45:35 GMT
EXPOSE 4222 6222 8222
# Sat, 03 Apr 2021 01:45:36 GMT
ENTRYPOINT ["/nats-server"]
# Sat, 03 Apr 2021 01:45:37 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:7919165d0b190df92f81ef4af9a0a2fef8a2da95dac86e567498a9364b0be069`  
		Last Modified: Sat, 03 Apr 2021 01:46:21 GMT  
		Size: 3.9 MB (3876974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdfa2b4e61cc1a65501d2feea740d0f932e2bf901c202226b24a7d787c0f4dff`  
		Last Modified: Sat, 03 Apr 2021 01:46:20 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2.1-scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:13c34571ac946007679eb9333b30ca2fc5225ea3afdeb3ec3082bf4e5befe284
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3850749 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9d8fa2c7d5a8fb8a3e96f92707cd39a3107455acd96b42415d60cf31cae334d`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 03 Apr 2021 03:48:01 GMT
COPY file:4d714e3c520aa8a1f5935c65806500f01ea25ace84372fd7f3aa0a06f1f626c9 in /nats-server 
# Sat, 03 Apr 2021 03:48:02 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Sat, 03 Apr 2021 03:48:03 GMT
EXPOSE 4222 6222 8222
# Sat, 03 Apr 2021 03:48:04 GMT
ENTRYPOINT ["/nats-server"]
# Sat, 03 Apr 2021 03:48:05 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:310f293639061b27b8965c8683cf2bffb7d9b58bdb924635525fa7d990f2f3fb`  
		Last Modified: Sat, 03 Apr 2021 03:48:48 GMT  
		Size: 3.9 MB (3850270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e64370dd792941a18253408636a97ab34ef2f6ea706da1fe18ae7e008a3b13e`  
		Last Modified: Sat, 03 Apr 2021 03:48:47 GMT  
		Size: 479.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.2.1-windowsservercore`

```console
$ docker pull nats@sha256:91810bbcbf606b0cf379000443d302c7b5d928cc7309c63da19917ca3ff0525f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1817; amd64
	-	windows version 10.0.14393.4283; amd64

### `nats:2.2.1-windowsservercore` - windows version 10.0.17763.1817; amd64

```console
$ docker pull nats@sha256:79eefa8948e2758f0659fb934899c37b05b67eb96c38b0e8c67c1a0974992423
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2480294595 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3875d7d95dfdb0356da902eee6142a19a85e38ae7ddde3bbf34b06e18765ecd7`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 27 Feb 2021 09:32:06 GMT
RUN Install update 1809-amd64
# Wed, 10 Mar 2021 14:15:30 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Mar 2021 16:54:55 GMT
ENV NATS_DOCKERIZED=1
# Sat, 03 Apr 2021 01:15:14 GMT
ENV NATS_SERVER=2.2.1
# Sat, 03 Apr 2021 01:15:16 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.2.1/nats-server-v2.2.1-windows-amd64.zip
# Sat, 03 Apr 2021 01:15:17 GMT
ENV GIT_DOWNLOAD_SHA256=1f0d48a7ba9200e2572016a9f3e1ec7e630f0518cc0b40950c14ff3a5d900924
# Sat, 03 Apr 2021 01:15:50 GMT
RUN Set-PSDebug -Trace 2
# Sat, 03 Apr 2021 01:17:04 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Sat, 03 Apr 2021 01:17:06 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Sat, 03 Apr 2021 01:17:07 GMT
EXPOSE 4222 6222 8222
# Sat, 03 Apr 2021 01:17:08 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Sat, 03 Apr 2021 01:17:09 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5ff1512f88ecd4ff0a91ade34d43733c48834433e35f062f80e6e70d706f8d73`  
		Size: 743.2 MB (743201590 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:31ae1fcdffac4071930a0d98172fc515a43c93aa55870e4b6cc8c789b9444e73`  
		Last Modified: Wed, 10 Mar 2021 16:22:41 GMT  
		Size: 1.3 KB (1305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cfde5dabd6353190a5343286e79ed9ad72f47f48ca9197e594b9771b5039e7d`  
		Last Modified: Wed, 10 Mar 2021 17:01:37 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4eb0ea2b178ae862896fca7bda0c5c677fd82870ca007ebe695e42f058831af`  
		Last Modified: Sat, 03 Apr 2021 01:22:03 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8c9d68c9aa9d29abd0c09f2016e9fcfc53bd185a7403989cec09108f661a977`  
		Last Modified: Sat, 03 Apr 2021 01:22:03 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b05ed1fd68964dcfc103f5452b7ee8528749d538e395dd36d17158cab031fdf`  
		Last Modified: Sat, 03 Apr 2021 01:22:03 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3994ed7efdb8fb7c71541583ff656c6c8e54e722284ec414d3ef00145cb43efa`  
		Last Modified: Sat, 03 Apr 2021 01:22:09 GMT  
		Size: 5.1 MB (5064967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0c3e4f395cd1bacff8cb6c6a451cfe4d56b4a054cfc15dd1a8b04a9e56240fa`  
		Last Modified: Sat, 03 Apr 2021 01:22:03 GMT  
		Size: 13.7 MB (13681925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bc88971a96126558018ca2f17f084db054369de555c8cb84a508c7a1394236e`  
		Last Modified: Sat, 03 Apr 2021 01:22:00 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66fa36b1a5dd3f83c94c4e1597659532cb557cd8f9cd414bb81f1049f39924af`  
		Last Modified: Sat, 03 Apr 2021 01:22:00 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4147b1dd2e59f8f133ab83ace94bf75ef78c0f9f261d49d65b7cc0b84d49438e`  
		Last Modified: Sat, 03 Apr 2021 01:22:00 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49b9455ff088b797d1cff54432e7f275092555cd8485bbf6b4aa926b88077f94`  
		Last Modified: Sat, 03 Apr 2021 01:22:00 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2.1-windowsservercore` - windows version 10.0.14393.4283; amd64

```console
$ docker pull nats@sha256:ea694b06746523df91b7d824d0fc9030b282cc666bf34e937103b72b280d8a09
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5817027558 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:265f2ee0b7a998cc6ce663873648377be2b81226575d11ed5d1537b35a4118bf`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 03 Mar 2021 18:02:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Mar 2021 14:25:01 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Mar 2021 16:57:09 GMT
ENV NATS_DOCKERIZED=1
# Sat, 03 Apr 2021 01:17:41 GMT
ENV NATS_SERVER=2.2.1
# Sat, 03 Apr 2021 01:17:42 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.2.1/nats-server-v2.2.1-windows-amd64.zip
# Sat, 03 Apr 2021 01:17:43 GMT
ENV GIT_DOWNLOAD_SHA256=1f0d48a7ba9200e2572016a9f3e1ec7e630f0518cc0b40950c14ff3a5d900924
# Sat, 03 Apr 2021 01:19:05 GMT
RUN Set-PSDebug -Trace 2
# Sat, 03 Apr 2021 01:21:10 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Sat, 03 Apr 2021 01:21:11 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Sat, 03 Apr 2021 01:21:12 GMT
EXPOSE 4222 6222 8222
# Sat, 03 Apr 2021 01:21:13 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Sat, 03 Apr 2021 01:21:14 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:30bda99601c5cbd3b2118409f401852ea648e2319bd81518723e476b28d764c5`  
		Size: 1.7 GB (1726924885 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5205e01a19ce3835a7f1caba14b71dbbcae05a77274c60358d9794ee0e2a3e65`  
		Last Modified: Wed, 10 Mar 2021 16:23:35 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4390a91a59ec3760f5740301d69b960d0f0b7fb212a8bc2201b27b93b24d4054`  
		Last Modified: Wed, 10 Mar 2021 17:02:23 GMT  
		Size: 1.3 KB (1305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdf068626801ee0e0c0bd2b1a1f9e05e2d16d27757653ade2a5cc0d971764f50`  
		Last Modified: Sat, 03 Apr 2021 01:22:47 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36e3dd9e9e868f213575a6d17e3fda275a2d47d15e2f9d13ad6d206a0f8567a7`  
		Last Modified: Sat, 03 Apr 2021 01:22:47 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:657647c528aa33d6da248e5aeeb7babe0f7976361e1654d5920cdb0b6c4848b9`  
		Last Modified: Sat, 03 Apr 2021 01:22:47 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:389f475c113034c3ad6f5619cf1bc1b11fdad81b5e5e009ba573539909b23423`  
		Last Modified: Sat, 03 Apr 2021 01:22:48 GMT  
		Size: 5.7 MB (5656062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd7a05da95e65b18383e1ae5b037f3b75a628a6af2949313789b364e70c3e7dc`  
		Last Modified: Sat, 03 Apr 2021 01:22:48 GMT  
		Size: 14.4 MB (14447531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55d02d4cabb443df53f1d6f7a6f93f8f9dda642d034916077f4fab20c5632675`  
		Last Modified: Sat, 03 Apr 2021 01:22:44 GMT  
		Size: 2.0 KB (1974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06b93a0d4c513ec838b27546bad996f092605e9c8399ad016f78b8b4cb96a900`  
		Last Modified: Sat, 03 Apr 2021 01:22:44 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8317ff85679d749fdf54c66f1b278c9f16aa11a116c5c0d288bc4f8debe41262`  
		Last Modified: Sat, 03 Apr 2021 01:22:44 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b8b1e736261cff8c3afa409fd73d85b78d6610a610e3b8eb3412798d3a18348`  
		Last Modified: Sat, 03 Apr 2021 01:22:44 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.2.1-windowsservercore-1809`

```console
$ docker pull nats@sha256:f8a4f8888f531755c5711af4f90423afca2a36de1890ddd11b74df0dad4bd18c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1817; amd64

### `nats:2.2.1-windowsservercore-1809` - windows version 10.0.17763.1817; amd64

```console
$ docker pull nats@sha256:79eefa8948e2758f0659fb934899c37b05b67eb96c38b0e8c67c1a0974992423
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2480294595 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3875d7d95dfdb0356da902eee6142a19a85e38ae7ddde3bbf34b06e18765ecd7`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 27 Feb 2021 09:32:06 GMT
RUN Install update 1809-amd64
# Wed, 10 Mar 2021 14:15:30 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Mar 2021 16:54:55 GMT
ENV NATS_DOCKERIZED=1
# Sat, 03 Apr 2021 01:15:14 GMT
ENV NATS_SERVER=2.2.1
# Sat, 03 Apr 2021 01:15:16 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.2.1/nats-server-v2.2.1-windows-amd64.zip
# Sat, 03 Apr 2021 01:15:17 GMT
ENV GIT_DOWNLOAD_SHA256=1f0d48a7ba9200e2572016a9f3e1ec7e630f0518cc0b40950c14ff3a5d900924
# Sat, 03 Apr 2021 01:15:50 GMT
RUN Set-PSDebug -Trace 2
# Sat, 03 Apr 2021 01:17:04 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Sat, 03 Apr 2021 01:17:06 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Sat, 03 Apr 2021 01:17:07 GMT
EXPOSE 4222 6222 8222
# Sat, 03 Apr 2021 01:17:08 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Sat, 03 Apr 2021 01:17:09 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5ff1512f88ecd4ff0a91ade34d43733c48834433e35f062f80e6e70d706f8d73`  
		Size: 743.2 MB (743201590 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:31ae1fcdffac4071930a0d98172fc515a43c93aa55870e4b6cc8c789b9444e73`  
		Last Modified: Wed, 10 Mar 2021 16:22:41 GMT  
		Size: 1.3 KB (1305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cfde5dabd6353190a5343286e79ed9ad72f47f48ca9197e594b9771b5039e7d`  
		Last Modified: Wed, 10 Mar 2021 17:01:37 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4eb0ea2b178ae862896fca7bda0c5c677fd82870ca007ebe695e42f058831af`  
		Last Modified: Sat, 03 Apr 2021 01:22:03 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8c9d68c9aa9d29abd0c09f2016e9fcfc53bd185a7403989cec09108f661a977`  
		Last Modified: Sat, 03 Apr 2021 01:22:03 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b05ed1fd68964dcfc103f5452b7ee8528749d538e395dd36d17158cab031fdf`  
		Last Modified: Sat, 03 Apr 2021 01:22:03 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3994ed7efdb8fb7c71541583ff656c6c8e54e722284ec414d3ef00145cb43efa`  
		Last Modified: Sat, 03 Apr 2021 01:22:09 GMT  
		Size: 5.1 MB (5064967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0c3e4f395cd1bacff8cb6c6a451cfe4d56b4a054cfc15dd1a8b04a9e56240fa`  
		Last Modified: Sat, 03 Apr 2021 01:22:03 GMT  
		Size: 13.7 MB (13681925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bc88971a96126558018ca2f17f084db054369de555c8cb84a508c7a1394236e`  
		Last Modified: Sat, 03 Apr 2021 01:22:00 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66fa36b1a5dd3f83c94c4e1597659532cb557cd8f9cd414bb81f1049f39924af`  
		Last Modified: Sat, 03 Apr 2021 01:22:00 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4147b1dd2e59f8f133ab83ace94bf75ef78c0f9f261d49d65b7cc0b84d49438e`  
		Last Modified: Sat, 03 Apr 2021 01:22:00 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49b9455ff088b797d1cff54432e7f275092555cd8485bbf6b4aa926b88077f94`  
		Last Modified: Sat, 03 Apr 2021 01:22:00 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.2.1-windowsservercore-ltsc2016`

```console
$ docker pull nats@sha256:a29981e9b9b26371bed2856c6ac2b18e78e0ec9db3aeb251d0d8b281501c7196
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4283; amd64

### `nats:2.2.1-windowsservercore-ltsc2016` - windows version 10.0.14393.4283; amd64

```console
$ docker pull nats@sha256:ea694b06746523df91b7d824d0fc9030b282cc666bf34e937103b72b280d8a09
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5817027558 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:265f2ee0b7a998cc6ce663873648377be2b81226575d11ed5d1537b35a4118bf`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 03 Mar 2021 18:02:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Mar 2021 14:25:01 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Mar 2021 16:57:09 GMT
ENV NATS_DOCKERIZED=1
# Sat, 03 Apr 2021 01:17:41 GMT
ENV NATS_SERVER=2.2.1
# Sat, 03 Apr 2021 01:17:42 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.2.1/nats-server-v2.2.1-windows-amd64.zip
# Sat, 03 Apr 2021 01:17:43 GMT
ENV GIT_DOWNLOAD_SHA256=1f0d48a7ba9200e2572016a9f3e1ec7e630f0518cc0b40950c14ff3a5d900924
# Sat, 03 Apr 2021 01:19:05 GMT
RUN Set-PSDebug -Trace 2
# Sat, 03 Apr 2021 01:21:10 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Sat, 03 Apr 2021 01:21:11 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Sat, 03 Apr 2021 01:21:12 GMT
EXPOSE 4222 6222 8222
# Sat, 03 Apr 2021 01:21:13 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Sat, 03 Apr 2021 01:21:14 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:30bda99601c5cbd3b2118409f401852ea648e2319bd81518723e476b28d764c5`  
		Size: 1.7 GB (1726924885 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5205e01a19ce3835a7f1caba14b71dbbcae05a77274c60358d9794ee0e2a3e65`  
		Last Modified: Wed, 10 Mar 2021 16:23:35 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4390a91a59ec3760f5740301d69b960d0f0b7fb212a8bc2201b27b93b24d4054`  
		Last Modified: Wed, 10 Mar 2021 17:02:23 GMT  
		Size: 1.3 KB (1305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdf068626801ee0e0c0bd2b1a1f9e05e2d16d27757653ade2a5cc0d971764f50`  
		Last Modified: Sat, 03 Apr 2021 01:22:47 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36e3dd9e9e868f213575a6d17e3fda275a2d47d15e2f9d13ad6d206a0f8567a7`  
		Last Modified: Sat, 03 Apr 2021 01:22:47 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:657647c528aa33d6da248e5aeeb7babe0f7976361e1654d5920cdb0b6c4848b9`  
		Last Modified: Sat, 03 Apr 2021 01:22:47 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:389f475c113034c3ad6f5619cf1bc1b11fdad81b5e5e009ba573539909b23423`  
		Last Modified: Sat, 03 Apr 2021 01:22:48 GMT  
		Size: 5.7 MB (5656062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd7a05da95e65b18383e1ae5b037f3b75a628a6af2949313789b364e70c3e7dc`  
		Last Modified: Sat, 03 Apr 2021 01:22:48 GMT  
		Size: 14.4 MB (14447531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55d02d4cabb443df53f1d6f7a6f93f8f9dda642d034916077f4fab20c5632675`  
		Last Modified: Sat, 03 Apr 2021 01:22:44 GMT  
		Size: 2.0 KB (1974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06b93a0d4c513ec838b27546bad996f092605e9c8399ad016f78b8b4cb96a900`  
		Last Modified: Sat, 03 Apr 2021 01:22:44 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8317ff85679d749fdf54c66f1b278c9f16aa11a116c5c0d288bc4f8debe41262`  
		Last Modified: Sat, 03 Apr 2021 01:22:44 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b8b1e736261cff8c3afa409fd73d85b78d6610a610e3b8eb3412798d3a18348`  
		Last Modified: Sat, 03 Apr 2021 01:22:44 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:alpine`

```console
$ docker pull nats@sha256:786039ea5743e66f92097f4c98419cdb7755824388806faae9ca893626cda20f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:alpine` - linux; amd64

```console
$ docker pull nats@sha256:11a99e623a9df5677bdcbcff33bd032975aabdc9c226e00410997607a5398ad0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7303859 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f56ceabe89d18dd0b0c58d97b018484ed43d818791b7a1d9e5e8a09123c6cbd5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 31 Mar 2021 20:10:06 GMT
ADD file:7119167b56ff1228b2fb639c768955ce9db7a999cd947179240b216dfa5ccbb9 in / 
# Wed, 31 Mar 2021 20:10:06 GMT
CMD ["/bin/sh"]
# Sat, 03 Apr 2021 03:02:20 GMT
ENV NATS_SERVER=2.2.1
# Sat, 03 Apr 2021 03:02:23 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='0123d924907282265190258662edf8ad4351055083b5040e3bdf59117bd1c51c' ;; 		armhf) natsArch='arm6'; sha256='da719b07fd57137f85bfa6cffc7d00841a9c1fb4cdf7ca9a537bfc3f99b71f36' ;; 		armv7) natsArch='arm7'; sha256='cf6e8d9a9cc5d05f7320fb4be8fc9239cb87b91c6600a61ce7a2fb63e2f29f5a' ;; 		x86_64) natsArch='amd64'; sha256='70cb40d78b82ea6c0ca926c31ef98d2e1c885cfe2f73f34883e4ca448366c2dd' ;; 		x86) natsArch='386'; sha256='da54d129f8a52c048ded61e3b62e946037a9464d02cf818e568bbf1e385ce6be' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Sat, 03 Apr 2021 03:02:23 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Sat, 03 Apr 2021 03:02:24 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Sat, 03 Apr 2021 03:02:24 GMT
EXPOSE 4222 6222 8222
# Sat, 03 Apr 2021 03:02:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 03 Apr 2021 03:02:24 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:ca3cd42a7c9525f6ce3d64c1a70982613a8235f0cc057ec9244052921853ef15`  
		Last Modified: Wed, 31 Mar 2021 20:10:46 GMT  
		Size: 2.8 MB (2811947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0ab87484469466c6eeb084bcbe5538907a8cca9e02c6c00ffc4e03bd68d4563`  
		Last Modified: Sat, 03 Apr 2021 03:03:06 GMT  
		Size: 4.5 MB (4490943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63537464a64606bc6b408c793c1b726d40b4b1a540a829516859d3405c203e37`  
		Last Modified: Sat, 03 Apr 2021 03:03:05 GMT  
		Size: 557.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:843bbc65e4b41319d487b9ba5eb3a58b709e795448cc632d75fb8f54d76868d9`  
		Last Modified: Sat, 03 Apr 2021 03:03:05 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:5980c4f84be539fd1b559624db6fa63ee409f825e4a93fa441598e93115d4b15
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6784924 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8f97d97f7e09aa5c9f936e0377789f200b06c8aabe846ce2591ebff76f7db8b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 31 Mar 2021 17:18:49 GMT
ADD file:988879d74f643b89539e5a0b6d74221621f19f4f87f722614addadc46ce47200 in / 
# Wed, 31 Mar 2021 17:18:50 GMT
CMD ["/bin/sh"]
# Sat, 03 Apr 2021 01:02:19 GMT
ENV NATS_SERVER=2.2.1
# Sat, 03 Apr 2021 01:02:24 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='0123d924907282265190258662edf8ad4351055083b5040e3bdf59117bd1c51c' ;; 		armhf) natsArch='arm6'; sha256='da719b07fd57137f85bfa6cffc7d00841a9c1fb4cdf7ca9a537bfc3f99b71f36' ;; 		armv7) natsArch='arm7'; sha256='cf6e8d9a9cc5d05f7320fb4be8fc9239cb87b91c6600a61ce7a2fb63e2f29f5a' ;; 		x86_64) natsArch='amd64'; sha256='70cb40d78b82ea6c0ca926c31ef98d2e1c885cfe2f73f34883e4ca448366c2dd' ;; 		x86) natsArch='386'; sha256='da54d129f8a52c048ded61e3b62e946037a9464d02cf818e568bbf1e385ce6be' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Sat, 03 Apr 2021 01:02:25 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Sat, 03 Apr 2021 01:02:26 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Sat, 03 Apr 2021 01:02:26 GMT
EXPOSE 4222 6222 8222
# Sat, 03 Apr 2021 01:02:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 03 Apr 2021 01:02:28 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:bb87125c6ee1ce30c6b33d2c96a9fbe46da4a290f7cb1dd73fd62d4e06503699`  
		Last Modified: Wed, 31 Mar 2021 17:19:55 GMT  
		Size: 2.6 MB (2622116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8d4b6ba6b297e822b0c0fe254f2d6b5afda81265eaf2481116af687cf66235c`  
		Last Modified: Sat, 03 Apr 2021 01:03:09 GMT  
		Size: 4.2 MB (4161834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ae0dfcf0132d6f11bd4762e4d1ec0b73f5ee36875a95dc78731673415f9de05`  
		Last Modified: Sat, 03 Apr 2021 01:03:07 GMT  
		Size: 561.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4f6ffd2be76e6334bd04318e19b02428d71b315b61ae8bb68ade8b07279ccff`  
		Last Modified: Sat, 03 Apr 2021 01:03:07 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:8e048143304eabc1fad2f149b2761e661ebe261c60e0ecb4cd0f58818ca12090
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6583142 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:04ad730346110f756c4e29df7ebe6e02cb97db3770b8fdda258f5f4def7c2f88`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 31 Mar 2021 18:13:27 GMT
ADD file:56e92c06393237a87e0a1ff475e9c9dc80e897d69ec20f45359b587906da345b in / 
# Wed, 31 Mar 2021 18:13:31 GMT
CMD ["/bin/sh"]
# Sat, 03 Apr 2021 01:45:11 GMT
ENV NATS_SERVER=2.2.1
# Sat, 03 Apr 2021 01:45:16 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='0123d924907282265190258662edf8ad4351055083b5040e3bdf59117bd1c51c' ;; 		armhf) natsArch='arm6'; sha256='da719b07fd57137f85bfa6cffc7d00841a9c1fb4cdf7ca9a537bfc3f99b71f36' ;; 		armv7) natsArch='arm7'; sha256='cf6e8d9a9cc5d05f7320fb4be8fc9239cb87b91c6600a61ce7a2fb63e2f29f5a' ;; 		x86_64) natsArch='amd64'; sha256='70cb40d78b82ea6c0ca926c31ef98d2e1c885cfe2f73f34883e4ca448366c2dd' ;; 		x86) natsArch='386'; sha256='da54d129f8a52c048ded61e3b62e946037a9464d02cf818e568bbf1e385ce6be' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Sat, 03 Apr 2021 01:45:17 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Sat, 03 Apr 2021 01:45:18 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Sat, 03 Apr 2021 01:45:19 GMT
EXPOSE 4222 6222 8222
# Sat, 03 Apr 2021 01:45:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 03 Apr 2021 01:45:21 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:07389e51ea05e1c9a3cb0ef92d31181f2afa1e445207ad99ffd8a94d6d6af295`  
		Last Modified: Wed, 31 Mar 2021 18:14:57 GMT  
		Size: 2.4 MB (2424108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7331da30076f2eba452960efaf8df4620f03624062670e29e8e3fb97823756b3`  
		Last Modified: Sat, 03 Apr 2021 01:46:03 GMT  
		Size: 4.2 MB (4158064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abd26a9a6149ca00bb0a5e94ae858765a0b787564c99ea0ba4ec23d5cd7a8bd9`  
		Last Modified: Sat, 03 Apr 2021 01:46:02 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96a5a7410fa6228e048f75c6327720948ad9d6dd06db4b594d43165c1f6cab1c`  
		Last Modified: Sat, 03 Apr 2021 01:46:01 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:980841965bacdff61fc62145784092e89a8c0db1f125fccc5e9d240f60f94e93
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6844304 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99075b219d76c9593adb6b735cc906569e0124a6761312332407ee8de31e6382`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 31 Mar 2021 17:21:21 GMT
ADD file:3b16ffee2b26d8af5db152fcc582aaccd9e1ec9e3343874e9969a205550fe07d in / 
# Wed, 31 Mar 2021 17:21:23 GMT
CMD ["/bin/sh"]
# Sat, 03 Apr 2021 03:47:42 GMT
ENV NATS_SERVER=2.2.1
# Sat, 03 Apr 2021 03:47:46 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='0123d924907282265190258662edf8ad4351055083b5040e3bdf59117bd1c51c' ;; 		armhf) natsArch='arm6'; sha256='da719b07fd57137f85bfa6cffc7d00841a9c1fb4cdf7ca9a537bfc3f99b71f36' ;; 		armv7) natsArch='arm7'; sha256='cf6e8d9a9cc5d05f7320fb4be8fc9239cb87b91c6600a61ce7a2fb63e2f29f5a' ;; 		x86_64) natsArch='amd64'; sha256='70cb40d78b82ea6c0ca926c31ef98d2e1c885cfe2f73f34883e4ca448366c2dd' ;; 		x86) natsArch='386'; sha256='da54d129f8a52c048ded61e3b62e946037a9464d02cf818e568bbf1e385ce6be' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Sat, 03 Apr 2021 03:47:47 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Sat, 03 Apr 2021 03:47:48 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Sat, 03 Apr 2021 03:47:49 GMT
EXPOSE 4222 6222 8222
# Sat, 03 Apr 2021 03:47:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 03 Apr 2021 03:47:51 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:912815139b61c8926da31f7701f0a924e7964e3713052bf1a53193a4562157f6`  
		Last Modified: Wed, 31 Mar 2021 17:22:41 GMT  
		Size: 2.7 MB (2711920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9228d7a2d7ff547081c5c823de18c8fa62bb6200cee9f820f437c3004e90f309`  
		Last Modified: Sat, 03 Apr 2021 03:48:31 GMT  
		Size: 4.1 MB (4131414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ec0c89cac556aea8879a9beeefc7c2f8528b16539e3765c11de3c76e564e6f6`  
		Last Modified: Sat, 03 Apr 2021 03:48:30 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08fc29c470aa8216b46da0c00b30283b238b812f9d1395be3920045c367005af`  
		Last Modified: Sat, 03 Apr 2021 03:48:30 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:alpine3.13`

```console
$ docker pull nats@sha256:786039ea5743e66f92097f4c98419cdb7755824388806faae9ca893626cda20f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:alpine3.13` - linux; amd64

```console
$ docker pull nats@sha256:11a99e623a9df5677bdcbcff33bd032975aabdc9c226e00410997607a5398ad0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7303859 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f56ceabe89d18dd0b0c58d97b018484ed43d818791b7a1d9e5e8a09123c6cbd5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 31 Mar 2021 20:10:06 GMT
ADD file:7119167b56ff1228b2fb639c768955ce9db7a999cd947179240b216dfa5ccbb9 in / 
# Wed, 31 Mar 2021 20:10:06 GMT
CMD ["/bin/sh"]
# Sat, 03 Apr 2021 03:02:20 GMT
ENV NATS_SERVER=2.2.1
# Sat, 03 Apr 2021 03:02:23 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='0123d924907282265190258662edf8ad4351055083b5040e3bdf59117bd1c51c' ;; 		armhf) natsArch='arm6'; sha256='da719b07fd57137f85bfa6cffc7d00841a9c1fb4cdf7ca9a537bfc3f99b71f36' ;; 		armv7) natsArch='arm7'; sha256='cf6e8d9a9cc5d05f7320fb4be8fc9239cb87b91c6600a61ce7a2fb63e2f29f5a' ;; 		x86_64) natsArch='amd64'; sha256='70cb40d78b82ea6c0ca926c31ef98d2e1c885cfe2f73f34883e4ca448366c2dd' ;; 		x86) natsArch='386'; sha256='da54d129f8a52c048ded61e3b62e946037a9464d02cf818e568bbf1e385ce6be' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Sat, 03 Apr 2021 03:02:23 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Sat, 03 Apr 2021 03:02:24 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Sat, 03 Apr 2021 03:02:24 GMT
EXPOSE 4222 6222 8222
# Sat, 03 Apr 2021 03:02:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 03 Apr 2021 03:02:24 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:ca3cd42a7c9525f6ce3d64c1a70982613a8235f0cc057ec9244052921853ef15`  
		Last Modified: Wed, 31 Mar 2021 20:10:46 GMT  
		Size: 2.8 MB (2811947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0ab87484469466c6eeb084bcbe5538907a8cca9e02c6c00ffc4e03bd68d4563`  
		Last Modified: Sat, 03 Apr 2021 03:03:06 GMT  
		Size: 4.5 MB (4490943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63537464a64606bc6b408c793c1b726d40b4b1a540a829516859d3405c203e37`  
		Last Modified: Sat, 03 Apr 2021 03:03:05 GMT  
		Size: 557.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:843bbc65e4b41319d487b9ba5eb3a58b709e795448cc632d75fb8f54d76868d9`  
		Last Modified: Sat, 03 Apr 2021 03:03:05 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.13` - linux; arm variant v6

```console
$ docker pull nats@sha256:5980c4f84be539fd1b559624db6fa63ee409f825e4a93fa441598e93115d4b15
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6784924 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8f97d97f7e09aa5c9f936e0377789f200b06c8aabe846ce2591ebff76f7db8b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 31 Mar 2021 17:18:49 GMT
ADD file:988879d74f643b89539e5a0b6d74221621f19f4f87f722614addadc46ce47200 in / 
# Wed, 31 Mar 2021 17:18:50 GMT
CMD ["/bin/sh"]
# Sat, 03 Apr 2021 01:02:19 GMT
ENV NATS_SERVER=2.2.1
# Sat, 03 Apr 2021 01:02:24 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='0123d924907282265190258662edf8ad4351055083b5040e3bdf59117bd1c51c' ;; 		armhf) natsArch='arm6'; sha256='da719b07fd57137f85bfa6cffc7d00841a9c1fb4cdf7ca9a537bfc3f99b71f36' ;; 		armv7) natsArch='arm7'; sha256='cf6e8d9a9cc5d05f7320fb4be8fc9239cb87b91c6600a61ce7a2fb63e2f29f5a' ;; 		x86_64) natsArch='amd64'; sha256='70cb40d78b82ea6c0ca926c31ef98d2e1c885cfe2f73f34883e4ca448366c2dd' ;; 		x86) natsArch='386'; sha256='da54d129f8a52c048ded61e3b62e946037a9464d02cf818e568bbf1e385ce6be' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Sat, 03 Apr 2021 01:02:25 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Sat, 03 Apr 2021 01:02:26 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Sat, 03 Apr 2021 01:02:26 GMT
EXPOSE 4222 6222 8222
# Sat, 03 Apr 2021 01:02:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 03 Apr 2021 01:02:28 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:bb87125c6ee1ce30c6b33d2c96a9fbe46da4a290f7cb1dd73fd62d4e06503699`  
		Last Modified: Wed, 31 Mar 2021 17:19:55 GMT  
		Size: 2.6 MB (2622116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8d4b6ba6b297e822b0c0fe254f2d6b5afda81265eaf2481116af687cf66235c`  
		Last Modified: Sat, 03 Apr 2021 01:03:09 GMT  
		Size: 4.2 MB (4161834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ae0dfcf0132d6f11bd4762e4d1ec0b73f5ee36875a95dc78731673415f9de05`  
		Last Modified: Sat, 03 Apr 2021 01:03:07 GMT  
		Size: 561.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4f6ffd2be76e6334bd04318e19b02428d71b315b61ae8bb68ade8b07279ccff`  
		Last Modified: Sat, 03 Apr 2021 01:03:07 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.13` - linux; arm variant v7

```console
$ docker pull nats@sha256:8e048143304eabc1fad2f149b2761e661ebe261c60e0ecb4cd0f58818ca12090
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6583142 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:04ad730346110f756c4e29df7ebe6e02cb97db3770b8fdda258f5f4def7c2f88`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 31 Mar 2021 18:13:27 GMT
ADD file:56e92c06393237a87e0a1ff475e9c9dc80e897d69ec20f45359b587906da345b in / 
# Wed, 31 Mar 2021 18:13:31 GMT
CMD ["/bin/sh"]
# Sat, 03 Apr 2021 01:45:11 GMT
ENV NATS_SERVER=2.2.1
# Sat, 03 Apr 2021 01:45:16 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='0123d924907282265190258662edf8ad4351055083b5040e3bdf59117bd1c51c' ;; 		armhf) natsArch='arm6'; sha256='da719b07fd57137f85bfa6cffc7d00841a9c1fb4cdf7ca9a537bfc3f99b71f36' ;; 		armv7) natsArch='arm7'; sha256='cf6e8d9a9cc5d05f7320fb4be8fc9239cb87b91c6600a61ce7a2fb63e2f29f5a' ;; 		x86_64) natsArch='amd64'; sha256='70cb40d78b82ea6c0ca926c31ef98d2e1c885cfe2f73f34883e4ca448366c2dd' ;; 		x86) natsArch='386'; sha256='da54d129f8a52c048ded61e3b62e946037a9464d02cf818e568bbf1e385ce6be' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Sat, 03 Apr 2021 01:45:17 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Sat, 03 Apr 2021 01:45:18 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Sat, 03 Apr 2021 01:45:19 GMT
EXPOSE 4222 6222 8222
# Sat, 03 Apr 2021 01:45:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 03 Apr 2021 01:45:21 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:07389e51ea05e1c9a3cb0ef92d31181f2afa1e445207ad99ffd8a94d6d6af295`  
		Last Modified: Wed, 31 Mar 2021 18:14:57 GMT  
		Size: 2.4 MB (2424108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7331da30076f2eba452960efaf8df4620f03624062670e29e8e3fb97823756b3`  
		Last Modified: Sat, 03 Apr 2021 01:46:03 GMT  
		Size: 4.2 MB (4158064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abd26a9a6149ca00bb0a5e94ae858765a0b787564c99ea0ba4ec23d5cd7a8bd9`  
		Last Modified: Sat, 03 Apr 2021 01:46:02 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96a5a7410fa6228e048f75c6327720948ad9d6dd06db4b594d43165c1f6cab1c`  
		Last Modified: Sat, 03 Apr 2021 01:46:01 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.13` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:980841965bacdff61fc62145784092e89a8c0db1f125fccc5e9d240f60f94e93
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6844304 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99075b219d76c9593adb6b735cc906569e0124a6761312332407ee8de31e6382`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 31 Mar 2021 17:21:21 GMT
ADD file:3b16ffee2b26d8af5db152fcc582aaccd9e1ec9e3343874e9969a205550fe07d in / 
# Wed, 31 Mar 2021 17:21:23 GMT
CMD ["/bin/sh"]
# Sat, 03 Apr 2021 03:47:42 GMT
ENV NATS_SERVER=2.2.1
# Sat, 03 Apr 2021 03:47:46 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='0123d924907282265190258662edf8ad4351055083b5040e3bdf59117bd1c51c' ;; 		armhf) natsArch='arm6'; sha256='da719b07fd57137f85bfa6cffc7d00841a9c1fb4cdf7ca9a537bfc3f99b71f36' ;; 		armv7) natsArch='arm7'; sha256='cf6e8d9a9cc5d05f7320fb4be8fc9239cb87b91c6600a61ce7a2fb63e2f29f5a' ;; 		x86_64) natsArch='amd64'; sha256='70cb40d78b82ea6c0ca926c31ef98d2e1c885cfe2f73f34883e4ca448366c2dd' ;; 		x86) natsArch='386'; sha256='da54d129f8a52c048ded61e3b62e946037a9464d02cf818e568bbf1e385ce6be' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Sat, 03 Apr 2021 03:47:47 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Sat, 03 Apr 2021 03:47:48 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Sat, 03 Apr 2021 03:47:49 GMT
EXPOSE 4222 6222 8222
# Sat, 03 Apr 2021 03:47:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 03 Apr 2021 03:47:51 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:912815139b61c8926da31f7701f0a924e7964e3713052bf1a53193a4562157f6`  
		Last Modified: Wed, 31 Mar 2021 17:22:41 GMT  
		Size: 2.7 MB (2711920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9228d7a2d7ff547081c5c823de18c8fa62bb6200cee9f820f437c3004e90f309`  
		Last Modified: Sat, 03 Apr 2021 03:48:31 GMT  
		Size: 4.1 MB (4131414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ec0c89cac556aea8879a9beeefc7c2f8528b16539e3765c11de3c76e564e6f6`  
		Last Modified: Sat, 03 Apr 2021 03:48:30 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08fc29c470aa8216b46da0c00b30283b238b812f9d1395be3920045c367005af`  
		Last Modified: Sat, 03 Apr 2021 03:48:30 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:latest`

```console
$ docker pull nats@sha256:5958ba516eb8f221dc01b26d0afece5f9a48f7f0e978c889d19d1e788a02531e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.1817; amd64

### `nats:latest` - linux; amd64

```console
$ docker pull nats@sha256:3bd24b6508d68c6d8835ecf42066a66f01b9e58d55c7a82d99eb3f1d9041fe15
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4208708 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f68fc0ca6306424854628406a234c7c5f76f2a13d658233ecefdb59a3de4ec89`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 03 Apr 2021 03:02:40 GMT
COPY file:494bfb1615387aa8aa24059641c501c246cffbb47653109c93d498a68ccce32a in /nats-server 
# Sat, 03 Apr 2021 03:02:41 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Sat, 03 Apr 2021 03:02:41 GMT
EXPOSE 4222 6222 8222
# Sat, 03 Apr 2021 03:02:41 GMT
ENTRYPOINT ["/nats-server"]
# Sat, 03 Apr 2021 03:02:41 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:832634cbfed021f934fff287987e6acb75f23228af46328d3f79d812b6462c57`  
		Last Modified: Sat, 03 Apr 2021 03:03:31 GMT  
		Size: 4.2 MB (4208232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91f381d2349aa770a85b4fde9e5c7794fe38c878aea8784f679b3f09728534a4`  
		Last Modified: Sat, 03 Apr 2021 03:03:30 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm variant v6

```console
$ docker pull nats@sha256:0c1db0c5e32501c283742665116d2ae34168be99f1f0298a17fe6a1a0c3c9cb1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3882437 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dadccf67b2f681485255da8d75647104535e861fb3ee82f610f6d42281a07300`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 03 Apr 2021 01:02:37 GMT
COPY file:54bee7857c6b5cc9e3287e28fd1ffbbd529d72e791a1746d90d0b66346698246 in /nats-server 
# Sat, 03 Apr 2021 01:02:38 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Sat, 03 Apr 2021 01:02:38 GMT
EXPOSE 4222 6222 8222
# Sat, 03 Apr 2021 01:02:39 GMT
ENTRYPOINT ["/nats-server"]
# Sat, 03 Apr 2021 01:02:40 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:91cca6fbde65445d7c75ad5de8204fd8356fa76f2dd2983a53b2c0d9b7255bd9`  
		Last Modified: Sat, 03 Apr 2021 01:03:23 GMT  
		Size: 3.9 MB (3881961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b8d6f093021c26c95a4df34d728495a189d358902c6fed301d6bc06e93f4e85`  
		Last Modified: Sat, 03 Apr 2021 01:03:22 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm variant v7

```console
$ docker pull nats@sha256:61dade57dcce93e1f3ea3e01779c4d2f1bf4ff21415290e42dfe72cba333f7d1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3877449 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64ad61fe367441505f4bdd49177124c6f6fbb5d9e212c6b871aec402ea6c4122`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 03 Apr 2021 01:45:33 GMT
COPY file:d95e297af0c7798d74c045b7143a48199a8e32ca5c5aa0b8d7c967a602bc1cfe in /nats-server 
# Sat, 03 Apr 2021 01:45:34 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Sat, 03 Apr 2021 01:45:35 GMT
EXPOSE 4222 6222 8222
# Sat, 03 Apr 2021 01:45:36 GMT
ENTRYPOINT ["/nats-server"]
# Sat, 03 Apr 2021 01:45:37 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:7919165d0b190df92f81ef4af9a0a2fef8a2da95dac86e567498a9364b0be069`  
		Last Modified: Sat, 03 Apr 2021 01:46:21 GMT  
		Size: 3.9 MB (3876974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdfa2b4e61cc1a65501d2feea740d0f932e2bf901c202226b24a7d787c0f4dff`  
		Last Modified: Sat, 03 Apr 2021 01:46:20 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:13c34571ac946007679eb9333b30ca2fc5225ea3afdeb3ec3082bf4e5befe284
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3850749 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9d8fa2c7d5a8fb8a3e96f92707cd39a3107455acd96b42415d60cf31cae334d`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 03 Apr 2021 03:48:01 GMT
COPY file:4d714e3c520aa8a1f5935c65806500f01ea25ace84372fd7f3aa0a06f1f626c9 in /nats-server 
# Sat, 03 Apr 2021 03:48:02 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Sat, 03 Apr 2021 03:48:03 GMT
EXPOSE 4222 6222 8222
# Sat, 03 Apr 2021 03:48:04 GMT
ENTRYPOINT ["/nats-server"]
# Sat, 03 Apr 2021 03:48:05 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:310f293639061b27b8965c8683cf2bffb7d9b58bdb924635525fa7d990f2f3fb`  
		Last Modified: Sat, 03 Apr 2021 03:48:48 GMT  
		Size: 3.9 MB (3850270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e64370dd792941a18253408636a97ab34ef2f6ea706da1fe18ae7e008a3b13e`  
		Last Modified: Sat, 03 Apr 2021 03:48:47 GMT  
		Size: 479.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - windows version 10.0.17763.1817; amd64

```console
$ docker pull nats@sha256:7400f49e711ad398f8708d78498cb89250765f194fcad4bfb28b0811dddce228
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.7 MB (105658317 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d32a24884d574cc6457ee6540f906dc735846c9ed2cd1b15cb1b79c0f0df8fd`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 26 Feb 2021 16:47:31 GMT
RUN Apply image 1809-amd64
# Wed, 10 Mar 2021 16:56:55 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Sat, 03 Apr 2021 01:17:28 GMT
RUN cmd /S /C #(nop) COPY file:428a7e80db4313301a46326a9a79832e9cbe7d78c94e749b5c295e813e484f21 in C:\nats-server.exe 
# Sat, 03 Apr 2021 01:17:29 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Sat, 03 Apr 2021 01:17:30 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Sat, 03 Apr 2021 01:17:30 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Sat, 03 Apr 2021 01:17:32 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a11c4ca8f1ba16b6e1395d4523be2215bd0871c2e3e4695b9f2b87bd7472be52`  
		Size: 101.4 MB (101389964 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f49969195f32b7e40a81e3d189259fec7ebf52ee0ec5dafd5f3f288715354fed`  
		Last Modified: Wed, 10 Mar 2021 17:01:57 GMT  
		Size: 1.0 KB (1047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b78be9ec55bfa99633688cc4d73e47268a005880724f5c31af765df173fe522b`  
		Last Modified: Sat, 03 Apr 2021 01:22:27 GMT  
		Size: 4.3 MB (4262100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93286c3879edf77d449ceff1ed34a72becb3264fead3b488a3f05415c4bb62ec`  
		Last Modified: Sat, 03 Apr 2021 01:22:26 GMT  
		Size: 1.8 KB (1761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a913d40db4af4450743a872058165885095d790cda716fcd48634e3d7f4143f`  
		Last Modified: Sat, 03 Apr 2021 01:22:26 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67f64ab62ffafadee29cddb026c057f47c1d88836cf8c2e1da91189a1289fafd`  
		Last Modified: Sat, 03 Apr 2021 01:22:26 GMT  
		Size: 1.1 KB (1102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f1de1af4e095d547a9e171edf595e46d67d5687074985d261582ae4618438fb`  
		Last Modified: Sat, 03 Apr 2021 01:22:26 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:linux`

```console
$ docker pull nats@sha256:f116a903fd14977153dc2ae74e3b0437762ee2a6c7858807246d6501b2a9af54
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:linux` - linux; amd64

```console
$ docker pull nats@sha256:3bd24b6508d68c6d8835ecf42066a66f01b9e58d55c7a82d99eb3f1d9041fe15
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4208708 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f68fc0ca6306424854628406a234c7c5f76f2a13d658233ecefdb59a3de4ec89`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 03 Apr 2021 03:02:40 GMT
COPY file:494bfb1615387aa8aa24059641c501c246cffbb47653109c93d498a68ccce32a in /nats-server 
# Sat, 03 Apr 2021 03:02:41 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Sat, 03 Apr 2021 03:02:41 GMT
EXPOSE 4222 6222 8222
# Sat, 03 Apr 2021 03:02:41 GMT
ENTRYPOINT ["/nats-server"]
# Sat, 03 Apr 2021 03:02:41 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:832634cbfed021f934fff287987e6acb75f23228af46328d3f79d812b6462c57`  
		Last Modified: Sat, 03 Apr 2021 03:03:31 GMT  
		Size: 4.2 MB (4208232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91f381d2349aa770a85b4fde9e5c7794fe38c878aea8784f679b3f09728534a4`  
		Last Modified: Sat, 03 Apr 2021 03:03:30 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:0c1db0c5e32501c283742665116d2ae34168be99f1f0298a17fe6a1a0c3c9cb1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3882437 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dadccf67b2f681485255da8d75647104535e861fb3ee82f610f6d42281a07300`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 03 Apr 2021 01:02:37 GMT
COPY file:54bee7857c6b5cc9e3287e28fd1ffbbd529d72e791a1746d90d0b66346698246 in /nats-server 
# Sat, 03 Apr 2021 01:02:38 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Sat, 03 Apr 2021 01:02:38 GMT
EXPOSE 4222 6222 8222
# Sat, 03 Apr 2021 01:02:39 GMT
ENTRYPOINT ["/nats-server"]
# Sat, 03 Apr 2021 01:02:40 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:91cca6fbde65445d7c75ad5de8204fd8356fa76f2dd2983a53b2c0d9b7255bd9`  
		Last Modified: Sat, 03 Apr 2021 01:03:23 GMT  
		Size: 3.9 MB (3881961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b8d6f093021c26c95a4df34d728495a189d358902c6fed301d6bc06e93f4e85`  
		Last Modified: Sat, 03 Apr 2021 01:03:22 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:61dade57dcce93e1f3ea3e01779c4d2f1bf4ff21415290e42dfe72cba333f7d1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3877449 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64ad61fe367441505f4bdd49177124c6f6fbb5d9e212c6b871aec402ea6c4122`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 03 Apr 2021 01:45:33 GMT
COPY file:d95e297af0c7798d74c045b7143a48199a8e32ca5c5aa0b8d7c967a602bc1cfe in /nats-server 
# Sat, 03 Apr 2021 01:45:34 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Sat, 03 Apr 2021 01:45:35 GMT
EXPOSE 4222 6222 8222
# Sat, 03 Apr 2021 01:45:36 GMT
ENTRYPOINT ["/nats-server"]
# Sat, 03 Apr 2021 01:45:37 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:7919165d0b190df92f81ef4af9a0a2fef8a2da95dac86e567498a9364b0be069`  
		Last Modified: Sat, 03 Apr 2021 01:46:21 GMT  
		Size: 3.9 MB (3876974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdfa2b4e61cc1a65501d2feea740d0f932e2bf901c202226b24a7d787c0f4dff`  
		Last Modified: Sat, 03 Apr 2021 01:46:20 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:13c34571ac946007679eb9333b30ca2fc5225ea3afdeb3ec3082bf4e5befe284
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3850749 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9d8fa2c7d5a8fb8a3e96f92707cd39a3107455acd96b42415d60cf31cae334d`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 03 Apr 2021 03:48:01 GMT
COPY file:4d714e3c520aa8a1f5935c65806500f01ea25ace84372fd7f3aa0a06f1f626c9 in /nats-server 
# Sat, 03 Apr 2021 03:48:02 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Sat, 03 Apr 2021 03:48:03 GMT
EXPOSE 4222 6222 8222
# Sat, 03 Apr 2021 03:48:04 GMT
ENTRYPOINT ["/nats-server"]
# Sat, 03 Apr 2021 03:48:05 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:310f293639061b27b8965c8683cf2bffb7d9b58bdb924635525fa7d990f2f3fb`  
		Last Modified: Sat, 03 Apr 2021 03:48:48 GMT  
		Size: 3.9 MB (3850270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e64370dd792941a18253408636a97ab34ef2f6ea706da1fe18ae7e008a3b13e`  
		Last Modified: Sat, 03 Apr 2021 03:48:47 GMT  
		Size: 479.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:nanoserver`

```console
$ docker pull nats@sha256:795115a3a3b1b5f4cbc7c017ddd52f46848199b694cff7aafbcb0c7d464925e5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1817; amd64

### `nats:nanoserver` - windows version 10.0.17763.1817; amd64

```console
$ docker pull nats@sha256:7400f49e711ad398f8708d78498cb89250765f194fcad4bfb28b0811dddce228
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.7 MB (105658317 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d32a24884d574cc6457ee6540f906dc735846c9ed2cd1b15cb1b79c0f0df8fd`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 26 Feb 2021 16:47:31 GMT
RUN Apply image 1809-amd64
# Wed, 10 Mar 2021 16:56:55 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Sat, 03 Apr 2021 01:17:28 GMT
RUN cmd /S /C #(nop) COPY file:428a7e80db4313301a46326a9a79832e9cbe7d78c94e749b5c295e813e484f21 in C:\nats-server.exe 
# Sat, 03 Apr 2021 01:17:29 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Sat, 03 Apr 2021 01:17:30 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Sat, 03 Apr 2021 01:17:30 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Sat, 03 Apr 2021 01:17:32 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a11c4ca8f1ba16b6e1395d4523be2215bd0871c2e3e4695b9f2b87bd7472be52`  
		Size: 101.4 MB (101389964 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f49969195f32b7e40a81e3d189259fec7ebf52ee0ec5dafd5f3f288715354fed`  
		Last Modified: Wed, 10 Mar 2021 17:01:57 GMT  
		Size: 1.0 KB (1047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b78be9ec55bfa99633688cc4d73e47268a005880724f5c31af765df173fe522b`  
		Last Modified: Sat, 03 Apr 2021 01:22:27 GMT  
		Size: 4.3 MB (4262100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93286c3879edf77d449ceff1ed34a72becb3264fead3b488a3f05415c4bb62ec`  
		Last Modified: Sat, 03 Apr 2021 01:22:26 GMT  
		Size: 1.8 KB (1761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a913d40db4af4450743a872058165885095d790cda716fcd48634e3d7f4143f`  
		Last Modified: Sat, 03 Apr 2021 01:22:26 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67f64ab62ffafadee29cddb026c057f47c1d88836cf8c2e1da91189a1289fafd`  
		Last Modified: Sat, 03 Apr 2021 01:22:26 GMT  
		Size: 1.1 KB (1102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f1de1af4e095d547a9e171edf595e46d67d5687074985d261582ae4618438fb`  
		Last Modified: Sat, 03 Apr 2021 01:22:26 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:nanoserver-1809`

```console
$ docker pull nats@sha256:795115a3a3b1b5f4cbc7c017ddd52f46848199b694cff7aafbcb0c7d464925e5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1817; amd64

### `nats:nanoserver-1809` - windows version 10.0.17763.1817; amd64

```console
$ docker pull nats@sha256:7400f49e711ad398f8708d78498cb89250765f194fcad4bfb28b0811dddce228
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.7 MB (105658317 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d32a24884d574cc6457ee6540f906dc735846c9ed2cd1b15cb1b79c0f0df8fd`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 26 Feb 2021 16:47:31 GMT
RUN Apply image 1809-amd64
# Wed, 10 Mar 2021 16:56:55 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Sat, 03 Apr 2021 01:17:28 GMT
RUN cmd /S /C #(nop) COPY file:428a7e80db4313301a46326a9a79832e9cbe7d78c94e749b5c295e813e484f21 in C:\nats-server.exe 
# Sat, 03 Apr 2021 01:17:29 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Sat, 03 Apr 2021 01:17:30 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Sat, 03 Apr 2021 01:17:30 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Sat, 03 Apr 2021 01:17:32 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a11c4ca8f1ba16b6e1395d4523be2215bd0871c2e3e4695b9f2b87bd7472be52`  
		Size: 101.4 MB (101389964 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f49969195f32b7e40a81e3d189259fec7ebf52ee0ec5dafd5f3f288715354fed`  
		Last Modified: Wed, 10 Mar 2021 17:01:57 GMT  
		Size: 1.0 KB (1047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b78be9ec55bfa99633688cc4d73e47268a005880724f5c31af765df173fe522b`  
		Last Modified: Sat, 03 Apr 2021 01:22:27 GMT  
		Size: 4.3 MB (4262100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93286c3879edf77d449ceff1ed34a72becb3264fead3b488a3f05415c4bb62ec`  
		Last Modified: Sat, 03 Apr 2021 01:22:26 GMT  
		Size: 1.8 KB (1761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a913d40db4af4450743a872058165885095d790cda716fcd48634e3d7f4143f`  
		Last Modified: Sat, 03 Apr 2021 01:22:26 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67f64ab62ffafadee29cddb026c057f47c1d88836cf8c2e1da91189a1289fafd`  
		Last Modified: Sat, 03 Apr 2021 01:22:26 GMT  
		Size: 1.1 KB (1102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f1de1af4e095d547a9e171edf595e46d67d5687074985d261582ae4618438fb`  
		Last Modified: Sat, 03 Apr 2021 01:22:26 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:scratch`

```console
$ docker pull nats@sha256:f116a903fd14977153dc2ae74e3b0437762ee2a6c7858807246d6501b2a9af54
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:scratch` - linux; amd64

```console
$ docker pull nats@sha256:3bd24b6508d68c6d8835ecf42066a66f01b9e58d55c7a82d99eb3f1d9041fe15
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4208708 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f68fc0ca6306424854628406a234c7c5f76f2a13d658233ecefdb59a3de4ec89`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 03 Apr 2021 03:02:40 GMT
COPY file:494bfb1615387aa8aa24059641c501c246cffbb47653109c93d498a68ccce32a in /nats-server 
# Sat, 03 Apr 2021 03:02:41 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Sat, 03 Apr 2021 03:02:41 GMT
EXPOSE 4222 6222 8222
# Sat, 03 Apr 2021 03:02:41 GMT
ENTRYPOINT ["/nats-server"]
# Sat, 03 Apr 2021 03:02:41 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:832634cbfed021f934fff287987e6acb75f23228af46328d3f79d812b6462c57`  
		Last Modified: Sat, 03 Apr 2021 03:03:31 GMT  
		Size: 4.2 MB (4208232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91f381d2349aa770a85b4fde9e5c7794fe38c878aea8784f679b3f09728534a4`  
		Last Modified: Sat, 03 Apr 2021 03:03:30 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:0c1db0c5e32501c283742665116d2ae34168be99f1f0298a17fe6a1a0c3c9cb1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3882437 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dadccf67b2f681485255da8d75647104535e861fb3ee82f610f6d42281a07300`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 03 Apr 2021 01:02:37 GMT
COPY file:54bee7857c6b5cc9e3287e28fd1ffbbd529d72e791a1746d90d0b66346698246 in /nats-server 
# Sat, 03 Apr 2021 01:02:38 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Sat, 03 Apr 2021 01:02:38 GMT
EXPOSE 4222 6222 8222
# Sat, 03 Apr 2021 01:02:39 GMT
ENTRYPOINT ["/nats-server"]
# Sat, 03 Apr 2021 01:02:40 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:91cca6fbde65445d7c75ad5de8204fd8356fa76f2dd2983a53b2c0d9b7255bd9`  
		Last Modified: Sat, 03 Apr 2021 01:03:23 GMT  
		Size: 3.9 MB (3881961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b8d6f093021c26c95a4df34d728495a189d358902c6fed301d6bc06e93f4e85`  
		Last Modified: Sat, 03 Apr 2021 01:03:22 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:61dade57dcce93e1f3ea3e01779c4d2f1bf4ff21415290e42dfe72cba333f7d1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3877449 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64ad61fe367441505f4bdd49177124c6f6fbb5d9e212c6b871aec402ea6c4122`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 03 Apr 2021 01:45:33 GMT
COPY file:d95e297af0c7798d74c045b7143a48199a8e32ca5c5aa0b8d7c967a602bc1cfe in /nats-server 
# Sat, 03 Apr 2021 01:45:34 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Sat, 03 Apr 2021 01:45:35 GMT
EXPOSE 4222 6222 8222
# Sat, 03 Apr 2021 01:45:36 GMT
ENTRYPOINT ["/nats-server"]
# Sat, 03 Apr 2021 01:45:37 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:7919165d0b190df92f81ef4af9a0a2fef8a2da95dac86e567498a9364b0be069`  
		Last Modified: Sat, 03 Apr 2021 01:46:21 GMT  
		Size: 3.9 MB (3876974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdfa2b4e61cc1a65501d2feea740d0f932e2bf901c202226b24a7d787c0f4dff`  
		Last Modified: Sat, 03 Apr 2021 01:46:20 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:13c34571ac946007679eb9333b30ca2fc5225ea3afdeb3ec3082bf4e5befe284
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3850749 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9d8fa2c7d5a8fb8a3e96f92707cd39a3107455acd96b42415d60cf31cae334d`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 03 Apr 2021 03:48:01 GMT
COPY file:4d714e3c520aa8a1f5935c65806500f01ea25ace84372fd7f3aa0a06f1f626c9 in /nats-server 
# Sat, 03 Apr 2021 03:48:02 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Sat, 03 Apr 2021 03:48:03 GMT
EXPOSE 4222 6222 8222
# Sat, 03 Apr 2021 03:48:04 GMT
ENTRYPOINT ["/nats-server"]
# Sat, 03 Apr 2021 03:48:05 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:310f293639061b27b8965c8683cf2bffb7d9b58bdb924635525fa7d990f2f3fb`  
		Last Modified: Sat, 03 Apr 2021 03:48:48 GMT  
		Size: 3.9 MB (3850270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e64370dd792941a18253408636a97ab34ef2f6ea706da1fe18ae7e008a3b13e`  
		Last Modified: Sat, 03 Apr 2021 03:48:47 GMT  
		Size: 479.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:windowsservercore`

```console
$ docker pull nats@sha256:91810bbcbf606b0cf379000443d302c7b5d928cc7309c63da19917ca3ff0525f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1817; amd64
	-	windows version 10.0.14393.4283; amd64

### `nats:windowsservercore` - windows version 10.0.17763.1817; amd64

```console
$ docker pull nats@sha256:79eefa8948e2758f0659fb934899c37b05b67eb96c38b0e8c67c1a0974992423
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2480294595 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3875d7d95dfdb0356da902eee6142a19a85e38ae7ddde3bbf34b06e18765ecd7`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 27 Feb 2021 09:32:06 GMT
RUN Install update 1809-amd64
# Wed, 10 Mar 2021 14:15:30 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Mar 2021 16:54:55 GMT
ENV NATS_DOCKERIZED=1
# Sat, 03 Apr 2021 01:15:14 GMT
ENV NATS_SERVER=2.2.1
# Sat, 03 Apr 2021 01:15:16 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.2.1/nats-server-v2.2.1-windows-amd64.zip
# Sat, 03 Apr 2021 01:15:17 GMT
ENV GIT_DOWNLOAD_SHA256=1f0d48a7ba9200e2572016a9f3e1ec7e630f0518cc0b40950c14ff3a5d900924
# Sat, 03 Apr 2021 01:15:50 GMT
RUN Set-PSDebug -Trace 2
# Sat, 03 Apr 2021 01:17:04 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Sat, 03 Apr 2021 01:17:06 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Sat, 03 Apr 2021 01:17:07 GMT
EXPOSE 4222 6222 8222
# Sat, 03 Apr 2021 01:17:08 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Sat, 03 Apr 2021 01:17:09 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5ff1512f88ecd4ff0a91ade34d43733c48834433e35f062f80e6e70d706f8d73`  
		Size: 743.2 MB (743201590 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:31ae1fcdffac4071930a0d98172fc515a43c93aa55870e4b6cc8c789b9444e73`  
		Last Modified: Wed, 10 Mar 2021 16:22:41 GMT  
		Size: 1.3 KB (1305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cfde5dabd6353190a5343286e79ed9ad72f47f48ca9197e594b9771b5039e7d`  
		Last Modified: Wed, 10 Mar 2021 17:01:37 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4eb0ea2b178ae862896fca7bda0c5c677fd82870ca007ebe695e42f058831af`  
		Last Modified: Sat, 03 Apr 2021 01:22:03 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8c9d68c9aa9d29abd0c09f2016e9fcfc53bd185a7403989cec09108f661a977`  
		Last Modified: Sat, 03 Apr 2021 01:22:03 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b05ed1fd68964dcfc103f5452b7ee8528749d538e395dd36d17158cab031fdf`  
		Last Modified: Sat, 03 Apr 2021 01:22:03 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3994ed7efdb8fb7c71541583ff656c6c8e54e722284ec414d3ef00145cb43efa`  
		Last Modified: Sat, 03 Apr 2021 01:22:09 GMT  
		Size: 5.1 MB (5064967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0c3e4f395cd1bacff8cb6c6a451cfe4d56b4a054cfc15dd1a8b04a9e56240fa`  
		Last Modified: Sat, 03 Apr 2021 01:22:03 GMT  
		Size: 13.7 MB (13681925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bc88971a96126558018ca2f17f084db054369de555c8cb84a508c7a1394236e`  
		Last Modified: Sat, 03 Apr 2021 01:22:00 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66fa36b1a5dd3f83c94c4e1597659532cb557cd8f9cd414bb81f1049f39924af`  
		Last Modified: Sat, 03 Apr 2021 01:22:00 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4147b1dd2e59f8f133ab83ace94bf75ef78c0f9f261d49d65b7cc0b84d49438e`  
		Last Modified: Sat, 03 Apr 2021 01:22:00 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49b9455ff088b797d1cff54432e7f275092555cd8485bbf6b4aa926b88077f94`  
		Last Modified: Sat, 03 Apr 2021 01:22:00 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:windowsservercore` - windows version 10.0.14393.4283; amd64

```console
$ docker pull nats@sha256:ea694b06746523df91b7d824d0fc9030b282cc666bf34e937103b72b280d8a09
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5817027558 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:265f2ee0b7a998cc6ce663873648377be2b81226575d11ed5d1537b35a4118bf`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 03 Mar 2021 18:02:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Mar 2021 14:25:01 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Mar 2021 16:57:09 GMT
ENV NATS_DOCKERIZED=1
# Sat, 03 Apr 2021 01:17:41 GMT
ENV NATS_SERVER=2.2.1
# Sat, 03 Apr 2021 01:17:42 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.2.1/nats-server-v2.2.1-windows-amd64.zip
# Sat, 03 Apr 2021 01:17:43 GMT
ENV GIT_DOWNLOAD_SHA256=1f0d48a7ba9200e2572016a9f3e1ec7e630f0518cc0b40950c14ff3a5d900924
# Sat, 03 Apr 2021 01:19:05 GMT
RUN Set-PSDebug -Trace 2
# Sat, 03 Apr 2021 01:21:10 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Sat, 03 Apr 2021 01:21:11 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Sat, 03 Apr 2021 01:21:12 GMT
EXPOSE 4222 6222 8222
# Sat, 03 Apr 2021 01:21:13 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Sat, 03 Apr 2021 01:21:14 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:30bda99601c5cbd3b2118409f401852ea648e2319bd81518723e476b28d764c5`  
		Size: 1.7 GB (1726924885 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5205e01a19ce3835a7f1caba14b71dbbcae05a77274c60358d9794ee0e2a3e65`  
		Last Modified: Wed, 10 Mar 2021 16:23:35 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4390a91a59ec3760f5740301d69b960d0f0b7fb212a8bc2201b27b93b24d4054`  
		Last Modified: Wed, 10 Mar 2021 17:02:23 GMT  
		Size: 1.3 KB (1305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdf068626801ee0e0c0bd2b1a1f9e05e2d16d27757653ade2a5cc0d971764f50`  
		Last Modified: Sat, 03 Apr 2021 01:22:47 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36e3dd9e9e868f213575a6d17e3fda275a2d47d15e2f9d13ad6d206a0f8567a7`  
		Last Modified: Sat, 03 Apr 2021 01:22:47 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:657647c528aa33d6da248e5aeeb7babe0f7976361e1654d5920cdb0b6c4848b9`  
		Last Modified: Sat, 03 Apr 2021 01:22:47 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:389f475c113034c3ad6f5619cf1bc1b11fdad81b5e5e009ba573539909b23423`  
		Last Modified: Sat, 03 Apr 2021 01:22:48 GMT  
		Size: 5.7 MB (5656062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd7a05da95e65b18383e1ae5b037f3b75a628a6af2949313789b364e70c3e7dc`  
		Last Modified: Sat, 03 Apr 2021 01:22:48 GMT  
		Size: 14.4 MB (14447531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55d02d4cabb443df53f1d6f7a6f93f8f9dda642d034916077f4fab20c5632675`  
		Last Modified: Sat, 03 Apr 2021 01:22:44 GMT  
		Size: 2.0 KB (1974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06b93a0d4c513ec838b27546bad996f092605e9c8399ad016f78b8b4cb96a900`  
		Last Modified: Sat, 03 Apr 2021 01:22:44 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8317ff85679d749fdf54c66f1b278c9f16aa11a116c5c0d288bc4f8debe41262`  
		Last Modified: Sat, 03 Apr 2021 01:22:44 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b8b1e736261cff8c3afa409fd73d85b78d6610a610e3b8eb3412798d3a18348`  
		Last Modified: Sat, 03 Apr 2021 01:22:44 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:windowsservercore-1809`

```console
$ docker pull nats@sha256:f8a4f8888f531755c5711af4f90423afca2a36de1890ddd11b74df0dad4bd18c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1817; amd64

### `nats:windowsservercore-1809` - windows version 10.0.17763.1817; amd64

```console
$ docker pull nats@sha256:79eefa8948e2758f0659fb934899c37b05b67eb96c38b0e8c67c1a0974992423
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2480294595 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3875d7d95dfdb0356da902eee6142a19a85e38ae7ddde3bbf34b06e18765ecd7`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 27 Feb 2021 09:32:06 GMT
RUN Install update 1809-amd64
# Wed, 10 Mar 2021 14:15:30 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Mar 2021 16:54:55 GMT
ENV NATS_DOCKERIZED=1
# Sat, 03 Apr 2021 01:15:14 GMT
ENV NATS_SERVER=2.2.1
# Sat, 03 Apr 2021 01:15:16 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.2.1/nats-server-v2.2.1-windows-amd64.zip
# Sat, 03 Apr 2021 01:15:17 GMT
ENV GIT_DOWNLOAD_SHA256=1f0d48a7ba9200e2572016a9f3e1ec7e630f0518cc0b40950c14ff3a5d900924
# Sat, 03 Apr 2021 01:15:50 GMT
RUN Set-PSDebug -Trace 2
# Sat, 03 Apr 2021 01:17:04 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Sat, 03 Apr 2021 01:17:06 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Sat, 03 Apr 2021 01:17:07 GMT
EXPOSE 4222 6222 8222
# Sat, 03 Apr 2021 01:17:08 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Sat, 03 Apr 2021 01:17:09 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5ff1512f88ecd4ff0a91ade34d43733c48834433e35f062f80e6e70d706f8d73`  
		Size: 743.2 MB (743201590 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:31ae1fcdffac4071930a0d98172fc515a43c93aa55870e4b6cc8c789b9444e73`  
		Last Modified: Wed, 10 Mar 2021 16:22:41 GMT  
		Size: 1.3 KB (1305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cfde5dabd6353190a5343286e79ed9ad72f47f48ca9197e594b9771b5039e7d`  
		Last Modified: Wed, 10 Mar 2021 17:01:37 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4eb0ea2b178ae862896fca7bda0c5c677fd82870ca007ebe695e42f058831af`  
		Last Modified: Sat, 03 Apr 2021 01:22:03 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8c9d68c9aa9d29abd0c09f2016e9fcfc53bd185a7403989cec09108f661a977`  
		Last Modified: Sat, 03 Apr 2021 01:22:03 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b05ed1fd68964dcfc103f5452b7ee8528749d538e395dd36d17158cab031fdf`  
		Last Modified: Sat, 03 Apr 2021 01:22:03 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3994ed7efdb8fb7c71541583ff656c6c8e54e722284ec414d3ef00145cb43efa`  
		Last Modified: Sat, 03 Apr 2021 01:22:09 GMT  
		Size: 5.1 MB (5064967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0c3e4f395cd1bacff8cb6c6a451cfe4d56b4a054cfc15dd1a8b04a9e56240fa`  
		Last Modified: Sat, 03 Apr 2021 01:22:03 GMT  
		Size: 13.7 MB (13681925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bc88971a96126558018ca2f17f084db054369de555c8cb84a508c7a1394236e`  
		Last Modified: Sat, 03 Apr 2021 01:22:00 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66fa36b1a5dd3f83c94c4e1597659532cb557cd8f9cd414bb81f1049f39924af`  
		Last Modified: Sat, 03 Apr 2021 01:22:00 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4147b1dd2e59f8f133ab83ace94bf75ef78c0f9f261d49d65b7cc0b84d49438e`  
		Last Modified: Sat, 03 Apr 2021 01:22:00 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49b9455ff088b797d1cff54432e7f275092555cd8485bbf6b4aa926b88077f94`  
		Last Modified: Sat, 03 Apr 2021 01:22:00 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:windowsservercore-ltsc2016`

```console
$ docker pull nats@sha256:a29981e9b9b26371bed2856c6ac2b18e78e0ec9db3aeb251d0d8b281501c7196
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4283; amd64

### `nats:windowsservercore-ltsc2016` - windows version 10.0.14393.4283; amd64

```console
$ docker pull nats@sha256:ea694b06746523df91b7d824d0fc9030b282cc666bf34e937103b72b280d8a09
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5817027558 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:265f2ee0b7a998cc6ce663873648377be2b81226575d11ed5d1537b35a4118bf`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 03 Mar 2021 18:02:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Mar 2021 14:25:01 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Mar 2021 16:57:09 GMT
ENV NATS_DOCKERIZED=1
# Sat, 03 Apr 2021 01:17:41 GMT
ENV NATS_SERVER=2.2.1
# Sat, 03 Apr 2021 01:17:42 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.2.1/nats-server-v2.2.1-windows-amd64.zip
# Sat, 03 Apr 2021 01:17:43 GMT
ENV GIT_DOWNLOAD_SHA256=1f0d48a7ba9200e2572016a9f3e1ec7e630f0518cc0b40950c14ff3a5d900924
# Sat, 03 Apr 2021 01:19:05 GMT
RUN Set-PSDebug -Trace 2
# Sat, 03 Apr 2021 01:21:10 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Sat, 03 Apr 2021 01:21:11 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Sat, 03 Apr 2021 01:21:12 GMT
EXPOSE 4222 6222 8222
# Sat, 03 Apr 2021 01:21:13 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Sat, 03 Apr 2021 01:21:14 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:30bda99601c5cbd3b2118409f401852ea648e2319bd81518723e476b28d764c5`  
		Size: 1.7 GB (1726924885 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5205e01a19ce3835a7f1caba14b71dbbcae05a77274c60358d9794ee0e2a3e65`  
		Last Modified: Wed, 10 Mar 2021 16:23:35 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4390a91a59ec3760f5740301d69b960d0f0b7fb212a8bc2201b27b93b24d4054`  
		Last Modified: Wed, 10 Mar 2021 17:02:23 GMT  
		Size: 1.3 KB (1305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdf068626801ee0e0c0bd2b1a1f9e05e2d16d27757653ade2a5cc0d971764f50`  
		Last Modified: Sat, 03 Apr 2021 01:22:47 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36e3dd9e9e868f213575a6d17e3fda275a2d47d15e2f9d13ad6d206a0f8567a7`  
		Last Modified: Sat, 03 Apr 2021 01:22:47 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:657647c528aa33d6da248e5aeeb7babe0f7976361e1654d5920cdb0b6c4848b9`  
		Last Modified: Sat, 03 Apr 2021 01:22:47 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:389f475c113034c3ad6f5619cf1bc1b11fdad81b5e5e009ba573539909b23423`  
		Last Modified: Sat, 03 Apr 2021 01:22:48 GMT  
		Size: 5.7 MB (5656062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd7a05da95e65b18383e1ae5b037f3b75a628a6af2949313789b364e70c3e7dc`  
		Last Modified: Sat, 03 Apr 2021 01:22:48 GMT  
		Size: 14.4 MB (14447531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55d02d4cabb443df53f1d6f7a6f93f8f9dda642d034916077f4fab20c5632675`  
		Last Modified: Sat, 03 Apr 2021 01:22:44 GMT  
		Size: 2.0 KB (1974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06b93a0d4c513ec838b27546bad996f092605e9c8399ad016f78b8b4cb96a900`  
		Last Modified: Sat, 03 Apr 2021 01:22:44 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8317ff85679d749fdf54c66f1b278c9f16aa11a116c5c0d288bc4f8debe41262`  
		Last Modified: Sat, 03 Apr 2021 01:22:44 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b8b1e736261cff8c3afa409fd73d85b78d6610a610e3b8eb3412798d3a18348`  
		Last Modified: Sat, 03 Apr 2021 01:22:44 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
