<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `nats-streaming`

-	[`nats-streaming:0.22`](#nats-streaming022)
-	[`nats-streaming:0.22-alpine`](#nats-streaming022-alpine)
-	[`nats-streaming:0.22-alpine3.14`](#nats-streaming022-alpine314)
-	[`nats-streaming:0.22-linux`](#nats-streaming022-linux)
-	[`nats-streaming:0.22-nanoserver`](#nats-streaming022-nanoserver)
-	[`nats-streaming:0.22-nanoserver-1809`](#nats-streaming022-nanoserver-1809)
-	[`nats-streaming:0.22-scratch`](#nats-streaming022-scratch)
-	[`nats-streaming:0.22-windowsservercore`](#nats-streaming022-windowsservercore)
-	[`nats-streaming:0.22-windowsservercore-1809`](#nats-streaming022-windowsservercore-1809)
-	[`nats-streaming:0.22-windowsservercore-ltsc2016`](#nats-streaming022-windowsservercore-ltsc2016)
-	[`nats-streaming:0.22.1`](#nats-streaming0221)
-	[`nats-streaming:0.22.1-alpine`](#nats-streaming0221-alpine)
-	[`nats-streaming:0.22.1-alpine3.14`](#nats-streaming0221-alpine314)
-	[`nats-streaming:0.22.1-linux`](#nats-streaming0221-linux)
-	[`nats-streaming:0.22.1-nanoserver`](#nats-streaming0221-nanoserver)
-	[`nats-streaming:0.22.1-nanoserver-1809`](#nats-streaming0221-nanoserver-1809)
-	[`nats-streaming:0.22.1-scratch`](#nats-streaming0221-scratch)
-	[`nats-streaming:0.22.1-windowsservercore`](#nats-streaming0221-windowsservercore)
-	[`nats-streaming:0.22.1-windowsservercore-1809`](#nats-streaming0221-windowsservercore-1809)
-	[`nats-streaming:0.22.1-windowsservercore-ltsc2016`](#nats-streaming0221-windowsservercore-ltsc2016)
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

## `nats-streaming:0.22`

```console
$ docker pull nats-streaming@sha256:f54d0597f76528b26771a5cacf18f82627877a247c788bcc0aad528f763c0b85
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.2061; amd64

### `nats-streaming:0.22` - linux; amd64

```console
$ docker pull nats-streaming@sha256:3c6c9375f9e9724462e98cfb98a7abb50ceeca73b3070ce061992c4009e32157
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7168713 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:184d7920ac61dd2e84320b8040f57980a7d605d42948a520ede12d421168c4ce`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 02 Aug 2021 22:20:03 GMT
COPY file:ca9a212ccef327f9c2e91a62a908ac0cdbd39b08be331ea2b209c2d724942e18 in /nats-streaming-server 
# Mon, 02 Aug 2021 22:20:03 GMT
EXPOSE 4222 8222
# Mon, 02 Aug 2021 22:20:03 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 02 Aug 2021 22:20:03 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:f3749ab6cbfff03714b5a6a1245fa249b67d19e7358b74cbc50232b14370481a`  
		Last Modified: Mon, 02 Aug 2021 22:20:48 GMT  
		Size: 7.2 MB (7168713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.22` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:e944d0e843d59d5979d7561c06b0c0adc874ceaa0bd34d3a7b536b25e8c9704d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.7 MB (6650246 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0146bbca3802c65d86e148b1d203b3d395ca1cd8a8bb89461888570d821dc4fb`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 02 Aug 2021 22:51:34 GMT
COPY file:68ac67d86d6ac617adc181feb43580415b7fc7640a3c7577bb3753c369908da0 in /nats-streaming-server 
# Mon, 02 Aug 2021 22:51:35 GMT
EXPOSE 4222 8222
# Mon, 02 Aug 2021 22:51:35 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 02 Aug 2021 22:51:35 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:c7e1d707b6179f690f3f44212cb8c9a3fe914d91d3f1ddbac9f176aa0610c90a`  
		Last Modified: Mon, 02 Aug 2021 22:53:32 GMT  
		Size: 6.7 MB (6650246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.22` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:a5e3d56b343f9091f353634f59f688998544ccd4f2cbb80001d08ea6a3207274
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6639768 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80206ae32558812ad047d8ab67519615e98e7df68a884fc32b6d5fd8f72593b0`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 02 Aug 2021 23:11:17 GMT
COPY file:79708b5d249193a95e72c506453fd1ecd3e2738ec2ff3423c4b2bd760f426da2 in /nats-streaming-server 
# Mon, 02 Aug 2021 23:11:18 GMT
EXPOSE 4222 8222
# Mon, 02 Aug 2021 23:11:18 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 02 Aug 2021 23:11:19 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:52753762f751e166edd44e37a0ef0a06b33c337bdeb66e4134ee8479a49dae68`  
		Last Modified: Mon, 02 Aug 2021 23:13:17 GMT  
		Size: 6.6 MB (6639768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.22` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:96652223cce95275138363a54affb8663ba46bc75831c2a9535375ab6d922143
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 MB (6546324 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:952bbd74028df1debbfe0e4665b514c66a36537d0868d41bc971ddb55793c442`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 02 Aug 2021 22:40:16 GMT
COPY file:a77d9769f43cc6943be482183091d3360eaadf93bf1ef5a67f0869d5555868a6 in /nats-streaming-server 
# Mon, 02 Aug 2021 22:40:17 GMT
EXPOSE 4222 8222
# Mon, 02 Aug 2021 22:40:17 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 02 Aug 2021 22:40:17 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4dc8aa7843ed2da454d59006acb180caee3f980d12034caacd4a32ffedab3df7`  
		Last Modified: Mon, 02 Aug 2021 22:41:24 GMT  
		Size: 6.5 MB (6546324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.22` - windows version 10.0.17763.2061; amd64

```console
$ docker pull nats-streaming@sha256:349783a72dc891fd56179a54e998371cfe730524625447c5e5f8c8f99ef7d065
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.0 MB (110023666 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b2c8c7df75f26ed571fde792979a0ab215e1f76ff8e9a7f250cc092b15254741`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 06 Jul 2021 20:06:39 GMT
RUN Apply image 1809-amd64
# Wed, 14 Jul 2021 02:35:24 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Mon, 02 Aug 2021 22:17:13 GMT
RUN cmd /S /C #(nop) COPY file:9670e5d1fe5a71e47c78fde01235a0bcbcafcfdeeacf96a7669f6e49343fb03b in C:\nats-streaming-server.exe 
# Mon, 02 Aug 2021 22:17:16 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Mon, 02 Aug 2021 22:17:18 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Mon, 02 Aug 2021 22:17:21 GMT
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
	-	`sha256:395219f11b245d57e94766328eb17b3d461dcfac8402452fdc67df4b9e64361e`  
		Last Modified: Mon, 02 Aug 2021 22:22:03 GMT  
		Size: 7.3 MB (7293366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ed48c75b28949dec2cdb6cb3ff1179ad63c4c4371eba6a69a24baf25f2f6599`  
		Last Modified: Mon, 02 Aug 2021 22:21:54 GMT  
		Size: 1.2 KB (1173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a9b056cd35fd11d0c1057a2de6be2e533de9455af3383d08143215e972c3fd1`  
		Last Modified: Mon, 02 Aug 2021 22:21:55 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20642618c26e07a2aaf5f4169ff1a42ac92cb50404ebb140d800a9da097779ca`  
		Last Modified: Mon, 02 Aug 2021 22:21:55 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.22-alpine`

```console
$ docker pull nats-streaming@sha256:38d70776fbcfcba9e1cae6b3bffbf6824cba9e88544f08a307917e9812b16fff
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.22-alpine` - linux; amd64

```console
$ docker pull nats-streaming@sha256:5b970a21e7a42e1ddda100078fd4b44e290ddbc7235c99ea5aa3ff0c060d41d7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.3 MB (10267671 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f28bef93a614347e0c25d51fbe54017e3e9f7826c8de64a1381b54e86178d49`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Tue, 15 Jun 2021 22:19:37 GMT
ADD file:f278386b0cef68136129f5f58c52445590a417b624d62bca158d4dc926c340df in / 
# Tue, 15 Jun 2021 22:19:37 GMT
CMD ["/bin/sh"]
# Mon, 02 Aug 2021 22:19:52 GMT
ENV NATS_STREAMING_SERVER=0.22.1
# Mon, 02 Aug 2021 22:19:55 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='581698d248a19ecae64e4048d153bc1021744a3da6284680a339f9f82a53a9cf' ;; 		armhf) natsArch='arm6'; sha256='438a89221bb0608e40d21e73ca27a4b70b8560730726942c0ade94a6b6013d6f' ;; 		armv7) natsArch='arm7'; sha256='4164baadd201d1374f7654d3e54a24d81ceb87a385867e31a82c1d1a69e3b1ae' ;; 		x86_64) natsArch='amd64'; sha256='f29e87ac9ff998c928aa8ebc8cf0c4d04d34a3d95b9900d92fd7dafab2bec8cc' ;; 		x86) natsArch='386'; sha256='0ca68e57babb8901d7afeb7569042730904887e718ddf860ef3ee54278753505' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Mon, 02 Aug 2021 22:19:55 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Mon, 02 Aug 2021 22:19:56 GMT
EXPOSE 4222 8222
# Mon, 02 Aug 2021 22:19:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 02 Aug 2021 22:19:56 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:5843afab387455b37944e709ee8c78d7520df80f8d01cf7f861aae63beeddb6b`  
		Last Modified: Tue, 15 Jun 2021 22:20:04 GMT  
		Size: 2.8 MB (2811478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:306ccc624ab08668c75b4cb54fa3a827395cbd62ead7f920e817c9543c2429fc`  
		Last Modified: Mon, 02 Aug 2021 22:20:27 GMT  
		Size: 7.5 MB (7455771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2df3190f676bc1419fb755d81046ffd2842fc34e02d94f40e080e45c9f96a44d`  
		Last Modified: Mon, 02 Aug 2021 22:20:25 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.22-alpine` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:a6cf6a518fea52b3fc47ed4572652aa0e2350898b54cdbcc0f778150de352dbd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.6 MB (9559904 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c8b625df6f0e93de9095159d166249a43a96ef9f3013e4a2c483b5ac7bc972b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 06 Aug 2021 17:49:32 GMT
ADD file:7f2c7deda009eabdcbbdccb11e854043d32c498e64e7e1ca02165d7bb4261d39 in / 
# Fri, 06 Aug 2021 17:49:32 GMT
CMD ["/bin/sh"]
# Fri, 06 Aug 2021 18:59:05 GMT
ENV NATS_STREAMING_SERVER=0.22.1
# Fri, 06 Aug 2021 18:59:10 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='581698d248a19ecae64e4048d153bc1021744a3da6284680a339f9f82a53a9cf' ;; 		armhf) natsArch='arm6'; sha256='438a89221bb0608e40d21e73ca27a4b70b8560730726942c0ade94a6b6013d6f' ;; 		armv7) natsArch='arm7'; sha256='4164baadd201d1374f7654d3e54a24d81ceb87a385867e31a82c1d1a69e3b1ae' ;; 		x86_64) natsArch='amd64'; sha256='f29e87ac9ff998c928aa8ebc8cf0c4d04d34a3d95b9900d92fd7dafab2bec8cc' ;; 		x86) natsArch='386'; sha256='0ca68e57babb8901d7afeb7569042730904887e718ddf860ef3ee54278753505' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 06 Aug 2021 18:59:10 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Fri, 06 Aug 2021 18:59:11 GMT
EXPOSE 4222 8222
# Fri, 06 Aug 2021 18:59:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 06 Aug 2021 18:59:12 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:f465bb3e9fcd0c42f936ecc566c6e40353c00f3089b2b2c2ea1663c30f89d3ab`  
		Last Modified: Fri, 06 Aug 2021 17:51:00 GMT  
		Size: 2.6 MB (2626350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:719cf2771983cbb32331cc8915e2edce30fbcb308f3504276742ffc9a3bc35fd`  
		Last Modified: Fri, 06 Aug 2021 19:00:56 GMT  
		Size: 6.9 MB (6933133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a72de2e4e74462365f574ec07048641b834163995d6b95fb88af2fca27e01883`  
		Last Modified: Fri, 06 Aug 2021 19:00:52 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.22-alpine` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:572d6d4e53f14a9544d472214ec89300b1dbcc5e001d38c43b3ca6c656938369
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.3 MB (9349872 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5cc85837d0c5d21cf170c6240732f68dacf8b8aefb18875e65bec1f20f22f614`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 30 Jul 2021 18:36:19 GMT
ADD file:416a8b507abdc6bdcb22997a4be0a4170796c3f9f77e315b2dbff2b0a212bc68 in / 
# Fri, 30 Jul 2021 18:36:20 GMT
CMD ["/bin/sh"]
# Mon, 02 Aug 2021 23:10:49 GMT
ENV NATS_STREAMING_SERVER=0.22.1
# Mon, 02 Aug 2021 23:10:54 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='581698d248a19ecae64e4048d153bc1021744a3da6284680a339f9f82a53a9cf' ;; 		armhf) natsArch='arm6'; sha256='438a89221bb0608e40d21e73ca27a4b70b8560730726942c0ade94a6b6013d6f' ;; 		armv7) natsArch='arm7'; sha256='4164baadd201d1374f7654d3e54a24d81ceb87a385867e31a82c1d1a69e3b1ae' ;; 		x86_64) natsArch='amd64'; sha256='f29e87ac9ff998c928aa8ebc8cf0c4d04d34a3d95b9900d92fd7dafab2bec8cc' ;; 		x86) natsArch='386'; sha256='0ca68e57babb8901d7afeb7569042730904887e718ddf860ef3ee54278753505' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Mon, 02 Aug 2021 23:10:55 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Mon, 02 Aug 2021 23:10:55 GMT
EXPOSE 4222 8222
# Mon, 02 Aug 2021 23:10:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 02 Aug 2021 23:10:56 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:136482bf81d1fa351b424ebb8c7e34d15f2c5ed3fc0b66b544b8312bda3d52d9`  
		Last Modified: Tue, 15 Jun 2021 23:16:40 GMT  
		Size: 2.4 MB (2427917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bc8de0e43f342d9a142a0dc8c4560fdfa32841c714e46ed1649ae4a279d1e21`  
		Last Modified: Mon, 02 Aug 2021 23:12:44 GMT  
		Size: 6.9 MB (6921533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7a71caf384c90eee69558606851a144c0a87373fbb93628bab4378eb2c2b064`  
		Last Modified: Mon, 02 Aug 2021 23:12:40 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.22-alpine` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:4748f630b68c3b5d641d144f6e5b595a1d7b971b88c3e084566de5b09ab40e52
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.5 MB (9540696 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b70739b129dcb70fd6c70dd84f1e010b28a3aac72190b7104a2c6fc0356620fb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Tue, 15 Jun 2021 21:44:56 GMT
ADD file:6797caacbfe41bfe44000b39ed017016c6fcc492b3d6557cdaba88536df6c876 in / 
# Tue, 15 Jun 2021 21:44:56 GMT
CMD ["/bin/sh"]
# Mon, 02 Aug 2021 22:40:03 GMT
ENV NATS_STREAMING_SERVER=0.22.1
# Mon, 02 Aug 2021 22:40:06 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='581698d248a19ecae64e4048d153bc1021744a3da6284680a339f9f82a53a9cf' ;; 		armhf) natsArch='arm6'; sha256='438a89221bb0608e40d21e73ca27a4b70b8560730726942c0ade94a6b6013d6f' ;; 		armv7) natsArch='arm7'; sha256='4164baadd201d1374f7654d3e54a24d81ceb87a385867e31a82c1d1a69e3b1ae' ;; 		x86_64) natsArch='amd64'; sha256='f29e87ac9ff998c928aa8ebc8cf0c4d04d34a3d95b9900d92fd7dafab2bec8cc' ;; 		x86) natsArch='386'; sha256='0ca68e57babb8901d7afeb7569042730904887e718ddf860ef3ee54278753505' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Mon, 02 Aug 2021 22:40:07 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Mon, 02 Aug 2021 22:40:07 GMT
EXPOSE 4222 8222
# Mon, 02 Aug 2021 22:40:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 02 Aug 2021 22:40:07 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:58ab47519297212468320b23b8100fc1b2b96e8d342040806ae509a778a0a07a`  
		Last Modified: Tue, 15 Jun 2021 21:46:03 GMT  
		Size: 2.7 MB (2709626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a67c736eba594f7a9632ed9a3416f2aa6aba6bcfec575c0ded9b19400460da6`  
		Last Modified: Mon, 02 Aug 2021 22:40:59 GMT  
		Size: 6.8 MB (6830648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:478361e31dd37d3b803c22aac304317c89b32ffd60d662da3cf963124c3eb292`  
		Last Modified: Mon, 02 Aug 2021 22:40:58 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.22-alpine3.14`

```console
$ docker pull nats-streaming@sha256:38d70776fbcfcba9e1cae6b3bffbf6824cba9e88544f08a307917e9812b16fff
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.22-alpine3.14` - linux; amd64

```console
$ docker pull nats-streaming@sha256:5b970a21e7a42e1ddda100078fd4b44e290ddbc7235c99ea5aa3ff0c060d41d7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.3 MB (10267671 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f28bef93a614347e0c25d51fbe54017e3e9f7826c8de64a1381b54e86178d49`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Tue, 15 Jun 2021 22:19:37 GMT
ADD file:f278386b0cef68136129f5f58c52445590a417b624d62bca158d4dc926c340df in / 
# Tue, 15 Jun 2021 22:19:37 GMT
CMD ["/bin/sh"]
# Mon, 02 Aug 2021 22:19:52 GMT
ENV NATS_STREAMING_SERVER=0.22.1
# Mon, 02 Aug 2021 22:19:55 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='581698d248a19ecae64e4048d153bc1021744a3da6284680a339f9f82a53a9cf' ;; 		armhf) natsArch='arm6'; sha256='438a89221bb0608e40d21e73ca27a4b70b8560730726942c0ade94a6b6013d6f' ;; 		armv7) natsArch='arm7'; sha256='4164baadd201d1374f7654d3e54a24d81ceb87a385867e31a82c1d1a69e3b1ae' ;; 		x86_64) natsArch='amd64'; sha256='f29e87ac9ff998c928aa8ebc8cf0c4d04d34a3d95b9900d92fd7dafab2bec8cc' ;; 		x86) natsArch='386'; sha256='0ca68e57babb8901d7afeb7569042730904887e718ddf860ef3ee54278753505' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Mon, 02 Aug 2021 22:19:55 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Mon, 02 Aug 2021 22:19:56 GMT
EXPOSE 4222 8222
# Mon, 02 Aug 2021 22:19:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 02 Aug 2021 22:19:56 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:5843afab387455b37944e709ee8c78d7520df80f8d01cf7f861aae63beeddb6b`  
		Last Modified: Tue, 15 Jun 2021 22:20:04 GMT  
		Size: 2.8 MB (2811478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:306ccc624ab08668c75b4cb54fa3a827395cbd62ead7f920e817c9543c2429fc`  
		Last Modified: Mon, 02 Aug 2021 22:20:27 GMT  
		Size: 7.5 MB (7455771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2df3190f676bc1419fb755d81046ffd2842fc34e02d94f40e080e45c9f96a44d`  
		Last Modified: Mon, 02 Aug 2021 22:20:25 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.22-alpine3.14` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:a6cf6a518fea52b3fc47ed4572652aa0e2350898b54cdbcc0f778150de352dbd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.6 MB (9559904 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c8b625df6f0e93de9095159d166249a43a96ef9f3013e4a2c483b5ac7bc972b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 06 Aug 2021 17:49:32 GMT
ADD file:7f2c7deda009eabdcbbdccb11e854043d32c498e64e7e1ca02165d7bb4261d39 in / 
# Fri, 06 Aug 2021 17:49:32 GMT
CMD ["/bin/sh"]
# Fri, 06 Aug 2021 18:59:05 GMT
ENV NATS_STREAMING_SERVER=0.22.1
# Fri, 06 Aug 2021 18:59:10 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='581698d248a19ecae64e4048d153bc1021744a3da6284680a339f9f82a53a9cf' ;; 		armhf) natsArch='arm6'; sha256='438a89221bb0608e40d21e73ca27a4b70b8560730726942c0ade94a6b6013d6f' ;; 		armv7) natsArch='arm7'; sha256='4164baadd201d1374f7654d3e54a24d81ceb87a385867e31a82c1d1a69e3b1ae' ;; 		x86_64) natsArch='amd64'; sha256='f29e87ac9ff998c928aa8ebc8cf0c4d04d34a3d95b9900d92fd7dafab2bec8cc' ;; 		x86) natsArch='386'; sha256='0ca68e57babb8901d7afeb7569042730904887e718ddf860ef3ee54278753505' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 06 Aug 2021 18:59:10 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Fri, 06 Aug 2021 18:59:11 GMT
EXPOSE 4222 8222
# Fri, 06 Aug 2021 18:59:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 06 Aug 2021 18:59:12 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:f465bb3e9fcd0c42f936ecc566c6e40353c00f3089b2b2c2ea1663c30f89d3ab`  
		Last Modified: Fri, 06 Aug 2021 17:51:00 GMT  
		Size: 2.6 MB (2626350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:719cf2771983cbb32331cc8915e2edce30fbcb308f3504276742ffc9a3bc35fd`  
		Last Modified: Fri, 06 Aug 2021 19:00:56 GMT  
		Size: 6.9 MB (6933133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a72de2e4e74462365f574ec07048641b834163995d6b95fb88af2fca27e01883`  
		Last Modified: Fri, 06 Aug 2021 19:00:52 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.22-alpine3.14` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:572d6d4e53f14a9544d472214ec89300b1dbcc5e001d38c43b3ca6c656938369
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.3 MB (9349872 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5cc85837d0c5d21cf170c6240732f68dacf8b8aefb18875e65bec1f20f22f614`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 30 Jul 2021 18:36:19 GMT
ADD file:416a8b507abdc6bdcb22997a4be0a4170796c3f9f77e315b2dbff2b0a212bc68 in / 
# Fri, 30 Jul 2021 18:36:20 GMT
CMD ["/bin/sh"]
# Mon, 02 Aug 2021 23:10:49 GMT
ENV NATS_STREAMING_SERVER=0.22.1
# Mon, 02 Aug 2021 23:10:54 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='581698d248a19ecae64e4048d153bc1021744a3da6284680a339f9f82a53a9cf' ;; 		armhf) natsArch='arm6'; sha256='438a89221bb0608e40d21e73ca27a4b70b8560730726942c0ade94a6b6013d6f' ;; 		armv7) natsArch='arm7'; sha256='4164baadd201d1374f7654d3e54a24d81ceb87a385867e31a82c1d1a69e3b1ae' ;; 		x86_64) natsArch='amd64'; sha256='f29e87ac9ff998c928aa8ebc8cf0c4d04d34a3d95b9900d92fd7dafab2bec8cc' ;; 		x86) natsArch='386'; sha256='0ca68e57babb8901d7afeb7569042730904887e718ddf860ef3ee54278753505' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Mon, 02 Aug 2021 23:10:55 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Mon, 02 Aug 2021 23:10:55 GMT
EXPOSE 4222 8222
# Mon, 02 Aug 2021 23:10:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 02 Aug 2021 23:10:56 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:136482bf81d1fa351b424ebb8c7e34d15f2c5ed3fc0b66b544b8312bda3d52d9`  
		Last Modified: Tue, 15 Jun 2021 23:16:40 GMT  
		Size: 2.4 MB (2427917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bc8de0e43f342d9a142a0dc8c4560fdfa32841c714e46ed1649ae4a279d1e21`  
		Last Modified: Mon, 02 Aug 2021 23:12:44 GMT  
		Size: 6.9 MB (6921533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7a71caf384c90eee69558606851a144c0a87373fbb93628bab4378eb2c2b064`  
		Last Modified: Mon, 02 Aug 2021 23:12:40 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.22-alpine3.14` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:4748f630b68c3b5d641d144f6e5b595a1d7b971b88c3e084566de5b09ab40e52
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.5 MB (9540696 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b70739b129dcb70fd6c70dd84f1e010b28a3aac72190b7104a2c6fc0356620fb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Tue, 15 Jun 2021 21:44:56 GMT
ADD file:6797caacbfe41bfe44000b39ed017016c6fcc492b3d6557cdaba88536df6c876 in / 
# Tue, 15 Jun 2021 21:44:56 GMT
CMD ["/bin/sh"]
# Mon, 02 Aug 2021 22:40:03 GMT
ENV NATS_STREAMING_SERVER=0.22.1
# Mon, 02 Aug 2021 22:40:06 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='581698d248a19ecae64e4048d153bc1021744a3da6284680a339f9f82a53a9cf' ;; 		armhf) natsArch='arm6'; sha256='438a89221bb0608e40d21e73ca27a4b70b8560730726942c0ade94a6b6013d6f' ;; 		armv7) natsArch='arm7'; sha256='4164baadd201d1374f7654d3e54a24d81ceb87a385867e31a82c1d1a69e3b1ae' ;; 		x86_64) natsArch='amd64'; sha256='f29e87ac9ff998c928aa8ebc8cf0c4d04d34a3d95b9900d92fd7dafab2bec8cc' ;; 		x86) natsArch='386'; sha256='0ca68e57babb8901d7afeb7569042730904887e718ddf860ef3ee54278753505' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Mon, 02 Aug 2021 22:40:07 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Mon, 02 Aug 2021 22:40:07 GMT
EXPOSE 4222 8222
# Mon, 02 Aug 2021 22:40:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 02 Aug 2021 22:40:07 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:58ab47519297212468320b23b8100fc1b2b96e8d342040806ae509a778a0a07a`  
		Last Modified: Tue, 15 Jun 2021 21:46:03 GMT  
		Size: 2.7 MB (2709626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a67c736eba594f7a9632ed9a3416f2aa6aba6bcfec575c0ded9b19400460da6`  
		Last Modified: Mon, 02 Aug 2021 22:40:59 GMT  
		Size: 6.8 MB (6830648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:478361e31dd37d3b803c22aac304317c89b32ffd60d662da3cf963124c3eb292`  
		Last Modified: Mon, 02 Aug 2021 22:40:58 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.22-linux`

```console
$ docker pull nats-streaming@sha256:7d3a953263095ea9d7018d32bd3483577d512550bc7890ba7743f48963cce893
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.22-linux` - linux; amd64

```console
$ docker pull nats-streaming@sha256:3c6c9375f9e9724462e98cfb98a7abb50ceeca73b3070ce061992c4009e32157
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7168713 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:184d7920ac61dd2e84320b8040f57980a7d605d42948a520ede12d421168c4ce`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 02 Aug 2021 22:20:03 GMT
COPY file:ca9a212ccef327f9c2e91a62a908ac0cdbd39b08be331ea2b209c2d724942e18 in /nats-streaming-server 
# Mon, 02 Aug 2021 22:20:03 GMT
EXPOSE 4222 8222
# Mon, 02 Aug 2021 22:20:03 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 02 Aug 2021 22:20:03 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:f3749ab6cbfff03714b5a6a1245fa249b67d19e7358b74cbc50232b14370481a`  
		Last Modified: Mon, 02 Aug 2021 22:20:48 GMT  
		Size: 7.2 MB (7168713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.22-linux` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:e944d0e843d59d5979d7561c06b0c0adc874ceaa0bd34d3a7b536b25e8c9704d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.7 MB (6650246 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0146bbca3802c65d86e148b1d203b3d395ca1cd8a8bb89461888570d821dc4fb`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 02 Aug 2021 22:51:34 GMT
COPY file:68ac67d86d6ac617adc181feb43580415b7fc7640a3c7577bb3753c369908da0 in /nats-streaming-server 
# Mon, 02 Aug 2021 22:51:35 GMT
EXPOSE 4222 8222
# Mon, 02 Aug 2021 22:51:35 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 02 Aug 2021 22:51:35 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:c7e1d707b6179f690f3f44212cb8c9a3fe914d91d3f1ddbac9f176aa0610c90a`  
		Last Modified: Mon, 02 Aug 2021 22:53:32 GMT  
		Size: 6.7 MB (6650246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.22-linux` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:a5e3d56b343f9091f353634f59f688998544ccd4f2cbb80001d08ea6a3207274
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6639768 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80206ae32558812ad047d8ab67519615e98e7df68a884fc32b6d5fd8f72593b0`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 02 Aug 2021 23:11:17 GMT
COPY file:79708b5d249193a95e72c506453fd1ecd3e2738ec2ff3423c4b2bd760f426da2 in /nats-streaming-server 
# Mon, 02 Aug 2021 23:11:18 GMT
EXPOSE 4222 8222
# Mon, 02 Aug 2021 23:11:18 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 02 Aug 2021 23:11:19 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:52753762f751e166edd44e37a0ef0a06b33c337bdeb66e4134ee8479a49dae68`  
		Last Modified: Mon, 02 Aug 2021 23:13:17 GMT  
		Size: 6.6 MB (6639768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.22-linux` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:96652223cce95275138363a54affb8663ba46bc75831c2a9535375ab6d922143
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 MB (6546324 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:952bbd74028df1debbfe0e4665b514c66a36537d0868d41bc971ddb55793c442`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 02 Aug 2021 22:40:16 GMT
COPY file:a77d9769f43cc6943be482183091d3360eaadf93bf1ef5a67f0869d5555868a6 in /nats-streaming-server 
# Mon, 02 Aug 2021 22:40:17 GMT
EXPOSE 4222 8222
# Mon, 02 Aug 2021 22:40:17 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 02 Aug 2021 22:40:17 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4dc8aa7843ed2da454d59006acb180caee3f980d12034caacd4a32ffedab3df7`  
		Last Modified: Mon, 02 Aug 2021 22:41:24 GMT  
		Size: 6.5 MB (6546324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.22-nanoserver`

```console
$ docker pull nats-streaming@sha256:a8998506db11878d76d6c5852804544f9c8129b9a980fe8c32ff898961a4664f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2061; amd64

### `nats-streaming:0.22-nanoserver` - windows version 10.0.17763.2061; amd64

```console
$ docker pull nats-streaming@sha256:349783a72dc891fd56179a54e998371cfe730524625447c5e5f8c8f99ef7d065
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.0 MB (110023666 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b2c8c7df75f26ed571fde792979a0ab215e1f76ff8e9a7f250cc092b15254741`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 06 Jul 2021 20:06:39 GMT
RUN Apply image 1809-amd64
# Wed, 14 Jul 2021 02:35:24 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Mon, 02 Aug 2021 22:17:13 GMT
RUN cmd /S /C #(nop) COPY file:9670e5d1fe5a71e47c78fde01235a0bcbcafcfdeeacf96a7669f6e49343fb03b in C:\nats-streaming-server.exe 
# Mon, 02 Aug 2021 22:17:16 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Mon, 02 Aug 2021 22:17:18 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Mon, 02 Aug 2021 22:17:21 GMT
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
	-	`sha256:395219f11b245d57e94766328eb17b3d461dcfac8402452fdc67df4b9e64361e`  
		Last Modified: Mon, 02 Aug 2021 22:22:03 GMT  
		Size: 7.3 MB (7293366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ed48c75b28949dec2cdb6cb3ff1179ad63c4c4371eba6a69a24baf25f2f6599`  
		Last Modified: Mon, 02 Aug 2021 22:21:54 GMT  
		Size: 1.2 KB (1173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a9b056cd35fd11d0c1057a2de6be2e533de9455af3383d08143215e972c3fd1`  
		Last Modified: Mon, 02 Aug 2021 22:21:55 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20642618c26e07a2aaf5f4169ff1a42ac92cb50404ebb140d800a9da097779ca`  
		Last Modified: Mon, 02 Aug 2021 22:21:55 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.22-nanoserver-1809`

```console
$ docker pull nats-streaming@sha256:a8998506db11878d76d6c5852804544f9c8129b9a980fe8c32ff898961a4664f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2061; amd64

### `nats-streaming:0.22-nanoserver-1809` - windows version 10.0.17763.2061; amd64

```console
$ docker pull nats-streaming@sha256:349783a72dc891fd56179a54e998371cfe730524625447c5e5f8c8f99ef7d065
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.0 MB (110023666 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b2c8c7df75f26ed571fde792979a0ab215e1f76ff8e9a7f250cc092b15254741`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 06 Jul 2021 20:06:39 GMT
RUN Apply image 1809-amd64
# Wed, 14 Jul 2021 02:35:24 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Mon, 02 Aug 2021 22:17:13 GMT
RUN cmd /S /C #(nop) COPY file:9670e5d1fe5a71e47c78fde01235a0bcbcafcfdeeacf96a7669f6e49343fb03b in C:\nats-streaming-server.exe 
# Mon, 02 Aug 2021 22:17:16 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Mon, 02 Aug 2021 22:17:18 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Mon, 02 Aug 2021 22:17:21 GMT
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
	-	`sha256:395219f11b245d57e94766328eb17b3d461dcfac8402452fdc67df4b9e64361e`  
		Last Modified: Mon, 02 Aug 2021 22:22:03 GMT  
		Size: 7.3 MB (7293366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ed48c75b28949dec2cdb6cb3ff1179ad63c4c4371eba6a69a24baf25f2f6599`  
		Last Modified: Mon, 02 Aug 2021 22:21:54 GMT  
		Size: 1.2 KB (1173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a9b056cd35fd11d0c1057a2de6be2e533de9455af3383d08143215e972c3fd1`  
		Last Modified: Mon, 02 Aug 2021 22:21:55 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20642618c26e07a2aaf5f4169ff1a42ac92cb50404ebb140d800a9da097779ca`  
		Last Modified: Mon, 02 Aug 2021 22:21:55 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.22-scratch`

```console
$ docker pull nats-streaming@sha256:7d3a953263095ea9d7018d32bd3483577d512550bc7890ba7743f48963cce893
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.22-scratch` - linux; amd64

```console
$ docker pull nats-streaming@sha256:3c6c9375f9e9724462e98cfb98a7abb50ceeca73b3070ce061992c4009e32157
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7168713 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:184d7920ac61dd2e84320b8040f57980a7d605d42948a520ede12d421168c4ce`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 02 Aug 2021 22:20:03 GMT
COPY file:ca9a212ccef327f9c2e91a62a908ac0cdbd39b08be331ea2b209c2d724942e18 in /nats-streaming-server 
# Mon, 02 Aug 2021 22:20:03 GMT
EXPOSE 4222 8222
# Mon, 02 Aug 2021 22:20:03 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 02 Aug 2021 22:20:03 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:f3749ab6cbfff03714b5a6a1245fa249b67d19e7358b74cbc50232b14370481a`  
		Last Modified: Mon, 02 Aug 2021 22:20:48 GMT  
		Size: 7.2 MB (7168713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.22-scratch` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:e944d0e843d59d5979d7561c06b0c0adc874ceaa0bd34d3a7b536b25e8c9704d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.7 MB (6650246 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0146bbca3802c65d86e148b1d203b3d395ca1cd8a8bb89461888570d821dc4fb`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 02 Aug 2021 22:51:34 GMT
COPY file:68ac67d86d6ac617adc181feb43580415b7fc7640a3c7577bb3753c369908da0 in /nats-streaming-server 
# Mon, 02 Aug 2021 22:51:35 GMT
EXPOSE 4222 8222
# Mon, 02 Aug 2021 22:51:35 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 02 Aug 2021 22:51:35 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:c7e1d707b6179f690f3f44212cb8c9a3fe914d91d3f1ddbac9f176aa0610c90a`  
		Last Modified: Mon, 02 Aug 2021 22:53:32 GMT  
		Size: 6.7 MB (6650246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.22-scratch` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:a5e3d56b343f9091f353634f59f688998544ccd4f2cbb80001d08ea6a3207274
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6639768 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80206ae32558812ad047d8ab67519615e98e7df68a884fc32b6d5fd8f72593b0`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 02 Aug 2021 23:11:17 GMT
COPY file:79708b5d249193a95e72c506453fd1ecd3e2738ec2ff3423c4b2bd760f426da2 in /nats-streaming-server 
# Mon, 02 Aug 2021 23:11:18 GMT
EXPOSE 4222 8222
# Mon, 02 Aug 2021 23:11:18 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 02 Aug 2021 23:11:19 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:52753762f751e166edd44e37a0ef0a06b33c337bdeb66e4134ee8479a49dae68`  
		Last Modified: Mon, 02 Aug 2021 23:13:17 GMT  
		Size: 6.6 MB (6639768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.22-scratch` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:96652223cce95275138363a54affb8663ba46bc75831c2a9535375ab6d922143
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 MB (6546324 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:952bbd74028df1debbfe0e4665b514c66a36537d0868d41bc971ddb55793c442`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 02 Aug 2021 22:40:16 GMT
COPY file:a77d9769f43cc6943be482183091d3360eaadf93bf1ef5a67f0869d5555868a6 in /nats-streaming-server 
# Mon, 02 Aug 2021 22:40:17 GMT
EXPOSE 4222 8222
# Mon, 02 Aug 2021 22:40:17 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 02 Aug 2021 22:40:17 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4dc8aa7843ed2da454d59006acb180caee3f980d12034caacd4a32ffedab3df7`  
		Last Modified: Mon, 02 Aug 2021 22:41:24 GMT  
		Size: 6.5 MB (6546324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.22-windowsservercore`

```console
$ docker pull nats-streaming@sha256:9889123db5aca4139825c5a01e3b51f879184e5afb7dc2eadf6d17144e422df3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.2061; amd64
	-	windows version 10.0.14393.4530; amd64

### `nats-streaming:0.22-windowsservercore` - windows version 10.0.17763.2061; amd64

```console
$ docker pull nats-streaming@sha256:f6b8175c40f3f10b3780b7c109018f478b76eff02f7f836799ccb6dbc547afff
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2693459206 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4430bbff42c38384275e1d9bc9c324202758dbfebec2f6cd6b28d789f82da1d4`
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
# Mon, 02 Aug 2021 22:14:15 GMT
ENV NATS_STREAMING_SERVER=0.22.1
# Mon, 02 Aug 2021 22:14:18 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.22.1/nats-streaming-server-v0.22.1-windows-amd64.zip
# Mon, 02 Aug 2021 22:14:20 GMT
ENV NATS_STREAMING_SERVER_SHASUM=4516852b493111b73ec06477be4a27e66f5abc9ca1ff4dd2b970232271611264
# Mon, 02 Aug 2021 22:15:13 GMT
RUN Set-PSDebug -Trace 2
# Mon, 02 Aug 2021 22:16:58 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Mon, 02 Aug 2021 22:17:01 GMT
EXPOSE 4222 8222
# Mon, 02 Aug 2021 22:17:03 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Mon, 02 Aug 2021 22:17:05 GMT
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
	-	`sha256:b82a3397b3004db7b8c949da737373cf77ed78fdc90030761e97b09e9c9da2bf`  
		Last Modified: Mon, 02 Aug 2021 22:21:36 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f572e3b3f17155a894e961cb378e5de8d16423892838ca8d407dc1b231bdc24`  
		Last Modified: Mon, 02 Aug 2021 22:21:37 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abda54712825ab0cf77038a010dd6c7242f1aeeabb71aaf24969fa2f52b3b290`  
		Last Modified: Mon, 02 Aug 2021 22:21:36 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7399265a146c0fbcbffb8fb2c4d1c03f880ba30c21f33870222c056d3645d4d6`  
		Last Modified: Mon, 02 Aug 2021 22:21:34 GMT  
		Size: 364.1 KB (364103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7a5c5de7479ffd1fbc76c31256335ccbb1634b15e36125a3dfb58104d89a28c`  
		Last Modified: Mon, 02 Aug 2021 22:21:42 GMT  
		Size: 7.6 MB (7636991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f117f06baadaabef0f04b3caf48313f15c143ec663ad83aacf76f5d4d54755f0`  
		Last Modified: Mon, 02 Aug 2021 22:21:33 GMT  
		Size: 1.4 KB (1380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:720a0dee2313cb05fd58b997c2bfedf8b50fc0d16e3f2607f3ebe7c3d1dcdd93`  
		Last Modified: Mon, 02 Aug 2021 22:21:33 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cbfab2e5a68567dff0f8c930bef2751e3ae565099264e67a7806e5b2c8dcad2`  
		Last Modified: Mon, 02 Aug 2021 22:21:33 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.22-windowsservercore` - windows version 10.0.14393.4530; amd64

```console
$ docker pull nats-streaming@sha256:860350027ca4ce7cc64bebf9130ba5945be2b66f699aa4b673230bc8ffea5c59
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6282131227 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e461920fa53ab45b03bab923188b17759cb5848b9e4d659fec9399b15db13a9`
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
# Mon, 02 Aug 2021 22:17:28 GMT
ENV NATS_STREAMING_SERVER=0.22.1
# Mon, 02 Aug 2021 22:17:30 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.22.1/nats-streaming-server-v0.22.1-windows-amd64.zip
# Mon, 02 Aug 2021 22:17:33 GMT
ENV NATS_STREAMING_SERVER_SHASUM=4516852b493111b73ec06477be4a27e66f5abc9ca1ff4dd2b970232271611264
# Mon, 02 Aug 2021 22:18:44 GMT
RUN Set-PSDebug -Trace 2
# Mon, 02 Aug 2021 22:20:44 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Mon, 02 Aug 2021 22:20:46 GMT
EXPOSE 4222 8222
# Mon, 02 Aug 2021 22:20:48 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Mon, 02 Aug 2021 22:20:51 GMT
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
	-	`sha256:01daf4d8d551d6c71e26b9bd4071c9351c0014204d91d856f62076352888ff60`  
		Last Modified: Mon, 02 Aug 2021 22:22:17 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:358b658f14950cb4b2565fbd69fe74eed09949766936621272cff6b3baec317e`  
		Last Modified: Mon, 02 Aug 2021 22:22:18 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3d659d88ad2536c4d7245d222179697bc67d83eb272e7bffa390b50b40c64c0`  
		Last Modified: Mon, 02 Aug 2021 22:22:17 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a581447cad2fda655b58c8e3bbd295b07bcc0205a4eb67c4ffe1b9e0fe479683`  
		Last Modified: Mon, 02 Aug 2021 22:22:15 GMT  
		Size: 364.7 KB (364703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71d3b74ad59b935bb18aa870ecb7df8da9772cefe1d5d3f2f2306d88377bc44a`  
		Last Modified: Mon, 02 Aug 2021 22:22:18 GMT  
		Size: 12.1 MB (12123210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ea62a2c358dd2cab71368c491b629f2cac1c30279e1f3b978bc6caafb67b622`  
		Last Modified: Mon, 02 Aug 2021 22:22:15 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4db9e168d575777fd554d75d34ce2211baa34995899ef0905b50611438ec670d`  
		Last Modified: Mon, 02 Aug 2021 22:22:15 GMT  
		Size: 1.4 KB (1386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:840688f6769f85ae88251d93ec16c131578aabbcaa04a53860c4d6723b77adf1`  
		Last Modified: Mon, 02 Aug 2021 22:22:15 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.22-windowsservercore-1809`

```console
$ docker pull nats-streaming@sha256:433e566e09863176f21000377e836734fb87f52a894eb753ae98476653157b8a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2061; amd64

### `nats-streaming:0.22-windowsservercore-1809` - windows version 10.0.17763.2061; amd64

```console
$ docker pull nats-streaming@sha256:f6b8175c40f3f10b3780b7c109018f478b76eff02f7f836799ccb6dbc547afff
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2693459206 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4430bbff42c38384275e1d9bc9c324202758dbfebec2f6cd6b28d789f82da1d4`
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
# Mon, 02 Aug 2021 22:14:15 GMT
ENV NATS_STREAMING_SERVER=0.22.1
# Mon, 02 Aug 2021 22:14:18 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.22.1/nats-streaming-server-v0.22.1-windows-amd64.zip
# Mon, 02 Aug 2021 22:14:20 GMT
ENV NATS_STREAMING_SERVER_SHASUM=4516852b493111b73ec06477be4a27e66f5abc9ca1ff4dd2b970232271611264
# Mon, 02 Aug 2021 22:15:13 GMT
RUN Set-PSDebug -Trace 2
# Mon, 02 Aug 2021 22:16:58 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Mon, 02 Aug 2021 22:17:01 GMT
EXPOSE 4222 8222
# Mon, 02 Aug 2021 22:17:03 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Mon, 02 Aug 2021 22:17:05 GMT
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
	-	`sha256:b82a3397b3004db7b8c949da737373cf77ed78fdc90030761e97b09e9c9da2bf`  
		Last Modified: Mon, 02 Aug 2021 22:21:36 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f572e3b3f17155a894e961cb378e5de8d16423892838ca8d407dc1b231bdc24`  
		Last Modified: Mon, 02 Aug 2021 22:21:37 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abda54712825ab0cf77038a010dd6c7242f1aeeabb71aaf24969fa2f52b3b290`  
		Last Modified: Mon, 02 Aug 2021 22:21:36 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7399265a146c0fbcbffb8fb2c4d1c03f880ba30c21f33870222c056d3645d4d6`  
		Last Modified: Mon, 02 Aug 2021 22:21:34 GMT  
		Size: 364.1 KB (364103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7a5c5de7479ffd1fbc76c31256335ccbb1634b15e36125a3dfb58104d89a28c`  
		Last Modified: Mon, 02 Aug 2021 22:21:42 GMT  
		Size: 7.6 MB (7636991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f117f06baadaabef0f04b3caf48313f15c143ec663ad83aacf76f5d4d54755f0`  
		Last Modified: Mon, 02 Aug 2021 22:21:33 GMT  
		Size: 1.4 KB (1380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:720a0dee2313cb05fd58b997c2bfedf8b50fc0d16e3f2607f3ebe7c3d1dcdd93`  
		Last Modified: Mon, 02 Aug 2021 22:21:33 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cbfab2e5a68567dff0f8c930bef2751e3ae565099264e67a7806e5b2c8dcad2`  
		Last Modified: Mon, 02 Aug 2021 22:21:33 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.22-windowsservercore-ltsc2016`

```console
$ docker pull nats-streaming@sha256:2b063c7774ef1b3c10036710cbfbbad511dd3951dccfa380271c036b784e83ea
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.14393.4530; amd64

### `nats-streaming:0.22-windowsservercore-ltsc2016` - windows version 10.0.14393.4530; amd64

```console
$ docker pull nats-streaming@sha256:860350027ca4ce7cc64bebf9130ba5945be2b66f699aa4b673230bc8ffea5c59
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6282131227 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e461920fa53ab45b03bab923188b17759cb5848b9e4d659fec9399b15db13a9`
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
# Mon, 02 Aug 2021 22:17:28 GMT
ENV NATS_STREAMING_SERVER=0.22.1
# Mon, 02 Aug 2021 22:17:30 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.22.1/nats-streaming-server-v0.22.1-windows-amd64.zip
# Mon, 02 Aug 2021 22:17:33 GMT
ENV NATS_STREAMING_SERVER_SHASUM=4516852b493111b73ec06477be4a27e66f5abc9ca1ff4dd2b970232271611264
# Mon, 02 Aug 2021 22:18:44 GMT
RUN Set-PSDebug -Trace 2
# Mon, 02 Aug 2021 22:20:44 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Mon, 02 Aug 2021 22:20:46 GMT
EXPOSE 4222 8222
# Mon, 02 Aug 2021 22:20:48 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Mon, 02 Aug 2021 22:20:51 GMT
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
	-	`sha256:01daf4d8d551d6c71e26b9bd4071c9351c0014204d91d856f62076352888ff60`  
		Last Modified: Mon, 02 Aug 2021 22:22:17 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:358b658f14950cb4b2565fbd69fe74eed09949766936621272cff6b3baec317e`  
		Last Modified: Mon, 02 Aug 2021 22:22:18 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3d659d88ad2536c4d7245d222179697bc67d83eb272e7bffa390b50b40c64c0`  
		Last Modified: Mon, 02 Aug 2021 22:22:17 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a581447cad2fda655b58c8e3bbd295b07bcc0205a4eb67c4ffe1b9e0fe479683`  
		Last Modified: Mon, 02 Aug 2021 22:22:15 GMT  
		Size: 364.7 KB (364703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71d3b74ad59b935bb18aa870ecb7df8da9772cefe1d5d3f2f2306d88377bc44a`  
		Last Modified: Mon, 02 Aug 2021 22:22:18 GMT  
		Size: 12.1 MB (12123210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ea62a2c358dd2cab71368c491b629f2cac1c30279e1f3b978bc6caafb67b622`  
		Last Modified: Mon, 02 Aug 2021 22:22:15 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4db9e168d575777fd554d75d34ce2211baa34995899ef0905b50611438ec670d`  
		Last Modified: Mon, 02 Aug 2021 22:22:15 GMT  
		Size: 1.4 KB (1386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:840688f6769f85ae88251d93ec16c131578aabbcaa04a53860c4d6723b77adf1`  
		Last Modified: Mon, 02 Aug 2021 22:22:15 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.22.1`

```console
$ docker pull nats-streaming@sha256:f54d0597f76528b26771a5cacf18f82627877a247c788bcc0aad528f763c0b85
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.2061; amd64

### `nats-streaming:0.22.1` - linux; amd64

```console
$ docker pull nats-streaming@sha256:3c6c9375f9e9724462e98cfb98a7abb50ceeca73b3070ce061992c4009e32157
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7168713 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:184d7920ac61dd2e84320b8040f57980a7d605d42948a520ede12d421168c4ce`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 02 Aug 2021 22:20:03 GMT
COPY file:ca9a212ccef327f9c2e91a62a908ac0cdbd39b08be331ea2b209c2d724942e18 in /nats-streaming-server 
# Mon, 02 Aug 2021 22:20:03 GMT
EXPOSE 4222 8222
# Mon, 02 Aug 2021 22:20:03 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 02 Aug 2021 22:20:03 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:f3749ab6cbfff03714b5a6a1245fa249b67d19e7358b74cbc50232b14370481a`  
		Last Modified: Mon, 02 Aug 2021 22:20:48 GMT  
		Size: 7.2 MB (7168713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.22.1` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:e944d0e843d59d5979d7561c06b0c0adc874ceaa0bd34d3a7b536b25e8c9704d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.7 MB (6650246 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0146bbca3802c65d86e148b1d203b3d395ca1cd8a8bb89461888570d821dc4fb`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 02 Aug 2021 22:51:34 GMT
COPY file:68ac67d86d6ac617adc181feb43580415b7fc7640a3c7577bb3753c369908da0 in /nats-streaming-server 
# Mon, 02 Aug 2021 22:51:35 GMT
EXPOSE 4222 8222
# Mon, 02 Aug 2021 22:51:35 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 02 Aug 2021 22:51:35 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:c7e1d707b6179f690f3f44212cb8c9a3fe914d91d3f1ddbac9f176aa0610c90a`  
		Last Modified: Mon, 02 Aug 2021 22:53:32 GMT  
		Size: 6.7 MB (6650246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.22.1` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:a5e3d56b343f9091f353634f59f688998544ccd4f2cbb80001d08ea6a3207274
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6639768 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80206ae32558812ad047d8ab67519615e98e7df68a884fc32b6d5fd8f72593b0`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 02 Aug 2021 23:11:17 GMT
COPY file:79708b5d249193a95e72c506453fd1ecd3e2738ec2ff3423c4b2bd760f426da2 in /nats-streaming-server 
# Mon, 02 Aug 2021 23:11:18 GMT
EXPOSE 4222 8222
# Mon, 02 Aug 2021 23:11:18 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 02 Aug 2021 23:11:19 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:52753762f751e166edd44e37a0ef0a06b33c337bdeb66e4134ee8479a49dae68`  
		Last Modified: Mon, 02 Aug 2021 23:13:17 GMT  
		Size: 6.6 MB (6639768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.22.1` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:96652223cce95275138363a54affb8663ba46bc75831c2a9535375ab6d922143
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 MB (6546324 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:952bbd74028df1debbfe0e4665b514c66a36537d0868d41bc971ddb55793c442`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 02 Aug 2021 22:40:16 GMT
COPY file:a77d9769f43cc6943be482183091d3360eaadf93bf1ef5a67f0869d5555868a6 in /nats-streaming-server 
# Mon, 02 Aug 2021 22:40:17 GMT
EXPOSE 4222 8222
# Mon, 02 Aug 2021 22:40:17 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 02 Aug 2021 22:40:17 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4dc8aa7843ed2da454d59006acb180caee3f980d12034caacd4a32ffedab3df7`  
		Last Modified: Mon, 02 Aug 2021 22:41:24 GMT  
		Size: 6.5 MB (6546324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.22.1` - windows version 10.0.17763.2061; amd64

```console
$ docker pull nats-streaming@sha256:349783a72dc891fd56179a54e998371cfe730524625447c5e5f8c8f99ef7d065
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.0 MB (110023666 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b2c8c7df75f26ed571fde792979a0ab215e1f76ff8e9a7f250cc092b15254741`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 06 Jul 2021 20:06:39 GMT
RUN Apply image 1809-amd64
# Wed, 14 Jul 2021 02:35:24 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Mon, 02 Aug 2021 22:17:13 GMT
RUN cmd /S /C #(nop) COPY file:9670e5d1fe5a71e47c78fde01235a0bcbcafcfdeeacf96a7669f6e49343fb03b in C:\nats-streaming-server.exe 
# Mon, 02 Aug 2021 22:17:16 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Mon, 02 Aug 2021 22:17:18 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Mon, 02 Aug 2021 22:17:21 GMT
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
	-	`sha256:395219f11b245d57e94766328eb17b3d461dcfac8402452fdc67df4b9e64361e`  
		Last Modified: Mon, 02 Aug 2021 22:22:03 GMT  
		Size: 7.3 MB (7293366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ed48c75b28949dec2cdb6cb3ff1179ad63c4c4371eba6a69a24baf25f2f6599`  
		Last Modified: Mon, 02 Aug 2021 22:21:54 GMT  
		Size: 1.2 KB (1173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a9b056cd35fd11d0c1057a2de6be2e533de9455af3383d08143215e972c3fd1`  
		Last Modified: Mon, 02 Aug 2021 22:21:55 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20642618c26e07a2aaf5f4169ff1a42ac92cb50404ebb140d800a9da097779ca`  
		Last Modified: Mon, 02 Aug 2021 22:21:55 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.22.1-alpine`

```console
$ docker pull nats-streaming@sha256:38d70776fbcfcba9e1cae6b3bffbf6824cba9e88544f08a307917e9812b16fff
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.22.1-alpine` - linux; amd64

```console
$ docker pull nats-streaming@sha256:5b970a21e7a42e1ddda100078fd4b44e290ddbc7235c99ea5aa3ff0c060d41d7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.3 MB (10267671 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f28bef93a614347e0c25d51fbe54017e3e9f7826c8de64a1381b54e86178d49`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Tue, 15 Jun 2021 22:19:37 GMT
ADD file:f278386b0cef68136129f5f58c52445590a417b624d62bca158d4dc926c340df in / 
# Tue, 15 Jun 2021 22:19:37 GMT
CMD ["/bin/sh"]
# Mon, 02 Aug 2021 22:19:52 GMT
ENV NATS_STREAMING_SERVER=0.22.1
# Mon, 02 Aug 2021 22:19:55 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='581698d248a19ecae64e4048d153bc1021744a3da6284680a339f9f82a53a9cf' ;; 		armhf) natsArch='arm6'; sha256='438a89221bb0608e40d21e73ca27a4b70b8560730726942c0ade94a6b6013d6f' ;; 		armv7) natsArch='arm7'; sha256='4164baadd201d1374f7654d3e54a24d81ceb87a385867e31a82c1d1a69e3b1ae' ;; 		x86_64) natsArch='amd64'; sha256='f29e87ac9ff998c928aa8ebc8cf0c4d04d34a3d95b9900d92fd7dafab2bec8cc' ;; 		x86) natsArch='386'; sha256='0ca68e57babb8901d7afeb7569042730904887e718ddf860ef3ee54278753505' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Mon, 02 Aug 2021 22:19:55 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Mon, 02 Aug 2021 22:19:56 GMT
EXPOSE 4222 8222
# Mon, 02 Aug 2021 22:19:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 02 Aug 2021 22:19:56 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:5843afab387455b37944e709ee8c78d7520df80f8d01cf7f861aae63beeddb6b`  
		Last Modified: Tue, 15 Jun 2021 22:20:04 GMT  
		Size: 2.8 MB (2811478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:306ccc624ab08668c75b4cb54fa3a827395cbd62ead7f920e817c9543c2429fc`  
		Last Modified: Mon, 02 Aug 2021 22:20:27 GMT  
		Size: 7.5 MB (7455771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2df3190f676bc1419fb755d81046ffd2842fc34e02d94f40e080e45c9f96a44d`  
		Last Modified: Mon, 02 Aug 2021 22:20:25 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.22.1-alpine` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:a6cf6a518fea52b3fc47ed4572652aa0e2350898b54cdbcc0f778150de352dbd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.6 MB (9559904 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c8b625df6f0e93de9095159d166249a43a96ef9f3013e4a2c483b5ac7bc972b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 06 Aug 2021 17:49:32 GMT
ADD file:7f2c7deda009eabdcbbdccb11e854043d32c498e64e7e1ca02165d7bb4261d39 in / 
# Fri, 06 Aug 2021 17:49:32 GMT
CMD ["/bin/sh"]
# Fri, 06 Aug 2021 18:59:05 GMT
ENV NATS_STREAMING_SERVER=0.22.1
# Fri, 06 Aug 2021 18:59:10 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='581698d248a19ecae64e4048d153bc1021744a3da6284680a339f9f82a53a9cf' ;; 		armhf) natsArch='arm6'; sha256='438a89221bb0608e40d21e73ca27a4b70b8560730726942c0ade94a6b6013d6f' ;; 		armv7) natsArch='arm7'; sha256='4164baadd201d1374f7654d3e54a24d81ceb87a385867e31a82c1d1a69e3b1ae' ;; 		x86_64) natsArch='amd64'; sha256='f29e87ac9ff998c928aa8ebc8cf0c4d04d34a3d95b9900d92fd7dafab2bec8cc' ;; 		x86) natsArch='386'; sha256='0ca68e57babb8901d7afeb7569042730904887e718ddf860ef3ee54278753505' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 06 Aug 2021 18:59:10 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Fri, 06 Aug 2021 18:59:11 GMT
EXPOSE 4222 8222
# Fri, 06 Aug 2021 18:59:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 06 Aug 2021 18:59:12 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:f465bb3e9fcd0c42f936ecc566c6e40353c00f3089b2b2c2ea1663c30f89d3ab`  
		Last Modified: Fri, 06 Aug 2021 17:51:00 GMT  
		Size: 2.6 MB (2626350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:719cf2771983cbb32331cc8915e2edce30fbcb308f3504276742ffc9a3bc35fd`  
		Last Modified: Fri, 06 Aug 2021 19:00:56 GMT  
		Size: 6.9 MB (6933133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a72de2e4e74462365f574ec07048641b834163995d6b95fb88af2fca27e01883`  
		Last Modified: Fri, 06 Aug 2021 19:00:52 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.22.1-alpine` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:572d6d4e53f14a9544d472214ec89300b1dbcc5e001d38c43b3ca6c656938369
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.3 MB (9349872 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5cc85837d0c5d21cf170c6240732f68dacf8b8aefb18875e65bec1f20f22f614`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 30 Jul 2021 18:36:19 GMT
ADD file:416a8b507abdc6bdcb22997a4be0a4170796c3f9f77e315b2dbff2b0a212bc68 in / 
# Fri, 30 Jul 2021 18:36:20 GMT
CMD ["/bin/sh"]
# Mon, 02 Aug 2021 23:10:49 GMT
ENV NATS_STREAMING_SERVER=0.22.1
# Mon, 02 Aug 2021 23:10:54 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='581698d248a19ecae64e4048d153bc1021744a3da6284680a339f9f82a53a9cf' ;; 		armhf) natsArch='arm6'; sha256='438a89221bb0608e40d21e73ca27a4b70b8560730726942c0ade94a6b6013d6f' ;; 		armv7) natsArch='arm7'; sha256='4164baadd201d1374f7654d3e54a24d81ceb87a385867e31a82c1d1a69e3b1ae' ;; 		x86_64) natsArch='amd64'; sha256='f29e87ac9ff998c928aa8ebc8cf0c4d04d34a3d95b9900d92fd7dafab2bec8cc' ;; 		x86) natsArch='386'; sha256='0ca68e57babb8901d7afeb7569042730904887e718ddf860ef3ee54278753505' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Mon, 02 Aug 2021 23:10:55 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Mon, 02 Aug 2021 23:10:55 GMT
EXPOSE 4222 8222
# Mon, 02 Aug 2021 23:10:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 02 Aug 2021 23:10:56 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:136482bf81d1fa351b424ebb8c7e34d15f2c5ed3fc0b66b544b8312bda3d52d9`  
		Last Modified: Tue, 15 Jun 2021 23:16:40 GMT  
		Size: 2.4 MB (2427917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bc8de0e43f342d9a142a0dc8c4560fdfa32841c714e46ed1649ae4a279d1e21`  
		Last Modified: Mon, 02 Aug 2021 23:12:44 GMT  
		Size: 6.9 MB (6921533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7a71caf384c90eee69558606851a144c0a87373fbb93628bab4378eb2c2b064`  
		Last Modified: Mon, 02 Aug 2021 23:12:40 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.22.1-alpine` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:4748f630b68c3b5d641d144f6e5b595a1d7b971b88c3e084566de5b09ab40e52
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.5 MB (9540696 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b70739b129dcb70fd6c70dd84f1e010b28a3aac72190b7104a2c6fc0356620fb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Tue, 15 Jun 2021 21:44:56 GMT
ADD file:6797caacbfe41bfe44000b39ed017016c6fcc492b3d6557cdaba88536df6c876 in / 
# Tue, 15 Jun 2021 21:44:56 GMT
CMD ["/bin/sh"]
# Mon, 02 Aug 2021 22:40:03 GMT
ENV NATS_STREAMING_SERVER=0.22.1
# Mon, 02 Aug 2021 22:40:06 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='581698d248a19ecae64e4048d153bc1021744a3da6284680a339f9f82a53a9cf' ;; 		armhf) natsArch='arm6'; sha256='438a89221bb0608e40d21e73ca27a4b70b8560730726942c0ade94a6b6013d6f' ;; 		armv7) natsArch='arm7'; sha256='4164baadd201d1374f7654d3e54a24d81ceb87a385867e31a82c1d1a69e3b1ae' ;; 		x86_64) natsArch='amd64'; sha256='f29e87ac9ff998c928aa8ebc8cf0c4d04d34a3d95b9900d92fd7dafab2bec8cc' ;; 		x86) natsArch='386'; sha256='0ca68e57babb8901d7afeb7569042730904887e718ddf860ef3ee54278753505' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Mon, 02 Aug 2021 22:40:07 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Mon, 02 Aug 2021 22:40:07 GMT
EXPOSE 4222 8222
# Mon, 02 Aug 2021 22:40:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 02 Aug 2021 22:40:07 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:58ab47519297212468320b23b8100fc1b2b96e8d342040806ae509a778a0a07a`  
		Last Modified: Tue, 15 Jun 2021 21:46:03 GMT  
		Size: 2.7 MB (2709626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a67c736eba594f7a9632ed9a3416f2aa6aba6bcfec575c0ded9b19400460da6`  
		Last Modified: Mon, 02 Aug 2021 22:40:59 GMT  
		Size: 6.8 MB (6830648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:478361e31dd37d3b803c22aac304317c89b32ffd60d662da3cf963124c3eb292`  
		Last Modified: Mon, 02 Aug 2021 22:40:58 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.22.1-alpine3.14`

```console
$ docker pull nats-streaming@sha256:38d70776fbcfcba9e1cae6b3bffbf6824cba9e88544f08a307917e9812b16fff
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.22.1-alpine3.14` - linux; amd64

```console
$ docker pull nats-streaming@sha256:5b970a21e7a42e1ddda100078fd4b44e290ddbc7235c99ea5aa3ff0c060d41d7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.3 MB (10267671 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f28bef93a614347e0c25d51fbe54017e3e9f7826c8de64a1381b54e86178d49`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Tue, 15 Jun 2021 22:19:37 GMT
ADD file:f278386b0cef68136129f5f58c52445590a417b624d62bca158d4dc926c340df in / 
# Tue, 15 Jun 2021 22:19:37 GMT
CMD ["/bin/sh"]
# Mon, 02 Aug 2021 22:19:52 GMT
ENV NATS_STREAMING_SERVER=0.22.1
# Mon, 02 Aug 2021 22:19:55 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='581698d248a19ecae64e4048d153bc1021744a3da6284680a339f9f82a53a9cf' ;; 		armhf) natsArch='arm6'; sha256='438a89221bb0608e40d21e73ca27a4b70b8560730726942c0ade94a6b6013d6f' ;; 		armv7) natsArch='arm7'; sha256='4164baadd201d1374f7654d3e54a24d81ceb87a385867e31a82c1d1a69e3b1ae' ;; 		x86_64) natsArch='amd64'; sha256='f29e87ac9ff998c928aa8ebc8cf0c4d04d34a3d95b9900d92fd7dafab2bec8cc' ;; 		x86) natsArch='386'; sha256='0ca68e57babb8901d7afeb7569042730904887e718ddf860ef3ee54278753505' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Mon, 02 Aug 2021 22:19:55 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Mon, 02 Aug 2021 22:19:56 GMT
EXPOSE 4222 8222
# Mon, 02 Aug 2021 22:19:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 02 Aug 2021 22:19:56 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:5843afab387455b37944e709ee8c78d7520df80f8d01cf7f861aae63beeddb6b`  
		Last Modified: Tue, 15 Jun 2021 22:20:04 GMT  
		Size: 2.8 MB (2811478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:306ccc624ab08668c75b4cb54fa3a827395cbd62ead7f920e817c9543c2429fc`  
		Last Modified: Mon, 02 Aug 2021 22:20:27 GMT  
		Size: 7.5 MB (7455771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2df3190f676bc1419fb755d81046ffd2842fc34e02d94f40e080e45c9f96a44d`  
		Last Modified: Mon, 02 Aug 2021 22:20:25 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.22.1-alpine3.14` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:a6cf6a518fea52b3fc47ed4572652aa0e2350898b54cdbcc0f778150de352dbd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.6 MB (9559904 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c8b625df6f0e93de9095159d166249a43a96ef9f3013e4a2c483b5ac7bc972b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 06 Aug 2021 17:49:32 GMT
ADD file:7f2c7deda009eabdcbbdccb11e854043d32c498e64e7e1ca02165d7bb4261d39 in / 
# Fri, 06 Aug 2021 17:49:32 GMT
CMD ["/bin/sh"]
# Fri, 06 Aug 2021 18:59:05 GMT
ENV NATS_STREAMING_SERVER=0.22.1
# Fri, 06 Aug 2021 18:59:10 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='581698d248a19ecae64e4048d153bc1021744a3da6284680a339f9f82a53a9cf' ;; 		armhf) natsArch='arm6'; sha256='438a89221bb0608e40d21e73ca27a4b70b8560730726942c0ade94a6b6013d6f' ;; 		armv7) natsArch='arm7'; sha256='4164baadd201d1374f7654d3e54a24d81ceb87a385867e31a82c1d1a69e3b1ae' ;; 		x86_64) natsArch='amd64'; sha256='f29e87ac9ff998c928aa8ebc8cf0c4d04d34a3d95b9900d92fd7dafab2bec8cc' ;; 		x86) natsArch='386'; sha256='0ca68e57babb8901d7afeb7569042730904887e718ddf860ef3ee54278753505' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 06 Aug 2021 18:59:10 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Fri, 06 Aug 2021 18:59:11 GMT
EXPOSE 4222 8222
# Fri, 06 Aug 2021 18:59:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 06 Aug 2021 18:59:12 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:f465bb3e9fcd0c42f936ecc566c6e40353c00f3089b2b2c2ea1663c30f89d3ab`  
		Last Modified: Fri, 06 Aug 2021 17:51:00 GMT  
		Size: 2.6 MB (2626350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:719cf2771983cbb32331cc8915e2edce30fbcb308f3504276742ffc9a3bc35fd`  
		Last Modified: Fri, 06 Aug 2021 19:00:56 GMT  
		Size: 6.9 MB (6933133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a72de2e4e74462365f574ec07048641b834163995d6b95fb88af2fca27e01883`  
		Last Modified: Fri, 06 Aug 2021 19:00:52 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.22.1-alpine3.14` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:572d6d4e53f14a9544d472214ec89300b1dbcc5e001d38c43b3ca6c656938369
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.3 MB (9349872 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5cc85837d0c5d21cf170c6240732f68dacf8b8aefb18875e65bec1f20f22f614`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 30 Jul 2021 18:36:19 GMT
ADD file:416a8b507abdc6bdcb22997a4be0a4170796c3f9f77e315b2dbff2b0a212bc68 in / 
# Fri, 30 Jul 2021 18:36:20 GMT
CMD ["/bin/sh"]
# Mon, 02 Aug 2021 23:10:49 GMT
ENV NATS_STREAMING_SERVER=0.22.1
# Mon, 02 Aug 2021 23:10:54 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='581698d248a19ecae64e4048d153bc1021744a3da6284680a339f9f82a53a9cf' ;; 		armhf) natsArch='arm6'; sha256='438a89221bb0608e40d21e73ca27a4b70b8560730726942c0ade94a6b6013d6f' ;; 		armv7) natsArch='arm7'; sha256='4164baadd201d1374f7654d3e54a24d81ceb87a385867e31a82c1d1a69e3b1ae' ;; 		x86_64) natsArch='amd64'; sha256='f29e87ac9ff998c928aa8ebc8cf0c4d04d34a3d95b9900d92fd7dafab2bec8cc' ;; 		x86) natsArch='386'; sha256='0ca68e57babb8901d7afeb7569042730904887e718ddf860ef3ee54278753505' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Mon, 02 Aug 2021 23:10:55 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Mon, 02 Aug 2021 23:10:55 GMT
EXPOSE 4222 8222
# Mon, 02 Aug 2021 23:10:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 02 Aug 2021 23:10:56 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:136482bf81d1fa351b424ebb8c7e34d15f2c5ed3fc0b66b544b8312bda3d52d9`  
		Last Modified: Tue, 15 Jun 2021 23:16:40 GMT  
		Size: 2.4 MB (2427917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bc8de0e43f342d9a142a0dc8c4560fdfa32841c714e46ed1649ae4a279d1e21`  
		Last Modified: Mon, 02 Aug 2021 23:12:44 GMT  
		Size: 6.9 MB (6921533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7a71caf384c90eee69558606851a144c0a87373fbb93628bab4378eb2c2b064`  
		Last Modified: Mon, 02 Aug 2021 23:12:40 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.22.1-alpine3.14` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:4748f630b68c3b5d641d144f6e5b595a1d7b971b88c3e084566de5b09ab40e52
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.5 MB (9540696 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b70739b129dcb70fd6c70dd84f1e010b28a3aac72190b7104a2c6fc0356620fb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Tue, 15 Jun 2021 21:44:56 GMT
ADD file:6797caacbfe41bfe44000b39ed017016c6fcc492b3d6557cdaba88536df6c876 in / 
# Tue, 15 Jun 2021 21:44:56 GMT
CMD ["/bin/sh"]
# Mon, 02 Aug 2021 22:40:03 GMT
ENV NATS_STREAMING_SERVER=0.22.1
# Mon, 02 Aug 2021 22:40:06 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='581698d248a19ecae64e4048d153bc1021744a3da6284680a339f9f82a53a9cf' ;; 		armhf) natsArch='arm6'; sha256='438a89221bb0608e40d21e73ca27a4b70b8560730726942c0ade94a6b6013d6f' ;; 		armv7) natsArch='arm7'; sha256='4164baadd201d1374f7654d3e54a24d81ceb87a385867e31a82c1d1a69e3b1ae' ;; 		x86_64) natsArch='amd64'; sha256='f29e87ac9ff998c928aa8ebc8cf0c4d04d34a3d95b9900d92fd7dafab2bec8cc' ;; 		x86) natsArch='386'; sha256='0ca68e57babb8901d7afeb7569042730904887e718ddf860ef3ee54278753505' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Mon, 02 Aug 2021 22:40:07 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Mon, 02 Aug 2021 22:40:07 GMT
EXPOSE 4222 8222
# Mon, 02 Aug 2021 22:40:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 02 Aug 2021 22:40:07 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:58ab47519297212468320b23b8100fc1b2b96e8d342040806ae509a778a0a07a`  
		Last Modified: Tue, 15 Jun 2021 21:46:03 GMT  
		Size: 2.7 MB (2709626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a67c736eba594f7a9632ed9a3416f2aa6aba6bcfec575c0ded9b19400460da6`  
		Last Modified: Mon, 02 Aug 2021 22:40:59 GMT  
		Size: 6.8 MB (6830648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:478361e31dd37d3b803c22aac304317c89b32ffd60d662da3cf963124c3eb292`  
		Last Modified: Mon, 02 Aug 2021 22:40:58 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.22.1-linux`

```console
$ docker pull nats-streaming@sha256:7d3a953263095ea9d7018d32bd3483577d512550bc7890ba7743f48963cce893
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.22.1-linux` - linux; amd64

```console
$ docker pull nats-streaming@sha256:3c6c9375f9e9724462e98cfb98a7abb50ceeca73b3070ce061992c4009e32157
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7168713 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:184d7920ac61dd2e84320b8040f57980a7d605d42948a520ede12d421168c4ce`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 02 Aug 2021 22:20:03 GMT
COPY file:ca9a212ccef327f9c2e91a62a908ac0cdbd39b08be331ea2b209c2d724942e18 in /nats-streaming-server 
# Mon, 02 Aug 2021 22:20:03 GMT
EXPOSE 4222 8222
# Mon, 02 Aug 2021 22:20:03 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 02 Aug 2021 22:20:03 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:f3749ab6cbfff03714b5a6a1245fa249b67d19e7358b74cbc50232b14370481a`  
		Last Modified: Mon, 02 Aug 2021 22:20:48 GMT  
		Size: 7.2 MB (7168713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.22.1-linux` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:e944d0e843d59d5979d7561c06b0c0adc874ceaa0bd34d3a7b536b25e8c9704d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.7 MB (6650246 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0146bbca3802c65d86e148b1d203b3d395ca1cd8a8bb89461888570d821dc4fb`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 02 Aug 2021 22:51:34 GMT
COPY file:68ac67d86d6ac617adc181feb43580415b7fc7640a3c7577bb3753c369908da0 in /nats-streaming-server 
# Mon, 02 Aug 2021 22:51:35 GMT
EXPOSE 4222 8222
# Mon, 02 Aug 2021 22:51:35 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 02 Aug 2021 22:51:35 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:c7e1d707b6179f690f3f44212cb8c9a3fe914d91d3f1ddbac9f176aa0610c90a`  
		Last Modified: Mon, 02 Aug 2021 22:53:32 GMT  
		Size: 6.7 MB (6650246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.22.1-linux` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:a5e3d56b343f9091f353634f59f688998544ccd4f2cbb80001d08ea6a3207274
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6639768 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80206ae32558812ad047d8ab67519615e98e7df68a884fc32b6d5fd8f72593b0`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 02 Aug 2021 23:11:17 GMT
COPY file:79708b5d249193a95e72c506453fd1ecd3e2738ec2ff3423c4b2bd760f426da2 in /nats-streaming-server 
# Mon, 02 Aug 2021 23:11:18 GMT
EXPOSE 4222 8222
# Mon, 02 Aug 2021 23:11:18 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 02 Aug 2021 23:11:19 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:52753762f751e166edd44e37a0ef0a06b33c337bdeb66e4134ee8479a49dae68`  
		Last Modified: Mon, 02 Aug 2021 23:13:17 GMT  
		Size: 6.6 MB (6639768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.22.1-linux` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:96652223cce95275138363a54affb8663ba46bc75831c2a9535375ab6d922143
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 MB (6546324 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:952bbd74028df1debbfe0e4665b514c66a36537d0868d41bc971ddb55793c442`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 02 Aug 2021 22:40:16 GMT
COPY file:a77d9769f43cc6943be482183091d3360eaadf93bf1ef5a67f0869d5555868a6 in /nats-streaming-server 
# Mon, 02 Aug 2021 22:40:17 GMT
EXPOSE 4222 8222
# Mon, 02 Aug 2021 22:40:17 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 02 Aug 2021 22:40:17 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4dc8aa7843ed2da454d59006acb180caee3f980d12034caacd4a32ffedab3df7`  
		Last Modified: Mon, 02 Aug 2021 22:41:24 GMT  
		Size: 6.5 MB (6546324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.22.1-nanoserver`

```console
$ docker pull nats-streaming@sha256:a8998506db11878d76d6c5852804544f9c8129b9a980fe8c32ff898961a4664f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2061; amd64

### `nats-streaming:0.22.1-nanoserver` - windows version 10.0.17763.2061; amd64

```console
$ docker pull nats-streaming@sha256:349783a72dc891fd56179a54e998371cfe730524625447c5e5f8c8f99ef7d065
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.0 MB (110023666 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b2c8c7df75f26ed571fde792979a0ab215e1f76ff8e9a7f250cc092b15254741`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 06 Jul 2021 20:06:39 GMT
RUN Apply image 1809-amd64
# Wed, 14 Jul 2021 02:35:24 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Mon, 02 Aug 2021 22:17:13 GMT
RUN cmd /S /C #(nop) COPY file:9670e5d1fe5a71e47c78fde01235a0bcbcafcfdeeacf96a7669f6e49343fb03b in C:\nats-streaming-server.exe 
# Mon, 02 Aug 2021 22:17:16 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Mon, 02 Aug 2021 22:17:18 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Mon, 02 Aug 2021 22:17:21 GMT
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
	-	`sha256:395219f11b245d57e94766328eb17b3d461dcfac8402452fdc67df4b9e64361e`  
		Last Modified: Mon, 02 Aug 2021 22:22:03 GMT  
		Size: 7.3 MB (7293366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ed48c75b28949dec2cdb6cb3ff1179ad63c4c4371eba6a69a24baf25f2f6599`  
		Last Modified: Mon, 02 Aug 2021 22:21:54 GMT  
		Size: 1.2 KB (1173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a9b056cd35fd11d0c1057a2de6be2e533de9455af3383d08143215e972c3fd1`  
		Last Modified: Mon, 02 Aug 2021 22:21:55 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20642618c26e07a2aaf5f4169ff1a42ac92cb50404ebb140d800a9da097779ca`  
		Last Modified: Mon, 02 Aug 2021 22:21:55 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.22.1-nanoserver-1809`

```console
$ docker pull nats-streaming@sha256:a8998506db11878d76d6c5852804544f9c8129b9a980fe8c32ff898961a4664f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2061; amd64

### `nats-streaming:0.22.1-nanoserver-1809` - windows version 10.0.17763.2061; amd64

```console
$ docker pull nats-streaming@sha256:349783a72dc891fd56179a54e998371cfe730524625447c5e5f8c8f99ef7d065
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.0 MB (110023666 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b2c8c7df75f26ed571fde792979a0ab215e1f76ff8e9a7f250cc092b15254741`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 06 Jul 2021 20:06:39 GMT
RUN Apply image 1809-amd64
# Wed, 14 Jul 2021 02:35:24 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Mon, 02 Aug 2021 22:17:13 GMT
RUN cmd /S /C #(nop) COPY file:9670e5d1fe5a71e47c78fde01235a0bcbcafcfdeeacf96a7669f6e49343fb03b in C:\nats-streaming-server.exe 
# Mon, 02 Aug 2021 22:17:16 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Mon, 02 Aug 2021 22:17:18 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Mon, 02 Aug 2021 22:17:21 GMT
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
	-	`sha256:395219f11b245d57e94766328eb17b3d461dcfac8402452fdc67df4b9e64361e`  
		Last Modified: Mon, 02 Aug 2021 22:22:03 GMT  
		Size: 7.3 MB (7293366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ed48c75b28949dec2cdb6cb3ff1179ad63c4c4371eba6a69a24baf25f2f6599`  
		Last Modified: Mon, 02 Aug 2021 22:21:54 GMT  
		Size: 1.2 KB (1173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a9b056cd35fd11d0c1057a2de6be2e533de9455af3383d08143215e972c3fd1`  
		Last Modified: Mon, 02 Aug 2021 22:21:55 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20642618c26e07a2aaf5f4169ff1a42ac92cb50404ebb140d800a9da097779ca`  
		Last Modified: Mon, 02 Aug 2021 22:21:55 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.22.1-scratch`

```console
$ docker pull nats-streaming@sha256:7d3a953263095ea9d7018d32bd3483577d512550bc7890ba7743f48963cce893
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.22.1-scratch` - linux; amd64

```console
$ docker pull nats-streaming@sha256:3c6c9375f9e9724462e98cfb98a7abb50ceeca73b3070ce061992c4009e32157
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7168713 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:184d7920ac61dd2e84320b8040f57980a7d605d42948a520ede12d421168c4ce`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 02 Aug 2021 22:20:03 GMT
COPY file:ca9a212ccef327f9c2e91a62a908ac0cdbd39b08be331ea2b209c2d724942e18 in /nats-streaming-server 
# Mon, 02 Aug 2021 22:20:03 GMT
EXPOSE 4222 8222
# Mon, 02 Aug 2021 22:20:03 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 02 Aug 2021 22:20:03 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:f3749ab6cbfff03714b5a6a1245fa249b67d19e7358b74cbc50232b14370481a`  
		Last Modified: Mon, 02 Aug 2021 22:20:48 GMT  
		Size: 7.2 MB (7168713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.22.1-scratch` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:e944d0e843d59d5979d7561c06b0c0adc874ceaa0bd34d3a7b536b25e8c9704d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.7 MB (6650246 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0146bbca3802c65d86e148b1d203b3d395ca1cd8a8bb89461888570d821dc4fb`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 02 Aug 2021 22:51:34 GMT
COPY file:68ac67d86d6ac617adc181feb43580415b7fc7640a3c7577bb3753c369908da0 in /nats-streaming-server 
# Mon, 02 Aug 2021 22:51:35 GMT
EXPOSE 4222 8222
# Mon, 02 Aug 2021 22:51:35 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 02 Aug 2021 22:51:35 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:c7e1d707b6179f690f3f44212cb8c9a3fe914d91d3f1ddbac9f176aa0610c90a`  
		Last Modified: Mon, 02 Aug 2021 22:53:32 GMT  
		Size: 6.7 MB (6650246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.22.1-scratch` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:a5e3d56b343f9091f353634f59f688998544ccd4f2cbb80001d08ea6a3207274
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6639768 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80206ae32558812ad047d8ab67519615e98e7df68a884fc32b6d5fd8f72593b0`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 02 Aug 2021 23:11:17 GMT
COPY file:79708b5d249193a95e72c506453fd1ecd3e2738ec2ff3423c4b2bd760f426da2 in /nats-streaming-server 
# Mon, 02 Aug 2021 23:11:18 GMT
EXPOSE 4222 8222
# Mon, 02 Aug 2021 23:11:18 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 02 Aug 2021 23:11:19 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:52753762f751e166edd44e37a0ef0a06b33c337bdeb66e4134ee8479a49dae68`  
		Last Modified: Mon, 02 Aug 2021 23:13:17 GMT  
		Size: 6.6 MB (6639768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.22.1-scratch` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:96652223cce95275138363a54affb8663ba46bc75831c2a9535375ab6d922143
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 MB (6546324 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:952bbd74028df1debbfe0e4665b514c66a36537d0868d41bc971ddb55793c442`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 02 Aug 2021 22:40:16 GMT
COPY file:a77d9769f43cc6943be482183091d3360eaadf93bf1ef5a67f0869d5555868a6 in /nats-streaming-server 
# Mon, 02 Aug 2021 22:40:17 GMT
EXPOSE 4222 8222
# Mon, 02 Aug 2021 22:40:17 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 02 Aug 2021 22:40:17 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4dc8aa7843ed2da454d59006acb180caee3f980d12034caacd4a32ffedab3df7`  
		Last Modified: Mon, 02 Aug 2021 22:41:24 GMT  
		Size: 6.5 MB (6546324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.22.1-windowsservercore`

```console
$ docker pull nats-streaming@sha256:9889123db5aca4139825c5a01e3b51f879184e5afb7dc2eadf6d17144e422df3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.2061; amd64
	-	windows version 10.0.14393.4530; amd64

### `nats-streaming:0.22.1-windowsservercore` - windows version 10.0.17763.2061; amd64

```console
$ docker pull nats-streaming@sha256:f6b8175c40f3f10b3780b7c109018f478b76eff02f7f836799ccb6dbc547afff
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2693459206 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4430bbff42c38384275e1d9bc9c324202758dbfebec2f6cd6b28d789f82da1d4`
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
# Mon, 02 Aug 2021 22:14:15 GMT
ENV NATS_STREAMING_SERVER=0.22.1
# Mon, 02 Aug 2021 22:14:18 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.22.1/nats-streaming-server-v0.22.1-windows-amd64.zip
# Mon, 02 Aug 2021 22:14:20 GMT
ENV NATS_STREAMING_SERVER_SHASUM=4516852b493111b73ec06477be4a27e66f5abc9ca1ff4dd2b970232271611264
# Mon, 02 Aug 2021 22:15:13 GMT
RUN Set-PSDebug -Trace 2
# Mon, 02 Aug 2021 22:16:58 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Mon, 02 Aug 2021 22:17:01 GMT
EXPOSE 4222 8222
# Mon, 02 Aug 2021 22:17:03 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Mon, 02 Aug 2021 22:17:05 GMT
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
	-	`sha256:b82a3397b3004db7b8c949da737373cf77ed78fdc90030761e97b09e9c9da2bf`  
		Last Modified: Mon, 02 Aug 2021 22:21:36 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f572e3b3f17155a894e961cb378e5de8d16423892838ca8d407dc1b231bdc24`  
		Last Modified: Mon, 02 Aug 2021 22:21:37 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abda54712825ab0cf77038a010dd6c7242f1aeeabb71aaf24969fa2f52b3b290`  
		Last Modified: Mon, 02 Aug 2021 22:21:36 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7399265a146c0fbcbffb8fb2c4d1c03f880ba30c21f33870222c056d3645d4d6`  
		Last Modified: Mon, 02 Aug 2021 22:21:34 GMT  
		Size: 364.1 KB (364103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7a5c5de7479ffd1fbc76c31256335ccbb1634b15e36125a3dfb58104d89a28c`  
		Last Modified: Mon, 02 Aug 2021 22:21:42 GMT  
		Size: 7.6 MB (7636991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f117f06baadaabef0f04b3caf48313f15c143ec663ad83aacf76f5d4d54755f0`  
		Last Modified: Mon, 02 Aug 2021 22:21:33 GMT  
		Size: 1.4 KB (1380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:720a0dee2313cb05fd58b997c2bfedf8b50fc0d16e3f2607f3ebe7c3d1dcdd93`  
		Last Modified: Mon, 02 Aug 2021 22:21:33 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cbfab2e5a68567dff0f8c930bef2751e3ae565099264e67a7806e5b2c8dcad2`  
		Last Modified: Mon, 02 Aug 2021 22:21:33 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.22.1-windowsservercore` - windows version 10.0.14393.4530; amd64

```console
$ docker pull nats-streaming@sha256:860350027ca4ce7cc64bebf9130ba5945be2b66f699aa4b673230bc8ffea5c59
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6282131227 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e461920fa53ab45b03bab923188b17759cb5848b9e4d659fec9399b15db13a9`
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
# Mon, 02 Aug 2021 22:17:28 GMT
ENV NATS_STREAMING_SERVER=0.22.1
# Mon, 02 Aug 2021 22:17:30 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.22.1/nats-streaming-server-v0.22.1-windows-amd64.zip
# Mon, 02 Aug 2021 22:17:33 GMT
ENV NATS_STREAMING_SERVER_SHASUM=4516852b493111b73ec06477be4a27e66f5abc9ca1ff4dd2b970232271611264
# Mon, 02 Aug 2021 22:18:44 GMT
RUN Set-PSDebug -Trace 2
# Mon, 02 Aug 2021 22:20:44 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Mon, 02 Aug 2021 22:20:46 GMT
EXPOSE 4222 8222
# Mon, 02 Aug 2021 22:20:48 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Mon, 02 Aug 2021 22:20:51 GMT
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
	-	`sha256:01daf4d8d551d6c71e26b9bd4071c9351c0014204d91d856f62076352888ff60`  
		Last Modified: Mon, 02 Aug 2021 22:22:17 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:358b658f14950cb4b2565fbd69fe74eed09949766936621272cff6b3baec317e`  
		Last Modified: Mon, 02 Aug 2021 22:22:18 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3d659d88ad2536c4d7245d222179697bc67d83eb272e7bffa390b50b40c64c0`  
		Last Modified: Mon, 02 Aug 2021 22:22:17 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a581447cad2fda655b58c8e3bbd295b07bcc0205a4eb67c4ffe1b9e0fe479683`  
		Last Modified: Mon, 02 Aug 2021 22:22:15 GMT  
		Size: 364.7 KB (364703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71d3b74ad59b935bb18aa870ecb7df8da9772cefe1d5d3f2f2306d88377bc44a`  
		Last Modified: Mon, 02 Aug 2021 22:22:18 GMT  
		Size: 12.1 MB (12123210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ea62a2c358dd2cab71368c491b629f2cac1c30279e1f3b978bc6caafb67b622`  
		Last Modified: Mon, 02 Aug 2021 22:22:15 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4db9e168d575777fd554d75d34ce2211baa34995899ef0905b50611438ec670d`  
		Last Modified: Mon, 02 Aug 2021 22:22:15 GMT  
		Size: 1.4 KB (1386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:840688f6769f85ae88251d93ec16c131578aabbcaa04a53860c4d6723b77adf1`  
		Last Modified: Mon, 02 Aug 2021 22:22:15 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.22.1-windowsservercore-1809`

```console
$ docker pull nats-streaming@sha256:433e566e09863176f21000377e836734fb87f52a894eb753ae98476653157b8a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2061; amd64

### `nats-streaming:0.22.1-windowsservercore-1809` - windows version 10.0.17763.2061; amd64

```console
$ docker pull nats-streaming@sha256:f6b8175c40f3f10b3780b7c109018f478b76eff02f7f836799ccb6dbc547afff
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2693459206 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4430bbff42c38384275e1d9bc9c324202758dbfebec2f6cd6b28d789f82da1d4`
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
# Mon, 02 Aug 2021 22:14:15 GMT
ENV NATS_STREAMING_SERVER=0.22.1
# Mon, 02 Aug 2021 22:14:18 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.22.1/nats-streaming-server-v0.22.1-windows-amd64.zip
# Mon, 02 Aug 2021 22:14:20 GMT
ENV NATS_STREAMING_SERVER_SHASUM=4516852b493111b73ec06477be4a27e66f5abc9ca1ff4dd2b970232271611264
# Mon, 02 Aug 2021 22:15:13 GMT
RUN Set-PSDebug -Trace 2
# Mon, 02 Aug 2021 22:16:58 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Mon, 02 Aug 2021 22:17:01 GMT
EXPOSE 4222 8222
# Mon, 02 Aug 2021 22:17:03 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Mon, 02 Aug 2021 22:17:05 GMT
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
	-	`sha256:b82a3397b3004db7b8c949da737373cf77ed78fdc90030761e97b09e9c9da2bf`  
		Last Modified: Mon, 02 Aug 2021 22:21:36 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f572e3b3f17155a894e961cb378e5de8d16423892838ca8d407dc1b231bdc24`  
		Last Modified: Mon, 02 Aug 2021 22:21:37 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abda54712825ab0cf77038a010dd6c7242f1aeeabb71aaf24969fa2f52b3b290`  
		Last Modified: Mon, 02 Aug 2021 22:21:36 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7399265a146c0fbcbffb8fb2c4d1c03f880ba30c21f33870222c056d3645d4d6`  
		Last Modified: Mon, 02 Aug 2021 22:21:34 GMT  
		Size: 364.1 KB (364103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7a5c5de7479ffd1fbc76c31256335ccbb1634b15e36125a3dfb58104d89a28c`  
		Last Modified: Mon, 02 Aug 2021 22:21:42 GMT  
		Size: 7.6 MB (7636991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f117f06baadaabef0f04b3caf48313f15c143ec663ad83aacf76f5d4d54755f0`  
		Last Modified: Mon, 02 Aug 2021 22:21:33 GMT  
		Size: 1.4 KB (1380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:720a0dee2313cb05fd58b997c2bfedf8b50fc0d16e3f2607f3ebe7c3d1dcdd93`  
		Last Modified: Mon, 02 Aug 2021 22:21:33 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cbfab2e5a68567dff0f8c930bef2751e3ae565099264e67a7806e5b2c8dcad2`  
		Last Modified: Mon, 02 Aug 2021 22:21:33 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.22.1-windowsservercore-ltsc2016`

```console
$ docker pull nats-streaming@sha256:2b063c7774ef1b3c10036710cbfbbad511dd3951dccfa380271c036b784e83ea
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.14393.4530; amd64

### `nats-streaming:0.22.1-windowsservercore-ltsc2016` - windows version 10.0.14393.4530; amd64

```console
$ docker pull nats-streaming@sha256:860350027ca4ce7cc64bebf9130ba5945be2b66f699aa4b673230bc8ffea5c59
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6282131227 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e461920fa53ab45b03bab923188b17759cb5848b9e4d659fec9399b15db13a9`
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
# Mon, 02 Aug 2021 22:17:28 GMT
ENV NATS_STREAMING_SERVER=0.22.1
# Mon, 02 Aug 2021 22:17:30 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.22.1/nats-streaming-server-v0.22.1-windows-amd64.zip
# Mon, 02 Aug 2021 22:17:33 GMT
ENV NATS_STREAMING_SERVER_SHASUM=4516852b493111b73ec06477be4a27e66f5abc9ca1ff4dd2b970232271611264
# Mon, 02 Aug 2021 22:18:44 GMT
RUN Set-PSDebug -Trace 2
# Mon, 02 Aug 2021 22:20:44 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Mon, 02 Aug 2021 22:20:46 GMT
EXPOSE 4222 8222
# Mon, 02 Aug 2021 22:20:48 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Mon, 02 Aug 2021 22:20:51 GMT
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
	-	`sha256:01daf4d8d551d6c71e26b9bd4071c9351c0014204d91d856f62076352888ff60`  
		Last Modified: Mon, 02 Aug 2021 22:22:17 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:358b658f14950cb4b2565fbd69fe74eed09949766936621272cff6b3baec317e`  
		Last Modified: Mon, 02 Aug 2021 22:22:18 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3d659d88ad2536c4d7245d222179697bc67d83eb272e7bffa390b50b40c64c0`  
		Last Modified: Mon, 02 Aug 2021 22:22:17 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a581447cad2fda655b58c8e3bbd295b07bcc0205a4eb67c4ffe1b9e0fe479683`  
		Last Modified: Mon, 02 Aug 2021 22:22:15 GMT  
		Size: 364.7 KB (364703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71d3b74ad59b935bb18aa870ecb7df8da9772cefe1d5d3f2f2306d88377bc44a`  
		Last Modified: Mon, 02 Aug 2021 22:22:18 GMT  
		Size: 12.1 MB (12123210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ea62a2c358dd2cab71368c491b629f2cac1c30279e1f3b978bc6caafb67b622`  
		Last Modified: Mon, 02 Aug 2021 22:22:15 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4db9e168d575777fd554d75d34ce2211baa34995899ef0905b50611438ec670d`  
		Last Modified: Mon, 02 Aug 2021 22:22:15 GMT  
		Size: 1.4 KB (1386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:840688f6769f85ae88251d93ec16c131578aabbcaa04a53860c4d6723b77adf1`  
		Last Modified: Mon, 02 Aug 2021 22:22:15 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:alpine`

```console
$ docker pull nats-streaming@sha256:38d70776fbcfcba9e1cae6b3bffbf6824cba9e88544f08a307917e9812b16fff
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:alpine` - linux; amd64

```console
$ docker pull nats-streaming@sha256:5b970a21e7a42e1ddda100078fd4b44e290ddbc7235c99ea5aa3ff0c060d41d7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.3 MB (10267671 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f28bef93a614347e0c25d51fbe54017e3e9f7826c8de64a1381b54e86178d49`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Tue, 15 Jun 2021 22:19:37 GMT
ADD file:f278386b0cef68136129f5f58c52445590a417b624d62bca158d4dc926c340df in / 
# Tue, 15 Jun 2021 22:19:37 GMT
CMD ["/bin/sh"]
# Mon, 02 Aug 2021 22:19:52 GMT
ENV NATS_STREAMING_SERVER=0.22.1
# Mon, 02 Aug 2021 22:19:55 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='581698d248a19ecae64e4048d153bc1021744a3da6284680a339f9f82a53a9cf' ;; 		armhf) natsArch='arm6'; sha256='438a89221bb0608e40d21e73ca27a4b70b8560730726942c0ade94a6b6013d6f' ;; 		armv7) natsArch='arm7'; sha256='4164baadd201d1374f7654d3e54a24d81ceb87a385867e31a82c1d1a69e3b1ae' ;; 		x86_64) natsArch='amd64'; sha256='f29e87ac9ff998c928aa8ebc8cf0c4d04d34a3d95b9900d92fd7dafab2bec8cc' ;; 		x86) natsArch='386'; sha256='0ca68e57babb8901d7afeb7569042730904887e718ddf860ef3ee54278753505' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Mon, 02 Aug 2021 22:19:55 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Mon, 02 Aug 2021 22:19:56 GMT
EXPOSE 4222 8222
# Mon, 02 Aug 2021 22:19:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 02 Aug 2021 22:19:56 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:5843afab387455b37944e709ee8c78d7520df80f8d01cf7f861aae63beeddb6b`  
		Last Modified: Tue, 15 Jun 2021 22:20:04 GMT  
		Size: 2.8 MB (2811478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:306ccc624ab08668c75b4cb54fa3a827395cbd62ead7f920e817c9543c2429fc`  
		Last Modified: Mon, 02 Aug 2021 22:20:27 GMT  
		Size: 7.5 MB (7455771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2df3190f676bc1419fb755d81046ffd2842fc34e02d94f40e080e45c9f96a44d`  
		Last Modified: Mon, 02 Aug 2021 22:20:25 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:a6cf6a518fea52b3fc47ed4572652aa0e2350898b54cdbcc0f778150de352dbd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.6 MB (9559904 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c8b625df6f0e93de9095159d166249a43a96ef9f3013e4a2c483b5ac7bc972b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 06 Aug 2021 17:49:32 GMT
ADD file:7f2c7deda009eabdcbbdccb11e854043d32c498e64e7e1ca02165d7bb4261d39 in / 
# Fri, 06 Aug 2021 17:49:32 GMT
CMD ["/bin/sh"]
# Fri, 06 Aug 2021 18:59:05 GMT
ENV NATS_STREAMING_SERVER=0.22.1
# Fri, 06 Aug 2021 18:59:10 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='581698d248a19ecae64e4048d153bc1021744a3da6284680a339f9f82a53a9cf' ;; 		armhf) natsArch='arm6'; sha256='438a89221bb0608e40d21e73ca27a4b70b8560730726942c0ade94a6b6013d6f' ;; 		armv7) natsArch='arm7'; sha256='4164baadd201d1374f7654d3e54a24d81ceb87a385867e31a82c1d1a69e3b1ae' ;; 		x86_64) natsArch='amd64'; sha256='f29e87ac9ff998c928aa8ebc8cf0c4d04d34a3d95b9900d92fd7dafab2bec8cc' ;; 		x86) natsArch='386'; sha256='0ca68e57babb8901d7afeb7569042730904887e718ddf860ef3ee54278753505' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 06 Aug 2021 18:59:10 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Fri, 06 Aug 2021 18:59:11 GMT
EXPOSE 4222 8222
# Fri, 06 Aug 2021 18:59:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 06 Aug 2021 18:59:12 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:f465bb3e9fcd0c42f936ecc566c6e40353c00f3089b2b2c2ea1663c30f89d3ab`  
		Last Modified: Fri, 06 Aug 2021 17:51:00 GMT  
		Size: 2.6 MB (2626350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:719cf2771983cbb32331cc8915e2edce30fbcb308f3504276742ffc9a3bc35fd`  
		Last Modified: Fri, 06 Aug 2021 19:00:56 GMT  
		Size: 6.9 MB (6933133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a72de2e4e74462365f574ec07048641b834163995d6b95fb88af2fca27e01883`  
		Last Modified: Fri, 06 Aug 2021 19:00:52 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:572d6d4e53f14a9544d472214ec89300b1dbcc5e001d38c43b3ca6c656938369
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.3 MB (9349872 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5cc85837d0c5d21cf170c6240732f68dacf8b8aefb18875e65bec1f20f22f614`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 30 Jul 2021 18:36:19 GMT
ADD file:416a8b507abdc6bdcb22997a4be0a4170796c3f9f77e315b2dbff2b0a212bc68 in / 
# Fri, 30 Jul 2021 18:36:20 GMT
CMD ["/bin/sh"]
# Mon, 02 Aug 2021 23:10:49 GMT
ENV NATS_STREAMING_SERVER=0.22.1
# Mon, 02 Aug 2021 23:10:54 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='581698d248a19ecae64e4048d153bc1021744a3da6284680a339f9f82a53a9cf' ;; 		armhf) natsArch='arm6'; sha256='438a89221bb0608e40d21e73ca27a4b70b8560730726942c0ade94a6b6013d6f' ;; 		armv7) natsArch='arm7'; sha256='4164baadd201d1374f7654d3e54a24d81ceb87a385867e31a82c1d1a69e3b1ae' ;; 		x86_64) natsArch='amd64'; sha256='f29e87ac9ff998c928aa8ebc8cf0c4d04d34a3d95b9900d92fd7dafab2bec8cc' ;; 		x86) natsArch='386'; sha256='0ca68e57babb8901d7afeb7569042730904887e718ddf860ef3ee54278753505' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Mon, 02 Aug 2021 23:10:55 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Mon, 02 Aug 2021 23:10:55 GMT
EXPOSE 4222 8222
# Mon, 02 Aug 2021 23:10:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 02 Aug 2021 23:10:56 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:136482bf81d1fa351b424ebb8c7e34d15f2c5ed3fc0b66b544b8312bda3d52d9`  
		Last Modified: Tue, 15 Jun 2021 23:16:40 GMT  
		Size: 2.4 MB (2427917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bc8de0e43f342d9a142a0dc8c4560fdfa32841c714e46ed1649ae4a279d1e21`  
		Last Modified: Mon, 02 Aug 2021 23:12:44 GMT  
		Size: 6.9 MB (6921533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7a71caf384c90eee69558606851a144c0a87373fbb93628bab4378eb2c2b064`  
		Last Modified: Mon, 02 Aug 2021 23:12:40 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:4748f630b68c3b5d641d144f6e5b595a1d7b971b88c3e084566de5b09ab40e52
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.5 MB (9540696 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b70739b129dcb70fd6c70dd84f1e010b28a3aac72190b7104a2c6fc0356620fb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Tue, 15 Jun 2021 21:44:56 GMT
ADD file:6797caacbfe41bfe44000b39ed017016c6fcc492b3d6557cdaba88536df6c876 in / 
# Tue, 15 Jun 2021 21:44:56 GMT
CMD ["/bin/sh"]
# Mon, 02 Aug 2021 22:40:03 GMT
ENV NATS_STREAMING_SERVER=0.22.1
# Mon, 02 Aug 2021 22:40:06 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='581698d248a19ecae64e4048d153bc1021744a3da6284680a339f9f82a53a9cf' ;; 		armhf) natsArch='arm6'; sha256='438a89221bb0608e40d21e73ca27a4b70b8560730726942c0ade94a6b6013d6f' ;; 		armv7) natsArch='arm7'; sha256='4164baadd201d1374f7654d3e54a24d81ceb87a385867e31a82c1d1a69e3b1ae' ;; 		x86_64) natsArch='amd64'; sha256='f29e87ac9ff998c928aa8ebc8cf0c4d04d34a3d95b9900d92fd7dafab2bec8cc' ;; 		x86) natsArch='386'; sha256='0ca68e57babb8901d7afeb7569042730904887e718ddf860ef3ee54278753505' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Mon, 02 Aug 2021 22:40:07 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Mon, 02 Aug 2021 22:40:07 GMT
EXPOSE 4222 8222
# Mon, 02 Aug 2021 22:40:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 02 Aug 2021 22:40:07 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:58ab47519297212468320b23b8100fc1b2b96e8d342040806ae509a778a0a07a`  
		Last Modified: Tue, 15 Jun 2021 21:46:03 GMT  
		Size: 2.7 MB (2709626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a67c736eba594f7a9632ed9a3416f2aa6aba6bcfec575c0ded9b19400460da6`  
		Last Modified: Mon, 02 Aug 2021 22:40:59 GMT  
		Size: 6.8 MB (6830648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:478361e31dd37d3b803c22aac304317c89b32ffd60d662da3cf963124c3eb292`  
		Last Modified: Mon, 02 Aug 2021 22:40:58 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:alpine3.14`

```console
$ docker pull nats-streaming@sha256:38d70776fbcfcba9e1cae6b3bffbf6824cba9e88544f08a307917e9812b16fff
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:alpine3.14` - linux; amd64

```console
$ docker pull nats-streaming@sha256:5b970a21e7a42e1ddda100078fd4b44e290ddbc7235c99ea5aa3ff0c060d41d7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.3 MB (10267671 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f28bef93a614347e0c25d51fbe54017e3e9f7826c8de64a1381b54e86178d49`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Tue, 15 Jun 2021 22:19:37 GMT
ADD file:f278386b0cef68136129f5f58c52445590a417b624d62bca158d4dc926c340df in / 
# Tue, 15 Jun 2021 22:19:37 GMT
CMD ["/bin/sh"]
# Mon, 02 Aug 2021 22:19:52 GMT
ENV NATS_STREAMING_SERVER=0.22.1
# Mon, 02 Aug 2021 22:19:55 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='581698d248a19ecae64e4048d153bc1021744a3da6284680a339f9f82a53a9cf' ;; 		armhf) natsArch='arm6'; sha256='438a89221bb0608e40d21e73ca27a4b70b8560730726942c0ade94a6b6013d6f' ;; 		armv7) natsArch='arm7'; sha256='4164baadd201d1374f7654d3e54a24d81ceb87a385867e31a82c1d1a69e3b1ae' ;; 		x86_64) natsArch='amd64'; sha256='f29e87ac9ff998c928aa8ebc8cf0c4d04d34a3d95b9900d92fd7dafab2bec8cc' ;; 		x86) natsArch='386'; sha256='0ca68e57babb8901d7afeb7569042730904887e718ddf860ef3ee54278753505' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Mon, 02 Aug 2021 22:19:55 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Mon, 02 Aug 2021 22:19:56 GMT
EXPOSE 4222 8222
# Mon, 02 Aug 2021 22:19:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 02 Aug 2021 22:19:56 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:5843afab387455b37944e709ee8c78d7520df80f8d01cf7f861aae63beeddb6b`  
		Last Modified: Tue, 15 Jun 2021 22:20:04 GMT  
		Size: 2.8 MB (2811478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:306ccc624ab08668c75b4cb54fa3a827395cbd62ead7f920e817c9543c2429fc`  
		Last Modified: Mon, 02 Aug 2021 22:20:27 GMT  
		Size: 7.5 MB (7455771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2df3190f676bc1419fb755d81046ffd2842fc34e02d94f40e080e45c9f96a44d`  
		Last Modified: Mon, 02 Aug 2021 22:20:25 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine3.14` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:a6cf6a518fea52b3fc47ed4572652aa0e2350898b54cdbcc0f778150de352dbd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.6 MB (9559904 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c8b625df6f0e93de9095159d166249a43a96ef9f3013e4a2c483b5ac7bc972b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 06 Aug 2021 17:49:32 GMT
ADD file:7f2c7deda009eabdcbbdccb11e854043d32c498e64e7e1ca02165d7bb4261d39 in / 
# Fri, 06 Aug 2021 17:49:32 GMT
CMD ["/bin/sh"]
# Fri, 06 Aug 2021 18:59:05 GMT
ENV NATS_STREAMING_SERVER=0.22.1
# Fri, 06 Aug 2021 18:59:10 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='581698d248a19ecae64e4048d153bc1021744a3da6284680a339f9f82a53a9cf' ;; 		armhf) natsArch='arm6'; sha256='438a89221bb0608e40d21e73ca27a4b70b8560730726942c0ade94a6b6013d6f' ;; 		armv7) natsArch='arm7'; sha256='4164baadd201d1374f7654d3e54a24d81ceb87a385867e31a82c1d1a69e3b1ae' ;; 		x86_64) natsArch='amd64'; sha256='f29e87ac9ff998c928aa8ebc8cf0c4d04d34a3d95b9900d92fd7dafab2bec8cc' ;; 		x86) natsArch='386'; sha256='0ca68e57babb8901d7afeb7569042730904887e718ddf860ef3ee54278753505' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 06 Aug 2021 18:59:10 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Fri, 06 Aug 2021 18:59:11 GMT
EXPOSE 4222 8222
# Fri, 06 Aug 2021 18:59:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 06 Aug 2021 18:59:12 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:f465bb3e9fcd0c42f936ecc566c6e40353c00f3089b2b2c2ea1663c30f89d3ab`  
		Last Modified: Fri, 06 Aug 2021 17:51:00 GMT  
		Size: 2.6 MB (2626350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:719cf2771983cbb32331cc8915e2edce30fbcb308f3504276742ffc9a3bc35fd`  
		Last Modified: Fri, 06 Aug 2021 19:00:56 GMT  
		Size: 6.9 MB (6933133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a72de2e4e74462365f574ec07048641b834163995d6b95fb88af2fca27e01883`  
		Last Modified: Fri, 06 Aug 2021 19:00:52 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine3.14` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:572d6d4e53f14a9544d472214ec89300b1dbcc5e001d38c43b3ca6c656938369
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.3 MB (9349872 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5cc85837d0c5d21cf170c6240732f68dacf8b8aefb18875e65bec1f20f22f614`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 30 Jul 2021 18:36:19 GMT
ADD file:416a8b507abdc6bdcb22997a4be0a4170796c3f9f77e315b2dbff2b0a212bc68 in / 
# Fri, 30 Jul 2021 18:36:20 GMT
CMD ["/bin/sh"]
# Mon, 02 Aug 2021 23:10:49 GMT
ENV NATS_STREAMING_SERVER=0.22.1
# Mon, 02 Aug 2021 23:10:54 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='581698d248a19ecae64e4048d153bc1021744a3da6284680a339f9f82a53a9cf' ;; 		armhf) natsArch='arm6'; sha256='438a89221bb0608e40d21e73ca27a4b70b8560730726942c0ade94a6b6013d6f' ;; 		armv7) natsArch='arm7'; sha256='4164baadd201d1374f7654d3e54a24d81ceb87a385867e31a82c1d1a69e3b1ae' ;; 		x86_64) natsArch='amd64'; sha256='f29e87ac9ff998c928aa8ebc8cf0c4d04d34a3d95b9900d92fd7dafab2bec8cc' ;; 		x86) natsArch='386'; sha256='0ca68e57babb8901d7afeb7569042730904887e718ddf860ef3ee54278753505' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Mon, 02 Aug 2021 23:10:55 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Mon, 02 Aug 2021 23:10:55 GMT
EXPOSE 4222 8222
# Mon, 02 Aug 2021 23:10:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 02 Aug 2021 23:10:56 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:136482bf81d1fa351b424ebb8c7e34d15f2c5ed3fc0b66b544b8312bda3d52d9`  
		Last Modified: Tue, 15 Jun 2021 23:16:40 GMT  
		Size: 2.4 MB (2427917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bc8de0e43f342d9a142a0dc8c4560fdfa32841c714e46ed1649ae4a279d1e21`  
		Last Modified: Mon, 02 Aug 2021 23:12:44 GMT  
		Size: 6.9 MB (6921533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7a71caf384c90eee69558606851a144c0a87373fbb93628bab4378eb2c2b064`  
		Last Modified: Mon, 02 Aug 2021 23:12:40 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine3.14` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:4748f630b68c3b5d641d144f6e5b595a1d7b971b88c3e084566de5b09ab40e52
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.5 MB (9540696 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b70739b129dcb70fd6c70dd84f1e010b28a3aac72190b7104a2c6fc0356620fb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Tue, 15 Jun 2021 21:44:56 GMT
ADD file:6797caacbfe41bfe44000b39ed017016c6fcc492b3d6557cdaba88536df6c876 in / 
# Tue, 15 Jun 2021 21:44:56 GMT
CMD ["/bin/sh"]
# Mon, 02 Aug 2021 22:40:03 GMT
ENV NATS_STREAMING_SERVER=0.22.1
# Mon, 02 Aug 2021 22:40:06 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='581698d248a19ecae64e4048d153bc1021744a3da6284680a339f9f82a53a9cf' ;; 		armhf) natsArch='arm6'; sha256='438a89221bb0608e40d21e73ca27a4b70b8560730726942c0ade94a6b6013d6f' ;; 		armv7) natsArch='arm7'; sha256='4164baadd201d1374f7654d3e54a24d81ceb87a385867e31a82c1d1a69e3b1ae' ;; 		x86_64) natsArch='amd64'; sha256='f29e87ac9ff998c928aa8ebc8cf0c4d04d34a3d95b9900d92fd7dafab2bec8cc' ;; 		x86) natsArch='386'; sha256='0ca68e57babb8901d7afeb7569042730904887e718ddf860ef3ee54278753505' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Mon, 02 Aug 2021 22:40:07 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Mon, 02 Aug 2021 22:40:07 GMT
EXPOSE 4222 8222
# Mon, 02 Aug 2021 22:40:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 02 Aug 2021 22:40:07 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:58ab47519297212468320b23b8100fc1b2b96e8d342040806ae509a778a0a07a`  
		Last Modified: Tue, 15 Jun 2021 21:46:03 GMT  
		Size: 2.7 MB (2709626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a67c736eba594f7a9632ed9a3416f2aa6aba6bcfec575c0ded9b19400460da6`  
		Last Modified: Mon, 02 Aug 2021 22:40:59 GMT  
		Size: 6.8 MB (6830648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:478361e31dd37d3b803c22aac304317c89b32ffd60d662da3cf963124c3eb292`  
		Last Modified: Mon, 02 Aug 2021 22:40:58 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:latest`

```console
$ docker pull nats-streaming@sha256:f54d0597f76528b26771a5cacf18f82627877a247c788bcc0aad528f763c0b85
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.2061; amd64

### `nats-streaming:latest` - linux; amd64

```console
$ docker pull nats-streaming@sha256:3c6c9375f9e9724462e98cfb98a7abb50ceeca73b3070ce061992c4009e32157
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7168713 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:184d7920ac61dd2e84320b8040f57980a7d605d42948a520ede12d421168c4ce`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 02 Aug 2021 22:20:03 GMT
COPY file:ca9a212ccef327f9c2e91a62a908ac0cdbd39b08be331ea2b209c2d724942e18 in /nats-streaming-server 
# Mon, 02 Aug 2021 22:20:03 GMT
EXPOSE 4222 8222
# Mon, 02 Aug 2021 22:20:03 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 02 Aug 2021 22:20:03 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:f3749ab6cbfff03714b5a6a1245fa249b67d19e7358b74cbc50232b14370481a`  
		Last Modified: Mon, 02 Aug 2021 22:20:48 GMT  
		Size: 7.2 MB (7168713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:latest` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:e944d0e843d59d5979d7561c06b0c0adc874ceaa0bd34d3a7b536b25e8c9704d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.7 MB (6650246 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0146bbca3802c65d86e148b1d203b3d395ca1cd8a8bb89461888570d821dc4fb`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 02 Aug 2021 22:51:34 GMT
COPY file:68ac67d86d6ac617adc181feb43580415b7fc7640a3c7577bb3753c369908da0 in /nats-streaming-server 
# Mon, 02 Aug 2021 22:51:35 GMT
EXPOSE 4222 8222
# Mon, 02 Aug 2021 22:51:35 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 02 Aug 2021 22:51:35 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:c7e1d707b6179f690f3f44212cb8c9a3fe914d91d3f1ddbac9f176aa0610c90a`  
		Last Modified: Mon, 02 Aug 2021 22:53:32 GMT  
		Size: 6.7 MB (6650246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:latest` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:a5e3d56b343f9091f353634f59f688998544ccd4f2cbb80001d08ea6a3207274
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6639768 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80206ae32558812ad047d8ab67519615e98e7df68a884fc32b6d5fd8f72593b0`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 02 Aug 2021 23:11:17 GMT
COPY file:79708b5d249193a95e72c506453fd1ecd3e2738ec2ff3423c4b2bd760f426da2 in /nats-streaming-server 
# Mon, 02 Aug 2021 23:11:18 GMT
EXPOSE 4222 8222
# Mon, 02 Aug 2021 23:11:18 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 02 Aug 2021 23:11:19 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:52753762f751e166edd44e37a0ef0a06b33c337bdeb66e4134ee8479a49dae68`  
		Last Modified: Mon, 02 Aug 2021 23:13:17 GMT  
		Size: 6.6 MB (6639768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:latest` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:96652223cce95275138363a54affb8663ba46bc75831c2a9535375ab6d922143
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 MB (6546324 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:952bbd74028df1debbfe0e4665b514c66a36537d0868d41bc971ddb55793c442`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 02 Aug 2021 22:40:16 GMT
COPY file:a77d9769f43cc6943be482183091d3360eaadf93bf1ef5a67f0869d5555868a6 in /nats-streaming-server 
# Mon, 02 Aug 2021 22:40:17 GMT
EXPOSE 4222 8222
# Mon, 02 Aug 2021 22:40:17 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 02 Aug 2021 22:40:17 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4dc8aa7843ed2da454d59006acb180caee3f980d12034caacd4a32ffedab3df7`  
		Last Modified: Mon, 02 Aug 2021 22:41:24 GMT  
		Size: 6.5 MB (6546324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:latest` - windows version 10.0.17763.2061; amd64

```console
$ docker pull nats-streaming@sha256:349783a72dc891fd56179a54e998371cfe730524625447c5e5f8c8f99ef7d065
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.0 MB (110023666 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b2c8c7df75f26ed571fde792979a0ab215e1f76ff8e9a7f250cc092b15254741`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 06 Jul 2021 20:06:39 GMT
RUN Apply image 1809-amd64
# Wed, 14 Jul 2021 02:35:24 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Mon, 02 Aug 2021 22:17:13 GMT
RUN cmd /S /C #(nop) COPY file:9670e5d1fe5a71e47c78fde01235a0bcbcafcfdeeacf96a7669f6e49343fb03b in C:\nats-streaming-server.exe 
# Mon, 02 Aug 2021 22:17:16 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Mon, 02 Aug 2021 22:17:18 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Mon, 02 Aug 2021 22:17:21 GMT
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
	-	`sha256:395219f11b245d57e94766328eb17b3d461dcfac8402452fdc67df4b9e64361e`  
		Last Modified: Mon, 02 Aug 2021 22:22:03 GMT  
		Size: 7.3 MB (7293366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ed48c75b28949dec2cdb6cb3ff1179ad63c4c4371eba6a69a24baf25f2f6599`  
		Last Modified: Mon, 02 Aug 2021 22:21:54 GMT  
		Size: 1.2 KB (1173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a9b056cd35fd11d0c1057a2de6be2e533de9455af3383d08143215e972c3fd1`  
		Last Modified: Mon, 02 Aug 2021 22:21:55 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20642618c26e07a2aaf5f4169ff1a42ac92cb50404ebb140d800a9da097779ca`  
		Last Modified: Mon, 02 Aug 2021 22:21:55 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:linux`

```console
$ docker pull nats-streaming@sha256:7d3a953263095ea9d7018d32bd3483577d512550bc7890ba7743f48963cce893
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:linux` - linux; amd64

```console
$ docker pull nats-streaming@sha256:3c6c9375f9e9724462e98cfb98a7abb50ceeca73b3070ce061992c4009e32157
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7168713 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:184d7920ac61dd2e84320b8040f57980a7d605d42948a520ede12d421168c4ce`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 02 Aug 2021 22:20:03 GMT
COPY file:ca9a212ccef327f9c2e91a62a908ac0cdbd39b08be331ea2b209c2d724942e18 in /nats-streaming-server 
# Mon, 02 Aug 2021 22:20:03 GMT
EXPOSE 4222 8222
# Mon, 02 Aug 2021 22:20:03 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 02 Aug 2021 22:20:03 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:f3749ab6cbfff03714b5a6a1245fa249b67d19e7358b74cbc50232b14370481a`  
		Last Modified: Mon, 02 Aug 2021 22:20:48 GMT  
		Size: 7.2 MB (7168713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:linux` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:e944d0e843d59d5979d7561c06b0c0adc874ceaa0bd34d3a7b536b25e8c9704d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.7 MB (6650246 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0146bbca3802c65d86e148b1d203b3d395ca1cd8a8bb89461888570d821dc4fb`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 02 Aug 2021 22:51:34 GMT
COPY file:68ac67d86d6ac617adc181feb43580415b7fc7640a3c7577bb3753c369908da0 in /nats-streaming-server 
# Mon, 02 Aug 2021 22:51:35 GMT
EXPOSE 4222 8222
# Mon, 02 Aug 2021 22:51:35 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 02 Aug 2021 22:51:35 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:c7e1d707b6179f690f3f44212cb8c9a3fe914d91d3f1ddbac9f176aa0610c90a`  
		Last Modified: Mon, 02 Aug 2021 22:53:32 GMT  
		Size: 6.7 MB (6650246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:linux` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:a5e3d56b343f9091f353634f59f688998544ccd4f2cbb80001d08ea6a3207274
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6639768 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80206ae32558812ad047d8ab67519615e98e7df68a884fc32b6d5fd8f72593b0`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 02 Aug 2021 23:11:17 GMT
COPY file:79708b5d249193a95e72c506453fd1ecd3e2738ec2ff3423c4b2bd760f426da2 in /nats-streaming-server 
# Mon, 02 Aug 2021 23:11:18 GMT
EXPOSE 4222 8222
# Mon, 02 Aug 2021 23:11:18 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 02 Aug 2021 23:11:19 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:52753762f751e166edd44e37a0ef0a06b33c337bdeb66e4134ee8479a49dae68`  
		Last Modified: Mon, 02 Aug 2021 23:13:17 GMT  
		Size: 6.6 MB (6639768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:linux` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:96652223cce95275138363a54affb8663ba46bc75831c2a9535375ab6d922143
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 MB (6546324 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:952bbd74028df1debbfe0e4665b514c66a36537d0868d41bc971ddb55793c442`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 02 Aug 2021 22:40:16 GMT
COPY file:a77d9769f43cc6943be482183091d3360eaadf93bf1ef5a67f0869d5555868a6 in /nats-streaming-server 
# Mon, 02 Aug 2021 22:40:17 GMT
EXPOSE 4222 8222
# Mon, 02 Aug 2021 22:40:17 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 02 Aug 2021 22:40:17 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4dc8aa7843ed2da454d59006acb180caee3f980d12034caacd4a32ffedab3df7`  
		Last Modified: Mon, 02 Aug 2021 22:41:24 GMT  
		Size: 6.5 MB (6546324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:nanoserver`

```console
$ docker pull nats-streaming@sha256:a8998506db11878d76d6c5852804544f9c8129b9a980fe8c32ff898961a4664f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2061; amd64

### `nats-streaming:nanoserver` - windows version 10.0.17763.2061; amd64

```console
$ docker pull nats-streaming@sha256:349783a72dc891fd56179a54e998371cfe730524625447c5e5f8c8f99ef7d065
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.0 MB (110023666 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b2c8c7df75f26ed571fde792979a0ab215e1f76ff8e9a7f250cc092b15254741`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 06 Jul 2021 20:06:39 GMT
RUN Apply image 1809-amd64
# Wed, 14 Jul 2021 02:35:24 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Mon, 02 Aug 2021 22:17:13 GMT
RUN cmd /S /C #(nop) COPY file:9670e5d1fe5a71e47c78fde01235a0bcbcafcfdeeacf96a7669f6e49343fb03b in C:\nats-streaming-server.exe 
# Mon, 02 Aug 2021 22:17:16 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Mon, 02 Aug 2021 22:17:18 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Mon, 02 Aug 2021 22:17:21 GMT
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
	-	`sha256:395219f11b245d57e94766328eb17b3d461dcfac8402452fdc67df4b9e64361e`  
		Last Modified: Mon, 02 Aug 2021 22:22:03 GMT  
		Size: 7.3 MB (7293366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ed48c75b28949dec2cdb6cb3ff1179ad63c4c4371eba6a69a24baf25f2f6599`  
		Last Modified: Mon, 02 Aug 2021 22:21:54 GMT  
		Size: 1.2 KB (1173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a9b056cd35fd11d0c1057a2de6be2e533de9455af3383d08143215e972c3fd1`  
		Last Modified: Mon, 02 Aug 2021 22:21:55 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20642618c26e07a2aaf5f4169ff1a42ac92cb50404ebb140d800a9da097779ca`  
		Last Modified: Mon, 02 Aug 2021 22:21:55 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:nanoserver-1809`

```console
$ docker pull nats-streaming@sha256:a8998506db11878d76d6c5852804544f9c8129b9a980fe8c32ff898961a4664f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2061; amd64

### `nats-streaming:nanoserver-1809` - windows version 10.0.17763.2061; amd64

```console
$ docker pull nats-streaming@sha256:349783a72dc891fd56179a54e998371cfe730524625447c5e5f8c8f99ef7d065
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.0 MB (110023666 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b2c8c7df75f26ed571fde792979a0ab215e1f76ff8e9a7f250cc092b15254741`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 06 Jul 2021 20:06:39 GMT
RUN Apply image 1809-amd64
# Wed, 14 Jul 2021 02:35:24 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Mon, 02 Aug 2021 22:17:13 GMT
RUN cmd /S /C #(nop) COPY file:9670e5d1fe5a71e47c78fde01235a0bcbcafcfdeeacf96a7669f6e49343fb03b in C:\nats-streaming-server.exe 
# Mon, 02 Aug 2021 22:17:16 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Mon, 02 Aug 2021 22:17:18 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Mon, 02 Aug 2021 22:17:21 GMT
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
	-	`sha256:395219f11b245d57e94766328eb17b3d461dcfac8402452fdc67df4b9e64361e`  
		Last Modified: Mon, 02 Aug 2021 22:22:03 GMT  
		Size: 7.3 MB (7293366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ed48c75b28949dec2cdb6cb3ff1179ad63c4c4371eba6a69a24baf25f2f6599`  
		Last Modified: Mon, 02 Aug 2021 22:21:54 GMT  
		Size: 1.2 KB (1173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a9b056cd35fd11d0c1057a2de6be2e533de9455af3383d08143215e972c3fd1`  
		Last Modified: Mon, 02 Aug 2021 22:21:55 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20642618c26e07a2aaf5f4169ff1a42ac92cb50404ebb140d800a9da097779ca`  
		Last Modified: Mon, 02 Aug 2021 22:21:55 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:scratch`

```console
$ docker pull nats-streaming@sha256:7d3a953263095ea9d7018d32bd3483577d512550bc7890ba7743f48963cce893
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:scratch` - linux; amd64

```console
$ docker pull nats-streaming@sha256:3c6c9375f9e9724462e98cfb98a7abb50ceeca73b3070ce061992c4009e32157
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7168713 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:184d7920ac61dd2e84320b8040f57980a7d605d42948a520ede12d421168c4ce`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 02 Aug 2021 22:20:03 GMT
COPY file:ca9a212ccef327f9c2e91a62a908ac0cdbd39b08be331ea2b209c2d724942e18 in /nats-streaming-server 
# Mon, 02 Aug 2021 22:20:03 GMT
EXPOSE 4222 8222
# Mon, 02 Aug 2021 22:20:03 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 02 Aug 2021 22:20:03 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:f3749ab6cbfff03714b5a6a1245fa249b67d19e7358b74cbc50232b14370481a`  
		Last Modified: Mon, 02 Aug 2021 22:20:48 GMT  
		Size: 7.2 MB (7168713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:scratch` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:e944d0e843d59d5979d7561c06b0c0adc874ceaa0bd34d3a7b536b25e8c9704d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.7 MB (6650246 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0146bbca3802c65d86e148b1d203b3d395ca1cd8a8bb89461888570d821dc4fb`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 02 Aug 2021 22:51:34 GMT
COPY file:68ac67d86d6ac617adc181feb43580415b7fc7640a3c7577bb3753c369908da0 in /nats-streaming-server 
# Mon, 02 Aug 2021 22:51:35 GMT
EXPOSE 4222 8222
# Mon, 02 Aug 2021 22:51:35 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 02 Aug 2021 22:51:35 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:c7e1d707b6179f690f3f44212cb8c9a3fe914d91d3f1ddbac9f176aa0610c90a`  
		Last Modified: Mon, 02 Aug 2021 22:53:32 GMT  
		Size: 6.7 MB (6650246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:scratch` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:a5e3d56b343f9091f353634f59f688998544ccd4f2cbb80001d08ea6a3207274
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6639768 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80206ae32558812ad047d8ab67519615e98e7df68a884fc32b6d5fd8f72593b0`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 02 Aug 2021 23:11:17 GMT
COPY file:79708b5d249193a95e72c506453fd1ecd3e2738ec2ff3423c4b2bd760f426da2 in /nats-streaming-server 
# Mon, 02 Aug 2021 23:11:18 GMT
EXPOSE 4222 8222
# Mon, 02 Aug 2021 23:11:18 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 02 Aug 2021 23:11:19 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:52753762f751e166edd44e37a0ef0a06b33c337bdeb66e4134ee8479a49dae68`  
		Last Modified: Mon, 02 Aug 2021 23:13:17 GMT  
		Size: 6.6 MB (6639768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:scratch` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:96652223cce95275138363a54affb8663ba46bc75831c2a9535375ab6d922143
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 MB (6546324 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:952bbd74028df1debbfe0e4665b514c66a36537d0868d41bc971ddb55793c442`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 02 Aug 2021 22:40:16 GMT
COPY file:a77d9769f43cc6943be482183091d3360eaadf93bf1ef5a67f0869d5555868a6 in /nats-streaming-server 
# Mon, 02 Aug 2021 22:40:17 GMT
EXPOSE 4222 8222
# Mon, 02 Aug 2021 22:40:17 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 02 Aug 2021 22:40:17 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4dc8aa7843ed2da454d59006acb180caee3f980d12034caacd4a32ffedab3df7`  
		Last Modified: Mon, 02 Aug 2021 22:41:24 GMT  
		Size: 6.5 MB (6546324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:windowsservercore`

```console
$ docker pull nats-streaming@sha256:9889123db5aca4139825c5a01e3b51f879184e5afb7dc2eadf6d17144e422df3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.2061; amd64
	-	windows version 10.0.14393.4530; amd64

### `nats-streaming:windowsservercore` - windows version 10.0.17763.2061; amd64

```console
$ docker pull nats-streaming@sha256:f6b8175c40f3f10b3780b7c109018f478b76eff02f7f836799ccb6dbc547afff
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2693459206 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4430bbff42c38384275e1d9bc9c324202758dbfebec2f6cd6b28d789f82da1d4`
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
# Mon, 02 Aug 2021 22:14:15 GMT
ENV NATS_STREAMING_SERVER=0.22.1
# Mon, 02 Aug 2021 22:14:18 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.22.1/nats-streaming-server-v0.22.1-windows-amd64.zip
# Mon, 02 Aug 2021 22:14:20 GMT
ENV NATS_STREAMING_SERVER_SHASUM=4516852b493111b73ec06477be4a27e66f5abc9ca1ff4dd2b970232271611264
# Mon, 02 Aug 2021 22:15:13 GMT
RUN Set-PSDebug -Trace 2
# Mon, 02 Aug 2021 22:16:58 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Mon, 02 Aug 2021 22:17:01 GMT
EXPOSE 4222 8222
# Mon, 02 Aug 2021 22:17:03 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Mon, 02 Aug 2021 22:17:05 GMT
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
	-	`sha256:b82a3397b3004db7b8c949da737373cf77ed78fdc90030761e97b09e9c9da2bf`  
		Last Modified: Mon, 02 Aug 2021 22:21:36 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f572e3b3f17155a894e961cb378e5de8d16423892838ca8d407dc1b231bdc24`  
		Last Modified: Mon, 02 Aug 2021 22:21:37 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abda54712825ab0cf77038a010dd6c7242f1aeeabb71aaf24969fa2f52b3b290`  
		Last Modified: Mon, 02 Aug 2021 22:21:36 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7399265a146c0fbcbffb8fb2c4d1c03f880ba30c21f33870222c056d3645d4d6`  
		Last Modified: Mon, 02 Aug 2021 22:21:34 GMT  
		Size: 364.1 KB (364103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7a5c5de7479ffd1fbc76c31256335ccbb1634b15e36125a3dfb58104d89a28c`  
		Last Modified: Mon, 02 Aug 2021 22:21:42 GMT  
		Size: 7.6 MB (7636991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f117f06baadaabef0f04b3caf48313f15c143ec663ad83aacf76f5d4d54755f0`  
		Last Modified: Mon, 02 Aug 2021 22:21:33 GMT  
		Size: 1.4 KB (1380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:720a0dee2313cb05fd58b997c2bfedf8b50fc0d16e3f2607f3ebe7c3d1dcdd93`  
		Last Modified: Mon, 02 Aug 2021 22:21:33 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cbfab2e5a68567dff0f8c930bef2751e3ae565099264e67a7806e5b2c8dcad2`  
		Last Modified: Mon, 02 Aug 2021 22:21:33 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:windowsservercore` - windows version 10.0.14393.4530; amd64

```console
$ docker pull nats-streaming@sha256:860350027ca4ce7cc64bebf9130ba5945be2b66f699aa4b673230bc8ffea5c59
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6282131227 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e461920fa53ab45b03bab923188b17759cb5848b9e4d659fec9399b15db13a9`
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
# Mon, 02 Aug 2021 22:17:28 GMT
ENV NATS_STREAMING_SERVER=0.22.1
# Mon, 02 Aug 2021 22:17:30 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.22.1/nats-streaming-server-v0.22.1-windows-amd64.zip
# Mon, 02 Aug 2021 22:17:33 GMT
ENV NATS_STREAMING_SERVER_SHASUM=4516852b493111b73ec06477be4a27e66f5abc9ca1ff4dd2b970232271611264
# Mon, 02 Aug 2021 22:18:44 GMT
RUN Set-PSDebug -Trace 2
# Mon, 02 Aug 2021 22:20:44 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Mon, 02 Aug 2021 22:20:46 GMT
EXPOSE 4222 8222
# Mon, 02 Aug 2021 22:20:48 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Mon, 02 Aug 2021 22:20:51 GMT
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
	-	`sha256:01daf4d8d551d6c71e26b9bd4071c9351c0014204d91d856f62076352888ff60`  
		Last Modified: Mon, 02 Aug 2021 22:22:17 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:358b658f14950cb4b2565fbd69fe74eed09949766936621272cff6b3baec317e`  
		Last Modified: Mon, 02 Aug 2021 22:22:18 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3d659d88ad2536c4d7245d222179697bc67d83eb272e7bffa390b50b40c64c0`  
		Last Modified: Mon, 02 Aug 2021 22:22:17 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a581447cad2fda655b58c8e3bbd295b07bcc0205a4eb67c4ffe1b9e0fe479683`  
		Last Modified: Mon, 02 Aug 2021 22:22:15 GMT  
		Size: 364.7 KB (364703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71d3b74ad59b935bb18aa870ecb7df8da9772cefe1d5d3f2f2306d88377bc44a`  
		Last Modified: Mon, 02 Aug 2021 22:22:18 GMT  
		Size: 12.1 MB (12123210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ea62a2c358dd2cab71368c491b629f2cac1c30279e1f3b978bc6caafb67b622`  
		Last Modified: Mon, 02 Aug 2021 22:22:15 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4db9e168d575777fd554d75d34ce2211baa34995899ef0905b50611438ec670d`  
		Last Modified: Mon, 02 Aug 2021 22:22:15 GMT  
		Size: 1.4 KB (1386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:840688f6769f85ae88251d93ec16c131578aabbcaa04a53860c4d6723b77adf1`  
		Last Modified: Mon, 02 Aug 2021 22:22:15 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:windowsservercore-1809`

```console
$ docker pull nats-streaming@sha256:433e566e09863176f21000377e836734fb87f52a894eb753ae98476653157b8a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2061; amd64

### `nats-streaming:windowsservercore-1809` - windows version 10.0.17763.2061; amd64

```console
$ docker pull nats-streaming@sha256:f6b8175c40f3f10b3780b7c109018f478b76eff02f7f836799ccb6dbc547afff
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2693459206 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4430bbff42c38384275e1d9bc9c324202758dbfebec2f6cd6b28d789f82da1d4`
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
# Mon, 02 Aug 2021 22:14:15 GMT
ENV NATS_STREAMING_SERVER=0.22.1
# Mon, 02 Aug 2021 22:14:18 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.22.1/nats-streaming-server-v0.22.1-windows-amd64.zip
# Mon, 02 Aug 2021 22:14:20 GMT
ENV NATS_STREAMING_SERVER_SHASUM=4516852b493111b73ec06477be4a27e66f5abc9ca1ff4dd2b970232271611264
# Mon, 02 Aug 2021 22:15:13 GMT
RUN Set-PSDebug -Trace 2
# Mon, 02 Aug 2021 22:16:58 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Mon, 02 Aug 2021 22:17:01 GMT
EXPOSE 4222 8222
# Mon, 02 Aug 2021 22:17:03 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Mon, 02 Aug 2021 22:17:05 GMT
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
	-	`sha256:b82a3397b3004db7b8c949da737373cf77ed78fdc90030761e97b09e9c9da2bf`  
		Last Modified: Mon, 02 Aug 2021 22:21:36 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f572e3b3f17155a894e961cb378e5de8d16423892838ca8d407dc1b231bdc24`  
		Last Modified: Mon, 02 Aug 2021 22:21:37 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abda54712825ab0cf77038a010dd6c7242f1aeeabb71aaf24969fa2f52b3b290`  
		Last Modified: Mon, 02 Aug 2021 22:21:36 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7399265a146c0fbcbffb8fb2c4d1c03f880ba30c21f33870222c056d3645d4d6`  
		Last Modified: Mon, 02 Aug 2021 22:21:34 GMT  
		Size: 364.1 KB (364103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7a5c5de7479ffd1fbc76c31256335ccbb1634b15e36125a3dfb58104d89a28c`  
		Last Modified: Mon, 02 Aug 2021 22:21:42 GMT  
		Size: 7.6 MB (7636991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f117f06baadaabef0f04b3caf48313f15c143ec663ad83aacf76f5d4d54755f0`  
		Last Modified: Mon, 02 Aug 2021 22:21:33 GMT  
		Size: 1.4 KB (1380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:720a0dee2313cb05fd58b997c2bfedf8b50fc0d16e3f2607f3ebe7c3d1dcdd93`  
		Last Modified: Mon, 02 Aug 2021 22:21:33 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cbfab2e5a68567dff0f8c930bef2751e3ae565099264e67a7806e5b2c8dcad2`  
		Last Modified: Mon, 02 Aug 2021 22:21:33 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:windowsservercore-ltsc2016`

```console
$ docker pull nats-streaming@sha256:2b063c7774ef1b3c10036710cbfbbad511dd3951dccfa380271c036b784e83ea
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.14393.4530; amd64

### `nats-streaming:windowsservercore-ltsc2016` - windows version 10.0.14393.4530; amd64

```console
$ docker pull nats-streaming@sha256:860350027ca4ce7cc64bebf9130ba5945be2b66f699aa4b673230bc8ffea5c59
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6282131227 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e461920fa53ab45b03bab923188b17759cb5848b9e4d659fec9399b15db13a9`
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
# Mon, 02 Aug 2021 22:17:28 GMT
ENV NATS_STREAMING_SERVER=0.22.1
# Mon, 02 Aug 2021 22:17:30 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.22.1/nats-streaming-server-v0.22.1-windows-amd64.zip
# Mon, 02 Aug 2021 22:17:33 GMT
ENV NATS_STREAMING_SERVER_SHASUM=4516852b493111b73ec06477be4a27e66f5abc9ca1ff4dd2b970232271611264
# Mon, 02 Aug 2021 22:18:44 GMT
RUN Set-PSDebug -Trace 2
# Mon, 02 Aug 2021 22:20:44 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Mon, 02 Aug 2021 22:20:46 GMT
EXPOSE 4222 8222
# Mon, 02 Aug 2021 22:20:48 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Mon, 02 Aug 2021 22:20:51 GMT
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
	-	`sha256:01daf4d8d551d6c71e26b9bd4071c9351c0014204d91d856f62076352888ff60`  
		Last Modified: Mon, 02 Aug 2021 22:22:17 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:358b658f14950cb4b2565fbd69fe74eed09949766936621272cff6b3baec317e`  
		Last Modified: Mon, 02 Aug 2021 22:22:18 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3d659d88ad2536c4d7245d222179697bc67d83eb272e7bffa390b50b40c64c0`  
		Last Modified: Mon, 02 Aug 2021 22:22:17 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a581447cad2fda655b58c8e3bbd295b07bcc0205a4eb67c4ffe1b9e0fe479683`  
		Last Modified: Mon, 02 Aug 2021 22:22:15 GMT  
		Size: 364.7 KB (364703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71d3b74ad59b935bb18aa870ecb7df8da9772cefe1d5d3f2f2306d88377bc44a`  
		Last Modified: Mon, 02 Aug 2021 22:22:18 GMT  
		Size: 12.1 MB (12123210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ea62a2c358dd2cab71368c491b629f2cac1c30279e1f3b978bc6caafb67b622`  
		Last Modified: Mon, 02 Aug 2021 22:22:15 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4db9e168d575777fd554d75d34ce2211baa34995899ef0905b50611438ec670d`  
		Last Modified: Mon, 02 Aug 2021 22:22:15 GMT  
		Size: 1.4 KB (1386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:840688f6769f85ae88251d93ec16c131578aabbcaa04a53860c4d6723b77adf1`  
		Last Modified: Mon, 02 Aug 2021 22:22:15 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
