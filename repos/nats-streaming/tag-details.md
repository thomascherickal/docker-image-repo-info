<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `nats-streaming`

-	[`nats-streaming:0.23`](#nats-streaming023)
-	[`nats-streaming:0.23-alpine`](#nats-streaming023-alpine)
-	[`nats-streaming:0.23-alpine3.14`](#nats-streaming023-alpine314)
-	[`nats-streaming:0.23-linux`](#nats-streaming023-linux)
-	[`nats-streaming:0.23-nanoserver`](#nats-streaming023-nanoserver)
-	[`nats-streaming:0.23-nanoserver-1809`](#nats-streaming023-nanoserver-1809)
-	[`nats-streaming:0.23-scratch`](#nats-streaming023-scratch)
-	[`nats-streaming:0.23-windowsservercore`](#nats-streaming023-windowsservercore)
-	[`nats-streaming:0.23-windowsservercore-1809`](#nats-streaming023-windowsservercore-1809)
-	[`nats-streaming:0.23-windowsservercore-ltsc2016`](#nats-streaming023-windowsservercore-ltsc2016)
-	[`nats-streaming:0.23.2`](#nats-streaming0232)
-	[`nats-streaming:0.23.2-alpine`](#nats-streaming0232-alpine)
-	[`nats-streaming:0.23.2-alpine3.14`](#nats-streaming0232-alpine314)
-	[`nats-streaming:0.23.2-linux`](#nats-streaming0232-linux)
-	[`nats-streaming:0.23.2-nanoserver`](#nats-streaming0232-nanoserver)
-	[`nats-streaming:0.23.2-nanoserver-1809`](#nats-streaming0232-nanoserver-1809)
-	[`nats-streaming:0.23.2-scratch`](#nats-streaming0232-scratch)
-	[`nats-streaming:0.23.2-windowsservercore`](#nats-streaming0232-windowsservercore)
-	[`nats-streaming:0.23.2-windowsservercore-1809`](#nats-streaming0232-windowsservercore-1809)
-	[`nats-streaming:0.23.2-windowsservercore-ltsc2016`](#nats-streaming0232-windowsservercore-ltsc2016)
-	[`nats-streaming:alpine`](#nats-streamingalpine)
-	[`nats-streaming:alpine3.14`](#nats-streamingalpine314)
-	[`nats-streaming:latest`](#nats-streaminglatest)
-	[`nats-streaming:linux`](#nats-streaminglinux)
-	[`nats-streaming:nanoserver`](#nats-streamingnanoserver)
-	[`nats-streaming:nanoserver-1809`](#nats-streamingnanoserver-1809)
-	[`nats-streaming:scratch`](#nats-streamingscratch)
-	[`nats-streaming:windowsservercore`](#nats-streamingwindowsservercore)
-	[`nats-streaming:windowsservercore-1809`](#nats-streamingwindowsservercore-1809)
-	[`nats-streaming:windowsservercore-ltsc2016`](#nats-streamingwindowsservercore-ltsc2016)

## `nats-streaming:0.23`

```console
$ docker pull nats-streaming@sha256:17f569d1c9e1468bbe3a7371279ccde5538ea320fd4ebd94600b904d2e742657
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.2452; amd64

### `nats-streaming:0.23` - linux; amd64

```console
$ docker pull nats-streaming@sha256:05a387b6bd267efd7806a67b7b4d431d054e69537a8dd00f0a874e71b48be7e1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7299150 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e1cf392bf11cb1f2dac51f4d09fa86f69859583c3ac7d4812f6c1887d485073`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Sat, 20 Nov 2021 02:21:16 GMT
COPY file:430b600f51b8ec2b8032b9ee2b54a3f23458b67e7fcd26e03d4a1c4fb292e8e3 in /nats-streaming-server 
# Sat, 20 Nov 2021 02:21:16 GMT
EXPOSE 4222 8222
# Sat, 20 Nov 2021 02:21:16 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Sat, 20 Nov 2021 02:21:17 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:ea39d064fdb9df476b776a2728cf769791a02b09590387975647243e2266b1ca`  
		Last Modified: Sat, 20 Nov 2021 02:22:01 GMT  
		Size: 7.3 MB (7299150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.23` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:0c1a07390ec1c002d89b5bcd0d0048c95f33f859d53b607ffdc16678e3f79bd8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6774516 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1392e1316cac3fc870ec9cd90c7973466ed1433895aee0166a624b060262b6b5`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Fri, 19 Nov 2021 23:50:00 GMT
COPY file:d86d6a12a47b28bc562444b508d1508f4f436aa57b4f9785d2f72f13991058d9 in /nats-streaming-server 
# Fri, 19 Nov 2021 23:50:00 GMT
EXPOSE 4222 8222
# Fri, 19 Nov 2021 23:50:01 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Fri, 19 Nov 2021 23:50:01 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:ada5d2acf52444276ec7168ad03307d61f3ac5bb2e33825f280ba40e265f0533`  
		Last Modified: Fri, 19 Nov 2021 23:51:55 GMT  
		Size: 6.8 MB (6774516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.23` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:cf7abf017ca4b10bcc16492ee29f54f9901fc6c40ae0e5eeba35423ce4346312
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6763075 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4f2b939f92968d68a30b61db2b05fae78f9b7545fb1060ebb0c535069d2a6e0`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Sat, 20 Nov 2021 02:34:09 GMT
COPY file:f737534371c307ebba33d860a23821186a07bfe6bac93b4f8db1052afabca519 in /nats-streaming-server 
# Sat, 20 Nov 2021 02:34:09 GMT
EXPOSE 4222 8222
# Sat, 20 Nov 2021 02:34:10 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Sat, 20 Nov 2021 02:34:10 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:f09d0d006743cce0f69db665ba3e97775e3e7ec87b782222a87b0e299de7abdd`  
		Last Modified: Sat, 20 Nov 2021 02:36:04 GMT  
		Size: 6.8 MB (6763075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.23` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:62364f60027f7c3607653a956cf2578021f20431d07038537298bd2e053f622d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.7 MB (6666709 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e200b7f1afcc145455136db22812cb59ac4b91d3018f34d80f3df1980798dfa`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Sat, 20 Nov 2021 04:21:01 GMT
COPY file:758facc101ea28c799c8630223bb78d0e4182d429b666642665350bc7a40a28d in /nats-streaming-server 
# Sat, 20 Nov 2021 04:21:01 GMT
EXPOSE 4222 8222
# Sat, 20 Nov 2021 04:21:02 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Sat, 20 Nov 2021 04:21:03 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:372c129ce02fe71df79c38000ee3af5425ca18626def1095c58ab7c9cc6a31a8`  
		Last Modified: Sat, 20 Nov 2021 04:22:04 GMT  
		Size: 6.7 MB (6666709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.23` - windows version 10.0.17763.2452; amd64

```console
$ docker pull nats-streaming@sha256:e5a5c9eee1f4f76f236ebf6a7049dd1956e9db04ae49b2b50c960eb7b51bfb17
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.5 MB (110458174 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86f5bfb309b8634f75a1184a8b349dc72fbe6750e195fa87c4ee3b7220ebc253`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Fri, 07 Jan 2022 22:25:06 GMT
RUN Apply image 1809-amd64
# Wed, 12 Jan 2022 15:13:42 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 12 Jan 2022 16:36:12 GMT
RUN cmd /S /C #(nop) COPY file:bb30895f60b97f75adc45bbc64dd23d70df079c19ad26c4f8d07ce1c88e77c96 in C:\nats-streaming-server.exe 
# Wed, 12 Jan 2022 16:36:13 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 12 Jan 2022 16:36:14 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 12 Jan 2022 16:36:15 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:3a78847ea829208edc2d7b320b7e602b9d12e47689499d5180a9cc7790dec4d7`  
		Size: 103.0 MB (103031066 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:db05d2e76671d91772a070867bf6f050343319070602a0f8239706d5d4d98387`  
		Last Modified: Wed, 12 Jan 2022 15:14:49 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60d32b598636a5d24f0e2fed2dcea425de4fb29e48ffe747b16de7d34ba96d44`  
		Last Modified: Wed, 12 Jan 2022 16:37:10 GMT  
		Size: 7.4 MB (7422473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:655251a8c00e62468ac138e6498ed5003026017f9e3aaa8a0890c8e4573e3e5d`  
		Last Modified: Wed, 12 Jan 2022 16:37:02 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99ce1684628b1c7cadb6b52866c3be12d063636d962797df7454acc55806596d`  
		Last Modified: Wed, 12 Jan 2022 16:37:02 GMT  
		Size: 1.2 KB (1161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:489b687ddd94c7a64a680862d4341e41ad8fd93a41455a22da84feac26690169`  
		Last Modified: Wed, 12 Jan 2022 16:37:02 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.23-alpine`

```console
$ docker pull nats-streaming@sha256:1c78a54f4963d1eff5a6bd8759a20b2336a5e300fcf5f62611101679c61e7d11
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.23-alpine` - linux; amd64

```console
$ docker pull nats-streaming@sha256:33d7a075703135ba18cf4918fccc35e6fbef1f74ac8bb18abb89a62fde7c4e02
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.4 MB (10404541 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c0d37898667fe6fa6289417167d7e7ce3799d21b08dc0ea4276850e2e8b54b8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:44 GMT
ADD file:762c899ec0505d1a32930ee804c5b008825f41611161be104076cba33b7e5b2b in / 
# Fri, 12 Nov 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Sat, 20 Nov 2021 02:20:53 GMT
ENV NATS_STREAMING_SERVER=0.23.2
# Sat, 20 Nov 2021 02:20:56 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='623cd04855e16ca52694964e01e3b50ded9747a45885bba1a705513da297f6fd' ;; 		armhf) natsArch='arm6'; sha256='fd40f251da335eb7b3cc63b08f8bc0a80d3a4df10fec4efdf6e60417248a5287' ;; 		armv7) natsArch='arm7'; sha256='83db867570654731de98f135f9f373d0758bd9c5a3ee304b65c8128e1d928023' ;; 		x86_64) natsArch='amd64'; sha256='d0c5ebc16901bdc4788d0382dab6f7ce69582e1bafea3ddba159b38ae87b6c81' ;; 		x86) natsArch='386'; sha256='8b9c5396a7747abc8415dc8ca915cf6cb2fd1b79b64ce7a4c3f5efb241cd389f' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Sat, 20 Nov 2021 02:20:56 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Sat, 20 Nov 2021 02:20:56 GMT
EXPOSE 4222 8222
# Sat, 20 Nov 2021 02:20:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 20 Nov 2021 02:20:57 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:97518928ae5f3d52d4164b314a7e73654eb686ecd8aafa0b79acd980773a740d`  
		Last Modified: Fri, 12 Nov 2021 17:20:39 GMT  
		Size: 2.8 MB (2822981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b719fc3addd4e8cc595271456fe9f9de32955502a0f0cadd27a40bfdce67cdf9`  
		Last Modified: Sat, 20 Nov 2021 02:21:41 GMT  
		Size: 7.6 MB (7581138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ae16eed54939fd32b16d2ffcc1ac1e816da3a11b3656bf2344d9d3180173bf5`  
		Last Modified: Sat, 20 Nov 2021 02:21:39 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.23-alpine` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:983f8ac2dbbaa85241dbc5508ee63b554e7ac9952787ddb8c11565fe8fa6f89d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.7 MB (9694130 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6428fa782d5b97614b699deec16e4b3715fe3df66e91d7c27b27104a5534c9f0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 12 Nov 2021 16:49:42 GMT
ADD file:6daf1fe862c00673bf9cf4d7e20b0bf253a56e7fb8ed5e730a4466ab9186e18a in / 
# Fri, 12 Nov 2021 16:49:44 GMT
CMD ["/bin/sh"]
# Fri, 19 Nov 2021 23:49:35 GMT
ENV NATS_STREAMING_SERVER=0.23.2
# Fri, 19 Nov 2021 23:49:40 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='623cd04855e16ca52694964e01e3b50ded9747a45885bba1a705513da297f6fd' ;; 		armhf) natsArch='arm6'; sha256='fd40f251da335eb7b3cc63b08f8bc0a80d3a4df10fec4efdf6e60417248a5287' ;; 		armv7) natsArch='arm7'; sha256='83db867570654731de98f135f9f373d0758bd9c5a3ee304b65c8128e1d928023' ;; 		x86_64) natsArch='amd64'; sha256='d0c5ebc16901bdc4788d0382dab6f7ce69582e1bafea3ddba159b38ae87b6c81' ;; 		x86) natsArch='386'; sha256='8b9c5396a7747abc8415dc8ca915cf6cb2fd1b79b64ce7a4c3f5efb241cd389f' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Fri, 19 Nov 2021 23:49:40 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Fri, 19 Nov 2021 23:49:41 GMT
EXPOSE 4222 8222
# Fri, 19 Nov 2021 23:49:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 19 Nov 2021 23:49:42 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:56afcfda5d78cc243287acbaad250c5e8c0f47aae620dd7c51985b0d3c9b2728`  
		Last Modified: Fri, 12 Nov 2021 16:51:32 GMT  
		Size: 2.6 MB (2635392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:824cebd74c6dc7b249f375f4f8b9b003e37db5170f8a26342ed408ae5f39da31`  
		Last Modified: Fri, 19 Nov 2021 23:51:24 GMT  
		Size: 7.1 MB (7058316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba898a9271af9b0a02e91bab485a625e6bba3437f8ed1953bd6497c5a6fee966`  
		Last Modified: Fri, 19 Nov 2021 23:51:19 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.23-alpine` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:8d102ba94dd539c86ae564d1671562cd9687b6001ef28c0a3b9358a31b395259
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.5 MB (9487244 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7fe704390d0d6f143b4d58b95fdb72ffd4050dc343669fad7792a25bbd8fc6ae`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 12 Nov 2021 16:57:35 GMT
ADD file:03e0720458c3475758bf4394afa56f2165198eb91e6e9581f7768e433744dd9b in / 
# Fri, 12 Nov 2021 16:57:36 GMT
CMD ["/bin/sh"]
# Sat, 20 Nov 2021 02:33:41 GMT
ENV NATS_STREAMING_SERVER=0.23.2
# Sat, 20 Nov 2021 02:33:46 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='623cd04855e16ca52694964e01e3b50ded9747a45885bba1a705513da297f6fd' ;; 		armhf) natsArch='arm6'; sha256='fd40f251da335eb7b3cc63b08f8bc0a80d3a4df10fec4efdf6e60417248a5287' ;; 		armv7) natsArch='arm7'; sha256='83db867570654731de98f135f9f373d0758bd9c5a3ee304b65c8128e1d928023' ;; 		x86_64) natsArch='amd64'; sha256='d0c5ebc16901bdc4788d0382dab6f7ce69582e1bafea3ddba159b38ae87b6c81' ;; 		x86) natsArch='386'; sha256='8b9c5396a7747abc8415dc8ca915cf6cb2fd1b79b64ce7a4c3f5efb241cd389f' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Sat, 20 Nov 2021 02:33:46 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Sat, 20 Nov 2021 02:33:47 GMT
EXPOSE 4222 8222
# Sat, 20 Nov 2021 02:33:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 20 Nov 2021 02:33:47 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:764d2e53e1a607f2d8261522185d5b9021ade3ec1a595664ee90308c00176899`  
		Last Modified: Fri, 12 Nov 2021 16:59:33 GMT  
		Size: 2.4 MB (2438618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d09b93296bc34cee4aad9d52835eae7e820697f4e8ce382165efb96a8901ea0c`  
		Last Modified: Sat, 20 Nov 2021 02:35:32 GMT  
		Size: 7.0 MB (7048204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:437c793edf6a99d693922586d1182b7f23998316f40d7f5f9e9c74fca0561094`  
		Last Modified: Sat, 20 Nov 2021 02:35:27 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.23-alpine` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:c87eb1e5ff911b6ca53a44595f294a4e79baef015629cd41355e25a3bcbebffc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.7 MB (9669856 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89205df0bff2640b3f02b3d8eddbce0582d123a8e34ae55fa68fb034b4e42bb4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 12 Nov 2021 16:39:58 GMT
ADD file:400c0466b29ccad54e0f6c0acef22542992828678c96693ef1f9f4d0551935d8 in / 
# Fri, 12 Nov 2021 16:39:58 GMT
CMD ["/bin/sh"]
# Sat, 20 Nov 2021 04:20:45 GMT
ENV NATS_STREAMING_SERVER=0.23.2
# Sat, 20 Nov 2021 04:20:49 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='623cd04855e16ca52694964e01e3b50ded9747a45885bba1a705513da297f6fd' ;; 		armhf) natsArch='arm6'; sha256='fd40f251da335eb7b3cc63b08f8bc0a80d3a4df10fec4efdf6e60417248a5287' ;; 		armv7) natsArch='arm7'; sha256='83db867570654731de98f135f9f373d0758bd9c5a3ee304b65c8128e1d928023' ;; 		x86_64) natsArch='amd64'; sha256='d0c5ebc16901bdc4788d0382dab6f7ce69582e1bafea3ddba159b38ae87b6c81' ;; 		x86) natsArch='386'; sha256='8b9c5396a7747abc8415dc8ca915cf6cb2fd1b79b64ce7a4c3f5efb241cd389f' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Sat, 20 Nov 2021 04:20:50 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Sat, 20 Nov 2021 04:20:50 GMT
EXPOSE 4222 8222
# Sat, 20 Nov 2021 04:20:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 20 Nov 2021 04:20:52 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:be307f383ecc62b27a29b599c3fc9d3129693a798e7fcce614f09174cfe2d354`  
		Last Modified: Fri, 12 Nov 2021 16:40:59 GMT  
		Size: 2.7 MB (2717700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a942eeaa58bb70c5a728104921dad38ccc6d39aca7c779aa1431c751506e6ab`  
		Last Modified: Sat, 20 Nov 2021 04:21:41 GMT  
		Size: 7.0 MB (6951735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd89828a2f02db651c46db6cbf2f637d36ecc30f847933336bb73135367cd013`  
		Last Modified: Sat, 20 Nov 2021 04:21:40 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.23-alpine3.14`

```console
$ docker pull nats-streaming@sha256:1c78a54f4963d1eff5a6bd8759a20b2336a5e300fcf5f62611101679c61e7d11
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.23-alpine3.14` - linux; amd64

```console
$ docker pull nats-streaming@sha256:33d7a075703135ba18cf4918fccc35e6fbef1f74ac8bb18abb89a62fde7c4e02
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.4 MB (10404541 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c0d37898667fe6fa6289417167d7e7ce3799d21b08dc0ea4276850e2e8b54b8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:44 GMT
ADD file:762c899ec0505d1a32930ee804c5b008825f41611161be104076cba33b7e5b2b in / 
# Fri, 12 Nov 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Sat, 20 Nov 2021 02:20:53 GMT
ENV NATS_STREAMING_SERVER=0.23.2
# Sat, 20 Nov 2021 02:20:56 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='623cd04855e16ca52694964e01e3b50ded9747a45885bba1a705513da297f6fd' ;; 		armhf) natsArch='arm6'; sha256='fd40f251da335eb7b3cc63b08f8bc0a80d3a4df10fec4efdf6e60417248a5287' ;; 		armv7) natsArch='arm7'; sha256='83db867570654731de98f135f9f373d0758bd9c5a3ee304b65c8128e1d928023' ;; 		x86_64) natsArch='amd64'; sha256='d0c5ebc16901bdc4788d0382dab6f7ce69582e1bafea3ddba159b38ae87b6c81' ;; 		x86) natsArch='386'; sha256='8b9c5396a7747abc8415dc8ca915cf6cb2fd1b79b64ce7a4c3f5efb241cd389f' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Sat, 20 Nov 2021 02:20:56 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Sat, 20 Nov 2021 02:20:56 GMT
EXPOSE 4222 8222
# Sat, 20 Nov 2021 02:20:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 20 Nov 2021 02:20:57 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:97518928ae5f3d52d4164b314a7e73654eb686ecd8aafa0b79acd980773a740d`  
		Last Modified: Fri, 12 Nov 2021 17:20:39 GMT  
		Size: 2.8 MB (2822981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b719fc3addd4e8cc595271456fe9f9de32955502a0f0cadd27a40bfdce67cdf9`  
		Last Modified: Sat, 20 Nov 2021 02:21:41 GMT  
		Size: 7.6 MB (7581138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ae16eed54939fd32b16d2ffcc1ac1e816da3a11b3656bf2344d9d3180173bf5`  
		Last Modified: Sat, 20 Nov 2021 02:21:39 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.23-alpine3.14` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:983f8ac2dbbaa85241dbc5508ee63b554e7ac9952787ddb8c11565fe8fa6f89d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.7 MB (9694130 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6428fa782d5b97614b699deec16e4b3715fe3df66e91d7c27b27104a5534c9f0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 12 Nov 2021 16:49:42 GMT
ADD file:6daf1fe862c00673bf9cf4d7e20b0bf253a56e7fb8ed5e730a4466ab9186e18a in / 
# Fri, 12 Nov 2021 16:49:44 GMT
CMD ["/bin/sh"]
# Fri, 19 Nov 2021 23:49:35 GMT
ENV NATS_STREAMING_SERVER=0.23.2
# Fri, 19 Nov 2021 23:49:40 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='623cd04855e16ca52694964e01e3b50ded9747a45885bba1a705513da297f6fd' ;; 		armhf) natsArch='arm6'; sha256='fd40f251da335eb7b3cc63b08f8bc0a80d3a4df10fec4efdf6e60417248a5287' ;; 		armv7) natsArch='arm7'; sha256='83db867570654731de98f135f9f373d0758bd9c5a3ee304b65c8128e1d928023' ;; 		x86_64) natsArch='amd64'; sha256='d0c5ebc16901bdc4788d0382dab6f7ce69582e1bafea3ddba159b38ae87b6c81' ;; 		x86) natsArch='386'; sha256='8b9c5396a7747abc8415dc8ca915cf6cb2fd1b79b64ce7a4c3f5efb241cd389f' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Fri, 19 Nov 2021 23:49:40 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Fri, 19 Nov 2021 23:49:41 GMT
EXPOSE 4222 8222
# Fri, 19 Nov 2021 23:49:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 19 Nov 2021 23:49:42 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:56afcfda5d78cc243287acbaad250c5e8c0f47aae620dd7c51985b0d3c9b2728`  
		Last Modified: Fri, 12 Nov 2021 16:51:32 GMT  
		Size: 2.6 MB (2635392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:824cebd74c6dc7b249f375f4f8b9b003e37db5170f8a26342ed408ae5f39da31`  
		Last Modified: Fri, 19 Nov 2021 23:51:24 GMT  
		Size: 7.1 MB (7058316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba898a9271af9b0a02e91bab485a625e6bba3437f8ed1953bd6497c5a6fee966`  
		Last Modified: Fri, 19 Nov 2021 23:51:19 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.23-alpine3.14` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:8d102ba94dd539c86ae564d1671562cd9687b6001ef28c0a3b9358a31b395259
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.5 MB (9487244 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7fe704390d0d6f143b4d58b95fdb72ffd4050dc343669fad7792a25bbd8fc6ae`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 12 Nov 2021 16:57:35 GMT
ADD file:03e0720458c3475758bf4394afa56f2165198eb91e6e9581f7768e433744dd9b in / 
# Fri, 12 Nov 2021 16:57:36 GMT
CMD ["/bin/sh"]
# Sat, 20 Nov 2021 02:33:41 GMT
ENV NATS_STREAMING_SERVER=0.23.2
# Sat, 20 Nov 2021 02:33:46 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='623cd04855e16ca52694964e01e3b50ded9747a45885bba1a705513da297f6fd' ;; 		armhf) natsArch='arm6'; sha256='fd40f251da335eb7b3cc63b08f8bc0a80d3a4df10fec4efdf6e60417248a5287' ;; 		armv7) natsArch='arm7'; sha256='83db867570654731de98f135f9f373d0758bd9c5a3ee304b65c8128e1d928023' ;; 		x86_64) natsArch='amd64'; sha256='d0c5ebc16901bdc4788d0382dab6f7ce69582e1bafea3ddba159b38ae87b6c81' ;; 		x86) natsArch='386'; sha256='8b9c5396a7747abc8415dc8ca915cf6cb2fd1b79b64ce7a4c3f5efb241cd389f' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Sat, 20 Nov 2021 02:33:46 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Sat, 20 Nov 2021 02:33:47 GMT
EXPOSE 4222 8222
# Sat, 20 Nov 2021 02:33:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 20 Nov 2021 02:33:47 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:764d2e53e1a607f2d8261522185d5b9021ade3ec1a595664ee90308c00176899`  
		Last Modified: Fri, 12 Nov 2021 16:59:33 GMT  
		Size: 2.4 MB (2438618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d09b93296bc34cee4aad9d52835eae7e820697f4e8ce382165efb96a8901ea0c`  
		Last Modified: Sat, 20 Nov 2021 02:35:32 GMT  
		Size: 7.0 MB (7048204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:437c793edf6a99d693922586d1182b7f23998316f40d7f5f9e9c74fca0561094`  
		Last Modified: Sat, 20 Nov 2021 02:35:27 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.23-alpine3.14` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:c87eb1e5ff911b6ca53a44595f294a4e79baef015629cd41355e25a3bcbebffc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.7 MB (9669856 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89205df0bff2640b3f02b3d8eddbce0582d123a8e34ae55fa68fb034b4e42bb4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 12 Nov 2021 16:39:58 GMT
ADD file:400c0466b29ccad54e0f6c0acef22542992828678c96693ef1f9f4d0551935d8 in / 
# Fri, 12 Nov 2021 16:39:58 GMT
CMD ["/bin/sh"]
# Sat, 20 Nov 2021 04:20:45 GMT
ENV NATS_STREAMING_SERVER=0.23.2
# Sat, 20 Nov 2021 04:20:49 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='623cd04855e16ca52694964e01e3b50ded9747a45885bba1a705513da297f6fd' ;; 		armhf) natsArch='arm6'; sha256='fd40f251da335eb7b3cc63b08f8bc0a80d3a4df10fec4efdf6e60417248a5287' ;; 		armv7) natsArch='arm7'; sha256='83db867570654731de98f135f9f373d0758bd9c5a3ee304b65c8128e1d928023' ;; 		x86_64) natsArch='amd64'; sha256='d0c5ebc16901bdc4788d0382dab6f7ce69582e1bafea3ddba159b38ae87b6c81' ;; 		x86) natsArch='386'; sha256='8b9c5396a7747abc8415dc8ca915cf6cb2fd1b79b64ce7a4c3f5efb241cd389f' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Sat, 20 Nov 2021 04:20:50 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Sat, 20 Nov 2021 04:20:50 GMT
EXPOSE 4222 8222
# Sat, 20 Nov 2021 04:20:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 20 Nov 2021 04:20:52 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:be307f383ecc62b27a29b599c3fc9d3129693a798e7fcce614f09174cfe2d354`  
		Last Modified: Fri, 12 Nov 2021 16:40:59 GMT  
		Size: 2.7 MB (2717700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a942eeaa58bb70c5a728104921dad38ccc6d39aca7c779aa1431c751506e6ab`  
		Last Modified: Sat, 20 Nov 2021 04:21:41 GMT  
		Size: 7.0 MB (6951735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd89828a2f02db651c46db6cbf2f637d36ecc30f847933336bb73135367cd013`  
		Last Modified: Sat, 20 Nov 2021 04:21:40 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.23-linux`

```console
$ docker pull nats-streaming@sha256:a80b4649e47eb1640ead441ff67bb621bffc4cecd39041fa6e9802fbdd9b3760
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.23-linux` - linux; amd64

```console
$ docker pull nats-streaming@sha256:05a387b6bd267efd7806a67b7b4d431d054e69537a8dd00f0a874e71b48be7e1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7299150 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e1cf392bf11cb1f2dac51f4d09fa86f69859583c3ac7d4812f6c1887d485073`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Sat, 20 Nov 2021 02:21:16 GMT
COPY file:430b600f51b8ec2b8032b9ee2b54a3f23458b67e7fcd26e03d4a1c4fb292e8e3 in /nats-streaming-server 
# Sat, 20 Nov 2021 02:21:16 GMT
EXPOSE 4222 8222
# Sat, 20 Nov 2021 02:21:16 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Sat, 20 Nov 2021 02:21:17 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:ea39d064fdb9df476b776a2728cf769791a02b09590387975647243e2266b1ca`  
		Last Modified: Sat, 20 Nov 2021 02:22:01 GMT  
		Size: 7.3 MB (7299150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.23-linux` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:0c1a07390ec1c002d89b5bcd0d0048c95f33f859d53b607ffdc16678e3f79bd8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6774516 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1392e1316cac3fc870ec9cd90c7973466ed1433895aee0166a624b060262b6b5`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Fri, 19 Nov 2021 23:50:00 GMT
COPY file:d86d6a12a47b28bc562444b508d1508f4f436aa57b4f9785d2f72f13991058d9 in /nats-streaming-server 
# Fri, 19 Nov 2021 23:50:00 GMT
EXPOSE 4222 8222
# Fri, 19 Nov 2021 23:50:01 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Fri, 19 Nov 2021 23:50:01 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:ada5d2acf52444276ec7168ad03307d61f3ac5bb2e33825f280ba40e265f0533`  
		Last Modified: Fri, 19 Nov 2021 23:51:55 GMT  
		Size: 6.8 MB (6774516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.23-linux` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:cf7abf017ca4b10bcc16492ee29f54f9901fc6c40ae0e5eeba35423ce4346312
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6763075 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4f2b939f92968d68a30b61db2b05fae78f9b7545fb1060ebb0c535069d2a6e0`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Sat, 20 Nov 2021 02:34:09 GMT
COPY file:f737534371c307ebba33d860a23821186a07bfe6bac93b4f8db1052afabca519 in /nats-streaming-server 
# Sat, 20 Nov 2021 02:34:09 GMT
EXPOSE 4222 8222
# Sat, 20 Nov 2021 02:34:10 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Sat, 20 Nov 2021 02:34:10 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:f09d0d006743cce0f69db665ba3e97775e3e7ec87b782222a87b0e299de7abdd`  
		Last Modified: Sat, 20 Nov 2021 02:36:04 GMT  
		Size: 6.8 MB (6763075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.23-linux` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:62364f60027f7c3607653a956cf2578021f20431d07038537298bd2e053f622d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.7 MB (6666709 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e200b7f1afcc145455136db22812cb59ac4b91d3018f34d80f3df1980798dfa`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Sat, 20 Nov 2021 04:21:01 GMT
COPY file:758facc101ea28c799c8630223bb78d0e4182d429b666642665350bc7a40a28d in /nats-streaming-server 
# Sat, 20 Nov 2021 04:21:01 GMT
EXPOSE 4222 8222
# Sat, 20 Nov 2021 04:21:02 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Sat, 20 Nov 2021 04:21:03 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:372c129ce02fe71df79c38000ee3af5425ca18626def1095c58ab7c9cc6a31a8`  
		Last Modified: Sat, 20 Nov 2021 04:22:04 GMT  
		Size: 6.7 MB (6666709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.23-nanoserver`

```console
$ docker pull nats-streaming@sha256:3deb3e84ece2e334a28e4b46853567baf661fb0d6e9965cb297783565c5c96c9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2452; amd64

### `nats-streaming:0.23-nanoserver` - windows version 10.0.17763.2452; amd64

```console
$ docker pull nats-streaming@sha256:e5a5c9eee1f4f76f236ebf6a7049dd1956e9db04ae49b2b50c960eb7b51bfb17
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.5 MB (110458174 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86f5bfb309b8634f75a1184a8b349dc72fbe6750e195fa87c4ee3b7220ebc253`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Fri, 07 Jan 2022 22:25:06 GMT
RUN Apply image 1809-amd64
# Wed, 12 Jan 2022 15:13:42 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 12 Jan 2022 16:36:12 GMT
RUN cmd /S /C #(nop) COPY file:bb30895f60b97f75adc45bbc64dd23d70df079c19ad26c4f8d07ce1c88e77c96 in C:\nats-streaming-server.exe 
# Wed, 12 Jan 2022 16:36:13 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 12 Jan 2022 16:36:14 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 12 Jan 2022 16:36:15 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:3a78847ea829208edc2d7b320b7e602b9d12e47689499d5180a9cc7790dec4d7`  
		Size: 103.0 MB (103031066 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:db05d2e76671d91772a070867bf6f050343319070602a0f8239706d5d4d98387`  
		Last Modified: Wed, 12 Jan 2022 15:14:49 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60d32b598636a5d24f0e2fed2dcea425de4fb29e48ffe747b16de7d34ba96d44`  
		Last Modified: Wed, 12 Jan 2022 16:37:10 GMT  
		Size: 7.4 MB (7422473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:655251a8c00e62468ac138e6498ed5003026017f9e3aaa8a0890c8e4573e3e5d`  
		Last Modified: Wed, 12 Jan 2022 16:37:02 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99ce1684628b1c7cadb6b52866c3be12d063636d962797df7454acc55806596d`  
		Last Modified: Wed, 12 Jan 2022 16:37:02 GMT  
		Size: 1.2 KB (1161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:489b687ddd94c7a64a680862d4341e41ad8fd93a41455a22da84feac26690169`  
		Last Modified: Wed, 12 Jan 2022 16:37:02 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.23-nanoserver-1809`

```console
$ docker pull nats-streaming@sha256:3deb3e84ece2e334a28e4b46853567baf661fb0d6e9965cb297783565c5c96c9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2452; amd64

### `nats-streaming:0.23-nanoserver-1809` - windows version 10.0.17763.2452; amd64

```console
$ docker pull nats-streaming@sha256:e5a5c9eee1f4f76f236ebf6a7049dd1956e9db04ae49b2b50c960eb7b51bfb17
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.5 MB (110458174 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86f5bfb309b8634f75a1184a8b349dc72fbe6750e195fa87c4ee3b7220ebc253`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Fri, 07 Jan 2022 22:25:06 GMT
RUN Apply image 1809-amd64
# Wed, 12 Jan 2022 15:13:42 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 12 Jan 2022 16:36:12 GMT
RUN cmd /S /C #(nop) COPY file:bb30895f60b97f75adc45bbc64dd23d70df079c19ad26c4f8d07ce1c88e77c96 in C:\nats-streaming-server.exe 
# Wed, 12 Jan 2022 16:36:13 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 12 Jan 2022 16:36:14 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 12 Jan 2022 16:36:15 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:3a78847ea829208edc2d7b320b7e602b9d12e47689499d5180a9cc7790dec4d7`  
		Size: 103.0 MB (103031066 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:db05d2e76671d91772a070867bf6f050343319070602a0f8239706d5d4d98387`  
		Last Modified: Wed, 12 Jan 2022 15:14:49 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60d32b598636a5d24f0e2fed2dcea425de4fb29e48ffe747b16de7d34ba96d44`  
		Last Modified: Wed, 12 Jan 2022 16:37:10 GMT  
		Size: 7.4 MB (7422473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:655251a8c00e62468ac138e6498ed5003026017f9e3aaa8a0890c8e4573e3e5d`  
		Last Modified: Wed, 12 Jan 2022 16:37:02 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99ce1684628b1c7cadb6b52866c3be12d063636d962797df7454acc55806596d`  
		Last Modified: Wed, 12 Jan 2022 16:37:02 GMT  
		Size: 1.2 KB (1161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:489b687ddd94c7a64a680862d4341e41ad8fd93a41455a22da84feac26690169`  
		Last Modified: Wed, 12 Jan 2022 16:37:02 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.23-scratch`

```console
$ docker pull nats-streaming@sha256:a80b4649e47eb1640ead441ff67bb621bffc4cecd39041fa6e9802fbdd9b3760
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.23-scratch` - linux; amd64

```console
$ docker pull nats-streaming@sha256:05a387b6bd267efd7806a67b7b4d431d054e69537a8dd00f0a874e71b48be7e1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7299150 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e1cf392bf11cb1f2dac51f4d09fa86f69859583c3ac7d4812f6c1887d485073`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Sat, 20 Nov 2021 02:21:16 GMT
COPY file:430b600f51b8ec2b8032b9ee2b54a3f23458b67e7fcd26e03d4a1c4fb292e8e3 in /nats-streaming-server 
# Sat, 20 Nov 2021 02:21:16 GMT
EXPOSE 4222 8222
# Sat, 20 Nov 2021 02:21:16 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Sat, 20 Nov 2021 02:21:17 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:ea39d064fdb9df476b776a2728cf769791a02b09590387975647243e2266b1ca`  
		Last Modified: Sat, 20 Nov 2021 02:22:01 GMT  
		Size: 7.3 MB (7299150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.23-scratch` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:0c1a07390ec1c002d89b5bcd0d0048c95f33f859d53b607ffdc16678e3f79bd8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6774516 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1392e1316cac3fc870ec9cd90c7973466ed1433895aee0166a624b060262b6b5`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Fri, 19 Nov 2021 23:50:00 GMT
COPY file:d86d6a12a47b28bc562444b508d1508f4f436aa57b4f9785d2f72f13991058d9 in /nats-streaming-server 
# Fri, 19 Nov 2021 23:50:00 GMT
EXPOSE 4222 8222
# Fri, 19 Nov 2021 23:50:01 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Fri, 19 Nov 2021 23:50:01 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:ada5d2acf52444276ec7168ad03307d61f3ac5bb2e33825f280ba40e265f0533`  
		Last Modified: Fri, 19 Nov 2021 23:51:55 GMT  
		Size: 6.8 MB (6774516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.23-scratch` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:cf7abf017ca4b10bcc16492ee29f54f9901fc6c40ae0e5eeba35423ce4346312
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6763075 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4f2b939f92968d68a30b61db2b05fae78f9b7545fb1060ebb0c535069d2a6e0`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Sat, 20 Nov 2021 02:34:09 GMT
COPY file:f737534371c307ebba33d860a23821186a07bfe6bac93b4f8db1052afabca519 in /nats-streaming-server 
# Sat, 20 Nov 2021 02:34:09 GMT
EXPOSE 4222 8222
# Sat, 20 Nov 2021 02:34:10 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Sat, 20 Nov 2021 02:34:10 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:f09d0d006743cce0f69db665ba3e97775e3e7ec87b782222a87b0e299de7abdd`  
		Last Modified: Sat, 20 Nov 2021 02:36:04 GMT  
		Size: 6.8 MB (6763075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.23-scratch` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:62364f60027f7c3607653a956cf2578021f20431d07038537298bd2e053f622d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.7 MB (6666709 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e200b7f1afcc145455136db22812cb59ac4b91d3018f34d80f3df1980798dfa`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Sat, 20 Nov 2021 04:21:01 GMT
COPY file:758facc101ea28c799c8630223bb78d0e4182d429b666642665350bc7a40a28d in /nats-streaming-server 
# Sat, 20 Nov 2021 04:21:01 GMT
EXPOSE 4222 8222
# Sat, 20 Nov 2021 04:21:02 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Sat, 20 Nov 2021 04:21:03 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:372c129ce02fe71df79c38000ee3af5425ca18626def1095c58ab7c9cc6a31a8`  
		Last Modified: Sat, 20 Nov 2021 04:22:04 GMT  
		Size: 6.7 MB (6666709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.23-windowsservercore`

```console
$ docker pull nats-streaming@sha256:60cddb85b5f5991f1e6bcf9b251048c924b7c717f62b1d49a5d7dbf3164f91a9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.2452; amd64
	-	windows version 10.0.14393.4886; amd64

### `nats-streaming:0.23-windowsservercore` - windows version 10.0.17763.2452; amd64

```console
$ docker pull nats-streaming@sha256:b7bd0b03c112bb6a886fc32de7f1416d9a8226341c7425a95714b893c064dabf
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2720323552 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6cf92bdf78d0e103b0277b51786c36629cfd72167d13e7e9e08b399b2a8167b3`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
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
# Wed, 12 Jan 2022 16:33:12 GMT
ENV NATS_STREAMING_SERVER=0.23.2
# Wed, 12 Jan 2022 16:33:13 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.23.2/nats-streaming-server-v0.23.2-windows-amd64.zip
# Wed, 12 Jan 2022 16:33:14 GMT
ENV NATS_STREAMING_SERVER_SHASUM=b28dc8e1565d6fece68781515f759b0ed870831cdf2f7925cff7cf9acb44e7ec
# Wed, 12 Jan 2022 16:34:10 GMT
RUN Set-PSDebug -Trace 2
# Wed, 12 Jan 2022 16:35:52 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 12 Jan 2022 16:35:54 GMT
EXPOSE 4222 8222
# Wed, 12 Jan 2022 16:35:55 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 12 Jan 2022 16:35:56 GMT
CMD ["-m" "8222"]
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
	-	`sha256:2e56f267999eb7fd5bcfb301b0f0e6052a8ae22ca628c389db83c562990cf444`  
		Last Modified: Wed, 12 Jan 2022 16:36:50 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:821e8ced70841dc00f55dcd8124121cbb0c430571a5e5d158741fcf29c4eb763`  
		Last Modified: Wed, 12 Jan 2022 16:36:49 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6f67c1564c45a427f773fc0876060b2020ca2453a98023b375fb06c5f53bf3b`  
		Last Modified: Wed, 12 Jan 2022 16:36:49 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:770a7c738c44f07d9a29e8d8cd2ed3ad2f85aa87d7d0bfba1e7efde7ff6c131b`  
		Last Modified: Wed, 12 Jan 2022 16:36:47 GMT  
		Size: 338.5 KB (338485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29ce328ddff49212914bc498c236b2fa59188c0aaa5086dcab210060f4a886f1`  
		Last Modified: Wed, 12 Jan 2022 16:36:50 GMT  
		Size: 7.7 MB (7742962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:091c2e64ef4827cbcb4a216d0422edb3669c90feafeb39b97d344bed44ea4b75`  
		Last Modified: Wed, 12 Jan 2022 16:36:47 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38db1a89341b657073620f8a786ceec8c75be7fc50ccc4a506c364942fa7bc40`  
		Last Modified: Wed, 12 Jan 2022 16:36:47 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1c36c3fb3a835905d4b5ab75dbb3b1e7d580f9723d36b7bf3cf9fcea75f6365`  
		Last Modified: Wed, 12 Jan 2022 16:36:47 GMT  
		Size: 1.4 KB (1381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.23-windowsservercore` - windows version 10.0.14393.4886; amd64

```console
$ docker pull nats-streaming@sha256:d55e31a14946b12f1d6c152dfb777ad1b2da038f0c957bde81c5cfb59cd1a97d
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6290824289 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:111095c35ecacfdbe68e1ef364f73124e3888020c1fdffe9c88d2b78bd021fa8`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
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
# Tue, 11 Jan 2022 19:57:41 GMT
ENV NATS_STREAMING_SERVER=0.23.2
# Tue, 11 Jan 2022 19:57:42 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.23.2/nats-streaming-server-v0.23.2-windows-amd64.zip
# Tue, 11 Jan 2022 19:57:43 GMT
ENV NATS_STREAMING_SERVER_SHASUM=b28dc8e1565d6fece68781515f759b0ed870831cdf2f7925cff7cf9acb44e7ec
# Tue, 11 Jan 2022 21:24:39 GMT
RUN Set-PSDebug -Trace 2
# Tue, 11 Jan 2022 21:26:28 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Tue, 11 Jan 2022 21:26:29 GMT
EXPOSE 4222 8222
# Tue, 11 Jan 2022 21:26:31 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Tue, 11 Jan 2022 21:26:32 GMT
CMD ["-m" "8222"]
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
	-	`sha256:b5cf3c8d8140ae38c2d505f95e5babf9f4505d67a6151d6fe3f9c751ef7d0dc5`  
		Last Modified: Tue, 11 Jan 2022 21:27:37 GMT  
		Size: 1.4 KB (1354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19dc2e3eee55193ca6704fc85c6992e8b9b8bd428d80239cd34ee31b8c72fdc5`  
		Last Modified: Tue, 11 Jan 2022 21:27:37 GMT  
		Size: 1.4 KB (1374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92cc106ea2da4cb4db419ee1efe603754ac4e6645cde9bdf6ee8bde96b5e342a`  
		Last Modified: Tue, 11 Jan 2022 21:27:37 GMT  
		Size: 1.4 KB (1363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c19b53c2023c3798cb5b4fb1bf2c6c906c1c9ec3f1a64fe6ca6832b146c5e926`  
		Last Modified: Tue, 11 Jan 2022 21:27:35 GMT  
		Size: 335.6 KB (335575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b49df4cdedb96e996d903b4a909a6204919bef00f7a72eea5fc92c42249b541c`  
		Last Modified: Tue, 11 Jan 2022 21:27:48 GMT  
		Size: 12.3 MB (12274958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf21ee223236021b829cf5aa5a4a19abe4854ed145378b8ca64aed39459a5611`  
		Last Modified: Tue, 11 Jan 2022 21:27:34 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc2ccb79a6a3985e5a419e8c0f1256719adee45c6ab7d7a049e39e42ee798e91`  
		Last Modified: Tue, 11 Jan 2022 21:27:34 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adb13dd255898f881701597b01fa5e3b8873647e6098933da4de040996a6188d`  
		Last Modified: Tue, 11 Jan 2022 21:27:34 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.23-windowsservercore-1809`

```console
$ docker pull nats-streaming@sha256:f4205543bce3358dd968000ee86d121344534bfeb34634fce3af7196029e72b1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2452; amd64

### `nats-streaming:0.23-windowsservercore-1809` - windows version 10.0.17763.2452; amd64

```console
$ docker pull nats-streaming@sha256:b7bd0b03c112bb6a886fc32de7f1416d9a8226341c7425a95714b893c064dabf
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2720323552 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6cf92bdf78d0e103b0277b51786c36629cfd72167d13e7e9e08b399b2a8167b3`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
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
# Wed, 12 Jan 2022 16:33:12 GMT
ENV NATS_STREAMING_SERVER=0.23.2
# Wed, 12 Jan 2022 16:33:13 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.23.2/nats-streaming-server-v0.23.2-windows-amd64.zip
# Wed, 12 Jan 2022 16:33:14 GMT
ENV NATS_STREAMING_SERVER_SHASUM=b28dc8e1565d6fece68781515f759b0ed870831cdf2f7925cff7cf9acb44e7ec
# Wed, 12 Jan 2022 16:34:10 GMT
RUN Set-PSDebug -Trace 2
# Wed, 12 Jan 2022 16:35:52 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 12 Jan 2022 16:35:54 GMT
EXPOSE 4222 8222
# Wed, 12 Jan 2022 16:35:55 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 12 Jan 2022 16:35:56 GMT
CMD ["-m" "8222"]
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
	-	`sha256:2e56f267999eb7fd5bcfb301b0f0e6052a8ae22ca628c389db83c562990cf444`  
		Last Modified: Wed, 12 Jan 2022 16:36:50 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:821e8ced70841dc00f55dcd8124121cbb0c430571a5e5d158741fcf29c4eb763`  
		Last Modified: Wed, 12 Jan 2022 16:36:49 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6f67c1564c45a427f773fc0876060b2020ca2453a98023b375fb06c5f53bf3b`  
		Last Modified: Wed, 12 Jan 2022 16:36:49 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:770a7c738c44f07d9a29e8d8cd2ed3ad2f85aa87d7d0bfba1e7efde7ff6c131b`  
		Last Modified: Wed, 12 Jan 2022 16:36:47 GMT  
		Size: 338.5 KB (338485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29ce328ddff49212914bc498c236b2fa59188c0aaa5086dcab210060f4a886f1`  
		Last Modified: Wed, 12 Jan 2022 16:36:50 GMT  
		Size: 7.7 MB (7742962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:091c2e64ef4827cbcb4a216d0422edb3669c90feafeb39b97d344bed44ea4b75`  
		Last Modified: Wed, 12 Jan 2022 16:36:47 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38db1a89341b657073620f8a786ceec8c75be7fc50ccc4a506c364942fa7bc40`  
		Last Modified: Wed, 12 Jan 2022 16:36:47 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1c36c3fb3a835905d4b5ab75dbb3b1e7d580f9723d36b7bf3cf9fcea75f6365`  
		Last Modified: Wed, 12 Jan 2022 16:36:47 GMT  
		Size: 1.4 KB (1381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.23-windowsservercore-ltsc2016`

```console
$ docker pull nats-streaming@sha256:8d7f645475c1ddf54332ac47ad4daa549c2a02a25e27f3062c39efed087fd0ba
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.14393.4886; amd64

### `nats-streaming:0.23-windowsservercore-ltsc2016` - windows version 10.0.14393.4886; amd64

```console
$ docker pull nats-streaming@sha256:d55e31a14946b12f1d6c152dfb777ad1b2da038f0c957bde81c5cfb59cd1a97d
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6290824289 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:111095c35ecacfdbe68e1ef364f73124e3888020c1fdffe9c88d2b78bd021fa8`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
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
# Tue, 11 Jan 2022 19:57:41 GMT
ENV NATS_STREAMING_SERVER=0.23.2
# Tue, 11 Jan 2022 19:57:42 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.23.2/nats-streaming-server-v0.23.2-windows-amd64.zip
# Tue, 11 Jan 2022 19:57:43 GMT
ENV NATS_STREAMING_SERVER_SHASUM=b28dc8e1565d6fece68781515f759b0ed870831cdf2f7925cff7cf9acb44e7ec
# Tue, 11 Jan 2022 21:24:39 GMT
RUN Set-PSDebug -Trace 2
# Tue, 11 Jan 2022 21:26:28 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Tue, 11 Jan 2022 21:26:29 GMT
EXPOSE 4222 8222
# Tue, 11 Jan 2022 21:26:31 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Tue, 11 Jan 2022 21:26:32 GMT
CMD ["-m" "8222"]
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
	-	`sha256:b5cf3c8d8140ae38c2d505f95e5babf9f4505d67a6151d6fe3f9c751ef7d0dc5`  
		Last Modified: Tue, 11 Jan 2022 21:27:37 GMT  
		Size: 1.4 KB (1354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19dc2e3eee55193ca6704fc85c6992e8b9b8bd428d80239cd34ee31b8c72fdc5`  
		Last Modified: Tue, 11 Jan 2022 21:27:37 GMT  
		Size: 1.4 KB (1374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92cc106ea2da4cb4db419ee1efe603754ac4e6645cde9bdf6ee8bde96b5e342a`  
		Last Modified: Tue, 11 Jan 2022 21:27:37 GMT  
		Size: 1.4 KB (1363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c19b53c2023c3798cb5b4fb1bf2c6c906c1c9ec3f1a64fe6ca6832b146c5e926`  
		Last Modified: Tue, 11 Jan 2022 21:27:35 GMT  
		Size: 335.6 KB (335575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b49df4cdedb96e996d903b4a909a6204919bef00f7a72eea5fc92c42249b541c`  
		Last Modified: Tue, 11 Jan 2022 21:27:48 GMT  
		Size: 12.3 MB (12274958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf21ee223236021b829cf5aa5a4a19abe4854ed145378b8ca64aed39459a5611`  
		Last Modified: Tue, 11 Jan 2022 21:27:34 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc2ccb79a6a3985e5a419e8c0f1256719adee45c6ab7d7a049e39e42ee798e91`  
		Last Modified: Tue, 11 Jan 2022 21:27:34 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adb13dd255898f881701597b01fa5e3b8873647e6098933da4de040996a6188d`  
		Last Modified: Tue, 11 Jan 2022 21:27:34 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.23.2`

```console
$ docker pull nats-streaming@sha256:17f569d1c9e1468bbe3a7371279ccde5538ea320fd4ebd94600b904d2e742657
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.2452; amd64

### `nats-streaming:0.23.2` - linux; amd64

```console
$ docker pull nats-streaming@sha256:05a387b6bd267efd7806a67b7b4d431d054e69537a8dd00f0a874e71b48be7e1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7299150 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e1cf392bf11cb1f2dac51f4d09fa86f69859583c3ac7d4812f6c1887d485073`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Sat, 20 Nov 2021 02:21:16 GMT
COPY file:430b600f51b8ec2b8032b9ee2b54a3f23458b67e7fcd26e03d4a1c4fb292e8e3 in /nats-streaming-server 
# Sat, 20 Nov 2021 02:21:16 GMT
EXPOSE 4222 8222
# Sat, 20 Nov 2021 02:21:16 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Sat, 20 Nov 2021 02:21:17 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:ea39d064fdb9df476b776a2728cf769791a02b09590387975647243e2266b1ca`  
		Last Modified: Sat, 20 Nov 2021 02:22:01 GMT  
		Size: 7.3 MB (7299150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.23.2` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:0c1a07390ec1c002d89b5bcd0d0048c95f33f859d53b607ffdc16678e3f79bd8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6774516 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1392e1316cac3fc870ec9cd90c7973466ed1433895aee0166a624b060262b6b5`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Fri, 19 Nov 2021 23:50:00 GMT
COPY file:d86d6a12a47b28bc562444b508d1508f4f436aa57b4f9785d2f72f13991058d9 in /nats-streaming-server 
# Fri, 19 Nov 2021 23:50:00 GMT
EXPOSE 4222 8222
# Fri, 19 Nov 2021 23:50:01 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Fri, 19 Nov 2021 23:50:01 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:ada5d2acf52444276ec7168ad03307d61f3ac5bb2e33825f280ba40e265f0533`  
		Last Modified: Fri, 19 Nov 2021 23:51:55 GMT  
		Size: 6.8 MB (6774516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.23.2` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:cf7abf017ca4b10bcc16492ee29f54f9901fc6c40ae0e5eeba35423ce4346312
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6763075 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4f2b939f92968d68a30b61db2b05fae78f9b7545fb1060ebb0c535069d2a6e0`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Sat, 20 Nov 2021 02:34:09 GMT
COPY file:f737534371c307ebba33d860a23821186a07bfe6bac93b4f8db1052afabca519 in /nats-streaming-server 
# Sat, 20 Nov 2021 02:34:09 GMT
EXPOSE 4222 8222
# Sat, 20 Nov 2021 02:34:10 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Sat, 20 Nov 2021 02:34:10 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:f09d0d006743cce0f69db665ba3e97775e3e7ec87b782222a87b0e299de7abdd`  
		Last Modified: Sat, 20 Nov 2021 02:36:04 GMT  
		Size: 6.8 MB (6763075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.23.2` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:62364f60027f7c3607653a956cf2578021f20431d07038537298bd2e053f622d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.7 MB (6666709 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e200b7f1afcc145455136db22812cb59ac4b91d3018f34d80f3df1980798dfa`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Sat, 20 Nov 2021 04:21:01 GMT
COPY file:758facc101ea28c799c8630223bb78d0e4182d429b666642665350bc7a40a28d in /nats-streaming-server 
# Sat, 20 Nov 2021 04:21:01 GMT
EXPOSE 4222 8222
# Sat, 20 Nov 2021 04:21:02 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Sat, 20 Nov 2021 04:21:03 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:372c129ce02fe71df79c38000ee3af5425ca18626def1095c58ab7c9cc6a31a8`  
		Last Modified: Sat, 20 Nov 2021 04:22:04 GMT  
		Size: 6.7 MB (6666709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.23.2` - windows version 10.0.17763.2452; amd64

```console
$ docker pull nats-streaming@sha256:e5a5c9eee1f4f76f236ebf6a7049dd1956e9db04ae49b2b50c960eb7b51bfb17
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.5 MB (110458174 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86f5bfb309b8634f75a1184a8b349dc72fbe6750e195fa87c4ee3b7220ebc253`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Fri, 07 Jan 2022 22:25:06 GMT
RUN Apply image 1809-amd64
# Wed, 12 Jan 2022 15:13:42 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 12 Jan 2022 16:36:12 GMT
RUN cmd /S /C #(nop) COPY file:bb30895f60b97f75adc45bbc64dd23d70df079c19ad26c4f8d07ce1c88e77c96 in C:\nats-streaming-server.exe 
# Wed, 12 Jan 2022 16:36:13 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 12 Jan 2022 16:36:14 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 12 Jan 2022 16:36:15 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:3a78847ea829208edc2d7b320b7e602b9d12e47689499d5180a9cc7790dec4d7`  
		Size: 103.0 MB (103031066 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:db05d2e76671d91772a070867bf6f050343319070602a0f8239706d5d4d98387`  
		Last Modified: Wed, 12 Jan 2022 15:14:49 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60d32b598636a5d24f0e2fed2dcea425de4fb29e48ffe747b16de7d34ba96d44`  
		Last Modified: Wed, 12 Jan 2022 16:37:10 GMT  
		Size: 7.4 MB (7422473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:655251a8c00e62468ac138e6498ed5003026017f9e3aaa8a0890c8e4573e3e5d`  
		Last Modified: Wed, 12 Jan 2022 16:37:02 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99ce1684628b1c7cadb6b52866c3be12d063636d962797df7454acc55806596d`  
		Last Modified: Wed, 12 Jan 2022 16:37:02 GMT  
		Size: 1.2 KB (1161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:489b687ddd94c7a64a680862d4341e41ad8fd93a41455a22da84feac26690169`  
		Last Modified: Wed, 12 Jan 2022 16:37:02 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.23.2-alpine`

```console
$ docker pull nats-streaming@sha256:1c78a54f4963d1eff5a6bd8759a20b2336a5e300fcf5f62611101679c61e7d11
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.23.2-alpine` - linux; amd64

```console
$ docker pull nats-streaming@sha256:33d7a075703135ba18cf4918fccc35e6fbef1f74ac8bb18abb89a62fde7c4e02
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.4 MB (10404541 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c0d37898667fe6fa6289417167d7e7ce3799d21b08dc0ea4276850e2e8b54b8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:44 GMT
ADD file:762c899ec0505d1a32930ee804c5b008825f41611161be104076cba33b7e5b2b in / 
# Fri, 12 Nov 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Sat, 20 Nov 2021 02:20:53 GMT
ENV NATS_STREAMING_SERVER=0.23.2
# Sat, 20 Nov 2021 02:20:56 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='623cd04855e16ca52694964e01e3b50ded9747a45885bba1a705513da297f6fd' ;; 		armhf) natsArch='arm6'; sha256='fd40f251da335eb7b3cc63b08f8bc0a80d3a4df10fec4efdf6e60417248a5287' ;; 		armv7) natsArch='arm7'; sha256='83db867570654731de98f135f9f373d0758bd9c5a3ee304b65c8128e1d928023' ;; 		x86_64) natsArch='amd64'; sha256='d0c5ebc16901bdc4788d0382dab6f7ce69582e1bafea3ddba159b38ae87b6c81' ;; 		x86) natsArch='386'; sha256='8b9c5396a7747abc8415dc8ca915cf6cb2fd1b79b64ce7a4c3f5efb241cd389f' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Sat, 20 Nov 2021 02:20:56 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Sat, 20 Nov 2021 02:20:56 GMT
EXPOSE 4222 8222
# Sat, 20 Nov 2021 02:20:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 20 Nov 2021 02:20:57 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:97518928ae5f3d52d4164b314a7e73654eb686ecd8aafa0b79acd980773a740d`  
		Last Modified: Fri, 12 Nov 2021 17:20:39 GMT  
		Size: 2.8 MB (2822981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b719fc3addd4e8cc595271456fe9f9de32955502a0f0cadd27a40bfdce67cdf9`  
		Last Modified: Sat, 20 Nov 2021 02:21:41 GMT  
		Size: 7.6 MB (7581138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ae16eed54939fd32b16d2ffcc1ac1e816da3a11b3656bf2344d9d3180173bf5`  
		Last Modified: Sat, 20 Nov 2021 02:21:39 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.23.2-alpine` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:983f8ac2dbbaa85241dbc5508ee63b554e7ac9952787ddb8c11565fe8fa6f89d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.7 MB (9694130 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6428fa782d5b97614b699deec16e4b3715fe3df66e91d7c27b27104a5534c9f0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 12 Nov 2021 16:49:42 GMT
ADD file:6daf1fe862c00673bf9cf4d7e20b0bf253a56e7fb8ed5e730a4466ab9186e18a in / 
# Fri, 12 Nov 2021 16:49:44 GMT
CMD ["/bin/sh"]
# Fri, 19 Nov 2021 23:49:35 GMT
ENV NATS_STREAMING_SERVER=0.23.2
# Fri, 19 Nov 2021 23:49:40 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='623cd04855e16ca52694964e01e3b50ded9747a45885bba1a705513da297f6fd' ;; 		armhf) natsArch='arm6'; sha256='fd40f251da335eb7b3cc63b08f8bc0a80d3a4df10fec4efdf6e60417248a5287' ;; 		armv7) natsArch='arm7'; sha256='83db867570654731de98f135f9f373d0758bd9c5a3ee304b65c8128e1d928023' ;; 		x86_64) natsArch='amd64'; sha256='d0c5ebc16901bdc4788d0382dab6f7ce69582e1bafea3ddba159b38ae87b6c81' ;; 		x86) natsArch='386'; sha256='8b9c5396a7747abc8415dc8ca915cf6cb2fd1b79b64ce7a4c3f5efb241cd389f' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Fri, 19 Nov 2021 23:49:40 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Fri, 19 Nov 2021 23:49:41 GMT
EXPOSE 4222 8222
# Fri, 19 Nov 2021 23:49:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 19 Nov 2021 23:49:42 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:56afcfda5d78cc243287acbaad250c5e8c0f47aae620dd7c51985b0d3c9b2728`  
		Last Modified: Fri, 12 Nov 2021 16:51:32 GMT  
		Size: 2.6 MB (2635392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:824cebd74c6dc7b249f375f4f8b9b003e37db5170f8a26342ed408ae5f39da31`  
		Last Modified: Fri, 19 Nov 2021 23:51:24 GMT  
		Size: 7.1 MB (7058316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba898a9271af9b0a02e91bab485a625e6bba3437f8ed1953bd6497c5a6fee966`  
		Last Modified: Fri, 19 Nov 2021 23:51:19 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.23.2-alpine` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:8d102ba94dd539c86ae564d1671562cd9687b6001ef28c0a3b9358a31b395259
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.5 MB (9487244 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7fe704390d0d6f143b4d58b95fdb72ffd4050dc343669fad7792a25bbd8fc6ae`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 12 Nov 2021 16:57:35 GMT
ADD file:03e0720458c3475758bf4394afa56f2165198eb91e6e9581f7768e433744dd9b in / 
# Fri, 12 Nov 2021 16:57:36 GMT
CMD ["/bin/sh"]
# Sat, 20 Nov 2021 02:33:41 GMT
ENV NATS_STREAMING_SERVER=0.23.2
# Sat, 20 Nov 2021 02:33:46 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='623cd04855e16ca52694964e01e3b50ded9747a45885bba1a705513da297f6fd' ;; 		armhf) natsArch='arm6'; sha256='fd40f251da335eb7b3cc63b08f8bc0a80d3a4df10fec4efdf6e60417248a5287' ;; 		armv7) natsArch='arm7'; sha256='83db867570654731de98f135f9f373d0758bd9c5a3ee304b65c8128e1d928023' ;; 		x86_64) natsArch='amd64'; sha256='d0c5ebc16901bdc4788d0382dab6f7ce69582e1bafea3ddba159b38ae87b6c81' ;; 		x86) natsArch='386'; sha256='8b9c5396a7747abc8415dc8ca915cf6cb2fd1b79b64ce7a4c3f5efb241cd389f' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Sat, 20 Nov 2021 02:33:46 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Sat, 20 Nov 2021 02:33:47 GMT
EXPOSE 4222 8222
# Sat, 20 Nov 2021 02:33:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 20 Nov 2021 02:33:47 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:764d2e53e1a607f2d8261522185d5b9021ade3ec1a595664ee90308c00176899`  
		Last Modified: Fri, 12 Nov 2021 16:59:33 GMT  
		Size: 2.4 MB (2438618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d09b93296bc34cee4aad9d52835eae7e820697f4e8ce382165efb96a8901ea0c`  
		Last Modified: Sat, 20 Nov 2021 02:35:32 GMT  
		Size: 7.0 MB (7048204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:437c793edf6a99d693922586d1182b7f23998316f40d7f5f9e9c74fca0561094`  
		Last Modified: Sat, 20 Nov 2021 02:35:27 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.23.2-alpine` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:c87eb1e5ff911b6ca53a44595f294a4e79baef015629cd41355e25a3bcbebffc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.7 MB (9669856 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89205df0bff2640b3f02b3d8eddbce0582d123a8e34ae55fa68fb034b4e42bb4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 12 Nov 2021 16:39:58 GMT
ADD file:400c0466b29ccad54e0f6c0acef22542992828678c96693ef1f9f4d0551935d8 in / 
# Fri, 12 Nov 2021 16:39:58 GMT
CMD ["/bin/sh"]
# Sat, 20 Nov 2021 04:20:45 GMT
ENV NATS_STREAMING_SERVER=0.23.2
# Sat, 20 Nov 2021 04:20:49 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='623cd04855e16ca52694964e01e3b50ded9747a45885bba1a705513da297f6fd' ;; 		armhf) natsArch='arm6'; sha256='fd40f251da335eb7b3cc63b08f8bc0a80d3a4df10fec4efdf6e60417248a5287' ;; 		armv7) natsArch='arm7'; sha256='83db867570654731de98f135f9f373d0758bd9c5a3ee304b65c8128e1d928023' ;; 		x86_64) natsArch='amd64'; sha256='d0c5ebc16901bdc4788d0382dab6f7ce69582e1bafea3ddba159b38ae87b6c81' ;; 		x86) natsArch='386'; sha256='8b9c5396a7747abc8415dc8ca915cf6cb2fd1b79b64ce7a4c3f5efb241cd389f' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Sat, 20 Nov 2021 04:20:50 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Sat, 20 Nov 2021 04:20:50 GMT
EXPOSE 4222 8222
# Sat, 20 Nov 2021 04:20:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 20 Nov 2021 04:20:52 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:be307f383ecc62b27a29b599c3fc9d3129693a798e7fcce614f09174cfe2d354`  
		Last Modified: Fri, 12 Nov 2021 16:40:59 GMT  
		Size: 2.7 MB (2717700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a942eeaa58bb70c5a728104921dad38ccc6d39aca7c779aa1431c751506e6ab`  
		Last Modified: Sat, 20 Nov 2021 04:21:41 GMT  
		Size: 7.0 MB (6951735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd89828a2f02db651c46db6cbf2f637d36ecc30f847933336bb73135367cd013`  
		Last Modified: Sat, 20 Nov 2021 04:21:40 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.23.2-alpine3.14`

```console
$ docker pull nats-streaming@sha256:1c78a54f4963d1eff5a6bd8759a20b2336a5e300fcf5f62611101679c61e7d11
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.23.2-alpine3.14` - linux; amd64

```console
$ docker pull nats-streaming@sha256:33d7a075703135ba18cf4918fccc35e6fbef1f74ac8bb18abb89a62fde7c4e02
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.4 MB (10404541 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c0d37898667fe6fa6289417167d7e7ce3799d21b08dc0ea4276850e2e8b54b8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:44 GMT
ADD file:762c899ec0505d1a32930ee804c5b008825f41611161be104076cba33b7e5b2b in / 
# Fri, 12 Nov 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Sat, 20 Nov 2021 02:20:53 GMT
ENV NATS_STREAMING_SERVER=0.23.2
# Sat, 20 Nov 2021 02:20:56 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='623cd04855e16ca52694964e01e3b50ded9747a45885bba1a705513da297f6fd' ;; 		armhf) natsArch='arm6'; sha256='fd40f251da335eb7b3cc63b08f8bc0a80d3a4df10fec4efdf6e60417248a5287' ;; 		armv7) natsArch='arm7'; sha256='83db867570654731de98f135f9f373d0758bd9c5a3ee304b65c8128e1d928023' ;; 		x86_64) natsArch='amd64'; sha256='d0c5ebc16901bdc4788d0382dab6f7ce69582e1bafea3ddba159b38ae87b6c81' ;; 		x86) natsArch='386'; sha256='8b9c5396a7747abc8415dc8ca915cf6cb2fd1b79b64ce7a4c3f5efb241cd389f' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Sat, 20 Nov 2021 02:20:56 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Sat, 20 Nov 2021 02:20:56 GMT
EXPOSE 4222 8222
# Sat, 20 Nov 2021 02:20:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 20 Nov 2021 02:20:57 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:97518928ae5f3d52d4164b314a7e73654eb686ecd8aafa0b79acd980773a740d`  
		Last Modified: Fri, 12 Nov 2021 17:20:39 GMT  
		Size: 2.8 MB (2822981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b719fc3addd4e8cc595271456fe9f9de32955502a0f0cadd27a40bfdce67cdf9`  
		Last Modified: Sat, 20 Nov 2021 02:21:41 GMT  
		Size: 7.6 MB (7581138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ae16eed54939fd32b16d2ffcc1ac1e816da3a11b3656bf2344d9d3180173bf5`  
		Last Modified: Sat, 20 Nov 2021 02:21:39 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.23.2-alpine3.14` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:983f8ac2dbbaa85241dbc5508ee63b554e7ac9952787ddb8c11565fe8fa6f89d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.7 MB (9694130 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6428fa782d5b97614b699deec16e4b3715fe3df66e91d7c27b27104a5534c9f0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 12 Nov 2021 16:49:42 GMT
ADD file:6daf1fe862c00673bf9cf4d7e20b0bf253a56e7fb8ed5e730a4466ab9186e18a in / 
# Fri, 12 Nov 2021 16:49:44 GMT
CMD ["/bin/sh"]
# Fri, 19 Nov 2021 23:49:35 GMT
ENV NATS_STREAMING_SERVER=0.23.2
# Fri, 19 Nov 2021 23:49:40 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='623cd04855e16ca52694964e01e3b50ded9747a45885bba1a705513da297f6fd' ;; 		armhf) natsArch='arm6'; sha256='fd40f251da335eb7b3cc63b08f8bc0a80d3a4df10fec4efdf6e60417248a5287' ;; 		armv7) natsArch='arm7'; sha256='83db867570654731de98f135f9f373d0758bd9c5a3ee304b65c8128e1d928023' ;; 		x86_64) natsArch='amd64'; sha256='d0c5ebc16901bdc4788d0382dab6f7ce69582e1bafea3ddba159b38ae87b6c81' ;; 		x86) natsArch='386'; sha256='8b9c5396a7747abc8415dc8ca915cf6cb2fd1b79b64ce7a4c3f5efb241cd389f' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Fri, 19 Nov 2021 23:49:40 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Fri, 19 Nov 2021 23:49:41 GMT
EXPOSE 4222 8222
# Fri, 19 Nov 2021 23:49:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 19 Nov 2021 23:49:42 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:56afcfda5d78cc243287acbaad250c5e8c0f47aae620dd7c51985b0d3c9b2728`  
		Last Modified: Fri, 12 Nov 2021 16:51:32 GMT  
		Size: 2.6 MB (2635392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:824cebd74c6dc7b249f375f4f8b9b003e37db5170f8a26342ed408ae5f39da31`  
		Last Modified: Fri, 19 Nov 2021 23:51:24 GMT  
		Size: 7.1 MB (7058316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba898a9271af9b0a02e91bab485a625e6bba3437f8ed1953bd6497c5a6fee966`  
		Last Modified: Fri, 19 Nov 2021 23:51:19 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.23.2-alpine3.14` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:8d102ba94dd539c86ae564d1671562cd9687b6001ef28c0a3b9358a31b395259
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.5 MB (9487244 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7fe704390d0d6f143b4d58b95fdb72ffd4050dc343669fad7792a25bbd8fc6ae`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 12 Nov 2021 16:57:35 GMT
ADD file:03e0720458c3475758bf4394afa56f2165198eb91e6e9581f7768e433744dd9b in / 
# Fri, 12 Nov 2021 16:57:36 GMT
CMD ["/bin/sh"]
# Sat, 20 Nov 2021 02:33:41 GMT
ENV NATS_STREAMING_SERVER=0.23.2
# Sat, 20 Nov 2021 02:33:46 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='623cd04855e16ca52694964e01e3b50ded9747a45885bba1a705513da297f6fd' ;; 		armhf) natsArch='arm6'; sha256='fd40f251da335eb7b3cc63b08f8bc0a80d3a4df10fec4efdf6e60417248a5287' ;; 		armv7) natsArch='arm7'; sha256='83db867570654731de98f135f9f373d0758bd9c5a3ee304b65c8128e1d928023' ;; 		x86_64) natsArch='amd64'; sha256='d0c5ebc16901bdc4788d0382dab6f7ce69582e1bafea3ddba159b38ae87b6c81' ;; 		x86) natsArch='386'; sha256='8b9c5396a7747abc8415dc8ca915cf6cb2fd1b79b64ce7a4c3f5efb241cd389f' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Sat, 20 Nov 2021 02:33:46 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Sat, 20 Nov 2021 02:33:47 GMT
EXPOSE 4222 8222
# Sat, 20 Nov 2021 02:33:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 20 Nov 2021 02:33:47 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:764d2e53e1a607f2d8261522185d5b9021ade3ec1a595664ee90308c00176899`  
		Last Modified: Fri, 12 Nov 2021 16:59:33 GMT  
		Size: 2.4 MB (2438618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d09b93296bc34cee4aad9d52835eae7e820697f4e8ce382165efb96a8901ea0c`  
		Last Modified: Sat, 20 Nov 2021 02:35:32 GMT  
		Size: 7.0 MB (7048204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:437c793edf6a99d693922586d1182b7f23998316f40d7f5f9e9c74fca0561094`  
		Last Modified: Sat, 20 Nov 2021 02:35:27 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.23.2-alpine3.14` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:c87eb1e5ff911b6ca53a44595f294a4e79baef015629cd41355e25a3bcbebffc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.7 MB (9669856 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89205df0bff2640b3f02b3d8eddbce0582d123a8e34ae55fa68fb034b4e42bb4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 12 Nov 2021 16:39:58 GMT
ADD file:400c0466b29ccad54e0f6c0acef22542992828678c96693ef1f9f4d0551935d8 in / 
# Fri, 12 Nov 2021 16:39:58 GMT
CMD ["/bin/sh"]
# Sat, 20 Nov 2021 04:20:45 GMT
ENV NATS_STREAMING_SERVER=0.23.2
# Sat, 20 Nov 2021 04:20:49 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='623cd04855e16ca52694964e01e3b50ded9747a45885bba1a705513da297f6fd' ;; 		armhf) natsArch='arm6'; sha256='fd40f251da335eb7b3cc63b08f8bc0a80d3a4df10fec4efdf6e60417248a5287' ;; 		armv7) natsArch='arm7'; sha256='83db867570654731de98f135f9f373d0758bd9c5a3ee304b65c8128e1d928023' ;; 		x86_64) natsArch='amd64'; sha256='d0c5ebc16901bdc4788d0382dab6f7ce69582e1bafea3ddba159b38ae87b6c81' ;; 		x86) natsArch='386'; sha256='8b9c5396a7747abc8415dc8ca915cf6cb2fd1b79b64ce7a4c3f5efb241cd389f' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Sat, 20 Nov 2021 04:20:50 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Sat, 20 Nov 2021 04:20:50 GMT
EXPOSE 4222 8222
# Sat, 20 Nov 2021 04:20:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 20 Nov 2021 04:20:52 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:be307f383ecc62b27a29b599c3fc9d3129693a798e7fcce614f09174cfe2d354`  
		Last Modified: Fri, 12 Nov 2021 16:40:59 GMT  
		Size: 2.7 MB (2717700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a942eeaa58bb70c5a728104921dad38ccc6d39aca7c779aa1431c751506e6ab`  
		Last Modified: Sat, 20 Nov 2021 04:21:41 GMT  
		Size: 7.0 MB (6951735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd89828a2f02db651c46db6cbf2f637d36ecc30f847933336bb73135367cd013`  
		Last Modified: Sat, 20 Nov 2021 04:21:40 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.23.2-linux`

```console
$ docker pull nats-streaming@sha256:a80b4649e47eb1640ead441ff67bb621bffc4cecd39041fa6e9802fbdd9b3760
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.23.2-linux` - linux; amd64

```console
$ docker pull nats-streaming@sha256:05a387b6bd267efd7806a67b7b4d431d054e69537a8dd00f0a874e71b48be7e1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7299150 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e1cf392bf11cb1f2dac51f4d09fa86f69859583c3ac7d4812f6c1887d485073`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Sat, 20 Nov 2021 02:21:16 GMT
COPY file:430b600f51b8ec2b8032b9ee2b54a3f23458b67e7fcd26e03d4a1c4fb292e8e3 in /nats-streaming-server 
# Sat, 20 Nov 2021 02:21:16 GMT
EXPOSE 4222 8222
# Sat, 20 Nov 2021 02:21:16 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Sat, 20 Nov 2021 02:21:17 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:ea39d064fdb9df476b776a2728cf769791a02b09590387975647243e2266b1ca`  
		Last Modified: Sat, 20 Nov 2021 02:22:01 GMT  
		Size: 7.3 MB (7299150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.23.2-linux` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:0c1a07390ec1c002d89b5bcd0d0048c95f33f859d53b607ffdc16678e3f79bd8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6774516 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1392e1316cac3fc870ec9cd90c7973466ed1433895aee0166a624b060262b6b5`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Fri, 19 Nov 2021 23:50:00 GMT
COPY file:d86d6a12a47b28bc562444b508d1508f4f436aa57b4f9785d2f72f13991058d9 in /nats-streaming-server 
# Fri, 19 Nov 2021 23:50:00 GMT
EXPOSE 4222 8222
# Fri, 19 Nov 2021 23:50:01 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Fri, 19 Nov 2021 23:50:01 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:ada5d2acf52444276ec7168ad03307d61f3ac5bb2e33825f280ba40e265f0533`  
		Last Modified: Fri, 19 Nov 2021 23:51:55 GMT  
		Size: 6.8 MB (6774516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.23.2-linux` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:cf7abf017ca4b10bcc16492ee29f54f9901fc6c40ae0e5eeba35423ce4346312
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6763075 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4f2b939f92968d68a30b61db2b05fae78f9b7545fb1060ebb0c535069d2a6e0`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Sat, 20 Nov 2021 02:34:09 GMT
COPY file:f737534371c307ebba33d860a23821186a07bfe6bac93b4f8db1052afabca519 in /nats-streaming-server 
# Sat, 20 Nov 2021 02:34:09 GMT
EXPOSE 4222 8222
# Sat, 20 Nov 2021 02:34:10 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Sat, 20 Nov 2021 02:34:10 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:f09d0d006743cce0f69db665ba3e97775e3e7ec87b782222a87b0e299de7abdd`  
		Last Modified: Sat, 20 Nov 2021 02:36:04 GMT  
		Size: 6.8 MB (6763075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.23.2-linux` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:62364f60027f7c3607653a956cf2578021f20431d07038537298bd2e053f622d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.7 MB (6666709 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e200b7f1afcc145455136db22812cb59ac4b91d3018f34d80f3df1980798dfa`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Sat, 20 Nov 2021 04:21:01 GMT
COPY file:758facc101ea28c799c8630223bb78d0e4182d429b666642665350bc7a40a28d in /nats-streaming-server 
# Sat, 20 Nov 2021 04:21:01 GMT
EXPOSE 4222 8222
# Sat, 20 Nov 2021 04:21:02 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Sat, 20 Nov 2021 04:21:03 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:372c129ce02fe71df79c38000ee3af5425ca18626def1095c58ab7c9cc6a31a8`  
		Last Modified: Sat, 20 Nov 2021 04:22:04 GMT  
		Size: 6.7 MB (6666709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.23.2-nanoserver`

```console
$ docker pull nats-streaming@sha256:3deb3e84ece2e334a28e4b46853567baf661fb0d6e9965cb297783565c5c96c9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2452; amd64

### `nats-streaming:0.23.2-nanoserver` - windows version 10.0.17763.2452; amd64

```console
$ docker pull nats-streaming@sha256:e5a5c9eee1f4f76f236ebf6a7049dd1956e9db04ae49b2b50c960eb7b51bfb17
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.5 MB (110458174 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86f5bfb309b8634f75a1184a8b349dc72fbe6750e195fa87c4ee3b7220ebc253`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Fri, 07 Jan 2022 22:25:06 GMT
RUN Apply image 1809-amd64
# Wed, 12 Jan 2022 15:13:42 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 12 Jan 2022 16:36:12 GMT
RUN cmd /S /C #(nop) COPY file:bb30895f60b97f75adc45bbc64dd23d70df079c19ad26c4f8d07ce1c88e77c96 in C:\nats-streaming-server.exe 
# Wed, 12 Jan 2022 16:36:13 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 12 Jan 2022 16:36:14 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 12 Jan 2022 16:36:15 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:3a78847ea829208edc2d7b320b7e602b9d12e47689499d5180a9cc7790dec4d7`  
		Size: 103.0 MB (103031066 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:db05d2e76671d91772a070867bf6f050343319070602a0f8239706d5d4d98387`  
		Last Modified: Wed, 12 Jan 2022 15:14:49 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60d32b598636a5d24f0e2fed2dcea425de4fb29e48ffe747b16de7d34ba96d44`  
		Last Modified: Wed, 12 Jan 2022 16:37:10 GMT  
		Size: 7.4 MB (7422473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:655251a8c00e62468ac138e6498ed5003026017f9e3aaa8a0890c8e4573e3e5d`  
		Last Modified: Wed, 12 Jan 2022 16:37:02 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99ce1684628b1c7cadb6b52866c3be12d063636d962797df7454acc55806596d`  
		Last Modified: Wed, 12 Jan 2022 16:37:02 GMT  
		Size: 1.2 KB (1161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:489b687ddd94c7a64a680862d4341e41ad8fd93a41455a22da84feac26690169`  
		Last Modified: Wed, 12 Jan 2022 16:37:02 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.23.2-nanoserver-1809`

```console
$ docker pull nats-streaming@sha256:3deb3e84ece2e334a28e4b46853567baf661fb0d6e9965cb297783565c5c96c9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2452; amd64

### `nats-streaming:0.23.2-nanoserver-1809` - windows version 10.0.17763.2452; amd64

```console
$ docker pull nats-streaming@sha256:e5a5c9eee1f4f76f236ebf6a7049dd1956e9db04ae49b2b50c960eb7b51bfb17
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.5 MB (110458174 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86f5bfb309b8634f75a1184a8b349dc72fbe6750e195fa87c4ee3b7220ebc253`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Fri, 07 Jan 2022 22:25:06 GMT
RUN Apply image 1809-amd64
# Wed, 12 Jan 2022 15:13:42 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 12 Jan 2022 16:36:12 GMT
RUN cmd /S /C #(nop) COPY file:bb30895f60b97f75adc45bbc64dd23d70df079c19ad26c4f8d07ce1c88e77c96 in C:\nats-streaming-server.exe 
# Wed, 12 Jan 2022 16:36:13 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 12 Jan 2022 16:36:14 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 12 Jan 2022 16:36:15 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:3a78847ea829208edc2d7b320b7e602b9d12e47689499d5180a9cc7790dec4d7`  
		Size: 103.0 MB (103031066 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:db05d2e76671d91772a070867bf6f050343319070602a0f8239706d5d4d98387`  
		Last Modified: Wed, 12 Jan 2022 15:14:49 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60d32b598636a5d24f0e2fed2dcea425de4fb29e48ffe747b16de7d34ba96d44`  
		Last Modified: Wed, 12 Jan 2022 16:37:10 GMT  
		Size: 7.4 MB (7422473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:655251a8c00e62468ac138e6498ed5003026017f9e3aaa8a0890c8e4573e3e5d`  
		Last Modified: Wed, 12 Jan 2022 16:37:02 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99ce1684628b1c7cadb6b52866c3be12d063636d962797df7454acc55806596d`  
		Last Modified: Wed, 12 Jan 2022 16:37:02 GMT  
		Size: 1.2 KB (1161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:489b687ddd94c7a64a680862d4341e41ad8fd93a41455a22da84feac26690169`  
		Last Modified: Wed, 12 Jan 2022 16:37:02 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.23.2-scratch`

```console
$ docker pull nats-streaming@sha256:a80b4649e47eb1640ead441ff67bb621bffc4cecd39041fa6e9802fbdd9b3760
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.23.2-scratch` - linux; amd64

```console
$ docker pull nats-streaming@sha256:05a387b6bd267efd7806a67b7b4d431d054e69537a8dd00f0a874e71b48be7e1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7299150 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e1cf392bf11cb1f2dac51f4d09fa86f69859583c3ac7d4812f6c1887d485073`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Sat, 20 Nov 2021 02:21:16 GMT
COPY file:430b600f51b8ec2b8032b9ee2b54a3f23458b67e7fcd26e03d4a1c4fb292e8e3 in /nats-streaming-server 
# Sat, 20 Nov 2021 02:21:16 GMT
EXPOSE 4222 8222
# Sat, 20 Nov 2021 02:21:16 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Sat, 20 Nov 2021 02:21:17 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:ea39d064fdb9df476b776a2728cf769791a02b09590387975647243e2266b1ca`  
		Last Modified: Sat, 20 Nov 2021 02:22:01 GMT  
		Size: 7.3 MB (7299150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.23.2-scratch` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:0c1a07390ec1c002d89b5bcd0d0048c95f33f859d53b607ffdc16678e3f79bd8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6774516 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1392e1316cac3fc870ec9cd90c7973466ed1433895aee0166a624b060262b6b5`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Fri, 19 Nov 2021 23:50:00 GMT
COPY file:d86d6a12a47b28bc562444b508d1508f4f436aa57b4f9785d2f72f13991058d9 in /nats-streaming-server 
# Fri, 19 Nov 2021 23:50:00 GMT
EXPOSE 4222 8222
# Fri, 19 Nov 2021 23:50:01 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Fri, 19 Nov 2021 23:50:01 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:ada5d2acf52444276ec7168ad03307d61f3ac5bb2e33825f280ba40e265f0533`  
		Last Modified: Fri, 19 Nov 2021 23:51:55 GMT  
		Size: 6.8 MB (6774516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.23.2-scratch` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:cf7abf017ca4b10bcc16492ee29f54f9901fc6c40ae0e5eeba35423ce4346312
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6763075 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4f2b939f92968d68a30b61db2b05fae78f9b7545fb1060ebb0c535069d2a6e0`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Sat, 20 Nov 2021 02:34:09 GMT
COPY file:f737534371c307ebba33d860a23821186a07bfe6bac93b4f8db1052afabca519 in /nats-streaming-server 
# Sat, 20 Nov 2021 02:34:09 GMT
EXPOSE 4222 8222
# Sat, 20 Nov 2021 02:34:10 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Sat, 20 Nov 2021 02:34:10 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:f09d0d006743cce0f69db665ba3e97775e3e7ec87b782222a87b0e299de7abdd`  
		Last Modified: Sat, 20 Nov 2021 02:36:04 GMT  
		Size: 6.8 MB (6763075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.23.2-scratch` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:62364f60027f7c3607653a956cf2578021f20431d07038537298bd2e053f622d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.7 MB (6666709 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e200b7f1afcc145455136db22812cb59ac4b91d3018f34d80f3df1980798dfa`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Sat, 20 Nov 2021 04:21:01 GMT
COPY file:758facc101ea28c799c8630223bb78d0e4182d429b666642665350bc7a40a28d in /nats-streaming-server 
# Sat, 20 Nov 2021 04:21:01 GMT
EXPOSE 4222 8222
# Sat, 20 Nov 2021 04:21:02 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Sat, 20 Nov 2021 04:21:03 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:372c129ce02fe71df79c38000ee3af5425ca18626def1095c58ab7c9cc6a31a8`  
		Last Modified: Sat, 20 Nov 2021 04:22:04 GMT  
		Size: 6.7 MB (6666709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.23.2-windowsservercore`

```console
$ docker pull nats-streaming@sha256:60cddb85b5f5991f1e6bcf9b251048c924b7c717f62b1d49a5d7dbf3164f91a9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.2452; amd64
	-	windows version 10.0.14393.4886; amd64

### `nats-streaming:0.23.2-windowsservercore` - windows version 10.0.17763.2452; amd64

```console
$ docker pull nats-streaming@sha256:b7bd0b03c112bb6a886fc32de7f1416d9a8226341c7425a95714b893c064dabf
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2720323552 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6cf92bdf78d0e103b0277b51786c36629cfd72167d13e7e9e08b399b2a8167b3`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
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
# Wed, 12 Jan 2022 16:33:12 GMT
ENV NATS_STREAMING_SERVER=0.23.2
# Wed, 12 Jan 2022 16:33:13 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.23.2/nats-streaming-server-v0.23.2-windows-amd64.zip
# Wed, 12 Jan 2022 16:33:14 GMT
ENV NATS_STREAMING_SERVER_SHASUM=b28dc8e1565d6fece68781515f759b0ed870831cdf2f7925cff7cf9acb44e7ec
# Wed, 12 Jan 2022 16:34:10 GMT
RUN Set-PSDebug -Trace 2
# Wed, 12 Jan 2022 16:35:52 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 12 Jan 2022 16:35:54 GMT
EXPOSE 4222 8222
# Wed, 12 Jan 2022 16:35:55 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 12 Jan 2022 16:35:56 GMT
CMD ["-m" "8222"]
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
	-	`sha256:2e56f267999eb7fd5bcfb301b0f0e6052a8ae22ca628c389db83c562990cf444`  
		Last Modified: Wed, 12 Jan 2022 16:36:50 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:821e8ced70841dc00f55dcd8124121cbb0c430571a5e5d158741fcf29c4eb763`  
		Last Modified: Wed, 12 Jan 2022 16:36:49 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6f67c1564c45a427f773fc0876060b2020ca2453a98023b375fb06c5f53bf3b`  
		Last Modified: Wed, 12 Jan 2022 16:36:49 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:770a7c738c44f07d9a29e8d8cd2ed3ad2f85aa87d7d0bfba1e7efde7ff6c131b`  
		Last Modified: Wed, 12 Jan 2022 16:36:47 GMT  
		Size: 338.5 KB (338485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29ce328ddff49212914bc498c236b2fa59188c0aaa5086dcab210060f4a886f1`  
		Last Modified: Wed, 12 Jan 2022 16:36:50 GMT  
		Size: 7.7 MB (7742962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:091c2e64ef4827cbcb4a216d0422edb3669c90feafeb39b97d344bed44ea4b75`  
		Last Modified: Wed, 12 Jan 2022 16:36:47 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38db1a89341b657073620f8a786ceec8c75be7fc50ccc4a506c364942fa7bc40`  
		Last Modified: Wed, 12 Jan 2022 16:36:47 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1c36c3fb3a835905d4b5ab75dbb3b1e7d580f9723d36b7bf3cf9fcea75f6365`  
		Last Modified: Wed, 12 Jan 2022 16:36:47 GMT  
		Size: 1.4 KB (1381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.23.2-windowsservercore` - windows version 10.0.14393.4886; amd64

```console
$ docker pull nats-streaming@sha256:d55e31a14946b12f1d6c152dfb777ad1b2da038f0c957bde81c5cfb59cd1a97d
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6290824289 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:111095c35ecacfdbe68e1ef364f73124e3888020c1fdffe9c88d2b78bd021fa8`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
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
# Tue, 11 Jan 2022 19:57:41 GMT
ENV NATS_STREAMING_SERVER=0.23.2
# Tue, 11 Jan 2022 19:57:42 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.23.2/nats-streaming-server-v0.23.2-windows-amd64.zip
# Tue, 11 Jan 2022 19:57:43 GMT
ENV NATS_STREAMING_SERVER_SHASUM=b28dc8e1565d6fece68781515f759b0ed870831cdf2f7925cff7cf9acb44e7ec
# Tue, 11 Jan 2022 21:24:39 GMT
RUN Set-PSDebug -Trace 2
# Tue, 11 Jan 2022 21:26:28 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Tue, 11 Jan 2022 21:26:29 GMT
EXPOSE 4222 8222
# Tue, 11 Jan 2022 21:26:31 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Tue, 11 Jan 2022 21:26:32 GMT
CMD ["-m" "8222"]
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
	-	`sha256:b5cf3c8d8140ae38c2d505f95e5babf9f4505d67a6151d6fe3f9c751ef7d0dc5`  
		Last Modified: Tue, 11 Jan 2022 21:27:37 GMT  
		Size: 1.4 KB (1354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19dc2e3eee55193ca6704fc85c6992e8b9b8bd428d80239cd34ee31b8c72fdc5`  
		Last Modified: Tue, 11 Jan 2022 21:27:37 GMT  
		Size: 1.4 KB (1374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92cc106ea2da4cb4db419ee1efe603754ac4e6645cde9bdf6ee8bde96b5e342a`  
		Last Modified: Tue, 11 Jan 2022 21:27:37 GMT  
		Size: 1.4 KB (1363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c19b53c2023c3798cb5b4fb1bf2c6c906c1c9ec3f1a64fe6ca6832b146c5e926`  
		Last Modified: Tue, 11 Jan 2022 21:27:35 GMT  
		Size: 335.6 KB (335575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b49df4cdedb96e996d903b4a909a6204919bef00f7a72eea5fc92c42249b541c`  
		Last Modified: Tue, 11 Jan 2022 21:27:48 GMT  
		Size: 12.3 MB (12274958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf21ee223236021b829cf5aa5a4a19abe4854ed145378b8ca64aed39459a5611`  
		Last Modified: Tue, 11 Jan 2022 21:27:34 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc2ccb79a6a3985e5a419e8c0f1256719adee45c6ab7d7a049e39e42ee798e91`  
		Last Modified: Tue, 11 Jan 2022 21:27:34 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adb13dd255898f881701597b01fa5e3b8873647e6098933da4de040996a6188d`  
		Last Modified: Tue, 11 Jan 2022 21:27:34 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.23.2-windowsservercore-1809`

```console
$ docker pull nats-streaming@sha256:f4205543bce3358dd968000ee86d121344534bfeb34634fce3af7196029e72b1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2452; amd64

### `nats-streaming:0.23.2-windowsservercore-1809` - windows version 10.0.17763.2452; amd64

```console
$ docker pull nats-streaming@sha256:b7bd0b03c112bb6a886fc32de7f1416d9a8226341c7425a95714b893c064dabf
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2720323552 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6cf92bdf78d0e103b0277b51786c36629cfd72167d13e7e9e08b399b2a8167b3`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
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
# Wed, 12 Jan 2022 16:33:12 GMT
ENV NATS_STREAMING_SERVER=0.23.2
# Wed, 12 Jan 2022 16:33:13 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.23.2/nats-streaming-server-v0.23.2-windows-amd64.zip
# Wed, 12 Jan 2022 16:33:14 GMT
ENV NATS_STREAMING_SERVER_SHASUM=b28dc8e1565d6fece68781515f759b0ed870831cdf2f7925cff7cf9acb44e7ec
# Wed, 12 Jan 2022 16:34:10 GMT
RUN Set-PSDebug -Trace 2
# Wed, 12 Jan 2022 16:35:52 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 12 Jan 2022 16:35:54 GMT
EXPOSE 4222 8222
# Wed, 12 Jan 2022 16:35:55 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 12 Jan 2022 16:35:56 GMT
CMD ["-m" "8222"]
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
	-	`sha256:2e56f267999eb7fd5bcfb301b0f0e6052a8ae22ca628c389db83c562990cf444`  
		Last Modified: Wed, 12 Jan 2022 16:36:50 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:821e8ced70841dc00f55dcd8124121cbb0c430571a5e5d158741fcf29c4eb763`  
		Last Modified: Wed, 12 Jan 2022 16:36:49 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6f67c1564c45a427f773fc0876060b2020ca2453a98023b375fb06c5f53bf3b`  
		Last Modified: Wed, 12 Jan 2022 16:36:49 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:770a7c738c44f07d9a29e8d8cd2ed3ad2f85aa87d7d0bfba1e7efde7ff6c131b`  
		Last Modified: Wed, 12 Jan 2022 16:36:47 GMT  
		Size: 338.5 KB (338485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29ce328ddff49212914bc498c236b2fa59188c0aaa5086dcab210060f4a886f1`  
		Last Modified: Wed, 12 Jan 2022 16:36:50 GMT  
		Size: 7.7 MB (7742962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:091c2e64ef4827cbcb4a216d0422edb3669c90feafeb39b97d344bed44ea4b75`  
		Last Modified: Wed, 12 Jan 2022 16:36:47 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38db1a89341b657073620f8a786ceec8c75be7fc50ccc4a506c364942fa7bc40`  
		Last Modified: Wed, 12 Jan 2022 16:36:47 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1c36c3fb3a835905d4b5ab75dbb3b1e7d580f9723d36b7bf3cf9fcea75f6365`  
		Last Modified: Wed, 12 Jan 2022 16:36:47 GMT  
		Size: 1.4 KB (1381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.23.2-windowsservercore-ltsc2016`

```console
$ docker pull nats-streaming@sha256:8d7f645475c1ddf54332ac47ad4daa549c2a02a25e27f3062c39efed087fd0ba
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.14393.4886; amd64

### `nats-streaming:0.23.2-windowsservercore-ltsc2016` - windows version 10.0.14393.4886; amd64

```console
$ docker pull nats-streaming@sha256:d55e31a14946b12f1d6c152dfb777ad1b2da038f0c957bde81c5cfb59cd1a97d
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6290824289 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:111095c35ecacfdbe68e1ef364f73124e3888020c1fdffe9c88d2b78bd021fa8`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
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
# Tue, 11 Jan 2022 19:57:41 GMT
ENV NATS_STREAMING_SERVER=0.23.2
# Tue, 11 Jan 2022 19:57:42 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.23.2/nats-streaming-server-v0.23.2-windows-amd64.zip
# Tue, 11 Jan 2022 19:57:43 GMT
ENV NATS_STREAMING_SERVER_SHASUM=b28dc8e1565d6fece68781515f759b0ed870831cdf2f7925cff7cf9acb44e7ec
# Tue, 11 Jan 2022 21:24:39 GMT
RUN Set-PSDebug -Trace 2
# Tue, 11 Jan 2022 21:26:28 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Tue, 11 Jan 2022 21:26:29 GMT
EXPOSE 4222 8222
# Tue, 11 Jan 2022 21:26:31 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Tue, 11 Jan 2022 21:26:32 GMT
CMD ["-m" "8222"]
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
	-	`sha256:b5cf3c8d8140ae38c2d505f95e5babf9f4505d67a6151d6fe3f9c751ef7d0dc5`  
		Last Modified: Tue, 11 Jan 2022 21:27:37 GMT  
		Size: 1.4 KB (1354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19dc2e3eee55193ca6704fc85c6992e8b9b8bd428d80239cd34ee31b8c72fdc5`  
		Last Modified: Tue, 11 Jan 2022 21:27:37 GMT  
		Size: 1.4 KB (1374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92cc106ea2da4cb4db419ee1efe603754ac4e6645cde9bdf6ee8bde96b5e342a`  
		Last Modified: Tue, 11 Jan 2022 21:27:37 GMT  
		Size: 1.4 KB (1363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c19b53c2023c3798cb5b4fb1bf2c6c906c1c9ec3f1a64fe6ca6832b146c5e926`  
		Last Modified: Tue, 11 Jan 2022 21:27:35 GMT  
		Size: 335.6 KB (335575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b49df4cdedb96e996d903b4a909a6204919bef00f7a72eea5fc92c42249b541c`  
		Last Modified: Tue, 11 Jan 2022 21:27:48 GMT  
		Size: 12.3 MB (12274958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf21ee223236021b829cf5aa5a4a19abe4854ed145378b8ca64aed39459a5611`  
		Last Modified: Tue, 11 Jan 2022 21:27:34 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc2ccb79a6a3985e5a419e8c0f1256719adee45c6ab7d7a049e39e42ee798e91`  
		Last Modified: Tue, 11 Jan 2022 21:27:34 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adb13dd255898f881701597b01fa5e3b8873647e6098933da4de040996a6188d`  
		Last Modified: Tue, 11 Jan 2022 21:27:34 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:alpine`

```console
$ docker pull nats-streaming@sha256:1c78a54f4963d1eff5a6bd8759a20b2336a5e300fcf5f62611101679c61e7d11
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:alpine` - linux; amd64

```console
$ docker pull nats-streaming@sha256:33d7a075703135ba18cf4918fccc35e6fbef1f74ac8bb18abb89a62fde7c4e02
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.4 MB (10404541 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c0d37898667fe6fa6289417167d7e7ce3799d21b08dc0ea4276850e2e8b54b8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:44 GMT
ADD file:762c899ec0505d1a32930ee804c5b008825f41611161be104076cba33b7e5b2b in / 
# Fri, 12 Nov 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Sat, 20 Nov 2021 02:20:53 GMT
ENV NATS_STREAMING_SERVER=0.23.2
# Sat, 20 Nov 2021 02:20:56 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='623cd04855e16ca52694964e01e3b50ded9747a45885bba1a705513da297f6fd' ;; 		armhf) natsArch='arm6'; sha256='fd40f251da335eb7b3cc63b08f8bc0a80d3a4df10fec4efdf6e60417248a5287' ;; 		armv7) natsArch='arm7'; sha256='83db867570654731de98f135f9f373d0758bd9c5a3ee304b65c8128e1d928023' ;; 		x86_64) natsArch='amd64'; sha256='d0c5ebc16901bdc4788d0382dab6f7ce69582e1bafea3ddba159b38ae87b6c81' ;; 		x86) natsArch='386'; sha256='8b9c5396a7747abc8415dc8ca915cf6cb2fd1b79b64ce7a4c3f5efb241cd389f' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Sat, 20 Nov 2021 02:20:56 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Sat, 20 Nov 2021 02:20:56 GMT
EXPOSE 4222 8222
# Sat, 20 Nov 2021 02:20:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 20 Nov 2021 02:20:57 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:97518928ae5f3d52d4164b314a7e73654eb686ecd8aafa0b79acd980773a740d`  
		Last Modified: Fri, 12 Nov 2021 17:20:39 GMT  
		Size: 2.8 MB (2822981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b719fc3addd4e8cc595271456fe9f9de32955502a0f0cadd27a40bfdce67cdf9`  
		Last Modified: Sat, 20 Nov 2021 02:21:41 GMT  
		Size: 7.6 MB (7581138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ae16eed54939fd32b16d2ffcc1ac1e816da3a11b3656bf2344d9d3180173bf5`  
		Last Modified: Sat, 20 Nov 2021 02:21:39 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:983f8ac2dbbaa85241dbc5508ee63b554e7ac9952787ddb8c11565fe8fa6f89d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.7 MB (9694130 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6428fa782d5b97614b699deec16e4b3715fe3df66e91d7c27b27104a5534c9f0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 12 Nov 2021 16:49:42 GMT
ADD file:6daf1fe862c00673bf9cf4d7e20b0bf253a56e7fb8ed5e730a4466ab9186e18a in / 
# Fri, 12 Nov 2021 16:49:44 GMT
CMD ["/bin/sh"]
# Fri, 19 Nov 2021 23:49:35 GMT
ENV NATS_STREAMING_SERVER=0.23.2
# Fri, 19 Nov 2021 23:49:40 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='623cd04855e16ca52694964e01e3b50ded9747a45885bba1a705513da297f6fd' ;; 		armhf) natsArch='arm6'; sha256='fd40f251da335eb7b3cc63b08f8bc0a80d3a4df10fec4efdf6e60417248a5287' ;; 		armv7) natsArch='arm7'; sha256='83db867570654731de98f135f9f373d0758bd9c5a3ee304b65c8128e1d928023' ;; 		x86_64) natsArch='amd64'; sha256='d0c5ebc16901bdc4788d0382dab6f7ce69582e1bafea3ddba159b38ae87b6c81' ;; 		x86) natsArch='386'; sha256='8b9c5396a7747abc8415dc8ca915cf6cb2fd1b79b64ce7a4c3f5efb241cd389f' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Fri, 19 Nov 2021 23:49:40 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Fri, 19 Nov 2021 23:49:41 GMT
EXPOSE 4222 8222
# Fri, 19 Nov 2021 23:49:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 19 Nov 2021 23:49:42 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:56afcfda5d78cc243287acbaad250c5e8c0f47aae620dd7c51985b0d3c9b2728`  
		Last Modified: Fri, 12 Nov 2021 16:51:32 GMT  
		Size: 2.6 MB (2635392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:824cebd74c6dc7b249f375f4f8b9b003e37db5170f8a26342ed408ae5f39da31`  
		Last Modified: Fri, 19 Nov 2021 23:51:24 GMT  
		Size: 7.1 MB (7058316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba898a9271af9b0a02e91bab485a625e6bba3437f8ed1953bd6497c5a6fee966`  
		Last Modified: Fri, 19 Nov 2021 23:51:19 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:8d102ba94dd539c86ae564d1671562cd9687b6001ef28c0a3b9358a31b395259
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.5 MB (9487244 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7fe704390d0d6f143b4d58b95fdb72ffd4050dc343669fad7792a25bbd8fc6ae`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 12 Nov 2021 16:57:35 GMT
ADD file:03e0720458c3475758bf4394afa56f2165198eb91e6e9581f7768e433744dd9b in / 
# Fri, 12 Nov 2021 16:57:36 GMT
CMD ["/bin/sh"]
# Sat, 20 Nov 2021 02:33:41 GMT
ENV NATS_STREAMING_SERVER=0.23.2
# Sat, 20 Nov 2021 02:33:46 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='623cd04855e16ca52694964e01e3b50ded9747a45885bba1a705513da297f6fd' ;; 		armhf) natsArch='arm6'; sha256='fd40f251da335eb7b3cc63b08f8bc0a80d3a4df10fec4efdf6e60417248a5287' ;; 		armv7) natsArch='arm7'; sha256='83db867570654731de98f135f9f373d0758bd9c5a3ee304b65c8128e1d928023' ;; 		x86_64) natsArch='amd64'; sha256='d0c5ebc16901bdc4788d0382dab6f7ce69582e1bafea3ddba159b38ae87b6c81' ;; 		x86) natsArch='386'; sha256='8b9c5396a7747abc8415dc8ca915cf6cb2fd1b79b64ce7a4c3f5efb241cd389f' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Sat, 20 Nov 2021 02:33:46 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Sat, 20 Nov 2021 02:33:47 GMT
EXPOSE 4222 8222
# Sat, 20 Nov 2021 02:33:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 20 Nov 2021 02:33:47 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:764d2e53e1a607f2d8261522185d5b9021ade3ec1a595664ee90308c00176899`  
		Last Modified: Fri, 12 Nov 2021 16:59:33 GMT  
		Size: 2.4 MB (2438618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d09b93296bc34cee4aad9d52835eae7e820697f4e8ce382165efb96a8901ea0c`  
		Last Modified: Sat, 20 Nov 2021 02:35:32 GMT  
		Size: 7.0 MB (7048204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:437c793edf6a99d693922586d1182b7f23998316f40d7f5f9e9c74fca0561094`  
		Last Modified: Sat, 20 Nov 2021 02:35:27 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:c87eb1e5ff911b6ca53a44595f294a4e79baef015629cd41355e25a3bcbebffc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.7 MB (9669856 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89205df0bff2640b3f02b3d8eddbce0582d123a8e34ae55fa68fb034b4e42bb4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 12 Nov 2021 16:39:58 GMT
ADD file:400c0466b29ccad54e0f6c0acef22542992828678c96693ef1f9f4d0551935d8 in / 
# Fri, 12 Nov 2021 16:39:58 GMT
CMD ["/bin/sh"]
# Sat, 20 Nov 2021 04:20:45 GMT
ENV NATS_STREAMING_SERVER=0.23.2
# Sat, 20 Nov 2021 04:20:49 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='623cd04855e16ca52694964e01e3b50ded9747a45885bba1a705513da297f6fd' ;; 		armhf) natsArch='arm6'; sha256='fd40f251da335eb7b3cc63b08f8bc0a80d3a4df10fec4efdf6e60417248a5287' ;; 		armv7) natsArch='arm7'; sha256='83db867570654731de98f135f9f373d0758bd9c5a3ee304b65c8128e1d928023' ;; 		x86_64) natsArch='amd64'; sha256='d0c5ebc16901bdc4788d0382dab6f7ce69582e1bafea3ddba159b38ae87b6c81' ;; 		x86) natsArch='386'; sha256='8b9c5396a7747abc8415dc8ca915cf6cb2fd1b79b64ce7a4c3f5efb241cd389f' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Sat, 20 Nov 2021 04:20:50 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Sat, 20 Nov 2021 04:20:50 GMT
EXPOSE 4222 8222
# Sat, 20 Nov 2021 04:20:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 20 Nov 2021 04:20:52 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:be307f383ecc62b27a29b599c3fc9d3129693a798e7fcce614f09174cfe2d354`  
		Last Modified: Fri, 12 Nov 2021 16:40:59 GMT  
		Size: 2.7 MB (2717700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a942eeaa58bb70c5a728104921dad38ccc6d39aca7c779aa1431c751506e6ab`  
		Last Modified: Sat, 20 Nov 2021 04:21:41 GMT  
		Size: 7.0 MB (6951735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd89828a2f02db651c46db6cbf2f637d36ecc30f847933336bb73135367cd013`  
		Last Modified: Sat, 20 Nov 2021 04:21:40 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:alpine3.14`

```console
$ docker pull nats-streaming@sha256:1c78a54f4963d1eff5a6bd8759a20b2336a5e300fcf5f62611101679c61e7d11
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:alpine3.14` - linux; amd64

```console
$ docker pull nats-streaming@sha256:33d7a075703135ba18cf4918fccc35e6fbef1f74ac8bb18abb89a62fde7c4e02
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.4 MB (10404541 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c0d37898667fe6fa6289417167d7e7ce3799d21b08dc0ea4276850e2e8b54b8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:44 GMT
ADD file:762c899ec0505d1a32930ee804c5b008825f41611161be104076cba33b7e5b2b in / 
# Fri, 12 Nov 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Sat, 20 Nov 2021 02:20:53 GMT
ENV NATS_STREAMING_SERVER=0.23.2
# Sat, 20 Nov 2021 02:20:56 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='623cd04855e16ca52694964e01e3b50ded9747a45885bba1a705513da297f6fd' ;; 		armhf) natsArch='arm6'; sha256='fd40f251da335eb7b3cc63b08f8bc0a80d3a4df10fec4efdf6e60417248a5287' ;; 		armv7) natsArch='arm7'; sha256='83db867570654731de98f135f9f373d0758bd9c5a3ee304b65c8128e1d928023' ;; 		x86_64) natsArch='amd64'; sha256='d0c5ebc16901bdc4788d0382dab6f7ce69582e1bafea3ddba159b38ae87b6c81' ;; 		x86) natsArch='386'; sha256='8b9c5396a7747abc8415dc8ca915cf6cb2fd1b79b64ce7a4c3f5efb241cd389f' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Sat, 20 Nov 2021 02:20:56 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Sat, 20 Nov 2021 02:20:56 GMT
EXPOSE 4222 8222
# Sat, 20 Nov 2021 02:20:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 20 Nov 2021 02:20:57 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:97518928ae5f3d52d4164b314a7e73654eb686ecd8aafa0b79acd980773a740d`  
		Last Modified: Fri, 12 Nov 2021 17:20:39 GMT  
		Size: 2.8 MB (2822981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b719fc3addd4e8cc595271456fe9f9de32955502a0f0cadd27a40bfdce67cdf9`  
		Last Modified: Sat, 20 Nov 2021 02:21:41 GMT  
		Size: 7.6 MB (7581138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ae16eed54939fd32b16d2ffcc1ac1e816da3a11b3656bf2344d9d3180173bf5`  
		Last Modified: Sat, 20 Nov 2021 02:21:39 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine3.14` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:983f8ac2dbbaa85241dbc5508ee63b554e7ac9952787ddb8c11565fe8fa6f89d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.7 MB (9694130 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6428fa782d5b97614b699deec16e4b3715fe3df66e91d7c27b27104a5534c9f0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 12 Nov 2021 16:49:42 GMT
ADD file:6daf1fe862c00673bf9cf4d7e20b0bf253a56e7fb8ed5e730a4466ab9186e18a in / 
# Fri, 12 Nov 2021 16:49:44 GMT
CMD ["/bin/sh"]
# Fri, 19 Nov 2021 23:49:35 GMT
ENV NATS_STREAMING_SERVER=0.23.2
# Fri, 19 Nov 2021 23:49:40 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='623cd04855e16ca52694964e01e3b50ded9747a45885bba1a705513da297f6fd' ;; 		armhf) natsArch='arm6'; sha256='fd40f251da335eb7b3cc63b08f8bc0a80d3a4df10fec4efdf6e60417248a5287' ;; 		armv7) natsArch='arm7'; sha256='83db867570654731de98f135f9f373d0758bd9c5a3ee304b65c8128e1d928023' ;; 		x86_64) natsArch='amd64'; sha256='d0c5ebc16901bdc4788d0382dab6f7ce69582e1bafea3ddba159b38ae87b6c81' ;; 		x86) natsArch='386'; sha256='8b9c5396a7747abc8415dc8ca915cf6cb2fd1b79b64ce7a4c3f5efb241cd389f' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Fri, 19 Nov 2021 23:49:40 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Fri, 19 Nov 2021 23:49:41 GMT
EXPOSE 4222 8222
# Fri, 19 Nov 2021 23:49:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 19 Nov 2021 23:49:42 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:56afcfda5d78cc243287acbaad250c5e8c0f47aae620dd7c51985b0d3c9b2728`  
		Last Modified: Fri, 12 Nov 2021 16:51:32 GMT  
		Size: 2.6 MB (2635392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:824cebd74c6dc7b249f375f4f8b9b003e37db5170f8a26342ed408ae5f39da31`  
		Last Modified: Fri, 19 Nov 2021 23:51:24 GMT  
		Size: 7.1 MB (7058316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba898a9271af9b0a02e91bab485a625e6bba3437f8ed1953bd6497c5a6fee966`  
		Last Modified: Fri, 19 Nov 2021 23:51:19 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine3.14` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:8d102ba94dd539c86ae564d1671562cd9687b6001ef28c0a3b9358a31b395259
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.5 MB (9487244 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7fe704390d0d6f143b4d58b95fdb72ffd4050dc343669fad7792a25bbd8fc6ae`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 12 Nov 2021 16:57:35 GMT
ADD file:03e0720458c3475758bf4394afa56f2165198eb91e6e9581f7768e433744dd9b in / 
# Fri, 12 Nov 2021 16:57:36 GMT
CMD ["/bin/sh"]
# Sat, 20 Nov 2021 02:33:41 GMT
ENV NATS_STREAMING_SERVER=0.23.2
# Sat, 20 Nov 2021 02:33:46 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='623cd04855e16ca52694964e01e3b50ded9747a45885bba1a705513da297f6fd' ;; 		armhf) natsArch='arm6'; sha256='fd40f251da335eb7b3cc63b08f8bc0a80d3a4df10fec4efdf6e60417248a5287' ;; 		armv7) natsArch='arm7'; sha256='83db867570654731de98f135f9f373d0758bd9c5a3ee304b65c8128e1d928023' ;; 		x86_64) natsArch='amd64'; sha256='d0c5ebc16901bdc4788d0382dab6f7ce69582e1bafea3ddba159b38ae87b6c81' ;; 		x86) natsArch='386'; sha256='8b9c5396a7747abc8415dc8ca915cf6cb2fd1b79b64ce7a4c3f5efb241cd389f' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Sat, 20 Nov 2021 02:33:46 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Sat, 20 Nov 2021 02:33:47 GMT
EXPOSE 4222 8222
# Sat, 20 Nov 2021 02:33:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 20 Nov 2021 02:33:47 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:764d2e53e1a607f2d8261522185d5b9021ade3ec1a595664ee90308c00176899`  
		Last Modified: Fri, 12 Nov 2021 16:59:33 GMT  
		Size: 2.4 MB (2438618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d09b93296bc34cee4aad9d52835eae7e820697f4e8ce382165efb96a8901ea0c`  
		Last Modified: Sat, 20 Nov 2021 02:35:32 GMT  
		Size: 7.0 MB (7048204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:437c793edf6a99d693922586d1182b7f23998316f40d7f5f9e9c74fca0561094`  
		Last Modified: Sat, 20 Nov 2021 02:35:27 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine3.14` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:c87eb1e5ff911b6ca53a44595f294a4e79baef015629cd41355e25a3bcbebffc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.7 MB (9669856 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89205df0bff2640b3f02b3d8eddbce0582d123a8e34ae55fa68fb034b4e42bb4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 12 Nov 2021 16:39:58 GMT
ADD file:400c0466b29ccad54e0f6c0acef22542992828678c96693ef1f9f4d0551935d8 in / 
# Fri, 12 Nov 2021 16:39:58 GMT
CMD ["/bin/sh"]
# Sat, 20 Nov 2021 04:20:45 GMT
ENV NATS_STREAMING_SERVER=0.23.2
# Sat, 20 Nov 2021 04:20:49 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='623cd04855e16ca52694964e01e3b50ded9747a45885bba1a705513da297f6fd' ;; 		armhf) natsArch='arm6'; sha256='fd40f251da335eb7b3cc63b08f8bc0a80d3a4df10fec4efdf6e60417248a5287' ;; 		armv7) natsArch='arm7'; sha256='83db867570654731de98f135f9f373d0758bd9c5a3ee304b65c8128e1d928023' ;; 		x86_64) natsArch='amd64'; sha256='d0c5ebc16901bdc4788d0382dab6f7ce69582e1bafea3ddba159b38ae87b6c81' ;; 		x86) natsArch='386'; sha256='8b9c5396a7747abc8415dc8ca915cf6cb2fd1b79b64ce7a4c3f5efb241cd389f' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Sat, 20 Nov 2021 04:20:50 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Sat, 20 Nov 2021 04:20:50 GMT
EXPOSE 4222 8222
# Sat, 20 Nov 2021 04:20:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 20 Nov 2021 04:20:52 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:be307f383ecc62b27a29b599c3fc9d3129693a798e7fcce614f09174cfe2d354`  
		Last Modified: Fri, 12 Nov 2021 16:40:59 GMT  
		Size: 2.7 MB (2717700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a942eeaa58bb70c5a728104921dad38ccc6d39aca7c779aa1431c751506e6ab`  
		Last Modified: Sat, 20 Nov 2021 04:21:41 GMT  
		Size: 7.0 MB (6951735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd89828a2f02db651c46db6cbf2f637d36ecc30f847933336bb73135367cd013`  
		Last Modified: Sat, 20 Nov 2021 04:21:40 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:latest`

```console
$ docker pull nats-streaming@sha256:17f569d1c9e1468bbe3a7371279ccde5538ea320fd4ebd94600b904d2e742657
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.2452; amd64

### `nats-streaming:latest` - linux; amd64

```console
$ docker pull nats-streaming@sha256:05a387b6bd267efd7806a67b7b4d431d054e69537a8dd00f0a874e71b48be7e1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7299150 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e1cf392bf11cb1f2dac51f4d09fa86f69859583c3ac7d4812f6c1887d485073`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Sat, 20 Nov 2021 02:21:16 GMT
COPY file:430b600f51b8ec2b8032b9ee2b54a3f23458b67e7fcd26e03d4a1c4fb292e8e3 in /nats-streaming-server 
# Sat, 20 Nov 2021 02:21:16 GMT
EXPOSE 4222 8222
# Sat, 20 Nov 2021 02:21:16 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Sat, 20 Nov 2021 02:21:17 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:ea39d064fdb9df476b776a2728cf769791a02b09590387975647243e2266b1ca`  
		Last Modified: Sat, 20 Nov 2021 02:22:01 GMT  
		Size: 7.3 MB (7299150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:latest` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:0c1a07390ec1c002d89b5bcd0d0048c95f33f859d53b607ffdc16678e3f79bd8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6774516 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1392e1316cac3fc870ec9cd90c7973466ed1433895aee0166a624b060262b6b5`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Fri, 19 Nov 2021 23:50:00 GMT
COPY file:d86d6a12a47b28bc562444b508d1508f4f436aa57b4f9785d2f72f13991058d9 in /nats-streaming-server 
# Fri, 19 Nov 2021 23:50:00 GMT
EXPOSE 4222 8222
# Fri, 19 Nov 2021 23:50:01 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Fri, 19 Nov 2021 23:50:01 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:ada5d2acf52444276ec7168ad03307d61f3ac5bb2e33825f280ba40e265f0533`  
		Last Modified: Fri, 19 Nov 2021 23:51:55 GMT  
		Size: 6.8 MB (6774516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:latest` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:cf7abf017ca4b10bcc16492ee29f54f9901fc6c40ae0e5eeba35423ce4346312
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6763075 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4f2b939f92968d68a30b61db2b05fae78f9b7545fb1060ebb0c535069d2a6e0`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Sat, 20 Nov 2021 02:34:09 GMT
COPY file:f737534371c307ebba33d860a23821186a07bfe6bac93b4f8db1052afabca519 in /nats-streaming-server 
# Sat, 20 Nov 2021 02:34:09 GMT
EXPOSE 4222 8222
# Sat, 20 Nov 2021 02:34:10 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Sat, 20 Nov 2021 02:34:10 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:f09d0d006743cce0f69db665ba3e97775e3e7ec87b782222a87b0e299de7abdd`  
		Last Modified: Sat, 20 Nov 2021 02:36:04 GMT  
		Size: 6.8 MB (6763075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:latest` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:62364f60027f7c3607653a956cf2578021f20431d07038537298bd2e053f622d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.7 MB (6666709 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e200b7f1afcc145455136db22812cb59ac4b91d3018f34d80f3df1980798dfa`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Sat, 20 Nov 2021 04:21:01 GMT
COPY file:758facc101ea28c799c8630223bb78d0e4182d429b666642665350bc7a40a28d in /nats-streaming-server 
# Sat, 20 Nov 2021 04:21:01 GMT
EXPOSE 4222 8222
# Sat, 20 Nov 2021 04:21:02 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Sat, 20 Nov 2021 04:21:03 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:372c129ce02fe71df79c38000ee3af5425ca18626def1095c58ab7c9cc6a31a8`  
		Last Modified: Sat, 20 Nov 2021 04:22:04 GMT  
		Size: 6.7 MB (6666709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:latest` - windows version 10.0.17763.2452; amd64

```console
$ docker pull nats-streaming@sha256:e5a5c9eee1f4f76f236ebf6a7049dd1956e9db04ae49b2b50c960eb7b51bfb17
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.5 MB (110458174 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86f5bfb309b8634f75a1184a8b349dc72fbe6750e195fa87c4ee3b7220ebc253`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Fri, 07 Jan 2022 22:25:06 GMT
RUN Apply image 1809-amd64
# Wed, 12 Jan 2022 15:13:42 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 12 Jan 2022 16:36:12 GMT
RUN cmd /S /C #(nop) COPY file:bb30895f60b97f75adc45bbc64dd23d70df079c19ad26c4f8d07ce1c88e77c96 in C:\nats-streaming-server.exe 
# Wed, 12 Jan 2022 16:36:13 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 12 Jan 2022 16:36:14 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 12 Jan 2022 16:36:15 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:3a78847ea829208edc2d7b320b7e602b9d12e47689499d5180a9cc7790dec4d7`  
		Size: 103.0 MB (103031066 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:db05d2e76671d91772a070867bf6f050343319070602a0f8239706d5d4d98387`  
		Last Modified: Wed, 12 Jan 2022 15:14:49 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60d32b598636a5d24f0e2fed2dcea425de4fb29e48ffe747b16de7d34ba96d44`  
		Last Modified: Wed, 12 Jan 2022 16:37:10 GMT  
		Size: 7.4 MB (7422473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:655251a8c00e62468ac138e6498ed5003026017f9e3aaa8a0890c8e4573e3e5d`  
		Last Modified: Wed, 12 Jan 2022 16:37:02 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99ce1684628b1c7cadb6b52866c3be12d063636d962797df7454acc55806596d`  
		Last Modified: Wed, 12 Jan 2022 16:37:02 GMT  
		Size: 1.2 KB (1161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:489b687ddd94c7a64a680862d4341e41ad8fd93a41455a22da84feac26690169`  
		Last Modified: Wed, 12 Jan 2022 16:37:02 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:linux`

```console
$ docker pull nats-streaming@sha256:a80b4649e47eb1640ead441ff67bb621bffc4cecd39041fa6e9802fbdd9b3760
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:linux` - linux; amd64

```console
$ docker pull nats-streaming@sha256:05a387b6bd267efd7806a67b7b4d431d054e69537a8dd00f0a874e71b48be7e1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7299150 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e1cf392bf11cb1f2dac51f4d09fa86f69859583c3ac7d4812f6c1887d485073`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Sat, 20 Nov 2021 02:21:16 GMT
COPY file:430b600f51b8ec2b8032b9ee2b54a3f23458b67e7fcd26e03d4a1c4fb292e8e3 in /nats-streaming-server 
# Sat, 20 Nov 2021 02:21:16 GMT
EXPOSE 4222 8222
# Sat, 20 Nov 2021 02:21:16 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Sat, 20 Nov 2021 02:21:17 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:ea39d064fdb9df476b776a2728cf769791a02b09590387975647243e2266b1ca`  
		Last Modified: Sat, 20 Nov 2021 02:22:01 GMT  
		Size: 7.3 MB (7299150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:linux` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:0c1a07390ec1c002d89b5bcd0d0048c95f33f859d53b607ffdc16678e3f79bd8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6774516 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1392e1316cac3fc870ec9cd90c7973466ed1433895aee0166a624b060262b6b5`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Fri, 19 Nov 2021 23:50:00 GMT
COPY file:d86d6a12a47b28bc562444b508d1508f4f436aa57b4f9785d2f72f13991058d9 in /nats-streaming-server 
# Fri, 19 Nov 2021 23:50:00 GMT
EXPOSE 4222 8222
# Fri, 19 Nov 2021 23:50:01 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Fri, 19 Nov 2021 23:50:01 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:ada5d2acf52444276ec7168ad03307d61f3ac5bb2e33825f280ba40e265f0533`  
		Last Modified: Fri, 19 Nov 2021 23:51:55 GMT  
		Size: 6.8 MB (6774516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:linux` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:cf7abf017ca4b10bcc16492ee29f54f9901fc6c40ae0e5eeba35423ce4346312
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6763075 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4f2b939f92968d68a30b61db2b05fae78f9b7545fb1060ebb0c535069d2a6e0`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Sat, 20 Nov 2021 02:34:09 GMT
COPY file:f737534371c307ebba33d860a23821186a07bfe6bac93b4f8db1052afabca519 in /nats-streaming-server 
# Sat, 20 Nov 2021 02:34:09 GMT
EXPOSE 4222 8222
# Sat, 20 Nov 2021 02:34:10 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Sat, 20 Nov 2021 02:34:10 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:f09d0d006743cce0f69db665ba3e97775e3e7ec87b782222a87b0e299de7abdd`  
		Last Modified: Sat, 20 Nov 2021 02:36:04 GMT  
		Size: 6.8 MB (6763075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:linux` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:62364f60027f7c3607653a956cf2578021f20431d07038537298bd2e053f622d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.7 MB (6666709 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e200b7f1afcc145455136db22812cb59ac4b91d3018f34d80f3df1980798dfa`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Sat, 20 Nov 2021 04:21:01 GMT
COPY file:758facc101ea28c799c8630223bb78d0e4182d429b666642665350bc7a40a28d in /nats-streaming-server 
# Sat, 20 Nov 2021 04:21:01 GMT
EXPOSE 4222 8222
# Sat, 20 Nov 2021 04:21:02 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Sat, 20 Nov 2021 04:21:03 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:372c129ce02fe71df79c38000ee3af5425ca18626def1095c58ab7c9cc6a31a8`  
		Last Modified: Sat, 20 Nov 2021 04:22:04 GMT  
		Size: 6.7 MB (6666709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:nanoserver`

```console
$ docker pull nats-streaming@sha256:3deb3e84ece2e334a28e4b46853567baf661fb0d6e9965cb297783565c5c96c9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2452; amd64

### `nats-streaming:nanoserver` - windows version 10.0.17763.2452; amd64

```console
$ docker pull nats-streaming@sha256:e5a5c9eee1f4f76f236ebf6a7049dd1956e9db04ae49b2b50c960eb7b51bfb17
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.5 MB (110458174 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86f5bfb309b8634f75a1184a8b349dc72fbe6750e195fa87c4ee3b7220ebc253`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Fri, 07 Jan 2022 22:25:06 GMT
RUN Apply image 1809-amd64
# Wed, 12 Jan 2022 15:13:42 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 12 Jan 2022 16:36:12 GMT
RUN cmd /S /C #(nop) COPY file:bb30895f60b97f75adc45bbc64dd23d70df079c19ad26c4f8d07ce1c88e77c96 in C:\nats-streaming-server.exe 
# Wed, 12 Jan 2022 16:36:13 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 12 Jan 2022 16:36:14 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 12 Jan 2022 16:36:15 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:3a78847ea829208edc2d7b320b7e602b9d12e47689499d5180a9cc7790dec4d7`  
		Size: 103.0 MB (103031066 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:db05d2e76671d91772a070867bf6f050343319070602a0f8239706d5d4d98387`  
		Last Modified: Wed, 12 Jan 2022 15:14:49 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60d32b598636a5d24f0e2fed2dcea425de4fb29e48ffe747b16de7d34ba96d44`  
		Last Modified: Wed, 12 Jan 2022 16:37:10 GMT  
		Size: 7.4 MB (7422473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:655251a8c00e62468ac138e6498ed5003026017f9e3aaa8a0890c8e4573e3e5d`  
		Last Modified: Wed, 12 Jan 2022 16:37:02 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99ce1684628b1c7cadb6b52866c3be12d063636d962797df7454acc55806596d`  
		Last Modified: Wed, 12 Jan 2022 16:37:02 GMT  
		Size: 1.2 KB (1161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:489b687ddd94c7a64a680862d4341e41ad8fd93a41455a22da84feac26690169`  
		Last Modified: Wed, 12 Jan 2022 16:37:02 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:nanoserver-1809`

```console
$ docker pull nats-streaming@sha256:3deb3e84ece2e334a28e4b46853567baf661fb0d6e9965cb297783565c5c96c9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2452; amd64

### `nats-streaming:nanoserver-1809` - windows version 10.0.17763.2452; amd64

```console
$ docker pull nats-streaming@sha256:e5a5c9eee1f4f76f236ebf6a7049dd1956e9db04ae49b2b50c960eb7b51bfb17
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.5 MB (110458174 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86f5bfb309b8634f75a1184a8b349dc72fbe6750e195fa87c4ee3b7220ebc253`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Fri, 07 Jan 2022 22:25:06 GMT
RUN Apply image 1809-amd64
# Wed, 12 Jan 2022 15:13:42 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 12 Jan 2022 16:36:12 GMT
RUN cmd /S /C #(nop) COPY file:bb30895f60b97f75adc45bbc64dd23d70df079c19ad26c4f8d07ce1c88e77c96 in C:\nats-streaming-server.exe 
# Wed, 12 Jan 2022 16:36:13 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 12 Jan 2022 16:36:14 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 12 Jan 2022 16:36:15 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:3a78847ea829208edc2d7b320b7e602b9d12e47689499d5180a9cc7790dec4d7`  
		Size: 103.0 MB (103031066 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:db05d2e76671d91772a070867bf6f050343319070602a0f8239706d5d4d98387`  
		Last Modified: Wed, 12 Jan 2022 15:14:49 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60d32b598636a5d24f0e2fed2dcea425de4fb29e48ffe747b16de7d34ba96d44`  
		Last Modified: Wed, 12 Jan 2022 16:37:10 GMT  
		Size: 7.4 MB (7422473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:655251a8c00e62468ac138e6498ed5003026017f9e3aaa8a0890c8e4573e3e5d`  
		Last Modified: Wed, 12 Jan 2022 16:37:02 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99ce1684628b1c7cadb6b52866c3be12d063636d962797df7454acc55806596d`  
		Last Modified: Wed, 12 Jan 2022 16:37:02 GMT  
		Size: 1.2 KB (1161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:489b687ddd94c7a64a680862d4341e41ad8fd93a41455a22da84feac26690169`  
		Last Modified: Wed, 12 Jan 2022 16:37:02 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:scratch`

```console
$ docker pull nats-streaming@sha256:a80b4649e47eb1640ead441ff67bb621bffc4cecd39041fa6e9802fbdd9b3760
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:scratch` - linux; amd64

```console
$ docker pull nats-streaming@sha256:05a387b6bd267efd7806a67b7b4d431d054e69537a8dd00f0a874e71b48be7e1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7299150 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e1cf392bf11cb1f2dac51f4d09fa86f69859583c3ac7d4812f6c1887d485073`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Sat, 20 Nov 2021 02:21:16 GMT
COPY file:430b600f51b8ec2b8032b9ee2b54a3f23458b67e7fcd26e03d4a1c4fb292e8e3 in /nats-streaming-server 
# Sat, 20 Nov 2021 02:21:16 GMT
EXPOSE 4222 8222
# Sat, 20 Nov 2021 02:21:16 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Sat, 20 Nov 2021 02:21:17 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:ea39d064fdb9df476b776a2728cf769791a02b09590387975647243e2266b1ca`  
		Last Modified: Sat, 20 Nov 2021 02:22:01 GMT  
		Size: 7.3 MB (7299150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:scratch` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:0c1a07390ec1c002d89b5bcd0d0048c95f33f859d53b607ffdc16678e3f79bd8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6774516 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1392e1316cac3fc870ec9cd90c7973466ed1433895aee0166a624b060262b6b5`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Fri, 19 Nov 2021 23:50:00 GMT
COPY file:d86d6a12a47b28bc562444b508d1508f4f436aa57b4f9785d2f72f13991058d9 in /nats-streaming-server 
# Fri, 19 Nov 2021 23:50:00 GMT
EXPOSE 4222 8222
# Fri, 19 Nov 2021 23:50:01 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Fri, 19 Nov 2021 23:50:01 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:ada5d2acf52444276ec7168ad03307d61f3ac5bb2e33825f280ba40e265f0533`  
		Last Modified: Fri, 19 Nov 2021 23:51:55 GMT  
		Size: 6.8 MB (6774516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:scratch` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:cf7abf017ca4b10bcc16492ee29f54f9901fc6c40ae0e5eeba35423ce4346312
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6763075 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4f2b939f92968d68a30b61db2b05fae78f9b7545fb1060ebb0c535069d2a6e0`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Sat, 20 Nov 2021 02:34:09 GMT
COPY file:f737534371c307ebba33d860a23821186a07bfe6bac93b4f8db1052afabca519 in /nats-streaming-server 
# Sat, 20 Nov 2021 02:34:09 GMT
EXPOSE 4222 8222
# Sat, 20 Nov 2021 02:34:10 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Sat, 20 Nov 2021 02:34:10 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:f09d0d006743cce0f69db665ba3e97775e3e7ec87b782222a87b0e299de7abdd`  
		Last Modified: Sat, 20 Nov 2021 02:36:04 GMT  
		Size: 6.8 MB (6763075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:scratch` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:62364f60027f7c3607653a956cf2578021f20431d07038537298bd2e053f622d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.7 MB (6666709 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e200b7f1afcc145455136db22812cb59ac4b91d3018f34d80f3df1980798dfa`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Sat, 20 Nov 2021 04:21:01 GMT
COPY file:758facc101ea28c799c8630223bb78d0e4182d429b666642665350bc7a40a28d in /nats-streaming-server 
# Sat, 20 Nov 2021 04:21:01 GMT
EXPOSE 4222 8222
# Sat, 20 Nov 2021 04:21:02 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Sat, 20 Nov 2021 04:21:03 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:372c129ce02fe71df79c38000ee3af5425ca18626def1095c58ab7c9cc6a31a8`  
		Last Modified: Sat, 20 Nov 2021 04:22:04 GMT  
		Size: 6.7 MB (6666709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:windowsservercore`

```console
$ docker pull nats-streaming@sha256:60cddb85b5f5991f1e6bcf9b251048c924b7c717f62b1d49a5d7dbf3164f91a9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.2452; amd64
	-	windows version 10.0.14393.4886; amd64

### `nats-streaming:windowsservercore` - windows version 10.0.17763.2452; amd64

```console
$ docker pull nats-streaming@sha256:b7bd0b03c112bb6a886fc32de7f1416d9a8226341c7425a95714b893c064dabf
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2720323552 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6cf92bdf78d0e103b0277b51786c36629cfd72167d13e7e9e08b399b2a8167b3`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
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
# Wed, 12 Jan 2022 16:33:12 GMT
ENV NATS_STREAMING_SERVER=0.23.2
# Wed, 12 Jan 2022 16:33:13 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.23.2/nats-streaming-server-v0.23.2-windows-amd64.zip
# Wed, 12 Jan 2022 16:33:14 GMT
ENV NATS_STREAMING_SERVER_SHASUM=b28dc8e1565d6fece68781515f759b0ed870831cdf2f7925cff7cf9acb44e7ec
# Wed, 12 Jan 2022 16:34:10 GMT
RUN Set-PSDebug -Trace 2
# Wed, 12 Jan 2022 16:35:52 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 12 Jan 2022 16:35:54 GMT
EXPOSE 4222 8222
# Wed, 12 Jan 2022 16:35:55 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 12 Jan 2022 16:35:56 GMT
CMD ["-m" "8222"]
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
	-	`sha256:2e56f267999eb7fd5bcfb301b0f0e6052a8ae22ca628c389db83c562990cf444`  
		Last Modified: Wed, 12 Jan 2022 16:36:50 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:821e8ced70841dc00f55dcd8124121cbb0c430571a5e5d158741fcf29c4eb763`  
		Last Modified: Wed, 12 Jan 2022 16:36:49 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6f67c1564c45a427f773fc0876060b2020ca2453a98023b375fb06c5f53bf3b`  
		Last Modified: Wed, 12 Jan 2022 16:36:49 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:770a7c738c44f07d9a29e8d8cd2ed3ad2f85aa87d7d0bfba1e7efde7ff6c131b`  
		Last Modified: Wed, 12 Jan 2022 16:36:47 GMT  
		Size: 338.5 KB (338485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29ce328ddff49212914bc498c236b2fa59188c0aaa5086dcab210060f4a886f1`  
		Last Modified: Wed, 12 Jan 2022 16:36:50 GMT  
		Size: 7.7 MB (7742962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:091c2e64ef4827cbcb4a216d0422edb3669c90feafeb39b97d344bed44ea4b75`  
		Last Modified: Wed, 12 Jan 2022 16:36:47 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38db1a89341b657073620f8a786ceec8c75be7fc50ccc4a506c364942fa7bc40`  
		Last Modified: Wed, 12 Jan 2022 16:36:47 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1c36c3fb3a835905d4b5ab75dbb3b1e7d580f9723d36b7bf3cf9fcea75f6365`  
		Last Modified: Wed, 12 Jan 2022 16:36:47 GMT  
		Size: 1.4 KB (1381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:windowsservercore` - windows version 10.0.14393.4886; amd64

```console
$ docker pull nats-streaming@sha256:d55e31a14946b12f1d6c152dfb777ad1b2da038f0c957bde81c5cfb59cd1a97d
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6290824289 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:111095c35ecacfdbe68e1ef364f73124e3888020c1fdffe9c88d2b78bd021fa8`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
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
# Tue, 11 Jan 2022 19:57:41 GMT
ENV NATS_STREAMING_SERVER=0.23.2
# Tue, 11 Jan 2022 19:57:42 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.23.2/nats-streaming-server-v0.23.2-windows-amd64.zip
# Tue, 11 Jan 2022 19:57:43 GMT
ENV NATS_STREAMING_SERVER_SHASUM=b28dc8e1565d6fece68781515f759b0ed870831cdf2f7925cff7cf9acb44e7ec
# Tue, 11 Jan 2022 21:24:39 GMT
RUN Set-PSDebug -Trace 2
# Tue, 11 Jan 2022 21:26:28 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Tue, 11 Jan 2022 21:26:29 GMT
EXPOSE 4222 8222
# Tue, 11 Jan 2022 21:26:31 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Tue, 11 Jan 2022 21:26:32 GMT
CMD ["-m" "8222"]
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
	-	`sha256:b5cf3c8d8140ae38c2d505f95e5babf9f4505d67a6151d6fe3f9c751ef7d0dc5`  
		Last Modified: Tue, 11 Jan 2022 21:27:37 GMT  
		Size: 1.4 KB (1354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19dc2e3eee55193ca6704fc85c6992e8b9b8bd428d80239cd34ee31b8c72fdc5`  
		Last Modified: Tue, 11 Jan 2022 21:27:37 GMT  
		Size: 1.4 KB (1374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92cc106ea2da4cb4db419ee1efe603754ac4e6645cde9bdf6ee8bde96b5e342a`  
		Last Modified: Tue, 11 Jan 2022 21:27:37 GMT  
		Size: 1.4 KB (1363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c19b53c2023c3798cb5b4fb1bf2c6c906c1c9ec3f1a64fe6ca6832b146c5e926`  
		Last Modified: Tue, 11 Jan 2022 21:27:35 GMT  
		Size: 335.6 KB (335575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b49df4cdedb96e996d903b4a909a6204919bef00f7a72eea5fc92c42249b541c`  
		Last Modified: Tue, 11 Jan 2022 21:27:48 GMT  
		Size: 12.3 MB (12274958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf21ee223236021b829cf5aa5a4a19abe4854ed145378b8ca64aed39459a5611`  
		Last Modified: Tue, 11 Jan 2022 21:27:34 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc2ccb79a6a3985e5a419e8c0f1256719adee45c6ab7d7a049e39e42ee798e91`  
		Last Modified: Tue, 11 Jan 2022 21:27:34 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adb13dd255898f881701597b01fa5e3b8873647e6098933da4de040996a6188d`  
		Last Modified: Tue, 11 Jan 2022 21:27:34 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:windowsservercore-1809`

```console
$ docker pull nats-streaming@sha256:f4205543bce3358dd968000ee86d121344534bfeb34634fce3af7196029e72b1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2452; amd64

### `nats-streaming:windowsservercore-1809` - windows version 10.0.17763.2452; amd64

```console
$ docker pull nats-streaming@sha256:b7bd0b03c112bb6a886fc32de7f1416d9a8226341c7425a95714b893c064dabf
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2720323552 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6cf92bdf78d0e103b0277b51786c36629cfd72167d13e7e9e08b399b2a8167b3`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
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
# Wed, 12 Jan 2022 16:33:12 GMT
ENV NATS_STREAMING_SERVER=0.23.2
# Wed, 12 Jan 2022 16:33:13 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.23.2/nats-streaming-server-v0.23.2-windows-amd64.zip
# Wed, 12 Jan 2022 16:33:14 GMT
ENV NATS_STREAMING_SERVER_SHASUM=b28dc8e1565d6fece68781515f759b0ed870831cdf2f7925cff7cf9acb44e7ec
# Wed, 12 Jan 2022 16:34:10 GMT
RUN Set-PSDebug -Trace 2
# Wed, 12 Jan 2022 16:35:52 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 12 Jan 2022 16:35:54 GMT
EXPOSE 4222 8222
# Wed, 12 Jan 2022 16:35:55 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 12 Jan 2022 16:35:56 GMT
CMD ["-m" "8222"]
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
	-	`sha256:2e56f267999eb7fd5bcfb301b0f0e6052a8ae22ca628c389db83c562990cf444`  
		Last Modified: Wed, 12 Jan 2022 16:36:50 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:821e8ced70841dc00f55dcd8124121cbb0c430571a5e5d158741fcf29c4eb763`  
		Last Modified: Wed, 12 Jan 2022 16:36:49 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6f67c1564c45a427f773fc0876060b2020ca2453a98023b375fb06c5f53bf3b`  
		Last Modified: Wed, 12 Jan 2022 16:36:49 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:770a7c738c44f07d9a29e8d8cd2ed3ad2f85aa87d7d0bfba1e7efde7ff6c131b`  
		Last Modified: Wed, 12 Jan 2022 16:36:47 GMT  
		Size: 338.5 KB (338485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29ce328ddff49212914bc498c236b2fa59188c0aaa5086dcab210060f4a886f1`  
		Last Modified: Wed, 12 Jan 2022 16:36:50 GMT  
		Size: 7.7 MB (7742962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:091c2e64ef4827cbcb4a216d0422edb3669c90feafeb39b97d344bed44ea4b75`  
		Last Modified: Wed, 12 Jan 2022 16:36:47 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38db1a89341b657073620f8a786ceec8c75be7fc50ccc4a506c364942fa7bc40`  
		Last Modified: Wed, 12 Jan 2022 16:36:47 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1c36c3fb3a835905d4b5ab75dbb3b1e7d580f9723d36b7bf3cf9fcea75f6365`  
		Last Modified: Wed, 12 Jan 2022 16:36:47 GMT  
		Size: 1.4 KB (1381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:windowsservercore-ltsc2016`

```console
$ docker pull nats-streaming@sha256:8d7f645475c1ddf54332ac47ad4daa549c2a02a25e27f3062c39efed087fd0ba
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.14393.4886; amd64

### `nats-streaming:windowsservercore-ltsc2016` - windows version 10.0.14393.4886; amd64

```console
$ docker pull nats-streaming@sha256:d55e31a14946b12f1d6c152dfb777ad1b2da038f0c957bde81c5cfb59cd1a97d
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6290824289 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:111095c35ecacfdbe68e1ef364f73124e3888020c1fdffe9c88d2b78bd021fa8`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
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
# Tue, 11 Jan 2022 19:57:41 GMT
ENV NATS_STREAMING_SERVER=0.23.2
# Tue, 11 Jan 2022 19:57:42 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.23.2/nats-streaming-server-v0.23.2-windows-amd64.zip
# Tue, 11 Jan 2022 19:57:43 GMT
ENV NATS_STREAMING_SERVER_SHASUM=b28dc8e1565d6fece68781515f759b0ed870831cdf2f7925cff7cf9acb44e7ec
# Tue, 11 Jan 2022 21:24:39 GMT
RUN Set-PSDebug -Trace 2
# Tue, 11 Jan 2022 21:26:28 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Tue, 11 Jan 2022 21:26:29 GMT
EXPOSE 4222 8222
# Tue, 11 Jan 2022 21:26:31 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Tue, 11 Jan 2022 21:26:32 GMT
CMD ["-m" "8222"]
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
	-	`sha256:b5cf3c8d8140ae38c2d505f95e5babf9f4505d67a6151d6fe3f9c751ef7d0dc5`  
		Last Modified: Tue, 11 Jan 2022 21:27:37 GMT  
		Size: 1.4 KB (1354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19dc2e3eee55193ca6704fc85c6992e8b9b8bd428d80239cd34ee31b8c72fdc5`  
		Last Modified: Tue, 11 Jan 2022 21:27:37 GMT  
		Size: 1.4 KB (1374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92cc106ea2da4cb4db419ee1efe603754ac4e6645cde9bdf6ee8bde96b5e342a`  
		Last Modified: Tue, 11 Jan 2022 21:27:37 GMT  
		Size: 1.4 KB (1363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c19b53c2023c3798cb5b4fb1bf2c6c906c1c9ec3f1a64fe6ca6832b146c5e926`  
		Last Modified: Tue, 11 Jan 2022 21:27:35 GMT  
		Size: 335.6 KB (335575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b49df4cdedb96e996d903b4a909a6204919bef00f7a72eea5fc92c42249b541c`  
		Last Modified: Tue, 11 Jan 2022 21:27:48 GMT  
		Size: 12.3 MB (12274958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf21ee223236021b829cf5aa5a4a19abe4854ed145378b8ca64aed39459a5611`  
		Last Modified: Tue, 11 Jan 2022 21:27:34 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc2ccb79a6a3985e5a419e8c0f1256719adee45c6ab7d7a049e39e42ee798e91`  
		Last Modified: Tue, 11 Jan 2022 21:27:34 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adb13dd255898f881701597b01fa5e3b8873647e6098933da4de040996a6188d`  
		Last Modified: Tue, 11 Jan 2022 21:27:34 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
