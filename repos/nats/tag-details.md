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
$ docker pull nats@sha256:f0c80abcc8d86c26b77b4cfbf150821d7e71ace88e2ea39d8a5bfa33caf0317a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.1879; amd64

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

### `nats:2` - windows version 10.0.17763.1879; amd64

```console
$ docker pull nats@sha256:545e15088a9a48d35878789abdde98cb7a98627e5a7c3be56f42abb2e13632e8
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.6 MB (105608630 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19ac61d30cc1900a1011f83ffa5dbcfd15a0a1754f790b94bdded5ed0cd4b673`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 08 Apr 2021 16:02:06 GMT
RUN Apply image 1809-amd64
# Wed, 14 Apr 2021 16:05:18 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 14 Apr 2021 16:05:20 GMT
RUN cmd /S /C #(nop) COPY file:428a7e80db4313301a46326a9a79832e9cbe7d78c94e749b5c295e813e484f21 in C:\nats-server.exe 
# Wed, 14 Apr 2021 16:05:21 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 14 Apr 2021 16:05:22 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 14 Apr 2021 16:05:22 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 14 Apr 2021 16:05:23 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:ea84579f6cd5b58fe78732be37450bd188c8923de3a2062664f3992861449b5c`  
		Size: 101.3 MB (101340157 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f8d27bfefcaaa84a89f93945c61ccf0af9ad50b1405d9acfa30e9da5ba1fb2db`  
		Last Modified: Wed, 14 Apr 2021 16:10:39 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6f599ec3e67dbcacd5ebae06ae984f5a688eba397e2280187ee399da88dc6ad`  
		Last Modified: Wed, 14 Apr 2021 16:10:38 GMT  
		Size: 4.3 MB (4262107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:780b42108cdc95774ec8d8239a9027e7382a875cf25306df1b01363dd2dc7aa4`  
		Last Modified: Wed, 14 Apr 2021 16:10:37 GMT  
		Size: 1.8 KB (1758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b002edb80987b79bb224f75e7c65e924d45dc54e548ce835539ca82dcdcc08e6`  
		Last Modified: Wed, 14 Apr 2021 16:10:37 GMT  
		Size: 1.2 KB (1176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c148b88ce7ff0e645ebee08b98beb32730028b41f85296f22b03154fa54614ac`  
		Last Modified: Wed, 14 Apr 2021 16:10:37 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43dc978ed7937ca238d82c78779b6e3a605e64ba31e2a5adac73bc7da1f63ede`  
		Last Modified: Wed, 14 Apr 2021 16:10:37 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-alpine`

```console
$ docker pull nats@sha256:cb99fd7d7cb5b5ed625ef86f9e847c26cb6e7c13f970765e77da331d0a13959d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-alpine` - linux; amd64

```console
$ docker pull nats@sha256:7b78ce1b52f0b0421d7f722c642c9b0feb9d340b9b4896b0c638960863934a0e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7303896 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d14bc60ccc43c89281be8e1cb48cba172a1bc16e08228e9fed919e32c40e64e6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 23:12:59 GMT
ENV NATS_SERVER=2.2.1
# Wed, 14 Apr 2021 23:13:02 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='0123d924907282265190258662edf8ad4351055083b5040e3bdf59117bd1c51c' ;; 		armhf) natsArch='arm6'; sha256='da719b07fd57137f85bfa6cffc7d00841a9c1fb4cdf7ca9a537bfc3f99b71f36' ;; 		armv7) natsArch='arm7'; sha256='cf6e8d9a9cc5d05f7320fb4be8fc9239cb87b91c6600a61ce7a2fb63e2f29f5a' ;; 		x86_64) natsArch='amd64'; sha256='70cb40d78b82ea6c0ca926c31ef98d2e1c885cfe2f73f34883e4ca448366c2dd' ;; 		x86) natsArch='386'; sha256='da54d129f8a52c048ded61e3b62e946037a9464d02cf818e568bbf1e385ce6be' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 14 Apr 2021 23:13:02 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Wed, 14 Apr 2021 23:13:02 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 14 Apr 2021 23:13:03 GMT
EXPOSE 4222 6222 8222
# Wed, 14 Apr 2021 23:13:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 23:13:03 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adf2b83a147ab10f7ee92b0624d9beb0101ff40b27dd92a1e74ec3bc972fa9f8`  
		Last Modified: Wed, 14 Apr 2021 23:13:45 GMT  
		Size: 4.5 MB (4490957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab1824f686e6029870ed0b1328708bbfe11b2c3b1bac6a461604b830ffdc13ce`  
		Last Modified: Wed, 14 Apr 2021 23:13:44 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:357bc9de7de4490d1629a64200e10f44bf96da1168b66f8bb512a3ce9d68bc23`  
		Last Modified: Wed, 14 Apr 2021 23:13:44 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:eb3c514a433f020cd80da54de5a877d42c7f8aef888eef6fcf72b0175626cbd1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6784935 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:abd439f99c0768fd1ea54123118765e2c3a5e6f7e7f44c358794ce23c8590216`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Apr 2021 18:49:39 GMT
ADD file:4479f0a51530e039edf231d87201896dcff908aa542a613cdccb015f93dda8a3 in / 
# Wed, 14 Apr 2021 18:49:40 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 21:48:34 GMT
ENV NATS_SERVER=2.2.1
# Wed, 14 Apr 2021 21:49:16 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='0123d924907282265190258662edf8ad4351055083b5040e3bdf59117bd1c51c' ;; 		armhf) natsArch='arm6'; sha256='da719b07fd57137f85bfa6cffc7d00841a9c1fb4cdf7ca9a537bfc3f99b71f36' ;; 		armv7) natsArch='arm7'; sha256='cf6e8d9a9cc5d05f7320fb4be8fc9239cb87b91c6600a61ce7a2fb63e2f29f5a' ;; 		x86_64) natsArch='amd64'; sha256='70cb40d78b82ea6c0ca926c31ef98d2e1c885cfe2f73f34883e4ca448366c2dd' ;; 		x86) natsArch='386'; sha256='da54d129f8a52c048ded61e3b62e946037a9464d02cf818e568bbf1e385ce6be' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 14 Apr 2021 21:49:31 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Wed, 14 Apr 2021 21:49:41 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 14 Apr 2021 21:49:50 GMT
EXPOSE 4222 6222 8222
# Wed, 14 Apr 2021 21:49:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 21:50:03 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:740c950346cf39c85b52576998695c9b909c24a58a8bb1b64cce91fda3ef1d3a`  
		Last Modified: Wed, 14 Apr 2021 18:50:30 GMT  
		Size: 2.6 MB (2622131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22164d2f45f59e8f1d873e8a0c4769559100e469dc09c3bcbb61163732b2f453`  
		Last Modified: Wed, 14 Apr 2021 21:52:09 GMT  
		Size: 4.2 MB (4161829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79de2833ed16322bc62170a748bd3d746b8b152ec85cffa0cd11a3c25d822b35`  
		Last Modified: Wed, 14 Apr 2021 21:52:06 GMT  
		Size: 561.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f686c25c87f7ee66f2990e18510448fe0a0063432d6f894bd1a1b0917eaf37a`  
		Last Modified: Wed, 14 Apr 2021 21:52:09 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:65016cde6a860e4e53a844e66d8944c0b72583aff8b0f17940f5883ce2025337
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6583191 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd85ddd622c92403cb491019f78c2760f9a3938378dadba44b3d1e382b1dd1db`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Apr 2021 18:57:39 GMT
ADD file:028c5b473d862250586e174c5dd19b37f8fc3bffbc02d888e72df30f32fd6129 in / 
# Wed, 14 Apr 2021 18:57:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 23:17:51 GMT
ENV NATS_SERVER=2.2.1
# Wed, 14 Apr 2021 23:17:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='0123d924907282265190258662edf8ad4351055083b5040e3bdf59117bd1c51c' ;; 		armhf) natsArch='arm6'; sha256='da719b07fd57137f85bfa6cffc7d00841a9c1fb4cdf7ca9a537bfc3f99b71f36' ;; 		armv7) natsArch='arm7'; sha256='cf6e8d9a9cc5d05f7320fb4be8fc9239cb87b91c6600a61ce7a2fb63e2f29f5a' ;; 		x86_64) natsArch='amd64'; sha256='70cb40d78b82ea6c0ca926c31ef98d2e1c885cfe2f73f34883e4ca448366c2dd' ;; 		x86) natsArch='386'; sha256='da54d129f8a52c048ded61e3b62e946037a9464d02cf818e568bbf1e385ce6be' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 14 Apr 2021 23:18:00 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Wed, 14 Apr 2021 23:18:02 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 14 Apr 2021 23:18:04 GMT
EXPOSE 4222 6222 8222
# Wed, 14 Apr 2021 23:18:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 23:18:09 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:e160e00eb35d5bc2373770873fbc9c8f5706045b0b06bfd1c364fcf69f02e9fe`  
		Last Modified: Wed, 14 Apr 2021 18:58:36 GMT  
		Size: 2.4 MB (2424145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3691a766339eab5091760e8ff801b39c69452b17fdd4fbd0e0cd710d241b5c5`  
		Last Modified: Wed, 14 Apr 2021 23:19:04 GMT  
		Size: 4.2 MB (4158072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a272e5ab96f7d43eb8e116aedf9e11bc1280f7ce6fbc83d2cbd82506c9ad760`  
		Last Modified: Wed, 14 Apr 2021 23:19:02 GMT  
		Size: 562.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e5adcdbbba76bad23d4bf8413449ce3ae2e70365468c47978d2c4ba7b937a67`  
		Last Modified: Wed, 14 Apr 2021 23:19:02 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:643201294279426bb51217496fc5e4053f55c0b29010efea1f201918efa1544a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6844402 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fd51943be05be331bd2fbd7b2494b10525553a8590e7041cda0723402b5d281a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Apr 2021 18:42:37 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Wed, 14 Apr 2021 18:42:38 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 23:37:11 GMT
ENV NATS_SERVER=2.2.1
# Wed, 14 Apr 2021 23:37:17 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='0123d924907282265190258662edf8ad4351055083b5040e3bdf59117bd1c51c' ;; 		armhf) natsArch='arm6'; sha256='da719b07fd57137f85bfa6cffc7d00841a9c1fb4cdf7ca9a537bfc3f99b71f36' ;; 		armv7) natsArch='arm7'; sha256='cf6e8d9a9cc5d05f7320fb4be8fc9239cb87b91c6600a61ce7a2fb63e2f29f5a' ;; 		x86_64) natsArch='amd64'; sha256='70cb40d78b82ea6c0ca926c31ef98d2e1c885cfe2f73f34883e4ca448366c2dd' ;; 		x86) natsArch='386'; sha256='da54d129f8a52c048ded61e3b62e946037a9464d02cf818e568bbf1e385ce6be' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 14 Apr 2021 23:37:18 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Wed, 14 Apr 2021 23:37:20 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 14 Apr 2021 23:37:25 GMT
EXPOSE 4222 6222 8222
# Wed, 14 Apr 2021 23:37:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 23:37:27 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:305503c7404cab7cb3fe558afe5d1b142f71b61815abb7d5b545be5d6fd274da`  
		Last Modified: Wed, 14 Apr 2021 23:41:37 GMT  
		Size: 4.1 MB (4131404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9504bc3187f368a20d4fe0020479a23dd57f07ea67deeb351297f4a8f1252dd7`  
		Last Modified: Wed, 14 Apr 2021 23:41:35 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0889a2e36f7ca1635400c49238cbb554ad2519b4a2c2cbfacff8cf2a1e21acd1`  
		Last Modified: Wed, 14 Apr 2021 23:41:35 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-alpine3.13`

```console
$ docker pull nats@sha256:cb99fd7d7cb5b5ed625ef86f9e847c26cb6e7c13f970765e77da331d0a13959d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-alpine3.13` - linux; amd64

```console
$ docker pull nats@sha256:7b78ce1b52f0b0421d7f722c642c9b0feb9d340b9b4896b0c638960863934a0e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7303896 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d14bc60ccc43c89281be8e1cb48cba172a1bc16e08228e9fed919e32c40e64e6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 23:12:59 GMT
ENV NATS_SERVER=2.2.1
# Wed, 14 Apr 2021 23:13:02 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='0123d924907282265190258662edf8ad4351055083b5040e3bdf59117bd1c51c' ;; 		armhf) natsArch='arm6'; sha256='da719b07fd57137f85bfa6cffc7d00841a9c1fb4cdf7ca9a537bfc3f99b71f36' ;; 		armv7) natsArch='arm7'; sha256='cf6e8d9a9cc5d05f7320fb4be8fc9239cb87b91c6600a61ce7a2fb63e2f29f5a' ;; 		x86_64) natsArch='amd64'; sha256='70cb40d78b82ea6c0ca926c31ef98d2e1c885cfe2f73f34883e4ca448366c2dd' ;; 		x86) natsArch='386'; sha256='da54d129f8a52c048ded61e3b62e946037a9464d02cf818e568bbf1e385ce6be' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 14 Apr 2021 23:13:02 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Wed, 14 Apr 2021 23:13:02 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 14 Apr 2021 23:13:03 GMT
EXPOSE 4222 6222 8222
# Wed, 14 Apr 2021 23:13:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 23:13:03 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adf2b83a147ab10f7ee92b0624d9beb0101ff40b27dd92a1e74ec3bc972fa9f8`  
		Last Modified: Wed, 14 Apr 2021 23:13:45 GMT  
		Size: 4.5 MB (4490957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab1824f686e6029870ed0b1328708bbfe11b2c3b1bac6a461604b830ffdc13ce`  
		Last Modified: Wed, 14 Apr 2021 23:13:44 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:357bc9de7de4490d1629a64200e10f44bf96da1168b66f8bb512a3ce9d68bc23`  
		Last Modified: Wed, 14 Apr 2021 23:13:44 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.13` - linux; arm variant v6

```console
$ docker pull nats@sha256:eb3c514a433f020cd80da54de5a877d42c7f8aef888eef6fcf72b0175626cbd1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6784935 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:abd439f99c0768fd1ea54123118765e2c3a5e6f7e7f44c358794ce23c8590216`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Apr 2021 18:49:39 GMT
ADD file:4479f0a51530e039edf231d87201896dcff908aa542a613cdccb015f93dda8a3 in / 
# Wed, 14 Apr 2021 18:49:40 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 21:48:34 GMT
ENV NATS_SERVER=2.2.1
# Wed, 14 Apr 2021 21:49:16 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='0123d924907282265190258662edf8ad4351055083b5040e3bdf59117bd1c51c' ;; 		armhf) natsArch='arm6'; sha256='da719b07fd57137f85bfa6cffc7d00841a9c1fb4cdf7ca9a537bfc3f99b71f36' ;; 		armv7) natsArch='arm7'; sha256='cf6e8d9a9cc5d05f7320fb4be8fc9239cb87b91c6600a61ce7a2fb63e2f29f5a' ;; 		x86_64) natsArch='amd64'; sha256='70cb40d78b82ea6c0ca926c31ef98d2e1c885cfe2f73f34883e4ca448366c2dd' ;; 		x86) natsArch='386'; sha256='da54d129f8a52c048ded61e3b62e946037a9464d02cf818e568bbf1e385ce6be' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 14 Apr 2021 21:49:31 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Wed, 14 Apr 2021 21:49:41 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 14 Apr 2021 21:49:50 GMT
EXPOSE 4222 6222 8222
# Wed, 14 Apr 2021 21:49:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 21:50:03 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:740c950346cf39c85b52576998695c9b909c24a58a8bb1b64cce91fda3ef1d3a`  
		Last Modified: Wed, 14 Apr 2021 18:50:30 GMT  
		Size: 2.6 MB (2622131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22164d2f45f59e8f1d873e8a0c4769559100e469dc09c3bcbb61163732b2f453`  
		Last Modified: Wed, 14 Apr 2021 21:52:09 GMT  
		Size: 4.2 MB (4161829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79de2833ed16322bc62170a748bd3d746b8b152ec85cffa0cd11a3c25d822b35`  
		Last Modified: Wed, 14 Apr 2021 21:52:06 GMT  
		Size: 561.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f686c25c87f7ee66f2990e18510448fe0a0063432d6f894bd1a1b0917eaf37a`  
		Last Modified: Wed, 14 Apr 2021 21:52:09 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.13` - linux; arm variant v7

```console
$ docker pull nats@sha256:65016cde6a860e4e53a844e66d8944c0b72583aff8b0f17940f5883ce2025337
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6583191 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd85ddd622c92403cb491019f78c2760f9a3938378dadba44b3d1e382b1dd1db`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Apr 2021 18:57:39 GMT
ADD file:028c5b473d862250586e174c5dd19b37f8fc3bffbc02d888e72df30f32fd6129 in / 
# Wed, 14 Apr 2021 18:57:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 23:17:51 GMT
ENV NATS_SERVER=2.2.1
# Wed, 14 Apr 2021 23:17:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='0123d924907282265190258662edf8ad4351055083b5040e3bdf59117bd1c51c' ;; 		armhf) natsArch='arm6'; sha256='da719b07fd57137f85bfa6cffc7d00841a9c1fb4cdf7ca9a537bfc3f99b71f36' ;; 		armv7) natsArch='arm7'; sha256='cf6e8d9a9cc5d05f7320fb4be8fc9239cb87b91c6600a61ce7a2fb63e2f29f5a' ;; 		x86_64) natsArch='amd64'; sha256='70cb40d78b82ea6c0ca926c31ef98d2e1c885cfe2f73f34883e4ca448366c2dd' ;; 		x86) natsArch='386'; sha256='da54d129f8a52c048ded61e3b62e946037a9464d02cf818e568bbf1e385ce6be' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 14 Apr 2021 23:18:00 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Wed, 14 Apr 2021 23:18:02 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 14 Apr 2021 23:18:04 GMT
EXPOSE 4222 6222 8222
# Wed, 14 Apr 2021 23:18:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 23:18:09 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:e160e00eb35d5bc2373770873fbc9c8f5706045b0b06bfd1c364fcf69f02e9fe`  
		Last Modified: Wed, 14 Apr 2021 18:58:36 GMT  
		Size: 2.4 MB (2424145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3691a766339eab5091760e8ff801b39c69452b17fdd4fbd0e0cd710d241b5c5`  
		Last Modified: Wed, 14 Apr 2021 23:19:04 GMT  
		Size: 4.2 MB (4158072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a272e5ab96f7d43eb8e116aedf9e11bc1280f7ce6fbc83d2cbd82506c9ad760`  
		Last Modified: Wed, 14 Apr 2021 23:19:02 GMT  
		Size: 562.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e5adcdbbba76bad23d4bf8413449ce3ae2e70365468c47978d2c4ba7b937a67`  
		Last Modified: Wed, 14 Apr 2021 23:19:02 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.13` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:643201294279426bb51217496fc5e4053f55c0b29010efea1f201918efa1544a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6844402 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fd51943be05be331bd2fbd7b2494b10525553a8590e7041cda0723402b5d281a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Apr 2021 18:42:37 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Wed, 14 Apr 2021 18:42:38 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 23:37:11 GMT
ENV NATS_SERVER=2.2.1
# Wed, 14 Apr 2021 23:37:17 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='0123d924907282265190258662edf8ad4351055083b5040e3bdf59117bd1c51c' ;; 		armhf) natsArch='arm6'; sha256='da719b07fd57137f85bfa6cffc7d00841a9c1fb4cdf7ca9a537bfc3f99b71f36' ;; 		armv7) natsArch='arm7'; sha256='cf6e8d9a9cc5d05f7320fb4be8fc9239cb87b91c6600a61ce7a2fb63e2f29f5a' ;; 		x86_64) natsArch='amd64'; sha256='70cb40d78b82ea6c0ca926c31ef98d2e1c885cfe2f73f34883e4ca448366c2dd' ;; 		x86) natsArch='386'; sha256='da54d129f8a52c048ded61e3b62e946037a9464d02cf818e568bbf1e385ce6be' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 14 Apr 2021 23:37:18 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Wed, 14 Apr 2021 23:37:20 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 14 Apr 2021 23:37:25 GMT
EXPOSE 4222 6222 8222
# Wed, 14 Apr 2021 23:37:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 23:37:27 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:305503c7404cab7cb3fe558afe5d1b142f71b61815abb7d5b545be5d6fd274da`  
		Last Modified: Wed, 14 Apr 2021 23:41:37 GMT  
		Size: 4.1 MB (4131404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9504bc3187f368a20d4fe0020479a23dd57f07ea67deeb351297f4a8f1252dd7`  
		Last Modified: Wed, 14 Apr 2021 23:41:35 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0889a2e36f7ca1635400c49238cbb554ad2519b4a2c2cbfacff8cf2a1e21acd1`  
		Last Modified: Wed, 14 Apr 2021 23:41:35 GMT  
		Size: 414.0 B  
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
$ docker pull nats@sha256:236c67f0c205b9cfab2809ce1dea44a20258d371c82264afd3172f29c8c70fb1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1879; amd64

### `nats:2-nanoserver` - windows version 10.0.17763.1879; amd64

```console
$ docker pull nats@sha256:545e15088a9a48d35878789abdde98cb7a98627e5a7c3be56f42abb2e13632e8
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.6 MB (105608630 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19ac61d30cc1900a1011f83ffa5dbcfd15a0a1754f790b94bdded5ed0cd4b673`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 08 Apr 2021 16:02:06 GMT
RUN Apply image 1809-amd64
# Wed, 14 Apr 2021 16:05:18 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 14 Apr 2021 16:05:20 GMT
RUN cmd /S /C #(nop) COPY file:428a7e80db4313301a46326a9a79832e9cbe7d78c94e749b5c295e813e484f21 in C:\nats-server.exe 
# Wed, 14 Apr 2021 16:05:21 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 14 Apr 2021 16:05:22 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 14 Apr 2021 16:05:22 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 14 Apr 2021 16:05:23 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:ea84579f6cd5b58fe78732be37450bd188c8923de3a2062664f3992861449b5c`  
		Size: 101.3 MB (101340157 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f8d27bfefcaaa84a89f93945c61ccf0af9ad50b1405d9acfa30e9da5ba1fb2db`  
		Last Modified: Wed, 14 Apr 2021 16:10:39 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6f599ec3e67dbcacd5ebae06ae984f5a688eba397e2280187ee399da88dc6ad`  
		Last Modified: Wed, 14 Apr 2021 16:10:38 GMT  
		Size: 4.3 MB (4262107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:780b42108cdc95774ec8d8239a9027e7382a875cf25306df1b01363dd2dc7aa4`  
		Last Modified: Wed, 14 Apr 2021 16:10:37 GMT  
		Size: 1.8 KB (1758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b002edb80987b79bb224f75e7c65e924d45dc54e548ce835539ca82dcdcc08e6`  
		Last Modified: Wed, 14 Apr 2021 16:10:37 GMT  
		Size: 1.2 KB (1176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c148b88ce7ff0e645ebee08b98beb32730028b41f85296f22b03154fa54614ac`  
		Last Modified: Wed, 14 Apr 2021 16:10:37 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43dc978ed7937ca238d82c78779b6e3a605e64ba31e2a5adac73bc7da1f63ede`  
		Last Modified: Wed, 14 Apr 2021 16:10:37 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-nanoserver-1809`

```console
$ docker pull nats@sha256:236c67f0c205b9cfab2809ce1dea44a20258d371c82264afd3172f29c8c70fb1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1879; amd64

### `nats:2-nanoserver-1809` - windows version 10.0.17763.1879; amd64

```console
$ docker pull nats@sha256:545e15088a9a48d35878789abdde98cb7a98627e5a7c3be56f42abb2e13632e8
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.6 MB (105608630 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19ac61d30cc1900a1011f83ffa5dbcfd15a0a1754f790b94bdded5ed0cd4b673`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 08 Apr 2021 16:02:06 GMT
RUN Apply image 1809-amd64
# Wed, 14 Apr 2021 16:05:18 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 14 Apr 2021 16:05:20 GMT
RUN cmd /S /C #(nop) COPY file:428a7e80db4313301a46326a9a79832e9cbe7d78c94e749b5c295e813e484f21 in C:\nats-server.exe 
# Wed, 14 Apr 2021 16:05:21 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 14 Apr 2021 16:05:22 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 14 Apr 2021 16:05:22 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 14 Apr 2021 16:05:23 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:ea84579f6cd5b58fe78732be37450bd188c8923de3a2062664f3992861449b5c`  
		Size: 101.3 MB (101340157 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f8d27bfefcaaa84a89f93945c61ccf0af9ad50b1405d9acfa30e9da5ba1fb2db`  
		Last Modified: Wed, 14 Apr 2021 16:10:39 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6f599ec3e67dbcacd5ebae06ae984f5a688eba397e2280187ee399da88dc6ad`  
		Last Modified: Wed, 14 Apr 2021 16:10:38 GMT  
		Size: 4.3 MB (4262107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:780b42108cdc95774ec8d8239a9027e7382a875cf25306df1b01363dd2dc7aa4`  
		Last Modified: Wed, 14 Apr 2021 16:10:37 GMT  
		Size: 1.8 KB (1758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b002edb80987b79bb224f75e7c65e924d45dc54e548ce835539ca82dcdcc08e6`  
		Last Modified: Wed, 14 Apr 2021 16:10:37 GMT  
		Size: 1.2 KB (1176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c148b88ce7ff0e645ebee08b98beb32730028b41f85296f22b03154fa54614ac`  
		Last Modified: Wed, 14 Apr 2021 16:10:37 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43dc978ed7937ca238d82c78779b6e3a605e64ba31e2a5adac73bc7da1f63ede`  
		Last Modified: Wed, 14 Apr 2021 16:10:37 GMT  
		Size: 1.1 KB (1149 bytes)  
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
$ docker pull nats@sha256:a6c1153fd919a539581471edd798478057cef10a6347e770d03336a20d5e472b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1879; amd64
	-	windows version 10.0.14393.4350; amd64

### `nats:2-windowsservercore` - windows version 10.0.17763.1879; amd64

```console
$ docker pull nats@sha256:9f3868f133ddd1a10ac71bbe835764e9d60e9b00081851a00ca05cd3362ea5d1
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2484142070 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2be425426bfa101eb4fdc6741eccbeaddde31c6c0761a665b4654dea39a17279`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 09 Apr 2021 20:34:41 GMT
RUN Install update 1809-amd64
# Wed, 14 Apr 2021 13:10:28 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 14 Apr 2021 16:02:50 GMT
ENV NATS_DOCKERIZED=1
# Wed, 14 Apr 2021 16:02:51 GMT
ENV NATS_SERVER=2.2.1
# Wed, 14 Apr 2021 16:02:52 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.2.1/nats-server-v2.2.1-windows-amd64.zip
# Wed, 14 Apr 2021 16:02:53 GMT
ENV GIT_DOWNLOAD_SHA256=1f0d48a7ba9200e2572016a9f3e1ec7e630f0518cc0b40950c14ff3a5d900924
# Wed, 14 Apr 2021 16:03:32 GMT
RUN Set-PSDebug -Trace 2
# Wed, 14 Apr 2021 16:04:53 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 14 Apr 2021 16:04:55 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 14 Apr 2021 16:04:56 GMT
EXPOSE 4222 6222 8222
# Wed, 14 Apr 2021 16:04:57 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 14 Apr 2021 16:04:58 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:399f118dfaa9a753e98d128238b944432c7bcabea88a2998a6efbbece28ed303`  
		Size: 751.4 MB (751421005 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b2159a5d0f75ce11e6fe71e4260ede5c3c88a9eb76a0ff43ac6746b2b9b96775`  
		Last Modified: Wed, 14 Apr 2021 15:37:10 GMT  
		Size: 1.4 KB (1446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e849354f21f856ec720d6daecc37978fd7246f376ba3c32fd63d4400cce357bc`  
		Last Modified: Wed, 14 Apr 2021 16:10:16 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daae5ee02f484d7c054ad550cbee6900a35477f4e23e322cc3af6eb7c4690416`  
		Last Modified: Wed, 14 Apr 2021 16:10:14 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d4df8575d5fc511a7ac278cfc55a4053b36afce4c0bcae2af0af7907c7f91e6`  
		Last Modified: Wed, 14 Apr 2021 16:10:14 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:570a7e5edba00d92281a4a147639b5fc0b6724693cbfed80007b5b5db612a3e8`  
		Last Modified: Wed, 14 Apr 2021 16:10:13 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60092b7b0679ad17236eb09b832adcc7bb67a5fd8c2d9a69ffbfc863716274c2`  
		Last Modified: Wed, 14 Apr 2021 16:10:15 GMT  
		Size: 5.1 MB (5072726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d5d3b99689d155ccd6cdf6acbc7ef61472c65ce2cee49f441c4c3b844242410`  
		Last Modified: Wed, 14 Apr 2021 16:10:13 GMT  
		Size: 9.3 MB (9302175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23dae780c7132cf39c97d1602e11b6a58481594df6d896054f3a9e6e9f54e63a`  
		Last Modified: Wed, 14 Apr 2021 16:10:10 GMT  
		Size: 2.0 KB (1957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95f2291e14ae4d6e97942f3284122a80c7c969cb9bcfc9a417a833439505f85d`  
		Last Modified: Wed, 14 Apr 2021 16:10:11 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69b07be56d63a82b0606023df13bf32a522a13a12a44c53116ec24d0c1bd2ca1`  
		Last Modified: Wed, 14 Apr 2021 16:10:11 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb6cc0327d5edba60d3e99a97fa6c015e1953c9451bc816f20d6d73a67b9e426`  
		Last Modified: Wed, 14 Apr 2021 16:10:11 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-windowsservercore` - windows version 10.0.14393.4350; amd64

```console
$ docker pull nats@sha256:ad5ac25aa423d2df82324037dd73fec641098cd5f198cf98ccf19f4ae640d1f5
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5814950471 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0fc9b58b0a6e7d867ee74a6023bf1768d2dad684760ace428c0bf425357fcc5c`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 07 Apr 2021 21:54:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 14 Apr 2021 13:22:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 14 Apr 2021 16:05:33 GMT
ENV NATS_DOCKERIZED=1
# Wed, 14 Apr 2021 16:05:33 GMT
ENV NATS_SERVER=2.2.1
# Wed, 14 Apr 2021 16:05:35 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.2.1/nats-server-v2.2.1-windows-amd64.zip
# Wed, 14 Apr 2021 16:05:35 GMT
ENV GIT_DOWNLOAD_SHA256=1f0d48a7ba9200e2572016a9f3e1ec7e630f0518cc0b40950c14ff3a5d900924
# Wed, 14 Apr 2021 16:06:59 GMT
RUN Set-PSDebug -Trace 2
# Wed, 14 Apr 2021 16:09:18 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 14 Apr 2021 16:09:19 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 14 Apr 2021 16:09:20 GMT
EXPOSE 4222 6222 8222
# Wed, 14 Apr 2021 16:09:21 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 14 Apr 2021 16:09:23 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:00b4edb823e6a375d179a28cbfa682c2379d62179e1518485902d6e68b9a9d1e`  
		Size: 1.7 GB (1724897968 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f616bb7876e6f944d82fa1802ffab5ca4931a63e1b999f0851b52120cda83539`  
		Last Modified: Wed, 14 Apr 2021 15:37:43 GMT  
		Size: 1.3 KB (1307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcfa54f43457753c391f21da5e9a5bf47c61c574c0da04b8614d0e84bf823f54`  
		Last Modified: Wed, 14 Apr 2021 16:11:03 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04d71ba1c574073f9d5dd016585c2fe26ac560c192f7aa36ce54d4c12832997f`  
		Last Modified: Wed, 14 Apr 2021 16:11:01 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e9f66539738348100cf9f1e6a5bc40e8c2123bafb9329f5df3cf20a2015db33`  
		Last Modified: Wed, 14 Apr 2021 16:11:00 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20f2eae922462b2537c1d0d32d548cb10190f6bda0d02da57440cc229da692b3`  
		Last Modified: Wed, 14 Apr 2021 16:11:00 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ea168f84532f340be87f19704511ee160cbdc5b9c6ad8962fcd80e9fb8efea7`  
		Last Modified: Wed, 14 Apr 2021 16:11:01 GMT  
		Size: 5.7 MB (5651953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2eda2d9556eb5afaf10e6300ac36ddc1383144ae65671ca3a01b24bac150c540`  
		Last Modified: Wed, 14 Apr 2021 16:11:01 GMT  
		Size: 14.4 MB (14401439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a04b0d9d602bb1f9c6fb7925bb92959ebcff2c30e6ca6a658cdd9976d662d70`  
		Last Modified: Wed, 14 Apr 2021 16:10:57 GMT  
		Size: 2.0 KB (1984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e5e865356a464c9006414a165a6d0ffb8f062fa737be2ad42e1aa58fcfca23c`  
		Last Modified: Wed, 14 Apr 2021 16:10:56 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3533148ddde03cc5f28669b26c30dee8685db418d250a4b4829e465c0be8a7e`  
		Last Modified: Wed, 14 Apr 2021 16:10:56 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4573099491ec9887bd66033f55b39f6b897d1f59f21f679fdff4f822ebd7ea15`  
		Last Modified: Wed, 14 Apr 2021 16:10:56 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-windowsservercore-1809`

```console
$ docker pull nats@sha256:3002e35b4bb91080eac08408891e6bb9155d38086cbb6fcfb654b61e0d2383e0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1879; amd64

### `nats:2-windowsservercore-1809` - windows version 10.0.17763.1879; amd64

```console
$ docker pull nats@sha256:9f3868f133ddd1a10ac71bbe835764e9d60e9b00081851a00ca05cd3362ea5d1
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2484142070 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2be425426bfa101eb4fdc6741eccbeaddde31c6c0761a665b4654dea39a17279`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 09 Apr 2021 20:34:41 GMT
RUN Install update 1809-amd64
# Wed, 14 Apr 2021 13:10:28 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 14 Apr 2021 16:02:50 GMT
ENV NATS_DOCKERIZED=1
# Wed, 14 Apr 2021 16:02:51 GMT
ENV NATS_SERVER=2.2.1
# Wed, 14 Apr 2021 16:02:52 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.2.1/nats-server-v2.2.1-windows-amd64.zip
# Wed, 14 Apr 2021 16:02:53 GMT
ENV GIT_DOWNLOAD_SHA256=1f0d48a7ba9200e2572016a9f3e1ec7e630f0518cc0b40950c14ff3a5d900924
# Wed, 14 Apr 2021 16:03:32 GMT
RUN Set-PSDebug -Trace 2
# Wed, 14 Apr 2021 16:04:53 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 14 Apr 2021 16:04:55 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 14 Apr 2021 16:04:56 GMT
EXPOSE 4222 6222 8222
# Wed, 14 Apr 2021 16:04:57 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 14 Apr 2021 16:04:58 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:399f118dfaa9a753e98d128238b944432c7bcabea88a2998a6efbbece28ed303`  
		Size: 751.4 MB (751421005 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b2159a5d0f75ce11e6fe71e4260ede5c3c88a9eb76a0ff43ac6746b2b9b96775`  
		Last Modified: Wed, 14 Apr 2021 15:37:10 GMT  
		Size: 1.4 KB (1446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e849354f21f856ec720d6daecc37978fd7246f376ba3c32fd63d4400cce357bc`  
		Last Modified: Wed, 14 Apr 2021 16:10:16 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daae5ee02f484d7c054ad550cbee6900a35477f4e23e322cc3af6eb7c4690416`  
		Last Modified: Wed, 14 Apr 2021 16:10:14 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d4df8575d5fc511a7ac278cfc55a4053b36afce4c0bcae2af0af7907c7f91e6`  
		Last Modified: Wed, 14 Apr 2021 16:10:14 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:570a7e5edba00d92281a4a147639b5fc0b6724693cbfed80007b5b5db612a3e8`  
		Last Modified: Wed, 14 Apr 2021 16:10:13 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60092b7b0679ad17236eb09b832adcc7bb67a5fd8c2d9a69ffbfc863716274c2`  
		Last Modified: Wed, 14 Apr 2021 16:10:15 GMT  
		Size: 5.1 MB (5072726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d5d3b99689d155ccd6cdf6acbc7ef61472c65ce2cee49f441c4c3b844242410`  
		Last Modified: Wed, 14 Apr 2021 16:10:13 GMT  
		Size: 9.3 MB (9302175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23dae780c7132cf39c97d1602e11b6a58481594df6d896054f3a9e6e9f54e63a`  
		Last Modified: Wed, 14 Apr 2021 16:10:10 GMT  
		Size: 2.0 KB (1957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95f2291e14ae4d6e97942f3284122a80c7c969cb9bcfc9a417a833439505f85d`  
		Last Modified: Wed, 14 Apr 2021 16:10:11 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69b07be56d63a82b0606023df13bf32a522a13a12a44c53116ec24d0c1bd2ca1`  
		Last Modified: Wed, 14 Apr 2021 16:10:11 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb6cc0327d5edba60d3e99a97fa6c015e1953c9451bc816f20d6d73a67b9e426`  
		Last Modified: Wed, 14 Apr 2021 16:10:11 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-windowsservercore-ltsc2016`

```console
$ docker pull nats@sha256:486439b61d7c8307b15b01bae5f574784e333ee642d1d3285e3bf61785ea00cd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4350; amd64

### `nats:2-windowsservercore-ltsc2016` - windows version 10.0.14393.4350; amd64

```console
$ docker pull nats@sha256:ad5ac25aa423d2df82324037dd73fec641098cd5f198cf98ccf19f4ae640d1f5
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5814950471 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0fc9b58b0a6e7d867ee74a6023bf1768d2dad684760ace428c0bf425357fcc5c`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 07 Apr 2021 21:54:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 14 Apr 2021 13:22:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 14 Apr 2021 16:05:33 GMT
ENV NATS_DOCKERIZED=1
# Wed, 14 Apr 2021 16:05:33 GMT
ENV NATS_SERVER=2.2.1
# Wed, 14 Apr 2021 16:05:35 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.2.1/nats-server-v2.2.1-windows-amd64.zip
# Wed, 14 Apr 2021 16:05:35 GMT
ENV GIT_DOWNLOAD_SHA256=1f0d48a7ba9200e2572016a9f3e1ec7e630f0518cc0b40950c14ff3a5d900924
# Wed, 14 Apr 2021 16:06:59 GMT
RUN Set-PSDebug -Trace 2
# Wed, 14 Apr 2021 16:09:18 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 14 Apr 2021 16:09:19 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 14 Apr 2021 16:09:20 GMT
EXPOSE 4222 6222 8222
# Wed, 14 Apr 2021 16:09:21 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 14 Apr 2021 16:09:23 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:00b4edb823e6a375d179a28cbfa682c2379d62179e1518485902d6e68b9a9d1e`  
		Size: 1.7 GB (1724897968 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f616bb7876e6f944d82fa1802ffab5ca4931a63e1b999f0851b52120cda83539`  
		Last Modified: Wed, 14 Apr 2021 15:37:43 GMT  
		Size: 1.3 KB (1307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcfa54f43457753c391f21da5e9a5bf47c61c574c0da04b8614d0e84bf823f54`  
		Last Modified: Wed, 14 Apr 2021 16:11:03 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04d71ba1c574073f9d5dd016585c2fe26ac560c192f7aa36ce54d4c12832997f`  
		Last Modified: Wed, 14 Apr 2021 16:11:01 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e9f66539738348100cf9f1e6a5bc40e8c2123bafb9329f5df3cf20a2015db33`  
		Last Modified: Wed, 14 Apr 2021 16:11:00 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20f2eae922462b2537c1d0d32d548cb10190f6bda0d02da57440cc229da692b3`  
		Last Modified: Wed, 14 Apr 2021 16:11:00 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ea168f84532f340be87f19704511ee160cbdc5b9c6ad8962fcd80e9fb8efea7`  
		Last Modified: Wed, 14 Apr 2021 16:11:01 GMT  
		Size: 5.7 MB (5651953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2eda2d9556eb5afaf10e6300ac36ddc1383144ae65671ca3a01b24bac150c540`  
		Last Modified: Wed, 14 Apr 2021 16:11:01 GMT  
		Size: 14.4 MB (14401439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a04b0d9d602bb1f9c6fb7925bb92959ebcff2c30e6ca6a658cdd9976d662d70`  
		Last Modified: Wed, 14 Apr 2021 16:10:57 GMT  
		Size: 2.0 KB (1984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e5e865356a464c9006414a165a6d0ffb8f062fa737be2ad42e1aa58fcfca23c`  
		Last Modified: Wed, 14 Apr 2021 16:10:56 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3533148ddde03cc5f28669b26c30dee8685db418d250a4b4829e465c0be8a7e`  
		Last Modified: Wed, 14 Apr 2021 16:10:56 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4573099491ec9887bd66033f55b39f6b897d1f59f21f679fdff4f822ebd7ea15`  
		Last Modified: Wed, 14 Apr 2021 16:10:56 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.2`

```console
$ docker pull nats@sha256:f0c80abcc8d86c26b77b4cfbf150821d7e71ace88e2ea39d8a5bfa33caf0317a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.1879; amd64

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

### `nats:2.2` - windows version 10.0.17763.1879; amd64

```console
$ docker pull nats@sha256:545e15088a9a48d35878789abdde98cb7a98627e5a7c3be56f42abb2e13632e8
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.6 MB (105608630 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19ac61d30cc1900a1011f83ffa5dbcfd15a0a1754f790b94bdded5ed0cd4b673`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 08 Apr 2021 16:02:06 GMT
RUN Apply image 1809-amd64
# Wed, 14 Apr 2021 16:05:18 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 14 Apr 2021 16:05:20 GMT
RUN cmd /S /C #(nop) COPY file:428a7e80db4313301a46326a9a79832e9cbe7d78c94e749b5c295e813e484f21 in C:\nats-server.exe 
# Wed, 14 Apr 2021 16:05:21 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 14 Apr 2021 16:05:22 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 14 Apr 2021 16:05:22 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 14 Apr 2021 16:05:23 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:ea84579f6cd5b58fe78732be37450bd188c8923de3a2062664f3992861449b5c`  
		Size: 101.3 MB (101340157 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f8d27bfefcaaa84a89f93945c61ccf0af9ad50b1405d9acfa30e9da5ba1fb2db`  
		Last Modified: Wed, 14 Apr 2021 16:10:39 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6f599ec3e67dbcacd5ebae06ae984f5a688eba397e2280187ee399da88dc6ad`  
		Last Modified: Wed, 14 Apr 2021 16:10:38 GMT  
		Size: 4.3 MB (4262107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:780b42108cdc95774ec8d8239a9027e7382a875cf25306df1b01363dd2dc7aa4`  
		Last Modified: Wed, 14 Apr 2021 16:10:37 GMT  
		Size: 1.8 KB (1758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b002edb80987b79bb224f75e7c65e924d45dc54e548ce835539ca82dcdcc08e6`  
		Last Modified: Wed, 14 Apr 2021 16:10:37 GMT  
		Size: 1.2 KB (1176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c148b88ce7ff0e645ebee08b98beb32730028b41f85296f22b03154fa54614ac`  
		Last Modified: Wed, 14 Apr 2021 16:10:37 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43dc978ed7937ca238d82c78779b6e3a605e64ba31e2a5adac73bc7da1f63ede`  
		Last Modified: Wed, 14 Apr 2021 16:10:37 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.2-alpine`

```console
$ docker pull nats@sha256:cb99fd7d7cb5b5ed625ef86f9e847c26cb6e7c13f970765e77da331d0a13959d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.2-alpine` - linux; amd64

```console
$ docker pull nats@sha256:7b78ce1b52f0b0421d7f722c642c9b0feb9d340b9b4896b0c638960863934a0e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7303896 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d14bc60ccc43c89281be8e1cb48cba172a1bc16e08228e9fed919e32c40e64e6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 23:12:59 GMT
ENV NATS_SERVER=2.2.1
# Wed, 14 Apr 2021 23:13:02 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='0123d924907282265190258662edf8ad4351055083b5040e3bdf59117bd1c51c' ;; 		armhf) natsArch='arm6'; sha256='da719b07fd57137f85bfa6cffc7d00841a9c1fb4cdf7ca9a537bfc3f99b71f36' ;; 		armv7) natsArch='arm7'; sha256='cf6e8d9a9cc5d05f7320fb4be8fc9239cb87b91c6600a61ce7a2fb63e2f29f5a' ;; 		x86_64) natsArch='amd64'; sha256='70cb40d78b82ea6c0ca926c31ef98d2e1c885cfe2f73f34883e4ca448366c2dd' ;; 		x86) natsArch='386'; sha256='da54d129f8a52c048ded61e3b62e946037a9464d02cf818e568bbf1e385ce6be' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 14 Apr 2021 23:13:02 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Wed, 14 Apr 2021 23:13:02 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 14 Apr 2021 23:13:03 GMT
EXPOSE 4222 6222 8222
# Wed, 14 Apr 2021 23:13:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 23:13:03 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adf2b83a147ab10f7ee92b0624d9beb0101ff40b27dd92a1e74ec3bc972fa9f8`  
		Last Modified: Wed, 14 Apr 2021 23:13:45 GMT  
		Size: 4.5 MB (4490957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab1824f686e6029870ed0b1328708bbfe11b2c3b1bac6a461604b830ffdc13ce`  
		Last Modified: Wed, 14 Apr 2021 23:13:44 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:357bc9de7de4490d1629a64200e10f44bf96da1168b66f8bb512a3ce9d68bc23`  
		Last Modified: Wed, 14 Apr 2021 23:13:44 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:eb3c514a433f020cd80da54de5a877d42c7f8aef888eef6fcf72b0175626cbd1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6784935 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:abd439f99c0768fd1ea54123118765e2c3a5e6f7e7f44c358794ce23c8590216`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Apr 2021 18:49:39 GMT
ADD file:4479f0a51530e039edf231d87201896dcff908aa542a613cdccb015f93dda8a3 in / 
# Wed, 14 Apr 2021 18:49:40 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 21:48:34 GMT
ENV NATS_SERVER=2.2.1
# Wed, 14 Apr 2021 21:49:16 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='0123d924907282265190258662edf8ad4351055083b5040e3bdf59117bd1c51c' ;; 		armhf) natsArch='arm6'; sha256='da719b07fd57137f85bfa6cffc7d00841a9c1fb4cdf7ca9a537bfc3f99b71f36' ;; 		armv7) natsArch='arm7'; sha256='cf6e8d9a9cc5d05f7320fb4be8fc9239cb87b91c6600a61ce7a2fb63e2f29f5a' ;; 		x86_64) natsArch='amd64'; sha256='70cb40d78b82ea6c0ca926c31ef98d2e1c885cfe2f73f34883e4ca448366c2dd' ;; 		x86) natsArch='386'; sha256='da54d129f8a52c048ded61e3b62e946037a9464d02cf818e568bbf1e385ce6be' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 14 Apr 2021 21:49:31 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Wed, 14 Apr 2021 21:49:41 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 14 Apr 2021 21:49:50 GMT
EXPOSE 4222 6222 8222
# Wed, 14 Apr 2021 21:49:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 21:50:03 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:740c950346cf39c85b52576998695c9b909c24a58a8bb1b64cce91fda3ef1d3a`  
		Last Modified: Wed, 14 Apr 2021 18:50:30 GMT  
		Size: 2.6 MB (2622131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22164d2f45f59e8f1d873e8a0c4769559100e469dc09c3bcbb61163732b2f453`  
		Last Modified: Wed, 14 Apr 2021 21:52:09 GMT  
		Size: 4.2 MB (4161829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79de2833ed16322bc62170a748bd3d746b8b152ec85cffa0cd11a3c25d822b35`  
		Last Modified: Wed, 14 Apr 2021 21:52:06 GMT  
		Size: 561.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f686c25c87f7ee66f2990e18510448fe0a0063432d6f894bd1a1b0917eaf37a`  
		Last Modified: Wed, 14 Apr 2021 21:52:09 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:65016cde6a860e4e53a844e66d8944c0b72583aff8b0f17940f5883ce2025337
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6583191 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd85ddd622c92403cb491019f78c2760f9a3938378dadba44b3d1e382b1dd1db`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Apr 2021 18:57:39 GMT
ADD file:028c5b473d862250586e174c5dd19b37f8fc3bffbc02d888e72df30f32fd6129 in / 
# Wed, 14 Apr 2021 18:57:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 23:17:51 GMT
ENV NATS_SERVER=2.2.1
# Wed, 14 Apr 2021 23:17:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='0123d924907282265190258662edf8ad4351055083b5040e3bdf59117bd1c51c' ;; 		armhf) natsArch='arm6'; sha256='da719b07fd57137f85bfa6cffc7d00841a9c1fb4cdf7ca9a537bfc3f99b71f36' ;; 		armv7) natsArch='arm7'; sha256='cf6e8d9a9cc5d05f7320fb4be8fc9239cb87b91c6600a61ce7a2fb63e2f29f5a' ;; 		x86_64) natsArch='amd64'; sha256='70cb40d78b82ea6c0ca926c31ef98d2e1c885cfe2f73f34883e4ca448366c2dd' ;; 		x86) natsArch='386'; sha256='da54d129f8a52c048ded61e3b62e946037a9464d02cf818e568bbf1e385ce6be' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 14 Apr 2021 23:18:00 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Wed, 14 Apr 2021 23:18:02 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 14 Apr 2021 23:18:04 GMT
EXPOSE 4222 6222 8222
# Wed, 14 Apr 2021 23:18:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 23:18:09 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:e160e00eb35d5bc2373770873fbc9c8f5706045b0b06bfd1c364fcf69f02e9fe`  
		Last Modified: Wed, 14 Apr 2021 18:58:36 GMT  
		Size: 2.4 MB (2424145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3691a766339eab5091760e8ff801b39c69452b17fdd4fbd0e0cd710d241b5c5`  
		Last Modified: Wed, 14 Apr 2021 23:19:04 GMT  
		Size: 4.2 MB (4158072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a272e5ab96f7d43eb8e116aedf9e11bc1280f7ce6fbc83d2cbd82506c9ad760`  
		Last Modified: Wed, 14 Apr 2021 23:19:02 GMT  
		Size: 562.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e5adcdbbba76bad23d4bf8413449ce3ae2e70365468c47978d2c4ba7b937a67`  
		Last Modified: Wed, 14 Apr 2021 23:19:02 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2-alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:643201294279426bb51217496fc5e4053f55c0b29010efea1f201918efa1544a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6844402 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fd51943be05be331bd2fbd7b2494b10525553a8590e7041cda0723402b5d281a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Apr 2021 18:42:37 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Wed, 14 Apr 2021 18:42:38 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 23:37:11 GMT
ENV NATS_SERVER=2.2.1
# Wed, 14 Apr 2021 23:37:17 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='0123d924907282265190258662edf8ad4351055083b5040e3bdf59117bd1c51c' ;; 		armhf) natsArch='arm6'; sha256='da719b07fd57137f85bfa6cffc7d00841a9c1fb4cdf7ca9a537bfc3f99b71f36' ;; 		armv7) natsArch='arm7'; sha256='cf6e8d9a9cc5d05f7320fb4be8fc9239cb87b91c6600a61ce7a2fb63e2f29f5a' ;; 		x86_64) natsArch='amd64'; sha256='70cb40d78b82ea6c0ca926c31ef98d2e1c885cfe2f73f34883e4ca448366c2dd' ;; 		x86) natsArch='386'; sha256='da54d129f8a52c048ded61e3b62e946037a9464d02cf818e568bbf1e385ce6be' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 14 Apr 2021 23:37:18 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Wed, 14 Apr 2021 23:37:20 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 14 Apr 2021 23:37:25 GMT
EXPOSE 4222 6222 8222
# Wed, 14 Apr 2021 23:37:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 23:37:27 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:305503c7404cab7cb3fe558afe5d1b142f71b61815abb7d5b545be5d6fd274da`  
		Last Modified: Wed, 14 Apr 2021 23:41:37 GMT  
		Size: 4.1 MB (4131404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9504bc3187f368a20d4fe0020479a23dd57f07ea67deeb351297f4a8f1252dd7`  
		Last Modified: Wed, 14 Apr 2021 23:41:35 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0889a2e36f7ca1635400c49238cbb554ad2519b4a2c2cbfacff8cf2a1e21acd1`  
		Last Modified: Wed, 14 Apr 2021 23:41:35 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.2-alpine3.13`

```console
$ docker pull nats@sha256:cb99fd7d7cb5b5ed625ef86f9e847c26cb6e7c13f970765e77da331d0a13959d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.2-alpine3.13` - linux; amd64

```console
$ docker pull nats@sha256:7b78ce1b52f0b0421d7f722c642c9b0feb9d340b9b4896b0c638960863934a0e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7303896 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d14bc60ccc43c89281be8e1cb48cba172a1bc16e08228e9fed919e32c40e64e6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 23:12:59 GMT
ENV NATS_SERVER=2.2.1
# Wed, 14 Apr 2021 23:13:02 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='0123d924907282265190258662edf8ad4351055083b5040e3bdf59117bd1c51c' ;; 		armhf) natsArch='arm6'; sha256='da719b07fd57137f85bfa6cffc7d00841a9c1fb4cdf7ca9a537bfc3f99b71f36' ;; 		armv7) natsArch='arm7'; sha256='cf6e8d9a9cc5d05f7320fb4be8fc9239cb87b91c6600a61ce7a2fb63e2f29f5a' ;; 		x86_64) natsArch='amd64'; sha256='70cb40d78b82ea6c0ca926c31ef98d2e1c885cfe2f73f34883e4ca448366c2dd' ;; 		x86) natsArch='386'; sha256='da54d129f8a52c048ded61e3b62e946037a9464d02cf818e568bbf1e385ce6be' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 14 Apr 2021 23:13:02 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Wed, 14 Apr 2021 23:13:02 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 14 Apr 2021 23:13:03 GMT
EXPOSE 4222 6222 8222
# Wed, 14 Apr 2021 23:13:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 23:13:03 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adf2b83a147ab10f7ee92b0624d9beb0101ff40b27dd92a1e74ec3bc972fa9f8`  
		Last Modified: Wed, 14 Apr 2021 23:13:45 GMT  
		Size: 4.5 MB (4490957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab1824f686e6029870ed0b1328708bbfe11b2c3b1bac6a461604b830ffdc13ce`  
		Last Modified: Wed, 14 Apr 2021 23:13:44 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:357bc9de7de4490d1629a64200e10f44bf96da1168b66f8bb512a3ce9d68bc23`  
		Last Modified: Wed, 14 Apr 2021 23:13:44 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2-alpine3.13` - linux; arm variant v6

```console
$ docker pull nats@sha256:eb3c514a433f020cd80da54de5a877d42c7f8aef888eef6fcf72b0175626cbd1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6784935 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:abd439f99c0768fd1ea54123118765e2c3a5e6f7e7f44c358794ce23c8590216`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Apr 2021 18:49:39 GMT
ADD file:4479f0a51530e039edf231d87201896dcff908aa542a613cdccb015f93dda8a3 in / 
# Wed, 14 Apr 2021 18:49:40 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 21:48:34 GMT
ENV NATS_SERVER=2.2.1
# Wed, 14 Apr 2021 21:49:16 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='0123d924907282265190258662edf8ad4351055083b5040e3bdf59117bd1c51c' ;; 		armhf) natsArch='arm6'; sha256='da719b07fd57137f85bfa6cffc7d00841a9c1fb4cdf7ca9a537bfc3f99b71f36' ;; 		armv7) natsArch='arm7'; sha256='cf6e8d9a9cc5d05f7320fb4be8fc9239cb87b91c6600a61ce7a2fb63e2f29f5a' ;; 		x86_64) natsArch='amd64'; sha256='70cb40d78b82ea6c0ca926c31ef98d2e1c885cfe2f73f34883e4ca448366c2dd' ;; 		x86) natsArch='386'; sha256='da54d129f8a52c048ded61e3b62e946037a9464d02cf818e568bbf1e385ce6be' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 14 Apr 2021 21:49:31 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Wed, 14 Apr 2021 21:49:41 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 14 Apr 2021 21:49:50 GMT
EXPOSE 4222 6222 8222
# Wed, 14 Apr 2021 21:49:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 21:50:03 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:740c950346cf39c85b52576998695c9b909c24a58a8bb1b64cce91fda3ef1d3a`  
		Last Modified: Wed, 14 Apr 2021 18:50:30 GMT  
		Size: 2.6 MB (2622131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22164d2f45f59e8f1d873e8a0c4769559100e469dc09c3bcbb61163732b2f453`  
		Last Modified: Wed, 14 Apr 2021 21:52:09 GMT  
		Size: 4.2 MB (4161829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79de2833ed16322bc62170a748bd3d746b8b152ec85cffa0cd11a3c25d822b35`  
		Last Modified: Wed, 14 Apr 2021 21:52:06 GMT  
		Size: 561.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f686c25c87f7ee66f2990e18510448fe0a0063432d6f894bd1a1b0917eaf37a`  
		Last Modified: Wed, 14 Apr 2021 21:52:09 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2-alpine3.13` - linux; arm variant v7

```console
$ docker pull nats@sha256:65016cde6a860e4e53a844e66d8944c0b72583aff8b0f17940f5883ce2025337
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6583191 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd85ddd622c92403cb491019f78c2760f9a3938378dadba44b3d1e382b1dd1db`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Apr 2021 18:57:39 GMT
ADD file:028c5b473d862250586e174c5dd19b37f8fc3bffbc02d888e72df30f32fd6129 in / 
# Wed, 14 Apr 2021 18:57:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 23:17:51 GMT
ENV NATS_SERVER=2.2.1
# Wed, 14 Apr 2021 23:17:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='0123d924907282265190258662edf8ad4351055083b5040e3bdf59117bd1c51c' ;; 		armhf) natsArch='arm6'; sha256='da719b07fd57137f85bfa6cffc7d00841a9c1fb4cdf7ca9a537bfc3f99b71f36' ;; 		armv7) natsArch='arm7'; sha256='cf6e8d9a9cc5d05f7320fb4be8fc9239cb87b91c6600a61ce7a2fb63e2f29f5a' ;; 		x86_64) natsArch='amd64'; sha256='70cb40d78b82ea6c0ca926c31ef98d2e1c885cfe2f73f34883e4ca448366c2dd' ;; 		x86) natsArch='386'; sha256='da54d129f8a52c048ded61e3b62e946037a9464d02cf818e568bbf1e385ce6be' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 14 Apr 2021 23:18:00 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Wed, 14 Apr 2021 23:18:02 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 14 Apr 2021 23:18:04 GMT
EXPOSE 4222 6222 8222
# Wed, 14 Apr 2021 23:18:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 23:18:09 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:e160e00eb35d5bc2373770873fbc9c8f5706045b0b06bfd1c364fcf69f02e9fe`  
		Last Modified: Wed, 14 Apr 2021 18:58:36 GMT  
		Size: 2.4 MB (2424145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3691a766339eab5091760e8ff801b39c69452b17fdd4fbd0e0cd710d241b5c5`  
		Last Modified: Wed, 14 Apr 2021 23:19:04 GMT  
		Size: 4.2 MB (4158072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a272e5ab96f7d43eb8e116aedf9e11bc1280f7ce6fbc83d2cbd82506c9ad760`  
		Last Modified: Wed, 14 Apr 2021 23:19:02 GMT  
		Size: 562.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e5adcdbbba76bad23d4bf8413449ce3ae2e70365468c47978d2c4ba7b937a67`  
		Last Modified: Wed, 14 Apr 2021 23:19:02 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2-alpine3.13` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:643201294279426bb51217496fc5e4053f55c0b29010efea1f201918efa1544a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6844402 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fd51943be05be331bd2fbd7b2494b10525553a8590e7041cda0723402b5d281a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Apr 2021 18:42:37 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Wed, 14 Apr 2021 18:42:38 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 23:37:11 GMT
ENV NATS_SERVER=2.2.1
# Wed, 14 Apr 2021 23:37:17 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='0123d924907282265190258662edf8ad4351055083b5040e3bdf59117bd1c51c' ;; 		armhf) natsArch='arm6'; sha256='da719b07fd57137f85bfa6cffc7d00841a9c1fb4cdf7ca9a537bfc3f99b71f36' ;; 		armv7) natsArch='arm7'; sha256='cf6e8d9a9cc5d05f7320fb4be8fc9239cb87b91c6600a61ce7a2fb63e2f29f5a' ;; 		x86_64) natsArch='amd64'; sha256='70cb40d78b82ea6c0ca926c31ef98d2e1c885cfe2f73f34883e4ca448366c2dd' ;; 		x86) natsArch='386'; sha256='da54d129f8a52c048ded61e3b62e946037a9464d02cf818e568bbf1e385ce6be' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 14 Apr 2021 23:37:18 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Wed, 14 Apr 2021 23:37:20 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 14 Apr 2021 23:37:25 GMT
EXPOSE 4222 6222 8222
# Wed, 14 Apr 2021 23:37:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 23:37:27 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:305503c7404cab7cb3fe558afe5d1b142f71b61815abb7d5b545be5d6fd274da`  
		Last Modified: Wed, 14 Apr 2021 23:41:37 GMT  
		Size: 4.1 MB (4131404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9504bc3187f368a20d4fe0020479a23dd57f07ea67deeb351297f4a8f1252dd7`  
		Last Modified: Wed, 14 Apr 2021 23:41:35 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0889a2e36f7ca1635400c49238cbb554ad2519b4a2c2cbfacff8cf2a1e21acd1`  
		Last Modified: Wed, 14 Apr 2021 23:41:35 GMT  
		Size: 414.0 B  
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
$ docker pull nats@sha256:236c67f0c205b9cfab2809ce1dea44a20258d371c82264afd3172f29c8c70fb1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1879; amd64

### `nats:2.2-nanoserver` - windows version 10.0.17763.1879; amd64

```console
$ docker pull nats@sha256:545e15088a9a48d35878789abdde98cb7a98627e5a7c3be56f42abb2e13632e8
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.6 MB (105608630 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19ac61d30cc1900a1011f83ffa5dbcfd15a0a1754f790b94bdded5ed0cd4b673`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 08 Apr 2021 16:02:06 GMT
RUN Apply image 1809-amd64
# Wed, 14 Apr 2021 16:05:18 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 14 Apr 2021 16:05:20 GMT
RUN cmd /S /C #(nop) COPY file:428a7e80db4313301a46326a9a79832e9cbe7d78c94e749b5c295e813e484f21 in C:\nats-server.exe 
# Wed, 14 Apr 2021 16:05:21 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 14 Apr 2021 16:05:22 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 14 Apr 2021 16:05:22 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 14 Apr 2021 16:05:23 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:ea84579f6cd5b58fe78732be37450bd188c8923de3a2062664f3992861449b5c`  
		Size: 101.3 MB (101340157 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f8d27bfefcaaa84a89f93945c61ccf0af9ad50b1405d9acfa30e9da5ba1fb2db`  
		Last Modified: Wed, 14 Apr 2021 16:10:39 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6f599ec3e67dbcacd5ebae06ae984f5a688eba397e2280187ee399da88dc6ad`  
		Last Modified: Wed, 14 Apr 2021 16:10:38 GMT  
		Size: 4.3 MB (4262107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:780b42108cdc95774ec8d8239a9027e7382a875cf25306df1b01363dd2dc7aa4`  
		Last Modified: Wed, 14 Apr 2021 16:10:37 GMT  
		Size: 1.8 KB (1758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b002edb80987b79bb224f75e7c65e924d45dc54e548ce835539ca82dcdcc08e6`  
		Last Modified: Wed, 14 Apr 2021 16:10:37 GMT  
		Size: 1.2 KB (1176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c148b88ce7ff0e645ebee08b98beb32730028b41f85296f22b03154fa54614ac`  
		Last Modified: Wed, 14 Apr 2021 16:10:37 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43dc978ed7937ca238d82c78779b6e3a605e64ba31e2a5adac73bc7da1f63ede`  
		Last Modified: Wed, 14 Apr 2021 16:10:37 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.2-nanoserver-1809`

```console
$ docker pull nats@sha256:236c67f0c205b9cfab2809ce1dea44a20258d371c82264afd3172f29c8c70fb1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1879; amd64

### `nats:2.2-nanoserver-1809` - windows version 10.0.17763.1879; amd64

```console
$ docker pull nats@sha256:545e15088a9a48d35878789abdde98cb7a98627e5a7c3be56f42abb2e13632e8
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.6 MB (105608630 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19ac61d30cc1900a1011f83ffa5dbcfd15a0a1754f790b94bdded5ed0cd4b673`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 08 Apr 2021 16:02:06 GMT
RUN Apply image 1809-amd64
# Wed, 14 Apr 2021 16:05:18 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 14 Apr 2021 16:05:20 GMT
RUN cmd /S /C #(nop) COPY file:428a7e80db4313301a46326a9a79832e9cbe7d78c94e749b5c295e813e484f21 in C:\nats-server.exe 
# Wed, 14 Apr 2021 16:05:21 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 14 Apr 2021 16:05:22 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 14 Apr 2021 16:05:22 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 14 Apr 2021 16:05:23 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:ea84579f6cd5b58fe78732be37450bd188c8923de3a2062664f3992861449b5c`  
		Size: 101.3 MB (101340157 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f8d27bfefcaaa84a89f93945c61ccf0af9ad50b1405d9acfa30e9da5ba1fb2db`  
		Last Modified: Wed, 14 Apr 2021 16:10:39 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6f599ec3e67dbcacd5ebae06ae984f5a688eba397e2280187ee399da88dc6ad`  
		Last Modified: Wed, 14 Apr 2021 16:10:38 GMT  
		Size: 4.3 MB (4262107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:780b42108cdc95774ec8d8239a9027e7382a875cf25306df1b01363dd2dc7aa4`  
		Last Modified: Wed, 14 Apr 2021 16:10:37 GMT  
		Size: 1.8 KB (1758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b002edb80987b79bb224f75e7c65e924d45dc54e548ce835539ca82dcdcc08e6`  
		Last Modified: Wed, 14 Apr 2021 16:10:37 GMT  
		Size: 1.2 KB (1176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c148b88ce7ff0e645ebee08b98beb32730028b41f85296f22b03154fa54614ac`  
		Last Modified: Wed, 14 Apr 2021 16:10:37 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43dc978ed7937ca238d82c78779b6e3a605e64ba31e2a5adac73bc7da1f63ede`  
		Last Modified: Wed, 14 Apr 2021 16:10:37 GMT  
		Size: 1.1 KB (1149 bytes)  
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
$ docker pull nats@sha256:a6c1153fd919a539581471edd798478057cef10a6347e770d03336a20d5e472b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1879; amd64
	-	windows version 10.0.14393.4350; amd64

### `nats:2.2-windowsservercore` - windows version 10.0.17763.1879; amd64

```console
$ docker pull nats@sha256:9f3868f133ddd1a10ac71bbe835764e9d60e9b00081851a00ca05cd3362ea5d1
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2484142070 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2be425426bfa101eb4fdc6741eccbeaddde31c6c0761a665b4654dea39a17279`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 09 Apr 2021 20:34:41 GMT
RUN Install update 1809-amd64
# Wed, 14 Apr 2021 13:10:28 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 14 Apr 2021 16:02:50 GMT
ENV NATS_DOCKERIZED=1
# Wed, 14 Apr 2021 16:02:51 GMT
ENV NATS_SERVER=2.2.1
# Wed, 14 Apr 2021 16:02:52 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.2.1/nats-server-v2.2.1-windows-amd64.zip
# Wed, 14 Apr 2021 16:02:53 GMT
ENV GIT_DOWNLOAD_SHA256=1f0d48a7ba9200e2572016a9f3e1ec7e630f0518cc0b40950c14ff3a5d900924
# Wed, 14 Apr 2021 16:03:32 GMT
RUN Set-PSDebug -Trace 2
# Wed, 14 Apr 2021 16:04:53 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 14 Apr 2021 16:04:55 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 14 Apr 2021 16:04:56 GMT
EXPOSE 4222 6222 8222
# Wed, 14 Apr 2021 16:04:57 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 14 Apr 2021 16:04:58 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:399f118dfaa9a753e98d128238b944432c7bcabea88a2998a6efbbece28ed303`  
		Size: 751.4 MB (751421005 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b2159a5d0f75ce11e6fe71e4260ede5c3c88a9eb76a0ff43ac6746b2b9b96775`  
		Last Modified: Wed, 14 Apr 2021 15:37:10 GMT  
		Size: 1.4 KB (1446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e849354f21f856ec720d6daecc37978fd7246f376ba3c32fd63d4400cce357bc`  
		Last Modified: Wed, 14 Apr 2021 16:10:16 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daae5ee02f484d7c054ad550cbee6900a35477f4e23e322cc3af6eb7c4690416`  
		Last Modified: Wed, 14 Apr 2021 16:10:14 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d4df8575d5fc511a7ac278cfc55a4053b36afce4c0bcae2af0af7907c7f91e6`  
		Last Modified: Wed, 14 Apr 2021 16:10:14 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:570a7e5edba00d92281a4a147639b5fc0b6724693cbfed80007b5b5db612a3e8`  
		Last Modified: Wed, 14 Apr 2021 16:10:13 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60092b7b0679ad17236eb09b832adcc7bb67a5fd8c2d9a69ffbfc863716274c2`  
		Last Modified: Wed, 14 Apr 2021 16:10:15 GMT  
		Size: 5.1 MB (5072726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d5d3b99689d155ccd6cdf6acbc7ef61472c65ce2cee49f441c4c3b844242410`  
		Last Modified: Wed, 14 Apr 2021 16:10:13 GMT  
		Size: 9.3 MB (9302175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23dae780c7132cf39c97d1602e11b6a58481594df6d896054f3a9e6e9f54e63a`  
		Last Modified: Wed, 14 Apr 2021 16:10:10 GMT  
		Size: 2.0 KB (1957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95f2291e14ae4d6e97942f3284122a80c7c969cb9bcfc9a417a833439505f85d`  
		Last Modified: Wed, 14 Apr 2021 16:10:11 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69b07be56d63a82b0606023df13bf32a522a13a12a44c53116ec24d0c1bd2ca1`  
		Last Modified: Wed, 14 Apr 2021 16:10:11 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb6cc0327d5edba60d3e99a97fa6c015e1953c9451bc816f20d6d73a67b9e426`  
		Last Modified: Wed, 14 Apr 2021 16:10:11 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2-windowsservercore` - windows version 10.0.14393.4350; amd64

```console
$ docker pull nats@sha256:ad5ac25aa423d2df82324037dd73fec641098cd5f198cf98ccf19f4ae640d1f5
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5814950471 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0fc9b58b0a6e7d867ee74a6023bf1768d2dad684760ace428c0bf425357fcc5c`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 07 Apr 2021 21:54:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 14 Apr 2021 13:22:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 14 Apr 2021 16:05:33 GMT
ENV NATS_DOCKERIZED=1
# Wed, 14 Apr 2021 16:05:33 GMT
ENV NATS_SERVER=2.2.1
# Wed, 14 Apr 2021 16:05:35 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.2.1/nats-server-v2.2.1-windows-amd64.zip
# Wed, 14 Apr 2021 16:05:35 GMT
ENV GIT_DOWNLOAD_SHA256=1f0d48a7ba9200e2572016a9f3e1ec7e630f0518cc0b40950c14ff3a5d900924
# Wed, 14 Apr 2021 16:06:59 GMT
RUN Set-PSDebug -Trace 2
# Wed, 14 Apr 2021 16:09:18 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 14 Apr 2021 16:09:19 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 14 Apr 2021 16:09:20 GMT
EXPOSE 4222 6222 8222
# Wed, 14 Apr 2021 16:09:21 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 14 Apr 2021 16:09:23 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:00b4edb823e6a375d179a28cbfa682c2379d62179e1518485902d6e68b9a9d1e`  
		Size: 1.7 GB (1724897968 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f616bb7876e6f944d82fa1802ffab5ca4931a63e1b999f0851b52120cda83539`  
		Last Modified: Wed, 14 Apr 2021 15:37:43 GMT  
		Size: 1.3 KB (1307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcfa54f43457753c391f21da5e9a5bf47c61c574c0da04b8614d0e84bf823f54`  
		Last Modified: Wed, 14 Apr 2021 16:11:03 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04d71ba1c574073f9d5dd016585c2fe26ac560c192f7aa36ce54d4c12832997f`  
		Last Modified: Wed, 14 Apr 2021 16:11:01 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e9f66539738348100cf9f1e6a5bc40e8c2123bafb9329f5df3cf20a2015db33`  
		Last Modified: Wed, 14 Apr 2021 16:11:00 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20f2eae922462b2537c1d0d32d548cb10190f6bda0d02da57440cc229da692b3`  
		Last Modified: Wed, 14 Apr 2021 16:11:00 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ea168f84532f340be87f19704511ee160cbdc5b9c6ad8962fcd80e9fb8efea7`  
		Last Modified: Wed, 14 Apr 2021 16:11:01 GMT  
		Size: 5.7 MB (5651953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2eda2d9556eb5afaf10e6300ac36ddc1383144ae65671ca3a01b24bac150c540`  
		Last Modified: Wed, 14 Apr 2021 16:11:01 GMT  
		Size: 14.4 MB (14401439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a04b0d9d602bb1f9c6fb7925bb92959ebcff2c30e6ca6a658cdd9976d662d70`  
		Last Modified: Wed, 14 Apr 2021 16:10:57 GMT  
		Size: 2.0 KB (1984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e5e865356a464c9006414a165a6d0ffb8f062fa737be2ad42e1aa58fcfca23c`  
		Last Modified: Wed, 14 Apr 2021 16:10:56 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3533148ddde03cc5f28669b26c30dee8685db418d250a4b4829e465c0be8a7e`  
		Last Modified: Wed, 14 Apr 2021 16:10:56 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4573099491ec9887bd66033f55b39f6b897d1f59f21f679fdff4f822ebd7ea15`  
		Last Modified: Wed, 14 Apr 2021 16:10:56 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.2-windowsservercore-1809`

```console
$ docker pull nats@sha256:3002e35b4bb91080eac08408891e6bb9155d38086cbb6fcfb654b61e0d2383e0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1879; amd64

### `nats:2.2-windowsservercore-1809` - windows version 10.0.17763.1879; amd64

```console
$ docker pull nats@sha256:9f3868f133ddd1a10ac71bbe835764e9d60e9b00081851a00ca05cd3362ea5d1
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2484142070 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2be425426bfa101eb4fdc6741eccbeaddde31c6c0761a665b4654dea39a17279`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 09 Apr 2021 20:34:41 GMT
RUN Install update 1809-amd64
# Wed, 14 Apr 2021 13:10:28 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 14 Apr 2021 16:02:50 GMT
ENV NATS_DOCKERIZED=1
# Wed, 14 Apr 2021 16:02:51 GMT
ENV NATS_SERVER=2.2.1
# Wed, 14 Apr 2021 16:02:52 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.2.1/nats-server-v2.2.1-windows-amd64.zip
# Wed, 14 Apr 2021 16:02:53 GMT
ENV GIT_DOWNLOAD_SHA256=1f0d48a7ba9200e2572016a9f3e1ec7e630f0518cc0b40950c14ff3a5d900924
# Wed, 14 Apr 2021 16:03:32 GMT
RUN Set-PSDebug -Trace 2
# Wed, 14 Apr 2021 16:04:53 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 14 Apr 2021 16:04:55 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 14 Apr 2021 16:04:56 GMT
EXPOSE 4222 6222 8222
# Wed, 14 Apr 2021 16:04:57 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 14 Apr 2021 16:04:58 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:399f118dfaa9a753e98d128238b944432c7bcabea88a2998a6efbbece28ed303`  
		Size: 751.4 MB (751421005 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b2159a5d0f75ce11e6fe71e4260ede5c3c88a9eb76a0ff43ac6746b2b9b96775`  
		Last Modified: Wed, 14 Apr 2021 15:37:10 GMT  
		Size: 1.4 KB (1446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e849354f21f856ec720d6daecc37978fd7246f376ba3c32fd63d4400cce357bc`  
		Last Modified: Wed, 14 Apr 2021 16:10:16 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daae5ee02f484d7c054ad550cbee6900a35477f4e23e322cc3af6eb7c4690416`  
		Last Modified: Wed, 14 Apr 2021 16:10:14 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d4df8575d5fc511a7ac278cfc55a4053b36afce4c0bcae2af0af7907c7f91e6`  
		Last Modified: Wed, 14 Apr 2021 16:10:14 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:570a7e5edba00d92281a4a147639b5fc0b6724693cbfed80007b5b5db612a3e8`  
		Last Modified: Wed, 14 Apr 2021 16:10:13 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60092b7b0679ad17236eb09b832adcc7bb67a5fd8c2d9a69ffbfc863716274c2`  
		Last Modified: Wed, 14 Apr 2021 16:10:15 GMT  
		Size: 5.1 MB (5072726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d5d3b99689d155ccd6cdf6acbc7ef61472c65ce2cee49f441c4c3b844242410`  
		Last Modified: Wed, 14 Apr 2021 16:10:13 GMT  
		Size: 9.3 MB (9302175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23dae780c7132cf39c97d1602e11b6a58481594df6d896054f3a9e6e9f54e63a`  
		Last Modified: Wed, 14 Apr 2021 16:10:10 GMT  
		Size: 2.0 KB (1957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95f2291e14ae4d6e97942f3284122a80c7c969cb9bcfc9a417a833439505f85d`  
		Last Modified: Wed, 14 Apr 2021 16:10:11 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69b07be56d63a82b0606023df13bf32a522a13a12a44c53116ec24d0c1bd2ca1`  
		Last Modified: Wed, 14 Apr 2021 16:10:11 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb6cc0327d5edba60d3e99a97fa6c015e1953c9451bc816f20d6d73a67b9e426`  
		Last Modified: Wed, 14 Apr 2021 16:10:11 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.2-windowsservercore-ltsc2016`

```console
$ docker pull nats@sha256:486439b61d7c8307b15b01bae5f574784e333ee642d1d3285e3bf61785ea00cd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4350; amd64

### `nats:2.2-windowsservercore-ltsc2016` - windows version 10.0.14393.4350; amd64

```console
$ docker pull nats@sha256:ad5ac25aa423d2df82324037dd73fec641098cd5f198cf98ccf19f4ae640d1f5
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5814950471 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0fc9b58b0a6e7d867ee74a6023bf1768d2dad684760ace428c0bf425357fcc5c`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 07 Apr 2021 21:54:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 14 Apr 2021 13:22:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 14 Apr 2021 16:05:33 GMT
ENV NATS_DOCKERIZED=1
# Wed, 14 Apr 2021 16:05:33 GMT
ENV NATS_SERVER=2.2.1
# Wed, 14 Apr 2021 16:05:35 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.2.1/nats-server-v2.2.1-windows-amd64.zip
# Wed, 14 Apr 2021 16:05:35 GMT
ENV GIT_DOWNLOAD_SHA256=1f0d48a7ba9200e2572016a9f3e1ec7e630f0518cc0b40950c14ff3a5d900924
# Wed, 14 Apr 2021 16:06:59 GMT
RUN Set-PSDebug -Trace 2
# Wed, 14 Apr 2021 16:09:18 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 14 Apr 2021 16:09:19 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 14 Apr 2021 16:09:20 GMT
EXPOSE 4222 6222 8222
# Wed, 14 Apr 2021 16:09:21 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 14 Apr 2021 16:09:23 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:00b4edb823e6a375d179a28cbfa682c2379d62179e1518485902d6e68b9a9d1e`  
		Size: 1.7 GB (1724897968 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f616bb7876e6f944d82fa1802ffab5ca4931a63e1b999f0851b52120cda83539`  
		Last Modified: Wed, 14 Apr 2021 15:37:43 GMT  
		Size: 1.3 KB (1307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcfa54f43457753c391f21da5e9a5bf47c61c574c0da04b8614d0e84bf823f54`  
		Last Modified: Wed, 14 Apr 2021 16:11:03 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04d71ba1c574073f9d5dd016585c2fe26ac560c192f7aa36ce54d4c12832997f`  
		Last Modified: Wed, 14 Apr 2021 16:11:01 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e9f66539738348100cf9f1e6a5bc40e8c2123bafb9329f5df3cf20a2015db33`  
		Last Modified: Wed, 14 Apr 2021 16:11:00 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20f2eae922462b2537c1d0d32d548cb10190f6bda0d02da57440cc229da692b3`  
		Last Modified: Wed, 14 Apr 2021 16:11:00 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ea168f84532f340be87f19704511ee160cbdc5b9c6ad8962fcd80e9fb8efea7`  
		Last Modified: Wed, 14 Apr 2021 16:11:01 GMT  
		Size: 5.7 MB (5651953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2eda2d9556eb5afaf10e6300ac36ddc1383144ae65671ca3a01b24bac150c540`  
		Last Modified: Wed, 14 Apr 2021 16:11:01 GMT  
		Size: 14.4 MB (14401439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a04b0d9d602bb1f9c6fb7925bb92959ebcff2c30e6ca6a658cdd9976d662d70`  
		Last Modified: Wed, 14 Apr 2021 16:10:57 GMT  
		Size: 2.0 KB (1984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e5e865356a464c9006414a165a6d0ffb8f062fa737be2ad42e1aa58fcfca23c`  
		Last Modified: Wed, 14 Apr 2021 16:10:56 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3533148ddde03cc5f28669b26c30dee8685db418d250a4b4829e465c0be8a7e`  
		Last Modified: Wed, 14 Apr 2021 16:10:56 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4573099491ec9887bd66033f55b39f6b897d1f59f21f679fdff4f822ebd7ea15`  
		Last Modified: Wed, 14 Apr 2021 16:10:56 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.2.1`

```console
$ docker pull nats@sha256:f0c80abcc8d86c26b77b4cfbf150821d7e71ace88e2ea39d8a5bfa33caf0317a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.1879; amd64

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

### `nats:2.2.1` - windows version 10.0.17763.1879; amd64

```console
$ docker pull nats@sha256:545e15088a9a48d35878789abdde98cb7a98627e5a7c3be56f42abb2e13632e8
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.6 MB (105608630 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19ac61d30cc1900a1011f83ffa5dbcfd15a0a1754f790b94bdded5ed0cd4b673`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 08 Apr 2021 16:02:06 GMT
RUN Apply image 1809-amd64
# Wed, 14 Apr 2021 16:05:18 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 14 Apr 2021 16:05:20 GMT
RUN cmd /S /C #(nop) COPY file:428a7e80db4313301a46326a9a79832e9cbe7d78c94e749b5c295e813e484f21 in C:\nats-server.exe 
# Wed, 14 Apr 2021 16:05:21 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 14 Apr 2021 16:05:22 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 14 Apr 2021 16:05:22 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 14 Apr 2021 16:05:23 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:ea84579f6cd5b58fe78732be37450bd188c8923de3a2062664f3992861449b5c`  
		Size: 101.3 MB (101340157 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f8d27bfefcaaa84a89f93945c61ccf0af9ad50b1405d9acfa30e9da5ba1fb2db`  
		Last Modified: Wed, 14 Apr 2021 16:10:39 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6f599ec3e67dbcacd5ebae06ae984f5a688eba397e2280187ee399da88dc6ad`  
		Last Modified: Wed, 14 Apr 2021 16:10:38 GMT  
		Size: 4.3 MB (4262107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:780b42108cdc95774ec8d8239a9027e7382a875cf25306df1b01363dd2dc7aa4`  
		Last Modified: Wed, 14 Apr 2021 16:10:37 GMT  
		Size: 1.8 KB (1758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b002edb80987b79bb224f75e7c65e924d45dc54e548ce835539ca82dcdcc08e6`  
		Last Modified: Wed, 14 Apr 2021 16:10:37 GMT  
		Size: 1.2 KB (1176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c148b88ce7ff0e645ebee08b98beb32730028b41f85296f22b03154fa54614ac`  
		Last Modified: Wed, 14 Apr 2021 16:10:37 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43dc978ed7937ca238d82c78779b6e3a605e64ba31e2a5adac73bc7da1f63ede`  
		Last Modified: Wed, 14 Apr 2021 16:10:37 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.2.1-alpine`

```console
$ docker pull nats@sha256:cb99fd7d7cb5b5ed625ef86f9e847c26cb6e7c13f970765e77da331d0a13959d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.2.1-alpine` - linux; amd64

```console
$ docker pull nats@sha256:7b78ce1b52f0b0421d7f722c642c9b0feb9d340b9b4896b0c638960863934a0e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7303896 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d14bc60ccc43c89281be8e1cb48cba172a1bc16e08228e9fed919e32c40e64e6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 23:12:59 GMT
ENV NATS_SERVER=2.2.1
# Wed, 14 Apr 2021 23:13:02 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='0123d924907282265190258662edf8ad4351055083b5040e3bdf59117bd1c51c' ;; 		armhf) natsArch='arm6'; sha256='da719b07fd57137f85bfa6cffc7d00841a9c1fb4cdf7ca9a537bfc3f99b71f36' ;; 		armv7) natsArch='arm7'; sha256='cf6e8d9a9cc5d05f7320fb4be8fc9239cb87b91c6600a61ce7a2fb63e2f29f5a' ;; 		x86_64) natsArch='amd64'; sha256='70cb40d78b82ea6c0ca926c31ef98d2e1c885cfe2f73f34883e4ca448366c2dd' ;; 		x86) natsArch='386'; sha256='da54d129f8a52c048ded61e3b62e946037a9464d02cf818e568bbf1e385ce6be' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 14 Apr 2021 23:13:02 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Wed, 14 Apr 2021 23:13:02 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 14 Apr 2021 23:13:03 GMT
EXPOSE 4222 6222 8222
# Wed, 14 Apr 2021 23:13:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 23:13:03 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adf2b83a147ab10f7ee92b0624d9beb0101ff40b27dd92a1e74ec3bc972fa9f8`  
		Last Modified: Wed, 14 Apr 2021 23:13:45 GMT  
		Size: 4.5 MB (4490957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab1824f686e6029870ed0b1328708bbfe11b2c3b1bac6a461604b830ffdc13ce`  
		Last Modified: Wed, 14 Apr 2021 23:13:44 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:357bc9de7de4490d1629a64200e10f44bf96da1168b66f8bb512a3ce9d68bc23`  
		Last Modified: Wed, 14 Apr 2021 23:13:44 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2.1-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:eb3c514a433f020cd80da54de5a877d42c7f8aef888eef6fcf72b0175626cbd1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6784935 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:abd439f99c0768fd1ea54123118765e2c3a5e6f7e7f44c358794ce23c8590216`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Apr 2021 18:49:39 GMT
ADD file:4479f0a51530e039edf231d87201896dcff908aa542a613cdccb015f93dda8a3 in / 
# Wed, 14 Apr 2021 18:49:40 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 21:48:34 GMT
ENV NATS_SERVER=2.2.1
# Wed, 14 Apr 2021 21:49:16 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='0123d924907282265190258662edf8ad4351055083b5040e3bdf59117bd1c51c' ;; 		armhf) natsArch='arm6'; sha256='da719b07fd57137f85bfa6cffc7d00841a9c1fb4cdf7ca9a537bfc3f99b71f36' ;; 		armv7) natsArch='arm7'; sha256='cf6e8d9a9cc5d05f7320fb4be8fc9239cb87b91c6600a61ce7a2fb63e2f29f5a' ;; 		x86_64) natsArch='amd64'; sha256='70cb40d78b82ea6c0ca926c31ef98d2e1c885cfe2f73f34883e4ca448366c2dd' ;; 		x86) natsArch='386'; sha256='da54d129f8a52c048ded61e3b62e946037a9464d02cf818e568bbf1e385ce6be' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 14 Apr 2021 21:49:31 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Wed, 14 Apr 2021 21:49:41 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 14 Apr 2021 21:49:50 GMT
EXPOSE 4222 6222 8222
# Wed, 14 Apr 2021 21:49:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 21:50:03 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:740c950346cf39c85b52576998695c9b909c24a58a8bb1b64cce91fda3ef1d3a`  
		Last Modified: Wed, 14 Apr 2021 18:50:30 GMT  
		Size: 2.6 MB (2622131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22164d2f45f59e8f1d873e8a0c4769559100e469dc09c3bcbb61163732b2f453`  
		Last Modified: Wed, 14 Apr 2021 21:52:09 GMT  
		Size: 4.2 MB (4161829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79de2833ed16322bc62170a748bd3d746b8b152ec85cffa0cd11a3c25d822b35`  
		Last Modified: Wed, 14 Apr 2021 21:52:06 GMT  
		Size: 561.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f686c25c87f7ee66f2990e18510448fe0a0063432d6f894bd1a1b0917eaf37a`  
		Last Modified: Wed, 14 Apr 2021 21:52:09 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2.1-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:65016cde6a860e4e53a844e66d8944c0b72583aff8b0f17940f5883ce2025337
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6583191 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd85ddd622c92403cb491019f78c2760f9a3938378dadba44b3d1e382b1dd1db`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Apr 2021 18:57:39 GMT
ADD file:028c5b473d862250586e174c5dd19b37f8fc3bffbc02d888e72df30f32fd6129 in / 
# Wed, 14 Apr 2021 18:57:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 23:17:51 GMT
ENV NATS_SERVER=2.2.1
# Wed, 14 Apr 2021 23:17:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='0123d924907282265190258662edf8ad4351055083b5040e3bdf59117bd1c51c' ;; 		armhf) natsArch='arm6'; sha256='da719b07fd57137f85bfa6cffc7d00841a9c1fb4cdf7ca9a537bfc3f99b71f36' ;; 		armv7) natsArch='arm7'; sha256='cf6e8d9a9cc5d05f7320fb4be8fc9239cb87b91c6600a61ce7a2fb63e2f29f5a' ;; 		x86_64) natsArch='amd64'; sha256='70cb40d78b82ea6c0ca926c31ef98d2e1c885cfe2f73f34883e4ca448366c2dd' ;; 		x86) natsArch='386'; sha256='da54d129f8a52c048ded61e3b62e946037a9464d02cf818e568bbf1e385ce6be' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 14 Apr 2021 23:18:00 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Wed, 14 Apr 2021 23:18:02 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 14 Apr 2021 23:18:04 GMT
EXPOSE 4222 6222 8222
# Wed, 14 Apr 2021 23:18:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 23:18:09 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:e160e00eb35d5bc2373770873fbc9c8f5706045b0b06bfd1c364fcf69f02e9fe`  
		Last Modified: Wed, 14 Apr 2021 18:58:36 GMT  
		Size: 2.4 MB (2424145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3691a766339eab5091760e8ff801b39c69452b17fdd4fbd0e0cd710d241b5c5`  
		Last Modified: Wed, 14 Apr 2021 23:19:04 GMT  
		Size: 4.2 MB (4158072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a272e5ab96f7d43eb8e116aedf9e11bc1280f7ce6fbc83d2cbd82506c9ad760`  
		Last Modified: Wed, 14 Apr 2021 23:19:02 GMT  
		Size: 562.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e5adcdbbba76bad23d4bf8413449ce3ae2e70365468c47978d2c4ba7b937a67`  
		Last Modified: Wed, 14 Apr 2021 23:19:02 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2.1-alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:643201294279426bb51217496fc5e4053f55c0b29010efea1f201918efa1544a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6844402 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fd51943be05be331bd2fbd7b2494b10525553a8590e7041cda0723402b5d281a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Apr 2021 18:42:37 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Wed, 14 Apr 2021 18:42:38 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 23:37:11 GMT
ENV NATS_SERVER=2.2.1
# Wed, 14 Apr 2021 23:37:17 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='0123d924907282265190258662edf8ad4351055083b5040e3bdf59117bd1c51c' ;; 		armhf) natsArch='arm6'; sha256='da719b07fd57137f85bfa6cffc7d00841a9c1fb4cdf7ca9a537bfc3f99b71f36' ;; 		armv7) natsArch='arm7'; sha256='cf6e8d9a9cc5d05f7320fb4be8fc9239cb87b91c6600a61ce7a2fb63e2f29f5a' ;; 		x86_64) natsArch='amd64'; sha256='70cb40d78b82ea6c0ca926c31ef98d2e1c885cfe2f73f34883e4ca448366c2dd' ;; 		x86) natsArch='386'; sha256='da54d129f8a52c048ded61e3b62e946037a9464d02cf818e568bbf1e385ce6be' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 14 Apr 2021 23:37:18 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Wed, 14 Apr 2021 23:37:20 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 14 Apr 2021 23:37:25 GMT
EXPOSE 4222 6222 8222
# Wed, 14 Apr 2021 23:37:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 23:37:27 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:305503c7404cab7cb3fe558afe5d1b142f71b61815abb7d5b545be5d6fd274da`  
		Last Modified: Wed, 14 Apr 2021 23:41:37 GMT  
		Size: 4.1 MB (4131404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9504bc3187f368a20d4fe0020479a23dd57f07ea67deeb351297f4a8f1252dd7`  
		Last Modified: Wed, 14 Apr 2021 23:41:35 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0889a2e36f7ca1635400c49238cbb554ad2519b4a2c2cbfacff8cf2a1e21acd1`  
		Last Modified: Wed, 14 Apr 2021 23:41:35 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.2.1-alpine3.13`

```console
$ docker pull nats@sha256:cb99fd7d7cb5b5ed625ef86f9e847c26cb6e7c13f970765e77da331d0a13959d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.2.1-alpine3.13` - linux; amd64

```console
$ docker pull nats@sha256:7b78ce1b52f0b0421d7f722c642c9b0feb9d340b9b4896b0c638960863934a0e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7303896 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d14bc60ccc43c89281be8e1cb48cba172a1bc16e08228e9fed919e32c40e64e6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 23:12:59 GMT
ENV NATS_SERVER=2.2.1
# Wed, 14 Apr 2021 23:13:02 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='0123d924907282265190258662edf8ad4351055083b5040e3bdf59117bd1c51c' ;; 		armhf) natsArch='arm6'; sha256='da719b07fd57137f85bfa6cffc7d00841a9c1fb4cdf7ca9a537bfc3f99b71f36' ;; 		armv7) natsArch='arm7'; sha256='cf6e8d9a9cc5d05f7320fb4be8fc9239cb87b91c6600a61ce7a2fb63e2f29f5a' ;; 		x86_64) natsArch='amd64'; sha256='70cb40d78b82ea6c0ca926c31ef98d2e1c885cfe2f73f34883e4ca448366c2dd' ;; 		x86) natsArch='386'; sha256='da54d129f8a52c048ded61e3b62e946037a9464d02cf818e568bbf1e385ce6be' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 14 Apr 2021 23:13:02 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Wed, 14 Apr 2021 23:13:02 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 14 Apr 2021 23:13:03 GMT
EXPOSE 4222 6222 8222
# Wed, 14 Apr 2021 23:13:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 23:13:03 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adf2b83a147ab10f7ee92b0624d9beb0101ff40b27dd92a1e74ec3bc972fa9f8`  
		Last Modified: Wed, 14 Apr 2021 23:13:45 GMT  
		Size: 4.5 MB (4490957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab1824f686e6029870ed0b1328708bbfe11b2c3b1bac6a461604b830ffdc13ce`  
		Last Modified: Wed, 14 Apr 2021 23:13:44 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:357bc9de7de4490d1629a64200e10f44bf96da1168b66f8bb512a3ce9d68bc23`  
		Last Modified: Wed, 14 Apr 2021 23:13:44 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2.1-alpine3.13` - linux; arm variant v6

```console
$ docker pull nats@sha256:eb3c514a433f020cd80da54de5a877d42c7f8aef888eef6fcf72b0175626cbd1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6784935 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:abd439f99c0768fd1ea54123118765e2c3a5e6f7e7f44c358794ce23c8590216`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Apr 2021 18:49:39 GMT
ADD file:4479f0a51530e039edf231d87201896dcff908aa542a613cdccb015f93dda8a3 in / 
# Wed, 14 Apr 2021 18:49:40 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 21:48:34 GMT
ENV NATS_SERVER=2.2.1
# Wed, 14 Apr 2021 21:49:16 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='0123d924907282265190258662edf8ad4351055083b5040e3bdf59117bd1c51c' ;; 		armhf) natsArch='arm6'; sha256='da719b07fd57137f85bfa6cffc7d00841a9c1fb4cdf7ca9a537bfc3f99b71f36' ;; 		armv7) natsArch='arm7'; sha256='cf6e8d9a9cc5d05f7320fb4be8fc9239cb87b91c6600a61ce7a2fb63e2f29f5a' ;; 		x86_64) natsArch='amd64'; sha256='70cb40d78b82ea6c0ca926c31ef98d2e1c885cfe2f73f34883e4ca448366c2dd' ;; 		x86) natsArch='386'; sha256='da54d129f8a52c048ded61e3b62e946037a9464d02cf818e568bbf1e385ce6be' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 14 Apr 2021 21:49:31 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Wed, 14 Apr 2021 21:49:41 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 14 Apr 2021 21:49:50 GMT
EXPOSE 4222 6222 8222
# Wed, 14 Apr 2021 21:49:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 21:50:03 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:740c950346cf39c85b52576998695c9b909c24a58a8bb1b64cce91fda3ef1d3a`  
		Last Modified: Wed, 14 Apr 2021 18:50:30 GMT  
		Size: 2.6 MB (2622131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22164d2f45f59e8f1d873e8a0c4769559100e469dc09c3bcbb61163732b2f453`  
		Last Modified: Wed, 14 Apr 2021 21:52:09 GMT  
		Size: 4.2 MB (4161829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79de2833ed16322bc62170a748bd3d746b8b152ec85cffa0cd11a3c25d822b35`  
		Last Modified: Wed, 14 Apr 2021 21:52:06 GMT  
		Size: 561.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f686c25c87f7ee66f2990e18510448fe0a0063432d6f894bd1a1b0917eaf37a`  
		Last Modified: Wed, 14 Apr 2021 21:52:09 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2.1-alpine3.13` - linux; arm variant v7

```console
$ docker pull nats@sha256:65016cde6a860e4e53a844e66d8944c0b72583aff8b0f17940f5883ce2025337
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6583191 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd85ddd622c92403cb491019f78c2760f9a3938378dadba44b3d1e382b1dd1db`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Apr 2021 18:57:39 GMT
ADD file:028c5b473d862250586e174c5dd19b37f8fc3bffbc02d888e72df30f32fd6129 in / 
# Wed, 14 Apr 2021 18:57:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 23:17:51 GMT
ENV NATS_SERVER=2.2.1
# Wed, 14 Apr 2021 23:17:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='0123d924907282265190258662edf8ad4351055083b5040e3bdf59117bd1c51c' ;; 		armhf) natsArch='arm6'; sha256='da719b07fd57137f85bfa6cffc7d00841a9c1fb4cdf7ca9a537bfc3f99b71f36' ;; 		armv7) natsArch='arm7'; sha256='cf6e8d9a9cc5d05f7320fb4be8fc9239cb87b91c6600a61ce7a2fb63e2f29f5a' ;; 		x86_64) natsArch='amd64'; sha256='70cb40d78b82ea6c0ca926c31ef98d2e1c885cfe2f73f34883e4ca448366c2dd' ;; 		x86) natsArch='386'; sha256='da54d129f8a52c048ded61e3b62e946037a9464d02cf818e568bbf1e385ce6be' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 14 Apr 2021 23:18:00 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Wed, 14 Apr 2021 23:18:02 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 14 Apr 2021 23:18:04 GMT
EXPOSE 4222 6222 8222
# Wed, 14 Apr 2021 23:18:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 23:18:09 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:e160e00eb35d5bc2373770873fbc9c8f5706045b0b06bfd1c364fcf69f02e9fe`  
		Last Modified: Wed, 14 Apr 2021 18:58:36 GMT  
		Size: 2.4 MB (2424145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3691a766339eab5091760e8ff801b39c69452b17fdd4fbd0e0cd710d241b5c5`  
		Last Modified: Wed, 14 Apr 2021 23:19:04 GMT  
		Size: 4.2 MB (4158072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a272e5ab96f7d43eb8e116aedf9e11bc1280f7ce6fbc83d2cbd82506c9ad760`  
		Last Modified: Wed, 14 Apr 2021 23:19:02 GMT  
		Size: 562.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e5adcdbbba76bad23d4bf8413449ce3ae2e70365468c47978d2c4ba7b937a67`  
		Last Modified: Wed, 14 Apr 2021 23:19:02 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2.1-alpine3.13` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:643201294279426bb51217496fc5e4053f55c0b29010efea1f201918efa1544a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6844402 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fd51943be05be331bd2fbd7b2494b10525553a8590e7041cda0723402b5d281a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Apr 2021 18:42:37 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Wed, 14 Apr 2021 18:42:38 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 23:37:11 GMT
ENV NATS_SERVER=2.2.1
# Wed, 14 Apr 2021 23:37:17 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='0123d924907282265190258662edf8ad4351055083b5040e3bdf59117bd1c51c' ;; 		armhf) natsArch='arm6'; sha256='da719b07fd57137f85bfa6cffc7d00841a9c1fb4cdf7ca9a537bfc3f99b71f36' ;; 		armv7) natsArch='arm7'; sha256='cf6e8d9a9cc5d05f7320fb4be8fc9239cb87b91c6600a61ce7a2fb63e2f29f5a' ;; 		x86_64) natsArch='amd64'; sha256='70cb40d78b82ea6c0ca926c31ef98d2e1c885cfe2f73f34883e4ca448366c2dd' ;; 		x86) natsArch='386'; sha256='da54d129f8a52c048ded61e3b62e946037a9464d02cf818e568bbf1e385ce6be' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 14 Apr 2021 23:37:18 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Wed, 14 Apr 2021 23:37:20 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 14 Apr 2021 23:37:25 GMT
EXPOSE 4222 6222 8222
# Wed, 14 Apr 2021 23:37:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 23:37:27 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:305503c7404cab7cb3fe558afe5d1b142f71b61815abb7d5b545be5d6fd274da`  
		Last Modified: Wed, 14 Apr 2021 23:41:37 GMT  
		Size: 4.1 MB (4131404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9504bc3187f368a20d4fe0020479a23dd57f07ea67deeb351297f4a8f1252dd7`  
		Last Modified: Wed, 14 Apr 2021 23:41:35 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0889a2e36f7ca1635400c49238cbb554ad2519b4a2c2cbfacff8cf2a1e21acd1`  
		Last Modified: Wed, 14 Apr 2021 23:41:35 GMT  
		Size: 414.0 B  
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
$ docker pull nats@sha256:236c67f0c205b9cfab2809ce1dea44a20258d371c82264afd3172f29c8c70fb1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1879; amd64

### `nats:2.2.1-nanoserver` - windows version 10.0.17763.1879; amd64

```console
$ docker pull nats@sha256:545e15088a9a48d35878789abdde98cb7a98627e5a7c3be56f42abb2e13632e8
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.6 MB (105608630 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19ac61d30cc1900a1011f83ffa5dbcfd15a0a1754f790b94bdded5ed0cd4b673`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 08 Apr 2021 16:02:06 GMT
RUN Apply image 1809-amd64
# Wed, 14 Apr 2021 16:05:18 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 14 Apr 2021 16:05:20 GMT
RUN cmd /S /C #(nop) COPY file:428a7e80db4313301a46326a9a79832e9cbe7d78c94e749b5c295e813e484f21 in C:\nats-server.exe 
# Wed, 14 Apr 2021 16:05:21 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 14 Apr 2021 16:05:22 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 14 Apr 2021 16:05:22 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 14 Apr 2021 16:05:23 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:ea84579f6cd5b58fe78732be37450bd188c8923de3a2062664f3992861449b5c`  
		Size: 101.3 MB (101340157 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f8d27bfefcaaa84a89f93945c61ccf0af9ad50b1405d9acfa30e9da5ba1fb2db`  
		Last Modified: Wed, 14 Apr 2021 16:10:39 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6f599ec3e67dbcacd5ebae06ae984f5a688eba397e2280187ee399da88dc6ad`  
		Last Modified: Wed, 14 Apr 2021 16:10:38 GMT  
		Size: 4.3 MB (4262107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:780b42108cdc95774ec8d8239a9027e7382a875cf25306df1b01363dd2dc7aa4`  
		Last Modified: Wed, 14 Apr 2021 16:10:37 GMT  
		Size: 1.8 KB (1758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b002edb80987b79bb224f75e7c65e924d45dc54e548ce835539ca82dcdcc08e6`  
		Last Modified: Wed, 14 Apr 2021 16:10:37 GMT  
		Size: 1.2 KB (1176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c148b88ce7ff0e645ebee08b98beb32730028b41f85296f22b03154fa54614ac`  
		Last Modified: Wed, 14 Apr 2021 16:10:37 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43dc978ed7937ca238d82c78779b6e3a605e64ba31e2a5adac73bc7da1f63ede`  
		Last Modified: Wed, 14 Apr 2021 16:10:37 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.2.1-nanoserver-1809`

```console
$ docker pull nats@sha256:236c67f0c205b9cfab2809ce1dea44a20258d371c82264afd3172f29c8c70fb1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1879; amd64

### `nats:2.2.1-nanoserver-1809` - windows version 10.0.17763.1879; amd64

```console
$ docker pull nats@sha256:545e15088a9a48d35878789abdde98cb7a98627e5a7c3be56f42abb2e13632e8
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.6 MB (105608630 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19ac61d30cc1900a1011f83ffa5dbcfd15a0a1754f790b94bdded5ed0cd4b673`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 08 Apr 2021 16:02:06 GMT
RUN Apply image 1809-amd64
# Wed, 14 Apr 2021 16:05:18 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 14 Apr 2021 16:05:20 GMT
RUN cmd /S /C #(nop) COPY file:428a7e80db4313301a46326a9a79832e9cbe7d78c94e749b5c295e813e484f21 in C:\nats-server.exe 
# Wed, 14 Apr 2021 16:05:21 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 14 Apr 2021 16:05:22 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 14 Apr 2021 16:05:22 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 14 Apr 2021 16:05:23 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:ea84579f6cd5b58fe78732be37450bd188c8923de3a2062664f3992861449b5c`  
		Size: 101.3 MB (101340157 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f8d27bfefcaaa84a89f93945c61ccf0af9ad50b1405d9acfa30e9da5ba1fb2db`  
		Last Modified: Wed, 14 Apr 2021 16:10:39 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6f599ec3e67dbcacd5ebae06ae984f5a688eba397e2280187ee399da88dc6ad`  
		Last Modified: Wed, 14 Apr 2021 16:10:38 GMT  
		Size: 4.3 MB (4262107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:780b42108cdc95774ec8d8239a9027e7382a875cf25306df1b01363dd2dc7aa4`  
		Last Modified: Wed, 14 Apr 2021 16:10:37 GMT  
		Size: 1.8 KB (1758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b002edb80987b79bb224f75e7c65e924d45dc54e548ce835539ca82dcdcc08e6`  
		Last Modified: Wed, 14 Apr 2021 16:10:37 GMT  
		Size: 1.2 KB (1176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c148b88ce7ff0e645ebee08b98beb32730028b41f85296f22b03154fa54614ac`  
		Last Modified: Wed, 14 Apr 2021 16:10:37 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43dc978ed7937ca238d82c78779b6e3a605e64ba31e2a5adac73bc7da1f63ede`  
		Last Modified: Wed, 14 Apr 2021 16:10:37 GMT  
		Size: 1.1 KB (1149 bytes)  
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
$ docker pull nats@sha256:a6c1153fd919a539581471edd798478057cef10a6347e770d03336a20d5e472b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1879; amd64
	-	windows version 10.0.14393.4350; amd64

### `nats:2.2.1-windowsservercore` - windows version 10.0.17763.1879; amd64

```console
$ docker pull nats@sha256:9f3868f133ddd1a10ac71bbe835764e9d60e9b00081851a00ca05cd3362ea5d1
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2484142070 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2be425426bfa101eb4fdc6741eccbeaddde31c6c0761a665b4654dea39a17279`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 09 Apr 2021 20:34:41 GMT
RUN Install update 1809-amd64
# Wed, 14 Apr 2021 13:10:28 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 14 Apr 2021 16:02:50 GMT
ENV NATS_DOCKERIZED=1
# Wed, 14 Apr 2021 16:02:51 GMT
ENV NATS_SERVER=2.2.1
# Wed, 14 Apr 2021 16:02:52 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.2.1/nats-server-v2.2.1-windows-amd64.zip
# Wed, 14 Apr 2021 16:02:53 GMT
ENV GIT_DOWNLOAD_SHA256=1f0d48a7ba9200e2572016a9f3e1ec7e630f0518cc0b40950c14ff3a5d900924
# Wed, 14 Apr 2021 16:03:32 GMT
RUN Set-PSDebug -Trace 2
# Wed, 14 Apr 2021 16:04:53 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 14 Apr 2021 16:04:55 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 14 Apr 2021 16:04:56 GMT
EXPOSE 4222 6222 8222
# Wed, 14 Apr 2021 16:04:57 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 14 Apr 2021 16:04:58 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:399f118dfaa9a753e98d128238b944432c7bcabea88a2998a6efbbece28ed303`  
		Size: 751.4 MB (751421005 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b2159a5d0f75ce11e6fe71e4260ede5c3c88a9eb76a0ff43ac6746b2b9b96775`  
		Last Modified: Wed, 14 Apr 2021 15:37:10 GMT  
		Size: 1.4 KB (1446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e849354f21f856ec720d6daecc37978fd7246f376ba3c32fd63d4400cce357bc`  
		Last Modified: Wed, 14 Apr 2021 16:10:16 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daae5ee02f484d7c054ad550cbee6900a35477f4e23e322cc3af6eb7c4690416`  
		Last Modified: Wed, 14 Apr 2021 16:10:14 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d4df8575d5fc511a7ac278cfc55a4053b36afce4c0bcae2af0af7907c7f91e6`  
		Last Modified: Wed, 14 Apr 2021 16:10:14 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:570a7e5edba00d92281a4a147639b5fc0b6724693cbfed80007b5b5db612a3e8`  
		Last Modified: Wed, 14 Apr 2021 16:10:13 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60092b7b0679ad17236eb09b832adcc7bb67a5fd8c2d9a69ffbfc863716274c2`  
		Last Modified: Wed, 14 Apr 2021 16:10:15 GMT  
		Size: 5.1 MB (5072726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d5d3b99689d155ccd6cdf6acbc7ef61472c65ce2cee49f441c4c3b844242410`  
		Last Modified: Wed, 14 Apr 2021 16:10:13 GMT  
		Size: 9.3 MB (9302175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23dae780c7132cf39c97d1602e11b6a58481594df6d896054f3a9e6e9f54e63a`  
		Last Modified: Wed, 14 Apr 2021 16:10:10 GMT  
		Size: 2.0 KB (1957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95f2291e14ae4d6e97942f3284122a80c7c969cb9bcfc9a417a833439505f85d`  
		Last Modified: Wed, 14 Apr 2021 16:10:11 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69b07be56d63a82b0606023df13bf32a522a13a12a44c53116ec24d0c1bd2ca1`  
		Last Modified: Wed, 14 Apr 2021 16:10:11 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb6cc0327d5edba60d3e99a97fa6c015e1953c9451bc816f20d6d73a67b9e426`  
		Last Modified: Wed, 14 Apr 2021 16:10:11 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2.1-windowsservercore` - windows version 10.0.14393.4350; amd64

```console
$ docker pull nats@sha256:ad5ac25aa423d2df82324037dd73fec641098cd5f198cf98ccf19f4ae640d1f5
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5814950471 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0fc9b58b0a6e7d867ee74a6023bf1768d2dad684760ace428c0bf425357fcc5c`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 07 Apr 2021 21:54:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 14 Apr 2021 13:22:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 14 Apr 2021 16:05:33 GMT
ENV NATS_DOCKERIZED=1
# Wed, 14 Apr 2021 16:05:33 GMT
ENV NATS_SERVER=2.2.1
# Wed, 14 Apr 2021 16:05:35 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.2.1/nats-server-v2.2.1-windows-amd64.zip
# Wed, 14 Apr 2021 16:05:35 GMT
ENV GIT_DOWNLOAD_SHA256=1f0d48a7ba9200e2572016a9f3e1ec7e630f0518cc0b40950c14ff3a5d900924
# Wed, 14 Apr 2021 16:06:59 GMT
RUN Set-PSDebug -Trace 2
# Wed, 14 Apr 2021 16:09:18 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 14 Apr 2021 16:09:19 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 14 Apr 2021 16:09:20 GMT
EXPOSE 4222 6222 8222
# Wed, 14 Apr 2021 16:09:21 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 14 Apr 2021 16:09:23 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:00b4edb823e6a375d179a28cbfa682c2379d62179e1518485902d6e68b9a9d1e`  
		Size: 1.7 GB (1724897968 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f616bb7876e6f944d82fa1802ffab5ca4931a63e1b999f0851b52120cda83539`  
		Last Modified: Wed, 14 Apr 2021 15:37:43 GMT  
		Size: 1.3 KB (1307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcfa54f43457753c391f21da5e9a5bf47c61c574c0da04b8614d0e84bf823f54`  
		Last Modified: Wed, 14 Apr 2021 16:11:03 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04d71ba1c574073f9d5dd016585c2fe26ac560c192f7aa36ce54d4c12832997f`  
		Last Modified: Wed, 14 Apr 2021 16:11:01 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e9f66539738348100cf9f1e6a5bc40e8c2123bafb9329f5df3cf20a2015db33`  
		Last Modified: Wed, 14 Apr 2021 16:11:00 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20f2eae922462b2537c1d0d32d548cb10190f6bda0d02da57440cc229da692b3`  
		Last Modified: Wed, 14 Apr 2021 16:11:00 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ea168f84532f340be87f19704511ee160cbdc5b9c6ad8962fcd80e9fb8efea7`  
		Last Modified: Wed, 14 Apr 2021 16:11:01 GMT  
		Size: 5.7 MB (5651953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2eda2d9556eb5afaf10e6300ac36ddc1383144ae65671ca3a01b24bac150c540`  
		Last Modified: Wed, 14 Apr 2021 16:11:01 GMT  
		Size: 14.4 MB (14401439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a04b0d9d602bb1f9c6fb7925bb92959ebcff2c30e6ca6a658cdd9976d662d70`  
		Last Modified: Wed, 14 Apr 2021 16:10:57 GMT  
		Size: 2.0 KB (1984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e5e865356a464c9006414a165a6d0ffb8f062fa737be2ad42e1aa58fcfca23c`  
		Last Modified: Wed, 14 Apr 2021 16:10:56 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3533148ddde03cc5f28669b26c30dee8685db418d250a4b4829e465c0be8a7e`  
		Last Modified: Wed, 14 Apr 2021 16:10:56 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4573099491ec9887bd66033f55b39f6b897d1f59f21f679fdff4f822ebd7ea15`  
		Last Modified: Wed, 14 Apr 2021 16:10:56 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.2.1-windowsservercore-1809`

```console
$ docker pull nats@sha256:3002e35b4bb91080eac08408891e6bb9155d38086cbb6fcfb654b61e0d2383e0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1879; amd64

### `nats:2.2.1-windowsservercore-1809` - windows version 10.0.17763.1879; amd64

```console
$ docker pull nats@sha256:9f3868f133ddd1a10ac71bbe835764e9d60e9b00081851a00ca05cd3362ea5d1
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2484142070 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2be425426bfa101eb4fdc6741eccbeaddde31c6c0761a665b4654dea39a17279`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 09 Apr 2021 20:34:41 GMT
RUN Install update 1809-amd64
# Wed, 14 Apr 2021 13:10:28 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 14 Apr 2021 16:02:50 GMT
ENV NATS_DOCKERIZED=1
# Wed, 14 Apr 2021 16:02:51 GMT
ENV NATS_SERVER=2.2.1
# Wed, 14 Apr 2021 16:02:52 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.2.1/nats-server-v2.2.1-windows-amd64.zip
# Wed, 14 Apr 2021 16:02:53 GMT
ENV GIT_DOWNLOAD_SHA256=1f0d48a7ba9200e2572016a9f3e1ec7e630f0518cc0b40950c14ff3a5d900924
# Wed, 14 Apr 2021 16:03:32 GMT
RUN Set-PSDebug -Trace 2
# Wed, 14 Apr 2021 16:04:53 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 14 Apr 2021 16:04:55 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 14 Apr 2021 16:04:56 GMT
EXPOSE 4222 6222 8222
# Wed, 14 Apr 2021 16:04:57 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 14 Apr 2021 16:04:58 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:399f118dfaa9a753e98d128238b944432c7bcabea88a2998a6efbbece28ed303`  
		Size: 751.4 MB (751421005 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b2159a5d0f75ce11e6fe71e4260ede5c3c88a9eb76a0ff43ac6746b2b9b96775`  
		Last Modified: Wed, 14 Apr 2021 15:37:10 GMT  
		Size: 1.4 KB (1446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e849354f21f856ec720d6daecc37978fd7246f376ba3c32fd63d4400cce357bc`  
		Last Modified: Wed, 14 Apr 2021 16:10:16 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daae5ee02f484d7c054ad550cbee6900a35477f4e23e322cc3af6eb7c4690416`  
		Last Modified: Wed, 14 Apr 2021 16:10:14 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d4df8575d5fc511a7ac278cfc55a4053b36afce4c0bcae2af0af7907c7f91e6`  
		Last Modified: Wed, 14 Apr 2021 16:10:14 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:570a7e5edba00d92281a4a147639b5fc0b6724693cbfed80007b5b5db612a3e8`  
		Last Modified: Wed, 14 Apr 2021 16:10:13 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60092b7b0679ad17236eb09b832adcc7bb67a5fd8c2d9a69ffbfc863716274c2`  
		Last Modified: Wed, 14 Apr 2021 16:10:15 GMT  
		Size: 5.1 MB (5072726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d5d3b99689d155ccd6cdf6acbc7ef61472c65ce2cee49f441c4c3b844242410`  
		Last Modified: Wed, 14 Apr 2021 16:10:13 GMT  
		Size: 9.3 MB (9302175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23dae780c7132cf39c97d1602e11b6a58481594df6d896054f3a9e6e9f54e63a`  
		Last Modified: Wed, 14 Apr 2021 16:10:10 GMT  
		Size: 2.0 KB (1957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95f2291e14ae4d6e97942f3284122a80c7c969cb9bcfc9a417a833439505f85d`  
		Last Modified: Wed, 14 Apr 2021 16:10:11 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69b07be56d63a82b0606023df13bf32a522a13a12a44c53116ec24d0c1bd2ca1`  
		Last Modified: Wed, 14 Apr 2021 16:10:11 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb6cc0327d5edba60d3e99a97fa6c015e1953c9451bc816f20d6d73a67b9e426`  
		Last Modified: Wed, 14 Apr 2021 16:10:11 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.2.1-windowsservercore-ltsc2016`

```console
$ docker pull nats@sha256:486439b61d7c8307b15b01bae5f574784e333ee642d1d3285e3bf61785ea00cd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4350; amd64

### `nats:2.2.1-windowsservercore-ltsc2016` - windows version 10.0.14393.4350; amd64

```console
$ docker pull nats@sha256:ad5ac25aa423d2df82324037dd73fec641098cd5f198cf98ccf19f4ae640d1f5
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5814950471 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0fc9b58b0a6e7d867ee74a6023bf1768d2dad684760ace428c0bf425357fcc5c`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 07 Apr 2021 21:54:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 14 Apr 2021 13:22:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 14 Apr 2021 16:05:33 GMT
ENV NATS_DOCKERIZED=1
# Wed, 14 Apr 2021 16:05:33 GMT
ENV NATS_SERVER=2.2.1
# Wed, 14 Apr 2021 16:05:35 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.2.1/nats-server-v2.2.1-windows-amd64.zip
# Wed, 14 Apr 2021 16:05:35 GMT
ENV GIT_DOWNLOAD_SHA256=1f0d48a7ba9200e2572016a9f3e1ec7e630f0518cc0b40950c14ff3a5d900924
# Wed, 14 Apr 2021 16:06:59 GMT
RUN Set-PSDebug -Trace 2
# Wed, 14 Apr 2021 16:09:18 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 14 Apr 2021 16:09:19 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 14 Apr 2021 16:09:20 GMT
EXPOSE 4222 6222 8222
# Wed, 14 Apr 2021 16:09:21 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 14 Apr 2021 16:09:23 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:00b4edb823e6a375d179a28cbfa682c2379d62179e1518485902d6e68b9a9d1e`  
		Size: 1.7 GB (1724897968 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f616bb7876e6f944d82fa1802ffab5ca4931a63e1b999f0851b52120cda83539`  
		Last Modified: Wed, 14 Apr 2021 15:37:43 GMT  
		Size: 1.3 KB (1307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcfa54f43457753c391f21da5e9a5bf47c61c574c0da04b8614d0e84bf823f54`  
		Last Modified: Wed, 14 Apr 2021 16:11:03 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04d71ba1c574073f9d5dd016585c2fe26ac560c192f7aa36ce54d4c12832997f`  
		Last Modified: Wed, 14 Apr 2021 16:11:01 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e9f66539738348100cf9f1e6a5bc40e8c2123bafb9329f5df3cf20a2015db33`  
		Last Modified: Wed, 14 Apr 2021 16:11:00 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20f2eae922462b2537c1d0d32d548cb10190f6bda0d02da57440cc229da692b3`  
		Last Modified: Wed, 14 Apr 2021 16:11:00 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ea168f84532f340be87f19704511ee160cbdc5b9c6ad8962fcd80e9fb8efea7`  
		Last Modified: Wed, 14 Apr 2021 16:11:01 GMT  
		Size: 5.7 MB (5651953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2eda2d9556eb5afaf10e6300ac36ddc1383144ae65671ca3a01b24bac150c540`  
		Last Modified: Wed, 14 Apr 2021 16:11:01 GMT  
		Size: 14.4 MB (14401439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a04b0d9d602bb1f9c6fb7925bb92959ebcff2c30e6ca6a658cdd9976d662d70`  
		Last Modified: Wed, 14 Apr 2021 16:10:57 GMT  
		Size: 2.0 KB (1984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e5e865356a464c9006414a165a6d0ffb8f062fa737be2ad42e1aa58fcfca23c`  
		Last Modified: Wed, 14 Apr 2021 16:10:56 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3533148ddde03cc5f28669b26c30dee8685db418d250a4b4829e465c0be8a7e`  
		Last Modified: Wed, 14 Apr 2021 16:10:56 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4573099491ec9887bd66033f55b39f6b897d1f59f21f679fdff4f822ebd7ea15`  
		Last Modified: Wed, 14 Apr 2021 16:10:56 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:alpine`

```console
$ docker pull nats@sha256:cb99fd7d7cb5b5ed625ef86f9e847c26cb6e7c13f970765e77da331d0a13959d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:alpine` - linux; amd64

```console
$ docker pull nats@sha256:7b78ce1b52f0b0421d7f722c642c9b0feb9d340b9b4896b0c638960863934a0e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7303896 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d14bc60ccc43c89281be8e1cb48cba172a1bc16e08228e9fed919e32c40e64e6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 23:12:59 GMT
ENV NATS_SERVER=2.2.1
# Wed, 14 Apr 2021 23:13:02 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='0123d924907282265190258662edf8ad4351055083b5040e3bdf59117bd1c51c' ;; 		armhf) natsArch='arm6'; sha256='da719b07fd57137f85bfa6cffc7d00841a9c1fb4cdf7ca9a537bfc3f99b71f36' ;; 		armv7) natsArch='arm7'; sha256='cf6e8d9a9cc5d05f7320fb4be8fc9239cb87b91c6600a61ce7a2fb63e2f29f5a' ;; 		x86_64) natsArch='amd64'; sha256='70cb40d78b82ea6c0ca926c31ef98d2e1c885cfe2f73f34883e4ca448366c2dd' ;; 		x86) natsArch='386'; sha256='da54d129f8a52c048ded61e3b62e946037a9464d02cf818e568bbf1e385ce6be' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 14 Apr 2021 23:13:02 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Wed, 14 Apr 2021 23:13:02 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 14 Apr 2021 23:13:03 GMT
EXPOSE 4222 6222 8222
# Wed, 14 Apr 2021 23:13:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 23:13:03 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adf2b83a147ab10f7ee92b0624d9beb0101ff40b27dd92a1e74ec3bc972fa9f8`  
		Last Modified: Wed, 14 Apr 2021 23:13:45 GMT  
		Size: 4.5 MB (4490957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab1824f686e6029870ed0b1328708bbfe11b2c3b1bac6a461604b830ffdc13ce`  
		Last Modified: Wed, 14 Apr 2021 23:13:44 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:357bc9de7de4490d1629a64200e10f44bf96da1168b66f8bb512a3ce9d68bc23`  
		Last Modified: Wed, 14 Apr 2021 23:13:44 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:eb3c514a433f020cd80da54de5a877d42c7f8aef888eef6fcf72b0175626cbd1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6784935 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:abd439f99c0768fd1ea54123118765e2c3a5e6f7e7f44c358794ce23c8590216`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Apr 2021 18:49:39 GMT
ADD file:4479f0a51530e039edf231d87201896dcff908aa542a613cdccb015f93dda8a3 in / 
# Wed, 14 Apr 2021 18:49:40 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 21:48:34 GMT
ENV NATS_SERVER=2.2.1
# Wed, 14 Apr 2021 21:49:16 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='0123d924907282265190258662edf8ad4351055083b5040e3bdf59117bd1c51c' ;; 		armhf) natsArch='arm6'; sha256='da719b07fd57137f85bfa6cffc7d00841a9c1fb4cdf7ca9a537bfc3f99b71f36' ;; 		armv7) natsArch='arm7'; sha256='cf6e8d9a9cc5d05f7320fb4be8fc9239cb87b91c6600a61ce7a2fb63e2f29f5a' ;; 		x86_64) natsArch='amd64'; sha256='70cb40d78b82ea6c0ca926c31ef98d2e1c885cfe2f73f34883e4ca448366c2dd' ;; 		x86) natsArch='386'; sha256='da54d129f8a52c048ded61e3b62e946037a9464d02cf818e568bbf1e385ce6be' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 14 Apr 2021 21:49:31 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Wed, 14 Apr 2021 21:49:41 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 14 Apr 2021 21:49:50 GMT
EXPOSE 4222 6222 8222
# Wed, 14 Apr 2021 21:49:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 21:50:03 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:740c950346cf39c85b52576998695c9b909c24a58a8bb1b64cce91fda3ef1d3a`  
		Last Modified: Wed, 14 Apr 2021 18:50:30 GMT  
		Size: 2.6 MB (2622131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22164d2f45f59e8f1d873e8a0c4769559100e469dc09c3bcbb61163732b2f453`  
		Last Modified: Wed, 14 Apr 2021 21:52:09 GMT  
		Size: 4.2 MB (4161829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79de2833ed16322bc62170a748bd3d746b8b152ec85cffa0cd11a3c25d822b35`  
		Last Modified: Wed, 14 Apr 2021 21:52:06 GMT  
		Size: 561.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f686c25c87f7ee66f2990e18510448fe0a0063432d6f894bd1a1b0917eaf37a`  
		Last Modified: Wed, 14 Apr 2021 21:52:09 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:65016cde6a860e4e53a844e66d8944c0b72583aff8b0f17940f5883ce2025337
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6583191 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd85ddd622c92403cb491019f78c2760f9a3938378dadba44b3d1e382b1dd1db`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Apr 2021 18:57:39 GMT
ADD file:028c5b473d862250586e174c5dd19b37f8fc3bffbc02d888e72df30f32fd6129 in / 
# Wed, 14 Apr 2021 18:57:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 23:17:51 GMT
ENV NATS_SERVER=2.2.1
# Wed, 14 Apr 2021 23:17:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='0123d924907282265190258662edf8ad4351055083b5040e3bdf59117bd1c51c' ;; 		armhf) natsArch='arm6'; sha256='da719b07fd57137f85bfa6cffc7d00841a9c1fb4cdf7ca9a537bfc3f99b71f36' ;; 		armv7) natsArch='arm7'; sha256='cf6e8d9a9cc5d05f7320fb4be8fc9239cb87b91c6600a61ce7a2fb63e2f29f5a' ;; 		x86_64) natsArch='amd64'; sha256='70cb40d78b82ea6c0ca926c31ef98d2e1c885cfe2f73f34883e4ca448366c2dd' ;; 		x86) natsArch='386'; sha256='da54d129f8a52c048ded61e3b62e946037a9464d02cf818e568bbf1e385ce6be' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 14 Apr 2021 23:18:00 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Wed, 14 Apr 2021 23:18:02 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 14 Apr 2021 23:18:04 GMT
EXPOSE 4222 6222 8222
# Wed, 14 Apr 2021 23:18:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 23:18:09 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:e160e00eb35d5bc2373770873fbc9c8f5706045b0b06bfd1c364fcf69f02e9fe`  
		Last Modified: Wed, 14 Apr 2021 18:58:36 GMT  
		Size: 2.4 MB (2424145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3691a766339eab5091760e8ff801b39c69452b17fdd4fbd0e0cd710d241b5c5`  
		Last Modified: Wed, 14 Apr 2021 23:19:04 GMT  
		Size: 4.2 MB (4158072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a272e5ab96f7d43eb8e116aedf9e11bc1280f7ce6fbc83d2cbd82506c9ad760`  
		Last Modified: Wed, 14 Apr 2021 23:19:02 GMT  
		Size: 562.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e5adcdbbba76bad23d4bf8413449ce3ae2e70365468c47978d2c4ba7b937a67`  
		Last Modified: Wed, 14 Apr 2021 23:19:02 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:643201294279426bb51217496fc5e4053f55c0b29010efea1f201918efa1544a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6844402 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fd51943be05be331bd2fbd7b2494b10525553a8590e7041cda0723402b5d281a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Apr 2021 18:42:37 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Wed, 14 Apr 2021 18:42:38 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 23:37:11 GMT
ENV NATS_SERVER=2.2.1
# Wed, 14 Apr 2021 23:37:17 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='0123d924907282265190258662edf8ad4351055083b5040e3bdf59117bd1c51c' ;; 		armhf) natsArch='arm6'; sha256='da719b07fd57137f85bfa6cffc7d00841a9c1fb4cdf7ca9a537bfc3f99b71f36' ;; 		armv7) natsArch='arm7'; sha256='cf6e8d9a9cc5d05f7320fb4be8fc9239cb87b91c6600a61ce7a2fb63e2f29f5a' ;; 		x86_64) natsArch='amd64'; sha256='70cb40d78b82ea6c0ca926c31ef98d2e1c885cfe2f73f34883e4ca448366c2dd' ;; 		x86) natsArch='386'; sha256='da54d129f8a52c048ded61e3b62e946037a9464d02cf818e568bbf1e385ce6be' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 14 Apr 2021 23:37:18 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Wed, 14 Apr 2021 23:37:20 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 14 Apr 2021 23:37:25 GMT
EXPOSE 4222 6222 8222
# Wed, 14 Apr 2021 23:37:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 23:37:27 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:305503c7404cab7cb3fe558afe5d1b142f71b61815abb7d5b545be5d6fd274da`  
		Last Modified: Wed, 14 Apr 2021 23:41:37 GMT  
		Size: 4.1 MB (4131404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9504bc3187f368a20d4fe0020479a23dd57f07ea67deeb351297f4a8f1252dd7`  
		Last Modified: Wed, 14 Apr 2021 23:41:35 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0889a2e36f7ca1635400c49238cbb554ad2519b4a2c2cbfacff8cf2a1e21acd1`  
		Last Modified: Wed, 14 Apr 2021 23:41:35 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:alpine3.13`

```console
$ docker pull nats@sha256:cb99fd7d7cb5b5ed625ef86f9e847c26cb6e7c13f970765e77da331d0a13959d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:alpine3.13` - linux; amd64

```console
$ docker pull nats@sha256:7b78ce1b52f0b0421d7f722c642c9b0feb9d340b9b4896b0c638960863934a0e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7303896 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d14bc60ccc43c89281be8e1cb48cba172a1bc16e08228e9fed919e32c40e64e6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 23:12:59 GMT
ENV NATS_SERVER=2.2.1
# Wed, 14 Apr 2021 23:13:02 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='0123d924907282265190258662edf8ad4351055083b5040e3bdf59117bd1c51c' ;; 		armhf) natsArch='arm6'; sha256='da719b07fd57137f85bfa6cffc7d00841a9c1fb4cdf7ca9a537bfc3f99b71f36' ;; 		armv7) natsArch='arm7'; sha256='cf6e8d9a9cc5d05f7320fb4be8fc9239cb87b91c6600a61ce7a2fb63e2f29f5a' ;; 		x86_64) natsArch='amd64'; sha256='70cb40d78b82ea6c0ca926c31ef98d2e1c885cfe2f73f34883e4ca448366c2dd' ;; 		x86) natsArch='386'; sha256='da54d129f8a52c048ded61e3b62e946037a9464d02cf818e568bbf1e385ce6be' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 14 Apr 2021 23:13:02 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Wed, 14 Apr 2021 23:13:02 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 14 Apr 2021 23:13:03 GMT
EXPOSE 4222 6222 8222
# Wed, 14 Apr 2021 23:13:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 23:13:03 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adf2b83a147ab10f7ee92b0624d9beb0101ff40b27dd92a1e74ec3bc972fa9f8`  
		Last Modified: Wed, 14 Apr 2021 23:13:45 GMT  
		Size: 4.5 MB (4490957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab1824f686e6029870ed0b1328708bbfe11b2c3b1bac6a461604b830ffdc13ce`  
		Last Modified: Wed, 14 Apr 2021 23:13:44 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:357bc9de7de4490d1629a64200e10f44bf96da1168b66f8bb512a3ce9d68bc23`  
		Last Modified: Wed, 14 Apr 2021 23:13:44 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.13` - linux; arm variant v6

```console
$ docker pull nats@sha256:eb3c514a433f020cd80da54de5a877d42c7f8aef888eef6fcf72b0175626cbd1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6784935 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:abd439f99c0768fd1ea54123118765e2c3a5e6f7e7f44c358794ce23c8590216`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Apr 2021 18:49:39 GMT
ADD file:4479f0a51530e039edf231d87201896dcff908aa542a613cdccb015f93dda8a3 in / 
# Wed, 14 Apr 2021 18:49:40 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 21:48:34 GMT
ENV NATS_SERVER=2.2.1
# Wed, 14 Apr 2021 21:49:16 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='0123d924907282265190258662edf8ad4351055083b5040e3bdf59117bd1c51c' ;; 		armhf) natsArch='arm6'; sha256='da719b07fd57137f85bfa6cffc7d00841a9c1fb4cdf7ca9a537bfc3f99b71f36' ;; 		armv7) natsArch='arm7'; sha256='cf6e8d9a9cc5d05f7320fb4be8fc9239cb87b91c6600a61ce7a2fb63e2f29f5a' ;; 		x86_64) natsArch='amd64'; sha256='70cb40d78b82ea6c0ca926c31ef98d2e1c885cfe2f73f34883e4ca448366c2dd' ;; 		x86) natsArch='386'; sha256='da54d129f8a52c048ded61e3b62e946037a9464d02cf818e568bbf1e385ce6be' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 14 Apr 2021 21:49:31 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Wed, 14 Apr 2021 21:49:41 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 14 Apr 2021 21:49:50 GMT
EXPOSE 4222 6222 8222
# Wed, 14 Apr 2021 21:49:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 21:50:03 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:740c950346cf39c85b52576998695c9b909c24a58a8bb1b64cce91fda3ef1d3a`  
		Last Modified: Wed, 14 Apr 2021 18:50:30 GMT  
		Size: 2.6 MB (2622131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22164d2f45f59e8f1d873e8a0c4769559100e469dc09c3bcbb61163732b2f453`  
		Last Modified: Wed, 14 Apr 2021 21:52:09 GMT  
		Size: 4.2 MB (4161829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79de2833ed16322bc62170a748bd3d746b8b152ec85cffa0cd11a3c25d822b35`  
		Last Modified: Wed, 14 Apr 2021 21:52:06 GMT  
		Size: 561.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f686c25c87f7ee66f2990e18510448fe0a0063432d6f894bd1a1b0917eaf37a`  
		Last Modified: Wed, 14 Apr 2021 21:52:09 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.13` - linux; arm variant v7

```console
$ docker pull nats@sha256:65016cde6a860e4e53a844e66d8944c0b72583aff8b0f17940f5883ce2025337
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6583191 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd85ddd622c92403cb491019f78c2760f9a3938378dadba44b3d1e382b1dd1db`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Apr 2021 18:57:39 GMT
ADD file:028c5b473d862250586e174c5dd19b37f8fc3bffbc02d888e72df30f32fd6129 in / 
# Wed, 14 Apr 2021 18:57:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 23:17:51 GMT
ENV NATS_SERVER=2.2.1
# Wed, 14 Apr 2021 23:17:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='0123d924907282265190258662edf8ad4351055083b5040e3bdf59117bd1c51c' ;; 		armhf) natsArch='arm6'; sha256='da719b07fd57137f85bfa6cffc7d00841a9c1fb4cdf7ca9a537bfc3f99b71f36' ;; 		armv7) natsArch='arm7'; sha256='cf6e8d9a9cc5d05f7320fb4be8fc9239cb87b91c6600a61ce7a2fb63e2f29f5a' ;; 		x86_64) natsArch='amd64'; sha256='70cb40d78b82ea6c0ca926c31ef98d2e1c885cfe2f73f34883e4ca448366c2dd' ;; 		x86) natsArch='386'; sha256='da54d129f8a52c048ded61e3b62e946037a9464d02cf818e568bbf1e385ce6be' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 14 Apr 2021 23:18:00 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Wed, 14 Apr 2021 23:18:02 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 14 Apr 2021 23:18:04 GMT
EXPOSE 4222 6222 8222
# Wed, 14 Apr 2021 23:18:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 23:18:09 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:e160e00eb35d5bc2373770873fbc9c8f5706045b0b06bfd1c364fcf69f02e9fe`  
		Last Modified: Wed, 14 Apr 2021 18:58:36 GMT  
		Size: 2.4 MB (2424145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3691a766339eab5091760e8ff801b39c69452b17fdd4fbd0e0cd710d241b5c5`  
		Last Modified: Wed, 14 Apr 2021 23:19:04 GMT  
		Size: 4.2 MB (4158072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a272e5ab96f7d43eb8e116aedf9e11bc1280f7ce6fbc83d2cbd82506c9ad760`  
		Last Modified: Wed, 14 Apr 2021 23:19:02 GMT  
		Size: 562.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e5adcdbbba76bad23d4bf8413449ce3ae2e70365468c47978d2c4ba7b937a67`  
		Last Modified: Wed, 14 Apr 2021 23:19:02 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.13` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:643201294279426bb51217496fc5e4053f55c0b29010efea1f201918efa1544a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6844402 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fd51943be05be331bd2fbd7b2494b10525553a8590e7041cda0723402b5d281a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Apr 2021 18:42:37 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Wed, 14 Apr 2021 18:42:38 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 23:37:11 GMT
ENV NATS_SERVER=2.2.1
# Wed, 14 Apr 2021 23:37:17 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='0123d924907282265190258662edf8ad4351055083b5040e3bdf59117bd1c51c' ;; 		armhf) natsArch='arm6'; sha256='da719b07fd57137f85bfa6cffc7d00841a9c1fb4cdf7ca9a537bfc3f99b71f36' ;; 		armv7) natsArch='arm7'; sha256='cf6e8d9a9cc5d05f7320fb4be8fc9239cb87b91c6600a61ce7a2fb63e2f29f5a' ;; 		x86_64) natsArch='amd64'; sha256='70cb40d78b82ea6c0ca926c31ef98d2e1c885cfe2f73f34883e4ca448366c2dd' ;; 		x86) natsArch='386'; sha256='da54d129f8a52c048ded61e3b62e946037a9464d02cf818e568bbf1e385ce6be' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 14 Apr 2021 23:37:18 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Wed, 14 Apr 2021 23:37:20 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 14 Apr 2021 23:37:25 GMT
EXPOSE 4222 6222 8222
# Wed, 14 Apr 2021 23:37:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 23:37:27 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:305503c7404cab7cb3fe558afe5d1b142f71b61815abb7d5b545be5d6fd274da`  
		Last Modified: Wed, 14 Apr 2021 23:41:37 GMT  
		Size: 4.1 MB (4131404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9504bc3187f368a20d4fe0020479a23dd57f07ea67deeb351297f4a8f1252dd7`  
		Last Modified: Wed, 14 Apr 2021 23:41:35 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0889a2e36f7ca1635400c49238cbb554ad2519b4a2c2cbfacff8cf2a1e21acd1`  
		Last Modified: Wed, 14 Apr 2021 23:41:35 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:latest`

```console
$ docker pull nats@sha256:f0c80abcc8d86c26b77b4cfbf150821d7e71ace88e2ea39d8a5bfa33caf0317a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.1879; amd64

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

### `nats:latest` - windows version 10.0.17763.1879; amd64

```console
$ docker pull nats@sha256:545e15088a9a48d35878789abdde98cb7a98627e5a7c3be56f42abb2e13632e8
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.6 MB (105608630 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19ac61d30cc1900a1011f83ffa5dbcfd15a0a1754f790b94bdded5ed0cd4b673`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 08 Apr 2021 16:02:06 GMT
RUN Apply image 1809-amd64
# Wed, 14 Apr 2021 16:05:18 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 14 Apr 2021 16:05:20 GMT
RUN cmd /S /C #(nop) COPY file:428a7e80db4313301a46326a9a79832e9cbe7d78c94e749b5c295e813e484f21 in C:\nats-server.exe 
# Wed, 14 Apr 2021 16:05:21 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 14 Apr 2021 16:05:22 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 14 Apr 2021 16:05:22 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 14 Apr 2021 16:05:23 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:ea84579f6cd5b58fe78732be37450bd188c8923de3a2062664f3992861449b5c`  
		Size: 101.3 MB (101340157 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f8d27bfefcaaa84a89f93945c61ccf0af9ad50b1405d9acfa30e9da5ba1fb2db`  
		Last Modified: Wed, 14 Apr 2021 16:10:39 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6f599ec3e67dbcacd5ebae06ae984f5a688eba397e2280187ee399da88dc6ad`  
		Last Modified: Wed, 14 Apr 2021 16:10:38 GMT  
		Size: 4.3 MB (4262107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:780b42108cdc95774ec8d8239a9027e7382a875cf25306df1b01363dd2dc7aa4`  
		Last Modified: Wed, 14 Apr 2021 16:10:37 GMT  
		Size: 1.8 KB (1758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b002edb80987b79bb224f75e7c65e924d45dc54e548ce835539ca82dcdcc08e6`  
		Last Modified: Wed, 14 Apr 2021 16:10:37 GMT  
		Size: 1.2 KB (1176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c148b88ce7ff0e645ebee08b98beb32730028b41f85296f22b03154fa54614ac`  
		Last Modified: Wed, 14 Apr 2021 16:10:37 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43dc978ed7937ca238d82c78779b6e3a605e64ba31e2a5adac73bc7da1f63ede`  
		Last Modified: Wed, 14 Apr 2021 16:10:37 GMT  
		Size: 1.1 KB (1149 bytes)  
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
$ docker pull nats@sha256:236c67f0c205b9cfab2809ce1dea44a20258d371c82264afd3172f29c8c70fb1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1879; amd64

### `nats:nanoserver` - windows version 10.0.17763.1879; amd64

```console
$ docker pull nats@sha256:545e15088a9a48d35878789abdde98cb7a98627e5a7c3be56f42abb2e13632e8
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.6 MB (105608630 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19ac61d30cc1900a1011f83ffa5dbcfd15a0a1754f790b94bdded5ed0cd4b673`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 08 Apr 2021 16:02:06 GMT
RUN Apply image 1809-amd64
# Wed, 14 Apr 2021 16:05:18 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 14 Apr 2021 16:05:20 GMT
RUN cmd /S /C #(nop) COPY file:428a7e80db4313301a46326a9a79832e9cbe7d78c94e749b5c295e813e484f21 in C:\nats-server.exe 
# Wed, 14 Apr 2021 16:05:21 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 14 Apr 2021 16:05:22 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 14 Apr 2021 16:05:22 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 14 Apr 2021 16:05:23 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:ea84579f6cd5b58fe78732be37450bd188c8923de3a2062664f3992861449b5c`  
		Size: 101.3 MB (101340157 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f8d27bfefcaaa84a89f93945c61ccf0af9ad50b1405d9acfa30e9da5ba1fb2db`  
		Last Modified: Wed, 14 Apr 2021 16:10:39 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6f599ec3e67dbcacd5ebae06ae984f5a688eba397e2280187ee399da88dc6ad`  
		Last Modified: Wed, 14 Apr 2021 16:10:38 GMT  
		Size: 4.3 MB (4262107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:780b42108cdc95774ec8d8239a9027e7382a875cf25306df1b01363dd2dc7aa4`  
		Last Modified: Wed, 14 Apr 2021 16:10:37 GMT  
		Size: 1.8 KB (1758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b002edb80987b79bb224f75e7c65e924d45dc54e548ce835539ca82dcdcc08e6`  
		Last Modified: Wed, 14 Apr 2021 16:10:37 GMT  
		Size: 1.2 KB (1176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c148b88ce7ff0e645ebee08b98beb32730028b41f85296f22b03154fa54614ac`  
		Last Modified: Wed, 14 Apr 2021 16:10:37 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43dc978ed7937ca238d82c78779b6e3a605e64ba31e2a5adac73bc7da1f63ede`  
		Last Modified: Wed, 14 Apr 2021 16:10:37 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:nanoserver-1809`

```console
$ docker pull nats@sha256:236c67f0c205b9cfab2809ce1dea44a20258d371c82264afd3172f29c8c70fb1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1879; amd64

### `nats:nanoserver-1809` - windows version 10.0.17763.1879; amd64

```console
$ docker pull nats@sha256:545e15088a9a48d35878789abdde98cb7a98627e5a7c3be56f42abb2e13632e8
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.6 MB (105608630 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19ac61d30cc1900a1011f83ffa5dbcfd15a0a1754f790b94bdded5ed0cd4b673`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 08 Apr 2021 16:02:06 GMT
RUN Apply image 1809-amd64
# Wed, 14 Apr 2021 16:05:18 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 14 Apr 2021 16:05:20 GMT
RUN cmd /S /C #(nop) COPY file:428a7e80db4313301a46326a9a79832e9cbe7d78c94e749b5c295e813e484f21 in C:\nats-server.exe 
# Wed, 14 Apr 2021 16:05:21 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 14 Apr 2021 16:05:22 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 14 Apr 2021 16:05:22 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 14 Apr 2021 16:05:23 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:ea84579f6cd5b58fe78732be37450bd188c8923de3a2062664f3992861449b5c`  
		Size: 101.3 MB (101340157 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f8d27bfefcaaa84a89f93945c61ccf0af9ad50b1405d9acfa30e9da5ba1fb2db`  
		Last Modified: Wed, 14 Apr 2021 16:10:39 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6f599ec3e67dbcacd5ebae06ae984f5a688eba397e2280187ee399da88dc6ad`  
		Last Modified: Wed, 14 Apr 2021 16:10:38 GMT  
		Size: 4.3 MB (4262107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:780b42108cdc95774ec8d8239a9027e7382a875cf25306df1b01363dd2dc7aa4`  
		Last Modified: Wed, 14 Apr 2021 16:10:37 GMT  
		Size: 1.8 KB (1758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b002edb80987b79bb224f75e7c65e924d45dc54e548ce835539ca82dcdcc08e6`  
		Last Modified: Wed, 14 Apr 2021 16:10:37 GMT  
		Size: 1.2 KB (1176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c148b88ce7ff0e645ebee08b98beb32730028b41f85296f22b03154fa54614ac`  
		Last Modified: Wed, 14 Apr 2021 16:10:37 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43dc978ed7937ca238d82c78779b6e3a605e64ba31e2a5adac73bc7da1f63ede`  
		Last Modified: Wed, 14 Apr 2021 16:10:37 GMT  
		Size: 1.1 KB (1149 bytes)  
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
$ docker pull nats@sha256:a6c1153fd919a539581471edd798478057cef10a6347e770d03336a20d5e472b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1879; amd64
	-	windows version 10.0.14393.4350; amd64

### `nats:windowsservercore` - windows version 10.0.17763.1879; amd64

```console
$ docker pull nats@sha256:9f3868f133ddd1a10ac71bbe835764e9d60e9b00081851a00ca05cd3362ea5d1
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2484142070 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2be425426bfa101eb4fdc6741eccbeaddde31c6c0761a665b4654dea39a17279`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 09 Apr 2021 20:34:41 GMT
RUN Install update 1809-amd64
# Wed, 14 Apr 2021 13:10:28 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 14 Apr 2021 16:02:50 GMT
ENV NATS_DOCKERIZED=1
# Wed, 14 Apr 2021 16:02:51 GMT
ENV NATS_SERVER=2.2.1
# Wed, 14 Apr 2021 16:02:52 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.2.1/nats-server-v2.2.1-windows-amd64.zip
# Wed, 14 Apr 2021 16:02:53 GMT
ENV GIT_DOWNLOAD_SHA256=1f0d48a7ba9200e2572016a9f3e1ec7e630f0518cc0b40950c14ff3a5d900924
# Wed, 14 Apr 2021 16:03:32 GMT
RUN Set-PSDebug -Trace 2
# Wed, 14 Apr 2021 16:04:53 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 14 Apr 2021 16:04:55 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 14 Apr 2021 16:04:56 GMT
EXPOSE 4222 6222 8222
# Wed, 14 Apr 2021 16:04:57 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 14 Apr 2021 16:04:58 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:399f118dfaa9a753e98d128238b944432c7bcabea88a2998a6efbbece28ed303`  
		Size: 751.4 MB (751421005 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b2159a5d0f75ce11e6fe71e4260ede5c3c88a9eb76a0ff43ac6746b2b9b96775`  
		Last Modified: Wed, 14 Apr 2021 15:37:10 GMT  
		Size: 1.4 KB (1446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e849354f21f856ec720d6daecc37978fd7246f376ba3c32fd63d4400cce357bc`  
		Last Modified: Wed, 14 Apr 2021 16:10:16 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daae5ee02f484d7c054ad550cbee6900a35477f4e23e322cc3af6eb7c4690416`  
		Last Modified: Wed, 14 Apr 2021 16:10:14 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d4df8575d5fc511a7ac278cfc55a4053b36afce4c0bcae2af0af7907c7f91e6`  
		Last Modified: Wed, 14 Apr 2021 16:10:14 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:570a7e5edba00d92281a4a147639b5fc0b6724693cbfed80007b5b5db612a3e8`  
		Last Modified: Wed, 14 Apr 2021 16:10:13 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60092b7b0679ad17236eb09b832adcc7bb67a5fd8c2d9a69ffbfc863716274c2`  
		Last Modified: Wed, 14 Apr 2021 16:10:15 GMT  
		Size: 5.1 MB (5072726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d5d3b99689d155ccd6cdf6acbc7ef61472c65ce2cee49f441c4c3b844242410`  
		Last Modified: Wed, 14 Apr 2021 16:10:13 GMT  
		Size: 9.3 MB (9302175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23dae780c7132cf39c97d1602e11b6a58481594df6d896054f3a9e6e9f54e63a`  
		Last Modified: Wed, 14 Apr 2021 16:10:10 GMT  
		Size: 2.0 KB (1957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95f2291e14ae4d6e97942f3284122a80c7c969cb9bcfc9a417a833439505f85d`  
		Last Modified: Wed, 14 Apr 2021 16:10:11 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69b07be56d63a82b0606023df13bf32a522a13a12a44c53116ec24d0c1bd2ca1`  
		Last Modified: Wed, 14 Apr 2021 16:10:11 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb6cc0327d5edba60d3e99a97fa6c015e1953c9451bc816f20d6d73a67b9e426`  
		Last Modified: Wed, 14 Apr 2021 16:10:11 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:windowsservercore` - windows version 10.0.14393.4350; amd64

```console
$ docker pull nats@sha256:ad5ac25aa423d2df82324037dd73fec641098cd5f198cf98ccf19f4ae640d1f5
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5814950471 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0fc9b58b0a6e7d867ee74a6023bf1768d2dad684760ace428c0bf425357fcc5c`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 07 Apr 2021 21:54:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 14 Apr 2021 13:22:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 14 Apr 2021 16:05:33 GMT
ENV NATS_DOCKERIZED=1
# Wed, 14 Apr 2021 16:05:33 GMT
ENV NATS_SERVER=2.2.1
# Wed, 14 Apr 2021 16:05:35 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.2.1/nats-server-v2.2.1-windows-amd64.zip
# Wed, 14 Apr 2021 16:05:35 GMT
ENV GIT_DOWNLOAD_SHA256=1f0d48a7ba9200e2572016a9f3e1ec7e630f0518cc0b40950c14ff3a5d900924
# Wed, 14 Apr 2021 16:06:59 GMT
RUN Set-PSDebug -Trace 2
# Wed, 14 Apr 2021 16:09:18 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 14 Apr 2021 16:09:19 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 14 Apr 2021 16:09:20 GMT
EXPOSE 4222 6222 8222
# Wed, 14 Apr 2021 16:09:21 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 14 Apr 2021 16:09:23 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:00b4edb823e6a375d179a28cbfa682c2379d62179e1518485902d6e68b9a9d1e`  
		Size: 1.7 GB (1724897968 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f616bb7876e6f944d82fa1802ffab5ca4931a63e1b999f0851b52120cda83539`  
		Last Modified: Wed, 14 Apr 2021 15:37:43 GMT  
		Size: 1.3 KB (1307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcfa54f43457753c391f21da5e9a5bf47c61c574c0da04b8614d0e84bf823f54`  
		Last Modified: Wed, 14 Apr 2021 16:11:03 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04d71ba1c574073f9d5dd016585c2fe26ac560c192f7aa36ce54d4c12832997f`  
		Last Modified: Wed, 14 Apr 2021 16:11:01 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e9f66539738348100cf9f1e6a5bc40e8c2123bafb9329f5df3cf20a2015db33`  
		Last Modified: Wed, 14 Apr 2021 16:11:00 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20f2eae922462b2537c1d0d32d548cb10190f6bda0d02da57440cc229da692b3`  
		Last Modified: Wed, 14 Apr 2021 16:11:00 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ea168f84532f340be87f19704511ee160cbdc5b9c6ad8962fcd80e9fb8efea7`  
		Last Modified: Wed, 14 Apr 2021 16:11:01 GMT  
		Size: 5.7 MB (5651953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2eda2d9556eb5afaf10e6300ac36ddc1383144ae65671ca3a01b24bac150c540`  
		Last Modified: Wed, 14 Apr 2021 16:11:01 GMT  
		Size: 14.4 MB (14401439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a04b0d9d602bb1f9c6fb7925bb92959ebcff2c30e6ca6a658cdd9976d662d70`  
		Last Modified: Wed, 14 Apr 2021 16:10:57 GMT  
		Size: 2.0 KB (1984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e5e865356a464c9006414a165a6d0ffb8f062fa737be2ad42e1aa58fcfca23c`  
		Last Modified: Wed, 14 Apr 2021 16:10:56 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3533148ddde03cc5f28669b26c30dee8685db418d250a4b4829e465c0be8a7e`  
		Last Modified: Wed, 14 Apr 2021 16:10:56 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4573099491ec9887bd66033f55b39f6b897d1f59f21f679fdff4f822ebd7ea15`  
		Last Modified: Wed, 14 Apr 2021 16:10:56 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:windowsservercore-1809`

```console
$ docker pull nats@sha256:3002e35b4bb91080eac08408891e6bb9155d38086cbb6fcfb654b61e0d2383e0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1879; amd64

### `nats:windowsservercore-1809` - windows version 10.0.17763.1879; amd64

```console
$ docker pull nats@sha256:9f3868f133ddd1a10ac71bbe835764e9d60e9b00081851a00ca05cd3362ea5d1
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2484142070 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2be425426bfa101eb4fdc6741eccbeaddde31c6c0761a665b4654dea39a17279`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 09 Apr 2021 20:34:41 GMT
RUN Install update 1809-amd64
# Wed, 14 Apr 2021 13:10:28 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 14 Apr 2021 16:02:50 GMT
ENV NATS_DOCKERIZED=1
# Wed, 14 Apr 2021 16:02:51 GMT
ENV NATS_SERVER=2.2.1
# Wed, 14 Apr 2021 16:02:52 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.2.1/nats-server-v2.2.1-windows-amd64.zip
# Wed, 14 Apr 2021 16:02:53 GMT
ENV GIT_DOWNLOAD_SHA256=1f0d48a7ba9200e2572016a9f3e1ec7e630f0518cc0b40950c14ff3a5d900924
# Wed, 14 Apr 2021 16:03:32 GMT
RUN Set-PSDebug -Trace 2
# Wed, 14 Apr 2021 16:04:53 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 14 Apr 2021 16:04:55 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 14 Apr 2021 16:04:56 GMT
EXPOSE 4222 6222 8222
# Wed, 14 Apr 2021 16:04:57 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 14 Apr 2021 16:04:58 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:399f118dfaa9a753e98d128238b944432c7bcabea88a2998a6efbbece28ed303`  
		Size: 751.4 MB (751421005 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b2159a5d0f75ce11e6fe71e4260ede5c3c88a9eb76a0ff43ac6746b2b9b96775`  
		Last Modified: Wed, 14 Apr 2021 15:37:10 GMT  
		Size: 1.4 KB (1446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e849354f21f856ec720d6daecc37978fd7246f376ba3c32fd63d4400cce357bc`  
		Last Modified: Wed, 14 Apr 2021 16:10:16 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daae5ee02f484d7c054ad550cbee6900a35477f4e23e322cc3af6eb7c4690416`  
		Last Modified: Wed, 14 Apr 2021 16:10:14 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d4df8575d5fc511a7ac278cfc55a4053b36afce4c0bcae2af0af7907c7f91e6`  
		Last Modified: Wed, 14 Apr 2021 16:10:14 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:570a7e5edba00d92281a4a147639b5fc0b6724693cbfed80007b5b5db612a3e8`  
		Last Modified: Wed, 14 Apr 2021 16:10:13 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60092b7b0679ad17236eb09b832adcc7bb67a5fd8c2d9a69ffbfc863716274c2`  
		Last Modified: Wed, 14 Apr 2021 16:10:15 GMT  
		Size: 5.1 MB (5072726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d5d3b99689d155ccd6cdf6acbc7ef61472c65ce2cee49f441c4c3b844242410`  
		Last Modified: Wed, 14 Apr 2021 16:10:13 GMT  
		Size: 9.3 MB (9302175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23dae780c7132cf39c97d1602e11b6a58481594df6d896054f3a9e6e9f54e63a`  
		Last Modified: Wed, 14 Apr 2021 16:10:10 GMT  
		Size: 2.0 KB (1957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95f2291e14ae4d6e97942f3284122a80c7c969cb9bcfc9a417a833439505f85d`  
		Last Modified: Wed, 14 Apr 2021 16:10:11 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69b07be56d63a82b0606023df13bf32a522a13a12a44c53116ec24d0c1bd2ca1`  
		Last Modified: Wed, 14 Apr 2021 16:10:11 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb6cc0327d5edba60d3e99a97fa6c015e1953c9451bc816f20d6d73a67b9e426`  
		Last Modified: Wed, 14 Apr 2021 16:10:11 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:windowsservercore-ltsc2016`

```console
$ docker pull nats@sha256:486439b61d7c8307b15b01bae5f574784e333ee642d1d3285e3bf61785ea00cd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4350; amd64

### `nats:windowsservercore-ltsc2016` - windows version 10.0.14393.4350; amd64

```console
$ docker pull nats@sha256:ad5ac25aa423d2df82324037dd73fec641098cd5f198cf98ccf19f4ae640d1f5
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5814950471 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0fc9b58b0a6e7d867ee74a6023bf1768d2dad684760ace428c0bf425357fcc5c`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 07 Apr 2021 21:54:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 14 Apr 2021 13:22:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 14 Apr 2021 16:05:33 GMT
ENV NATS_DOCKERIZED=1
# Wed, 14 Apr 2021 16:05:33 GMT
ENV NATS_SERVER=2.2.1
# Wed, 14 Apr 2021 16:05:35 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.2.1/nats-server-v2.2.1-windows-amd64.zip
# Wed, 14 Apr 2021 16:05:35 GMT
ENV GIT_DOWNLOAD_SHA256=1f0d48a7ba9200e2572016a9f3e1ec7e630f0518cc0b40950c14ff3a5d900924
# Wed, 14 Apr 2021 16:06:59 GMT
RUN Set-PSDebug -Trace 2
# Wed, 14 Apr 2021 16:09:18 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 14 Apr 2021 16:09:19 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 14 Apr 2021 16:09:20 GMT
EXPOSE 4222 6222 8222
# Wed, 14 Apr 2021 16:09:21 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 14 Apr 2021 16:09:23 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:00b4edb823e6a375d179a28cbfa682c2379d62179e1518485902d6e68b9a9d1e`  
		Size: 1.7 GB (1724897968 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f616bb7876e6f944d82fa1802ffab5ca4931a63e1b999f0851b52120cda83539`  
		Last Modified: Wed, 14 Apr 2021 15:37:43 GMT  
		Size: 1.3 KB (1307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcfa54f43457753c391f21da5e9a5bf47c61c574c0da04b8614d0e84bf823f54`  
		Last Modified: Wed, 14 Apr 2021 16:11:03 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04d71ba1c574073f9d5dd016585c2fe26ac560c192f7aa36ce54d4c12832997f`  
		Last Modified: Wed, 14 Apr 2021 16:11:01 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e9f66539738348100cf9f1e6a5bc40e8c2123bafb9329f5df3cf20a2015db33`  
		Last Modified: Wed, 14 Apr 2021 16:11:00 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20f2eae922462b2537c1d0d32d548cb10190f6bda0d02da57440cc229da692b3`  
		Last Modified: Wed, 14 Apr 2021 16:11:00 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ea168f84532f340be87f19704511ee160cbdc5b9c6ad8962fcd80e9fb8efea7`  
		Last Modified: Wed, 14 Apr 2021 16:11:01 GMT  
		Size: 5.7 MB (5651953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2eda2d9556eb5afaf10e6300ac36ddc1383144ae65671ca3a01b24bac150c540`  
		Last Modified: Wed, 14 Apr 2021 16:11:01 GMT  
		Size: 14.4 MB (14401439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a04b0d9d602bb1f9c6fb7925bb92959ebcff2c30e6ca6a658cdd9976d662d70`  
		Last Modified: Wed, 14 Apr 2021 16:10:57 GMT  
		Size: 2.0 KB (1984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e5e865356a464c9006414a165a6d0ffb8f062fa737be2ad42e1aa58fcfca23c`  
		Last Modified: Wed, 14 Apr 2021 16:10:56 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3533148ddde03cc5f28669b26c30dee8685db418d250a4b4829e465c0be8a7e`  
		Last Modified: Wed, 14 Apr 2021 16:10:56 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4573099491ec9887bd66033f55b39f6b897d1f59f21f679fdff4f822ebd7ea15`  
		Last Modified: Wed, 14 Apr 2021 16:10:56 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
