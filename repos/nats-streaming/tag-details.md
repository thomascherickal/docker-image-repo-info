<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `nats-streaming`

-	[`nats-streaming:0.24`](#nats-streaming024)
-	[`nats-streaming:0.24-alpine`](#nats-streaming024-alpine)
-	[`nats-streaming:0.24-alpine3.15`](#nats-streaming024-alpine315)
-	[`nats-streaming:0.24-linux`](#nats-streaming024-linux)
-	[`nats-streaming:0.24-nanoserver`](#nats-streaming024-nanoserver)
-	[`nats-streaming:0.24-nanoserver-1809`](#nats-streaming024-nanoserver-1809)
-	[`nats-streaming:0.24-scratch`](#nats-streaming024-scratch)
-	[`nats-streaming:0.24-windowsservercore`](#nats-streaming024-windowsservercore)
-	[`nats-streaming:0.24-windowsservercore-1809`](#nats-streaming024-windowsservercore-1809)
-	[`nats-streaming:0.24.4`](#nats-streaming0244)
-	[`nats-streaming:0.24.4-alpine`](#nats-streaming0244-alpine)
-	[`nats-streaming:0.24.4-alpine3.15`](#nats-streaming0244-alpine315)
-	[`nats-streaming:0.24.4-linux`](#nats-streaming0244-linux)
-	[`nats-streaming:0.24.4-nanoserver`](#nats-streaming0244-nanoserver)
-	[`nats-streaming:0.24.4-nanoserver-1809`](#nats-streaming0244-nanoserver-1809)
-	[`nats-streaming:0.24.4-scratch`](#nats-streaming0244-scratch)
-	[`nats-streaming:0.24.4-windowsservercore`](#nats-streaming0244-windowsservercore)
-	[`nats-streaming:0.24.4-windowsservercore-1809`](#nats-streaming0244-windowsservercore-1809)
-	[`nats-streaming:alpine`](#nats-streamingalpine)
-	[`nats-streaming:alpine3.15`](#nats-streamingalpine315)
-	[`nats-streaming:latest`](#nats-streaminglatest)
-	[`nats-streaming:linux`](#nats-streaminglinux)
-	[`nats-streaming:nanoserver`](#nats-streamingnanoserver)
-	[`nats-streaming:nanoserver-1809`](#nats-streamingnanoserver-1809)
-	[`nats-streaming:scratch`](#nats-streamingscratch)
-	[`nats-streaming:windowsservercore`](#nats-streamingwindowsservercore)
-	[`nats-streaming:windowsservercore-1809`](#nats-streamingwindowsservercore-1809)

## `nats-streaming:0.24`

```console
$ docker pull nats-streaming@sha256:a8d0b16eaeeb2b6cb4647f942d5a178b7e44d5709388c86fa1357239cf14ea1e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.2803; amd64

### `nats-streaming:0.24` - linux; amd64

```console
$ docker pull nats-streaming@sha256:3ff22408a43de2d67d38aa689b7fede88f92a6e02e9b746402c51441f22a80bd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7160576 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1be4ca5ff457718dd135cac991a2fce8902861901e8f1c7c86e614d68589dced`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 19 Apr 2022 18:19:58 GMT
COPY file:3a9e1a664fc216f321851b3ca6ab92594e42c425862d179ee6a292b590bfe37b in /nats-streaming-server 
# Tue, 19 Apr 2022 18:19:58 GMT
EXPOSE 4222 8222
# Tue, 19 Apr 2022 18:19:58 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 19 Apr 2022 18:19:58 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:f7464e210e47808da4af767838d0a84dada171f8ad1dce32071319a05d071a20`  
		Last Modified: Tue, 19 Apr 2022 18:20:40 GMT  
		Size: 7.2 MB (7160576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.24` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:afa50deb7af027ad2d1a54f53febadf28e189be0adb82039ea429ce57e1d590c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.7 MB (6666873 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:04f3328d94b185bf70d0866dfa2cb72566e7260e4704cfb2cfef87998649aebd`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 19 Apr 2022 18:49:58 GMT
COPY file:6b8eedac2a0774aea5449501f9ae8c79e7be3d3e55863b7703b427f601cbdd4d in /nats-streaming-server 
# Tue, 19 Apr 2022 18:49:58 GMT
EXPOSE 4222 8222
# Tue, 19 Apr 2022 18:49:59 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 19 Apr 2022 18:49:59 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:dbf88d448d58aea59c794a9388b56a7fe82335bef22b8200658329645f9b783a`  
		Last Modified: Tue, 19 Apr 2022 18:51:59 GMT  
		Size: 6.7 MB (6666873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.24` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:e8e52a390d9cefe82a9f17a19e2e05c49d4c56a27b05fb956108c047d5a93b31
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.7 MB (6657656 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:42f1e8f63244361974ea334f20240f6d4f94fc96d7e89051e0769eece666b959`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 19 Apr 2022 18:58:20 GMT
COPY file:17bb63ff84cf537d44fe2a6c3b62b7c20b07b7ddd09ec3e118a9ee70593166c5 in /nats-streaming-server 
# Tue, 19 Apr 2022 18:58:20 GMT
EXPOSE 4222 8222
# Tue, 19 Apr 2022 18:58:21 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 19 Apr 2022 18:58:21 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:501cd5abe17e56e7e4b1c9fb82796e05c14f6dcbf6e964d8c37a33da0eb82757`  
		Last Modified: Tue, 19 Apr 2022 19:00:12 GMT  
		Size: 6.7 MB (6657656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.24` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:e0dc96baa5b7e5dda328b37aa3b8b0c7a8181a6c2b1d987de42b4e5a4fb9398b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6577779 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:274efdfafa30ae2eb7eaaf98eb985e537ddf89be65804d4fdcd414d900365792`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 19 Apr 2022 18:40:21 GMT
COPY file:72420de7c1c1682a55d493d3d9f792d57edc400b24e51ea6987297cc55493b40 in /nats-streaming-server 
# Tue, 19 Apr 2022 18:40:21 GMT
EXPOSE 4222 8222
# Tue, 19 Apr 2022 18:40:22 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 19 Apr 2022 18:40:23 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4a8d243c291d90e3cac092a5d52ec5fe51c7d35bfc569928db3dda38febf3171`  
		Last Modified: Tue, 19 Apr 2022 18:41:22 GMT  
		Size: 6.6 MB (6577779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.24` - windows version 10.0.17763.2803; amd64

```console
$ docker pull nats-streaming@sha256:f7dcabdb7e29722bc9a94ca7545627fb80bceee30902037d345e7ad3ccdc25e4
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.4 MB (110372947 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db815bd2a9cad87072f5c232a6fd4f15c055cfdb61f213ce993afc03a96acb4d`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 04 Apr 2022 10:52:49 GMT
RUN Apply image 1809-amd64
# Wed, 13 Apr 2022 14:45:42 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Tue, 19 Apr 2022 18:18:45 GMT
RUN cmd /S /C #(nop) COPY file:ca12266791259eaa127475f881c8435e255693982581b95714c2329c1c0c3517 in C:\nats-streaming-server.exe 
# Tue, 19 Apr 2022 18:18:46 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Tue, 19 Apr 2022 18:18:47 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Tue, 19 Apr 2022 18:18:48 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:6fc97003d8b7f593fe071cf3ea64f3ce760cc060f3402bb6b1b849c040e222d5`  
		Size: 103.1 MB (103096169 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a6063f744e542c21ce471bdd7ff0dd6063d8d2a9670afbbc64d086813afd6385`  
		Last Modified: Wed, 13 Apr 2022 14:46:35 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9411ac6dc5ee77971f18c4586ba71147422eec4ca4d30dcc320376336f320e5`  
		Last Modified: Tue, 19 Apr 2022 18:19:44 GMT  
		Size: 7.3 MB (7272107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ba1c750731efcee6ebf143a7cf297c1846074c73db7022f94ebdf9ecab5843e`  
		Last Modified: Tue, 19 Apr 2022 18:19:36 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5e494cba0579a95caf948aed68f7f18e8c554774b11313fc73801906d60cba9`  
		Last Modified: Tue, 19 Apr 2022 18:19:36 GMT  
		Size: 1.2 KB (1192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d745e14762b2ee17a49256c2b5940e11f97dc7c944ef9127faa8ae713bcf9d34`  
		Last Modified: Tue, 19 Apr 2022 18:19:36 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.24-alpine`

```console
$ docker pull nats-streaming@sha256:4afc203c1b06db771f04248b810082a998d82540b7962f4f318b760b94918c4c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.24-alpine` - linux; amd64

```console
$ docker pull nats-streaming@sha256:4eb3d3f7784016d57166fb89356a963be2b929bbce0639c40efd6a48dfbeab50
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.2 MB (10248491 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0fa2e30f307c690778bcda9368b96aebbd4007db005d6d8d57416bf9f7d93381`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Tue, 05 Apr 2022 00:19:59 GMT
ADD file:5d673d25da3a14ce1f6cf66e4c7fd4f4b85a3759a9d93efb3fd9ff852b5b56e4 in / 
# Tue, 05 Apr 2022 00:19:59 GMT
CMD ["/bin/sh"]
# Tue, 19 Apr 2022 18:19:47 GMT
ENV NATS_STREAMING_SERVER=0.24.4
# Tue, 19 Apr 2022 18:19:49 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='abf61454846309f4350a209aa86d8def4ceefaa35b576fe027915f31eeaaebf6' ;; 		armhf) natsArch='arm6'; sha256='bc6efafbf051b8bbabe868240ffa9f88a5676727e3c6a5ffc13542ebd0d6585c' ;; 		armv7) natsArch='arm7'; sha256='7950f6ea4b5385454350c8979d6062aa710400a2d21a3a44d971e8535d944545' ;; 		x86_64) natsArch='amd64'; sha256='e7b1db559c02d123d0aabdf0d3a93803eb0778aa733a26ec9067c833bd5728b9' ;; 		x86) natsArch='386'; sha256='941a7be15b8f3d2ba18508baaced39884b1ed86214c2afb2c2bcfcfad3743903' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Tue, 19 Apr 2022 18:19:50 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Tue, 19 Apr 2022 18:19:50 GMT
EXPOSE 4222 8222
# Tue, 19 Apr 2022 18:19:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 19 Apr 2022 18:19:50 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:df9b9388f04ad6279a7410b85cedfdcb2208c0a003da7ab5613af71079148139`  
		Last Modified: Mon, 04 Apr 2022 19:10:16 GMT  
		Size: 2.8 MB (2814559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:618bc609c0fe2d2c7dce4a5a08dcb487ee273dfab15895d917e4f5c2425e54de`  
		Last Modified: Tue, 19 Apr 2022 18:20:20 GMT  
		Size: 7.4 MB (7433512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78cdc64ae36d5c3024c2af60810ec1bfff47708a2492efc85d7f5bfecf7abcfe`  
		Last Modified: Tue, 19 Apr 2022 18:20:16 GMT  
		Size: 420.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.24-alpine` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:092009bcc3beed0c4e6dd0b2e36eb45082919a3cf6178ac42576e7599efefb26
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.6 MB (9562443 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6edad2d6e424051bf23151c9f0b88c0a1ae0f02e7ca579630d5f54da30fb8e69`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Mon, 04 Apr 2022 23:49:42 GMT
ADD file:159dcddaab900372df882a4e94615ed84250e9cea3e74bc0479d98280342f596 in / 
# Mon, 04 Apr 2022 23:49:42 GMT
CMD ["/bin/sh"]
# Tue, 19 Apr 2022 18:49:33 GMT
ENV NATS_STREAMING_SERVER=0.24.4
# Tue, 19 Apr 2022 18:49:37 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='abf61454846309f4350a209aa86d8def4ceefaa35b576fe027915f31eeaaebf6' ;; 		armhf) natsArch='arm6'; sha256='bc6efafbf051b8bbabe868240ffa9f88a5676727e3c6a5ffc13542ebd0d6585c' ;; 		armv7) natsArch='arm7'; sha256='7950f6ea4b5385454350c8979d6062aa710400a2d21a3a44d971e8535d944545' ;; 		x86_64) natsArch='amd64'; sha256='e7b1db559c02d123d0aabdf0d3a93803eb0778aa733a26ec9067c833bd5728b9' ;; 		x86) natsArch='386'; sha256='941a7be15b8f3d2ba18508baaced39884b1ed86214c2afb2c2bcfcfad3743903' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Tue, 19 Apr 2022 18:49:38 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Tue, 19 Apr 2022 18:49:38 GMT
EXPOSE 4222 8222
# Tue, 19 Apr 2022 18:49:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 19 Apr 2022 18:49:39 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:c319b1fc4ed70b8241a7ce6ac0c4015d354bf5cf8c01eb73c50b6709c0c46e49`  
		Last Modified: Mon, 04 Apr 2022 19:09:22 GMT  
		Size: 2.6 MB (2621972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7749efc5f39c770d1ec4c0ef3a405656aa5e1993fbdacd7d21f3d4707ff1a72c`  
		Last Modified: Tue, 19 Apr 2022 18:51:22 GMT  
		Size: 6.9 MB (6940049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a23a7c4070e79cc4538b1305be5da3a4b615da587a7fd569a0be26bd110fa84`  
		Last Modified: Tue, 19 Apr 2022 18:51:18 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.24-alpine` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:43fa0020bbe495315ac2f09debe4bf6b27dd74790d26ac3366750c3055e58a3c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.4 MB (9354606 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4afe09639533164664c235319932921bedc9450ecd3de243641a70c7a583c5d1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Mon, 04 Apr 2022 23:57:34 GMT
ADD file:20f8cdddc53a4a8bd78945fc32fe08e9f80ab3b16dc20a9aa4ba73b79f2bc71c in / 
# Mon, 04 Apr 2022 23:57:35 GMT
CMD ["/bin/sh"]
# Tue, 19 Apr 2022 18:57:51 GMT
ENV NATS_STREAMING_SERVER=0.24.4
# Tue, 19 Apr 2022 18:57:55 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='abf61454846309f4350a209aa86d8def4ceefaa35b576fe027915f31eeaaebf6' ;; 		armhf) natsArch='arm6'; sha256='bc6efafbf051b8bbabe868240ffa9f88a5676727e3c6a5ffc13542ebd0d6585c' ;; 		armv7) natsArch='arm7'; sha256='7950f6ea4b5385454350c8979d6062aa710400a2d21a3a44d971e8535d944545' ;; 		x86_64) natsArch='amd64'; sha256='e7b1db559c02d123d0aabdf0d3a93803eb0778aa733a26ec9067c833bd5728b9' ;; 		x86) natsArch='386'; sha256='941a7be15b8f3d2ba18508baaced39884b1ed86214c2afb2c2bcfcfad3743903' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Tue, 19 Apr 2022 18:57:56 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Tue, 19 Apr 2022 18:57:56 GMT
EXPOSE 4222 8222
# Tue, 19 Apr 2022 18:57:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 19 Apr 2022 18:57:57 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:57fb4b5f1a47c953ca5703f0f81ce14e5d01cf23aa79558b5adb961cc526e320`  
		Last Modified: Mon, 04 Apr 2022 19:09:36 GMT  
		Size: 2.4 MB (2424323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cab0ba64de7ddcb969882eb8b609a89179c2d441a4bcc7317ae977fd7dda4e23`  
		Last Modified: Tue, 19 Apr 2022 18:59:41 GMT  
		Size: 6.9 MB (6929861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27e7fde7215edaedba408f2d6f77c7043df6c84d3309cffeb7f8b14f1c0b82c0`  
		Last Modified: Tue, 19 Apr 2022 18:59:37 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.24-alpine` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:bef1eb9f86f148797e14e6dd500934864bd8611f0256715a932c286bbedbddb4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.6 MB (9567309 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89a27b9fd024c9823aa8be1c38baede9477c1bf1ab37ddbec1c6d01c2a3a658a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:31 GMT
ADD file:90e56af13188c7f0283d244a0d70b853d8bef8587a41f1da8eac3a2aba8964ef in / 
# Mon, 04 Apr 2022 23:39:31 GMT
CMD ["/bin/sh"]
# Tue, 19 Apr 2022 18:40:04 GMT
ENV NATS_STREAMING_SERVER=0.24.4
# Tue, 19 Apr 2022 18:40:07 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='abf61454846309f4350a209aa86d8def4ceefaa35b576fe027915f31eeaaebf6' ;; 		armhf) natsArch='arm6'; sha256='bc6efafbf051b8bbabe868240ffa9f88a5676727e3c6a5ffc13542ebd0d6585c' ;; 		armv7) natsArch='arm7'; sha256='7950f6ea4b5385454350c8979d6062aa710400a2d21a3a44d971e8535d944545' ;; 		x86_64) natsArch='amd64'; sha256='e7b1db559c02d123d0aabdf0d3a93803eb0778aa733a26ec9067c833bd5728b9' ;; 		x86) natsArch='386'; sha256='941a7be15b8f3d2ba18508baaced39884b1ed86214c2afb2c2bcfcfad3743903' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Tue, 19 Apr 2022 18:40:09 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Tue, 19 Apr 2022 18:40:09 GMT
EXPOSE 4222 8222
# Tue, 19 Apr 2022 18:40:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 19 Apr 2022 18:40:11 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:9981e73032c8833e387a8f96986e560edbed12c38119e0edb0439c9c2234eac9`  
		Last Modified: Mon, 04 Apr 2022 19:09:10 GMT  
		Size: 2.7 MB (2716477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0812492999c8bb5bc4d5d0f3cf25e7e1a474b07e1400c864e6f714d6c9771fb1`  
		Last Modified: Tue, 19 Apr 2022 18:40:59 GMT  
		Size: 6.9 MB (6850411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0aedb2f212694a12d2b97ef1d1079ba39d77f30b8574a79cc0421d472c6dfae`  
		Last Modified: Tue, 19 Apr 2022 18:40:58 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.24-alpine3.15`

```console
$ docker pull nats-streaming@sha256:4afc203c1b06db771f04248b810082a998d82540b7962f4f318b760b94918c4c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.24-alpine3.15` - linux; amd64

```console
$ docker pull nats-streaming@sha256:4eb3d3f7784016d57166fb89356a963be2b929bbce0639c40efd6a48dfbeab50
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.2 MB (10248491 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0fa2e30f307c690778bcda9368b96aebbd4007db005d6d8d57416bf9f7d93381`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Tue, 05 Apr 2022 00:19:59 GMT
ADD file:5d673d25da3a14ce1f6cf66e4c7fd4f4b85a3759a9d93efb3fd9ff852b5b56e4 in / 
# Tue, 05 Apr 2022 00:19:59 GMT
CMD ["/bin/sh"]
# Tue, 19 Apr 2022 18:19:47 GMT
ENV NATS_STREAMING_SERVER=0.24.4
# Tue, 19 Apr 2022 18:19:49 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='abf61454846309f4350a209aa86d8def4ceefaa35b576fe027915f31eeaaebf6' ;; 		armhf) natsArch='arm6'; sha256='bc6efafbf051b8bbabe868240ffa9f88a5676727e3c6a5ffc13542ebd0d6585c' ;; 		armv7) natsArch='arm7'; sha256='7950f6ea4b5385454350c8979d6062aa710400a2d21a3a44d971e8535d944545' ;; 		x86_64) natsArch='amd64'; sha256='e7b1db559c02d123d0aabdf0d3a93803eb0778aa733a26ec9067c833bd5728b9' ;; 		x86) natsArch='386'; sha256='941a7be15b8f3d2ba18508baaced39884b1ed86214c2afb2c2bcfcfad3743903' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Tue, 19 Apr 2022 18:19:50 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Tue, 19 Apr 2022 18:19:50 GMT
EXPOSE 4222 8222
# Tue, 19 Apr 2022 18:19:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 19 Apr 2022 18:19:50 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:df9b9388f04ad6279a7410b85cedfdcb2208c0a003da7ab5613af71079148139`  
		Last Modified: Mon, 04 Apr 2022 19:10:16 GMT  
		Size: 2.8 MB (2814559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:618bc609c0fe2d2c7dce4a5a08dcb487ee273dfab15895d917e4f5c2425e54de`  
		Last Modified: Tue, 19 Apr 2022 18:20:20 GMT  
		Size: 7.4 MB (7433512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78cdc64ae36d5c3024c2af60810ec1bfff47708a2492efc85d7f5bfecf7abcfe`  
		Last Modified: Tue, 19 Apr 2022 18:20:16 GMT  
		Size: 420.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.24-alpine3.15` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:092009bcc3beed0c4e6dd0b2e36eb45082919a3cf6178ac42576e7599efefb26
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.6 MB (9562443 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6edad2d6e424051bf23151c9f0b88c0a1ae0f02e7ca579630d5f54da30fb8e69`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Mon, 04 Apr 2022 23:49:42 GMT
ADD file:159dcddaab900372df882a4e94615ed84250e9cea3e74bc0479d98280342f596 in / 
# Mon, 04 Apr 2022 23:49:42 GMT
CMD ["/bin/sh"]
# Tue, 19 Apr 2022 18:49:33 GMT
ENV NATS_STREAMING_SERVER=0.24.4
# Tue, 19 Apr 2022 18:49:37 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='abf61454846309f4350a209aa86d8def4ceefaa35b576fe027915f31eeaaebf6' ;; 		armhf) natsArch='arm6'; sha256='bc6efafbf051b8bbabe868240ffa9f88a5676727e3c6a5ffc13542ebd0d6585c' ;; 		armv7) natsArch='arm7'; sha256='7950f6ea4b5385454350c8979d6062aa710400a2d21a3a44d971e8535d944545' ;; 		x86_64) natsArch='amd64'; sha256='e7b1db559c02d123d0aabdf0d3a93803eb0778aa733a26ec9067c833bd5728b9' ;; 		x86) natsArch='386'; sha256='941a7be15b8f3d2ba18508baaced39884b1ed86214c2afb2c2bcfcfad3743903' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Tue, 19 Apr 2022 18:49:38 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Tue, 19 Apr 2022 18:49:38 GMT
EXPOSE 4222 8222
# Tue, 19 Apr 2022 18:49:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 19 Apr 2022 18:49:39 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:c319b1fc4ed70b8241a7ce6ac0c4015d354bf5cf8c01eb73c50b6709c0c46e49`  
		Last Modified: Mon, 04 Apr 2022 19:09:22 GMT  
		Size: 2.6 MB (2621972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7749efc5f39c770d1ec4c0ef3a405656aa5e1993fbdacd7d21f3d4707ff1a72c`  
		Last Modified: Tue, 19 Apr 2022 18:51:22 GMT  
		Size: 6.9 MB (6940049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a23a7c4070e79cc4538b1305be5da3a4b615da587a7fd569a0be26bd110fa84`  
		Last Modified: Tue, 19 Apr 2022 18:51:18 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.24-alpine3.15` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:43fa0020bbe495315ac2f09debe4bf6b27dd74790d26ac3366750c3055e58a3c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.4 MB (9354606 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4afe09639533164664c235319932921bedc9450ecd3de243641a70c7a583c5d1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Mon, 04 Apr 2022 23:57:34 GMT
ADD file:20f8cdddc53a4a8bd78945fc32fe08e9f80ab3b16dc20a9aa4ba73b79f2bc71c in / 
# Mon, 04 Apr 2022 23:57:35 GMT
CMD ["/bin/sh"]
# Tue, 19 Apr 2022 18:57:51 GMT
ENV NATS_STREAMING_SERVER=0.24.4
# Tue, 19 Apr 2022 18:57:55 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='abf61454846309f4350a209aa86d8def4ceefaa35b576fe027915f31eeaaebf6' ;; 		armhf) natsArch='arm6'; sha256='bc6efafbf051b8bbabe868240ffa9f88a5676727e3c6a5ffc13542ebd0d6585c' ;; 		armv7) natsArch='arm7'; sha256='7950f6ea4b5385454350c8979d6062aa710400a2d21a3a44d971e8535d944545' ;; 		x86_64) natsArch='amd64'; sha256='e7b1db559c02d123d0aabdf0d3a93803eb0778aa733a26ec9067c833bd5728b9' ;; 		x86) natsArch='386'; sha256='941a7be15b8f3d2ba18508baaced39884b1ed86214c2afb2c2bcfcfad3743903' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Tue, 19 Apr 2022 18:57:56 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Tue, 19 Apr 2022 18:57:56 GMT
EXPOSE 4222 8222
# Tue, 19 Apr 2022 18:57:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 19 Apr 2022 18:57:57 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:57fb4b5f1a47c953ca5703f0f81ce14e5d01cf23aa79558b5adb961cc526e320`  
		Last Modified: Mon, 04 Apr 2022 19:09:36 GMT  
		Size: 2.4 MB (2424323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cab0ba64de7ddcb969882eb8b609a89179c2d441a4bcc7317ae977fd7dda4e23`  
		Last Modified: Tue, 19 Apr 2022 18:59:41 GMT  
		Size: 6.9 MB (6929861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27e7fde7215edaedba408f2d6f77c7043df6c84d3309cffeb7f8b14f1c0b82c0`  
		Last Modified: Tue, 19 Apr 2022 18:59:37 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.24-alpine3.15` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:bef1eb9f86f148797e14e6dd500934864bd8611f0256715a932c286bbedbddb4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.6 MB (9567309 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89a27b9fd024c9823aa8be1c38baede9477c1bf1ab37ddbec1c6d01c2a3a658a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:31 GMT
ADD file:90e56af13188c7f0283d244a0d70b853d8bef8587a41f1da8eac3a2aba8964ef in / 
# Mon, 04 Apr 2022 23:39:31 GMT
CMD ["/bin/sh"]
# Tue, 19 Apr 2022 18:40:04 GMT
ENV NATS_STREAMING_SERVER=0.24.4
# Tue, 19 Apr 2022 18:40:07 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='abf61454846309f4350a209aa86d8def4ceefaa35b576fe027915f31eeaaebf6' ;; 		armhf) natsArch='arm6'; sha256='bc6efafbf051b8bbabe868240ffa9f88a5676727e3c6a5ffc13542ebd0d6585c' ;; 		armv7) natsArch='arm7'; sha256='7950f6ea4b5385454350c8979d6062aa710400a2d21a3a44d971e8535d944545' ;; 		x86_64) natsArch='amd64'; sha256='e7b1db559c02d123d0aabdf0d3a93803eb0778aa733a26ec9067c833bd5728b9' ;; 		x86) natsArch='386'; sha256='941a7be15b8f3d2ba18508baaced39884b1ed86214c2afb2c2bcfcfad3743903' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Tue, 19 Apr 2022 18:40:09 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Tue, 19 Apr 2022 18:40:09 GMT
EXPOSE 4222 8222
# Tue, 19 Apr 2022 18:40:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 19 Apr 2022 18:40:11 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:9981e73032c8833e387a8f96986e560edbed12c38119e0edb0439c9c2234eac9`  
		Last Modified: Mon, 04 Apr 2022 19:09:10 GMT  
		Size: 2.7 MB (2716477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0812492999c8bb5bc4d5d0f3cf25e7e1a474b07e1400c864e6f714d6c9771fb1`  
		Last Modified: Tue, 19 Apr 2022 18:40:59 GMT  
		Size: 6.9 MB (6850411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0aedb2f212694a12d2b97ef1d1079ba39d77f30b8574a79cc0421d472c6dfae`  
		Last Modified: Tue, 19 Apr 2022 18:40:58 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.24-linux`

```console
$ docker pull nats-streaming@sha256:bf7595fa0e1871058be97fa42b8155f796e95f2582fb2141a11f4a51cdff18e9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.24-linux` - linux; amd64

```console
$ docker pull nats-streaming@sha256:3ff22408a43de2d67d38aa689b7fede88f92a6e02e9b746402c51441f22a80bd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7160576 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1be4ca5ff457718dd135cac991a2fce8902861901e8f1c7c86e614d68589dced`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 19 Apr 2022 18:19:58 GMT
COPY file:3a9e1a664fc216f321851b3ca6ab92594e42c425862d179ee6a292b590bfe37b in /nats-streaming-server 
# Tue, 19 Apr 2022 18:19:58 GMT
EXPOSE 4222 8222
# Tue, 19 Apr 2022 18:19:58 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 19 Apr 2022 18:19:58 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:f7464e210e47808da4af767838d0a84dada171f8ad1dce32071319a05d071a20`  
		Last Modified: Tue, 19 Apr 2022 18:20:40 GMT  
		Size: 7.2 MB (7160576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.24-linux` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:afa50deb7af027ad2d1a54f53febadf28e189be0adb82039ea429ce57e1d590c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.7 MB (6666873 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:04f3328d94b185bf70d0866dfa2cb72566e7260e4704cfb2cfef87998649aebd`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 19 Apr 2022 18:49:58 GMT
COPY file:6b8eedac2a0774aea5449501f9ae8c79e7be3d3e55863b7703b427f601cbdd4d in /nats-streaming-server 
# Tue, 19 Apr 2022 18:49:58 GMT
EXPOSE 4222 8222
# Tue, 19 Apr 2022 18:49:59 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 19 Apr 2022 18:49:59 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:dbf88d448d58aea59c794a9388b56a7fe82335bef22b8200658329645f9b783a`  
		Last Modified: Tue, 19 Apr 2022 18:51:59 GMT  
		Size: 6.7 MB (6666873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.24-linux` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:e8e52a390d9cefe82a9f17a19e2e05c49d4c56a27b05fb956108c047d5a93b31
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.7 MB (6657656 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:42f1e8f63244361974ea334f20240f6d4f94fc96d7e89051e0769eece666b959`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 19 Apr 2022 18:58:20 GMT
COPY file:17bb63ff84cf537d44fe2a6c3b62b7c20b07b7ddd09ec3e118a9ee70593166c5 in /nats-streaming-server 
# Tue, 19 Apr 2022 18:58:20 GMT
EXPOSE 4222 8222
# Tue, 19 Apr 2022 18:58:21 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 19 Apr 2022 18:58:21 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:501cd5abe17e56e7e4b1c9fb82796e05c14f6dcbf6e964d8c37a33da0eb82757`  
		Last Modified: Tue, 19 Apr 2022 19:00:12 GMT  
		Size: 6.7 MB (6657656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.24-linux` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:e0dc96baa5b7e5dda328b37aa3b8b0c7a8181a6c2b1d987de42b4e5a4fb9398b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6577779 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:274efdfafa30ae2eb7eaaf98eb985e537ddf89be65804d4fdcd414d900365792`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 19 Apr 2022 18:40:21 GMT
COPY file:72420de7c1c1682a55d493d3d9f792d57edc400b24e51ea6987297cc55493b40 in /nats-streaming-server 
# Tue, 19 Apr 2022 18:40:21 GMT
EXPOSE 4222 8222
# Tue, 19 Apr 2022 18:40:22 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 19 Apr 2022 18:40:23 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4a8d243c291d90e3cac092a5d52ec5fe51c7d35bfc569928db3dda38febf3171`  
		Last Modified: Tue, 19 Apr 2022 18:41:22 GMT  
		Size: 6.6 MB (6577779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.24-nanoserver`

```console
$ docker pull nats-streaming@sha256:5f0fd8d176c73f6fd991c80241c4d8ad94259cff1ea5994dae8aea7b99d35a67
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2803; amd64

### `nats-streaming:0.24-nanoserver` - windows version 10.0.17763.2803; amd64

```console
$ docker pull nats-streaming@sha256:f7dcabdb7e29722bc9a94ca7545627fb80bceee30902037d345e7ad3ccdc25e4
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.4 MB (110372947 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db815bd2a9cad87072f5c232a6fd4f15c055cfdb61f213ce993afc03a96acb4d`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 04 Apr 2022 10:52:49 GMT
RUN Apply image 1809-amd64
# Wed, 13 Apr 2022 14:45:42 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Tue, 19 Apr 2022 18:18:45 GMT
RUN cmd /S /C #(nop) COPY file:ca12266791259eaa127475f881c8435e255693982581b95714c2329c1c0c3517 in C:\nats-streaming-server.exe 
# Tue, 19 Apr 2022 18:18:46 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Tue, 19 Apr 2022 18:18:47 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Tue, 19 Apr 2022 18:18:48 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:6fc97003d8b7f593fe071cf3ea64f3ce760cc060f3402bb6b1b849c040e222d5`  
		Size: 103.1 MB (103096169 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a6063f744e542c21ce471bdd7ff0dd6063d8d2a9670afbbc64d086813afd6385`  
		Last Modified: Wed, 13 Apr 2022 14:46:35 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9411ac6dc5ee77971f18c4586ba71147422eec4ca4d30dcc320376336f320e5`  
		Last Modified: Tue, 19 Apr 2022 18:19:44 GMT  
		Size: 7.3 MB (7272107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ba1c750731efcee6ebf143a7cf297c1846074c73db7022f94ebdf9ecab5843e`  
		Last Modified: Tue, 19 Apr 2022 18:19:36 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5e494cba0579a95caf948aed68f7f18e8c554774b11313fc73801906d60cba9`  
		Last Modified: Tue, 19 Apr 2022 18:19:36 GMT  
		Size: 1.2 KB (1192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d745e14762b2ee17a49256c2b5940e11f97dc7c944ef9127faa8ae713bcf9d34`  
		Last Modified: Tue, 19 Apr 2022 18:19:36 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.24-nanoserver-1809`

```console
$ docker pull nats-streaming@sha256:5f0fd8d176c73f6fd991c80241c4d8ad94259cff1ea5994dae8aea7b99d35a67
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2803; amd64

### `nats-streaming:0.24-nanoserver-1809` - windows version 10.0.17763.2803; amd64

```console
$ docker pull nats-streaming@sha256:f7dcabdb7e29722bc9a94ca7545627fb80bceee30902037d345e7ad3ccdc25e4
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.4 MB (110372947 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db815bd2a9cad87072f5c232a6fd4f15c055cfdb61f213ce993afc03a96acb4d`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 04 Apr 2022 10:52:49 GMT
RUN Apply image 1809-amd64
# Wed, 13 Apr 2022 14:45:42 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Tue, 19 Apr 2022 18:18:45 GMT
RUN cmd /S /C #(nop) COPY file:ca12266791259eaa127475f881c8435e255693982581b95714c2329c1c0c3517 in C:\nats-streaming-server.exe 
# Tue, 19 Apr 2022 18:18:46 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Tue, 19 Apr 2022 18:18:47 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Tue, 19 Apr 2022 18:18:48 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:6fc97003d8b7f593fe071cf3ea64f3ce760cc060f3402bb6b1b849c040e222d5`  
		Size: 103.1 MB (103096169 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a6063f744e542c21ce471bdd7ff0dd6063d8d2a9670afbbc64d086813afd6385`  
		Last Modified: Wed, 13 Apr 2022 14:46:35 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9411ac6dc5ee77971f18c4586ba71147422eec4ca4d30dcc320376336f320e5`  
		Last Modified: Tue, 19 Apr 2022 18:19:44 GMT  
		Size: 7.3 MB (7272107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ba1c750731efcee6ebf143a7cf297c1846074c73db7022f94ebdf9ecab5843e`  
		Last Modified: Tue, 19 Apr 2022 18:19:36 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5e494cba0579a95caf948aed68f7f18e8c554774b11313fc73801906d60cba9`  
		Last Modified: Tue, 19 Apr 2022 18:19:36 GMT  
		Size: 1.2 KB (1192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d745e14762b2ee17a49256c2b5940e11f97dc7c944ef9127faa8ae713bcf9d34`  
		Last Modified: Tue, 19 Apr 2022 18:19:36 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.24-scratch`

```console
$ docker pull nats-streaming@sha256:bf7595fa0e1871058be97fa42b8155f796e95f2582fb2141a11f4a51cdff18e9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.24-scratch` - linux; amd64

```console
$ docker pull nats-streaming@sha256:3ff22408a43de2d67d38aa689b7fede88f92a6e02e9b746402c51441f22a80bd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7160576 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1be4ca5ff457718dd135cac991a2fce8902861901e8f1c7c86e614d68589dced`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 19 Apr 2022 18:19:58 GMT
COPY file:3a9e1a664fc216f321851b3ca6ab92594e42c425862d179ee6a292b590bfe37b in /nats-streaming-server 
# Tue, 19 Apr 2022 18:19:58 GMT
EXPOSE 4222 8222
# Tue, 19 Apr 2022 18:19:58 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 19 Apr 2022 18:19:58 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:f7464e210e47808da4af767838d0a84dada171f8ad1dce32071319a05d071a20`  
		Last Modified: Tue, 19 Apr 2022 18:20:40 GMT  
		Size: 7.2 MB (7160576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.24-scratch` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:afa50deb7af027ad2d1a54f53febadf28e189be0adb82039ea429ce57e1d590c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.7 MB (6666873 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:04f3328d94b185bf70d0866dfa2cb72566e7260e4704cfb2cfef87998649aebd`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 19 Apr 2022 18:49:58 GMT
COPY file:6b8eedac2a0774aea5449501f9ae8c79e7be3d3e55863b7703b427f601cbdd4d in /nats-streaming-server 
# Tue, 19 Apr 2022 18:49:58 GMT
EXPOSE 4222 8222
# Tue, 19 Apr 2022 18:49:59 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 19 Apr 2022 18:49:59 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:dbf88d448d58aea59c794a9388b56a7fe82335bef22b8200658329645f9b783a`  
		Last Modified: Tue, 19 Apr 2022 18:51:59 GMT  
		Size: 6.7 MB (6666873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.24-scratch` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:e8e52a390d9cefe82a9f17a19e2e05c49d4c56a27b05fb956108c047d5a93b31
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.7 MB (6657656 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:42f1e8f63244361974ea334f20240f6d4f94fc96d7e89051e0769eece666b959`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 19 Apr 2022 18:58:20 GMT
COPY file:17bb63ff84cf537d44fe2a6c3b62b7c20b07b7ddd09ec3e118a9ee70593166c5 in /nats-streaming-server 
# Tue, 19 Apr 2022 18:58:20 GMT
EXPOSE 4222 8222
# Tue, 19 Apr 2022 18:58:21 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 19 Apr 2022 18:58:21 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:501cd5abe17e56e7e4b1c9fb82796e05c14f6dcbf6e964d8c37a33da0eb82757`  
		Last Modified: Tue, 19 Apr 2022 19:00:12 GMT  
		Size: 6.7 MB (6657656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.24-scratch` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:e0dc96baa5b7e5dda328b37aa3b8b0c7a8181a6c2b1d987de42b4e5a4fb9398b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6577779 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:274efdfafa30ae2eb7eaaf98eb985e537ddf89be65804d4fdcd414d900365792`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 19 Apr 2022 18:40:21 GMT
COPY file:72420de7c1c1682a55d493d3d9f792d57edc400b24e51ea6987297cc55493b40 in /nats-streaming-server 
# Tue, 19 Apr 2022 18:40:21 GMT
EXPOSE 4222 8222
# Tue, 19 Apr 2022 18:40:22 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 19 Apr 2022 18:40:23 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4a8d243c291d90e3cac092a5d52ec5fe51c7d35bfc569928db3dda38febf3171`  
		Last Modified: Tue, 19 Apr 2022 18:41:22 GMT  
		Size: 6.6 MB (6577779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.24-windowsservercore`

```console
$ docker pull nats-streaming@sha256:86c23aeb014348875713589438ea483f5d1f8c2c81a6dae1437392934b1792ef
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2803; amd64

### `nats-streaming:0.24-windowsservercore` - windows version 10.0.17763.2803; amd64

```console
$ docker pull nats-streaming@sha256:72f0e5b61606638041efba42873ea1291d8b05d973accd3fa4fb8d87a81dcb5f
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2723900130 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b04dd0632cb73bbae0011b92981b880cef224abb6cb100902b20f342efce7de6`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 04 Apr 2022 11:20:25 GMT
RUN Install update 1809-amd64
# Wed, 13 Apr 2022 12:43:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 Apr 2022 14:42:30 GMT
ENV NATS_DOCKERIZED=1
# Tue, 19 Apr 2022 18:15:31 GMT
ENV NATS_STREAMING_SERVER=0.24.4
# Tue, 19 Apr 2022 18:15:32 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.24.4/nats-streaming-server-v0.24.4-windows-amd64.zip
# Tue, 19 Apr 2022 18:15:33 GMT
ENV NATS_STREAMING_SERVER_SHASUM=147b39fb88a9eb45c3f5692365fa6ee17d95c627bb4ecde7601f68151ace6c41
# Tue, 19 Apr 2022 18:16:48 GMT
RUN Set-PSDebug -Trace 2
# Tue, 19 Apr 2022 18:18:32 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Tue, 19 Apr 2022 18:18:33 GMT
EXPOSE 4222 8222
# Tue, 19 Apr 2022 18:18:34 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Tue, 19 Apr 2022 18:18:35 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ba8181afd4264392fbbf8df14fb4cddc55fbe085ab000e986b789678bc2bb171`  
		Size: 997.6 MB (997587446 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7ebb23aa64bff633cfa3c62b190d84f0e870b04fecb1910f65d0870b5c7f8981`  
		Last Modified: Wed, 13 Apr 2022 14:12:24 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d838c7a98a95bee63894bac798124e8c8572bcacc23e22d85332d453a03a7d7c`  
		Last Modified: Wed, 13 Apr 2022 14:46:17 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63c30d5de5c74ae8a10de14dcc644f3d8db3247159e379e97bfa4a735c0484b6`  
		Last Modified: Tue, 19 Apr 2022 18:19:18 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:611dcea795d1cfe41e1bed673aced23eeba03240c857b46e94747a9b1cddc357`  
		Last Modified: Tue, 19 Apr 2022 18:19:18 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71f868b0b44531e50958ac6c35c161df79228938ab68d4cc7f2b5ddb6384bbd6`  
		Last Modified: Tue, 19 Apr 2022 18:19:18 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d1bd238023271362f8a5a1136b0e5dc705f18688f793dfd34788834dcfbaf32`  
		Last Modified: Tue, 19 Apr 2022 18:19:16 GMT  
		Size: 359.5 KB (359505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0216f3dd53c339c5889dc7bf0dcdcc98ff1b6841b330934f5b991fff52f4574`  
		Last Modified: Tue, 19 Apr 2022 18:19:24 GMT  
		Size: 7.6 MB (7608996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9a52e26f86cff8b968456c51fce3ae5ddb74a9f265da6aec6c4c0104be544b8`  
		Last Modified: Tue, 19 Apr 2022 18:19:16 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4d63ac7f4ccd54465f51b2b43d349150f3ab34b0e60ccc8a22fb65b0bbe1b76`  
		Last Modified: Tue, 19 Apr 2022 18:19:15 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7b91f9f9d8dda9458f9dea3b30fd662ae28ec4bb3bdf3d98f9ccfc1a9be475f`  
		Last Modified: Tue, 19 Apr 2022 18:19:16 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.24-windowsservercore-1809`

```console
$ docker pull nats-streaming@sha256:86c23aeb014348875713589438ea483f5d1f8c2c81a6dae1437392934b1792ef
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2803; amd64

### `nats-streaming:0.24-windowsservercore-1809` - windows version 10.0.17763.2803; amd64

```console
$ docker pull nats-streaming@sha256:72f0e5b61606638041efba42873ea1291d8b05d973accd3fa4fb8d87a81dcb5f
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2723900130 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b04dd0632cb73bbae0011b92981b880cef224abb6cb100902b20f342efce7de6`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 04 Apr 2022 11:20:25 GMT
RUN Install update 1809-amd64
# Wed, 13 Apr 2022 12:43:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 Apr 2022 14:42:30 GMT
ENV NATS_DOCKERIZED=1
# Tue, 19 Apr 2022 18:15:31 GMT
ENV NATS_STREAMING_SERVER=0.24.4
# Tue, 19 Apr 2022 18:15:32 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.24.4/nats-streaming-server-v0.24.4-windows-amd64.zip
# Tue, 19 Apr 2022 18:15:33 GMT
ENV NATS_STREAMING_SERVER_SHASUM=147b39fb88a9eb45c3f5692365fa6ee17d95c627bb4ecde7601f68151ace6c41
# Tue, 19 Apr 2022 18:16:48 GMT
RUN Set-PSDebug -Trace 2
# Tue, 19 Apr 2022 18:18:32 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Tue, 19 Apr 2022 18:18:33 GMT
EXPOSE 4222 8222
# Tue, 19 Apr 2022 18:18:34 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Tue, 19 Apr 2022 18:18:35 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ba8181afd4264392fbbf8df14fb4cddc55fbe085ab000e986b789678bc2bb171`  
		Size: 997.6 MB (997587446 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7ebb23aa64bff633cfa3c62b190d84f0e870b04fecb1910f65d0870b5c7f8981`  
		Last Modified: Wed, 13 Apr 2022 14:12:24 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d838c7a98a95bee63894bac798124e8c8572bcacc23e22d85332d453a03a7d7c`  
		Last Modified: Wed, 13 Apr 2022 14:46:17 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63c30d5de5c74ae8a10de14dcc644f3d8db3247159e379e97bfa4a735c0484b6`  
		Last Modified: Tue, 19 Apr 2022 18:19:18 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:611dcea795d1cfe41e1bed673aced23eeba03240c857b46e94747a9b1cddc357`  
		Last Modified: Tue, 19 Apr 2022 18:19:18 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71f868b0b44531e50958ac6c35c161df79228938ab68d4cc7f2b5ddb6384bbd6`  
		Last Modified: Tue, 19 Apr 2022 18:19:18 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d1bd238023271362f8a5a1136b0e5dc705f18688f793dfd34788834dcfbaf32`  
		Last Modified: Tue, 19 Apr 2022 18:19:16 GMT  
		Size: 359.5 KB (359505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0216f3dd53c339c5889dc7bf0dcdcc98ff1b6841b330934f5b991fff52f4574`  
		Last Modified: Tue, 19 Apr 2022 18:19:24 GMT  
		Size: 7.6 MB (7608996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9a52e26f86cff8b968456c51fce3ae5ddb74a9f265da6aec6c4c0104be544b8`  
		Last Modified: Tue, 19 Apr 2022 18:19:16 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4d63ac7f4ccd54465f51b2b43d349150f3ab34b0e60ccc8a22fb65b0bbe1b76`  
		Last Modified: Tue, 19 Apr 2022 18:19:15 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7b91f9f9d8dda9458f9dea3b30fd662ae28ec4bb3bdf3d98f9ccfc1a9be475f`  
		Last Modified: Tue, 19 Apr 2022 18:19:16 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.24.4`

```console
$ docker pull nats-streaming@sha256:a8d0b16eaeeb2b6cb4647f942d5a178b7e44d5709388c86fa1357239cf14ea1e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.2803; amd64

### `nats-streaming:0.24.4` - linux; amd64

```console
$ docker pull nats-streaming@sha256:3ff22408a43de2d67d38aa689b7fede88f92a6e02e9b746402c51441f22a80bd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7160576 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1be4ca5ff457718dd135cac991a2fce8902861901e8f1c7c86e614d68589dced`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 19 Apr 2022 18:19:58 GMT
COPY file:3a9e1a664fc216f321851b3ca6ab92594e42c425862d179ee6a292b590bfe37b in /nats-streaming-server 
# Tue, 19 Apr 2022 18:19:58 GMT
EXPOSE 4222 8222
# Tue, 19 Apr 2022 18:19:58 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 19 Apr 2022 18:19:58 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:f7464e210e47808da4af767838d0a84dada171f8ad1dce32071319a05d071a20`  
		Last Modified: Tue, 19 Apr 2022 18:20:40 GMT  
		Size: 7.2 MB (7160576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.24.4` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:afa50deb7af027ad2d1a54f53febadf28e189be0adb82039ea429ce57e1d590c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.7 MB (6666873 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:04f3328d94b185bf70d0866dfa2cb72566e7260e4704cfb2cfef87998649aebd`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 19 Apr 2022 18:49:58 GMT
COPY file:6b8eedac2a0774aea5449501f9ae8c79e7be3d3e55863b7703b427f601cbdd4d in /nats-streaming-server 
# Tue, 19 Apr 2022 18:49:58 GMT
EXPOSE 4222 8222
# Tue, 19 Apr 2022 18:49:59 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 19 Apr 2022 18:49:59 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:dbf88d448d58aea59c794a9388b56a7fe82335bef22b8200658329645f9b783a`  
		Last Modified: Tue, 19 Apr 2022 18:51:59 GMT  
		Size: 6.7 MB (6666873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.24.4` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:e8e52a390d9cefe82a9f17a19e2e05c49d4c56a27b05fb956108c047d5a93b31
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.7 MB (6657656 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:42f1e8f63244361974ea334f20240f6d4f94fc96d7e89051e0769eece666b959`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 19 Apr 2022 18:58:20 GMT
COPY file:17bb63ff84cf537d44fe2a6c3b62b7c20b07b7ddd09ec3e118a9ee70593166c5 in /nats-streaming-server 
# Tue, 19 Apr 2022 18:58:20 GMT
EXPOSE 4222 8222
# Tue, 19 Apr 2022 18:58:21 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 19 Apr 2022 18:58:21 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:501cd5abe17e56e7e4b1c9fb82796e05c14f6dcbf6e964d8c37a33da0eb82757`  
		Last Modified: Tue, 19 Apr 2022 19:00:12 GMT  
		Size: 6.7 MB (6657656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.24.4` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:e0dc96baa5b7e5dda328b37aa3b8b0c7a8181a6c2b1d987de42b4e5a4fb9398b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6577779 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:274efdfafa30ae2eb7eaaf98eb985e537ddf89be65804d4fdcd414d900365792`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 19 Apr 2022 18:40:21 GMT
COPY file:72420de7c1c1682a55d493d3d9f792d57edc400b24e51ea6987297cc55493b40 in /nats-streaming-server 
# Tue, 19 Apr 2022 18:40:21 GMT
EXPOSE 4222 8222
# Tue, 19 Apr 2022 18:40:22 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 19 Apr 2022 18:40:23 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4a8d243c291d90e3cac092a5d52ec5fe51c7d35bfc569928db3dda38febf3171`  
		Last Modified: Tue, 19 Apr 2022 18:41:22 GMT  
		Size: 6.6 MB (6577779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.24.4` - windows version 10.0.17763.2803; amd64

```console
$ docker pull nats-streaming@sha256:f7dcabdb7e29722bc9a94ca7545627fb80bceee30902037d345e7ad3ccdc25e4
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.4 MB (110372947 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db815bd2a9cad87072f5c232a6fd4f15c055cfdb61f213ce993afc03a96acb4d`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 04 Apr 2022 10:52:49 GMT
RUN Apply image 1809-amd64
# Wed, 13 Apr 2022 14:45:42 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Tue, 19 Apr 2022 18:18:45 GMT
RUN cmd /S /C #(nop) COPY file:ca12266791259eaa127475f881c8435e255693982581b95714c2329c1c0c3517 in C:\nats-streaming-server.exe 
# Tue, 19 Apr 2022 18:18:46 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Tue, 19 Apr 2022 18:18:47 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Tue, 19 Apr 2022 18:18:48 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:6fc97003d8b7f593fe071cf3ea64f3ce760cc060f3402bb6b1b849c040e222d5`  
		Size: 103.1 MB (103096169 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a6063f744e542c21ce471bdd7ff0dd6063d8d2a9670afbbc64d086813afd6385`  
		Last Modified: Wed, 13 Apr 2022 14:46:35 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9411ac6dc5ee77971f18c4586ba71147422eec4ca4d30dcc320376336f320e5`  
		Last Modified: Tue, 19 Apr 2022 18:19:44 GMT  
		Size: 7.3 MB (7272107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ba1c750731efcee6ebf143a7cf297c1846074c73db7022f94ebdf9ecab5843e`  
		Last Modified: Tue, 19 Apr 2022 18:19:36 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5e494cba0579a95caf948aed68f7f18e8c554774b11313fc73801906d60cba9`  
		Last Modified: Tue, 19 Apr 2022 18:19:36 GMT  
		Size: 1.2 KB (1192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d745e14762b2ee17a49256c2b5940e11f97dc7c944ef9127faa8ae713bcf9d34`  
		Last Modified: Tue, 19 Apr 2022 18:19:36 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.24.4-alpine`

```console
$ docker pull nats-streaming@sha256:4afc203c1b06db771f04248b810082a998d82540b7962f4f318b760b94918c4c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.24.4-alpine` - linux; amd64

```console
$ docker pull nats-streaming@sha256:4eb3d3f7784016d57166fb89356a963be2b929bbce0639c40efd6a48dfbeab50
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.2 MB (10248491 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0fa2e30f307c690778bcda9368b96aebbd4007db005d6d8d57416bf9f7d93381`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Tue, 05 Apr 2022 00:19:59 GMT
ADD file:5d673d25da3a14ce1f6cf66e4c7fd4f4b85a3759a9d93efb3fd9ff852b5b56e4 in / 
# Tue, 05 Apr 2022 00:19:59 GMT
CMD ["/bin/sh"]
# Tue, 19 Apr 2022 18:19:47 GMT
ENV NATS_STREAMING_SERVER=0.24.4
# Tue, 19 Apr 2022 18:19:49 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='abf61454846309f4350a209aa86d8def4ceefaa35b576fe027915f31eeaaebf6' ;; 		armhf) natsArch='arm6'; sha256='bc6efafbf051b8bbabe868240ffa9f88a5676727e3c6a5ffc13542ebd0d6585c' ;; 		armv7) natsArch='arm7'; sha256='7950f6ea4b5385454350c8979d6062aa710400a2d21a3a44d971e8535d944545' ;; 		x86_64) natsArch='amd64'; sha256='e7b1db559c02d123d0aabdf0d3a93803eb0778aa733a26ec9067c833bd5728b9' ;; 		x86) natsArch='386'; sha256='941a7be15b8f3d2ba18508baaced39884b1ed86214c2afb2c2bcfcfad3743903' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Tue, 19 Apr 2022 18:19:50 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Tue, 19 Apr 2022 18:19:50 GMT
EXPOSE 4222 8222
# Tue, 19 Apr 2022 18:19:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 19 Apr 2022 18:19:50 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:df9b9388f04ad6279a7410b85cedfdcb2208c0a003da7ab5613af71079148139`  
		Last Modified: Mon, 04 Apr 2022 19:10:16 GMT  
		Size: 2.8 MB (2814559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:618bc609c0fe2d2c7dce4a5a08dcb487ee273dfab15895d917e4f5c2425e54de`  
		Last Modified: Tue, 19 Apr 2022 18:20:20 GMT  
		Size: 7.4 MB (7433512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78cdc64ae36d5c3024c2af60810ec1bfff47708a2492efc85d7f5bfecf7abcfe`  
		Last Modified: Tue, 19 Apr 2022 18:20:16 GMT  
		Size: 420.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.24.4-alpine` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:092009bcc3beed0c4e6dd0b2e36eb45082919a3cf6178ac42576e7599efefb26
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.6 MB (9562443 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6edad2d6e424051bf23151c9f0b88c0a1ae0f02e7ca579630d5f54da30fb8e69`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Mon, 04 Apr 2022 23:49:42 GMT
ADD file:159dcddaab900372df882a4e94615ed84250e9cea3e74bc0479d98280342f596 in / 
# Mon, 04 Apr 2022 23:49:42 GMT
CMD ["/bin/sh"]
# Tue, 19 Apr 2022 18:49:33 GMT
ENV NATS_STREAMING_SERVER=0.24.4
# Tue, 19 Apr 2022 18:49:37 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='abf61454846309f4350a209aa86d8def4ceefaa35b576fe027915f31eeaaebf6' ;; 		armhf) natsArch='arm6'; sha256='bc6efafbf051b8bbabe868240ffa9f88a5676727e3c6a5ffc13542ebd0d6585c' ;; 		armv7) natsArch='arm7'; sha256='7950f6ea4b5385454350c8979d6062aa710400a2d21a3a44d971e8535d944545' ;; 		x86_64) natsArch='amd64'; sha256='e7b1db559c02d123d0aabdf0d3a93803eb0778aa733a26ec9067c833bd5728b9' ;; 		x86) natsArch='386'; sha256='941a7be15b8f3d2ba18508baaced39884b1ed86214c2afb2c2bcfcfad3743903' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Tue, 19 Apr 2022 18:49:38 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Tue, 19 Apr 2022 18:49:38 GMT
EXPOSE 4222 8222
# Tue, 19 Apr 2022 18:49:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 19 Apr 2022 18:49:39 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:c319b1fc4ed70b8241a7ce6ac0c4015d354bf5cf8c01eb73c50b6709c0c46e49`  
		Last Modified: Mon, 04 Apr 2022 19:09:22 GMT  
		Size: 2.6 MB (2621972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7749efc5f39c770d1ec4c0ef3a405656aa5e1993fbdacd7d21f3d4707ff1a72c`  
		Last Modified: Tue, 19 Apr 2022 18:51:22 GMT  
		Size: 6.9 MB (6940049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a23a7c4070e79cc4538b1305be5da3a4b615da587a7fd569a0be26bd110fa84`  
		Last Modified: Tue, 19 Apr 2022 18:51:18 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.24.4-alpine` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:43fa0020bbe495315ac2f09debe4bf6b27dd74790d26ac3366750c3055e58a3c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.4 MB (9354606 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4afe09639533164664c235319932921bedc9450ecd3de243641a70c7a583c5d1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Mon, 04 Apr 2022 23:57:34 GMT
ADD file:20f8cdddc53a4a8bd78945fc32fe08e9f80ab3b16dc20a9aa4ba73b79f2bc71c in / 
# Mon, 04 Apr 2022 23:57:35 GMT
CMD ["/bin/sh"]
# Tue, 19 Apr 2022 18:57:51 GMT
ENV NATS_STREAMING_SERVER=0.24.4
# Tue, 19 Apr 2022 18:57:55 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='abf61454846309f4350a209aa86d8def4ceefaa35b576fe027915f31eeaaebf6' ;; 		armhf) natsArch='arm6'; sha256='bc6efafbf051b8bbabe868240ffa9f88a5676727e3c6a5ffc13542ebd0d6585c' ;; 		armv7) natsArch='arm7'; sha256='7950f6ea4b5385454350c8979d6062aa710400a2d21a3a44d971e8535d944545' ;; 		x86_64) natsArch='amd64'; sha256='e7b1db559c02d123d0aabdf0d3a93803eb0778aa733a26ec9067c833bd5728b9' ;; 		x86) natsArch='386'; sha256='941a7be15b8f3d2ba18508baaced39884b1ed86214c2afb2c2bcfcfad3743903' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Tue, 19 Apr 2022 18:57:56 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Tue, 19 Apr 2022 18:57:56 GMT
EXPOSE 4222 8222
# Tue, 19 Apr 2022 18:57:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 19 Apr 2022 18:57:57 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:57fb4b5f1a47c953ca5703f0f81ce14e5d01cf23aa79558b5adb961cc526e320`  
		Last Modified: Mon, 04 Apr 2022 19:09:36 GMT  
		Size: 2.4 MB (2424323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cab0ba64de7ddcb969882eb8b609a89179c2d441a4bcc7317ae977fd7dda4e23`  
		Last Modified: Tue, 19 Apr 2022 18:59:41 GMT  
		Size: 6.9 MB (6929861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27e7fde7215edaedba408f2d6f77c7043df6c84d3309cffeb7f8b14f1c0b82c0`  
		Last Modified: Tue, 19 Apr 2022 18:59:37 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.24.4-alpine` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:bef1eb9f86f148797e14e6dd500934864bd8611f0256715a932c286bbedbddb4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.6 MB (9567309 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89a27b9fd024c9823aa8be1c38baede9477c1bf1ab37ddbec1c6d01c2a3a658a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:31 GMT
ADD file:90e56af13188c7f0283d244a0d70b853d8bef8587a41f1da8eac3a2aba8964ef in / 
# Mon, 04 Apr 2022 23:39:31 GMT
CMD ["/bin/sh"]
# Tue, 19 Apr 2022 18:40:04 GMT
ENV NATS_STREAMING_SERVER=0.24.4
# Tue, 19 Apr 2022 18:40:07 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='abf61454846309f4350a209aa86d8def4ceefaa35b576fe027915f31eeaaebf6' ;; 		armhf) natsArch='arm6'; sha256='bc6efafbf051b8bbabe868240ffa9f88a5676727e3c6a5ffc13542ebd0d6585c' ;; 		armv7) natsArch='arm7'; sha256='7950f6ea4b5385454350c8979d6062aa710400a2d21a3a44d971e8535d944545' ;; 		x86_64) natsArch='amd64'; sha256='e7b1db559c02d123d0aabdf0d3a93803eb0778aa733a26ec9067c833bd5728b9' ;; 		x86) natsArch='386'; sha256='941a7be15b8f3d2ba18508baaced39884b1ed86214c2afb2c2bcfcfad3743903' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Tue, 19 Apr 2022 18:40:09 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Tue, 19 Apr 2022 18:40:09 GMT
EXPOSE 4222 8222
# Tue, 19 Apr 2022 18:40:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 19 Apr 2022 18:40:11 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:9981e73032c8833e387a8f96986e560edbed12c38119e0edb0439c9c2234eac9`  
		Last Modified: Mon, 04 Apr 2022 19:09:10 GMT  
		Size: 2.7 MB (2716477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0812492999c8bb5bc4d5d0f3cf25e7e1a474b07e1400c864e6f714d6c9771fb1`  
		Last Modified: Tue, 19 Apr 2022 18:40:59 GMT  
		Size: 6.9 MB (6850411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0aedb2f212694a12d2b97ef1d1079ba39d77f30b8574a79cc0421d472c6dfae`  
		Last Modified: Tue, 19 Apr 2022 18:40:58 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.24.4-alpine3.15`

```console
$ docker pull nats-streaming@sha256:4afc203c1b06db771f04248b810082a998d82540b7962f4f318b760b94918c4c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.24.4-alpine3.15` - linux; amd64

```console
$ docker pull nats-streaming@sha256:4eb3d3f7784016d57166fb89356a963be2b929bbce0639c40efd6a48dfbeab50
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.2 MB (10248491 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0fa2e30f307c690778bcda9368b96aebbd4007db005d6d8d57416bf9f7d93381`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Tue, 05 Apr 2022 00:19:59 GMT
ADD file:5d673d25da3a14ce1f6cf66e4c7fd4f4b85a3759a9d93efb3fd9ff852b5b56e4 in / 
# Tue, 05 Apr 2022 00:19:59 GMT
CMD ["/bin/sh"]
# Tue, 19 Apr 2022 18:19:47 GMT
ENV NATS_STREAMING_SERVER=0.24.4
# Tue, 19 Apr 2022 18:19:49 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='abf61454846309f4350a209aa86d8def4ceefaa35b576fe027915f31eeaaebf6' ;; 		armhf) natsArch='arm6'; sha256='bc6efafbf051b8bbabe868240ffa9f88a5676727e3c6a5ffc13542ebd0d6585c' ;; 		armv7) natsArch='arm7'; sha256='7950f6ea4b5385454350c8979d6062aa710400a2d21a3a44d971e8535d944545' ;; 		x86_64) natsArch='amd64'; sha256='e7b1db559c02d123d0aabdf0d3a93803eb0778aa733a26ec9067c833bd5728b9' ;; 		x86) natsArch='386'; sha256='941a7be15b8f3d2ba18508baaced39884b1ed86214c2afb2c2bcfcfad3743903' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Tue, 19 Apr 2022 18:19:50 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Tue, 19 Apr 2022 18:19:50 GMT
EXPOSE 4222 8222
# Tue, 19 Apr 2022 18:19:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 19 Apr 2022 18:19:50 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:df9b9388f04ad6279a7410b85cedfdcb2208c0a003da7ab5613af71079148139`  
		Last Modified: Mon, 04 Apr 2022 19:10:16 GMT  
		Size: 2.8 MB (2814559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:618bc609c0fe2d2c7dce4a5a08dcb487ee273dfab15895d917e4f5c2425e54de`  
		Last Modified: Tue, 19 Apr 2022 18:20:20 GMT  
		Size: 7.4 MB (7433512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78cdc64ae36d5c3024c2af60810ec1bfff47708a2492efc85d7f5bfecf7abcfe`  
		Last Modified: Tue, 19 Apr 2022 18:20:16 GMT  
		Size: 420.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.24.4-alpine3.15` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:092009bcc3beed0c4e6dd0b2e36eb45082919a3cf6178ac42576e7599efefb26
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.6 MB (9562443 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6edad2d6e424051bf23151c9f0b88c0a1ae0f02e7ca579630d5f54da30fb8e69`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Mon, 04 Apr 2022 23:49:42 GMT
ADD file:159dcddaab900372df882a4e94615ed84250e9cea3e74bc0479d98280342f596 in / 
# Mon, 04 Apr 2022 23:49:42 GMT
CMD ["/bin/sh"]
# Tue, 19 Apr 2022 18:49:33 GMT
ENV NATS_STREAMING_SERVER=0.24.4
# Tue, 19 Apr 2022 18:49:37 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='abf61454846309f4350a209aa86d8def4ceefaa35b576fe027915f31eeaaebf6' ;; 		armhf) natsArch='arm6'; sha256='bc6efafbf051b8bbabe868240ffa9f88a5676727e3c6a5ffc13542ebd0d6585c' ;; 		armv7) natsArch='arm7'; sha256='7950f6ea4b5385454350c8979d6062aa710400a2d21a3a44d971e8535d944545' ;; 		x86_64) natsArch='amd64'; sha256='e7b1db559c02d123d0aabdf0d3a93803eb0778aa733a26ec9067c833bd5728b9' ;; 		x86) natsArch='386'; sha256='941a7be15b8f3d2ba18508baaced39884b1ed86214c2afb2c2bcfcfad3743903' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Tue, 19 Apr 2022 18:49:38 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Tue, 19 Apr 2022 18:49:38 GMT
EXPOSE 4222 8222
# Tue, 19 Apr 2022 18:49:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 19 Apr 2022 18:49:39 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:c319b1fc4ed70b8241a7ce6ac0c4015d354bf5cf8c01eb73c50b6709c0c46e49`  
		Last Modified: Mon, 04 Apr 2022 19:09:22 GMT  
		Size: 2.6 MB (2621972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7749efc5f39c770d1ec4c0ef3a405656aa5e1993fbdacd7d21f3d4707ff1a72c`  
		Last Modified: Tue, 19 Apr 2022 18:51:22 GMT  
		Size: 6.9 MB (6940049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a23a7c4070e79cc4538b1305be5da3a4b615da587a7fd569a0be26bd110fa84`  
		Last Modified: Tue, 19 Apr 2022 18:51:18 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.24.4-alpine3.15` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:43fa0020bbe495315ac2f09debe4bf6b27dd74790d26ac3366750c3055e58a3c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.4 MB (9354606 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4afe09639533164664c235319932921bedc9450ecd3de243641a70c7a583c5d1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Mon, 04 Apr 2022 23:57:34 GMT
ADD file:20f8cdddc53a4a8bd78945fc32fe08e9f80ab3b16dc20a9aa4ba73b79f2bc71c in / 
# Mon, 04 Apr 2022 23:57:35 GMT
CMD ["/bin/sh"]
# Tue, 19 Apr 2022 18:57:51 GMT
ENV NATS_STREAMING_SERVER=0.24.4
# Tue, 19 Apr 2022 18:57:55 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='abf61454846309f4350a209aa86d8def4ceefaa35b576fe027915f31eeaaebf6' ;; 		armhf) natsArch='arm6'; sha256='bc6efafbf051b8bbabe868240ffa9f88a5676727e3c6a5ffc13542ebd0d6585c' ;; 		armv7) natsArch='arm7'; sha256='7950f6ea4b5385454350c8979d6062aa710400a2d21a3a44d971e8535d944545' ;; 		x86_64) natsArch='amd64'; sha256='e7b1db559c02d123d0aabdf0d3a93803eb0778aa733a26ec9067c833bd5728b9' ;; 		x86) natsArch='386'; sha256='941a7be15b8f3d2ba18508baaced39884b1ed86214c2afb2c2bcfcfad3743903' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Tue, 19 Apr 2022 18:57:56 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Tue, 19 Apr 2022 18:57:56 GMT
EXPOSE 4222 8222
# Tue, 19 Apr 2022 18:57:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 19 Apr 2022 18:57:57 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:57fb4b5f1a47c953ca5703f0f81ce14e5d01cf23aa79558b5adb961cc526e320`  
		Last Modified: Mon, 04 Apr 2022 19:09:36 GMT  
		Size: 2.4 MB (2424323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cab0ba64de7ddcb969882eb8b609a89179c2d441a4bcc7317ae977fd7dda4e23`  
		Last Modified: Tue, 19 Apr 2022 18:59:41 GMT  
		Size: 6.9 MB (6929861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27e7fde7215edaedba408f2d6f77c7043df6c84d3309cffeb7f8b14f1c0b82c0`  
		Last Modified: Tue, 19 Apr 2022 18:59:37 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.24.4-alpine3.15` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:bef1eb9f86f148797e14e6dd500934864bd8611f0256715a932c286bbedbddb4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.6 MB (9567309 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89a27b9fd024c9823aa8be1c38baede9477c1bf1ab37ddbec1c6d01c2a3a658a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:31 GMT
ADD file:90e56af13188c7f0283d244a0d70b853d8bef8587a41f1da8eac3a2aba8964ef in / 
# Mon, 04 Apr 2022 23:39:31 GMT
CMD ["/bin/sh"]
# Tue, 19 Apr 2022 18:40:04 GMT
ENV NATS_STREAMING_SERVER=0.24.4
# Tue, 19 Apr 2022 18:40:07 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='abf61454846309f4350a209aa86d8def4ceefaa35b576fe027915f31eeaaebf6' ;; 		armhf) natsArch='arm6'; sha256='bc6efafbf051b8bbabe868240ffa9f88a5676727e3c6a5ffc13542ebd0d6585c' ;; 		armv7) natsArch='arm7'; sha256='7950f6ea4b5385454350c8979d6062aa710400a2d21a3a44d971e8535d944545' ;; 		x86_64) natsArch='amd64'; sha256='e7b1db559c02d123d0aabdf0d3a93803eb0778aa733a26ec9067c833bd5728b9' ;; 		x86) natsArch='386'; sha256='941a7be15b8f3d2ba18508baaced39884b1ed86214c2afb2c2bcfcfad3743903' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Tue, 19 Apr 2022 18:40:09 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Tue, 19 Apr 2022 18:40:09 GMT
EXPOSE 4222 8222
# Tue, 19 Apr 2022 18:40:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 19 Apr 2022 18:40:11 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:9981e73032c8833e387a8f96986e560edbed12c38119e0edb0439c9c2234eac9`  
		Last Modified: Mon, 04 Apr 2022 19:09:10 GMT  
		Size: 2.7 MB (2716477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0812492999c8bb5bc4d5d0f3cf25e7e1a474b07e1400c864e6f714d6c9771fb1`  
		Last Modified: Tue, 19 Apr 2022 18:40:59 GMT  
		Size: 6.9 MB (6850411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0aedb2f212694a12d2b97ef1d1079ba39d77f30b8574a79cc0421d472c6dfae`  
		Last Modified: Tue, 19 Apr 2022 18:40:58 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.24.4-linux`

```console
$ docker pull nats-streaming@sha256:bf7595fa0e1871058be97fa42b8155f796e95f2582fb2141a11f4a51cdff18e9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.24.4-linux` - linux; amd64

```console
$ docker pull nats-streaming@sha256:3ff22408a43de2d67d38aa689b7fede88f92a6e02e9b746402c51441f22a80bd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7160576 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1be4ca5ff457718dd135cac991a2fce8902861901e8f1c7c86e614d68589dced`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 19 Apr 2022 18:19:58 GMT
COPY file:3a9e1a664fc216f321851b3ca6ab92594e42c425862d179ee6a292b590bfe37b in /nats-streaming-server 
# Tue, 19 Apr 2022 18:19:58 GMT
EXPOSE 4222 8222
# Tue, 19 Apr 2022 18:19:58 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 19 Apr 2022 18:19:58 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:f7464e210e47808da4af767838d0a84dada171f8ad1dce32071319a05d071a20`  
		Last Modified: Tue, 19 Apr 2022 18:20:40 GMT  
		Size: 7.2 MB (7160576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.24.4-linux` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:afa50deb7af027ad2d1a54f53febadf28e189be0adb82039ea429ce57e1d590c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.7 MB (6666873 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:04f3328d94b185bf70d0866dfa2cb72566e7260e4704cfb2cfef87998649aebd`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 19 Apr 2022 18:49:58 GMT
COPY file:6b8eedac2a0774aea5449501f9ae8c79e7be3d3e55863b7703b427f601cbdd4d in /nats-streaming-server 
# Tue, 19 Apr 2022 18:49:58 GMT
EXPOSE 4222 8222
# Tue, 19 Apr 2022 18:49:59 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 19 Apr 2022 18:49:59 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:dbf88d448d58aea59c794a9388b56a7fe82335bef22b8200658329645f9b783a`  
		Last Modified: Tue, 19 Apr 2022 18:51:59 GMT  
		Size: 6.7 MB (6666873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.24.4-linux` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:e8e52a390d9cefe82a9f17a19e2e05c49d4c56a27b05fb956108c047d5a93b31
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.7 MB (6657656 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:42f1e8f63244361974ea334f20240f6d4f94fc96d7e89051e0769eece666b959`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 19 Apr 2022 18:58:20 GMT
COPY file:17bb63ff84cf537d44fe2a6c3b62b7c20b07b7ddd09ec3e118a9ee70593166c5 in /nats-streaming-server 
# Tue, 19 Apr 2022 18:58:20 GMT
EXPOSE 4222 8222
# Tue, 19 Apr 2022 18:58:21 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 19 Apr 2022 18:58:21 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:501cd5abe17e56e7e4b1c9fb82796e05c14f6dcbf6e964d8c37a33da0eb82757`  
		Last Modified: Tue, 19 Apr 2022 19:00:12 GMT  
		Size: 6.7 MB (6657656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.24.4-linux` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:e0dc96baa5b7e5dda328b37aa3b8b0c7a8181a6c2b1d987de42b4e5a4fb9398b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6577779 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:274efdfafa30ae2eb7eaaf98eb985e537ddf89be65804d4fdcd414d900365792`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 19 Apr 2022 18:40:21 GMT
COPY file:72420de7c1c1682a55d493d3d9f792d57edc400b24e51ea6987297cc55493b40 in /nats-streaming-server 
# Tue, 19 Apr 2022 18:40:21 GMT
EXPOSE 4222 8222
# Tue, 19 Apr 2022 18:40:22 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 19 Apr 2022 18:40:23 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4a8d243c291d90e3cac092a5d52ec5fe51c7d35bfc569928db3dda38febf3171`  
		Last Modified: Tue, 19 Apr 2022 18:41:22 GMT  
		Size: 6.6 MB (6577779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.24.4-nanoserver`

```console
$ docker pull nats-streaming@sha256:5f0fd8d176c73f6fd991c80241c4d8ad94259cff1ea5994dae8aea7b99d35a67
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2803; amd64

### `nats-streaming:0.24.4-nanoserver` - windows version 10.0.17763.2803; amd64

```console
$ docker pull nats-streaming@sha256:f7dcabdb7e29722bc9a94ca7545627fb80bceee30902037d345e7ad3ccdc25e4
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.4 MB (110372947 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db815bd2a9cad87072f5c232a6fd4f15c055cfdb61f213ce993afc03a96acb4d`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 04 Apr 2022 10:52:49 GMT
RUN Apply image 1809-amd64
# Wed, 13 Apr 2022 14:45:42 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Tue, 19 Apr 2022 18:18:45 GMT
RUN cmd /S /C #(nop) COPY file:ca12266791259eaa127475f881c8435e255693982581b95714c2329c1c0c3517 in C:\nats-streaming-server.exe 
# Tue, 19 Apr 2022 18:18:46 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Tue, 19 Apr 2022 18:18:47 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Tue, 19 Apr 2022 18:18:48 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:6fc97003d8b7f593fe071cf3ea64f3ce760cc060f3402bb6b1b849c040e222d5`  
		Size: 103.1 MB (103096169 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a6063f744e542c21ce471bdd7ff0dd6063d8d2a9670afbbc64d086813afd6385`  
		Last Modified: Wed, 13 Apr 2022 14:46:35 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9411ac6dc5ee77971f18c4586ba71147422eec4ca4d30dcc320376336f320e5`  
		Last Modified: Tue, 19 Apr 2022 18:19:44 GMT  
		Size: 7.3 MB (7272107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ba1c750731efcee6ebf143a7cf297c1846074c73db7022f94ebdf9ecab5843e`  
		Last Modified: Tue, 19 Apr 2022 18:19:36 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5e494cba0579a95caf948aed68f7f18e8c554774b11313fc73801906d60cba9`  
		Last Modified: Tue, 19 Apr 2022 18:19:36 GMT  
		Size: 1.2 KB (1192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d745e14762b2ee17a49256c2b5940e11f97dc7c944ef9127faa8ae713bcf9d34`  
		Last Modified: Tue, 19 Apr 2022 18:19:36 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.24.4-nanoserver-1809`

```console
$ docker pull nats-streaming@sha256:5f0fd8d176c73f6fd991c80241c4d8ad94259cff1ea5994dae8aea7b99d35a67
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2803; amd64

### `nats-streaming:0.24.4-nanoserver-1809` - windows version 10.0.17763.2803; amd64

```console
$ docker pull nats-streaming@sha256:f7dcabdb7e29722bc9a94ca7545627fb80bceee30902037d345e7ad3ccdc25e4
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.4 MB (110372947 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db815bd2a9cad87072f5c232a6fd4f15c055cfdb61f213ce993afc03a96acb4d`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 04 Apr 2022 10:52:49 GMT
RUN Apply image 1809-amd64
# Wed, 13 Apr 2022 14:45:42 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Tue, 19 Apr 2022 18:18:45 GMT
RUN cmd /S /C #(nop) COPY file:ca12266791259eaa127475f881c8435e255693982581b95714c2329c1c0c3517 in C:\nats-streaming-server.exe 
# Tue, 19 Apr 2022 18:18:46 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Tue, 19 Apr 2022 18:18:47 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Tue, 19 Apr 2022 18:18:48 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:6fc97003d8b7f593fe071cf3ea64f3ce760cc060f3402bb6b1b849c040e222d5`  
		Size: 103.1 MB (103096169 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a6063f744e542c21ce471bdd7ff0dd6063d8d2a9670afbbc64d086813afd6385`  
		Last Modified: Wed, 13 Apr 2022 14:46:35 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9411ac6dc5ee77971f18c4586ba71147422eec4ca4d30dcc320376336f320e5`  
		Last Modified: Tue, 19 Apr 2022 18:19:44 GMT  
		Size: 7.3 MB (7272107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ba1c750731efcee6ebf143a7cf297c1846074c73db7022f94ebdf9ecab5843e`  
		Last Modified: Tue, 19 Apr 2022 18:19:36 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5e494cba0579a95caf948aed68f7f18e8c554774b11313fc73801906d60cba9`  
		Last Modified: Tue, 19 Apr 2022 18:19:36 GMT  
		Size: 1.2 KB (1192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d745e14762b2ee17a49256c2b5940e11f97dc7c944ef9127faa8ae713bcf9d34`  
		Last Modified: Tue, 19 Apr 2022 18:19:36 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.24.4-scratch`

```console
$ docker pull nats-streaming@sha256:bf7595fa0e1871058be97fa42b8155f796e95f2582fb2141a11f4a51cdff18e9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.24.4-scratch` - linux; amd64

```console
$ docker pull nats-streaming@sha256:3ff22408a43de2d67d38aa689b7fede88f92a6e02e9b746402c51441f22a80bd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7160576 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1be4ca5ff457718dd135cac991a2fce8902861901e8f1c7c86e614d68589dced`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 19 Apr 2022 18:19:58 GMT
COPY file:3a9e1a664fc216f321851b3ca6ab92594e42c425862d179ee6a292b590bfe37b in /nats-streaming-server 
# Tue, 19 Apr 2022 18:19:58 GMT
EXPOSE 4222 8222
# Tue, 19 Apr 2022 18:19:58 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 19 Apr 2022 18:19:58 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:f7464e210e47808da4af767838d0a84dada171f8ad1dce32071319a05d071a20`  
		Last Modified: Tue, 19 Apr 2022 18:20:40 GMT  
		Size: 7.2 MB (7160576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.24.4-scratch` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:afa50deb7af027ad2d1a54f53febadf28e189be0adb82039ea429ce57e1d590c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.7 MB (6666873 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:04f3328d94b185bf70d0866dfa2cb72566e7260e4704cfb2cfef87998649aebd`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 19 Apr 2022 18:49:58 GMT
COPY file:6b8eedac2a0774aea5449501f9ae8c79e7be3d3e55863b7703b427f601cbdd4d in /nats-streaming-server 
# Tue, 19 Apr 2022 18:49:58 GMT
EXPOSE 4222 8222
# Tue, 19 Apr 2022 18:49:59 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 19 Apr 2022 18:49:59 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:dbf88d448d58aea59c794a9388b56a7fe82335bef22b8200658329645f9b783a`  
		Last Modified: Tue, 19 Apr 2022 18:51:59 GMT  
		Size: 6.7 MB (6666873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.24.4-scratch` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:e8e52a390d9cefe82a9f17a19e2e05c49d4c56a27b05fb956108c047d5a93b31
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.7 MB (6657656 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:42f1e8f63244361974ea334f20240f6d4f94fc96d7e89051e0769eece666b959`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 19 Apr 2022 18:58:20 GMT
COPY file:17bb63ff84cf537d44fe2a6c3b62b7c20b07b7ddd09ec3e118a9ee70593166c5 in /nats-streaming-server 
# Tue, 19 Apr 2022 18:58:20 GMT
EXPOSE 4222 8222
# Tue, 19 Apr 2022 18:58:21 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 19 Apr 2022 18:58:21 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:501cd5abe17e56e7e4b1c9fb82796e05c14f6dcbf6e964d8c37a33da0eb82757`  
		Last Modified: Tue, 19 Apr 2022 19:00:12 GMT  
		Size: 6.7 MB (6657656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.24.4-scratch` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:e0dc96baa5b7e5dda328b37aa3b8b0c7a8181a6c2b1d987de42b4e5a4fb9398b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6577779 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:274efdfafa30ae2eb7eaaf98eb985e537ddf89be65804d4fdcd414d900365792`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 19 Apr 2022 18:40:21 GMT
COPY file:72420de7c1c1682a55d493d3d9f792d57edc400b24e51ea6987297cc55493b40 in /nats-streaming-server 
# Tue, 19 Apr 2022 18:40:21 GMT
EXPOSE 4222 8222
# Tue, 19 Apr 2022 18:40:22 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 19 Apr 2022 18:40:23 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4a8d243c291d90e3cac092a5d52ec5fe51c7d35bfc569928db3dda38febf3171`  
		Last Modified: Tue, 19 Apr 2022 18:41:22 GMT  
		Size: 6.6 MB (6577779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.24.4-windowsservercore`

```console
$ docker pull nats-streaming@sha256:86c23aeb014348875713589438ea483f5d1f8c2c81a6dae1437392934b1792ef
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2803; amd64

### `nats-streaming:0.24.4-windowsservercore` - windows version 10.0.17763.2803; amd64

```console
$ docker pull nats-streaming@sha256:72f0e5b61606638041efba42873ea1291d8b05d973accd3fa4fb8d87a81dcb5f
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2723900130 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b04dd0632cb73bbae0011b92981b880cef224abb6cb100902b20f342efce7de6`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 04 Apr 2022 11:20:25 GMT
RUN Install update 1809-amd64
# Wed, 13 Apr 2022 12:43:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 Apr 2022 14:42:30 GMT
ENV NATS_DOCKERIZED=1
# Tue, 19 Apr 2022 18:15:31 GMT
ENV NATS_STREAMING_SERVER=0.24.4
# Tue, 19 Apr 2022 18:15:32 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.24.4/nats-streaming-server-v0.24.4-windows-amd64.zip
# Tue, 19 Apr 2022 18:15:33 GMT
ENV NATS_STREAMING_SERVER_SHASUM=147b39fb88a9eb45c3f5692365fa6ee17d95c627bb4ecde7601f68151ace6c41
# Tue, 19 Apr 2022 18:16:48 GMT
RUN Set-PSDebug -Trace 2
# Tue, 19 Apr 2022 18:18:32 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Tue, 19 Apr 2022 18:18:33 GMT
EXPOSE 4222 8222
# Tue, 19 Apr 2022 18:18:34 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Tue, 19 Apr 2022 18:18:35 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ba8181afd4264392fbbf8df14fb4cddc55fbe085ab000e986b789678bc2bb171`  
		Size: 997.6 MB (997587446 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7ebb23aa64bff633cfa3c62b190d84f0e870b04fecb1910f65d0870b5c7f8981`  
		Last Modified: Wed, 13 Apr 2022 14:12:24 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d838c7a98a95bee63894bac798124e8c8572bcacc23e22d85332d453a03a7d7c`  
		Last Modified: Wed, 13 Apr 2022 14:46:17 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63c30d5de5c74ae8a10de14dcc644f3d8db3247159e379e97bfa4a735c0484b6`  
		Last Modified: Tue, 19 Apr 2022 18:19:18 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:611dcea795d1cfe41e1bed673aced23eeba03240c857b46e94747a9b1cddc357`  
		Last Modified: Tue, 19 Apr 2022 18:19:18 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71f868b0b44531e50958ac6c35c161df79228938ab68d4cc7f2b5ddb6384bbd6`  
		Last Modified: Tue, 19 Apr 2022 18:19:18 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d1bd238023271362f8a5a1136b0e5dc705f18688f793dfd34788834dcfbaf32`  
		Last Modified: Tue, 19 Apr 2022 18:19:16 GMT  
		Size: 359.5 KB (359505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0216f3dd53c339c5889dc7bf0dcdcc98ff1b6841b330934f5b991fff52f4574`  
		Last Modified: Tue, 19 Apr 2022 18:19:24 GMT  
		Size: 7.6 MB (7608996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9a52e26f86cff8b968456c51fce3ae5ddb74a9f265da6aec6c4c0104be544b8`  
		Last Modified: Tue, 19 Apr 2022 18:19:16 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4d63ac7f4ccd54465f51b2b43d349150f3ab34b0e60ccc8a22fb65b0bbe1b76`  
		Last Modified: Tue, 19 Apr 2022 18:19:15 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7b91f9f9d8dda9458f9dea3b30fd662ae28ec4bb3bdf3d98f9ccfc1a9be475f`  
		Last Modified: Tue, 19 Apr 2022 18:19:16 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.24.4-windowsservercore-1809`

```console
$ docker pull nats-streaming@sha256:86c23aeb014348875713589438ea483f5d1f8c2c81a6dae1437392934b1792ef
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2803; amd64

### `nats-streaming:0.24.4-windowsservercore-1809` - windows version 10.0.17763.2803; amd64

```console
$ docker pull nats-streaming@sha256:72f0e5b61606638041efba42873ea1291d8b05d973accd3fa4fb8d87a81dcb5f
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2723900130 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b04dd0632cb73bbae0011b92981b880cef224abb6cb100902b20f342efce7de6`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 04 Apr 2022 11:20:25 GMT
RUN Install update 1809-amd64
# Wed, 13 Apr 2022 12:43:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 Apr 2022 14:42:30 GMT
ENV NATS_DOCKERIZED=1
# Tue, 19 Apr 2022 18:15:31 GMT
ENV NATS_STREAMING_SERVER=0.24.4
# Tue, 19 Apr 2022 18:15:32 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.24.4/nats-streaming-server-v0.24.4-windows-amd64.zip
# Tue, 19 Apr 2022 18:15:33 GMT
ENV NATS_STREAMING_SERVER_SHASUM=147b39fb88a9eb45c3f5692365fa6ee17d95c627bb4ecde7601f68151ace6c41
# Tue, 19 Apr 2022 18:16:48 GMT
RUN Set-PSDebug -Trace 2
# Tue, 19 Apr 2022 18:18:32 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Tue, 19 Apr 2022 18:18:33 GMT
EXPOSE 4222 8222
# Tue, 19 Apr 2022 18:18:34 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Tue, 19 Apr 2022 18:18:35 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ba8181afd4264392fbbf8df14fb4cddc55fbe085ab000e986b789678bc2bb171`  
		Size: 997.6 MB (997587446 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7ebb23aa64bff633cfa3c62b190d84f0e870b04fecb1910f65d0870b5c7f8981`  
		Last Modified: Wed, 13 Apr 2022 14:12:24 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d838c7a98a95bee63894bac798124e8c8572bcacc23e22d85332d453a03a7d7c`  
		Last Modified: Wed, 13 Apr 2022 14:46:17 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63c30d5de5c74ae8a10de14dcc644f3d8db3247159e379e97bfa4a735c0484b6`  
		Last Modified: Tue, 19 Apr 2022 18:19:18 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:611dcea795d1cfe41e1bed673aced23eeba03240c857b46e94747a9b1cddc357`  
		Last Modified: Tue, 19 Apr 2022 18:19:18 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71f868b0b44531e50958ac6c35c161df79228938ab68d4cc7f2b5ddb6384bbd6`  
		Last Modified: Tue, 19 Apr 2022 18:19:18 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d1bd238023271362f8a5a1136b0e5dc705f18688f793dfd34788834dcfbaf32`  
		Last Modified: Tue, 19 Apr 2022 18:19:16 GMT  
		Size: 359.5 KB (359505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0216f3dd53c339c5889dc7bf0dcdcc98ff1b6841b330934f5b991fff52f4574`  
		Last Modified: Tue, 19 Apr 2022 18:19:24 GMT  
		Size: 7.6 MB (7608996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9a52e26f86cff8b968456c51fce3ae5ddb74a9f265da6aec6c4c0104be544b8`  
		Last Modified: Tue, 19 Apr 2022 18:19:16 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4d63ac7f4ccd54465f51b2b43d349150f3ab34b0e60ccc8a22fb65b0bbe1b76`  
		Last Modified: Tue, 19 Apr 2022 18:19:15 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7b91f9f9d8dda9458f9dea3b30fd662ae28ec4bb3bdf3d98f9ccfc1a9be475f`  
		Last Modified: Tue, 19 Apr 2022 18:19:16 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:alpine`

```console
$ docker pull nats-streaming@sha256:4afc203c1b06db771f04248b810082a998d82540b7962f4f318b760b94918c4c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:alpine` - linux; amd64

```console
$ docker pull nats-streaming@sha256:4eb3d3f7784016d57166fb89356a963be2b929bbce0639c40efd6a48dfbeab50
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.2 MB (10248491 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0fa2e30f307c690778bcda9368b96aebbd4007db005d6d8d57416bf9f7d93381`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Tue, 05 Apr 2022 00:19:59 GMT
ADD file:5d673d25da3a14ce1f6cf66e4c7fd4f4b85a3759a9d93efb3fd9ff852b5b56e4 in / 
# Tue, 05 Apr 2022 00:19:59 GMT
CMD ["/bin/sh"]
# Tue, 19 Apr 2022 18:19:47 GMT
ENV NATS_STREAMING_SERVER=0.24.4
# Tue, 19 Apr 2022 18:19:49 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='abf61454846309f4350a209aa86d8def4ceefaa35b576fe027915f31eeaaebf6' ;; 		armhf) natsArch='arm6'; sha256='bc6efafbf051b8bbabe868240ffa9f88a5676727e3c6a5ffc13542ebd0d6585c' ;; 		armv7) natsArch='arm7'; sha256='7950f6ea4b5385454350c8979d6062aa710400a2d21a3a44d971e8535d944545' ;; 		x86_64) natsArch='amd64'; sha256='e7b1db559c02d123d0aabdf0d3a93803eb0778aa733a26ec9067c833bd5728b9' ;; 		x86) natsArch='386'; sha256='941a7be15b8f3d2ba18508baaced39884b1ed86214c2afb2c2bcfcfad3743903' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Tue, 19 Apr 2022 18:19:50 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Tue, 19 Apr 2022 18:19:50 GMT
EXPOSE 4222 8222
# Tue, 19 Apr 2022 18:19:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 19 Apr 2022 18:19:50 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:df9b9388f04ad6279a7410b85cedfdcb2208c0a003da7ab5613af71079148139`  
		Last Modified: Mon, 04 Apr 2022 19:10:16 GMT  
		Size: 2.8 MB (2814559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:618bc609c0fe2d2c7dce4a5a08dcb487ee273dfab15895d917e4f5c2425e54de`  
		Last Modified: Tue, 19 Apr 2022 18:20:20 GMT  
		Size: 7.4 MB (7433512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78cdc64ae36d5c3024c2af60810ec1bfff47708a2492efc85d7f5bfecf7abcfe`  
		Last Modified: Tue, 19 Apr 2022 18:20:16 GMT  
		Size: 420.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:092009bcc3beed0c4e6dd0b2e36eb45082919a3cf6178ac42576e7599efefb26
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.6 MB (9562443 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6edad2d6e424051bf23151c9f0b88c0a1ae0f02e7ca579630d5f54da30fb8e69`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Mon, 04 Apr 2022 23:49:42 GMT
ADD file:159dcddaab900372df882a4e94615ed84250e9cea3e74bc0479d98280342f596 in / 
# Mon, 04 Apr 2022 23:49:42 GMT
CMD ["/bin/sh"]
# Tue, 19 Apr 2022 18:49:33 GMT
ENV NATS_STREAMING_SERVER=0.24.4
# Tue, 19 Apr 2022 18:49:37 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='abf61454846309f4350a209aa86d8def4ceefaa35b576fe027915f31eeaaebf6' ;; 		armhf) natsArch='arm6'; sha256='bc6efafbf051b8bbabe868240ffa9f88a5676727e3c6a5ffc13542ebd0d6585c' ;; 		armv7) natsArch='arm7'; sha256='7950f6ea4b5385454350c8979d6062aa710400a2d21a3a44d971e8535d944545' ;; 		x86_64) natsArch='amd64'; sha256='e7b1db559c02d123d0aabdf0d3a93803eb0778aa733a26ec9067c833bd5728b9' ;; 		x86) natsArch='386'; sha256='941a7be15b8f3d2ba18508baaced39884b1ed86214c2afb2c2bcfcfad3743903' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Tue, 19 Apr 2022 18:49:38 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Tue, 19 Apr 2022 18:49:38 GMT
EXPOSE 4222 8222
# Tue, 19 Apr 2022 18:49:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 19 Apr 2022 18:49:39 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:c319b1fc4ed70b8241a7ce6ac0c4015d354bf5cf8c01eb73c50b6709c0c46e49`  
		Last Modified: Mon, 04 Apr 2022 19:09:22 GMT  
		Size: 2.6 MB (2621972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7749efc5f39c770d1ec4c0ef3a405656aa5e1993fbdacd7d21f3d4707ff1a72c`  
		Last Modified: Tue, 19 Apr 2022 18:51:22 GMT  
		Size: 6.9 MB (6940049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a23a7c4070e79cc4538b1305be5da3a4b615da587a7fd569a0be26bd110fa84`  
		Last Modified: Tue, 19 Apr 2022 18:51:18 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:43fa0020bbe495315ac2f09debe4bf6b27dd74790d26ac3366750c3055e58a3c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.4 MB (9354606 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4afe09639533164664c235319932921bedc9450ecd3de243641a70c7a583c5d1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Mon, 04 Apr 2022 23:57:34 GMT
ADD file:20f8cdddc53a4a8bd78945fc32fe08e9f80ab3b16dc20a9aa4ba73b79f2bc71c in / 
# Mon, 04 Apr 2022 23:57:35 GMT
CMD ["/bin/sh"]
# Tue, 19 Apr 2022 18:57:51 GMT
ENV NATS_STREAMING_SERVER=0.24.4
# Tue, 19 Apr 2022 18:57:55 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='abf61454846309f4350a209aa86d8def4ceefaa35b576fe027915f31eeaaebf6' ;; 		armhf) natsArch='arm6'; sha256='bc6efafbf051b8bbabe868240ffa9f88a5676727e3c6a5ffc13542ebd0d6585c' ;; 		armv7) natsArch='arm7'; sha256='7950f6ea4b5385454350c8979d6062aa710400a2d21a3a44d971e8535d944545' ;; 		x86_64) natsArch='amd64'; sha256='e7b1db559c02d123d0aabdf0d3a93803eb0778aa733a26ec9067c833bd5728b9' ;; 		x86) natsArch='386'; sha256='941a7be15b8f3d2ba18508baaced39884b1ed86214c2afb2c2bcfcfad3743903' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Tue, 19 Apr 2022 18:57:56 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Tue, 19 Apr 2022 18:57:56 GMT
EXPOSE 4222 8222
# Tue, 19 Apr 2022 18:57:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 19 Apr 2022 18:57:57 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:57fb4b5f1a47c953ca5703f0f81ce14e5d01cf23aa79558b5adb961cc526e320`  
		Last Modified: Mon, 04 Apr 2022 19:09:36 GMT  
		Size: 2.4 MB (2424323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cab0ba64de7ddcb969882eb8b609a89179c2d441a4bcc7317ae977fd7dda4e23`  
		Last Modified: Tue, 19 Apr 2022 18:59:41 GMT  
		Size: 6.9 MB (6929861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27e7fde7215edaedba408f2d6f77c7043df6c84d3309cffeb7f8b14f1c0b82c0`  
		Last Modified: Tue, 19 Apr 2022 18:59:37 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:bef1eb9f86f148797e14e6dd500934864bd8611f0256715a932c286bbedbddb4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.6 MB (9567309 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89a27b9fd024c9823aa8be1c38baede9477c1bf1ab37ddbec1c6d01c2a3a658a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:31 GMT
ADD file:90e56af13188c7f0283d244a0d70b853d8bef8587a41f1da8eac3a2aba8964ef in / 
# Mon, 04 Apr 2022 23:39:31 GMT
CMD ["/bin/sh"]
# Tue, 19 Apr 2022 18:40:04 GMT
ENV NATS_STREAMING_SERVER=0.24.4
# Tue, 19 Apr 2022 18:40:07 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='abf61454846309f4350a209aa86d8def4ceefaa35b576fe027915f31eeaaebf6' ;; 		armhf) natsArch='arm6'; sha256='bc6efafbf051b8bbabe868240ffa9f88a5676727e3c6a5ffc13542ebd0d6585c' ;; 		armv7) natsArch='arm7'; sha256='7950f6ea4b5385454350c8979d6062aa710400a2d21a3a44d971e8535d944545' ;; 		x86_64) natsArch='amd64'; sha256='e7b1db559c02d123d0aabdf0d3a93803eb0778aa733a26ec9067c833bd5728b9' ;; 		x86) natsArch='386'; sha256='941a7be15b8f3d2ba18508baaced39884b1ed86214c2afb2c2bcfcfad3743903' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Tue, 19 Apr 2022 18:40:09 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Tue, 19 Apr 2022 18:40:09 GMT
EXPOSE 4222 8222
# Tue, 19 Apr 2022 18:40:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 19 Apr 2022 18:40:11 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:9981e73032c8833e387a8f96986e560edbed12c38119e0edb0439c9c2234eac9`  
		Last Modified: Mon, 04 Apr 2022 19:09:10 GMT  
		Size: 2.7 MB (2716477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0812492999c8bb5bc4d5d0f3cf25e7e1a474b07e1400c864e6f714d6c9771fb1`  
		Last Modified: Tue, 19 Apr 2022 18:40:59 GMT  
		Size: 6.9 MB (6850411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0aedb2f212694a12d2b97ef1d1079ba39d77f30b8574a79cc0421d472c6dfae`  
		Last Modified: Tue, 19 Apr 2022 18:40:58 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:alpine3.15`

```console
$ docker pull nats-streaming@sha256:4afc203c1b06db771f04248b810082a998d82540b7962f4f318b760b94918c4c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:alpine3.15` - linux; amd64

```console
$ docker pull nats-streaming@sha256:4eb3d3f7784016d57166fb89356a963be2b929bbce0639c40efd6a48dfbeab50
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.2 MB (10248491 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0fa2e30f307c690778bcda9368b96aebbd4007db005d6d8d57416bf9f7d93381`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Tue, 05 Apr 2022 00:19:59 GMT
ADD file:5d673d25da3a14ce1f6cf66e4c7fd4f4b85a3759a9d93efb3fd9ff852b5b56e4 in / 
# Tue, 05 Apr 2022 00:19:59 GMT
CMD ["/bin/sh"]
# Tue, 19 Apr 2022 18:19:47 GMT
ENV NATS_STREAMING_SERVER=0.24.4
# Tue, 19 Apr 2022 18:19:49 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='abf61454846309f4350a209aa86d8def4ceefaa35b576fe027915f31eeaaebf6' ;; 		armhf) natsArch='arm6'; sha256='bc6efafbf051b8bbabe868240ffa9f88a5676727e3c6a5ffc13542ebd0d6585c' ;; 		armv7) natsArch='arm7'; sha256='7950f6ea4b5385454350c8979d6062aa710400a2d21a3a44d971e8535d944545' ;; 		x86_64) natsArch='amd64'; sha256='e7b1db559c02d123d0aabdf0d3a93803eb0778aa733a26ec9067c833bd5728b9' ;; 		x86) natsArch='386'; sha256='941a7be15b8f3d2ba18508baaced39884b1ed86214c2afb2c2bcfcfad3743903' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Tue, 19 Apr 2022 18:19:50 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Tue, 19 Apr 2022 18:19:50 GMT
EXPOSE 4222 8222
# Tue, 19 Apr 2022 18:19:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 19 Apr 2022 18:19:50 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:df9b9388f04ad6279a7410b85cedfdcb2208c0a003da7ab5613af71079148139`  
		Last Modified: Mon, 04 Apr 2022 19:10:16 GMT  
		Size: 2.8 MB (2814559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:618bc609c0fe2d2c7dce4a5a08dcb487ee273dfab15895d917e4f5c2425e54de`  
		Last Modified: Tue, 19 Apr 2022 18:20:20 GMT  
		Size: 7.4 MB (7433512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78cdc64ae36d5c3024c2af60810ec1bfff47708a2492efc85d7f5bfecf7abcfe`  
		Last Modified: Tue, 19 Apr 2022 18:20:16 GMT  
		Size: 420.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine3.15` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:092009bcc3beed0c4e6dd0b2e36eb45082919a3cf6178ac42576e7599efefb26
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.6 MB (9562443 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6edad2d6e424051bf23151c9f0b88c0a1ae0f02e7ca579630d5f54da30fb8e69`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Mon, 04 Apr 2022 23:49:42 GMT
ADD file:159dcddaab900372df882a4e94615ed84250e9cea3e74bc0479d98280342f596 in / 
# Mon, 04 Apr 2022 23:49:42 GMT
CMD ["/bin/sh"]
# Tue, 19 Apr 2022 18:49:33 GMT
ENV NATS_STREAMING_SERVER=0.24.4
# Tue, 19 Apr 2022 18:49:37 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='abf61454846309f4350a209aa86d8def4ceefaa35b576fe027915f31eeaaebf6' ;; 		armhf) natsArch='arm6'; sha256='bc6efafbf051b8bbabe868240ffa9f88a5676727e3c6a5ffc13542ebd0d6585c' ;; 		armv7) natsArch='arm7'; sha256='7950f6ea4b5385454350c8979d6062aa710400a2d21a3a44d971e8535d944545' ;; 		x86_64) natsArch='amd64'; sha256='e7b1db559c02d123d0aabdf0d3a93803eb0778aa733a26ec9067c833bd5728b9' ;; 		x86) natsArch='386'; sha256='941a7be15b8f3d2ba18508baaced39884b1ed86214c2afb2c2bcfcfad3743903' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Tue, 19 Apr 2022 18:49:38 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Tue, 19 Apr 2022 18:49:38 GMT
EXPOSE 4222 8222
# Tue, 19 Apr 2022 18:49:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 19 Apr 2022 18:49:39 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:c319b1fc4ed70b8241a7ce6ac0c4015d354bf5cf8c01eb73c50b6709c0c46e49`  
		Last Modified: Mon, 04 Apr 2022 19:09:22 GMT  
		Size: 2.6 MB (2621972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7749efc5f39c770d1ec4c0ef3a405656aa5e1993fbdacd7d21f3d4707ff1a72c`  
		Last Modified: Tue, 19 Apr 2022 18:51:22 GMT  
		Size: 6.9 MB (6940049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a23a7c4070e79cc4538b1305be5da3a4b615da587a7fd569a0be26bd110fa84`  
		Last Modified: Tue, 19 Apr 2022 18:51:18 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine3.15` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:43fa0020bbe495315ac2f09debe4bf6b27dd74790d26ac3366750c3055e58a3c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.4 MB (9354606 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4afe09639533164664c235319932921bedc9450ecd3de243641a70c7a583c5d1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Mon, 04 Apr 2022 23:57:34 GMT
ADD file:20f8cdddc53a4a8bd78945fc32fe08e9f80ab3b16dc20a9aa4ba73b79f2bc71c in / 
# Mon, 04 Apr 2022 23:57:35 GMT
CMD ["/bin/sh"]
# Tue, 19 Apr 2022 18:57:51 GMT
ENV NATS_STREAMING_SERVER=0.24.4
# Tue, 19 Apr 2022 18:57:55 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='abf61454846309f4350a209aa86d8def4ceefaa35b576fe027915f31eeaaebf6' ;; 		armhf) natsArch='arm6'; sha256='bc6efafbf051b8bbabe868240ffa9f88a5676727e3c6a5ffc13542ebd0d6585c' ;; 		armv7) natsArch='arm7'; sha256='7950f6ea4b5385454350c8979d6062aa710400a2d21a3a44d971e8535d944545' ;; 		x86_64) natsArch='amd64'; sha256='e7b1db559c02d123d0aabdf0d3a93803eb0778aa733a26ec9067c833bd5728b9' ;; 		x86) natsArch='386'; sha256='941a7be15b8f3d2ba18508baaced39884b1ed86214c2afb2c2bcfcfad3743903' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Tue, 19 Apr 2022 18:57:56 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Tue, 19 Apr 2022 18:57:56 GMT
EXPOSE 4222 8222
# Tue, 19 Apr 2022 18:57:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 19 Apr 2022 18:57:57 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:57fb4b5f1a47c953ca5703f0f81ce14e5d01cf23aa79558b5adb961cc526e320`  
		Last Modified: Mon, 04 Apr 2022 19:09:36 GMT  
		Size: 2.4 MB (2424323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cab0ba64de7ddcb969882eb8b609a89179c2d441a4bcc7317ae977fd7dda4e23`  
		Last Modified: Tue, 19 Apr 2022 18:59:41 GMT  
		Size: 6.9 MB (6929861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27e7fde7215edaedba408f2d6f77c7043df6c84d3309cffeb7f8b14f1c0b82c0`  
		Last Modified: Tue, 19 Apr 2022 18:59:37 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine3.15` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:bef1eb9f86f148797e14e6dd500934864bd8611f0256715a932c286bbedbddb4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.6 MB (9567309 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89a27b9fd024c9823aa8be1c38baede9477c1bf1ab37ddbec1c6d01c2a3a658a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:31 GMT
ADD file:90e56af13188c7f0283d244a0d70b853d8bef8587a41f1da8eac3a2aba8964ef in / 
# Mon, 04 Apr 2022 23:39:31 GMT
CMD ["/bin/sh"]
# Tue, 19 Apr 2022 18:40:04 GMT
ENV NATS_STREAMING_SERVER=0.24.4
# Tue, 19 Apr 2022 18:40:07 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='abf61454846309f4350a209aa86d8def4ceefaa35b576fe027915f31eeaaebf6' ;; 		armhf) natsArch='arm6'; sha256='bc6efafbf051b8bbabe868240ffa9f88a5676727e3c6a5ffc13542ebd0d6585c' ;; 		armv7) natsArch='arm7'; sha256='7950f6ea4b5385454350c8979d6062aa710400a2d21a3a44d971e8535d944545' ;; 		x86_64) natsArch='amd64'; sha256='e7b1db559c02d123d0aabdf0d3a93803eb0778aa733a26ec9067c833bd5728b9' ;; 		x86) natsArch='386'; sha256='941a7be15b8f3d2ba18508baaced39884b1ed86214c2afb2c2bcfcfad3743903' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Tue, 19 Apr 2022 18:40:09 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Tue, 19 Apr 2022 18:40:09 GMT
EXPOSE 4222 8222
# Tue, 19 Apr 2022 18:40:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 19 Apr 2022 18:40:11 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:9981e73032c8833e387a8f96986e560edbed12c38119e0edb0439c9c2234eac9`  
		Last Modified: Mon, 04 Apr 2022 19:09:10 GMT  
		Size: 2.7 MB (2716477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0812492999c8bb5bc4d5d0f3cf25e7e1a474b07e1400c864e6f714d6c9771fb1`  
		Last Modified: Tue, 19 Apr 2022 18:40:59 GMT  
		Size: 6.9 MB (6850411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0aedb2f212694a12d2b97ef1d1079ba39d77f30b8574a79cc0421d472c6dfae`  
		Last Modified: Tue, 19 Apr 2022 18:40:58 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:latest`

```console
$ docker pull nats-streaming@sha256:a8d0b16eaeeb2b6cb4647f942d5a178b7e44d5709388c86fa1357239cf14ea1e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.2803; amd64

### `nats-streaming:latest` - linux; amd64

```console
$ docker pull nats-streaming@sha256:3ff22408a43de2d67d38aa689b7fede88f92a6e02e9b746402c51441f22a80bd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7160576 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1be4ca5ff457718dd135cac991a2fce8902861901e8f1c7c86e614d68589dced`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 19 Apr 2022 18:19:58 GMT
COPY file:3a9e1a664fc216f321851b3ca6ab92594e42c425862d179ee6a292b590bfe37b in /nats-streaming-server 
# Tue, 19 Apr 2022 18:19:58 GMT
EXPOSE 4222 8222
# Tue, 19 Apr 2022 18:19:58 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 19 Apr 2022 18:19:58 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:f7464e210e47808da4af767838d0a84dada171f8ad1dce32071319a05d071a20`  
		Last Modified: Tue, 19 Apr 2022 18:20:40 GMT  
		Size: 7.2 MB (7160576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:latest` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:afa50deb7af027ad2d1a54f53febadf28e189be0adb82039ea429ce57e1d590c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.7 MB (6666873 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:04f3328d94b185bf70d0866dfa2cb72566e7260e4704cfb2cfef87998649aebd`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 19 Apr 2022 18:49:58 GMT
COPY file:6b8eedac2a0774aea5449501f9ae8c79e7be3d3e55863b7703b427f601cbdd4d in /nats-streaming-server 
# Tue, 19 Apr 2022 18:49:58 GMT
EXPOSE 4222 8222
# Tue, 19 Apr 2022 18:49:59 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 19 Apr 2022 18:49:59 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:dbf88d448d58aea59c794a9388b56a7fe82335bef22b8200658329645f9b783a`  
		Last Modified: Tue, 19 Apr 2022 18:51:59 GMT  
		Size: 6.7 MB (6666873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:latest` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:e8e52a390d9cefe82a9f17a19e2e05c49d4c56a27b05fb956108c047d5a93b31
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.7 MB (6657656 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:42f1e8f63244361974ea334f20240f6d4f94fc96d7e89051e0769eece666b959`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 19 Apr 2022 18:58:20 GMT
COPY file:17bb63ff84cf537d44fe2a6c3b62b7c20b07b7ddd09ec3e118a9ee70593166c5 in /nats-streaming-server 
# Tue, 19 Apr 2022 18:58:20 GMT
EXPOSE 4222 8222
# Tue, 19 Apr 2022 18:58:21 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 19 Apr 2022 18:58:21 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:501cd5abe17e56e7e4b1c9fb82796e05c14f6dcbf6e964d8c37a33da0eb82757`  
		Last Modified: Tue, 19 Apr 2022 19:00:12 GMT  
		Size: 6.7 MB (6657656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:latest` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:e0dc96baa5b7e5dda328b37aa3b8b0c7a8181a6c2b1d987de42b4e5a4fb9398b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6577779 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:274efdfafa30ae2eb7eaaf98eb985e537ddf89be65804d4fdcd414d900365792`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 19 Apr 2022 18:40:21 GMT
COPY file:72420de7c1c1682a55d493d3d9f792d57edc400b24e51ea6987297cc55493b40 in /nats-streaming-server 
# Tue, 19 Apr 2022 18:40:21 GMT
EXPOSE 4222 8222
# Tue, 19 Apr 2022 18:40:22 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 19 Apr 2022 18:40:23 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4a8d243c291d90e3cac092a5d52ec5fe51c7d35bfc569928db3dda38febf3171`  
		Last Modified: Tue, 19 Apr 2022 18:41:22 GMT  
		Size: 6.6 MB (6577779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:latest` - windows version 10.0.17763.2803; amd64

```console
$ docker pull nats-streaming@sha256:f7dcabdb7e29722bc9a94ca7545627fb80bceee30902037d345e7ad3ccdc25e4
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.4 MB (110372947 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db815bd2a9cad87072f5c232a6fd4f15c055cfdb61f213ce993afc03a96acb4d`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 04 Apr 2022 10:52:49 GMT
RUN Apply image 1809-amd64
# Wed, 13 Apr 2022 14:45:42 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Tue, 19 Apr 2022 18:18:45 GMT
RUN cmd /S /C #(nop) COPY file:ca12266791259eaa127475f881c8435e255693982581b95714c2329c1c0c3517 in C:\nats-streaming-server.exe 
# Tue, 19 Apr 2022 18:18:46 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Tue, 19 Apr 2022 18:18:47 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Tue, 19 Apr 2022 18:18:48 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:6fc97003d8b7f593fe071cf3ea64f3ce760cc060f3402bb6b1b849c040e222d5`  
		Size: 103.1 MB (103096169 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a6063f744e542c21ce471bdd7ff0dd6063d8d2a9670afbbc64d086813afd6385`  
		Last Modified: Wed, 13 Apr 2022 14:46:35 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9411ac6dc5ee77971f18c4586ba71147422eec4ca4d30dcc320376336f320e5`  
		Last Modified: Tue, 19 Apr 2022 18:19:44 GMT  
		Size: 7.3 MB (7272107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ba1c750731efcee6ebf143a7cf297c1846074c73db7022f94ebdf9ecab5843e`  
		Last Modified: Tue, 19 Apr 2022 18:19:36 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5e494cba0579a95caf948aed68f7f18e8c554774b11313fc73801906d60cba9`  
		Last Modified: Tue, 19 Apr 2022 18:19:36 GMT  
		Size: 1.2 KB (1192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d745e14762b2ee17a49256c2b5940e11f97dc7c944ef9127faa8ae713bcf9d34`  
		Last Modified: Tue, 19 Apr 2022 18:19:36 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:linux`

```console
$ docker pull nats-streaming@sha256:bf7595fa0e1871058be97fa42b8155f796e95f2582fb2141a11f4a51cdff18e9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:linux` - linux; amd64

```console
$ docker pull nats-streaming@sha256:3ff22408a43de2d67d38aa689b7fede88f92a6e02e9b746402c51441f22a80bd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7160576 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1be4ca5ff457718dd135cac991a2fce8902861901e8f1c7c86e614d68589dced`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 19 Apr 2022 18:19:58 GMT
COPY file:3a9e1a664fc216f321851b3ca6ab92594e42c425862d179ee6a292b590bfe37b in /nats-streaming-server 
# Tue, 19 Apr 2022 18:19:58 GMT
EXPOSE 4222 8222
# Tue, 19 Apr 2022 18:19:58 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 19 Apr 2022 18:19:58 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:f7464e210e47808da4af767838d0a84dada171f8ad1dce32071319a05d071a20`  
		Last Modified: Tue, 19 Apr 2022 18:20:40 GMT  
		Size: 7.2 MB (7160576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:linux` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:afa50deb7af027ad2d1a54f53febadf28e189be0adb82039ea429ce57e1d590c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.7 MB (6666873 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:04f3328d94b185bf70d0866dfa2cb72566e7260e4704cfb2cfef87998649aebd`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 19 Apr 2022 18:49:58 GMT
COPY file:6b8eedac2a0774aea5449501f9ae8c79e7be3d3e55863b7703b427f601cbdd4d in /nats-streaming-server 
# Tue, 19 Apr 2022 18:49:58 GMT
EXPOSE 4222 8222
# Tue, 19 Apr 2022 18:49:59 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 19 Apr 2022 18:49:59 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:dbf88d448d58aea59c794a9388b56a7fe82335bef22b8200658329645f9b783a`  
		Last Modified: Tue, 19 Apr 2022 18:51:59 GMT  
		Size: 6.7 MB (6666873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:linux` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:e8e52a390d9cefe82a9f17a19e2e05c49d4c56a27b05fb956108c047d5a93b31
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.7 MB (6657656 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:42f1e8f63244361974ea334f20240f6d4f94fc96d7e89051e0769eece666b959`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 19 Apr 2022 18:58:20 GMT
COPY file:17bb63ff84cf537d44fe2a6c3b62b7c20b07b7ddd09ec3e118a9ee70593166c5 in /nats-streaming-server 
# Tue, 19 Apr 2022 18:58:20 GMT
EXPOSE 4222 8222
# Tue, 19 Apr 2022 18:58:21 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 19 Apr 2022 18:58:21 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:501cd5abe17e56e7e4b1c9fb82796e05c14f6dcbf6e964d8c37a33da0eb82757`  
		Last Modified: Tue, 19 Apr 2022 19:00:12 GMT  
		Size: 6.7 MB (6657656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:linux` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:e0dc96baa5b7e5dda328b37aa3b8b0c7a8181a6c2b1d987de42b4e5a4fb9398b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6577779 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:274efdfafa30ae2eb7eaaf98eb985e537ddf89be65804d4fdcd414d900365792`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 19 Apr 2022 18:40:21 GMT
COPY file:72420de7c1c1682a55d493d3d9f792d57edc400b24e51ea6987297cc55493b40 in /nats-streaming-server 
# Tue, 19 Apr 2022 18:40:21 GMT
EXPOSE 4222 8222
# Tue, 19 Apr 2022 18:40:22 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 19 Apr 2022 18:40:23 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4a8d243c291d90e3cac092a5d52ec5fe51c7d35bfc569928db3dda38febf3171`  
		Last Modified: Tue, 19 Apr 2022 18:41:22 GMT  
		Size: 6.6 MB (6577779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:nanoserver`

```console
$ docker pull nats-streaming@sha256:5f0fd8d176c73f6fd991c80241c4d8ad94259cff1ea5994dae8aea7b99d35a67
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2803; amd64

### `nats-streaming:nanoserver` - windows version 10.0.17763.2803; amd64

```console
$ docker pull nats-streaming@sha256:f7dcabdb7e29722bc9a94ca7545627fb80bceee30902037d345e7ad3ccdc25e4
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.4 MB (110372947 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db815bd2a9cad87072f5c232a6fd4f15c055cfdb61f213ce993afc03a96acb4d`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 04 Apr 2022 10:52:49 GMT
RUN Apply image 1809-amd64
# Wed, 13 Apr 2022 14:45:42 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Tue, 19 Apr 2022 18:18:45 GMT
RUN cmd /S /C #(nop) COPY file:ca12266791259eaa127475f881c8435e255693982581b95714c2329c1c0c3517 in C:\nats-streaming-server.exe 
# Tue, 19 Apr 2022 18:18:46 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Tue, 19 Apr 2022 18:18:47 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Tue, 19 Apr 2022 18:18:48 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:6fc97003d8b7f593fe071cf3ea64f3ce760cc060f3402bb6b1b849c040e222d5`  
		Size: 103.1 MB (103096169 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a6063f744e542c21ce471bdd7ff0dd6063d8d2a9670afbbc64d086813afd6385`  
		Last Modified: Wed, 13 Apr 2022 14:46:35 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9411ac6dc5ee77971f18c4586ba71147422eec4ca4d30dcc320376336f320e5`  
		Last Modified: Tue, 19 Apr 2022 18:19:44 GMT  
		Size: 7.3 MB (7272107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ba1c750731efcee6ebf143a7cf297c1846074c73db7022f94ebdf9ecab5843e`  
		Last Modified: Tue, 19 Apr 2022 18:19:36 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5e494cba0579a95caf948aed68f7f18e8c554774b11313fc73801906d60cba9`  
		Last Modified: Tue, 19 Apr 2022 18:19:36 GMT  
		Size: 1.2 KB (1192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d745e14762b2ee17a49256c2b5940e11f97dc7c944ef9127faa8ae713bcf9d34`  
		Last Modified: Tue, 19 Apr 2022 18:19:36 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:nanoserver-1809`

```console
$ docker pull nats-streaming@sha256:5f0fd8d176c73f6fd991c80241c4d8ad94259cff1ea5994dae8aea7b99d35a67
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2803; amd64

### `nats-streaming:nanoserver-1809` - windows version 10.0.17763.2803; amd64

```console
$ docker pull nats-streaming@sha256:f7dcabdb7e29722bc9a94ca7545627fb80bceee30902037d345e7ad3ccdc25e4
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.4 MB (110372947 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db815bd2a9cad87072f5c232a6fd4f15c055cfdb61f213ce993afc03a96acb4d`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 04 Apr 2022 10:52:49 GMT
RUN Apply image 1809-amd64
# Wed, 13 Apr 2022 14:45:42 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Tue, 19 Apr 2022 18:18:45 GMT
RUN cmd /S /C #(nop) COPY file:ca12266791259eaa127475f881c8435e255693982581b95714c2329c1c0c3517 in C:\nats-streaming-server.exe 
# Tue, 19 Apr 2022 18:18:46 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Tue, 19 Apr 2022 18:18:47 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Tue, 19 Apr 2022 18:18:48 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:6fc97003d8b7f593fe071cf3ea64f3ce760cc060f3402bb6b1b849c040e222d5`  
		Size: 103.1 MB (103096169 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a6063f744e542c21ce471bdd7ff0dd6063d8d2a9670afbbc64d086813afd6385`  
		Last Modified: Wed, 13 Apr 2022 14:46:35 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9411ac6dc5ee77971f18c4586ba71147422eec4ca4d30dcc320376336f320e5`  
		Last Modified: Tue, 19 Apr 2022 18:19:44 GMT  
		Size: 7.3 MB (7272107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ba1c750731efcee6ebf143a7cf297c1846074c73db7022f94ebdf9ecab5843e`  
		Last Modified: Tue, 19 Apr 2022 18:19:36 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5e494cba0579a95caf948aed68f7f18e8c554774b11313fc73801906d60cba9`  
		Last Modified: Tue, 19 Apr 2022 18:19:36 GMT  
		Size: 1.2 KB (1192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d745e14762b2ee17a49256c2b5940e11f97dc7c944ef9127faa8ae713bcf9d34`  
		Last Modified: Tue, 19 Apr 2022 18:19:36 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:scratch`

```console
$ docker pull nats-streaming@sha256:bf7595fa0e1871058be97fa42b8155f796e95f2582fb2141a11f4a51cdff18e9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:scratch` - linux; amd64

```console
$ docker pull nats-streaming@sha256:3ff22408a43de2d67d38aa689b7fede88f92a6e02e9b746402c51441f22a80bd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7160576 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1be4ca5ff457718dd135cac991a2fce8902861901e8f1c7c86e614d68589dced`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 19 Apr 2022 18:19:58 GMT
COPY file:3a9e1a664fc216f321851b3ca6ab92594e42c425862d179ee6a292b590bfe37b in /nats-streaming-server 
# Tue, 19 Apr 2022 18:19:58 GMT
EXPOSE 4222 8222
# Tue, 19 Apr 2022 18:19:58 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 19 Apr 2022 18:19:58 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:f7464e210e47808da4af767838d0a84dada171f8ad1dce32071319a05d071a20`  
		Last Modified: Tue, 19 Apr 2022 18:20:40 GMT  
		Size: 7.2 MB (7160576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:scratch` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:afa50deb7af027ad2d1a54f53febadf28e189be0adb82039ea429ce57e1d590c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.7 MB (6666873 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:04f3328d94b185bf70d0866dfa2cb72566e7260e4704cfb2cfef87998649aebd`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 19 Apr 2022 18:49:58 GMT
COPY file:6b8eedac2a0774aea5449501f9ae8c79e7be3d3e55863b7703b427f601cbdd4d in /nats-streaming-server 
# Tue, 19 Apr 2022 18:49:58 GMT
EXPOSE 4222 8222
# Tue, 19 Apr 2022 18:49:59 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 19 Apr 2022 18:49:59 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:dbf88d448d58aea59c794a9388b56a7fe82335bef22b8200658329645f9b783a`  
		Last Modified: Tue, 19 Apr 2022 18:51:59 GMT  
		Size: 6.7 MB (6666873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:scratch` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:e8e52a390d9cefe82a9f17a19e2e05c49d4c56a27b05fb956108c047d5a93b31
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.7 MB (6657656 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:42f1e8f63244361974ea334f20240f6d4f94fc96d7e89051e0769eece666b959`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 19 Apr 2022 18:58:20 GMT
COPY file:17bb63ff84cf537d44fe2a6c3b62b7c20b07b7ddd09ec3e118a9ee70593166c5 in /nats-streaming-server 
# Tue, 19 Apr 2022 18:58:20 GMT
EXPOSE 4222 8222
# Tue, 19 Apr 2022 18:58:21 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 19 Apr 2022 18:58:21 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:501cd5abe17e56e7e4b1c9fb82796e05c14f6dcbf6e964d8c37a33da0eb82757`  
		Last Modified: Tue, 19 Apr 2022 19:00:12 GMT  
		Size: 6.7 MB (6657656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:scratch` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:e0dc96baa5b7e5dda328b37aa3b8b0c7a8181a6c2b1d987de42b4e5a4fb9398b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6577779 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:274efdfafa30ae2eb7eaaf98eb985e537ddf89be65804d4fdcd414d900365792`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 19 Apr 2022 18:40:21 GMT
COPY file:72420de7c1c1682a55d493d3d9f792d57edc400b24e51ea6987297cc55493b40 in /nats-streaming-server 
# Tue, 19 Apr 2022 18:40:21 GMT
EXPOSE 4222 8222
# Tue, 19 Apr 2022 18:40:22 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 19 Apr 2022 18:40:23 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4a8d243c291d90e3cac092a5d52ec5fe51c7d35bfc569928db3dda38febf3171`  
		Last Modified: Tue, 19 Apr 2022 18:41:22 GMT  
		Size: 6.6 MB (6577779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:windowsservercore`

```console
$ docker pull nats-streaming@sha256:86c23aeb014348875713589438ea483f5d1f8c2c81a6dae1437392934b1792ef
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2803; amd64

### `nats-streaming:windowsservercore` - windows version 10.0.17763.2803; amd64

```console
$ docker pull nats-streaming@sha256:72f0e5b61606638041efba42873ea1291d8b05d973accd3fa4fb8d87a81dcb5f
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2723900130 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b04dd0632cb73bbae0011b92981b880cef224abb6cb100902b20f342efce7de6`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 04 Apr 2022 11:20:25 GMT
RUN Install update 1809-amd64
# Wed, 13 Apr 2022 12:43:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 Apr 2022 14:42:30 GMT
ENV NATS_DOCKERIZED=1
# Tue, 19 Apr 2022 18:15:31 GMT
ENV NATS_STREAMING_SERVER=0.24.4
# Tue, 19 Apr 2022 18:15:32 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.24.4/nats-streaming-server-v0.24.4-windows-amd64.zip
# Tue, 19 Apr 2022 18:15:33 GMT
ENV NATS_STREAMING_SERVER_SHASUM=147b39fb88a9eb45c3f5692365fa6ee17d95c627bb4ecde7601f68151ace6c41
# Tue, 19 Apr 2022 18:16:48 GMT
RUN Set-PSDebug -Trace 2
# Tue, 19 Apr 2022 18:18:32 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Tue, 19 Apr 2022 18:18:33 GMT
EXPOSE 4222 8222
# Tue, 19 Apr 2022 18:18:34 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Tue, 19 Apr 2022 18:18:35 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ba8181afd4264392fbbf8df14fb4cddc55fbe085ab000e986b789678bc2bb171`  
		Size: 997.6 MB (997587446 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7ebb23aa64bff633cfa3c62b190d84f0e870b04fecb1910f65d0870b5c7f8981`  
		Last Modified: Wed, 13 Apr 2022 14:12:24 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d838c7a98a95bee63894bac798124e8c8572bcacc23e22d85332d453a03a7d7c`  
		Last Modified: Wed, 13 Apr 2022 14:46:17 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63c30d5de5c74ae8a10de14dcc644f3d8db3247159e379e97bfa4a735c0484b6`  
		Last Modified: Tue, 19 Apr 2022 18:19:18 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:611dcea795d1cfe41e1bed673aced23eeba03240c857b46e94747a9b1cddc357`  
		Last Modified: Tue, 19 Apr 2022 18:19:18 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71f868b0b44531e50958ac6c35c161df79228938ab68d4cc7f2b5ddb6384bbd6`  
		Last Modified: Tue, 19 Apr 2022 18:19:18 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d1bd238023271362f8a5a1136b0e5dc705f18688f793dfd34788834dcfbaf32`  
		Last Modified: Tue, 19 Apr 2022 18:19:16 GMT  
		Size: 359.5 KB (359505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0216f3dd53c339c5889dc7bf0dcdcc98ff1b6841b330934f5b991fff52f4574`  
		Last Modified: Tue, 19 Apr 2022 18:19:24 GMT  
		Size: 7.6 MB (7608996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9a52e26f86cff8b968456c51fce3ae5ddb74a9f265da6aec6c4c0104be544b8`  
		Last Modified: Tue, 19 Apr 2022 18:19:16 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4d63ac7f4ccd54465f51b2b43d349150f3ab34b0e60ccc8a22fb65b0bbe1b76`  
		Last Modified: Tue, 19 Apr 2022 18:19:15 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7b91f9f9d8dda9458f9dea3b30fd662ae28ec4bb3bdf3d98f9ccfc1a9be475f`  
		Last Modified: Tue, 19 Apr 2022 18:19:16 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:windowsservercore-1809`

```console
$ docker pull nats-streaming@sha256:86c23aeb014348875713589438ea483f5d1f8c2c81a6dae1437392934b1792ef
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2803; amd64

### `nats-streaming:windowsservercore-1809` - windows version 10.0.17763.2803; amd64

```console
$ docker pull nats-streaming@sha256:72f0e5b61606638041efba42873ea1291d8b05d973accd3fa4fb8d87a81dcb5f
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2723900130 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b04dd0632cb73bbae0011b92981b880cef224abb6cb100902b20f342efce7de6`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 04 Apr 2022 11:20:25 GMT
RUN Install update 1809-amd64
# Wed, 13 Apr 2022 12:43:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 Apr 2022 14:42:30 GMT
ENV NATS_DOCKERIZED=1
# Tue, 19 Apr 2022 18:15:31 GMT
ENV NATS_STREAMING_SERVER=0.24.4
# Tue, 19 Apr 2022 18:15:32 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.24.4/nats-streaming-server-v0.24.4-windows-amd64.zip
# Tue, 19 Apr 2022 18:15:33 GMT
ENV NATS_STREAMING_SERVER_SHASUM=147b39fb88a9eb45c3f5692365fa6ee17d95c627bb4ecde7601f68151ace6c41
# Tue, 19 Apr 2022 18:16:48 GMT
RUN Set-PSDebug -Trace 2
# Tue, 19 Apr 2022 18:18:32 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Tue, 19 Apr 2022 18:18:33 GMT
EXPOSE 4222 8222
# Tue, 19 Apr 2022 18:18:34 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Tue, 19 Apr 2022 18:18:35 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ba8181afd4264392fbbf8df14fb4cddc55fbe085ab000e986b789678bc2bb171`  
		Size: 997.6 MB (997587446 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7ebb23aa64bff633cfa3c62b190d84f0e870b04fecb1910f65d0870b5c7f8981`  
		Last Modified: Wed, 13 Apr 2022 14:12:24 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d838c7a98a95bee63894bac798124e8c8572bcacc23e22d85332d453a03a7d7c`  
		Last Modified: Wed, 13 Apr 2022 14:46:17 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63c30d5de5c74ae8a10de14dcc644f3d8db3247159e379e97bfa4a735c0484b6`  
		Last Modified: Tue, 19 Apr 2022 18:19:18 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:611dcea795d1cfe41e1bed673aced23eeba03240c857b46e94747a9b1cddc357`  
		Last Modified: Tue, 19 Apr 2022 18:19:18 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71f868b0b44531e50958ac6c35c161df79228938ab68d4cc7f2b5ddb6384bbd6`  
		Last Modified: Tue, 19 Apr 2022 18:19:18 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d1bd238023271362f8a5a1136b0e5dc705f18688f793dfd34788834dcfbaf32`  
		Last Modified: Tue, 19 Apr 2022 18:19:16 GMT  
		Size: 359.5 KB (359505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0216f3dd53c339c5889dc7bf0dcdcc98ff1b6841b330934f5b991fff52f4574`  
		Last Modified: Tue, 19 Apr 2022 18:19:24 GMT  
		Size: 7.6 MB (7608996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9a52e26f86cff8b968456c51fce3ae5ddb74a9f265da6aec6c4c0104be544b8`  
		Last Modified: Tue, 19 Apr 2022 18:19:16 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4d63ac7f4ccd54465f51b2b43d349150f3ab34b0e60ccc8a22fb65b0bbe1b76`  
		Last Modified: Tue, 19 Apr 2022 18:19:15 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7b91f9f9d8dda9458f9dea3b30fd662ae28ec4bb3bdf3d98f9ccfc1a9be475f`  
		Last Modified: Tue, 19 Apr 2022 18:19:16 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
