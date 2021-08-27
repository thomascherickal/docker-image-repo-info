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
$ docker pull nats-streaming@sha256:f0716868aa216d2a8803f3580bd512fc699da2d7a6af8ff6c5c857d47192e6e7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.2114; amd64

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

### `nats-streaming:0.22` - windows version 10.0.17763.2114; amd64

```console
$ docker pull nats-streaming@sha256:6cf5f132f44fee4ec7d112868c7525aac42e5eef00cd0298e1efdffcb1df5251
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.0 MB (110038648 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7863a1802021516178bb5e20547b7e410590d3ad269287d3d99fd163070dc55b`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 05 Aug 2021 19:15:20 GMT
RUN Apply image 1809-amd64
# Wed, 25 Aug 2021 16:07:56 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 25 Aug 2021 19:33:43 GMT
RUN cmd /S /C #(nop) COPY file:9670e5d1fe5a71e47c78fde01235a0bcbcafcfdeeacf96a7669f6e49343fb03b in C:\nats-streaming-server.exe 
# Wed, 25 Aug 2021 19:33:45 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 25 Aug 2021 19:33:45 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 25 Aug 2021 19:33:46 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:bc8517709e9cfff223cb034ff5be8fcbfa5409de286cdac9ae1b8878ebea6b84`  
		Size: 102.7 MB (102741177 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ae8616c17f5cca409a4b1289387e37dc532657ba2b52bb60713ff621acccd506`  
		Last Modified: Wed, 25 Aug 2021 16:11:20 GMT  
		Size: 1.0 KB (1022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa124ed4fe9f29ce6e3db339e67e84f8667fe9ad034f27a42d6554c473e49de1`  
		Last Modified: Wed, 25 Aug 2021 19:37:03 GMT  
		Size: 7.3 MB (7293262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e47ccb646b6561c33cebea3e0f6ffb755fbcec2983095a9fcd42cda5c49b519`  
		Last Modified: Wed, 25 Aug 2021 19:37:01 GMT  
		Size: 1.1 KB (1069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:993faf624f9f41d879898713c9dd7875da6724079bf4f9d0a8af4c5a780dd6c0`  
		Last Modified: Wed, 25 Aug 2021 19:37:00 GMT  
		Size: 1.1 KB (1050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2df1fdf71a2973683c32f5a7cbf28584f357d292855672645e4fda8b1200e200`  
		Last Modified: Wed, 25 Aug 2021 19:37:01 GMT  
		Size: 1.1 KB (1068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.22-alpine`

```console
$ docker pull nats-streaming@sha256:025dd4f7090b799587d1ba45d887a67d44f9d12ad0b7c474a8e72c3886150382
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.22-alpine` - linux; amd64

```console
$ docker pull nats-streaming@sha256:490adf058de78b1fe4f0d33864796f8a112c3b784c6e90ba22e45153fe74d900
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.3 MB (10270658 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fabf0e12d64e19686c51b041dd0cc13952c874c78e6f6c5e113a95dd59c4ea55`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 27 Aug 2021 20:46:27 GMT
ENV NATS_STREAMING_SERVER=0.22.1
# Fri, 27 Aug 2021 20:46:31 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='581698d248a19ecae64e4048d153bc1021744a3da6284680a339f9f82a53a9cf' ;; 		armhf) natsArch='arm6'; sha256='438a89221bb0608e40d21e73ca27a4b70b8560730726942c0ade94a6b6013d6f' ;; 		armv7) natsArch='arm7'; sha256='4164baadd201d1374f7654d3e54a24d81ceb87a385867e31a82c1d1a69e3b1ae' ;; 		x86_64) natsArch='amd64'; sha256='f29e87ac9ff998c928aa8ebc8cf0c4d04d34a3d95b9900d92fd7dafab2bec8cc' ;; 		x86) natsArch='386'; sha256='0ca68e57babb8901d7afeb7569042730904887e718ddf860ef3ee54278753505' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 27 Aug 2021 20:46:31 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Fri, 27 Aug 2021 20:46:32 GMT
EXPOSE 4222 8222
# Fri, 27 Aug 2021 20:46:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 Aug 2021 20:46:33 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8848530ed3e01ccf52dafe72a2e2c14ec4f6ec52809524bd71c33cbe193e5ad3`  
		Last Modified: Fri, 27 Aug 2021 20:47:18 GMT  
		Size: 7.5 MB (7455792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0a13cfe7f8352b89abb0a8ea81910d679c36c4a90d6d88d7f8a9059471b2e31`  
		Last Modified: Fri, 27 Aug 2021 20:47:16 GMT  
		Size: 420.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.22-alpine` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:9cda74ceed2f45daa20c52af4aa059d5af71f373753072e64d1223e5de592e64
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.6 MB (9561001 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f85120fadd96bf6e11b7fa82dd813c6d56b9aff9cb577d22dc8cbaaae6ac263`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 27 Aug 2021 17:49:29 GMT
ADD file:1c1c4520d49cb6e8f795f3b953d1ed3c3c77868b98b53a455169c254fcec5acd in / 
# Fri, 27 Aug 2021 17:49:30 GMT
CMD ["/bin/sh"]
# Fri, 27 Aug 2021 19:24:22 GMT
ENV NATS_STREAMING_SERVER=0.22.1
# Fri, 27 Aug 2021 19:24:28 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='581698d248a19ecae64e4048d153bc1021744a3da6284680a339f9f82a53a9cf' ;; 		armhf) natsArch='arm6'; sha256='438a89221bb0608e40d21e73ca27a4b70b8560730726942c0ade94a6b6013d6f' ;; 		armv7) natsArch='arm7'; sha256='4164baadd201d1374f7654d3e54a24d81ceb87a385867e31a82c1d1a69e3b1ae' ;; 		x86_64) natsArch='amd64'; sha256='f29e87ac9ff998c928aa8ebc8cf0c4d04d34a3d95b9900d92fd7dafab2bec8cc' ;; 		x86) natsArch='386'; sha256='0ca68e57babb8901d7afeb7569042730904887e718ddf860ef3ee54278753505' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 27 Aug 2021 19:24:29 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Fri, 27 Aug 2021 19:24:29 GMT
EXPOSE 4222 8222
# Fri, 27 Aug 2021 19:24:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 Aug 2021 19:24:30 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:2e78c0f86ba9a1fed30df20cb48c9cc73e9626399f12749d36b892ff99c0ecf5`  
		Last Modified: Fri, 27 Aug 2021 17:50:55 GMT  
		Size: 2.6 MB (2627447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:320a6a97adac4a737e1997906fcc9d6922c1ae39980382314b88be30f8b64ea3`  
		Last Modified: Fri, 27 Aug 2021 19:26:12 GMT  
		Size: 6.9 MB (6933133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92e6007c46c9095e062e9214fe2c0618a2b2fe8642c7f6162972036163e330ad`  
		Last Modified: Fri, 27 Aug 2021 19:26:08 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.22-alpine` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:7970395d00490fad62f2a51288db47d251cab92ec7634bef6de42343f8e8eedc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.4 MB (9351328 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e19086c92b47964c105a8ed130ff7219833adab1ca8e211c1ad0b0a049866252`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 06 Aug 2021 17:57:32 GMT
ADD file:3a35ff3ac0d80289d419a4d6d8319610c38e1936d296addafb9aaf506946230f in / 
# Fri, 06 Aug 2021 17:57:32 GMT
CMD ["/bin/sh"]
# Fri, 06 Aug 2021 20:29:42 GMT
ENV NATS_STREAMING_SERVER=0.22.1
# Fri, 06 Aug 2021 20:29:48 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='581698d248a19ecae64e4048d153bc1021744a3da6284680a339f9f82a53a9cf' ;; 		armhf) natsArch='arm6'; sha256='438a89221bb0608e40d21e73ca27a4b70b8560730726942c0ade94a6b6013d6f' ;; 		armv7) natsArch='arm7'; sha256='4164baadd201d1374f7654d3e54a24d81ceb87a385867e31a82c1d1a69e3b1ae' ;; 		x86_64) natsArch='amd64'; sha256='f29e87ac9ff998c928aa8ebc8cf0c4d04d34a3d95b9900d92fd7dafab2bec8cc' ;; 		x86) natsArch='386'; sha256='0ca68e57babb8901d7afeb7569042730904887e718ddf860ef3ee54278753505' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 06 Aug 2021 20:29:48 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Fri, 06 Aug 2021 20:29:49 GMT
EXPOSE 4222 8222
# Fri, 06 Aug 2021 20:29:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 06 Aug 2021 20:29:50 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:4ee0caa23b369b04827640a4be298bf4ff7bacd030c77e915f5d7fb8f987594a`  
		Last Modified: Fri, 06 Aug 2021 17:58:57 GMT  
		Size: 2.4 MB (2429359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e14712e6c4fbdd823f35d0df7aa1345088ce3d89727133dcef4adb1105ecb5f`  
		Last Modified: Fri, 06 Aug 2021 20:31:34 GMT  
		Size: 6.9 MB (6921548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e18c45098374f86d0784e7840a2c0fd15ce636edfee6d3ebc23432fd0cc47be5`  
		Last Modified: Fri, 06 Aug 2021 20:31:30 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.22-alpine` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:366b541434718f0d0bd3e6fffb5dd27db81774c771dc0ecb69c00819fb1b3997
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.5 MB (9542913 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:244415bb00005ee5391d41fc5b03c3477bcf4f2c70a6d081a65dc46b732956c4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Fri, 27 Aug 2021 20:20:38 GMT
ENV NATS_STREAMING_SERVER=0.22.1
# Fri, 27 Aug 2021 20:20:41 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='581698d248a19ecae64e4048d153bc1021744a3da6284680a339f9f82a53a9cf' ;; 		armhf) natsArch='arm6'; sha256='438a89221bb0608e40d21e73ca27a4b70b8560730726942c0ade94a6b6013d6f' ;; 		armv7) natsArch='arm7'; sha256='4164baadd201d1374f7654d3e54a24d81ceb87a385867e31a82c1d1a69e3b1ae' ;; 		x86_64) natsArch='amd64'; sha256='f29e87ac9ff998c928aa8ebc8cf0c4d04d34a3d95b9900d92fd7dafab2bec8cc' ;; 		x86) natsArch='386'; sha256='0ca68e57babb8901d7afeb7569042730904887e718ddf860ef3ee54278753505' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 27 Aug 2021 20:20:41 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Fri, 27 Aug 2021 20:20:41 GMT
EXPOSE 4222 8222
# Fri, 27 Aug 2021 20:20:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 Aug 2021 20:20:41 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:552d1f2373af9bfe12033568ebbfb0ccbb0de11279f9a415a29207e264d7f4d9`  
		Last Modified: Fri, 27 Aug 2021 17:40:18 GMT  
		Size: 2.7 MB (2711827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:069785721c5e4cdee5b76770ae83cf97b47105b106c53b06922f570ba743dadb`  
		Last Modified: Fri, 27 Aug 2021 20:21:32 GMT  
		Size: 6.8 MB (6830666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df70eb7a18c78f5cbb612b797fe94d277338f4bd8e5dfd47cba3d97d57e0e352`  
		Last Modified: Fri, 27 Aug 2021 20:21:31 GMT  
		Size: 420.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.22-alpine3.14`

```console
$ docker pull nats-streaming@sha256:025dd4f7090b799587d1ba45d887a67d44f9d12ad0b7c474a8e72c3886150382
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.22-alpine3.14` - linux; amd64

```console
$ docker pull nats-streaming@sha256:490adf058de78b1fe4f0d33864796f8a112c3b784c6e90ba22e45153fe74d900
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.3 MB (10270658 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fabf0e12d64e19686c51b041dd0cc13952c874c78e6f6c5e113a95dd59c4ea55`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 27 Aug 2021 20:46:27 GMT
ENV NATS_STREAMING_SERVER=0.22.1
# Fri, 27 Aug 2021 20:46:31 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='581698d248a19ecae64e4048d153bc1021744a3da6284680a339f9f82a53a9cf' ;; 		armhf) natsArch='arm6'; sha256='438a89221bb0608e40d21e73ca27a4b70b8560730726942c0ade94a6b6013d6f' ;; 		armv7) natsArch='arm7'; sha256='4164baadd201d1374f7654d3e54a24d81ceb87a385867e31a82c1d1a69e3b1ae' ;; 		x86_64) natsArch='amd64'; sha256='f29e87ac9ff998c928aa8ebc8cf0c4d04d34a3d95b9900d92fd7dafab2bec8cc' ;; 		x86) natsArch='386'; sha256='0ca68e57babb8901d7afeb7569042730904887e718ddf860ef3ee54278753505' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 27 Aug 2021 20:46:31 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Fri, 27 Aug 2021 20:46:32 GMT
EXPOSE 4222 8222
# Fri, 27 Aug 2021 20:46:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 Aug 2021 20:46:33 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8848530ed3e01ccf52dafe72a2e2c14ec4f6ec52809524bd71c33cbe193e5ad3`  
		Last Modified: Fri, 27 Aug 2021 20:47:18 GMT  
		Size: 7.5 MB (7455792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0a13cfe7f8352b89abb0a8ea81910d679c36c4a90d6d88d7f8a9059471b2e31`  
		Last Modified: Fri, 27 Aug 2021 20:47:16 GMT  
		Size: 420.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.22-alpine3.14` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:9cda74ceed2f45daa20c52af4aa059d5af71f373753072e64d1223e5de592e64
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.6 MB (9561001 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f85120fadd96bf6e11b7fa82dd813c6d56b9aff9cb577d22dc8cbaaae6ac263`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 27 Aug 2021 17:49:29 GMT
ADD file:1c1c4520d49cb6e8f795f3b953d1ed3c3c77868b98b53a455169c254fcec5acd in / 
# Fri, 27 Aug 2021 17:49:30 GMT
CMD ["/bin/sh"]
# Fri, 27 Aug 2021 19:24:22 GMT
ENV NATS_STREAMING_SERVER=0.22.1
# Fri, 27 Aug 2021 19:24:28 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='581698d248a19ecae64e4048d153bc1021744a3da6284680a339f9f82a53a9cf' ;; 		armhf) natsArch='arm6'; sha256='438a89221bb0608e40d21e73ca27a4b70b8560730726942c0ade94a6b6013d6f' ;; 		armv7) natsArch='arm7'; sha256='4164baadd201d1374f7654d3e54a24d81ceb87a385867e31a82c1d1a69e3b1ae' ;; 		x86_64) natsArch='amd64'; sha256='f29e87ac9ff998c928aa8ebc8cf0c4d04d34a3d95b9900d92fd7dafab2bec8cc' ;; 		x86) natsArch='386'; sha256='0ca68e57babb8901d7afeb7569042730904887e718ddf860ef3ee54278753505' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 27 Aug 2021 19:24:29 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Fri, 27 Aug 2021 19:24:29 GMT
EXPOSE 4222 8222
# Fri, 27 Aug 2021 19:24:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 Aug 2021 19:24:30 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:2e78c0f86ba9a1fed30df20cb48c9cc73e9626399f12749d36b892ff99c0ecf5`  
		Last Modified: Fri, 27 Aug 2021 17:50:55 GMT  
		Size: 2.6 MB (2627447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:320a6a97adac4a737e1997906fcc9d6922c1ae39980382314b88be30f8b64ea3`  
		Last Modified: Fri, 27 Aug 2021 19:26:12 GMT  
		Size: 6.9 MB (6933133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92e6007c46c9095e062e9214fe2c0618a2b2fe8642c7f6162972036163e330ad`  
		Last Modified: Fri, 27 Aug 2021 19:26:08 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.22-alpine3.14` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:7970395d00490fad62f2a51288db47d251cab92ec7634bef6de42343f8e8eedc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.4 MB (9351328 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e19086c92b47964c105a8ed130ff7219833adab1ca8e211c1ad0b0a049866252`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 06 Aug 2021 17:57:32 GMT
ADD file:3a35ff3ac0d80289d419a4d6d8319610c38e1936d296addafb9aaf506946230f in / 
# Fri, 06 Aug 2021 17:57:32 GMT
CMD ["/bin/sh"]
# Fri, 06 Aug 2021 20:29:42 GMT
ENV NATS_STREAMING_SERVER=0.22.1
# Fri, 06 Aug 2021 20:29:48 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='581698d248a19ecae64e4048d153bc1021744a3da6284680a339f9f82a53a9cf' ;; 		armhf) natsArch='arm6'; sha256='438a89221bb0608e40d21e73ca27a4b70b8560730726942c0ade94a6b6013d6f' ;; 		armv7) natsArch='arm7'; sha256='4164baadd201d1374f7654d3e54a24d81ceb87a385867e31a82c1d1a69e3b1ae' ;; 		x86_64) natsArch='amd64'; sha256='f29e87ac9ff998c928aa8ebc8cf0c4d04d34a3d95b9900d92fd7dafab2bec8cc' ;; 		x86) natsArch='386'; sha256='0ca68e57babb8901d7afeb7569042730904887e718ddf860ef3ee54278753505' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 06 Aug 2021 20:29:48 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Fri, 06 Aug 2021 20:29:49 GMT
EXPOSE 4222 8222
# Fri, 06 Aug 2021 20:29:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 06 Aug 2021 20:29:50 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:4ee0caa23b369b04827640a4be298bf4ff7bacd030c77e915f5d7fb8f987594a`  
		Last Modified: Fri, 06 Aug 2021 17:58:57 GMT  
		Size: 2.4 MB (2429359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e14712e6c4fbdd823f35d0df7aa1345088ce3d89727133dcef4adb1105ecb5f`  
		Last Modified: Fri, 06 Aug 2021 20:31:34 GMT  
		Size: 6.9 MB (6921548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e18c45098374f86d0784e7840a2c0fd15ce636edfee6d3ebc23432fd0cc47be5`  
		Last Modified: Fri, 06 Aug 2021 20:31:30 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.22-alpine3.14` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:366b541434718f0d0bd3e6fffb5dd27db81774c771dc0ecb69c00819fb1b3997
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.5 MB (9542913 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:244415bb00005ee5391d41fc5b03c3477bcf4f2c70a6d081a65dc46b732956c4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Fri, 27 Aug 2021 20:20:38 GMT
ENV NATS_STREAMING_SERVER=0.22.1
# Fri, 27 Aug 2021 20:20:41 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='581698d248a19ecae64e4048d153bc1021744a3da6284680a339f9f82a53a9cf' ;; 		armhf) natsArch='arm6'; sha256='438a89221bb0608e40d21e73ca27a4b70b8560730726942c0ade94a6b6013d6f' ;; 		armv7) natsArch='arm7'; sha256='4164baadd201d1374f7654d3e54a24d81ceb87a385867e31a82c1d1a69e3b1ae' ;; 		x86_64) natsArch='amd64'; sha256='f29e87ac9ff998c928aa8ebc8cf0c4d04d34a3d95b9900d92fd7dafab2bec8cc' ;; 		x86) natsArch='386'; sha256='0ca68e57babb8901d7afeb7569042730904887e718ddf860ef3ee54278753505' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 27 Aug 2021 20:20:41 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Fri, 27 Aug 2021 20:20:41 GMT
EXPOSE 4222 8222
# Fri, 27 Aug 2021 20:20:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 Aug 2021 20:20:41 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:552d1f2373af9bfe12033568ebbfb0ccbb0de11279f9a415a29207e264d7f4d9`  
		Last Modified: Fri, 27 Aug 2021 17:40:18 GMT  
		Size: 2.7 MB (2711827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:069785721c5e4cdee5b76770ae83cf97b47105b106c53b06922f570ba743dadb`  
		Last Modified: Fri, 27 Aug 2021 20:21:32 GMT  
		Size: 6.8 MB (6830666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df70eb7a18c78f5cbb612b797fe94d277338f4bd8e5dfd47cba3d97d57e0e352`  
		Last Modified: Fri, 27 Aug 2021 20:21:31 GMT  
		Size: 420.0 B  
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
$ docker pull nats-streaming@sha256:d86bdcb9e19d16a21ea8eb07693268eab508df92a0df40021ca3b296412ba430
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2114; amd64

### `nats-streaming:0.22-nanoserver` - windows version 10.0.17763.2114; amd64

```console
$ docker pull nats-streaming@sha256:6cf5f132f44fee4ec7d112868c7525aac42e5eef00cd0298e1efdffcb1df5251
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.0 MB (110038648 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7863a1802021516178bb5e20547b7e410590d3ad269287d3d99fd163070dc55b`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 05 Aug 2021 19:15:20 GMT
RUN Apply image 1809-amd64
# Wed, 25 Aug 2021 16:07:56 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 25 Aug 2021 19:33:43 GMT
RUN cmd /S /C #(nop) COPY file:9670e5d1fe5a71e47c78fde01235a0bcbcafcfdeeacf96a7669f6e49343fb03b in C:\nats-streaming-server.exe 
# Wed, 25 Aug 2021 19:33:45 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 25 Aug 2021 19:33:45 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 25 Aug 2021 19:33:46 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:bc8517709e9cfff223cb034ff5be8fcbfa5409de286cdac9ae1b8878ebea6b84`  
		Size: 102.7 MB (102741177 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ae8616c17f5cca409a4b1289387e37dc532657ba2b52bb60713ff621acccd506`  
		Last Modified: Wed, 25 Aug 2021 16:11:20 GMT  
		Size: 1.0 KB (1022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa124ed4fe9f29ce6e3db339e67e84f8667fe9ad034f27a42d6554c473e49de1`  
		Last Modified: Wed, 25 Aug 2021 19:37:03 GMT  
		Size: 7.3 MB (7293262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e47ccb646b6561c33cebea3e0f6ffb755fbcec2983095a9fcd42cda5c49b519`  
		Last Modified: Wed, 25 Aug 2021 19:37:01 GMT  
		Size: 1.1 KB (1069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:993faf624f9f41d879898713c9dd7875da6724079bf4f9d0a8af4c5a780dd6c0`  
		Last Modified: Wed, 25 Aug 2021 19:37:00 GMT  
		Size: 1.1 KB (1050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2df1fdf71a2973683c32f5a7cbf28584f357d292855672645e4fda8b1200e200`  
		Last Modified: Wed, 25 Aug 2021 19:37:01 GMT  
		Size: 1.1 KB (1068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.22-nanoserver-1809`

```console
$ docker pull nats-streaming@sha256:d86bdcb9e19d16a21ea8eb07693268eab508df92a0df40021ca3b296412ba430
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2114; amd64

### `nats-streaming:0.22-nanoserver-1809` - windows version 10.0.17763.2114; amd64

```console
$ docker pull nats-streaming@sha256:6cf5f132f44fee4ec7d112868c7525aac42e5eef00cd0298e1efdffcb1df5251
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.0 MB (110038648 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7863a1802021516178bb5e20547b7e410590d3ad269287d3d99fd163070dc55b`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 05 Aug 2021 19:15:20 GMT
RUN Apply image 1809-amd64
# Wed, 25 Aug 2021 16:07:56 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 25 Aug 2021 19:33:43 GMT
RUN cmd /S /C #(nop) COPY file:9670e5d1fe5a71e47c78fde01235a0bcbcafcfdeeacf96a7669f6e49343fb03b in C:\nats-streaming-server.exe 
# Wed, 25 Aug 2021 19:33:45 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 25 Aug 2021 19:33:45 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 25 Aug 2021 19:33:46 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:bc8517709e9cfff223cb034ff5be8fcbfa5409de286cdac9ae1b8878ebea6b84`  
		Size: 102.7 MB (102741177 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ae8616c17f5cca409a4b1289387e37dc532657ba2b52bb60713ff621acccd506`  
		Last Modified: Wed, 25 Aug 2021 16:11:20 GMT  
		Size: 1.0 KB (1022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa124ed4fe9f29ce6e3db339e67e84f8667fe9ad034f27a42d6554c473e49de1`  
		Last Modified: Wed, 25 Aug 2021 19:37:03 GMT  
		Size: 7.3 MB (7293262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e47ccb646b6561c33cebea3e0f6ffb755fbcec2983095a9fcd42cda5c49b519`  
		Last Modified: Wed, 25 Aug 2021 19:37:01 GMT  
		Size: 1.1 KB (1069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:993faf624f9f41d879898713c9dd7875da6724079bf4f9d0a8af4c5a780dd6c0`  
		Last Modified: Wed, 25 Aug 2021 19:37:00 GMT  
		Size: 1.1 KB (1050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2df1fdf71a2973683c32f5a7cbf28584f357d292855672645e4fda8b1200e200`  
		Last Modified: Wed, 25 Aug 2021 19:37:01 GMT  
		Size: 1.1 KB (1068 bytes)  
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
$ docker pull nats-streaming@sha256:0fd0290d10cf965f1222f90fa114908b384cb8a816e81780143f32e89185a017
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.2114; amd64
	-	windows version 10.0.14393.4583; amd64

### `nats-streaming:0.22-windowsservercore` - windows version 10.0.17763.2114; amd64

```console
$ docker pull nats-streaming@sha256:d6ba04cfbedbf1ce9e219918c40dd6989e1d50a8e2398bb1d69fb19597056636
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2694026981 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:54951a15532bfdfb9b767cb2b92cb384b91b1c66f44a6cfb259769a168458b7f`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 05 Aug 2021 19:44:34 GMT
RUN Install update 1809-amd64
# Wed, 25 Aug 2021 13:46:35 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 25 Aug 2021 16:05:30 GMT
ENV NATS_DOCKERIZED=1
# Wed, 25 Aug 2021 19:31:01 GMT
ENV NATS_STREAMING_SERVER=0.22.1
# Wed, 25 Aug 2021 19:31:02 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.22.1/nats-streaming-server-v0.22.1-windows-amd64.zip
# Wed, 25 Aug 2021 19:31:03 GMT
ENV NATS_STREAMING_SERVER_SHASUM=4516852b493111b73ec06477be4a27e66f5abc9ca1ff4dd2b970232271611264
# Wed, 25 Aug 2021 19:31:55 GMT
RUN Set-PSDebug -Trace 2
# Wed, 25 Aug 2021 19:33:24 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 25 Aug 2021 19:33:25 GMT
EXPOSE 4222 8222
# Wed, 25 Aug 2021 19:33:26 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 25 Aug 2021 19:33:27 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c67ded6868b61d392a0c096f911563fd6bc0bc3ed4fe401d077b3718a1b0cdaf`  
		Size: 967.7 MB (967665054 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:985da5cbc0735e1c422e766af23125ba345f431cb337ea43ec32298d0bb8e4ea`  
		Last Modified: Wed, 25 Aug 2021 15:45:02 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3dbdd68a4b0c278695b3e1d401d7eddfb0f0e3aa1e28aed88eb700059648f8f`  
		Last Modified: Wed, 25 Aug 2021 16:11:02 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d02eff460789c6fa51a517221660dddad01c753689cf4d911deed4be925fdfa`  
		Last Modified: Wed, 25 Aug 2021 19:36:40 GMT  
		Size: 1.3 KB (1296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c67c923b3231b172039016dd78d64494840a068f83b7c2eb0610b3916e0f880d`  
		Last Modified: Wed, 25 Aug 2021 19:36:40 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13c73a6e9ff96bac535744e077e3966558cf33b742d3b384e6b77e72d96b4a49`  
		Last Modified: Wed, 25 Aug 2021 19:36:40 GMT  
		Size: 1.4 KB (1351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:652b4bfafc795b6a09e751ef642f31936038547b6223596beda9dc1bbd74f2df`  
		Last Modified: Wed, 25 Aug 2021 19:36:37 GMT  
		Size: 372.7 KB (372655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6d3118388d00fe0ce41388dbed69f505de317c0d9a6551664b34909e0308b85`  
		Last Modified: Wed, 25 Aug 2021 19:36:48 GMT  
		Size: 7.6 MB (7645717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35fd537c3fc591dceb1461535c52fc98243ac3b3fea45db58c6ebc492862440c`  
		Last Modified: Wed, 25 Aug 2021 19:36:37 GMT  
		Size: 1.3 KB (1311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21f9050479fb189fc4a85ae128bcc6a114f42e9139901390f4c6ef669c1ce49a`  
		Last Modified: Wed, 25 Aug 2021 19:36:37 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e587562615088e9b1f845a826539d4c81323caf3b84153496ac0f3c1c8afc45`  
		Last Modified: Wed, 25 Aug 2021 19:36:37 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.22-windowsservercore` - windows version 10.0.14393.4583; amd64

```console
$ docker pull nats-streaming@sha256:b122147602333b9a276aa52c700aae01f366dcad7b0d79a86009a7f8313bbb5a
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6278962413 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:624e3804e5c78766e9c54be1e5b1be3e39dd9aa56935b2944e21531a991f5377`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Sun, 01 Aug 2021 08:52:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 25 Aug 2021 13:59:32 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 25 Aug 2021 16:08:06 GMT
ENV NATS_DOCKERIZED=1
# Wed, 25 Aug 2021 19:33:53 GMT
ENV NATS_STREAMING_SERVER=0.22.1
# Wed, 25 Aug 2021 19:33:53 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.22.1/nats-streaming-server-v0.22.1-windows-amd64.zip
# Wed, 25 Aug 2021 19:33:54 GMT
ENV NATS_STREAMING_SERVER_SHASUM=4516852b493111b73ec06477be4a27e66f5abc9ca1ff4dd2b970232271611264
# Wed, 25 Aug 2021 19:34:35 GMT
RUN Set-PSDebug -Trace 2
# Wed, 25 Aug 2021 19:36:09 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 25 Aug 2021 19:36:10 GMT
EXPOSE 4222 8222
# Wed, 25 Aug 2021 19:36:10 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 25 Aug 2021 19:36:11 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c427f892fe74603ae09d4e49b25f8f7046f957054034dc9f462e0e88d7bffaa5`  
		Size: 2.2 GB (2200980134 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a869803fc3d8292f0fe1bc6ed35e1ceedbd7c797a1486767a55f88c6c28ed4c5`  
		Last Modified: Wed, 25 Aug 2021 15:45:25 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a745f96c10790ef3a2006dbd4c116eb2f1552fd3c4a38fca179a8160e9918ac1`  
		Last Modified: Wed, 25 Aug 2021 16:11:42 GMT  
		Size: 1.3 KB (1329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbb2b2f51b28100175c4c31970f69c26566bea4ec51d87a91555fe5091be241f`  
		Last Modified: Wed, 25 Aug 2021 19:37:17 GMT  
		Size: 1.3 KB (1322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d23161af967280f0d95595b25ca572083145ff8330ed8248c015bf100be1c838`  
		Last Modified: Wed, 25 Aug 2021 19:37:17 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11b49b5a10129016e785edeb8fba72f2d2a8658e8239af2b0fe530c3ae5a53c5`  
		Last Modified: Wed, 25 Aug 2021 19:37:16 GMT  
		Size: 1.3 KB (1314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b369c4a91f133df3608ec1e4cbb5ab7020ac16c0db6684465e735fc719da9a9`  
		Last Modified: Wed, 25 Aug 2021 19:37:14 GMT  
		Size: 336.8 KB (336786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc65df0e7918917488aea97873a4358dfad7b2914701e183c0865d4174c0dd62`  
		Last Modified: Wed, 25 Aug 2021 19:37:22 GMT  
		Size: 7.6 MB (7649022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:131ab6c361a3936d54c3e6d59a85f42d4171d9639f2c4feadb13b7eae8e9ff52`  
		Last Modified: Wed, 25 Aug 2021 19:37:14 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cabe016e1cfca773de7a8d1279fe766c82e6e6e91a9cff7c4725c06a13baa8c`  
		Last Modified: Wed, 25 Aug 2021 19:37:14 GMT  
		Size: 1.3 KB (1325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bf87ca03d1c93fa8e08d0c4be5fc32f8e091424df743e3aeab09d8dd776e5e6`  
		Last Modified: Wed, 25 Aug 2021 19:37:14 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.22-windowsservercore-1809`

```console
$ docker pull nats-streaming@sha256:6c691bb80388e286a736ac34253f62975b7da9bd039815b3fb7b82f3ebec4740
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2114; amd64

### `nats-streaming:0.22-windowsservercore-1809` - windows version 10.0.17763.2114; amd64

```console
$ docker pull nats-streaming@sha256:d6ba04cfbedbf1ce9e219918c40dd6989e1d50a8e2398bb1d69fb19597056636
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2694026981 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:54951a15532bfdfb9b767cb2b92cb384b91b1c66f44a6cfb259769a168458b7f`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 05 Aug 2021 19:44:34 GMT
RUN Install update 1809-amd64
# Wed, 25 Aug 2021 13:46:35 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 25 Aug 2021 16:05:30 GMT
ENV NATS_DOCKERIZED=1
# Wed, 25 Aug 2021 19:31:01 GMT
ENV NATS_STREAMING_SERVER=0.22.1
# Wed, 25 Aug 2021 19:31:02 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.22.1/nats-streaming-server-v0.22.1-windows-amd64.zip
# Wed, 25 Aug 2021 19:31:03 GMT
ENV NATS_STREAMING_SERVER_SHASUM=4516852b493111b73ec06477be4a27e66f5abc9ca1ff4dd2b970232271611264
# Wed, 25 Aug 2021 19:31:55 GMT
RUN Set-PSDebug -Trace 2
# Wed, 25 Aug 2021 19:33:24 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 25 Aug 2021 19:33:25 GMT
EXPOSE 4222 8222
# Wed, 25 Aug 2021 19:33:26 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 25 Aug 2021 19:33:27 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c67ded6868b61d392a0c096f911563fd6bc0bc3ed4fe401d077b3718a1b0cdaf`  
		Size: 967.7 MB (967665054 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:985da5cbc0735e1c422e766af23125ba345f431cb337ea43ec32298d0bb8e4ea`  
		Last Modified: Wed, 25 Aug 2021 15:45:02 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3dbdd68a4b0c278695b3e1d401d7eddfb0f0e3aa1e28aed88eb700059648f8f`  
		Last Modified: Wed, 25 Aug 2021 16:11:02 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d02eff460789c6fa51a517221660dddad01c753689cf4d911deed4be925fdfa`  
		Last Modified: Wed, 25 Aug 2021 19:36:40 GMT  
		Size: 1.3 KB (1296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c67c923b3231b172039016dd78d64494840a068f83b7c2eb0610b3916e0f880d`  
		Last Modified: Wed, 25 Aug 2021 19:36:40 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13c73a6e9ff96bac535744e077e3966558cf33b742d3b384e6b77e72d96b4a49`  
		Last Modified: Wed, 25 Aug 2021 19:36:40 GMT  
		Size: 1.4 KB (1351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:652b4bfafc795b6a09e751ef642f31936038547b6223596beda9dc1bbd74f2df`  
		Last Modified: Wed, 25 Aug 2021 19:36:37 GMT  
		Size: 372.7 KB (372655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6d3118388d00fe0ce41388dbed69f505de317c0d9a6551664b34909e0308b85`  
		Last Modified: Wed, 25 Aug 2021 19:36:48 GMT  
		Size: 7.6 MB (7645717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35fd537c3fc591dceb1461535c52fc98243ac3b3fea45db58c6ebc492862440c`  
		Last Modified: Wed, 25 Aug 2021 19:36:37 GMT  
		Size: 1.3 KB (1311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21f9050479fb189fc4a85ae128bcc6a114f42e9139901390f4c6ef669c1ce49a`  
		Last Modified: Wed, 25 Aug 2021 19:36:37 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e587562615088e9b1f845a826539d4c81323caf3b84153496ac0f3c1c8afc45`  
		Last Modified: Wed, 25 Aug 2021 19:36:37 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.22-windowsservercore-ltsc2016`

```console
$ docker pull nats-streaming@sha256:8004e2870ca327f887f2e30cc0fa4d36d010512baf99a2ba286275ea0405144c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.14393.4583; amd64

### `nats-streaming:0.22-windowsservercore-ltsc2016` - windows version 10.0.14393.4583; amd64

```console
$ docker pull nats-streaming@sha256:b122147602333b9a276aa52c700aae01f366dcad7b0d79a86009a7f8313bbb5a
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6278962413 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:624e3804e5c78766e9c54be1e5b1be3e39dd9aa56935b2944e21531a991f5377`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Sun, 01 Aug 2021 08:52:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 25 Aug 2021 13:59:32 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 25 Aug 2021 16:08:06 GMT
ENV NATS_DOCKERIZED=1
# Wed, 25 Aug 2021 19:33:53 GMT
ENV NATS_STREAMING_SERVER=0.22.1
# Wed, 25 Aug 2021 19:33:53 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.22.1/nats-streaming-server-v0.22.1-windows-amd64.zip
# Wed, 25 Aug 2021 19:33:54 GMT
ENV NATS_STREAMING_SERVER_SHASUM=4516852b493111b73ec06477be4a27e66f5abc9ca1ff4dd2b970232271611264
# Wed, 25 Aug 2021 19:34:35 GMT
RUN Set-PSDebug -Trace 2
# Wed, 25 Aug 2021 19:36:09 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 25 Aug 2021 19:36:10 GMT
EXPOSE 4222 8222
# Wed, 25 Aug 2021 19:36:10 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 25 Aug 2021 19:36:11 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c427f892fe74603ae09d4e49b25f8f7046f957054034dc9f462e0e88d7bffaa5`  
		Size: 2.2 GB (2200980134 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a869803fc3d8292f0fe1bc6ed35e1ceedbd7c797a1486767a55f88c6c28ed4c5`  
		Last Modified: Wed, 25 Aug 2021 15:45:25 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a745f96c10790ef3a2006dbd4c116eb2f1552fd3c4a38fca179a8160e9918ac1`  
		Last Modified: Wed, 25 Aug 2021 16:11:42 GMT  
		Size: 1.3 KB (1329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbb2b2f51b28100175c4c31970f69c26566bea4ec51d87a91555fe5091be241f`  
		Last Modified: Wed, 25 Aug 2021 19:37:17 GMT  
		Size: 1.3 KB (1322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d23161af967280f0d95595b25ca572083145ff8330ed8248c015bf100be1c838`  
		Last Modified: Wed, 25 Aug 2021 19:37:17 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11b49b5a10129016e785edeb8fba72f2d2a8658e8239af2b0fe530c3ae5a53c5`  
		Last Modified: Wed, 25 Aug 2021 19:37:16 GMT  
		Size: 1.3 KB (1314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b369c4a91f133df3608ec1e4cbb5ab7020ac16c0db6684465e735fc719da9a9`  
		Last Modified: Wed, 25 Aug 2021 19:37:14 GMT  
		Size: 336.8 KB (336786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc65df0e7918917488aea97873a4358dfad7b2914701e183c0865d4174c0dd62`  
		Last Modified: Wed, 25 Aug 2021 19:37:22 GMT  
		Size: 7.6 MB (7649022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:131ab6c361a3936d54c3e6d59a85f42d4171d9639f2c4feadb13b7eae8e9ff52`  
		Last Modified: Wed, 25 Aug 2021 19:37:14 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cabe016e1cfca773de7a8d1279fe766c82e6e6e91a9cff7c4725c06a13baa8c`  
		Last Modified: Wed, 25 Aug 2021 19:37:14 GMT  
		Size: 1.3 KB (1325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bf87ca03d1c93fa8e08d0c4be5fc32f8e091424df743e3aeab09d8dd776e5e6`  
		Last Modified: Wed, 25 Aug 2021 19:37:14 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.22.1`

```console
$ docker pull nats-streaming@sha256:f0716868aa216d2a8803f3580bd512fc699da2d7a6af8ff6c5c857d47192e6e7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.2114; amd64

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

### `nats-streaming:0.22.1` - windows version 10.0.17763.2114; amd64

```console
$ docker pull nats-streaming@sha256:6cf5f132f44fee4ec7d112868c7525aac42e5eef00cd0298e1efdffcb1df5251
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.0 MB (110038648 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7863a1802021516178bb5e20547b7e410590d3ad269287d3d99fd163070dc55b`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 05 Aug 2021 19:15:20 GMT
RUN Apply image 1809-amd64
# Wed, 25 Aug 2021 16:07:56 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 25 Aug 2021 19:33:43 GMT
RUN cmd /S /C #(nop) COPY file:9670e5d1fe5a71e47c78fde01235a0bcbcafcfdeeacf96a7669f6e49343fb03b in C:\nats-streaming-server.exe 
# Wed, 25 Aug 2021 19:33:45 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 25 Aug 2021 19:33:45 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 25 Aug 2021 19:33:46 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:bc8517709e9cfff223cb034ff5be8fcbfa5409de286cdac9ae1b8878ebea6b84`  
		Size: 102.7 MB (102741177 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ae8616c17f5cca409a4b1289387e37dc532657ba2b52bb60713ff621acccd506`  
		Last Modified: Wed, 25 Aug 2021 16:11:20 GMT  
		Size: 1.0 KB (1022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa124ed4fe9f29ce6e3db339e67e84f8667fe9ad034f27a42d6554c473e49de1`  
		Last Modified: Wed, 25 Aug 2021 19:37:03 GMT  
		Size: 7.3 MB (7293262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e47ccb646b6561c33cebea3e0f6ffb755fbcec2983095a9fcd42cda5c49b519`  
		Last Modified: Wed, 25 Aug 2021 19:37:01 GMT  
		Size: 1.1 KB (1069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:993faf624f9f41d879898713c9dd7875da6724079bf4f9d0a8af4c5a780dd6c0`  
		Last Modified: Wed, 25 Aug 2021 19:37:00 GMT  
		Size: 1.1 KB (1050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2df1fdf71a2973683c32f5a7cbf28584f357d292855672645e4fda8b1200e200`  
		Last Modified: Wed, 25 Aug 2021 19:37:01 GMT  
		Size: 1.1 KB (1068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.22.1-alpine`

```console
$ docker pull nats-streaming@sha256:025dd4f7090b799587d1ba45d887a67d44f9d12ad0b7c474a8e72c3886150382
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.22.1-alpine` - linux; amd64

```console
$ docker pull nats-streaming@sha256:490adf058de78b1fe4f0d33864796f8a112c3b784c6e90ba22e45153fe74d900
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.3 MB (10270658 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fabf0e12d64e19686c51b041dd0cc13952c874c78e6f6c5e113a95dd59c4ea55`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 27 Aug 2021 20:46:27 GMT
ENV NATS_STREAMING_SERVER=0.22.1
# Fri, 27 Aug 2021 20:46:31 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='581698d248a19ecae64e4048d153bc1021744a3da6284680a339f9f82a53a9cf' ;; 		armhf) natsArch='arm6'; sha256='438a89221bb0608e40d21e73ca27a4b70b8560730726942c0ade94a6b6013d6f' ;; 		armv7) natsArch='arm7'; sha256='4164baadd201d1374f7654d3e54a24d81ceb87a385867e31a82c1d1a69e3b1ae' ;; 		x86_64) natsArch='amd64'; sha256='f29e87ac9ff998c928aa8ebc8cf0c4d04d34a3d95b9900d92fd7dafab2bec8cc' ;; 		x86) natsArch='386'; sha256='0ca68e57babb8901d7afeb7569042730904887e718ddf860ef3ee54278753505' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 27 Aug 2021 20:46:31 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Fri, 27 Aug 2021 20:46:32 GMT
EXPOSE 4222 8222
# Fri, 27 Aug 2021 20:46:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 Aug 2021 20:46:33 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8848530ed3e01ccf52dafe72a2e2c14ec4f6ec52809524bd71c33cbe193e5ad3`  
		Last Modified: Fri, 27 Aug 2021 20:47:18 GMT  
		Size: 7.5 MB (7455792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0a13cfe7f8352b89abb0a8ea81910d679c36c4a90d6d88d7f8a9059471b2e31`  
		Last Modified: Fri, 27 Aug 2021 20:47:16 GMT  
		Size: 420.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.22.1-alpine` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:9cda74ceed2f45daa20c52af4aa059d5af71f373753072e64d1223e5de592e64
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.6 MB (9561001 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f85120fadd96bf6e11b7fa82dd813c6d56b9aff9cb577d22dc8cbaaae6ac263`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 27 Aug 2021 17:49:29 GMT
ADD file:1c1c4520d49cb6e8f795f3b953d1ed3c3c77868b98b53a455169c254fcec5acd in / 
# Fri, 27 Aug 2021 17:49:30 GMT
CMD ["/bin/sh"]
# Fri, 27 Aug 2021 19:24:22 GMT
ENV NATS_STREAMING_SERVER=0.22.1
# Fri, 27 Aug 2021 19:24:28 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='581698d248a19ecae64e4048d153bc1021744a3da6284680a339f9f82a53a9cf' ;; 		armhf) natsArch='arm6'; sha256='438a89221bb0608e40d21e73ca27a4b70b8560730726942c0ade94a6b6013d6f' ;; 		armv7) natsArch='arm7'; sha256='4164baadd201d1374f7654d3e54a24d81ceb87a385867e31a82c1d1a69e3b1ae' ;; 		x86_64) natsArch='amd64'; sha256='f29e87ac9ff998c928aa8ebc8cf0c4d04d34a3d95b9900d92fd7dafab2bec8cc' ;; 		x86) natsArch='386'; sha256='0ca68e57babb8901d7afeb7569042730904887e718ddf860ef3ee54278753505' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 27 Aug 2021 19:24:29 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Fri, 27 Aug 2021 19:24:29 GMT
EXPOSE 4222 8222
# Fri, 27 Aug 2021 19:24:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 Aug 2021 19:24:30 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:2e78c0f86ba9a1fed30df20cb48c9cc73e9626399f12749d36b892ff99c0ecf5`  
		Last Modified: Fri, 27 Aug 2021 17:50:55 GMT  
		Size: 2.6 MB (2627447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:320a6a97adac4a737e1997906fcc9d6922c1ae39980382314b88be30f8b64ea3`  
		Last Modified: Fri, 27 Aug 2021 19:26:12 GMT  
		Size: 6.9 MB (6933133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92e6007c46c9095e062e9214fe2c0618a2b2fe8642c7f6162972036163e330ad`  
		Last Modified: Fri, 27 Aug 2021 19:26:08 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.22.1-alpine` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:7970395d00490fad62f2a51288db47d251cab92ec7634bef6de42343f8e8eedc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.4 MB (9351328 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e19086c92b47964c105a8ed130ff7219833adab1ca8e211c1ad0b0a049866252`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 06 Aug 2021 17:57:32 GMT
ADD file:3a35ff3ac0d80289d419a4d6d8319610c38e1936d296addafb9aaf506946230f in / 
# Fri, 06 Aug 2021 17:57:32 GMT
CMD ["/bin/sh"]
# Fri, 06 Aug 2021 20:29:42 GMT
ENV NATS_STREAMING_SERVER=0.22.1
# Fri, 06 Aug 2021 20:29:48 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='581698d248a19ecae64e4048d153bc1021744a3da6284680a339f9f82a53a9cf' ;; 		armhf) natsArch='arm6'; sha256='438a89221bb0608e40d21e73ca27a4b70b8560730726942c0ade94a6b6013d6f' ;; 		armv7) natsArch='arm7'; sha256='4164baadd201d1374f7654d3e54a24d81ceb87a385867e31a82c1d1a69e3b1ae' ;; 		x86_64) natsArch='amd64'; sha256='f29e87ac9ff998c928aa8ebc8cf0c4d04d34a3d95b9900d92fd7dafab2bec8cc' ;; 		x86) natsArch='386'; sha256='0ca68e57babb8901d7afeb7569042730904887e718ddf860ef3ee54278753505' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 06 Aug 2021 20:29:48 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Fri, 06 Aug 2021 20:29:49 GMT
EXPOSE 4222 8222
# Fri, 06 Aug 2021 20:29:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 06 Aug 2021 20:29:50 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:4ee0caa23b369b04827640a4be298bf4ff7bacd030c77e915f5d7fb8f987594a`  
		Last Modified: Fri, 06 Aug 2021 17:58:57 GMT  
		Size: 2.4 MB (2429359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e14712e6c4fbdd823f35d0df7aa1345088ce3d89727133dcef4adb1105ecb5f`  
		Last Modified: Fri, 06 Aug 2021 20:31:34 GMT  
		Size: 6.9 MB (6921548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e18c45098374f86d0784e7840a2c0fd15ce636edfee6d3ebc23432fd0cc47be5`  
		Last Modified: Fri, 06 Aug 2021 20:31:30 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.22.1-alpine` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:366b541434718f0d0bd3e6fffb5dd27db81774c771dc0ecb69c00819fb1b3997
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.5 MB (9542913 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:244415bb00005ee5391d41fc5b03c3477bcf4f2c70a6d081a65dc46b732956c4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Fri, 27 Aug 2021 20:20:38 GMT
ENV NATS_STREAMING_SERVER=0.22.1
# Fri, 27 Aug 2021 20:20:41 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='581698d248a19ecae64e4048d153bc1021744a3da6284680a339f9f82a53a9cf' ;; 		armhf) natsArch='arm6'; sha256='438a89221bb0608e40d21e73ca27a4b70b8560730726942c0ade94a6b6013d6f' ;; 		armv7) natsArch='arm7'; sha256='4164baadd201d1374f7654d3e54a24d81ceb87a385867e31a82c1d1a69e3b1ae' ;; 		x86_64) natsArch='amd64'; sha256='f29e87ac9ff998c928aa8ebc8cf0c4d04d34a3d95b9900d92fd7dafab2bec8cc' ;; 		x86) natsArch='386'; sha256='0ca68e57babb8901d7afeb7569042730904887e718ddf860ef3ee54278753505' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 27 Aug 2021 20:20:41 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Fri, 27 Aug 2021 20:20:41 GMT
EXPOSE 4222 8222
# Fri, 27 Aug 2021 20:20:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 Aug 2021 20:20:41 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:552d1f2373af9bfe12033568ebbfb0ccbb0de11279f9a415a29207e264d7f4d9`  
		Last Modified: Fri, 27 Aug 2021 17:40:18 GMT  
		Size: 2.7 MB (2711827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:069785721c5e4cdee5b76770ae83cf97b47105b106c53b06922f570ba743dadb`  
		Last Modified: Fri, 27 Aug 2021 20:21:32 GMT  
		Size: 6.8 MB (6830666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df70eb7a18c78f5cbb612b797fe94d277338f4bd8e5dfd47cba3d97d57e0e352`  
		Last Modified: Fri, 27 Aug 2021 20:21:31 GMT  
		Size: 420.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.22.1-alpine3.14`

```console
$ docker pull nats-streaming@sha256:025dd4f7090b799587d1ba45d887a67d44f9d12ad0b7c474a8e72c3886150382
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.22.1-alpine3.14` - linux; amd64

```console
$ docker pull nats-streaming@sha256:490adf058de78b1fe4f0d33864796f8a112c3b784c6e90ba22e45153fe74d900
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.3 MB (10270658 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fabf0e12d64e19686c51b041dd0cc13952c874c78e6f6c5e113a95dd59c4ea55`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 27 Aug 2021 20:46:27 GMT
ENV NATS_STREAMING_SERVER=0.22.1
# Fri, 27 Aug 2021 20:46:31 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='581698d248a19ecae64e4048d153bc1021744a3da6284680a339f9f82a53a9cf' ;; 		armhf) natsArch='arm6'; sha256='438a89221bb0608e40d21e73ca27a4b70b8560730726942c0ade94a6b6013d6f' ;; 		armv7) natsArch='arm7'; sha256='4164baadd201d1374f7654d3e54a24d81ceb87a385867e31a82c1d1a69e3b1ae' ;; 		x86_64) natsArch='amd64'; sha256='f29e87ac9ff998c928aa8ebc8cf0c4d04d34a3d95b9900d92fd7dafab2bec8cc' ;; 		x86) natsArch='386'; sha256='0ca68e57babb8901d7afeb7569042730904887e718ddf860ef3ee54278753505' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 27 Aug 2021 20:46:31 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Fri, 27 Aug 2021 20:46:32 GMT
EXPOSE 4222 8222
# Fri, 27 Aug 2021 20:46:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 Aug 2021 20:46:33 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8848530ed3e01ccf52dafe72a2e2c14ec4f6ec52809524bd71c33cbe193e5ad3`  
		Last Modified: Fri, 27 Aug 2021 20:47:18 GMT  
		Size: 7.5 MB (7455792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0a13cfe7f8352b89abb0a8ea81910d679c36c4a90d6d88d7f8a9059471b2e31`  
		Last Modified: Fri, 27 Aug 2021 20:47:16 GMT  
		Size: 420.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.22.1-alpine3.14` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:9cda74ceed2f45daa20c52af4aa059d5af71f373753072e64d1223e5de592e64
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.6 MB (9561001 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f85120fadd96bf6e11b7fa82dd813c6d56b9aff9cb577d22dc8cbaaae6ac263`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 27 Aug 2021 17:49:29 GMT
ADD file:1c1c4520d49cb6e8f795f3b953d1ed3c3c77868b98b53a455169c254fcec5acd in / 
# Fri, 27 Aug 2021 17:49:30 GMT
CMD ["/bin/sh"]
# Fri, 27 Aug 2021 19:24:22 GMT
ENV NATS_STREAMING_SERVER=0.22.1
# Fri, 27 Aug 2021 19:24:28 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='581698d248a19ecae64e4048d153bc1021744a3da6284680a339f9f82a53a9cf' ;; 		armhf) natsArch='arm6'; sha256='438a89221bb0608e40d21e73ca27a4b70b8560730726942c0ade94a6b6013d6f' ;; 		armv7) natsArch='arm7'; sha256='4164baadd201d1374f7654d3e54a24d81ceb87a385867e31a82c1d1a69e3b1ae' ;; 		x86_64) natsArch='amd64'; sha256='f29e87ac9ff998c928aa8ebc8cf0c4d04d34a3d95b9900d92fd7dafab2bec8cc' ;; 		x86) natsArch='386'; sha256='0ca68e57babb8901d7afeb7569042730904887e718ddf860ef3ee54278753505' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 27 Aug 2021 19:24:29 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Fri, 27 Aug 2021 19:24:29 GMT
EXPOSE 4222 8222
# Fri, 27 Aug 2021 19:24:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 Aug 2021 19:24:30 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:2e78c0f86ba9a1fed30df20cb48c9cc73e9626399f12749d36b892ff99c0ecf5`  
		Last Modified: Fri, 27 Aug 2021 17:50:55 GMT  
		Size: 2.6 MB (2627447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:320a6a97adac4a737e1997906fcc9d6922c1ae39980382314b88be30f8b64ea3`  
		Last Modified: Fri, 27 Aug 2021 19:26:12 GMT  
		Size: 6.9 MB (6933133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92e6007c46c9095e062e9214fe2c0618a2b2fe8642c7f6162972036163e330ad`  
		Last Modified: Fri, 27 Aug 2021 19:26:08 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.22.1-alpine3.14` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:7970395d00490fad62f2a51288db47d251cab92ec7634bef6de42343f8e8eedc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.4 MB (9351328 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e19086c92b47964c105a8ed130ff7219833adab1ca8e211c1ad0b0a049866252`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 06 Aug 2021 17:57:32 GMT
ADD file:3a35ff3ac0d80289d419a4d6d8319610c38e1936d296addafb9aaf506946230f in / 
# Fri, 06 Aug 2021 17:57:32 GMT
CMD ["/bin/sh"]
# Fri, 06 Aug 2021 20:29:42 GMT
ENV NATS_STREAMING_SERVER=0.22.1
# Fri, 06 Aug 2021 20:29:48 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='581698d248a19ecae64e4048d153bc1021744a3da6284680a339f9f82a53a9cf' ;; 		armhf) natsArch='arm6'; sha256='438a89221bb0608e40d21e73ca27a4b70b8560730726942c0ade94a6b6013d6f' ;; 		armv7) natsArch='arm7'; sha256='4164baadd201d1374f7654d3e54a24d81ceb87a385867e31a82c1d1a69e3b1ae' ;; 		x86_64) natsArch='amd64'; sha256='f29e87ac9ff998c928aa8ebc8cf0c4d04d34a3d95b9900d92fd7dafab2bec8cc' ;; 		x86) natsArch='386'; sha256='0ca68e57babb8901d7afeb7569042730904887e718ddf860ef3ee54278753505' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 06 Aug 2021 20:29:48 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Fri, 06 Aug 2021 20:29:49 GMT
EXPOSE 4222 8222
# Fri, 06 Aug 2021 20:29:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 06 Aug 2021 20:29:50 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:4ee0caa23b369b04827640a4be298bf4ff7bacd030c77e915f5d7fb8f987594a`  
		Last Modified: Fri, 06 Aug 2021 17:58:57 GMT  
		Size: 2.4 MB (2429359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e14712e6c4fbdd823f35d0df7aa1345088ce3d89727133dcef4adb1105ecb5f`  
		Last Modified: Fri, 06 Aug 2021 20:31:34 GMT  
		Size: 6.9 MB (6921548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e18c45098374f86d0784e7840a2c0fd15ce636edfee6d3ebc23432fd0cc47be5`  
		Last Modified: Fri, 06 Aug 2021 20:31:30 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.22.1-alpine3.14` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:366b541434718f0d0bd3e6fffb5dd27db81774c771dc0ecb69c00819fb1b3997
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.5 MB (9542913 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:244415bb00005ee5391d41fc5b03c3477bcf4f2c70a6d081a65dc46b732956c4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Fri, 27 Aug 2021 20:20:38 GMT
ENV NATS_STREAMING_SERVER=0.22.1
# Fri, 27 Aug 2021 20:20:41 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='581698d248a19ecae64e4048d153bc1021744a3da6284680a339f9f82a53a9cf' ;; 		armhf) natsArch='arm6'; sha256='438a89221bb0608e40d21e73ca27a4b70b8560730726942c0ade94a6b6013d6f' ;; 		armv7) natsArch='arm7'; sha256='4164baadd201d1374f7654d3e54a24d81ceb87a385867e31a82c1d1a69e3b1ae' ;; 		x86_64) natsArch='amd64'; sha256='f29e87ac9ff998c928aa8ebc8cf0c4d04d34a3d95b9900d92fd7dafab2bec8cc' ;; 		x86) natsArch='386'; sha256='0ca68e57babb8901d7afeb7569042730904887e718ddf860ef3ee54278753505' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 27 Aug 2021 20:20:41 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Fri, 27 Aug 2021 20:20:41 GMT
EXPOSE 4222 8222
# Fri, 27 Aug 2021 20:20:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 Aug 2021 20:20:41 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:552d1f2373af9bfe12033568ebbfb0ccbb0de11279f9a415a29207e264d7f4d9`  
		Last Modified: Fri, 27 Aug 2021 17:40:18 GMT  
		Size: 2.7 MB (2711827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:069785721c5e4cdee5b76770ae83cf97b47105b106c53b06922f570ba743dadb`  
		Last Modified: Fri, 27 Aug 2021 20:21:32 GMT  
		Size: 6.8 MB (6830666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df70eb7a18c78f5cbb612b797fe94d277338f4bd8e5dfd47cba3d97d57e0e352`  
		Last Modified: Fri, 27 Aug 2021 20:21:31 GMT  
		Size: 420.0 B  
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
$ docker pull nats-streaming@sha256:d86bdcb9e19d16a21ea8eb07693268eab508df92a0df40021ca3b296412ba430
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2114; amd64

### `nats-streaming:0.22.1-nanoserver` - windows version 10.0.17763.2114; amd64

```console
$ docker pull nats-streaming@sha256:6cf5f132f44fee4ec7d112868c7525aac42e5eef00cd0298e1efdffcb1df5251
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.0 MB (110038648 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7863a1802021516178bb5e20547b7e410590d3ad269287d3d99fd163070dc55b`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 05 Aug 2021 19:15:20 GMT
RUN Apply image 1809-amd64
# Wed, 25 Aug 2021 16:07:56 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 25 Aug 2021 19:33:43 GMT
RUN cmd /S /C #(nop) COPY file:9670e5d1fe5a71e47c78fde01235a0bcbcafcfdeeacf96a7669f6e49343fb03b in C:\nats-streaming-server.exe 
# Wed, 25 Aug 2021 19:33:45 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 25 Aug 2021 19:33:45 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 25 Aug 2021 19:33:46 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:bc8517709e9cfff223cb034ff5be8fcbfa5409de286cdac9ae1b8878ebea6b84`  
		Size: 102.7 MB (102741177 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ae8616c17f5cca409a4b1289387e37dc532657ba2b52bb60713ff621acccd506`  
		Last Modified: Wed, 25 Aug 2021 16:11:20 GMT  
		Size: 1.0 KB (1022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa124ed4fe9f29ce6e3db339e67e84f8667fe9ad034f27a42d6554c473e49de1`  
		Last Modified: Wed, 25 Aug 2021 19:37:03 GMT  
		Size: 7.3 MB (7293262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e47ccb646b6561c33cebea3e0f6ffb755fbcec2983095a9fcd42cda5c49b519`  
		Last Modified: Wed, 25 Aug 2021 19:37:01 GMT  
		Size: 1.1 KB (1069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:993faf624f9f41d879898713c9dd7875da6724079bf4f9d0a8af4c5a780dd6c0`  
		Last Modified: Wed, 25 Aug 2021 19:37:00 GMT  
		Size: 1.1 KB (1050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2df1fdf71a2973683c32f5a7cbf28584f357d292855672645e4fda8b1200e200`  
		Last Modified: Wed, 25 Aug 2021 19:37:01 GMT  
		Size: 1.1 KB (1068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.22.1-nanoserver-1809`

```console
$ docker pull nats-streaming@sha256:d86bdcb9e19d16a21ea8eb07693268eab508df92a0df40021ca3b296412ba430
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2114; amd64

### `nats-streaming:0.22.1-nanoserver-1809` - windows version 10.0.17763.2114; amd64

```console
$ docker pull nats-streaming@sha256:6cf5f132f44fee4ec7d112868c7525aac42e5eef00cd0298e1efdffcb1df5251
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.0 MB (110038648 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7863a1802021516178bb5e20547b7e410590d3ad269287d3d99fd163070dc55b`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 05 Aug 2021 19:15:20 GMT
RUN Apply image 1809-amd64
# Wed, 25 Aug 2021 16:07:56 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 25 Aug 2021 19:33:43 GMT
RUN cmd /S /C #(nop) COPY file:9670e5d1fe5a71e47c78fde01235a0bcbcafcfdeeacf96a7669f6e49343fb03b in C:\nats-streaming-server.exe 
# Wed, 25 Aug 2021 19:33:45 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 25 Aug 2021 19:33:45 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 25 Aug 2021 19:33:46 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:bc8517709e9cfff223cb034ff5be8fcbfa5409de286cdac9ae1b8878ebea6b84`  
		Size: 102.7 MB (102741177 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ae8616c17f5cca409a4b1289387e37dc532657ba2b52bb60713ff621acccd506`  
		Last Modified: Wed, 25 Aug 2021 16:11:20 GMT  
		Size: 1.0 KB (1022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa124ed4fe9f29ce6e3db339e67e84f8667fe9ad034f27a42d6554c473e49de1`  
		Last Modified: Wed, 25 Aug 2021 19:37:03 GMT  
		Size: 7.3 MB (7293262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e47ccb646b6561c33cebea3e0f6ffb755fbcec2983095a9fcd42cda5c49b519`  
		Last Modified: Wed, 25 Aug 2021 19:37:01 GMT  
		Size: 1.1 KB (1069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:993faf624f9f41d879898713c9dd7875da6724079bf4f9d0a8af4c5a780dd6c0`  
		Last Modified: Wed, 25 Aug 2021 19:37:00 GMT  
		Size: 1.1 KB (1050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2df1fdf71a2973683c32f5a7cbf28584f357d292855672645e4fda8b1200e200`  
		Last Modified: Wed, 25 Aug 2021 19:37:01 GMT  
		Size: 1.1 KB (1068 bytes)  
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
$ docker pull nats-streaming@sha256:0fd0290d10cf965f1222f90fa114908b384cb8a816e81780143f32e89185a017
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.2114; amd64
	-	windows version 10.0.14393.4583; amd64

### `nats-streaming:0.22.1-windowsservercore` - windows version 10.0.17763.2114; amd64

```console
$ docker pull nats-streaming@sha256:d6ba04cfbedbf1ce9e219918c40dd6989e1d50a8e2398bb1d69fb19597056636
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2694026981 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:54951a15532bfdfb9b767cb2b92cb384b91b1c66f44a6cfb259769a168458b7f`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 05 Aug 2021 19:44:34 GMT
RUN Install update 1809-amd64
# Wed, 25 Aug 2021 13:46:35 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 25 Aug 2021 16:05:30 GMT
ENV NATS_DOCKERIZED=1
# Wed, 25 Aug 2021 19:31:01 GMT
ENV NATS_STREAMING_SERVER=0.22.1
# Wed, 25 Aug 2021 19:31:02 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.22.1/nats-streaming-server-v0.22.1-windows-amd64.zip
# Wed, 25 Aug 2021 19:31:03 GMT
ENV NATS_STREAMING_SERVER_SHASUM=4516852b493111b73ec06477be4a27e66f5abc9ca1ff4dd2b970232271611264
# Wed, 25 Aug 2021 19:31:55 GMT
RUN Set-PSDebug -Trace 2
# Wed, 25 Aug 2021 19:33:24 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 25 Aug 2021 19:33:25 GMT
EXPOSE 4222 8222
# Wed, 25 Aug 2021 19:33:26 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 25 Aug 2021 19:33:27 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c67ded6868b61d392a0c096f911563fd6bc0bc3ed4fe401d077b3718a1b0cdaf`  
		Size: 967.7 MB (967665054 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:985da5cbc0735e1c422e766af23125ba345f431cb337ea43ec32298d0bb8e4ea`  
		Last Modified: Wed, 25 Aug 2021 15:45:02 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3dbdd68a4b0c278695b3e1d401d7eddfb0f0e3aa1e28aed88eb700059648f8f`  
		Last Modified: Wed, 25 Aug 2021 16:11:02 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d02eff460789c6fa51a517221660dddad01c753689cf4d911deed4be925fdfa`  
		Last Modified: Wed, 25 Aug 2021 19:36:40 GMT  
		Size: 1.3 KB (1296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c67c923b3231b172039016dd78d64494840a068f83b7c2eb0610b3916e0f880d`  
		Last Modified: Wed, 25 Aug 2021 19:36:40 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13c73a6e9ff96bac535744e077e3966558cf33b742d3b384e6b77e72d96b4a49`  
		Last Modified: Wed, 25 Aug 2021 19:36:40 GMT  
		Size: 1.4 KB (1351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:652b4bfafc795b6a09e751ef642f31936038547b6223596beda9dc1bbd74f2df`  
		Last Modified: Wed, 25 Aug 2021 19:36:37 GMT  
		Size: 372.7 KB (372655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6d3118388d00fe0ce41388dbed69f505de317c0d9a6551664b34909e0308b85`  
		Last Modified: Wed, 25 Aug 2021 19:36:48 GMT  
		Size: 7.6 MB (7645717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35fd537c3fc591dceb1461535c52fc98243ac3b3fea45db58c6ebc492862440c`  
		Last Modified: Wed, 25 Aug 2021 19:36:37 GMT  
		Size: 1.3 KB (1311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21f9050479fb189fc4a85ae128bcc6a114f42e9139901390f4c6ef669c1ce49a`  
		Last Modified: Wed, 25 Aug 2021 19:36:37 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e587562615088e9b1f845a826539d4c81323caf3b84153496ac0f3c1c8afc45`  
		Last Modified: Wed, 25 Aug 2021 19:36:37 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.22.1-windowsservercore` - windows version 10.0.14393.4583; amd64

```console
$ docker pull nats-streaming@sha256:b122147602333b9a276aa52c700aae01f366dcad7b0d79a86009a7f8313bbb5a
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6278962413 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:624e3804e5c78766e9c54be1e5b1be3e39dd9aa56935b2944e21531a991f5377`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Sun, 01 Aug 2021 08:52:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 25 Aug 2021 13:59:32 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 25 Aug 2021 16:08:06 GMT
ENV NATS_DOCKERIZED=1
# Wed, 25 Aug 2021 19:33:53 GMT
ENV NATS_STREAMING_SERVER=0.22.1
# Wed, 25 Aug 2021 19:33:53 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.22.1/nats-streaming-server-v0.22.1-windows-amd64.zip
# Wed, 25 Aug 2021 19:33:54 GMT
ENV NATS_STREAMING_SERVER_SHASUM=4516852b493111b73ec06477be4a27e66f5abc9ca1ff4dd2b970232271611264
# Wed, 25 Aug 2021 19:34:35 GMT
RUN Set-PSDebug -Trace 2
# Wed, 25 Aug 2021 19:36:09 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 25 Aug 2021 19:36:10 GMT
EXPOSE 4222 8222
# Wed, 25 Aug 2021 19:36:10 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 25 Aug 2021 19:36:11 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c427f892fe74603ae09d4e49b25f8f7046f957054034dc9f462e0e88d7bffaa5`  
		Size: 2.2 GB (2200980134 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a869803fc3d8292f0fe1bc6ed35e1ceedbd7c797a1486767a55f88c6c28ed4c5`  
		Last Modified: Wed, 25 Aug 2021 15:45:25 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a745f96c10790ef3a2006dbd4c116eb2f1552fd3c4a38fca179a8160e9918ac1`  
		Last Modified: Wed, 25 Aug 2021 16:11:42 GMT  
		Size: 1.3 KB (1329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbb2b2f51b28100175c4c31970f69c26566bea4ec51d87a91555fe5091be241f`  
		Last Modified: Wed, 25 Aug 2021 19:37:17 GMT  
		Size: 1.3 KB (1322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d23161af967280f0d95595b25ca572083145ff8330ed8248c015bf100be1c838`  
		Last Modified: Wed, 25 Aug 2021 19:37:17 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11b49b5a10129016e785edeb8fba72f2d2a8658e8239af2b0fe530c3ae5a53c5`  
		Last Modified: Wed, 25 Aug 2021 19:37:16 GMT  
		Size: 1.3 KB (1314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b369c4a91f133df3608ec1e4cbb5ab7020ac16c0db6684465e735fc719da9a9`  
		Last Modified: Wed, 25 Aug 2021 19:37:14 GMT  
		Size: 336.8 KB (336786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc65df0e7918917488aea97873a4358dfad7b2914701e183c0865d4174c0dd62`  
		Last Modified: Wed, 25 Aug 2021 19:37:22 GMT  
		Size: 7.6 MB (7649022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:131ab6c361a3936d54c3e6d59a85f42d4171d9639f2c4feadb13b7eae8e9ff52`  
		Last Modified: Wed, 25 Aug 2021 19:37:14 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cabe016e1cfca773de7a8d1279fe766c82e6e6e91a9cff7c4725c06a13baa8c`  
		Last Modified: Wed, 25 Aug 2021 19:37:14 GMT  
		Size: 1.3 KB (1325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bf87ca03d1c93fa8e08d0c4be5fc32f8e091424df743e3aeab09d8dd776e5e6`  
		Last Modified: Wed, 25 Aug 2021 19:37:14 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.22.1-windowsservercore-1809`

```console
$ docker pull nats-streaming@sha256:6c691bb80388e286a736ac34253f62975b7da9bd039815b3fb7b82f3ebec4740
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2114; amd64

### `nats-streaming:0.22.1-windowsservercore-1809` - windows version 10.0.17763.2114; amd64

```console
$ docker pull nats-streaming@sha256:d6ba04cfbedbf1ce9e219918c40dd6989e1d50a8e2398bb1d69fb19597056636
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2694026981 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:54951a15532bfdfb9b767cb2b92cb384b91b1c66f44a6cfb259769a168458b7f`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 05 Aug 2021 19:44:34 GMT
RUN Install update 1809-amd64
# Wed, 25 Aug 2021 13:46:35 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 25 Aug 2021 16:05:30 GMT
ENV NATS_DOCKERIZED=1
# Wed, 25 Aug 2021 19:31:01 GMT
ENV NATS_STREAMING_SERVER=0.22.1
# Wed, 25 Aug 2021 19:31:02 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.22.1/nats-streaming-server-v0.22.1-windows-amd64.zip
# Wed, 25 Aug 2021 19:31:03 GMT
ENV NATS_STREAMING_SERVER_SHASUM=4516852b493111b73ec06477be4a27e66f5abc9ca1ff4dd2b970232271611264
# Wed, 25 Aug 2021 19:31:55 GMT
RUN Set-PSDebug -Trace 2
# Wed, 25 Aug 2021 19:33:24 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 25 Aug 2021 19:33:25 GMT
EXPOSE 4222 8222
# Wed, 25 Aug 2021 19:33:26 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 25 Aug 2021 19:33:27 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c67ded6868b61d392a0c096f911563fd6bc0bc3ed4fe401d077b3718a1b0cdaf`  
		Size: 967.7 MB (967665054 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:985da5cbc0735e1c422e766af23125ba345f431cb337ea43ec32298d0bb8e4ea`  
		Last Modified: Wed, 25 Aug 2021 15:45:02 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3dbdd68a4b0c278695b3e1d401d7eddfb0f0e3aa1e28aed88eb700059648f8f`  
		Last Modified: Wed, 25 Aug 2021 16:11:02 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d02eff460789c6fa51a517221660dddad01c753689cf4d911deed4be925fdfa`  
		Last Modified: Wed, 25 Aug 2021 19:36:40 GMT  
		Size: 1.3 KB (1296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c67c923b3231b172039016dd78d64494840a068f83b7c2eb0610b3916e0f880d`  
		Last Modified: Wed, 25 Aug 2021 19:36:40 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13c73a6e9ff96bac535744e077e3966558cf33b742d3b384e6b77e72d96b4a49`  
		Last Modified: Wed, 25 Aug 2021 19:36:40 GMT  
		Size: 1.4 KB (1351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:652b4bfafc795b6a09e751ef642f31936038547b6223596beda9dc1bbd74f2df`  
		Last Modified: Wed, 25 Aug 2021 19:36:37 GMT  
		Size: 372.7 KB (372655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6d3118388d00fe0ce41388dbed69f505de317c0d9a6551664b34909e0308b85`  
		Last Modified: Wed, 25 Aug 2021 19:36:48 GMT  
		Size: 7.6 MB (7645717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35fd537c3fc591dceb1461535c52fc98243ac3b3fea45db58c6ebc492862440c`  
		Last Modified: Wed, 25 Aug 2021 19:36:37 GMT  
		Size: 1.3 KB (1311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21f9050479fb189fc4a85ae128bcc6a114f42e9139901390f4c6ef669c1ce49a`  
		Last Modified: Wed, 25 Aug 2021 19:36:37 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e587562615088e9b1f845a826539d4c81323caf3b84153496ac0f3c1c8afc45`  
		Last Modified: Wed, 25 Aug 2021 19:36:37 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.22.1-windowsservercore-ltsc2016`

```console
$ docker pull nats-streaming@sha256:8004e2870ca327f887f2e30cc0fa4d36d010512baf99a2ba286275ea0405144c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.14393.4583; amd64

### `nats-streaming:0.22.1-windowsservercore-ltsc2016` - windows version 10.0.14393.4583; amd64

```console
$ docker pull nats-streaming@sha256:b122147602333b9a276aa52c700aae01f366dcad7b0d79a86009a7f8313bbb5a
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6278962413 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:624e3804e5c78766e9c54be1e5b1be3e39dd9aa56935b2944e21531a991f5377`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Sun, 01 Aug 2021 08:52:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 25 Aug 2021 13:59:32 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 25 Aug 2021 16:08:06 GMT
ENV NATS_DOCKERIZED=1
# Wed, 25 Aug 2021 19:33:53 GMT
ENV NATS_STREAMING_SERVER=0.22.1
# Wed, 25 Aug 2021 19:33:53 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.22.1/nats-streaming-server-v0.22.1-windows-amd64.zip
# Wed, 25 Aug 2021 19:33:54 GMT
ENV NATS_STREAMING_SERVER_SHASUM=4516852b493111b73ec06477be4a27e66f5abc9ca1ff4dd2b970232271611264
# Wed, 25 Aug 2021 19:34:35 GMT
RUN Set-PSDebug -Trace 2
# Wed, 25 Aug 2021 19:36:09 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 25 Aug 2021 19:36:10 GMT
EXPOSE 4222 8222
# Wed, 25 Aug 2021 19:36:10 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 25 Aug 2021 19:36:11 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c427f892fe74603ae09d4e49b25f8f7046f957054034dc9f462e0e88d7bffaa5`  
		Size: 2.2 GB (2200980134 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a869803fc3d8292f0fe1bc6ed35e1ceedbd7c797a1486767a55f88c6c28ed4c5`  
		Last Modified: Wed, 25 Aug 2021 15:45:25 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a745f96c10790ef3a2006dbd4c116eb2f1552fd3c4a38fca179a8160e9918ac1`  
		Last Modified: Wed, 25 Aug 2021 16:11:42 GMT  
		Size: 1.3 KB (1329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbb2b2f51b28100175c4c31970f69c26566bea4ec51d87a91555fe5091be241f`  
		Last Modified: Wed, 25 Aug 2021 19:37:17 GMT  
		Size: 1.3 KB (1322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d23161af967280f0d95595b25ca572083145ff8330ed8248c015bf100be1c838`  
		Last Modified: Wed, 25 Aug 2021 19:37:17 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11b49b5a10129016e785edeb8fba72f2d2a8658e8239af2b0fe530c3ae5a53c5`  
		Last Modified: Wed, 25 Aug 2021 19:37:16 GMT  
		Size: 1.3 KB (1314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b369c4a91f133df3608ec1e4cbb5ab7020ac16c0db6684465e735fc719da9a9`  
		Last Modified: Wed, 25 Aug 2021 19:37:14 GMT  
		Size: 336.8 KB (336786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc65df0e7918917488aea97873a4358dfad7b2914701e183c0865d4174c0dd62`  
		Last Modified: Wed, 25 Aug 2021 19:37:22 GMT  
		Size: 7.6 MB (7649022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:131ab6c361a3936d54c3e6d59a85f42d4171d9639f2c4feadb13b7eae8e9ff52`  
		Last Modified: Wed, 25 Aug 2021 19:37:14 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cabe016e1cfca773de7a8d1279fe766c82e6e6e91a9cff7c4725c06a13baa8c`  
		Last Modified: Wed, 25 Aug 2021 19:37:14 GMT  
		Size: 1.3 KB (1325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bf87ca03d1c93fa8e08d0c4be5fc32f8e091424df743e3aeab09d8dd776e5e6`  
		Last Modified: Wed, 25 Aug 2021 19:37:14 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:alpine`

```console
$ docker pull nats-streaming@sha256:025dd4f7090b799587d1ba45d887a67d44f9d12ad0b7c474a8e72c3886150382
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:alpine` - linux; amd64

```console
$ docker pull nats-streaming@sha256:490adf058de78b1fe4f0d33864796f8a112c3b784c6e90ba22e45153fe74d900
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.3 MB (10270658 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fabf0e12d64e19686c51b041dd0cc13952c874c78e6f6c5e113a95dd59c4ea55`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 27 Aug 2021 20:46:27 GMT
ENV NATS_STREAMING_SERVER=0.22.1
# Fri, 27 Aug 2021 20:46:31 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='581698d248a19ecae64e4048d153bc1021744a3da6284680a339f9f82a53a9cf' ;; 		armhf) natsArch='arm6'; sha256='438a89221bb0608e40d21e73ca27a4b70b8560730726942c0ade94a6b6013d6f' ;; 		armv7) natsArch='arm7'; sha256='4164baadd201d1374f7654d3e54a24d81ceb87a385867e31a82c1d1a69e3b1ae' ;; 		x86_64) natsArch='amd64'; sha256='f29e87ac9ff998c928aa8ebc8cf0c4d04d34a3d95b9900d92fd7dafab2bec8cc' ;; 		x86) natsArch='386'; sha256='0ca68e57babb8901d7afeb7569042730904887e718ddf860ef3ee54278753505' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 27 Aug 2021 20:46:31 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Fri, 27 Aug 2021 20:46:32 GMT
EXPOSE 4222 8222
# Fri, 27 Aug 2021 20:46:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 Aug 2021 20:46:33 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8848530ed3e01ccf52dafe72a2e2c14ec4f6ec52809524bd71c33cbe193e5ad3`  
		Last Modified: Fri, 27 Aug 2021 20:47:18 GMT  
		Size: 7.5 MB (7455792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0a13cfe7f8352b89abb0a8ea81910d679c36c4a90d6d88d7f8a9059471b2e31`  
		Last Modified: Fri, 27 Aug 2021 20:47:16 GMT  
		Size: 420.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:9cda74ceed2f45daa20c52af4aa059d5af71f373753072e64d1223e5de592e64
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.6 MB (9561001 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f85120fadd96bf6e11b7fa82dd813c6d56b9aff9cb577d22dc8cbaaae6ac263`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 27 Aug 2021 17:49:29 GMT
ADD file:1c1c4520d49cb6e8f795f3b953d1ed3c3c77868b98b53a455169c254fcec5acd in / 
# Fri, 27 Aug 2021 17:49:30 GMT
CMD ["/bin/sh"]
# Fri, 27 Aug 2021 19:24:22 GMT
ENV NATS_STREAMING_SERVER=0.22.1
# Fri, 27 Aug 2021 19:24:28 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='581698d248a19ecae64e4048d153bc1021744a3da6284680a339f9f82a53a9cf' ;; 		armhf) natsArch='arm6'; sha256='438a89221bb0608e40d21e73ca27a4b70b8560730726942c0ade94a6b6013d6f' ;; 		armv7) natsArch='arm7'; sha256='4164baadd201d1374f7654d3e54a24d81ceb87a385867e31a82c1d1a69e3b1ae' ;; 		x86_64) natsArch='amd64'; sha256='f29e87ac9ff998c928aa8ebc8cf0c4d04d34a3d95b9900d92fd7dafab2bec8cc' ;; 		x86) natsArch='386'; sha256='0ca68e57babb8901d7afeb7569042730904887e718ddf860ef3ee54278753505' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 27 Aug 2021 19:24:29 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Fri, 27 Aug 2021 19:24:29 GMT
EXPOSE 4222 8222
# Fri, 27 Aug 2021 19:24:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 Aug 2021 19:24:30 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:2e78c0f86ba9a1fed30df20cb48c9cc73e9626399f12749d36b892ff99c0ecf5`  
		Last Modified: Fri, 27 Aug 2021 17:50:55 GMT  
		Size: 2.6 MB (2627447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:320a6a97adac4a737e1997906fcc9d6922c1ae39980382314b88be30f8b64ea3`  
		Last Modified: Fri, 27 Aug 2021 19:26:12 GMT  
		Size: 6.9 MB (6933133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92e6007c46c9095e062e9214fe2c0618a2b2fe8642c7f6162972036163e330ad`  
		Last Modified: Fri, 27 Aug 2021 19:26:08 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:7970395d00490fad62f2a51288db47d251cab92ec7634bef6de42343f8e8eedc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.4 MB (9351328 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e19086c92b47964c105a8ed130ff7219833adab1ca8e211c1ad0b0a049866252`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 06 Aug 2021 17:57:32 GMT
ADD file:3a35ff3ac0d80289d419a4d6d8319610c38e1936d296addafb9aaf506946230f in / 
# Fri, 06 Aug 2021 17:57:32 GMT
CMD ["/bin/sh"]
# Fri, 06 Aug 2021 20:29:42 GMT
ENV NATS_STREAMING_SERVER=0.22.1
# Fri, 06 Aug 2021 20:29:48 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='581698d248a19ecae64e4048d153bc1021744a3da6284680a339f9f82a53a9cf' ;; 		armhf) natsArch='arm6'; sha256='438a89221bb0608e40d21e73ca27a4b70b8560730726942c0ade94a6b6013d6f' ;; 		armv7) natsArch='arm7'; sha256='4164baadd201d1374f7654d3e54a24d81ceb87a385867e31a82c1d1a69e3b1ae' ;; 		x86_64) natsArch='amd64'; sha256='f29e87ac9ff998c928aa8ebc8cf0c4d04d34a3d95b9900d92fd7dafab2bec8cc' ;; 		x86) natsArch='386'; sha256='0ca68e57babb8901d7afeb7569042730904887e718ddf860ef3ee54278753505' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 06 Aug 2021 20:29:48 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Fri, 06 Aug 2021 20:29:49 GMT
EXPOSE 4222 8222
# Fri, 06 Aug 2021 20:29:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 06 Aug 2021 20:29:50 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:4ee0caa23b369b04827640a4be298bf4ff7bacd030c77e915f5d7fb8f987594a`  
		Last Modified: Fri, 06 Aug 2021 17:58:57 GMT  
		Size: 2.4 MB (2429359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e14712e6c4fbdd823f35d0df7aa1345088ce3d89727133dcef4adb1105ecb5f`  
		Last Modified: Fri, 06 Aug 2021 20:31:34 GMT  
		Size: 6.9 MB (6921548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e18c45098374f86d0784e7840a2c0fd15ce636edfee6d3ebc23432fd0cc47be5`  
		Last Modified: Fri, 06 Aug 2021 20:31:30 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:366b541434718f0d0bd3e6fffb5dd27db81774c771dc0ecb69c00819fb1b3997
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.5 MB (9542913 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:244415bb00005ee5391d41fc5b03c3477bcf4f2c70a6d081a65dc46b732956c4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Fri, 27 Aug 2021 20:20:38 GMT
ENV NATS_STREAMING_SERVER=0.22.1
# Fri, 27 Aug 2021 20:20:41 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='581698d248a19ecae64e4048d153bc1021744a3da6284680a339f9f82a53a9cf' ;; 		armhf) natsArch='arm6'; sha256='438a89221bb0608e40d21e73ca27a4b70b8560730726942c0ade94a6b6013d6f' ;; 		armv7) natsArch='arm7'; sha256='4164baadd201d1374f7654d3e54a24d81ceb87a385867e31a82c1d1a69e3b1ae' ;; 		x86_64) natsArch='amd64'; sha256='f29e87ac9ff998c928aa8ebc8cf0c4d04d34a3d95b9900d92fd7dafab2bec8cc' ;; 		x86) natsArch='386'; sha256='0ca68e57babb8901d7afeb7569042730904887e718ddf860ef3ee54278753505' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 27 Aug 2021 20:20:41 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Fri, 27 Aug 2021 20:20:41 GMT
EXPOSE 4222 8222
# Fri, 27 Aug 2021 20:20:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 Aug 2021 20:20:41 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:552d1f2373af9bfe12033568ebbfb0ccbb0de11279f9a415a29207e264d7f4d9`  
		Last Modified: Fri, 27 Aug 2021 17:40:18 GMT  
		Size: 2.7 MB (2711827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:069785721c5e4cdee5b76770ae83cf97b47105b106c53b06922f570ba743dadb`  
		Last Modified: Fri, 27 Aug 2021 20:21:32 GMT  
		Size: 6.8 MB (6830666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df70eb7a18c78f5cbb612b797fe94d277338f4bd8e5dfd47cba3d97d57e0e352`  
		Last Modified: Fri, 27 Aug 2021 20:21:31 GMT  
		Size: 420.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:alpine3.14`

```console
$ docker pull nats-streaming@sha256:025dd4f7090b799587d1ba45d887a67d44f9d12ad0b7c474a8e72c3886150382
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:alpine3.14` - linux; amd64

```console
$ docker pull nats-streaming@sha256:490adf058de78b1fe4f0d33864796f8a112c3b784c6e90ba22e45153fe74d900
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.3 MB (10270658 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fabf0e12d64e19686c51b041dd0cc13952c874c78e6f6c5e113a95dd59c4ea55`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 27 Aug 2021 20:46:27 GMT
ENV NATS_STREAMING_SERVER=0.22.1
# Fri, 27 Aug 2021 20:46:31 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='581698d248a19ecae64e4048d153bc1021744a3da6284680a339f9f82a53a9cf' ;; 		armhf) natsArch='arm6'; sha256='438a89221bb0608e40d21e73ca27a4b70b8560730726942c0ade94a6b6013d6f' ;; 		armv7) natsArch='arm7'; sha256='4164baadd201d1374f7654d3e54a24d81ceb87a385867e31a82c1d1a69e3b1ae' ;; 		x86_64) natsArch='amd64'; sha256='f29e87ac9ff998c928aa8ebc8cf0c4d04d34a3d95b9900d92fd7dafab2bec8cc' ;; 		x86) natsArch='386'; sha256='0ca68e57babb8901d7afeb7569042730904887e718ddf860ef3ee54278753505' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 27 Aug 2021 20:46:31 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Fri, 27 Aug 2021 20:46:32 GMT
EXPOSE 4222 8222
# Fri, 27 Aug 2021 20:46:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 Aug 2021 20:46:33 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8848530ed3e01ccf52dafe72a2e2c14ec4f6ec52809524bd71c33cbe193e5ad3`  
		Last Modified: Fri, 27 Aug 2021 20:47:18 GMT  
		Size: 7.5 MB (7455792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0a13cfe7f8352b89abb0a8ea81910d679c36c4a90d6d88d7f8a9059471b2e31`  
		Last Modified: Fri, 27 Aug 2021 20:47:16 GMT  
		Size: 420.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine3.14` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:9cda74ceed2f45daa20c52af4aa059d5af71f373753072e64d1223e5de592e64
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.6 MB (9561001 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f85120fadd96bf6e11b7fa82dd813c6d56b9aff9cb577d22dc8cbaaae6ac263`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 27 Aug 2021 17:49:29 GMT
ADD file:1c1c4520d49cb6e8f795f3b953d1ed3c3c77868b98b53a455169c254fcec5acd in / 
# Fri, 27 Aug 2021 17:49:30 GMT
CMD ["/bin/sh"]
# Fri, 27 Aug 2021 19:24:22 GMT
ENV NATS_STREAMING_SERVER=0.22.1
# Fri, 27 Aug 2021 19:24:28 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='581698d248a19ecae64e4048d153bc1021744a3da6284680a339f9f82a53a9cf' ;; 		armhf) natsArch='arm6'; sha256='438a89221bb0608e40d21e73ca27a4b70b8560730726942c0ade94a6b6013d6f' ;; 		armv7) natsArch='arm7'; sha256='4164baadd201d1374f7654d3e54a24d81ceb87a385867e31a82c1d1a69e3b1ae' ;; 		x86_64) natsArch='amd64'; sha256='f29e87ac9ff998c928aa8ebc8cf0c4d04d34a3d95b9900d92fd7dafab2bec8cc' ;; 		x86) natsArch='386'; sha256='0ca68e57babb8901d7afeb7569042730904887e718ddf860ef3ee54278753505' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 27 Aug 2021 19:24:29 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Fri, 27 Aug 2021 19:24:29 GMT
EXPOSE 4222 8222
# Fri, 27 Aug 2021 19:24:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 Aug 2021 19:24:30 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:2e78c0f86ba9a1fed30df20cb48c9cc73e9626399f12749d36b892ff99c0ecf5`  
		Last Modified: Fri, 27 Aug 2021 17:50:55 GMT  
		Size: 2.6 MB (2627447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:320a6a97adac4a737e1997906fcc9d6922c1ae39980382314b88be30f8b64ea3`  
		Last Modified: Fri, 27 Aug 2021 19:26:12 GMT  
		Size: 6.9 MB (6933133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92e6007c46c9095e062e9214fe2c0618a2b2fe8642c7f6162972036163e330ad`  
		Last Modified: Fri, 27 Aug 2021 19:26:08 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine3.14` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:7970395d00490fad62f2a51288db47d251cab92ec7634bef6de42343f8e8eedc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.4 MB (9351328 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e19086c92b47964c105a8ed130ff7219833adab1ca8e211c1ad0b0a049866252`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 06 Aug 2021 17:57:32 GMT
ADD file:3a35ff3ac0d80289d419a4d6d8319610c38e1936d296addafb9aaf506946230f in / 
# Fri, 06 Aug 2021 17:57:32 GMT
CMD ["/bin/sh"]
# Fri, 06 Aug 2021 20:29:42 GMT
ENV NATS_STREAMING_SERVER=0.22.1
# Fri, 06 Aug 2021 20:29:48 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='581698d248a19ecae64e4048d153bc1021744a3da6284680a339f9f82a53a9cf' ;; 		armhf) natsArch='arm6'; sha256='438a89221bb0608e40d21e73ca27a4b70b8560730726942c0ade94a6b6013d6f' ;; 		armv7) natsArch='arm7'; sha256='4164baadd201d1374f7654d3e54a24d81ceb87a385867e31a82c1d1a69e3b1ae' ;; 		x86_64) natsArch='amd64'; sha256='f29e87ac9ff998c928aa8ebc8cf0c4d04d34a3d95b9900d92fd7dafab2bec8cc' ;; 		x86) natsArch='386'; sha256='0ca68e57babb8901d7afeb7569042730904887e718ddf860ef3ee54278753505' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 06 Aug 2021 20:29:48 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Fri, 06 Aug 2021 20:29:49 GMT
EXPOSE 4222 8222
# Fri, 06 Aug 2021 20:29:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 06 Aug 2021 20:29:50 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:4ee0caa23b369b04827640a4be298bf4ff7bacd030c77e915f5d7fb8f987594a`  
		Last Modified: Fri, 06 Aug 2021 17:58:57 GMT  
		Size: 2.4 MB (2429359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e14712e6c4fbdd823f35d0df7aa1345088ce3d89727133dcef4adb1105ecb5f`  
		Last Modified: Fri, 06 Aug 2021 20:31:34 GMT  
		Size: 6.9 MB (6921548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e18c45098374f86d0784e7840a2c0fd15ce636edfee6d3ebc23432fd0cc47be5`  
		Last Modified: Fri, 06 Aug 2021 20:31:30 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine3.14` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:366b541434718f0d0bd3e6fffb5dd27db81774c771dc0ecb69c00819fb1b3997
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.5 MB (9542913 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:244415bb00005ee5391d41fc5b03c3477bcf4f2c70a6d081a65dc46b732956c4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Fri, 27 Aug 2021 20:20:38 GMT
ENV NATS_STREAMING_SERVER=0.22.1
# Fri, 27 Aug 2021 20:20:41 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='581698d248a19ecae64e4048d153bc1021744a3da6284680a339f9f82a53a9cf' ;; 		armhf) natsArch='arm6'; sha256='438a89221bb0608e40d21e73ca27a4b70b8560730726942c0ade94a6b6013d6f' ;; 		armv7) natsArch='arm7'; sha256='4164baadd201d1374f7654d3e54a24d81ceb87a385867e31a82c1d1a69e3b1ae' ;; 		x86_64) natsArch='amd64'; sha256='f29e87ac9ff998c928aa8ebc8cf0c4d04d34a3d95b9900d92fd7dafab2bec8cc' ;; 		x86) natsArch='386'; sha256='0ca68e57babb8901d7afeb7569042730904887e718ddf860ef3ee54278753505' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 27 Aug 2021 20:20:41 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Fri, 27 Aug 2021 20:20:41 GMT
EXPOSE 4222 8222
# Fri, 27 Aug 2021 20:20:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 Aug 2021 20:20:41 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:552d1f2373af9bfe12033568ebbfb0ccbb0de11279f9a415a29207e264d7f4d9`  
		Last Modified: Fri, 27 Aug 2021 17:40:18 GMT  
		Size: 2.7 MB (2711827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:069785721c5e4cdee5b76770ae83cf97b47105b106c53b06922f570ba743dadb`  
		Last Modified: Fri, 27 Aug 2021 20:21:32 GMT  
		Size: 6.8 MB (6830666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df70eb7a18c78f5cbb612b797fe94d277338f4bd8e5dfd47cba3d97d57e0e352`  
		Last Modified: Fri, 27 Aug 2021 20:21:31 GMT  
		Size: 420.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:latest`

```console
$ docker pull nats-streaming@sha256:f0716868aa216d2a8803f3580bd512fc699da2d7a6af8ff6c5c857d47192e6e7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.2114; amd64

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

### `nats-streaming:latest` - windows version 10.0.17763.2114; amd64

```console
$ docker pull nats-streaming@sha256:6cf5f132f44fee4ec7d112868c7525aac42e5eef00cd0298e1efdffcb1df5251
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.0 MB (110038648 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7863a1802021516178bb5e20547b7e410590d3ad269287d3d99fd163070dc55b`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 05 Aug 2021 19:15:20 GMT
RUN Apply image 1809-amd64
# Wed, 25 Aug 2021 16:07:56 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 25 Aug 2021 19:33:43 GMT
RUN cmd /S /C #(nop) COPY file:9670e5d1fe5a71e47c78fde01235a0bcbcafcfdeeacf96a7669f6e49343fb03b in C:\nats-streaming-server.exe 
# Wed, 25 Aug 2021 19:33:45 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 25 Aug 2021 19:33:45 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 25 Aug 2021 19:33:46 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:bc8517709e9cfff223cb034ff5be8fcbfa5409de286cdac9ae1b8878ebea6b84`  
		Size: 102.7 MB (102741177 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ae8616c17f5cca409a4b1289387e37dc532657ba2b52bb60713ff621acccd506`  
		Last Modified: Wed, 25 Aug 2021 16:11:20 GMT  
		Size: 1.0 KB (1022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa124ed4fe9f29ce6e3db339e67e84f8667fe9ad034f27a42d6554c473e49de1`  
		Last Modified: Wed, 25 Aug 2021 19:37:03 GMT  
		Size: 7.3 MB (7293262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e47ccb646b6561c33cebea3e0f6ffb755fbcec2983095a9fcd42cda5c49b519`  
		Last Modified: Wed, 25 Aug 2021 19:37:01 GMT  
		Size: 1.1 KB (1069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:993faf624f9f41d879898713c9dd7875da6724079bf4f9d0a8af4c5a780dd6c0`  
		Last Modified: Wed, 25 Aug 2021 19:37:00 GMT  
		Size: 1.1 KB (1050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2df1fdf71a2973683c32f5a7cbf28584f357d292855672645e4fda8b1200e200`  
		Last Modified: Wed, 25 Aug 2021 19:37:01 GMT  
		Size: 1.1 KB (1068 bytes)  
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
$ docker pull nats-streaming@sha256:d86bdcb9e19d16a21ea8eb07693268eab508df92a0df40021ca3b296412ba430
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2114; amd64

### `nats-streaming:nanoserver` - windows version 10.0.17763.2114; amd64

```console
$ docker pull nats-streaming@sha256:6cf5f132f44fee4ec7d112868c7525aac42e5eef00cd0298e1efdffcb1df5251
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.0 MB (110038648 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7863a1802021516178bb5e20547b7e410590d3ad269287d3d99fd163070dc55b`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 05 Aug 2021 19:15:20 GMT
RUN Apply image 1809-amd64
# Wed, 25 Aug 2021 16:07:56 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 25 Aug 2021 19:33:43 GMT
RUN cmd /S /C #(nop) COPY file:9670e5d1fe5a71e47c78fde01235a0bcbcafcfdeeacf96a7669f6e49343fb03b in C:\nats-streaming-server.exe 
# Wed, 25 Aug 2021 19:33:45 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 25 Aug 2021 19:33:45 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 25 Aug 2021 19:33:46 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:bc8517709e9cfff223cb034ff5be8fcbfa5409de286cdac9ae1b8878ebea6b84`  
		Size: 102.7 MB (102741177 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ae8616c17f5cca409a4b1289387e37dc532657ba2b52bb60713ff621acccd506`  
		Last Modified: Wed, 25 Aug 2021 16:11:20 GMT  
		Size: 1.0 KB (1022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa124ed4fe9f29ce6e3db339e67e84f8667fe9ad034f27a42d6554c473e49de1`  
		Last Modified: Wed, 25 Aug 2021 19:37:03 GMT  
		Size: 7.3 MB (7293262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e47ccb646b6561c33cebea3e0f6ffb755fbcec2983095a9fcd42cda5c49b519`  
		Last Modified: Wed, 25 Aug 2021 19:37:01 GMT  
		Size: 1.1 KB (1069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:993faf624f9f41d879898713c9dd7875da6724079bf4f9d0a8af4c5a780dd6c0`  
		Last Modified: Wed, 25 Aug 2021 19:37:00 GMT  
		Size: 1.1 KB (1050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2df1fdf71a2973683c32f5a7cbf28584f357d292855672645e4fda8b1200e200`  
		Last Modified: Wed, 25 Aug 2021 19:37:01 GMT  
		Size: 1.1 KB (1068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:nanoserver-1809`

```console
$ docker pull nats-streaming@sha256:d86bdcb9e19d16a21ea8eb07693268eab508df92a0df40021ca3b296412ba430
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2114; amd64

### `nats-streaming:nanoserver-1809` - windows version 10.0.17763.2114; amd64

```console
$ docker pull nats-streaming@sha256:6cf5f132f44fee4ec7d112868c7525aac42e5eef00cd0298e1efdffcb1df5251
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.0 MB (110038648 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7863a1802021516178bb5e20547b7e410590d3ad269287d3d99fd163070dc55b`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 05 Aug 2021 19:15:20 GMT
RUN Apply image 1809-amd64
# Wed, 25 Aug 2021 16:07:56 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 25 Aug 2021 19:33:43 GMT
RUN cmd /S /C #(nop) COPY file:9670e5d1fe5a71e47c78fde01235a0bcbcafcfdeeacf96a7669f6e49343fb03b in C:\nats-streaming-server.exe 
# Wed, 25 Aug 2021 19:33:45 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 25 Aug 2021 19:33:45 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 25 Aug 2021 19:33:46 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:bc8517709e9cfff223cb034ff5be8fcbfa5409de286cdac9ae1b8878ebea6b84`  
		Size: 102.7 MB (102741177 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ae8616c17f5cca409a4b1289387e37dc532657ba2b52bb60713ff621acccd506`  
		Last Modified: Wed, 25 Aug 2021 16:11:20 GMT  
		Size: 1.0 KB (1022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa124ed4fe9f29ce6e3db339e67e84f8667fe9ad034f27a42d6554c473e49de1`  
		Last Modified: Wed, 25 Aug 2021 19:37:03 GMT  
		Size: 7.3 MB (7293262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e47ccb646b6561c33cebea3e0f6ffb755fbcec2983095a9fcd42cda5c49b519`  
		Last Modified: Wed, 25 Aug 2021 19:37:01 GMT  
		Size: 1.1 KB (1069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:993faf624f9f41d879898713c9dd7875da6724079bf4f9d0a8af4c5a780dd6c0`  
		Last Modified: Wed, 25 Aug 2021 19:37:00 GMT  
		Size: 1.1 KB (1050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2df1fdf71a2973683c32f5a7cbf28584f357d292855672645e4fda8b1200e200`  
		Last Modified: Wed, 25 Aug 2021 19:37:01 GMT  
		Size: 1.1 KB (1068 bytes)  
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
$ docker pull nats-streaming@sha256:0fd0290d10cf965f1222f90fa114908b384cb8a816e81780143f32e89185a017
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.2114; amd64
	-	windows version 10.0.14393.4583; amd64

### `nats-streaming:windowsservercore` - windows version 10.0.17763.2114; amd64

```console
$ docker pull nats-streaming@sha256:d6ba04cfbedbf1ce9e219918c40dd6989e1d50a8e2398bb1d69fb19597056636
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2694026981 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:54951a15532bfdfb9b767cb2b92cb384b91b1c66f44a6cfb259769a168458b7f`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 05 Aug 2021 19:44:34 GMT
RUN Install update 1809-amd64
# Wed, 25 Aug 2021 13:46:35 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 25 Aug 2021 16:05:30 GMT
ENV NATS_DOCKERIZED=1
# Wed, 25 Aug 2021 19:31:01 GMT
ENV NATS_STREAMING_SERVER=0.22.1
# Wed, 25 Aug 2021 19:31:02 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.22.1/nats-streaming-server-v0.22.1-windows-amd64.zip
# Wed, 25 Aug 2021 19:31:03 GMT
ENV NATS_STREAMING_SERVER_SHASUM=4516852b493111b73ec06477be4a27e66f5abc9ca1ff4dd2b970232271611264
# Wed, 25 Aug 2021 19:31:55 GMT
RUN Set-PSDebug -Trace 2
# Wed, 25 Aug 2021 19:33:24 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 25 Aug 2021 19:33:25 GMT
EXPOSE 4222 8222
# Wed, 25 Aug 2021 19:33:26 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 25 Aug 2021 19:33:27 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c67ded6868b61d392a0c096f911563fd6bc0bc3ed4fe401d077b3718a1b0cdaf`  
		Size: 967.7 MB (967665054 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:985da5cbc0735e1c422e766af23125ba345f431cb337ea43ec32298d0bb8e4ea`  
		Last Modified: Wed, 25 Aug 2021 15:45:02 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3dbdd68a4b0c278695b3e1d401d7eddfb0f0e3aa1e28aed88eb700059648f8f`  
		Last Modified: Wed, 25 Aug 2021 16:11:02 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d02eff460789c6fa51a517221660dddad01c753689cf4d911deed4be925fdfa`  
		Last Modified: Wed, 25 Aug 2021 19:36:40 GMT  
		Size: 1.3 KB (1296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c67c923b3231b172039016dd78d64494840a068f83b7c2eb0610b3916e0f880d`  
		Last Modified: Wed, 25 Aug 2021 19:36:40 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13c73a6e9ff96bac535744e077e3966558cf33b742d3b384e6b77e72d96b4a49`  
		Last Modified: Wed, 25 Aug 2021 19:36:40 GMT  
		Size: 1.4 KB (1351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:652b4bfafc795b6a09e751ef642f31936038547b6223596beda9dc1bbd74f2df`  
		Last Modified: Wed, 25 Aug 2021 19:36:37 GMT  
		Size: 372.7 KB (372655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6d3118388d00fe0ce41388dbed69f505de317c0d9a6551664b34909e0308b85`  
		Last Modified: Wed, 25 Aug 2021 19:36:48 GMT  
		Size: 7.6 MB (7645717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35fd537c3fc591dceb1461535c52fc98243ac3b3fea45db58c6ebc492862440c`  
		Last Modified: Wed, 25 Aug 2021 19:36:37 GMT  
		Size: 1.3 KB (1311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21f9050479fb189fc4a85ae128bcc6a114f42e9139901390f4c6ef669c1ce49a`  
		Last Modified: Wed, 25 Aug 2021 19:36:37 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e587562615088e9b1f845a826539d4c81323caf3b84153496ac0f3c1c8afc45`  
		Last Modified: Wed, 25 Aug 2021 19:36:37 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:windowsservercore` - windows version 10.0.14393.4583; amd64

```console
$ docker pull nats-streaming@sha256:b122147602333b9a276aa52c700aae01f366dcad7b0d79a86009a7f8313bbb5a
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6278962413 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:624e3804e5c78766e9c54be1e5b1be3e39dd9aa56935b2944e21531a991f5377`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Sun, 01 Aug 2021 08:52:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 25 Aug 2021 13:59:32 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 25 Aug 2021 16:08:06 GMT
ENV NATS_DOCKERIZED=1
# Wed, 25 Aug 2021 19:33:53 GMT
ENV NATS_STREAMING_SERVER=0.22.1
# Wed, 25 Aug 2021 19:33:53 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.22.1/nats-streaming-server-v0.22.1-windows-amd64.zip
# Wed, 25 Aug 2021 19:33:54 GMT
ENV NATS_STREAMING_SERVER_SHASUM=4516852b493111b73ec06477be4a27e66f5abc9ca1ff4dd2b970232271611264
# Wed, 25 Aug 2021 19:34:35 GMT
RUN Set-PSDebug -Trace 2
# Wed, 25 Aug 2021 19:36:09 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 25 Aug 2021 19:36:10 GMT
EXPOSE 4222 8222
# Wed, 25 Aug 2021 19:36:10 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 25 Aug 2021 19:36:11 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c427f892fe74603ae09d4e49b25f8f7046f957054034dc9f462e0e88d7bffaa5`  
		Size: 2.2 GB (2200980134 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a869803fc3d8292f0fe1bc6ed35e1ceedbd7c797a1486767a55f88c6c28ed4c5`  
		Last Modified: Wed, 25 Aug 2021 15:45:25 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a745f96c10790ef3a2006dbd4c116eb2f1552fd3c4a38fca179a8160e9918ac1`  
		Last Modified: Wed, 25 Aug 2021 16:11:42 GMT  
		Size: 1.3 KB (1329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbb2b2f51b28100175c4c31970f69c26566bea4ec51d87a91555fe5091be241f`  
		Last Modified: Wed, 25 Aug 2021 19:37:17 GMT  
		Size: 1.3 KB (1322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d23161af967280f0d95595b25ca572083145ff8330ed8248c015bf100be1c838`  
		Last Modified: Wed, 25 Aug 2021 19:37:17 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11b49b5a10129016e785edeb8fba72f2d2a8658e8239af2b0fe530c3ae5a53c5`  
		Last Modified: Wed, 25 Aug 2021 19:37:16 GMT  
		Size: 1.3 KB (1314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b369c4a91f133df3608ec1e4cbb5ab7020ac16c0db6684465e735fc719da9a9`  
		Last Modified: Wed, 25 Aug 2021 19:37:14 GMT  
		Size: 336.8 KB (336786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc65df0e7918917488aea97873a4358dfad7b2914701e183c0865d4174c0dd62`  
		Last Modified: Wed, 25 Aug 2021 19:37:22 GMT  
		Size: 7.6 MB (7649022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:131ab6c361a3936d54c3e6d59a85f42d4171d9639f2c4feadb13b7eae8e9ff52`  
		Last Modified: Wed, 25 Aug 2021 19:37:14 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cabe016e1cfca773de7a8d1279fe766c82e6e6e91a9cff7c4725c06a13baa8c`  
		Last Modified: Wed, 25 Aug 2021 19:37:14 GMT  
		Size: 1.3 KB (1325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bf87ca03d1c93fa8e08d0c4be5fc32f8e091424df743e3aeab09d8dd776e5e6`  
		Last Modified: Wed, 25 Aug 2021 19:37:14 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:windowsservercore-1809`

```console
$ docker pull nats-streaming@sha256:6c691bb80388e286a736ac34253f62975b7da9bd039815b3fb7b82f3ebec4740
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2114; amd64

### `nats-streaming:windowsservercore-1809` - windows version 10.0.17763.2114; amd64

```console
$ docker pull nats-streaming@sha256:d6ba04cfbedbf1ce9e219918c40dd6989e1d50a8e2398bb1d69fb19597056636
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2694026981 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:54951a15532bfdfb9b767cb2b92cb384b91b1c66f44a6cfb259769a168458b7f`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 05 Aug 2021 19:44:34 GMT
RUN Install update 1809-amd64
# Wed, 25 Aug 2021 13:46:35 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 25 Aug 2021 16:05:30 GMT
ENV NATS_DOCKERIZED=1
# Wed, 25 Aug 2021 19:31:01 GMT
ENV NATS_STREAMING_SERVER=0.22.1
# Wed, 25 Aug 2021 19:31:02 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.22.1/nats-streaming-server-v0.22.1-windows-amd64.zip
# Wed, 25 Aug 2021 19:31:03 GMT
ENV NATS_STREAMING_SERVER_SHASUM=4516852b493111b73ec06477be4a27e66f5abc9ca1ff4dd2b970232271611264
# Wed, 25 Aug 2021 19:31:55 GMT
RUN Set-PSDebug -Trace 2
# Wed, 25 Aug 2021 19:33:24 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 25 Aug 2021 19:33:25 GMT
EXPOSE 4222 8222
# Wed, 25 Aug 2021 19:33:26 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 25 Aug 2021 19:33:27 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c67ded6868b61d392a0c096f911563fd6bc0bc3ed4fe401d077b3718a1b0cdaf`  
		Size: 967.7 MB (967665054 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:985da5cbc0735e1c422e766af23125ba345f431cb337ea43ec32298d0bb8e4ea`  
		Last Modified: Wed, 25 Aug 2021 15:45:02 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3dbdd68a4b0c278695b3e1d401d7eddfb0f0e3aa1e28aed88eb700059648f8f`  
		Last Modified: Wed, 25 Aug 2021 16:11:02 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d02eff460789c6fa51a517221660dddad01c753689cf4d911deed4be925fdfa`  
		Last Modified: Wed, 25 Aug 2021 19:36:40 GMT  
		Size: 1.3 KB (1296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c67c923b3231b172039016dd78d64494840a068f83b7c2eb0610b3916e0f880d`  
		Last Modified: Wed, 25 Aug 2021 19:36:40 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13c73a6e9ff96bac535744e077e3966558cf33b742d3b384e6b77e72d96b4a49`  
		Last Modified: Wed, 25 Aug 2021 19:36:40 GMT  
		Size: 1.4 KB (1351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:652b4bfafc795b6a09e751ef642f31936038547b6223596beda9dc1bbd74f2df`  
		Last Modified: Wed, 25 Aug 2021 19:36:37 GMT  
		Size: 372.7 KB (372655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6d3118388d00fe0ce41388dbed69f505de317c0d9a6551664b34909e0308b85`  
		Last Modified: Wed, 25 Aug 2021 19:36:48 GMT  
		Size: 7.6 MB (7645717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35fd537c3fc591dceb1461535c52fc98243ac3b3fea45db58c6ebc492862440c`  
		Last Modified: Wed, 25 Aug 2021 19:36:37 GMT  
		Size: 1.3 KB (1311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21f9050479fb189fc4a85ae128bcc6a114f42e9139901390f4c6ef669c1ce49a`  
		Last Modified: Wed, 25 Aug 2021 19:36:37 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e587562615088e9b1f845a826539d4c81323caf3b84153496ac0f3c1c8afc45`  
		Last Modified: Wed, 25 Aug 2021 19:36:37 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:windowsservercore-ltsc2016`

```console
$ docker pull nats-streaming@sha256:8004e2870ca327f887f2e30cc0fa4d36d010512baf99a2ba286275ea0405144c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.14393.4583; amd64

### `nats-streaming:windowsservercore-ltsc2016` - windows version 10.0.14393.4583; amd64

```console
$ docker pull nats-streaming@sha256:b122147602333b9a276aa52c700aae01f366dcad7b0d79a86009a7f8313bbb5a
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6278962413 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:624e3804e5c78766e9c54be1e5b1be3e39dd9aa56935b2944e21531a991f5377`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Sun, 01 Aug 2021 08:52:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 25 Aug 2021 13:59:32 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 25 Aug 2021 16:08:06 GMT
ENV NATS_DOCKERIZED=1
# Wed, 25 Aug 2021 19:33:53 GMT
ENV NATS_STREAMING_SERVER=0.22.1
# Wed, 25 Aug 2021 19:33:53 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.22.1/nats-streaming-server-v0.22.1-windows-amd64.zip
# Wed, 25 Aug 2021 19:33:54 GMT
ENV NATS_STREAMING_SERVER_SHASUM=4516852b493111b73ec06477be4a27e66f5abc9ca1ff4dd2b970232271611264
# Wed, 25 Aug 2021 19:34:35 GMT
RUN Set-PSDebug -Trace 2
# Wed, 25 Aug 2021 19:36:09 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 25 Aug 2021 19:36:10 GMT
EXPOSE 4222 8222
# Wed, 25 Aug 2021 19:36:10 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 25 Aug 2021 19:36:11 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c427f892fe74603ae09d4e49b25f8f7046f957054034dc9f462e0e88d7bffaa5`  
		Size: 2.2 GB (2200980134 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a869803fc3d8292f0fe1bc6ed35e1ceedbd7c797a1486767a55f88c6c28ed4c5`  
		Last Modified: Wed, 25 Aug 2021 15:45:25 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a745f96c10790ef3a2006dbd4c116eb2f1552fd3c4a38fca179a8160e9918ac1`  
		Last Modified: Wed, 25 Aug 2021 16:11:42 GMT  
		Size: 1.3 KB (1329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbb2b2f51b28100175c4c31970f69c26566bea4ec51d87a91555fe5091be241f`  
		Last Modified: Wed, 25 Aug 2021 19:37:17 GMT  
		Size: 1.3 KB (1322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d23161af967280f0d95595b25ca572083145ff8330ed8248c015bf100be1c838`  
		Last Modified: Wed, 25 Aug 2021 19:37:17 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11b49b5a10129016e785edeb8fba72f2d2a8658e8239af2b0fe530c3ae5a53c5`  
		Last Modified: Wed, 25 Aug 2021 19:37:16 GMT  
		Size: 1.3 KB (1314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b369c4a91f133df3608ec1e4cbb5ab7020ac16c0db6684465e735fc719da9a9`  
		Last Modified: Wed, 25 Aug 2021 19:37:14 GMT  
		Size: 336.8 KB (336786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc65df0e7918917488aea97873a4358dfad7b2914701e183c0865d4174c0dd62`  
		Last Modified: Wed, 25 Aug 2021 19:37:22 GMT  
		Size: 7.6 MB (7649022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:131ab6c361a3936d54c3e6d59a85f42d4171d9639f2c4feadb13b7eae8e9ff52`  
		Last Modified: Wed, 25 Aug 2021 19:37:14 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cabe016e1cfca773de7a8d1279fe766c82e6e6e91a9cff7c4725c06a13baa8c`  
		Last Modified: Wed, 25 Aug 2021 19:37:14 GMT  
		Size: 1.3 KB (1325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bf87ca03d1c93fa8e08d0c4be5fc32f8e091424df743e3aeab09d8dd776e5e6`  
		Last Modified: Wed, 25 Aug 2021 19:37:14 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
