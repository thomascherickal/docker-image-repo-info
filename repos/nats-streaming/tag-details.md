<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `nats-streaming`

-	[`nats-streaming:0.19`](#nats-streaming019)
-	[`nats-streaming:0.19.0`](#nats-streaming0190)
-	[`nats-streaming:0.19.0-alpine`](#nats-streaming0190-alpine)
-	[`nats-streaming:0.19.0-alpine3.12`](#nats-streaming0190-alpine312)
-	[`nats-streaming:0.19.0-linux`](#nats-streaming0190-linux)
-	[`nats-streaming:0.19.0-nanoserver`](#nats-streaming0190-nanoserver)
-	[`nats-streaming:0.19.0-nanoserver-1809`](#nats-streaming0190-nanoserver-1809)
-	[`nats-streaming:0.19.0-scratch`](#nats-streaming0190-scratch)
-	[`nats-streaming:0.19.0-windowsservercore`](#nats-streaming0190-windowsservercore)
-	[`nats-streaming:0.19.0-windowsservercore-1809`](#nats-streaming0190-windowsservercore-1809)
-	[`nats-streaming:0.19.0-windowsservercore-ltsc2016`](#nats-streaming0190-windowsservercore-ltsc2016)
-	[`nats-streaming:0.19-alpine`](#nats-streaming019-alpine)
-	[`nats-streaming:0.19-alpine3.12`](#nats-streaming019-alpine312)
-	[`nats-streaming:0.19-linux`](#nats-streaming019-linux)
-	[`nats-streaming:0.19-nanoserver`](#nats-streaming019-nanoserver)
-	[`nats-streaming:0.19-nanoserver-1809`](#nats-streaming019-nanoserver-1809)
-	[`nats-streaming:0.19-scratch`](#nats-streaming019-scratch)
-	[`nats-streaming:0.19-windowsservercore`](#nats-streaming019-windowsservercore)
-	[`nats-streaming:0.19-windowsservercore-1809`](#nats-streaming019-windowsservercore-1809)
-	[`nats-streaming:0.19-windowsservercore-ltsc2016`](#nats-streaming019-windowsservercore-ltsc2016)
-	[`nats-streaming:alpine`](#nats-streamingalpine)
-	[`nats-streaming:alpine3.12`](#nats-streamingalpine312)
-	[`nats-streaming:latest`](#nats-streaminglatest)
-	[`nats-streaming:linux`](#nats-streaminglinux)
-	[`nats-streaming:nanoserver`](#nats-streamingnanoserver)
-	[`nats-streaming:nanoserver-1809`](#nats-streamingnanoserver-1809)
-	[`nats-streaming:scratch`](#nats-streamingscratch)
-	[`nats-streaming:windowsservercore`](#nats-streamingwindowsservercore)
-	[`nats-streaming:windowsservercore-1809`](#nats-streamingwindowsservercore-1809)
-	[`nats-streaming:windowsservercore-ltsc2016`](#nats-streamingwindowsservercore-ltsc2016)

## `nats-streaming:0.19`

```console
$ docker pull nats-streaming@sha256:38acdd0ea58e27f121a475e4aeacfa95206a22240d8999150df940aa5246c0ce
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; arm variant v6
	-	linux; arm variant v7

### `nats-streaming:0.19` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:f334d10ef2a4663d8d7d920d96321cd97f050b82a5d55d588192f074f60dd814
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 MB (6049845 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9eecfd5ab4178a65e952a7cf1d248a556a6ae2c328ac8b68923146d64734db03`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 02 Nov 2020 23:56:28 GMT
COPY file:d6896b1c93dcd497494c972f9274fcc634a4f4a8d63a0191bdb87f6336aec0d7 in /nats-streaming-server 
# Mon, 02 Nov 2020 23:56:28 GMT
EXPOSE 4222 8222
# Mon, 02 Nov 2020 23:56:29 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 02 Nov 2020 23:56:29 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:7f165fb71ab77e8081dbfa13656cdf9e5e005002d6c3afa0aac40667a0f97af8`  
		Last Modified: Mon, 02 Nov 2020 23:57:04 GMT  
		Size: 6.0 MB (6049845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.19` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:5fd0943909d8aedafb888e099c9f64d234023ad780805ed7c939692ebfd8304d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 MB (6043163 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f37071e856ae40dc3c8c5e10b359d1640fd67a6110741c0957af2031032ed6ce`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 03 Nov 2020 00:05:23 GMT
COPY file:d232132ddff1d85d3a2f5c80a91c80023cbc103d816387e06d604cf97238e52c in /nats-streaming-server 
# Tue, 03 Nov 2020 00:05:24 GMT
EXPOSE 4222 8222
# Tue, 03 Nov 2020 00:05:24 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 03 Nov 2020 00:05:25 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:9c7227cc1040d04ca7763cfb53ab58bc32ae54921990516adf8e13374ac9ef29`  
		Last Modified: Tue, 03 Nov 2020 00:05:57 GMT  
		Size: 6.0 MB (6043163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.19.0`

```console
$ docker pull nats-streaming@sha256:38acdd0ea58e27f121a475e4aeacfa95206a22240d8999150df940aa5246c0ce
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; arm variant v6
	-	linux; arm variant v7

### `nats-streaming:0.19.0` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:f334d10ef2a4663d8d7d920d96321cd97f050b82a5d55d588192f074f60dd814
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 MB (6049845 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9eecfd5ab4178a65e952a7cf1d248a556a6ae2c328ac8b68923146d64734db03`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 02 Nov 2020 23:56:28 GMT
COPY file:d6896b1c93dcd497494c972f9274fcc634a4f4a8d63a0191bdb87f6336aec0d7 in /nats-streaming-server 
# Mon, 02 Nov 2020 23:56:28 GMT
EXPOSE 4222 8222
# Mon, 02 Nov 2020 23:56:29 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 02 Nov 2020 23:56:29 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:7f165fb71ab77e8081dbfa13656cdf9e5e005002d6c3afa0aac40667a0f97af8`  
		Last Modified: Mon, 02 Nov 2020 23:57:04 GMT  
		Size: 6.0 MB (6049845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.19.0` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:5fd0943909d8aedafb888e099c9f64d234023ad780805ed7c939692ebfd8304d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 MB (6043163 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f37071e856ae40dc3c8c5e10b359d1640fd67a6110741c0957af2031032ed6ce`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 03 Nov 2020 00:05:23 GMT
COPY file:d232132ddff1d85d3a2f5c80a91c80023cbc103d816387e06d604cf97238e52c in /nats-streaming-server 
# Tue, 03 Nov 2020 00:05:24 GMT
EXPOSE 4222 8222
# Tue, 03 Nov 2020 00:05:24 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 03 Nov 2020 00:05:25 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:9c7227cc1040d04ca7763cfb53ab58bc32ae54921990516adf8e13374ac9ef29`  
		Last Modified: Tue, 03 Nov 2020 00:05:57 GMT  
		Size: 6.0 MB (6043163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.19.0-alpine`

```console
$ docker pull nats-streaming@sha256:c240732dc2a588fe00d65a036722c05ede2b8ff624d86c9809a68f649d24670a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; arm variant v6
	-	linux; arm variant v7

### `nats-streaming:0.19.0-alpine` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:2a58d6644e94cc17212ec6a604029ebe9f855ceeee7fa66171bdc8aa6c7113ba
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.9 MB (8932203 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b8391afd58a04ec8cf1ab166357c9495c5aa4d32bc4bb4472e577874f42fe55d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Thu, 22 Oct 2020 02:01:09 GMT
ADD file:dec4d3b6cf21c59820d1d74a554d0a193b5f4859e00b932f31ffe73f554d5afb in / 
# Thu, 22 Oct 2020 02:01:12 GMT
CMD ["/bin/sh"]
# Mon, 02 Nov 2020 23:56:13 GMT
ENV NATS_STREAMING_SERVER=0.19.0
# Mon, 02 Nov 2020 23:56:17 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='d582023b8f9fe33b98f0faa6396aae8d5366ecade7e56cde912e21e5b93ea670' ;; 		armhf) natsArch='arm6'; sha256='f4af03e6cbb19f3ad9ea57217607dcf4b68018e1879859c847e2680917fc7139' ;; 		armv7) natsArch='arm7'; sha256='ec8c5ca693344e8b24de9ac955c38de757af8c5760658fc29ed2fbd804803fad' ;; 		x86_64) natsArch='amd64'; sha256='fc15530faec66b61de5140c2b99927c5839caff1c4c17f8bffbf4432fab83017' ;; 		x86) natsArch='386'; sha256='655f0f7cebf727317974006ad4a13ddacd3520f15266e854c2b01681e499bf80' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Mon, 02 Nov 2020 23:56:17 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Mon, 02 Nov 2020 23:56:18 GMT
EXPOSE 4222 8222
# Mon, 02 Nov 2020 23:56:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 02 Nov 2020 23:56:19 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:bad30e7b45c14f784ef29a828b5fc69db0ebdefebcde6a7c98f4f77ffc93a546`  
		Last Modified: Thu, 22 Oct 2020 02:01:42 GMT  
		Size: 2.6 MB (2601912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21cba1ed5b5094a02c017d654b758674905ec0bb2535d3311fcdd61dce32b319`  
		Last Modified: Mon, 02 Nov 2020 23:56:50 GMT  
		Size: 6.3 MB (6329871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3992f15ff4c1a7660c4a81854ec33d3e4973405c7095ceb0bd8a7865fff21c9f`  
		Last Modified: Mon, 02 Nov 2020 23:56:47 GMT  
		Size: 420.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.19.0-alpine` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:6a6c52fc272b91cff878ca25bddc432f19583a2e41e5e92288f0e64d0c649896
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.7 MB (8730479 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b4347330ee2d9b26f7fafaadc370627e71670505b340c9e4b54d791afcb3a6b2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Thu, 22 Oct 2020 01:58:13 GMT
ADD file:46f89172426e9f5b1d669a2ca7ab218fc2deaef1caeeab88f2b5bd443ac9773d in / 
# Thu, 22 Oct 2020 01:58:14 GMT
CMD ["/bin/sh"]
# Tue, 03 Nov 2020 00:05:05 GMT
ENV NATS_STREAMING_SERVER=0.19.0
# Tue, 03 Nov 2020 00:05:09 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='d582023b8f9fe33b98f0faa6396aae8d5366ecade7e56cde912e21e5b93ea670' ;; 		armhf) natsArch='arm6'; sha256='f4af03e6cbb19f3ad9ea57217607dcf4b68018e1879859c847e2680917fc7139' ;; 		armv7) natsArch='arm7'; sha256='ec8c5ca693344e8b24de9ac955c38de757af8c5760658fc29ed2fbd804803fad' ;; 		x86_64) natsArch='amd64'; sha256='fc15530faec66b61de5140c2b99927c5839caff1c4c17f8bffbf4432fab83017' ;; 		x86) natsArch='386'; sha256='655f0f7cebf727317974006ad4a13ddacd3520f15266e854c2b01681e499bf80' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Tue, 03 Nov 2020 00:05:09 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Tue, 03 Nov 2020 00:05:10 GMT
EXPOSE 4222 8222
# Tue, 03 Nov 2020 00:05:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 03 Nov 2020 00:05:11 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:5f2023fd85a4e68f37fe41421fd89f30e69b98a645613521c57c01317561eee3`  
		Last Modified: Thu, 22 Oct 2020 01:58:45 GMT  
		Size: 2.4 MB (2405675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34033d6dabe9c0f77f765bf2fce39f1eef24c163cfa802ec78f0e2e1bea9da7c`  
		Last Modified: Tue, 03 Nov 2020 00:05:43 GMT  
		Size: 6.3 MB (6324384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b0a98c9d7b5d859df80140920031b236b38ff88a4ff09d3bf8cfc5b9776e436`  
		Last Modified: Tue, 03 Nov 2020 00:05:40 GMT  
		Size: 420.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.19.0-alpine3.12`

```console
$ docker pull nats-streaming@sha256:c240732dc2a588fe00d65a036722c05ede2b8ff624d86c9809a68f649d24670a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; arm variant v6
	-	linux; arm variant v7

### `nats-streaming:0.19.0-alpine3.12` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:2a58d6644e94cc17212ec6a604029ebe9f855ceeee7fa66171bdc8aa6c7113ba
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.9 MB (8932203 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b8391afd58a04ec8cf1ab166357c9495c5aa4d32bc4bb4472e577874f42fe55d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Thu, 22 Oct 2020 02:01:09 GMT
ADD file:dec4d3b6cf21c59820d1d74a554d0a193b5f4859e00b932f31ffe73f554d5afb in / 
# Thu, 22 Oct 2020 02:01:12 GMT
CMD ["/bin/sh"]
# Mon, 02 Nov 2020 23:56:13 GMT
ENV NATS_STREAMING_SERVER=0.19.0
# Mon, 02 Nov 2020 23:56:17 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='d582023b8f9fe33b98f0faa6396aae8d5366ecade7e56cde912e21e5b93ea670' ;; 		armhf) natsArch='arm6'; sha256='f4af03e6cbb19f3ad9ea57217607dcf4b68018e1879859c847e2680917fc7139' ;; 		armv7) natsArch='arm7'; sha256='ec8c5ca693344e8b24de9ac955c38de757af8c5760658fc29ed2fbd804803fad' ;; 		x86_64) natsArch='amd64'; sha256='fc15530faec66b61de5140c2b99927c5839caff1c4c17f8bffbf4432fab83017' ;; 		x86) natsArch='386'; sha256='655f0f7cebf727317974006ad4a13ddacd3520f15266e854c2b01681e499bf80' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Mon, 02 Nov 2020 23:56:17 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Mon, 02 Nov 2020 23:56:18 GMT
EXPOSE 4222 8222
# Mon, 02 Nov 2020 23:56:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 02 Nov 2020 23:56:19 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:bad30e7b45c14f784ef29a828b5fc69db0ebdefebcde6a7c98f4f77ffc93a546`  
		Last Modified: Thu, 22 Oct 2020 02:01:42 GMT  
		Size: 2.6 MB (2601912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21cba1ed5b5094a02c017d654b758674905ec0bb2535d3311fcdd61dce32b319`  
		Last Modified: Mon, 02 Nov 2020 23:56:50 GMT  
		Size: 6.3 MB (6329871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3992f15ff4c1a7660c4a81854ec33d3e4973405c7095ceb0bd8a7865fff21c9f`  
		Last Modified: Mon, 02 Nov 2020 23:56:47 GMT  
		Size: 420.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.19.0-alpine3.12` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:6a6c52fc272b91cff878ca25bddc432f19583a2e41e5e92288f0e64d0c649896
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.7 MB (8730479 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b4347330ee2d9b26f7fafaadc370627e71670505b340c9e4b54d791afcb3a6b2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Thu, 22 Oct 2020 01:58:13 GMT
ADD file:46f89172426e9f5b1d669a2ca7ab218fc2deaef1caeeab88f2b5bd443ac9773d in / 
# Thu, 22 Oct 2020 01:58:14 GMT
CMD ["/bin/sh"]
# Tue, 03 Nov 2020 00:05:05 GMT
ENV NATS_STREAMING_SERVER=0.19.0
# Tue, 03 Nov 2020 00:05:09 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='d582023b8f9fe33b98f0faa6396aae8d5366ecade7e56cde912e21e5b93ea670' ;; 		armhf) natsArch='arm6'; sha256='f4af03e6cbb19f3ad9ea57217607dcf4b68018e1879859c847e2680917fc7139' ;; 		armv7) natsArch='arm7'; sha256='ec8c5ca693344e8b24de9ac955c38de757af8c5760658fc29ed2fbd804803fad' ;; 		x86_64) natsArch='amd64'; sha256='fc15530faec66b61de5140c2b99927c5839caff1c4c17f8bffbf4432fab83017' ;; 		x86) natsArch='386'; sha256='655f0f7cebf727317974006ad4a13ddacd3520f15266e854c2b01681e499bf80' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Tue, 03 Nov 2020 00:05:09 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Tue, 03 Nov 2020 00:05:10 GMT
EXPOSE 4222 8222
# Tue, 03 Nov 2020 00:05:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 03 Nov 2020 00:05:11 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:5f2023fd85a4e68f37fe41421fd89f30e69b98a645613521c57c01317561eee3`  
		Last Modified: Thu, 22 Oct 2020 01:58:45 GMT  
		Size: 2.4 MB (2405675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34033d6dabe9c0f77f765bf2fce39f1eef24c163cfa802ec78f0e2e1bea9da7c`  
		Last Modified: Tue, 03 Nov 2020 00:05:43 GMT  
		Size: 6.3 MB (6324384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b0a98c9d7b5d859df80140920031b236b38ff88a4ff09d3bf8cfc5b9776e436`  
		Last Modified: Tue, 03 Nov 2020 00:05:40 GMT  
		Size: 420.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.19.0-linux`

```console
$ docker pull nats-streaming@sha256:38acdd0ea58e27f121a475e4aeacfa95206a22240d8999150df940aa5246c0ce
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; arm variant v6
	-	linux; arm variant v7

### `nats-streaming:0.19.0-linux` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:f334d10ef2a4663d8d7d920d96321cd97f050b82a5d55d588192f074f60dd814
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 MB (6049845 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9eecfd5ab4178a65e952a7cf1d248a556a6ae2c328ac8b68923146d64734db03`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 02 Nov 2020 23:56:28 GMT
COPY file:d6896b1c93dcd497494c972f9274fcc634a4f4a8d63a0191bdb87f6336aec0d7 in /nats-streaming-server 
# Mon, 02 Nov 2020 23:56:28 GMT
EXPOSE 4222 8222
# Mon, 02 Nov 2020 23:56:29 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 02 Nov 2020 23:56:29 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:7f165fb71ab77e8081dbfa13656cdf9e5e005002d6c3afa0aac40667a0f97af8`  
		Last Modified: Mon, 02 Nov 2020 23:57:04 GMT  
		Size: 6.0 MB (6049845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.19.0-linux` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:5fd0943909d8aedafb888e099c9f64d234023ad780805ed7c939692ebfd8304d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 MB (6043163 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f37071e856ae40dc3c8c5e10b359d1640fd67a6110741c0957af2031032ed6ce`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 03 Nov 2020 00:05:23 GMT
COPY file:d232132ddff1d85d3a2f5c80a91c80023cbc103d816387e06d604cf97238e52c in /nats-streaming-server 
# Tue, 03 Nov 2020 00:05:24 GMT
EXPOSE 4222 8222
# Tue, 03 Nov 2020 00:05:24 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 03 Nov 2020 00:05:25 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:9c7227cc1040d04ca7763cfb53ab58bc32ae54921990516adf8e13374ac9ef29`  
		Last Modified: Tue, 03 Nov 2020 00:05:57 GMT  
		Size: 6.0 MB (6043163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.19.0-nanoserver`

```console
$ docker pull nats-streaming@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:

## `nats-streaming:0.19.0-nanoserver-1809`

```console
$ docker pull nats-streaming@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:

## `nats-streaming:0.19.0-scratch`

```console
$ docker pull nats-streaming@sha256:38acdd0ea58e27f121a475e4aeacfa95206a22240d8999150df940aa5246c0ce
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; arm variant v6
	-	linux; arm variant v7

### `nats-streaming:0.19.0-scratch` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:f334d10ef2a4663d8d7d920d96321cd97f050b82a5d55d588192f074f60dd814
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 MB (6049845 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9eecfd5ab4178a65e952a7cf1d248a556a6ae2c328ac8b68923146d64734db03`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 02 Nov 2020 23:56:28 GMT
COPY file:d6896b1c93dcd497494c972f9274fcc634a4f4a8d63a0191bdb87f6336aec0d7 in /nats-streaming-server 
# Mon, 02 Nov 2020 23:56:28 GMT
EXPOSE 4222 8222
# Mon, 02 Nov 2020 23:56:29 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 02 Nov 2020 23:56:29 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:7f165fb71ab77e8081dbfa13656cdf9e5e005002d6c3afa0aac40667a0f97af8`  
		Last Modified: Mon, 02 Nov 2020 23:57:04 GMT  
		Size: 6.0 MB (6049845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.19.0-scratch` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:5fd0943909d8aedafb888e099c9f64d234023ad780805ed7c939692ebfd8304d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 MB (6043163 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f37071e856ae40dc3c8c5e10b359d1640fd67a6110741c0957af2031032ed6ce`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 03 Nov 2020 00:05:23 GMT
COPY file:d232132ddff1d85d3a2f5c80a91c80023cbc103d816387e06d604cf97238e52c in /nats-streaming-server 
# Tue, 03 Nov 2020 00:05:24 GMT
EXPOSE 4222 8222
# Tue, 03 Nov 2020 00:05:24 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 03 Nov 2020 00:05:25 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:9c7227cc1040d04ca7763cfb53ab58bc32ae54921990516adf8e13374ac9ef29`  
		Last Modified: Tue, 03 Nov 2020 00:05:57 GMT  
		Size: 6.0 MB (6043163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.19.0-windowsservercore`

```console
$ docker pull nats-streaming@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:

## `nats-streaming:0.19.0-windowsservercore-1809`

```console
$ docker pull nats-streaming@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:

## `nats-streaming:0.19.0-windowsservercore-ltsc2016`

```console
$ docker pull nats-streaming@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:

## `nats-streaming:0.19-alpine`

```console
$ docker pull nats-streaming@sha256:c240732dc2a588fe00d65a036722c05ede2b8ff624d86c9809a68f649d24670a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; arm variant v6
	-	linux; arm variant v7

### `nats-streaming:0.19-alpine` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:2a58d6644e94cc17212ec6a604029ebe9f855ceeee7fa66171bdc8aa6c7113ba
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.9 MB (8932203 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b8391afd58a04ec8cf1ab166357c9495c5aa4d32bc4bb4472e577874f42fe55d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Thu, 22 Oct 2020 02:01:09 GMT
ADD file:dec4d3b6cf21c59820d1d74a554d0a193b5f4859e00b932f31ffe73f554d5afb in / 
# Thu, 22 Oct 2020 02:01:12 GMT
CMD ["/bin/sh"]
# Mon, 02 Nov 2020 23:56:13 GMT
ENV NATS_STREAMING_SERVER=0.19.0
# Mon, 02 Nov 2020 23:56:17 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='d582023b8f9fe33b98f0faa6396aae8d5366ecade7e56cde912e21e5b93ea670' ;; 		armhf) natsArch='arm6'; sha256='f4af03e6cbb19f3ad9ea57217607dcf4b68018e1879859c847e2680917fc7139' ;; 		armv7) natsArch='arm7'; sha256='ec8c5ca693344e8b24de9ac955c38de757af8c5760658fc29ed2fbd804803fad' ;; 		x86_64) natsArch='amd64'; sha256='fc15530faec66b61de5140c2b99927c5839caff1c4c17f8bffbf4432fab83017' ;; 		x86) natsArch='386'; sha256='655f0f7cebf727317974006ad4a13ddacd3520f15266e854c2b01681e499bf80' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Mon, 02 Nov 2020 23:56:17 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Mon, 02 Nov 2020 23:56:18 GMT
EXPOSE 4222 8222
# Mon, 02 Nov 2020 23:56:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 02 Nov 2020 23:56:19 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:bad30e7b45c14f784ef29a828b5fc69db0ebdefebcde6a7c98f4f77ffc93a546`  
		Last Modified: Thu, 22 Oct 2020 02:01:42 GMT  
		Size: 2.6 MB (2601912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21cba1ed5b5094a02c017d654b758674905ec0bb2535d3311fcdd61dce32b319`  
		Last Modified: Mon, 02 Nov 2020 23:56:50 GMT  
		Size: 6.3 MB (6329871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3992f15ff4c1a7660c4a81854ec33d3e4973405c7095ceb0bd8a7865fff21c9f`  
		Last Modified: Mon, 02 Nov 2020 23:56:47 GMT  
		Size: 420.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.19-alpine` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:6a6c52fc272b91cff878ca25bddc432f19583a2e41e5e92288f0e64d0c649896
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.7 MB (8730479 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b4347330ee2d9b26f7fafaadc370627e71670505b340c9e4b54d791afcb3a6b2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Thu, 22 Oct 2020 01:58:13 GMT
ADD file:46f89172426e9f5b1d669a2ca7ab218fc2deaef1caeeab88f2b5bd443ac9773d in / 
# Thu, 22 Oct 2020 01:58:14 GMT
CMD ["/bin/sh"]
# Tue, 03 Nov 2020 00:05:05 GMT
ENV NATS_STREAMING_SERVER=0.19.0
# Tue, 03 Nov 2020 00:05:09 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='d582023b8f9fe33b98f0faa6396aae8d5366ecade7e56cde912e21e5b93ea670' ;; 		armhf) natsArch='arm6'; sha256='f4af03e6cbb19f3ad9ea57217607dcf4b68018e1879859c847e2680917fc7139' ;; 		armv7) natsArch='arm7'; sha256='ec8c5ca693344e8b24de9ac955c38de757af8c5760658fc29ed2fbd804803fad' ;; 		x86_64) natsArch='amd64'; sha256='fc15530faec66b61de5140c2b99927c5839caff1c4c17f8bffbf4432fab83017' ;; 		x86) natsArch='386'; sha256='655f0f7cebf727317974006ad4a13ddacd3520f15266e854c2b01681e499bf80' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Tue, 03 Nov 2020 00:05:09 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Tue, 03 Nov 2020 00:05:10 GMT
EXPOSE 4222 8222
# Tue, 03 Nov 2020 00:05:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 03 Nov 2020 00:05:11 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:5f2023fd85a4e68f37fe41421fd89f30e69b98a645613521c57c01317561eee3`  
		Last Modified: Thu, 22 Oct 2020 01:58:45 GMT  
		Size: 2.4 MB (2405675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34033d6dabe9c0f77f765bf2fce39f1eef24c163cfa802ec78f0e2e1bea9da7c`  
		Last Modified: Tue, 03 Nov 2020 00:05:43 GMT  
		Size: 6.3 MB (6324384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b0a98c9d7b5d859df80140920031b236b38ff88a4ff09d3bf8cfc5b9776e436`  
		Last Modified: Tue, 03 Nov 2020 00:05:40 GMT  
		Size: 420.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.19-alpine3.12`

```console
$ docker pull nats-streaming@sha256:c240732dc2a588fe00d65a036722c05ede2b8ff624d86c9809a68f649d24670a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; arm variant v6
	-	linux; arm variant v7

### `nats-streaming:0.19-alpine3.12` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:2a58d6644e94cc17212ec6a604029ebe9f855ceeee7fa66171bdc8aa6c7113ba
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.9 MB (8932203 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b8391afd58a04ec8cf1ab166357c9495c5aa4d32bc4bb4472e577874f42fe55d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Thu, 22 Oct 2020 02:01:09 GMT
ADD file:dec4d3b6cf21c59820d1d74a554d0a193b5f4859e00b932f31ffe73f554d5afb in / 
# Thu, 22 Oct 2020 02:01:12 GMT
CMD ["/bin/sh"]
# Mon, 02 Nov 2020 23:56:13 GMT
ENV NATS_STREAMING_SERVER=0.19.0
# Mon, 02 Nov 2020 23:56:17 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='d582023b8f9fe33b98f0faa6396aae8d5366ecade7e56cde912e21e5b93ea670' ;; 		armhf) natsArch='arm6'; sha256='f4af03e6cbb19f3ad9ea57217607dcf4b68018e1879859c847e2680917fc7139' ;; 		armv7) natsArch='arm7'; sha256='ec8c5ca693344e8b24de9ac955c38de757af8c5760658fc29ed2fbd804803fad' ;; 		x86_64) natsArch='amd64'; sha256='fc15530faec66b61de5140c2b99927c5839caff1c4c17f8bffbf4432fab83017' ;; 		x86) natsArch='386'; sha256='655f0f7cebf727317974006ad4a13ddacd3520f15266e854c2b01681e499bf80' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Mon, 02 Nov 2020 23:56:17 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Mon, 02 Nov 2020 23:56:18 GMT
EXPOSE 4222 8222
# Mon, 02 Nov 2020 23:56:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 02 Nov 2020 23:56:19 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:bad30e7b45c14f784ef29a828b5fc69db0ebdefebcde6a7c98f4f77ffc93a546`  
		Last Modified: Thu, 22 Oct 2020 02:01:42 GMT  
		Size: 2.6 MB (2601912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21cba1ed5b5094a02c017d654b758674905ec0bb2535d3311fcdd61dce32b319`  
		Last Modified: Mon, 02 Nov 2020 23:56:50 GMT  
		Size: 6.3 MB (6329871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3992f15ff4c1a7660c4a81854ec33d3e4973405c7095ceb0bd8a7865fff21c9f`  
		Last Modified: Mon, 02 Nov 2020 23:56:47 GMT  
		Size: 420.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.19-alpine3.12` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:6a6c52fc272b91cff878ca25bddc432f19583a2e41e5e92288f0e64d0c649896
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.7 MB (8730479 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b4347330ee2d9b26f7fafaadc370627e71670505b340c9e4b54d791afcb3a6b2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Thu, 22 Oct 2020 01:58:13 GMT
ADD file:46f89172426e9f5b1d669a2ca7ab218fc2deaef1caeeab88f2b5bd443ac9773d in / 
# Thu, 22 Oct 2020 01:58:14 GMT
CMD ["/bin/sh"]
# Tue, 03 Nov 2020 00:05:05 GMT
ENV NATS_STREAMING_SERVER=0.19.0
# Tue, 03 Nov 2020 00:05:09 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='d582023b8f9fe33b98f0faa6396aae8d5366ecade7e56cde912e21e5b93ea670' ;; 		armhf) natsArch='arm6'; sha256='f4af03e6cbb19f3ad9ea57217607dcf4b68018e1879859c847e2680917fc7139' ;; 		armv7) natsArch='arm7'; sha256='ec8c5ca693344e8b24de9ac955c38de757af8c5760658fc29ed2fbd804803fad' ;; 		x86_64) natsArch='amd64'; sha256='fc15530faec66b61de5140c2b99927c5839caff1c4c17f8bffbf4432fab83017' ;; 		x86) natsArch='386'; sha256='655f0f7cebf727317974006ad4a13ddacd3520f15266e854c2b01681e499bf80' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Tue, 03 Nov 2020 00:05:09 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Tue, 03 Nov 2020 00:05:10 GMT
EXPOSE 4222 8222
# Tue, 03 Nov 2020 00:05:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 03 Nov 2020 00:05:11 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:5f2023fd85a4e68f37fe41421fd89f30e69b98a645613521c57c01317561eee3`  
		Last Modified: Thu, 22 Oct 2020 01:58:45 GMT  
		Size: 2.4 MB (2405675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34033d6dabe9c0f77f765bf2fce39f1eef24c163cfa802ec78f0e2e1bea9da7c`  
		Last Modified: Tue, 03 Nov 2020 00:05:43 GMT  
		Size: 6.3 MB (6324384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b0a98c9d7b5d859df80140920031b236b38ff88a4ff09d3bf8cfc5b9776e436`  
		Last Modified: Tue, 03 Nov 2020 00:05:40 GMT  
		Size: 420.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.19-linux`

```console
$ docker pull nats-streaming@sha256:38acdd0ea58e27f121a475e4aeacfa95206a22240d8999150df940aa5246c0ce
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; arm variant v6
	-	linux; arm variant v7

### `nats-streaming:0.19-linux` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:f334d10ef2a4663d8d7d920d96321cd97f050b82a5d55d588192f074f60dd814
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 MB (6049845 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9eecfd5ab4178a65e952a7cf1d248a556a6ae2c328ac8b68923146d64734db03`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 02 Nov 2020 23:56:28 GMT
COPY file:d6896b1c93dcd497494c972f9274fcc634a4f4a8d63a0191bdb87f6336aec0d7 in /nats-streaming-server 
# Mon, 02 Nov 2020 23:56:28 GMT
EXPOSE 4222 8222
# Mon, 02 Nov 2020 23:56:29 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 02 Nov 2020 23:56:29 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:7f165fb71ab77e8081dbfa13656cdf9e5e005002d6c3afa0aac40667a0f97af8`  
		Last Modified: Mon, 02 Nov 2020 23:57:04 GMT  
		Size: 6.0 MB (6049845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.19-linux` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:5fd0943909d8aedafb888e099c9f64d234023ad780805ed7c939692ebfd8304d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 MB (6043163 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f37071e856ae40dc3c8c5e10b359d1640fd67a6110741c0957af2031032ed6ce`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 03 Nov 2020 00:05:23 GMT
COPY file:d232132ddff1d85d3a2f5c80a91c80023cbc103d816387e06d604cf97238e52c in /nats-streaming-server 
# Tue, 03 Nov 2020 00:05:24 GMT
EXPOSE 4222 8222
# Tue, 03 Nov 2020 00:05:24 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 03 Nov 2020 00:05:25 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:9c7227cc1040d04ca7763cfb53ab58bc32ae54921990516adf8e13374ac9ef29`  
		Last Modified: Tue, 03 Nov 2020 00:05:57 GMT  
		Size: 6.0 MB (6043163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.19-nanoserver`

```console
$ docker pull nats-streaming@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:

## `nats-streaming:0.19-nanoserver-1809`

```console
$ docker pull nats-streaming@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:

## `nats-streaming:0.19-scratch`

```console
$ docker pull nats-streaming@sha256:38acdd0ea58e27f121a475e4aeacfa95206a22240d8999150df940aa5246c0ce
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; arm variant v6
	-	linux; arm variant v7

### `nats-streaming:0.19-scratch` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:f334d10ef2a4663d8d7d920d96321cd97f050b82a5d55d588192f074f60dd814
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 MB (6049845 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9eecfd5ab4178a65e952a7cf1d248a556a6ae2c328ac8b68923146d64734db03`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 02 Nov 2020 23:56:28 GMT
COPY file:d6896b1c93dcd497494c972f9274fcc634a4f4a8d63a0191bdb87f6336aec0d7 in /nats-streaming-server 
# Mon, 02 Nov 2020 23:56:28 GMT
EXPOSE 4222 8222
# Mon, 02 Nov 2020 23:56:29 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 02 Nov 2020 23:56:29 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:7f165fb71ab77e8081dbfa13656cdf9e5e005002d6c3afa0aac40667a0f97af8`  
		Last Modified: Mon, 02 Nov 2020 23:57:04 GMT  
		Size: 6.0 MB (6049845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.19-scratch` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:5fd0943909d8aedafb888e099c9f64d234023ad780805ed7c939692ebfd8304d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 MB (6043163 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f37071e856ae40dc3c8c5e10b359d1640fd67a6110741c0957af2031032ed6ce`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 03 Nov 2020 00:05:23 GMT
COPY file:d232132ddff1d85d3a2f5c80a91c80023cbc103d816387e06d604cf97238e52c in /nats-streaming-server 
# Tue, 03 Nov 2020 00:05:24 GMT
EXPOSE 4222 8222
# Tue, 03 Nov 2020 00:05:24 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 03 Nov 2020 00:05:25 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:9c7227cc1040d04ca7763cfb53ab58bc32ae54921990516adf8e13374ac9ef29`  
		Last Modified: Tue, 03 Nov 2020 00:05:57 GMT  
		Size: 6.0 MB (6043163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.19-windowsservercore`

```console
$ docker pull nats-streaming@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:

## `nats-streaming:0.19-windowsservercore-1809`

```console
$ docker pull nats-streaming@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:

## `nats-streaming:0.19-windowsservercore-ltsc2016`

```console
$ docker pull nats-streaming@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:

## `nats-streaming:alpine`

```console
$ docker pull nats-streaming@sha256:31cfb9794a53c308e59076c863ac375b3fc53c2fa800152a271df02ad7f71f2a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:alpine` - linux; amd64

```console
$ docker pull nats-streaming@sha256:26c179bfe34f31c821aa7b38083c0d4d3d96977eb3864d3c5a15157997b3f643
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.0 MB (9014534 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae46b411ada6bf35dd2255a5183b0e47b3c82be305fc90ef424e1ee01f6ecb50`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Thu, 22 Oct 2020 02:19:24 GMT
ADD file:f17f65714f703db9012f00e5ec98d0b2541ff6147c2633f7ab9ba659d0c507f4 in / 
# Thu, 22 Oct 2020 02:19:24 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 07:52:32 GMT
ENV NATS_STREAMING_SERVER=0.18.0
# Thu, 22 Oct 2020 07:52:35 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='ff2a51618b79685264f980fe868f1c7af583c419b6406cc63d4811f3c98ca8fe' ;; 		armhf) natsArch='arm6'; sha256='629e17255f12fd80e051772a6dd18a7f65e692b4abef0786b421eb8b6ab85db4' ;; 		armv7) natsArch='arm7'; sha256='94e499af6a6391519315e8bcd5127c43c1d1a442ef945956286e77b4366c92c9' ;; 		x86_64) natsArch='amd64'; sha256='6252e9262efc81a41ade3f43b68e014d1e635d3e3bf9cbcd2b09c3a030a0d5e6' ;; 		x86) natsArch='386'; sha256='886ebd2e5eb99e30ff9e9d8907d7bd49dafacffce1dc921427e5754a4ec26f55' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 22 Oct 2020 07:52:35 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Thu, 22 Oct 2020 07:52:35 GMT
EXPOSE 4222 8222
# Thu, 22 Oct 2020 07:52:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Oct 2020 07:52:35 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:188c0c94c7c576fff0792aca7ec73d67a2f7f4cb3a6e53a84559337260b36964`  
		Last Modified: Thu, 22 Oct 2020 02:19:57 GMT  
		Size: 2.8 MB (2796860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c76f4b5e5eeb12aee0c5f3546936bba2ab032e31435700df0ee99b613ee90035`  
		Last Modified: Thu, 22 Oct 2020 07:53:08 GMT  
		Size: 6.2 MB (6217252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8085ae4fc692a672c22fa027b363dd68a7ff97e2a7843c8dffaedb93d6531f18`  
		Last Modified: Thu, 22 Oct 2020 07:53:07 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:2a58d6644e94cc17212ec6a604029ebe9f855ceeee7fa66171bdc8aa6c7113ba
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.9 MB (8932203 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b8391afd58a04ec8cf1ab166357c9495c5aa4d32bc4bb4472e577874f42fe55d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Thu, 22 Oct 2020 02:01:09 GMT
ADD file:dec4d3b6cf21c59820d1d74a554d0a193b5f4859e00b932f31ffe73f554d5afb in / 
# Thu, 22 Oct 2020 02:01:12 GMT
CMD ["/bin/sh"]
# Mon, 02 Nov 2020 23:56:13 GMT
ENV NATS_STREAMING_SERVER=0.19.0
# Mon, 02 Nov 2020 23:56:17 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='d582023b8f9fe33b98f0faa6396aae8d5366ecade7e56cde912e21e5b93ea670' ;; 		armhf) natsArch='arm6'; sha256='f4af03e6cbb19f3ad9ea57217607dcf4b68018e1879859c847e2680917fc7139' ;; 		armv7) natsArch='arm7'; sha256='ec8c5ca693344e8b24de9ac955c38de757af8c5760658fc29ed2fbd804803fad' ;; 		x86_64) natsArch='amd64'; sha256='fc15530faec66b61de5140c2b99927c5839caff1c4c17f8bffbf4432fab83017' ;; 		x86) natsArch='386'; sha256='655f0f7cebf727317974006ad4a13ddacd3520f15266e854c2b01681e499bf80' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Mon, 02 Nov 2020 23:56:17 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Mon, 02 Nov 2020 23:56:18 GMT
EXPOSE 4222 8222
# Mon, 02 Nov 2020 23:56:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 02 Nov 2020 23:56:19 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:bad30e7b45c14f784ef29a828b5fc69db0ebdefebcde6a7c98f4f77ffc93a546`  
		Last Modified: Thu, 22 Oct 2020 02:01:42 GMT  
		Size: 2.6 MB (2601912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21cba1ed5b5094a02c017d654b758674905ec0bb2535d3311fcdd61dce32b319`  
		Last Modified: Mon, 02 Nov 2020 23:56:50 GMT  
		Size: 6.3 MB (6329871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3992f15ff4c1a7660c4a81854ec33d3e4973405c7095ceb0bd8a7865fff21c9f`  
		Last Modified: Mon, 02 Nov 2020 23:56:47 GMT  
		Size: 420.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:6a6c52fc272b91cff878ca25bddc432f19583a2e41e5e92288f0e64d0c649896
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.7 MB (8730479 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b4347330ee2d9b26f7fafaadc370627e71670505b340c9e4b54d791afcb3a6b2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Thu, 22 Oct 2020 01:58:13 GMT
ADD file:46f89172426e9f5b1d669a2ca7ab218fc2deaef1caeeab88f2b5bd443ac9773d in / 
# Thu, 22 Oct 2020 01:58:14 GMT
CMD ["/bin/sh"]
# Tue, 03 Nov 2020 00:05:05 GMT
ENV NATS_STREAMING_SERVER=0.19.0
# Tue, 03 Nov 2020 00:05:09 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='d582023b8f9fe33b98f0faa6396aae8d5366ecade7e56cde912e21e5b93ea670' ;; 		armhf) natsArch='arm6'; sha256='f4af03e6cbb19f3ad9ea57217607dcf4b68018e1879859c847e2680917fc7139' ;; 		armv7) natsArch='arm7'; sha256='ec8c5ca693344e8b24de9ac955c38de757af8c5760658fc29ed2fbd804803fad' ;; 		x86_64) natsArch='amd64'; sha256='fc15530faec66b61de5140c2b99927c5839caff1c4c17f8bffbf4432fab83017' ;; 		x86) natsArch='386'; sha256='655f0f7cebf727317974006ad4a13ddacd3520f15266e854c2b01681e499bf80' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Tue, 03 Nov 2020 00:05:09 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Tue, 03 Nov 2020 00:05:10 GMT
EXPOSE 4222 8222
# Tue, 03 Nov 2020 00:05:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 03 Nov 2020 00:05:11 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:5f2023fd85a4e68f37fe41421fd89f30e69b98a645613521c57c01317561eee3`  
		Last Modified: Thu, 22 Oct 2020 01:58:45 GMT  
		Size: 2.4 MB (2405675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34033d6dabe9c0f77f765bf2fce39f1eef24c163cfa802ec78f0e2e1bea9da7c`  
		Last Modified: Tue, 03 Nov 2020 00:05:43 GMT  
		Size: 6.3 MB (6324384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b0a98c9d7b5d859df80140920031b236b38ff88a4ff09d3bf8cfc5b9776e436`  
		Last Modified: Tue, 03 Nov 2020 00:05:40 GMT  
		Size: 420.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:daaf0fb6b7f6fef7a7bf1a77c3870fbdd06674e2a484edaf9e4ab899c437ce19
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.5 MB (8457874 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5656790a7a499d508511728804d36a7c0dd43a0da379b16c60dd0caf5db8038f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Thu, 22 Oct 2020 02:01:01 GMT
ADD file:55c4e9752146061a2b5f76027221329f423687987c0744ef577130c60ff0ba42 in / 
# Thu, 22 Oct 2020 02:01:06 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 04:50:51 GMT
ENV NATS_STREAMING_SERVER=0.18.0
# Thu, 22 Oct 2020 04:51:52 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='ff2a51618b79685264f980fe868f1c7af583c419b6406cc63d4811f3c98ca8fe' ;; 		armhf) natsArch='arm6'; sha256='629e17255f12fd80e051772a6dd18a7f65e692b4abef0786b421eb8b6ab85db4' ;; 		armv7) natsArch='arm7'; sha256='94e499af6a6391519315e8bcd5127c43c1d1a442ef945956286e77b4366c92c9' ;; 		x86_64) natsArch='amd64'; sha256='6252e9262efc81a41ade3f43b68e014d1e635d3e3bf9cbcd2b09c3a030a0d5e6' ;; 		x86) natsArch='386'; sha256='886ebd2e5eb99e30ff9e9d8907d7bd49dafacffce1dc921427e5754a4ec26f55' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 22 Oct 2020 04:52:07 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Thu, 22 Oct 2020 04:52:15 GMT
EXPOSE 4222 8222
# Thu, 22 Oct 2020 04:52:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Oct 2020 04:52:45 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:5f621e34cdf485f410766dc9a0fc7855d17916d0f6583b58cbdce7c28831f527`  
		Last Modified: Thu, 22 Oct 2020 02:01:38 GMT  
		Size: 2.7 MB (2706555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc30703e8fb5cc62462a7b6e574e4d799c7007d721c62f25a94fccab3d01e822`  
		Last Modified: Thu, 22 Oct 2020 04:54:32 GMT  
		Size: 5.8 MB (5750897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30d9a7dd3da884d035a9f0595c38c9a25698f83a0b57102f0a0132d5d2c7f5b2`  
		Last Modified: Thu, 22 Oct 2020 04:54:32 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:alpine3.12`

```console
$ docker pull nats-streaming@sha256:31cfb9794a53c308e59076c863ac375b3fc53c2fa800152a271df02ad7f71f2a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:alpine3.12` - linux; amd64

```console
$ docker pull nats-streaming@sha256:26c179bfe34f31c821aa7b38083c0d4d3d96977eb3864d3c5a15157997b3f643
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.0 MB (9014534 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae46b411ada6bf35dd2255a5183b0e47b3c82be305fc90ef424e1ee01f6ecb50`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Thu, 22 Oct 2020 02:19:24 GMT
ADD file:f17f65714f703db9012f00e5ec98d0b2541ff6147c2633f7ab9ba659d0c507f4 in / 
# Thu, 22 Oct 2020 02:19:24 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 07:52:32 GMT
ENV NATS_STREAMING_SERVER=0.18.0
# Thu, 22 Oct 2020 07:52:35 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='ff2a51618b79685264f980fe868f1c7af583c419b6406cc63d4811f3c98ca8fe' ;; 		armhf) natsArch='arm6'; sha256='629e17255f12fd80e051772a6dd18a7f65e692b4abef0786b421eb8b6ab85db4' ;; 		armv7) natsArch='arm7'; sha256='94e499af6a6391519315e8bcd5127c43c1d1a442ef945956286e77b4366c92c9' ;; 		x86_64) natsArch='amd64'; sha256='6252e9262efc81a41ade3f43b68e014d1e635d3e3bf9cbcd2b09c3a030a0d5e6' ;; 		x86) natsArch='386'; sha256='886ebd2e5eb99e30ff9e9d8907d7bd49dafacffce1dc921427e5754a4ec26f55' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 22 Oct 2020 07:52:35 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Thu, 22 Oct 2020 07:52:35 GMT
EXPOSE 4222 8222
# Thu, 22 Oct 2020 07:52:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Oct 2020 07:52:35 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:188c0c94c7c576fff0792aca7ec73d67a2f7f4cb3a6e53a84559337260b36964`  
		Last Modified: Thu, 22 Oct 2020 02:19:57 GMT  
		Size: 2.8 MB (2796860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c76f4b5e5eeb12aee0c5f3546936bba2ab032e31435700df0ee99b613ee90035`  
		Last Modified: Thu, 22 Oct 2020 07:53:08 GMT  
		Size: 6.2 MB (6217252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8085ae4fc692a672c22fa027b363dd68a7ff97e2a7843c8dffaedb93d6531f18`  
		Last Modified: Thu, 22 Oct 2020 07:53:07 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine3.12` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:2a58d6644e94cc17212ec6a604029ebe9f855ceeee7fa66171bdc8aa6c7113ba
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.9 MB (8932203 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b8391afd58a04ec8cf1ab166357c9495c5aa4d32bc4bb4472e577874f42fe55d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Thu, 22 Oct 2020 02:01:09 GMT
ADD file:dec4d3b6cf21c59820d1d74a554d0a193b5f4859e00b932f31ffe73f554d5afb in / 
# Thu, 22 Oct 2020 02:01:12 GMT
CMD ["/bin/sh"]
# Mon, 02 Nov 2020 23:56:13 GMT
ENV NATS_STREAMING_SERVER=0.19.0
# Mon, 02 Nov 2020 23:56:17 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='d582023b8f9fe33b98f0faa6396aae8d5366ecade7e56cde912e21e5b93ea670' ;; 		armhf) natsArch='arm6'; sha256='f4af03e6cbb19f3ad9ea57217607dcf4b68018e1879859c847e2680917fc7139' ;; 		armv7) natsArch='arm7'; sha256='ec8c5ca693344e8b24de9ac955c38de757af8c5760658fc29ed2fbd804803fad' ;; 		x86_64) natsArch='amd64'; sha256='fc15530faec66b61de5140c2b99927c5839caff1c4c17f8bffbf4432fab83017' ;; 		x86) natsArch='386'; sha256='655f0f7cebf727317974006ad4a13ddacd3520f15266e854c2b01681e499bf80' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Mon, 02 Nov 2020 23:56:17 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Mon, 02 Nov 2020 23:56:18 GMT
EXPOSE 4222 8222
# Mon, 02 Nov 2020 23:56:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 02 Nov 2020 23:56:19 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:bad30e7b45c14f784ef29a828b5fc69db0ebdefebcde6a7c98f4f77ffc93a546`  
		Last Modified: Thu, 22 Oct 2020 02:01:42 GMT  
		Size: 2.6 MB (2601912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21cba1ed5b5094a02c017d654b758674905ec0bb2535d3311fcdd61dce32b319`  
		Last Modified: Mon, 02 Nov 2020 23:56:50 GMT  
		Size: 6.3 MB (6329871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3992f15ff4c1a7660c4a81854ec33d3e4973405c7095ceb0bd8a7865fff21c9f`  
		Last Modified: Mon, 02 Nov 2020 23:56:47 GMT  
		Size: 420.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine3.12` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:6a6c52fc272b91cff878ca25bddc432f19583a2e41e5e92288f0e64d0c649896
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.7 MB (8730479 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b4347330ee2d9b26f7fafaadc370627e71670505b340c9e4b54d791afcb3a6b2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Thu, 22 Oct 2020 01:58:13 GMT
ADD file:46f89172426e9f5b1d669a2ca7ab218fc2deaef1caeeab88f2b5bd443ac9773d in / 
# Thu, 22 Oct 2020 01:58:14 GMT
CMD ["/bin/sh"]
# Tue, 03 Nov 2020 00:05:05 GMT
ENV NATS_STREAMING_SERVER=0.19.0
# Tue, 03 Nov 2020 00:05:09 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='d582023b8f9fe33b98f0faa6396aae8d5366ecade7e56cde912e21e5b93ea670' ;; 		armhf) natsArch='arm6'; sha256='f4af03e6cbb19f3ad9ea57217607dcf4b68018e1879859c847e2680917fc7139' ;; 		armv7) natsArch='arm7'; sha256='ec8c5ca693344e8b24de9ac955c38de757af8c5760658fc29ed2fbd804803fad' ;; 		x86_64) natsArch='amd64'; sha256='fc15530faec66b61de5140c2b99927c5839caff1c4c17f8bffbf4432fab83017' ;; 		x86) natsArch='386'; sha256='655f0f7cebf727317974006ad4a13ddacd3520f15266e854c2b01681e499bf80' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Tue, 03 Nov 2020 00:05:09 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Tue, 03 Nov 2020 00:05:10 GMT
EXPOSE 4222 8222
# Tue, 03 Nov 2020 00:05:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 03 Nov 2020 00:05:11 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:5f2023fd85a4e68f37fe41421fd89f30e69b98a645613521c57c01317561eee3`  
		Last Modified: Thu, 22 Oct 2020 01:58:45 GMT  
		Size: 2.4 MB (2405675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34033d6dabe9c0f77f765bf2fce39f1eef24c163cfa802ec78f0e2e1bea9da7c`  
		Last Modified: Tue, 03 Nov 2020 00:05:43 GMT  
		Size: 6.3 MB (6324384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b0a98c9d7b5d859df80140920031b236b38ff88a4ff09d3bf8cfc5b9776e436`  
		Last Modified: Tue, 03 Nov 2020 00:05:40 GMT  
		Size: 420.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine3.12` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:daaf0fb6b7f6fef7a7bf1a77c3870fbdd06674e2a484edaf9e4ab899c437ce19
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.5 MB (8457874 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5656790a7a499d508511728804d36a7c0dd43a0da379b16c60dd0caf5db8038f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Thu, 22 Oct 2020 02:01:01 GMT
ADD file:55c4e9752146061a2b5f76027221329f423687987c0744ef577130c60ff0ba42 in / 
# Thu, 22 Oct 2020 02:01:06 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 04:50:51 GMT
ENV NATS_STREAMING_SERVER=0.18.0
# Thu, 22 Oct 2020 04:51:52 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='ff2a51618b79685264f980fe868f1c7af583c419b6406cc63d4811f3c98ca8fe' ;; 		armhf) natsArch='arm6'; sha256='629e17255f12fd80e051772a6dd18a7f65e692b4abef0786b421eb8b6ab85db4' ;; 		armv7) natsArch='arm7'; sha256='94e499af6a6391519315e8bcd5127c43c1d1a442ef945956286e77b4366c92c9' ;; 		x86_64) natsArch='amd64'; sha256='6252e9262efc81a41ade3f43b68e014d1e635d3e3bf9cbcd2b09c3a030a0d5e6' ;; 		x86) natsArch='386'; sha256='886ebd2e5eb99e30ff9e9d8907d7bd49dafacffce1dc921427e5754a4ec26f55' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 22 Oct 2020 04:52:07 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Thu, 22 Oct 2020 04:52:15 GMT
EXPOSE 4222 8222
# Thu, 22 Oct 2020 04:52:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Oct 2020 04:52:45 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:5f621e34cdf485f410766dc9a0fc7855d17916d0f6583b58cbdce7c28831f527`  
		Last Modified: Thu, 22 Oct 2020 02:01:38 GMT  
		Size: 2.7 MB (2706555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc30703e8fb5cc62462a7b6e574e4d799c7007d721c62f25a94fccab3d01e822`  
		Last Modified: Thu, 22 Oct 2020 04:54:32 GMT  
		Size: 5.8 MB (5750897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30d9a7dd3da884d035a9f0595c38c9a25698f83a0b57102f0a0132d5d2c7f5b2`  
		Last Modified: Thu, 22 Oct 2020 04:54:32 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:latest`

```console
$ docker pull nats-streaming@sha256:a4b9bf1b8bc1b7daae162cf9df407e40a3cbbc8aff30388506199ab1872801e6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.1518; amd64

### `nats-streaming:latest` - linux; amd64

```console
$ docker pull nats-streaming@sha256:eff8b99b0e3d89b6161ceb975a8c1ca063ac9a8e868eed448736a866551357ca
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 MB (5936411 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51d28dc2950a94ff3d73d86750b57ba3c6dae964c671dbac699c2f17eecd5880`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 25 Jun 2020 19:25:44 GMT
COPY file:6241d3a0b9f20d843fc13c1bd49fd4376e4daae879837447249456f65dfe9ead in /nats-streaming-server 
# Thu, 25 Jun 2020 19:25:44 GMT
EXPOSE 4222 8222
# Thu, 25 Jun 2020 19:25:44 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Thu, 25 Jun 2020 19:25:44 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:908e6af6575b3ee0ca4b089b18f72d87607c39809caeee4bb662b347aa23b895`  
		Last Modified: Thu, 25 Jun 2020 19:26:07 GMT  
		Size: 5.9 MB (5936411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:latest` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:f334d10ef2a4663d8d7d920d96321cd97f050b82a5d55d588192f074f60dd814
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 MB (6049845 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9eecfd5ab4178a65e952a7cf1d248a556a6ae2c328ac8b68923146d64734db03`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 02 Nov 2020 23:56:28 GMT
COPY file:d6896b1c93dcd497494c972f9274fcc634a4f4a8d63a0191bdb87f6336aec0d7 in /nats-streaming-server 
# Mon, 02 Nov 2020 23:56:28 GMT
EXPOSE 4222 8222
# Mon, 02 Nov 2020 23:56:29 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 02 Nov 2020 23:56:29 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:7f165fb71ab77e8081dbfa13656cdf9e5e005002d6c3afa0aac40667a0f97af8`  
		Last Modified: Mon, 02 Nov 2020 23:57:04 GMT  
		Size: 6.0 MB (6049845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:latest` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:5fd0943909d8aedafb888e099c9f64d234023ad780805ed7c939692ebfd8304d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 MB (6043163 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f37071e856ae40dc3c8c5e10b359d1640fd67a6110741c0957af2031032ed6ce`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 03 Nov 2020 00:05:23 GMT
COPY file:d232132ddff1d85d3a2f5c80a91c80023cbc103d816387e06d604cf97238e52c in /nats-streaming-server 
# Tue, 03 Nov 2020 00:05:24 GMT
EXPOSE 4222 8222
# Tue, 03 Nov 2020 00:05:24 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 03 Nov 2020 00:05:25 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:9c7227cc1040d04ca7763cfb53ab58bc32ae54921990516adf8e13374ac9ef29`  
		Last Modified: Tue, 03 Nov 2020 00:05:57 GMT  
		Size: 6.0 MB (6043163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:latest` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:ed524c7b14a4b6e91428f8c765455f742c4351657468296a8b63bdefecd5ceb1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.5 MB (5469641 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2424d5ea5176bb2af173ccb2222a5d39ff53c785fdad2bfc1045d5c66aee5185`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Wed, 29 Jul 2020 22:40:10 GMT
COPY file:f3f47d8e20155d8cbd02ab8a9f26c3be2763cf0430c38ab1071fb6949f9e466c in /nats-streaming-server 
# Wed, 29 Jul 2020 22:40:11 GMT
EXPOSE 4222 8222
# Wed, 29 Jul 2020 22:40:11 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Wed, 29 Jul 2020 22:40:12 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:58414d7c10a2a92ebdcb56bcf4a04f62f2f370c1e415c008fda228ab012a1a45`  
		Last Modified: Wed, 29 Jul 2020 22:40:42 GMT  
		Size: 5.5 MB (5469641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:latest` - windows version 10.0.17763.1518; amd64

```console
$ docker pull nats-streaming@sha256:5fe78c067270813d55b50f43526093fa5887e6ce0b17e50068d9fd2f013f5af7
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.2 MB (107152777 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2f1c8cf4a6107c2adfb5131e75eb07af94b224315df507b07c2647e7995407c`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Wed, 30 Sep 2020 11:25:56 GMT
RUN Apply image 1809-amd64
# Wed, 14 Oct 2020 16:26:27 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 14 Oct 2020 21:18:22 GMT
RUN cmd /S /C #(nop) COPY file:4a858ac4da943f868519572e3fb6817fd379875f2bff0bcb5f03c5bdddc496a8 in C:\nats-streaming-server.exe 
# Wed, 14 Oct 2020 21:18:24 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 14 Oct 2020 21:18:24 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 14 Oct 2020 21:18:25 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:aab6118ce69c93410df7fa15842a6e3b3c7ff20b639c779b5d5f78e7653eaa07`  
		Size: 101.2 MB (101205155 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:93b9a3c3e46fc1677426e3be7ce449b91d540c5ae2147380034cc4e1dc7445c3`  
		Last Modified: Wed, 14 Oct 2020 16:31:12 GMT  
		Size: 910.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:769b7d23be974b2320a99d82b94318b3e5273830bcaaa7298b1312a50c704a91`  
		Last Modified: Wed, 14 Oct 2020 21:22:27 GMT  
		Size: 5.9 MB (5944112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcdd787a9d9610ed9d1a66cfb6ccebc8bdfa4c957a79fd5423a2fae39a80bcd5`  
		Last Modified: Wed, 14 Oct 2020 21:22:24 GMT  
		Size: 866.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53d49f0c5dabaf0f2ab4c562171ac5a0715778b723068c6ed01eb5c0d99b7090`  
		Last Modified: Wed, 14 Oct 2020 21:22:25 GMT  
		Size: 869.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa13689bfb5655cc9da97e67c2acaf2293b4f8f07dffaa7f1a7c2cbaa570e83a`  
		Last Modified: Wed, 14 Oct 2020 21:22:26 GMT  
		Size: 865.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:linux`

```console
$ docker pull nats-streaming@sha256:8df5984380dbe779b490ebe2082c1000b06de56790cd3d47be6df854407d3c31
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:linux` - linux; amd64

```console
$ docker pull nats-streaming@sha256:eff8b99b0e3d89b6161ceb975a8c1ca063ac9a8e868eed448736a866551357ca
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 MB (5936411 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51d28dc2950a94ff3d73d86750b57ba3c6dae964c671dbac699c2f17eecd5880`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 25 Jun 2020 19:25:44 GMT
COPY file:6241d3a0b9f20d843fc13c1bd49fd4376e4daae879837447249456f65dfe9ead in /nats-streaming-server 
# Thu, 25 Jun 2020 19:25:44 GMT
EXPOSE 4222 8222
# Thu, 25 Jun 2020 19:25:44 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Thu, 25 Jun 2020 19:25:44 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:908e6af6575b3ee0ca4b089b18f72d87607c39809caeee4bb662b347aa23b895`  
		Last Modified: Thu, 25 Jun 2020 19:26:07 GMT  
		Size: 5.9 MB (5936411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:linux` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:f334d10ef2a4663d8d7d920d96321cd97f050b82a5d55d588192f074f60dd814
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 MB (6049845 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9eecfd5ab4178a65e952a7cf1d248a556a6ae2c328ac8b68923146d64734db03`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 02 Nov 2020 23:56:28 GMT
COPY file:d6896b1c93dcd497494c972f9274fcc634a4f4a8d63a0191bdb87f6336aec0d7 in /nats-streaming-server 
# Mon, 02 Nov 2020 23:56:28 GMT
EXPOSE 4222 8222
# Mon, 02 Nov 2020 23:56:29 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 02 Nov 2020 23:56:29 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:7f165fb71ab77e8081dbfa13656cdf9e5e005002d6c3afa0aac40667a0f97af8`  
		Last Modified: Mon, 02 Nov 2020 23:57:04 GMT  
		Size: 6.0 MB (6049845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:linux` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:5fd0943909d8aedafb888e099c9f64d234023ad780805ed7c939692ebfd8304d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 MB (6043163 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f37071e856ae40dc3c8c5e10b359d1640fd67a6110741c0957af2031032ed6ce`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 03 Nov 2020 00:05:23 GMT
COPY file:d232132ddff1d85d3a2f5c80a91c80023cbc103d816387e06d604cf97238e52c in /nats-streaming-server 
# Tue, 03 Nov 2020 00:05:24 GMT
EXPOSE 4222 8222
# Tue, 03 Nov 2020 00:05:24 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 03 Nov 2020 00:05:25 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:9c7227cc1040d04ca7763cfb53ab58bc32ae54921990516adf8e13374ac9ef29`  
		Last Modified: Tue, 03 Nov 2020 00:05:57 GMT  
		Size: 6.0 MB (6043163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:linux` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:ed524c7b14a4b6e91428f8c765455f742c4351657468296a8b63bdefecd5ceb1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.5 MB (5469641 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2424d5ea5176bb2af173ccb2222a5d39ff53c785fdad2bfc1045d5c66aee5185`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Wed, 29 Jul 2020 22:40:10 GMT
COPY file:f3f47d8e20155d8cbd02ab8a9f26c3be2763cf0430c38ab1071fb6949f9e466c in /nats-streaming-server 
# Wed, 29 Jul 2020 22:40:11 GMT
EXPOSE 4222 8222
# Wed, 29 Jul 2020 22:40:11 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Wed, 29 Jul 2020 22:40:12 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:58414d7c10a2a92ebdcb56bcf4a04f62f2f370c1e415c008fda228ab012a1a45`  
		Last Modified: Wed, 29 Jul 2020 22:40:42 GMT  
		Size: 5.5 MB (5469641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:nanoserver`

```console
$ docker pull nats-streaming@sha256:1e5b89da01e9359e18bce50086ba40b514492eff4a7979976f08ddd7cda0e7eb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1518; amd64

### `nats-streaming:nanoserver` - windows version 10.0.17763.1518; amd64

```console
$ docker pull nats-streaming@sha256:5fe78c067270813d55b50f43526093fa5887e6ce0b17e50068d9fd2f013f5af7
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.2 MB (107152777 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2f1c8cf4a6107c2adfb5131e75eb07af94b224315df507b07c2647e7995407c`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Wed, 30 Sep 2020 11:25:56 GMT
RUN Apply image 1809-amd64
# Wed, 14 Oct 2020 16:26:27 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 14 Oct 2020 21:18:22 GMT
RUN cmd /S /C #(nop) COPY file:4a858ac4da943f868519572e3fb6817fd379875f2bff0bcb5f03c5bdddc496a8 in C:\nats-streaming-server.exe 
# Wed, 14 Oct 2020 21:18:24 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 14 Oct 2020 21:18:24 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 14 Oct 2020 21:18:25 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:aab6118ce69c93410df7fa15842a6e3b3c7ff20b639c779b5d5f78e7653eaa07`  
		Size: 101.2 MB (101205155 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:93b9a3c3e46fc1677426e3be7ce449b91d540c5ae2147380034cc4e1dc7445c3`  
		Last Modified: Wed, 14 Oct 2020 16:31:12 GMT  
		Size: 910.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:769b7d23be974b2320a99d82b94318b3e5273830bcaaa7298b1312a50c704a91`  
		Last Modified: Wed, 14 Oct 2020 21:22:27 GMT  
		Size: 5.9 MB (5944112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcdd787a9d9610ed9d1a66cfb6ccebc8bdfa4c957a79fd5423a2fae39a80bcd5`  
		Last Modified: Wed, 14 Oct 2020 21:22:24 GMT  
		Size: 866.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53d49f0c5dabaf0f2ab4c562171ac5a0715778b723068c6ed01eb5c0d99b7090`  
		Last Modified: Wed, 14 Oct 2020 21:22:25 GMT  
		Size: 869.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa13689bfb5655cc9da97e67c2acaf2293b4f8f07dffaa7f1a7c2cbaa570e83a`  
		Last Modified: Wed, 14 Oct 2020 21:22:26 GMT  
		Size: 865.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:nanoserver-1809`

```console
$ docker pull nats-streaming@sha256:1e5b89da01e9359e18bce50086ba40b514492eff4a7979976f08ddd7cda0e7eb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1518; amd64

### `nats-streaming:nanoserver-1809` - windows version 10.0.17763.1518; amd64

```console
$ docker pull nats-streaming@sha256:5fe78c067270813d55b50f43526093fa5887e6ce0b17e50068d9fd2f013f5af7
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.2 MB (107152777 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2f1c8cf4a6107c2adfb5131e75eb07af94b224315df507b07c2647e7995407c`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Wed, 30 Sep 2020 11:25:56 GMT
RUN Apply image 1809-amd64
# Wed, 14 Oct 2020 16:26:27 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 14 Oct 2020 21:18:22 GMT
RUN cmd /S /C #(nop) COPY file:4a858ac4da943f868519572e3fb6817fd379875f2bff0bcb5f03c5bdddc496a8 in C:\nats-streaming-server.exe 
# Wed, 14 Oct 2020 21:18:24 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 14 Oct 2020 21:18:24 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 14 Oct 2020 21:18:25 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:aab6118ce69c93410df7fa15842a6e3b3c7ff20b639c779b5d5f78e7653eaa07`  
		Size: 101.2 MB (101205155 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:93b9a3c3e46fc1677426e3be7ce449b91d540c5ae2147380034cc4e1dc7445c3`  
		Last Modified: Wed, 14 Oct 2020 16:31:12 GMT  
		Size: 910.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:769b7d23be974b2320a99d82b94318b3e5273830bcaaa7298b1312a50c704a91`  
		Last Modified: Wed, 14 Oct 2020 21:22:27 GMT  
		Size: 5.9 MB (5944112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcdd787a9d9610ed9d1a66cfb6ccebc8bdfa4c957a79fd5423a2fae39a80bcd5`  
		Last Modified: Wed, 14 Oct 2020 21:22:24 GMT  
		Size: 866.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53d49f0c5dabaf0f2ab4c562171ac5a0715778b723068c6ed01eb5c0d99b7090`  
		Last Modified: Wed, 14 Oct 2020 21:22:25 GMT  
		Size: 869.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa13689bfb5655cc9da97e67c2acaf2293b4f8f07dffaa7f1a7c2cbaa570e83a`  
		Last Modified: Wed, 14 Oct 2020 21:22:26 GMT  
		Size: 865.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:scratch`

```console
$ docker pull nats-streaming@sha256:8df5984380dbe779b490ebe2082c1000b06de56790cd3d47be6df854407d3c31
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:scratch` - linux; amd64

```console
$ docker pull nats-streaming@sha256:eff8b99b0e3d89b6161ceb975a8c1ca063ac9a8e868eed448736a866551357ca
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 MB (5936411 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51d28dc2950a94ff3d73d86750b57ba3c6dae964c671dbac699c2f17eecd5880`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 25 Jun 2020 19:25:44 GMT
COPY file:6241d3a0b9f20d843fc13c1bd49fd4376e4daae879837447249456f65dfe9ead in /nats-streaming-server 
# Thu, 25 Jun 2020 19:25:44 GMT
EXPOSE 4222 8222
# Thu, 25 Jun 2020 19:25:44 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Thu, 25 Jun 2020 19:25:44 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:908e6af6575b3ee0ca4b089b18f72d87607c39809caeee4bb662b347aa23b895`  
		Last Modified: Thu, 25 Jun 2020 19:26:07 GMT  
		Size: 5.9 MB (5936411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:scratch` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:f334d10ef2a4663d8d7d920d96321cd97f050b82a5d55d588192f074f60dd814
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 MB (6049845 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9eecfd5ab4178a65e952a7cf1d248a556a6ae2c328ac8b68923146d64734db03`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 02 Nov 2020 23:56:28 GMT
COPY file:d6896b1c93dcd497494c972f9274fcc634a4f4a8d63a0191bdb87f6336aec0d7 in /nats-streaming-server 
# Mon, 02 Nov 2020 23:56:28 GMT
EXPOSE 4222 8222
# Mon, 02 Nov 2020 23:56:29 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 02 Nov 2020 23:56:29 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:7f165fb71ab77e8081dbfa13656cdf9e5e005002d6c3afa0aac40667a0f97af8`  
		Last Modified: Mon, 02 Nov 2020 23:57:04 GMT  
		Size: 6.0 MB (6049845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:scratch` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:5fd0943909d8aedafb888e099c9f64d234023ad780805ed7c939692ebfd8304d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 MB (6043163 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f37071e856ae40dc3c8c5e10b359d1640fd67a6110741c0957af2031032ed6ce`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 03 Nov 2020 00:05:23 GMT
COPY file:d232132ddff1d85d3a2f5c80a91c80023cbc103d816387e06d604cf97238e52c in /nats-streaming-server 
# Tue, 03 Nov 2020 00:05:24 GMT
EXPOSE 4222 8222
# Tue, 03 Nov 2020 00:05:24 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 03 Nov 2020 00:05:25 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:9c7227cc1040d04ca7763cfb53ab58bc32ae54921990516adf8e13374ac9ef29`  
		Last Modified: Tue, 03 Nov 2020 00:05:57 GMT  
		Size: 6.0 MB (6043163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:scratch` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:ed524c7b14a4b6e91428f8c765455f742c4351657468296a8b63bdefecd5ceb1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.5 MB (5469641 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2424d5ea5176bb2af173ccb2222a5d39ff53c785fdad2bfc1045d5c66aee5185`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Wed, 29 Jul 2020 22:40:10 GMT
COPY file:f3f47d8e20155d8cbd02ab8a9f26c3be2763cf0430c38ab1071fb6949f9e466c in /nats-streaming-server 
# Wed, 29 Jul 2020 22:40:11 GMT
EXPOSE 4222 8222
# Wed, 29 Jul 2020 22:40:11 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Wed, 29 Jul 2020 22:40:12 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:58414d7c10a2a92ebdcb56bcf4a04f62f2f370c1e415c008fda228ab012a1a45`  
		Last Modified: Wed, 29 Jul 2020 22:40:42 GMT  
		Size: 5.5 MB (5469641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:windowsservercore`

```console
$ docker pull nats-streaming@sha256:703f5c6e18f6b6fb9a71e02e82d60dd49a81a1d8a019d63b0e69638f48308655
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1518; amd64
	-	windows version 10.0.14393.3986; amd64

### `nats-streaming:windowsservercore` - windows version 10.0.17763.1518; amd64

```console
$ docker pull nats-streaming@sha256:70b42a44e4c316c6ecc48df4fb62c4db99d13b04c89328cd36dd8efdb19989ca
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2394083789 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b1437375b044d88a76f1ab92ff2d13179e676433420499971157766876878f2`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 01 Oct 2020 02:26:38 GMT
RUN Install update 1809-amd64
# Wed, 14 Oct 2020 12:58:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 14 Oct 2020 16:24:30 GMT
ENV NATS_DOCKERIZED=1
# Wed, 14 Oct 2020 21:16:23 GMT
ENV NATS_STREAMING_SERVER=0.18.0
# Wed, 14 Oct 2020 21:16:24 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.18.0/nats-streaming-server-v0.18.0-windows-amd64.zip
# Wed, 14 Oct 2020 21:16:25 GMT
ENV GIT_DOWNLOAD_SHA256=a0c0261df2ce589fe9706617323e06c5bcae70511112eae921681b1169674bc8
# Wed, 14 Oct 2020 21:16:54 GMT
RUN Set-PSDebug -Trace 2
# Wed, 14 Oct 2020 21:18:13 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 14 Oct 2020 21:18:14 GMT
EXPOSE 4222 8222
# Wed, 14 Oct 2020 21:18:15 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 14 Oct 2020 21:18:16 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:406ffb8432a757e84f7594e85c676620dec6955e0475ac271aa4dd5c0531190d`  
		Size: 655.8 MB (655757265 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d839ec6fa74e5e869036dfd823e95452a7afcde18ac997af483c88c21b92ad8c`  
		Last Modified: Wed, 14 Oct 2020 16:02:33 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad001e4fbf5cfc7ed201221adacaa53c349e1df3803ec7e47dadb618535d55ab`  
		Last Modified: Wed, 14 Oct 2020 16:30:17 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fc6cb14531ba1a622448955b3b8cf69c5acdde60f2e96977e6d39f703a323e5`  
		Last Modified: Wed, 14 Oct 2020 21:22:04 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:284f49480b938a703154befeeb82ed7d66cedd399a196c26e8750c29bb27d01d`  
		Last Modified: Wed, 14 Oct 2020 21:22:03 GMT  
		Size: 1.1 KB (1141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:443f56bc014d6ed1b009eda85392ae23d5b87d9d44f330bef5eb1bd08093e26b`  
		Last Modified: Wed, 14 Oct 2020 21:22:03 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9560c003b35bf850722898a9b94bd691004d8cfb2b3c4854c4be9c5fec5e12d4`  
		Last Modified: Wed, 14 Oct 2020 21:22:01 GMT  
		Size: 4.8 MB (4842155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9625e22456a51048f7d722cfd4d43a0392737c7d33fd9feb4df1919f16bcc4cc`  
		Last Modified: Wed, 14 Oct 2020 21:22:04 GMT  
		Size: 15.1 MB (15142401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56a64e86100073b367da8bcf41924e6b24167d0b7301e35b37eae584ba719533`  
		Last Modified: Wed, 14 Oct 2020 21:22:00 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fabff48d9454c599eb2bfff68136f92d54db619cce1ae464b226cdfb7c252f28`  
		Last Modified: Wed, 14 Oct 2020 21:22:00 GMT  
		Size: 1.1 KB (1119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b47bdf371d62da958d9f95e23963ac11a7ede6a4c9bcf06c44afe2f51d6af14`  
		Last Modified: Wed, 14 Oct 2020 21:21:59 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:windowsservercore` - windows version 10.0.14393.3986; amd64

```console
$ docker pull nats-streaming@sha256:92df1036dfd3c72bcf7a142e21e3d1776e8d386bbef43a105bb3def3c9b8aec6
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5762657171 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:186129d9ce285a35807c00a5899c67f185d62239c091634ec5801f481613bc06`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Fri, 02 Oct 2020 17:07:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 14 Oct 2020 13:36:27 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 14 Oct 2020 16:26:37 GMT
ENV NATS_DOCKERIZED=1
# Wed, 14 Oct 2020 21:18:30 GMT
ENV NATS_STREAMING_SERVER=0.18.0
# Wed, 14 Oct 2020 21:18:31 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.18.0/nats-streaming-server-v0.18.0-windows-amd64.zip
# Wed, 14 Oct 2020 21:18:31 GMT
ENV GIT_DOWNLOAD_SHA256=a0c0261df2ce589fe9706617323e06c5bcae70511112eae921681b1169674bc8
# Wed, 14 Oct 2020 21:19:36 GMT
RUN Set-PSDebug -Trace 2
# Wed, 14 Oct 2020 21:21:34 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 14 Oct 2020 21:21:35 GMT
EXPOSE 4222 8222
# Wed, 14 Oct 2020 21:21:36 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 14 Oct 2020 21:21:37 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:17a32268498b2feefa5457f0423ac15473596d514e48c694ef54d740a9a5067d`  
		Size: 1.7 GB (1671365753 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bb0caa156c690c0274404e38041b8eb56dcd2c15edbc269fc4c619eb667cb7ff`  
		Last Modified: Wed, 14 Oct 2020 16:03:09 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abca8ce1a1e304feeddabd9e49e2e5fad5622924c75d97368a7fda9a6eacf3eb`  
		Last Modified: Wed, 14 Oct 2020 16:31:41 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:686b0a818740f1633b74c2225d6f031cc5715c09a4881a438a13fba93d307f25`  
		Last Modified: Wed, 14 Oct 2020 21:22:44 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d196c7cff012be9e007f86a2631135b35f4244060c069a7b117a74ada9de2fa7`  
		Last Modified: Wed, 14 Oct 2020 21:22:44 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23f009c551166c1757f25dd72ee5d85fc490974f9850ba13dc1648a96ccce42e`  
		Last Modified: Wed, 14 Oct 2020 21:22:43 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ace6d560181c9b8d74da192fecd5f17ff9c2972464f57308d6ab0a4bb5f028ad`  
		Last Modified: Wed, 14 Oct 2020 21:22:42 GMT  
		Size: 5.4 MB (5425219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f421d0869e3cbe5b8580ee0612ddfc8a9afe94d285d80db4f6659869c583c83`  
		Last Modified: Wed, 14 Oct 2020 21:22:45 GMT  
		Size: 15.9 MB (15871237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4d937f908a310fa9b1957cf7d45f93cdfede8f5fb275cdc998d945256ed08d6`  
		Last Modified: Wed, 14 Oct 2020 21:22:41 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24f3c49e9d40da03d9a3c60f34aa4e5819584d55c708216829aa3f00d408353f`  
		Last Modified: Wed, 14 Oct 2020 21:22:40 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2088679ebef164efa3ed0b7a7a70064336481303027587ac6bce796c5400bbab`  
		Last Modified: Wed, 14 Oct 2020 21:22:41 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:windowsservercore-1809`

```console
$ docker pull nats-streaming@sha256:d2a8ab1805575e9ca0eb21c568ea5bd01b41643f75dd2c2a39c1ec73eb7b7497
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1518; amd64

### `nats-streaming:windowsservercore-1809` - windows version 10.0.17763.1518; amd64

```console
$ docker pull nats-streaming@sha256:70b42a44e4c316c6ecc48df4fb62c4db99d13b04c89328cd36dd8efdb19989ca
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2394083789 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b1437375b044d88a76f1ab92ff2d13179e676433420499971157766876878f2`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 01 Oct 2020 02:26:38 GMT
RUN Install update 1809-amd64
# Wed, 14 Oct 2020 12:58:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 14 Oct 2020 16:24:30 GMT
ENV NATS_DOCKERIZED=1
# Wed, 14 Oct 2020 21:16:23 GMT
ENV NATS_STREAMING_SERVER=0.18.0
# Wed, 14 Oct 2020 21:16:24 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.18.0/nats-streaming-server-v0.18.0-windows-amd64.zip
# Wed, 14 Oct 2020 21:16:25 GMT
ENV GIT_DOWNLOAD_SHA256=a0c0261df2ce589fe9706617323e06c5bcae70511112eae921681b1169674bc8
# Wed, 14 Oct 2020 21:16:54 GMT
RUN Set-PSDebug -Trace 2
# Wed, 14 Oct 2020 21:18:13 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 14 Oct 2020 21:18:14 GMT
EXPOSE 4222 8222
# Wed, 14 Oct 2020 21:18:15 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 14 Oct 2020 21:18:16 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:406ffb8432a757e84f7594e85c676620dec6955e0475ac271aa4dd5c0531190d`  
		Size: 655.8 MB (655757265 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d839ec6fa74e5e869036dfd823e95452a7afcde18ac997af483c88c21b92ad8c`  
		Last Modified: Wed, 14 Oct 2020 16:02:33 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad001e4fbf5cfc7ed201221adacaa53c349e1df3803ec7e47dadb618535d55ab`  
		Last Modified: Wed, 14 Oct 2020 16:30:17 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fc6cb14531ba1a622448955b3b8cf69c5acdde60f2e96977e6d39f703a323e5`  
		Last Modified: Wed, 14 Oct 2020 21:22:04 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:284f49480b938a703154befeeb82ed7d66cedd399a196c26e8750c29bb27d01d`  
		Last Modified: Wed, 14 Oct 2020 21:22:03 GMT  
		Size: 1.1 KB (1141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:443f56bc014d6ed1b009eda85392ae23d5b87d9d44f330bef5eb1bd08093e26b`  
		Last Modified: Wed, 14 Oct 2020 21:22:03 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9560c003b35bf850722898a9b94bd691004d8cfb2b3c4854c4be9c5fec5e12d4`  
		Last Modified: Wed, 14 Oct 2020 21:22:01 GMT  
		Size: 4.8 MB (4842155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9625e22456a51048f7d722cfd4d43a0392737c7d33fd9feb4df1919f16bcc4cc`  
		Last Modified: Wed, 14 Oct 2020 21:22:04 GMT  
		Size: 15.1 MB (15142401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56a64e86100073b367da8bcf41924e6b24167d0b7301e35b37eae584ba719533`  
		Last Modified: Wed, 14 Oct 2020 21:22:00 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fabff48d9454c599eb2bfff68136f92d54db619cce1ae464b226cdfb7c252f28`  
		Last Modified: Wed, 14 Oct 2020 21:22:00 GMT  
		Size: 1.1 KB (1119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b47bdf371d62da958d9f95e23963ac11a7ede6a4c9bcf06c44afe2f51d6af14`  
		Last Modified: Wed, 14 Oct 2020 21:21:59 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:windowsservercore-ltsc2016`

```console
$ docker pull nats-streaming@sha256:806b8bf4edc8956db2e8fe23a961df238868b04a2700820d4fc838407abc255b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3986; amd64

### `nats-streaming:windowsservercore-ltsc2016` - windows version 10.0.14393.3986; amd64

```console
$ docker pull nats-streaming@sha256:92df1036dfd3c72bcf7a142e21e3d1776e8d386bbef43a105bb3def3c9b8aec6
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5762657171 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:186129d9ce285a35807c00a5899c67f185d62239c091634ec5801f481613bc06`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Fri, 02 Oct 2020 17:07:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 14 Oct 2020 13:36:27 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 14 Oct 2020 16:26:37 GMT
ENV NATS_DOCKERIZED=1
# Wed, 14 Oct 2020 21:18:30 GMT
ENV NATS_STREAMING_SERVER=0.18.0
# Wed, 14 Oct 2020 21:18:31 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.18.0/nats-streaming-server-v0.18.0-windows-amd64.zip
# Wed, 14 Oct 2020 21:18:31 GMT
ENV GIT_DOWNLOAD_SHA256=a0c0261df2ce589fe9706617323e06c5bcae70511112eae921681b1169674bc8
# Wed, 14 Oct 2020 21:19:36 GMT
RUN Set-PSDebug -Trace 2
# Wed, 14 Oct 2020 21:21:34 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 14 Oct 2020 21:21:35 GMT
EXPOSE 4222 8222
# Wed, 14 Oct 2020 21:21:36 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 14 Oct 2020 21:21:37 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:17a32268498b2feefa5457f0423ac15473596d514e48c694ef54d740a9a5067d`  
		Size: 1.7 GB (1671365753 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bb0caa156c690c0274404e38041b8eb56dcd2c15edbc269fc4c619eb667cb7ff`  
		Last Modified: Wed, 14 Oct 2020 16:03:09 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abca8ce1a1e304feeddabd9e49e2e5fad5622924c75d97368a7fda9a6eacf3eb`  
		Last Modified: Wed, 14 Oct 2020 16:31:41 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:686b0a818740f1633b74c2225d6f031cc5715c09a4881a438a13fba93d307f25`  
		Last Modified: Wed, 14 Oct 2020 21:22:44 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d196c7cff012be9e007f86a2631135b35f4244060c069a7b117a74ada9de2fa7`  
		Last Modified: Wed, 14 Oct 2020 21:22:44 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23f009c551166c1757f25dd72ee5d85fc490974f9850ba13dc1648a96ccce42e`  
		Last Modified: Wed, 14 Oct 2020 21:22:43 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ace6d560181c9b8d74da192fecd5f17ff9c2972464f57308d6ab0a4bb5f028ad`  
		Last Modified: Wed, 14 Oct 2020 21:22:42 GMT  
		Size: 5.4 MB (5425219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f421d0869e3cbe5b8580ee0612ddfc8a9afe94d285d80db4f6659869c583c83`  
		Last Modified: Wed, 14 Oct 2020 21:22:45 GMT  
		Size: 15.9 MB (15871237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4d937f908a310fa9b1957cf7d45f93cdfede8f5fb275cdc998d945256ed08d6`  
		Last Modified: Wed, 14 Oct 2020 21:22:41 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24f3c49e9d40da03d9a3c60f34aa4e5819584d55c708216829aa3f00d408353f`  
		Last Modified: Wed, 14 Oct 2020 21:22:40 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2088679ebef164efa3ed0b7a7a70064336481303027587ac6bce796c5400bbab`  
		Last Modified: Wed, 14 Oct 2020 21:22:41 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
