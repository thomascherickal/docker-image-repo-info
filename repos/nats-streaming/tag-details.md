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
$ docker pull nats-streaming@sha256:c3b67c2c329064941f788aeb9e2f357b1d2c4ed918487e44c56b735dd3825e6c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.2366; amd64

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

### `nats-streaming:0.23` - windows version 10.0.17763.2366; amd64

```console
$ docker pull nats-streaming@sha256:a4dba6a1799f5368dc9d421fd4ea4fd201eddd12c10864382c9d1b6bc14c6aeb
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.3 MB (110331179 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc58ce624f6204540e8ac39bafdd9726fbc32ea7c229b38b030f5f2e64cec9d2`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 07 Dec 2021 04:37:11 GMT
RUN Apply image 1809-amd64
# Sat, 18 Dec 2021 04:34:39 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Sat, 18 Dec 2021 08:02:47 GMT
RUN cmd /S /C #(nop) COPY file:bb30895f60b97f75adc45bbc64dd23d70df079c19ad26c4f8d07ce1c88e77c96 in C:\nats-streaming-server.exe 
# Sat, 18 Dec 2021 08:02:48 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Sat, 18 Dec 2021 08:02:49 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Sat, 18 Dec 2021 08:02:49 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:034b2f457cdf6a0d3f7024523d40fd6eeb8568e6c76d9fa56f4053fcf3a21d63`  
		Size: 102.9 MB (102904001 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4f56553f84cd7b4574c0b4d1ee6585d70eda0c9f3a5f1b276ec5e7cdc713bd74`  
		Last Modified: Sat, 18 Dec 2021 08:06:40 GMT  
		Size: 1.2 KB (1178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a1496d31642d0470cbd25b3b734e0088588c71a12ec3db986575765cf928b8c`  
		Last Modified: Sat, 18 Dec 2021 08:06:42 GMT  
		Size: 7.4 MB (7422515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d168df35b99b660b4221d21e47cc005e082df581fe415650ba67380ef77d51ed`  
		Last Modified: Sat, 18 Dec 2021 08:06:40 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f89cbe2ec75329f034c70155d630a4909bc7359f7a267f72844775e87c70631`  
		Last Modified: Sat, 18 Dec 2021 08:06:40 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c1ef79bfe81d12d8f6ae9b2499ef4e6f42bc0241fe3df4d7215ba2c6a25d251`  
		Last Modified: Sat, 18 Dec 2021 08:06:40 GMT  
		Size: 1.2 KB (1168 bytes)  
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
$ docker pull nats-streaming@sha256:9d12cde295f11487b395d0ff1500b3dc5e7343a26b80efca806bab8993c3e546
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2366; amd64

### `nats-streaming:0.23-nanoserver` - windows version 10.0.17763.2366; amd64

```console
$ docker pull nats-streaming@sha256:a4dba6a1799f5368dc9d421fd4ea4fd201eddd12c10864382c9d1b6bc14c6aeb
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.3 MB (110331179 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc58ce624f6204540e8ac39bafdd9726fbc32ea7c229b38b030f5f2e64cec9d2`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 07 Dec 2021 04:37:11 GMT
RUN Apply image 1809-amd64
# Sat, 18 Dec 2021 04:34:39 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Sat, 18 Dec 2021 08:02:47 GMT
RUN cmd /S /C #(nop) COPY file:bb30895f60b97f75adc45bbc64dd23d70df079c19ad26c4f8d07ce1c88e77c96 in C:\nats-streaming-server.exe 
# Sat, 18 Dec 2021 08:02:48 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Sat, 18 Dec 2021 08:02:49 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Sat, 18 Dec 2021 08:02:49 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:034b2f457cdf6a0d3f7024523d40fd6eeb8568e6c76d9fa56f4053fcf3a21d63`  
		Size: 102.9 MB (102904001 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4f56553f84cd7b4574c0b4d1ee6585d70eda0c9f3a5f1b276ec5e7cdc713bd74`  
		Last Modified: Sat, 18 Dec 2021 08:06:40 GMT  
		Size: 1.2 KB (1178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a1496d31642d0470cbd25b3b734e0088588c71a12ec3db986575765cf928b8c`  
		Last Modified: Sat, 18 Dec 2021 08:06:42 GMT  
		Size: 7.4 MB (7422515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d168df35b99b660b4221d21e47cc005e082df581fe415650ba67380ef77d51ed`  
		Last Modified: Sat, 18 Dec 2021 08:06:40 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f89cbe2ec75329f034c70155d630a4909bc7359f7a267f72844775e87c70631`  
		Last Modified: Sat, 18 Dec 2021 08:06:40 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c1ef79bfe81d12d8f6ae9b2499ef4e6f42bc0241fe3df4d7215ba2c6a25d251`  
		Last Modified: Sat, 18 Dec 2021 08:06:40 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.23-nanoserver-1809`

```console
$ docker pull nats-streaming@sha256:9d12cde295f11487b395d0ff1500b3dc5e7343a26b80efca806bab8993c3e546
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2366; amd64

### `nats-streaming:0.23-nanoserver-1809` - windows version 10.0.17763.2366; amd64

```console
$ docker pull nats-streaming@sha256:a4dba6a1799f5368dc9d421fd4ea4fd201eddd12c10864382c9d1b6bc14c6aeb
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.3 MB (110331179 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc58ce624f6204540e8ac39bafdd9726fbc32ea7c229b38b030f5f2e64cec9d2`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 07 Dec 2021 04:37:11 GMT
RUN Apply image 1809-amd64
# Sat, 18 Dec 2021 04:34:39 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Sat, 18 Dec 2021 08:02:47 GMT
RUN cmd /S /C #(nop) COPY file:bb30895f60b97f75adc45bbc64dd23d70df079c19ad26c4f8d07ce1c88e77c96 in C:\nats-streaming-server.exe 
# Sat, 18 Dec 2021 08:02:48 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Sat, 18 Dec 2021 08:02:49 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Sat, 18 Dec 2021 08:02:49 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:034b2f457cdf6a0d3f7024523d40fd6eeb8568e6c76d9fa56f4053fcf3a21d63`  
		Size: 102.9 MB (102904001 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4f56553f84cd7b4574c0b4d1ee6585d70eda0c9f3a5f1b276ec5e7cdc713bd74`  
		Last Modified: Sat, 18 Dec 2021 08:06:40 GMT  
		Size: 1.2 KB (1178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a1496d31642d0470cbd25b3b734e0088588c71a12ec3db986575765cf928b8c`  
		Last Modified: Sat, 18 Dec 2021 08:06:42 GMT  
		Size: 7.4 MB (7422515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d168df35b99b660b4221d21e47cc005e082df581fe415650ba67380ef77d51ed`  
		Last Modified: Sat, 18 Dec 2021 08:06:40 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f89cbe2ec75329f034c70155d630a4909bc7359f7a267f72844775e87c70631`  
		Last Modified: Sat, 18 Dec 2021 08:06:40 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c1ef79bfe81d12d8f6ae9b2499ef4e6f42bc0241fe3df4d7215ba2c6a25d251`  
		Last Modified: Sat, 18 Dec 2021 08:06:40 GMT  
		Size: 1.2 KB (1168 bytes)  
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
$ docker pull nats-streaming@sha256:be9484f94d3f173a10ce890420589378d6f8ca4bd0205f0197cdfa6d0646ea69
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.2366; amd64
	-	windows version 10.0.14393.4825; amd64

### `nats-streaming:0.23-windowsservercore` - windows version 10.0.17763.2366; amd64

```console
$ docker pull nats-streaming@sha256:420220a9afa15857377173cc8f141ae0373a42f666d9d133fcf747088a6d87a0
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2716755888 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e34c0986c57d10e61a41f5d9d253df4fb832be016255f195afb5b747924e636d`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 07 Dec 2021 04:56:01 GMT
RUN Install update 1809-amd64
# Sat, 18 Dec 2021 01:40:43 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Sat, 18 Dec 2021 04:32:10 GMT
ENV NATS_DOCKERIZED=1
# Sat, 18 Dec 2021 07:59:49 GMT
ENV NATS_STREAMING_SERVER=0.23.2
# Sat, 18 Dec 2021 07:59:50 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.23.2/nats-streaming-server-v0.23.2-windows-amd64.zip
# Sat, 18 Dec 2021 07:59:51 GMT
ENV NATS_STREAMING_SERVER_SHASUM=b28dc8e1565d6fece68781515f759b0ed870831cdf2f7925cff7cf9acb44e7ec
# Sat, 18 Dec 2021 08:00:48 GMT
RUN Set-PSDebug -Trace 2
# Sat, 18 Dec 2021 08:02:34 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Sat, 18 Dec 2021 08:02:35 GMT
EXPOSE 4222 8222
# Sat, 18 Dec 2021 08:02:36 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Sat, 18 Dec 2021 08:02:37 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5ee7a7ea9cf22f75886179907a41810a992e21f3d0c57cc10d2147ce9237701c`  
		Size: 990.3 MB (990271574 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d22d2238b031d3f13bcd6c144e80f8f8402332b8ee8e53cc54b7912c3ac808cb`  
		Last Modified: Sat, 18 Dec 2021 03:59:34 GMT  
		Size: 1.4 KB (1444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44c5f7f5394b88876960b5ac27980fb2e22584cf50ecde4d9537e88ddbf849c3`  
		Last Modified: Sat, 18 Dec 2021 08:06:16 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d4330e24c7d8e5e42a117873554d01f36a0dc5de956de58eb98bc343f3b7053`  
		Last Modified: Sat, 18 Dec 2021 08:06:16 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a85e10ba361bd6036ce996ef1fc18a56eae46bfe2f2a3aa167c91a9910e44b1e`  
		Last Modified: Sat, 18 Dec 2021 08:06:16 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73619ef7215a1f395f4b26e9d2c8f3163b1eadc526a4b86834c34d2d210bbbb5`  
		Last Modified: Sat, 18 Dec 2021 08:06:16 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:585f06960fbd4efa8dc36c8d215c51aa6c8e6adadb62e05f799bc7770a768385`  
		Last Modified: Sat, 18 Dec 2021 08:06:14 GMT  
		Size: 365.8 KB (365782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b13efc00f53324e98bc4459fd1a2e6c14d2dbb3ddce59ac2d39a8d2976ead8d`  
		Last Modified: Sat, 18 Dec 2021 08:06:22 GMT  
		Size: 7.8 MB (7774250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cfbd74dd7052b02b86f232c8f3bc9d759fd4f2a1f81fcf4748927895a03331c`  
		Last Modified: Sat, 18 Dec 2021 08:06:14 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9da21c0ea9106d6386e5f731911254e0aad700297c81ecb6b7cbc2b22a81e36`  
		Last Modified: Sat, 18 Dec 2021 08:06:14 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2561dd2bec68b686d5c3e5494fffeb0a77f681864f74eb9fed80413145fbeca2`  
		Last Modified: Sat, 18 Dec 2021 08:06:14 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.23-windowsservercore` - windows version 10.0.14393.4825; amd64

```console
$ docker pull nats-streaming@sha256:2209b5c3482a96a3dae3e8ade7aae5ec6caa7e077ad472779bada808eecbc268
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6287324539 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b52052c1bd51b6280c83afbc804f342150ad5265b218136f8b7fb1b464b7810`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 08 Dec 2021 08:38:00 GMT
RUN Install update ltsc2016-amd64
# Sat, 18 Dec 2021 01:55:44 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Sat, 18 Dec 2021 04:34:51 GMT
ENV NATS_DOCKERIZED=1
# Sat, 18 Dec 2021 08:02:56 GMT
ENV NATS_STREAMING_SERVER=0.23.2
# Sat, 18 Dec 2021 08:02:57 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.23.2/nats-streaming-server-v0.23.2-windows-amd64.zip
# Sat, 18 Dec 2021 08:02:58 GMT
ENV NATS_STREAMING_SERVER_SHASUM=b28dc8e1565d6fece68781515f759b0ed870831cdf2f7925cff7cf9acb44e7ec
# Sat, 18 Dec 2021 08:03:46 GMT
RUN Set-PSDebug -Trace 2
# Sat, 18 Dec 2021 08:05:31 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Sat, 18 Dec 2021 08:05:32 GMT
EXPOSE 4222 8222
# Sat, 18 Dec 2021 08:05:33 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Sat, 18 Dec 2021 08:05:34 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2d026d646213ccf73d9f0584941d108253d62e73df2a74e070776884b7b0242b`  
		Size: 2.2 GB (2204728802 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f6bffd19db3f71ba2031bea25a529c67034869e7e1bbf9e2431d5ee747bd6d6d`  
		Last Modified: Sat, 18 Dec 2021 04:00:01 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05006360e7d5d5f0fc5160410fd98cfab768e620dca3f3fbc5b44e611e3039b4`  
		Last Modified: Sat, 18 Dec 2021 08:06:58 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c79673abbfda8355eb19c36d4a838ea039890c3b36baaa24cd9c6f350f9dbaf6`  
		Last Modified: Sat, 18 Dec 2021 08:06:57 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56135df6f0d37ae5054fdc25bf5318d041b879e122c85613d52e71729262aea1`  
		Last Modified: Sat, 18 Dec 2021 08:06:57 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ec44dadd27b2b6ed2c809e4535ad5c1cb2ced6a10857849e9434b533cdb27ce`  
		Last Modified: Sat, 18 Dec 2021 08:06:57 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9f0a80a8e8d81c759bbe086bda6032ced235dd3acd963be9eb97a6aa4fe794d`  
		Last Modified: Sat, 18 Dec 2021 08:06:55 GMT  
		Size: 328.3 KB (328284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fc6eb7f28bcbbc325f606ce67eb09e5996052f69f474b1460ee1a08fd6f326a`  
		Last Modified: Sat, 18 Dec 2021 08:06:58 GMT  
		Size: 12.3 MB (12270678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d1b9cee769ed5bc39fd057d6669bc9630960eebf6507cd19a5f4b9ebc5a4953`  
		Last Modified: Sat, 18 Dec 2021 08:06:55 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8df8e108c24c7aff3a16b44fbf9243d457b7d5d45e701f2af5601985424595b7`  
		Last Modified: Sat, 18 Dec 2021 08:06:55 GMT  
		Size: 1.3 KB (1343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:298ef1dbe7d3eca580edccaab1932ba55fc39eeef55cb80c3221a4abf9e1f0e5`  
		Last Modified: Sat, 18 Dec 2021 08:06:55 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.23-windowsservercore-1809`

```console
$ docker pull nats-streaming@sha256:e8717b1af9495be0396d6b91c3b9be076fc62c4d5c27222d253340050d8e70bb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2366; amd64

### `nats-streaming:0.23-windowsservercore-1809` - windows version 10.0.17763.2366; amd64

```console
$ docker pull nats-streaming@sha256:420220a9afa15857377173cc8f141ae0373a42f666d9d133fcf747088a6d87a0
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2716755888 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e34c0986c57d10e61a41f5d9d253df4fb832be016255f195afb5b747924e636d`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 07 Dec 2021 04:56:01 GMT
RUN Install update 1809-amd64
# Sat, 18 Dec 2021 01:40:43 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Sat, 18 Dec 2021 04:32:10 GMT
ENV NATS_DOCKERIZED=1
# Sat, 18 Dec 2021 07:59:49 GMT
ENV NATS_STREAMING_SERVER=0.23.2
# Sat, 18 Dec 2021 07:59:50 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.23.2/nats-streaming-server-v0.23.2-windows-amd64.zip
# Sat, 18 Dec 2021 07:59:51 GMT
ENV NATS_STREAMING_SERVER_SHASUM=b28dc8e1565d6fece68781515f759b0ed870831cdf2f7925cff7cf9acb44e7ec
# Sat, 18 Dec 2021 08:00:48 GMT
RUN Set-PSDebug -Trace 2
# Sat, 18 Dec 2021 08:02:34 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Sat, 18 Dec 2021 08:02:35 GMT
EXPOSE 4222 8222
# Sat, 18 Dec 2021 08:02:36 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Sat, 18 Dec 2021 08:02:37 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5ee7a7ea9cf22f75886179907a41810a992e21f3d0c57cc10d2147ce9237701c`  
		Size: 990.3 MB (990271574 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d22d2238b031d3f13bcd6c144e80f8f8402332b8ee8e53cc54b7912c3ac808cb`  
		Last Modified: Sat, 18 Dec 2021 03:59:34 GMT  
		Size: 1.4 KB (1444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44c5f7f5394b88876960b5ac27980fb2e22584cf50ecde4d9537e88ddbf849c3`  
		Last Modified: Sat, 18 Dec 2021 08:06:16 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d4330e24c7d8e5e42a117873554d01f36a0dc5de956de58eb98bc343f3b7053`  
		Last Modified: Sat, 18 Dec 2021 08:06:16 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a85e10ba361bd6036ce996ef1fc18a56eae46bfe2f2a3aa167c91a9910e44b1e`  
		Last Modified: Sat, 18 Dec 2021 08:06:16 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73619ef7215a1f395f4b26e9d2c8f3163b1eadc526a4b86834c34d2d210bbbb5`  
		Last Modified: Sat, 18 Dec 2021 08:06:16 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:585f06960fbd4efa8dc36c8d215c51aa6c8e6adadb62e05f799bc7770a768385`  
		Last Modified: Sat, 18 Dec 2021 08:06:14 GMT  
		Size: 365.8 KB (365782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b13efc00f53324e98bc4459fd1a2e6c14d2dbb3ddce59ac2d39a8d2976ead8d`  
		Last Modified: Sat, 18 Dec 2021 08:06:22 GMT  
		Size: 7.8 MB (7774250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cfbd74dd7052b02b86f232c8f3bc9d759fd4f2a1f81fcf4748927895a03331c`  
		Last Modified: Sat, 18 Dec 2021 08:06:14 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9da21c0ea9106d6386e5f731911254e0aad700297c81ecb6b7cbc2b22a81e36`  
		Last Modified: Sat, 18 Dec 2021 08:06:14 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2561dd2bec68b686d5c3e5494fffeb0a77f681864f74eb9fed80413145fbeca2`  
		Last Modified: Sat, 18 Dec 2021 08:06:14 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.23-windowsservercore-ltsc2016`

```console
$ docker pull nats-streaming@sha256:62945f3e51902319046e2bd0464be26fc730aea2850268b77ce48818ad493d09
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.14393.4825; amd64

### `nats-streaming:0.23-windowsservercore-ltsc2016` - windows version 10.0.14393.4825; amd64

```console
$ docker pull nats-streaming@sha256:2209b5c3482a96a3dae3e8ade7aae5ec6caa7e077ad472779bada808eecbc268
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6287324539 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b52052c1bd51b6280c83afbc804f342150ad5265b218136f8b7fb1b464b7810`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 08 Dec 2021 08:38:00 GMT
RUN Install update ltsc2016-amd64
# Sat, 18 Dec 2021 01:55:44 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Sat, 18 Dec 2021 04:34:51 GMT
ENV NATS_DOCKERIZED=1
# Sat, 18 Dec 2021 08:02:56 GMT
ENV NATS_STREAMING_SERVER=0.23.2
# Sat, 18 Dec 2021 08:02:57 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.23.2/nats-streaming-server-v0.23.2-windows-amd64.zip
# Sat, 18 Dec 2021 08:02:58 GMT
ENV NATS_STREAMING_SERVER_SHASUM=b28dc8e1565d6fece68781515f759b0ed870831cdf2f7925cff7cf9acb44e7ec
# Sat, 18 Dec 2021 08:03:46 GMT
RUN Set-PSDebug -Trace 2
# Sat, 18 Dec 2021 08:05:31 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Sat, 18 Dec 2021 08:05:32 GMT
EXPOSE 4222 8222
# Sat, 18 Dec 2021 08:05:33 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Sat, 18 Dec 2021 08:05:34 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2d026d646213ccf73d9f0584941d108253d62e73df2a74e070776884b7b0242b`  
		Size: 2.2 GB (2204728802 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f6bffd19db3f71ba2031bea25a529c67034869e7e1bbf9e2431d5ee747bd6d6d`  
		Last Modified: Sat, 18 Dec 2021 04:00:01 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05006360e7d5d5f0fc5160410fd98cfab768e620dca3f3fbc5b44e611e3039b4`  
		Last Modified: Sat, 18 Dec 2021 08:06:58 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c79673abbfda8355eb19c36d4a838ea039890c3b36baaa24cd9c6f350f9dbaf6`  
		Last Modified: Sat, 18 Dec 2021 08:06:57 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56135df6f0d37ae5054fdc25bf5318d041b879e122c85613d52e71729262aea1`  
		Last Modified: Sat, 18 Dec 2021 08:06:57 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ec44dadd27b2b6ed2c809e4535ad5c1cb2ced6a10857849e9434b533cdb27ce`  
		Last Modified: Sat, 18 Dec 2021 08:06:57 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9f0a80a8e8d81c759bbe086bda6032ced235dd3acd963be9eb97a6aa4fe794d`  
		Last Modified: Sat, 18 Dec 2021 08:06:55 GMT  
		Size: 328.3 KB (328284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fc6eb7f28bcbbc325f606ce67eb09e5996052f69f474b1460ee1a08fd6f326a`  
		Last Modified: Sat, 18 Dec 2021 08:06:58 GMT  
		Size: 12.3 MB (12270678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d1b9cee769ed5bc39fd057d6669bc9630960eebf6507cd19a5f4b9ebc5a4953`  
		Last Modified: Sat, 18 Dec 2021 08:06:55 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8df8e108c24c7aff3a16b44fbf9243d457b7d5d45e701f2af5601985424595b7`  
		Last Modified: Sat, 18 Dec 2021 08:06:55 GMT  
		Size: 1.3 KB (1343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:298ef1dbe7d3eca580edccaab1932ba55fc39eeef55cb80c3221a4abf9e1f0e5`  
		Last Modified: Sat, 18 Dec 2021 08:06:55 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.23.2`

```console
$ docker pull nats-streaming@sha256:c3b67c2c329064941f788aeb9e2f357b1d2c4ed918487e44c56b735dd3825e6c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.2366; amd64

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

### `nats-streaming:0.23.2` - windows version 10.0.17763.2366; amd64

```console
$ docker pull nats-streaming@sha256:a4dba6a1799f5368dc9d421fd4ea4fd201eddd12c10864382c9d1b6bc14c6aeb
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.3 MB (110331179 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc58ce624f6204540e8ac39bafdd9726fbc32ea7c229b38b030f5f2e64cec9d2`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 07 Dec 2021 04:37:11 GMT
RUN Apply image 1809-amd64
# Sat, 18 Dec 2021 04:34:39 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Sat, 18 Dec 2021 08:02:47 GMT
RUN cmd /S /C #(nop) COPY file:bb30895f60b97f75adc45bbc64dd23d70df079c19ad26c4f8d07ce1c88e77c96 in C:\nats-streaming-server.exe 
# Sat, 18 Dec 2021 08:02:48 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Sat, 18 Dec 2021 08:02:49 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Sat, 18 Dec 2021 08:02:49 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:034b2f457cdf6a0d3f7024523d40fd6eeb8568e6c76d9fa56f4053fcf3a21d63`  
		Size: 102.9 MB (102904001 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4f56553f84cd7b4574c0b4d1ee6585d70eda0c9f3a5f1b276ec5e7cdc713bd74`  
		Last Modified: Sat, 18 Dec 2021 08:06:40 GMT  
		Size: 1.2 KB (1178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a1496d31642d0470cbd25b3b734e0088588c71a12ec3db986575765cf928b8c`  
		Last Modified: Sat, 18 Dec 2021 08:06:42 GMT  
		Size: 7.4 MB (7422515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d168df35b99b660b4221d21e47cc005e082df581fe415650ba67380ef77d51ed`  
		Last Modified: Sat, 18 Dec 2021 08:06:40 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f89cbe2ec75329f034c70155d630a4909bc7359f7a267f72844775e87c70631`  
		Last Modified: Sat, 18 Dec 2021 08:06:40 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c1ef79bfe81d12d8f6ae9b2499ef4e6f42bc0241fe3df4d7215ba2c6a25d251`  
		Last Modified: Sat, 18 Dec 2021 08:06:40 GMT  
		Size: 1.2 KB (1168 bytes)  
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
$ docker pull nats-streaming@sha256:9d12cde295f11487b395d0ff1500b3dc5e7343a26b80efca806bab8993c3e546
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2366; amd64

### `nats-streaming:0.23.2-nanoserver` - windows version 10.0.17763.2366; amd64

```console
$ docker pull nats-streaming@sha256:a4dba6a1799f5368dc9d421fd4ea4fd201eddd12c10864382c9d1b6bc14c6aeb
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.3 MB (110331179 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc58ce624f6204540e8ac39bafdd9726fbc32ea7c229b38b030f5f2e64cec9d2`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 07 Dec 2021 04:37:11 GMT
RUN Apply image 1809-amd64
# Sat, 18 Dec 2021 04:34:39 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Sat, 18 Dec 2021 08:02:47 GMT
RUN cmd /S /C #(nop) COPY file:bb30895f60b97f75adc45bbc64dd23d70df079c19ad26c4f8d07ce1c88e77c96 in C:\nats-streaming-server.exe 
# Sat, 18 Dec 2021 08:02:48 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Sat, 18 Dec 2021 08:02:49 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Sat, 18 Dec 2021 08:02:49 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:034b2f457cdf6a0d3f7024523d40fd6eeb8568e6c76d9fa56f4053fcf3a21d63`  
		Size: 102.9 MB (102904001 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4f56553f84cd7b4574c0b4d1ee6585d70eda0c9f3a5f1b276ec5e7cdc713bd74`  
		Last Modified: Sat, 18 Dec 2021 08:06:40 GMT  
		Size: 1.2 KB (1178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a1496d31642d0470cbd25b3b734e0088588c71a12ec3db986575765cf928b8c`  
		Last Modified: Sat, 18 Dec 2021 08:06:42 GMT  
		Size: 7.4 MB (7422515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d168df35b99b660b4221d21e47cc005e082df581fe415650ba67380ef77d51ed`  
		Last Modified: Sat, 18 Dec 2021 08:06:40 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f89cbe2ec75329f034c70155d630a4909bc7359f7a267f72844775e87c70631`  
		Last Modified: Sat, 18 Dec 2021 08:06:40 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c1ef79bfe81d12d8f6ae9b2499ef4e6f42bc0241fe3df4d7215ba2c6a25d251`  
		Last Modified: Sat, 18 Dec 2021 08:06:40 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.23.2-nanoserver-1809`

```console
$ docker pull nats-streaming@sha256:9d12cde295f11487b395d0ff1500b3dc5e7343a26b80efca806bab8993c3e546
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2366; amd64

### `nats-streaming:0.23.2-nanoserver-1809` - windows version 10.0.17763.2366; amd64

```console
$ docker pull nats-streaming@sha256:a4dba6a1799f5368dc9d421fd4ea4fd201eddd12c10864382c9d1b6bc14c6aeb
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.3 MB (110331179 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc58ce624f6204540e8ac39bafdd9726fbc32ea7c229b38b030f5f2e64cec9d2`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 07 Dec 2021 04:37:11 GMT
RUN Apply image 1809-amd64
# Sat, 18 Dec 2021 04:34:39 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Sat, 18 Dec 2021 08:02:47 GMT
RUN cmd /S /C #(nop) COPY file:bb30895f60b97f75adc45bbc64dd23d70df079c19ad26c4f8d07ce1c88e77c96 in C:\nats-streaming-server.exe 
# Sat, 18 Dec 2021 08:02:48 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Sat, 18 Dec 2021 08:02:49 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Sat, 18 Dec 2021 08:02:49 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:034b2f457cdf6a0d3f7024523d40fd6eeb8568e6c76d9fa56f4053fcf3a21d63`  
		Size: 102.9 MB (102904001 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4f56553f84cd7b4574c0b4d1ee6585d70eda0c9f3a5f1b276ec5e7cdc713bd74`  
		Last Modified: Sat, 18 Dec 2021 08:06:40 GMT  
		Size: 1.2 KB (1178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a1496d31642d0470cbd25b3b734e0088588c71a12ec3db986575765cf928b8c`  
		Last Modified: Sat, 18 Dec 2021 08:06:42 GMT  
		Size: 7.4 MB (7422515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d168df35b99b660b4221d21e47cc005e082df581fe415650ba67380ef77d51ed`  
		Last Modified: Sat, 18 Dec 2021 08:06:40 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f89cbe2ec75329f034c70155d630a4909bc7359f7a267f72844775e87c70631`  
		Last Modified: Sat, 18 Dec 2021 08:06:40 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c1ef79bfe81d12d8f6ae9b2499ef4e6f42bc0241fe3df4d7215ba2c6a25d251`  
		Last Modified: Sat, 18 Dec 2021 08:06:40 GMT  
		Size: 1.2 KB (1168 bytes)  
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
$ docker pull nats-streaming@sha256:be9484f94d3f173a10ce890420589378d6f8ca4bd0205f0197cdfa6d0646ea69
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.2366; amd64
	-	windows version 10.0.14393.4825; amd64

### `nats-streaming:0.23.2-windowsservercore` - windows version 10.0.17763.2366; amd64

```console
$ docker pull nats-streaming@sha256:420220a9afa15857377173cc8f141ae0373a42f666d9d133fcf747088a6d87a0
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2716755888 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e34c0986c57d10e61a41f5d9d253df4fb832be016255f195afb5b747924e636d`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 07 Dec 2021 04:56:01 GMT
RUN Install update 1809-amd64
# Sat, 18 Dec 2021 01:40:43 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Sat, 18 Dec 2021 04:32:10 GMT
ENV NATS_DOCKERIZED=1
# Sat, 18 Dec 2021 07:59:49 GMT
ENV NATS_STREAMING_SERVER=0.23.2
# Sat, 18 Dec 2021 07:59:50 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.23.2/nats-streaming-server-v0.23.2-windows-amd64.zip
# Sat, 18 Dec 2021 07:59:51 GMT
ENV NATS_STREAMING_SERVER_SHASUM=b28dc8e1565d6fece68781515f759b0ed870831cdf2f7925cff7cf9acb44e7ec
# Sat, 18 Dec 2021 08:00:48 GMT
RUN Set-PSDebug -Trace 2
# Sat, 18 Dec 2021 08:02:34 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Sat, 18 Dec 2021 08:02:35 GMT
EXPOSE 4222 8222
# Sat, 18 Dec 2021 08:02:36 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Sat, 18 Dec 2021 08:02:37 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5ee7a7ea9cf22f75886179907a41810a992e21f3d0c57cc10d2147ce9237701c`  
		Size: 990.3 MB (990271574 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d22d2238b031d3f13bcd6c144e80f8f8402332b8ee8e53cc54b7912c3ac808cb`  
		Last Modified: Sat, 18 Dec 2021 03:59:34 GMT  
		Size: 1.4 KB (1444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44c5f7f5394b88876960b5ac27980fb2e22584cf50ecde4d9537e88ddbf849c3`  
		Last Modified: Sat, 18 Dec 2021 08:06:16 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d4330e24c7d8e5e42a117873554d01f36a0dc5de956de58eb98bc343f3b7053`  
		Last Modified: Sat, 18 Dec 2021 08:06:16 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a85e10ba361bd6036ce996ef1fc18a56eae46bfe2f2a3aa167c91a9910e44b1e`  
		Last Modified: Sat, 18 Dec 2021 08:06:16 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73619ef7215a1f395f4b26e9d2c8f3163b1eadc526a4b86834c34d2d210bbbb5`  
		Last Modified: Sat, 18 Dec 2021 08:06:16 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:585f06960fbd4efa8dc36c8d215c51aa6c8e6adadb62e05f799bc7770a768385`  
		Last Modified: Sat, 18 Dec 2021 08:06:14 GMT  
		Size: 365.8 KB (365782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b13efc00f53324e98bc4459fd1a2e6c14d2dbb3ddce59ac2d39a8d2976ead8d`  
		Last Modified: Sat, 18 Dec 2021 08:06:22 GMT  
		Size: 7.8 MB (7774250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cfbd74dd7052b02b86f232c8f3bc9d759fd4f2a1f81fcf4748927895a03331c`  
		Last Modified: Sat, 18 Dec 2021 08:06:14 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9da21c0ea9106d6386e5f731911254e0aad700297c81ecb6b7cbc2b22a81e36`  
		Last Modified: Sat, 18 Dec 2021 08:06:14 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2561dd2bec68b686d5c3e5494fffeb0a77f681864f74eb9fed80413145fbeca2`  
		Last Modified: Sat, 18 Dec 2021 08:06:14 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.23.2-windowsservercore` - windows version 10.0.14393.4825; amd64

```console
$ docker pull nats-streaming@sha256:2209b5c3482a96a3dae3e8ade7aae5ec6caa7e077ad472779bada808eecbc268
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6287324539 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b52052c1bd51b6280c83afbc804f342150ad5265b218136f8b7fb1b464b7810`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 08 Dec 2021 08:38:00 GMT
RUN Install update ltsc2016-amd64
# Sat, 18 Dec 2021 01:55:44 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Sat, 18 Dec 2021 04:34:51 GMT
ENV NATS_DOCKERIZED=1
# Sat, 18 Dec 2021 08:02:56 GMT
ENV NATS_STREAMING_SERVER=0.23.2
# Sat, 18 Dec 2021 08:02:57 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.23.2/nats-streaming-server-v0.23.2-windows-amd64.zip
# Sat, 18 Dec 2021 08:02:58 GMT
ENV NATS_STREAMING_SERVER_SHASUM=b28dc8e1565d6fece68781515f759b0ed870831cdf2f7925cff7cf9acb44e7ec
# Sat, 18 Dec 2021 08:03:46 GMT
RUN Set-PSDebug -Trace 2
# Sat, 18 Dec 2021 08:05:31 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Sat, 18 Dec 2021 08:05:32 GMT
EXPOSE 4222 8222
# Sat, 18 Dec 2021 08:05:33 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Sat, 18 Dec 2021 08:05:34 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2d026d646213ccf73d9f0584941d108253d62e73df2a74e070776884b7b0242b`  
		Size: 2.2 GB (2204728802 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f6bffd19db3f71ba2031bea25a529c67034869e7e1bbf9e2431d5ee747bd6d6d`  
		Last Modified: Sat, 18 Dec 2021 04:00:01 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05006360e7d5d5f0fc5160410fd98cfab768e620dca3f3fbc5b44e611e3039b4`  
		Last Modified: Sat, 18 Dec 2021 08:06:58 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c79673abbfda8355eb19c36d4a838ea039890c3b36baaa24cd9c6f350f9dbaf6`  
		Last Modified: Sat, 18 Dec 2021 08:06:57 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56135df6f0d37ae5054fdc25bf5318d041b879e122c85613d52e71729262aea1`  
		Last Modified: Sat, 18 Dec 2021 08:06:57 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ec44dadd27b2b6ed2c809e4535ad5c1cb2ced6a10857849e9434b533cdb27ce`  
		Last Modified: Sat, 18 Dec 2021 08:06:57 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9f0a80a8e8d81c759bbe086bda6032ced235dd3acd963be9eb97a6aa4fe794d`  
		Last Modified: Sat, 18 Dec 2021 08:06:55 GMT  
		Size: 328.3 KB (328284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fc6eb7f28bcbbc325f606ce67eb09e5996052f69f474b1460ee1a08fd6f326a`  
		Last Modified: Sat, 18 Dec 2021 08:06:58 GMT  
		Size: 12.3 MB (12270678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d1b9cee769ed5bc39fd057d6669bc9630960eebf6507cd19a5f4b9ebc5a4953`  
		Last Modified: Sat, 18 Dec 2021 08:06:55 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8df8e108c24c7aff3a16b44fbf9243d457b7d5d45e701f2af5601985424595b7`  
		Last Modified: Sat, 18 Dec 2021 08:06:55 GMT  
		Size: 1.3 KB (1343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:298ef1dbe7d3eca580edccaab1932ba55fc39eeef55cb80c3221a4abf9e1f0e5`  
		Last Modified: Sat, 18 Dec 2021 08:06:55 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.23.2-windowsservercore-1809`

```console
$ docker pull nats-streaming@sha256:e8717b1af9495be0396d6b91c3b9be076fc62c4d5c27222d253340050d8e70bb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2366; amd64

### `nats-streaming:0.23.2-windowsservercore-1809` - windows version 10.0.17763.2366; amd64

```console
$ docker pull nats-streaming@sha256:420220a9afa15857377173cc8f141ae0373a42f666d9d133fcf747088a6d87a0
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2716755888 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e34c0986c57d10e61a41f5d9d253df4fb832be016255f195afb5b747924e636d`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 07 Dec 2021 04:56:01 GMT
RUN Install update 1809-amd64
# Sat, 18 Dec 2021 01:40:43 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Sat, 18 Dec 2021 04:32:10 GMT
ENV NATS_DOCKERIZED=1
# Sat, 18 Dec 2021 07:59:49 GMT
ENV NATS_STREAMING_SERVER=0.23.2
# Sat, 18 Dec 2021 07:59:50 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.23.2/nats-streaming-server-v0.23.2-windows-amd64.zip
# Sat, 18 Dec 2021 07:59:51 GMT
ENV NATS_STREAMING_SERVER_SHASUM=b28dc8e1565d6fece68781515f759b0ed870831cdf2f7925cff7cf9acb44e7ec
# Sat, 18 Dec 2021 08:00:48 GMT
RUN Set-PSDebug -Trace 2
# Sat, 18 Dec 2021 08:02:34 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Sat, 18 Dec 2021 08:02:35 GMT
EXPOSE 4222 8222
# Sat, 18 Dec 2021 08:02:36 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Sat, 18 Dec 2021 08:02:37 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5ee7a7ea9cf22f75886179907a41810a992e21f3d0c57cc10d2147ce9237701c`  
		Size: 990.3 MB (990271574 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d22d2238b031d3f13bcd6c144e80f8f8402332b8ee8e53cc54b7912c3ac808cb`  
		Last Modified: Sat, 18 Dec 2021 03:59:34 GMT  
		Size: 1.4 KB (1444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44c5f7f5394b88876960b5ac27980fb2e22584cf50ecde4d9537e88ddbf849c3`  
		Last Modified: Sat, 18 Dec 2021 08:06:16 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d4330e24c7d8e5e42a117873554d01f36a0dc5de956de58eb98bc343f3b7053`  
		Last Modified: Sat, 18 Dec 2021 08:06:16 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a85e10ba361bd6036ce996ef1fc18a56eae46bfe2f2a3aa167c91a9910e44b1e`  
		Last Modified: Sat, 18 Dec 2021 08:06:16 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73619ef7215a1f395f4b26e9d2c8f3163b1eadc526a4b86834c34d2d210bbbb5`  
		Last Modified: Sat, 18 Dec 2021 08:06:16 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:585f06960fbd4efa8dc36c8d215c51aa6c8e6adadb62e05f799bc7770a768385`  
		Last Modified: Sat, 18 Dec 2021 08:06:14 GMT  
		Size: 365.8 KB (365782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b13efc00f53324e98bc4459fd1a2e6c14d2dbb3ddce59ac2d39a8d2976ead8d`  
		Last Modified: Sat, 18 Dec 2021 08:06:22 GMT  
		Size: 7.8 MB (7774250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cfbd74dd7052b02b86f232c8f3bc9d759fd4f2a1f81fcf4748927895a03331c`  
		Last Modified: Sat, 18 Dec 2021 08:06:14 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9da21c0ea9106d6386e5f731911254e0aad700297c81ecb6b7cbc2b22a81e36`  
		Last Modified: Sat, 18 Dec 2021 08:06:14 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2561dd2bec68b686d5c3e5494fffeb0a77f681864f74eb9fed80413145fbeca2`  
		Last Modified: Sat, 18 Dec 2021 08:06:14 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.23.2-windowsservercore-ltsc2016`

```console
$ docker pull nats-streaming@sha256:62945f3e51902319046e2bd0464be26fc730aea2850268b77ce48818ad493d09
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.14393.4825; amd64

### `nats-streaming:0.23.2-windowsservercore-ltsc2016` - windows version 10.0.14393.4825; amd64

```console
$ docker pull nats-streaming@sha256:2209b5c3482a96a3dae3e8ade7aae5ec6caa7e077ad472779bada808eecbc268
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6287324539 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b52052c1bd51b6280c83afbc804f342150ad5265b218136f8b7fb1b464b7810`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 08 Dec 2021 08:38:00 GMT
RUN Install update ltsc2016-amd64
# Sat, 18 Dec 2021 01:55:44 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Sat, 18 Dec 2021 04:34:51 GMT
ENV NATS_DOCKERIZED=1
# Sat, 18 Dec 2021 08:02:56 GMT
ENV NATS_STREAMING_SERVER=0.23.2
# Sat, 18 Dec 2021 08:02:57 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.23.2/nats-streaming-server-v0.23.2-windows-amd64.zip
# Sat, 18 Dec 2021 08:02:58 GMT
ENV NATS_STREAMING_SERVER_SHASUM=b28dc8e1565d6fece68781515f759b0ed870831cdf2f7925cff7cf9acb44e7ec
# Sat, 18 Dec 2021 08:03:46 GMT
RUN Set-PSDebug -Trace 2
# Sat, 18 Dec 2021 08:05:31 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Sat, 18 Dec 2021 08:05:32 GMT
EXPOSE 4222 8222
# Sat, 18 Dec 2021 08:05:33 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Sat, 18 Dec 2021 08:05:34 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2d026d646213ccf73d9f0584941d108253d62e73df2a74e070776884b7b0242b`  
		Size: 2.2 GB (2204728802 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f6bffd19db3f71ba2031bea25a529c67034869e7e1bbf9e2431d5ee747bd6d6d`  
		Last Modified: Sat, 18 Dec 2021 04:00:01 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05006360e7d5d5f0fc5160410fd98cfab768e620dca3f3fbc5b44e611e3039b4`  
		Last Modified: Sat, 18 Dec 2021 08:06:58 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c79673abbfda8355eb19c36d4a838ea039890c3b36baaa24cd9c6f350f9dbaf6`  
		Last Modified: Sat, 18 Dec 2021 08:06:57 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56135df6f0d37ae5054fdc25bf5318d041b879e122c85613d52e71729262aea1`  
		Last Modified: Sat, 18 Dec 2021 08:06:57 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ec44dadd27b2b6ed2c809e4535ad5c1cb2ced6a10857849e9434b533cdb27ce`  
		Last Modified: Sat, 18 Dec 2021 08:06:57 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9f0a80a8e8d81c759bbe086bda6032ced235dd3acd963be9eb97a6aa4fe794d`  
		Last Modified: Sat, 18 Dec 2021 08:06:55 GMT  
		Size: 328.3 KB (328284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fc6eb7f28bcbbc325f606ce67eb09e5996052f69f474b1460ee1a08fd6f326a`  
		Last Modified: Sat, 18 Dec 2021 08:06:58 GMT  
		Size: 12.3 MB (12270678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d1b9cee769ed5bc39fd057d6669bc9630960eebf6507cd19a5f4b9ebc5a4953`  
		Last Modified: Sat, 18 Dec 2021 08:06:55 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8df8e108c24c7aff3a16b44fbf9243d457b7d5d45e701f2af5601985424595b7`  
		Last Modified: Sat, 18 Dec 2021 08:06:55 GMT  
		Size: 1.3 KB (1343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:298ef1dbe7d3eca580edccaab1932ba55fc39eeef55cb80c3221a4abf9e1f0e5`  
		Last Modified: Sat, 18 Dec 2021 08:06:55 GMT  
		Size: 1.3 KB (1294 bytes)  
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
$ docker pull nats-streaming@sha256:c3b67c2c329064941f788aeb9e2f357b1d2c4ed918487e44c56b735dd3825e6c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.2366; amd64

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

### `nats-streaming:latest` - windows version 10.0.17763.2366; amd64

```console
$ docker pull nats-streaming@sha256:a4dba6a1799f5368dc9d421fd4ea4fd201eddd12c10864382c9d1b6bc14c6aeb
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.3 MB (110331179 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc58ce624f6204540e8ac39bafdd9726fbc32ea7c229b38b030f5f2e64cec9d2`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 07 Dec 2021 04:37:11 GMT
RUN Apply image 1809-amd64
# Sat, 18 Dec 2021 04:34:39 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Sat, 18 Dec 2021 08:02:47 GMT
RUN cmd /S /C #(nop) COPY file:bb30895f60b97f75adc45bbc64dd23d70df079c19ad26c4f8d07ce1c88e77c96 in C:\nats-streaming-server.exe 
# Sat, 18 Dec 2021 08:02:48 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Sat, 18 Dec 2021 08:02:49 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Sat, 18 Dec 2021 08:02:49 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:034b2f457cdf6a0d3f7024523d40fd6eeb8568e6c76d9fa56f4053fcf3a21d63`  
		Size: 102.9 MB (102904001 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4f56553f84cd7b4574c0b4d1ee6585d70eda0c9f3a5f1b276ec5e7cdc713bd74`  
		Last Modified: Sat, 18 Dec 2021 08:06:40 GMT  
		Size: 1.2 KB (1178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a1496d31642d0470cbd25b3b734e0088588c71a12ec3db986575765cf928b8c`  
		Last Modified: Sat, 18 Dec 2021 08:06:42 GMT  
		Size: 7.4 MB (7422515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d168df35b99b660b4221d21e47cc005e082df581fe415650ba67380ef77d51ed`  
		Last Modified: Sat, 18 Dec 2021 08:06:40 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f89cbe2ec75329f034c70155d630a4909bc7359f7a267f72844775e87c70631`  
		Last Modified: Sat, 18 Dec 2021 08:06:40 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c1ef79bfe81d12d8f6ae9b2499ef4e6f42bc0241fe3df4d7215ba2c6a25d251`  
		Last Modified: Sat, 18 Dec 2021 08:06:40 GMT  
		Size: 1.2 KB (1168 bytes)  
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
$ docker pull nats-streaming@sha256:9d12cde295f11487b395d0ff1500b3dc5e7343a26b80efca806bab8993c3e546
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2366; amd64

### `nats-streaming:nanoserver` - windows version 10.0.17763.2366; amd64

```console
$ docker pull nats-streaming@sha256:a4dba6a1799f5368dc9d421fd4ea4fd201eddd12c10864382c9d1b6bc14c6aeb
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.3 MB (110331179 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc58ce624f6204540e8ac39bafdd9726fbc32ea7c229b38b030f5f2e64cec9d2`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 07 Dec 2021 04:37:11 GMT
RUN Apply image 1809-amd64
# Sat, 18 Dec 2021 04:34:39 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Sat, 18 Dec 2021 08:02:47 GMT
RUN cmd /S /C #(nop) COPY file:bb30895f60b97f75adc45bbc64dd23d70df079c19ad26c4f8d07ce1c88e77c96 in C:\nats-streaming-server.exe 
# Sat, 18 Dec 2021 08:02:48 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Sat, 18 Dec 2021 08:02:49 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Sat, 18 Dec 2021 08:02:49 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:034b2f457cdf6a0d3f7024523d40fd6eeb8568e6c76d9fa56f4053fcf3a21d63`  
		Size: 102.9 MB (102904001 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4f56553f84cd7b4574c0b4d1ee6585d70eda0c9f3a5f1b276ec5e7cdc713bd74`  
		Last Modified: Sat, 18 Dec 2021 08:06:40 GMT  
		Size: 1.2 KB (1178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a1496d31642d0470cbd25b3b734e0088588c71a12ec3db986575765cf928b8c`  
		Last Modified: Sat, 18 Dec 2021 08:06:42 GMT  
		Size: 7.4 MB (7422515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d168df35b99b660b4221d21e47cc005e082df581fe415650ba67380ef77d51ed`  
		Last Modified: Sat, 18 Dec 2021 08:06:40 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f89cbe2ec75329f034c70155d630a4909bc7359f7a267f72844775e87c70631`  
		Last Modified: Sat, 18 Dec 2021 08:06:40 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c1ef79bfe81d12d8f6ae9b2499ef4e6f42bc0241fe3df4d7215ba2c6a25d251`  
		Last Modified: Sat, 18 Dec 2021 08:06:40 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:nanoserver-1809`

```console
$ docker pull nats-streaming@sha256:9d12cde295f11487b395d0ff1500b3dc5e7343a26b80efca806bab8993c3e546
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2366; amd64

### `nats-streaming:nanoserver-1809` - windows version 10.0.17763.2366; amd64

```console
$ docker pull nats-streaming@sha256:a4dba6a1799f5368dc9d421fd4ea4fd201eddd12c10864382c9d1b6bc14c6aeb
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.3 MB (110331179 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc58ce624f6204540e8ac39bafdd9726fbc32ea7c229b38b030f5f2e64cec9d2`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 07 Dec 2021 04:37:11 GMT
RUN Apply image 1809-amd64
# Sat, 18 Dec 2021 04:34:39 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Sat, 18 Dec 2021 08:02:47 GMT
RUN cmd /S /C #(nop) COPY file:bb30895f60b97f75adc45bbc64dd23d70df079c19ad26c4f8d07ce1c88e77c96 in C:\nats-streaming-server.exe 
# Sat, 18 Dec 2021 08:02:48 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Sat, 18 Dec 2021 08:02:49 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Sat, 18 Dec 2021 08:02:49 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:034b2f457cdf6a0d3f7024523d40fd6eeb8568e6c76d9fa56f4053fcf3a21d63`  
		Size: 102.9 MB (102904001 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4f56553f84cd7b4574c0b4d1ee6585d70eda0c9f3a5f1b276ec5e7cdc713bd74`  
		Last Modified: Sat, 18 Dec 2021 08:06:40 GMT  
		Size: 1.2 KB (1178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a1496d31642d0470cbd25b3b734e0088588c71a12ec3db986575765cf928b8c`  
		Last Modified: Sat, 18 Dec 2021 08:06:42 GMT  
		Size: 7.4 MB (7422515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d168df35b99b660b4221d21e47cc005e082df581fe415650ba67380ef77d51ed`  
		Last Modified: Sat, 18 Dec 2021 08:06:40 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f89cbe2ec75329f034c70155d630a4909bc7359f7a267f72844775e87c70631`  
		Last Modified: Sat, 18 Dec 2021 08:06:40 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c1ef79bfe81d12d8f6ae9b2499ef4e6f42bc0241fe3df4d7215ba2c6a25d251`  
		Last Modified: Sat, 18 Dec 2021 08:06:40 GMT  
		Size: 1.2 KB (1168 bytes)  
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
$ docker pull nats-streaming@sha256:be9484f94d3f173a10ce890420589378d6f8ca4bd0205f0197cdfa6d0646ea69
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.2366; amd64
	-	windows version 10.0.14393.4825; amd64

### `nats-streaming:windowsservercore` - windows version 10.0.17763.2366; amd64

```console
$ docker pull nats-streaming@sha256:420220a9afa15857377173cc8f141ae0373a42f666d9d133fcf747088a6d87a0
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2716755888 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e34c0986c57d10e61a41f5d9d253df4fb832be016255f195afb5b747924e636d`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 07 Dec 2021 04:56:01 GMT
RUN Install update 1809-amd64
# Sat, 18 Dec 2021 01:40:43 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Sat, 18 Dec 2021 04:32:10 GMT
ENV NATS_DOCKERIZED=1
# Sat, 18 Dec 2021 07:59:49 GMT
ENV NATS_STREAMING_SERVER=0.23.2
# Sat, 18 Dec 2021 07:59:50 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.23.2/nats-streaming-server-v0.23.2-windows-amd64.zip
# Sat, 18 Dec 2021 07:59:51 GMT
ENV NATS_STREAMING_SERVER_SHASUM=b28dc8e1565d6fece68781515f759b0ed870831cdf2f7925cff7cf9acb44e7ec
# Sat, 18 Dec 2021 08:00:48 GMT
RUN Set-PSDebug -Trace 2
# Sat, 18 Dec 2021 08:02:34 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Sat, 18 Dec 2021 08:02:35 GMT
EXPOSE 4222 8222
# Sat, 18 Dec 2021 08:02:36 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Sat, 18 Dec 2021 08:02:37 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5ee7a7ea9cf22f75886179907a41810a992e21f3d0c57cc10d2147ce9237701c`  
		Size: 990.3 MB (990271574 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d22d2238b031d3f13bcd6c144e80f8f8402332b8ee8e53cc54b7912c3ac808cb`  
		Last Modified: Sat, 18 Dec 2021 03:59:34 GMT  
		Size: 1.4 KB (1444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44c5f7f5394b88876960b5ac27980fb2e22584cf50ecde4d9537e88ddbf849c3`  
		Last Modified: Sat, 18 Dec 2021 08:06:16 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d4330e24c7d8e5e42a117873554d01f36a0dc5de956de58eb98bc343f3b7053`  
		Last Modified: Sat, 18 Dec 2021 08:06:16 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a85e10ba361bd6036ce996ef1fc18a56eae46bfe2f2a3aa167c91a9910e44b1e`  
		Last Modified: Sat, 18 Dec 2021 08:06:16 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73619ef7215a1f395f4b26e9d2c8f3163b1eadc526a4b86834c34d2d210bbbb5`  
		Last Modified: Sat, 18 Dec 2021 08:06:16 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:585f06960fbd4efa8dc36c8d215c51aa6c8e6adadb62e05f799bc7770a768385`  
		Last Modified: Sat, 18 Dec 2021 08:06:14 GMT  
		Size: 365.8 KB (365782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b13efc00f53324e98bc4459fd1a2e6c14d2dbb3ddce59ac2d39a8d2976ead8d`  
		Last Modified: Sat, 18 Dec 2021 08:06:22 GMT  
		Size: 7.8 MB (7774250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cfbd74dd7052b02b86f232c8f3bc9d759fd4f2a1f81fcf4748927895a03331c`  
		Last Modified: Sat, 18 Dec 2021 08:06:14 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9da21c0ea9106d6386e5f731911254e0aad700297c81ecb6b7cbc2b22a81e36`  
		Last Modified: Sat, 18 Dec 2021 08:06:14 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2561dd2bec68b686d5c3e5494fffeb0a77f681864f74eb9fed80413145fbeca2`  
		Last Modified: Sat, 18 Dec 2021 08:06:14 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:windowsservercore` - windows version 10.0.14393.4825; amd64

```console
$ docker pull nats-streaming@sha256:2209b5c3482a96a3dae3e8ade7aae5ec6caa7e077ad472779bada808eecbc268
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6287324539 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b52052c1bd51b6280c83afbc804f342150ad5265b218136f8b7fb1b464b7810`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 08 Dec 2021 08:38:00 GMT
RUN Install update ltsc2016-amd64
# Sat, 18 Dec 2021 01:55:44 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Sat, 18 Dec 2021 04:34:51 GMT
ENV NATS_DOCKERIZED=1
# Sat, 18 Dec 2021 08:02:56 GMT
ENV NATS_STREAMING_SERVER=0.23.2
# Sat, 18 Dec 2021 08:02:57 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.23.2/nats-streaming-server-v0.23.2-windows-amd64.zip
# Sat, 18 Dec 2021 08:02:58 GMT
ENV NATS_STREAMING_SERVER_SHASUM=b28dc8e1565d6fece68781515f759b0ed870831cdf2f7925cff7cf9acb44e7ec
# Sat, 18 Dec 2021 08:03:46 GMT
RUN Set-PSDebug -Trace 2
# Sat, 18 Dec 2021 08:05:31 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Sat, 18 Dec 2021 08:05:32 GMT
EXPOSE 4222 8222
# Sat, 18 Dec 2021 08:05:33 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Sat, 18 Dec 2021 08:05:34 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2d026d646213ccf73d9f0584941d108253d62e73df2a74e070776884b7b0242b`  
		Size: 2.2 GB (2204728802 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f6bffd19db3f71ba2031bea25a529c67034869e7e1bbf9e2431d5ee747bd6d6d`  
		Last Modified: Sat, 18 Dec 2021 04:00:01 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05006360e7d5d5f0fc5160410fd98cfab768e620dca3f3fbc5b44e611e3039b4`  
		Last Modified: Sat, 18 Dec 2021 08:06:58 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c79673abbfda8355eb19c36d4a838ea039890c3b36baaa24cd9c6f350f9dbaf6`  
		Last Modified: Sat, 18 Dec 2021 08:06:57 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56135df6f0d37ae5054fdc25bf5318d041b879e122c85613d52e71729262aea1`  
		Last Modified: Sat, 18 Dec 2021 08:06:57 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ec44dadd27b2b6ed2c809e4535ad5c1cb2ced6a10857849e9434b533cdb27ce`  
		Last Modified: Sat, 18 Dec 2021 08:06:57 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9f0a80a8e8d81c759bbe086bda6032ced235dd3acd963be9eb97a6aa4fe794d`  
		Last Modified: Sat, 18 Dec 2021 08:06:55 GMT  
		Size: 328.3 KB (328284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fc6eb7f28bcbbc325f606ce67eb09e5996052f69f474b1460ee1a08fd6f326a`  
		Last Modified: Sat, 18 Dec 2021 08:06:58 GMT  
		Size: 12.3 MB (12270678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d1b9cee769ed5bc39fd057d6669bc9630960eebf6507cd19a5f4b9ebc5a4953`  
		Last Modified: Sat, 18 Dec 2021 08:06:55 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8df8e108c24c7aff3a16b44fbf9243d457b7d5d45e701f2af5601985424595b7`  
		Last Modified: Sat, 18 Dec 2021 08:06:55 GMT  
		Size: 1.3 KB (1343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:298ef1dbe7d3eca580edccaab1932ba55fc39eeef55cb80c3221a4abf9e1f0e5`  
		Last Modified: Sat, 18 Dec 2021 08:06:55 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:windowsservercore-1809`

```console
$ docker pull nats-streaming@sha256:e8717b1af9495be0396d6b91c3b9be076fc62c4d5c27222d253340050d8e70bb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2366; amd64

### `nats-streaming:windowsservercore-1809` - windows version 10.0.17763.2366; amd64

```console
$ docker pull nats-streaming@sha256:420220a9afa15857377173cc8f141ae0373a42f666d9d133fcf747088a6d87a0
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2716755888 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e34c0986c57d10e61a41f5d9d253df4fb832be016255f195afb5b747924e636d`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 07 Dec 2021 04:56:01 GMT
RUN Install update 1809-amd64
# Sat, 18 Dec 2021 01:40:43 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Sat, 18 Dec 2021 04:32:10 GMT
ENV NATS_DOCKERIZED=1
# Sat, 18 Dec 2021 07:59:49 GMT
ENV NATS_STREAMING_SERVER=0.23.2
# Sat, 18 Dec 2021 07:59:50 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.23.2/nats-streaming-server-v0.23.2-windows-amd64.zip
# Sat, 18 Dec 2021 07:59:51 GMT
ENV NATS_STREAMING_SERVER_SHASUM=b28dc8e1565d6fece68781515f759b0ed870831cdf2f7925cff7cf9acb44e7ec
# Sat, 18 Dec 2021 08:00:48 GMT
RUN Set-PSDebug -Trace 2
# Sat, 18 Dec 2021 08:02:34 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Sat, 18 Dec 2021 08:02:35 GMT
EXPOSE 4222 8222
# Sat, 18 Dec 2021 08:02:36 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Sat, 18 Dec 2021 08:02:37 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5ee7a7ea9cf22f75886179907a41810a992e21f3d0c57cc10d2147ce9237701c`  
		Size: 990.3 MB (990271574 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d22d2238b031d3f13bcd6c144e80f8f8402332b8ee8e53cc54b7912c3ac808cb`  
		Last Modified: Sat, 18 Dec 2021 03:59:34 GMT  
		Size: 1.4 KB (1444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44c5f7f5394b88876960b5ac27980fb2e22584cf50ecde4d9537e88ddbf849c3`  
		Last Modified: Sat, 18 Dec 2021 08:06:16 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d4330e24c7d8e5e42a117873554d01f36a0dc5de956de58eb98bc343f3b7053`  
		Last Modified: Sat, 18 Dec 2021 08:06:16 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a85e10ba361bd6036ce996ef1fc18a56eae46bfe2f2a3aa167c91a9910e44b1e`  
		Last Modified: Sat, 18 Dec 2021 08:06:16 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73619ef7215a1f395f4b26e9d2c8f3163b1eadc526a4b86834c34d2d210bbbb5`  
		Last Modified: Sat, 18 Dec 2021 08:06:16 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:585f06960fbd4efa8dc36c8d215c51aa6c8e6adadb62e05f799bc7770a768385`  
		Last Modified: Sat, 18 Dec 2021 08:06:14 GMT  
		Size: 365.8 KB (365782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b13efc00f53324e98bc4459fd1a2e6c14d2dbb3ddce59ac2d39a8d2976ead8d`  
		Last Modified: Sat, 18 Dec 2021 08:06:22 GMT  
		Size: 7.8 MB (7774250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cfbd74dd7052b02b86f232c8f3bc9d759fd4f2a1f81fcf4748927895a03331c`  
		Last Modified: Sat, 18 Dec 2021 08:06:14 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9da21c0ea9106d6386e5f731911254e0aad700297c81ecb6b7cbc2b22a81e36`  
		Last Modified: Sat, 18 Dec 2021 08:06:14 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2561dd2bec68b686d5c3e5494fffeb0a77f681864f74eb9fed80413145fbeca2`  
		Last Modified: Sat, 18 Dec 2021 08:06:14 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:windowsservercore-ltsc2016`

```console
$ docker pull nats-streaming@sha256:62945f3e51902319046e2bd0464be26fc730aea2850268b77ce48818ad493d09
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.14393.4825; amd64

### `nats-streaming:windowsservercore-ltsc2016` - windows version 10.0.14393.4825; amd64

```console
$ docker pull nats-streaming@sha256:2209b5c3482a96a3dae3e8ade7aae5ec6caa7e077ad472779bada808eecbc268
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6287324539 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b52052c1bd51b6280c83afbc804f342150ad5265b218136f8b7fb1b464b7810`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 08 Dec 2021 08:38:00 GMT
RUN Install update ltsc2016-amd64
# Sat, 18 Dec 2021 01:55:44 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Sat, 18 Dec 2021 04:34:51 GMT
ENV NATS_DOCKERIZED=1
# Sat, 18 Dec 2021 08:02:56 GMT
ENV NATS_STREAMING_SERVER=0.23.2
# Sat, 18 Dec 2021 08:02:57 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.23.2/nats-streaming-server-v0.23.2-windows-amd64.zip
# Sat, 18 Dec 2021 08:02:58 GMT
ENV NATS_STREAMING_SERVER_SHASUM=b28dc8e1565d6fece68781515f759b0ed870831cdf2f7925cff7cf9acb44e7ec
# Sat, 18 Dec 2021 08:03:46 GMT
RUN Set-PSDebug -Trace 2
# Sat, 18 Dec 2021 08:05:31 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Sat, 18 Dec 2021 08:05:32 GMT
EXPOSE 4222 8222
# Sat, 18 Dec 2021 08:05:33 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Sat, 18 Dec 2021 08:05:34 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2d026d646213ccf73d9f0584941d108253d62e73df2a74e070776884b7b0242b`  
		Size: 2.2 GB (2204728802 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f6bffd19db3f71ba2031bea25a529c67034869e7e1bbf9e2431d5ee747bd6d6d`  
		Last Modified: Sat, 18 Dec 2021 04:00:01 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05006360e7d5d5f0fc5160410fd98cfab768e620dca3f3fbc5b44e611e3039b4`  
		Last Modified: Sat, 18 Dec 2021 08:06:58 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c79673abbfda8355eb19c36d4a838ea039890c3b36baaa24cd9c6f350f9dbaf6`  
		Last Modified: Sat, 18 Dec 2021 08:06:57 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56135df6f0d37ae5054fdc25bf5318d041b879e122c85613d52e71729262aea1`  
		Last Modified: Sat, 18 Dec 2021 08:06:57 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ec44dadd27b2b6ed2c809e4535ad5c1cb2ced6a10857849e9434b533cdb27ce`  
		Last Modified: Sat, 18 Dec 2021 08:06:57 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9f0a80a8e8d81c759bbe086bda6032ced235dd3acd963be9eb97a6aa4fe794d`  
		Last Modified: Sat, 18 Dec 2021 08:06:55 GMT  
		Size: 328.3 KB (328284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fc6eb7f28bcbbc325f606ce67eb09e5996052f69f474b1460ee1a08fd6f326a`  
		Last Modified: Sat, 18 Dec 2021 08:06:58 GMT  
		Size: 12.3 MB (12270678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d1b9cee769ed5bc39fd057d6669bc9630960eebf6507cd19a5f4b9ebc5a4953`  
		Last Modified: Sat, 18 Dec 2021 08:06:55 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8df8e108c24c7aff3a16b44fbf9243d457b7d5d45e701f2af5601985424595b7`  
		Last Modified: Sat, 18 Dec 2021 08:06:55 GMT  
		Size: 1.3 KB (1343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:298ef1dbe7d3eca580edccaab1932ba55fc39eeef55cb80c3221a4abf9e1f0e5`  
		Last Modified: Sat, 18 Dec 2021 08:06:55 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
