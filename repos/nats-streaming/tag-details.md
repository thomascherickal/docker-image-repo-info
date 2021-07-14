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
$ docker pull nats-streaming@sha256:edf770c6014121e4ea3aac9d7493a33db0256a2e4424a8463446e6649919dbee
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.2061; amd64

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

### `nats-streaming:0.22` - windows version 10.0.17763.2061; amd64

```console
$ docker pull nats-streaming@sha256:9d7e58b6bd4fd1ef45339a3497ef7d6a402444f4015ad419d920758ad398c253
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.7 MB (109664361 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ba10fd6c3016a2b0355ec120bdecdcd05c850fb5881ef2436371c86c57688f7`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 06 Jul 2021 20:06:39 GMT
RUN Apply image 1809-amd64
# Wed, 14 Jul 2021 02:35:24 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 14 Jul 2021 18:09:34 GMT
RUN cmd /S /C #(nop) COPY file:72a29a3f2d4a0bd237295ad8b2a317a32c76cbb8a1af898a564024d5013c0475 in C:\nats-streaming-server.exe 
# Wed, 14 Jul 2021 18:09:38 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 14 Jul 2021 18:09:41 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 14 Jul 2021 18:09:44 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:29d43e56445c5279a6386c4dfe4d1ada3c7124ade9cb7b0f2757e58ffc7cd10b`  
		Size: 102.7 MB (102725622 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ec20c4c9f6fa5e782e09342d50033ef24c4049a9dad1befd33c96759b71da6de`  
		Last Modified: Wed, 14 Jul 2021 02:40:36 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c90e8afac4445cb889af58b8a590bdc86382f1e91b54e20bc1009269430e8d7b`  
		Last Modified: Wed, 14 Jul 2021 18:14:47 GMT  
		Size: 6.9 MB (6934158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54dedbbe81a86e2b328335cbf90c2056b3cf884b7bb41a3a2322b58509040298`  
		Last Modified: Wed, 14 Jul 2021 18:14:45 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7b0a78349321bd097f09f3ac8c826322e4c48a945f77e33b86e5699f7477180`  
		Last Modified: Wed, 14 Jul 2021 18:14:45 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c19f14b31cad0b01978407b9da3ddcdd9b2ee36d8a558aa4a30f5bcb62c6ab63`  
		Last Modified: Wed, 14 Jul 2021 18:14:45 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.22-alpine`

```console
$ docker pull nats-streaming@sha256:a06335f6921f2afb19872d3fa0a852f37390de4a9322b6fe0499f6223f56f595
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
$ docker pull nats-streaming@sha256:8b2d71e9d5ba6e809239f8689f194badfe4604cf66b8663f284ba101268c1057
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.0 MB (8967124 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:313d2bfb32eb974d6db3373750c748020c32ab3d2af5783131fc457c185427a0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Tue, 15 Jun 2021 23:15:15 GMT
ADD file:028c5b473d862250586e174c5dd19b37f8fc3bffbc02d888e72df30f32fd6129 in / 
# Tue, 15 Jun 2021 23:15:16 GMT
CMD ["/bin/sh"]
# Wed, 16 Jun 2021 13:43:31 GMT
ENV NATS_STREAMING_SERVER=0.22.0
# Wed, 16 Jun 2021 13:43:35 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='3ffc4b74f469b97a8ce0edff8b645baf89d9f9f3debdfa7088a0ceac3ed6c37b' ;; 		armhf) natsArch='arm6'; sha256='abe201b1a90cd2e8db39989c81a2c76d3956035745c68d0c7e090fc8c5a138c8' ;; 		armv7) natsArch='arm7'; sha256='d218edd395f980ea91a54624b4cc1fe0220268171ee596a24d7c01c15a7dbb7f' ;; 		x86_64) natsArch='amd64'; sha256='72f5b899167a8866d4b82d1bf9bc14b5d047e6b1ab127dd0085e9eb91a89f097' ;; 		x86) natsArch='386'; sha256='d87bb204228c5e820747e1682dbfb56289e3ddadcfe129b9c9fcf1ad7c0ba053' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 16 Jun 2021 13:43:36 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Wed, 16 Jun 2021 13:43:36 GMT
EXPOSE 4222 8222
# Wed, 16 Jun 2021 13:43:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Jun 2021 13:43:36 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:e160e00eb35d5bc2373770873fbc9c8f5706045b0b06bfd1c364fcf69f02e9fe`  
		Last Modified: Wed, 14 Apr 2021 18:58:36 GMT  
		Size: 2.4 MB (2424145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5db581fac4dfc7d9b487585f9c9ff1ff19f13bb78dc8dd867f6ee6384cb1369`  
		Last Modified: Wed, 16 Jun 2021 13:44:55 GMT  
		Size: 6.5 MB (6542558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b04f15b84ffa9c43ee28a5f4d9f840032b8b96228dcb21f25b093102559d896b`  
		Last Modified: Wed, 16 Jun 2021 13:44:53 GMT  
		Size: 421.0 B  
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
$ docker pull nats-streaming@sha256:a06335f6921f2afb19872d3fa0a852f37390de4a9322b6fe0499f6223f56f595
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
$ docker pull nats-streaming@sha256:8b2d71e9d5ba6e809239f8689f194badfe4604cf66b8663f284ba101268c1057
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.0 MB (8967124 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:313d2bfb32eb974d6db3373750c748020c32ab3d2af5783131fc457c185427a0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Tue, 15 Jun 2021 23:15:15 GMT
ADD file:028c5b473d862250586e174c5dd19b37f8fc3bffbc02d888e72df30f32fd6129 in / 
# Tue, 15 Jun 2021 23:15:16 GMT
CMD ["/bin/sh"]
# Wed, 16 Jun 2021 13:43:31 GMT
ENV NATS_STREAMING_SERVER=0.22.0
# Wed, 16 Jun 2021 13:43:35 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='3ffc4b74f469b97a8ce0edff8b645baf89d9f9f3debdfa7088a0ceac3ed6c37b' ;; 		armhf) natsArch='arm6'; sha256='abe201b1a90cd2e8db39989c81a2c76d3956035745c68d0c7e090fc8c5a138c8' ;; 		armv7) natsArch='arm7'; sha256='d218edd395f980ea91a54624b4cc1fe0220268171ee596a24d7c01c15a7dbb7f' ;; 		x86_64) natsArch='amd64'; sha256='72f5b899167a8866d4b82d1bf9bc14b5d047e6b1ab127dd0085e9eb91a89f097' ;; 		x86) natsArch='386'; sha256='d87bb204228c5e820747e1682dbfb56289e3ddadcfe129b9c9fcf1ad7c0ba053' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 16 Jun 2021 13:43:36 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Wed, 16 Jun 2021 13:43:36 GMT
EXPOSE 4222 8222
# Wed, 16 Jun 2021 13:43:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Jun 2021 13:43:36 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:e160e00eb35d5bc2373770873fbc9c8f5706045b0b06bfd1c364fcf69f02e9fe`  
		Last Modified: Wed, 14 Apr 2021 18:58:36 GMT  
		Size: 2.4 MB (2424145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5db581fac4dfc7d9b487585f9c9ff1ff19f13bb78dc8dd867f6ee6384cb1369`  
		Last Modified: Wed, 16 Jun 2021 13:44:55 GMT  
		Size: 6.5 MB (6542558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b04f15b84ffa9c43ee28a5f4d9f840032b8b96228dcb21f25b093102559d896b`  
		Last Modified: Wed, 16 Jun 2021 13:44:53 GMT  
		Size: 421.0 B  
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
$ docker pull nats-streaming@sha256:afca78bb9fd8e82b1d8dafd00b6e413e795093987abc8b7d198758a95a6bc585
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.2061; amd64

### `nats-streaming:0.22-nanoserver` - windows version 10.0.17763.2061; amd64

```console
$ docker pull nats-streaming@sha256:9d7e58b6bd4fd1ef45339a3497ef7d6a402444f4015ad419d920758ad398c253
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.7 MB (109664361 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ba10fd6c3016a2b0355ec120bdecdcd05c850fb5881ef2436371c86c57688f7`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 06 Jul 2021 20:06:39 GMT
RUN Apply image 1809-amd64
# Wed, 14 Jul 2021 02:35:24 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 14 Jul 2021 18:09:34 GMT
RUN cmd /S /C #(nop) COPY file:72a29a3f2d4a0bd237295ad8b2a317a32c76cbb8a1af898a564024d5013c0475 in C:\nats-streaming-server.exe 
# Wed, 14 Jul 2021 18:09:38 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 14 Jul 2021 18:09:41 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 14 Jul 2021 18:09:44 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:29d43e56445c5279a6386c4dfe4d1ada3c7124ade9cb7b0f2757e58ffc7cd10b`  
		Size: 102.7 MB (102725622 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ec20c4c9f6fa5e782e09342d50033ef24c4049a9dad1befd33c96759b71da6de`  
		Last Modified: Wed, 14 Jul 2021 02:40:36 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c90e8afac4445cb889af58b8a590bdc86382f1e91b54e20bc1009269430e8d7b`  
		Last Modified: Wed, 14 Jul 2021 18:14:47 GMT  
		Size: 6.9 MB (6934158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54dedbbe81a86e2b328335cbf90c2056b3cf884b7bb41a3a2322b58509040298`  
		Last Modified: Wed, 14 Jul 2021 18:14:45 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7b0a78349321bd097f09f3ac8c826322e4c48a945f77e33b86e5699f7477180`  
		Last Modified: Wed, 14 Jul 2021 18:14:45 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c19f14b31cad0b01978407b9da3ddcdd9b2ee36d8a558aa4a30f5bcb62c6ab63`  
		Last Modified: Wed, 14 Jul 2021 18:14:45 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.22-nanoserver-1809`

```console
$ docker pull nats-streaming@sha256:afca78bb9fd8e82b1d8dafd00b6e413e795093987abc8b7d198758a95a6bc585
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.2061; amd64

### `nats-streaming:0.22-nanoserver-1809` - windows version 10.0.17763.2061; amd64

```console
$ docker pull nats-streaming@sha256:9d7e58b6bd4fd1ef45339a3497ef7d6a402444f4015ad419d920758ad398c253
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.7 MB (109664361 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ba10fd6c3016a2b0355ec120bdecdcd05c850fb5881ef2436371c86c57688f7`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 06 Jul 2021 20:06:39 GMT
RUN Apply image 1809-amd64
# Wed, 14 Jul 2021 02:35:24 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 14 Jul 2021 18:09:34 GMT
RUN cmd /S /C #(nop) COPY file:72a29a3f2d4a0bd237295ad8b2a317a32c76cbb8a1af898a564024d5013c0475 in C:\nats-streaming-server.exe 
# Wed, 14 Jul 2021 18:09:38 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 14 Jul 2021 18:09:41 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 14 Jul 2021 18:09:44 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:29d43e56445c5279a6386c4dfe4d1ada3c7124ade9cb7b0f2757e58ffc7cd10b`  
		Size: 102.7 MB (102725622 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ec20c4c9f6fa5e782e09342d50033ef24c4049a9dad1befd33c96759b71da6de`  
		Last Modified: Wed, 14 Jul 2021 02:40:36 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c90e8afac4445cb889af58b8a590bdc86382f1e91b54e20bc1009269430e8d7b`  
		Last Modified: Wed, 14 Jul 2021 18:14:47 GMT  
		Size: 6.9 MB (6934158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54dedbbe81a86e2b328335cbf90c2056b3cf884b7bb41a3a2322b58509040298`  
		Last Modified: Wed, 14 Jul 2021 18:14:45 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7b0a78349321bd097f09f3ac8c826322e4c48a945f77e33b86e5699f7477180`  
		Last Modified: Wed, 14 Jul 2021 18:14:45 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c19f14b31cad0b01978407b9da3ddcdd9b2ee36d8a558aa4a30f5bcb62c6ab63`  
		Last Modified: Wed, 14 Jul 2021 18:14:45 GMT  
		Size: 1.1 KB (1148 bytes)  
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
$ docker pull nats-streaming@sha256:5a47a5386f08c246e61fdb7176fed959a7681b0bfbd0f6c347f0392e893558af
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.2061; amd64
	-	windows version 10.0.14393.4530; amd64

### `nats-streaming:0.22-windowsservercore` - windows version 10.0.17763.2061; amd64

```console
$ docker pull nats-streaming@sha256:63ca349de872bd42e0977f4246444adb1282f44673a2885c242429de92bc276d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2693100521 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:821eefa949e48160cbd78370042a30b599c173e30585c9e0267045dfacee2488`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 06 Jul 2021 20:34:18 GMT
RUN Install update 1809-amd64
# Wed, 14 Jul 2021 01:07:27 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 14 Jul 2021 02:31:26 GMT
ENV NATS_DOCKERIZED=1
# Wed, 14 Jul 2021 18:06:06 GMT
ENV NATS_STREAMING_SERVER=0.22.0
# Wed, 14 Jul 2021 18:06:08 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.22.0/nats-streaming-server-v0.22.0-windows-amd64.zip
# Wed, 14 Jul 2021 18:06:11 GMT
ENV GIT_DOWNLOAD_SHA256=436c16330efbd0767d9a69dcdf2d3badd4e2598fab23c4f4a192e9d9982c2c92
# Wed, 14 Jul 2021 18:07:11 GMT
RUN Set-PSDebug -Trace 2
# Wed, 14 Jul 2021 18:09:11 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 14 Jul 2021 18:09:14 GMT
EXPOSE 4222 8222
# Wed, 14 Jul 2021 18:09:17 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 14 Jul 2021 18:09:20 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f143c6fed32d477c35b660b2e108ea62e3593c03e44bd9ced208ce52b26b0841`  
		Size: 967.1 MB (967113907 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:adcec6ff907307155c0652222cc9b95a0cc964d4c371e02767e72a5c90472192`  
		Last Modified: Wed, 14 Jul 2021 02:02:19 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f92bdc410321db22d4cf09322869bd9fb2495788c3725624c86d76a6ab3d95d3`  
		Last Modified: Wed, 14 Jul 2021 02:40:16 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4057892101207121360a73faf4dca58c8d6a0bae3bddba124324243bf82f8976`  
		Last Modified: Wed, 14 Jul 2021 18:14:26 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22c2bf3f49a28310b6f20865971fa9b74b600f5288d0da41d85cd3edfed06ab2`  
		Last Modified: Wed, 14 Jul 2021 18:14:26 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b8137a5d079643858ba3385400b934f060f91d9073e0b75e153a7d84623821d`  
		Last Modified: Wed, 14 Jul 2021 18:14:26 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8c50c1de08ec39901fd043365aec3d9ef8c0549ea3669064478276cb8511b1d`  
		Last Modified: Wed, 14 Jul 2021 18:14:24 GMT  
		Size: 364.2 KB (364238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce83bc914faa405040d8788b9995ce447002056425d8d66be1702743ca22871d`  
		Last Modified: Wed, 14 Jul 2021 18:14:32 GMT  
		Size: 7.3 MB (7278180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee11b9df16fbb6a30a224f08de9894c2f03c4a67b17593c9c2bff3e8802d2fa7`  
		Last Modified: Wed, 14 Jul 2021 18:14:23 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e330ba2bb253cf3eb60924484591be1b76f1f7bd76bac5bb452ffd8ba7c45b8e`  
		Last Modified: Wed, 14 Jul 2021 18:14:23 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac321f95e98c7918decd7118f16edefb9f477e75e52b0f096760f0e2266f0edf`  
		Last Modified: Wed, 14 Jul 2021 18:14:23 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.22-windowsservercore` - windows version 10.0.14393.4530; amd64

```console
$ docker pull nats-streaming@sha256:3ad8c929da66bbecb80008f907271ef5c487403117c5427ed2a07c8e5cc12902
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6281753287 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:45e6693e2a665263f7b8e9067f54ab7cf94a1a5ed7c4bae189a41b98731ce538`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Fri, 09 Jul 2021 05:02:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 14 Jul 2021 01:14:25 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 14 Jul 2021 02:35:48 GMT
ENV NATS_DOCKERIZED=1
# Wed, 14 Jul 2021 18:09:52 GMT
ENV NATS_STREAMING_SERVER=0.22.0
# Wed, 14 Jul 2021 18:09:55 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.22.0/nats-streaming-server-v0.22.0-windows-amd64.zip
# Wed, 14 Jul 2021 18:09:58 GMT
ENV GIT_DOWNLOAD_SHA256=436c16330efbd0767d9a69dcdf2d3badd4e2598fab23c4f4a192e9d9982c2c92
# Wed, 14 Jul 2021 18:11:28 GMT
RUN Set-PSDebug -Trace 2
# Wed, 14 Jul 2021 18:13:47 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 14 Jul 2021 18:13:50 GMT
EXPOSE 4222 8222
# Wed, 14 Jul 2021 18:13:53 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 14 Jul 2021 18:13:55 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a567de41cc349380b25967f180fb1b6b2431bda61ccaaf69d78a33bc9523614a`  
		Size: 2.2 GB (2199646155 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:fed351b78c876c55ec9c7e75d3b9d1b146c5c5dfeb4b5480c0a7c384322df98c`  
		Last Modified: Wed, 14 Jul 2021 02:03:37 GMT  
		Size: 1.4 KB (1444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf08cae8b8db8f3f89e1a9192d393f2da55b44efce4e778fdb58debe2d608275`  
		Last Modified: Wed, 14 Jul 2021 02:40:57 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2feaa7f132d0998b20ad8e1a39c70f7b203986b1920414980bc697f368765d5b`  
		Last Modified: Wed, 14 Jul 2021 18:15:02 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:963d57a144a26f409de2590ce7dcc4eadc787418255737dc70426d7f9082daf9`  
		Last Modified: Wed, 14 Jul 2021 18:15:02 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8ff055cfb27b499cdaf607d5678758a37a200f18cb17ae5444e3e3fbcdc0674`  
		Last Modified: Wed, 14 Jul 2021 18:15:02 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:500b6d026b69103572ab1cfbdadc92ee006f84be89dd397f135f9bedc593fd73`  
		Last Modified: Wed, 14 Jul 2021 18:14:59 GMT  
		Size: 352.1 KB (352069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40da8c0535202c9b305dae1dc40ebe93909e2bc230eabb255309331807baf465`  
		Last Modified: Wed, 14 Jul 2021 18:15:03 GMT  
		Size: 11.8 MB (11757923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6970a1f8eda65e922ce1b5f0a9bba085a1651d7e327422230c343ba6c1e1a3d0`  
		Last Modified: Wed, 14 Jul 2021 18:14:59 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:424f05177cfed5b98dda36cadc9fbee19cba9421a5166678aa8e318792dd94bb`  
		Last Modified: Wed, 14 Jul 2021 18:14:59 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ea1fe02e0ee3dbbe6543d7020be6c660a206ef6c1dc8041bd4a736b276fa15c`  
		Last Modified: Wed, 14 Jul 2021 18:14:59 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.22-windowsservercore-1809`

```console
$ docker pull nats-streaming@sha256:877c8e5166313ea6fde0584d92b18f50ad4c2d0840f8a03082318e7aafac7aac
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.2061; amd64

### `nats-streaming:0.22-windowsservercore-1809` - windows version 10.0.17763.2061; amd64

```console
$ docker pull nats-streaming@sha256:63ca349de872bd42e0977f4246444adb1282f44673a2885c242429de92bc276d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2693100521 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:821eefa949e48160cbd78370042a30b599c173e30585c9e0267045dfacee2488`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 06 Jul 2021 20:34:18 GMT
RUN Install update 1809-amd64
# Wed, 14 Jul 2021 01:07:27 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 14 Jul 2021 02:31:26 GMT
ENV NATS_DOCKERIZED=1
# Wed, 14 Jul 2021 18:06:06 GMT
ENV NATS_STREAMING_SERVER=0.22.0
# Wed, 14 Jul 2021 18:06:08 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.22.0/nats-streaming-server-v0.22.0-windows-amd64.zip
# Wed, 14 Jul 2021 18:06:11 GMT
ENV GIT_DOWNLOAD_SHA256=436c16330efbd0767d9a69dcdf2d3badd4e2598fab23c4f4a192e9d9982c2c92
# Wed, 14 Jul 2021 18:07:11 GMT
RUN Set-PSDebug -Trace 2
# Wed, 14 Jul 2021 18:09:11 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 14 Jul 2021 18:09:14 GMT
EXPOSE 4222 8222
# Wed, 14 Jul 2021 18:09:17 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 14 Jul 2021 18:09:20 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f143c6fed32d477c35b660b2e108ea62e3593c03e44bd9ced208ce52b26b0841`  
		Size: 967.1 MB (967113907 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:adcec6ff907307155c0652222cc9b95a0cc964d4c371e02767e72a5c90472192`  
		Last Modified: Wed, 14 Jul 2021 02:02:19 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f92bdc410321db22d4cf09322869bd9fb2495788c3725624c86d76a6ab3d95d3`  
		Last Modified: Wed, 14 Jul 2021 02:40:16 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4057892101207121360a73faf4dca58c8d6a0bae3bddba124324243bf82f8976`  
		Last Modified: Wed, 14 Jul 2021 18:14:26 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22c2bf3f49a28310b6f20865971fa9b74b600f5288d0da41d85cd3edfed06ab2`  
		Last Modified: Wed, 14 Jul 2021 18:14:26 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b8137a5d079643858ba3385400b934f060f91d9073e0b75e153a7d84623821d`  
		Last Modified: Wed, 14 Jul 2021 18:14:26 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8c50c1de08ec39901fd043365aec3d9ef8c0549ea3669064478276cb8511b1d`  
		Last Modified: Wed, 14 Jul 2021 18:14:24 GMT  
		Size: 364.2 KB (364238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce83bc914faa405040d8788b9995ce447002056425d8d66be1702743ca22871d`  
		Last Modified: Wed, 14 Jul 2021 18:14:32 GMT  
		Size: 7.3 MB (7278180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee11b9df16fbb6a30a224f08de9894c2f03c4a67b17593c9c2bff3e8802d2fa7`  
		Last Modified: Wed, 14 Jul 2021 18:14:23 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e330ba2bb253cf3eb60924484591be1b76f1f7bd76bac5bb452ffd8ba7c45b8e`  
		Last Modified: Wed, 14 Jul 2021 18:14:23 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac321f95e98c7918decd7118f16edefb9f477e75e52b0f096760f0e2266f0edf`  
		Last Modified: Wed, 14 Jul 2021 18:14:23 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.22-windowsservercore-ltsc2016`

```console
$ docker pull nats-streaming@sha256:9c0cb24674c9c3e1f330cb6e104e1be4355694715cde356dfb21732a03fd84af
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4530; amd64

### `nats-streaming:0.22-windowsservercore-ltsc2016` - windows version 10.0.14393.4530; amd64

```console
$ docker pull nats-streaming@sha256:3ad8c929da66bbecb80008f907271ef5c487403117c5427ed2a07c8e5cc12902
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6281753287 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:45e6693e2a665263f7b8e9067f54ab7cf94a1a5ed7c4bae189a41b98731ce538`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Fri, 09 Jul 2021 05:02:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 14 Jul 2021 01:14:25 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 14 Jul 2021 02:35:48 GMT
ENV NATS_DOCKERIZED=1
# Wed, 14 Jul 2021 18:09:52 GMT
ENV NATS_STREAMING_SERVER=0.22.0
# Wed, 14 Jul 2021 18:09:55 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.22.0/nats-streaming-server-v0.22.0-windows-amd64.zip
# Wed, 14 Jul 2021 18:09:58 GMT
ENV GIT_DOWNLOAD_SHA256=436c16330efbd0767d9a69dcdf2d3badd4e2598fab23c4f4a192e9d9982c2c92
# Wed, 14 Jul 2021 18:11:28 GMT
RUN Set-PSDebug -Trace 2
# Wed, 14 Jul 2021 18:13:47 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 14 Jul 2021 18:13:50 GMT
EXPOSE 4222 8222
# Wed, 14 Jul 2021 18:13:53 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 14 Jul 2021 18:13:55 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a567de41cc349380b25967f180fb1b6b2431bda61ccaaf69d78a33bc9523614a`  
		Size: 2.2 GB (2199646155 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:fed351b78c876c55ec9c7e75d3b9d1b146c5c5dfeb4b5480c0a7c384322df98c`  
		Last Modified: Wed, 14 Jul 2021 02:03:37 GMT  
		Size: 1.4 KB (1444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf08cae8b8db8f3f89e1a9192d393f2da55b44efce4e778fdb58debe2d608275`  
		Last Modified: Wed, 14 Jul 2021 02:40:57 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2feaa7f132d0998b20ad8e1a39c70f7b203986b1920414980bc697f368765d5b`  
		Last Modified: Wed, 14 Jul 2021 18:15:02 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:963d57a144a26f409de2590ce7dcc4eadc787418255737dc70426d7f9082daf9`  
		Last Modified: Wed, 14 Jul 2021 18:15:02 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8ff055cfb27b499cdaf607d5678758a37a200f18cb17ae5444e3e3fbcdc0674`  
		Last Modified: Wed, 14 Jul 2021 18:15:02 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:500b6d026b69103572ab1cfbdadc92ee006f84be89dd397f135f9bedc593fd73`  
		Last Modified: Wed, 14 Jul 2021 18:14:59 GMT  
		Size: 352.1 KB (352069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40da8c0535202c9b305dae1dc40ebe93909e2bc230eabb255309331807baf465`  
		Last Modified: Wed, 14 Jul 2021 18:15:03 GMT  
		Size: 11.8 MB (11757923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6970a1f8eda65e922ce1b5f0a9bba085a1651d7e327422230c343ba6c1e1a3d0`  
		Last Modified: Wed, 14 Jul 2021 18:14:59 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:424f05177cfed5b98dda36cadc9fbee19cba9421a5166678aa8e318792dd94bb`  
		Last Modified: Wed, 14 Jul 2021 18:14:59 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ea1fe02e0ee3dbbe6543d7020be6c660a206ef6c1dc8041bd4a736b276fa15c`  
		Last Modified: Wed, 14 Jul 2021 18:14:59 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.22.0`

```console
$ docker pull nats-streaming@sha256:edf770c6014121e4ea3aac9d7493a33db0256a2e4424a8463446e6649919dbee
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.2061; amd64

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

### `nats-streaming:0.22.0` - windows version 10.0.17763.2061; amd64

```console
$ docker pull nats-streaming@sha256:9d7e58b6bd4fd1ef45339a3497ef7d6a402444f4015ad419d920758ad398c253
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.7 MB (109664361 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ba10fd6c3016a2b0355ec120bdecdcd05c850fb5881ef2436371c86c57688f7`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 06 Jul 2021 20:06:39 GMT
RUN Apply image 1809-amd64
# Wed, 14 Jul 2021 02:35:24 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 14 Jul 2021 18:09:34 GMT
RUN cmd /S /C #(nop) COPY file:72a29a3f2d4a0bd237295ad8b2a317a32c76cbb8a1af898a564024d5013c0475 in C:\nats-streaming-server.exe 
# Wed, 14 Jul 2021 18:09:38 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 14 Jul 2021 18:09:41 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 14 Jul 2021 18:09:44 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:29d43e56445c5279a6386c4dfe4d1ada3c7124ade9cb7b0f2757e58ffc7cd10b`  
		Size: 102.7 MB (102725622 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ec20c4c9f6fa5e782e09342d50033ef24c4049a9dad1befd33c96759b71da6de`  
		Last Modified: Wed, 14 Jul 2021 02:40:36 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c90e8afac4445cb889af58b8a590bdc86382f1e91b54e20bc1009269430e8d7b`  
		Last Modified: Wed, 14 Jul 2021 18:14:47 GMT  
		Size: 6.9 MB (6934158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54dedbbe81a86e2b328335cbf90c2056b3cf884b7bb41a3a2322b58509040298`  
		Last Modified: Wed, 14 Jul 2021 18:14:45 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7b0a78349321bd097f09f3ac8c826322e4c48a945f77e33b86e5699f7477180`  
		Last Modified: Wed, 14 Jul 2021 18:14:45 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c19f14b31cad0b01978407b9da3ddcdd9b2ee36d8a558aa4a30f5bcb62c6ab63`  
		Last Modified: Wed, 14 Jul 2021 18:14:45 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.22.0-alpine`

```console
$ docker pull nats-streaming@sha256:a06335f6921f2afb19872d3fa0a852f37390de4a9322b6fe0499f6223f56f595
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
$ docker pull nats-streaming@sha256:8b2d71e9d5ba6e809239f8689f194badfe4604cf66b8663f284ba101268c1057
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.0 MB (8967124 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:313d2bfb32eb974d6db3373750c748020c32ab3d2af5783131fc457c185427a0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Tue, 15 Jun 2021 23:15:15 GMT
ADD file:028c5b473d862250586e174c5dd19b37f8fc3bffbc02d888e72df30f32fd6129 in / 
# Tue, 15 Jun 2021 23:15:16 GMT
CMD ["/bin/sh"]
# Wed, 16 Jun 2021 13:43:31 GMT
ENV NATS_STREAMING_SERVER=0.22.0
# Wed, 16 Jun 2021 13:43:35 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='3ffc4b74f469b97a8ce0edff8b645baf89d9f9f3debdfa7088a0ceac3ed6c37b' ;; 		armhf) natsArch='arm6'; sha256='abe201b1a90cd2e8db39989c81a2c76d3956035745c68d0c7e090fc8c5a138c8' ;; 		armv7) natsArch='arm7'; sha256='d218edd395f980ea91a54624b4cc1fe0220268171ee596a24d7c01c15a7dbb7f' ;; 		x86_64) natsArch='amd64'; sha256='72f5b899167a8866d4b82d1bf9bc14b5d047e6b1ab127dd0085e9eb91a89f097' ;; 		x86) natsArch='386'; sha256='d87bb204228c5e820747e1682dbfb56289e3ddadcfe129b9c9fcf1ad7c0ba053' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 16 Jun 2021 13:43:36 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Wed, 16 Jun 2021 13:43:36 GMT
EXPOSE 4222 8222
# Wed, 16 Jun 2021 13:43:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Jun 2021 13:43:36 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:e160e00eb35d5bc2373770873fbc9c8f5706045b0b06bfd1c364fcf69f02e9fe`  
		Last Modified: Wed, 14 Apr 2021 18:58:36 GMT  
		Size: 2.4 MB (2424145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5db581fac4dfc7d9b487585f9c9ff1ff19f13bb78dc8dd867f6ee6384cb1369`  
		Last Modified: Wed, 16 Jun 2021 13:44:55 GMT  
		Size: 6.5 MB (6542558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b04f15b84ffa9c43ee28a5f4d9f840032b8b96228dcb21f25b093102559d896b`  
		Last Modified: Wed, 16 Jun 2021 13:44:53 GMT  
		Size: 421.0 B  
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
$ docker pull nats-streaming@sha256:a06335f6921f2afb19872d3fa0a852f37390de4a9322b6fe0499f6223f56f595
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
$ docker pull nats-streaming@sha256:8b2d71e9d5ba6e809239f8689f194badfe4604cf66b8663f284ba101268c1057
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.0 MB (8967124 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:313d2bfb32eb974d6db3373750c748020c32ab3d2af5783131fc457c185427a0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Tue, 15 Jun 2021 23:15:15 GMT
ADD file:028c5b473d862250586e174c5dd19b37f8fc3bffbc02d888e72df30f32fd6129 in / 
# Tue, 15 Jun 2021 23:15:16 GMT
CMD ["/bin/sh"]
# Wed, 16 Jun 2021 13:43:31 GMT
ENV NATS_STREAMING_SERVER=0.22.0
# Wed, 16 Jun 2021 13:43:35 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='3ffc4b74f469b97a8ce0edff8b645baf89d9f9f3debdfa7088a0ceac3ed6c37b' ;; 		armhf) natsArch='arm6'; sha256='abe201b1a90cd2e8db39989c81a2c76d3956035745c68d0c7e090fc8c5a138c8' ;; 		armv7) natsArch='arm7'; sha256='d218edd395f980ea91a54624b4cc1fe0220268171ee596a24d7c01c15a7dbb7f' ;; 		x86_64) natsArch='amd64'; sha256='72f5b899167a8866d4b82d1bf9bc14b5d047e6b1ab127dd0085e9eb91a89f097' ;; 		x86) natsArch='386'; sha256='d87bb204228c5e820747e1682dbfb56289e3ddadcfe129b9c9fcf1ad7c0ba053' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 16 Jun 2021 13:43:36 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Wed, 16 Jun 2021 13:43:36 GMT
EXPOSE 4222 8222
# Wed, 16 Jun 2021 13:43:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Jun 2021 13:43:36 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:e160e00eb35d5bc2373770873fbc9c8f5706045b0b06bfd1c364fcf69f02e9fe`  
		Last Modified: Wed, 14 Apr 2021 18:58:36 GMT  
		Size: 2.4 MB (2424145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5db581fac4dfc7d9b487585f9c9ff1ff19f13bb78dc8dd867f6ee6384cb1369`  
		Last Modified: Wed, 16 Jun 2021 13:44:55 GMT  
		Size: 6.5 MB (6542558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b04f15b84ffa9c43ee28a5f4d9f840032b8b96228dcb21f25b093102559d896b`  
		Last Modified: Wed, 16 Jun 2021 13:44:53 GMT  
		Size: 421.0 B  
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
$ docker pull nats-streaming@sha256:afca78bb9fd8e82b1d8dafd00b6e413e795093987abc8b7d198758a95a6bc585
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.2061; amd64

### `nats-streaming:0.22.0-nanoserver` - windows version 10.0.17763.2061; amd64

```console
$ docker pull nats-streaming@sha256:9d7e58b6bd4fd1ef45339a3497ef7d6a402444f4015ad419d920758ad398c253
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.7 MB (109664361 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ba10fd6c3016a2b0355ec120bdecdcd05c850fb5881ef2436371c86c57688f7`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 06 Jul 2021 20:06:39 GMT
RUN Apply image 1809-amd64
# Wed, 14 Jul 2021 02:35:24 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 14 Jul 2021 18:09:34 GMT
RUN cmd /S /C #(nop) COPY file:72a29a3f2d4a0bd237295ad8b2a317a32c76cbb8a1af898a564024d5013c0475 in C:\nats-streaming-server.exe 
# Wed, 14 Jul 2021 18:09:38 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 14 Jul 2021 18:09:41 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 14 Jul 2021 18:09:44 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:29d43e56445c5279a6386c4dfe4d1ada3c7124ade9cb7b0f2757e58ffc7cd10b`  
		Size: 102.7 MB (102725622 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ec20c4c9f6fa5e782e09342d50033ef24c4049a9dad1befd33c96759b71da6de`  
		Last Modified: Wed, 14 Jul 2021 02:40:36 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c90e8afac4445cb889af58b8a590bdc86382f1e91b54e20bc1009269430e8d7b`  
		Last Modified: Wed, 14 Jul 2021 18:14:47 GMT  
		Size: 6.9 MB (6934158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54dedbbe81a86e2b328335cbf90c2056b3cf884b7bb41a3a2322b58509040298`  
		Last Modified: Wed, 14 Jul 2021 18:14:45 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7b0a78349321bd097f09f3ac8c826322e4c48a945f77e33b86e5699f7477180`  
		Last Modified: Wed, 14 Jul 2021 18:14:45 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c19f14b31cad0b01978407b9da3ddcdd9b2ee36d8a558aa4a30f5bcb62c6ab63`  
		Last Modified: Wed, 14 Jul 2021 18:14:45 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.22.0-nanoserver-1809`

```console
$ docker pull nats-streaming@sha256:afca78bb9fd8e82b1d8dafd00b6e413e795093987abc8b7d198758a95a6bc585
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.2061; amd64

### `nats-streaming:0.22.0-nanoserver-1809` - windows version 10.0.17763.2061; amd64

```console
$ docker pull nats-streaming@sha256:9d7e58b6bd4fd1ef45339a3497ef7d6a402444f4015ad419d920758ad398c253
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.7 MB (109664361 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ba10fd6c3016a2b0355ec120bdecdcd05c850fb5881ef2436371c86c57688f7`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 06 Jul 2021 20:06:39 GMT
RUN Apply image 1809-amd64
# Wed, 14 Jul 2021 02:35:24 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 14 Jul 2021 18:09:34 GMT
RUN cmd /S /C #(nop) COPY file:72a29a3f2d4a0bd237295ad8b2a317a32c76cbb8a1af898a564024d5013c0475 in C:\nats-streaming-server.exe 
# Wed, 14 Jul 2021 18:09:38 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 14 Jul 2021 18:09:41 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 14 Jul 2021 18:09:44 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:29d43e56445c5279a6386c4dfe4d1ada3c7124ade9cb7b0f2757e58ffc7cd10b`  
		Size: 102.7 MB (102725622 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ec20c4c9f6fa5e782e09342d50033ef24c4049a9dad1befd33c96759b71da6de`  
		Last Modified: Wed, 14 Jul 2021 02:40:36 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c90e8afac4445cb889af58b8a590bdc86382f1e91b54e20bc1009269430e8d7b`  
		Last Modified: Wed, 14 Jul 2021 18:14:47 GMT  
		Size: 6.9 MB (6934158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54dedbbe81a86e2b328335cbf90c2056b3cf884b7bb41a3a2322b58509040298`  
		Last Modified: Wed, 14 Jul 2021 18:14:45 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7b0a78349321bd097f09f3ac8c826322e4c48a945f77e33b86e5699f7477180`  
		Last Modified: Wed, 14 Jul 2021 18:14:45 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c19f14b31cad0b01978407b9da3ddcdd9b2ee36d8a558aa4a30f5bcb62c6ab63`  
		Last Modified: Wed, 14 Jul 2021 18:14:45 GMT  
		Size: 1.1 KB (1148 bytes)  
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
$ docker pull nats-streaming@sha256:5a47a5386f08c246e61fdb7176fed959a7681b0bfbd0f6c347f0392e893558af
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.2061; amd64
	-	windows version 10.0.14393.4530; amd64

### `nats-streaming:0.22.0-windowsservercore` - windows version 10.0.17763.2061; amd64

```console
$ docker pull nats-streaming@sha256:63ca349de872bd42e0977f4246444adb1282f44673a2885c242429de92bc276d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2693100521 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:821eefa949e48160cbd78370042a30b599c173e30585c9e0267045dfacee2488`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 06 Jul 2021 20:34:18 GMT
RUN Install update 1809-amd64
# Wed, 14 Jul 2021 01:07:27 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 14 Jul 2021 02:31:26 GMT
ENV NATS_DOCKERIZED=1
# Wed, 14 Jul 2021 18:06:06 GMT
ENV NATS_STREAMING_SERVER=0.22.0
# Wed, 14 Jul 2021 18:06:08 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.22.0/nats-streaming-server-v0.22.0-windows-amd64.zip
# Wed, 14 Jul 2021 18:06:11 GMT
ENV GIT_DOWNLOAD_SHA256=436c16330efbd0767d9a69dcdf2d3badd4e2598fab23c4f4a192e9d9982c2c92
# Wed, 14 Jul 2021 18:07:11 GMT
RUN Set-PSDebug -Trace 2
# Wed, 14 Jul 2021 18:09:11 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 14 Jul 2021 18:09:14 GMT
EXPOSE 4222 8222
# Wed, 14 Jul 2021 18:09:17 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 14 Jul 2021 18:09:20 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f143c6fed32d477c35b660b2e108ea62e3593c03e44bd9ced208ce52b26b0841`  
		Size: 967.1 MB (967113907 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:adcec6ff907307155c0652222cc9b95a0cc964d4c371e02767e72a5c90472192`  
		Last Modified: Wed, 14 Jul 2021 02:02:19 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f92bdc410321db22d4cf09322869bd9fb2495788c3725624c86d76a6ab3d95d3`  
		Last Modified: Wed, 14 Jul 2021 02:40:16 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4057892101207121360a73faf4dca58c8d6a0bae3bddba124324243bf82f8976`  
		Last Modified: Wed, 14 Jul 2021 18:14:26 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22c2bf3f49a28310b6f20865971fa9b74b600f5288d0da41d85cd3edfed06ab2`  
		Last Modified: Wed, 14 Jul 2021 18:14:26 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b8137a5d079643858ba3385400b934f060f91d9073e0b75e153a7d84623821d`  
		Last Modified: Wed, 14 Jul 2021 18:14:26 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8c50c1de08ec39901fd043365aec3d9ef8c0549ea3669064478276cb8511b1d`  
		Last Modified: Wed, 14 Jul 2021 18:14:24 GMT  
		Size: 364.2 KB (364238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce83bc914faa405040d8788b9995ce447002056425d8d66be1702743ca22871d`  
		Last Modified: Wed, 14 Jul 2021 18:14:32 GMT  
		Size: 7.3 MB (7278180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee11b9df16fbb6a30a224f08de9894c2f03c4a67b17593c9c2bff3e8802d2fa7`  
		Last Modified: Wed, 14 Jul 2021 18:14:23 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e330ba2bb253cf3eb60924484591be1b76f1f7bd76bac5bb452ffd8ba7c45b8e`  
		Last Modified: Wed, 14 Jul 2021 18:14:23 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac321f95e98c7918decd7118f16edefb9f477e75e52b0f096760f0e2266f0edf`  
		Last Modified: Wed, 14 Jul 2021 18:14:23 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.22.0-windowsservercore` - windows version 10.0.14393.4530; amd64

```console
$ docker pull nats-streaming@sha256:3ad8c929da66bbecb80008f907271ef5c487403117c5427ed2a07c8e5cc12902
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6281753287 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:45e6693e2a665263f7b8e9067f54ab7cf94a1a5ed7c4bae189a41b98731ce538`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Fri, 09 Jul 2021 05:02:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 14 Jul 2021 01:14:25 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 14 Jul 2021 02:35:48 GMT
ENV NATS_DOCKERIZED=1
# Wed, 14 Jul 2021 18:09:52 GMT
ENV NATS_STREAMING_SERVER=0.22.0
# Wed, 14 Jul 2021 18:09:55 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.22.0/nats-streaming-server-v0.22.0-windows-amd64.zip
# Wed, 14 Jul 2021 18:09:58 GMT
ENV GIT_DOWNLOAD_SHA256=436c16330efbd0767d9a69dcdf2d3badd4e2598fab23c4f4a192e9d9982c2c92
# Wed, 14 Jul 2021 18:11:28 GMT
RUN Set-PSDebug -Trace 2
# Wed, 14 Jul 2021 18:13:47 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 14 Jul 2021 18:13:50 GMT
EXPOSE 4222 8222
# Wed, 14 Jul 2021 18:13:53 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 14 Jul 2021 18:13:55 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a567de41cc349380b25967f180fb1b6b2431bda61ccaaf69d78a33bc9523614a`  
		Size: 2.2 GB (2199646155 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:fed351b78c876c55ec9c7e75d3b9d1b146c5c5dfeb4b5480c0a7c384322df98c`  
		Last Modified: Wed, 14 Jul 2021 02:03:37 GMT  
		Size: 1.4 KB (1444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf08cae8b8db8f3f89e1a9192d393f2da55b44efce4e778fdb58debe2d608275`  
		Last Modified: Wed, 14 Jul 2021 02:40:57 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2feaa7f132d0998b20ad8e1a39c70f7b203986b1920414980bc697f368765d5b`  
		Last Modified: Wed, 14 Jul 2021 18:15:02 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:963d57a144a26f409de2590ce7dcc4eadc787418255737dc70426d7f9082daf9`  
		Last Modified: Wed, 14 Jul 2021 18:15:02 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8ff055cfb27b499cdaf607d5678758a37a200f18cb17ae5444e3e3fbcdc0674`  
		Last Modified: Wed, 14 Jul 2021 18:15:02 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:500b6d026b69103572ab1cfbdadc92ee006f84be89dd397f135f9bedc593fd73`  
		Last Modified: Wed, 14 Jul 2021 18:14:59 GMT  
		Size: 352.1 KB (352069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40da8c0535202c9b305dae1dc40ebe93909e2bc230eabb255309331807baf465`  
		Last Modified: Wed, 14 Jul 2021 18:15:03 GMT  
		Size: 11.8 MB (11757923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6970a1f8eda65e922ce1b5f0a9bba085a1651d7e327422230c343ba6c1e1a3d0`  
		Last Modified: Wed, 14 Jul 2021 18:14:59 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:424f05177cfed5b98dda36cadc9fbee19cba9421a5166678aa8e318792dd94bb`  
		Last Modified: Wed, 14 Jul 2021 18:14:59 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ea1fe02e0ee3dbbe6543d7020be6c660a206ef6c1dc8041bd4a736b276fa15c`  
		Last Modified: Wed, 14 Jul 2021 18:14:59 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.22.0-windowsservercore-1809`

```console
$ docker pull nats-streaming@sha256:877c8e5166313ea6fde0584d92b18f50ad4c2d0840f8a03082318e7aafac7aac
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.2061; amd64

### `nats-streaming:0.22.0-windowsservercore-1809` - windows version 10.0.17763.2061; amd64

```console
$ docker pull nats-streaming@sha256:63ca349de872bd42e0977f4246444adb1282f44673a2885c242429de92bc276d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2693100521 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:821eefa949e48160cbd78370042a30b599c173e30585c9e0267045dfacee2488`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 06 Jul 2021 20:34:18 GMT
RUN Install update 1809-amd64
# Wed, 14 Jul 2021 01:07:27 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 14 Jul 2021 02:31:26 GMT
ENV NATS_DOCKERIZED=1
# Wed, 14 Jul 2021 18:06:06 GMT
ENV NATS_STREAMING_SERVER=0.22.0
# Wed, 14 Jul 2021 18:06:08 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.22.0/nats-streaming-server-v0.22.0-windows-amd64.zip
# Wed, 14 Jul 2021 18:06:11 GMT
ENV GIT_DOWNLOAD_SHA256=436c16330efbd0767d9a69dcdf2d3badd4e2598fab23c4f4a192e9d9982c2c92
# Wed, 14 Jul 2021 18:07:11 GMT
RUN Set-PSDebug -Trace 2
# Wed, 14 Jul 2021 18:09:11 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 14 Jul 2021 18:09:14 GMT
EXPOSE 4222 8222
# Wed, 14 Jul 2021 18:09:17 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 14 Jul 2021 18:09:20 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f143c6fed32d477c35b660b2e108ea62e3593c03e44bd9ced208ce52b26b0841`  
		Size: 967.1 MB (967113907 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:adcec6ff907307155c0652222cc9b95a0cc964d4c371e02767e72a5c90472192`  
		Last Modified: Wed, 14 Jul 2021 02:02:19 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f92bdc410321db22d4cf09322869bd9fb2495788c3725624c86d76a6ab3d95d3`  
		Last Modified: Wed, 14 Jul 2021 02:40:16 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4057892101207121360a73faf4dca58c8d6a0bae3bddba124324243bf82f8976`  
		Last Modified: Wed, 14 Jul 2021 18:14:26 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22c2bf3f49a28310b6f20865971fa9b74b600f5288d0da41d85cd3edfed06ab2`  
		Last Modified: Wed, 14 Jul 2021 18:14:26 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b8137a5d079643858ba3385400b934f060f91d9073e0b75e153a7d84623821d`  
		Last Modified: Wed, 14 Jul 2021 18:14:26 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8c50c1de08ec39901fd043365aec3d9ef8c0549ea3669064478276cb8511b1d`  
		Last Modified: Wed, 14 Jul 2021 18:14:24 GMT  
		Size: 364.2 KB (364238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce83bc914faa405040d8788b9995ce447002056425d8d66be1702743ca22871d`  
		Last Modified: Wed, 14 Jul 2021 18:14:32 GMT  
		Size: 7.3 MB (7278180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee11b9df16fbb6a30a224f08de9894c2f03c4a67b17593c9c2bff3e8802d2fa7`  
		Last Modified: Wed, 14 Jul 2021 18:14:23 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e330ba2bb253cf3eb60924484591be1b76f1f7bd76bac5bb452ffd8ba7c45b8e`  
		Last Modified: Wed, 14 Jul 2021 18:14:23 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac321f95e98c7918decd7118f16edefb9f477e75e52b0f096760f0e2266f0edf`  
		Last Modified: Wed, 14 Jul 2021 18:14:23 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.22.0-windowsservercore-ltsc2016`

```console
$ docker pull nats-streaming@sha256:9c0cb24674c9c3e1f330cb6e104e1be4355694715cde356dfb21732a03fd84af
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4530; amd64

### `nats-streaming:0.22.0-windowsservercore-ltsc2016` - windows version 10.0.14393.4530; amd64

```console
$ docker pull nats-streaming@sha256:3ad8c929da66bbecb80008f907271ef5c487403117c5427ed2a07c8e5cc12902
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6281753287 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:45e6693e2a665263f7b8e9067f54ab7cf94a1a5ed7c4bae189a41b98731ce538`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Fri, 09 Jul 2021 05:02:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 14 Jul 2021 01:14:25 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 14 Jul 2021 02:35:48 GMT
ENV NATS_DOCKERIZED=1
# Wed, 14 Jul 2021 18:09:52 GMT
ENV NATS_STREAMING_SERVER=0.22.0
# Wed, 14 Jul 2021 18:09:55 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.22.0/nats-streaming-server-v0.22.0-windows-amd64.zip
# Wed, 14 Jul 2021 18:09:58 GMT
ENV GIT_DOWNLOAD_SHA256=436c16330efbd0767d9a69dcdf2d3badd4e2598fab23c4f4a192e9d9982c2c92
# Wed, 14 Jul 2021 18:11:28 GMT
RUN Set-PSDebug -Trace 2
# Wed, 14 Jul 2021 18:13:47 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 14 Jul 2021 18:13:50 GMT
EXPOSE 4222 8222
# Wed, 14 Jul 2021 18:13:53 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 14 Jul 2021 18:13:55 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a567de41cc349380b25967f180fb1b6b2431bda61ccaaf69d78a33bc9523614a`  
		Size: 2.2 GB (2199646155 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:fed351b78c876c55ec9c7e75d3b9d1b146c5c5dfeb4b5480c0a7c384322df98c`  
		Last Modified: Wed, 14 Jul 2021 02:03:37 GMT  
		Size: 1.4 KB (1444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf08cae8b8db8f3f89e1a9192d393f2da55b44efce4e778fdb58debe2d608275`  
		Last Modified: Wed, 14 Jul 2021 02:40:57 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2feaa7f132d0998b20ad8e1a39c70f7b203986b1920414980bc697f368765d5b`  
		Last Modified: Wed, 14 Jul 2021 18:15:02 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:963d57a144a26f409de2590ce7dcc4eadc787418255737dc70426d7f9082daf9`  
		Last Modified: Wed, 14 Jul 2021 18:15:02 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8ff055cfb27b499cdaf607d5678758a37a200f18cb17ae5444e3e3fbcdc0674`  
		Last Modified: Wed, 14 Jul 2021 18:15:02 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:500b6d026b69103572ab1cfbdadc92ee006f84be89dd397f135f9bedc593fd73`  
		Last Modified: Wed, 14 Jul 2021 18:14:59 GMT  
		Size: 352.1 KB (352069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40da8c0535202c9b305dae1dc40ebe93909e2bc230eabb255309331807baf465`  
		Last Modified: Wed, 14 Jul 2021 18:15:03 GMT  
		Size: 11.8 MB (11757923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6970a1f8eda65e922ce1b5f0a9bba085a1651d7e327422230c343ba6c1e1a3d0`  
		Last Modified: Wed, 14 Jul 2021 18:14:59 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:424f05177cfed5b98dda36cadc9fbee19cba9421a5166678aa8e318792dd94bb`  
		Last Modified: Wed, 14 Jul 2021 18:14:59 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ea1fe02e0ee3dbbe6543d7020be6c660a206ef6c1dc8041bd4a736b276fa15c`  
		Last Modified: Wed, 14 Jul 2021 18:14:59 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:alpine`

```console
$ docker pull nats-streaming@sha256:a06335f6921f2afb19872d3fa0a852f37390de4a9322b6fe0499f6223f56f595
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
$ docker pull nats-streaming@sha256:8b2d71e9d5ba6e809239f8689f194badfe4604cf66b8663f284ba101268c1057
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.0 MB (8967124 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:313d2bfb32eb974d6db3373750c748020c32ab3d2af5783131fc457c185427a0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Tue, 15 Jun 2021 23:15:15 GMT
ADD file:028c5b473d862250586e174c5dd19b37f8fc3bffbc02d888e72df30f32fd6129 in / 
# Tue, 15 Jun 2021 23:15:16 GMT
CMD ["/bin/sh"]
# Wed, 16 Jun 2021 13:43:31 GMT
ENV NATS_STREAMING_SERVER=0.22.0
# Wed, 16 Jun 2021 13:43:35 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='3ffc4b74f469b97a8ce0edff8b645baf89d9f9f3debdfa7088a0ceac3ed6c37b' ;; 		armhf) natsArch='arm6'; sha256='abe201b1a90cd2e8db39989c81a2c76d3956035745c68d0c7e090fc8c5a138c8' ;; 		armv7) natsArch='arm7'; sha256='d218edd395f980ea91a54624b4cc1fe0220268171ee596a24d7c01c15a7dbb7f' ;; 		x86_64) natsArch='amd64'; sha256='72f5b899167a8866d4b82d1bf9bc14b5d047e6b1ab127dd0085e9eb91a89f097' ;; 		x86) natsArch='386'; sha256='d87bb204228c5e820747e1682dbfb56289e3ddadcfe129b9c9fcf1ad7c0ba053' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 16 Jun 2021 13:43:36 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Wed, 16 Jun 2021 13:43:36 GMT
EXPOSE 4222 8222
# Wed, 16 Jun 2021 13:43:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Jun 2021 13:43:36 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:e160e00eb35d5bc2373770873fbc9c8f5706045b0b06bfd1c364fcf69f02e9fe`  
		Last Modified: Wed, 14 Apr 2021 18:58:36 GMT  
		Size: 2.4 MB (2424145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5db581fac4dfc7d9b487585f9c9ff1ff19f13bb78dc8dd867f6ee6384cb1369`  
		Last Modified: Wed, 16 Jun 2021 13:44:55 GMT  
		Size: 6.5 MB (6542558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b04f15b84ffa9c43ee28a5f4d9f840032b8b96228dcb21f25b093102559d896b`  
		Last Modified: Wed, 16 Jun 2021 13:44:53 GMT  
		Size: 421.0 B  
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
$ docker pull nats-streaming@sha256:a06335f6921f2afb19872d3fa0a852f37390de4a9322b6fe0499f6223f56f595
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
$ docker pull nats-streaming@sha256:8b2d71e9d5ba6e809239f8689f194badfe4604cf66b8663f284ba101268c1057
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.0 MB (8967124 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:313d2bfb32eb974d6db3373750c748020c32ab3d2af5783131fc457c185427a0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Tue, 15 Jun 2021 23:15:15 GMT
ADD file:028c5b473d862250586e174c5dd19b37f8fc3bffbc02d888e72df30f32fd6129 in / 
# Tue, 15 Jun 2021 23:15:16 GMT
CMD ["/bin/sh"]
# Wed, 16 Jun 2021 13:43:31 GMT
ENV NATS_STREAMING_SERVER=0.22.0
# Wed, 16 Jun 2021 13:43:35 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='3ffc4b74f469b97a8ce0edff8b645baf89d9f9f3debdfa7088a0ceac3ed6c37b' ;; 		armhf) natsArch='arm6'; sha256='abe201b1a90cd2e8db39989c81a2c76d3956035745c68d0c7e090fc8c5a138c8' ;; 		armv7) natsArch='arm7'; sha256='d218edd395f980ea91a54624b4cc1fe0220268171ee596a24d7c01c15a7dbb7f' ;; 		x86_64) natsArch='amd64'; sha256='72f5b899167a8866d4b82d1bf9bc14b5d047e6b1ab127dd0085e9eb91a89f097' ;; 		x86) natsArch='386'; sha256='d87bb204228c5e820747e1682dbfb56289e3ddadcfe129b9c9fcf1ad7c0ba053' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 16 Jun 2021 13:43:36 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Wed, 16 Jun 2021 13:43:36 GMT
EXPOSE 4222 8222
# Wed, 16 Jun 2021 13:43:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Jun 2021 13:43:36 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:e160e00eb35d5bc2373770873fbc9c8f5706045b0b06bfd1c364fcf69f02e9fe`  
		Last Modified: Wed, 14 Apr 2021 18:58:36 GMT  
		Size: 2.4 MB (2424145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5db581fac4dfc7d9b487585f9c9ff1ff19f13bb78dc8dd867f6ee6384cb1369`  
		Last Modified: Wed, 16 Jun 2021 13:44:55 GMT  
		Size: 6.5 MB (6542558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b04f15b84ffa9c43ee28a5f4d9f840032b8b96228dcb21f25b093102559d896b`  
		Last Modified: Wed, 16 Jun 2021 13:44:53 GMT  
		Size: 421.0 B  
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
$ docker pull nats-streaming@sha256:edf770c6014121e4ea3aac9d7493a33db0256a2e4424a8463446e6649919dbee
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.2061; amd64

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

### `nats-streaming:latest` - windows version 10.0.17763.2061; amd64

```console
$ docker pull nats-streaming@sha256:9d7e58b6bd4fd1ef45339a3497ef7d6a402444f4015ad419d920758ad398c253
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.7 MB (109664361 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ba10fd6c3016a2b0355ec120bdecdcd05c850fb5881ef2436371c86c57688f7`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 06 Jul 2021 20:06:39 GMT
RUN Apply image 1809-amd64
# Wed, 14 Jul 2021 02:35:24 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 14 Jul 2021 18:09:34 GMT
RUN cmd /S /C #(nop) COPY file:72a29a3f2d4a0bd237295ad8b2a317a32c76cbb8a1af898a564024d5013c0475 in C:\nats-streaming-server.exe 
# Wed, 14 Jul 2021 18:09:38 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 14 Jul 2021 18:09:41 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 14 Jul 2021 18:09:44 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:29d43e56445c5279a6386c4dfe4d1ada3c7124ade9cb7b0f2757e58ffc7cd10b`  
		Size: 102.7 MB (102725622 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ec20c4c9f6fa5e782e09342d50033ef24c4049a9dad1befd33c96759b71da6de`  
		Last Modified: Wed, 14 Jul 2021 02:40:36 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c90e8afac4445cb889af58b8a590bdc86382f1e91b54e20bc1009269430e8d7b`  
		Last Modified: Wed, 14 Jul 2021 18:14:47 GMT  
		Size: 6.9 MB (6934158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54dedbbe81a86e2b328335cbf90c2056b3cf884b7bb41a3a2322b58509040298`  
		Last Modified: Wed, 14 Jul 2021 18:14:45 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7b0a78349321bd097f09f3ac8c826322e4c48a945f77e33b86e5699f7477180`  
		Last Modified: Wed, 14 Jul 2021 18:14:45 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c19f14b31cad0b01978407b9da3ddcdd9b2ee36d8a558aa4a30f5bcb62c6ab63`  
		Last Modified: Wed, 14 Jul 2021 18:14:45 GMT  
		Size: 1.1 KB (1148 bytes)  
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
$ docker pull nats-streaming@sha256:afca78bb9fd8e82b1d8dafd00b6e413e795093987abc8b7d198758a95a6bc585
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.2061; amd64

### `nats-streaming:nanoserver` - windows version 10.0.17763.2061; amd64

```console
$ docker pull nats-streaming@sha256:9d7e58b6bd4fd1ef45339a3497ef7d6a402444f4015ad419d920758ad398c253
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.7 MB (109664361 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ba10fd6c3016a2b0355ec120bdecdcd05c850fb5881ef2436371c86c57688f7`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 06 Jul 2021 20:06:39 GMT
RUN Apply image 1809-amd64
# Wed, 14 Jul 2021 02:35:24 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 14 Jul 2021 18:09:34 GMT
RUN cmd /S /C #(nop) COPY file:72a29a3f2d4a0bd237295ad8b2a317a32c76cbb8a1af898a564024d5013c0475 in C:\nats-streaming-server.exe 
# Wed, 14 Jul 2021 18:09:38 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 14 Jul 2021 18:09:41 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 14 Jul 2021 18:09:44 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:29d43e56445c5279a6386c4dfe4d1ada3c7124ade9cb7b0f2757e58ffc7cd10b`  
		Size: 102.7 MB (102725622 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ec20c4c9f6fa5e782e09342d50033ef24c4049a9dad1befd33c96759b71da6de`  
		Last Modified: Wed, 14 Jul 2021 02:40:36 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c90e8afac4445cb889af58b8a590bdc86382f1e91b54e20bc1009269430e8d7b`  
		Last Modified: Wed, 14 Jul 2021 18:14:47 GMT  
		Size: 6.9 MB (6934158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54dedbbe81a86e2b328335cbf90c2056b3cf884b7bb41a3a2322b58509040298`  
		Last Modified: Wed, 14 Jul 2021 18:14:45 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7b0a78349321bd097f09f3ac8c826322e4c48a945f77e33b86e5699f7477180`  
		Last Modified: Wed, 14 Jul 2021 18:14:45 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c19f14b31cad0b01978407b9da3ddcdd9b2ee36d8a558aa4a30f5bcb62c6ab63`  
		Last Modified: Wed, 14 Jul 2021 18:14:45 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:nanoserver-1809`

```console
$ docker pull nats-streaming@sha256:afca78bb9fd8e82b1d8dafd00b6e413e795093987abc8b7d198758a95a6bc585
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.2061; amd64

### `nats-streaming:nanoserver-1809` - windows version 10.0.17763.2061; amd64

```console
$ docker pull nats-streaming@sha256:9d7e58b6bd4fd1ef45339a3497ef7d6a402444f4015ad419d920758ad398c253
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.7 MB (109664361 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ba10fd6c3016a2b0355ec120bdecdcd05c850fb5881ef2436371c86c57688f7`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 06 Jul 2021 20:06:39 GMT
RUN Apply image 1809-amd64
# Wed, 14 Jul 2021 02:35:24 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 14 Jul 2021 18:09:34 GMT
RUN cmd /S /C #(nop) COPY file:72a29a3f2d4a0bd237295ad8b2a317a32c76cbb8a1af898a564024d5013c0475 in C:\nats-streaming-server.exe 
# Wed, 14 Jul 2021 18:09:38 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 14 Jul 2021 18:09:41 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 14 Jul 2021 18:09:44 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:29d43e56445c5279a6386c4dfe4d1ada3c7124ade9cb7b0f2757e58ffc7cd10b`  
		Size: 102.7 MB (102725622 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ec20c4c9f6fa5e782e09342d50033ef24c4049a9dad1befd33c96759b71da6de`  
		Last Modified: Wed, 14 Jul 2021 02:40:36 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c90e8afac4445cb889af58b8a590bdc86382f1e91b54e20bc1009269430e8d7b`  
		Last Modified: Wed, 14 Jul 2021 18:14:47 GMT  
		Size: 6.9 MB (6934158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54dedbbe81a86e2b328335cbf90c2056b3cf884b7bb41a3a2322b58509040298`  
		Last Modified: Wed, 14 Jul 2021 18:14:45 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7b0a78349321bd097f09f3ac8c826322e4c48a945f77e33b86e5699f7477180`  
		Last Modified: Wed, 14 Jul 2021 18:14:45 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c19f14b31cad0b01978407b9da3ddcdd9b2ee36d8a558aa4a30f5bcb62c6ab63`  
		Last Modified: Wed, 14 Jul 2021 18:14:45 GMT  
		Size: 1.1 KB (1148 bytes)  
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
$ docker pull nats-streaming@sha256:5a47a5386f08c246e61fdb7176fed959a7681b0bfbd0f6c347f0392e893558af
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.2061; amd64
	-	windows version 10.0.14393.4530; amd64

### `nats-streaming:windowsservercore` - windows version 10.0.17763.2061; amd64

```console
$ docker pull nats-streaming@sha256:63ca349de872bd42e0977f4246444adb1282f44673a2885c242429de92bc276d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2693100521 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:821eefa949e48160cbd78370042a30b599c173e30585c9e0267045dfacee2488`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 06 Jul 2021 20:34:18 GMT
RUN Install update 1809-amd64
# Wed, 14 Jul 2021 01:07:27 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 14 Jul 2021 02:31:26 GMT
ENV NATS_DOCKERIZED=1
# Wed, 14 Jul 2021 18:06:06 GMT
ENV NATS_STREAMING_SERVER=0.22.0
# Wed, 14 Jul 2021 18:06:08 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.22.0/nats-streaming-server-v0.22.0-windows-amd64.zip
# Wed, 14 Jul 2021 18:06:11 GMT
ENV GIT_DOWNLOAD_SHA256=436c16330efbd0767d9a69dcdf2d3badd4e2598fab23c4f4a192e9d9982c2c92
# Wed, 14 Jul 2021 18:07:11 GMT
RUN Set-PSDebug -Trace 2
# Wed, 14 Jul 2021 18:09:11 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 14 Jul 2021 18:09:14 GMT
EXPOSE 4222 8222
# Wed, 14 Jul 2021 18:09:17 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 14 Jul 2021 18:09:20 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f143c6fed32d477c35b660b2e108ea62e3593c03e44bd9ced208ce52b26b0841`  
		Size: 967.1 MB (967113907 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:adcec6ff907307155c0652222cc9b95a0cc964d4c371e02767e72a5c90472192`  
		Last Modified: Wed, 14 Jul 2021 02:02:19 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f92bdc410321db22d4cf09322869bd9fb2495788c3725624c86d76a6ab3d95d3`  
		Last Modified: Wed, 14 Jul 2021 02:40:16 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4057892101207121360a73faf4dca58c8d6a0bae3bddba124324243bf82f8976`  
		Last Modified: Wed, 14 Jul 2021 18:14:26 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22c2bf3f49a28310b6f20865971fa9b74b600f5288d0da41d85cd3edfed06ab2`  
		Last Modified: Wed, 14 Jul 2021 18:14:26 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b8137a5d079643858ba3385400b934f060f91d9073e0b75e153a7d84623821d`  
		Last Modified: Wed, 14 Jul 2021 18:14:26 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8c50c1de08ec39901fd043365aec3d9ef8c0549ea3669064478276cb8511b1d`  
		Last Modified: Wed, 14 Jul 2021 18:14:24 GMT  
		Size: 364.2 KB (364238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce83bc914faa405040d8788b9995ce447002056425d8d66be1702743ca22871d`  
		Last Modified: Wed, 14 Jul 2021 18:14:32 GMT  
		Size: 7.3 MB (7278180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee11b9df16fbb6a30a224f08de9894c2f03c4a67b17593c9c2bff3e8802d2fa7`  
		Last Modified: Wed, 14 Jul 2021 18:14:23 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e330ba2bb253cf3eb60924484591be1b76f1f7bd76bac5bb452ffd8ba7c45b8e`  
		Last Modified: Wed, 14 Jul 2021 18:14:23 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac321f95e98c7918decd7118f16edefb9f477e75e52b0f096760f0e2266f0edf`  
		Last Modified: Wed, 14 Jul 2021 18:14:23 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:windowsservercore` - windows version 10.0.14393.4530; amd64

```console
$ docker pull nats-streaming@sha256:3ad8c929da66bbecb80008f907271ef5c487403117c5427ed2a07c8e5cc12902
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6281753287 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:45e6693e2a665263f7b8e9067f54ab7cf94a1a5ed7c4bae189a41b98731ce538`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Fri, 09 Jul 2021 05:02:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 14 Jul 2021 01:14:25 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 14 Jul 2021 02:35:48 GMT
ENV NATS_DOCKERIZED=1
# Wed, 14 Jul 2021 18:09:52 GMT
ENV NATS_STREAMING_SERVER=0.22.0
# Wed, 14 Jul 2021 18:09:55 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.22.0/nats-streaming-server-v0.22.0-windows-amd64.zip
# Wed, 14 Jul 2021 18:09:58 GMT
ENV GIT_DOWNLOAD_SHA256=436c16330efbd0767d9a69dcdf2d3badd4e2598fab23c4f4a192e9d9982c2c92
# Wed, 14 Jul 2021 18:11:28 GMT
RUN Set-PSDebug -Trace 2
# Wed, 14 Jul 2021 18:13:47 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 14 Jul 2021 18:13:50 GMT
EXPOSE 4222 8222
# Wed, 14 Jul 2021 18:13:53 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 14 Jul 2021 18:13:55 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a567de41cc349380b25967f180fb1b6b2431bda61ccaaf69d78a33bc9523614a`  
		Size: 2.2 GB (2199646155 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:fed351b78c876c55ec9c7e75d3b9d1b146c5c5dfeb4b5480c0a7c384322df98c`  
		Last Modified: Wed, 14 Jul 2021 02:03:37 GMT  
		Size: 1.4 KB (1444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf08cae8b8db8f3f89e1a9192d393f2da55b44efce4e778fdb58debe2d608275`  
		Last Modified: Wed, 14 Jul 2021 02:40:57 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2feaa7f132d0998b20ad8e1a39c70f7b203986b1920414980bc697f368765d5b`  
		Last Modified: Wed, 14 Jul 2021 18:15:02 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:963d57a144a26f409de2590ce7dcc4eadc787418255737dc70426d7f9082daf9`  
		Last Modified: Wed, 14 Jul 2021 18:15:02 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8ff055cfb27b499cdaf607d5678758a37a200f18cb17ae5444e3e3fbcdc0674`  
		Last Modified: Wed, 14 Jul 2021 18:15:02 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:500b6d026b69103572ab1cfbdadc92ee006f84be89dd397f135f9bedc593fd73`  
		Last Modified: Wed, 14 Jul 2021 18:14:59 GMT  
		Size: 352.1 KB (352069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40da8c0535202c9b305dae1dc40ebe93909e2bc230eabb255309331807baf465`  
		Last Modified: Wed, 14 Jul 2021 18:15:03 GMT  
		Size: 11.8 MB (11757923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6970a1f8eda65e922ce1b5f0a9bba085a1651d7e327422230c343ba6c1e1a3d0`  
		Last Modified: Wed, 14 Jul 2021 18:14:59 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:424f05177cfed5b98dda36cadc9fbee19cba9421a5166678aa8e318792dd94bb`  
		Last Modified: Wed, 14 Jul 2021 18:14:59 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ea1fe02e0ee3dbbe6543d7020be6c660a206ef6c1dc8041bd4a736b276fa15c`  
		Last Modified: Wed, 14 Jul 2021 18:14:59 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:windowsservercore-1809`

```console
$ docker pull nats-streaming@sha256:877c8e5166313ea6fde0584d92b18f50ad4c2d0840f8a03082318e7aafac7aac
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.2061; amd64

### `nats-streaming:windowsservercore-1809` - windows version 10.0.17763.2061; amd64

```console
$ docker pull nats-streaming@sha256:63ca349de872bd42e0977f4246444adb1282f44673a2885c242429de92bc276d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2693100521 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:821eefa949e48160cbd78370042a30b599c173e30585c9e0267045dfacee2488`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 06 Jul 2021 20:34:18 GMT
RUN Install update 1809-amd64
# Wed, 14 Jul 2021 01:07:27 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 14 Jul 2021 02:31:26 GMT
ENV NATS_DOCKERIZED=1
# Wed, 14 Jul 2021 18:06:06 GMT
ENV NATS_STREAMING_SERVER=0.22.0
# Wed, 14 Jul 2021 18:06:08 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.22.0/nats-streaming-server-v0.22.0-windows-amd64.zip
# Wed, 14 Jul 2021 18:06:11 GMT
ENV GIT_DOWNLOAD_SHA256=436c16330efbd0767d9a69dcdf2d3badd4e2598fab23c4f4a192e9d9982c2c92
# Wed, 14 Jul 2021 18:07:11 GMT
RUN Set-PSDebug -Trace 2
# Wed, 14 Jul 2021 18:09:11 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 14 Jul 2021 18:09:14 GMT
EXPOSE 4222 8222
# Wed, 14 Jul 2021 18:09:17 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 14 Jul 2021 18:09:20 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f143c6fed32d477c35b660b2e108ea62e3593c03e44bd9ced208ce52b26b0841`  
		Size: 967.1 MB (967113907 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:adcec6ff907307155c0652222cc9b95a0cc964d4c371e02767e72a5c90472192`  
		Last Modified: Wed, 14 Jul 2021 02:02:19 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f92bdc410321db22d4cf09322869bd9fb2495788c3725624c86d76a6ab3d95d3`  
		Last Modified: Wed, 14 Jul 2021 02:40:16 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4057892101207121360a73faf4dca58c8d6a0bae3bddba124324243bf82f8976`  
		Last Modified: Wed, 14 Jul 2021 18:14:26 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22c2bf3f49a28310b6f20865971fa9b74b600f5288d0da41d85cd3edfed06ab2`  
		Last Modified: Wed, 14 Jul 2021 18:14:26 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b8137a5d079643858ba3385400b934f060f91d9073e0b75e153a7d84623821d`  
		Last Modified: Wed, 14 Jul 2021 18:14:26 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8c50c1de08ec39901fd043365aec3d9ef8c0549ea3669064478276cb8511b1d`  
		Last Modified: Wed, 14 Jul 2021 18:14:24 GMT  
		Size: 364.2 KB (364238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce83bc914faa405040d8788b9995ce447002056425d8d66be1702743ca22871d`  
		Last Modified: Wed, 14 Jul 2021 18:14:32 GMT  
		Size: 7.3 MB (7278180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee11b9df16fbb6a30a224f08de9894c2f03c4a67b17593c9c2bff3e8802d2fa7`  
		Last Modified: Wed, 14 Jul 2021 18:14:23 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e330ba2bb253cf3eb60924484591be1b76f1f7bd76bac5bb452ffd8ba7c45b8e`  
		Last Modified: Wed, 14 Jul 2021 18:14:23 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac321f95e98c7918decd7118f16edefb9f477e75e52b0f096760f0e2266f0edf`  
		Last Modified: Wed, 14 Jul 2021 18:14:23 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:windowsservercore-ltsc2016`

```console
$ docker pull nats-streaming@sha256:9c0cb24674c9c3e1f330cb6e104e1be4355694715cde356dfb21732a03fd84af
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4530; amd64

### `nats-streaming:windowsservercore-ltsc2016` - windows version 10.0.14393.4530; amd64

```console
$ docker pull nats-streaming@sha256:3ad8c929da66bbecb80008f907271ef5c487403117c5427ed2a07c8e5cc12902
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6281753287 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:45e6693e2a665263f7b8e9067f54ab7cf94a1a5ed7c4bae189a41b98731ce538`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Fri, 09 Jul 2021 05:02:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 14 Jul 2021 01:14:25 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 14 Jul 2021 02:35:48 GMT
ENV NATS_DOCKERIZED=1
# Wed, 14 Jul 2021 18:09:52 GMT
ENV NATS_STREAMING_SERVER=0.22.0
# Wed, 14 Jul 2021 18:09:55 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.22.0/nats-streaming-server-v0.22.0-windows-amd64.zip
# Wed, 14 Jul 2021 18:09:58 GMT
ENV GIT_DOWNLOAD_SHA256=436c16330efbd0767d9a69dcdf2d3badd4e2598fab23c4f4a192e9d9982c2c92
# Wed, 14 Jul 2021 18:11:28 GMT
RUN Set-PSDebug -Trace 2
# Wed, 14 Jul 2021 18:13:47 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 14 Jul 2021 18:13:50 GMT
EXPOSE 4222 8222
# Wed, 14 Jul 2021 18:13:53 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 14 Jul 2021 18:13:55 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a567de41cc349380b25967f180fb1b6b2431bda61ccaaf69d78a33bc9523614a`  
		Size: 2.2 GB (2199646155 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:fed351b78c876c55ec9c7e75d3b9d1b146c5c5dfeb4b5480c0a7c384322df98c`  
		Last Modified: Wed, 14 Jul 2021 02:03:37 GMT  
		Size: 1.4 KB (1444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf08cae8b8db8f3f89e1a9192d393f2da55b44efce4e778fdb58debe2d608275`  
		Last Modified: Wed, 14 Jul 2021 02:40:57 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2feaa7f132d0998b20ad8e1a39c70f7b203986b1920414980bc697f368765d5b`  
		Last Modified: Wed, 14 Jul 2021 18:15:02 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:963d57a144a26f409de2590ce7dcc4eadc787418255737dc70426d7f9082daf9`  
		Last Modified: Wed, 14 Jul 2021 18:15:02 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8ff055cfb27b499cdaf607d5678758a37a200f18cb17ae5444e3e3fbcdc0674`  
		Last Modified: Wed, 14 Jul 2021 18:15:02 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:500b6d026b69103572ab1cfbdadc92ee006f84be89dd397f135f9bedc593fd73`  
		Last Modified: Wed, 14 Jul 2021 18:14:59 GMT  
		Size: 352.1 KB (352069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40da8c0535202c9b305dae1dc40ebe93909e2bc230eabb255309331807baf465`  
		Last Modified: Wed, 14 Jul 2021 18:15:03 GMT  
		Size: 11.8 MB (11757923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6970a1f8eda65e922ce1b5f0a9bba085a1651d7e327422230c343ba6c1e1a3d0`  
		Last Modified: Wed, 14 Jul 2021 18:14:59 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:424f05177cfed5b98dda36cadc9fbee19cba9421a5166678aa8e318792dd94bb`  
		Last Modified: Wed, 14 Jul 2021 18:14:59 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ea1fe02e0ee3dbbe6543d7020be6c660a206ef6c1dc8041bd4a736b276fa15c`  
		Last Modified: Wed, 14 Jul 2021 18:14:59 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
