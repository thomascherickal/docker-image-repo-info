<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `nats-streaming`

-	[`nats-streaming:0.18`](#nats-streaming018)
-	[`nats-streaming:0.18.0`](#nats-streaming0180)
-	[`nats-streaming:0.18.0-alpine`](#nats-streaming0180-alpine)
-	[`nats-streaming:0.18.0-alpine3.12`](#nats-streaming0180-alpine312)
-	[`nats-streaming:0.18.0-linux`](#nats-streaming0180-linux)
-	[`nats-streaming:0.18.0-nanoserver`](#nats-streaming0180-nanoserver)
-	[`nats-streaming:0.18.0-nanoserver-1809`](#nats-streaming0180-nanoserver-1809)
-	[`nats-streaming:0.18.0-scratch`](#nats-streaming0180-scratch)
-	[`nats-streaming:0.18.0-windowsservercore`](#nats-streaming0180-windowsservercore)
-	[`nats-streaming:0.18.0-windowsservercore-1809`](#nats-streaming0180-windowsservercore-1809)
-	[`nats-streaming:0.18.0-windowsservercore-ltsc2016`](#nats-streaming0180-windowsservercore-ltsc2016)
-	[`nats-streaming:0.18-alpine`](#nats-streaming018-alpine)
-	[`nats-streaming:0.18-alpine3.12`](#nats-streaming018-alpine312)
-	[`nats-streaming:0.18-linux`](#nats-streaming018-linux)
-	[`nats-streaming:0.18-nanoserver`](#nats-streaming018-nanoserver)
-	[`nats-streaming:0.18-nanoserver-1809`](#nats-streaming018-nanoserver-1809)
-	[`nats-streaming:0.18-scratch`](#nats-streaming018-scratch)
-	[`nats-streaming:0.18-windowsservercore`](#nats-streaming018-windowsservercore)
-	[`nats-streaming:0.18-windowsservercore-1809`](#nats-streaming018-windowsservercore-1809)
-	[`nats-streaming:0.18-windowsservercore-ltsc2016`](#nats-streaming018-windowsservercore-ltsc2016)
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

## `nats-streaming:0.18`

```console
$ docker pull nats-streaming@sha256:b6a6edcfc853b2e70689250639914f0a9f8e3ea21027548861ccb673d208114e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.1518; amd64

### `nats-streaming:0.18` - linux; amd64

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

### `nats-streaming:0.18` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:95ded92d384b4d9631841677a2d34b175cba6cbb4b4fa127b7a754b9f57c849e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.5 MB (5530521 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:24577fc60833cbc345883a4b8ee0eed5044ed08c199307ea0b9f951f7d5b6d3c`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 25 Jun 2020 19:50:40 GMT
COPY file:7145d006cd221687dcd9139e9e58f09c1f07ee9ce00f3485d297197fdd5ba444 in /nats-streaming-server 
# Thu, 25 Jun 2020 19:50:41 GMT
EXPOSE 4222 8222
# Thu, 25 Jun 2020 19:50:42 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Thu, 25 Jun 2020 19:50:43 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:ef961e603a1ec489ef1932fb068478ad9e98f8417ff4fefb8d4678e8653a5771`  
		Last Modified: Thu, 25 Jun 2020 19:51:16 GMT  
		Size: 5.5 MB (5530521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.18` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:60e9dc71017275b017a750e7be04e9c16abd50c6b6bc589ddf399588e44a509c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.5 MB (5523586 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b4b24c4ac594ac46c22186488b6b2138f48703c79ebce756ae461ac777a7b486`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 25 Jun 2020 19:02:38 GMT
COPY file:2b6e0add99a6d3c42ba8b65af53581560646dbdaf347b23e6dde1f4267fa57bc in /nats-streaming-server 
# Thu, 25 Jun 2020 19:02:38 GMT
EXPOSE 4222 8222
# Thu, 25 Jun 2020 19:02:39 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Thu, 25 Jun 2020 19:02:40 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:7af54707b9f6fd805487c0afe7fd52962e5abd3d1ab43335ccfc7224a2018844`  
		Last Modified: Thu, 25 Jun 2020 19:03:22 GMT  
		Size: 5.5 MB (5523586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.18` - linux; arm64 variant v8

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

### `nats-streaming:0.18` - windows version 10.0.17763.1518; amd64

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

## `nats-streaming:0.18.0`

```console
$ docker pull nats-streaming@sha256:b6a6edcfc853b2e70689250639914f0a9f8e3ea21027548861ccb673d208114e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.1518; amd64

### `nats-streaming:0.18.0` - linux; amd64

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

### `nats-streaming:0.18.0` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:95ded92d384b4d9631841677a2d34b175cba6cbb4b4fa127b7a754b9f57c849e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.5 MB (5530521 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:24577fc60833cbc345883a4b8ee0eed5044ed08c199307ea0b9f951f7d5b6d3c`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 25 Jun 2020 19:50:40 GMT
COPY file:7145d006cd221687dcd9139e9e58f09c1f07ee9ce00f3485d297197fdd5ba444 in /nats-streaming-server 
# Thu, 25 Jun 2020 19:50:41 GMT
EXPOSE 4222 8222
# Thu, 25 Jun 2020 19:50:42 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Thu, 25 Jun 2020 19:50:43 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:ef961e603a1ec489ef1932fb068478ad9e98f8417ff4fefb8d4678e8653a5771`  
		Last Modified: Thu, 25 Jun 2020 19:51:16 GMT  
		Size: 5.5 MB (5530521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.18.0` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:60e9dc71017275b017a750e7be04e9c16abd50c6b6bc589ddf399588e44a509c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.5 MB (5523586 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b4b24c4ac594ac46c22186488b6b2138f48703c79ebce756ae461ac777a7b486`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 25 Jun 2020 19:02:38 GMT
COPY file:2b6e0add99a6d3c42ba8b65af53581560646dbdaf347b23e6dde1f4267fa57bc in /nats-streaming-server 
# Thu, 25 Jun 2020 19:02:38 GMT
EXPOSE 4222 8222
# Thu, 25 Jun 2020 19:02:39 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Thu, 25 Jun 2020 19:02:40 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:7af54707b9f6fd805487c0afe7fd52962e5abd3d1ab43335ccfc7224a2018844`  
		Last Modified: Thu, 25 Jun 2020 19:03:22 GMT  
		Size: 5.5 MB (5523586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.18.0` - linux; arm64 variant v8

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

### `nats-streaming:0.18.0` - windows version 10.0.17763.1518; amd64

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

## `nats-streaming:0.18.0-alpine`

```console
$ docker pull nats-streaming@sha256:ef19a7373b6ab0b6b4a207cb550e85a7898d683aaae3d9e1361ba69d7d987541
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.18.0-alpine` - linux; amd64

```console
$ docker pull nats-streaming@sha256:f773acd3701babcf267f460eace482aaa2847fdb79d08850fca955fe69c12e8f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.0 MB (9015139 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:76f6db6849462b8b7abf8b8226c566f28b86a57b5b89b7771e1987f837252cc8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Thu, 25 Jun 2020 19:25:24 GMT
ENV NATS_STREAMING_SERVER=0.18.0
# Wed, 29 Jul 2020 23:26:37 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='ff2a51618b79685264f980fe868f1c7af583c419b6406cc63d4811f3c98ca8fe' ;; 		armhf) natsArch='arm6'; sha256='629e17255f12fd80e051772a6dd18a7f65e692b4abef0786b421eb8b6ab85db4' ;; 		armv7) natsArch='arm7'; sha256='94e499af6a6391519315e8bcd5127c43c1d1a442ef945956286e77b4366c92c9' ;; 		x86_64) natsArch='amd64'; sha256='6252e9262efc81a41ade3f43b68e014d1e635d3e3bf9cbcd2b09c3a030a0d5e6' ;; 		x86) natsArch='386'; sha256='886ebd2e5eb99e30ff9e9d8907d7bd49dafacffce1dc921427e5754a4ec26f55' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 29 Jul 2020 23:26:37 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Wed, 29 Jul 2020 23:26:37 GMT
EXPOSE 4222 8222
# Wed, 29 Jul 2020 23:26:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Jul 2020 23:26:37 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:df20fa9351a15782c64e6dddb2d4a6f50bf6d3688060a34c4014b0d9a752eb4c`  
		Last Modified: Fri, 29 May 2020 21:20:06 GMT  
		Size: 2.8 MB (2797541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd351f099985ea9a52973cdd0eaeff72c72744a8c9f82a1cbc8664bffc094fdb`  
		Last Modified: Wed, 29 Jul 2020 23:26:57 GMT  
		Size: 6.2 MB (6217176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd65001efde87dd38a54a1b153608623d270593a572dda8cfa5b0a144138251e`  
		Last Modified: Wed, 29 Jul 2020 23:26:55 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.18.0-alpine` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:e66e8c57c226879ac8535b680ee1391ef87ae2bcc5690ec7ecbf93a4066c82a6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.4 MB (8414433 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:857496a37e19bdea5173718e9e76bb7a4a0d3c535b434feabab434f0ba9e90f9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 29 May 2020 21:50:55 GMT
ADD file:f46e997a56849423db17e5fc9f0249ab6c73b155245927dba5fcb9dfd65f622f in / 
# Fri, 29 May 2020 21:50:56 GMT
CMD ["/bin/sh"]
# Thu, 25 Jun 2020 19:50:21 GMT
ENV NATS_STREAMING_SERVER=0.18.0
# Wed, 29 Jul 2020 23:01:31 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='ff2a51618b79685264f980fe868f1c7af583c419b6406cc63d4811f3c98ca8fe' ;; 		armhf) natsArch='arm6'; sha256='629e17255f12fd80e051772a6dd18a7f65e692b4abef0786b421eb8b6ab85db4' ;; 		armv7) natsArch='arm7'; sha256='94e499af6a6391519315e8bcd5127c43c1d1a442ef945956286e77b4366c92c9' ;; 		x86_64) natsArch='amd64'; sha256='6252e9262efc81a41ade3f43b68e014d1e635d3e3bf9cbcd2b09c3a030a0d5e6' ;; 		x86) natsArch='386'; sha256='886ebd2e5eb99e30ff9e9d8907d7bd49dafacffce1dc921427e5754a4ec26f55' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 29 Jul 2020 23:01:32 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Wed, 29 Jul 2020 23:01:33 GMT
EXPOSE 4222 8222
# Wed, 29 Jul 2020 23:01:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Jul 2020 23:01:34 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:b4b72e716706d29f5d2351709c20bf737b94f876a5472a43ff1b6e203c65d27f`  
		Last Modified: Fri, 29 May 2020 21:51:30 GMT  
		Size: 2.6 MB (2603286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:406c29efa0cf9678b606f95b786cc832aa806186815fb1ca94233b6704050bbc`  
		Last Modified: Wed, 29 Jul 2020 23:02:00 GMT  
		Size: 5.8 MB (5810724 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09492963cd9edfd3f0ced5fb4042e7d537ee7fde04c3880c4a91bc84f9b46a6f`  
		Last Modified: Wed, 29 Jul 2020 23:01:59 GMT  
		Size: 423.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.18.0-alpine` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:a20ba55bef224ae45cc82582ac9191883a54e523a0ccbbe04365a9d5f373e561
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.2 MB (8213849 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ed41b19417bfe6bc079828554b1e892e5b04728503f6b6742aaabf260080863`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 29 May 2020 21:02:07 GMT
ADD file:e97bf0d217846312b19a9f7264604851aedd125c23b4d291eed4c69b880dce26 in / 
# Fri, 29 May 2020 21:02:08 GMT
CMD ["/bin/sh"]
# Thu, 25 Jun 2020 18:58:53 GMT
ENV NATS_STREAMING_SERVER=0.18.0
# Wed, 29 Jul 2020 23:16:33 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='ff2a51618b79685264f980fe868f1c7af583c419b6406cc63d4811f3c98ca8fe' ;; 		armhf) natsArch='arm6'; sha256='629e17255f12fd80e051772a6dd18a7f65e692b4abef0786b421eb8b6ab85db4' ;; 		armv7) natsArch='arm7'; sha256='94e499af6a6391519315e8bcd5127c43c1d1a442ef945956286e77b4366c92c9' ;; 		x86_64) natsArch='amd64'; sha256='6252e9262efc81a41ade3f43b68e014d1e635d3e3bf9cbcd2b09c3a030a0d5e6' ;; 		x86) natsArch='386'; sha256='886ebd2e5eb99e30ff9e9d8907d7bd49dafacffce1dc921427e5754a4ec26f55' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 29 Jul 2020 23:16:34 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Wed, 29 Jul 2020 23:16:35 GMT
EXPOSE 4222 8222
# Wed, 29 Jul 2020 23:16:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Jul 2020 23:16:36 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:52278dd8e57993669c5b72a9620e89bebdc098f2af2379caaa8945f7403f77a2`  
		Last Modified: Fri, 29 May 2020 21:02:38 GMT  
		Size: 2.4 MB (2406763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14a1e6d591214ac54fc11baa4e27cf3cc7d9f0b6a65f186a67a96ced744cc569`  
		Last Modified: Wed, 29 Jul 2020 23:17:02 GMT  
		Size: 5.8 MB (5806663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94627b007b78566192f9591c03d4e2245b2f4943dd979b9d14d389edc2b60f96`  
		Last Modified: Wed, 29 Jul 2020 23:17:00 GMT  
		Size: 423.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.18.0-alpine` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:2efd83c7baf426a5da8223e4bd05f9278545d8fe81270934a16416e73c68e5b6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.5 MB (8459346 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:671f8011bed05657f23e61f2c1011683c94045a8c893ed9aab290b88aa383e94`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 29 May 2020 21:43:19 GMT
ADD file:7574aee4e37a85460ab889212d52912723a9b30dda1c060548f0deb4a05fc398 in / 
# Fri, 29 May 2020 21:43:20 GMT
CMD ["/bin/sh"]
# Fri, 24 Jul 2020 16:29:11 GMT
ENV NATS_STREAMING_SERVER=0.18.0
# Wed, 29 Jul 2020 22:39:58 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='ff2a51618b79685264f980fe868f1c7af583c419b6406cc63d4811f3c98ca8fe' ;; 		armhf) natsArch='arm6'; sha256='629e17255f12fd80e051772a6dd18a7f65e692b4abef0786b421eb8b6ab85db4' ;; 		armv7) natsArch='arm7'; sha256='94e499af6a6391519315e8bcd5127c43c1d1a442ef945956286e77b4366c92c9' ;; 		x86_64) natsArch='amd64'; sha256='6252e9262efc81a41ade3f43b68e014d1e635d3e3bf9cbcd2b09c3a030a0d5e6' ;; 		x86) natsArch='386'; sha256='886ebd2e5eb99e30ff9e9d8907d7bd49dafacffce1dc921427e5754a4ec26f55' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 29 Jul 2020 22:39:59 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Wed, 29 Jul 2020 22:39:59 GMT
EXPOSE 4222 8222
# Wed, 29 Jul 2020 22:40:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Jul 2020 22:40:00 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:b538f80385f9b48122e3da068c932a96ea5018afa3c7be79da00437414bd18cd`  
		Last Modified: Fri, 29 May 2020 21:43:57 GMT  
		Size: 2.7 MB (2707964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9b7179a5be80ec5254ffae42b351490af025c30cac276c5f48df27ba082d2c3`  
		Last Modified: Wed, 29 Jul 2020 22:40:30 GMT  
		Size: 5.8 MB (5750960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b945e4e25ec28f56f7dd8226e5e8ce479b9fb61cb6456eda8662d9d35acbd583`  
		Last Modified: Wed, 29 Jul 2020 22:40:28 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.18.0-alpine3.12`

```console
$ docker pull nats-streaming@sha256:ef19a7373b6ab0b6b4a207cb550e85a7898d683aaae3d9e1361ba69d7d987541
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.18.0-alpine3.12` - linux; amd64

```console
$ docker pull nats-streaming@sha256:f773acd3701babcf267f460eace482aaa2847fdb79d08850fca955fe69c12e8f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.0 MB (9015139 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:76f6db6849462b8b7abf8b8226c566f28b86a57b5b89b7771e1987f837252cc8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Thu, 25 Jun 2020 19:25:24 GMT
ENV NATS_STREAMING_SERVER=0.18.0
# Wed, 29 Jul 2020 23:26:37 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='ff2a51618b79685264f980fe868f1c7af583c419b6406cc63d4811f3c98ca8fe' ;; 		armhf) natsArch='arm6'; sha256='629e17255f12fd80e051772a6dd18a7f65e692b4abef0786b421eb8b6ab85db4' ;; 		armv7) natsArch='arm7'; sha256='94e499af6a6391519315e8bcd5127c43c1d1a442ef945956286e77b4366c92c9' ;; 		x86_64) natsArch='amd64'; sha256='6252e9262efc81a41ade3f43b68e014d1e635d3e3bf9cbcd2b09c3a030a0d5e6' ;; 		x86) natsArch='386'; sha256='886ebd2e5eb99e30ff9e9d8907d7bd49dafacffce1dc921427e5754a4ec26f55' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 29 Jul 2020 23:26:37 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Wed, 29 Jul 2020 23:26:37 GMT
EXPOSE 4222 8222
# Wed, 29 Jul 2020 23:26:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Jul 2020 23:26:37 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:df20fa9351a15782c64e6dddb2d4a6f50bf6d3688060a34c4014b0d9a752eb4c`  
		Last Modified: Fri, 29 May 2020 21:20:06 GMT  
		Size: 2.8 MB (2797541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd351f099985ea9a52973cdd0eaeff72c72744a8c9f82a1cbc8664bffc094fdb`  
		Last Modified: Wed, 29 Jul 2020 23:26:57 GMT  
		Size: 6.2 MB (6217176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd65001efde87dd38a54a1b153608623d270593a572dda8cfa5b0a144138251e`  
		Last Modified: Wed, 29 Jul 2020 23:26:55 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.18.0-alpine3.12` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:e66e8c57c226879ac8535b680ee1391ef87ae2bcc5690ec7ecbf93a4066c82a6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.4 MB (8414433 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:857496a37e19bdea5173718e9e76bb7a4a0d3c535b434feabab434f0ba9e90f9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 29 May 2020 21:50:55 GMT
ADD file:f46e997a56849423db17e5fc9f0249ab6c73b155245927dba5fcb9dfd65f622f in / 
# Fri, 29 May 2020 21:50:56 GMT
CMD ["/bin/sh"]
# Thu, 25 Jun 2020 19:50:21 GMT
ENV NATS_STREAMING_SERVER=0.18.0
# Wed, 29 Jul 2020 23:01:31 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='ff2a51618b79685264f980fe868f1c7af583c419b6406cc63d4811f3c98ca8fe' ;; 		armhf) natsArch='arm6'; sha256='629e17255f12fd80e051772a6dd18a7f65e692b4abef0786b421eb8b6ab85db4' ;; 		armv7) natsArch='arm7'; sha256='94e499af6a6391519315e8bcd5127c43c1d1a442ef945956286e77b4366c92c9' ;; 		x86_64) natsArch='amd64'; sha256='6252e9262efc81a41ade3f43b68e014d1e635d3e3bf9cbcd2b09c3a030a0d5e6' ;; 		x86) natsArch='386'; sha256='886ebd2e5eb99e30ff9e9d8907d7bd49dafacffce1dc921427e5754a4ec26f55' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 29 Jul 2020 23:01:32 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Wed, 29 Jul 2020 23:01:33 GMT
EXPOSE 4222 8222
# Wed, 29 Jul 2020 23:01:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Jul 2020 23:01:34 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:b4b72e716706d29f5d2351709c20bf737b94f876a5472a43ff1b6e203c65d27f`  
		Last Modified: Fri, 29 May 2020 21:51:30 GMT  
		Size: 2.6 MB (2603286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:406c29efa0cf9678b606f95b786cc832aa806186815fb1ca94233b6704050bbc`  
		Last Modified: Wed, 29 Jul 2020 23:02:00 GMT  
		Size: 5.8 MB (5810724 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09492963cd9edfd3f0ced5fb4042e7d537ee7fde04c3880c4a91bc84f9b46a6f`  
		Last Modified: Wed, 29 Jul 2020 23:01:59 GMT  
		Size: 423.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.18.0-alpine3.12` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:a20ba55bef224ae45cc82582ac9191883a54e523a0ccbbe04365a9d5f373e561
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.2 MB (8213849 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ed41b19417bfe6bc079828554b1e892e5b04728503f6b6742aaabf260080863`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 29 May 2020 21:02:07 GMT
ADD file:e97bf0d217846312b19a9f7264604851aedd125c23b4d291eed4c69b880dce26 in / 
# Fri, 29 May 2020 21:02:08 GMT
CMD ["/bin/sh"]
# Thu, 25 Jun 2020 18:58:53 GMT
ENV NATS_STREAMING_SERVER=0.18.0
# Wed, 29 Jul 2020 23:16:33 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='ff2a51618b79685264f980fe868f1c7af583c419b6406cc63d4811f3c98ca8fe' ;; 		armhf) natsArch='arm6'; sha256='629e17255f12fd80e051772a6dd18a7f65e692b4abef0786b421eb8b6ab85db4' ;; 		armv7) natsArch='arm7'; sha256='94e499af6a6391519315e8bcd5127c43c1d1a442ef945956286e77b4366c92c9' ;; 		x86_64) natsArch='amd64'; sha256='6252e9262efc81a41ade3f43b68e014d1e635d3e3bf9cbcd2b09c3a030a0d5e6' ;; 		x86) natsArch='386'; sha256='886ebd2e5eb99e30ff9e9d8907d7bd49dafacffce1dc921427e5754a4ec26f55' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 29 Jul 2020 23:16:34 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Wed, 29 Jul 2020 23:16:35 GMT
EXPOSE 4222 8222
# Wed, 29 Jul 2020 23:16:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Jul 2020 23:16:36 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:52278dd8e57993669c5b72a9620e89bebdc098f2af2379caaa8945f7403f77a2`  
		Last Modified: Fri, 29 May 2020 21:02:38 GMT  
		Size: 2.4 MB (2406763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14a1e6d591214ac54fc11baa4e27cf3cc7d9f0b6a65f186a67a96ced744cc569`  
		Last Modified: Wed, 29 Jul 2020 23:17:02 GMT  
		Size: 5.8 MB (5806663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94627b007b78566192f9591c03d4e2245b2f4943dd979b9d14d389edc2b60f96`  
		Last Modified: Wed, 29 Jul 2020 23:17:00 GMT  
		Size: 423.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.18.0-alpine3.12` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:2efd83c7baf426a5da8223e4bd05f9278545d8fe81270934a16416e73c68e5b6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.5 MB (8459346 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:671f8011bed05657f23e61f2c1011683c94045a8c893ed9aab290b88aa383e94`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 29 May 2020 21:43:19 GMT
ADD file:7574aee4e37a85460ab889212d52912723a9b30dda1c060548f0deb4a05fc398 in / 
# Fri, 29 May 2020 21:43:20 GMT
CMD ["/bin/sh"]
# Fri, 24 Jul 2020 16:29:11 GMT
ENV NATS_STREAMING_SERVER=0.18.0
# Wed, 29 Jul 2020 22:39:58 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='ff2a51618b79685264f980fe868f1c7af583c419b6406cc63d4811f3c98ca8fe' ;; 		armhf) natsArch='arm6'; sha256='629e17255f12fd80e051772a6dd18a7f65e692b4abef0786b421eb8b6ab85db4' ;; 		armv7) natsArch='arm7'; sha256='94e499af6a6391519315e8bcd5127c43c1d1a442ef945956286e77b4366c92c9' ;; 		x86_64) natsArch='amd64'; sha256='6252e9262efc81a41ade3f43b68e014d1e635d3e3bf9cbcd2b09c3a030a0d5e6' ;; 		x86) natsArch='386'; sha256='886ebd2e5eb99e30ff9e9d8907d7bd49dafacffce1dc921427e5754a4ec26f55' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 29 Jul 2020 22:39:59 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Wed, 29 Jul 2020 22:39:59 GMT
EXPOSE 4222 8222
# Wed, 29 Jul 2020 22:40:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Jul 2020 22:40:00 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:b538f80385f9b48122e3da068c932a96ea5018afa3c7be79da00437414bd18cd`  
		Last Modified: Fri, 29 May 2020 21:43:57 GMT  
		Size: 2.7 MB (2707964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9b7179a5be80ec5254ffae42b351490af025c30cac276c5f48df27ba082d2c3`  
		Last Modified: Wed, 29 Jul 2020 22:40:30 GMT  
		Size: 5.8 MB (5750960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b945e4e25ec28f56f7dd8226e5e8ce479b9fb61cb6456eda8662d9d35acbd583`  
		Last Modified: Wed, 29 Jul 2020 22:40:28 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.18.0-linux`

```console
$ docker pull nats-streaming@sha256:6ab20bdd5317c0c00aa163f02cbf5d430e4381f6f1ae77fba2063c797b5acbb0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.18.0-linux` - linux; amd64

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

### `nats-streaming:0.18.0-linux` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:95ded92d384b4d9631841677a2d34b175cba6cbb4b4fa127b7a754b9f57c849e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.5 MB (5530521 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:24577fc60833cbc345883a4b8ee0eed5044ed08c199307ea0b9f951f7d5b6d3c`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 25 Jun 2020 19:50:40 GMT
COPY file:7145d006cd221687dcd9139e9e58f09c1f07ee9ce00f3485d297197fdd5ba444 in /nats-streaming-server 
# Thu, 25 Jun 2020 19:50:41 GMT
EXPOSE 4222 8222
# Thu, 25 Jun 2020 19:50:42 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Thu, 25 Jun 2020 19:50:43 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:ef961e603a1ec489ef1932fb068478ad9e98f8417ff4fefb8d4678e8653a5771`  
		Last Modified: Thu, 25 Jun 2020 19:51:16 GMT  
		Size: 5.5 MB (5530521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.18.0-linux` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:60e9dc71017275b017a750e7be04e9c16abd50c6b6bc589ddf399588e44a509c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.5 MB (5523586 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b4b24c4ac594ac46c22186488b6b2138f48703c79ebce756ae461ac777a7b486`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 25 Jun 2020 19:02:38 GMT
COPY file:2b6e0add99a6d3c42ba8b65af53581560646dbdaf347b23e6dde1f4267fa57bc in /nats-streaming-server 
# Thu, 25 Jun 2020 19:02:38 GMT
EXPOSE 4222 8222
# Thu, 25 Jun 2020 19:02:39 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Thu, 25 Jun 2020 19:02:40 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:7af54707b9f6fd805487c0afe7fd52962e5abd3d1ab43335ccfc7224a2018844`  
		Last Modified: Thu, 25 Jun 2020 19:03:22 GMT  
		Size: 5.5 MB (5523586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.18.0-linux` - linux; arm64 variant v8

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

## `nats-streaming:0.18.0-nanoserver`

```console
$ docker pull nats-streaming@sha256:1e5b89da01e9359e18bce50086ba40b514492eff4a7979976f08ddd7cda0e7eb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1518; amd64

### `nats-streaming:0.18.0-nanoserver` - windows version 10.0.17763.1518; amd64

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

## `nats-streaming:0.18.0-nanoserver-1809`

```console
$ docker pull nats-streaming@sha256:1e5b89da01e9359e18bce50086ba40b514492eff4a7979976f08ddd7cda0e7eb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1518; amd64

### `nats-streaming:0.18.0-nanoserver-1809` - windows version 10.0.17763.1518; amd64

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

## `nats-streaming:0.18.0-scratch`

```console
$ docker pull nats-streaming@sha256:6ab20bdd5317c0c00aa163f02cbf5d430e4381f6f1ae77fba2063c797b5acbb0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.18.0-scratch` - linux; amd64

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

### `nats-streaming:0.18.0-scratch` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:95ded92d384b4d9631841677a2d34b175cba6cbb4b4fa127b7a754b9f57c849e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.5 MB (5530521 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:24577fc60833cbc345883a4b8ee0eed5044ed08c199307ea0b9f951f7d5b6d3c`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 25 Jun 2020 19:50:40 GMT
COPY file:7145d006cd221687dcd9139e9e58f09c1f07ee9ce00f3485d297197fdd5ba444 in /nats-streaming-server 
# Thu, 25 Jun 2020 19:50:41 GMT
EXPOSE 4222 8222
# Thu, 25 Jun 2020 19:50:42 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Thu, 25 Jun 2020 19:50:43 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:ef961e603a1ec489ef1932fb068478ad9e98f8417ff4fefb8d4678e8653a5771`  
		Last Modified: Thu, 25 Jun 2020 19:51:16 GMT  
		Size: 5.5 MB (5530521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.18.0-scratch` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:60e9dc71017275b017a750e7be04e9c16abd50c6b6bc589ddf399588e44a509c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.5 MB (5523586 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b4b24c4ac594ac46c22186488b6b2138f48703c79ebce756ae461ac777a7b486`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 25 Jun 2020 19:02:38 GMT
COPY file:2b6e0add99a6d3c42ba8b65af53581560646dbdaf347b23e6dde1f4267fa57bc in /nats-streaming-server 
# Thu, 25 Jun 2020 19:02:38 GMT
EXPOSE 4222 8222
# Thu, 25 Jun 2020 19:02:39 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Thu, 25 Jun 2020 19:02:40 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:7af54707b9f6fd805487c0afe7fd52962e5abd3d1ab43335ccfc7224a2018844`  
		Last Modified: Thu, 25 Jun 2020 19:03:22 GMT  
		Size: 5.5 MB (5523586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.18.0-scratch` - linux; arm64 variant v8

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

## `nats-streaming:0.18.0-windowsservercore`

```console
$ docker pull nats-streaming@sha256:703f5c6e18f6b6fb9a71e02e82d60dd49a81a1d8a019d63b0e69638f48308655
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1518; amd64
	-	windows version 10.0.14393.3986; amd64

### `nats-streaming:0.18.0-windowsservercore` - windows version 10.0.17763.1518; amd64

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

### `nats-streaming:0.18.0-windowsservercore` - windows version 10.0.14393.3986; amd64

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

## `nats-streaming:0.18.0-windowsservercore-1809`

```console
$ docker pull nats-streaming@sha256:d2a8ab1805575e9ca0eb21c568ea5bd01b41643f75dd2c2a39c1ec73eb7b7497
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1518; amd64

### `nats-streaming:0.18.0-windowsservercore-1809` - windows version 10.0.17763.1518; amd64

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

## `nats-streaming:0.18.0-windowsservercore-ltsc2016`

```console
$ docker pull nats-streaming@sha256:806b8bf4edc8956db2e8fe23a961df238868b04a2700820d4fc838407abc255b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3986; amd64

### `nats-streaming:0.18.0-windowsservercore-ltsc2016` - windows version 10.0.14393.3986; amd64

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

## `nats-streaming:0.18-alpine`

```console
$ docker pull nats-streaming@sha256:ef19a7373b6ab0b6b4a207cb550e85a7898d683aaae3d9e1361ba69d7d987541
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.18-alpine` - linux; amd64

```console
$ docker pull nats-streaming@sha256:f773acd3701babcf267f460eace482aaa2847fdb79d08850fca955fe69c12e8f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.0 MB (9015139 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:76f6db6849462b8b7abf8b8226c566f28b86a57b5b89b7771e1987f837252cc8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Thu, 25 Jun 2020 19:25:24 GMT
ENV NATS_STREAMING_SERVER=0.18.0
# Wed, 29 Jul 2020 23:26:37 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='ff2a51618b79685264f980fe868f1c7af583c419b6406cc63d4811f3c98ca8fe' ;; 		armhf) natsArch='arm6'; sha256='629e17255f12fd80e051772a6dd18a7f65e692b4abef0786b421eb8b6ab85db4' ;; 		armv7) natsArch='arm7'; sha256='94e499af6a6391519315e8bcd5127c43c1d1a442ef945956286e77b4366c92c9' ;; 		x86_64) natsArch='amd64'; sha256='6252e9262efc81a41ade3f43b68e014d1e635d3e3bf9cbcd2b09c3a030a0d5e6' ;; 		x86) natsArch='386'; sha256='886ebd2e5eb99e30ff9e9d8907d7bd49dafacffce1dc921427e5754a4ec26f55' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 29 Jul 2020 23:26:37 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Wed, 29 Jul 2020 23:26:37 GMT
EXPOSE 4222 8222
# Wed, 29 Jul 2020 23:26:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Jul 2020 23:26:37 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:df20fa9351a15782c64e6dddb2d4a6f50bf6d3688060a34c4014b0d9a752eb4c`  
		Last Modified: Fri, 29 May 2020 21:20:06 GMT  
		Size: 2.8 MB (2797541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd351f099985ea9a52973cdd0eaeff72c72744a8c9f82a1cbc8664bffc094fdb`  
		Last Modified: Wed, 29 Jul 2020 23:26:57 GMT  
		Size: 6.2 MB (6217176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd65001efde87dd38a54a1b153608623d270593a572dda8cfa5b0a144138251e`  
		Last Modified: Wed, 29 Jul 2020 23:26:55 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.18-alpine` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:e66e8c57c226879ac8535b680ee1391ef87ae2bcc5690ec7ecbf93a4066c82a6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.4 MB (8414433 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:857496a37e19bdea5173718e9e76bb7a4a0d3c535b434feabab434f0ba9e90f9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 29 May 2020 21:50:55 GMT
ADD file:f46e997a56849423db17e5fc9f0249ab6c73b155245927dba5fcb9dfd65f622f in / 
# Fri, 29 May 2020 21:50:56 GMT
CMD ["/bin/sh"]
# Thu, 25 Jun 2020 19:50:21 GMT
ENV NATS_STREAMING_SERVER=0.18.0
# Wed, 29 Jul 2020 23:01:31 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='ff2a51618b79685264f980fe868f1c7af583c419b6406cc63d4811f3c98ca8fe' ;; 		armhf) natsArch='arm6'; sha256='629e17255f12fd80e051772a6dd18a7f65e692b4abef0786b421eb8b6ab85db4' ;; 		armv7) natsArch='arm7'; sha256='94e499af6a6391519315e8bcd5127c43c1d1a442ef945956286e77b4366c92c9' ;; 		x86_64) natsArch='amd64'; sha256='6252e9262efc81a41ade3f43b68e014d1e635d3e3bf9cbcd2b09c3a030a0d5e6' ;; 		x86) natsArch='386'; sha256='886ebd2e5eb99e30ff9e9d8907d7bd49dafacffce1dc921427e5754a4ec26f55' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 29 Jul 2020 23:01:32 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Wed, 29 Jul 2020 23:01:33 GMT
EXPOSE 4222 8222
# Wed, 29 Jul 2020 23:01:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Jul 2020 23:01:34 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:b4b72e716706d29f5d2351709c20bf737b94f876a5472a43ff1b6e203c65d27f`  
		Last Modified: Fri, 29 May 2020 21:51:30 GMT  
		Size: 2.6 MB (2603286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:406c29efa0cf9678b606f95b786cc832aa806186815fb1ca94233b6704050bbc`  
		Last Modified: Wed, 29 Jul 2020 23:02:00 GMT  
		Size: 5.8 MB (5810724 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09492963cd9edfd3f0ced5fb4042e7d537ee7fde04c3880c4a91bc84f9b46a6f`  
		Last Modified: Wed, 29 Jul 2020 23:01:59 GMT  
		Size: 423.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.18-alpine` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:a20ba55bef224ae45cc82582ac9191883a54e523a0ccbbe04365a9d5f373e561
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.2 MB (8213849 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ed41b19417bfe6bc079828554b1e892e5b04728503f6b6742aaabf260080863`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 29 May 2020 21:02:07 GMT
ADD file:e97bf0d217846312b19a9f7264604851aedd125c23b4d291eed4c69b880dce26 in / 
# Fri, 29 May 2020 21:02:08 GMT
CMD ["/bin/sh"]
# Thu, 25 Jun 2020 18:58:53 GMT
ENV NATS_STREAMING_SERVER=0.18.0
# Wed, 29 Jul 2020 23:16:33 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='ff2a51618b79685264f980fe868f1c7af583c419b6406cc63d4811f3c98ca8fe' ;; 		armhf) natsArch='arm6'; sha256='629e17255f12fd80e051772a6dd18a7f65e692b4abef0786b421eb8b6ab85db4' ;; 		armv7) natsArch='arm7'; sha256='94e499af6a6391519315e8bcd5127c43c1d1a442ef945956286e77b4366c92c9' ;; 		x86_64) natsArch='amd64'; sha256='6252e9262efc81a41ade3f43b68e014d1e635d3e3bf9cbcd2b09c3a030a0d5e6' ;; 		x86) natsArch='386'; sha256='886ebd2e5eb99e30ff9e9d8907d7bd49dafacffce1dc921427e5754a4ec26f55' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 29 Jul 2020 23:16:34 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Wed, 29 Jul 2020 23:16:35 GMT
EXPOSE 4222 8222
# Wed, 29 Jul 2020 23:16:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Jul 2020 23:16:36 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:52278dd8e57993669c5b72a9620e89bebdc098f2af2379caaa8945f7403f77a2`  
		Last Modified: Fri, 29 May 2020 21:02:38 GMT  
		Size: 2.4 MB (2406763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14a1e6d591214ac54fc11baa4e27cf3cc7d9f0b6a65f186a67a96ced744cc569`  
		Last Modified: Wed, 29 Jul 2020 23:17:02 GMT  
		Size: 5.8 MB (5806663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94627b007b78566192f9591c03d4e2245b2f4943dd979b9d14d389edc2b60f96`  
		Last Modified: Wed, 29 Jul 2020 23:17:00 GMT  
		Size: 423.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.18-alpine` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:2efd83c7baf426a5da8223e4bd05f9278545d8fe81270934a16416e73c68e5b6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.5 MB (8459346 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:671f8011bed05657f23e61f2c1011683c94045a8c893ed9aab290b88aa383e94`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 29 May 2020 21:43:19 GMT
ADD file:7574aee4e37a85460ab889212d52912723a9b30dda1c060548f0deb4a05fc398 in / 
# Fri, 29 May 2020 21:43:20 GMT
CMD ["/bin/sh"]
# Fri, 24 Jul 2020 16:29:11 GMT
ENV NATS_STREAMING_SERVER=0.18.0
# Wed, 29 Jul 2020 22:39:58 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='ff2a51618b79685264f980fe868f1c7af583c419b6406cc63d4811f3c98ca8fe' ;; 		armhf) natsArch='arm6'; sha256='629e17255f12fd80e051772a6dd18a7f65e692b4abef0786b421eb8b6ab85db4' ;; 		armv7) natsArch='arm7'; sha256='94e499af6a6391519315e8bcd5127c43c1d1a442ef945956286e77b4366c92c9' ;; 		x86_64) natsArch='amd64'; sha256='6252e9262efc81a41ade3f43b68e014d1e635d3e3bf9cbcd2b09c3a030a0d5e6' ;; 		x86) natsArch='386'; sha256='886ebd2e5eb99e30ff9e9d8907d7bd49dafacffce1dc921427e5754a4ec26f55' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 29 Jul 2020 22:39:59 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Wed, 29 Jul 2020 22:39:59 GMT
EXPOSE 4222 8222
# Wed, 29 Jul 2020 22:40:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Jul 2020 22:40:00 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:b538f80385f9b48122e3da068c932a96ea5018afa3c7be79da00437414bd18cd`  
		Last Modified: Fri, 29 May 2020 21:43:57 GMT  
		Size: 2.7 MB (2707964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9b7179a5be80ec5254ffae42b351490af025c30cac276c5f48df27ba082d2c3`  
		Last Modified: Wed, 29 Jul 2020 22:40:30 GMT  
		Size: 5.8 MB (5750960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b945e4e25ec28f56f7dd8226e5e8ce479b9fb61cb6456eda8662d9d35acbd583`  
		Last Modified: Wed, 29 Jul 2020 22:40:28 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.18-alpine3.12`

```console
$ docker pull nats-streaming@sha256:ef19a7373b6ab0b6b4a207cb550e85a7898d683aaae3d9e1361ba69d7d987541
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.18-alpine3.12` - linux; amd64

```console
$ docker pull nats-streaming@sha256:f773acd3701babcf267f460eace482aaa2847fdb79d08850fca955fe69c12e8f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.0 MB (9015139 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:76f6db6849462b8b7abf8b8226c566f28b86a57b5b89b7771e1987f837252cc8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Thu, 25 Jun 2020 19:25:24 GMT
ENV NATS_STREAMING_SERVER=0.18.0
# Wed, 29 Jul 2020 23:26:37 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='ff2a51618b79685264f980fe868f1c7af583c419b6406cc63d4811f3c98ca8fe' ;; 		armhf) natsArch='arm6'; sha256='629e17255f12fd80e051772a6dd18a7f65e692b4abef0786b421eb8b6ab85db4' ;; 		armv7) natsArch='arm7'; sha256='94e499af6a6391519315e8bcd5127c43c1d1a442ef945956286e77b4366c92c9' ;; 		x86_64) natsArch='amd64'; sha256='6252e9262efc81a41ade3f43b68e014d1e635d3e3bf9cbcd2b09c3a030a0d5e6' ;; 		x86) natsArch='386'; sha256='886ebd2e5eb99e30ff9e9d8907d7bd49dafacffce1dc921427e5754a4ec26f55' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 29 Jul 2020 23:26:37 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Wed, 29 Jul 2020 23:26:37 GMT
EXPOSE 4222 8222
# Wed, 29 Jul 2020 23:26:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Jul 2020 23:26:37 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:df20fa9351a15782c64e6dddb2d4a6f50bf6d3688060a34c4014b0d9a752eb4c`  
		Last Modified: Fri, 29 May 2020 21:20:06 GMT  
		Size: 2.8 MB (2797541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd351f099985ea9a52973cdd0eaeff72c72744a8c9f82a1cbc8664bffc094fdb`  
		Last Modified: Wed, 29 Jul 2020 23:26:57 GMT  
		Size: 6.2 MB (6217176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd65001efde87dd38a54a1b153608623d270593a572dda8cfa5b0a144138251e`  
		Last Modified: Wed, 29 Jul 2020 23:26:55 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.18-alpine3.12` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:e66e8c57c226879ac8535b680ee1391ef87ae2bcc5690ec7ecbf93a4066c82a6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.4 MB (8414433 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:857496a37e19bdea5173718e9e76bb7a4a0d3c535b434feabab434f0ba9e90f9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 29 May 2020 21:50:55 GMT
ADD file:f46e997a56849423db17e5fc9f0249ab6c73b155245927dba5fcb9dfd65f622f in / 
# Fri, 29 May 2020 21:50:56 GMT
CMD ["/bin/sh"]
# Thu, 25 Jun 2020 19:50:21 GMT
ENV NATS_STREAMING_SERVER=0.18.0
# Wed, 29 Jul 2020 23:01:31 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='ff2a51618b79685264f980fe868f1c7af583c419b6406cc63d4811f3c98ca8fe' ;; 		armhf) natsArch='arm6'; sha256='629e17255f12fd80e051772a6dd18a7f65e692b4abef0786b421eb8b6ab85db4' ;; 		armv7) natsArch='arm7'; sha256='94e499af6a6391519315e8bcd5127c43c1d1a442ef945956286e77b4366c92c9' ;; 		x86_64) natsArch='amd64'; sha256='6252e9262efc81a41ade3f43b68e014d1e635d3e3bf9cbcd2b09c3a030a0d5e6' ;; 		x86) natsArch='386'; sha256='886ebd2e5eb99e30ff9e9d8907d7bd49dafacffce1dc921427e5754a4ec26f55' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 29 Jul 2020 23:01:32 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Wed, 29 Jul 2020 23:01:33 GMT
EXPOSE 4222 8222
# Wed, 29 Jul 2020 23:01:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Jul 2020 23:01:34 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:b4b72e716706d29f5d2351709c20bf737b94f876a5472a43ff1b6e203c65d27f`  
		Last Modified: Fri, 29 May 2020 21:51:30 GMT  
		Size: 2.6 MB (2603286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:406c29efa0cf9678b606f95b786cc832aa806186815fb1ca94233b6704050bbc`  
		Last Modified: Wed, 29 Jul 2020 23:02:00 GMT  
		Size: 5.8 MB (5810724 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09492963cd9edfd3f0ced5fb4042e7d537ee7fde04c3880c4a91bc84f9b46a6f`  
		Last Modified: Wed, 29 Jul 2020 23:01:59 GMT  
		Size: 423.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.18-alpine3.12` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:a20ba55bef224ae45cc82582ac9191883a54e523a0ccbbe04365a9d5f373e561
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.2 MB (8213849 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ed41b19417bfe6bc079828554b1e892e5b04728503f6b6742aaabf260080863`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 29 May 2020 21:02:07 GMT
ADD file:e97bf0d217846312b19a9f7264604851aedd125c23b4d291eed4c69b880dce26 in / 
# Fri, 29 May 2020 21:02:08 GMT
CMD ["/bin/sh"]
# Thu, 25 Jun 2020 18:58:53 GMT
ENV NATS_STREAMING_SERVER=0.18.0
# Wed, 29 Jul 2020 23:16:33 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='ff2a51618b79685264f980fe868f1c7af583c419b6406cc63d4811f3c98ca8fe' ;; 		armhf) natsArch='arm6'; sha256='629e17255f12fd80e051772a6dd18a7f65e692b4abef0786b421eb8b6ab85db4' ;; 		armv7) natsArch='arm7'; sha256='94e499af6a6391519315e8bcd5127c43c1d1a442ef945956286e77b4366c92c9' ;; 		x86_64) natsArch='amd64'; sha256='6252e9262efc81a41ade3f43b68e014d1e635d3e3bf9cbcd2b09c3a030a0d5e6' ;; 		x86) natsArch='386'; sha256='886ebd2e5eb99e30ff9e9d8907d7bd49dafacffce1dc921427e5754a4ec26f55' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 29 Jul 2020 23:16:34 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Wed, 29 Jul 2020 23:16:35 GMT
EXPOSE 4222 8222
# Wed, 29 Jul 2020 23:16:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Jul 2020 23:16:36 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:52278dd8e57993669c5b72a9620e89bebdc098f2af2379caaa8945f7403f77a2`  
		Last Modified: Fri, 29 May 2020 21:02:38 GMT  
		Size: 2.4 MB (2406763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14a1e6d591214ac54fc11baa4e27cf3cc7d9f0b6a65f186a67a96ced744cc569`  
		Last Modified: Wed, 29 Jul 2020 23:17:02 GMT  
		Size: 5.8 MB (5806663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94627b007b78566192f9591c03d4e2245b2f4943dd979b9d14d389edc2b60f96`  
		Last Modified: Wed, 29 Jul 2020 23:17:00 GMT  
		Size: 423.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.18-alpine3.12` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:2efd83c7baf426a5da8223e4bd05f9278545d8fe81270934a16416e73c68e5b6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.5 MB (8459346 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:671f8011bed05657f23e61f2c1011683c94045a8c893ed9aab290b88aa383e94`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 29 May 2020 21:43:19 GMT
ADD file:7574aee4e37a85460ab889212d52912723a9b30dda1c060548f0deb4a05fc398 in / 
# Fri, 29 May 2020 21:43:20 GMT
CMD ["/bin/sh"]
# Fri, 24 Jul 2020 16:29:11 GMT
ENV NATS_STREAMING_SERVER=0.18.0
# Wed, 29 Jul 2020 22:39:58 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='ff2a51618b79685264f980fe868f1c7af583c419b6406cc63d4811f3c98ca8fe' ;; 		armhf) natsArch='arm6'; sha256='629e17255f12fd80e051772a6dd18a7f65e692b4abef0786b421eb8b6ab85db4' ;; 		armv7) natsArch='arm7'; sha256='94e499af6a6391519315e8bcd5127c43c1d1a442ef945956286e77b4366c92c9' ;; 		x86_64) natsArch='amd64'; sha256='6252e9262efc81a41ade3f43b68e014d1e635d3e3bf9cbcd2b09c3a030a0d5e6' ;; 		x86) natsArch='386'; sha256='886ebd2e5eb99e30ff9e9d8907d7bd49dafacffce1dc921427e5754a4ec26f55' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 29 Jul 2020 22:39:59 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Wed, 29 Jul 2020 22:39:59 GMT
EXPOSE 4222 8222
# Wed, 29 Jul 2020 22:40:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Jul 2020 22:40:00 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:b538f80385f9b48122e3da068c932a96ea5018afa3c7be79da00437414bd18cd`  
		Last Modified: Fri, 29 May 2020 21:43:57 GMT  
		Size: 2.7 MB (2707964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9b7179a5be80ec5254ffae42b351490af025c30cac276c5f48df27ba082d2c3`  
		Last Modified: Wed, 29 Jul 2020 22:40:30 GMT  
		Size: 5.8 MB (5750960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b945e4e25ec28f56f7dd8226e5e8ce479b9fb61cb6456eda8662d9d35acbd583`  
		Last Modified: Wed, 29 Jul 2020 22:40:28 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.18-linux`

```console
$ docker pull nats-streaming@sha256:6ab20bdd5317c0c00aa163f02cbf5d430e4381f6f1ae77fba2063c797b5acbb0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.18-linux` - linux; amd64

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

### `nats-streaming:0.18-linux` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:95ded92d384b4d9631841677a2d34b175cba6cbb4b4fa127b7a754b9f57c849e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.5 MB (5530521 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:24577fc60833cbc345883a4b8ee0eed5044ed08c199307ea0b9f951f7d5b6d3c`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 25 Jun 2020 19:50:40 GMT
COPY file:7145d006cd221687dcd9139e9e58f09c1f07ee9ce00f3485d297197fdd5ba444 in /nats-streaming-server 
# Thu, 25 Jun 2020 19:50:41 GMT
EXPOSE 4222 8222
# Thu, 25 Jun 2020 19:50:42 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Thu, 25 Jun 2020 19:50:43 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:ef961e603a1ec489ef1932fb068478ad9e98f8417ff4fefb8d4678e8653a5771`  
		Last Modified: Thu, 25 Jun 2020 19:51:16 GMT  
		Size: 5.5 MB (5530521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.18-linux` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:60e9dc71017275b017a750e7be04e9c16abd50c6b6bc589ddf399588e44a509c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.5 MB (5523586 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b4b24c4ac594ac46c22186488b6b2138f48703c79ebce756ae461ac777a7b486`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 25 Jun 2020 19:02:38 GMT
COPY file:2b6e0add99a6d3c42ba8b65af53581560646dbdaf347b23e6dde1f4267fa57bc in /nats-streaming-server 
# Thu, 25 Jun 2020 19:02:38 GMT
EXPOSE 4222 8222
# Thu, 25 Jun 2020 19:02:39 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Thu, 25 Jun 2020 19:02:40 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:7af54707b9f6fd805487c0afe7fd52962e5abd3d1ab43335ccfc7224a2018844`  
		Last Modified: Thu, 25 Jun 2020 19:03:22 GMT  
		Size: 5.5 MB (5523586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.18-linux` - linux; arm64 variant v8

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

## `nats-streaming:0.18-nanoserver`

```console
$ docker pull nats-streaming@sha256:1e5b89da01e9359e18bce50086ba40b514492eff4a7979976f08ddd7cda0e7eb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1518; amd64

### `nats-streaming:0.18-nanoserver` - windows version 10.0.17763.1518; amd64

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

## `nats-streaming:0.18-nanoserver-1809`

```console
$ docker pull nats-streaming@sha256:1e5b89da01e9359e18bce50086ba40b514492eff4a7979976f08ddd7cda0e7eb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1518; amd64

### `nats-streaming:0.18-nanoserver-1809` - windows version 10.0.17763.1518; amd64

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

## `nats-streaming:0.18-scratch`

```console
$ docker pull nats-streaming@sha256:6ab20bdd5317c0c00aa163f02cbf5d430e4381f6f1ae77fba2063c797b5acbb0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.18-scratch` - linux; amd64

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

### `nats-streaming:0.18-scratch` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:95ded92d384b4d9631841677a2d34b175cba6cbb4b4fa127b7a754b9f57c849e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.5 MB (5530521 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:24577fc60833cbc345883a4b8ee0eed5044ed08c199307ea0b9f951f7d5b6d3c`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 25 Jun 2020 19:50:40 GMT
COPY file:7145d006cd221687dcd9139e9e58f09c1f07ee9ce00f3485d297197fdd5ba444 in /nats-streaming-server 
# Thu, 25 Jun 2020 19:50:41 GMT
EXPOSE 4222 8222
# Thu, 25 Jun 2020 19:50:42 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Thu, 25 Jun 2020 19:50:43 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:ef961e603a1ec489ef1932fb068478ad9e98f8417ff4fefb8d4678e8653a5771`  
		Last Modified: Thu, 25 Jun 2020 19:51:16 GMT  
		Size: 5.5 MB (5530521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.18-scratch` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:60e9dc71017275b017a750e7be04e9c16abd50c6b6bc589ddf399588e44a509c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.5 MB (5523586 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b4b24c4ac594ac46c22186488b6b2138f48703c79ebce756ae461ac777a7b486`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 25 Jun 2020 19:02:38 GMT
COPY file:2b6e0add99a6d3c42ba8b65af53581560646dbdaf347b23e6dde1f4267fa57bc in /nats-streaming-server 
# Thu, 25 Jun 2020 19:02:38 GMT
EXPOSE 4222 8222
# Thu, 25 Jun 2020 19:02:39 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Thu, 25 Jun 2020 19:02:40 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:7af54707b9f6fd805487c0afe7fd52962e5abd3d1ab43335ccfc7224a2018844`  
		Last Modified: Thu, 25 Jun 2020 19:03:22 GMT  
		Size: 5.5 MB (5523586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.18-scratch` - linux; arm64 variant v8

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

## `nats-streaming:0.18-windowsservercore`

```console
$ docker pull nats-streaming@sha256:703f5c6e18f6b6fb9a71e02e82d60dd49a81a1d8a019d63b0e69638f48308655
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1518; amd64
	-	windows version 10.0.14393.3986; amd64

### `nats-streaming:0.18-windowsservercore` - windows version 10.0.17763.1518; amd64

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

### `nats-streaming:0.18-windowsservercore` - windows version 10.0.14393.3986; amd64

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

## `nats-streaming:0.18-windowsservercore-1809`

```console
$ docker pull nats-streaming@sha256:d2a8ab1805575e9ca0eb21c568ea5bd01b41643f75dd2c2a39c1ec73eb7b7497
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1518; amd64

### `nats-streaming:0.18-windowsservercore-1809` - windows version 10.0.17763.1518; amd64

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

## `nats-streaming:0.18-windowsservercore-ltsc2016`

```console
$ docker pull nats-streaming@sha256:806b8bf4edc8956db2e8fe23a961df238868b04a2700820d4fc838407abc255b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3986; amd64

### `nats-streaming:0.18-windowsservercore-ltsc2016` - windows version 10.0.14393.3986; amd64

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

## `nats-streaming:alpine`

```console
$ docker pull nats-streaming@sha256:ef19a7373b6ab0b6b4a207cb550e85a7898d683aaae3d9e1361ba69d7d987541
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:alpine` - linux; amd64

```console
$ docker pull nats-streaming@sha256:f773acd3701babcf267f460eace482aaa2847fdb79d08850fca955fe69c12e8f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.0 MB (9015139 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:76f6db6849462b8b7abf8b8226c566f28b86a57b5b89b7771e1987f837252cc8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Thu, 25 Jun 2020 19:25:24 GMT
ENV NATS_STREAMING_SERVER=0.18.0
# Wed, 29 Jul 2020 23:26:37 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='ff2a51618b79685264f980fe868f1c7af583c419b6406cc63d4811f3c98ca8fe' ;; 		armhf) natsArch='arm6'; sha256='629e17255f12fd80e051772a6dd18a7f65e692b4abef0786b421eb8b6ab85db4' ;; 		armv7) natsArch='arm7'; sha256='94e499af6a6391519315e8bcd5127c43c1d1a442ef945956286e77b4366c92c9' ;; 		x86_64) natsArch='amd64'; sha256='6252e9262efc81a41ade3f43b68e014d1e635d3e3bf9cbcd2b09c3a030a0d5e6' ;; 		x86) natsArch='386'; sha256='886ebd2e5eb99e30ff9e9d8907d7bd49dafacffce1dc921427e5754a4ec26f55' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 29 Jul 2020 23:26:37 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Wed, 29 Jul 2020 23:26:37 GMT
EXPOSE 4222 8222
# Wed, 29 Jul 2020 23:26:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Jul 2020 23:26:37 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:df20fa9351a15782c64e6dddb2d4a6f50bf6d3688060a34c4014b0d9a752eb4c`  
		Last Modified: Fri, 29 May 2020 21:20:06 GMT  
		Size: 2.8 MB (2797541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd351f099985ea9a52973cdd0eaeff72c72744a8c9f82a1cbc8664bffc094fdb`  
		Last Modified: Wed, 29 Jul 2020 23:26:57 GMT  
		Size: 6.2 MB (6217176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd65001efde87dd38a54a1b153608623d270593a572dda8cfa5b0a144138251e`  
		Last Modified: Wed, 29 Jul 2020 23:26:55 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:e66e8c57c226879ac8535b680ee1391ef87ae2bcc5690ec7ecbf93a4066c82a6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.4 MB (8414433 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:857496a37e19bdea5173718e9e76bb7a4a0d3c535b434feabab434f0ba9e90f9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 29 May 2020 21:50:55 GMT
ADD file:f46e997a56849423db17e5fc9f0249ab6c73b155245927dba5fcb9dfd65f622f in / 
# Fri, 29 May 2020 21:50:56 GMT
CMD ["/bin/sh"]
# Thu, 25 Jun 2020 19:50:21 GMT
ENV NATS_STREAMING_SERVER=0.18.0
# Wed, 29 Jul 2020 23:01:31 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='ff2a51618b79685264f980fe868f1c7af583c419b6406cc63d4811f3c98ca8fe' ;; 		armhf) natsArch='arm6'; sha256='629e17255f12fd80e051772a6dd18a7f65e692b4abef0786b421eb8b6ab85db4' ;; 		armv7) natsArch='arm7'; sha256='94e499af6a6391519315e8bcd5127c43c1d1a442ef945956286e77b4366c92c9' ;; 		x86_64) natsArch='amd64'; sha256='6252e9262efc81a41ade3f43b68e014d1e635d3e3bf9cbcd2b09c3a030a0d5e6' ;; 		x86) natsArch='386'; sha256='886ebd2e5eb99e30ff9e9d8907d7bd49dafacffce1dc921427e5754a4ec26f55' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 29 Jul 2020 23:01:32 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Wed, 29 Jul 2020 23:01:33 GMT
EXPOSE 4222 8222
# Wed, 29 Jul 2020 23:01:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Jul 2020 23:01:34 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:b4b72e716706d29f5d2351709c20bf737b94f876a5472a43ff1b6e203c65d27f`  
		Last Modified: Fri, 29 May 2020 21:51:30 GMT  
		Size: 2.6 MB (2603286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:406c29efa0cf9678b606f95b786cc832aa806186815fb1ca94233b6704050bbc`  
		Last Modified: Wed, 29 Jul 2020 23:02:00 GMT  
		Size: 5.8 MB (5810724 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09492963cd9edfd3f0ced5fb4042e7d537ee7fde04c3880c4a91bc84f9b46a6f`  
		Last Modified: Wed, 29 Jul 2020 23:01:59 GMT  
		Size: 423.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:a20ba55bef224ae45cc82582ac9191883a54e523a0ccbbe04365a9d5f373e561
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.2 MB (8213849 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ed41b19417bfe6bc079828554b1e892e5b04728503f6b6742aaabf260080863`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 29 May 2020 21:02:07 GMT
ADD file:e97bf0d217846312b19a9f7264604851aedd125c23b4d291eed4c69b880dce26 in / 
# Fri, 29 May 2020 21:02:08 GMT
CMD ["/bin/sh"]
# Thu, 25 Jun 2020 18:58:53 GMT
ENV NATS_STREAMING_SERVER=0.18.0
# Wed, 29 Jul 2020 23:16:33 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='ff2a51618b79685264f980fe868f1c7af583c419b6406cc63d4811f3c98ca8fe' ;; 		armhf) natsArch='arm6'; sha256='629e17255f12fd80e051772a6dd18a7f65e692b4abef0786b421eb8b6ab85db4' ;; 		armv7) natsArch='arm7'; sha256='94e499af6a6391519315e8bcd5127c43c1d1a442ef945956286e77b4366c92c9' ;; 		x86_64) natsArch='amd64'; sha256='6252e9262efc81a41ade3f43b68e014d1e635d3e3bf9cbcd2b09c3a030a0d5e6' ;; 		x86) natsArch='386'; sha256='886ebd2e5eb99e30ff9e9d8907d7bd49dafacffce1dc921427e5754a4ec26f55' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 29 Jul 2020 23:16:34 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Wed, 29 Jul 2020 23:16:35 GMT
EXPOSE 4222 8222
# Wed, 29 Jul 2020 23:16:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Jul 2020 23:16:36 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:52278dd8e57993669c5b72a9620e89bebdc098f2af2379caaa8945f7403f77a2`  
		Last Modified: Fri, 29 May 2020 21:02:38 GMT  
		Size: 2.4 MB (2406763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14a1e6d591214ac54fc11baa4e27cf3cc7d9f0b6a65f186a67a96ced744cc569`  
		Last Modified: Wed, 29 Jul 2020 23:17:02 GMT  
		Size: 5.8 MB (5806663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94627b007b78566192f9591c03d4e2245b2f4943dd979b9d14d389edc2b60f96`  
		Last Modified: Wed, 29 Jul 2020 23:17:00 GMT  
		Size: 423.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:2efd83c7baf426a5da8223e4bd05f9278545d8fe81270934a16416e73c68e5b6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.5 MB (8459346 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:671f8011bed05657f23e61f2c1011683c94045a8c893ed9aab290b88aa383e94`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 29 May 2020 21:43:19 GMT
ADD file:7574aee4e37a85460ab889212d52912723a9b30dda1c060548f0deb4a05fc398 in / 
# Fri, 29 May 2020 21:43:20 GMT
CMD ["/bin/sh"]
# Fri, 24 Jul 2020 16:29:11 GMT
ENV NATS_STREAMING_SERVER=0.18.0
# Wed, 29 Jul 2020 22:39:58 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='ff2a51618b79685264f980fe868f1c7af583c419b6406cc63d4811f3c98ca8fe' ;; 		armhf) natsArch='arm6'; sha256='629e17255f12fd80e051772a6dd18a7f65e692b4abef0786b421eb8b6ab85db4' ;; 		armv7) natsArch='arm7'; sha256='94e499af6a6391519315e8bcd5127c43c1d1a442ef945956286e77b4366c92c9' ;; 		x86_64) natsArch='amd64'; sha256='6252e9262efc81a41ade3f43b68e014d1e635d3e3bf9cbcd2b09c3a030a0d5e6' ;; 		x86) natsArch='386'; sha256='886ebd2e5eb99e30ff9e9d8907d7bd49dafacffce1dc921427e5754a4ec26f55' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 29 Jul 2020 22:39:59 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Wed, 29 Jul 2020 22:39:59 GMT
EXPOSE 4222 8222
# Wed, 29 Jul 2020 22:40:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Jul 2020 22:40:00 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:b538f80385f9b48122e3da068c932a96ea5018afa3c7be79da00437414bd18cd`  
		Last Modified: Fri, 29 May 2020 21:43:57 GMT  
		Size: 2.7 MB (2707964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9b7179a5be80ec5254ffae42b351490af025c30cac276c5f48df27ba082d2c3`  
		Last Modified: Wed, 29 Jul 2020 22:40:30 GMT  
		Size: 5.8 MB (5750960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b945e4e25ec28f56f7dd8226e5e8ce479b9fb61cb6456eda8662d9d35acbd583`  
		Last Modified: Wed, 29 Jul 2020 22:40:28 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:alpine3.12`

```console
$ docker pull nats-streaming@sha256:ef19a7373b6ab0b6b4a207cb550e85a7898d683aaae3d9e1361ba69d7d987541
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:alpine3.12` - linux; amd64

```console
$ docker pull nats-streaming@sha256:f773acd3701babcf267f460eace482aaa2847fdb79d08850fca955fe69c12e8f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.0 MB (9015139 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:76f6db6849462b8b7abf8b8226c566f28b86a57b5b89b7771e1987f837252cc8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Thu, 25 Jun 2020 19:25:24 GMT
ENV NATS_STREAMING_SERVER=0.18.0
# Wed, 29 Jul 2020 23:26:37 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='ff2a51618b79685264f980fe868f1c7af583c419b6406cc63d4811f3c98ca8fe' ;; 		armhf) natsArch='arm6'; sha256='629e17255f12fd80e051772a6dd18a7f65e692b4abef0786b421eb8b6ab85db4' ;; 		armv7) natsArch='arm7'; sha256='94e499af6a6391519315e8bcd5127c43c1d1a442ef945956286e77b4366c92c9' ;; 		x86_64) natsArch='amd64'; sha256='6252e9262efc81a41ade3f43b68e014d1e635d3e3bf9cbcd2b09c3a030a0d5e6' ;; 		x86) natsArch='386'; sha256='886ebd2e5eb99e30ff9e9d8907d7bd49dafacffce1dc921427e5754a4ec26f55' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 29 Jul 2020 23:26:37 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Wed, 29 Jul 2020 23:26:37 GMT
EXPOSE 4222 8222
# Wed, 29 Jul 2020 23:26:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Jul 2020 23:26:37 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:df20fa9351a15782c64e6dddb2d4a6f50bf6d3688060a34c4014b0d9a752eb4c`  
		Last Modified: Fri, 29 May 2020 21:20:06 GMT  
		Size: 2.8 MB (2797541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd351f099985ea9a52973cdd0eaeff72c72744a8c9f82a1cbc8664bffc094fdb`  
		Last Modified: Wed, 29 Jul 2020 23:26:57 GMT  
		Size: 6.2 MB (6217176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd65001efde87dd38a54a1b153608623d270593a572dda8cfa5b0a144138251e`  
		Last Modified: Wed, 29 Jul 2020 23:26:55 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine3.12` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:e66e8c57c226879ac8535b680ee1391ef87ae2bcc5690ec7ecbf93a4066c82a6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.4 MB (8414433 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:857496a37e19bdea5173718e9e76bb7a4a0d3c535b434feabab434f0ba9e90f9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 29 May 2020 21:50:55 GMT
ADD file:f46e997a56849423db17e5fc9f0249ab6c73b155245927dba5fcb9dfd65f622f in / 
# Fri, 29 May 2020 21:50:56 GMT
CMD ["/bin/sh"]
# Thu, 25 Jun 2020 19:50:21 GMT
ENV NATS_STREAMING_SERVER=0.18.0
# Wed, 29 Jul 2020 23:01:31 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='ff2a51618b79685264f980fe868f1c7af583c419b6406cc63d4811f3c98ca8fe' ;; 		armhf) natsArch='arm6'; sha256='629e17255f12fd80e051772a6dd18a7f65e692b4abef0786b421eb8b6ab85db4' ;; 		armv7) natsArch='arm7'; sha256='94e499af6a6391519315e8bcd5127c43c1d1a442ef945956286e77b4366c92c9' ;; 		x86_64) natsArch='amd64'; sha256='6252e9262efc81a41ade3f43b68e014d1e635d3e3bf9cbcd2b09c3a030a0d5e6' ;; 		x86) natsArch='386'; sha256='886ebd2e5eb99e30ff9e9d8907d7bd49dafacffce1dc921427e5754a4ec26f55' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 29 Jul 2020 23:01:32 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Wed, 29 Jul 2020 23:01:33 GMT
EXPOSE 4222 8222
# Wed, 29 Jul 2020 23:01:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Jul 2020 23:01:34 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:b4b72e716706d29f5d2351709c20bf737b94f876a5472a43ff1b6e203c65d27f`  
		Last Modified: Fri, 29 May 2020 21:51:30 GMT  
		Size: 2.6 MB (2603286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:406c29efa0cf9678b606f95b786cc832aa806186815fb1ca94233b6704050bbc`  
		Last Modified: Wed, 29 Jul 2020 23:02:00 GMT  
		Size: 5.8 MB (5810724 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09492963cd9edfd3f0ced5fb4042e7d537ee7fde04c3880c4a91bc84f9b46a6f`  
		Last Modified: Wed, 29 Jul 2020 23:01:59 GMT  
		Size: 423.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine3.12` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:a20ba55bef224ae45cc82582ac9191883a54e523a0ccbbe04365a9d5f373e561
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.2 MB (8213849 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ed41b19417bfe6bc079828554b1e892e5b04728503f6b6742aaabf260080863`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 29 May 2020 21:02:07 GMT
ADD file:e97bf0d217846312b19a9f7264604851aedd125c23b4d291eed4c69b880dce26 in / 
# Fri, 29 May 2020 21:02:08 GMT
CMD ["/bin/sh"]
# Thu, 25 Jun 2020 18:58:53 GMT
ENV NATS_STREAMING_SERVER=0.18.0
# Wed, 29 Jul 2020 23:16:33 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='ff2a51618b79685264f980fe868f1c7af583c419b6406cc63d4811f3c98ca8fe' ;; 		armhf) natsArch='arm6'; sha256='629e17255f12fd80e051772a6dd18a7f65e692b4abef0786b421eb8b6ab85db4' ;; 		armv7) natsArch='arm7'; sha256='94e499af6a6391519315e8bcd5127c43c1d1a442ef945956286e77b4366c92c9' ;; 		x86_64) natsArch='amd64'; sha256='6252e9262efc81a41ade3f43b68e014d1e635d3e3bf9cbcd2b09c3a030a0d5e6' ;; 		x86) natsArch='386'; sha256='886ebd2e5eb99e30ff9e9d8907d7bd49dafacffce1dc921427e5754a4ec26f55' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 29 Jul 2020 23:16:34 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Wed, 29 Jul 2020 23:16:35 GMT
EXPOSE 4222 8222
# Wed, 29 Jul 2020 23:16:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Jul 2020 23:16:36 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:52278dd8e57993669c5b72a9620e89bebdc098f2af2379caaa8945f7403f77a2`  
		Last Modified: Fri, 29 May 2020 21:02:38 GMT  
		Size: 2.4 MB (2406763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14a1e6d591214ac54fc11baa4e27cf3cc7d9f0b6a65f186a67a96ced744cc569`  
		Last Modified: Wed, 29 Jul 2020 23:17:02 GMT  
		Size: 5.8 MB (5806663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94627b007b78566192f9591c03d4e2245b2f4943dd979b9d14d389edc2b60f96`  
		Last Modified: Wed, 29 Jul 2020 23:17:00 GMT  
		Size: 423.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine3.12` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:2efd83c7baf426a5da8223e4bd05f9278545d8fe81270934a16416e73c68e5b6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.5 MB (8459346 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:671f8011bed05657f23e61f2c1011683c94045a8c893ed9aab290b88aa383e94`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 29 May 2020 21:43:19 GMT
ADD file:7574aee4e37a85460ab889212d52912723a9b30dda1c060548f0deb4a05fc398 in / 
# Fri, 29 May 2020 21:43:20 GMT
CMD ["/bin/sh"]
# Fri, 24 Jul 2020 16:29:11 GMT
ENV NATS_STREAMING_SERVER=0.18.0
# Wed, 29 Jul 2020 22:39:58 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='ff2a51618b79685264f980fe868f1c7af583c419b6406cc63d4811f3c98ca8fe' ;; 		armhf) natsArch='arm6'; sha256='629e17255f12fd80e051772a6dd18a7f65e692b4abef0786b421eb8b6ab85db4' ;; 		armv7) natsArch='arm7'; sha256='94e499af6a6391519315e8bcd5127c43c1d1a442ef945956286e77b4366c92c9' ;; 		x86_64) natsArch='amd64'; sha256='6252e9262efc81a41ade3f43b68e014d1e635d3e3bf9cbcd2b09c3a030a0d5e6' ;; 		x86) natsArch='386'; sha256='886ebd2e5eb99e30ff9e9d8907d7bd49dafacffce1dc921427e5754a4ec26f55' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 29 Jul 2020 22:39:59 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Wed, 29 Jul 2020 22:39:59 GMT
EXPOSE 4222 8222
# Wed, 29 Jul 2020 22:40:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Jul 2020 22:40:00 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:b538f80385f9b48122e3da068c932a96ea5018afa3c7be79da00437414bd18cd`  
		Last Modified: Fri, 29 May 2020 21:43:57 GMT  
		Size: 2.7 MB (2707964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9b7179a5be80ec5254ffae42b351490af025c30cac276c5f48df27ba082d2c3`  
		Last Modified: Wed, 29 Jul 2020 22:40:30 GMT  
		Size: 5.8 MB (5750960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b945e4e25ec28f56f7dd8226e5e8ce479b9fb61cb6456eda8662d9d35acbd583`  
		Last Modified: Wed, 29 Jul 2020 22:40:28 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:latest`

```console
$ docker pull nats-streaming@sha256:b6a6edcfc853b2e70689250639914f0a9f8e3ea21027548861ccb673d208114e
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
$ docker pull nats-streaming@sha256:95ded92d384b4d9631841677a2d34b175cba6cbb4b4fa127b7a754b9f57c849e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.5 MB (5530521 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:24577fc60833cbc345883a4b8ee0eed5044ed08c199307ea0b9f951f7d5b6d3c`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 25 Jun 2020 19:50:40 GMT
COPY file:7145d006cd221687dcd9139e9e58f09c1f07ee9ce00f3485d297197fdd5ba444 in /nats-streaming-server 
# Thu, 25 Jun 2020 19:50:41 GMT
EXPOSE 4222 8222
# Thu, 25 Jun 2020 19:50:42 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Thu, 25 Jun 2020 19:50:43 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:ef961e603a1ec489ef1932fb068478ad9e98f8417ff4fefb8d4678e8653a5771`  
		Last Modified: Thu, 25 Jun 2020 19:51:16 GMT  
		Size: 5.5 MB (5530521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:latest` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:60e9dc71017275b017a750e7be04e9c16abd50c6b6bc589ddf399588e44a509c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.5 MB (5523586 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b4b24c4ac594ac46c22186488b6b2138f48703c79ebce756ae461ac777a7b486`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 25 Jun 2020 19:02:38 GMT
COPY file:2b6e0add99a6d3c42ba8b65af53581560646dbdaf347b23e6dde1f4267fa57bc in /nats-streaming-server 
# Thu, 25 Jun 2020 19:02:38 GMT
EXPOSE 4222 8222
# Thu, 25 Jun 2020 19:02:39 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Thu, 25 Jun 2020 19:02:40 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:7af54707b9f6fd805487c0afe7fd52962e5abd3d1ab43335ccfc7224a2018844`  
		Last Modified: Thu, 25 Jun 2020 19:03:22 GMT  
		Size: 5.5 MB (5523586 bytes)  
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
$ docker pull nats-streaming@sha256:6ab20bdd5317c0c00aa163f02cbf5d430e4381f6f1ae77fba2063c797b5acbb0
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
$ docker pull nats-streaming@sha256:95ded92d384b4d9631841677a2d34b175cba6cbb4b4fa127b7a754b9f57c849e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.5 MB (5530521 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:24577fc60833cbc345883a4b8ee0eed5044ed08c199307ea0b9f951f7d5b6d3c`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 25 Jun 2020 19:50:40 GMT
COPY file:7145d006cd221687dcd9139e9e58f09c1f07ee9ce00f3485d297197fdd5ba444 in /nats-streaming-server 
# Thu, 25 Jun 2020 19:50:41 GMT
EXPOSE 4222 8222
# Thu, 25 Jun 2020 19:50:42 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Thu, 25 Jun 2020 19:50:43 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:ef961e603a1ec489ef1932fb068478ad9e98f8417ff4fefb8d4678e8653a5771`  
		Last Modified: Thu, 25 Jun 2020 19:51:16 GMT  
		Size: 5.5 MB (5530521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:linux` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:60e9dc71017275b017a750e7be04e9c16abd50c6b6bc589ddf399588e44a509c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.5 MB (5523586 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b4b24c4ac594ac46c22186488b6b2138f48703c79ebce756ae461ac777a7b486`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 25 Jun 2020 19:02:38 GMT
COPY file:2b6e0add99a6d3c42ba8b65af53581560646dbdaf347b23e6dde1f4267fa57bc in /nats-streaming-server 
# Thu, 25 Jun 2020 19:02:38 GMT
EXPOSE 4222 8222
# Thu, 25 Jun 2020 19:02:39 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Thu, 25 Jun 2020 19:02:40 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:7af54707b9f6fd805487c0afe7fd52962e5abd3d1ab43335ccfc7224a2018844`  
		Last Modified: Thu, 25 Jun 2020 19:03:22 GMT  
		Size: 5.5 MB (5523586 bytes)  
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
$ docker pull nats-streaming@sha256:6ab20bdd5317c0c00aa163f02cbf5d430e4381f6f1ae77fba2063c797b5acbb0
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
$ docker pull nats-streaming@sha256:95ded92d384b4d9631841677a2d34b175cba6cbb4b4fa127b7a754b9f57c849e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.5 MB (5530521 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:24577fc60833cbc345883a4b8ee0eed5044ed08c199307ea0b9f951f7d5b6d3c`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 25 Jun 2020 19:50:40 GMT
COPY file:7145d006cd221687dcd9139e9e58f09c1f07ee9ce00f3485d297197fdd5ba444 in /nats-streaming-server 
# Thu, 25 Jun 2020 19:50:41 GMT
EXPOSE 4222 8222
# Thu, 25 Jun 2020 19:50:42 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Thu, 25 Jun 2020 19:50:43 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:ef961e603a1ec489ef1932fb068478ad9e98f8417ff4fefb8d4678e8653a5771`  
		Last Modified: Thu, 25 Jun 2020 19:51:16 GMT  
		Size: 5.5 MB (5530521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:scratch` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:60e9dc71017275b017a750e7be04e9c16abd50c6b6bc589ddf399588e44a509c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.5 MB (5523586 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b4b24c4ac594ac46c22186488b6b2138f48703c79ebce756ae461ac777a7b486`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 25 Jun 2020 19:02:38 GMT
COPY file:2b6e0add99a6d3c42ba8b65af53581560646dbdaf347b23e6dde1f4267fa57bc in /nats-streaming-server 
# Thu, 25 Jun 2020 19:02:38 GMT
EXPOSE 4222 8222
# Thu, 25 Jun 2020 19:02:39 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Thu, 25 Jun 2020 19:02:40 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:7af54707b9f6fd805487c0afe7fd52962e5abd3d1ab43335ccfc7224a2018844`  
		Last Modified: Thu, 25 Jun 2020 19:03:22 GMT  
		Size: 5.5 MB (5523586 bytes)  
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
