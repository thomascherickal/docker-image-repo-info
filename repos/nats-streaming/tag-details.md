<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `nats-streaming`

-	[`nats-streaming:0.22`](#nats-streaming022)
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
-	[`nats-streaming:0.22-alpine`](#nats-streaming022-alpine)
-	[`nats-streaming:0.22-alpine3.14`](#nats-streaming022-alpine314)
-	[`nats-streaming:0.22-linux`](#nats-streaming022-linux)
-	[`nats-streaming:0.22-nanoserver`](#nats-streaming022-nanoserver)
-	[`nats-streaming:0.22-nanoserver-1809`](#nats-streaming022-nanoserver-1809)
-	[`nats-streaming:0.22-scratch`](#nats-streaming022-scratch)
-	[`nats-streaming:0.22-windowsservercore`](#nats-streaming022-windowsservercore)
-	[`nats-streaming:0.22-windowsservercore-1809`](#nats-streaming022-windowsservercore-1809)
-	[`nats-streaming:0.22-windowsservercore-ltsc2016`](#nats-streaming022-windowsservercore-ltsc2016)
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
$ docker pull nats-streaming@sha256:42ec681f33c9c9fd6737322526f566c8c54f969e6d2db09591645ad26990b30e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.2183; amd64

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

### `nats-streaming:0.22` - windows version 10.0.17763.2183; amd64

```console
$ docker pull nats-streaming@sha256:f7300d49f73a0e5451f68fcf439d1e5b75b5a891aa04e8ff537b523b15d45fc6
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.0 MB (110001330 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa93dcd937d8cd2009cb8f123551ce0f46c671f91465df126ce8475110a4f6cd`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 13 Sep 2021 03:45:12 GMT
RUN Apply image 1809-amd64
# Wed, 15 Sep 2021 15:43:05 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 15 Sep 2021 18:51:57 GMT
RUN cmd /S /C #(nop) COPY file:9670e5d1fe5a71e47c78fde01235a0bcbcafcfdeeacf96a7669f6e49343fb03b in C:\nats-streaming-server.exe 
# Wed, 15 Sep 2021 18:51:58 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 15 Sep 2021 18:51:59 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 15 Sep 2021 18:51:59 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:3585a81ca503e6c63dce938a5606f4171d7461e51000a92054b3f5692786d6c9`  
		Size: 102.7 MB (102703785 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:66dbf96361e9ec1f64f66e255a947eab476edef46c3f9a3b4ede943fa8b87699`  
		Last Modified: Wed, 15 Sep 2021 15:46:11 GMT  
		Size: 1.1 KB (1089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07e5a8a8a1823e7ab1aab125064b8d7d94f6dacefba9d82b815174cb4c32a833`  
		Last Modified: Wed, 15 Sep 2021 18:55:12 GMT  
		Size: 7.3 MB (7293261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16df1d39830ccb4fa2828c96b6c6ec476f1f3a292bdbd01053a21c6c9457750b`  
		Last Modified: Wed, 15 Sep 2021 18:55:04 GMT  
		Size: 1.1 KB (1114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43f99c367ebf7f75f5e675f26e18195abf8826890c87d26039e2c58b38a681d6`  
		Last Modified: Wed, 15 Sep 2021 18:55:04 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3052f7738f8821f9a96f777624d74a7b0b9c7fe0bcecce51d3586ea05479556d`  
		Last Modified: Wed, 15 Sep 2021 18:55:04 GMT  
		Size: 1.0 KB (1030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.22.1`

```console
$ docker pull nats-streaming@sha256:42ec681f33c9c9fd6737322526f566c8c54f969e6d2db09591645ad26990b30e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.2183; amd64

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

### `nats-streaming:0.22.1` - windows version 10.0.17763.2183; amd64

```console
$ docker pull nats-streaming@sha256:f7300d49f73a0e5451f68fcf439d1e5b75b5a891aa04e8ff537b523b15d45fc6
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.0 MB (110001330 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa93dcd937d8cd2009cb8f123551ce0f46c671f91465df126ce8475110a4f6cd`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 13 Sep 2021 03:45:12 GMT
RUN Apply image 1809-amd64
# Wed, 15 Sep 2021 15:43:05 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 15 Sep 2021 18:51:57 GMT
RUN cmd /S /C #(nop) COPY file:9670e5d1fe5a71e47c78fde01235a0bcbcafcfdeeacf96a7669f6e49343fb03b in C:\nats-streaming-server.exe 
# Wed, 15 Sep 2021 18:51:58 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 15 Sep 2021 18:51:59 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 15 Sep 2021 18:51:59 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:3585a81ca503e6c63dce938a5606f4171d7461e51000a92054b3f5692786d6c9`  
		Size: 102.7 MB (102703785 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:66dbf96361e9ec1f64f66e255a947eab476edef46c3f9a3b4ede943fa8b87699`  
		Last Modified: Wed, 15 Sep 2021 15:46:11 GMT  
		Size: 1.1 KB (1089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07e5a8a8a1823e7ab1aab125064b8d7d94f6dacefba9d82b815174cb4c32a833`  
		Last Modified: Wed, 15 Sep 2021 18:55:12 GMT  
		Size: 7.3 MB (7293261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16df1d39830ccb4fa2828c96b6c6ec476f1f3a292bdbd01053a21c6c9457750b`  
		Last Modified: Wed, 15 Sep 2021 18:55:04 GMT  
		Size: 1.1 KB (1114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43f99c367ebf7f75f5e675f26e18195abf8826890c87d26039e2c58b38a681d6`  
		Last Modified: Wed, 15 Sep 2021 18:55:04 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3052f7738f8821f9a96f777624d74a7b0b9c7fe0bcecce51d3586ea05479556d`  
		Last Modified: Wed, 15 Sep 2021 18:55:04 GMT  
		Size: 1.0 KB (1030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.22.1-alpine`

```console
$ docker pull nats-streaming@sha256:faa20055417a6b6df8cfc690c34b132b3291b66699d13be2be328d2682c2e0e0
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
$ docker pull nats-streaming@sha256:709bf964baa04bed21788daab878aaf76613f67b25782dfa91f68dac883c1e96
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.4 MB (9352403 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:120c9c54d0d41980417a67786d13b07474948f1a4fe697b1bfe029344e8b5d55`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 27 Aug 2021 17:57:31 GMT
ADD file:a7da7992ccea54d3295231027614f138aa45c4d4a25ea6ec9bf7b316b9f67d95 in / 
# Fri, 27 Aug 2021 17:57:32 GMT
CMD ["/bin/sh"]
# Fri, 27 Aug 2021 21:15:57 GMT
ENV NATS_STREAMING_SERVER=0.22.1
# Fri, 27 Aug 2021 21:16:03 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='581698d248a19ecae64e4048d153bc1021744a3da6284680a339f9f82a53a9cf' ;; 		armhf) natsArch='arm6'; sha256='438a89221bb0608e40d21e73ca27a4b70b8560730726942c0ade94a6b6013d6f' ;; 		armv7) natsArch='arm7'; sha256='4164baadd201d1374f7654d3e54a24d81ceb87a385867e31a82c1d1a69e3b1ae' ;; 		x86_64) natsArch='amd64'; sha256='f29e87ac9ff998c928aa8ebc8cf0c4d04d34a3d95b9900d92fd7dafab2bec8cc' ;; 		x86) natsArch='386'; sha256='0ca68e57babb8901d7afeb7569042730904887e718ddf860ef3ee54278753505' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 27 Aug 2021 21:16:03 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Fri, 27 Aug 2021 21:16:04 GMT
EXPOSE 4222 8222
# Fri, 27 Aug 2021 21:16:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 Aug 2021 21:16:05 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:a14774a5a62e0f454febaec7cb603e18a6a8e25ef9da4a4da85b155bdd5e5a7a`  
		Last Modified: Fri, 27 Aug 2021 17:59:00 GMT  
		Size: 2.4 MB (2430419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7d0e8657e131875280f89b03741d9c7b5b154791cef8ce515fe711e4185a32d`  
		Last Modified: Fri, 27 Aug 2021 21:17:51 GMT  
		Size: 6.9 MB (6921563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20506d2b8361ef74d3f9c4e5dc7489f829d0181c070aca1b163eb8f540762e4c`  
		Last Modified: Fri, 27 Aug 2021 21:17:47 GMT  
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
$ docker pull nats-streaming@sha256:faa20055417a6b6df8cfc690c34b132b3291b66699d13be2be328d2682c2e0e0
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
$ docker pull nats-streaming@sha256:709bf964baa04bed21788daab878aaf76613f67b25782dfa91f68dac883c1e96
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.4 MB (9352403 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:120c9c54d0d41980417a67786d13b07474948f1a4fe697b1bfe029344e8b5d55`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 27 Aug 2021 17:57:31 GMT
ADD file:a7da7992ccea54d3295231027614f138aa45c4d4a25ea6ec9bf7b316b9f67d95 in / 
# Fri, 27 Aug 2021 17:57:32 GMT
CMD ["/bin/sh"]
# Fri, 27 Aug 2021 21:15:57 GMT
ENV NATS_STREAMING_SERVER=0.22.1
# Fri, 27 Aug 2021 21:16:03 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='581698d248a19ecae64e4048d153bc1021744a3da6284680a339f9f82a53a9cf' ;; 		armhf) natsArch='arm6'; sha256='438a89221bb0608e40d21e73ca27a4b70b8560730726942c0ade94a6b6013d6f' ;; 		armv7) natsArch='arm7'; sha256='4164baadd201d1374f7654d3e54a24d81ceb87a385867e31a82c1d1a69e3b1ae' ;; 		x86_64) natsArch='amd64'; sha256='f29e87ac9ff998c928aa8ebc8cf0c4d04d34a3d95b9900d92fd7dafab2bec8cc' ;; 		x86) natsArch='386'; sha256='0ca68e57babb8901d7afeb7569042730904887e718ddf860ef3ee54278753505' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 27 Aug 2021 21:16:03 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Fri, 27 Aug 2021 21:16:04 GMT
EXPOSE 4222 8222
# Fri, 27 Aug 2021 21:16:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 Aug 2021 21:16:05 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:a14774a5a62e0f454febaec7cb603e18a6a8e25ef9da4a4da85b155bdd5e5a7a`  
		Last Modified: Fri, 27 Aug 2021 17:59:00 GMT  
		Size: 2.4 MB (2430419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7d0e8657e131875280f89b03741d9c7b5b154791cef8ce515fe711e4185a32d`  
		Last Modified: Fri, 27 Aug 2021 21:17:51 GMT  
		Size: 6.9 MB (6921563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20506d2b8361ef74d3f9c4e5dc7489f829d0181c070aca1b163eb8f540762e4c`  
		Last Modified: Fri, 27 Aug 2021 21:17:47 GMT  
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
$ docker pull nats-streaming@sha256:d825481c4d8339d300a56d9f3eeaecf48ae0c071064bfa5ccfb1d9393ff52765
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2183; amd64

### `nats-streaming:0.22.1-nanoserver` - windows version 10.0.17763.2183; amd64

```console
$ docker pull nats-streaming@sha256:f7300d49f73a0e5451f68fcf439d1e5b75b5a891aa04e8ff537b523b15d45fc6
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.0 MB (110001330 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa93dcd937d8cd2009cb8f123551ce0f46c671f91465df126ce8475110a4f6cd`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 13 Sep 2021 03:45:12 GMT
RUN Apply image 1809-amd64
# Wed, 15 Sep 2021 15:43:05 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 15 Sep 2021 18:51:57 GMT
RUN cmd /S /C #(nop) COPY file:9670e5d1fe5a71e47c78fde01235a0bcbcafcfdeeacf96a7669f6e49343fb03b in C:\nats-streaming-server.exe 
# Wed, 15 Sep 2021 18:51:58 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 15 Sep 2021 18:51:59 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 15 Sep 2021 18:51:59 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:3585a81ca503e6c63dce938a5606f4171d7461e51000a92054b3f5692786d6c9`  
		Size: 102.7 MB (102703785 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:66dbf96361e9ec1f64f66e255a947eab476edef46c3f9a3b4ede943fa8b87699`  
		Last Modified: Wed, 15 Sep 2021 15:46:11 GMT  
		Size: 1.1 KB (1089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07e5a8a8a1823e7ab1aab125064b8d7d94f6dacefba9d82b815174cb4c32a833`  
		Last Modified: Wed, 15 Sep 2021 18:55:12 GMT  
		Size: 7.3 MB (7293261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16df1d39830ccb4fa2828c96b6c6ec476f1f3a292bdbd01053a21c6c9457750b`  
		Last Modified: Wed, 15 Sep 2021 18:55:04 GMT  
		Size: 1.1 KB (1114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43f99c367ebf7f75f5e675f26e18195abf8826890c87d26039e2c58b38a681d6`  
		Last Modified: Wed, 15 Sep 2021 18:55:04 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3052f7738f8821f9a96f777624d74a7b0b9c7fe0bcecce51d3586ea05479556d`  
		Last Modified: Wed, 15 Sep 2021 18:55:04 GMT  
		Size: 1.0 KB (1030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.22.1-nanoserver-1809`

```console
$ docker pull nats-streaming@sha256:d825481c4d8339d300a56d9f3eeaecf48ae0c071064bfa5ccfb1d9393ff52765
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2183; amd64

### `nats-streaming:0.22.1-nanoserver-1809` - windows version 10.0.17763.2183; amd64

```console
$ docker pull nats-streaming@sha256:f7300d49f73a0e5451f68fcf439d1e5b75b5a891aa04e8ff537b523b15d45fc6
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.0 MB (110001330 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa93dcd937d8cd2009cb8f123551ce0f46c671f91465df126ce8475110a4f6cd`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 13 Sep 2021 03:45:12 GMT
RUN Apply image 1809-amd64
# Wed, 15 Sep 2021 15:43:05 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 15 Sep 2021 18:51:57 GMT
RUN cmd /S /C #(nop) COPY file:9670e5d1fe5a71e47c78fde01235a0bcbcafcfdeeacf96a7669f6e49343fb03b in C:\nats-streaming-server.exe 
# Wed, 15 Sep 2021 18:51:58 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 15 Sep 2021 18:51:59 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 15 Sep 2021 18:51:59 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:3585a81ca503e6c63dce938a5606f4171d7461e51000a92054b3f5692786d6c9`  
		Size: 102.7 MB (102703785 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:66dbf96361e9ec1f64f66e255a947eab476edef46c3f9a3b4ede943fa8b87699`  
		Last Modified: Wed, 15 Sep 2021 15:46:11 GMT  
		Size: 1.1 KB (1089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07e5a8a8a1823e7ab1aab125064b8d7d94f6dacefba9d82b815174cb4c32a833`  
		Last Modified: Wed, 15 Sep 2021 18:55:12 GMT  
		Size: 7.3 MB (7293261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16df1d39830ccb4fa2828c96b6c6ec476f1f3a292bdbd01053a21c6c9457750b`  
		Last Modified: Wed, 15 Sep 2021 18:55:04 GMT  
		Size: 1.1 KB (1114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43f99c367ebf7f75f5e675f26e18195abf8826890c87d26039e2c58b38a681d6`  
		Last Modified: Wed, 15 Sep 2021 18:55:04 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3052f7738f8821f9a96f777624d74a7b0b9c7fe0bcecce51d3586ea05479556d`  
		Last Modified: Wed, 15 Sep 2021 18:55:04 GMT  
		Size: 1.0 KB (1030 bytes)  
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
$ docker pull nats-streaming@sha256:216e97a64fbe21529831ff1ddac989c2147fe68298359fb82b1c304153c9f38a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.2183; amd64
	-	windows version 10.0.14393.4651; amd64

### `nats-streaming:0.22.1-windowsservercore` - windows version 10.0.17763.2183; amd64

```console
$ docker pull nats-streaming@sha256:48f5ee8c66860f96f1851945d34a317b4038c171a4fc036953bd45e22ae600b8
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2694683224 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03cd19bbfbdb07be71a6322be26c8f7fce0969a83528b4755cf4c72f694719ed`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 13 Sep 2021 04:08:33 GMT
RUN Install update 1809-amd64
# Wed, 15 Sep 2021 13:14:12 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 15 Sep 2021 15:40:54 GMT
ENV NATS_DOCKERIZED=1
# Wed, 15 Sep 2021 18:49:45 GMT
ENV NATS_STREAMING_SERVER=0.22.1
# Wed, 15 Sep 2021 18:49:46 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.22.1/nats-streaming-server-v0.22.1-windows-amd64.zip
# Wed, 15 Sep 2021 18:49:47 GMT
ENV NATS_STREAMING_SERVER_SHASUM=4516852b493111b73ec06477be4a27e66f5abc9ca1ff4dd2b970232271611264
# Wed, 15 Sep 2021 18:50:28 GMT
RUN Set-PSDebug -Trace 2
# Wed, 15 Sep 2021 18:51:48 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 15 Sep 2021 18:51:49 GMT
EXPOSE 4222 8222
# Wed, 15 Sep 2021 18:51:49 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 15 Sep 2021 18:51:50 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a0ddf88812f10c7d6edc858aa9784ff5ca9de4a7bb631909c090090343abd059`  
		Size: 968.4 MB (968365008 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:6c4091e033b8590db7b89fded6d31ac2224162744daa4d7a7a66cbebd4b8c228`  
		Last Modified: Wed, 15 Sep 2021 15:04:44 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c75402e6fab70f623ca8becfa5bb563e5630bbb4dac8adb11e385d75e171aed`  
		Last Modified: Wed, 15 Sep 2021 15:45:53 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffaf075a271862d4bc05568114cc4eeb60f8de9ba30ac6e3fe5355849d4000cd`  
		Last Modified: Wed, 15 Sep 2021 18:54:52 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4835bde54170d4fcd660b52c8dfed238e8f2ab963f2a9285e591fe7115fa2283`  
		Last Modified: Wed, 15 Sep 2021 18:54:51 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c477ff70b750b36312766e21da88df14a9d42d6926bf3e30ba1c64308b163d8a`  
		Last Modified: Wed, 15 Sep 2021 18:54:51 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcc35663cd24c79f3cf7d67b95f50e510f509c986a1743d126193cb8838145e6`  
		Last Modified: Wed, 15 Sep 2021 18:54:49 GMT  
		Size: 349.2 KB (349224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4772ba9bdad7c934060bfc5561978af7dcccb05ea78ebb2ccbf13749d804db1`  
		Last Modified: Wed, 15 Sep 2021 18:54:51 GMT  
		Size: 7.6 MB (7625617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:000708a1ba81b80dbbfebe82d875a1116e8ad8659232936d8b5c19710445658c`  
		Last Modified: Wed, 15 Sep 2021 18:54:49 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a977d7698cf7e509b59d133fe3f5c720b1ac86dd8c0e4ced1e82c548c4cfd47`  
		Last Modified: Wed, 15 Sep 2021 18:54:49 GMT  
		Size: 1.3 KB (1327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3653acfe476962adc853584e37df0eddc16574f7588d42731309f7b95aa9f315`  
		Last Modified: Wed, 15 Sep 2021 18:54:49 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.22.1-windowsservercore` - windows version 10.0.14393.4651; amd64

```console
$ docker pull nats-streaming@sha256:db420b05307ebc5425e2ed494fe11c71977ae9644d6cc08cea9a32388a8f92f9
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6279315014 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9224e56def9350d516ffcf46c72c2fe923a1e699e78612f8f084568b4a884b93`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 13 Sep 2021 01:03:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 15 Sep 2021 13:26:09 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 15 Sep 2021 15:43:15 GMT
ENV NATS_DOCKERIZED=1
# Wed, 15 Sep 2021 18:52:05 GMT
ENV NATS_STREAMING_SERVER=0.22.1
# Wed, 15 Sep 2021 18:52:06 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.22.1/nats-streaming-server-v0.22.1-windows-amd64.zip
# Wed, 15 Sep 2021 18:52:07 GMT
ENV NATS_STREAMING_SERVER_SHASUM=4516852b493111b73ec06477be4a27e66f5abc9ca1ff4dd2b970232271611264
# Wed, 15 Sep 2021 18:52:47 GMT
RUN Set-PSDebug -Trace 2
# Wed, 15 Sep 2021 18:54:15 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 15 Sep 2021 18:54:16 GMT
EXPOSE 4222 8222
# Wed, 15 Sep 2021 18:54:17 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 15 Sep 2021 18:54:18 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e9b8281bf21e46c781fb54e4f15f5728e2c44dea4219c9e6deeb732f1d909d3b`  
		Size: 2.2 GB (2201342322 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5796468f91731000e9a76e836156826a1cd4ed963bcd80e6558c538a12c2132d`  
		Last Modified: Wed, 15 Sep 2021 15:05:15 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:611fe9c559abed986280087eef7d362a6ecb9ad281b1427395fdfc2d99d3d9c4`  
		Last Modified: Wed, 15 Sep 2021 15:46:29 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cc80b5d1ce6897bdd090b01daa650e63019faa977ef23c8248e4ab254310830`  
		Last Modified: Wed, 15 Sep 2021 18:55:26 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be2342d91ff82328bf8ba622555f8083b3c2311603f49e600e921a3b424852ec`  
		Last Modified: Wed, 15 Sep 2021 18:55:25 GMT  
		Size: 1.3 KB (1296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f61c2209638a7d2ded082cb0eb17bd8856f27d50a02eadc7a623429f008fe26`  
		Last Modified: Wed, 15 Sep 2021 18:55:25 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df5019f36414f6f8aee86294793001d1cdf5631d45a6901646229fc1e85e01c2`  
		Last Modified: Wed, 15 Sep 2021 18:55:23 GMT  
		Size: 332.6 KB (332556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f748d4a8c2babe5e9ba487dbb17fcec2eeed0dcd1ce7b3e11d8ed12adeb75d1`  
		Last Modified: Wed, 15 Sep 2021 18:55:31 GMT  
		Size: 7.6 MB (7643649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4386a8452b0b6cfe5bb3563f552cfcfa025a77c50e0b7b383f486c6609b8e3b`  
		Last Modified: Wed, 15 Sep 2021 18:55:23 GMT  
		Size: 1.3 KB (1325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20c1401d40019edc4f2a3ba3ccbdd1c088c2f1e28bfa1d2255721cd3ff172d43`  
		Last Modified: Wed, 15 Sep 2021 18:55:23 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:207050f1ea57a9f8edae4f5caead9eb05022d7428e2b17637b719213bce914a4`  
		Last Modified: Wed, 15 Sep 2021 18:55:23 GMT  
		Size: 1.3 KB (1302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.22.1-windowsservercore-1809`

```console
$ docker pull nats-streaming@sha256:2e38de84651e01073fb06b20a95117b46cb69db1b1173946ad98503097ab5df2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2183; amd64

### `nats-streaming:0.22.1-windowsservercore-1809` - windows version 10.0.17763.2183; amd64

```console
$ docker pull nats-streaming@sha256:48f5ee8c66860f96f1851945d34a317b4038c171a4fc036953bd45e22ae600b8
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2694683224 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03cd19bbfbdb07be71a6322be26c8f7fce0969a83528b4755cf4c72f694719ed`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 13 Sep 2021 04:08:33 GMT
RUN Install update 1809-amd64
# Wed, 15 Sep 2021 13:14:12 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 15 Sep 2021 15:40:54 GMT
ENV NATS_DOCKERIZED=1
# Wed, 15 Sep 2021 18:49:45 GMT
ENV NATS_STREAMING_SERVER=0.22.1
# Wed, 15 Sep 2021 18:49:46 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.22.1/nats-streaming-server-v0.22.1-windows-amd64.zip
# Wed, 15 Sep 2021 18:49:47 GMT
ENV NATS_STREAMING_SERVER_SHASUM=4516852b493111b73ec06477be4a27e66f5abc9ca1ff4dd2b970232271611264
# Wed, 15 Sep 2021 18:50:28 GMT
RUN Set-PSDebug -Trace 2
# Wed, 15 Sep 2021 18:51:48 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 15 Sep 2021 18:51:49 GMT
EXPOSE 4222 8222
# Wed, 15 Sep 2021 18:51:49 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 15 Sep 2021 18:51:50 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a0ddf88812f10c7d6edc858aa9784ff5ca9de4a7bb631909c090090343abd059`  
		Size: 968.4 MB (968365008 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:6c4091e033b8590db7b89fded6d31ac2224162744daa4d7a7a66cbebd4b8c228`  
		Last Modified: Wed, 15 Sep 2021 15:04:44 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c75402e6fab70f623ca8becfa5bb563e5630bbb4dac8adb11e385d75e171aed`  
		Last Modified: Wed, 15 Sep 2021 15:45:53 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffaf075a271862d4bc05568114cc4eeb60f8de9ba30ac6e3fe5355849d4000cd`  
		Last Modified: Wed, 15 Sep 2021 18:54:52 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4835bde54170d4fcd660b52c8dfed238e8f2ab963f2a9285e591fe7115fa2283`  
		Last Modified: Wed, 15 Sep 2021 18:54:51 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c477ff70b750b36312766e21da88df14a9d42d6926bf3e30ba1c64308b163d8a`  
		Last Modified: Wed, 15 Sep 2021 18:54:51 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcc35663cd24c79f3cf7d67b95f50e510f509c986a1743d126193cb8838145e6`  
		Last Modified: Wed, 15 Sep 2021 18:54:49 GMT  
		Size: 349.2 KB (349224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4772ba9bdad7c934060bfc5561978af7dcccb05ea78ebb2ccbf13749d804db1`  
		Last Modified: Wed, 15 Sep 2021 18:54:51 GMT  
		Size: 7.6 MB (7625617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:000708a1ba81b80dbbfebe82d875a1116e8ad8659232936d8b5c19710445658c`  
		Last Modified: Wed, 15 Sep 2021 18:54:49 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a977d7698cf7e509b59d133fe3f5c720b1ac86dd8c0e4ced1e82c548c4cfd47`  
		Last Modified: Wed, 15 Sep 2021 18:54:49 GMT  
		Size: 1.3 KB (1327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3653acfe476962adc853584e37df0eddc16574f7588d42731309f7b95aa9f315`  
		Last Modified: Wed, 15 Sep 2021 18:54:49 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.22.1-windowsservercore-ltsc2016`

```console
$ docker pull nats-streaming@sha256:2355a62bb57d76c5ec35a02432c7c159489e6739f13c2249af33a1257cf55b65
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.14393.4651; amd64

### `nats-streaming:0.22.1-windowsservercore-ltsc2016` - windows version 10.0.14393.4651; amd64

```console
$ docker pull nats-streaming@sha256:db420b05307ebc5425e2ed494fe11c71977ae9644d6cc08cea9a32388a8f92f9
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6279315014 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9224e56def9350d516ffcf46c72c2fe923a1e699e78612f8f084568b4a884b93`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 13 Sep 2021 01:03:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 15 Sep 2021 13:26:09 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 15 Sep 2021 15:43:15 GMT
ENV NATS_DOCKERIZED=1
# Wed, 15 Sep 2021 18:52:05 GMT
ENV NATS_STREAMING_SERVER=0.22.1
# Wed, 15 Sep 2021 18:52:06 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.22.1/nats-streaming-server-v0.22.1-windows-amd64.zip
# Wed, 15 Sep 2021 18:52:07 GMT
ENV NATS_STREAMING_SERVER_SHASUM=4516852b493111b73ec06477be4a27e66f5abc9ca1ff4dd2b970232271611264
# Wed, 15 Sep 2021 18:52:47 GMT
RUN Set-PSDebug -Trace 2
# Wed, 15 Sep 2021 18:54:15 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 15 Sep 2021 18:54:16 GMT
EXPOSE 4222 8222
# Wed, 15 Sep 2021 18:54:17 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 15 Sep 2021 18:54:18 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e9b8281bf21e46c781fb54e4f15f5728e2c44dea4219c9e6deeb732f1d909d3b`  
		Size: 2.2 GB (2201342322 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5796468f91731000e9a76e836156826a1cd4ed963bcd80e6558c538a12c2132d`  
		Last Modified: Wed, 15 Sep 2021 15:05:15 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:611fe9c559abed986280087eef7d362a6ecb9ad281b1427395fdfc2d99d3d9c4`  
		Last Modified: Wed, 15 Sep 2021 15:46:29 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cc80b5d1ce6897bdd090b01daa650e63019faa977ef23c8248e4ab254310830`  
		Last Modified: Wed, 15 Sep 2021 18:55:26 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be2342d91ff82328bf8ba622555f8083b3c2311603f49e600e921a3b424852ec`  
		Last Modified: Wed, 15 Sep 2021 18:55:25 GMT  
		Size: 1.3 KB (1296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f61c2209638a7d2ded082cb0eb17bd8856f27d50a02eadc7a623429f008fe26`  
		Last Modified: Wed, 15 Sep 2021 18:55:25 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df5019f36414f6f8aee86294793001d1cdf5631d45a6901646229fc1e85e01c2`  
		Last Modified: Wed, 15 Sep 2021 18:55:23 GMT  
		Size: 332.6 KB (332556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f748d4a8c2babe5e9ba487dbb17fcec2eeed0dcd1ce7b3e11d8ed12adeb75d1`  
		Last Modified: Wed, 15 Sep 2021 18:55:31 GMT  
		Size: 7.6 MB (7643649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4386a8452b0b6cfe5bb3563f552cfcfa025a77c50e0b7b383f486c6609b8e3b`  
		Last Modified: Wed, 15 Sep 2021 18:55:23 GMT  
		Size: 1.3 KB (1325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20c1401d40019edc4f2a3ba3ccbdd1c088c2f1e28bfa1d2255721cd3ff172d43`  
		Last Modified: Wed, 15 Sep 2021 18:55:23 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:207050f1ea57a9f8edae4f5caead9eb05022d7428e2b17637b719213bce914a4`  
		Last Modified: Wed, 15 Sep 2021 18:55:23 GMT  
		Size: 1.3 KB (1302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.22-alpine`

```console
$ docker pull nats-streaming@sha256:faa20055417a6b6df8cfc690c34b132b3291b66699d13be2be328d2682c2e0e0
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
$ docker pull nats-streaming@sha256:709bf964baa04bed21788daab878aaf76613f67b25782dfa91f68dac883c1e96
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.4 MB (9352403 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:120c9c54d0d41980417a67786d13b07474948f1a4fe697b1bfe029344e8b5d55`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 27 Aug 2021 17:57:31 GMT
ADD file:a7da7992ccea54d3295231027614f138aa45c4d4a25ea6ec9bf7b316b9f67d95 in / 
# Fri, 27 Aug 2021 17:57:32 GMT
CMD ["/bin/sh"]
# Fri, 27 Aug 2021 21:15:57 GMT
ENV NATS_STREAMING_SERVER=0.22.1
# Fri, 27 Aug 2021 21:16:03 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='581698d248a19ecae64e4048d153bc1021744a3da6284680a339f9f82a53a9cf' ;; 		armhf) natsArch='arm6'; sha256='438a89221bb0608e40d21e73ca27a4b70b8560730726942c0ade94a6b6013d6f' ;; 		armv7) natsArch='arm7'; sha256='4164baadd201d1374f7654d3e54a24d81ceb87a385867e31a82c1d1a69e3b1ae' ;; 		x86_64) natsArch='amd64'; sha256='f29e87ac9ff998c928aa8ebc8cf0c4d04d34a3d95b9900d92fd7dafab2bec8cc' ;; 		x86) natsArch='386'; sha256='0ca68e57babb8901d7afeb7569042730904887e718ddf860ef3ee54278753505' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 27 Aug 2021 21:16:03 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Fri, 27 Aug 2021 21:16:04 GMT
EXPOSE 4222 8222
# Fri, 27 Aug 2021 21:16:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 Aug 2021 21:16:05 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:a14774a5a62e0f454febaec7cb603e18a6a8e25ef9da4a4da85b155bdd5e5a7a`  
		Last Modified: Fri, 27 Aug 2021 17:59:00 GMT  
		Size: 2.4 MB (2430419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7d0e8657e131875280f89b03741d9c7b5b154791cef8ce515fe711e4185a32d`  
		Last Modified: Fri, 27 Aug 2021 21:17:51 GMT  
		Size: 6.9 MB (6921563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20506d2b8361ef74d3f9c4e5dc7489f829d0181c070aca1b163eb8f540762e4c`  
		Last Modified: Fri, 27 Aug 2021 21:17:47 GMT  
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
$ docker pull nats-streaming@sha256:faa20055417a6b6df8cfc690c34b132b3291b66699d13be2be328d2682c2e0e0
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
$ docker pull nats-streaming@sha256:709bf964baa04bed21788daab878aaf76613f67b25782dfa91f68dac883c1e96
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.4 MB (9352403 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:120c9c54d0d41980417a67786d13b07474948f1a4fe697b1bfe029344e8b5d55`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 27 Aug 2021 17:57:31 GMT
ADD file:a7da7992ccea54d3295231027614f138aa45c4d4a25ea6ec9bf7b316b9f67d95 in / 
# Fri, 27 Aug 2021 17:57:32 GMT
CMD ["/bin/sh"]
# Fri, 27 Aug 2021 21:15:57 GMT
ENV NATS_STREAMING_SERVER=0.22.1
# Fri, 27 Aug 2021 21:16:03 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='581698d248a19ecae64e4048d153bc1021744a3da6284680a339f9f82a53a9cf' ;; 		armhf) natsArch='arm6'; sha256='438a89221bb0608e40d21e73ca27a4b70b8560730726942c0ade94a6b6013d6f' ;; 		armv7) natsArch='arm7'; sha256='4164baadd201d1374f7654d3e54a24d81ceb87a385867e31a82c1d1a69e3b1ae' ;; 		x86_64) natsArch='amd64'; sha256='f29e87ac9ff998c928aa8ebc8cf0c4d04d34a3d95b9900d92fd7dafab2bec8cc' ;; 		x86) natsArch='386'; sha256='0ca68e57babb8901d7afeb7569042730904887e718ddf860ef3ee54278753505' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 27 Aug 2021 21:16:03 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Fri, 27 Aug 2021 21:16:04 GMT
EXPOSE 4222 8222
# Fri, 27 Aug 2021 21:16:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 Aug 2021 21:16:05 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:a14774a5a62e0f454febaec7cb603e18a6a8e25ef9da4a4da85b155bdd5e5a7a`  
		Last Modified: Fri, 27 Aug 2021 17:59:00 GMT  
		Size: 2.4 MB (2430419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7d0e8657e131875280f89b03741d9c7b5b154791cef8ce515fe711e4185a32d`  
		Last Modified: Fri, 27 Aug 2021 21:17:51 GMT  
		Size: 6.9 MB (6921563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20506d2b8361ef74d3f9c4e5dc7489f829d0181c070aca1b163eb8f540762e4c`  
		Last Modified: Fri, 27 Aug 2021 21:17:47 GMT  
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
$ docker pull nats-streaming@sha256:d825481c4d8339d300a56d9f3eeaecf48ae0c071064bfa5ccfb1d9393ff52765
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2183; amd64

### `nats-streaming:0.22-nanoserver` - windows version 10.0.17763.2183; amd64

```console
$ docker pull nats-streaming@sha256:f7300d49f73a0e5451f68fcf439d1e5b75b5a891aa04e8ff537b523b15d45fc6
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.0 MB (110001330 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa93dcd937d8cd2009cb8f123551ce0f46c671f91465df126ce8475110a4f6cd`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 13 Sep 2021 03:45:12 GMT
RUN Apply image 1809-amd64
# Wed, 15 Sep 2021 15:43:05 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 15 Sep 2021 18:51:57 GMT
RUN cmd /S /C #(nop) COPY file:9670e5d1fe5a71e47c78fde01235a0bcbcafcfdeeacf96a7669f6e49343fb03b in C:\nats-streaming-server.exe 
# Wed, 15 Sep 2021 18:51:58 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 15 Sep 2021 18:51:59 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 15 Sep 2021 18:51:59 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:3585a81ca503e6c63dce938a5606f4171d7461e51000a92054b3f5692786d6c9`  
		Size: 102.7 MB (102703785 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:66dbf96361e9ec1f64f66e255a947eab476edef46c3f9a3b4ede943fa8b87699`  
		Last Modified: Wed, 15 Sep 2021 15:46:11 GMT  
		Size: 1.1 KB (1089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07e5a8a8a1823e7ab1aab125064b8d7d94f6dacefba9d82b815174cb4c32a833`  
		Last Modified: Wed, 15 Sep 2021 18:55:12 GMT  
		Size: 7.3 MB (7293261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16df1d39830ccb4fa2828c96b6c6ec476f1f3a292bdbd01053a21c6c9457750b`  
		Last Modified: Wed, 15 Sep 2021 18:55:04 GMT  
		Size: 1.1 KB (1114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43f99c367ebf7f75f5e675f26e18195abf8826890c87d26039e2c58b38a681d6`  
		Last Modified: Wed, 15 Sep 2021 18:55:04 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3052f7738f8821f9a96f777624d74a7b0b9c7fe0bcecce51d3586ea05479556d`  
		Last Modified: Wed, 15 Sep 2021 18:55:04 GMT  
		Size: 1.0 KB (1030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.22-nanoserver-1809`

```console
$ docker pull nats-streaming@sha256:d825481c4d8339d300a56d9f3eeaecf48ae0c071064bfa5ccfb1d9393ff52765
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2183; amd64

### `nats-streaming:0.22-nanoserver-1809` - windows version 10.0.17763.2183; amd64

```console
$ docker pull nats-streaming@sha256:f7300d49f73a0e5451f68fcf439d1e5b75b5a891aa04e8ff537b523b15d45fc6
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.0 MB (110001330 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa93dcd937d8cd2009cb8f123551ce0f46c671f91465df126ce8475110a4f6cd`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 13 Sep 2021 03:45:12 GMT
RUN Apply image 1809-amd64
# Wed, 15 Sep 2021 15:43:05 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 15 Sep 2021 18:51:57 GMT
RUN cmd /S /C #(nop) COPY file:9670e5d1fe5a71e47c78fde01235a0bcbcafcfdeeacf96a7669f6e49343fb03b in C:\nats-streaming-server.exe 
# Wed, 15 Sep 2021 18:51:58 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 15 Sep 2021 18:51:59 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 15 Sep 2021 18:51:59 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:3585a81ca503e6c63dce938a5606f4171d7461e51000a92054b3f5692786d6c9`  
		Size: 102.7 MB (102703785 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:66dbf96361e9ec1f64f66e255a947eab476edef46c3f9a3b4ede943fa8b87699`  
		Last Modified: Wed, 15 Sep 2021 15:46:11 GMT  
		Size: 1.1 KB (1089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07e5a8a8a1823e7ab1aab125064b8d7d94f6dacefba9d82b815174cb4c32a833`  
		Last Modified: Wed, 15 Sep 2021 18:55:12 GMT  
		Size: 7.3 MB (7293261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16df1d39830ccb4fa2828c96b6c6ec476f1f3a292bdbd01053a21c6c9457750b`  
		Last Modified: Wed, 15 Sep 2021 18:55:04 GMT  
		Size: 1.1 KB (1114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43f99c367ebf7f75f5e675f26e18195abf8826890c87d26039e2c58b38a681d6`  
		Last Modified: Wed, 15 Sep 2021 18:55:04 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3052f7738f8821f9a96f777624d74a7b0b9c7fe0bcecce51d3586ea05479556d`  
		Last Modified: Wed, 15 Sep 2021 18:55:04 GMT  
		Size: 1.0 KB (1030 bytes)  
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
$ docker pull nats-streaming@sha256:216e97a64fbe21529831ff1ddac989c2147fe68298359fb82b1c304153c9f38a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.2183; amd64
	-	windows version 10.0.14393.4651; amd64

### `nats-streaming:0.22-windowsservercore` - windows version 10.0.17763.2183; amd64

```console
$ docker pull nats-streaming@sha256:48f5ee8c66860f96f1851945d34a317b4038c171a4fc036953bd45e22ae600b8
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2694683224 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03cd19bbfbdb07be71a6322be26c8f7fce0969a83528b4755cf4c72f694719ed`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 13 Sep 2021 04:08:33 GMT
RUN Install update 1809-amd64
# Wed, 15 Sep 2021 13:14:12 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 15 Sep 2021 15:40:54 GMT
ENV NATS_DOCKERIZED=1
# Wed, 15 Sep 2021 18:49:45 GMT
ENV NATS_STREAMING_SERVER=0.22.1
# Wed, 15 Sep 2021 18:49:46 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.22.1/nats-streaming-server-v0.22.1-windows-amd64.zip
# Wed, 15 Sep 2021 18:49:47 GMT
ENV NATS_STREAMING_SERVER_SHASUM=4516852b493111b73ec06477be4a27e66f5abc9ca1ff4dd2b970232271611264
# Wed, 15 Sep 2021 18:50:28 GMT
RUN Set-PSDebug -Trace 2
# Wed, 15 Sep 2021 18:51:48 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 15 Sep 2021 18:51:49 GMT
EXPOSE 4222 8222
# Wed, 15 Sep 2021 18:51:49 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 15 Sep 2021 18:51:50 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a0ddf88812f10c7d6edc858aa9784ff5ca9de4a7bb631909c090090343abd059`  
		Size: 968.4 MB (968365008 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:6c4091e033b8590db7b89fded6d31ac2224162744daa4d7a7a66cbebd4b8c228`  
		Last Modified: Wed, 15 Sep 2021 15:04:44 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c75402e6fab70f623ca8becfa5bb563e5630bbb4dac8adb11e385d75e171aed`  
		Last Modified: Wed, 15 Sep 2021 15:45:53 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffaf075a271862d4bc05568114cc4eeb60f8de9ba30ac6e3fe5355849d4000cd`  
		Last Modified: Wed, 15 Sep 2021 18:54:52 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4835bde54170d4fcd660b52c8dfed238e8f2ab963f2a9285e591fe7115fa2283`  
		Last Modified: Wed, 15 Sep 2021 18:54:51 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c477ff70b750b36312766e21da88df14a9d42d6926bf3e30ba1c64308b163d8a`  
		Last Modified: Wed, 15 Sep 2021 18:54:51 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcc35663cd24c79f3cf7d67b95f50e510f509c986a1743d126193cb8838145e6`  
		Last Modified: Wed, 15 Sep 2021 18:54:49 GMT  
		Size: 349.2 KB (349224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4772ba9bdad7c934060bfc5561978af7dcccb05ea78ebb2ccbf13749d804db1`  
		Last Modified: Wed, 15 Sep 2021 18:54:51 GMT  
		Size: 7.6 MB (7625617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:000708a1ba81b80dbbfebe82d875a1116e8ad8659232936d8b5c19710445658c`  
		Last Modified: Wed, 15 Sep 2021 18:54:49 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a977d7698cf7e509b59d133fe3f5c720b1ac86dd8c0e4ced1e82c548c4cfd47`  
		Last Modified: Wed, 15 Sep 2021 18:54:49 GMT  
		Size: 1.3 KB (1327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3653acfe476962adc853584e37df0eddc16574f7588d42731309f7b95aa9f315`  
		Last Modified: Wed, 15 Sep 2021 18:54:49 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.22-windowsservercore` - windows version 10.0.14393.4651; amd64

```console
$ docker pull nats-streaming@sha256:db420b05307ebc5425e2ed494fe11c71977ae9644d6cc08cea9a32388a8f92f9
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6279315014 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9224e56def9350d516ffcf46c72c2fe923a1e699e78612f8f084568b4a884b93`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 13 Sep 2021 01:03:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 15 Sep 2021 13:26:09 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 15 Sep 2021 15:43:15 GMT
ENV NATS_DOCKERIZED=1
# Wed, 15 Sep 2021 18:52:05 GMT
ENV NATS_STREAMING_SERVER=0.22.1
# Wed, 15 Sep 2021 18:52:06 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.22.1/nats-streaming-server-v0.22.1-windows-amd64.zip
# Wed, 15 Sep 2021 18:52:07 GMT
ENV NATS_STREAMING_SERVER_SHASUM=4516852b493111b73ec06477be4a27e66f5abc9ca1ff4dd2b970232271611264
# Wed, 15 Sep 2021 18:52:47 GMT
RUN Set-PSDebug -Trace 2
# Wed, 15 Sep 2021 18:54:15 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 15 Sep 2021 18:54:16 GMT
EXPOSE 4222 8222
# Wed, 15 Sep 2021 18:54:17 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 15 Sep 2021 18:54:18 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e9b8281bf21e46c781fb54e4f15f5728e2c44dea4219c9e6deeb732f1d909d3b`  
		Size: 2.2 GB (2201342322 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5796468f91731000e9a76e836156826a1cd4ed963bcd80e6558c538a12c2132d`  
		Last Modified: Wed, 15 Sep 2021 15:05:15 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:611fe9c559abed986280087eef7d362a6ecb9ad281b1427395fdfc2d99d3d9c4`  
		Last Modified: Wed, 15 Sep 2021 15:46:29 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cc80b5d1ce6897bdd090b01daa650e63019faa977ef23c8248e4ab254310830`  
		Last Modified: Wed, 15 Sep 2021 18:55:26 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be2342d91ff82328bf8ba622555f8083b3c2311603f49e600e921a3b424852ec`  
		Last Modified: Wed, 15 Sep 2021 18:55:25 GMT  
		Size: 1.3 KB (1296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f61c2209638a7d2ded082cb0eb17bd8856f27d50a02eadc7a623429f008fe26`  
		Last Modified: Wed, 15 Sep 2021 18:55:25 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df5019f36414f6f8aee86294793001d1cdf5631d45a6901646229fc1e85e01c2`  
		Last Modified: Wed, 15 Sep 2021 18:55:23 GMT  
		Size: 332.6 KB (332556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f748d4a8c2babe5e9ba487dbb17fcec2eeed0dcd1ce7b3e11d8ed12adeb75d1`  
		Last Modified: Wed, 15 Sep 2021 18:55:31 GMT  
		Size: 7.6 MB (7643649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4386a8452b0b6cfe5bb3563f552cfcfa025a77c50e0b7b383f486c6609b8e3b`  
		Last Modified: Wed, 15 Sep 2021 18:55:23 GMT  
		Size: 1.3 KB (1325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20c1401d40019edc4f2a3ba3ccbdd1c088c2f1e28bfa1d2255721cd3ff172d43`  
		Last Modified: Wed, 15 Sep 2021 18:55:23 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:207050f1ea57a9f8edae4f5caead9eb05022d7428e2b17637b719213bce914a4`  
		Last Modified: Wed, 15 Sep 2021 18:55:23 GMT  
		Size: 1.3 KB (1302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.22-windowsservercore-1809`

```console
$ docker pull nats-streaming@sha256:2e38de84651e01073fb06b20a95117b46cb69db1b1173946ad98503097ab5df2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2183; amd64

### `nats-streaming:0.22-windowsservercore-1809` - windows version 10.0.17763.2183; amd64

```console
$ docker pull nats-streaming@sha256:48f5ee8c66860f96f1851945d34a317b4038c171a4fc036953bd45e22ae600b8
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2694683224 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03cd19bbfbdb07be71a6322be26c8f7fce0969a83528b4755cf4c72f694719ed`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 13 Sep 2021 04:08:33 GMT
RUN Install update 1809-amd64
# Wed, 15 Sep 2021 13:14:12 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 15 Sep 2021 15:40:54 GMT
ENV NATS_DOCKERIZED=1
# Wed, 15 Sep 2021 18:49:45 GMT
ENV NATS_STREAMING_SERVER=0.22.1
# Wed, 15 Sep 2021 18:49:46 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.22.1/nats-streaming-server-v0.22.1-windows-amd64.zip
# Wed, 15 Sep 2021 18:49:47 GMT
ENV NATS_STREAMING_SERVER_SHASUM=4516852b493111b73ec06477be4a27e66f5abc9ca1ff4dd2b970232271611264
# Wed, 15 Sep 2021 18:50:28 GMT
RUN Set-PSDebug -Trace 2
# Wed, 15 Sep 2021 18:51:48 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 15 Sep 2021 18:51:49 GMT
EXPOSE 4222 8222
# Wed, 15 Sep 2021 18:51:49 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 15 Sep 2021 18:51:50 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a0ddf88812f10c7d6edc858aa9784ff5ca9de4a7bb631909c090090343abd059`  
		Size: 968.4 MB (968365008 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:6c4091e033b8590db7b89fded6d31ac2224162744daa4d7a7a66cbebd4b8c228`  
		Last Modified: Wed, 15 Sep 2021 15:04:44 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c75402e6fab70f623ca8becfa5bb563e5630bbb4dac8adb11e385d75e171aed`  
		Last Modified: Wed, 15 Sep 2021 15:45:53 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffaf075a271862d4bc05568114cc4eeb60f8de9ba30ac6e3fe5355849d4000cd`  
		Last Modified: Wed, 15 Sep 2021 18:54:52 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4835bde54170d4fcd660b52c8dfed238e8f2ab963f2a9285e591fe7115fa2283`  
		Last Modified: Wed, 15 Sep 2021 18:54:51 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c477ff70b750b36312766e21da88df14a9d42d6926bf3e30ba1c64308b163d8a`  
		Last Modified: Wed, 15 Sep 2021 18:54:51 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcc35663cd24c79f3cf7d67b95f50e510f509c986a1743d126193cb8838145e6`  
		Last Modified: Wed, 15 Sep 2021 18:54:49 GMT  
		Size: 349.2 KB (349224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4772ba9bdad7c934060bfc5561978af7dcccb05ea78ebb2ccbf13749d804db1`  
		Last Modified: Wed, 15 Sep 2021 18:54:51 GMT  
		Size: 7.6 MB (7625617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:000708a1ba81b80dbbfebe82d875a1116e8ad8659232936d8b5c19710445658c`  
		Last Modified: Wed, 15 Sep 2021 18:54:49 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a977d7698cf7e509b59d133fe3f5c720b1ac86dd8c0e4ced1e82c548c4cfd47`  
		Last Modified: Wed, 15 Sep 2021 18:54:49 GMT  
		Size: 1.3 KB (1327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3653acfe476962adc853584e37df0eddc16574f7588d42731309f7b95aa9f315`  
		Last Modified: Wed, 15 Sep 2021 18:54:49 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.22-windowsservercore-ltsc2016`

```console
$ docker pull nats-streaming@sha256:2355a62bb57d76c5ec35a02432c7c159489e6739f13c2249af33a1257cf55b65
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.14393.4651; amd64

### `nats-streaming:0.22-windowsservercore-ltsc2016` - windows version 10.0.14393.4651; amd64

```console
$ docker pull nats-streaming@sha256:db420b05307ebc5425e2ed494fe11c71977ae9644d6cc08cea9a32388a8f92f9
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6279315014 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9224e56def9350d516ffcf46c72c2fe923a1e699e78612f8f084568b4a884b93`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 13 Sep 2021 01:03:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 15 Sep 2021 13:26:09 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 15 Sep 2021 15:43:15 GMT
ENV NATS_DOCKERIZED=1
# Wed, 15 Sep 2021 18:52:05 GMT
ENV NATS_STREAMING_SERVER=0.22.1
# Wed, 15 Sep 2021 18:52:06 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.22.1/nats-streaming-server-v0.22.1-windows-amd64.zip
# Wed, 15 Sep 2021 18:52:07 GMT
ENV NATS_STREAMING_SERVER_SHASUM=4516852b493111b73ec06477be4a27e66f5abc9ca1ff4dd2b970232271611264
# Wed, 15 Sep 2021 18:52:47 GMT
RUN Set-PSDebug -Trace 2
# Wed, 15 Sep 2021 18:54:15 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 15 Sep 2021 18:54:16 GMT
EXPOSE 4222 8222
# Wed, 15 Sep 2021 18:54:17 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 15 Sep 2021 18:54:18 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e9b8281bf21e46c781fb54e4f15f5728e2c44dea4219c9e6deeb732f1d909d3b`  
		Size: 2.2 GB (2201342322 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5796468f91731000e9a76e836156826a1cd4ed963bcd80e6558c538a12c2132d`  
		Last Modified: Wed, 15 Sep 2021 15:05:15 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:611fe9c559abed986280087eef7d362a6ecb9ad281b1427395fdfc2d99d3d9c4`  
		Last Modified: Wed, 15 Sep 2021 15:46:29 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cc80b5d1ce6897bdd090b01daa650e63019faa977ef23c8248e4ab254310830`  
		Last Modified: Wed, 15 Sep 2021 18:55:26 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be2342d91ff82328bf8ba622555f8083b3c2311603f49e600e921a3b424852ec`  
		Last Modified: Wed, 15 Sep 2021 18:55:25 GMT  
		Size: 1.3 KB (1296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f61c2209638a7d2ded082cb0eb17bd8856f27d50a02eadc7a623429f008fe26`  
		Last Modified: Wed, 15 Sep 2021 18:55:25 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df5019f36414f6f8aee86294793001d1cdf5631d45a6901646229fc1e85e01c2`  
		Last Modified: Wed, 15 Sep 2021 18:55:23 GMT  
		Size: 332.6 KB (332556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f748d4a8c2babe5e9ba487dbb17fcec2eeed0dcd1ce7b3e11d8ed12adeb75d1`  
		Last Modified: Wed, 15 Sep 2021 18:55:31 GMT  
		Size: 7.6 MB (7643649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4386a8452b0b6cfe5bb3563f552cfcfa025a77c50e0b7b383f486c6609b8e3b`  
		Last Modified: Wed, 15 Sep 2021 18:55:23 GMT  
		Size: 1.3 KB (1325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20c1401d40019edc4f2a3ba3ccbdd1c088c2f1e28bfa1d2255721cd3ff172d43`  
		Last Modified: Wed, 15 Sep 2021 18:55:23 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:207050f1ea57a9f8edae4f5caead9eb05022d7428e2b17637b719213bce914a4`  
		Last Modified: Wed, 15 Sep 2021 18:55:23 GMT  
		Size: 1.3 KB (1302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:alpine`

```console
$ docker pull nats-streaming@sha256:faa20055417a6b6df8cfc690c34b132b3291b66699d13be2be328d2682c2e0e0
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
$ docker pull nats-streaming@sha256:709bf964baa04bed21788daab878aaf76613f67b25782dfa91f68dac883c1e96
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.4 MB (9352403 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:120c9c54d0d41980417a67786d13b07474948f1a4fe697b1bfe029344e8b5d55`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 27 Aug 2021 17:57:31 GMT
ADD file:a7da7992ccea54d3295231027614f138aa45c4d4a25ea6ec9bf7b316b9f67d95 in / 
# Fri, 27 Aug 2021 17:57:32 GMT
CMD ["/bin/sh"]
# Fri, 27 Aug 2021 21:15:57 GMT
ENV NATS_STREAMING_SERVER=0.22.1
# Fri, 27 Aug 2021 21:16:03 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='581698d248a19ecae64e4048d153bc1021744a3da6284680a339f9f82a53a9cf' ;; 		armhf) natsArch='arm6'; sha256='438a89221bb0608e40d21e73ca27a4b70b8560730726942c0ade94a6b6013d6f' ;; 		armv7) natsArch='arm7'; sha256='4164baadd201d1374f7654d3e54a24d81ceb87a385867e31a82c1d1a69e3b1ae' ;; 		x86_64) natsArch='amd64'; sha256='f29e87ac9ff998c928aa8ebc8cf0c4d04d34a3d95b9900d92fd7dafab2bec8cc' ;; 		x86) natsArch='386'; sha256='0ca68e57babb8901d7afeb7569042730904887e718ddf860ef3ee54278753505' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 27 Aug 2021 21:16:03 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Fri, 27 Aug 2021 21:16:04 GMT
EXPOSE 4222 8222
# Fri, 27 Aug 2021 21:16:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 Aug 2021 21:16:05 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:a14774a5a62e0f454febaec7cb603e18a6a8e25ef9da4a4da85b155bdd5e5a7a`  
		Last Modified: Fri, 27 Aug 2021 17:59:00 GMT  
		Size: 2.4 MB (2430419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7d0e8657e131875280f89b03741d9c7b5b154791cef8ce515fe711e4185a32d`  
		Last Modified: Fri, 27 Aug 2021 21:17:51 GMT  
		Size: 6.9 MB (6921563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20506d2b8361ef74d3f9c4e5dc7489f829d0181c070aca1b163eb8f540762e4c`  
		Last Modified: Fri, 27 Aug 2021 21:17:47 GMT  
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
$ docker pull nats-streaming@sha256:faa20055417a6b6df8cfc690c34b132b3291b66699d13be2be328d2682c2e0e0
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
$ docker pull nats-streaming@sha256:709bf964baa04bed21788daab878aaf76613f67b25782dfa91f68dac883c1e96
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.4 MB (9352403 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:120c9c54d0d41980417a67786d13b07474948f1a4fe697b1bfe029344e8b5d55`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 27 Aug 2021 17:57:31 GMT
ADD file:a7da7992ccea54d3295231027614f138aa45c4d4a25ea6ec9bf7b316b9f67d95 in / 
# Fri, 27 Aug 2021 17:57:32 GMT
CMD ["/bin/sh"]
# Fri, 27 Aug 2021 21:15:57 GMT
ENV NATS_STREAMING_SERVER=0.22.1
# Fri, 27 Aug 2021 21:16:03 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='581698d248a19ecae64e4048d153bc1021744a3da6284680a339f9f82a53a9cf' ;; 		armhf) natsArch='arm6'; sha256='438a89221bb0608e40d21e73ca27a4b70b8560730726942c0ade94a6b6013d6f' ;; 		armv7) natsArch='arm7'; sha256='4164baadd201d1374f7654d3e54a24d81ceb87a385867e31a82c1d1a69e3b1ae' ;; 		x86_64) natsArch='amd64'; sha256='f29e87ac9ff998c928aa8ebc8cf0c4d04d34a3d95b9900d92fd7dafab2bec8cc' ;; 		x86) natsArch='386'; sha256='0ca68e57babb8901d7afeb7569042730904887e718ddf860ef3ee54278753505' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 27 Aug 2021 21:16:03 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Fri, 27 Aug 2021 21:16:04 GMT
EXPOSE 4222 8222
# Fri, 27 Aug 2021 21:16:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 Aug 2021 21:16:05 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:a14774a5a62e0f454febaec7cb603e18a6a8e25ef9da4a4da85b155bdd5e5a7a`  
		Last Modified: Fri, 27 Aug 2021 17:59:00 GMT  
		Size: 2.4 MB (2430419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7d0e8657e131875280f89b03741d9c7b5b154791cef8ce515fe711e4185a32d`  
		Last Modified: Fri, 27 Aug 2021 21:17:51 GMT  
		Size: 6.9 MB (6921563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20506d2b8361ef74d3f9c4e5dc7489f829d0181c070aca1b163eb8f540762e4c`  
		Last Modified: Fri, 27 Aug 2021 21:17:47 GMT  
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
$ docker pull nats-streaming@sha256:42ec681f33c9c9fd6737322526f566c8c54f969e6d2db09591645ad26990b30e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.2183; amd64

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

### `nats-streaming:latest` - windows version 10.0.17763.2183; amd64

```console
$ docker pull nats-streaming@sha256:f7300d49f73a0e5451f68fcf439d1e5b75b5a891aa04e8ff537b523b15d45fc6
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.0 MB (110001330 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa93dcd937d8cd2009cb8f123551ce0f46c671f91465df126ce8475110a4f6cd`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 13 Sep 2021 03:45:12 GMT
RUN Apply image 1809-amd64
# Wed, 15 Sep 2021 15:43:05 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 15 Sep 2021 18:51:57 GMT
RUN cmd /S /C #(nop) COPY file:9670e5d1fe5a71e47c78fde01235a0bcbcafcfdeeacf96a7669f6e49343fb03b in C:\nats-streaming-server.exe 
# Wed, 15 Sep 2021 18:51:58 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 15 Sep 2021 18:51:59 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 15 Sep 2021 18:51:59 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:3585a81ca503e6c63dce938a5606f4171d7461e51000a92054b3f5692786d6c9`  
		Size: 102.7 MB (102703785 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:66dbf96361e9ec1f64f66e255a947eab476edef46c3f9a3b4ede943fa8b87699`  
		Last Modified: Wed, 15 Sep 2021 15:46:11 GMT  
		Size: 1.1 KB (1089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07e5a8a8a1823e7ab1aab125064b8d7d94f6dacefba9d82b815174cb4c32a833`  
		Last Modified: Wed, 15 Sep 2021 18:55:12 GMT  
		Size: 7.3 MB (7293261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16df1d39830ccb4fa2828c96b6c6ec476f1f3a292bdbd01053a21c6c9457750b`  
		Last Modified: Wed, 15 Sep 2021 18:55:04 GMT  
		Size: 1.1 KB (1114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43f99c367ebf7f75f5e675f26e18195abf8826890c87d26039e2c58b38a681d6`  
		Last Modified: Wed, 15 Sep 2021 18:55:04 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3052f7738f8821f9a96f777624d74a7b0b9c7fe0bcecce51d3586ea05479556d`  
		Last Modified: Wed, 15 Sep 2021 18:55:04 GMT  
		Size: 1.0 KB (1030 bytes)  
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
$ docker pull nats-streaming@sha256:d825481c4d8339d300a56d9f3eeaecf48ae0c071064bfa5ccfb1d9393ff52765
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2183; amd64

### `nats-streaming:nanoserver` - windows version 10.0.17763.2183; amd64

```console
$ docker pull nats-streaming@sha256:f7300d49f73a0e5451f68fcf439d1e5b75b5a891aa04e8ff537b523b15d45fc6
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.0 MB (110001330 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa93dcd937d8cd2009cb8f123551ce0f46c671f91465df126ce8475110a4f6cd`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 13 Sep 2021 03:45:12 GMT
RUN Apply image 1809-amd64
# Wed, 15 Sep 2021 15:43:05 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 15 Sep 2021 18:51:57 GMT
RUN cmd /S /C #(nop) COPY file:9670e5d1fe5a71e47c78fde01235a0bcbcafcfdeeacf96a7669f6e49343fb03b in C:\nats-streaming-server.exe 
# Wed, 15 Sep 2021 18:51:58 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 15 Sep 2021 18:51:59 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 15 Sep 2021 18:51:59 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:3585a81ca503e6c63dce938a5606f4171d7461e51000a92054b3f5692786d6c9`  
		Size: 102.7 MB (102703785 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:66dbf96361e9ec1f64f66e255a947eab476edef46c3f9a3b4ede943fa8b87699`  
		Last Modified: Wed, 15 Sep 2021 15:46:11 GMT  
		Size: 1.1 KB (1089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07e5a8a8a1823e7ab1aab125064b8d7d94f6dacefba9d82b815174cb4c32a833`  
		Last Modified: Wed, 15 Sep 2021 18:55:12 GMT  
		Size: 7.3 MB (7293261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16df1d39830ccb4fa2828c96b6c6ec476f1f3a292bdbd01053a21c6c9457750b`  
		Last Modified: Wed, 15 Sep 2021 18:55:04 GMT  
		Size: 1.1 KB (1114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43f99c367ebf7f75f5e675f26e18195abf8826890c87d26039e2c58b38a681d6`  
		Last Modified: Wed, 15 Sep 2021 18:55:04 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3052f7738f8821f9a96f777624d74a7b0b9c7fe0bcecce51d3586ea05479556d`  
		Last Modified: Wed, 15 Sep 2021 18:55:04 GMT  
		Size: 1.0 KB (1030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:nanoserver-1809`

```console
$ docker pull nats-streaming@sha256:d825481c4d8339d300a56d9f3eeaecf48ae0c071064bfa5ccfb1d9393ff52765
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2183; amd64

### `nats-streaming:nanoserver-1809` - windows version 10.0.17763.2183; amd64

```console
$ docker pull nats-streaming@sha256:f7300d49f73a0e5451f68fcf439d1e5b75b5a891aa04e8ff537b523b15d45fc6
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.0 MB (110001330 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa93dcd937d8cd2009cb8f123551ce0f46c671f91465df126ce8475110a4f6cd`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 13 Sep 2021 03:45:12 GMT
RUN Apply image 1809-amd64
# Wed, 15 Sep 2021 15:43:05 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 15 Sep 2021 18:51:57 GMT
RUN cmd /S /C #(nop) COPY file:9670e5d1fe5a71e47c78fde01235a0bcbcafcfdeeacf96a7669f6e49343fb03b in C:\nats-streaming-server.exe 
# Wed, 15 Sep 2021 18:51:58 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 15 Sep 2021 18:51:59 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 15 Sep 2021 18:51:59 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:3585a81ca503e6c63dce938a5606f4171d7461e51000a92054b3f5692786d6c9`  
		Size: 102.7 MB (102703785 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:66dbf96361e9ec1f64f66e255a947eab476edef46c3f9a3b4ede943fa8b87699`  
		Last Modified: Wed, 15 Sep 2021 15:46:11 GMT  
		Size: 1.1 KB (1089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07e5a8a8a1823e7ab1aab125064b8d7d94f6dacefba9d82b815174cb4c32a833`  
		Last Modified: Wed, 15 Sep 2021 18:55:12 GMT  
		Size: 7.3 MB (7293261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16df1d39830ccb4fa2828c96b6c6ec476f1f3a292bdbd01053a21c6c9457750b`  
		Last Modified: Wed, 15 Sep 2021 18:55:04 GMT  
		Size: 1.1 KB (1114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43f99c367ebf7f75f5e675f26e18195abf8826890c87d26039e2c58b38a681d6`  
		Last Modified: Wed, 15 Sep 2021 18:55:04 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3052f7738f8821f9a96f777624d74a7b0b9c7fe0bcecce51d3586ea05479556d`  
		Last Modified: Wed, 15 Sep 2021 18:55:04 GMT  
		Size: 1.0 KB (1030 bytes)  
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
$ docker pull nats-streaming@sha256:216e97a64fbe21529831ff1ddac989c2147fe68298359fb82b1c304153c9f38a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.2183; amd64
	-	windows version 10.0.14393.4651; amd64

### `nats-streaming:windowsservercore` - windows version 10.0.17763.2183; amd64

```console
$ docker pull nats-streaming@sha256:48f5ee8c66860f96f1851945d34a317b4038c171a4fc036953bd45e22ae600b8
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2694683224 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03cd19bbfbdb07be71a6322be26c8f7fce0969a83528b4755cf4c72f694719ed`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 13 Sep 2021 04:08:33 GMT
RUN Install update 1809-amd64
# Wed, 15 Sep 2021 13:14:12 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 15 Sep 2021 15:40:54 GMT
ENV NATS_DOCKERIZED=1
# Wed, 15 Sep 2021 18:49:45 GMT
ENV NATS_STREAMING_SERVER=0.22.1
# Wed, 15 Sep 2021 18:49:46 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.22.1/nats-streaming-server-v0.22.1-windows-amd64.zip
# Wed, 15 Sep 2021 18:49:47 GMT
ENV NATS_STREAMING_SERVER_SHASUM=4516852b493111b73ec06477be4a27e66f5abc9ca1ff4dd2b970232271611264
# Wed, 15 Sep 2021 18:50:28 GMT
RUN Set-PSDebug -Trace 2
# Wed, 15 Sep 2021 18:51:48 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 15 Sep 2021 18:51:49 GMT
EXPOSE 4222 8222
# Wed, 15 Sep 2021 18:51:49 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 15 Sep 2021 18:51:50 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a0ddf88812f10c7d6edc858aa9784ff5ca9de4a7bb631909c090090343abd059`  
		Size: 968.4 MB (968365008 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:6c4091e033b8590db7b89fded6d31ac2224162744daa4d7a7a66cbebd4b8c228`  
		Last Modified: Wed, 15 Sep 2021 15:04:44 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c75402e6fab70f623ca8becfa5bb563e5630bbb4dac8adb11e385d75e171aed`  
		Last Modified: Wed, 15 Sep 2021 15:45:53 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffaf075a271862d4bc05568114cc4eeb60f8de9ba30ac6e3fe5355849d4000cd`  
		Last Modified: Wed, 15 Sep 2021 18:54:52 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4835bde54170d4fcd660b52c8dfed238e8f2ab963f2a9285e591fe7115fa2283`  
		Last Modified: Wed, 15 Sep 2021 18:54:51 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c477ff70b750b36312766e21da88df14a9d42d6926bf3e30ba1c64308b163d8a`  
		Last Modified: Wed, 15 Sep 2021 18:54:51 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcc35663cd24c79f3cf7d67b95f50e510f509c986a1743d126193cb8838145e6`  
		Last Modified: Wed, 15 Sep 2021 18:54:49 GMT  
		Size: 349.2 KB (349224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4772ba9bdad7c934060bfc5561978af7dcccb05ea78ebb2ccbf13749d804db1`  
		Last Modified: Wed, 15 Sep 2021 18:54:51 GMT  
		Size: 7.6 MB (7625617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:000708a1ba81b80dbbfebe82d875a1116e8ad8659232936d8b5c19710445658c`  
		Last Modified: Wed, 15 Sep 2021 18:54:49 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a977d7698cf7e509b59d133fe3f5c720b1ac86dd8c0e4ced1e82c548c4cfd47`  
		Last Modified: Wed, 15 Sep 2021 18:54:49 GMT  
		Size: 1.3 KB (1327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3653acfe476962adc853584e37df0eddc16574f7588d42731309f7b95aa9f315`  
		Last Modified: Wed, 15 Sep 2021 18:54:49 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:windowsservercore` - windows version 10.0.14393.4651; amd64

```console
$ docker pull nats-streaming@sha256:db420b05307ebc5425e2ed494fe11c71977ae9644d6cc08cea9a32388a8f92f9
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6279315014 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9224e56def9350d516ffcf46c72c2fe923a1e699e78612f8f084568b4a884b93`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 13 Sep 2021 01:03:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 15 Sep 2021 13:26:09 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 15 Sep 2021 15:43:15 GMT
ENV NATS_DOCKERIZED=1
# Wed, 15 Sep 2021 18:52:05 GMT
ENV NATS_STREAMING_SERVER=0.22.1
# Wed, 15 Sep 2021 18:52:06 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.22.1/nats-streaming-server-v0.22.1-windows-amd64.zip
# Wed, 15 Sep 2021 18:52:07 GMT
ENV NATS_STREAMING_SERVER_SHASUM=4516852b493111b73ec06477be4a27e66f5abc9ca1ff4dd2b970232271611264
# Wed, 15 Sep 2021 18:52:47 GMT
RUN Set-PSDebug -Trace 2
# Wed, 15 Sep 2021 18:54:15 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 15 Sep 2021 18:54:16 GMT
EXPOSE 4222 8222
# Wed, 15 Sep 2021 18:54:17 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 15 Sep 2021 18:54:18 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e9b8281bf21e46c781fb54e4f15f5728e2c44dea4219c9e6deeb732f1d909d3b`  
		Size: 2.2 GB (2201342322 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5796468f91731000e9a76e836156826a1cd4ed963bcd80e6558c538a12c2132d`  
		Last Modified: Wed, 15 Sep 2021 15:05:15 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:611fe9c559abed986280087eef7d362a6ecb9ad281b1427395fdfc2d99d3d9c4`  
		Last Modified: Wed, 15 Sep 2021 15:46:29 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cc80b5d1ce6897bdd090b01daa650e63019faa977ef23c8248e4ab254310830`  
		Last Modified: Wed, 15 Sep 2021 18:55:26 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be2342d91ff82328bf8ba622555f8083b3c2311603f49e600e921a3b424852ec`  
		Last Modified: Wed, 15 Sep 2021 18:55:25 GMT  
		Size: 1.3 KB (1296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f61c2209638a7d2ded082cb0eb17bd8856f27d50a02eadc7a623429f008fe26`  
		Last Modified: Wed, 15 Sep 2021 18:55:25 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df5019f36414f6f8aee86294793001d1cdf5631d45a6901646229fc1e85e01c2`  
		Last Modified: Wed, 15 Sep 2021 18:55:23 GMT  
		Size: 332.6 KB (332556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f748d4a8c2babe5e9ba487dbb17fcec2eeed0dcd1ce7b3e11d8ed12adeb75d1`  
		Last Modified: Wed, 15 Sep 2021 18:55:31 GMT  
		Size: 7.6 MB (7643649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4386a8452b0b6cfe5bb3563f552cfcfa025a77c50e0b7b383f486c6609b8e3b`  
		Last Modified: Wed, 15 Sep 2021 18:55:23 GMT  
		Size: 1.3 KB (1325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20c1401d40019edc4f2a3ba3ccbdd1c088c2f1e28bfa1d2255721cd3ff172d43`  
		Last Modified: Wed, 15 Sep 2021 18:55:23 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:207050f1ea57a9f8edae4f5caead9eb05022d7428e2b17637b719213bce914a4`  
		Last Modified: Wed, 15 Sep 2021 18:55:23 GMT  
		Size: 1.3 KB (1302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:windowsservercore-1809`

```console
$ docker pull nats-streaming@sha256:2e38de84651e01073fb06b20a95117b46cb69db1b1173946ad98503097ab5df2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2183; amd64

### `nats-streaming:windowsservercore-1809` - windows version 10.0.17763.2183; amd64

```console
$ docker pull nats-streaming@sha256:48f5ee8c66860f96f1851945d34a317b4038c171a4fc036953bd45e22ae600b8
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2694683224 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03cd19bbfbdb07be71a6322be26c8f7fce0969a83528b4755cf4c72f694719ed`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 13 Sep 2021 04:08:33 GMT
RUN Install update 1809-amd64
# Wed, 15 Sep 2021 13:14:12 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 15 Sep 2021 15:40:54 GMT
ENV NATS_DOCKERIZED=1
# Wed, 15 Sep 2021 18:49:45 GMT
ENV NATS_STREAMING_SERVER=0.22.1
# Wed, 15 Sep 2021 18:49:46 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.22.1/nats-streaming-server-v0.22.1-windows-amd64.zip
# Wed, 15 Sep 2021 18:49:47 GMT
ENV NATS_STREAMING_SERVER_SHASUM=4516852b493111b73ec06477be4a27e66f5abc9ca1ff4dd2b970232271611264
# Wed, 15 Sep 2021 18:50:28 GMT
RUN Set-PSDebug -Trace 2
# Wed, 15 Sep 2021 18:51:48 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 15 Sep 2021 18:51:49 GMT
EXPOSE 4222 8222
# Wed, 15 Sep 2021 18:51:49 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 15 Sep 2021 18:51:50 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a0ddf88812f10c7d6edc858aa9784ff5ca9de4a7bb631909c090090343abd059`  
		Size: 968.4 MB (968365008 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:6c4091e033b8590db7b89fded6d31ac2224162744daa4d7a7a66cbebd4b8c228`  
		Last Modified: Wed, 15 Sep 2021 15:04:44 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c75402e6fab70f623ca8becfa5bb563e5630bbb4dac8adb11e385d75e171aed`  
		Last Modified: Wed, 15 Sep 2021 15:45:53 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffaf075a271862d4bc05568114cc4eeb60f8de9ba30ac6e3fe5355849d4000cd`  
		Last Modified: Wed, 15 Sep 2021 18:54:52 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4835bde54170d4fcd660b52c8dfed238e8f2ab963f2a9285e591fe7115fa2283`  
		Last Modified: Wed, 15 Sep 2021 18:54:51 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c477ff70b750b36312766e21da88df14a9d42d6926bf3e30ba1c64308b163d8a`  
		Last Modified: Wed, 15 Sep 2021 18:54:51 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcc35663cd24c79f3cf7d67b95f50e510f509c986a1743d126193cb8838145e6`  
		Last Modified: Wed, 15 Sep 2021 18:54:49 GMT  
		Size: 349.2 KB (349224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4772ba9bdad7c934060bfc5561978af7dcccb05ea78ebb2ccbf13749d804db1`  
		Last Modified: Wed, 15 Sep 2021 18:54:51 GMT  
		Size: 7.6 MB (7625617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:000708a1ba81b80dbbfebe82d875a1116e8ad8659232936d8b5c19710445658c`  
		Last Modified: Wed, 15 Sep 2021 18:54:49 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a977d7698cf7e509b59d133fe3f5c720b1ac86dd8c0e4ced1e82c548c4cfd47`  
		Last Modified: Wed, 15 Sep 2021 18:54:49 GMT  
		Size: 1.3 KB (1327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3653acfe476962adc853584e37df0eddc16574f7588d42731309f7b95aa9f315`  
		Last Modified: Wed, 15 Sep 2021 18:54:49 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:windowsservercore-ltsc2016`

```console
$ docker pull nats-streaming@sha256:2355a62bb57d76c5ec35a02432c7c159489e6739f13c2249af33a1257cf55b65
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.14393.4651; amd64

### `nats-streaming:windowsservercore-ltsc2016` - windows version 10.0.14393.4651; amd64

```console
$ docker pull nats-streaming@sha256:db420b05307ebc5425e2ed494fe11c71977ae9644d6cc08cea9a32388a8f92f9
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6279315014 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9224e56def9350d516ffcf46c72c2fe923a1e699e78612f8f084568b4a884b93`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 13 Sep 2021 01:03:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 15 Sep 2021 13:26:09 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 15 Sep 2021 15:43:15 GMT
ENV NATS_DOCKERIZED=1
# Wed, 15 Sep 2021 18:52:05 GMT
ENV NATS_STREAMING_SERVER=0.22.1
# Wed, 15 Sep 2021 18:52:06 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.22.1/nats-streaming-server-v0.22.1-windows-amd64.zip
# Wed, 15 Sep 2021 18:52:07 GMT
ENV NATS_STREAMING_SERVER_SHASUM=4516852b493111b73ec06477be4a27e66f5abc9ca1ff4dd2b970232271611264
# Wed, 15 Sep 2021 18:52:47 GMT
RUN Set-PSDebug -Trace 2
# Wed, 15 Sep 2021 18:54:15 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 15 Sep 2021 18:54:16 GMT
EXPOSE 4222 8222
# Wed, 15 Sep 2021 18:54:17 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 15 Sep 2021 18:54:18 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e9b8281bf21e46c781fb54e4f15f5728e2c44dea4219c9e6deeb732f1d909d3b`  
		Size: 2.2 GB (2201342322 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5796468f91731000e9a76e836156826a1cd4ed963bcd80e6558c538a12c2132d`  
		Last Modified: Wed, 15 Sep 2021 15:05:15 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:611fe9c559abed986280087eef7d362a6ecb9ad281b1427395fdfc2d99d3d9c4`  
		Last Modified: Wed, 15 Sep 2021 15:46:29 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cc80b5d1ce6897bdd090b01daa650e63019faa977ef23c8248e4ab254310830`  
		Last Modified: Wed, 15 Sep 2021 18:55:26 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be2342d91ff82328bf8ba622555f8083b3c2311603f49e600e921a3b424852ec`  
		Last Modified: Wed, 15 Sep 2021 18:55:25 GMT  
		Size: 1.3 KB (1296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f61c2209638a7d2ded082cb0eb17bd8856f27d50a02eadc7a623429f008fe26`  
		Last Modified: Wed, 15 Sep 2021 18:55:25 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df5019f36414f6f8aee86294793001d1cdf5631d45a6901646229fc1e85e01c2`  
		Last Modified: Wed, 15 Sep 2021 18:55:23 GMT  
		Size: 332.6 KB (332556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f748d4a8c2babe5e9ba487dbb17fcec2eeed0dcd1ce7b3e11d8ed12adeb75d1`  
		Last Modified: Wed, 15 Sep 2021 18:55:31 GMT  
		Size: 7.6 MB (7643649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4386a8452b0b6cfe5bb3563f552cfcfa025a77c50e0b7b383f486c6609b8e3b`  
		Last Modified: Wed, 15 Sep 2021 18:55:23 GMT  
		Size: 1.3 KB (1325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20c1401d40019edc4f2a3ba3ccbdd1c088c2f1e28bfa1d2255721cd3ff172d43`  
		Last Modified: Wed, 15 Sep 2021 18:55:23 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:207050f1ea57a9f8edae4f5caead9eb05022d7428e2b17637b719213bce914a4`  
		Last Modified: Wed, 15 Sep 2021 18:55:23 GMT  
		Size: 1.3 KB (1302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
