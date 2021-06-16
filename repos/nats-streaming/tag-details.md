<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `nats-streaming`

-	[`nats-streaming:0.22`](#nats-streaming022)
-	[`nats-streaming:0.22-alpine`](#nats-streaming022-alpine)
-	[`nats-streaming:0.22-alpine3.13`](#nats-streaming022-alpine313)
-	[`nats-streaming:0.22-linux`](#nats-streaming022-linux)
-	[`nats-streaming:0.22-nanoserver`](#nats-streaming022-nanoserver)
-	[`nats-streaming:0.22-nanoserver-1809`](#nats-streaming022-nanoserver-1809)
-	[`nats-streaming:0.22-scratch`](#nats-streaming022-scratch)
-	[`nats-streaming:0.22-windowsservercore`](#nats-streaming022-windowsservercore)
-	[`nats-streaming:0.22-windowsservercore-1809`](#nats-streaming022-windowsservercore-1809)
-	[`nats-streaming:0.22-windowsservercore-ltsc2016`](#nats-streaming022-windowsservercore-ltsc2016)
-	[`nats-streaming:0.22.0`](#nats-streaming0220)
-	[`nats-streaming:0.22.0-alpine`](#nats-streaming0220-alpine)
-	[`nats-streaming:0.22.0-alpine3.13`](#nats-streaming0220-alpine313)
-	[`nats-streaming:0.22.0-linux`](#nats-streaming0220-linux)
-	[`nats-streaming:0.22.0-nanoserver`](#nats-streaming0220-nanoserver)
-	[`nats-streaming:0.22.0-nanoserver-1809`](#nats-streaming0220-nanoserver-1809)
-	[`nats-streaming:0.22.0-scratch`](#nats-streaming0220-scratch)
-	[`nats-streaming:0.22.0-windowsservercore`](#nats-streaming0220-windowsservercore)
-	[`nats-streaming:0.22.0-windowsservercore-1809`](#nats-streaming0220-windowsservercore-1809)
-	[`nats-streaming:0.22.0-windowsservercore-ltsc2016`](#nats-streaming0220-windowsservercore-ltsc2016)
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

## `nats-streaming:0.22`

```console
$ docker pull nats-streaming@sha256:05ae257f52770a83cab1f239eaeacc1954cd48cb6218782a619ba3fcc12dbd6c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.1999; amd64

### `nats-streaming:0.22` - linux; amd64

```console
$ docker pull nats-streaming@sha256:ba1be2cd913a1e9f1ffc9445e5c04c169db333819beb7204deb3bc7c29fde5a8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6800613 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12f2d32e0c9a23e5a9a5cb19c8b1404a9cc7af17915e33eabb71e55767848df7`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Wed, 02 Jun 2021 05:47:24 GMT
COPY file:bbdef008b65f574a4e4593641e45dd6cdff5e8261d06d8f3959963f686dcdb78 in /nats-streaming-server 
# Wed, 02 Jun 2021 05:47:24 GMT
EXPOSE 4222 8222
# Wed, 02 Jun 2021 05:47:24 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Wed, 02 Jun 2021 05:47:24 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:afa0998a9989cfec22c4ad772da3ca685ea7ccf963253ff9c27edf33a00d49c6`  
		Last Modified: Wed, 02 Jun 2021 05:48:07 GMT  
		Size: 6.8 MB (6800613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.22` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:1bef88847972d6206955fdc84742cb2505dcdf9ec86c2ef8bd6b5629c88ef2f3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 MB (6269700 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:258e5207bc79452baf170c0dc0a5c955f71c72fadc9fff82bffecc06eb3e1e81`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 01 Jun 2021 23:54:46 GMT
COPY file:a4f69de3d07c6870dde4796b4de69a931a699d7e5b6ec30b2f25f6a23d66cb33 in /nats-streaming-server 
# Tue, 01 Jun 2021 23:54:47 GMT
EXPOSE 4222 8222
# Tue, 01 Jun 2021 23:54:47 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 01 Jun 2021 23:54:47 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:8ab135edb380ca588ed7d11dbea1418006a6708ae7ae5effad8d86bcef90198e`  
		Last Modified: Tue, 01 Jun 2021 23:56:26 GMT  
		Size: 6.3 MB (6269700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.22` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:a6c122176a5ff4bdae9a653ebb1cf3e0672cd240250547b855ae0f8894496225
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 MB (6259769 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ccaf377f82ea563a543d1a8bcf9a53870f6427a0cacae9f9ad5e46e6c7eabff`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Wed, 02 Jun 2021 03:13:19 GMT
COPY file:6e08520addf5d0c5d064e431d76487779d8fd8f4c03f71a72dc4e2c81812a922 in /nats-streaming-server 
# Wed, 02 Jun 2021 03:13:20 GMT
EXPOSE 4222 8222
# Wed, 02 Jun 2021 03:13:20 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Wed, 02 Jun 2021 03:13:20 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:887fd90bbdf32bb85ec9e85b63e60eccca791d6c882e30de0c10e6e583ccbb65`  
		Last Modified: Wed, 02 Jun 2021 03:15:02 GMT  
		Size: 6.3 MB (6259769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.22` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:bd5a415582b3f1d079d6498c12ea9138d7bde01dcd3a5f5a35a1731edf4c889f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.2 MB (6197708 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:16d36744f70db176ba94e376a65c5edda55a7167035e7dffdf217e594c1ac283`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Wed, 02 Jun 2021 02:14:00 GMT
COPY file:ef2047bb70888b72ef213e68689b3b8ae622cc597cd07b313c26b278418788bd in /nats-streaming-server 
# Wed, 02 Jun 2021 02:14:00 GMT
EXPOSE 4222 8222
# Wed, 02 Jun 2021 02:14:01 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Wed, 02 Jun 2021 02:14:01 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:ddf987a265c2be80179a2683a2d725f5a7e9fb477bc5752443a6d955be681a50`  
		Last Modified: Wed, 02 Jun 2021 02:15:07 GMT  
		Size: 6.2 MB (6197708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.22` - windows version 10.0.17763.1999; amd64

```console
$ docker pull nats-streaming@sha256:94fafaf460823aa892ed913e1f95a42f617b0b0ade5f63fec023190aad998802
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.6 MB (109610228 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:58e2b8ca8f56a4b97f31133be06094bd3eeb0219661aba4e8aaaad7a79d723c6`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Sun, 06 Jun 2021 04:04:04 GMT
RUN Apply image 1809-amd64
# Wed, 09 Jun 2021 15:55:07 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 09 Jun 2021 20:24:03 GMT
RUN cmd /S /C #(nop) COPY file:72a29a3f2d4a0bd237295ad8b2a317a32c76cbb8a1af898a564024d5013c0475 in C:\nats-streaming-server.exe 
# Wed, 09 Jun 2021 20:24:05 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 09 Jun 2021 20:24:07 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 09 Jun 2021 20:24:10 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:e4800203e906d49fbdaf1eeab4de72f28796d5b9a1ea44f8d7461001cfa56614`  
		Size: 102.7 MB (102671454 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:80d93ce19113bbf944b699f12e59395e0eabeb00ccd1fd5dc7df46bb115eba2f`  
		Last Modified: Wed, 09 Jun 2021 15:59:58 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:348b9d29d0e17e2575302e48a756c01845f95766a27b3efd5037e69dc02c3ffd`  
		Last Modified: Wed, 09 Jun 2021 20:29:05 GMT  
		Size: 6.9 MB (6934149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cfbb95c41b561debff13c2fdc579566b502a46d04cc2aa8636fc043d67cf6f9`  
		Last Modified: Wed, 09 Jun 2021 20:28:57 GMT  
		Size: 1.2 KB (1184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1321261d7f7de3d8a203008e1bd4541c0a15f00938a86e8f610acd674513bff3`  
		Last Modified: Wed, 09 Jun 2021 20:28:57 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58df4d427933ebe735d64a9ffec8fb7774cc74c1158c33e365322810443cc018`  
		Last Modified: Wed, 09 Jun 2021 20:28:57 GMT  
		Size: 1.2 KB (1167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.22-alpine`

```console
$ docker pull nats-streaming@sha256:99da8c602fc3b57ef730efda710a4e62d47a9e62c772b854c255081cd7f2f7fa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.22-alpine` - linux; amd64

```console
$ docker pull nats-streaming@sha256:25457c5b382da1fb7ab66c4f977ad38915b109e9bf0d4440f2ae2f314d3bcc97
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.9 MB (9894969 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:443be2e221357fdae9e3405207feb4e1f061dce181882a1cf208543e029bc8fa`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Wed, 02 Jun 2021 05:47:13 GMT
ENV NATS_STREAMING_SERVER=0.22.0
# Wed, 02 Jun 2021 05:47:16 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='3ffc4b74f469b97a8ce0edff8b645baf89d9f9f3debdfa7088a0ceac3ed6c37b' ;; 		armhf) natsArch='arm6'; sha256='abe201b1a90cd2e8db39989c81a2c76d3956035745c68d0c7e090fc8c5a138c8' ;; 		armv7) natsArch='arm7'; sha256='d218edd395f980ea91a54624b4cc1fe0220268171ee596a24d7c01c15a7dbb7f' ;; 		x86_64) natsArch='amd64'; sha256='72f5b899167a8866d4b82d1bf9bc14b5d047e6b1ab127dd0085e9eb91a89f097' ;; 		x86) natsArch='386'; sha256='d87bb204228c5e820747e1682dbfb56289e3ddadcfe129b9c9fcf1ad7c0ba053' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 02 Jun 2021 05:47:16 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Wed, 02 Jun 2021 05:47:16 GMT
EXPOSE 4222 8222
# Wed, 02 Jun 2021 05:47:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 02 Jun 2021 05:47:17 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4795908dc4759b01d3e4dd956343fb777c34c32afc57d2a4a96014fa67a41206`  
		Last Modified: Wed, 02 Jun 2021 05:47:46 GMT  
		Size: 7.1 MB (7082579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bf7f8694c616cf8f24559388ba77e2349a8da60a47001bfd26c85997d87b593`  
		Last Modified: Wed, 02 Jun 2021 05:47:45 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.22-alpine` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:7bc8b6da7d8065b7aa858b4520894ad45868c6a99266b4388fec303dd7fa4357
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.2 MB (9175683 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1fa8f1250edffbb08905947aa23b69e8cb17e049ac8790674031e8511024fb5d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Tue, 15 Jun 2021 22:57:34 GMT
ADD file:4479f0a51530e039edf231d87201896dcff908aa542a613cdccb015f93dda8a3 in / 
# Tue, 15 Jun 2021 22:57:34 GMT
CMD ["/bin/sh"]
# Wed, 16 Jun 2021 11:21:18 GMT
ENV NATS_STREAMING_SERVER=0.22.0
# Wed, 16 Jun 2021 11:21:21 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='3ffc4b74f469b97a8ce0edff8b645baf89d9f9f3debdfa7088a0ceac3ed6c37b' ;; 		armhf) natsArch='arm6'; sha256='abe201b1a90cd2e8db39989c81a2c76d3956035745c68d0c7e090fc8c5a138c8' ;; 		armv7) natsArch='arm7'; sha256='d218edd395f980ea91a54624b4cc1fe0220268171ee596a24d7c01c15a7dbb7f' ;; 		x86_64) natsArch='amd64'; sha256='72f5b899167a8866d4b82d1bf9bc14b5d047e6b1ab127dd0085e9eb91a89f097' ;; 		x86) natsArch='386'; sha256='d87bb204228c5e820747e1682dbfb56289e3ddadcfe129b9c9fcf1ad7c0ba053' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 16 Jun 2021 11:21:22 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Wed, 16 Jun 2021 11:21:22 GMT
EXPOSE 4222 8222
# Wed, 16 Jun 2021 11:21:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Jun 2021 11:21:22 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:740c950346cf39c85b52576998695c9b909c24a58a8bb1b64cce91fda3ef1d3a`  
		Last Modified: Wed, 14 Apr 2021 18:50:30 GMT  
		Size: 2.6 MB (2622131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25dbe7b857ca17019fb0e3e3b5439aaf5211a0b71cc2e017cb9465df530b8499`  
		Last Modified: Wed, 16 Jun 2021 11:22:38 GMT  
		Size: 6.6 MB (6553129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df6ca706362f12c5b456b49cbb3448d3189e225a08bffffdecb00fe040b2816f`  
		Last Modified: Wed, 16 Jun 2021 11:22:36 GMT  
		Size: 423.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.22-alpine` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:094bdcea75742a31480bd4f5771f741f7490f46a7bade1b1e6836fc2ab0e14f9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.0 MB (8967137 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:16a7379dc428ab28ff200036e6f1a917c42724a035ffc0d548ecb01f9954593f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 14 Apr 2021 18:57:39 GMT
ADD file:028c5b473d862250586e174c5dd19b37f8fc3bffbc02d888e72df30f32fd6129 in / 
# Wed, 14 Apr 2021 18:57:39 GMT
CMD ["/bin/sh"]
# Wed, 02 Jun 2021 03:12:59 GMT
ENV NATS_STREAMING_SERVER=0.22.0
# Wed, 02 Jun 2021 03:13:03 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='3ffc4b74f469b97a8ce0edff8b645baf89d9f9f3debdfa7088a0ceac3ed6c37b' ;; 		armhf) natsArch='arm6'; sha256='abe201b1a90cd2e8db39989c81a2c76d3956035745c68d0c7e090fc8c5a138c8' ;; 		armv7) natsArch='arm7'; sha256='d218edd395f980ea91a54624b4cc1fe0220268171ee596a24d7c01c15a7dbb7f' ;; 		x86_64) natsArch='amd64'; sha256='72f5b899167a8866d4b82d1bf9bc14b5d047e6b1ab127dd0085e9eb91a89f097' ;; 		x86) natsArch='386'; sha256='d87bb204228c5e820747e1682dbfb56289e3ddadcfe129b9c9fcf1ad7c0ba053' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 02 Jun 2021 03:13:03 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Wed, 02 Jun 2021 03:13:03 GMT
EXPOSE 4222 8222
# Wed, 02 Jun 2021 03:13:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 02 Jun 2021 03:13:03 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:e160e00eb35d5bc2373770873fbc9c8f5706045b0b06bfd1c364fcf69f02e9fe`  
		Last Modified: Wed, 14 Apr 2021 18:58:36 GMT  
		Size: 2.4 MB (2424145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcef365af48832fc326fce4ba5cec1feba2d3830122e812be8f7c68c4eba747b`  
		Last Modified: Wed, 02 Jun 2021 03:14:30 GMT  
		Size: 6.5 MB (6542570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:773ab986cb0c82686f2f65fa84b5189bb9194ebe32dc1d4f734e8842539f05fc`  
		Last Modified: Wed, 02 Jun 2021 03:14:29 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.22-alpine` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:885349fb8c0102784700ebcdedc5f335a0b0079ccc30f93dc8349bb5ff7b3ba6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.2 MB (9192675 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7fbf7556b1dda05ceae2f1e33ba452f09a4e16e136faea904618586f5e8e643c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Tue, 15 Jun 2021 21:45:03 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Tue, 15 Jun 2021 21:45:04 GMT
CMD ["/bin/sh"]
# Wed, 16 Jun 2021 01:10:22 GMT
ENV NATS_STREAMING_SERVER=0.22.0
# Wed, 16 Jun 2021 01:10:25 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='3ffc4b74f469b97a8ce0edff8b645baf89d9f9f3debdfa7088a0ceac3ed6c37b' ;; 		armhf) natsArch='arm6'; sha256='abe201b1a90cd2e8db39989c81a2c76d3956035745c68d0c7e090fc8c5a138c8' ;; 		armv7) natsArch='arm7'; sha256='d218edd395f980ea91a54624b4cc1fe0220268171ee596a24d7c01c15a7dbb7f' ;; 		x86_64) natsArch='amd64'; sha256='72f5b899167a8866d4b82d1bf9bc14b5d047e6b1ab127dd0085e9eb91a89f097' ;; 		x86) natsArch='386'; sha256='d87bb204228c5e820747e1682dbfb56289e3ddadcfe129b9c9fcf1ad7c0ba053' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 16 Jun 2021 01:10:25 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Wed, 16 Jun 2021 01:10:25 GMT
EXPOSE 4222 8222
# Wed, 16 Jun 2021 01:10:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Jun 2021 01:10:26 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ed1df6d6dbc94e5c85bddb8f9a8dbaa65a5f97ef70e3b4c2a6ce6d46611ef62`  
		Last Modified: Wed, 16 Jun 2021 01:11:18 GMT  
		Size: 6.5 MB (6480227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5409d34dbaa07dcbd979022c1e953c405331b8f63d8e51e47e05f1fbedd24241`  
		Last Modified: Wed, 16 Jun 2021 01:11:16 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.22-alpine3.13`

```console
$ docker pull nats-streaming@sha256:99da8c602fc3b57ef730efda710a4e62d47a9e62c772b854c255081cd7f2f7fa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.22-alpine3.13` - linux; amd64

```console
$ docker pull nats-streaming@sha256:25457c5b382da1fb7ab66c4f977ad38915b109e9bf0d4440f2ae2f314d3bcc97
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.9 MB (9894969 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:443be2e221357fdae9e3405207feb4e1f061dce181882a1cf208543e029bc8fa`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Wed, 02 Jun 2021 05:47:13 GMT
ENV NATS_STREAMING_SERVER=0.22.0
# Wed, 02 Jun 2021 05:47:16 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='3ffc4b74f469b97a8ce0edff8b645baf89d9f9f3debdfa7088a0ceac3ed6c37b' ;; 		armhf) natsArch='arm6'; sha256='abe201b1a90cd2e8db39989c81a2c76d3956035745c68d0c7e090fc8c5a138c8' ;; 		armv7) natsArch='arm7'; sha256='d218edd395f980ea91a54624b4cc1fe0220268171ee596a24d7c01c15a7dbb7f' ;; 		x86_64) natsArch='amd64'; sha256='72f5b899167a8866d4b82d1bf9bc14b5d047e6b1ab127dd0085e9eb91a89f097' ;; 		x86) natsArch='386'; sha256='d87bb204228c5e820747e1682dbfb56289e3ddadcfe129b9c9fcf1ad7c0ba053' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 02 Jun 2021 05:47:16 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Wed, 02 Jun 2021 05:47:16 GMT
EXPOSE 4222 8222
# Wed, 02 Jun 2021 05:47:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 02 Jun 2021 05:47:17 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4795908dc4759b01d3e4dd956343fb777c34c32afc57d2a4a96014fa67a41206`  
		Last Modified: Wed, 02 Jun 2021 05:47:46 GMT  
		Size: 7.1 MB (7082579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bf7f8694c616cf8f24559388ba77e2349a8da60a47001bfd26c85997d87b593`  
		Last Modified: Wed, 02 Jun 2021 05:47:45 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.22-alpine3.13` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:7bc8b6da7d8065b7aa858b4520894ad45868c6a99266b4388fec303dd7fa4357
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.2 MB (9175683 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1fa8f1250edffbb08905947aa23b69e8cb17e049ac8790674031e8511024fb5d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Tue, 15 Jun 2021 22:57:34 GMT
ADD file:4479f0a51530e039edf231d87201896dcff908aa542a613cdccb015f93dda8a3 in / 
# Tue, 15 Jun 2021 22:57:34 GMT
CMD ["/bin/sh"]
# Wed, 16 Jun 2021 11:21:18 GMT
ENV NATS_STREAMING_SERVER=0.22.0
# Wed, 16 Jun 2021 11:21:21 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='3ffc4b74f469b97a8ce0edff8b645baf89d9f9f3debdfa7088a0ceac3ed6c37b' ;; 		armhf) natsArch='arm6'; sha256='abe201b1a90cd2e8db39989c81a2c76d3956035745c68d0c7e090fc8c5a138c8' ;; 		armv7) natsArch='arm7'; sha256='d218edd395f980ea91a54624b4cc1fe0220268171ee596a24d7c01c15a7dbb7f' ;; 		x86_64) natsArch='amd64'; sha256='72f5b899167a8866d4b82d1bf9bc14b5d047e6b1ab127dd0085e9eb91a89f097' ;; 		x86) natsArch='386'; sha256='d87bb204228c5e820747e1682dbfb56289e3ddadcfe129b9c9fcf1ad7c0ba053' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 16 Jun 2021 11:21:22 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Wed, 16 Jun 2021 11:21:22 GMT
EXPOSE 4222 8222
# Wed, 16 Jun 2021 11:21:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Jun 2021 11:21:22 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:740c950346cf39c85b52576998695c9b909c24a58a8bb1b64cce91fda3ef1d3a`  
		Last Modified: Wed, 14 Apr 2021 18:50:30 GMT  
		Size: 2.6 MB (2622131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25dbe7b857ca17019fb0e3e3b5439aaf5211a0b71cc2e017cb9465df530b8499`  
		Last Modified: Wed, 16 Jun 2021 11:22:38 GMT  
		Size: 6.6 MB (6553129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df6ca706362f12c5b456b49cbb3448d3189e225a08bffffdecb00fe040b2816f`  
		Last Modified: Wed, 16 Jun 2021 11:22:36 GMT  
		Size: 423.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.22-alpine3.13` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:094bdcea75742a31480bd4f5771f741f7490f46a7bade1b1e6836fc2ab0e14f9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.0 MB (8967137 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:16a7379dc428ab28ff200036e6f1a917c42724a035ffc0d548ecb01f9954593f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 14 Apr 2021 18:57:39 GMT
ADD file:028c5b473d862250586e174c5dd19b37f8fc3bffbc02d888e72df30f32fd6129 in / 
# Wed, 14 Apr 2021 18:57:39 GMT
CMD ["/bin/sh"]
# Wed, 02 Jun 2021 03:12:59 GMT
ENV NATS_STREAMING_SERVER=0.22.0
# Wed, 02 Jun 2021 03:13:03 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='3ffc4b74f469b97a8ce0edff8b645baf89d9f9f3debdfa7088a0ceac3ed6c37b' ;; 		armhf) natsArch='arm6'; sha256='abe201b1a90cd2e8db39989c81a2c76d3956035745c68d0c7e090fc8c5a138c8' ;; 		armv7) natsArch='arm7'; sha256='d218edd395f980ea91a54624b4cc1fe0220268171ee596a24d7c01c15a7dbb7f' ;; 		x86_64) natsArch='amd64'; sha256='72f5b899167a8866d4b82d1bf9bc14b5d047e6b1ab127dd0085e9eb91a89f097' ;; 		x86) natsArch='386'; sha256='d87bb204228c5e820747e1682dbfb56289e3ddadcfe129b9c9fcf1ad7c0ba053' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 02 Jun 2021 03:13:03 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Wed, 02 Jun 2021 03:13:03 GMT
EXPOSE 4222 8222
# Wed, 02 Jun 2021 03:13:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 02 Jun 2021 03:13:03 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:e160e00eb35d5bc2373770873fbc9c8f5706045b0b06bfd1c364fcf69f02e9fe`  
		Last Modified: Wed, 14 Apr 2021 18:58:36 GMT  
		Size: 2.4 MB (2424145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcef365af48832fc326fce4ba5cec1feba2d3830122e812be8f7c68c4eba747b`  
		Last Modified: Wed, 02 Jun 2021 03:14:30 GMT  
		Size: 6.5 MB (6542570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:773ab986cb0c82686f2f65fa84b5189bb9194ebe32dc1d4f734e8842539f05fc`  
		Last Modified: Wed, 02 Jun 2021 03:14:29 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.22-alpine3.13` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:885349fb8c0102784700ebcdedc5f335a0b0079ccc30f93dc8349bb5ff7b3ba6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.2 MB (9192675 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7fbf7556b1dda05ceae2f1e33ba452f09a4e16e136faea904618586f5e8e643c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Tue, 15 Jun 2021 21:45:03 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Tue, 15 Jun 2021 21:45:04 GMT
CMD ["/bin/sh"]
# Wed, 16 Jun 2021 01:10:22 GMT
ENV NATS_STREAMING_SERVER=0.22.0
# Wed, 16 Jun 2021 01:10:25 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='3ffc4b74f469b97a8ce0edff8b645baf89d9f9f3debdfa7088a0ceac3ed6c37b' ;; 		armhf) natsArch='arm6'; sha256='abe201b1a90cd2e8db39989c81a2c76d3956035745c68d0c7e090fc8c5a138c8' ;; 		armv7) natsArch='arm7'; sha256='d218edd395f980ea91a54624b4cc1fe0220268171ee596a24d7c01c15a7dbb7f' ;; 		x86_64) natsArch='amd64'; sha256='72f5b899167a8866d4b82d1bf9bc14b5d047e6b1ab127dd0085e9eb91a89f097' ;; 		x86) natsArch='386'; sha256='d87bb204228c5e820747e1682dbfb56289e3ddadcfe129b9c9fcf1ad7c0ba053' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 16 Jun 2021 01:10:25 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Wed, 16 Jun 2021 01:10:25 GMT
EXPOSE 4222 8222
# Wed, 16 Jun 2021 01:10:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Jun 2021 01:10:26 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ed1df6d6dbc94e5c85bddb8f9a8dbaa65a5f97ef70e3b4c2a6ce6d46611ef62`  
		Last Modified: Wed, 16 Jun 2021 01:11:18 GMT  
		Size: 6.5 MB (6480227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5409d34dbaa07dcbd979022c1e953c405331b8f63d8e51e47e05f1fbedd24241`  
		Last Modified: Wed, 16 Jun 2021 01:11:16 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.22-linux`

```console
$ docker pull nats-streaming@sha256:29a31360a13ce43c1a19b01d048213225f0ca3daaf0ac9f75e4ff9e21fcb656f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.22-linux` - linux; amd64

```console
$ docker pull nats-streaming@sha256:ba1be2cd913a1e9f1ffc9445e5c04c169db333819beb7204deb3bc7c29fde5a8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6800613 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12f2d32e0c9a23e5a9a5cb19c8b1404a9cc7af17915e33eabb71e55767848df7`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Wed, 02 Jun 2021 05:47:24 GMT
COPY file:bbdef008b65f574a4e4593641e45dd6cdff5e8261d06d8f3959963f686dcdb78 in /nats-streaming-server 
# Wed, 02 Jun 2021 05:47:24 GMT
EXPOSE 4222 8222
# Wed, 02 Jun 2021 05:47:24 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Wed, 02 Jun 2021 05:47:24 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:afa0998a9989cfec22c4ad772da3ca685ea7ccf963253ff9c27edf33a00d49c6`  
		Last Modified: Wed, 02 Jun 2021 05:48:07 GMT  
		Size: 6.8 MB (6800613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.22-linux` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:1bef88847972d6206955fdc84742cb2505dcdf9ec86c2ef8bd6b5629c88ef2f3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 MB (6269700 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:258e5207bc79452baf170c0dc0a5c955f71c72fadc9fff82bffecc06eb3e1e81`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 01 Jun 2021 23:54:46 GMT
COPY file:a4f69de3d07c6870dde4796b4de69a931a699d7e5b6ec30b2f25f6a23d66cb33 in /nats-streaming-server 
# Tue, 01 Jun 2021 23:54:47 GMT
EXPOSE 4222 8222
# Tue, 01 Jun 2021 23:54:47 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 01 Jun 2021 23:54:47 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:8ab135edb380ca588ed7d11dbea1418006a6708ae7ae5effad8d86bcef90198e`  
		Last Modified: Tue, 01 Jun 2021 23:56:26 GMT  
		Size: 6.3 MB (6269700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.22-linux` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:a6c122176a5ff4bdae9a653ebb1cf3e0672cd240250547b855ae0f8894496225
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 MB (6259769 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ccaf377f82ea563a543d1a8bcf9a53870f6427a0cacae9f9ad5e46e6c7eabff`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Wed, 02 Jun 2021 03:13:19 GMT
COPY file:6e08520addf5d0c5d064e431d76487779d8fd8f4c03f71a72dc4e2c81812a922 in /nats-streaming-server 
# Wed, 02 Jun 2021 03:13:20 GMT
EXPOSE 4222 8222
# Wed, 02 Jun 2021 03:13:20 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Wed, 02 Jun 2021 03:13:20 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:887fd90bbdf32bb85ec9e85b63e60eccca791d6c882e30de0c10e6e583ccbb65`  
		Last Modified: Wed, 02 Jun 2021 03:15:02 GMT  
		Size: 6.3 MB (6259769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.22-linux` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:bd5a415582b3f1d079d6498c12ea9138d7bde01dcd3a5f5a35a1731edf4c889f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.2 MB (6197708 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:16d36744f70db176ba94e376a65c5edda55a7167035e7dffdf217e594c1ac283`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Wed, 02 Jun 2021 02:14:00 GMT
COPY file:ef2047bb70888b72ef213e68689b3b8ae622cc597cd07b313c26b278418788bd in /nats-streaming-server 
# Wed, 02 Jun 2021 02:14:00 GMT
EXPOSE 4222 8222
# Wed, 02 Jun 2021 02:14:01 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Wed, 02 Jun 2021 02:14:01 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:ddf987a265c2be80179a2683a2d725f5a7e9fb477bc5752443a6d955be681a50`  
		Last Modified: Wed, 02 Jun 2021 02:15:07 GMT  
		Size: 6.2 MB (6197708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.22-nanoserver`

```console
$ docker pull nats-streaming@sha256:1db69154831d3b3a88080c69533b678362e4d86676ca33b2e50336765c7436bd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1999; amd64

### `nats-streaming:0.22-nanoserver` - windows version 10.0.17763.1999; amd64

```console
$ docker pull nats-streaming@sha256:94fafaf460823aa892ed913e1f95a42f617b0b0ade5f63fec023190aad998802
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.6 MB (109610228 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:58e2b8ca8f56a4b97f31133be06094bd3eeb0219661aba4e8aaaad7a79d723c6`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Sun, 06 Jun 2021 04:04:04 GMT
RUN Apply image 1809-amd64
# Wed, 09 Jun 2021 15:55:07 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 09 Jun 2021 20:24:03 GMT
RUN cmd /S /C #(nop) COPY file:72a29a3f2d4a0bd237295ad8b2a317a32c76cbb8a1af898a564024d5013c0475 in C:\nats-streaming-server.exe 
# Wed, 09 Jun 2021 20:24:05 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 09 Jun 2021 20:24:07 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 09 Jun 2021 20:24:10 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:e4800203e906d49fbdaf1eeab4de72f28796d5b9a1ea44f8d7461001cfa56614`  
		Size: 102.7 MB (102671454 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:80d93ce19113bbf944b699f12e59395e0eabeb00ccd1fd5dc7df46bb115eba2f`  
		Last Modified: Wed, 09 Jun 2021 15:59:58 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:348b9d29d0e17e2575302e48a756c01845f95766a27b3efd5037e69dc02c3ffd`  
		Last Modified: Wed, 09 Jun 2021 20:29:05 GMT  
		Size: 6.9 MB (6934149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cfbb95c41b561debff13c2fdc579566b502a46d04cc2aa8636fc043d67cf6f9`  
		Last Modified: Wed, 09 Jun 2021 20:28:57 GMT  
		Size: 1.2 KB (1184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1321261d7f7de3d8a203008e1bd4541c0a15f00938a86e8f610acd674513bff3`  
		Last Modified: Wed, 09 Jun 2021 20:28:57 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58df4d427933ebe735d64a9ffec8fb7774cc74c1158c33e365322810443cc018`  
		Last Modified: Wed, 09 Jun 2021 20:28:57 GMT  
		Size: 1.2 KB (1167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.22-nanoserver-1809`

```console
$ docker pull nats-streaming@sha256:1db69154831d3b3a88080c69533b678362e4d86676ca33b2e50336765c7436bd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1999; amd64

### `nats-streaming:0.22-nanoserver-1809` - windows version 10.0.17763.1999; amd64

```console
$ docker pull nats-streaming@sha256:94fafaf460823aa892ed913e1f95a42f617b0b0ade5f63fec023190aad998802
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.6 MB (109610228 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:58e2b8ca8f56a4b97f31133be06094bd3eeb0219661aba4e8aaaad7a79d723c6`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Sun, 06 Jun 2021 04:04:04 GMT
RUN Apply image 1809-amd64
# Wed, 09 Jun 2021 15:55:07 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 09 Jun 2021 20:24:03 GMT
RUN cmd /S /C #(nop) COPY file:72a29a3f2d4a0bd237295ad8b2a317a32c76cbb8a1af898a564024d5013c0475 in C:\nats-streaming-server.exe 
# Wed, 09 Jun 2021 20:24:05 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 09 Jun 2021 20:24:07 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 09 Jun 2021 20:24:10 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:e4800203e906d49fbdaf1eeab4de72f28796d5b9a1ea44f8d7461001cfa56614`  
		Size: 102.7 MB (102671454 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:80d93ce19113bbf944b699f12e59395e0eabeb00ccd1fd5dc7df46bb115eba2f`  
		Last Modified: Wed, 09 Jun 2021 15:59:58 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:348b9d29d0e17e2575302e48a756c01845f95766a27b3efd5037e69dc02c3ffd`  
		Last Modified: Wed, 09 Jun 2021 20:29:05 GMT  
		Size: 6.9 MB (6934149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cfbb95c41b561debff13c2fdc579566b502a46d04cc2aa8636fc043d67cf6f9`  
		Last Modified: Wed, 09 Jun 2021 20:28:57 GMT  
		Size: 1.2 KB (1184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1321261d7f7de3d8a203008e1bd4541c0a15f00938a86e8f610acd674513bff3`  
		Last Modified: Wed, 09 Jun 2021 20:28:57 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58df4d427933ebe735d64a9ffec8fb7774cc74c1158c33e365322810443cc018`  
		Last Modified: Wed, 09 Jun 2021 20:28:57 GMT  
		Size: 1.2 KB (1167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.22-scratch`

```console
$ docker pull nats-streaming@sha256:29a31360a13ce43c1a19b01d048213225f0ca3daaf0ac9f75e4ff9e21fcb656f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.22-scratch` - linux; amd64

```console
$ docker pull nats-streaming@sha256:ba1be2cd913a1e9f1ffc9445e5c04c169db333819beb7204deb3bc7c29fde5a8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6800613 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12f2d32e0c9a23e5a9a5cb19c8b1404a9cc7af17915e33eabb71e55767848df7`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Wed, 02 Jun 2021 05:47:24 GMT
COPY file:bbdef008b65f574a4e4593641e45dd6cdff5e8261d06d8f3959963f686dcdb78 in /nats-streaming-server 
# Wed, 02 Jun 2021 05:47:24 GMT
EXPOSE 4222 8222
# Wed, 02 Jun 2021 05:47:24 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Wed, 02 Jun 2021 05:47:24 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:afa0998a9989cfec22c4ad772da3ca685ea7ccf963253ff9c27edf33a00d49c6`  
		Last Modified: Wed, 02 Jun 2021 05:48:07 GMT  
		Size: 6.8 MB (6800613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.22-scratch` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:1bef88847972d6206955fdc84742cb2505dcdf9ec86c2ef8bd6b5629c88ef2f3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 MB (6269700 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:258e5207bc79452baf170c0dc0a5c955f71c72fadc9fff82bffecc06eb3e1e81`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 01 Jun 2021 23:54:46 GMT
COPY file:a4f69de3d07c6870dde4796b4de69a931a699d7e5b6ec30b2f25f6a23d66cb33 in /nats-streaming-server 
# Tue, 01 Jun 2021 23:54:47 GMT
EXPOSE 4222 8222
# Tue, 01 Jun 2021 23:54:47 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 01 Jun 2021 23:54:47 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:8ab135edb380ca588ed7d11dbea1418006a6708ae7ae5effad8d86bcef90198e`  
		Last Modified: Tue, 01 Jun 2021 23:56:26 GMT  
		Size: 6.3 MB (6269700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.22-scratch` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:a6c122176a5ff4bdae9a653ebb1cf3e0672cd240250547b855ae0f8894496225
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 MB (6259769 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ccaf377f82ea563a543d1a8bcf9a53870f6427a0cacae9f9ad5e46e6c7eabff`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Wed, 02 Jun 2021 03:13:19 GMT
COPY file:6e08520addf5d0c5d064e431d76487779d8fd8f4c03f71a72dc4e2c81812a922 in /nats-streaming-server 
# Wed, 02 Jun 2021 03:13:20 GMT
EXPOSE 4222 8222
# Wed, 02 Jun 2021 03:13:20 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Wed, 02 Jun 2021 03:13:20 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:887fd90bbdf32bb85ec9e85b63e60eccca791d6c882e30de0c10e6e583ccbb65`  
		Last Modified: Wed, 02 Jun 2021 03:15:02 GMT  
		Size: 6.3 MB (6259769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.22-scratch` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:bd5a415582b3f1d079d6498c12ea9138d7bde01dcd3a5f5a35a1731edf4c889f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.2 MB (6197708 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:16d36744f70db176ba94e376a65c5edda55a7167035e7dffdf217e594c1ac283`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Wed, 02 Jun 2021 02:14:00 GMT
COPY file:ef2047bb70888b72ef213e68689b3b8ae622cc597cd07b313c26b278418788bd in /nats-streaming-server 
# Wed, 02 Jun 2021 02:14:00 GMT
EXPOSE 4222 8222
# Wed, 02 Jun 2021 02:14:01 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Wed, 02 Jun 2021 02:14:01 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:ddf987a265c2be80179a2683a2d725f5a7e9fb477bc5752443a6d955be681a50`  
		Last Modified: Wed, 02 Jun 2021 02:15:07 GMT  
		Size: 6.2 MB (6197708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.22-windowsservercore`

```console
$ docker pull nats-streaming@sha256:d53324a82d4959035f5ee013123eff935d4b10bcb37fbf63b0e6e37114a7d661
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1999; amd64
	-	windows version 10.0.14393.4467; amd64

### `nats-streaming:0.22-windowsservercore` - windows version 10.0.17763.1999; amd64

```console
$ docker pull nats-streaming@sha256:22abf51575f1bd50cccf86230258446c5cf719355e0ad48133786855f2c76c6c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2649198709 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d9a338521a6c092730c8066de4356133fa0b82ec4122f50d54a8fecd8a01ead`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
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
# Wed, 09 Jun 2021 20:21:49 GMT
ENV NATS_STREAMING_SERVER=0.22.0
# Wed, 09 Jun 2021 20:21:51 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.22.0/nats-streaming-server-v0.22.0-windows-amd64.zip
# Wed, 09 Jun 2021 20:21:54 GMT
ENV GIT_DOWNLOAD_SHA256=436c16330efbd0767d9a69dcdf2d3badd4e2598fab23c4f4a192e9d9982c2c92
# Wed, 09 Jun 2021 20:22:22 GMT
RUN Set-PSDebug -Trace 2
# Wed, 09 Jun 2021 20:23:43 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 09 Jun 2021 20:23:45 GMT
EXPOSE 4222 8222
# Wed, 09 Jun 2021 20:23:48 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 09 Jun 2021 20:23:50 GMT
CMD ["-m" "8222"]
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
	-	`sha256:2ce4b948c1a0090b613b7cf3caf73010af9ec5e2d3f2f1ff54177cf4d10a3e4b`  
		Last Modified: Wed, 09 Jun 2021 20:28:39 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:091f859d3e2c08bea4918bd73dd5179d67ec1cc848d31e861e8d8d54d3135e16`  
		Last Modified: Wed, 09 Jun 2021 20:28:39 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:065cc30c1c1a7502e7a8f8984ef62b8f6dac71d678e5fdbdfc4ac7886ae2dee1`  
		Last Modified: Wed, 09 Jun 2021 20:28:39 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:907007f7199ec34ff53edbf50c29cf96587f12e39407d042ce7ee894bc5c8010`  
		Last Modified: Wed, 09 Jun 2021 20:28:36 GMT  
		Size: 342.8 KB (342788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98435664ae81c44aa558ea460acb4b57148b65cd80fa1a5873fee91c8d6f784e`  
		Last Modified: Wed, 09 Jun 2021 20:28:44 GMT  
		Size: 7.3 MB (7259596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5089624a9545a210e2098609d71eb68eb27580b3bb9333bfeef73cf7185df9ff`  
		Last Modified: Wed, 09 Jun 2021 20:28:36 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc477e9744316e1163a516d61b0d028bf9876b297a2aeff872ab83c478c89d89`  
		Last Modified: Wed, 09 Jun 2021 20:28:36 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f65a67fb6dd9f5bb509e1e9f4ad38f5beed7d810d2f7ffc39a961be929c95228`  
		Last Modified: Wed, 09 Jun 2021 20:28:36 GMT  
		Size: 1.4 KB (1385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.22-windowsservercore` - windows version 10.0.14393.4467; amd64

```console
$ docker pull nats-streaming@sha256:c1d1676348d3cc256527165d36fdb7096c23cadb25a41724b9d716e816930192
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6277864201 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed49864d98975c3b2d97e536c6f86c43a8d6df1e09903b12259a9d5009fb1b07`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
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
# Wed, 09 Jun 2021 20:24:18 GMT
ENV NATS_STREAMING_SERVER=0.22.0
# Wed, 09 Jun 2021 20:24:20 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.22.0/nats-streaming-server-v0.22.0-windows-amd64.zip
# Wed, 09 Jun 2021 20:24:22 GMT
ENV GIT_DOWNLOAD_SHA256=436c16330efbd0767d9a69dcdf2d3badd4e2598fab23c4f4a192e9d9982c2c92
# Wed, 09 Jun 2021 20:25:38 GMT
RUN Set-PSDebug -Trace 2
# Wed, 09 Jun 2021 20:27:59 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 09 Jun 2021 20:28:02 GMT
EXPOSE 4222 8222
# Wed, 09 Jun 2021 20:28:05 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 09 Jun 2021 20:28:07 GMT
CMD ["-m" "8222"]
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
	-	`sha256:dc5848e927e0f88d330cfd4d69ff5b33a883c0926f224b083d84658b124b4eff`  
		Last Modified: Wed, 09 Jun 2021 20:29:21 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c560d2270f78e7dec252e2f64f0e115ce098ccb7e292f89dc10e8c96b6409b7a`  
		Last Modified: Wed, 09 Jun 2021 20:29:21 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8df992a1ddf947618230669ac99ede1f6100d23bffefc379015097d6ab55de11`  
		Last Modified: Wed, 09 Jun 2021 20:29:20 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d1c5d78268da7d5a12285ca6e0b9ee14a4c092effdf1f0c1ef9def8724a38dc`  
		Last Modified: Wed, 09 Jun 2021 20:29:18 GMT  
		Size: 341.8 KB (341824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21e2d30fad367283448bcc184a08542dfd3e4d0f13691f608f48111fa360ca8a`  
		Last Modified: Wed, 09 Jun 2021 20:29:21 GMT  
		Size: 11.8 MB (11783856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90a63b8e3d31cde8595bcc53bffd235ec17496ec80e358d2dd963fe75965ea1e`  
		Last Modified: Wed, 09 Jun 2021 20:29:18 GMT  
		Size: 1.4 KB (1444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e14db649ae2c7bc33a1fad8a90d8ebec3336062ba22a9922f7e5fc3af262b470`  
		Last Modified: Wed, 09 Jun 2021 20:29:18 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5715b2e77233052328e64dc4f9dcbe9fb8a8f8d0b452405716447e4addb11458`  
		Last Modified: Wed, 09 Jun 2021 20:29:18 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.22-windowsservercore-1809`

```console
$ docker pull nats-streaming@sha256:cf19c0a807a7bc0417a8331f534bef50ae3147a7302679b2370a0976de91d4d2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1999; amd64

### `nats-streaming:0.22-windowsservercore-1809` - windows version 10.0.17763.1999; amd64

```console
$ docker pull nats-streaming@sha256:22abf51575f1bd50cccf86230258446c5cf719355e0ad48133786855f2c76c6c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2649198709 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d9a338521a6c092730c8066de4356133fa0b82ec4122f50d54a8fecd8a01ead`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
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
# Wed, 09 Jun 2021 20:21:49 GMT
ENV NATS_STREAMING_SERVER=0.22.0
# Wed, 09 Jun 2021 20:21:51 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.22.0/nats-streaming-server-v0.22.0-windows-amd64.zip
# Wed, 09 Jun 2021 20:21:54 GMT
ENV GIT_DOWNLOAD_SHA256=436c16330efbd0767d9a69dcdf2d3badd4e2598fab23c4f4a192e9d9982c2c92
# Wed, 09 Jun 2021 20:22:22 GMT
RUN Set-PSDebug -Trace 2
# Wed, 09 Jun 2021 20:23:43 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 09 Jun 2021 20:23:45 GMT
EXPOSE 4222 8222
# Wed, 09 Jun 2021 20:23:48 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 09 Jun 2021 20:23:50 GMT
CMD ["-m" "8222"]
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
	-	`sha256:2ce4b948c1a0090b613b7cf3caf73010af9ec5e2d3f2f1ff54177cf4d10a3e4b`  
		Last Modified: Wed, 09 Jun 2021 20:28:39 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:091f859d3e2c08bea4918bd73dd5179d67ec1cc848d31e861e8d8d54d3135e16`  
		Last Modified: Wed, 09 Jun 2021 20:28:39 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:065cc30c1c1a7502e7a8f8984ef62b8f6dac71d678e5fdbdfc4ac7886ae2dee1`  
		Last Modified: Wed, 09 Jun 2021 20:28:39 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:907007f7199ec34ff53edbf50c29cf96587f12e39407d042ce7ee894bc5c8010`  
		Last Modified: Wed, 09 Jun 2021 20:28:36 GMT  
		Size: 342.8 KB (342788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98435664ae81c44aa558ea460acb4b57148b65cd80fa1a5873fee91c8d6f784e`  
		Last Modified: Wed, 09 Jun 2021 20:28:44 GMT  
		Size: 7.3 MB (7259596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5089624a9545a210e2098609d71eb68eb27580b3bb9333bfeef73cf7185df9ff`  
		Last Modified: Wed, 09 Jun 2021 20:28:36 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc477e9744316e1163a516d61b0d028bf9876b297a2aeff872ab83c478c89d89`  
		Last Modified: Wed, 09 Jun 2021 20:28:36 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f65a67fb6dd9f5bb509e1e9f4ad38f5beed7d810d2f7ffc39a961be929c95228`  
		Last Modified: Wed, 09 Jun 2021 20:28:36 GMT  
		Size: 1.4 KB (1385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.22-windowsservercore-ltsc2016`

```console
$ docker pull nats-streaming@sha256:78dfec8176857148ddb64a840849ab4e2a2e717f41402c8d82122aae81a02fb8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4467; amd64

### `nats-streaming:0.22-windowsservercore-ltsc2016` - windows version 10.0.14393.4467; amd64

```console
$ docker pull nats-streaming@sha256:c1d1676348d3cc256527165d36fdb7096c23cadb25a41724b9d716e816930192
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6277864201 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed49864d98975c3b2d97e536c6f86c43a8d6df1e09903b12259a9d5009fb1b07`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
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
# Wed, 09 Jun 2021 20:24:18 GMT
ENV NATS_STREAMING_SERVER=0.22.0
# Wed, 09 Jun 2021 20:24:20 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.22.0/nats-streaming-server-v0.22.0-windows-amd64.zip
# Wed, 09 Jun 2021 20:24:22 GMT
ENV GIT_DOWNLOAD_SHA256=436c16330efbd0767d9a69dcdf2d3badd4e2598fab23c4f4a192e9d9982c2c92
# Wed, 09 Jun 2021 20:25:38 GMT
RUN Set-PSDebug -Trace 2
# Wed, 09 Jun 2021 20:27:59 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 09 Jun 2021 20:28:02 GMT
EXPOSE 4222 8222
# Wed, 09 Jun 2021 20:28:05 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 09 Jun 2021 20:28:07 GMT
CMD ["-m" "8222"]
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
	-	`sha256:dc5848e927e0f88d330cfd4d69ff5b33a883c0926f224b083d84658b124b4eff`  
		Last Modified: Wed, 09 Jun 2021 20:29:21 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c560d2270f78e7dec252e2f64f0e115ce098ccb7e292f89dc10e8c96b6409b7a`  
		Last Modified: Wed, 09 Jun 2021 20:29:21 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8df992a1ddf947618230669ac99ede1f6100d23bffefc379015097d6ab55de11`  
		Last Modified: Wed, 09 Jun 2021 20:29:20 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d1c5d78268da7d5a12285ca6e0b9ee14a4c092effdf1f0c1ef9def8724a38dc`  
		Last Modified: Wed, 09 Jun 2021 20:29:18 GMT  
		Size: 341.8 KB (341824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21e2d30fad367283448bcc184a08542dfd3e4d0f13691f608f48111fa360ca8a`  
		Last Modified: Wed, 09 Jun 2021 20:29:21 GMT  
		Size: 11.8 MB (11783856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90a63b8e3d31cde8595bcc53bffd235ec17496ec80e358d2dd963fe75965ea1e`  
		Last Modified: Wed, 09 Jun 2021 20:29:18 GMT  
		Size: 1.4 KB (1444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e14db649ae2c7bc33a1fad8a90d8ebec3336062ba22a9922f7e5fc3af262b470`  
		Last Modified: Wed, 09 Jun 2021 20:29:18 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5715b2e77233052328e64dc4f9dcbe9fb8a8f8d0b452405716447e4addb11458`  
		Last Modified: Wed, 09 Jun 2021 20:29:18 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.22.0`

```console
$ docker pull nats-streaming@sha256:05ae257f52770a83cab1f239eaeacc1954cd48cb6218782a619ba3fcc12dbd6c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.1999; amd64

### `nats-streaming:0.22.0` - linux; amd64

```console
$ docker pull nats-streaming@sha256:ba1be2cd913a1e9f1ffc9445e5c04c169db333819beb7204deb3bc7c29fde5a8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6800613 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12f2d32e0c9a23e5a9a5cb19c8b1404a9cc7af17915e33eabb71e55767848df7`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Wed, 02 Jun 2021 05:47:24 GMT
COPY file:bbdef008b65f574a4e4593641e45dd6cdff5e8261d06d8f3959963f686dcdb78 in /nats-streaming-server 
# Wed, 02 Jun 2021 05:47:24 GMT
EXPOSE 4222 8222
# Wed, 02 Jun 2021 05:47:24 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Wed, 02 Jun 2021 05:47:24 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:afa0998a9989cfec22c4ad772da3ca685ea7ccf963253ff9c27edf33a00d49c6`  
		Last Modified: Wed, 02 Jun 2021 05:48:07 GMT  
		Size: 6.8 MB (6800613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.22.0` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:1bef88847972d6206955fdc84742cb2505dcdf9ec86c2ef8bd6b5629c88ef2f3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 MB (6269700 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:258e5207bc79452baf170c0dc0a5c955f71c72fadc9fff82bffecc06eb3e1e81`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 01 Jun 2021 23:54:46 GMT
COPY file:a4f69de3d07c6870dde4796b4de69a931a699d7e5b6ec30b2f25f6a23d66cb33 in /nats-streaming-server 
# Tue, 01 Jun 2021 23:54:47 GMT
EXPOSE 4222 8222
# Tue, 01 Jun 2021 23:54:47 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 01 Jun 2021 23:54:47 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:8ab135edb380ca588ed7d11dbea1418006a6708ae7ae5effad8d86bcef90198e`  
		Last Modified: Tue, 01 Jun 2021 23:56:26 GMT  
		Size: 6.3 MB (6269700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.22.0` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:a6c122176a5ff4bdae9a653ebb1cf3e0672cd240250547b855ae0f8894496225
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 MB (6259769 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ccaf377f82ea563a543d1a8bcf9a53870f6427a0cacae9f9ad5e46e6c7eabff`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Wed, 02 Jun 2021 03:13:19 GMT
COPY file:6e08520addf5d0c5d064e431d76487779d8fd8f4c03f71a72dc4e2c81812a922 in /nats-streaming-server 
# Wed, 02 Jun 2021 03:13:20 GMT
EXPOSE 4222 8222
# Wed, 02 Jun 2021 03:13:20 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Wed, 02 Jun 2021 03:13:20 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:887fd90bbdf32bb85ec9e85b63e60eccca791d6c882e30de0c10e6e583ccbb65`  
		Last Modified: Wed, 02 Jun 2021 03:15:02 GMT  
		Size: 6.3 MB (6259769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.22.0` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:bd5a415582b3f1d079d6498c12ea9138d7bde01dcd3a5f5a35a1731edf4c889f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.2 MB (6197708 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:16d36744f70db176ba94e376a65c5edda55a7167035e7dffdf217e594c1ac283`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Wed, 02 Jun 2021 02:14:00 GMT
COPY file:ef2047bb70888b72ef213e68689b3b8ae622cc597cd07b313c26b278418788bd in /nats-streaming-server 
# Wed, 02 Jun 2021 02:14:00 GMT
EXPOSE 4222 8222
# Wed, 02 Jun 2021 02:14:01 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Wed, 02 Jun 2021 02:14:01 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:ddf987a265c2be80179a2683a2d725f5a7e9fb477bc5752443a6d955be681a50`  
		Last Modified: Wed, 02 Jun 2021 02:15:07 GMT  
		Size: 6.2 MB (6197708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.22.0` - windows version 10.0.17763.1999; amd64

```console
$ docker pull nats-streaming@sha256:94fafaf460823aa892ed913e1f95a42f617b0b0ade5f63fec023190aad998802
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.6 MB (109610228 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:58e2b8ca8f56a4b97f31133be06094bd3eeb0219661aba4e8aaaad7a79d723c6`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Sun, 06 Jun 2021 04:04:04 GMT
RUN Apply image 1809-amd64
# Wed, 09 Jun 2021 15:55:07 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 09 Jun 2021 20:24:03 GMT
RUN cmd /S /C #(nop) COPY file:72a29a3f2d4a0bd237295ad8b2a317a32c76cbb8a1af898a564024d5013c0475 in C:\nats-streaming-server.exe 
# Wed, 09 Jun 2021 20:24:05 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 09 Jun 2021 20:24:07 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 09 Jun 2021 20:24:10 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:e4800203e906d49fbdaf1eeab4de72f28796d5b9a1ea44f8d7461001cfa56614`  
		Size: 102.7 MB (102671454 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:80d93ce19113bbf944b699f12e59395e0eabeb00ccd1fd5dc7df46bb115eba2f`  
		Last Modified: Wed, 09 Jun 2021 15:59:58 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:348b9d29d0e17e2575302e48a756c01845f95766a27b3efd5037e69dc02c3ffd`  
		Last Modified: Wed, 09 Jun 2021 20:29:05 GMT  
		Size: 6.9 MB (6934149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cfbb95c41b561debff13c2fdc579566b502a46d04cc2aa8636fc043d67cf6f9`  
		Last Modified: Wed, 09 Jun 2021 20:28:57 GMT  
		Size: 1.2 KB (1184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1321261d7f7de3d8a203008e1bd4541c0a15f00938a86e8f610acd674513bff3`  
		Last Modified: Wed, 09 Jun 2021 20:28:57 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58df4d427933ebe735d64a9ffec8fb7774cc74c1158c33e365322810443cc018`  
		Last Modified: Wed, 09 Jun 2021 20:28:57 GMT  
		Size: 1.2 KB (1167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.22.0-alpine`

```console
$ docker pull nats-streaming@sha256:99da8c602fc3b57ef730efda710a4e62d47a9e62c772b854c255081cd7f2f7fa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.22.0-alpine` - linux; amd64

```console
$ docker pull nats-streaming@sha256:25457c5b382da1fb7ab66c4f977ad38915b109e9bf0d4440f2ae2f314d3bcc97
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.9 MB (9894969 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:443be2e221357fdae9e3405207feb4e1f061dce181882a1cf208543e029bc8fa`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Wed, 02 Jun 2021 05:47:13 GMT
ENV NATS_STREAMING_SERVER=0.22.0
# Wed, 02 Jun 2021 05:47:16 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='3ffc4b74f469b97a8ce0edff8b645baf89d9f9f3debdfa7088a0ceac3ed6c37b' ;; 		armhf) natsArch='arm6'; sha256='abe201b1a90cd2e8db39989c81a2c76d3956035745c68d0c7e090fc8c5a138c8' ;; 		armv7) natsArch='arm7'; sha256='d218edd395f980ea91a54624b4cc1fe0220268171ee596a24d7c01c15a7dbb7f' ;; 		x86_64) natsArch='amd64'; sha256='72f5b899167a8866d4b82d1bf9bc14b5d047e6b1ab127dd0085e9eb91a89f097' ;; 		x86) natsArch='386'; sha256='d87bb204228c5e820747e1682dbfb56289e3ddadcfe129b9c9fcf1ad7c0ba053' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 02 Jun 2021 05:47:16 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Wed, 02 Jun 2021 05:47:16 GMT
EXPOSE 4222 8222
# Wed, 02 Jun 2021 05:47:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 02 Jun 2021 05:47:17 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4795908dc4759b01d3e4dd956343fb777c34c32afc57d2a4a96014fa67a41206`  
		Last Modified: Wed, 02 Jun 2021 05:47:46 GMT  
		Size: 7.1 MB (7082579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bf7f8694c616cf8f24559388ba77e2349a8da60a47001bfd26c85997d87b593`  
		Last Modified: Wed, 02 Jun 2021 05:47:45 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.22.0-alpine` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:7bc8b6da7d8065b7aa858b4520894ad45868c6a99266b4388fec303dd7fa4357
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.2 MB (9175683 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1fa8f1250edffbb08905947aa23b69e8cb17e049ac8790674031e8511024fb5d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Tue, 15 Jun 2021 22:57:34 GMT
ADD file:4479f0a51530e039edf231d87201896dcff908aa542a613cdccb015f93dda8a3 in / 
# Tue, 15 Jun 2021 22:57:34 GMT
CMD ["/bin/sh"]
# Wed, 16 Jun 2021 11:21:18 GMT
ENV NATS_STREAMING_SERVER=0.22.0
# Wed, 16 Jun 2021 11:21:21 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='3ffc4b74f469b97a8ce0edff8b645baf89d9f9f3debdfa7088a0ceac3ed6c37b' ;; 		armhf) natsArch='arm6'; sha256='abe201b1a90cd2e8db39989c81a2c76d3956035745c68d0c7e090fc8c5a138c8' ;; 		armv7) natsArch='arm7'; sha256='d218edd395f980ea91a54624b4cc1fe0220268171ee596a24d7c01c15a7dbb7f' ;; 		x86_64) natsArch='amd64'; sha256='72f5b899167a8866d4b82d1bf9bc14b5d047e6b1ab127dd0085e9eb91a89f097' ;; 		x86) natsArch='386'; sha256='d87bb204228c5e820747e1682dbfb56289e3ddadcfe129b9c9fcf1ad7c0ba053' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 16 Jun 2021 11:21:22 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Wed, 16 Jun 2021 11:21:22 GMT
EXPOSE 4222 8222
# Wed, 16 Jun 2021 11:21:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Jun 2021 11:21:22 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:740c950346cf39c85b52576998695c9b909c24a58a8bb1b64cce91fda3ef1d3a`  
		Last Modified: Wed, 14 Apr 2021 18:50:30 GMT  
		Size: 2.6 MB (2622131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25dbe7b857ca17019fb0e3e3b5439aaf5211a0b71cc2e017cb9465df530b8499`  
		Last Modified: Wed, 16 Jun 2021 11:22:38 GMT  
		Size: 6.6 MB (6553129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df6ca706362f12c5b456b49cbb3448d3189e225a08bffffdecb00fe040b2816f`  
		Last Modified: Wed, 16 Jun 2021 11:22:36 GMT  
		Size: 423.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.22.0-alpine` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:094bdcea75742a31480bd4f5771f741f7490f46a7bade1b1e6836fc2ab0e14f9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.0 MB (8967137 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:16a7379dc428ab28ff200036e6f1a917c42724a035ffc0d548ecb01f9954593f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 14 Apr 2021 18:57:39 GMT
ADD file:028c5b473d862250586e174c5dd19b37f8fc3bffbc02d888e72df30f32fd6129 in / 
# Wed, 14 Apr 2021 18:57:39 GMT
CMD ["/bin/sh"]
# Wed, 02 Jun 2021 03:12:59 GMT
ENV NATS_STREAMING_SERVER=0.22.0
# Wed, 02 Jun 2021 03:13:03 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='3ffc4b74f469b97a8ce0edff8b645baf89d9f9f3debdfa7088a0ceac3ed6c37b' ;; 		armhf) natsArch='arm6'; sha256='abe201b1a90cd2e8db39989c81a2c76d3956035745c68d0c7e090fc8c5a138c8' ;; 		armv7) natsArch='arm7'; sha256='d218edd395f980ea91a54624b4cc1fe0220268171ee596a24d7c01c15a7dbb7f' ;; 		x86_64) natsArch='amd64'; sha256='72f5b899167a8866d4b82d1bf9bc14b5d047e6b1ab127dd0085e9eb91a89f097' ;; 		x86) natsArch='386'; sha256='d87bb204228c5e820747e1682dbfb56289e3ddadcfe129b9c9fcf1ad7c0ba053' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 02 Jun 2021 03:13:03 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Wed, 02 Jun 2021 03:13:03 GMT
EXPOSE 4222 8222
# Wed, 02 Jun 2021 03:13:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 02 Jun 2021 03:13:03 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:e160e00eb35d5bc2373770873fbc9c8f5706045b0b06bfd1c364fcf69f02e9fe`  
		Last Modified: Wed, 14 Apr 2021 18:58:36 GMT  
		Size: 2.4 MB (2424145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcef365af48832fc326fce4ba5cec1feba2d3830122e812be8f7c68c4eba747b`  
		Last Modified: Wed, 02 Jun 2021 03:14:30 GMT  
		Size: 6.5 MB (6542570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:773ab986cb0c82686f2f65fa84b5189bb9194ebe32dc1d4f734e8842539f05fc`  
		Last Modified: Wed, 02 Jun 2021 03:14:29 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.22.0-alpine` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:885349fb8c0102784700ebcdedc5f335a0b0079ccc30f93dc8349bb5ff7b3ba6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.2 MB (9192675 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7fbf7556b1dda05ceae2f1e33ba452f09a4e16e136faea904618586f5e8e643c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Tue, 15 Jun 2021 21:45:03 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Tue, 15 Jun 2021 21:45:04 GMT
CMD ["/bin/sh"]
# Wed, 16 Jun 2021 01:10:22 GMT
ENV NATS_STREAMING_SERVER=0.22.0
# Wed, 16 Jun 2021 01:10:25 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='3ffc4b74f469b97a8ce0edff8b645baf89d9f9f3debdfa7088a0ceac3ed6c37b' ;; 		armhf) natsArch='arm6'; sha256='abe201b1a90cd2e8db39989c81a2c76d3956035745c68d0c7e090fc8c5a138c8' ;; 		armv7) natsArch='arm7'; sha256='d218edd395f980ea91a54624b4cc1fe0220268171ee596a24d7c01c15a7dbb7f' ;; 		x86_64) natsArch='amd64'; sha256='72f5b899167a8866d4b82d1bf9bc14b5d047e6b1ab127dd0085e9eb91a89f097' ;; 		x86) natsArch='386'; sha256='d87bb204228c5e820747e1682dbfb56289e3ddadcfe129b9c9fcf1ad7c0ba053' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 16 Jun 2021 01:10:25 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Wed, 16 Jun 2021 01:10:25 GMT
EXPOSE 4222 8222
# Wed, 16 Jun 2021 01:10:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Jun 2021 01:10:26 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ed1df6d6dbc94e5c85bddb8f9a8dbaa65a5f97ef70e3b4c2a6ce6d46611ef62`  
		Last Modified: Wed, 16 Jun 2021 01:11:18 GMT  
		Size: 6.5 MB (6480227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5409d34dbaa07dcbd979022c1e953c405331b8f63d8e51e47e05f1fbedd24241`  
		Last Modified: Wed, 16 Jun 2021 01:11:16 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.22.0-alpine3.13`

```console
$ docker pull nats-streaming@sha256:99da8c602fc3b57ef730efda710a4e62d47a9e62c772b854c255081cd7f2f7fa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.22.0-alpine3.13` - linux; amd64

```console
$ docker pull nats-streaming@sha256:25457c5b382da1fb7ab66c4f977ad38915b109e9bf0d4440f2ae2f314d3bcc97
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.9 MB (9894969 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:443be2e221357fdae9e3405207feb4e1f061dce181882a1cf208543e029bc8fa`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Wed, 02 Jun 2021 05:47:13 GMT
ENV NATS_STREAMING_SERVER=0.22.0
# Wed, 02 Jun 2021 05:47:16 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='3ffc4b74f469b97a8ce0edff8b645baf89d9f9f3debdfa7088a0ceac3ed6c37b' ;; 		armhf) natsArch='arm6'; sha256='abe201b1a90cd2e8db39989c81a2c76d3956035745c68d0c7e090fc8c5a138c8' ;; 		armv7) natsArch='arm7'; sha256='d218edd395f980ea91a54624b4cc1fe0220268171ee596a24d7c01c15a7dbb7f' ;; 		x86_64) natsArch='amd64'; sha256='72f5b899167a8866d4b82d1bf9bc14b5d047e6b1ab127dd0085e9eb91a89f097' ;; 		x86) natsArch='386'; sha256='d87bb204228c5e820747e1682dbfb56289e3ddadcfe129b9c9fcf1ad7c0ba053' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 02 Jun 2021 05:47:16 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Wed, 02 Jun 2021 05:47:16 GMT
EXPOSE 4222 8222
# Wed, 02 Jun 2021 05:47:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 02 Jun 2021 05:47:17 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4795908dc4759b01d3e4dd956343fb777c34c32afc57d2a4a96014fa67a41206`  
		Last Modified: Wed, 02 Jun 2021 05:47:46 GMT  
		Size: 7.1 MB (7082579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bf7f8694c616cf8f24559388ba77e2349a8da60a47001bfd26c85997d87b593`  
		Last Modified: Wed, 02 Jun 2021 05:47:45 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.22.0-alpine3.13` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:7bc8b6da7d8065b7aa858b4520894ad45868c6a99266b4388fec303dd7fa4357
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.2 MB (9175683 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1fa8f1250edffbb08905947aa23b69e8cb17e049ac8790674031e8511024fb5d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Tue, 15 Jun 2021 22:57:34 GMT
ADD file:4479f0a51530e039edf231d87201896dcff908aa542a613cdccb015f93dda8a3 in / 
# Tue, 15 Jun 2021 22:57:34 GMT
CMD ["/bin/sh"]
# Wed, 16 Jun 2021 11:21:18 GMT
ENV NATS_STREAMING_SERVER=0.22.0
# Wed, 16 Jun 2021 11:21:21 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='3ffc4b74f469b97a8ce0edff8b645baf89d9f9f3debdfa7088a0ceac3ed6c37b' ;; 		armhf) natsArch='arm6'; sha256='abe201b1a90cd2e8db39989c81a2c76d3956035745c68d0c7e090fc8c5a138c8' ;; 		armv7) natsArch='arm7'; sha256='d218edd395f980ea91a54624b4cc1fe0220268171ee596a24d7c01c15a7dbb7f' ;; 		x86_64) natsArch='amd64'; sha256='72f5b899167a8866d4b82d1bf9bc14b5d047e6b1ab127dd0085e9eb91a89f097' ;; 		x86) natsArch='386'; sha256='d87bb204228c5e820747e1682dbfb56289e3ddadcfe129b9c9fcf1ad7c0ba053' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 16 Jun 2021 11:21:22 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Wed, 16 Jun 2021 11:21:22 GMT
EXPOSE 4222 8222
# Wed, 16 Jun 2021 11:21:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Jun 2021 11:21:22 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:740c950346cf39c85b52576998695c9b909c24a58a8bb1b64cce91fda3ef1d3a`  
		Last Modified: Wed, 14 Apr 2021 18:50:30 GMT  
		Size: 2.6 MB (2622131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25dbe7b857ca17019fb0e3e3b5439aaf5211a0b71cc2e017cb9465df530b8499`  
		Last Modified: Wed, 16 Jun 2021 11:22:38 GMT  
		Size: 6.6 MB (6553129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df6ca706362f12c5b456b49cbb3448d3189e225a08bffffdecb00fe040b2816f`  
		Last Modified: Wed, 16 Jun 2021 11:22:36 GMT  
		Size: 423.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.22.0-alpine3.13` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:094bdcea75742a31480bd4f5771f741f7490f46a7bade1b1e6836fc2ab0e14f9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.0 MB (8967137 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:16a7379dc428ab28ff200036e6f1a917c42724a035ffc0d548ecb01f9954593f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 14 Apr 2021 18:57:39 GMT
ADD file:028c5b473d862250586e174c5dd19b37f8fc3bffbc02d888e72df30f32fd6129 in / 
# Wed, 14 Apr 2021 18:57:39 GMT
CMD ["/bin/sh"]
# Wed, 02 Jun 2021 03:12:59 GMT
ENV NATS_STREAMING_SERVER=0.22.0
# Wed, 02 Jun 2021 03:13:03 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='3ffc4b74f469b97a8ce0edff8b645baf89d9f9f3debdfa7088a0ceac3ed6c37b' ;; 		armhf) natsArch='arm6'; sha256='abe201b1a90cd2e8db39989c81a2c76d3956035745c68d0c7e090fc8c5a138c8' ;; 		armv7) natsArch='arm7'; sha256='d218edd395f980ea91a54624b4cc1fe0220268171ee596a24d7c01c15a7dbb7f' ;; 		x86_64) natsArch='amd64'; sha256='72f5b899167a8866d4b82d1bf9bc14b5d047e6b1ab127dd0085e9eb91a89f097' ;; 		x86) natsArch='386'; sha256='d87bb204228c5e820747e1682dbfb56289e3ddadcfe129b9c9fcf1ad7c0ba053' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 02 Jun 2021 03:13:03 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Wed, 02 Jun 2021 03:13:03 GMT
EXPOSE 4222 8222
# Wed, 02 Jun 2021 03:13:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 02 Jun 2021 03:13:03 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:e160e00eb35d5bc2373770873fbc9c8f5706045b0b06bfd1c364fcf69f02e9fe`  
		Last Modified: Wed, 14 Apr 2021 18:58:36 GMT  
		Size: 2.4 MB (2424145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcef365af48832fc326fce4ba5cec1feba2d3830122e812be8f7c68c4eba747b`  
		Last Modified: Wed, 02 Jun 2021 03:14:30 GMT  
		Size: 6.5 MB (6542570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:773ab986cb0c82686f2f65fa84b5189bb9194ebe32dc1d4f734e8842539f05fc`  
		Last Modified: Wed, 02 Jun 2021 03:14:29 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.22.0-alpine3.13` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:885349fb8c0102784700ebcdedc5f335a0b0079ccc30f93dc8349bb5ff7b3ba6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.2 MB (9192675 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7fbf7556b1dda05ceae2f1e33ba452f09a4e16e136faea904618586f5e8e643c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Tue, 15 Jun 2021 21:45:03 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Tue, 15 Jun 2021 21:45:04 GMT
CMD ["/bin/sh"]
# Wed, 16 Jun 2021 01:10:22 GMT
ENV NATS_STREAMING_SERVER=0.22.0
# Wed, 16 Jun 2021 01:10:25 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='3ffc4b74f469b97a8ce0edff8b645baf89d9f9f3debdfa7088a0ceac3ed6c37b' ;; 		armhf) natsArch='arm6'; sha256='abe201b1a90cd2e8db39989c81a2c76d3956035745c68d0c7e090fc8c5a138c8' ;; 		armv7) natsArch='arm7'; sha256='d218edd395f980ea91a54624b4cc1fe0220268171ee596a24d7c01c15a7dbb7f' ;; 		x86_64) natsArch='amd64'; sha256='72f5b899167a8866d4b82d1bf9bc14b5d047e6b1ab127dd0085e9eb91a89f097' ;; 		x86) natsArch='386'; sha256='d87bb204228c5e820747e1682dbfb56289e3ddadcfe129b9c9fcf1ad7c0ba053' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 16 Jun 2021 01:10:25 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Wed, 16 Jun 2021 01:10:25 GMT
EXPOSE 4222 8222
# Wed, 16 Jun 2021 01:10:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Jun 2021 01:10:26 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ed1df6d6dbc94e5c85bddb8f9a8dbaa65a5f97ef70e3b4c2a6ce6d46611ef62`  
		Last Modified: Wed, 16 Jun 2021 01:11:18 GMT  
		Size: 6.5 MB (6480227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5409d34dbaa07dcbd979022c1e953c405331b8f63d8e51e47e05f1fbedd24241`  
		Last Modified: Wed, 16 Jun 2021 01:11:16 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.22.0-linux`

```console
$ docker pull nats-streaming@sha256:29a31360a13ce43c1a19b01d048213225f0ca3daaf0ac9f75e4ff9e21fcb656f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.22.0-linux` - linux; amd64

```console
$ docker pull nats-streaming@sha256:ba1be2cd913a1e9f1ffc9445e5c04c169db333819beb7204deb3bc7c29fde5a8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6800613 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12f2d32e0c9a23e5a9a5cb19c8b1404a9cc7af17915e33eabb71e55767848df7`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Wed, 02 Jun 2021 05:47:24 GMT
COPY file:bbdef008b65f574a4e4593641e45dd6cdff5e8261d06d8f3959963f686dcdb78 in /nats-streaming-server 
# Wed, 02 Jun 2021 05:47:24 GMT
EXPOSE 4222 8222
# Wed, 02 Jun 2021 05:47:24 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Wed, 02 Jun 2021 05:47:24 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:afa0998a9989cfec22c4ad772da3ca685ea7ccf963253ff9c27edf33a00d49c6`  
		Last Modified: Wed, 02 Jun 2021 05:48:07 GMT  
		Size: 6.8 MB (6800613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.22.0-linux` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:1bef88847972d6206955fdc84742cb2505dcdf9ec86c2ef8bd6b5629c88ef2f3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 MB (6269700 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:258e5207bc79452baf170c0dc0a5c955f71c72fadc9fff82bffecc06eb3e1e81`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 01 Jun 2021 23:54:46 GMT
COPY file:a4f69de3d07c6870dde4796b4de69a931a699d7e5b6ec30b2f25f6a23d66cb33 in /nats-streaming-server 
# Tue, 01 Jun 2021 23:54:47 GMT
EXPOSE 4222 8222
# Tue, 01 Jun 2021 23:54:47 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 01 Jun 2021 23:54:47 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:8ab135edb380ca588ed7d11dbea1418006a6708ae7ae5effad8d86bcef90198e`  
		Last Modified: Tue, 01 Jun 2021 23:56:26 GMT  
		Size: 6.3 MB (6269700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.22.0-linux` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:a6c122176a5ff4bdae9a653ebb1cf3e0672cd240250547b855ae0f8894496225
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 MB (6259769 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ccaf377f82ea563a543d1a8bcf9a53870f6427a0cacae9f9ad5e46e6c7eabff`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Wed, 02 Jun 2021 03:13:19 GMT
COPY file:6e08520addf5d0c5d064e431d76487779d8fd8f4c03f71a72dc4e2c81812a922 in /nats-streaming-server 
# Wed, 02 Jun 2021 03:13:20 GMT
EXPOSE 4222 8222
# Wed, 02 Jun 2021 03:13:20 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Wed, 02 Jun 2021 03:13:20 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:887fd90bbdf32bb85ec9e85b63e60eccca791d6c882e30de0c10e6e583ccbb65`  
		Last Modified: Wed, 02 Jun 2021 03:15:02 GMT  
		Size: 6.3 MB (6259769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.22.0-linux` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:bd5a415582b3f1d079d6498c12ea9138d7bde01dcd3a5f5a35a1731edf4c889f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.2 MB (6197708 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:16d36744f70db176ba94e376a65c5edda55a7167035e7dffdf217e594c1ac283`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Wed, 02 Jun 2021 02:14:00 GMT
COPY file:ef2047bb70888b72ef213e68689b3b8ae622cc597cd07b313c26b278418788bd in /nats-streaming-server 
# Wed, 02 Jun 2021 02:14:00 GMT
EXPOSE 4222 8222
# Wed, 02 Jun 2021 02:14:01 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Wed, 02 Jun 2021 02:14:01 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:ddf987a265c2be80179a2683a2d725f5a7e9fb477bc5752443a6d955be681a50`  
		Last Modified: Wed, 02 Jun 2021 02:15:07 GMT  
		Size: 6.2 MB (6197708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.22.0-nanoserver`

```console
$ docker pull nats-streaming@sha256:1db69154831d3b3a88080c69533b678362e4d86676ca33b2e50336765c7436bd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1999; amd64

### `nats-streaming:0.22.0-nanoserver` - windows version 10.0.17763.1999; amd64

```console
$ docker pull nats-streaming@sha256:94fafaf460823aa892ed913e1f95a42f617b0b0ade5f63fec023190aad998802
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.6 MB (109610228 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:58e2b8ca8f56a4b97f31133be06094bd3eeb0219661aba4e8aaaad7a79d723c6`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Sun, 06 Jun 2021 04:04:04 GMT
RUN Apply image 1809-amd64
# Wed, 09 Jun 2021 15:55:07 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 09 Jun 2021 20:24:03 GMT
RUN cmd /S /C #(nop) COPY file:72a29a3f2d4a0bd237295ad8b2a317a32c76cbb8a1af898a564024d5013c0475 in C:\nats-streaming-server.exe 
# Wed, 09 Jun 2021 20:24:05 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 09 Jun 2021 20:24:07 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 09 Jun 2021 20:24:10 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:e4800203e906d49fbdaf1eeab4de72f28796d5b9a1ea44f8d7461001cfa56614`  
		Size: 102.7 MB (102671454 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:80d93ce19113bbf944b699f12e59395e0eabeb00ccd1fd5dc7df46bb115eba2f`  
		Last Modified: Wed, 09 Jun 2021 15:59:58 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:348b9d29d0e17e2575302e48a756c01845f95766a27b3efd5037e69dc02c3ffd`  
		Last Modified: Wed, 09 Jun 2021 20:29:05 GMT  
		Size: 6.9 MB (6934149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cfbb95c41b561debff13c2fdc579566b502a46d04cc2aa8636fc043d67cf6f9`  
		Last Modified: Wed, 09 Jun 2021 20:28:57 GMT  
		Size: 1.2 KB (1184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1321261d7f7de3d8a203008e1bd4541c0a15f00938a86e8f610acd674513bff3`  
		Last Modified: Wed, 09 Jun 2021 20:28:57 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58df4d427933ebe735d64a9ffec8fb7774cc74c1158c33e365322810443cc018`  
		Last Modified: Wed, 09 Jun 2021 20:28:57 GMT  
		Size: 1.2 KB (1167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.22.0-nanoserver-1809`

```console
$ docker pull nats-streaming@sha256:1db69154831d3b3a88080c69533b678362e4d86676ca33b2e50336765c7436bd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1999; amd64

### `nats-streaming:0.22.0-nanoserver-1809` - windows version 10.0.17763.1999; amd64

```console
$ docker pull nats-streaming@sha256:94fafaf460823aa892ed913e1f95a42f617b0b0ade5f63fec023190aad998802
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.6 MB (109610228 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:58e2b8ca8f56a4b97f31133be06094bd3eeb0219661aba4e8aaaad7a79d723c6`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Sun, 06 Jun 2021 04:04:04 GMT
RUN Apply image 1809-amd64
# Wed, 09 Jun 2021 15:55:07 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 09 Jun 2021 20:24:03 GMT
RUN cmd /S /C #(nop) COPY file:72a29a3f2d4a0bd237295ad8b2a317a32c76cbb8a1af898a564024d5013c0475 in C:\nats-streaming-server.exe 
# Wed, 09 Jun 2021 20:24:05 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 09 Jun 2021 20:24:07 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 09 Jun 2021 20:24:10 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:e4800203e906d49fbdaf1eeab4de72f28796d5b9a1ea44f8d7461001cfa56614`  
		Size: 102.7 MB (102671454 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:80d93ce19113bbf944b699f12e59395e0eabeb00ccd1fd5dc7df46bb115eba2f`  
		Last Modified: Wed, 09 Jun 2021 15:59:58 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:348b9d29d0e17e2575302e48a756c01845f95766a27b3efd5037e69dc02c3ffd`  
		Last Modified: Wed, 09 Jun 2021 20:29:05 GMT  
		Size: 6.9 MB (6934149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cfbb95c41b561debff13c2fdc579566b502a46d04cc2aa8636fc043d67cf6f9`  
		Last Modified: Wed, 09 Jun 2021 20:28:57 GMT  
		Size: 1.2 KB (1184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1321261d7f7de3d8a203008e1bd4541c0a15f00938a86e8f610acd674513bff3`  
		Last Modified: Wed, 09 Jun 2021 20:28:57 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58df4d427933ebe735d64a9ffec8fb7774cc74c1158c33e365322810443cc018`  
		Last Modified: Wed, 09 Jun 2021 20:28:57 GMT  
		Size: 1.2 KB (1167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.22.0-scratch`

```console
$ docker pull nats-streaming@sha256:29a31360a13ce43c1a19b01d048213225f0ca3daaf0ac9f75e4ff9e21fcb656f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.22.0-scratch` - linux; amd64

```console
$ docker pull nats-streaming@sha256:ba1be2cd913a1e9f1ffc9445e5c04c169db333819beb7204deb3bc7c29fde5a8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6800613 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12f2d32e0c9a23e5a9a5cb19c8b1404a9cc7af17915e33eabb71e55767848df7`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Wed, 02 Jun 2021 05:47:24 GMT
COPY file:bbdef008b65f574a4e4593641e45dd6cdff5e8261d06d8f3959963f686dcdb78 in /nats-streaming-server 
# Wed, 02 Jun 2021 05:47:24 GMT
EXPOSE 4222 8222
# Wed, 02 Jun 2021 05:47:24 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Wed, 02 Jun 2021 05:47:24 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:afa0998a9989cfec22c4ad772da3ca685ea7ccf963253ff9c27edf33a00d49c6`  
		Last Modified: Wed, 02 Jun 2021 05:48:07 GMT  
		Size: 6.8 MB (6800613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.22.0-scratch` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:1bef88847972d6206955fdc84742cb2505dcdf9ec86c2ef8bd6b5629c88ef2f3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 MB (6269700 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:258e5207bc79452baf170c0dc0a5c955f71c72fadc9fff82bffecc06eb3e1e81`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 01 Jun 2021 23:54:46 GMT
COPY file:a4f69de3d07c6870dde4796b4de69a931a699d7e5b6ec30b2f25f6a23d66cb33 in /nats-streaming-server 
# Tue, 01 Jun 2021 23:54:47 GMT
EXPOSE 4222 8222
# Tue, 01 Jun 2021 23:54:47 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 01 Jun 2021 23:54:47 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:8ab135edb380ca588ed7d11dbea1418006a6708ae7ae5effad8d86bcef90198e`  
		Last Modified: Tue, 01 Jun 2021 23:56:26 GMT  
		Size: 6.3 MB (6269700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.22.0-scratch` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:a6c122176a5ff4bdae9a653ebb1cf3e0672cd240250547b855ae0f8894496225
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 MB (6259769 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ccaf377f82ea563a543d1a8bcf9a53870f6427a0cacae9f9ad5e46e6c7eabff`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Wed, 02 Jun 2021 03:13:19 GMT
COPY file:6e08520addf5d0c5d064e431d76487779d8fd8f4c03f71a72dc4e2c81812a922 in /nats-streaming-server 
# Wed, 02 Jun 2021 03:13:20 GMT
EXPOSE 4222 8222
# Wed, 02 Jun 2021 03:13:20 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Wed, 02 Jun 2021 03:13:20 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:887fd90bbdf32bb85ec9e85b63e60eccca791d6c882e30de0c10e6e583ccbb65`  
		Last Modified: Wed, 02 Jun 2021 03:15:02 GMT  
		Size: 6.3 MB (6259769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.22.0-scratch` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:bd5a415582b3f1d079d6498c12ea9138d7bde01dcd3a5f5a35a1731edf4c889f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.2 MB (6197708 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:16d36744f70db176ba94e376a65c5edda55a7167035e7dffdf217e594c1ac283`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Wed, 02 Jun 2021 02:14:00 GMT
COPY file:ef2047bb70888b72ef213e68689b3b8ae622cc597cd07b313c26b278418788bd in /nats-streaming-server 
# Wed, 02 Jun 2021 02:14:00 GMT
EXPOSE 4222 8222
# Wed, 02 Jun 2021 02:14:01 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Wed, 02 Jun 2021 02:14:01 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:ddf987a265c2be80179a2683a2d725f5a7e9fb477bc5752443a6d955be681a50`  
		Last Modified: Wed, 02 Jun 2021 02:15:07 GMT  
		Size: 6.2 MB (6197708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.22.0-windowsservercore`

```console
$ docker pull nats-streaming@sha256:d53324a82d4959035f5ee013123eff935d4b10bcb37fbf63b0e6e37114a7d661
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1999; amd64
	-	windows version 10.0.14393.4467; amd64

### `nats-streaming:0.22.0-windowsservercore` - windows version 10.0.17763.1999; amd64

```console
$ docker pull nats-streaming@sha256:22abf51575f1bd50cccf86230258446c5cf719355e0ad48133786855f2c76c6c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2649198709 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d9a338521a6c092730c8066de4356133fa0b82ec4122f50d54a8fecd8a01ead`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
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
# Wed, 09 Jun 2021 20:21:49 GMT
ENV NATS_STREAMING_SERVER=0.22.0
# Wed, 09 Jun 2021 20:21:51 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.22.0/nats-streaming-server-v0.22.0-windows-amd64.zip
# Wed, 09 Jun 2021 20:21:54 GMT
ENV GIT_DOWNLOAD_SHA256=436c16330efbd0767d9a69dcdf2d3badd4e2598fab23c4f4a192e9d9982c2c92
# Wed, 09 Jun 2021 20:22:22 GMT
RUN Set-PSDebug -Trace 2
# Wed, 09 Jun 2021 20:23:43 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 09 Jun 2021 20:23:45 GMT
EXPOSE 4222 8222
# Wed, 09 Jun 2021 20:23:48 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 09 Jun 2021 20:23:50 GMT
CMD ["-m" "8222"]
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
	-	`sha256:2ce4b948c1a0090b613b7cf3caf73010af9ec5e2d3f2f1ff54177cf4d10a3e4b`  
		Last Modified: Wed, 09 Jun 2021 20:28:39 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:091f859d3e2c08bea4918bd73dd5179d67ec1cc848d31e861e8d8d54d3135e16`  
		Last Modified: Wed, 09 Jun 2021 20:28:39 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:065cc30c1c1a7502e7a8f8984ef62b8f6dac71d678e5fdbdfc4ac7886ae2dee1`  
		Last Modified: Wed, 09 Jun 2021 20:28:39 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:907007f7199ec34ff53edbf50c29cf96587f12e39407d042ce7ee894bc5c8010`  
		Last Modified: Wed, 09 Jun 2021 20:28:36 GMT  
		Size: 342.8 KB (342788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98435664ae81c44aa558ea460acb4b57148b65cd80fa1a5873fee91c8d6f784e`  
		Last Modified: Wed, 09 Jun 2021 20:28:44 GMT  
		Size: 7.3 MB (7259596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5089624a9545a210e2098609d71eb68eb27580b3bb9333bfeef73cf7185df9ff`  
		Last Modified: Wed, 09 Jun 2021 20:28:36 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc477e9744316e1163a516d61b0d028bf9876b297a2aeff872ab83c478c89d89`  
		Last Modified: Wed, 09 Jun 2021 20:28:36 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f65a67fb6dd9f5bb509e1e9f4ad38f5beed7d810d2f7ffc39a961be929c95228`  
		Last Modified: Wed, 09 Jun 2021 20:28:36 GMT  
		Size: 1.4 KB (1385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.22.0-windowsservercore` - windows version 10.0.14393.4467; amd64

```console
$ docker pull nats-streaming@sha256:c1d1676348d3cc256527165d36fdb7096c23cadb25a41724b9d716e816930192
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6277864201 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed49864d98975c3b2d97e536c6f86c43a8d6df1e09903b12259a9d5009fb1b07`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
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
# Wed, 09 Jun 2021 20:24:18 GMT
ENV NATS_STREAMING_SERVER=0.22.0
# Wed, 09 Jun 2021 20:24:20 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.22.0/nats-streaming-server-v0.22.0-windows-amd64.zip
# Wed, 09 Jun 2021 20:24:22 GMT
ENV GIT_DOWNLOAD_SHA256=436c16330efbd0767d9a69dcdf2d3badd4e2598fab23c4f4a192e9d9982c2c92
# Wed, 09 Jun 2021 20:25:38 GMT
RUN Set-PSDebug -Trace 2
# Wed, 09 Jun 2021 20:27:59 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 09 Jun 2021 20:28:02 GMT
EXPOSE 4222 8222
# Wed, 09 Jun 2021 20:28:05 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 09 Jun 2021 20:28:07 GMT
CMD ["-m" "8222"]
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
	-	`sha256:dc5848e927e0f88d330cfd4d69ff5b33a883c0926f224b083d84658b124b4eff`  
		Last Modified: Wed, 09 Jun 2021 20:29:21 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c560d2270f78e7dec252e2f64f0e115ce098ccb7e292f89dc10e8c96b6409b7a`  
		Last Modified: Wed, 09 Jun 2021 20:29:21 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8df992a1ddf947618230669ac99ede1f6100d23bffefc379015097d6ab55de11`  
		Last Modified: Wed, 09 Jun 2021 20:29:20 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d1c5d78268da7d5a12285ca6e0b9ee14a4c092effdf1f0c1ef9def8724a38dc`  
		Last Modified: Wed, 09 Jun 2021 20:29:18 GMT  
		Size: 341.8 KB (341824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21e2d30fad367283448bcc184a08542dfd3e4d0f13691f608f48111fa360ca8a`  
		Last Modified: Wed, 09 Jun 2021 20:29:21 GMT  
		Size: 11.8 MB (11783856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90a63b8e3d31cde8595bcc53bffd235ec17496ec80e358d2dd963fe75965ea1e`  
		Last Modified: Wed, 09 Jun 2021 20:29:18 GMT  
		Size: 1.4 KB (1444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e14db649ae2c7bc33a1fad8a90d8ebec3336062ba22a9922f7e5fc3af262b470`  
		Last Modified: Wed, 09 Jun 2021 20:29:18 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5715b2e77233052328e64dc4f9dcbe9fb8a8f8d0b452405716447e4addb11458`  
		Last Modified: Wed, 09 Jun 2021 20:29:18 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.22.0-windowsservercore-1809`

```console
$ docker pull nats-streaming@sha256:cf19c0a807a7bc0417a8331f534bef50ae3147a7302679b2370a0976de91d4d2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1999; amd64

### `nats-streaming:0.22.0-windowsservercore-1809` - windows version 10.0.17763.1999; amd64

```console
$ docker pull nats-streaming@sha256:22abf51575f1bd50cccf86230258446c5cf719355e0ad48133786855f2c76c6c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2649198709 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d9a338521a6c092730c8066de4356133fa0b82ec4122f50d54a8fecd8a01ead`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
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
# Wed, 09 Jun 2021 20:21:49 GMT
ENV NATS_STREAMING_SERVER=0.22.0
# Wed, 09 Jun 2021 20:21:51 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.22.0/nats-streaming-server-v0.22.0-windows-amd64.zip
# Wed, 09 Jun 2021 20:21:54 GMT
ENV GIT_DOWNLOAD_SHA256=436c16330efbd0767d9a69dcdf2d3badd4e2598fab23c4f4a192e9d9982c2c92
# Wed, 09 Jun 2021 20:22:22 GMT
RUN Set-PSDebug -Trace 2
# Wed, 09 Jun 2021 20:23:43 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 09 Jun 2021 20:23:45 GMT
EXPOSE 4222 8222
# Wed, 09 Jun 2021 20:23:48 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 09 Jun 2021 20:23:50 GMT
CMD ["-m" "8222"]
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
	-	`sha256:2ce4b948c1a0090b613b7cf3caf73010af9ec5e2d3f2f1ff54177cf4d10a3e4b`  
		Last Modified: Wed, 09 Jun 2021 20:28:39 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:091f859d3e2c08bea4918bd73dd5179d67ec1cc848d31e861e8d8d54d3135e16`  
		Last Modified: Wed, 09 Jun 2021 20:28:39 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:065cc30c1c1a7502e7a8f8984ef62b8f6dac71d678e5fdbdfc4ac7886ae2dee1`  
		Last Modified: Wed, 09 Jun 2021 20:28:39 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:907007f7199ec34ff53edbf50c29cf96587f12e39407d042ce7ee894bc5c8010`  
		Last Modified: Wed, 09 Jun 2021 20:28:36 GMT  
		Size: 342.8 KB (342788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98435664ae81c44aa558ea460acb4b57148b65cd80fa1a5873fee91c8d6f784e`  
		Last Modified: Wed, 09 Jun 2021 20:28:44 GMT  
		Size: 7.3 MB (7259596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5089624a9545a210e2098609d71eb68eb27580b3bb9333bfeef73cf7185df9ff`  
		Last Modified: Wed, 09 Jun 2021 20:28:36 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc477e9744316e1163a516d61b0d028bf9876b297a2aeff872ab83c478c89d89`  
		Last Modified: Wed, 09 Jun 2021 20:28:36 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f65a67fb6dd9f5bb509e1e9f4ad38f5beed7d810d2f7ffc39a961be929c95228`  
		Last Modified: Wed, 09 Jun 2021 20:28:36 GMT  
		Size: 1.4 KB (1385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.22.0-windowsservercore-ltsc2016`

```console
$ docker pull nats-streaming@sha256:78dfec8176857148ddb64a840849ab4e2a2e717f41402c8d82122aae81a02fb8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4467; amd64

### `nats-streaming:0.22.0-windowsservercore-ltsc2016` - windows version 10.0.14393.4467; amd64

```console
$ docker pull nats-streaming@sha256:c1d1676348d3cc256527165d36fdb7096c23cadb25a41724b9d716e816930192
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6277864201 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed49864d98975c3b2d97e536c6f86c43a8d6df1e09903b12259a9d5009fb1b07`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
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
# Wed, 09 Jun 2021 20:24:18 GMT
ENV NATS_STREAMING_SERVER=0.22.0
# Wed, 09 Jun 2021 20:24:20 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.22.0/nats-streaming-server-v0.22.0-windows-amd64.zip
# Wed, 09 Jun 2021 20:24:22 GMT
ENV GIT_DOWNLOAD_SHA256=436c16330efbd0767d9a69dcdf2d3badd4e2598fab23c4f4a192e9d9982c2c92
# Wed, 09 Jun 2021 20:25:38 GMT
RUN Set-PSDebug -Trace 2
# Wed, 09 Jun 2021 20:27:59 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 09 Jun 2021 20:28:02 GMT
EXPOSE 4222 8222
# Wed, 09 Jun 2021 20:28:05 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 09 Jun 2021 20:28:07 GMT
CMD ["-m" "8222"]
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
	-	`sha256:dc5848e927e0f88d330cfd4d69ff5b33a883c0926f224b083d84658b124b4eff`  
		Last Modified: Wed, 09 Jun 2021 20:29:21 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c560d2270f78e7dec252e2f64f0e115ce098ccb7e292f89dc10e8c96b6409b7a`  
		Last Modified: Wed, 09 Jun 2021 20:29:21 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8df992a1ddf947618230669ac99ede1f6100d23bffefc379015097d6ab55de11`  
		Last Modified: Wed, 09 Jun 2021 20:29:20 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d1c5d78268da7d5a12285ca6e0b9ee14a4c092effdf1f0c1ef9def8724a38dc`  
		Last Modified: Wed, 09 Jun 2021 20:29:18 GMT  
		Size: 341.8 KB (341824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21e2d30fad367283448bcc184a08542dfd3e4d0f13691f608f48111fa360ca8a`  
		Last Modified: Wed, 09 Jun 2021 20:29:21 GMT  
		Size: 11.8 MB (11783856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90a63b8e3d31cde8595bcc53bffd235ec17496ec80e358d2dd963fe75965ea1e`  
		Last Modified: Wed, 09 Jun 2021 20:29:18 GMT  
		Size: 1.4 KB (1444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e14db649ae2c7bc33a1fad8a90d8ebec3336062ba22a9922f7e5fc3af262b470`  
		Last Modified: Wed, 09 Jun 2021 20:29:18 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5715b2e77233052328e64dc4f9dcbe9fb8a8f8d0b452405716447e4addb11458`  
		Last Modified: Wed, 09 Jun 2021 20:29:18 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:alpine`

```console
$ docker pull nats-streaming@sha256:99da8c602fc3b57ef730efda710a4e62d47a9e62c772b854c255081cd7f2f7fa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:alpine` - linux; amd64

```console
$ docker pull nats-streaming@sha256:25457c5b382da1fb7ab66c4f977ad38915b109e9bf0d4440f2ae2f314d3bcc97
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.9 MB (9894969 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:443be2e221357fdae9e3405207feb4e1f061dce181882a1cf208543e029bc8fa`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Wed, 02 Jun 2021 05:47:13 GMT
ENV NATS_STREAMING_SERVER=0.22.0
# Wed, 02 Jun 2021 05:47:16 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='3ffc4b74f469b97a8ce0edff8b645baf89d9f9f3debdfa7088a0ceac3ed6c37b' ;; 		armhf) natsArch='arm6'; sha256='abe201b1a90cd2e8db39989c81a2c76d3956035745c68d0c7e090fc8c5a138c8' ;; 		armv7) natsArch='arm7'; sha256='d218edd395f980ea91a54624b4cc1fe0220268171ee596a24d7c01c15a7dbb7f' ;; 		x86_64) natsArch='amd64'; sha256='72f5b899167a8866d4b82d1bf9bc14b5d047e6b1ab127dd0085e9eb91a89f097' ;; 		x86) natsArch='386'; sha256='d87bb204228c5e820747e1682dbfb56289e3ddadcfe129b9c9fcf1ad7c0ba053' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 02 Jun 2021 05:47:16 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Wed, 02 Jun 2021 05:47:16 GMT
EXPOSE 4222 8222
# Wed, 02 Jun 2021 05:47:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 02 Jun 2021 05:47:17 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4795908dc4759b01d3e4dd956343fb777c34c32afc57d2a4a96014fa67a41206`  
		Last Modified: Wed, 02 Jun 2021 05:47:46 GMT  
		Size: 7.1 MB (7082579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bf7f8694c616cf8f24559388ba77e2349a8da60a47001bfd26c85997d87b593`  
		Last Modified: Wed, 02 Jun 2021 05:47:45 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:7bc8b6da7d8065b7aa858b4520894ad45868c6a99266b4388fec303dd7fa4357
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.2 MB (9175683 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1fa8f1250edffbb08905947aa23b69e8cb17e049ac8790674031e8511024fb5d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Tue, 15 Jun 2021 22:57:34 GMT
ADD file:4479f0a51530e039edf231d87201896dcff908aa542a613cdccb015f93dda8a3 in / 
# Tue, 15 Jun 2021 22:57:34 GMT
CMD ["/bin/sh"]
# Wed, 16 Jun 2021 11:21:18 GMT
ENV NATS_STREAMING_SERVER=0.22.0
# Wed, 16 Jun 2021 11:21:21 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='3ffc4b74f469b97a8ce0edff8b645baf89d9f9f3debdfa7088a0ceac3ed6c37b' ;; 		armhf) natsArch='arm6'; sha256='abe201b1a90cd2e8db39989c81a2c76d3956035745c68d0c7e090fc8c5a138c8' ;; 		armv7) natsArch='arm7'; sha256='d218edd395f980ea91a54624b4cc1fe0220268171ee596a24d7c01c15a7dbb7f' ;; 		x86_64) natsArch='amd64'; sha256='72f5b899167a8866d4b82d1bf9bc14b5d047e6b1ab127dd0085e9eb91a89f097' ;; 		x86) natsArch='386'; sha256='d87bb204228c5e820747e1682dbfb56289e3ddadcfe129b9c9fcf1ad7c0ba053' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 16 Jun 2021 11:21:22 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Wed, 16 Jun 2021 11:21:22 GMT
EXPOSE 4222 8222
# Wed, 16 Jun 2021 11:21:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Jun 2021 11:21:22 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:740c950346cf39c85b52576998695c9b909c24a58a8bb1b64cce91fda3ef1d3a`  
		Last Modified: Wed, 14 Apr 2021 18:50:30 GMT  
		Size: 2.6 MB (2622131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25dbe7b857ca17019fb0e3e3b5439aaf5211a0b71cc2e017cb9465df530b8499`  
		Last Modified: Wed, 16 Jun 2021 11:22:38 GMT  
		Size: 6.6 MB (6553129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df6ca706362f12c5b456b49cbb3448d3189e225a08bffffdecb00fe040b2816f`  
		Last Modified: Wed, 16 Jun 2021 11:22:36 GMT  
		Size: 423.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:094bdcea75742a31480bd4f5771f741f7490f46a7bade1b1e6836fc2ab0e14f9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.0 MB (8967137 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:16a7379dc428ab28ff200036e6f1a917c42724a035ffc0d548ecb01f9954593f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 14 Apr 2021 18:57:39 GMT
ADD file:028c5b473d862250586e174c5dd19b37f8fc3bffbc02d888e72df30f32fd6129 in / 
# Wed, 14 Apr 2021 18:57:39 GMT
CMD ["/bin/sh"]
# Wed, 02 Jun 2021 03:12:59 GMT
ENV NATS_STREAMING_SERVER=0.22.0
# Wed, 02 Jun 2021 03:13:03 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='3ffc4b74f469b97a8ce0edff8b645baf89d9f9f3debdfa7088a0ceac3ed6c37b' ;; 		armhf) natsArch='arm6'; sha256='abe201b1a90cd2e8db39989c81a2c76d3956035745c68d0c7e090fc8c5a138c8' ;; 		armv7) natsArch='arm7'; sha256='d218edd395f980ea91a54624b4cc1fe0220268171ee596a24d7c01c15a7dbb7f' ;; 		x86_64) natsArch='amd64'; sha256='72f5b899167a8866d4b82d1bf9bc14b5d047e6b1ab127dd0085e9eb91a89f097' ;; 		x86) natsArch='386'; sha256='d87bb204228c5e820747e1682dbfb56289e3ddadcfe129b9c9fcf1ad7c0ba053' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 02 Jun 2021 03:13:03 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Wed, 02 Jun 2021 03:13:03 GMT
EXPOSE 4222 8222
# Wed, 02 Jun 2021 03:13:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 02 Jun 2021 03:13:03 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:e160e00eb35d5bc2373770873fbc9c8f5706045b0b06bfd1c364fcf69f02e9fe`  
		Last Modified: Wed, 14 Apr 2021 18:58:36 GMT  
		Size: 2.4 MB (2424145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcef365af48832fc326fce4ba5cec1feba2d3830122e812be8f7c68c4eba747b`  
		Last Modified: Wed, 02 Jun 2021 03:14:30 GMT  
		Size: 6.5 MB (6542570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:773ab986cb0c82686f2f65fa84b5189bb9194ebe32dc1d4f734e8842539f05fc`  
		Last Modified: Wed, 02 Jun 2021 03:14:29 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:885349fb8c0102784700ebcdedc5f335a0b0079ccc30f93dc8349bb5ff7b3ba6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.2 MB (9192675 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7fbf7556b1dda05ceae2f1e33ba452f09a4e16e136faea904618586f5e8e643c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Tue, 15 Jun 2021 21:45:03 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Tue, 15 Jun 2021 21:45:04 GMT
CMD ["/bin/sh"]
# Wed, 16 Jun 2021 01:10:22 GMT
ENV NATS_STREAMING_SERVER=0.22.0
# Wed, 16 Jun 2021 01:10:25 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='3ffc4b74f469b97a8ce0edff8b645baf89d9f9f3debdfa7088a0ceac3ed6c37b' ;; 		armhf) natsArch='arm6'; sha256='abe201b1a90cd2e8db39989c81a2c76d3956035745c68d0c7e090fc8c5a138c8' ;; 		armv7) natsArch='arm7'; sha256='d218edd395f980ea91a54624b4cc1fe0220268171ee596a24d7c01c15a7dbb7f' ;; 		x86_64) natsArch='amd64'; sha256='72f5b899167a8866d4b82d1bf9bc14b5d047e6b1ab127dd0085e9eb91a89f097' ;; 		x86) natsArch='386'; sha256='d87bb204228c5e820747e1682dbfb56289e3ddadcfe129b9c9fcf1ad7c0ba053' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 16 Jun 2021 01:10:25 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Wed, 16 Jun 2021 01:10:25 GMT
EXPOSE 4222 8222
# Wed, 16 Jun 2021 01:10:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Jun 2021 01:10:26 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ed1df6d6dbc94e5c85bddb8f9a8dbaa65a5f97ef70e3b4c2a6ce6d46611ef62`  
		Last Modified: Wed, 16 Jun 2021 01:11:18 GMT  
		Size: 6.5 MB (6480227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5409d34dbaa07dcbd979022c1e953c405331b8f63d8e51e47e05f1fbedd24241`  
		Last Modified: Wed, 16 Jun 2021 01:11:16 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:alpine3.13`

```console
$ docker pull nats-streaming@sha256:99da8c602fc3b57ef730efda710a4e62d47a9e62c772b854c255081cd7f2f7fa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:alpine3.13` - linux; amd64

```console
$ docker pull nats-streaming@sha256:25457c5b382da1fb7ab66c4f977ad38915b109e9bf0d4440f2ae2f314d3bcc97
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.9 MB (9894969 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:443be2e221357fdae9e3405207feb4e1f061dce181882a1cf208543e029bc8fa`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Wed, 02 Jun 2021 05:47:13 GMT
ENV NATS_STREAMING_SERVER=0.22.0
# Wed, 02 Jun 2021 05:47:16 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='3ffc4b74f469b97a8ce0edff8b645baf89d9f9f3debdfa7088a0ceac3ed6c37b' ;; 		armhf) natsArch='arm6'; sha256='abe201b1a90cd2e8db39989c81a2c76d3956035745c68d0c7e090fc8c5a138c8' ;; 		armv7) natsArch='arm7'; sha256='d218edd395f980ea91a54624b4cc1fe0220268171ee596a24d7c01c15a7dbb7f' ;; 		x86_64) natsArch='amd64'; sha256='72f5b899167a8866d4b82d1bf9bc14b5d047e6b1ab127dd0085e9eb91a89f097' ;; 		x86) natsArch='386'; sha256='d87bb204228c5e820747e1682dbfb56289e3ddadcfe129b9c9fcf1ad7c0ba053' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 02 Jun 2021 05:47:16 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Wed, 02 Jun 2021 05:47:16 GMT
EXPOSE 4222 8222
# Wed, 02 Jun 2021 05:47:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 02 Jun 2021 05:47:17 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4795908dc4759b01d3e4dd956343fb777c34c32afc57d2a4a96014fa67a41206`  
		Last Modified: Wed, 02 Jun 2021 05:47:46 GMT  
		Size: 7.1 MB (7082579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bf7f8694c616cf8f24559388ba77e2349a8da60a47001bfd26c85997d87b593`  
		Last Modified: Wed, 02 Jun 2021 05:47:45 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine3.13` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:7bc8b6da7d8065b7aa858b4520894ad45868c6a99266b4388fec303dd7fa4357
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.2 MB (9175683 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1fa8f1250edffbb08905947aa23b69e8cb17e049ac8790674031e8511024fb5d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Tue, 15 Jun 2021 22:57:34 GMT
ADD file:4479f0a51530e039edf231d87201896dcff908aa542a613cdccb015f93dda8a3 in / 
# Tue, 15 Jun 2021 22:57:34 GMT
CMD ["/bin/sh"]
# Wed, 16 Jun 2021 11:21:18 GMT
ENV NATS_STREAMING_SERVER=0.22.0
# Wed, 16 Jun 2021 11:21:21 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='3ffc4b74f469b97a8ce0edff8b645baf89d9f9f3debdfa7088a0ceac3ed6c37b' ;; 		armhf) natsArch='arm6'; sha256='abe201b1a90cd2e8db39989c81a2c76d3956035745c68d0c7e090fc8c5a138c8' ;; 		armv7) natsArch='arm7'; sha256='d218edd395f980ea91a54624b4cc1fe0220268171ee596a24d7c01c15a7dbb7f' ;; 		x86_64) natsArch='amd64'; sha256='72f5b899167a8866d4b82d1bf9bc14b5d047e6b1ab127dd0085e9eb91a89f097' ;; 		x86) natsArch='386'; sha256='d87bb204228c5e820747e1682dbfb56289e3ddadcfe129b9c9fcf1ad7c0ba053' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 16 Jun 2021 11:21:22 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Wed, 16 Jun 2021 11:21:22 GMT
EXPOSE 4222 8222
# Wed, 16 Jun 2021 11:21:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Jun 2021 11:21:22 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:740c950346cf39c85b52576998695c9b909c24a58a8bb1b64cce91fda3ef1d3a`  
		Last Modified: Wed, 14 Apr 2021 18:50:30 GMT  
		Size: 2.6 MB (2622131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25dbe7b857ca17019fb0e3e3b5439aaf5211a0b71cc2e017cb9465df530b8499`  
		Last Modified: Wed, 16 Jun 2021 11:22:38 GMT  
		Size: 6.6 MB (6553129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df6ca706362f12c5b456b49cbb3448d3189e225a08bffffdecb00fe040b2816f`  
		Last Modified: Wed, 16 Jun 2021 11:22:36 GMT  
		Size: 423.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine3.13` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:094bdcea75742a31480bd4f5771f741f7490f46a7bade1b1e6836fc2ab0e14f9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.0 MB (8967137 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:16a7379dc428ab28ff200036e6f1a917c42724a035ffc0d548ecb01f9954593f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 14 Apr 2021 18:57:39 GMT
ADD file:028c5b473d862250586e174c5dd19b37f8fc3bffbc02d888e72df30f32fd6129 in / 
# Wed, 14 Apr 2021 18:57:39 GMT
CMD ["/bin/sh"]
# Wed, 02 Jun 2021 03:12:59 GMT
ENV NATS_STREAMING_SERVER=0.22.0
# Wed, 02 Jun 2021 03:13:03 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='3ffc4b74f469b97a8ce0edff8b645baf89d9f9f3debdfa7088a0ceac3ed6c37b' ;; 		armhf) natsArch='arm6'; sha256='abe201b1a90cd2e8db39989c81a2c76d3956035745c68d0c7e090fc8c5a138c8' ;; 		armv7) natsArch='arm7'; sha256='d218edd395f980ea91a54624b4cc1fe0220268171ee596a24d7c01c15a7dbb7f' ;; 		x86_64) natsArch='amd64'; sha256='72f5b899167a8866d4b82d1bf9bc14b5d047e6b1ab127dd0085e9eb91a89f097' ;; 		x86) natsArch='386'; sha256='d87bb204228c5e820747e1682dbfb56289e3ddadcfe129b9c9fcf1ad7c0ba053' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 02 Jun 2021 03:13:03 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Wed, 02 Jun 2021 03:13:03 GMT
EXPOSE 4222 8222
# Wed, 02 Jun 2021 03:13:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 02 Jun 2021 03:13:03 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:e160e00eb35d5bc2373770873fbc9c8f5706045b0b06bfd1c364fcf69f02e9fe`  
		Last Modified: Wed, 14 Apr 2021 18:58:36 GMT  
		Size: 2.4 MB (2424145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcef365af48832fc326fce4ba5cec1feba2d3830122e812be8f7c68c4eba747b`  
		Last Modified: Wed, 02 Jun 2021 03:14:30 GMT  
		Size: 6.5 MB (6542570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:773ab986cb0c82686f2f65fa84b5189bb9194ebe32dc1d4f734e8842539f05fc`  
		Last Modified: Wed, 02 Jun 2021 03:14:29 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine3.13` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:885349fb8c0102784700ebcdedc5f335a0b0079ccc30f93dc8349bb5ff7b3ba6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.2 MB (9192675 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7fbf7556b1dda05ceae2f1e33ba452f09a4e16e136faea904618586f5e8e643c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Tue, 15 Jun 2021 21:45:03 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Tue, 15 Jun 2021 21:45:04 GMT
CMD ["/bin/sh"]
# Wed, 16 Jun 2021 01:10:22 GMT
ENV NATS_STREAMING_SERVER=0.22.0
# Wed, 16 Jun 2021 01:10:25 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='3ffc4b74f469b97a8ce0edff8b645baf89d9f9f3debdfa7088a0ceac3ed6c37b' ;; 		armhf) natsArch='arm6'; sha256='abe201b1a90cd2e8db39989c81a2c76d3956035745c68d0c7e090fc8c5a138c8' ;; 		armv7) natsArch='arm7'; sha256='d218edd395f980ea91a54624b4cc1fe0220268171ee596a24d7c01c15a7dbb7f' ;; 		x86_64) natsArch='amd64'; sha256='72f5b899167a8866d4b82d1bf9bc14b5d047e6b1ab127dd0085e9eb91a89f097' ;; 		x86) natsArch='386'; sha256='d87bb204228c5e820747e1682dbfb56289e3ddadcfe129b9c9fcf1ad7c0ba053' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 16 Jun 2021 01:10:25 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Wed, 16 Jun 2021 01:10:25 GMT
EXPOSE 4222 8222
# Wed, 16 Jun 2021 01:10:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Jun 2021 01:10:26 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ed1df6d6dbc94e5c85bddb8f9a8dbaa65a5f97ef70e3b4c2a6ce6d46611ef62`  
		Last Modified: Wed, 16 Jun 2021 01:11:18 GMT  
		Size: 6.5 MB (6480227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5409d34dbaa07dcbd979022c1e953c405331b8f63d8e51e47e05f1fbedd24241`  
		Last Modified: Wed, 16 Jun 2021 01:11:16 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:latest`

```console
$ docker pull nats-streaming@sha256:05ae257f52770a83cab1f239eaeacc1954cd48cb6218782a619ba3fcc12dbd6c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.1999; amd64

### `nats-streaming:latest` - linux; amd64

```console
$ docker pull nats-streaming@sha256:ba1be2cd913a1e9f1ffc9445e5c04c169db333819beb7204deb3bc7c29fde5a8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6800613 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12f2d32e0c9a23e5a9a5cb19c8b1404a9cc7af17915e33eabb71e55767848df7`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Wed, 02 Jun 2021 05:47:24 GMT
COPY file:bbdef008b65f574a4e4593641e45dd6cdff5e8261d06d8f3959963f686dcdb78 in /nats-streaming-server 
# Wed, 02 Jun 2021 05:47:24 GMT
EXPOSE 4222 8222
# Wed, 02 Jun 2021 05:47:24 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Wed, 02 Jun 2021 05:47:24 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:afa0998a9989cfec22c4ad772da3ca685ea7ccf963253ff9c27edf33a00d49c6`  
		Last Modified: Wed, 02 Jun 2021 05:48:07 GMT  
		Size: 6.8 MB (6800613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:latest` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:1bef88847972d6206955fdc84742cb2505dcdf9ec86c2ef8bd6b5629c88ef2f3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 MB (6269700 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:258e5207bc79452baf170c0dc0a5c955f71c72fadc9fff82bffecc06eb3e1e81`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 01 Jun 2021 23:54:46 GMT
COPY file:a4f69de3d07c6870dde4796b4de69a931a699d7e5b6ec30b2f25f6a23d66cb33 in /nats-streaming-server 
# Tue, 01 Jun 2021 23:54:47 GMT
EXPOSE 4222 8222
# Tue, 01 Jun 2021 23:54:47 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 01 Jun 2021 23:54:47 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:8ab135edb380ca588ed7d11dbea1418006a6708ae7ae5effad8d86bcef90198e`  
		Last Modified: Tue, 01 Jun 2021 23:56:26 GMT  
		Size: 6.3 MB (6269700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:latest` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:a6c122176a5ff4bdae9a653ebb1cf3e0672cd240250547b855ae0f8894496225
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 MB (6259769 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ccaf377f82ea563a543d1a8bcf9a53870f6427a0cacae9f9ad5e46e6c7eabff`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Wed, 02 Jun 2021 03:13:19 GMT
COPY file:6e08520addf5d0c5d064e431d76487779d8fd8f4c03f71a72dc4e2c81812a922 in /nats-streaming-server 
# Wed, 02 Jun 2021 03:13:20 GMT
EXPOSE 4222 8222
# Wed, 02 Jun 2021 03:13:20 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Wed, 02 Jun 2021 03:13:20 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:887fd90bbdf32bb85ec9e85b63e60eccca791d6c882e30de0c10e6e583ccbb65`  
		Last Modified: Wed, 02 Jun 2021 03:15:02 GMT  
		Size: 6.3 MB (6259769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:latest` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:bd5a415582b3f1d079d6498c12ea9138d7bde01dcd3a5f5a35a1731edf4c889f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.2 MB (6197708 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:16d36744f70db176ba94e376a65c5edda55a7167035e7dffdf217e594c1ac283`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Wed, 02 Jun 2021 02:14:00 GMT
COPY file:ef2047bb70888b72ef213e68689b3b8ae622cc597cd07b313c26b278418788bd in /nats-streaming-server 
# Wed, 02 Jun 2021 02:14:00 GMT
EXPOSE 4222 8222
# Wed, 02 Jun 2021 02:14:01 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Wed, 02 Jun 2021 02:14:01 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:ddf987a265c2be80179a2683a2d725f5a7e9fb477bc5752443a6d955be681a50`  
		Last Modified: Wed, 02 Jun 2021 02:15:07 GMT  
		Size: 6.2 MB (6197708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:latest` - windows version 10.0.17763.1999; amd64

```console
$ docker pull nats-streaming@sha256:94fafaf460823aa892ed913e1f95a42f617b0b0ade5f63fec023190aad998802
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.6 MB (109610228 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:58e2b8ca8f56a4b97f31133be06094bd3eeb0219661aba4e8aaaad7a79d723c6`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Sun, 06 Jun 2021 04:04:04 GMT
RUN Apply image 1809-amd64
# Wed, 09 Jun 2021 15:55:07 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 09 Jun 2021 20:24:03 GMT
RUN cmd /S /C #(nop) COPY file:72a29a3f2d4a0bd237295ad8b2a317a32c76cbb8a1af898a564024d5013c0475 in C:\nats-streaming-server.exe 
# Wed, 09 Jun 2021 20:24:05 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 09 Jun 2021 20:24:07 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 09 Jun 2021 20:24:10 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:e4800203e906d49fbdaf1eeab4de72f28796d5b9a1ea44f8d7461001cfa56614`  
		Size: 102.7 MB (102671454 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:80d93ce19113bbf944b699f12e59395e0eabeb00ccd1fd5dc7df46bb115eba2f`  
		Last Modified: Wed, 09 Jun 2021 15:59:58 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:348b9d29d0e17e2575302e48a756c01845f95766a27b3efd5037e69dc02c3ffd`  
		Last Modified: Wed, 09 Jun 2021 20:29:05 GMT  
		Size: 6.9 MB (6934149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cfbb95c41b561debff13c2fdc579566b502a46d04cc2aa8636fc043d67cf6f9`  
		Last Modified: Wed, 09 Jun 2021 20:28:57 GMT  
		Size: 1.2 KB (1184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1321261d7f7de3d8a203008e1bd4541c0a15f00938a86e8f610acd674513bff3`  
		Last Modified: Wed, 09 Jun 2021 20:28:57 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58df4d427933ebe735d64a9ffec8fb7774cc74c1158c33e365322810443cc018`  
		Last Modified: Wed, 09 Jun 2021 20:28:57 GMT  
		Size: 1.2 KB (1167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:linux`

```console
$ docker pull nats-streaming@sha256:29a31360a13ce43c1a19b01d048213225f0ca3daaf0ac9f75e4ff9e21fcb656f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:linux` - linux; amd64

```console
$ docker pull nats-streaming@sha256:ba1be2cd913a1e9f1ffc9445e5c04c169db333819beb7204deb3bc7c29fde5a8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6800613 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12f2d32e0c9a23e5a9a5cb19c8b1404a9cc7af17915e33eabb71e55767848df7`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Wed, 02 Jun 2021 05:47:24 GMT
COPY file:bbdef008b65f574a4e4593641e45dd6cdff5e8261d06d8f3959963f686dcdb78 in /nats-streaming-server 
# Wed, 02 Jun 2021 05:47:24 GMT
EXPOSE 4222 8222
# Wed, 02 Jun 2021 05:47:24 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Wed, 02 Jun 2021 05:47:24 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:afa0998a9989cfec22c4ad772da3ca685ea7ccf963253ff9c27edf33a00d49c6`  
		Last Modified: Wed, 02 Jun 2021 05:48:07 GMT  
		Size: 6.8 MB (6800613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:linux` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:1bef88847972d6206955fdc84742cb2505dcdf9ec86c2ef8bd6b5629c88ef2f3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 MB (6269700 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:258e5207bc79452baf170c0dc0a5c955f71c72fadc9fff82bffecc06eb3e1e81`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 01 Jun 2021 23:54:46 GMT
COPY file:a4f69de3d07c6870dde4796b4de69a931a699d7e5b6ec30b2f25f6a23d66cb33 in /nats-streaming-server 
# Tue, 01 Jun 2021 23:54:47 GMT
EXPOSE 4222 8222
# Tue, 01 Jun 2021 23:54:47 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 01 Jun 2021 23:54:47 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:8ab135edb380ca588ed7d11dbea1418006a6708ae7ae5effad8d86bcef90198e`  
		Last Modified: Tue, 01 Jun 2021 23:56:26 GMT  
		Size: 6.3 MB (6269700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:linux` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:a6c122176a5ff4bdae9a653ebb1cf3e0672cd240250547b855ae0f8894496225
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 MB (6259769 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ccaf377f82ea563a543d1a8bcf9a53870f6427a0cacae9f9ad5e46e6c7eabff`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Wed, 02 Jun 2021 03:13:19 GMT
COPY file:6e08520addf5d0c5d064e431d76487779d8fd8f4c03f71a72dc4e2c81812a922 in /nats-streaming-server 
# Wed, 02 Jun 2021 03:13:20 GMT
EXPOSE 4222 8222
# Wed, 02 Jun 2021 03:13:20 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Wed, 02 Jun 2021 03:13:20 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:887fd90bbdf32bb85ec9e85b63e60eccca791d6c882e30de0c10e6e583ccbb65`  
		Last Modified: Wed, 02 Jun 2021 03:15:02 GMT  
		Size: 6.3 MB (6259769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:linux` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:bd5a415582b3f1d079d6498c12ea9138d7bde01dcd3a5f5a35a1731edf4c889f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.2 MB (6197708 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:16d36744f70db176ba94e376a65c5edda55a7167035e7dffdf217e594c1ac283`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Wed, 02 Jun 2021 02:14:00 GMT
COPY file:ef2047bb70888b72ef213e68689b3b8ae622cc597cd07b313c26b278418788bd in /nats-streaming-server 
# Wed, 02 Jun 2021 02:14:00 GMT
EXPOSE 4222 8222
# Wed, 02 Jun 2021 02:14:01 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Wed, 02 Jun 2021 02:14:01 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:ddf987a265c2be80179a2683a2d725f5a7e9fb477bc5752443a6d955be681a50`  
		Last Modified: Wed, 02 Jun 2021 02:15:07 GMT  
		Size: 6.2 MB (6197708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:nanoserver`

```console
$ docker pull nats-streaming@sha256:1db69154831d3b3a88080c69533b678362e4d86676ca33b2e50336765c7436bd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1999; amd64

### `nats-streaming:nanoserver` - windows version 10.0.17763.1999; amd64

```console
$ docker pull nats-streaming@sha256:94fafaf460823aa892ed913e1f95a42f617b0b0ade5f63fec023190aad998802
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.6 MB (109610228 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:58e2b8ca8f56a4b97f31133be06094bd3eeb0219661aba4e8aaaad7a79d723c6`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Sun, 06 Jun 2021 04:04:04 GMT
RUN Apply image 1809-amd64
# Wed, 09 Jun 2021 15:55:07 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 09 Jun 2021 20:24:03 GMT
RUN cmd /S /C #(nop) COPY file:72a29a3f2d4a0bd237295ad8b2a317a32c76cbb8a1af898a564024d5013c0475 in C:\nats-streaming-server.exe 
# Wed, 09 Jun 2021 20:24:05 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 09 Jun 2021 20:24:07 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 09 Jun 2021 20:24:10 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:e4800203e906d49fbdaf1eeab4de72f28796d5b9a1ea44f8d7461001cfa56614`  
		Size: 102.7 MB (102671454 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:80d93ce19113bbf944b699f12e59395e0eabeb00ccd1fd5dc7df46bb115eba2f`  
		Last Modified: Wed, 09 Jun 2021 15:59:58 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:348b9d29d0e17e2575302e48a756c01845f95766a27b3efd5037e69dc02c3ffd`  
		Last Modified: Wed, 09 Jun 2021 20:29:05 GMT  
		Size: 6.9 MB (6934149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cfbb95c41b561debff13c2fdc579566b502a46d04cc2aa8636fc043d67cf6f9`  
		Last Modified: Wed, 09 Jun 2021 20:28:57 GMT  
		Size: 1.2 KB (1184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1321261d7f7de3d8a203008e1bd4541c0a15f00938a86e8f610acd674513bff3`  
		Last Modified: Wed, 09 Jun 2021 20:28:57 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58df4d427933ebe735d64a9ffec8fb7774cc74c1158c33e365322810443cc018`  
		Last Modified: Wed, 09 Jun 2021 20:28:57 GMT  
		Size: 1.2 KB (1167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:nanoserver-1809`

```console
$ docker pull nats-streaming@sha256:1db69154831d3b3a88080c69533b678362e4d86676ca33b2e50336765c7436bd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1999; amd64

### `nats-streaming:nanoserver-1809` - windows version 10.0.17763.1999; amd64

```console
$ docker pull nats-streaming@sha256:94fafaf460823aa892ed913e1f95a42f617b0b0ade5f63fec023190aad998802
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.6 MB (109610228 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:58e2b8ca8f56a4b97f31133be06094bd3eeb0219661aba4e8aaaad7a79d723c6`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Sun, 06 Jun 2021 04:04:04 GMT
RUN Apply image 1809-amd64
# Wed, 09 Jun 2021 15:55:07 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 09 Jun 2021 20:24:03 GMT
RUN cmd /S /C #(nop) COPY file:72a29a3f2d4a0bd237295ad8b2a317a32c76cbb8a1af898a564024d5013c0475 in C:\nats-streaming-server.exe 
# Wed, 09 Jun 2021 20:24:05 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 09 Jun 2021 20:24:07 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 09 Jun 2021 20:24:10 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:e4800203e906d49fbdaf1eeab4de72f28796d5b9a1ea44f8d7461001cfa56614`  
		Size: 102.7 MB (102671454 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:80d93ce19113bbf944b699f12e59395e0eabeb00ccd1fd5dc7df46bb115eba2f`  
		Last Modified: Wed, 09 Jun 2021 15:59:58 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:348b9d29d0e17e2575302e48a756c01845f95766a27b3efd5037e69dc02c3ffd`  
		Last Modified: Wed, 09 Jun 2021 20:29:05 GMT  
		Size: 6.9 MB (6934149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cfbb95c41b561debff13c2fdc579566b502a46d04cc2aa8636fc043d67cf6f9`  
		Last Modified: Wed, 09 Jun 2021 20:28:57 GMT  
		Size: 1.2 KB (1184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1321261d7f7de3d8a203008e1bd4541c0a15f00938a86e8f610acd674513bff3`  
		Last Modified: Wed, 09 Jun 2021 20:28:57 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58df4d427933ebe735d64a9ffec8fb7774cc74c1158c33e365322810443cc018`  
		Last Modified: Wed, 09 Jun 2021 20:28:57 GMT  
		Size: 1.2 KB (1167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:scratch`

```console
$ docker pull nats-streaming@sha256:29a31360a13ce43c1a19b01d048213225f0ca3daaf0ac9f75e4ff9e21fcb656f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:scratch` - linux; amd64

```console
$ docker pull nats-streaming@sha256:ba1be2cd913a1e9f1ffc9445e5c04c169db333819beb7204deb3bc7c29fde5a8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6800613 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12f2d32e0c9a23e5a9a5cb19c8b1404a9cc7af17915e33eabb71e55767848df7`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Wed, 02 Jun 2021 05:47:24 GMT
COPY file:bbdef008b65f574a4e4593641e45dd6cdff5e8261d06d8f3959963f686dcdb78 in /nats-streaming-server 
# Wed, 02 Jun 2021 05:47:24 GMT
EXPOSE 4222 8222
# Wed, 02 Jun 2021 05:47:24 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Wed, 02 Jun 2021 05:47:24 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:afa0998a9989cfec22c4ad772da3ca685ea7ccf963253ff9c27edf33a00d49c6`  
		Last Modified: Wed, 02 Jun 2021 05:48:07 GMT  
		Size: 6.8 MB (6800613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:scratch` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:1bef88847972d6206955fdc84742cb2505dcdf9ec86c2ef8bd6b5629c88ef2f3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 MB (6269700 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:258e5207bc79452baf170c0dc0a5c955f71c72fadc9fff82bffecc06eb3e1e81`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 01 Jun 2021 23:54:46 GMT
COPY file:a4f69de3d07c6870dde4796b4de69a931a699d7e5b6ec30b2f25f6a23d66cb33 in /nats-streaming-server 
# Tue, 01 Jun 2021 23:54:47 GMT
EXPOSE 4222 8222
# Tue, 01 Jun 2021 23:54:47 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 01 Jun 2021 23:54:47 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:8ab135edb380ca588ed7d11dbea1418006a6708ae7ae5effad8d86bcef90198e`  
		Last Modified: Tue, 01 Jun 2021 23:56:26 GMT  
		Size: 6.3 MB (6269700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:scratch` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:a6c122176a5ff4bdae9a653ebb1cf3e0672cd240250547b855ae0f8894496225
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 MB (6259769 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ccaf377f82ea563a543d1a8bcf9a53870f6427a0cacae9f9ad5e46e6c7eabff`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Wed, 02 Jun 2021 03:13:19 GMT
COPY file:6e08520addf5d0c5d064e431d76487779d8fd8f4c03f71a72dc4e2c81812a922 in /nats-streaming-server 
# Wed, 02 Jun 2021 03:13:20 GMT
EXPOSE 4222 8222
# Wed, 02 Jun 2021 03:13:20 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Wed, 02 Jun 2021 03:13:20 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:887fd90bbdf32bb85ec9e85b63e60eccca791d6c882e30de0c10e6e583ccbb65`  
		Last Modified: Wed, 02 Jun 2021 03:15:02 GMT  
		Size: 6.3 MB (6259769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:scratch` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:bd5a415582b3f1d079d6498c12ea9138d7bde01dcd3a5f5a35a1731edf4c889f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.2 MB (6197708 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:16d36744f70db176ba94e376a65c5edda55a7167035e7dffdf217e594c1ac283`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Wed, 02 Jun 2021 02:14:00 GMT
COPY file:ef2047bb70888b72ef213e68689b3b8ae622cc597cd07b313c26b278418788bd in /nats-streaming-server 
# Wed, 02 Jun 2021 02:14:00 GMT
EXPOSE 4222 8222
# Wed, 02 Jun 2021 02:14:01 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Wed, 02 Jun 2021 02:14:01 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:ddf987a265c2be80179a2683a2d725f5a7e9fb477bc5752443a6d955be681a50`  
		Last Modified: Wed, 02 Jun 2021 02:15:07 GMT  
		Size: 6.2 MB (6197708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:windowsservercore`

```console
$ docker pull nats-streaming@sha256:d53324a82d4959035f5ee013123eff935d4b10bcb37fbf63b0e6e37114a7d661
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1999; amd64
	-	windows version 10.0.14393.4467; amd64

### `nats-streaming:windowsservercore` - windows version 10.0.17763.1999; amd64

```console
$ docker pull nats-streaming@sha256:22abf51575f1bd50cccf86230258446c5cf719355e0ad48133786855f2c76c6c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2649198709 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d9a338521a6c092730c8066de4356133fa0b82ec4122f50d54a8fecd8a01ead`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
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
# Wed, 09 Jun 2021 20:21:49 GMT
ENV NATS_STREAMING_SERVER=0.22.0
# Wed, 09 Jun 2021 20:21:51 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.22.0/nats-streaming-server-v0.22.0-windows-amd64.zip
# Wed, 09 Jun 2021 20:21:54 GMT
ENV GIT_DOWNLOAD_SHA256=436c16330efbd0767d9a69dcdf2d3badd4e2598fab23c4f4a192e9d9982c2c92
# Wed, 09 Jun 2021 20:22:22 GMT
RUN Set-PSDebug -Trace 2
# Wed, 09 Jun 2021 20:23:43 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 09 Jun 2021 20:23:45 GMT
EXPOSE 4222 8222
# Wed, 09 Jun 2021 20:23:48 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 09 Jun 2021 20:23:50 GMT
CMD ["-m" "8222"]
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
	-	`sha256:2ce4b948c1a0090b613b7cf3caf73010af9ec5e2d3f2f1ff54177cf4d10a3e4b`  
		Last Modified: Wed, 09 Jun 2021 20:28:39 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:091f859d3e2c08bea4918bd73dd5179d67ec1cc848d31e861e8d8d54d3135e16`  
		Last Modified: Wed, 09 Jun 2021 20:28:39 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:065cc30c1c1a7502e7a8f8984ef62b8f6dac71d678e5fdbdfc4ac7886ae2dee1`  
		Last Modified: Wed, 09 Jun 2021 20:28:39 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:907007f7199ec34ff53edbf50c29cf96587f12e39407d042ce7ee894bc5c8010`  
		Last Modified: Wed, 09 Jun 2021 20:28:36 GMT  
		Size: 342.8 KB (342788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98435664ae81c44aa558ea460acb4b57148b65cd80fa1a5873fee91c8d6f784e`  
		Last Modified: Wed, 09 Jun 2021 20:28:44 GMT  
		Size: 7.3 MB (7259596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5089624a9545a210e2098609d71eb68eb27580b3bb9333bfeef73cf7185df9ff`  
		Last Modified: Wed, 09 Jun 2021 20:28:36 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc477e9744316e1163a516d61b0d028bf9876b297a2aeff872ab83c478c89d89`  
		Last Modified: Wed, 09 Jun 2021 20:28:36 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f65a67fb6dd9f5bb509e1e9f4ad38f5beed7d810d2f7ffc39a961be929c95228`  
		Last Modified: Wed, 09 Jun 2021 20:28:36 GMT  
		Size: 1.4 KB (1385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:windowsservercore` - windows version 10.0.14393.4467; amd64

```console
$ docker pull nats-streaming@sha256:c1d1676348d3cc256527165d36fdb7096c23cadb25a41724b9d716e816930192
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6277864201 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed49864d98975c3b2d97e536c6f86c43a8d6df1e09903b12259a9d5009fb1b07`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
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
# Wed, 09 Jun 2021 20:24:18 GMT
ENV NATS_STREAMING_SERVER=0.22.0
# Wed, 09 Jun 2021 20:24:20 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.22.0/nats-streaming-server-v0.22.0-windows-amd64.zip
# Wed, 09 Jun 2021 20:24:22 GMT
ENV GIT_DOWNLOAD_SHA256=436c16330efbd0767d9a69dcdf2d3badd4e2598fab23c4f4a192e9d9982c2c92
# Wed, 09 Jun 2021 20:25:38 GMT
RUN Set-PSDebug -Trace 2
# Wed, 09 Jun 2021 20:27:59 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 09 Jun 2021 20:28:02 GMT
EXPOSE 4222 8222
# Wed, 09 Jun 2021 20:28:05 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 09 Jun 2021 20:28:07 GMT
CMD ["-m" "8222"]
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
	-	`sha256:dc5848e927e0f88d330cfd4d69ff5b33a883c0926f224b083d84658b124b4eff`  
		Last Modified: Wed, 09 Jun 2021 20:29:21 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c560d2270f78e7dec252e2f64f0e115ce098ccb7e292f89dc10e8c96b6409b7a`  
		Last Modified: Wed, 09 Jun 2021 20:29:21 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8df992a1ddf947618230669ac99ede1f6100d23bffefc379015097d6ab55de11`  
		Last Modified: Wed, 09 Jun 2021 20:29:20 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d1c5d78268da7d5a12285ca6e0b9ee14a4c092effdf1f0c1ef9def8724a38dc`  
		Last Modified: Wed, 09 Jun 2021 20:29:18 GMT  
		Size: 341.8 KB (341824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21e2d30fad367283448bcc184a08542dfd3e4d0f13691f608f48111fa360ca8a`  
		Last Modified: Wed, 09 Jun 2021 20:29:21 GMT  
		Size: 11.8 MB (11783856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90a63b8e3d31cde8595bcc53bffd235ec17496ec80e358d2dd963fe75965ea1e`  
		Last Modified: Wed, 09 Jun 2021 20:29:18 GMT  
		Size: 1.4 KB (1444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e14db649ae2c7bc33a1fad8a90d8ebec3336062ba22a9922f7e5fc3af262b470`  
		Last Modified: Wed, 09 Jun 2021 20:29:18 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5715b2e77233052328e64dc4f9dcbe9fb8a8f8d0b452405716447e4addb11458`  
		Last Modified: Wed, 09 Jun 2021 20:29:18 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:windowsservercore-1809`

```console
$ docker pull nats-streaming@sha256:cf19c0a807a7bc0417a8331f534bef50ae3147a7302679b2370a0976de91d4d2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1999; amd64

### `nats-streaming:windowsservercore-1809` - windows version 10.0.17763.1999; amd64

```console
$ docker pull nats-streaming@sha256:22abf51575f1bd50cccf86230258446c5cf719355e0ad48133786855f2c76c6c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2649198709 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d9a338521a6c092730c8066de4356133fa0b82ec4122f50d54a8fecd8a01ead`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
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
# Wed, 09 Jun 2021 20:21:49 GMT
ENV NATS_STREAMING_SERVER=0.22.0
# Wed, 09 Jun 2021 20:21:51 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.22.0/nats-streaming-server-v0.22.0-windows-amd64.zip
# Wed, 09 Jun 2021 20:21:54 GMT
ENV GIT_DOWNLOAD_SHA256=436c16330efbd0767d9a69dcdf2d3badd4e2598fab23c4f4a192e9d9982c2c92
# Wed, 09 Jun 2021 20:22:22 GMT
RUN Set-PSDebug -Trace 2
# Wed, 09 Jun 2021 20:23:43 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 09 Jun 2021 20:23:45 GMT
EXPOSE 4222 8222
# Wed, 09 Jun 2021 20:23:48 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 09 Jun 2021 20:23:50 GMT
CMD ["-m" "8222"]
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
	-	`sha256:2ce4b948c1a0090b613b7cf3caf73010af9ec5e2d3f2f1ff54177cf4d10a3e4b`  
		Last Modified: Wed, 09 Jun 2021 20:28:39 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:091f859d3e2c08bea4918bd73dd5179d67ec1cc848d31e861e8d8d54d3135e16`  
		Last Modified: Wed, 09 Jun 2021 20:28:39 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:065cc30c1c1a7502e7a8f8984ef62b8f6dac71d678e5fdbdfc4ac7886ae2dee1`  
		Last Modified: Wed, 09 Jun 2021 20:28:39 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:907007f7199ec34ff53edbf50c29cf96587f12e39407d042ce7ee894bc5c8010`  
		Last Modified: Wed, 09 Jun 2021 20:28:36 GMT  
		Size: 342.8 KB (342788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98435664ae81c44aa558ea460acb4b57148b65cd80fa1a5873fee91c8d6f784e`  
		Last Modified: Wed, 09 Jun 2021 20:28:44 GMT  
		Size: 7.3 MB (7259596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5089624a9545a210e2098609d71eb68eb27580b3bb9333bfeef73cf7185df9ff`  
		Last Modified: Wed, 09 Jun 2021 20:28:36 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc477e9744316e1163a516d61b0d028bf9876b297a2aeff872ab83c478c89d89`  
		Last Modified: Wed, 09 Jun 2021 20:28:36 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f65a67fb6dd9f5bb509e1e9f4ad38f5beed7d810d2f7ffc39a961be929c95228`  
		Last Modified: Wed, 09 Jun 2021 20:28:36 GMT  
		Size: 1.4 KB (1385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:windowsservercore-ltsc2016`

```console
$ docker pull nats-streaming@sha256:78dfec8176857148ddb64a840849ab4e2a2e717f41402c8d82122aae81a02fb8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4467; amd64

### `nats-streaming:windowsservercore-ltsc2016` - windows version 10.0.14393.4467; amd64

```console
$ docker pull nats-streaming@sha256:c1d1676348d3cc256527165d36fdb7096c23cadb25a41724b9d716e816930192
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6277864201 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed49864d98975c3b2d97e536c6f86c43a8d6df1e09903b12259a9d5009fb1b07`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
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
# Wed, 09 Jun 2021 20:24:18 GMT
ENV NATS_STREAMING_SERVER=0.22.0
# Wed, 09 Jun 2021 20:24:20 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.22.0/nats-streaming-server-v0.22.0-windows-amd64.zip
# Wed, 09 Jun 2021 20:24:22 GMT
ENV GIT_DOWNLOAD_SHA256=436c16330efbd0767d9a69dcdf2d3badd4e2598fab23c4f4a192e9d9982c2c92
# Wed, 09 Jun 2021 20:25:38 GMT
RUN Set-PSDebug -Trace 2
# Wed, 09 Jun 2021 20:27:59 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 09 Jun 2021 20:28:02 GMT
EXPOSE 4222 8222
# Wed, 09 Jun 2021 20:28:05 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 09 Jun 2021 20:28:07 GMT
CMD ["-m" "8222"]
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
	-	`sha256:dc5848e927e0f88d330cfd4d69ff5b33a883c0926f224b083d84658b124b4eff`  
		Last Modified: Wed, 09 Jun 2021 20:29:21 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c560d2270f78e7dec252e2f64f0e115ce098ccb7e292f89dc10e8c96b6409b7a`  
		Last Modified: Wed, 09 Jun 2021 20:29:21 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8df992a1ddf947618230669ac99ede1f6100d23bffefc379015097d6ab55de11`  
		Last Modified: Wed, 09 Jun 2021 20:29:20 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d1c5d78268da7d5a12285ca6e0b9ee14a4c092effdf1f0c1ef9def8724a38dc`  
		Last Modified: Wed, 09 Jun 2021 20:29:18 GMT  
		Size: 341.8 KB (341824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21e2d30fad367283448bcc184a08542dfd3e4d0f13691f608f48111fa360ca8a`  
		Last Modified: Wed, 09 Jun 2021 20:29:21 GMT  
		Size: 11.8 MB (11783856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90a63b8e3d31cde8595bcc53bffd235ec17496ec80e358d2dd963fe75965ea1e`  
		Last Modified: Wed, 09 Jun 2021 20:29:18 GMT  
		Size: 1.4 KB (1444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e14db649ae2c7bc33a1fad8a90d8ebec3336062ba22a9922f7e5fc3af262b470`  
		Last Modified: Wed, 09 Jun 2021 20:29:18 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5715b2e77233052328e64dc4f9dcbe9fb8a8f8d0b452405716447e4addb11458`  
		Last Modified: Wed, 09 Jun 2021 20:29:18 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
