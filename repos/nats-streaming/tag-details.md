<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `nats-streaming`

-	[`nats-streaming:0.21`](#nats-streaming021)
-	[`nats-streaming:0.21-alpine`](#nats-streaming021-alpine)
-	[`nats-streaming:0.21-alpine3.13`](#nats-streaming021-alpine313)
-	[`nats-streaming:0.21-linux`](#nats-streaming021-linux)
-	[`nats-streaming:0.21-nanoserver`](#nats-streaming021-nanoserver)
-	[`nats-streaming:0.21-nanoserver-1809`](#nats-streaming021-nanoserver-1809)
-	[`nats-streaming:0.21-scratch`](#nats-streaming021-scratch)
-	[`nats-streaming:0.21-windowsservercore`](#nats-streaming021-windowsservercore)
-	[`nats-streaming:0.21-windowsservercore-1809`](#nats-streaming021-windowsservercore-1809)
-	[`nats-streaming:0.21-windowsservercore-ltsc2016`](#nats-streaming021-windowsservercore-ltsc2016)
-	[`nats-streaming:0.21.1`](#nats-streaming0211)
-	[`nats-streaming:0.21.1-alpine`](#nats-streaming0211-alpine)
-	[`nats-streaming:0.21.1-alpine3.13`](#nats-streaming0211-alpine313)
-	[`nats-streaming:0.21.1-linux`](#nats-streaming0211-linux)
-	[`nats-streaming:0.21.1-nanoserver`](#nats-streaming0211-nanoserver)
-	[`nats-streaming:0.21.1-nanoserver-1809`](#nats-streaming0211-nanoserver-1809)
-	[`nats-streaming:0.21.1-scratch`](#nats-streaming0211-scratch)
-	[`nats-streaming:0.21.1-windowsservercore`](#nats-streaming0211-windowsservercore)
-	[`nats-streaming:0.21.1-windowsservercore-1809`](#nats-streaming0211-windowsservercore-1809)
-	[`nats-streaming:0.21.1-windowsservercore-ltsc2016`](#nats-streaming0211-windowsservercore-ltsc2016)
-	[`nats-streaming:alpine`](#nats-streamingalpine)
-	[`nats-streaming:alpine3.13`](#nats-streamingalpine313)
-	[`nats-streaming:latest`](#nats-streaminglatest)
-	[`nats-streaming:linux`](#nats-streaminglinux)
-	[`nats-streaming:nanoserver`](#nats-streamingnanoserver)
-	[`nats-streaming:nanoserver-1809`](#nats-streamingnanoserver-1809)
-	[`nats-streaming:scratch`](#nats-streamingscratch)
-	[`nats-streaming:windowsservercore`](#nats-streamingwindowsservercore)
-	[`nats-streaming:windowsservercore-1809`](#nats-streamingwindowsservercore-1809)
-	[`nats-streaming:windowsservercore-ltsc2016`](#nats-streamingwindowsservercore-ltsc2016)

## `nats-streaming:0.21`

```console
$ docker pull nats-streaming@sha256:42dd817d3798a2288a0dfbd2a8f520b497ff170316f38a13c4d09f2be70f4e99
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.1817; amd64

### `nats-streaming:0.21` - linux; amd64

```console
$ docker pull nats-streaming@sha256:aa6af76760541ce71d366ac25554ad7caa95aea8cd230dd2688fd76b0645b329
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.7 MB (5680474 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31671965fc8e3e2d623279516e43fd9d1a5d8d82a19fe709c69d7bfe7ac50085`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Sat, 06 Mar 2021 07:43:28 GMT
COPY file:2c21a07cd43acfd157f86c6cf727430cf07e201a3bf3668b2083f473385db991 in /nats-streaming-server 
# Sat, 06 Mar 2021 07:43:28 GMT
EXPOSE 4222 8222
# Sat, 06 Mar 2021 07:43:29 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Sat, 06 Mar 2021 07:43:29 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:6f1c3ed40f752c2108b0e5d9224fba83d5045dac3370f93a50d91af0bc201c05`  
		Last Modified: Sat, 06 Mar 2021 07:44:17 GMT  
		Size: 5.7 MB (5680474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.21` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:907a450228b0d46339c5af803a9475165f7cfd9d20d5e09e8f66f9d048d1f7b9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.3 MB (5252895 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8c6d73cc983f6821e57de28a32cec901f28d3c5ada68aa9e71a1880962a9f07`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Sat, 06 Mar 2021 02:10:29 GMT
COPY file:bd617234b457ddee67b99f0e411029c6d5badad5059fbd81239c0acfe92cd4b7 in /nats-streaming-server 
# Sat, 06 Mar 2021 02:10:30 GMT
EXPOSE 4222 8222
# Sat, 06 Mar 2021 02:10:31 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Sat, 06 Mar 2021 02:10:31 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:ef1f32aa7a9ce9c8d42c909d32f61dabfa957c0b6a2b3590cd5e5847fb634355`  
		Last Modified: Sat, 06 Mar 2021 02:11:15 GMT  
		Size: 5.3 MB (5252895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.21` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:ae774aee41bd64306207d739d2290639f673c9c66c367a83f155a923fe8c13f6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5246286 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ce52186dd957f6b70b086fdcbc8212e079e5ed5e3e0013f8f72b3922535a56e`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Sat, 06 Mar 2021 01:00:25 GMT
COPY file:546c18b3e8e91d453d1a325c6e4dbc3c945564c010676da1abe89a653a0dea84 in /nats-streaming-server 
# Sat, 06 Mar 2021 01:00:27 GMT
EXPOSE 4222 8222
# Sat, 06 Mar 2021 01:00:28 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Sat, 06 Mar 2021 01:00:29 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:ed8ed2aa5d978cf51ebe3454de1832aeb40919052c5cb17d5b63865c31fc03c7`  
		Last Modified: Sat, 06 Mar 2021 01:01:07 GMT  
		Size: 5.2 MB (5246286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.21` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:7fccb492771f9c26f12f03c49e84ba4fb4d7004c6d142f4a7b83337d92feda95
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5170586 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07e817dd7b95371ae514afe3154e4aeba302d94dbed618a0aba7ece8696c13c6`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Sat, 06 Mar 2021 01:51:04 GMT
COPY file:ed938be8d92952afe74223a94317bf582d9bcf2c458a54733da01a37a65d421b in /nats-streaming-server 
# Sat, 06 Mar 2021 01:51:05 GMT
EXPOSE 4222 8222
# Sat, 06 Mar 2021 01:51:06 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Sat, 06 Mar 2021 01:51:07 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:f5ab53e298c8bd7b93e991f4b12e4015cde7d604e6d5ee086e994a86e0556094`  
		Last Modified: Sat, 06 Mar 2021 01:51:46 GMT  
		Size: 5.2 MB (5170586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.21` - windows version 10.0.17763.1817; amd64

```console
$ docker pull nats-streaming@sha256:b1027771e781ed856534f3ee9d9fc845e0a08d4ac903949056fa3613a1025713
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.2 MB (107205225 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:034c288a390667cc8689271b4c68b1f38eb2887a9931320f9fea3cd6cdb28dfb`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Fri, 26 Feb 2021 16:47:31 GMT
RUN Apply image 1809-amd64
# Wed, 10 Mar 2021 16:56:55 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 10 Mar 2021 21:49:39 GMT
RUN cmd /S /C #(nop) COPY file:189ca6af047e9f9cf54ab2176b48588e01c7497fe0b5b0d7b2614ebad66ed089 in C:\nats-streaming-server.exe 
# Wed, 10 Mar 2021 21:49:40 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 10 Mar 2021 21:49:41 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 10 Mar 2021 21:49:42 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:a11c4ca8f1ba16b6e1395d4523be2215bd0871c2e3e4695b9f2b87bd7472be52`  
		Size: 101.4 MB (101389964 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f49969195f32b7e40a81e3d189259fec7ebf52ee0ec5dafd5f3f288715354fed`  
		Last Modified: Wed, 10 Mar 2021 17:01:57 GMT  
		Size: 1.0 KB (1047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d5345eab816862154342d0ef80781aae11144d15f84ad4ac1d5ed1bbf9b083e`  
		Last Modified: Wed, 10 Mar 2021 21:54:51 GMT  
		Size: 5.8 MB (5810691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d886b78bda0fe938d4c7e8a21e511102e719280871d97e9e7b3d4589222dffd`  
		Last Modified: Wed, 10 Mar 2021 21:54:51 GMT  
		Size: 1.2 KB (1180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3fce35e6d75d0e8ea6539c3a0e1f335dec61dfabde67c34ec07260f715ea526`  
		Last Modified: Wed, 10 Mar 2021 21:54:50 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b95ed8adcfdc36bcc766c7ca9db14a0bca9768321cc35854aa2d896ef75ea4ab`  
		Last Modified: Wed, 10 Mar 2021 21:54:49 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.21-alpine`

```console
$ docker pull nats-streaming@sha256:1941dba2b56c072871d4ce1aecc9b9ec0f9ac9776e8c59aaf6252b6d180fbf59
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.21-alpine` - linux; amd64

```console
$ docker pull nats-streaming@sha256:701fa3e7165e338d3fb61b4f7068af826829b094fc089e1b7866466bc4cba85e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.8 MB (8774552 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3593598c050f5241766331b8aed01f6c3f42b71938fc11f47bbfa18d74c829be`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 17 Feb 2021 21:19:54 GMT
ADD file:80bf8bd014071345b1c0364eeb0a5e48f3fb0d87f9c31cb990e57caa652b59b8 in / 
# Wed, 17 Feb 2021 21:19:54 GMT
CMD ["/bin/sh"]
# Sat, 06 Mar 2021 07:43:18 GMT
ENV NATS_STREAMING_SERVER=0.21.1
# Sat, 06 Mar 2021 07:43:22 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='06d591a61084aab1046e818486c2ee7c3936214c92dc257084693d6ffe06342b' ;; 		armhf) natsArch='arm6'; sha256='085375782abe1bacbd6fc609ce6a6721f029cba312733479204c89bf92f1e188' ;; 		armv7) natsArch='arm7'; sha256='947d91512b47ba98198bef7f799670c40cf6949f2ba2e98b5c133e6166e9b97c' ;; 		x86_64) natsArch='amd64'; sha256='85fd7fd3c7b71cbc9043900f9110b028f1fdc042c6500eed065e6e2c3331f62e' ;; 		x86) natsArch='386'; sha256='475b0f015726af99c9ea779c8bbbeaa729ef90f43dd2715273fea81fb90ea63a' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Sat, 06 Mar 2021 07:43:22 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Sat, 06 Mar 2021 07:43:22 GMT
EXPOSE 4222 8222
# Sat, 06 Mar 2021 07:43:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 06 Mar 2021 07:43:23 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:ba3557a56b150f9b813f9d02274d62914fd8fce120dd374d9ee17b87cf1d277d`  
		Last Modified: Wed, 17 Feb 2021 21:20:25 GMT  
		Size: 2.8 MB (2811657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ae3e2d2b3e48427fd1213fbc4722666443f13ca1a6709825a2afbbf6381367d`  
		Last Modified: Sat, 06 Mar 2021 07:43:55 GMT  
		Size: 6.0 MB (5962472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19a250278b77e3fdc0d10076a12c9d14803a891ccfb31290836d192e35da8a03`  
		Last Modified: Sat, 06 Mar 2021 07:43:54 GMT  
		Size: 423.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.21-alpine` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:19373a83f61771319d0aacfab1086d496a2dd1535970f8a20652d56cf2b7578e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.2 MB (8156412 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:935ff18ff1bfcc7d421f422b0d98ef2b111e05c4e09b1e57aef68d71b18156b9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Thu, 25 Mar 2021 22:50:09 GMT
ADD file:ca4136238cb9a01d079efd129bccd1470945d7d4320da61373af90645a4b1146 in / 
# Thu, 25 Mar 2021 22:50:28 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 05:57:34 GMT
ENV NATS_STREAMING_SERVER=0.21.1
# Fri, 26 Mar 2021 05:57:41 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='06d591a61084aab1046e818486c2ee7c3936214c92dc257084693d6ffe06342b' ;; 		armhf) natsArch='arm6'; sha256='085375782abe1bacbd6fc609ce6a6721f029cba312733479204c89bf92f1e188' ;; 		armv7) natsArch='arm7'; sha256='947d91512b47ba98198bef7f799670c40cf6949f2ba2e98b5c133e6166e9b97c' ;; 		x86_64) natsArch='amd64'; sha256='85fd7fd3c7b71cbc9043900f9110b028f1fdc042c6500eed065e6e2c3331f62e' ;; 		x86) natsArch='386'; sha256='475b0f015726af99c9ea779c8bbbeaa729ef90f43dd2715273fea81fb90ea63a' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 26 Mar 2021 05:57:42 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Fri, 26 Mar 2021 05:57:43 GMT
EXPOSE 4222 8222
# Fri, 26 Mar 2021 05:57:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 05:57:46 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:bca6a70a54896d072b6919d2ae18d3ef685bc7aed783731f68a4adac0fb93d52`  
		Last Modified: Thu, 25 Mar 2021 22:54:24 GMT  
		Size: 2.6 MB (2622062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37dde547b7fced1153630086dee787892a218966ea430c2964f55f72bcbbf83a`  
		Last Modified: Fri, 26 Mar 2021 05:58:16 GMT  
		Size: 5.5 MB (5533929 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df980303a7fb93b8683964b371b30ef03ef35e26de48621d858290228f8b3346`  
		Last Modified: Fri, 26 Mar 2021 05:58:14 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.21-alpine` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:f167b7ef1b6e893d3e176ad7fd41597e8a4da3720d0694b407e19e24b68cd5f6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.0 MB (7951584 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e033b7fa5e49122eff8379884102467952cb9d40190588eee42fd608ecbfe3d9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Thu, 25 Mar 2021 22:05:53 GMT
ADD file:44ef6cff6e7d37a67c5846eb792fec65025702c00c56ff96801ac79bf81b0cc3 in / 
# Thu, 25 Mar 2021 22:05:55 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 01:51:55 GMT
ENV NATS_STREAMING_SERVER=0.21.1
# Fri, 26 Mar 2021 01:52:03 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='06d591a61084aab1046e818486c2ee7c3936214c92dc257084693d6ffe06342b' ;; 		armhf) natsArch='arm6'; sha256='085375782abe1bacbd6fc609ce6a6721f029cba312733479204c89bf92f1e188' ;; 		armv7) natsArch='arm7'; sha256='947d91512b47ba98198bef7f799670c40cf6949f2ba2e98b5c133e6166e9b97c' ;; 		x86_64) natsArch='amd64'; sha256='85fd7fd3c7b71cbc9043900f9110b028f1fdc042c6500eed065e6e2c3331f62e' ;; 		x86) natsArch='386'; sha256='475b0f015726af99c9ea779c8bbbeaa729ef90f43dd2715273fea81fb90ea63a' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 26 Mar 2021 01:52:05 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Fri, 26 Mar 2021 01:52:11 GMT
EXPOSE 4222 8222
# Fri, 26 Mar 2021 01:52:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 01:52:14 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:6c1162af251f0d5ab4945f8506f3265b86d0a03cda37f703c2446a71a233bc20`  
		Last Modified: Thu, 25 Mar 2021 22:07:21 GMT  
		Size: 2.4 MB (2423999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61ca624cfb490a8a9fb48110381475a59604ddfd4920f6496398a887f8a37b73`  
		Last Modified: Fri, 26 Mar 2021 01:52:52 GMT  
		Size: 5.5 MB (5527163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3957a11b701f02a3361d365cd9b9c63fcafa89f362a40471a527bb31bbbe1de6`  
		Last Modified: Fri, 26 Mar 2021 01:52:50 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.21-alpine` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:1740e224df015e33133a9db91519ebc8601bf64861cde979a2ed6c556b649395
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.2 MB (8164487 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:205e781a3be342b949194bab8b6fde3763da1876fe7fac88af8efa1a07b3f204`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 17 Feb 2021 20:39:29 GMT
ADD file:3bf1497bd250cf7c73c12231dc4ebe3a3a67f2cd99e35bce47ef6674683aeb1d in / 
# Wed, 17 Feb 2021 20:39:30 GMT
CMD ["/bin/sh"]
# Sat, 06 Mar 2021 01:46:28 GMT
ENV NATS_STREAMING_SERVER=0.21.1
# Sat, 06 Mar 2021 01:46:33 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='06d591a61084aab1046e818486c2ee7c3936214c92dc257084693d6ffe06342b' ;; 		armhf) natsArch='arm6'; sha256='085375782abe1bacbd6fc609ce6a6721f029cba312733479204c89bf92f1e188' ;; 		armv7) natsArch='arm7'; sha256='947d91512b47ba98198bef7f799670c40cf6949f2ba2e98b5c133e6166e9b97c' ;; 		x86_64) natsArch='amd64'; sha256='85fd7fd3c7b71cbc9043900f9110b028f1fdc042c6500eed065e6e2c3331f62e' ;; 		x86) natsArch='386'; sha256='475b0f015726af99c9ea779c8bbbeaa729ef90f43dd2715273fea81fb90ea63a' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Sat, 06 Mar 2021 01:46:33 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Sat, 06 Mar 2021 01:46:34 GMT
EXPOSE 4222 8222
# Sat, 06 Mar 2021 01:46:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 06 Mar 2021 01:46:35 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:069a56d6d07f6b186fbb82e4486616b9be9a37ce32a63013af6cddcb65898182`  
		Last Modified: Wed, 17 Feb 2021 20:40:04 GMT  
		Size: 2.7 MB (2711572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e334db32136252e9605e0a6ef0426e8c0c50e757bb238a24330339d3dedbe84`  
		Last Modified: Sat, 06 Mar 2021 01:51:34 GMT  
		Size: 5.5 MB (5452492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7e903d8d08305b07378aef2e8c19af9f0d6b899ce053c33e5b6022c07b155e2`  
		Last Modified: Sat, 06 Mar 2021 01:51:32 GMT  
		Size: 423.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.21-alpine3.13`

```console
$ docker pull nats-streaming@sha256:1941dba2b56c072871d4ce1aecc9b9ec0f9ac9776e8c59aaf6252b6d180fbf59
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.21-alpine3.13` - linux; amd64

```console
$ docker pull nats-streaming@sha256:701fa3e7165e338d3fb61b4f7068af826829b094fc089e1b7866466bc4cba85e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.8 MB (8774552 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3593598c050f5241766331b8aed01f6c3f42b71938fc11f47bbfa18d74c829be`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 17 Feb 2021 21:19:54 GMT
ADD file:80bf8bd014071345b1c0364eeb0a5e48f3fb0d87f9c31cb990e57caa652b59b8 in / 
# Wed, 17 Feb 2021 21:19:54 GMT
CMD ["/bin/sh"]
# Sat, 06 Mar 2021 07:43:18 GMT
ENV NATS_STREAMING_SERVER=0.21.1
# Sat, 06 Mar 2021 07:43:22 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='06d591a61084aab1046e818486c2ee7c3936214c92dc257084693d6ffe06342b' ;; 		armhf) natsArch='arm6'; sha256='085375782abe1bacbd6fc609ce6a6721f029cba312733479204c89bf92f1e188' ;; 		armv7) natsArch='arm7'; sha256='947d91512b47ba98198bef7f799670c40cf6949f2ba2e98b5c133e6166e9b97c' ;; 		x86_64) natsArch='amd64'; sha256='85fd7fd3c7b71cbc9043900f9110b028f1fdc042c6500eed065e6e2c3331f62e' ;; 		x86) natsArch='386'; sha256='475b0f015726af99c9ea779c8bbbeaa729ef90f43dd2715273fea81fb90ea63a' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Sat, 06 Mar 2021 07:43:22 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Sat, 06 Mar 2021 07:43:22 GMT
EXPOSE 4222 8222
# Sat, 06 Mar 2021 07:43:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 06 Mar 2021 07:43:23 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:ba3557a56b150f9b813f9d02274d62914fd8fce120dd374d9ee17b87cf1d277d`  
		Last Modified: Wed, 17 Feb 2021 21:20:25 GMT  
		Size: 2.8 MB (2811657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ae3e2d2b3e48427fd1213fbc4722666443f13ca1a6709825a2afbbf6381367d`  
		Last Modified: Sat, 06 Mar 2021 07:43:55 GMT  
		Size: 6.0 MB (5962472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19a250278b77e3fdc0d10076a12c9d14803a891ccfb31290836d192e35da8a03`  
		Last Modified: Sat, 06 Mar 2021 07:43:54 GMT  
		Size: 423.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.21-alpine3.13` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:19373a83f61771319d0aacfab1086d496a2dd1535970f8a20652d56cf2b7578e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.2 MB (8156412 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:935ff18ff1bfcc7d421f422b0d98ef2b111e05c4e09b1e57aef68d71b18156b9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Thu, 25 Mar 2021 22:50:09 GMT
ADD file:ca4136238cb9a01d079efd129bccd1470945d7d4320da61373af90645a4b1146 in / 
# Thu, 25 Mar 2021 22:50:28 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 05:57:34 GMT
ENV NATS_STREAMING_SERVER=0.21.1
# Fri, 26 Mar 2021 05:57:41 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='06d591a61084aab1046e818486c2ee7c3936214c92dc257084693d6ffe06342b' ;; 		armhf) natsArch='arm6'; sha256='085375782abe1bacbd6fc609ce6a6721f029cba312733479204c89bf92f1e188' ;; 		armv7) natsArch='arm7'; sha256='947d91512b47ba98198bef7f799670c40cf6949f2ba2e98b5c133e6166e9b97c' ;; 		x86_64) natsArch='amd64'; sha256='85fd7fd3c7b71cbc9043900f9110b028f1fdc042c6500eed065e6e2c3331f62e' ;; 		x86) natsArch='386'; sha256='475b0f015726af99c9ea779c8bbbeaa729ef90f43dd2715273fea81fb90ea63a' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 26 Mar 2021 05:57:42 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Fri, 26 Mar 2021 05:57:43 GMT
EXPOSE 4222 8222
# Fri, 26 Mar 2021 05:57:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 05:57:46 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:bca6a70a54896d072b6919d2ae18d3ef685bc7aed783731f68a4adac0fb93d52`  
		Last Modified: Thu, 25 Mar 2021 22:54:24 GMT  
		Size: 2.6 MB (2622062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37dde547b7fced1153630086dee787892a218966ea430c2964f55f72bcbbf83a`  
		Last Modified: Fri, 26 Mar 2021 05:58:16 GMT  
		Size: 5.5 MB (5533929 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df980303a7fb93b8683964b371b30ef03ef35e26de48621d858290228f8b3346`  
		Last Modified: Fri, 26 Mar 2021 05:58:14 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.21-alpine3.13` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:f167b7ef1b6e893d3e176ad7fd41597e8a4da3720d0694b407e19e24b68cd5f6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.0 MB (7951584 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e033b7fa5e49122eff8379884102467952cb9d40190588eee42fd608ecbfe3d9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Thu, 25 Mar 2021 22:05:53 GMT
ADD file:44ef6cff6e7d37a67c5846eb792fec65025702c00c56ff96801ac79bf81b0cc3 in / 
# Thu, 25 Mar 2021 22:05:55 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 01:51:55 GMT
ENV NATS_STREAMING_SERVER=0.21.1
# Fri, 26 Mar 2021 01:52:03 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='06d591a61084aab1046e818486c2ee7c3936214c92dc257084693d6ffe06342b' ;; 		armhf) natsArch='arm6'; sha256='085375782abe1bacbd6fc609ce6a6721f029cba312733479204c89bf92f1e188' ;; 		armv7) natsArch='arm7'; sha256='947d91512b47ba98198bef7f799670c40cf6949f2ba2e98b5c133e6166e9b97c' ;; 		x86_64) natsArch='amd64'; sha256='85fd7fd3c7b71cbc9043900f9110b028f1fdc042c6500eed065e6e2c3331f62e' ;; 		x86) natsArch='386'; sha256='475b0f015726af99c9ea779c8bbbeaa729ef90f43dd2715273fea81fb90ea63a' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 26 Mar 2021 01:52:05 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Fri, 26 Mar 2021 01:52:11 GMT
EXPOSE 4222 8222
# Fri, 26 Mar 2021 01:52:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 01:52:14 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:6c1162af251f0d5ab4945f8506f3265b86d0a03cda37f703c2446a71a233bc20`  
		Last Modified: Thu, 25 Mar 2021 22:07:21 GMT  
		Size: 2.4 MB (2423999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61ca624cfb490a8a9fb48110381475a59604ddfd4920f6496398a887f8a37b73`  
		Last Modified: Fri, 26 Mar 2021 01:52:52 GMT  
		Size: 5.5 MB (5527163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3957a11b701f02a3361d365cd9b9c63fcafa89f362a40471a527bb31bbbe1de6`  
		Last Modified: Fri, 26 Mar 2021 01:52:50 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.21-alpine3.13` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:1740e224df015e33133a9db91519ebc8601bf64861cde979a2ed6c556b649395
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.2 MB (8164487 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:205e781a3be342b949194bab8b6fde3763da1876fe7fac88af8efa1a07b3f204`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 17 Feb 2021 20:39:29 GMT
ADD file:3bf1497bd250cf7c73c12231dc4ebe3a3a67f2cd99e35bce47ef6674683aeb1d in / 
# Wed, 17 Feb 2021 20:39:30 GMT
CMD ["/bin/sh"]
# Sat, 06 Mar 2021 01:46:28 GMT
ENV NATS_STREAMING_SERVER=0.21.1
# Sat, 06 Mar 2021 01:46:33 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='06d591a61084aab1046e818486c2ee7c3936214c92dc257084693d6ffe06342b' ;; 		armhf) natsArch='arm6'; sha256='085375782abe1bacbd6fc609ce6a6721f029cba312733479204c89bf92f1e188' ;; 		armv7) natsArch='arm7'; sha256='947d91512b47ba98198bef7f799670c40cf6949f2ba2e98b5c133e6166e9b97c' ;; 		x86_64) natsArch='amd64'; sha256='85fd7fd3c7b71cbc9043900f9110b028f1fdc042c6500eed065e6e2c3331f62e' ;; 		x86) natsArch='386'; sha256='475b0f015726af99c9ea779c8bbbeaa729ef90f43dd2715273fea81fb90ea63a' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Sat, 06 Mar 2021 01:46:33 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Sat, 06 Mar 2021 01:46:34 GMT
EXPOSE 4222 8222
# Sat, 06 Mar 2021 01:46:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 06 Mar 2021 01:46:35 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:069a56d6d07f6b186fbb82e4486616b9be9a37ce32a63013af6cddcb65898182`  
		Last Modified: Wed, 17 Feb 2021 20:40:04 GMT  
		Size: 2.7 MB (2711572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e334db32136252e9605e0a6ef0426e8c0c50e757bb238a24330339d3dedbe84`  
		Last Modified: Sat, 06 Mar 2021 01:51:34 GMT  
		Size: 5.5 MB (5452492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7e903d8d08305b07378aef2e8c19af9f0d6b899ce053c33e5b6022c07b155e2`  
		Last Modified: Sat, 06 Mar 2021 01:51:32 GMT  
		Size: 423.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.21-linux`

```console
$ docker pull nats-streaming@sha256:26603f9112b727df8e9736407a1ec1ab031317a9f6964ba0d407baea6b8d152c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.21-linux` - linux; amd64

```console
$ docker pull nats-streaming@sha256:aa6af76760541ce71d366ac25554ad7caa95aea8cd230dd2688fd76b0645b329
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.7 MB (5680474 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31671965fc8e3e2d623279516e43fd9d1a5d8d82a19fe709c69d7bfe7ac50085`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Sat, 06 Mar 2021 07:43:28 GMT
COPY file:2c21a07cd43acfd157f86c6cf727430cf07e201a3bf3668b2083f473385db991 in /nats-streaming-server 
# Sat, 06 Mar 2021 07:43:28 GMT
EXPOSE 4222 8222
# Sat, 06 Mar 2021 07:43:29 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Sat, 06 Mar 2021 07:43:29 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:6f1c3ed40f752c2108b0e5d9224fba83d5045dac3370f93a50d91af0bc201c05`  
		Last Modified: Sat, 06 Mar 2021 07:44:17 GMT  
		Size: 5.7 MB (5680474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.21-linux` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:907a450228b0d46339c5af803a9475165f7cfd9d20d5e09e8f66f9d048d1f7b9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.3 MB (5252895 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8c6d73cc983f6821e57de28a32cec901f28d3c5ada68aa9e71a1880962a9f07`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Sat, 06 Mar 2021 02:10:29 GMT
COPY file:bd617234b457ddee67b99f0e411029c6d5badad5059fbd81239c0acfe92cd4b7 in /nats-streaming-server 
# Sat, 06 Mar 2021 02:10:30 GMT
EXPOSE 4222 8222
# Sat, 06 Mar 2021 02:10:31 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Sat, 06 Mar 2021 02:10:31 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:ef1f32aa7a9ce9c8d42c909d32f61dabfa957c0b6a2b3590cd5e5847fb634355`  
		Last Modified: Sat, 06 Mar 2021 02:11:15 GMT  
		Size: 5.3 MB (5252895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.21-linux` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:ae774aee41bd64306207d739d2290639f673c9c66c367a83f155a923fe8c13f6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5246286 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ce52186dd957f6b70b086fdcbc8212e079e5ed5e3e0013f8f72b3922535a56e`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Sat, 06 Mar 2021 01:00:25 GMT
COPY file:546c18b3e8e91d453d1a325c6e4dbc3c945564c010676da1abe89a653a0dea84 in /nats-streaming-server 
# Sat, 06 Mar 2021 01:00:27 GMT
EXPOSE 4222 8222
# Sat, 06 Mar 2021 01:00:28 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Sat, 06 Mar 2021 01:00:29 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:ed8ed2aa5d978cf51ebe3454de1832aeb40919052c5cb17d5b63865c31fc03c7`  
		Last Modified: Sat, 06 Mar 2021 01:01:07 GMT  
		Size: 5.2 MB (5246286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.21-linux` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:7fccb492771f9c26f12f03c49e84ba4fb4d7004c6d142f4a7b83337d92feda95
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5170586 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07e817dd7b95371ae514afe3154e4aeba302d94dbed618a0aba7ece8696c13c6`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Sat, 06 Mar 2021 01:51:04 GMT
COPY file:ed938be8d92952afe74223a94317bf582d9bcf2c458a54733da01a37a65d421b in /nats-streaming-server 
# Sat, 06 Mar 2021 01:51:05 GMT
EXPOSE 4222 8222
# Sat, 06 Mar 2021 01:51:06 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Sat, 06 Mar 2021 01:51:07 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:f5ab53e298c8bd7b93e991f4b12e4015cde7d604e6d5ee086e994a86e0556094`  
		Last Modified: Sat, 06 Mar 2021 01:51:46 GMT  
		Size: 5.2 MB (5170586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.21-nanoserver`

```console
$ docker pull nats-streaming@sha256:87d3bbcab917eb6d04e19e5623d88b465ff072b603fa498c4b7299035fbdf1e7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1817; amd64

### `nats-streaming:0.21-nanoserver` - windows version 10.0.17763.1817; amd64

```console
$ docker pull nats-streaming@sha256:b1027771e781ed856534f3ee9d9fc845e0a08d4ac903949056fa3613a1025713
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.2 MB (107205225 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:034c288a390667cc8689271b4c68b1f38eb2887a9931320f9fea3cd6cdb28dfb`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Fri, 26 Feb 2021 16:47:31 GMT
RUN Apply image 1809-amd64
# Wed, 10 Mar 2021 16:56:55 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 10 Mar 2021 21:49:39 GMT
RUN cmd /S /C #(nop) COPY file:189ca6af047e9f9cf54ab2176b48588e01c7497fe0b5b0d7b2614ebad66ed089 in C:\nats-streaming-server.exe 
# Wed, 10 Mar 2021 21:49:40 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 10 Mar 2021 21:49:41 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 10 Mar 2021 21:49:42 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:a11c4ca8f1ba16b6e1395d4523be2215bd0871c2e3e4695b9f2b87bd7472be52`  
		Size: 101.4 MB (101389964 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f49969195f32b7e40a81e3d189259fec7ebf52ee0ec5dafd5f3f288715354fed`  
		Last Modified: Wed, 10 Mar 2021 17:01:57 GMT  
		Size: 1.0 KB (1047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d5345eab816862154342d0ef80781aae11144d15f84ad4ac1d5ed1bbf9b083e`  
		Last Modified: Wed, 10 Mar 2021 21:54:51 GMT  
		Size: 5.8 MB (5810691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d886b78bda0fe938d4c7e8a21e511102e719280871d97e9e7b3d4589222dffd`  
		Last Modified: Wed, 10 Mar 2021 21:54:51 GMT  
		Size: 1.2 KB (1180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3fce35e6d75d0e8ea6539c3a0e1f335dec61dfabde67c34ec07260f715ea526`  
		Last Modified: Wed, 10 Mar 2021 21:54:50 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b95ed8adcfdc36bcc766c7ca9db14a0bca9768321cc35854aa2d896ef75ea4ab`  
		Last Modified: Wed, 10 Mar 2021 21:54:49 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.21-nanoserver-1809`

```console
$ docker pull nats-streaming@sha256:87d3bbcab917eb6d04e19e5623d88b465ff072b603fa498c4b7299035fbdf1e7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1817; amd64

### `nats-streaming:0.21-nanoserver-1809` - windows version 10.0.17763.1817; amd64

```console
$ docker pull nats-streaming@sha256:b1027771e781ed856534f3ee9d9fc845e0a08d4ac903949056fa3613a1025713
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.2 MB (107205225 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:034c288a390667cc8689271b4c68b1f38eb2887a9931320f9fea3cd6cdb28dfb`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Fri, 26 Feb 2021 16:47:31 GMT
RUN Apply image 1809-amd64
# Wed, 10 Mar 2021 16:56:55 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 10 Mar 2021 21:49:39 GMT
RUN cmd /S /C #(nop) COPY file:189ca6af047e9f9cf54ab2176b48588e01c7497fe0b5b0d7b2614ebad66ed089 in C:\nats-streaming-server.exe 
# Wed, 10 Mar 2021 21:49:40 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 10 Mar 2021 21:49:41 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 10 Mar 2021 21:49:42 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:a11c4ca8f1ba16b6e1395d4523be2215bd0871c2e3e4695b9f2b87bd7472be52`  
		Size: 101.4 MB (101389964 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f49969195f32b7e40a81e3d189259fec7ebf52ee0ec5dafd5f3f288715354fed`  
		Last Modified: Wed, 10 Mar 2021 17:01:57 GMT  
		Size: 1.0 KB (1047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d5345eab816862154342d0ef80781aae11144d15f84ad4ac1d5ed1bbf9b083e`  
		Last Modified: Wed, 10 Mar 2021 21:54:51 GMT  
		Size: 5.8 MB (5810691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d886b78bda0fe938d4c7e8a21e511102e719280871d97e9e7b3d4589222dffd`  
		Last Modified: Wed, 10 Mar 2021 21:54:51 GMT  
		Size: 1.2 KB (1180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3fce35e6d75d0e8ea6539c3a0e1f335dec61dfabde67c34ec07260f715ea526`  
		Last Modified: Wed, 10 Mar 2021 21:54:50 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b95ed8adcfdc36bcc766c7ca9db14a0bca9768321cc35854aa2d896ef75ea4ab`  
		Last Modified: Wed, 10 Mar 2021 21:54:49 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.21-scratch`

```console
$ docker pull nats-streaming@sha256:26603f9112b727df8e9736407a1ec1ab031317a9f6964ba0d407baea6b8d152c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.21-scratch` - linux; amd64

```console
$ docker pull nats-streaming@sha256:aa6af76760541ce71d366ac25554ad7caa95aea8cd230dd2688fd76b0645b329
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.7 MB (5680474 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31671965fc8e3e2d623279516e43fd9d1a5d8d82a19fe709c69d7bfe7ac50085`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Sat, 06 Mar 2021 07:43:28 GMT
COPY file:2c21a07cd43acfd157f86c6cf727430cf07e201a3bf3668b2083f473385db991 in /nats-streaming-server 
# Sat, 06 Mar 2021 07:43:28 GMT
EXPOSE 4222 8222
# Sat, 06 Mar 2021 07:43:29 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Sat, 06 Mar 2021 07:43:29 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:6f1c3ed40f752c2108b0e5d9224fba83d5045dac3370f93a50d91af0bc201c05`  
		Last Modified: Sat, 06 Mar 2021 07:44:17 GMT  
		Size: 5.7 MB (5680474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.21-scratch` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:907a450228b0d46339c5af803a9475165f7cfd9d20d5e09e8f66f9d048d1f7b9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.3 MB (5252895 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8c6d73cc983f6821e57de28a32cec901f28d3c5ada68aa9e71a1880962a9f07`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Sat, 06 Mar 2021 02:10:29 GMT
COPY file:bd617234b457ddee67b99f0e411029c6d5badad5059fbd81239c0acfe92cd4b7 in /nats-streaming-server 
# Sat, 06 Mar 2021 02:10:30 GMT
EXPOSE 4222 8222
# Sat, 06 Mar 2021 02:10:31 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Sat, 06 Mar 2021 02:10:31 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:ef1f32aa7a9ce9c8d42c909d32f61dabfa957c0b6a2b3590cd5e5847fb634355`  
		Last Modified: Sat, 06 Mar 2021 02:11:15 GMT  
		Size: 5.3 MB (5252895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.21-scratch` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:ae774aee41bd64306207d739d2290639f673c9c66c367a83f155a923fe8c13f6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5246286 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ce52186dd957f6b70b086fdcbc8212e079e5ed5e3e0013f8f72b3922535a56e`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Sat, 06 Mar 2021 01:00:25 GMT
COPY file:546c18b3e8e91d453d1a325c6e4dbc3c945564c010676da1abe89a653a0dea84 in /nats-streaming-server 
# Sat, 06 Mar 2021 01:00:27 GMT
EXPOSE 4222 8222
# Sat, 06 Mar 2021 01:00:28 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Sat, 06 Mar 2021 01:00:29 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:ed8ed2aa5d978cf51ebe3454de1832aeb40919052c5cb17d5b63865c31fc03c7`  
		Last Modified: Sat, 06 Mar 2021 01:01:07 GMT  
		Size: 5.2 MB (5246286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.21-scratch` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:7fccb492771f9c26f12f03c49e84ba4fb4d7004c6d142f4a7b83337d92feda95
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5170586 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07e817dd7b95371ae514afe3154e4aeba302d94dbed618a0aba7ece8696c13c6`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Sat, 06 Mar 2021 01:51:04 GMT
COPY file:ed938be8d92952afe74223a94317bf582d9bcf2c458a54733da01a37a65d421b in /nats-streaming-server 
# Sat, 06 Mar 2021 01:51:05 GMT
EXPOSE 4222 8222
# Sat, 06 Mar 2021 01:51:06 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Sat, 06 Mar 2021 01:51:07 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:f5ab53e298c8bd7b93e991f4b12e4015cde7d604e6d5ee086e994a86e0556094`  
		Last Modified: Sat, 06 Mar 2021 01:51:46 GMT  
		Size: 5.2 MB (5170586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.21-windowsservercore`

```console
$ docker pull nats-streaming@sha256:66bcec534b0a6ed19b5da3dcfda012ddc502d29eebfd14ce18b84e8e72879a30
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1817; amd64
	-	windows version 10.0.14393.4283; amd64

### `nats-streaming:0.21-windowsservercore` - windows version 10.0.17763.1817; amd64

```console
$ docker pull nats-streaming@sha256:7c32d8674de2b5a73ba6be51bb6514302b5c28001cb43905c393a60b63302467
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2481844979 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:201caf193f01ab7ea82dbd134d0a0e2fe29e689b1e03dfd0f19f0e397c693db6`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
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
# Wed, 10 Mar 2021 21:47:25 GMT
ENV NATS_STREAMING_SERVER=0.21.1
# Wed, 10 Mar 2021 21:47:26 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.21.1/nats-streaming-server-v0.21.1-windows-amd64.zip
# Wed, 10 Mar 2021 21:47:27 GMT
ENV GIT_DOWNLOAD_SHA256=798ec9b686a8dcb4de93074f416eab067a0896b52ccfc05b65a5e21d55e634e5
# Wed, 10 Mar 2021 21:48:01 GMT
RUN Set-PSDebug -Trace 2
# Wed, 10 Mar 2021 21:49:26 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 10 Mar 2021 21:49:27 GMT
EXPOSE 4222 8222
# Wed, 10 Mar 2021 21:49:28 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 10 Mar 2021 21:49:29 GMT
CMD ["-m" "8222"]
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
	-	`sha256:53877335227f3a676a7b42a4bfe29f3b308e4af725358ddb37e2a44fa6921a80`  
		Last Modified: Wed, 10 Mar 2021 21:54:20 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dded724566db49b2c3de437e8fc07b33da7a82fefc8ee1d6a90ce90bfb721914`  
		Last Modified: Wed, 10 Mar 2021 21:54:20 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55a9876360e291e6db5b15d8903e950e266fac317bbc049509fe3d0380a967ad`  
		Last Modified: Wed, 10 Mar 2021 21:54:20 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b3231bc8381e2d5c4e0ae136f5651b2459e1c4cfb039dc7d04233feace0fb3d`  
		Last Modified: Wed, 10 Mar 2021 21:54:19 GMT  
		Size: 5.1 MB (5064941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71a29a16a4eecc21940d5d0238db4f5e29fdf352f211193dd0d6ddc0a8392dee`  
		Last Modified: Wed, 10 Mar 2021 21:54:35 GMT  
		Size: 15.2 MB (15234342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60e3f696c440330f05de9af154fef7a7668334bfd83a5b6891ece035ed7ec703`  
		Last Modified: Wed, 10 Mar 2021 21:54:17 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ad4ce6f8f2d876a7c5fd7cd6fa233132de5181d550403653062f6ecdc0bd1e5`  
		Last Modified: Wed, 10 Mar 2021 21:54:18 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00a0ea7fcfe009366fde55d37e5932c25b24e3d6d81960f8781f792e143878a2`  
		Last Modified: Wed, 10 Mar 2021 21:54:17 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.21-windowsservercore` - windows version 10.0.14393.4283; amd64

```console
$ docker pull nats-streaming@sha256:594f9b8a930c3fbb8aacf7073d6822799c21005df6b94a9f1a3da70a8ef6df2a
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5818554710 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:77a6062b4ea3c0f03780986b01c644987bf4ad33acbf270f345b28aef38775fe`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
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
# Wed, 10 Mar 2021 21:49:49 GMT
ENV NATS_STREAMING_SERVER=0.21.1
# Wed, 10 Mar 2021 21:49:50 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.21.1/nats-streaming-server-v0.21.1-windows-amd64.zip
# Wed, 10 Mar 2021 21:49:51 GMT
ENV GIT_DOWNLOAD_SHA256=798ec9b686a8dcb4de93074f416eab067a0896b52ccfc05b65a5e21d55e634e5
# Wed, 10 Mar 2021 21:51:17 GMT
RUN Set-PSDebug -Trace 2
# Wed, 10 Mar 2021 21:53:25 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 10 Mar 2021 21:53:26 GMT
EXPOSE 4222 8222
# Wed, 10 Mar 2021 21:53:27 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 10 Mar 2021 21:53:28 GMT
CMD ["-m" "8222"]
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
	-	`sha256:3ea87885047b4a1f6a8e0632983da50ba4f31825a69b4f1e13ccb486984dbb81`  
		Last Modified: Wed, 10 Mar 2021 21:55:07 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57acbb65b7dc63351cdcbb771089539683461cd139e5a805bc3f0127181f38b1`  
		Last Modified: Wed, 10 Mar 2021 21:55:07 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5a204c1ad231fc6dfe4d92999bbe0aa9bad4a980ac2f89cdc05255a29a2bb0d`  
		Last Modified: Wed, 10 Mar 2021 21:55:07 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:817aa91f0e76ec219774d8759cba12fd464149e745865ab86ced46d6348f7d7f`  
		Last Modified: Wed, 10 Mar 2021 21:55:06 GMT  
		Size: 5.6 MB (5647336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a811f82bd6b42793f3d47bd0f94e40f0fbb9eefbe192813e03c13c50e897d604`  
		Last Modified: Wed, 10 Mar 2021 21:55:24 GMT  
		Size: 16.0 MB (15985398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba9f62bca657f59242456b4816b9f7ede6deced4cc0c1f90543b33b636084b98`  
		Last Modified: Wed, 10 Mar 2021 21:55:05 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf0ec3239c36380ddf5a7cda6e2fcdd186a3226ea98b17f33b0e083f84d5674e`  
		Last Modified: Wed, 10 Mar 2021 21:55:05 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ae978e2e615d8811e5f542215f7fefa26cdfc9025deee761d653bc3973fda1c`  
		Last Modified: Wed, 10 Mar 2021 21:55:05 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.21-windowsservercore-1809`

```console
$ docker pull nats-streaming@sha256:4bcd57606636d40356494deb4e00e85814521e94ea1d39150b42ed55d5da2276
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1817; amd64

### `nats-streaming:0.21-windowsservercore-1809` - windows version 10.0.17763.1817; amd64

```console
$ docker pull nats-streaming@sha256:7c32d8674de2b5a73ba6be51bb6514302b5c28001cb43905c393a60b63302467
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2481844979 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:201caf193f01ab7ea82dbd134d0a0e2fe29e689b1e03dfd0f19f0e397c693db6`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
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
# Wed, 10 Mar 2021 21:47:25 GMT
ENV NATS_STREAMING_SERVER=0.21.1
# Wed, 10 Mar 2021 21:47:26 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.21.1/nats-streaming-server-v0.21.1-windows-amd64.zip
# Wed, 10 Mar 2021 21:47:27 GMT
ENV GIT_DOWNLOAD_SHA256=798ec9b686a8dcb4de93074f416eab067a0896b52ccfc05b65a5e21d55e634e5
# Wed, 10 Mar 2021 21:48:01 GMT
RUN Set-PSDebug -Trace 2
# Wed, 10 Mar 2021 21:49:26 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 10 Mar 2021 21:49:27 GMT
EXPOSE 4222 8222
# Wed, 10 Mar 2021 21:49:28 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 10 Mar 2021 21:49:29 GMT
CMD ["-m" "8222"]
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
	-	`sha256:53877335227f3a676a7b42a4bfe29f3b308e4af725358ddb37e2a44fa6921a80`  
		Last Modified: Wed, 10 Mar 2021 21:54:20 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dded724566db49b2c3de437e8fc07b33da7a82fefc8ee1d6a90ce90bfb721914`  
		Last Modified: Wed, 10 Mar 2021 21:54:20 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55a9876360e291e6db5b15d8903e950e266fac317bbc049509fe3d0380a967ad`  
		Last Modified: Wed, 10 Mar 2021 21:54:20 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b3231bc8381e2d5c4e0ae136f5651b2459e1c4cfb039dc7d04233feace0fb3d`  
		Last Modified: Wed, 10 Mar 2021 21:54:19 GMT  
		Size: 5.1 MB (5064941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71a29a16a4eecc21940d5d0238db4f5e29fdf352f211193dd0d6ddc0a8392dee`  
		Last Modified: Wed, 10 Mar 2021 21:54:35 GMT  
		Size: 15.2 MB (15234342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60e3f696c440330f05de9af154fef7a7668334bfd83a5b6891ece035ed7ec703`  
		Last Modified: Wed, 10 Mar 2021 21:54:17 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ad4ce6f8f2d876a7c5fd7cd6fa233132de5181d550403653062f6ecdc0bd1e5`  
		Last Modified: Wed, 10 Mar 2021 21:54:18 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00a0ea7fcfe009366fde55d37e5932c25b24e3d6d81960f8781f792e143878a2`  
		Last Modified: Wed, 10 Mar 2021 21:54:17 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.21-windowsservercore-ltsc2016`

```console
$ docker pull nats-streaming@sha256:a79ba4262fcf0cb90e75fab395c2d6dc8126dbc4bfa7bddc82f31cfcd3c25409
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4283; amd64

### `nats-streaming:0.21-windowsservercore-ltsc2016` - windows version 10.0.14393.4283; amd64

```console
$ docker pull nats-streaming@sha256:594f9b8a930c3fbb8aacf7073d6822799c21005df6b94a9f1a3da70a8ef6df2a
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5818554710 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:77a6062b4ea3c0f03780986b01c644987bf4ad33acbf270f345b28aef38775fe`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
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
# Wed, 10 Mar 2021 21:49:49 GMT
ENV NATS_STREAMING_SERVER=0.21.1
# Wed, 10 Mar 2021 21:49:50 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.21.1/nats-streaming-server-v0.21.1-windows-amd64.zip
# Wed, 10 Mar 2021 21:49:51 GMT
ENV GIT_DOWNLOAD_SHA256=798ec9b686a8dcb4de93074f416eab067a0896b52ccfc05b65a5e21d55e634e5
# Wed, 10 Mar 2021 21:51:17 GMT
RUN Set-PSDebug -Trace 2
# Wed, 10 Mar 2021 21:53:25 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 10 Mar 2021 21:53:26 GMT
EXPOSE 4222 8222
# Wed, 10 Mar 2021 21:53:27 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 10 Mar 2021 21:53:28 GMT
CMD ["-m" "8222"]
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
	-	`sha256:3ea87885047b4a1f6a8e0632983da50ba4f31825a69b4f1e13ccb486984dbb81`  
		Last Modified: Wed, 10 Mar 2021 21:55:07 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57acbb65b7dc63351cdcbb771089539683461cd139e5a805bc3f0127181f38b1`  
		Last Modified: Wed, 10 Mar 2021 21:55:07 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5a204c1ad231fc6dfe4d92999bbe0aa9bad4a980ac2f89cdc05255a29a2bb0d`  
		Last Modified: Wed, 10 Mar 2021 21:55:07 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:817aa91f0e76ec219774d8759cba12fd464149e745865ab86ced46d6348f7d7f`  
		Last Modified: Wed, 10 Mar 2021 21:55:06 GMT  
		Size: 5.6 MB (5647336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a811f82bd6b42793f3d47bd0f94e40f0fbb9eefbe192813e03c13c50e897d604`  
		Last Modified: Wed, 10 Mar 2021 21:55:24 GMT  
		Size: 16.0 MB (15985398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba9f62bca657f59242456b4816b9f7ede6deced4cc0c1f90543b33b636084b98`  
		Last Modified: Wed, 10 Mar 2021 21:55:05 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf0ec3239c36380ddf5a7cda6e2fcdd186a3226ea98b17f33b0e083f84d5674e`  
		Last Modified: Wed, 10 Mar 2021 21:55:05 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ae978e2e615d8811e5f542215f7fefa26cdfc9025deee761d653bc3973fda1c`  
		Last Modified: Wed, 10 Mar 2021 21:55:05 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.21.1`

```console
$ docker pull nats-streaming@sha256:42dd817d3798a2288a0dfbd2a8f520b497ff170316f38a13c4d09f2be70f4e99
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.1817; amd64

### `nats-streaming:0.21.1` - linux; amd64

```console
$ docker pull nats-streaming@sha256:aa6af76760541ce71d366ac25554ad7caa95aea8cd230dd2688fd76b0645b329
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.7 MB (5680474 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31671965fc8e3e2d623279516e43fd9d1a5d8d82a19fe709c69d7bfe7ac50085`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Sat, 06 Mar 2021 07:43:28 GMT
COPY file:2c21a07cd43acfd157f86c6cf727430cf07e201a3bf3668b2083f473385db991 in /nats-streaming-server 
# Sat, 06 Mar 2021 07:43:28 GMT
EXPOSE 4222 8222
# Sat, 06 Mar 2021 07:43:29 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Sat, 06 Mar 2021 07:43:29 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:6f1c3ed40f752c2108b0e5d9224fba83d5045dac3370f93a50d91af0bc201c05`  
		Last Modified: Sat, 06 Mar 2021 07:44:17 GMT  
		Size: 5.7 MB (5680474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.21.1` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:907a450228b0d46339c5af803a9475165f7cfd9d20d5e09e8f66f9d048d1f7b9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.3 MB (5252895 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8c6d73cc983f6821e57de28a32cec901f28d3c5ada68aa9e71a1880962a9f07`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Sat, 06 Mar 2021 02:10:29 GMT
COPY file:bd617234b457ddee67b99f0e411029c6d5badad5059fbd81239c0acfe92cd4b7 in /nats-streaming-server 
# Sat, 06 Mar 2021 02:10:30 GMT
EXPOSE 4222 8222
# Sat, 06 Mar 2021 02:10:31 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Sat, 06 Mar 2021 02:10:31 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:ef1f32aa7a9ce9c8d42c909d32f61dabfa957c0b6a2b3590cd5e5847fb634355`  
		Last Modified: Sat, 06 Mar 2021 02:11:15 GMT  
		Size: 5.3 MB (5252895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.21.1` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:ae774aee41bd64306207d739d2290639f673c9c66c367a83f155a923fe8c13f6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5246286 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ce52186dd957f6b70b086fdcbc8212e079e5ed5e3e0013f8f72b3922535a56e`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Sat, 06 Mar 2021 01:00:25 GMT
COPY file:546c18b3e8e91d453d1a325c6e4dbc3c945564c010676da1abe89a653a0dea84 in /nats-streaming-server 
# Sat, 06 Mar 2021 01:00:27 GMT
EXPOSE 4222 8222
# Sat, 06 Mar 2021 01:00:28 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Sat, 06 Mar 2021 01:00:29 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:ed8ed2aa5d978cf51ebe3454de1832aeb40919052c5cb17d5b63865c31fc03c7`  
		Last Modified: Sat, 06 Mar 2021 01:01:07 GMT  
		Size: 5.2 MB (5246286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.21.1` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:7fccb492771f9c26f12f03c49e84ba4fb4d7004c6d142f4a7b83337d92feda95
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5170586 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07e817dd7b95371ae514afe3154e4aeba302d94dbed618a0aba7ece8696c13c6`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Sat, 06 Mar 2021 01:51:04 GMT
COPY file:ed938be8d92952afe74223a94317bf582d9bcf2c458a54733da01a37a65d421b in /nats-streaming-server 
# Sat, 06 Mar 2021 01:51:05 GMT
EXPOSE 4222 8222
# Sat, 06 Mar 2021 01:51:06 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Sat, 06 Mar 2021 01:51:07 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:f5ab53e298c8bd7b93e991f4b12e4015cde7d604e6d5ee086e994a86e0556094`  
		Last Modified: Sat, 06 Mar 2021 01:51:46 GMT  
		Size: 5.2 MB (5170586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.21.1` - windows version 10.0.17763.1817; amd64

```console
$ docker pull nats-streaming@sha256:b1027771e781ed856534f3ee9d9fc845e0a08d4ac903949056fa3613a1025713
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.2 MB (107205225 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:034c288a390667cc8689271b4c68b1f38eb2887a9931320f9fea3cd6cdb28dfb`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Fri, 26 Feb 2021 16:47:31 GMT
RUN Apply image 1809-amd64
# Wed, 10 Mar 2021 16:56:55 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 10 Mar 2021 21:49:39 GMT
RUN cmd /S /C #(nop) COPY file:189ca6af047e9f9cf54ab2176b48588e01c7497fe0b5b0d7b2614ebad66ed089 in C:\nats-streaming-server.exe 
# Wed, 10 Mar 2021 21:49:40 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 10 Mar 2021 21:49:41 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 10 Mar 2021 21:49:42 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:a11c4ca8f1ba16b6e1395d4523be2215bd0871c2e3e4695b9f2b87bd7472be52`  
		Size: 101.4 MB (101389964 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f49969195f32b7e40a81e3d189259fec7ebf52ee0ec5dafd5f3f288715354fed`  
		Last Modified: Wed, 10 Mar 2021 17:01:57 GMT  
		Size: 1.0 KB (1047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d5345eab816862154342d0ef80781aae11144d15f84ad4ac1d5ed1bbf9b083e`  
		Last Modified: Wed, 10 Mar 2021 21:54:51 GMT  
		Size: 5.8 MB (5810691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d886b78bda0fe938d4c7e8a21e511102e719280871d97e9e7b3d4589222dffd`  
		Last Modified: Wed, 10 Mar 2021 21:54:51 GMT  
		Size: 1.2 KB (1180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3fce35e6d75d0e8ea6539c3a0e1f335dec61dfabde67c34ec07260f715ea526`  
		Last Modified: Wed, 10 Mar 2021 21:54:50 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b95ed8adcfdc36bcc766c7ca9db14a0bca9768321cc35854aa2d896ef75ea4ab`  
		Last Modified: Wed, 10 Mar 2021 21:54:49 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.21.1-alpine`

```console
$ docker pull nats-streaming@sha256:1941dba2b56c072871d4ce1aecc9b9ec0f9ac9776e8c59aaf6252b6d180fbf59
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.21.1-alpine` - linux; amd64

```console
$ docker pull nats-streaming@sha256:701fa3e7165e338d3fb61b4f7068af826829b094fc089e1b7866466bc4cba85e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.8 MB (8774552 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3593598c050f5241766331b8aed01f6c3f42b71938fc11f47bbfa18d74c829be`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 17 Feb 2021 21:19:54 GMT
ADD file:80bf8bd014071345b1c0364eeb0a5e48f3fb0d87f9c31cb990e57caa652b59b8 in / 
# Wed, 17 Feb 2021 21:19:54 GMT
CMD ["/bin/sh"]
# Sat, 06 Mar 2021 07:43:18 GMT
ENV NATS_STREAMING_SERVER=0.21.1
# Sat, 06 Mar 2021 07:43:22 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='06d591a61084aab1046e818486c2ee7c3936214c92dc257084693d6ffe06342b' ;; 		armhf) natsArch='arm6'; sha256='085375782abe1bacbd6fc609ce6a6721f029cba312733479204c89bf92f1e188' ;; 		armv7) natsArch='arm7'; sha256='947d91512b47ba98198bef7f799670c40cf6949f2ba2e98b5c133e6166e9b97c' ;; 		x86_64) natsArch='amd64'; sha256='85fd7fd3c7b71cbc9043900f9110b028f1fdc042c6500eed065e6e2c3331f62e' ;; 		x86) natsArch='386'; sha256='475b0f015726af99c9ea779c8bbbeaa729ef90f43dd2715273fea81fb90ea63a' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Sat, 06 Mar 2021 07:43:22 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Sat, 06 Mar 2021 07:43:22 GMT
EXPOSE 4222 8222
# Sat, 06 Mar 2021 07:43:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 06 Mar 2021 07:43:23 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:ba3557a56b150f9b813f9d02274d62914fd8fce120dd374d9ee17b87cf1d277d`  
		Last Modified: Wed, 17 Feb 2021 21:20:25 GMT  
		Size: 2.8 MB (2811657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ae3e2d2b3e48427fd1213fbc4722666443f13ca1a6709825a2afbbf6381367d`  
		Last Modified: Sat, 06 Mar 2021 07:43:55 GMT  
		Size: 6.0 MB (5962472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19a250278b77e3fdc0d10076a12c9d14803a891ccfb31290836d192e35da8a03`  
		Last Modified: Sat, 06 Mar 2021 07:43:54 GMT  
		Size: 423.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.21.1-alpine` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:19373a83f61771319d0aacfab1086d496a2dd1535970f8a20652d56cf2b7578e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.2 MB (8156412 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:935ff18ff1bfcc7d421f422b0d98ef2b111e05c4e09b1e57aef68d71b18156b9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Thu, 25 Mar 2021 22:50:09 GMT
ADD file:ca4136238cb9a01d079efd129bccd1470945d7d4320da61373af90645a4b1146 in / 
# Thu, 25 Mar 2021 22:50:28 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 05:57:34 GMT
ENV NATS_STREAMING_SERVER=0.21.1
# Fri, 26 Mar 2021 05:57:41 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='06d591a61084aab1046e818486c2ee7c3936214c92dc257084693d6ffe06342b' ;; 		armhf) natsArch='arm6'; sha256='085375782abe1bacbd6fc609ce6a6721f029cba312733479204c89bf92f1e188' ;; 		armv7) natsArch='arm7'; sha256='947d91512b47ba98198bef7f799670c40cf6949f2ba2e98b5c133e6166e9b97c' ;; 		x86_64) natsArch='amd64'; sha256='85fd7fd3c7b71cbc9043900f9110b028f1fdc042c6500eed065e6e2c3331f62e' ;; 		x86) natsArch='386'; sha256='475b0f015726af99c9ea779c8bbbeaa729ef90f43dd2715273fea81fb90ea63a' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 26 Mar 2021 05:57:42 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Fri, 26 Mar 2021 05:57:43 GMT
EXPOSE 4222 8222
# Fri, 26 Mar 2021 05:57:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 05:57:46 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:bca6a70a54896d072b6919d2ae18d3ef685bc7aed783731f68a4adac0fb93d52`  
		Last Modified: Thu, 25 Mar 2021 22:54:24 GMT  
		Size: 2.6 MB (2622062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37dde547b7fced1153630086dee787892a218966ea430c2964f55f72bcbbf83a`  
		Last Modified: Fri, 26 Mar 2021 05:58:16 GMT  
		Size: 5.5 MB (5533929 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df980303a7fb93b8683964b371b30ef03ef35e26de48621d858290228f8b3346`  
		Last Modified: Fri, 26 Mar 2021 05:58:14 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.21.1-alpine` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:f167b7ef1b6e893d3e176ad7fd41597e8a4da3720d0694b407e19e24b68cd5f6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.0 MB (7951584 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e033b7fa5e49122eff8379884102467952cb9d40190588eee42fd608ecbfe3d9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Thu, 25 Mar 2021 22:05:53 GMT
ADD file:44ef6cff6e7d37a67c5846eb792fec65025702c00c56ff96801ac79bf81b0cc3 in / 
# Thu, 25 Mar 2021 22:05:55 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 01:51:55 GMT
ENV NATS_STREAMING_SERVER=0.21.1
# Fri, 26 Mar 2021 01:52:03 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='06d591a61084aab1046e818486c2ee7c3936214c92dc257084693d6ffe06342b' ;; 		armhf) natsArch='arm6'; sha256='085375782abe1bacbd6fc609ce6a6721f029cba312733479204c89bf92f1e188' ;; 		armv7) natsArch='arm7'; sha256='947d91512b47ba98198bef7f799670c40cf6949f2ba2e98b5c133e6166e9b97c' ;; 		x86_64) natsArch='amd64'; sha256='85fd7fd3c7b71cbc9043900f9110b028f1fdc042c6500eed065e6e2c3331f62e' ;; 		x86) natsArch='386'; sha256='475b0f015726af99c9ea779c8bbbeaa729ef90f43dd2715273fea81fb90ea63a' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 26 Mar 2021 01:52:05 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Fri, 26 Mar 2021 01:52:11 GMT
EXPOSE 4222 8222
# Fri, 26 Mar 2021 01:52:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 01:52:14 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:6c1162af251f0d5ab4945f8506f3265b86d0a03cda37f703c2446a71a233bc20`  
		Last Modified: Thu, 25 Mar 2021 22:07:21 GMT  
		Size: 2.4 MB (2423999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61ca624cfb490a8a9fb48110381475a59604ddfd4920f6496398a887f8a37b73`  
		Last Modified: Fri, 26 Mar 2021 01:52:52 GMT  
		Size: 5.5 MB (5527163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3957a11b701f02a3361d365cd9b9c63fcafa89f362a40471a527bb31bbbe1de6`  
		Last Modified: Fri, 26 Mar 2021 01:52:50 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.21.1-alpine` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:1740e224df015e33133a9db91519ebc8601bf64861cde979a2ed6c556b649395
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.2 MB (8164487 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:205e781a3be342b949194bab8b6fde3763da1876fe7fac88af8efa1a07b3f204`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 17 Feb 2021 20:39:29 GMT
ADD file:3bf1497bd250cf7c73c12231dc4ebe3a3a67f2cd99e35bce47ef6674683aeb1d in / 
# Wed, 17 Feb 2021 20:39:30 GMT
CMD ["/bin/sh"]
# Sat, 06 Mar 2021 01:46:28 GMT
ENV NATS_STREAMING_SERVER=0.21.1
# Sat, 06 Mar 2021 01:46:33 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='06d591a61084aab1046e818486c2ee7c3936214c92dc257084693d6ffe06342b' ;; 		armhf) natsArch='arm6'; sha256='085375782abe1bacbd6fc609ce6a6721f029cba312733479204c89bf92f1e188' ;; 		armv7) natsArch='arm7'; sha256='947d91512b47ba98198bef7f799670c40cf6949f2ba2e98b5c133e6166e9b97c' ;; 		x86_64) natsArch='amd64'; sha256='85fd7fd3c7b71cbc9043900f9110b028f1fdc042c6500eed065e6e2c3331f62e' ;; 		x86) natsArch='386'; sha256='475b0f015726af99c9ea779c8bbbeaa729ef90f43dd2715273fea81fb90ea63a' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Sat, 06 Mar 2021 01:46:33 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Sat, 06 Mar 2021 01:46:34 GMT
EXPOSE 4222 8222
# Sat, 06 Mar 2021 01:46:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 06 Mar 2021 01:46:35 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:069a56d6d07f6b186fbb82e4486616b9be9a37ce32a63013af6cddcb65898182`  
		Last Modified: Wed, 17 Feb 2021 20:40:04 GMT  
		Size: 2.7 MB (2711572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e334db32136252e9605e0a6ef0426e8c0c50e757bb238a24330339d3dedbe84`  
		Last Modified: Sat, 06 Mar 2021 01:51:34 GMT  
		Size: 5.5 MB (5452492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7e903d8d08305b07378aef2e8c19af9f0d6b899ce053c33e5b6022c07b155e2`  
		Last Modified: Sat, 06 Mar 2021 01:51:32 GMT  
		Size: 423.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.21.1-alpine3.13`

```console
$ docker pull nats-streaming@sha256:1941dba2b56c072871d4ce1aecc9b9ec0f9ac9776e8c59aaf6252b6d180fbf59
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.21.1-alpine3.13` - linux; amd64

```console
$ docker pull nats-streaming@sha256:701fa3e7165e338d3fb61b4f7068af826829b094fc089e1b7866466bc4cba85e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.8 MB (8774552 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3593598c050f5241766331b8aed01f6c3f42b71938fc11f47bbfa18d74c829be`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 17 Feb 2021 21:19:54 GMT
ADD file:80bf8bd014071345b1c0364eeb0a5e48f3fb0d87f9c31cb990e57caa652b59b8 in / 
# Wed, 17 Feb 2021 21:19:54 GMT
CMD ["/bin/sh"]
# Sat, 06 Mar 2021 07:43:18 GMT
ENV NATS_STREAMING_SERVER=0.21.1
# Sat, 06 Mar 2021 07:43:22 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='06d591a61084aab1046e818486c2ee7c3936214c92dc257084693d6ffe06342b' ;; 		armhf) natsArch='arm6'; sha256='085375782abe1bacbd6fc609ce6a6721f029cba312733479204c89bf92f1e188' ;; 		armv7) natsArch='arm7'; sha256='947d91512b47ba98198bef7f799670c40cf6949f2ba2e98b5c133e6166e9b97c' ;; 		x86_64) natsArch='amd64'; sha256='85fd7fd3c7b71cbc9043900f9110b028f1fdc042c6500eed065e6e2c3331f62e' ;; 		x86) natsArch='386'; sha256='475b0f015726af99c9ea779c8bbbeaa729ef90f43dd2715273fea81fb90ea63a' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Sat, 06 Mar 2021 07:43:22 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Sat, 06 Mar 2021 07:43:22 GMT
EXPOSE 4222 8222
# Sat, 06 Mar 2021 07:43:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 06 Mar 2021 07:43:23 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:ba3557a56b150f9b813f9d02274d62914fd8fce120dd374d9ee17b87cf1d277d`  
		Last Modified: Wed, 17 Feb 2021 21:20:25 GMT  
		Size: 2.8 MB (2811657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ae3e2d2b3e48427fd1213fbc4722666443f13ca1a6709825a2afbbf6381367d`  
		Last Modified: Sat, 06 Mar 2021 07:43:55 GMT  
		Size: 6.0 MB (5962472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19a250278b77e3fdc0d10076a12c9d14803a891ccfb31290836d192e35da8a03`  
		Last Modified: Sat, 06 Mar 2021 07:43:54 GMT  
		Size: 423.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.21.1-alpine3.13` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:19373a83f61771319d0aacfab1086d496a2dd1535970f8a20652d56cf2b7578e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.2 MB (8156412 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:935ff18ff1bfcc7d421f422b0d98ef2b111e05c4e09b1e57aef68d71b18156b9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Thu, 25 Mar 2021 22:50:09 GMT
ADD file:ca4136238cb9a01d079efd129bccd1470945d7d4320da61373af90645a4b1146 in / 
# Thu, 25 Mar 2021 22:50:28 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 05:57:34 GMT
ENV NATS_STREAMING_SERVER=0.21.1
# Fri, 26 Mar 2021 05:57:41 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='06d591a61084aab1046e818486c2ee7c3936214c92dc257084693d6ffe06342b' ;; 		armhf) natsArch='arm6'; sha256='085375782abe1bacbd6fc609ce6a6721f029cba312733479204c89bf92f1e188' ;; 		armv7) natsArch='arm7'; sha256='947d91512b47ba98198bef7f799670c40cf6949f2ba2e98b5c133e6166e9b97c' ;; 		x86_64) natsArch='amd64'; sha256='85fd7fd3c7b71cbc9043900f9110b028f1fdc042c6500eed065e6e2c3331f62e' ;; 		x86) natsArch='386'; sha256='475b0f015726af99c9ea779c8bbbeaa729ef90f43dd2715273fea81fb90ea63a' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 26 Mar 2021 05:57:42 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Fri, 26 Mar 2021 05:57:43 GMT
EXPOSE 4222 8222
# Fri, 26 Mar 2021 05:57:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 05:57:46 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:bca6a70a54896d072b6919d2ae18d3ef685bc7aed783731f68a4adac0fb93d52`  
		Last Modified: Thu, 25 Mar 2021 22:54:24 GMT  
		Size: 2.6 MB (2622062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37dde547b7fced1153630086dee787892a218966ea430c2964f55f72bcbbf83a`  
		Last Modified: Fri, 26 Mar 2021 05:58:16 GMT  
		Size: 5.5 MB (5533929 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df980303a7fb93b8683964b371b30ef03ef35e26de48621d858290228f8b3346`  
		Last Modified: Fri, 26 Mar 2021 05:58:14 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.21.1-alpine3.13` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:f167b7ef1b6e893d3e176ad7fd41597e8a4da3720d0694b407e19e24b68cd5f6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.0 MB (7951584 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e033b7fa5e49122eff8379884102467952cb9d40190588eee42fd608ecbfe3d9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Thu, 25 Mar 2021 22:05:53 GMT
ADD file:44ef6cff6e7d37a67c5846eb792fec65025702c00c56ff96801ac79bf81b0cc3 in / 
# Thu, 25 Mar 2021 22:05:55 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 01:51:55 GMT
ENV NATS_STREAMING_SERVER=0.21.1
# Fri, 26 Mar 2021 01:52:03 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='06d591a61084aab1046e818486c2ee7c3936214c92dc257084693d6ffe06342b' ;; 		armhf) natsArch='arm6'; sha256='085375782abe1bacbd6fc609ce6a6721f029cba312733479204c89bf92f1e188' ;; 		armv7) natsArch='arm7'; sha256='947d91512b47ba98198bef7f799670c40cf6949f2ba2e98b5c133e6166e9b97c' ;; 		x86_64) natsArch='amd64'; sha256='85fd7fd3c7b71cbc9043900f9110b028f1fdc042c6500eed065e6e2c3331f62e' ;; 		x86) natsArch='386'; sha256='475b0f015726af99c9ea779c8bbbeaa729ef90f43dd2715273fea81fb90ea63a' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 26 Mar 2021 01:52:05 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Fri, 26 Mar 2021 01:52:11 GMT
EXPOSE 4222 8222
# Fri, 26 Mar 2021 01:52:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 01:52:14 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:6c1162af251f0d5ab4945f8506f3265b86d0a03cda37f703c2446a71a233bc20`  
		Last Modified: Thu, 25 Mar 2021 22:07:21 GMT  
		Size: 2.4 MB (2423999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61ca624cfb490a8a9fb48110381475a59604ddfd4920f6496398a887f8a37b73`  
		Last Modified: Fri, 26 Mar 2021 01:52:52 GMT  
		Size: 5.5 MB (5527163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3957a11b701f02a3361d365cd9b9c63fcafa89f362a40471a527bb31bbbe1de6`  
		Last Modified: Fri, 26 Mar 2021 01:52:50 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.21.1-alpine3.13` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:1740e224df015e33133a9db91519ebc8601bf64861cde979a2ed6c556b649395
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.2 MB (8164487 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:205e781a3be342b949194bab8b6fde3763da1876fe7fac88af8efa1a07b3f204`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 17 Feb 2021 20:39:29 GMT
ADD file:3bf1497bd250cf7c73c12231dc4ebe3a3a67f2cd99e35bce47ef6674683aeb1d in / 
# Wed, 17 Feb 2021 20:39:30 GMT
CMD ["/bin/sh"]
# Sat, 06 Mar 2021 01:46:28 GMT
ENV NATS_STREAMING_SERVER=0.21.1
# Sat, 06 Mar 2021 01:46:33 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='06d591a61084aab1046e818486c2ee7c3936214c92dc257084693d6ffe06342b' ;; 		armhf) natsArch='arm6'; sha256='085375782abe1bacbd6fc609ce6a6721f029cba312733479204c89bf92f1e188' ;; 		armv7) natsArch='arm7'; sha256='947d91512b47ba98198bef7f799670c40cf6949f2ba2e98b5c133e6166e9b97c' ;; 		x86_64) natsArch='amd64'; sha256='85fd7fd3c7b71cbc9043900f9110b028f1fdc042c6500eed065e6e2c3331f62e' ;; 		x86) natsArch='386'; sha256='475b0f015726af99c9ea779c8bbbeaa729ef90f43dd2715273fea81fb90ea63a' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Sat, 06 Mar 2021 01:46:33 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Sat, 06 Mar 2021 01:46:34 GMT
EXPOSE 4222 8222
# Sat, 06 Mar 2021 01:46:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 06 Mar 2021 01:46:35 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:069a56d6d07f6b186fbb82e4486616b9be9a37ce32a63013af6cddcb65898182`  
		Last Modified: Wed, 17 Feb 2021 20:40:04 GMT  
		Size: 2.7 MB (2711572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e334db32136252e9605e0a6ef0426e8c0c50e757bb238a24330339d3dedbe84`  
		Last Modified: Sat, 06 Mar 2021 01:51:34 GMT  
		Size: 5.5 MB (5452492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7e903d8d08305b07378aef2e8c19af9f0d6b899ce053c33e5b6022c07b155e2`  
		Last Modified: Sat, 06 Mar 2021 01:51:32 GMT  
		Size: 423.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.21.1-linux`

```console
$ docker pull nats-streaming@sha256:26603f9112b727df8e9736407a1ec1ab031317a9f6964ba0d407baea6b8d152c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.21.1-linux` - linux; amd64

```console
$ docker pull nats-streaming@sha256:aa6af76760541ce71d366ac25554ad7caa95aea8cd230dd2688fd76b0645b329
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.7 MB (5680474 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31671965fc8e3e2d623279516e43fd9d1a5d8d82a19fe709c69d7bfe7ac50085`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Sat, 06 Mar 2021 07:43:28 GMT
COPY file:2c21a07cd43acfd157f86c6cf727430cf07e201a3bf3668b2083f473385db991 in /nats-streaming-server 
# Sat, 06 Mar 2021 07:43:28 GMT
EXPOSE 4222 8222
# Sat, 06 Mar 2021 07:43:29 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Sat, 06 Mar 2021 07:43:29 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:6f1c3ed40f752c2108b0e5d9224fba83d5045dac3370f93a50d91af0bc201c05`  
		Last Modified: Sat, 06 Mar 2021 07:44:17 GMT  
		Size: 5.7 MB (5680474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.21.1-linux` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:907a450228b0d46339c5af803a9475165f7cfd9d20d5e09e8f66f9d048d1f7b9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.3 MB (5252895 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8c6d73cc983f6821e57de28a32cec901f28d3c5ada68aa9e71a1880962a9f07`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Sat, 06 Mar 2021 02:10:29 GMT
COPY file:bd617234b457ddee67b99f0e411029c6d5badad5059fbd81239c0acfe92cd4b7 in /nats-streaming-server 
# Sat, 06 Mar 2021 02:10:30 GMT
EXPOSE 4222 8222
# Sat, 06 Mar 2021 02:10:31 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Sat, 06 Mar 2021 02:10:31 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:ef1f32aa7a9ce9c8d42c909d32f61dabfa957c0b6a2b3590cd5e5847fb634355`  
		Last Modified: Sat, 06 Mar 2021 02:11:15 GMT  
		Size: 5.3 MB (5252895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.21.1-linux` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:ae774aee41bd64306207d739d2290639f673c9c66c367a83f155a923fe8c13f6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5246286 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ce52186dd957f6b70b086fdcbc8212e079e5ed5e3e0013f8f72b3922535a56e`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Sat, 06 Mar 2021 01:00:25 GMT
COPY file:546c18b3e8e91d453d1a325c6e4dbc3c945564c010676da1abe89a653a0dea84 in /nats-streaming-server 
# Sat, 06 Mar 2021 01:00:27 GMT
EXPOSE 4222 8222
# Sat, 06 Mar 2021 01:00:28 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Sat, 06 Mar 2021 01:00:29 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:ed8ed2aa5d978cf51ebe3454de1832aeb40919052c5cb17d5b63865c31fc03c7`  
		Last Modified: Sat, 06 Mar 2021 01:01:07 GMT  
		Size: 5.2 MB (5246286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.21.1-linux` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:7fccb492771f9c26f12f03c49e84ba4fb4d7004c6d142f4a7b83337d92feda95
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5170586 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07e817dd7b95371ae514afe3154e4aeba302d94dbed618a0aba7ece8696c13c6`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Sat, 06 Mar 2021 01:51:04 GMT
COPY file:ed938be8d92952afe74223a94317bf582d9bcf2c458a54733da01a37a65d421b in /nats-streaming-server 
# Sat, 06 Mar 2021 01:51:05 GMT
EXPOSE 4222 8222
# Sat, 06 Mar 2021 01:51:06 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Sat, 06 Mar 2021 01:51:07 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:f5ab53e298c8bd7b93e991f4b12e4015cde7d604e6d5ee086e994a86e0556094`  
		Last Modified: Sat, 06 Mar 2021 01:51:46 GMT  
		Size: 5.2 MB (5170586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.21.1-nanoserver`

```console
$ docker pull nats-streaming@sha256:87d3bbcab917eb6d04e19e5623d88b465ff072b603fa498c4b7299035fbdf1e7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1817; amd64

### `nats-streaming:0.21.1-nanoserver` - windows version 10.0.17763.1817; amd64

```console
$ docker pull nats-streaming@sha256:b1027771e781ed856534f3ee9d9fc845e0a08d4ac903949056fa3613a1025713
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.2 MB (107205225 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:034c288a390667cc8689271b4c68b1f38eb2887a9931320f9fea3cd6cdb28dfb`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Fri, 26 Feb 2021 16:47:31 GMT
RUN Apply image 1809-amd64
# Wed, 10 Mar 2021 16:56:55 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 10 Mar 2021 21:49:39 GMT
RUN cmd /S /C #(nop) COPY file:189ca6af047e9f9cf54ab2176b48588e01c7497fe0b5b0d7b2614ebad66ed089 in C:\nats-streaming-server.exe 
# Wed, 10 Mar 2021 21:49:40 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 10 Mar 2021 21:49:41 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 10 Mar 2021 21:49:42 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:a11c4ca8f1ba16b6e1395d4523be2215bd0871c2e3e4695b9f2b87bd7472be52`  
		Size: 101.4 MB (101389964 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f49969195f32b7e40a81e3d189259fec7ebf52ee0ec5dafd5f3f288715354fed`  
		Last Modified: Wed, 10 Mar 2021 17:01:57 GMT  
		Size: 1.0 KB (1047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d5345eab816862154342d0ef80781aae11144d15f84ad4ac1d5ed1bbf9b083e`  
		Last Modified: Wed, 10 Mar 2021 21:54:51 GMT  
		Size: 5.8 MB (5810691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d886b78bda0fe938d4c7e8a21e511102e719280871d97e9e7b3d4589222dffd`  
		Last Modified: Wed, 10 Mar 2021 21:54:51 GMT  
		Size: 1.2 KB (1180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3fce35e6d75d0e8ea6539c3a0e1f335dec61dfabde67c34ec07260f715ea526`  
		Last Modified: Wed, 10 Mar 2021 21:54:50 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b95ed8adcfdc36bcc766c7ca9db14a0bca9768321cc35854aa2d896ef75ea4ab`  
		Last Modified: Wed, 10 Mar 2021 21:54:49 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.21.1-nanoserver-1809`

```console
$ docker pull nats-streaming@sha256:87d3bbcab917eb6d04e19e5623d88b465ff072b603fa498c4b7299035fbdf1e7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1817; amd64

### `nats-streaming:0.21.1-nanoserver-1809` - windows version 10.0.17763.1817; amd64

```console
$ docker pull nats-streaming@sha256:b1027771e781ed856534f3ee9d9fc845e0a08d4ac903949056fa3613a1025713
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.2 MB (107205225 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:034c288a390667cc8689271b4c68b1f38eb2887a9931320f9fea3cd6cdb28dfb`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Fri, 26 Feb 2021 16:47:31 GMT
RUN Apply image 1809-amd64
# Wed, 10 Mar 2021 16:56:55 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 10 Mar 2021 21:49:39 GMT
RUN cmd /S /C #(nop) COPY file:189ca6af047e9f9cf54ab2176b48588e01c7497fe0b5b0d7b2614ebad66ed089 in C:\nats-streaming-server.exe 
# Wed, 10 Mar 2021 21:49:40 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 10 Mar 2021 21:49:41 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 10 Mar 2021 21:49:42 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:a11c4ca8f1ba16b6e1395d4523be2215bd0871c2e3e4695b9f2b87bd7472be52`  
		Size: 101.4 MB (101389964 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f49969195f32b7e40a81e3d189259fec7ebf52ee0ec5dafd5f3f288715354fed`  
		Last Modified: Wed, 10 Mar 2021 17:01:57 GMT  
		Size: 1.0 KB (1047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d5345eab816862154342d0ef80781aae11144d15f84ad4ac1d5ed1bbf9b083e`  
		Last Modified: Wed, 10 Mar 2021 21:54:51 GMT  
		Size: 5.8 MB (5810691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d886b78bda0fe938d4c7e8a21e511102e719280871d97e9e7b3d4589222dffd`  
		Last Modified: Wed, 10 Mar 2021 21:54:51 GMT  
		Size: 1.2 KB (1180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3fce35e6d75d0e8ea6539c3a0e1f335dec61dfabde67c34ec07260f715ea526`  
		Last Modified: Wed, 10 Mar 2021 21:54:50 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b95ed8adcfdc36bcc766c7ca9db14a0bca9768321cc35854aa2d896ef75ea4ab`  
		Last Modified: Wed, 10 Mar 2021 21:54:49 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.21.1-scratch`

```console
$ docker pull nats-streaming@sha256:26603f9112b727df8e9736407a1ec1ab031317a9f6964ba0d407baea6b8d152c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.21.1-scratch` - linux; amd64

```console
$ docker pull nats-streaming@sha256:aa6af76760541ce71d366ac25554ad7caa95aea8cd230dd2688fd76b0645b329
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.7 MB (5680474 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31671965fc8e3e2d623279516e43fd9d1a5d8d82a19fe709c69d7bfe7ac50085`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Sat, 06 Mar 2021 07:43:28 GMT
COPY file:2c21a07cd43acfd157f86c6cf727430cf07e201a3bf3668b2083f473385db991 in /nats-streaming-server 
# Sat, 06 Mar 2021 07:43:28 GMT
EXPOSE 4222 8222
# Sat, 06 Mar 2021 07:43:29 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Sat, 06 Mar 2021 07:43:29 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:6f1c3ed40f752c2108b0e5d9224fba83d5045dac3370f93a50d91af0bc201c05`  
		Last Modified: Sat, 06 Mar 2021 07:44:17 GMT  
		Size: 5.7 MB (5680474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.21.1-scratch` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:907a450228b0d46339c5af803a9475165f7cfd9d20d5e09e8f66f9d048d1f7b9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.3 MB (5252895 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8c6d73cc983f6821e57de28a32cec901f28d3c5ada68aa9e71a1880962a9f07`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Sat, 06 Mar 2021 02:10:29 GMT
COPY file:bd617234b457ddee67b99f0e411029c6d5badad5059fbd81239c0acfe92cd4b7 in /nats-streaming-server 
# Sat, 06 Mar 2021 02:10:30 GMT
EXPOSE 4222 8222
# Sat, 06 Mar 2021 02:10:31 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Sat, 06 Mar 2021 02:10:31 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:ef1f32aa7a9ce9c8d42c909d32f61dabfa957c0b6a2b3590cd5e5847fb634355`  
		Last Modified: Sat, 06 Mar 2021 02:11:15 GMT  
		Size: 5.3 MB (5252895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.21.1-scratch` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:ae774aee41bd64306207d739d2290639f673c9c66c367a83f155a923fe8c13f6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5246286 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ce52186dd957f6b70b086fdcbc8212e079e5ed5e3e0013f8f72b3922535a56e`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Sat, 06 Mar 2021 01:00:25 GMT
COPY file:546c18b3e8e91d453d1a325c6e4dbc3c945564c010676da1abe89a653a0dea84 in /nats-streaming-server 
# Sat, 06 Mar 2021 01:00:27 GMT
EXPOSE 4222 8222
# Sat, 06 Mar 2021 01:00:28 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Sat, 06 Mar 2021 01:00:29 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:ed8ed2aa5d978cf51ebe3454de1832aeb40919052c5cb17d5b63865c31fc03c7`  
		Last Modified: Sat, 06 Mar 2021 01:01:07 GMT  
		Size: 5.2 MB (5246286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.21.1-scratch` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:7fccb492771f9c26f12f03c49e84ba4fb4d7004c6d142f4a7b83337d92feda95
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5170586 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07e817dd7b95371ae514afe3154e4aeba302d94dbed618a0aba7ece8696c13c6`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Sat, 06 Mar 2021 01:51:04 GMT
COPY file:ed938be8d92952afe74223a94317bf582d9bcf2c458a54733da01a37a65d421b in /nats-streaming-server 
# Sat, 06 Mar 2021 01:51:05 GMT
EXPOSE 4222 8222
# Sat, 06 Mar 2021 01:51:06 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Sat, 06 Mar 2021 01:51:07 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:f5ab53e298c8bd7b93e991f4b12e4015cde7d604e6d5ee086e994a86e0556094`  
		Last Modified: Sat, 06 Mar 2021 01:51:46 GMT  
		Size: 5.2 MB (5170586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.21.1-windowsservercore`

```console
$ docker pull nats-streaming@sha256:66bcec534b0a6ed19b5da3dcfda012ddc502d29eebfd14ce18b84e8e72879a30
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1817; amd64
	-	windows version 10.0.14393.4283; amd64

### `nats-streaming:0.21.1-windowsservercore` - windows version 10.0.17763.1817; amd64

```console
$ docker pull nats-streaming@sha256:7c32d8674de2b5a73ba6be51bb6514302b5c28001cb43905c393a60b63302467
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2481844979 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:201caf193f01ab7ea82dbd134d0a0e2fe29e689b1e03dfd0f19f0e397c693db6`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
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
# Wed, 10 Mar 2021 21:47:25 GMT
ENV NATS_STREAMING_SERVER=0.21.1
# Wed, 10 Mar 2021 21:47:26 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.21.1/nats-streaming-server-v0.21.1-windows-amd64.zip
# Wed, 10 Mar 2021 21:47:27 GMT
ENV GIT_DOWNLOAD_SHA256=798ec9b686a8dcb4de93074f416eab067a0896b52ccfc05b65a5e21d55e634e5
# Wed, 10 Mar 2021 21:48:01 GMT
RUN Set-PSDebug -Trace 2
# Wed, 10 Mar 2021 21:49:26 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 10 Mar 2021 21:49:27 GMT
EXPOSE 4222 8222
# Wed, 10 Mar 2021 21:49:28 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 10 Mar 2021 21:49:29 GMT
CMD ["-m" "8222"]
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
	-	`sha256:53877335227f3a676a7b42a4bfe29f3b308e4af725358ddb37e2a44fa6921a80`  
		Last Modified: Wed, 10 Mar 2021 21:54:20 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dded724566db49b2c3de437e8fc07b33da7a82fefc8ee1d6a90ce90bfb721914`  
		Last Modified: Wed, 10 Mar 2021 21:54:20 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55a9876360e291e6db5b15d8903e950e266fac317bbc049509fe3d0380a967ad`  
		Last Modified: Wed, 10 Mar 2021 21:54:20 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b3231bc8381e2d5c4e0ae136f5651b2459e1c4cfb039dc7d04233feace0fb3d`  
		Last Modified: Wed, 10 Mar 2021 21:54:19 GMT  
		Size: 5.1 MB (5064941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71a29a16a4eecc21940d5d0238db4f5e29fdf352f211193dd0d6ddc0a8392dee`  
		Last Modified: Wed, 10 Mar 2021 21:54:35 GMT  
		Size: 15.2 MB (15234342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60e3f696c440330f05de9af154fef7a7668334bfd83a5b6891ece035ed7ec703`  
		Last Modified: Wed, 10 Mar 2021 21:54:17 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ad4ce6f8f2d876a7c5fd7cd6fa233132de5181d550403653062f6ecdc0bd1e5`  
		Last Modified: Wed, 10 Mar 2021 21:54:18 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00a0ea7fcfe009366fde55d37e5932c25b24e3d6d81960f8781f792e143878a2`  
		Last Modified: Wed, 10 Mar 2021 21:54:17 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.21.1-windowsservercore` - windows version 10.0.14393.4283; amd64

```console
$ docker pull nats-streaming@sha256:594f9b8a930c3fbb8aacf7073d6822799c21005df6b94a9f1a3da70a8ef6df2a
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5818554710 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:77a6062b4ea3c0f03780986b01c644987bf4ad33acbf270f345b28aef38775fe`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
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
# Wed, 10 Mar 2021 21:49:49 GMT
ENV NATS_STREAMING_SERVER=0.21.1
# Wed, 10 Mar 2021 21:49:50 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.21.1/nats-streaming-server-v0.21.1-windows-amd64.zip
# Wed, 10 Mar 2021 21:49:51 GMT
ENV GIT_DOWNLOAD_SHA256=798ec9b686a8dcb4de93074f416eab067a0896b52ccfc05b65a5e21d55e634e5
# Wed, 10 Mar 2021 21:51:17 GMT
RUN Set-PSDebug -Trace 2
# Wed, 10 Mar 2021 21:53:25 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 10 Mar 2021 21:53:26 GMT
EXPOSE 4222 8222
# Wed, 10 Mar 2021 21:53:27 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 10 Mar 2021 21:53:28 GMT
CMD ["-m" "8222"]
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
	-	`sha256:3ea87885047b4a1f6a8e0632983da50ba4f31825a69b4f1e13ccb486984dbb81`  
		Last Modified: Wed, 10 Mar 2021 21:55:07 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57acbb65b7dc63351cdcbb771089539683461cd139e5a805bc3f0127181f38b1`  
		Last Modified: Wed, 10 Mar 2021 21:55:07 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5a204c1ad231fc6dfe4d92999bbe0aa9bad4a980ac2f89cdc05255a29a2bb0d`  
		Last Modified: Wed, 10 Mar 2021 21:55:07 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:817aa91f0e76ec219774d8759cba12fd464149e745865ab86ced46d6348f7d7f`  
		Last Modified: Wed, 10 Mar 2021 21:55:06 GMT  
		Size: 5.6 MB (5647336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a811f82bd6b42793f3d47bd0f94e40f0fbb9eefbe192813e03c13c50e897d604`  
		Last Modified: Wed, 10 Mar 2021 21:55:24 GMT  
		Size: 16.0 MB (15985398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba9f62bca657f59242456b4816b9f7ede6deced4cc0c1f90543b33b636084b98`  
		Last Modified: Wed, 10 Mar 2021 21:55:05 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf0ec3239c36380ddf5a7cda6e2fcdd186a3226ea98b17f33b0e083f84d5674e`  
		Last Modified: Wed, 10 Mar 2021 21:55:05 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ae978e2e615d8811e5f542215f7fefa26cdfc9025deee761d653bc3973fda1c`  
		Last Modified: Wed, 10 Mar 2021 21:55:05 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.21.1-windowsservercore-1809`

```console
$ docker pull nats-streaming@sha256:4bcd57606636d40356494deb4e00e85814521e94ea1d39150b42ed55d5da2276
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1817; amd64

### `nats-streaming:0.21.1-windowsservercore-1809` - windows version 10.0.17763.1817; amd64

```console
$ docker pull nats-streaming@sha256:7c32d8674de2b5a73ba6be51bb6514302b5c28001cb43905c393a60b63302467
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2481844979 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:201caf193f01ab7ea82dbd134d0a0e2fe29e689b1e03dfd0f19f0e397c693db6`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
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
# Wed, 10 Mar 2021 21:47:25 GMT
ENV NATS_STREAMING_SERVER=0.21.1
# Wed, 10 Mar 2021 21:47:26 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.21.1/nats-streaming-server-v0.21.1-windows-amd64.zip
# Wed, 10 Mar 2021 21:47:27 GMT
ENV GIT_DOWNLOAD_SHA256=798ec9b686a8dcb4de93074f416eab067a0896b52ccfc05b65a5e21d55e634e5
# Wed, 10 Mar 2021 21:48:01 GMT
RUN Set-PSDebug -Trace 2
# Wed, 10 Mar 2021 21:49:26 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 10 Mar 2021 21:49:27 GMT
EXPOSE 4222 8222
# Wed, 10 Mar 2021 21:49:28 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 10 Mar 2021 21:49:29 GMT
CMD ["-m" "8222"]
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
	-	`sha256:53877335227f3a676a7b42a4bfe29f3b308e4af725358ddb37e2a44fa6921a80`  
		Last Modified: Wed, 10 Mar 2021 21:54:20 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dded724566db49b2c3de437e8fc07b33da7a82fefc8ee1d6a90ce90bfb721914`  
		Last Modified: Wed, 10 Mar 2021 21:54:20 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55a9876360e291e6db5b15d8903e950e266fac317bbc049509fe3d0380a967ad`  
		Last Modified: Wed, 10 Mar 2021 21:54:20 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b3231bc8381e2d5c4e0ae136f5651b2459e1c4cfb039dc7d04233feace0fb3d`  
		Last Modified: Wed, 10 Mar 2021 21:54:19 GMT  
		Size: 5.1 MB (5064941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71a29a16a4eecc21940d5d0238db4f5e29fdf352f211193dd0d6ddc0a8392dee`  
		Last Modified: Wed, 10 Mar 2021 21:54:35 GMT  
		Size: 15.2 MB (15234342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60e3f696c440330f05de9af154fef7a7668334bfd83a5b6891ece035ed7ec703`  
		Last Modified: Wed, 10 Mar 2021 21:54:17 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ad4ce6f8f2d876a7c5fd7cd6fa233132de5181d550403653062f6ecdc0bd1e5`  
		Last Modified: Wed, 10 Mar 2021 21:54:18 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00a0ea7fcfe009366fde55d37e5932c25b24e3d6d81960f8781f792e143878a2`  
		Last Modified: Wed, 10 Mar 2021 21:54:17 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.21.1-windowsservercore-ltsc2016`

```console
$ docker pull nats-streaming@sha256:a79ba4262fcf0cb90e75fab395c2d6dc8126dbc4bfa7bddc82f31cfcd3c25409
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4283; amd64

### `nats-streaming:0.21.1-windowsservercore-ltsc2016` - windows version 10.0.14393.4283; amd64

```console
$ docker pull nats-streaming@sha256:594f9b8a930c3fbb8aacf7073d6822799c21005df6b94a9f1a3da70a8ef6df2a
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5818554710 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:77a6062b4ea3c0f03780986b01c644987bf4ad33acbf270f345b28aef38775fe`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
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
# Wed, 10 Mar 2021 21:49:49 GMT
ENV NATS_STREAMING_SERVER=0.21.1
# Wed, 10 Mar 2021 21:49:50 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.21.1/nats-streaming-server-v0.21.1-windows-amd64.zip
# Wed, 10 Mar 2021 21:49:51 GMT
ENV GIT_DOWNLOAD_SHA256=798ec9b686a8dcb4de93074f416eab067a0896b52ccfc05b65a5e21d55e634e5
# Wed, 10 Mar 2021 21:51:17 GMT
RUN Set-PSDebug -Trace 2
# Wed, 10 Mar 2021 21:53:25 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 10 Mar 2021 21:53:26 GMT
EXPOSE 4222 8222
# Wed, 10 Mar 2021 21:53:27 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 10 Mar 2021 21:53:28 GMT
CMD ["-m" "8222"]
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
	-	`sha256:3ea87885047b4a1f6a8e0632983da50ba4f31825a69b4f1e13ccb486984dbb81`  
		Last Modified: Wed, 10 Mar 2021 21:55:07 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57acbb65b7dc63351cdcbb771089539683461cd139e5a805bc3f0127181f38b1`  
		Last Modified: Wed, 10 Mar 2021 21:55:07 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5a204c1ad231fc6dfe4d92999bbe0aa9bad4a980ac2f89cdc05255a29a2bb0d`  
		Last Modified: Wed, 10 Mar 2021 21:55:07 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:817aa91f0e76ec219774d8759cba12fd464149e745865ab86ced46d6348f7d7f`  
		Last Modified: Wed, 10 Mar 2021 21:55:06 GMT  
		Size: 5.6 MB (5647336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a811f82bd6b42793f3d47bd0f94e40f0fbb9eefbe192813e03c13c50e897d604`  
		Last Modified: Wed, 10 Mar 2021 21:55:24 GMT  
		Size: 16.0 MB (15985398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba9f62bca657f59242456b4816b9f7ede6deced4cc0c1f90543b33b636084b98`  
		Last Modified: Wed, 10 Mar 2021 21:55:05 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf0ec3239c36380ddf5a7cda6e2fcdd186a3226ea98b17f33b0e083f84d5674e`  
		Last Modified: Wed, 10 Mar 2021 21:55:05 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ae978e2e615d8811e5f542215f7fefa26cdfc9025deee761d653bc3973fda1c`  
		Last Modified: Wed, 10 Mar 2021 21:55:05 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:alpine`

```console
$ docker pull nats-streaming@sha256:9d1c10a7c73c7bf354e12a1c24620e4020a5f81d3cb06ff73316305558ebf83f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:alpine` - linux; amd64

```console
$ docker pull nats-streaming@sha256:3ff85e83ddea77c39183aed2eae77d09809eeecbfd51aa8e8ab2cc3ca136a0db
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.8 MB (8774557 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:012e69812f1330d74532543e68955276fbb8390f06a1c627873fbfd88ec23f3c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Thu, 25 Mar 2021 22:19:32 GMT
ADD file:6b081cabb4b256ee07587d249c4989b5b679375529542b81550a65b6f19f274e in / 
# Thu, 25 Mar 2021 22:19:32 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 08:12:03 GMT
ENV NATS_STREAMING_SERVER=0.21.1
# Fri, 26 Mar 2021 08:12:06 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='06d591a61084aab1046e818486c2ee7c3936214c92dc257084693d6ffe06342b' ;; 		armhf) natsArch='arm6'; sha256='085375782abe1bacbd6fc609ce6a6721f029cba312733479204c89bf92f1e188' ;; 		armv7) natsArch='arm7'; sha256='947d91512b47ba98198bef7f799670c40cf6949f2ba2e98b5c133e6166e9b97c' ;; 		x86_64) natsArch='amd64'; sha256='85fd7fd3c7b71cbc9043900f9110b028f1fdc042c6500eed065e6e2c3331f62e' ;; 		x86) natsArch='386'; sha256='475b0f015726af99c9ea779c8bbbeaa729ef90f43dd2715273fea81fb90ea63a' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 26 Mar 2021 08:12:06 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Fri, 26 Mar 2021 08:12:06 GMT
EXPOSE 4222 8222
# Fri, 26 Mar 2021 08:12:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 08:12:07 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:9aae54b2144e5b2b00c610f8805128f4f86822e1e52d3714c463744a431f0f4a`  
		Last Modified: Thu, 25 Mar 2021 22:20:18 GMT  
		Size: 2.8 MB (2811681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f43604faee33fd935c231c8add7a2f9f6d33712dc31de6ae1e1fde55fbbcb83`  
		Last Modified: Fri, 26 Mar 2021 08:12:37 GMT  
		Size: 6.0 MB (5962455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:173cba00661220a72d7a394a5993bdc17325ab50875040ecc6eb5bc6dc8e65c9`  
		Last Modified: Fri, 26 Mar 2021 08:12:36 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:19373a83f61771319d0aacfab1086d496a2dd1535970f8a20652d56cf2b7578e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.2 MB (8156412 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:935ff18ff1bfcc7d421f422b0d98ef2b111e05c4e09b1e57aef68d71b18156b9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Thu, 25 Mar 2021 22:50:09 GMT
ADD file:ca4136238cb9a01d079efd129bccd1470945d7d4320da61373af90645a4b1146 in / 
# Thu, 25 Mar 2021 22:50:28 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 05:57:34 GMT
ENV NATS_STREAMING_SERVER=0.21.1
# Fri, 26 Mar 2021 05:57:41 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='06d591a61084aab1046e818486c2ee7c3936214c92dc257084693d6ffe06342b' ;; 		armhf) natsArch='arm6'; sha256='085375782abe1bacbd6fc609ce6a6721f029cba312733479204c89bf92f1e188' ;; 		armv7) natsArch='arm7'; sha256='947d91512b47ba98198bef7f799670c40cf6949f2ba2e98b5c133e6166e9b97c' ;; 		x86_64) natsArch='amd64'; sha256='85fd7fd3c7b71cbc9043900f9110b028f1fdc042c6500eed065e6e2c3331f62e' ;; 		x86) natsArch='386'; sha256='475b0f015726af99c9ea779c8bbbeaa729ef90f43dd2715273fea81fb90ea63a' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 26 Mar 2021 05:57:42 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Fri, 26 Mar 2021 05:57:43 GMT
EXPOSE 4222 8222
# Fri, 26 Mar 2021 05:57:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 05:57:46 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:bca6a70a54896d072b6919d2ae18d3ef685bc7aed783731f68a4adac0fb93d52`  
		Last Modified: Thu, 25 Mar 2021 22:54:24 GMT  
		Size: 2.6 MB (2622062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37dde547b7fced1153630086dee787892a218966ea430c2964f55f72bcbbf83a`  
		Last Modified: Fri, 26 Mar 2021 05:58:16 GMT  
		Size: 5.5 MB (5533929 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df980303a7fb93b8683964b371b30ef03ef35e26de48621d858290228f8b3346`  
		Last Modified: Fri, 26 Mar 2021 05:58:14 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:f167b7ef1b6e893d3e176ad7fd41597e8a4da3720d0694b407e19e24b68cd5f6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.0 MB (7951584 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e033b7fa5e49122eff8379884102467952cb9d40190588eee42fd608ecbfe3d9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Thu, 25 Mar 2021 22:05:53 GMT
ADD file:44ef6cff6e7d37a67c5846eb792fec65025702c00c56ff96801ac79bf81b0cc3 in / 
# Thu, 25 Mar 2021 22:05:55 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 01:51:55 GMT
ENV NATS_STREAMING_SERVER=0.21.1
# Fri, 26 Mar 2021 01:52:03 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='06d591a61084aab1046e818486c2ee7c3936214c92dc257084693d6ffe06342b' ;; 		armhf) natsArch='arm6'; sha256='085375782abe1bacbd6fc609ce6a6721f029cba312733479204c89bf92f1e188' ;; 		armv7) natsArch='arm7'; sha256='947d91512b47ba98198bef7f799670c40cf6949f2ba2e98b5c133e6166e9b97c' ;; 		x86_64) natsArch='amd64'; sha256='85fd7fd3c7b71cbc9043900f9110b028f1fdc042c6500eed065e6e2c3331f62e' ;; 		x86) natsArch='386'; sha256='475b0f015726af99c9ea779c8bbbeaa729ef90f43dd2715273fea81fb90ea63a' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 26 Mar 2021 01:52:05 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Fri, 26 Mar 2021 01:52:11 GMT
EXPOSE 4222 8222
# Fri, 26 Mar 2021 01:52:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 01:52:14 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:6c1162af251f0d5ab4945f8506f3265b86d0a03cda37f703c2446a71a233bc20`  
		Last Modified: Thu, 25 Mar 2021 22:07:21 GMT  
		Size: 2.4 MB (2423999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61ca624cfb490a8a9fb48110381475a59604ddfd4920f6496398a887f8a37b73`  
		Last Modified: Fri, 26 Mar 2021 01:52:52 GMT  
		Size: 5.5 MB (5527163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3957a11b701f02a3361d365cd9b9c63fcafa89f362a40471a527bb31bbbe1de6`  
		Last Modified: Fri, 26 Mar 2021 01:52:50 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:1740e224df015e33133a9db91519ebc8601bf64861cde979a2ed6c556b649395
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.2 MB (8164487 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:205e781a3be342b949194bab8b6fde3763da1876fe7fac88af8efa1a07b3f204`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 17 Feb 2021 20:39:29 GMT
ADD file:3bf1497bd250cf7c73c12231dc4ebe3a3a67f2cd99e35bce47ef6674683aeb1d in / 
# Wed, 17 Feb 2021 20:39:30 GMT
CMD ["/bin/sh"]
# Sat, 06 Mar 2021 01:46:28 GMT
ENV NATS_STREAMING_SERVER=0.21.1
# Sat, 06 Mar 2021 01:46:33 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='06d591a61084aab1046e818486c2ee7c3936214c92dc257084693d6ffe06342b' ;; 		armhf) natsArch='arm6'; sha256='085375782abe1bacbd6fc609ce6a6721f029cba312733479204c89bf92f1e188' ;; 		armv7) natsArch='arm7'; sha256='947d91512b47ba98198bef7f799670c40cf6949f2ba2e98b5c133e6166e9b97c' ;; 		x86_64) natsArch='amd64'; sha256='85fd7fd3c7b71cbc9043900f9110b028f1fdc042c6500eed065e6e2c3331f62e' ;; 		x86) natsArch='386'; sha256='475b0f015726af99c9ea779c8bbbeaa729ef90f43dd2715273fea81fb90ea63a' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Sat, 06 Mar 2021 01:46:33 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Sat, 06 Mar 2021 01:46:34 GMT
EXPOSE 4222 8222
# Sat, 06 Mar 2021 01:46:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 06 Mar 2021 01:46:35 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:069a56d6d07f6b186fbb82e4486616b9be9a37ce32a63013af6cddcb65898182`  
		Last Modified: Wed, 17 Feb 2021 20:40:04 GMT  
		Size: 2.7 MB (2711572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e334db32136252e9605e0a6ef0426e8c0c50e757bb238a24330339d3dedbe84`  
		Last Modified: Sat, 06 Mar 2021 01:51:34 GMT  
		Size: 5.5 MB (5452492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7e903d8d08305b07378aef2e8c19af9f0d6b899ce053c33e5b6022c07b155e2`  
		Last Modified: Sat, 06 Mar 2021 01:51:32 GMT  
		Size: 423.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:alpine3.13`

```console
$ docker pull nats-streaming@sha256:9d1c10a7c73c7bf354e12a1c24620e4020a5f81d3cb06ff73316305558ebf83f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:alpine3.13` - linux; amd64

```console
$ docker pull nats-streaming@sha256:3ff85e83ddea77c39183aed2eae77d09809eeecbfd51aa8e8ab2cc3ca136a0db
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.8 MB (8774557 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:012e69812f1330d74532543e68955276fbb8390f06a1c627873fbfd88ec23f3c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Thu, 25 Mar 2021 22:19:32 GMT
ADD file:6b081cabb4b256ee07587d249c4989b5b679375529542b81550a65b6f19f274e in / 
# Thu, 25 Mar 2021 22:19:32 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 08:12:03 GMT
ENV NATS_STREAMING_SERVER=0.21.1
# Fri, 26 Mar 2021 08:12:06 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='06d591a61084aab1046e818486c2ee7c3936214c92dc257084693d6ffe06342b' ;; 		armhf) natsArch='arm6'; sha256='085375782abe1bacbd6fc609ce6a6721f029cba312733479204c89bf92f1e188' ;; 		armv7) natsArch='arm7'; sha256='947d91512b47ba98198bef7f799670c40cf6949f2ba2e98b5c133e6166e9b97c' ;; 		x86_64) natsArch='amd64'; sha256='85fd7fd3c7b71cbc9043900f9110b028f1fdc042c6500eed065e6e2c3331f62e' ;; 		x86) natsArch='386'; sha256='475b0f015726af99c9ea779c8bbbeaa729ef90f43dd2715273fea81fb90ea63a' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 26 Mar 2021 08:12:06 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Fri, 26 Mar 2021 08:12:06 GMT
EXPOSE 4222 8222
# Fri, 26 Mar 2021 08:12:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 08:12:07 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:9aae54b2144e5b2b00c610f8805128f4f86822e1e52d3714c463744a431f0f4a`  
		Last Modified: Thu, 25 Mar 2021 22:20:18 GMT  
		Size: 2.8 MB (2811681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f43604faee33fd935c231c8add7a2f9f6d33712dc31de6ae1e1fde55fbbcb83`  
		Last Modified: Fri, 26 Mar 2021 08:12:37 GMT  
		Size: 6.0 MB (5962455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:173cba00661220a72d7a394a5993bdc17325ab50875040ecc6eb5bc6dc8e65c9`  
		Last Modified: Fri, 26 Mar 2021 08:12:36 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine3.13` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:19373a83f61771319d0aacfab1086d496a2dd1535970f8a20652d56cf2b7578e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.2 MB (8156412 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:935ff18ff1bfcc7d421f422b0d98ef2b111e05c4e09b1e57aef68d71b18156b9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Thu, 25 Mar 2021 22:50:09 GMT
ADD file:ca4136238cb9a01d079efd129bccd1470945d7d4320da61373af90645a4b1146 in / 
# Thu, 25 Mar 2021 22:50:28 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 05:57:34 GMT
ENV NATS_STREAMING_SERVER=0.21.1
# Fri, 26 Mar 2021 05:57:41 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='06d591a61084aab1046e818486c2ee7c3936214c92dc257084693d6ffe06342b' ;; 		armhf) natsArch='arm6'; sha256='085375782abe1bacbd6fc609ce6a6721f029cba312733479204c89bf92f1e188' ;; 		armv7) natsArch='arm7'; sha256='947d91512b47ba98198bef7f799670c40cf6949f2ba2e98b5c133e6166e9b97c' ;; 		x86_64) natsArch='amd64'; sha256='85fd7fd3c7b71cbc9043900f9110b028f1fdc042c6500eed065e6e2c3331f62e' ;; 		x86) natsArch='386'; sha256='475b0f015726af99c9ea779c8bbbeaa729ef90f43dd2715273fea81fb90ea63a' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 26 Mar 2021 05:57:42 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Fri, 26 Mar 2021 05:57:43 GMT
EXPOSE 4222 8222
# Fri, 26 Mar 2021 05:57:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 05:57:46 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:bca6a70a54896d072b6919d2ae18d3ef685bc7aed783731f68a4adac0fb93d52`  
		Last Modified: Thu, 25 Mar 2021 22:54:24 GMT  
		Size: 2.6 MB (2622062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37dde547b7fced1153630086dee787892a218966ea430c2964f55f72bcbbf83a`  
		Last Modified: Fri, 26 Mar 2021 05:58:16 GMT  
		Size: 5.5 MB (5533929 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df980303a7fb93b8683964b371b30ef03ef35e26de48621d858290228f8b3346`  
		Last Modified: Fri, 26 Mar 2021 05:58:14 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine3.13` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:f167b7ef1b6e893d3e176ad7fd41597e8a4da3720d0694b407e19e24b68cd5f6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.0 MB (7951584 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e033b7fa5e49122eff8379884102467952cb9d40190588eee42fd608ecbfe3d9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Thu, 25 Mar 2021 22:05:53 GMT
ADD file:44ef6cff6e7d37a67c5846eb792fec65025702c00c56ff96801ac79bf81b0cc3 in / 
# Thu, 25 Mar 2021 22:05:55 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 01:51:55 GMT
ENV NATS_STREAMING_SERVER=0.21.1
# Fri, 26 Mar 2021 01:52:03 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='06d591a61084aab1046e818486c2ee7c3936214c92dc257084693d6ffe06342b' ;; 		armhf) natsArch='arm6'; sha256='085375782abe1bacbd6fc609ce6a6721f029cba312733479204c89bf92f1e188' ;; 		armv7) natsArch='arm7'; sha256='947d91512b47ba98198bef7f799670c40cf6949f2ba2e98b5c133e6166e9b97c' ;; 		x86_64) natsArch='amd64'; sha256='85fd7fd3c7b71cbc9043900f9110b028f1fdc042c6500eed065e6e2c3331f62e' ;; 		x86) natsArch='386'; sha256='475b0f015726af99c9ea779c8bbbeaa729ef90f43dd2715273fea81fb90ea63a' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 26 Mar 2021 01:52:05 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Fri, 26 Mar 2021 01:52:11 GMT
EXPOSE 4222 8222
# Fri, 26 Mar 2021 01:52:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 01:52:14 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:6c1162af251f0d5ab4945f8506f3265b86d0a03cda37f703c2446a71a233bc20`  
		Last Modified: Thu, 25 Mar 2021 22:07:21 GMT  
		Size: 2.4 MB (2423999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61ca624cfb490a8a9fb48110381475a59604ddfd4920f6496398a887f8a37b73`  
		Last Modified: Fri, 26 Mar 2021 01:52:52 GMT  
		Size: 5.5 MB (5527163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3957a11b701f02a3361d365cd9b9c63fcafa89f362a40471a527bb31bbbe1de6`  
		Last Modified: Fri, 26 Mar 2021 01:52:50 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine3.13` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:1740e224df015e33133a9db91519ebc8601bf64861cde979a2ed6c556b649395
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.2 MB (8164487 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:205e781a3be342b949194bab8b6fde3763da1876fe7fac88af8efa1a07b3f204`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 17 Feb 2021 20:39:29 GMT
ADD file:3bf1497bd250cf7c73c12231dc4ebe3a3a67f2cd99e35bce47ef6674683aeb1d in / 
# Wed, 17 Feb 2021 20:39:30 GMT
CMD ["/bin/sh"]
# Sat, 06 Mar 2021 01:46:28 GMT
ENV NATS_STREAMING_SERVER=0.21.1
# Sat, 06 Mar 2021 01:46:33 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='06d591a61084aab1046e818486c2ee7c3936214c92dc257084693d6ffe06342b' ;; 		armhf) natsArch='arm6'; sha256='085375782abe1bacbd6fc609ce6a6721f029cba312733479204c89bf92f1e188' ;; 		armv7) natsArch='arm7'; sha256='947d91512b47ba98198bef7f799670c40cf6949f2ba2e98b5c133e6166e9b97c' ;; 		x86_64) natsArch='amd64'; sha256='85fd7fd3c7b71cbc9043900f9110b028f1fdc042c6500eed065e6e2c3331f62e' ;; 		x86) natsArch='386'; sha256='475b0f015726af99c9ea779c8bbbeaa729ef90f43dd2715273fea81fb90ea63a' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Sat, 06 Mar 2021 01:46:33 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Sat, 06 Mar 2021 01:46:34 GMT
EXPOSE 4222 8222
# Sat, 06 Mar 2021 01:46:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 06 Mar 2021 01:46:35 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:069a56d6d07f6b186fbb82e4486616b9be9a37ce32a63013af6cddcb65898182`  
		Last Modified: Wed, 17 Feb 2021 20:40:04 GMT  
		Size: 2.7 MB (2711572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e334db32136252e9605e0a6ef0426e8c0c50e757bb238a24330339d3dedbe84`  
		Last Modified: Sat, 06 Mar 2021 01:51:34 GMT  
		Size: 5.5 MB (5452492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7e903d8d08305b07378aef2e8c19af9f0d6b899ce053c33e5b6022c07b155e2`  
		Last Modified: Sat, 06 Mar 2021 01:51:32 GMT  
		Size: 423.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:latest`

```console
$ docker pull nats-streaming@sha256:42dd817d3798a2288a0dfbd2a8f520b497ff170316f38a13c4d09f2be70f4e99
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.1817; amd64

### `nats-streaming:latest` - linux; amd64

```console
$ docker pull nats-streaming@sha256:aa6af76760541ce71d366ac25554ad7caa95aea8cd230dd2688fd76b0645b329
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.7 MB (5680474 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31671965fc8e3e2d623279516e43fd9d1a5d8d82a19fe709c69d7bfe7ac50085`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Sat, 06 Mar 2021 07:43:28 GMT
COPY file:2c21a07cd43acfd157f86c6cf727430cf07e201a3bf3668b2083f473385db991 in /nats-streaming-server 
# Sat, 06 Mar 2021 07:43:28 GMT
EXPOSE 4222 8222
# Sat, 06 Mar 2021 07:43:29 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Sat, 06 Mar 2021 07:43:29 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:6f1c3ed40f752c2108b0e5d9224fba83d5045dac3370f93a50d91af0bc201c05`  
		Last Modified: Sat, 06 Mar 2021 07:44:17 GMT  
		Size: 5.7 MB (5680474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:latest` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:907a450228b0d46339c5af803a9475165f7cfd9d20d5e09e8f66f9d048d1f7b9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.3 MB (5252895 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8c6d73cc983f6821e57de28a32cec901f28d3c5ada68aa9e71a1880962a9f07`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Sat, 06 Mar 2021 02:10:29 GMT
COPY file:bd617234b457ddee67b99f0e411029c6d5badad5059fbd81239c0acfe92cd4b7 in /nats-streaming-server 
# Sat, 06 Mar 2021 02:10:30 GMT
EXPOSE 4222 8222
# Sat, 06 Mar 2021 02:10:31 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Sat, 06 Mar 2021 02:10:31 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:ef1f32aa7a9ce9c8d42c909d32f61dabfa957c0b6a2b3590cd5e5847fb634355`  
		Last Modified: Sat, 06 Mar 2021 02:11:15 GMT  
		Size: 5.3 MB (5252895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:latest` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:ae774aee41bd64306207d739d2290639f673c9c66c367a83f155a923fe8c13f6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5246286 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ce52186dd957f6b70b086fdcbc8212e079e5ed5e3e0013f8f72b3922535a56e`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Sat, 06 Mar 2021 01:00:25 GMT
COPY file:546c18b3e8e91d453d1a325c6e4dbc3c945564c010676da1abe89a653a0dea84 in /nats-streaming-server 
# Sat, 06 Mar 2021 01:00:27 GMT
EXPOSE 4222 8222
# Sat, 06 Mar 2021 01:00:28 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Sat, 06 Mar 2021 01:00:29 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:ed8ed2aa5d978cf51ebe3454de1832aeb40919052c5cb17d5b63865c31fc03c7`  
		Last Modified: Sat, 06 Mar 2021 01:01:07 GMT  
		Size: 5.2 MB (5246286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:latest` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:7fccb492771f9c26f12f03c49e84ba4fb4d7004c6d142f4a7b83337d92feda95
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5170586 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07e817dd7b95371ae514afe3154e4aeba302d94dbed618a0aba7ece8696c13c6`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Sat, 06 Mar 2021 01:51:04 GMT
COPY file:ed938be8d92952afe74223a94317bf582d9bcf2c458a54733da01a37a65d421b in /nats-streaming-server 
# Sat, 06 Mar 2021 01:51:05 GMT
EXPOSE 4222 8222
# Sat, 06 Mar 2021 01:51:06 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Sat, 06 Mar 2021 01:51:07 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:f5ab53e298c8bd7b93e991f4b12e4015cde7d604e6d5ee086e994a86e0556094`  
		Last Modified: Sat, 06 Mar 2021 01:51:46 GMT  
		Size: 5.2 MB (5170586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:latest` - windows version 10.0.17763.1817; amd64

```console
$ docker pull nats-streaming@sha256:b1027771e781ed856534f3ee9d9fc845e0a08d4ac903949056fa3613a1025713
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.2 MB (107205225 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:034c288a390667cc8689271b4c68b1f38eb2887a9931320f9fea3cd6cdb28dfb`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Fri, 26 Feb 2021 16:47:31 GMT
RUN Apply image 1809-amd64
# Wed, 10 Mar 2021 16:56:55 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 10 Mar 2021 21:49:39 GMT
RUN cmd /S /C #(nop) COPY file:189ca6af047e9f9cf54ab2176b48588e01c7497fe0b5b0d7b2614ebad66ed089 in C:\nats-streaming-server.exe 
# Wed, 10 Mar 2021 21:49:40 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 10 Mar 2021 21:49:41 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 10 Mar 2021 21:49:42 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:a11c4ca8f1ba16b6e1395d4523be2215bd0871c2e3e4695b9f2b87bd7472be52`  
		Size: 101.4 MB (101389964 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f49969195f32b7e40a81e3d189259fec7ebf52ee0ec5dafd5f3f288715354fed`  
		Last Modified: Wed, 10 Mar 2021 17:01:57 GMT  
		Size: 1.0 KB (1047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d5345eab816862154342d0ef80781aae11144d15f84ad4ac1d5ed1bbf9b083e`  
		Last Modified: Wed, 10 Mar 2021 21:54:51 GMT  
		Size: 5.8 MB (5810691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d886b78bda0fe938d4c7e8a21e511102e719280871d97e9e7b3d4589222dffd`  
		Last Modified: Wed, 10 Mar 2021 21:54:51 GMT  
		Size: 1.2 KB (1180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3fce35e6d75d0e8ea6539c3a0e1f335dec61dfabde67c34ec07260f715ea526`  
		Last Modified: Wed, 10 Mar 2021 21:54:50 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b95ed8adcfdc36bcc766c7ca9db14a0bca9768321cc35854aa2d896ef75ea4ab`  
		Last Modified: Wed, 10 Mar 2021 21:54:49 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:linux`

```console
$ docker pull nats-streaming@sha256:26603f9112b727df8e9736407a1ec1ab031317a9f6964ba0d407baea6b8d152c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:linux` - linux; amd64

```console
$ docker pull nats-streaming@sha256:aa6af76760541ce71d366ac25554ad7caa95aea8cd230dd2688fd76b0645b329
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.7 MB (5680474 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31671965fc8e3e2d623279516e43fd9d1a5d8d82a19fe709c69d7bfe7ac50085`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Sat, 06 Mar 2021 07:43:28 GMT
COPY file:2c21a07cd43acfd157f86c6cf727430cf07e201a3bf3668b2083f473385db991 in /nats-streaming-server 
# Sat, 06 Mar 2021 07:43:28 GMT
EXPOSE 4222 8222
# Sat, 06 Mar 2021 07:43:29 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Sat, 06 Mar 2021 07:43:29 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:6f1c3ed40f752c2108b0e5d9224fba83d5045dac3370f93a50d91af0bc201c05`  
		Last Modified: Sat, 06 Mar 2021 07:44:17 GMT  
		Size: 5.7 MB (5680474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:linux` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:907a450228b0d46339c5af803a9475165f7cfd9d20d5e09e8f66f9d048d1f7b9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.3 MB (5252895 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8c6d73cc983f6821e57de28a32cec901f28d3c5ada68aa9e71a1880962a9f07`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Sat, 06 Mar 2021 02:10:29 GMT
COPY file:bd617234b457ddee67b99f0e411029c6d5badad5059fbd81239c0acfe92cd4b7 in /nats-streaming-server 
# Sat, 06 Mar 2021 02:10:30 GMT
EXPOSE 4222 8222
# Sat, 06 Mar 2021 02:10:31 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Sat, 06 Mar 2021 02:10:31 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:ef1f32aa7a9ce9c8d42c909d32f61dabfa957c0b6a2b3590cd5e5847fb634355`  
		Last Modified: Sat, 06 Mar 2021 02:11:15 GMT  
		Size: 5.3 MB (5252895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:linux` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:ae774aee41bd64306207d739d2290639f673c9c66c367a83f155a923fe8c13f6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5246286 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ce52186dd957f6b70b086fdcbc8212e079e5ed5e3e0013f8f72b3922535a56e`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Sat, 06 Mar 2021 01:00:25 GMT
COPY file:546c18b3e8e91d453d1a325c6e4dbc3c945564c010676da1abe89a653a0dea84 in /nats-streaming-server 
# Sat, 06 Mar 2021 01:00:27 GMT
EXPOSE 4222 8222
# Sat, 06 Mar 2021 01:00:28 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Sat, 06 Mar 2021 01:00:29 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:ed8ed2aa5d978cf51ebe3454de1832aeb40919052c5cb17d5b63865c31fc03c7`  
		Last Modified: Sat, 06 Mar 2021 01:01:07 GMT  
		Size: 5.2 MB (5246286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:linux` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:7fccb492771f9c26f12f03c49e84ba4fb4d7004c6d142f4a7b83337d92feda95
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5170586 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07e817dd7b95371ae514afe3154e4aeba302d94dbed618a0aba7ece8696c13c6`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Sat, 06 Mar 2021 01:51:04 GMT
COPY file:ed938be8d92952afe74223a94317bf582d9bcf2c458a54733da01a37a65d421b in /nats-streaming-server 
# Sat, 06 Mar 2021 01:51:05 GMT
EXPOSE 4222 8222
# Sat, 06 Mar 2021 01:51:06 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Sat, 06 Mar 2021 01:51:07 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:f5ab53e298c8bd7b93e991f4b12e4015cde7d604e6d5ee086e994a86e0556094`  
		Last Modified: Sat, 06 Mar 2021 01:51:46 GMT  
		Size: 5.2 MB (5170586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:nanoserver`

```console
$ docker pull nats-streaming@sha256:87d3bbcab917eb6d04e19e5623d88b465ff072b603fa498c4b7299035fbdf1e7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1817; amd64

### `nats-streaming:nanoserver` - windows version 10.0.17763.1817; amd64

```console
$ docker pull nats-streaming@sha256:b1027771e781ed856534f3ee9d9fc845e0a08d4ac903949056fa3613a1025713
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.2 MB (107205225 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:034c288a390667cc8689271b4c68b1f38eb2887a9931320f9fea3cd6cdb28dfb`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Fri, 26 Feb 2021 16:47:31 GMT
RUN Apply image 1809-amd64
# Wed, 10 Mar 2021 16:56:55 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 10 Mar 2021 21:49:39 GMT
RUN cmd /S /C #(nop) COPY file:189ca6af047e9f9cf54ab2176b48588e01c7497fe0b5b0d7b2614ebad66ed089 in C:\nats-streaming-server.exe 
# Wed, 10 Mar 2021 21:49:40 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 10 Mar 2021 21:49:41 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 10 Mar 2021 21:49:42 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:a11c4ca8f1ba16b6e1395d4523be2215bd0871c2e3e4695b9f2b87bd7472be52`  
		Size: 101.4 MB (101389964 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f49969195f32b7e40a81e3d189259fec7ebf52ee0ec5dafd5f3f288715354fed`  
		Last Modified: Wed, 10 Mar 2021 17:01:57 GMT  
		Size: 1.0 KB (1047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d5345eab816862154342d0ef80781aae11144d15f84ad4ac1d5ed1bbf9b083e`  
		Last Modified: Wed, 10 Mar 2021 21:54:51 GMT  
		Size: 5.8 MB (5810691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d886b78bda0fe938d4c7e8a21e511102e719280871d97e9e7b3d4589222dffd`  
		Last Modified: Wed, 10 Mar 2021 21:54:51 GMT  
		Size: 1.2 KB (1180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3fce35e6d75d0e8ea6539c3a0e1f335dec61dfabde67c34ec07260f715ea526`  
		Last Modified: Wed, 10 Mar 2021 21:54:50 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b95ed8adcfdc36bcc766c7ca9db14a0bca9768321cc35854aa2d896ef75ea4ab`  
		Last Modified: Wed, 10 Mar 2021 21:54:49 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:nanoserver-1809`

```console
$ docker pull nats-streaming@sha256:87d3bbcab917eb6d04e19e5623d88b465ff072b603fa498c4b7299035fbdf1e7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1817; amd64

### `nats-streaming:nanoserver-1809` - windows version 10.0.17763.1817; amd64

```console
$ docker pull nats-streaming@sha256:b1027771e781ed856534f3ee9d9fc845e0a08d4ac903949056fa3613a1025713
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.2 MB (107205225 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:034c288a390667cc8689271b4c68b1f38eb2887a9931320f9fea3cd6cdb28dfb`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Fri, 26 Feb 2021 16:47:31 GMT
RUN Apply image 1809-amd64
# Wed, 10 Mar 2021 16:56:55 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 10 Mar 2021 21:49:39 GMT
RUN cmd /S /C #(nop) COPY file:189ca6af047e9f9cf54ab2176b48588e01c7497fe0b5b0d7b2614ebad66ed089 in C:\nats-streaming-server.exe 
# Wed, 10 Mar 2021 21:49:40 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 10 Mar 2021 21:49:41 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 10 Mar 2021 21:49:42 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:a11c4ca8f1ba16b6e1395d4523be2215bd0871c2e3e4695b9f2b87bd7472be52`  
		Size: 101.4 MB (101389964 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f49969195f32b7e40a81e3d189259fec7ebf52ee0ec5dafd5f3f288715354fed`  
		Last Modified: Wed, 10 Mar 2021 17:01:57 GMT  
		Size: 1.0 KB (1047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d5345eab816862154342d0ef80781aae11144d15f84ad4ac1d5ed1bbf9b083e`  
		Last Modified: Wed, 10 Mar 2021 21:54:51 GMT  
		Size: 5.8 MB (5810691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d886b78bda0fe938d4c7e8a21e511102e719280871d97e9e7b3d4589222dffd`  
		Last Modified: Wed, 10 Mar 2021 21:54:51 GMT  
		Size: 1.2 KB (1180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3fce35e6d75d0e8ea6539c3a0e1f335dec61dfabde67c34ec07260f715ea526`  
		Last Modified: Wed, 10 Mar 2021 21:54:50 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b95ed8adcfdc36bcc766c7ca9db14a0bca9768321cc35854aa2d896ef75ea4ab`  
		Last Modified: Wed, 10 Mar 2021 21:54:49 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:scratch`

```console
$ docker pull nats-streaming@sha256:26603f9112b727df8e9736407a1ec1ab031317a9f6964ba0d407baea6b8d152c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:scratch` - linux; amd64

```console
$ docker pull nats-streaming@sha256:aa6af76760541ce71d366ac25554ad7caa95aea8cd230dd2688fd76b0645b329
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.7 MB (5680474 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31671965fc8e3e2d623279516e43fd9d1a5d8d82a19fe709c69d7bfe7ac50085`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Sat, 06 Mar 2021 07:43:28 GMT
COPY file:2c21a07cd43acfd157f86c6cf727430cf07e201a3bf3668b2083f473385db991 in /nats-streaming-server 
# Sat, 06 Mar 2021 07:43:28 GMT
EXPOSE 4222 8222
# Sat, 06 Mar 2021 07:43:29 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Sat, 06 Mar 2021 07:43:29 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:6f1c3ed40f752c2108b0e5d9224fba83d5045dac3370f93a50d91af0bc201c05`  
		Last Modified: Sat, 06 Mar 2021 07:44:17 GMT  
		Size: 5.7 MB (5680474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:scratch` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:907a450228b0d46339c5af803a9475165f7cfd9d20d5e09e8f66f9d048d1f7b9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.3 MB (5252895 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8c6d73cc983f6821e57de28a32cec901f28d3c5ada68aa9e71a1880962a9f07`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Sat, 06 Mar 2021 02:10:29 GMT
COPY file:bd617234b457ddee67b99f0e411029c6d5badad5059fbd81239c0acfe92cd4b7 in /nats-streaming-server 
# Sat, 06 Mar 2021 02:10:30 GMT
EXPOSE 4222 8222
# Sat, 06 Mar 2021 02:10:31 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Sat, 06 Mar 2021 02:10:31 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:ef1f32aa7a9ce9c8d42c909d32f61dabfa957c0b6a2b3590cd5e5847fb634355`  
		Last Modified: Sat, 06 Mar 2021 02:11:15 GMT  
		Size: 5.3 MB (5252895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:scratch` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:ae774aee41bd64306207d739d2290639f673c9c66c367a83f155a923fe8c13f6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5246286 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ce52186dd957f6b70b086fdcbc8212e079e5ed5e3e0013f8f72b3922535a56e`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Sat, 06 Mar 2021 01:00:25 GMT
COPY file:546c18b3e8e91d453d1a325c6e4dbc3c945564c010676da1abe89a653a0dea84 in /nats-streaming-server 
# Sat, 06 Mar 2021 01:00:27 GMT
EXPOSE 4222 8222
# Sat, 06 Mar 2021 01:00:28 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Sat, 06 Mar 2021 01:00:29 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:ed8ed2aa5d978cf51ebe3454de1832aeb40919052c5cb17d5b63865c31fc03c7`  
		Last Modified: Sat, 06 Mar 2021 01:01:07 GMT  
		Size: 5.2 MB (5246286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:scratch` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:7fccb492771f9c26f12f03c49e84ba4fb4d7004c6d142f4a7b83337d92feda95
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5170586 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07e817dd7b95371ae514afe3154e4aeba302d94dbed618a0aba7ece8696c13c6`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Sat, 06 Mar 2021 01:51:04 GMT
COPY file:ed938be8d92952afe74223a94317bf582d9bcf2c458a54733da01a37a65d421b in /nats-streaming-server 
# Sat, 06 Mar 2021 01:51:05 GMT
EXPOSE 4222 8222
# Sat, 06 Mar 2021 01:51:06 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Sat, 06 Mar 2021 01:51:07 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:f5ab53e298c8bd7b93e991f4b12e4015cde7d604e6d5ee086e994a86e0556094`  
		Last Modified: Sat, 06 Mar 2021 01:51:46 GMT  
		Size: 5.2 MB (5170586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:windowsservercore`

```console
$ docker pull nats-streaming@sha256:66bcec534b0a6ed19b5da3dcfda012ddc502d29eebfd14ce18b84e8e72879a30
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1817; amd64
	-	windows version 10.0.14393.4283; amd64

### `nats-streaming:windowsservercore` - windows version 10.0.17763.1817; amd64

```console
$ docker pull nats-streaming@sha256:7c32d8674de2b5a73ba6be51bb6514302b5c28001cb43905c393a60b63302467
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2481844979 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:201caf193f01ab7ea82dbd134d0a0e2fe29e689b1e03dfd0f19f0e397c693db6`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
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
# Wed, 10 Mar 2021 21:47:25 GMT
ENV NATS_STREAMING_SERVER=0.21.1
# Wed, 10 Mar 2021 21:47:26 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.21.1/nats-streaming-server-v0.21.1-windows-amd64.zip
# Wed, 10 Mar 2021 21:47:27 GMT
ENV GIT_DOWNLOAD_SHA256=798ec9b686a8dcb4de93074f416eab067a0896b52ccfc05b65a5e21d55e634e5
# Wed, 10 Mar 2021 21:48:01 GMT
RUN Set-PSDebug -Trace 2
# Wed, 10 Mar 2021 21:49:26 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 10 Mar 2021 21:49:27 GMT
EXPOSE 4222 8222
# Wed, 10 Mar 2021 21:49:28 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 10 Mar 2021 21:49:29 GMT
CMD ["-m" "8222"]
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
	-	`sha256:53877335227f3a676a7b42a4bfe29f3b308e4af725358ddb37e2a44fa6921a80`  
		Last Modified: Wed, 10 Mar 2021 21:54:20 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dded724566db49b2c3de437e8fc07b33da7a82fefc8ee1d6a90ce90bfb721914`  
		Last Modified: Wed, 10 Mar 2021 21:54:20 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55a9876360e291e6db5b15d8903e950e266fac317bbc049509fe3d0380a967ad`  
		Last Modified: Wed, 10 Mar 2021 21:54:20 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b3231bc8381e2d5c4e0ae136f5651b2459e1c4cfb039dc7d04233feace0fb3d`  
		Last Modified: Wed, 10 Mar 2021 21:54:19 GMT  
		Size: 5.1 MB (5064941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71a29a16a4eecc21940d5d0238db4f5e29fdf352f211193dd0d6ddc0a8392dee`  
		Last Modified: Wed, 10 Mar 2021 21:54:35 GMT  
		Size: 15.2 MB (15234342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60e3f696c440330f05de9af154fef7a7668334bfd83a5b6891ece035ed7ec703`  
		Last Modified: Wed, 10 Mar 2021 21:54:17 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ad4ce6f8f2d876a7c5fd7cd6fa233132de5181d550403653062f6ecdc0bd1e5`  
		Last Modified: Wed, 10 Mar 2021 21:54:18 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00a0ea7fcfe009366fde55d37e5932c25b24e3d6d81960f8781f792e143878a2`  
		Last Modified: Wed, 10 Mar 2021 21:54:17 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:windowsservercore` - windows version 10.0.14393.4283; amd64

```console
$ docker pull nats-streaming@sha256:594f9b8a930c3fbb8aacf7073d6822799c21005df6b94a9f1a3da70a8ef6df2a
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5818554710 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:77a6062b4ea3c0f03780986b01c644987bf4ad33acbf270f345b28aef38775fe`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
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
# Wed, 10 Mar 2021 21:49:49 GMT
ENV NATS_STREAMING_SERVER=0.21.1
# Wed, 10 Mar 2021 21:49:50 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.21.1/nats-streaming-server-v0.21.1-windows-amd64.zip
# Wed, 10 Mar 2021 21:49:51 GMT
ENV GIT_DOWNLOAD_SHA256=798ec9b686a8dcb4de93074f416eab067a0896b52ccfc05b65a5e21d55e634e5
# Wed, 10 Mar 2021 21:51:17 GMT
RUN Set-PSDebug -Trace 2
# Wed, 10 Mar 2021 21:53:25 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 10 Mar 2021 21:53:26 GMT
EXPOSE 4222 8222
# Wed, 10 Mar 2021 21:53:27 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 10 Mar 2021 21:53:28 GMT
CMD ["-m" "8222"]
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
	-	`sha256:3ea87885047b4a1f6a8e0632983da50ba4f31825a69b4f1e13ccb486984dbb81`  
		Last Modified: Wed, 10 Mar 2021 21:55:07 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57acbb65b7dc63351cdcbb771089539683461cd139e5a805bc3f0127181f38b1`  
		Last Modified: Wed, 10 Mar 2021 21:55:07 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5a204c1ad231fc6dfe4d92999bbe0aa9bad4a980ac2f89cdc05255a29a2bb0d`  
		Last Modified: Wed, 10 Mar 2021 21:55:07 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:817aa91f0e76ec219774d8759cba12fd464149e745865ab86ced46d6348f7d7f`  
		Last Modified: Wed, 10 Mar 2021 21:55:06 GMT  
		Size: 5.6 MB (5647336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a811f82bd6b42793f3d47bd0f94e40f0fbb9eefbe192813e03c13c50e897d604`  
		Last Modified: Wed, 10 Mar 2021 21:55:24 GMT  
		Size: 16.0 MB (15985398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba9f62bca657f59242456b4816b9f7ede6deced4cc0c1f90543b33b636084b98`  
		Last Modified: Wed, 10 Mar 2021 21:55:05 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf0ec3239c36380ddf5a7cda6e2fcdd186a3226ea98b17f33b0e083f84d5674e`  
		Last Modified: Wed, 10 Mar 2021 21:55:05 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ae978e2e615d8811e5f542215f7fefa26cdfc9025deee761d653bc3973fda1c`  
		Last Modified: Wed, 10 Mar 2021 21:55:05 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:windowsservercore-1809`

```console
$ docker pull nats-streaming@sha256:4bcd57606636d40356494deb4e00e85814521e94ea1d39150b42ed55d5da2276
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1817; amd64

### `nats-streaming:windowsservercore-1809` - windows version 10.0.17763.1817; amd64

```console
$ docker pull nats-streaming@sha256:7c32d8674de2b5a73ba6be51bb6514302b5c28001cb43905c393a60b63302467
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2481844979 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:201caf193f01ab7ea82dbd134d0a0e2fe29e689b1e03dfd0f19f0e397c693db6`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
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
# Wed, 10 Mar 2021 21:47:25 GMT
ENV NATS_STREAMING_SERVER=0.21.1
# Wed, 10 Mar 2021 21:47:26 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.21.1/nats-streaming-server-v0.21.1-windows-amd64.zip
# Wed, 10 Mar 2021 21:47:27 GMT
ENV GIT_DOWNLOAD_SHA256=798ec9b686a8dcb4de93074f416eab067a0896b52ccfc05b65a5e21d55e634e5
# Wed, 10 Mar 2021 21:48:01 GMT
RUN Set-PSDebug -Trace 2
# Wed, 10 Mar 2021 21:49:26 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 10 Mar 2021 21:49:27 GMT
EXPOSE 4222 8222
# Wed, 10 Mar 2021 21:49:28 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 10 Mar 2021 21:49:29 GMT
CMD ["-m" "8222"]
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
	-	`sha256:53877335227f3a676a7b42a4bfe29f3b308e4af725358ddb37e2a44fa6921a80`  
		Last Modified: Wed, 10 Mar 2021 21:54:20 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dded724566db49b2c3de437e8fc07b33da7a82fefc8ee1d6a90ce90bfb721914`  
		Last Modified: Wed, 10 Mar 2021 21:54:20 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55a9876360e291e6db5b15d8903e950e266fac317bbc049509fe3d0380a967ad`  
		Last Modified: Wed, 10 Mar 2021 21:54:20 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b3231bc8381e2d5c4e0ae136f5651b2459e1c4cfb039dc7d04233feace0fb3d`  
		Last Modified: Wed, 10 Mar 2021 21:54:19 GMT  
		Size: 5.1 MB (5064941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71a29a16a4eecc21940d5d0238db4f5e29fdf352f211193dd0d6ddc0a8392dee`  
		Last Modified: Wed, 10 Mar 2021 21:54:35 GMT  
		Size: 15.2 MB (15234342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60e3f696c440330f05de9af154fef7a7668334bfd83a5b6891ece035ed7ec703`  
		Last Modified: Wed, 10 Mar 2021 21:54:17 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ad4ce6f8f2d876a7c5fd7cd6fa233132de5181d550403653062f6ecdc0bd1e5`  
		Last Modified: Wed, 10 Mar 2021 21:54:18 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00a0ea7fcfe009366fde55d37e5932c25b24e3d6d81960f8781f792e143878a2`  
		Last Modified: Wed, 10 Mar 2021 21:54:17 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:windowsservercore-ltsc2016`

```console
$ docker pull nats-streaming@sha256:a79ba4262fcf0cb90e75fab395c2d6dc8126dbc4bfa7bddc82f31cfcd3c25409
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4283; amd64

### `nats-streaming:windowsservercore-ltsc2016` - windows version 10.0.14393.4283; amd64

```console
$ docker pull nats-streaming@sha256:594f9b8a930c3fbb8aacf7073d6822799c21005df6b94a9f1a3da70a8ef6df2a
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5818554710 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:77a6062b4ea3c0f03780986b01c644987bf4ad33acbf270f345b28aef38775fe`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
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
# Wed, 10 Mar 2021 21:49:49 GMT
ENV NATS_STREAMING_SERVER=0.21.1
# Wed, 10 Mar 2021 21:49:50 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.21.1/nats-streaming-server-v0.21.1-windows-amd64.zip
# Wed, 10 Mar 2021 21:49:51 GMT
ENV GIT_DOWNLOAD_SHA256=798ec9b686a8dcb4de93074f416eab067a0896b52ccfc05b65a5e21d55e634e5
# Wed, 10 Mar 2021 21:51:17 GMT
RUN Set-PSDebug -Trace 2
# Wed, 10 Mar 2021 21:53:25 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 10 Mar 2021 21:53:26 GMT
EXPOSE 4222 8222
# Wed, 10 Mar 2021 21:53:27 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 10 Mar 2021 21:53:28 GMT
CMD ["-m" "8222"]
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
	-	`sha256:3ea87885047b4a1f6a8e0632983da50ba4f31825a69b4f1e13ccb486984dbb81`  
		Last Modified: Wed, 10 Mar 2021 21:55:07 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57acbb65b7dc63351cdcbb771089539683461cd139e5a805bc3f0127181f38b1`  
		Last Modified: Wed, 10 Mar 2021 21:55:07 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5a204c1ad231fc6dfe4d92999bbe0aa9bad4a980ac2f89cdc05255a29a2bb0d`  
		Last Modified: Wed, 10 Mar 2021 21:55:07 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:817aa91f0e76ec219774d8759cba12fd464149e745865ab86ced46d6348f7d7f`  
		Last Modified: Wed, 10 Mar 2021 21:55:06 GMT  
		Size: 5.6 MB (5647336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a811f82bd6b42793f3d47bd0f94e40f0fbb9eefbe192813e03c13c50e897d604`  
		Last Modified: Wed, 10 Mar 2021 21:55:24 GMT  
		Size: 16.0 MB (15985398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba9f62bca657f59242456b4816b9f7ede6deced4cc0c1f90543b33b636084b98`  
		Last Modified: Wed, 10 Mar 2021 21:55:05 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf0ec3239c36380ddf5a7cda6e2fcdd186a3226ea98b17f33b0e083f84d5674e`  
		Last Modified: Wed, 10 Mar 2021 21:55:05 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ae978e2e615d8811e5f542215f7fefa26cdfc9025deee761d653bc3973fda1c`  
		Last Modified: Wed, 10 Mar 2021 21:55:05 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
