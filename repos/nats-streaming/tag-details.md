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
$ docker pull nats-streaming@sha256:46f30dff859ef0690c053a1a9514adbc3bcba3210b9565c940813498ac3db83d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.1339; amd64

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

### `nats-streaming:0.18` - windows version 10.0.17763.1339; amd64

```console
$ docker pull nats-streaming@sha256:536fc04821f79ce86cbaffab4f58b9bb1b2e697f4f1d17b263e02270d1edba47
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.8 MB (106843336 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:40d8dcc1cfa38989cad5eccdc9993517e290c787fc43f466403bd00c1a7ba261`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 07 Jul 2020 13:50:07 GMT
RUN Apply image 1809-amd64
# Wed, 15 Jul 2020 15:05:14 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 15 Jul 2020 21:09:37 GMT
RUN cmd /S /C #(nop) COPY file:4a858ac4da943f868519572e3fb6817fd379875f2bff0bcb5f03c5bdddc496a8 in C:\nats-streaming-server.exe 
# Wed, 15 Jul 2020 21:09:40 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 15 Jul 2020 21:09:40 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 15 Jul 2020 21:09:41 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:dc95608099543221ef539391bfece5c1ce37b97af9da457f5990349cab028a12`  
		Size: 100.9 MB (100895619 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5f0c27d781c53928c03429d5b34e0f49fc26b7e7c996c1d9a2a8474162eade60`  
		Last Modified: Wed, 15 Jul 2020 15:09:50 GMT  
		Size: 869.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c37823d2bd2a59a1d84d807658bb5995febdf048b1f99233390d2b049939efd1`  
		Last Modified: Wed, 15 Jul 2020 21:14:05 GMT  
		Size: 5.9 MB (5944137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9fe8f765dc0de3583e36e3f3ef18e3a3f3a3f75312e35ac1d42c0d95ce90cc0`  
		Last Modified: Wed, 15 Jul 2020 21:14:04 GMT  
		Size: 906.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:349d8da345d930244c13a48049c9f9001d4a04866a33ee215586352c788b5e88`  
		Last Modified: Wed, 15 Jul 2020 21:14:01 GMT  
		Size: 913.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32f6fe573eab456a9f7b72357c56803fb00bdc82c4919d22ab75252383bf5bd9`  
		Last Modified: Wed, 15 Jul 2020 21:14:01 GMT  
		Size: 892.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.18.0`

```console
$ docker pull nats-streaming@sha256:46f30dff859ef0690c053a1a9514adbc3bcba3210b9565c940813498ac3db83d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.1339; amd64

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

### `nats-streaming:0.18.0` - windows version 10.0.17763.1339; amd64

```console
$ docker pull nats-streaming@sha256:536fc04821f79ce86cbaffab4f58b9bb1b2e697f4f1d17b263e02270d1edba47
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.8 MB (106843336 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:40d8dcc1cfa38989cad5eccdc9993517e290c787fc43f466403bd00c1a7ba261`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 07 Jul 2020 13:50:07 GMT
RUN Apply image 1809-amd64
# Wed, 15 Jul 2020 15:05:14 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 15 Jul 2020 21:09:37 GMT
RUN cmd /S /C #(nop) COPY file:4a858ac4da943f868519572e3fb6817fd379875f2bff0bcb5f03c5bdddc496a8 in C:\nats-streaming-server.exe 
# Wed, 15 Jul 2020 21:09:40 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 15 Jul 2020 21:09:40 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 15 Jul 2020 21:09:41 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:dc95608099543221ef539391bfece5c1ce37b97af9da457f5990349cab028a12`  
		Size: 100.9 MB (100895619 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5f0c27d781c53928c03429d5b34e0f49fc26b7e7c996c1d9a2a8474162eade60`  
		Last Modified: Wed, 15 Jul 2020 15:09:50 GMT  
		Size: 869.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c37823d2bd2a59a1d84d807658bb5995febdf048b1f99233390d2b049939efd1`  
		Last Modified: Wed, 15 Jul 2020 21:14:05 GMT  
		Size: 5.9 MB (5944137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9fe8f765dc0de3583e36e3f3ef18e3a3f3a3f75312e35ac1d42c0d95ce90cc0`  
		Last Modified: Wed, 15 Jul 2020 21:14:04 GMT  
		Size: 906.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:349d8da345d930244c13a48049c9f9001d4a04866a33ee215586352c788b5e88`  
		Last Modified: Wed, 15 Jul 2020 21:14:01 GMT  
		Size: 913.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32f6fe573eab456a9f7b72357c56803fb00bdc82c4919d22ab75252383bf5bd9`  
		Last Modified: Wed, 15 Jul 2020 21:14:01 GMT  
		Size: 892.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.18.0-alpine`

```console
$ docker pull nats-streaming@sha256:83affddfe9cc74a10f8b960f772b4b6afbdf6ce3a73699ed6c31c0c6c4a7bf22
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.18.0-alpine` - linux; amd64

```console
$ docker pull nats-streaming@sha256:9f71614879c6e9c774410e5315004fc3f6b8f2e52a6e1c6dbe2f203e6c285df0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.0 MB (9015136 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a5b225e159253af34dce2a69079773d857596bf528268a384b2fd1a0b8af6f3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Thu, 25 Jun 2020 19:25:24 GMT
ENV NATS_STREAMING_SERVER=0.18.0
# Thu, 25 Jun 2020 19:25:26 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		arm64) natsArch='arm64'; sha256='ff2a51618b79685264f980fe868f1c7af583c419b6406cc63d4811f3c98ca8fe' ;; 		armhf) natsArch='arm6'; sha256='629e17255f12fd80e051772a6dd18a7f65e692b4abef0786b421eb8b6ab85db4' ;; 		armv7) natsArch='arm7'; sha256='94e499af6a6391519315e8bcd5127c43c1d1a442ef945956286e77b4366c92c9' ;; 		x86_64) natsArch='amd64'; sha256='6252e9262efc81a41ade3f43b68e014d1e635d3e3bf9cbcd2b09c3a030a0d5e6' ;; 		x86) natsArch='386'; sha256='886ebd2e5eb99e30ff9e9d8907d7bd49dafacffce1dc921427e5754a4ec26f55' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 25 Jun 2020 19:25:26 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Thu, 25 Jun 2020 19:25:26 GMT
EXPOSE 4222 8222
# Thu, 25 Jun 2020 19:25:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 25 Jun 2020 19:25:26 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:df20fa9351a15782c64e6dddb2d4a6f50bf6d3688060a34c4014b0d9a752eb4c`  
		Last Modified: Fri, 29 May 2020 21:20:06 GMT  
		Size: 2.8 MB (2797541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:638813c8986e4931f6582e649523542695f342c8cb8083284a6c1e1cd7b4b119`  
		Last Modified: Thu, 25 Jun 2020 19:25:59 GMT  
		Size: 6.2 MB (6217173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cba66f363cd2d1a64d4578d0f9f604c52be7e910debc173b3c61aef5549ed716`  
		Last Modified: Thu, 25 Jun 2020 19:25:58 GMT  
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
$ docker pull nats-streaming@sha256:83affddfe9cc74a10f8b960f772b4b6afbdf6ce3a73699ed6c31c0c6c4a7bf22
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.18.0-alpine3.12` - linux; amd64

```console
$ docker pull nats-streaming@sha256:9f71614879c6e9c774410e5315004fc3f6b8f2e52a6e1c6dbe2f203e6c285df0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.0 MB (9015136 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a5b225e159253af34dce2a69079773d857596bf528268a384b2fd1a0b8af6f3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Thu, 25 Jun 2020 19:25:24 GMT
ENV NATS_STREAMING_SERVER=0.18.0
# Thu, 25 Jun 2020 19:25:26 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		arm64) natsArch='arm64'; sha256='ff2a51618b79685264f980fe868f1c7af583c419b6406cc63d4811f3c98ca8fe' ;; 		armhf) natsArch='arm6'; sha256='629e17255f12fd80e051772a6dd18a7f65e692b4abef0786b421eb8b6ab85db4' ;; 		armv7) natsArch='arm7'; sha256='94e499af6a6391519315e8bcd5127c43c1d1a442ef945956286e77b4366c92c9' ;; 		x86_64) natsArch='amd64'; sha256='6252e9262efc81a41ade3f43b68e014d1e635d3e3bf9cbcd2b09c3a030a0d5e6' ;; 		x86) natsArch='386'; sha256='886ebd2e5eb99e30ff9e9d8907d7bd49dafacffce1dc921427e5754a4ec26f55' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 25 Jun 2020 19:25:26 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Thu, 25 Jun 2020 19:25:26 GMT
EXPOSE 4222 8222
# Thu, 25 Jun 2020 19:25:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 25 Jun 2020 19:25:26 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:df20fa9351a15782c64e6dddb2d4a6f50bf6d3688060a34c4014b0d9a752eb4c`  
		Last Modified: Fri, 29 May 2020 21:20:06 GMT  
		Size: 2.8 MB (2797541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:638813c8986e4931f6582e649523542695f342c8cb8083284a6c1e1cd7b4b119`  
		Last Modified: Thu, 25 Jun 2020 19:25:59 GMT  
		Size: 6.2 MB (6217173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cba66f363cd2d1a64d4578d0f9f604c52be7e910debc173b3c61aef5549ed716`  
		Last Modified: Thu, 25 Jun 2020 19:25:58 GMT  
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
$ docker pull nats-streaming@sha256:26aa5bae956b8a0445c9021af0290737bdc950d3da65ec399e49c1352cc3ea84
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1339; amd64

### `nats-streaming:0.18.0-nanoserver` - windows version 10.0.17763.1339; amd64

```console
$ docker pull nats-streaming@sha256:536fc04821f79ce86cbaffab4f58b9bb1b2e697f4f1d17b263e02270d1edba47
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.8 MB (106843336 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:40d8dcc1cfa38989cad5eccdc9993517e290c787fc43f466403bd00c1a7ba261`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 07 Jul 2020 13:50:07 GMT
RUN Apply image 1809-amd64
# Wed, 15 Jul 2020 15:05:14 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 15 Jul 2020 21:09:37 GMT
RUN cmd /S /C #(nop) COPY file:4a858ac4da943f868519572e3fb6817fd379875f2bff0bcb5f03c5bdddc496a8 in C:\nats-streaming-server.exe 
# Wed, 15 Jul 2020 21:09:40 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 15 Jul 2020 21:09:40 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 15 Jul 2020 21:09:41 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:dc95608099543221ef539391bfece5c1ce37b97af9da457f5990349cab028a12`  
		Size: 100.9 MB (100895619 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5f0c27d781c53928c03429d5b34e0f49fc26b7e7c996c1d9a2a8474162eade60`  
		Last Modified: Wed, 15 Jul 2020 15:09:50 GMT  
		Size: 869.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c37823d2bd2a59a1d84d807658bb5995febdf048b1f99233390d2b049939efd1`  
		Last Modified: Wed, 15 Jul 2020 21:14:05 GMT  
		Size: 5.9 MB (5944137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9fe8f765dc0de3583e36e3f3ef18e3a3f3a3f75312e35ac1d42c0d95ce90cc0`  
		Last Modified: Wed, 15 Jul 2020 21:14:04 GMT  
		Size: 906.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:349d8da345d930244c13a48049c9f9001d4a04866a33ee215586352c788b5e88`  
		Last Modified: Wed, 15 Jul 2020 21:14:01 GMT  
		Size: 913.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32f6fe573eab456a9f7b72357c56803fb00bdc82c4919d22ab75252383bf5bd9`  
		Last Modified: Wed, 15 Jul 2020 21:14:01 GMT  
		Size: 892.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.18.0-nanoserver-1809`

```console
$ docker pull nats-streaming@sha256:26aa5bae956b8a0445c9021af0290737bdc950d3da65ec399e49c1352cc3ea84
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1339; amd64

### `nats-streaming:0.18.0-nanoserver-1809` - windows version 10.0.17763.1339; amd64

```console
$ docker pull nats-streaming@sha256:536fc04821f79ce86cbaffab4f58b9bb1b2e697f4f1d17b263e02270d1edba47
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.8 MB (106843336 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:40d8dcc1cfa38989cad5eccdc9993517e290c787fc43f466403bd00c1a7ba261`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 07 Jul 2020 13:50:07 GMT
RUN Apply image 1809-amd64
# Wed, 15 Jul 2020 15:05:14 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 15 Jul 2020 21:09:37 GMT
RUN cmd /S /C #(nop) COPY file:4a858ac4da943f868519572e3fb6817fd379875f2bff0bcb5f03c5bdddc496a8 in C:\nats-streaming-server.exe 
# Wed, 15 Jul 2020 21:09:40 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 15 Jul 2020 21:09:40 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 15 Jul 2020 21:09:41 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:dc95608099543221ef539391bfece5c1ce37b97af9da457f5990349cab028a12`  
		Size: 100.9 MB (100895619 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5f0c27d781c53928c03429d5b34e0f49fc26b7e7c996c1d9a2a8474162eade60`  
		Last Modified: Wed, 15 Jul 2020 15:09:50 GMT  
		Size: 869.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c37823d2bd2a59a1d84d807658bb5995febdf048b1f99233390d2b049939efd1`  
		Last Modified: Wed, 15 Jul 2020 21:14:05 GMT  
		Size: 5.9 MB (5944137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9fe8f765dc0de3583e36e3f3ef18e3a3f3a3f75312e35ac1d42c0d95ce90cc0`  
		Last Modified: Wed, 15 Jul 2020 21:14:04 GMT  
		Size: 906.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:349d8da345d930244c13a48049c9f9001d4a04866a33ee215586352c788b5e88`  
		Last Modified: Wed, 15 Jul 2020 21:14:01 GMT  
		Size: 913.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32f6fe573eab456a9f7b72357c56803fb00bdc82c4919d22ab75252383bf5bd9`  
		Last Modified: Wed, 15 Jul 2020 21:14:01 GMT  
		Size: 892.0 B  
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
$ docker pull nats-streaming@sha256:90f956a0b4d242f64dc27f084e4322ad40f669004f06d6660fde87222b4f25bd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1339; amd64
	-	windows version 10.0.14393.3808; amd64

### `nats-streaming:0.18.0-windowsservercore` - windows version 10.0.17763.1339; amd64

```console
$ docker pull nats-streaming@sha256:fd2b16284f5c09bc81615f52d55aa557e0c4faaf4ffbe623fa9c4a9f855094ca
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2330067351 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7796ffa578afe3152a7069c15ad9993baf8de4b7e748bbf2eb9013ecc443ef9a`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Wed, 08 Jul 2020 04:26:49 GMT
RUN Install update 1809-amd64
# Wed, 15 Jul 2020 12:15:48 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 15 Jul 2020 15:03:03 GMT
ENV NATS_DOCKERIZED=1
# Wed, 15 Jul 2020 21:07:08 GMT
ENV NATS_STREAMING_SERVER=0.18.0
# Wed, 15 Jul 2020 21:07:09 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.18.0/nats-streaming-server-v0.18.0-windows-amd64.zip
# Wed, 15 Jul 2020 21:07:10 GMT
ENV GIT_DOWNLOAD_SHA256=a0c0261df2ce589fe9706617323e06c5bcae70511112eae921681b1169674bc8
# Wed, 15 Jul 2020 21:07:45 GMT
RUN Set-PSDebug -Trace 2
# Wed, 15 Jul 2020 21:09:17 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 15 Jul 2020 21:09:18 GMT
EXPOSE 4222 8222
# Wed, 15 Jul 2020 21:09:20 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 15 Jul 2020 21:09:21 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:fc1b9e59edad2bf789457b52138acc367e86072b73bf862eaf96be70f4d4edbb`  
		Size: 591.9 MB (591859374 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:1cc883a0e3509a474bb32f3c40411bf86219325ae9710e25a5dcce6b44eef357`  
		Last Modified: Wed, 15 Jul 2020 14:32:06 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73dd35c9a62007b6ded1ca968562be97de62ea3e2b3c7db85f4a50baaa9efecb`  
		Last Modified: Wed, 15 Jul 2020 15:09:33 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb6c591c0a8170250552e7e384d3a79de15e68f382a34d1e5752c6c7ab0cbfb5`  
		Last Modified: Wed, 15 Jul 2020 21:13:48 GMT  
		Size: 1.1 KB (1084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a1d80c963f67159f6b9cbf927c2fd4bdf00c6f73353f96b1baf98daaa6c7cb5`  
		Last Modified: Wed, 15 Jul 2020 21:13:48 GMT  
		Size: 1.1 KB (1083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26e611a275568f5c39624077dd6209104cd19177aeced5c0b7e0f00e9e7aaa2b`  
		Last Modified: Wed, 15 Jul 2020 21:13:47 GMT  
		Size: 1.1 KB (1070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c167f6381ec0f43e4cfcc10919a987bf178e694e5b2b4cdff32b39161c9411f`  
		Last Modified: Wed, 15 Jul 2020 21:13:47 GMT  
		Size: 4.8 MB (4800424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffec8d449046498ebfc5d1d69f93ec54cb307a7cd7b2a46003d66c63b69edbcd`  
		Last Modified: Wed, 15 Jul 2020 21:13:49 GMT  
		Size: 15.1 MB (15065705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8b0372f086e7590d8b3b4f0c70dbe11c050d24011d09293dc8e1978e0cd25f0`  
		Last Modified: Wed, 15 Jul 2020 21:13:45 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:189e0c6e97c31e972420da6bed768b9f5fb8a5644521f539e83e4ed9c4b13155`  
		Last Modified: Wed, 15 Jul 2020 21:13:45 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a1d615621d3c5ab9becb58f63dd233e553d272091e768dae0074d3c0bd9d124`  
		Last Modified: Wed, 15 Jul 2020 21:13:46 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.18.0-windowsservercore` - windows version 10.0.14393.3808; amd64

```console
$ docker pull nats-streaming@sha256:daf9e5a9590ebd64d8629288af9923d028c3130df505f7ff6d2badab5fdb36a4
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5758611587 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b14d84aa3c32e47f13a9aa728500047ce78b9247002ddf8006b19e08bc213366`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 07 Jul 2020 21:05:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 15 Jul 2020 12:24:48 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 15 Jul 2020 15:05:26 GMT
ENV NATS_DOCKERIZED=1
# Wed, 15 Jul 2020 21:09:46 GMT
ENV NATS_STREAMING_SERVER=0.18.0
# Wed, 15 Jul 2020 21:09:47 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.18.0/nats-streaming-server-v0.18.0-windows-amd64.zip
# Wed, 15 Jul 2020 21:09:48 GMT
ENV GIT_DOWNLOAD_SHA256=a0c0261df2ce589fe9706617323e06c5bcae70511112eae921681b1169674bc8
# Wed, 15 Jul 2020 21:11:13 GMT
RUN Set-PSDebug -Trace 2
# Wed, 15 Jul 2020 21:13:11 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 15 Jul 2020 21:13:14 GMT
EXPOSE 4222 8222
# Wed, 15 Jul 2020 21:13:15 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 15 Jul 2020 21:13:16 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:802c4beb8b091968ccf1bb4a853ded7955ddb79e6f8775a5155cb5ed07dcbcab`  
		Size: 1.7 GB (1667476199 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3393eecaf56a66035ab178b379bacf81d30373b630b34b2973501f259aadb0f6`  
		Last Modified: Wed, 15 Jul 2020 14:32:38 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1430ee68db5fe3026683f1b7c74f31ae748da71bf8ad611efede726e9e036b1`  
		Last Modified: Wed, 15 Jul 2020 15:10:21 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75bee39dfb46c142a6dd8c7b99236cd36b36ed56346c403d7be4fb8623f9b8d5`  
		Last Modified: Wed, 15 Jul 2020 21:14:20 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b7de9a5c713789f72af564cdc5f28c0dba85d4b95332f815a7d0ba032170616`  
		Last Modified: Wed, 15 Jul 2020 21:14:20 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7ba6847dae4e00016f022ecb49741fecdfb048a3cf945beed074720180415ff`  
		Last Modified: Wed, 15 Jul 2020 21:14:20 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d62e9ba6e0d6f49e9b722408130b963a54818538f1d9f7f3856239f03795f5ab`  
		Last Modified: Wed, 15 Jul 2020 21:14:19 GMT  
		Size: 5.4 MB (5379274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c099f3a69d1984acb328df528418c5d92a1a208d1949990ebaac1b8256e12b9`  
		Last Modified: Wed, 15 Jul 2020 21:14:21 GMT  
		Size: 15.8 MB (15761002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ec2f283e382f964302246e46c7558554d80d222708541d0ad673e912fd538f4`  
		Last Modified: Wed, 15 Jul 2020 21:14:17 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:748659c661458abcab3c6af30d446fd311404a91f63607c45c10b8620a484270`  
		Last Modified: Wed, 15 Jul 2020 21:14:17 GMT  
		Size: 1.1 KB (1136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fed56fa4c13c0af0264cde0de3b1c5c2d040ed6e725662e6b19057481de9dd0f`  
		Last Modified: Wed, 15 Jul 2020 21:14:17 GMT  
		Size: 1.2 KB (1192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.18.0-windowsservercore-1809`

```console
$ docker pull nats-streaming@sha256:323a035ec861fdcbe10d0001a4e9ac0d868297b1b59a6bf7019257715c0f117f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1339; amd64

### `nats-streaming:0.18.0-windowsservercore-1809` - windows version 10.0.17763.1339; amd64

```console
$ docker pull nats-streaming@sha256:fd2b16284f5c09bc81615f52d55aa557e0c4faaf4ffbe623fa9c4a9f855094ca
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2330067351 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7796ffa578afe3152a7069c15ad9993baf8de4b7e748bbf2eb9013ecc443ef9a`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Wed, 08 Jul 2020 04:26:49 GMT
RUN Install update 1809-amd64
# Wed, 15 Jul 2020 12:15:48 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 15 Jul 2020 15:03:03 GMT
ENV NATS_DOCKERIZED=1
# Wed, 15 Jul 2020 21:07:08 GMT
ENV NATS_STREAMING_SERVER=0.18.0
# Wed, 15 Jul 2020 21:07:09 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.18.0/nats-streaming-server-v0.18.0-windows-amd64.zip
# Wed, 15 Jul 2020 21:07:10 GMT
ENV GIT_DOWNLOAD_SHA256=a0c0261df2ce589fe9706617323e06c5bcae70511112eae921681b1169674bc8
# Wed, 15 Jul 2020 21:07:45 GMT
RUN Set-PSDebug -Trace 2
# Wed, 15 Jul 2020 21:09:17 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 15 Jul 2020 21:09:18 GMT
EXPOSE 4222 8222
# Wed, 15 Jul 2020 21:09:20 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 15 Jul 2020 21:09:21 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:fc1b9e59edad2bf789457b52138acc367e86072b73bf862eaf96be70f4d4edbb`  
		Size: 591.9 MB (591859374 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:1cc883a0e3509a474bb32f3c40411bf86219325ae9710e25a5dcce6b44eef357`  
		Last Modified: Wed, 15 Jul 2020 14:32:06 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73dd35c9a62007b6ded1ca968562be97de62ea3e2b3c7db85f4a50baaa9efecb`  
		Last Modified: Wed, 15 Jul 2020 15:09:33 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb6c591c0a8170250552e7e384d3a79de15e68f382a34d1e5752c6c7ab0cbfb5`  
		Last Modified: Wed, 15 Jul 2020 21:13:48 GMT  
		Size: 1.1 KB (1084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a1d80c963f67159f6b9cbf927c2fd4bdf00c6f73353f96b1baf98daaa6c7cb5`  
		Last Modified: Wed, 15 Jul 2020 21:13:48 GMT  
		Size: 1.1 KB (1083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26e611a275568f5c39624077dd6209104cd19177aeced5c0b7e0f00e9e7aaa2b`  
		Last Modified: Wed, 15 Jul 2020 21:13:47 GMT  
		Size: 1.1 KB (1070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c167f6381ec0f43e4cfcc10919a987bf178e694e5b2b4cdff32b39161c9411f`  
		Last Modified: Wed, 15 Jul 2020 21:13:47 GMT  
		Size: 4.8 MB (4800424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffec8d449046498ebfc5d1d69f93ec54cb307a7cd7b2a46003d66c63b69edbcd`  
		Last Modified: Wed, 15 Jul 2020 21:13:49 GMT  
		Size: 15.1 MB (15065705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8b0372f086e7590d8b3b4f0c70dbe11c050d24011d09293dc8e1978e0cd25f0`  
		Last Modified: Wed, 15 Jul 2020 21:13:45 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:189e0c6e97c31e972420da6bed768b9f5fb8a5644521f539e83e4ed9c4b13155`  
		Last Modified: Wed, 15 Jul 2020 21:13:45 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a1d615621d3c5ab9becb58f63dd233e553d272091e768dae0074d3c0bd9d124`  
		Last Modified: Wed, 15 Jul 2020 21:13:46 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.18.0-windowsservercore-ltsc2016`

```console
$ docker pull nats-streaming@sha256:9c89c6a37c2686bd1a2ab08e5ddf4a16103a3e37b7649535bc37b16444c5bcca
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3808; amd64

### `nats-streaming:0.18.0-windowsservercore-ltsc2016` - windows version 10.0.14393.3808; amd64

```console
$ docker pull nats-streaming@sha256:daf9e5a9590ebd64d8629288af9923d028c3130df505f7ff6d2badab5fdb36a4
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5758611587 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b14d84aa3c32e47f13a9aa728500047ce78b9247002ddf8006b19e08bc213366`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 07 Jul 2020 21:05:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 15 Jul 2020 12:24:48 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 15 Jul 2020 15:05:26 GMT
ENV NATS_DOCKERIZED=1
# Wed, 15 Jul 2020 21:09:46 GMT
ENV NATS_STREAMING_SERVER=0.18.0
# Wed, 15 Jul 2020 21:09:47 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.18.0/nats-streaming-server-v0.18.0-windows-amd64.zip
# Wed, 15 Jul 2020 21:09:48 GMT
ENV GIT_DOWNLOAD_SHA256=a0c0261df2ce589fe9706617323e06c5bcae70511112eae921681b1169674bc8
# Wed, 15 Jul 2020 21:11:13 GMT
RUN Set-PSDebug -Trace 2
# Wed, 15 Jul 2020 21:13:11 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 15 Jul 2020 21:13:14 GMT
EXPOSE 4222 8222
# Wed, 15 Jul 2020 21:13:15 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 15 Jul 2020 21:13:16 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:802c4beb8b091968ccf1bb4a853ded7955ddb79e6f8775a5155cb5ed07dcbcab`  
		Size: 1.7 GB (1667476199 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3393eecaf56a66035ab178b379bacf81d30373b630b34b2973501f259aadb0f6`  
		Last Modified: Wed, 15 Jul 2020 14:32:38 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1430ee68db5fe3026683f1b7c74f31ae748da71bf8ad611efede726e9e036b1`  
		Last Modified: Wed, 15 Jul 2020 15:10:21 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75bee39dfb46c142a6dd8c7b99236cd36b36ed56346c403d7be4fb8623f9b8d5`  
		Last Modified: Wed, 15 Jul 2020 21:14:20 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b7de9a5c713789f72af564cdc5f28c0dba85d4b95332f815a7d0ba032170616`  
		Last Modified: Wed, 15 Jul 2020 21:14:20 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7ba6847dae4e00016f022ecb49741fecdfb048a3cf945beed074720180415ff`  
		Last Modified: Wed, 15 Jul 2020 21:14:20 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d62e9ba6e0d6f49e9b722408130b963a54818538f1d9f7f3856239f03795f5ab`  
		Last Modified: Wed, 15 Jul 2020 21:14:19 GMT  
		Size: 5.4 MB (5379274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c099f3a69d1984acb328df528418c5d92a1a208d1949990ebaac1b8256e12b9`  
		Last Modified: Wed, 15 Jul 2020 21:14:21 GMT  
		Size: 15.8 MB (15761002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ec2f283e382f964302246e46c7558554d80d222708541d0ad673e912fd538f4`  
		Last Modified: Wed, 15 Jul 2020 21:14:17 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:748659c661458abcab3c6af30d446fd311404a91f63607c45c10b8620a484270`  
		Last Modified: Wed, 15 Jul 2020 21:14:17 GMT  
		Size: 1.1 KB (1136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fed56fa4c13c0af0264cde0de3b1c5c2d040ed6e725662e6b19057481de9dd0f`  
		Last Modified: Wed, 15 Jul 2020 21:14:17 GMT  
		Size: 1.2 KB (1192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.18-alpine`

```console
$ docker pull nats-streaming@sha256:83affddfe9cc74a10f8b960f772b4b6afbdf6ce3a73699ed6c31c0c6c4a7bf22
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.18-alpine` - linux; amd64

```console
$ docker pull nats-streaming@sha256:9f71614879c6e9c774410e5315004fc3f6b8f2e52a6e1c6dbe2f203e6c285df0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.0 MB (9015136 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a5b225e159253af34dce2a69079773d857596bf528268a384b2fd1a0b8af6f3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Thu, 25 Jun 2020 19:25:24 GMT
ENV NATS_STREAMING_SERVER=0.18.0
# Thu, 25 Jun 2020 19:25:26 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		arm64) natsArch='arm64'; sha256='ff2a51618b79685264f980fe868f1c7af583c419b6406cc63d4811f3c98ca8fe' ;; 		armhf) natsArch='arm6'; sha256='629e17255f12fd80e051772a6dd18a7f65e692b4abef0786b421eb8b6ab85db4' ;; 		armv7) natsArch='arm7'; sha256='94e499af6a6391519315e8bcd5127c43c1d1a442ef945956286e77b4366c92c9' ;; 		x86_64) natsArch='amd64'; sha256='6252e9262efc81a41ade3f43b68e014d1e635d3e3bf9cbcd2b09c3a030a0d5e6' ;; 		x86) natsArch='386'; sha256='886ebd2e5eb99e30ff9e9d8907d7bd49dafacffce1dc921427e5754a4ec26f55' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 25 Jun 2020 19:25:26 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Thu, 25 Jun 2020 19:25:26 GMT
EXPOSE 4222 8222
# Thu, 25 Jun 2020 19:25:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 25 Jun 2020 19:25:26 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:df20fa9351a15782c64e6dddb2d4a6f50bf6d3688060a34c4014b0d9a752eb4c`  
		Last Modified: Fri, 29 May 2020 21:20:06 GMT  
		Size: 2.8 MB (2797541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:638813c8986e4931f6582e649523542695f342c8cb8083284a6c1e1cd7b4b119`  
		Last Modified: Thu, 25 Jun 2020 19:25:59 GMT  
		Size: 6.2 MB (6217173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cba66f363cd2d1a64d4578d0f9f604c52be7e910debc173b3c61aef5549ed716`  
		Last Modified: Thu, 25 Jun 2020 19:25:58 GMT  
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
$ docker pull nats-streaming@sha256:83affddfe9cc74a10f8b960f772b4b6afbdf6ce3a73699ed6c31c0c6c4a7bf22
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.18-alpine3.12` - linux; amd64

```console
$ docker pull nats-streaming@sha256:9f71614879c6e9c774410e5315004fc3f6b8f2e52a6e1c6dbe2f203e6c285df0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.0 MB (9015136 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a5b225e159253af34dce2a69079773d857596bf528268a384b2fd1a0b8af6f3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Thu, 25 Jun 2020 19:25:24 GMT
ENV NATS_STREAMING_SERVER=0.18.0
# Thu, 25 Jun 2020 19:25:26 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		arm64) natsArch='arm64'; sha256='ff2a51618b79685264f980fe868f1c7af583c419b6406cc63d4811f3c98ca8fe' ;; 		armhf) natsArch='arm6'; sha256='629e17255f12fd80e051772a6dd18a7f65e692b4abef0786b421eb8b6ab85db4' ;; 		armv7) natsArch='arm7'; sha256='94e499af6a6391519315e8bcd5127c43c1d1a442ef945956286e77b4366c92c9' ;; 		x86_64) natsArch='amd64'; sha256='6252e9262efc81a41ade3f43b68e014d1e635d3e3bf9cbcd2b09c3a030a0d5e6' ;; 		x86) natsArch='386'; sha256='886ebd2e5eb99e30ff9e9d8907d7bd49dafacffce1dc921427e5754a4ec26f55' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 25 Jun 2020 19:25:26 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Thu, 25 Jun 2020 19:25:26 GMT
EXPOSE 4222 8222
# Thu, 25 Jun 2020 19:25:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 25 Jun 2020 19:25:26 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:df20fa9351a15782c64e6dddb2d4a6f50bf6d3688060a34c4014b0d9a752eb4c`  
		Last Modified: Fri, 29 May 2020 21:20:06 GMT  
		Size: 2.8 MB (2797541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:638813c8986e4931f6582e649523542695f342c8cb8083284a6c1e1cd7b4b119`  
		Last Modified: Thu, 25 Jun 2020 19:25:59 GMT  
		Size: 6.2 MB (6217173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cba66f363cd2d1a64d4578d0f9f604c52be7e910debc173b3c61aef5549ed716`  
		Last Modified: Thu, 25 Jun 2020 19:25:58 GMT  
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
$ docker pull nats-streaming@sha256:26aa5bae956b8a0445c9021af0290737bdc950d3da65ec399e49c1352cc3ea84
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1339; amd64

### `nats-streaming:0.18-nanoserver` - windows version 10.0.17763.1339; amd64

```console
$ docker pull nats-streaming@sha256:536fc04821f79ce86cbaffab4f58b9bb1b2e697f4f1d17b263e02270d1edba47
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.8 MB (106843336 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:40d8dcc1cfa38989cad5eccdc9993517e290c787fc43f466403bd00c1a7ba261`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 07 Jul 2020 13:50:07 GMT
RUN Apply image 1809-amd64
# Wed, 15 Jul 2020 15:05:14 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 15 Jul 2020 21:09:37 GMT
RUN cmd /S /C #(nop) COPY file:4a858ac4da943f868519572e3fb6817fd379875f2bff0bcb5f03c5bdddc496a8 in C:\nats-streaming-server.exe 
# Wed, 15 Jul 2020 21:09:40 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 15 Jul 2020 21:09:40 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 15 Jul 2020 21:09:41 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:dc95608099543221ef539391bfece5c1ce37b97af9da457f5990349cab028a12`  
		Size: 100.9 MB (100895619 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5f0c27d781c53928c03429d5b34e0f49fc26b7e7c996c1d9a2a8474162eade60`  
		Last Modified: Wed, 15 Jul 2020 15:09:50 GMT  
		Size: 869.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c37823d2bd2a59a1d84d807658bb5995febdf048b1f99233390d2b049939efd1`  
		Last Modified: Wed, 15 Jul 2020 21:14:05 GMT  
		Size: 5.9 MB (5944137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9fe8f765dc0de3583e36e3f3ef18e3a3f3a3f75312e35ac1d42c0d95ce90cc0`  
		Last Modified: Wed, 15 Jul 2020 21:14:04 GMT  
		Size: 906.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:349d8da345d930244c13a48049c9f9001d4a04866a33ee215586352c788b5e88`  
		Last Modified: Wed, 15 Jul 2020 21:14:01 GMT  
		Size: 913.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32f6fe573eab456a9f7b72357c56803fb00bdc82c4919d22ab75252383bf5bd9`  
		Last Modified: Wed, 15 Jul 2020 21:14:01 GMT  
		Size: 892.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.18-nanoserver-1809`

```console
$ docker pull nats-streaming@sha256:26aa5bae956b8a0445c9021af0290737bdc950d3da65ec399e49c1352cc3ea84
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1339; amd64

### `nats-streaming:0.18-nanoserver-1809` - windows version 10.0.17763.1339; amd64

```console
$ docker pull nats-streaming@sha256:536fc04821f79ce86cbaffab4f58b9bb1b2e697f4f1d17b263e02270d1edba47
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.8 MB (106843336 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:40d8dcc1cfa38989cad5eccdc9993517e290c787fc43f466403bd00c1a7ba261`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 07 Jul 2020 13:50:07 GMT
RUN Apply image 1809-amd64
# Wed, 15 Jul 2020 15:05:14 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 15 Jul 2020 21:09:37 GMT
RUN cmd /S /C #(nop) COPY file:4a858ac4da943f868519572e3fb6817fd379875f2bff0bcb5f03c5bdddc496a8 in C:\nats-streaming-server.exe 
# Wed, 15 Jul 2020 21:09:40 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 15 Jul 2020 21:09:40 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 15 Jul 2020 21:09:41 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:dc95608099543221ef539391bfece5c1ce37b97af9da457f5990349cab028a12`  
		Size: 100.9 MB (100895619 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5f0c27d781c53928c03429d5b34e0f49fc26b7e7c996c1d9a2a8474162eade60`  
		Last Modified: Wed, 15 Jul 2020 15:09:50 GMT  
		Size: 869.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c37823d2bd2a59a1d84d807658bb5995febdf048b1f99233390d2b049939efd1`  
		Last Modified: Wed, 15 Jul 2020 21:14:05 GMT  
		Size: 5.9 MB (5944137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9fe8f765dc0de3583e36e3f3ef18e3a3f3a3f75312e35ac1d42c0d95ce90cc0`  
		Last Modified: Wed, 15 Jul 2020 21:14:04 GMT  
		Size: 906.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:349d8da345d930244c13a48049c9f9001d4a04866a33ee215586352c788b5e88`  
		Last Modified: Wed, 15 Jul 2020 21:14:01 GMT  
		Size: 913.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32f6fe573eab456a9f7b72357c56803fb00bdc82c4919d22ab75252383bf5bd9`  
		Last Modified: Wed, 15 Jul 2020 21:14:01 GMT  
		Size: 892.0 B  
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
$ docker pull nats-streaming@sha256:90f956a0b4d242f64dc27f084e4322ad40f669004f06d6660fde87222b4f25bd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1339; amd64
	-	windows version 10.0.14393.3808; amd64

### `nats-streaming:0.18-windowsservercore` - windows version 10.0.17763.1339; amd64

```console
$ docker pull nats-streaming@sha256:fd2b16284f5c09bc81615f52d55aa557e0c4faaf4ffbe623fa9c4a9f855094ca
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2330067351 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7796ffa578afe3152a7069c15ad9993baf8de4b7e748bbf2eb9013ecc443ef9a`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Wed, 08 Jul 2020 04:26:49 GMT
RUN Install update 1809-amd64
# Wed, 15 Jul 2020 12:15:48 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 15 Jul 2020 15:03:03 GMT
ENV NATS_DOCKERIZED=1
# Wed, 15 Jul 2020 21:07:08 GMT
ENV NATS_STREAMING_SERVER=0.18.0
# Wed, 15 Jul 2020 21:07:09 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.18.0/nats-streaming-server-v0.18.0-windows-amd64.zip
# Wed, 15 Jul 2020 21:07:10 GMT
ENV GIT_DOWNLOAD_SHA256=a0c0261df2ce589fe9706617323e06c5bcae70511112eae921681b1169674bc8
# Wed, 15 Jul 2020 21:07:45 GMT
RUN Set-PSDebug -Trace 2
# Wed, 15 Jul 2020 21:09:17 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 15 Jul 2020 21:09:18 GMT
EXPOSE 4222 8222
# Wed, 15 Jul 2020 21:09:20 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 15 Jul 2020 21:09:21 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:fc1b9e59edad2bf789457b52138acc367e86072b73bf862eaf96be70f4d4edbb`  
		Size: 591.9 MB (591859374 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:1cc883a0e3509a474bb32f3c40411bf86219325ae9710e25a5dcce6b44eef357`  
		Last Modified: Wed, 15 Jul 2020 14:32:06 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73dd35c9a62007b6ded1ca968562be97de62ea3e2b3c7db85f4a50baaa9efecb`  
		Last Modified: Wed, 15 Jul 2020 15:09:33 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb6c591c0a8170250552e7e384d3a79de15e68f382a34d1e5752c6c7ab0cbfb5`  
		Last Modified: Wed, 15 Jul 2020 21:13:48 GMT  
		Size: 1.1 KB (1084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a1d80c963f67159f6b9cbf927c2fd4bdf00c6f73353f96b1baf98daaa6c7cb5`  
		Last Modified: Wed, 15 Jul 2020 21:13:48 GMT  
		Size: 1.1 KB (1083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26e611a275568f5c39624077dd6209104cd19177aeced5c0b7e0f00e9e7aaa2b`  
		Last Modified: Wed, 15 Jul 2020 21:13:47 GMT  
		Size: 1.1 KB (1070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c167f6381ec0f43e4cfcc10919a987bf178e694e5b2b4cdff32b39161c9411f`  
		Last Modified: Wed, 15 Jul 2020 21:13:47 GMT  
		Size: 4.8 MB (4800424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffec8d449046498ebfc5d1d69f93ec54cb307a7cd7b2a46003d66c63b69edbcd`  
		Last Modified: Wed, 15 Jul 2020 21:13:49 GMT  
		Size: 15.1 MB (15065705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8b0372f086e7590d8b3b4f0c70dbe11c050d24011d09293dc8e1978e0cd25f0`  
		Last Modified: Wed, 15 Jul 2020 21:13:45 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:189e0c6e97c31e972420da6bed768b9f5fb8a5644521f539e83e4ed9c4b13155`  
		Last Modified: Wed, 15 Jul 2020 21:13:45 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a1d615621d3c5ab9becb58f63dd233e553d272091e768dae0074d3c0bd9d124`  
		Last Modified: Wed, 15 Jul 2020 21:13:46 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.18-windowsservercore` - windows version 10.0.14393.3808; amd64

```console
$ docker pull nats-streaming@sha256:daf9e5a9590ebd64d8629288af9923d028c3130df505f7ff6d2badab5fdb36a4
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5758611587 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b14d84aa3c32e47f13a9aa728500047ce78b9247002ddf8006b19e08bc213366`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 07 Jul 2020 21:05:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 15 Jul 2020 12:24:48 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 15 Jul 2020 15:05:26 GMT
ENV NATS_DOCKERIZED=1
# Wed, 15 Jul 2020 21:09:46 GMT
ENV NATS_STREAMING_SERVER=0.18.0
# Wed, 15 Jul 2020 21:09:47 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.18.0/nats-streaming-server-v0.18.0-windows-amd64.zip
# Wed, 15 Jul 2020 21:09:48 GMT
ENV GIT_DOWNLOAD_SHA256=a0c0261df2ce589fe9706617323e06c5bcae70511112eae921681b1169674bc8
# Wed, 15 Jul 2020 21:11:13 GMT
RUN Set-PSDebug -Trace 2
# Wed, 15 Jul 2020 21:13:11 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 15 Jul 2020 21:13:14 GMT
EXPOSE 4222 8222
# Wed, 15 Jul 2020 21:13:15 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 15 Jul 2020 21:13:16 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:802c4beb8b091968ccf1bb4a853ded7955ddb79e6f8775a5155cb5ed07dcbcab`  
		Size: 1.7 GB (1667476199 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3393eecaf56a66035ab178b379bacf81d30373b630b34b2973501f259aadb0f6`  
		Last Modified: Wed, 15 Jul 2020 14:32:38 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1430ee68db5fe3026683f1b7c74f31ae748da71bf8ad611efede726e9e036b1`  
		Last Modified: Wed, 15 Jul 2020 15:10:21 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75bee39dfb46c142a6dd8c7b99236cd36b36ed56346c403d7be4fb8623f9b8d5`  
		Last Modified: Wed, 15 Jul 2020 21:14:20 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b7de9a5c713789f72af564cdc5f28c0dba85d4b95332f815a7d0ba032170616`  
		Last Modified: Wed, 15 Jul 2020 21:14:20 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7ba6847dae4e00016f022ecb49741fecdfb048a3cf945beed074720180415ff`  
		Last Modified: Wed, 15 Jul 2020 21:14:20 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d62e9ba6e0d6f49e9b722408130b963a54818538f1d9f7f3856239f03795f5ab`  
		Last Modified: Wed, 15 Jul 2020 21:14:19 GMT  
		Size: 5.4 MB (5379274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c099f3a69d1984acb328df528418c5d92a1a208d1949990ebaac1b8256e12b9`  
		Last Modified: Wed, 15 Jul 2020 21:14:21 GMT  
		Size: 15.8 MB (15761002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ec2f283e382f964302246e46c7558554d80d222708541d0ad673e912fd538f4`  
		Last Modified: Wed, 15 Jul 2020 21:14:17 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:748659c661458abcab3c6af30d446fd311404a91f63607c45c10b8620a484270`  
		Last Modified: Wed, 15 Jul 2020 21:14:17 GMT  
		Size: 1.1 KB (1136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fed56fa4c13c0af0264cde0de3b1c5c2d040ed6e725662e6b19057481de9dd0f`  
		Last Modified: Wed, 15 Jul 2020 21:14:17 GMT  
		Size: 1.2 KB (1192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.18-windowsservercore-1809`

```console
$ docker pull nats-streaming@sha256:323a035ec861fdcbe10d0001a4e9ac0d868297b1b59a6bf7019257715c0f117f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1339; amd64

### `nats-streaming:0.18-windowsservercore-1809` - windows version 10.0.17763.1339; amd64

```console
$ docker pull nats-streaming@sha256:fd2b16284f5c09bc81615f52d55aa557e0c4faaf4ffbe623fa9c4a9f855094ca
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2330067351 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7796ffa578afe3152a7069c15ad9993baf8de4b7e748bbf2eb9013ecc443ef9a`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Wed, 08 Jul 2020 04:26:49 GMT
RUN Install update 1809-amd64
# Wed, 15 Jul 2020 12:15:48 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 15 Jul 2020 15:03:03 GMT
ENV NATS_DOCKERIZED=1
# Wed, 15 Jul 2020 21:07:08 GMT
ENV NATS_STREAMING_SERVER=0.18.0
# Wed, 15 Jul 2020 21:07:09 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.18.0/nats-streaming-server-v0.18.0-windows-amd64.zip
# Wed, 15 Jul 2020 21:07:10 GMT
ENV GIT_DOWNLOAD_SHA256=a0c0261df2ce589fe9706617323e06c5bcae70511112eae921681b1169674bc8
# Wed, 15 Jul 2020 21:07:45 GMT
RUN Set-PSDebug -Trace 2
# Wed, 15 Jul 2020 21:09:17 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 15 Jul 2020 21:09:18 GMT
EXPOSE 4222 8222
# Wed, 15 Jul 2020 21:09:20 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 15 Jul 2020 21:09:21 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:fc1b9e59edad2bf789457b52138acc367e86072b73bf862eaf96be70f4d4edbb`  
		Size: 591.9 MB (591859374 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:1cc883a0e3509a474bb32f3c40411bf86219325ae9710e25a5dcce6b44eef357`  
		Last Modified: Wed, 15 Jul 2020 14:32:06 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73dd35c9a62007b6ded1ca968562be97de62ea3e2b3c7db85f4a50baaa9efecb`  
		Last Modified: Wed, 15 Jul 2020 15:09:33 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb6c591c0a8170250552e7e384d3a79de15e68f382a34d1e5752c6c7ab0cbfb5`  
		Last Modified: Wed, 15 Jul 2020 21:13:48 GMT  
		Size: 1.1 KB (1084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a1d80c963f67159f6b9cbf927c2fd4bdf00c6f73353f96b1baf98daaa6c7cb5`  
		Last Modified: Wed, 15 Jul 2020 21:13:48 GMT  
		Size: 1.1 KB (1083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26e611a275568f5c39624077dd6209104cd19177aeced5c0b7e0f00e9e7aaa2b`  
		Last Modified: Wed, 15 Jul 2020 21:13:47 GMT  
		Size: 1.1 KB (1070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c167f6381ec0f43e4cfcc10919a987bf178e694e5b2b4cdff32b39161c9411f`  
		Last Modified: Wed, 15 Jul 2020 21:13:47 GMT  
		Size: 4.8 MB (4800424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffec8d449046498ebfc5d1d69f93ec54cb307a7cd7b2a46003d66c63b69edbcd`  
		Last Modified: Wed, 15 Jul 2020 21:13:49 GMT  
		Size: 15.1 MB (15065705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8b0372f086e7590d8b3b4f0c70dbe11c050d24011d09293dc8e1978e0cd25f0`  
		Last Modified: Wed, 15 Jul 2020 21:13:45 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:189e0c6e97c31e972420da6bed768b9f5fb8a5644521f539e83e4ed9c4b13155`  
		Last Modified: Wed, 15 Jul 2020 21:13:45 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a1d615621d3c5ab9becb58f63dd233e553d272091e768dae0074d3c0bd9d124`  
		Last Modified: Wed, 15 Jul 2020 21:13:46 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.18-windowsservercore-ltsc2016`

```console
$ docker pull nats-streaming@sha256:9c89c6a37c2686bd1a2ab08e5ddf4a16103a3e37b7649535bc37b16444c5bcca
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3808; amd64

### `nats-streaming:0.18-windowsservercore-ltsc2016` - windows version 10.0.14393.3808; amd64

```console
$ docker pull nats-streaming@sha256:daf9e5a9590ebd64d8629288af9923d028c3130df505f7ff6d2badab5fdb36a4
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5758611587 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b14d84aa3c32e47f13a9aa728500047ce78b9247002ddf8006b19e08bc213366`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 07 Jul 2020 21:05:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 15 Jul 2020 12:24:48 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 15 Jul 2020 15:05:26 GMT
ENV NATS_DOCKERIZED=1
# Wed, 15 Jul 2020 21:09:46 GMT
ENV NATS_STREAMING_SERVER=0.18.0
# Wed, 15 Jul 2020 21:09:47 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.18.0/nats-streaming-server-v0.18.0-windows-amd64.zip
# Wed, 15 Jul 2020 21:09:48 GMT
ENV GIT_DOWNLOAD_SHA256=a0c0261df2ce589fe9706617323e06c5bcae70511112eae921681b1169674bc8
# Wed, 15 Jul 2020 21:11:13 GMT
RUN Set-PSDebug -Trace 2
# Wed, 15 Jul 2020 21:13:11 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 15 Jul 2020 21:13:14 GMT
EXPOSE 4222 8222
# Wed, 15 Jul 2020 21:13:15 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 15 Jul 2020 21:13:16 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:802c4beb8b091968ccf1bb4a853ded7955ddb79e6f8775a5155cb5ed07dcbcab`  
		Size: 1.7 GB (1667476199 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3393eecaf56a66035ab178b379bacf81d30373b630b34b2973501f259aadb0f6`  
		Last Modified: Wed, 15 Jul 2020 14:32:38 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1430ee68db5fe3026683f1b7c74f31ae748da71bf8ad611efede726e9e036b1`  
		Last Modified: Wed, 15 Jul 2020 15:10:21 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75bee39dfb46c142a6dd8c7b99236cd36b36ed56346c403d7be4fb8623f9b8d5`  
		Last Modified: Wed, 15 Jul 2020 21:14:20 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b7de9a5c713789f72af564cdc5f28c0dba85d4b95332f815a7d0ba032170616`  
		Last Modified: Wed, 15 Jul 2020 21:14:20 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7ba6847dae4e00016f022ecb49741fecdfb048a3cf945beed074720180415ff`  
		Last Modified: Wed, 15 Jul 2020 21:14:20 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d62e9ba6e0d6f49e9b722408130b963a54818538f1d9f7f3856239f03795f5ab`  
		Last Modified: Wed, 15 Jul 2020 21:14:19 GMT  
		Size: 5.4 MB (5379274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c099f3a69d1984acb328df528418c5d92a1a208d1949990ebaac1b8256e12b9`  
		Last Modified: Wed, 15 Jul 2020 21:14:21 GMT  
		Size: 15.8 MB (15761002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ec2f283e382f964302246e46c7558554d80d222708541d0ad673e912fd538f4`  
		Last Modified: Wed, 15 Jul 2020 21:14:17 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:748659c661458abcab3c6af30d446fd311404a91f63607c45c10b8620a484270`  
		Last Modified: Wed, 15 Jul 2020 21:14:17 GMT  
		Size: 1.1 KB (1136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fed56fa4c13c0af0264cde0de3b1c5c2d040ed6e725662e6b19057481de9dd0f`  
		Last Modified: Wed, 15 Jul 2020 21:14:17 GMT  
		Size: 1.2 KB (1192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:alpine`

```console
$ docker pull nats-streaming@sha256:83affddfe9cc74a10f8b960f772b4b6afbdf6ce3a73699ed6c31c0c6c4a7bf22
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:alpine` - linux; amd64

```console
$ docker pull nats-streaming@sha256:9f71614879c6e9c774410e5315004fc3f6b8f2e52a6e1c6dbe2f203e6c285df0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.0 MB (9015136 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a5b225e159253af34dce2a69079773d857596bf528268a384b2fd1a0b8af6f3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Thu, 25 Jun 2020 19:25:24 GMT
ENV NATS_STREAMING_SERVER=0.18.0
# Thu, 25 Jun 2020 19:25:26 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		arm64) natsArch='arm64'; sha256='ff2a51618b79685264f980fe868f1c7af583c419b6406cc63d4811f3c98ca8fe' ;; 		armhf) natsArch='arm6'; sha256='629e17255f12fd80e051772a6dd18a7f65e692b4abef0786b421eb8b6ab85db4' ;; 		armv7) natsArch='arm7'; sha256='94e499af6a6391519315e8bcd5127c43c1d1a442ef945956286e77b4366c92c9' ;; 		x86_64) natsArch='amd64'; sha256='6252e9262efc81a41ade3f43b68e014d1e635d3e3bf9cbcd2b09c3a030a0d5e6' ;; 		x86) natsArch='386'; sha256='886ebd2e5eb99e30ff9e9d8907d7bd49dafacffce1dc921427e5754a4ec26f55' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 25 Jun 2020 19:25:26 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Thu, 25 Jun 2020 19:25:26 GMT
EXPOSE 4222 8222
# Thu, 25 Jun 2020 19:25:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 25 Jun 2020 19:25:26 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:df20fa9351a15782c64e6dddb2d4a6f50bf6d3688060a34c4014b0d9a752eb4c`  
		Last Modified: Fri, 29 May 2020 21:20:06 GMT  
		Size: 2.8 MB (2797541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:638813c8986e4931f6582e649523542695f342c8cb8083284a6c1e1cd7b4b119`  
		Last Modified: Thu, 25 Jun 2020 19:25:59 GMT  
		Size: 6.2 MB (6217173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cba66f363cd2d1a64d4578d0f9f604c52be7e910debc173b3c61aef5549ed716`  
		Last Modified: Thu, 25 Jun 2020 19:25:58 GMT  
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
$ docker pull nats-streaming@sha256:83affddfe9cc74a10f8b960f772b4b6afbdf6ce3a73699ed6c31c0c6c4a7bf22
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:alpine3.12` - linux; amd64

```console
$ docker pull nats-streaming@sha256:9f71614879c6e9c774410e5315004fc3f6b8f2e52a6e1c6dbe2f203e6c285df0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.0 MB (9015136 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a5b225e159253af34dce2a69079773d857596bf528268a384b2fd1a0b8af6f3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Thu, 25 Jun 2020 19:25:24 GMT
ENV NATS_STREAMING_SERVER=0.18.0
# Thu, 25 Jun 2020 19:25:26 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		arm64) natsArch='arm64'; sha256='ff2a51618b79685264f980fe868f1c7af583c419b6406cc63d4811f3c98ca8fe' ;; 		armhf) natsArch='arm6'; sha256='629e17255f12fd80e051772a6dd18a7f65e692b4abef0786b421eb8b6ab85db4' ;; 		armv7) natsArch='arm7'; sha256='94e499af6a6391519315e8bcd5127c43c1d1a442ef945956286e77b4366c92c9' ;; 		x86_64) natsArch='amd64'; sha256='6252e9262efc81a41ade3f43b68e014d1e635d3e3bf9cbcd2b09c3a030a0d5e6' ;; 		x86) natsArch='386'; sha256='886ebd2e5eb99e30ff9e9d8907d7bd49dafacffce1dc921427e5754a4ec26f55' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 25 Jun 2020 19:25:26 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Thu, 25 Jun 2020 19:25:26 GMT
EXPOSE 4222 8222
# Thu, 25 Jun 2020 19:25:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 25 Jun 2020 19:25:26 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:df20fa9351a15782c64e6dddb2d4a6f50bf6d3688060a34c4014b0d9a752eb4c`  
		Last Modified: Fri, 29 May 2020 21:20:06 GMT  
		Size: 2.8 MB (2797541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:638813c8986e4931f6582e649523542695f342c8cb8083284a6c1e1cd7b4b119`  
		Last Modified: Thu, 25 Jun 2020 19:25:59 GMT  
		Size: 6.2 MB (6217173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cba66f363cd2d1a64d4578d0f9f604c52be7e910debc173b3c61aef5549ed716`  
		Last Modified: Thu, 25 Jun 2020 19:25:58 GMT  
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
$ docker pull nats-streaming@sha256:46f30dff859ef0690c053a1a9514adbc3bcba3210b9565c940813498ac3db83d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.1339; amd64

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

### `nats-streaming:latest` - windows version 10.0.17763.1339; amd64

```console
$ docker pull nats-streaming@sha256:536fc04821f79ce86cbaffab4f58b9bb1b2e697f4f1d17b263e02270d1edba47
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.8 MB (106843336 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:40d8dcc1cfa38989cad5eccdc9993517e290c787fc43f466403bd00c1a7ba261`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 07 Jul 2020 13:50:07 GMT
RUN Apply image 1809-amd64
# Wed, 15 Jul 2020 15:05:14 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 15 Jul 2020 21:09:37 GMT
RUN cmd /S /C #(nop) COPY file:4a858ac4da943f868519572e3fb6817fd379875f2bff0bcb5f03c5bdddc496a8 in C:\nats-streaming-server.exe 
# Wed, 15 Jul 2020 21:09:40 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 15 Jul 2020 21:09:40 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 15 Jul 2020 21:09:41 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:dc95608099543221ef539391bfece5c1ce37b97af9da457f5990349cab028a12`  
		Size: 100.9 MB (100895619 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5f0c27d781c53928c03429d5b34e0f49fc26b7e7c996c1d9a2a8474162eade60`  
		Last Modified: Wed, 15 Jul 2020 15:09:50 GMT  
		Size: 869.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c37823d2bd2a59a1d84d807658bb5995febdf048b1f99233390d2b049939efd1`  
		Last Modified: Wed, 15 Jul 2020 21:14:05 GMT  
		Size: 5.9 MB (5944137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9fe8f765dc0de3583e36e3f3ef18e3a3f3a3f75312e35ac1d42c0d95ce90cc0`  
		Last Modified: Wed, 15 Jul 2020 21:14:04 GMT  
		Size: 906.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:349d8da345d930244c13a48049c9f9001d4a04866a33ee215586352c788b5e88`  
		Last Modified: Wed, 15 Jul 2020 21:14:01 GMT  
		Size: 913.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32f6fe573eab456a9f7b72357c56803fb00bdc82c4919d22ab75252383bf5bd9`  
		Last Modified: Wed, 15 Jul 2020 21:14:01 GMT  
		Size: 892.0 B  
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
$ docker pull nats-streaming@sha256:26aa5bae956b8a0445c9021af0290737bdc950d3da65ec399e49c1352cc3ea84
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1339; amd64

### `nats-streaming:nanoserver` - windows version 10.0.17763.1339; amd64

```console
$ docker pull nats-streaming@sha256:536fc04821f79ce86cbaffab4f58b9bb1b2e697f4f1d17b263e02270d1edba47
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.8 MB (106843336 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:40d8dcc1cfa38989cad5eccdc9993517e290c787fc43f466403bd00c1a7ba261`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 07 Jul 2020 13:50:07 GMT
RUN Apply image 1809-amd64
# Wed, 15 Jul 2020 15:05:14 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 15 Jul 2020 21:09:37 GMT
RUN cmd /S /C #(nop) COPY file:4a858ac4da943f868519572e3fb6817fd379875f2bff0bcb5f03c5bdddc496a8 in C:\nats-streaming-server.exe 
# Wed, 15 Jul 2020 21:09:40 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 15 Jul 2020 21:09:40 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 15 Jul 2020 21:09:41 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:dc95608099543221ef539391bfece5c1ce37b97af9da457f5990349cab028a12`  
		Size: 100.9 MB (100895619 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5f0c27d781c53928c03429d5b34e0f49fc26b7e7c996c1d9a2a8474162eade60`  
		Last Modified: Wed, 15 Jul 2020 15:09:50 GMT  
		Size: 869.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c37823d2bd2a59a1d84d807658bb5995febdf048b1f99233390d2b049939efd1`  
		Last Modified: Wed, 15 Jul 2020 21:14:05 GMT  
		Size: 5.9 MB (5944137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9fe8f765dc0de3583e36e3f3ef18e3a3f3a3f75312e35ac1d42c0d95ce90cc0`  
		Last Modified: Wed, 15 Jul 2020 21:14:04 GMT  
		Size: 906.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:349d8da345d930244c13a48049c9f9001d4a04866a33ee215586352c788b5e88`  
		Last Modified: Wed, 15 Jul 2020 21:14:01 GMT  
		Size: 913.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32f6fe573eab456a9f7b72357c56803fb00bdc82c4919d22ab75252383bf5bd9`  
		Last Modified: Wed, 15 Jul 2020 21:14:01 GMT  
		Size: 892.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:nanoserver-1809`

```console
$ docker pull nats-streaming@sha256:26aa5bae956b8a0445c9021af0290737bdc950d3da65ec399e49c1352cc3ea84
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1339; amd64

### `nats-streaming:nanoserver-1809` - windows version 10.0.17763.1339; amd64

```console
$ docker pull nats-streaming@sha256:536fc04821f79ce86cbaffab4f58b9bb1b2e697f4f1d17b263e02270d1edba47
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.8 MB (106843336 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:40d8dcc1cfa38989cad5eccdc9993517e290c787fc43f466403bd00c1a7ba261`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 07 Jul 2020 13:50:07 GMT
RUN Apply image 1809-amd64
# Wed, 15 Jul 2020 15:05:14 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 15 Jul 2020 21:09:37 GMT
RUN cmd /S /C #(nop) COPY file:4a858ac4da943f868519572e3fb6817fd379875f2bff0bcb5f03c5bdddc496a8 in C:\nats-streaming-server.exe 
# Wed, 15 Jul 2020 21:09:40 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 15 Jul 2020 21:09:40 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 15 Jul 2020 21:09:41 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:dc95608099543221ef539391bfece5c1ce37b97af9da457f5990349cab028a12`  
		Size: 100.9 MB (100895619 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5f0c27d781c53928c03429d5b34e0f49fc26b7e7c996c1d9a2a8474162eade60`  
		Last Modified: Wed, 15 Jul 2020 15:09:50 GMT  
		Size: 869.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c37823d2bd2a59a1d84d807658bb5995febdf048b1f99233390d2b049939efd1`  
		Last Modified: Wed, 15 Jul 2020 21:14:05 GMT  
		Size: 5.9 MB (5944137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9fe8f765dc0de3583e36e3f3ef18e3a3f3a3f75312e35ac1d42c0d95ce90cc0`  
		Last Modified: Wed, 15 Jul 2020 21:14:04 GMT  
		Size: 906.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:349d8da345d930244c13a48049c9f9001d4a04866a33ee215586352c788b5e88`  
		Last Modified: Wed, 15 Jul 2020 21:14:01 GMT  
		Size: 913.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32f6fe573eab456a9f7b72357c56803fb00bdc82c4919d22ab75252383bf5bd9`  
		Last Modified: Wed, 15 Jul 2020 21:14:01 GMT  
		Size: 892.0 B  
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
$ docker pull nats-streaming@sha256:90f956a0b4d242f64dc27f084e4322ad40f669004f06d6660fde87222b4f25bd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1339; amd64
	-	windows version 10.0.14393.3808; amd64

### `nats-streaming:windowsservercore` - windows version 10.0.17763.1339; amd64

```console
$ docker pull nats-streaming@sha256:fd2b16284f5c09bc81615f52d55aa557e0c4faaf4ffbe623fa9c4a9f855094ca
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2330067351 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7796ffa578afe3152a7069c15ad9993baf8de4b7e748bbf2eb9013ecc443ef9a`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Wed, 08 Jul 2020 04:26:49 GMT
RUN Install update 1809-amd64
# Wed, 15 Jul 2020 12:15:48 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 15 Jul 2020 15:03:03 GMT
ENV NATS_DOCKERIZED=1
# Wed, 15 Jul 2020 21:07:08 GMT
ENV NATS_STREAMING_SERVER=0.18.0
# Wed, 15 Jul 2020 21:07:09 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.18.0/nats-streaming-server-v0.18.0-windows-amd64.zip
# Wed, 15 Jul 2020 21:07:10 GMT
ENV GIT_DOWNLOAD_SHA256=a0c0261df2ce589fe9706617323e06c5bcae70511112eae921681b1169674bc8
# Wed, 15 Jul 2020 21:07:45 GMT
RUN Set-PSDebug -Trace 2
# Wed, 15 Jul 2020 21:09:17 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 15 Jul 2020 21:09:18 GMT
EXPOSE 4222 8222
# Wed, 15 Jul 2020 21:09:20 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 15 Jul 2020 21:09:21 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:fc1b9e59edad2bf789457b52138acc367e86072b73bf862eaf96be70f4d4edbb`  
		Size: 591.9 MB (591859374 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:1cc883a0e3509a474bb32f3c40411bf86219325ae9710e25a5dcce6b44eef357`  
		Last Modified: Wed, 15 Jul 2020 14:32:06 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73dd35c9a62007b6ded1ca968562be97de62ea3e2b3c7db85f4a50baaa9efecb`  
		Last Modified: Wed, 15 Jul 2020 15:09:33 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb6c591c0a8170250552e7e384d3a79de15e68f382a34d1e5752c6c7ab0cbfb5`  
		Last Modified: Wed, 15 Jul 2020 21:13:48 GMT  
		Size: 1.1 KB (1084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a1d80c963f67159f6b9cbf927c2fd4bdf00c6f73353f96b1baf98daaa6c7cb5`  
		Last Modified: Wed, 15 Jul 2020 21:13:48 GMT  
		Size: 1.1 KB (1083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26e611a275568f5c39624077dd6209104cd19177aeced5c0b7e0f00e9e7aaa2b`  
		Last Modified: Wed, 15 Jul 2020 21:13:47 GMT  
		Size: 1.1 KB (1070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c167f6381ec0f43e4cfcc10919a987bf178e694e5b2b4cdff32b39161c9411f`  
		Last Modified: Wed, 15 Jul 2020 21:13:47 GMT  
		Size: 4.8 MB (4800424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffec8d449046498ebfc5d1d69f93ec54cb307a7cd7b2a46003d66c63b69edbcd`  
		Last Modified: Wed, 15 Jul 2020 21:13:49 GMT  
		Size: 15.1 MB (15065705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8b0372f086e7590d8b3b4f0c70dbe11c050d24011d09293dc8e1978e0cd25f0`  
		Last Modified: Wed, 15 Jul 2020 21:13:45 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:189e0c6e97c31e972420da6bed768b9f5fb8a5644521f539e83e4ed9c4b13155`  
		Last Modified: Wed, 15 Jul 2020 21:13:45 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a1d615621d3c5ab9becb58f63dd233e553d272091e768dae0074d3c0bd9d124`  
		Last Modified: Wed, 15 Jul 2020 21:13:46 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:windowsservercore` - windows version 10.0.14393.3808; amd64

```console
$ docker pull nats-streaming@sha256:daf9e5a9590ebd64d8629288af9923d028c3130df505f7ff6d2badab5fdb36a4
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5758611587 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b14d84aa3c32e47f13a9aa728500047ce78b9247002ddf8006b19e08bc213366`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 07 Jul 2020 21:05:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 15 Jul 2020 12:24:48 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 15 Jul 2020 15:05:26 GMT
ENV NATS_DOCKERIZED=1
# Wed, 15 Jul 2020 21:09:46 GMT
ENV NATS_STREAMING_SERVER=0.18.0
# Wed, 15 Jul 2020 21:09:47 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.18.0/nats-streaming-server-v0.18.0-windows-amd64.zip
# Wed, 15 Jul 2020 21:09:48 GMT
ENV GIT_DOWNLOAD_SHA256=a0c0261df2ce589fe9706617323e06c5bcae70511112eae921681b1169674bc8
# Wed, 15 Jul 2020 21:11:13 GMT
RUN Set-PSDebug -Trace 2
# Wed, 15 Jul 2020 21:13:11 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 15 Jul 2020 21:13:14 GMT
EXPOSE 4222 8222
# Wed, 15 Jul 2020 21:13:15 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 15 Jul 2020 21:13:16 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:802c4beb8b091968ccf1bb4a853ded7955ddb79e6f8775a5155cb5ed07dcbcab`  
		Size: 1.7 GB (1667476199 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3393eecaf56a66035ab178b379bacf81d30373b630b34b2973501f259aadb0f6`  
		Last Modified: Wed, 15 Jul 2020 14:32:38 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1430ee68db5fe3026683f1b7c74f31ae748da71bf8ad611efede726e9e036b1`  
		Last Modified: Wed, 15 Jul 2020 15:10:21 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75bee39dfb46c142a6dd8c7b99236cd36b36ed56346c403d7be4fb8623f9b8d5`  
		Last Modified: Wed, 15 Jul 2020 21:14:20 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b7de9a5c713789f72af564cdc5f28c0dba85d4b95332f815a7d0ba032170616`  
		Last Modified: Wed, 15 Jul 2020 21:14:20 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7ba6847dae4e00016f022ecb49741fecdfb048a3cf945beed074720180415ff`  
		Last Modified: Wed, 15 Jul 2020 21:14:20 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d62e9ba6e0d6f49e9b722408130b963a54818538f1d9f7f3856239f03795f5ab`  
		Last Modified: Wed, 15 Jul 2020 21:14:19 GMT  
		Size: 5.4 MB (5379274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c099f3a69d1984acb328df528418c5d92a1a208d1949990ebaac1b8256e12b9`  
		Last Modified: Wed, 15 Jul 2020 21:14:21 GMT  
		Size: 15.8 MB (15761002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ec2f283e382f964302246e46c7558554d80d222708541d0ad673e912fd538f4`  
		Last Modified: Wed, 15 Jul 2020 21:14:17 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:748659c661458abcab3c6af30d446fd311404a91f63607c45c10b8620a484270`  
		Last Modified: Wed, 15 Jul 2020 21:14:17 GMT  
		Size: 1.1 KB (1136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fed56fa4c13c0af0264cde0de3b1c5c2d040ed6e725662e6b19057481de9dd0f`  
		Last Modified: Wed, 15 Jul 2020 21:14:17 GMT  
		Size: 1.2 KB (1192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:windowsservercore-1809`

```console
$ docker pull nats-streaming@sha256:323a035ec861fdcbe10d0001a4e9ac0d868297b1b59a6bf7019257715c0f117f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1339; amd64

### `nats-streaming:windowsservercore-1809` - windows version 10.0.17763.1339; amd64

```console
$ docker pull nats-streaming@sha256:fd2b16284f5c09bc81615f52d55aa557e0c4faaf4ffbe623fa9c4a9f855094ca
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2330067351 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7796ffa578afe3152a7069c15ad9993baf8de4b7e748bbf2eb9013ecc443ef9a`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Wed, 08 Jul 2020 04:26:49 GMT
RUN Install update 1809-amd64
# Wed, 15 Jul 2020 12:15:48 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 15 Jul 2020 15:03:03 GMT
ENV NATS_DOCKERIZED=1
# Wed, 15 Jul 2020 21:07:08 GMT
ENV NATS_STREAMING_SERVER=0.18.0
# Wed, 15 Jul 2020 21:07:09 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.18.0/nats-streaming-server-v0.18.0-windows-amd64.zip
# Wed, 15 Jul 2020 21:07:10 GMT
ENV GIT_DOWNLOAD_SHA256=a0c0261df2ce589fe9706617323e06c5bcae70511112eae921681b1169674bc8
# Wed, 15 Jul 2020 21:07:45 GMT
RUN Set-PSDebug -Trace 2
# Wed, 15 Jul 2020 21:09:17 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 15 Jul 2020 21:09:18 GMT
EXPOSE 4222 8222
# Wed, 15 Jul 2020 21:09:20 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 15 Jul 2020 21:09:21 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:fc1b9e59edad2bf789457b52138acc367e86072b73bf862eaf96be70f4d4edbb`  
		Size: 591.9 MB (591859374 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:1cc883a0e3509a474bb32f3c40411bf86219325ae9710e25a5dcce6b44eef357`  
		Last Modified: Wed, 15 Jul 2020 14:32:06 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73dd35c9a62007b6ded1ca968562be97de62ea3e2b3c7db85f4a50baaa9efecb`  
		Last Modified: Wed, 15 Jul 2020 15:09:33 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb6c591c0a8170250552e7e384d3a79de15e68f382a34d1e5752c6c7ab0cbfb5`  
		Last Modified: Wed, 15 Jul 2020 21:13:48 GMT  
		Size: 1.1 KB (1084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a1d80c963f67159f6b9cbf927c2fd4bdf00c6f73353f96b1baf98daaa6c7cb5`  
		Last Modified: Wed, 15 Jul 2020 21:13:48 GMT  
		Size: 1.1 KB (1083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26e611a275568f5c39624077dd6209104cd19177aeced5c0b7e0f00e9e7aaa2b`  
		Last Modified: Wed, 15 Jul 2020 21:13:47 GMT  
		Size: 1.1 KB (1070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c167f6381ec0f43e4cfcc10919a987bf178e694e5b2b4cdff32b39161c9411f`  
		Last Modified: Wed, 15 Jul 2020 21:13:47 GMT  
		Size: 4.8 MB (4800424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffec8d449046498ebfc5d1d69f93ec54cb307a7cd7b2a46003d66c63b69edbcd`  
		Last Modified: Wed, 15 Jul 2020 21:13:49 GMT  
		Size: 15.1 MB (15065705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8b0372f086e7590d8b3b4f0c70dbe11c050d24011d09293dc8e1978e0cd25f0`  
		Last Modified: Wed, 15 Jul 2020 21:13:45 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:189e0c6e97c31e972420da6bed768b9f5fb8a5644521f539e83e4ed9c4b13155`  
		Last Modified: Wed, 15 Jul 2020 21:13:45 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a1d615621d3c5ab9becb58f63dd233e553d272091e768dae0074d3c0bd9d124`  
		Last Modified: Wed, 15 Jul 2020 21:13:46 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:windowsservercore-ltsc2016`

```console
$ docker pull nats-streaming@sha256:9c89c6a37c2686bd1a2ab08e5ddf4a16103a3e37b7649535bc37b16444c5bcca
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3808; amd64

### `nats-streaming:windowsservercore-ltsc2016` - windows version 10.0.14393.3808; amd64

```console
$ docker pull nats-streaming@sha256:daf9e5a9590ebd64d8629288af9923d028c3130df505f7ff6d2badab5fdb36a4
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5758611587 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b14d84aa3c32e47f13a9aa728500047ce78b9247002ddf8006b19e08bc213366`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 07 Jul 2020 21:05:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 15 Jul 2020 12:24:48 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 15 Jul 2020 15:05:26 GMT
ENV NATS_DOCKERIZED=1
# Wed, 15 Jul 2020 21:09:46 GMT
ENV NATS_STREAMING_SERVER=0.18.0
# Wed, 15 Jul 2020 21:09:47 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.18.0/nats-streaming-server-v0.18.0-windows-amd64.zip
# Wed, 15 Jul 2020 21:09:48 GMT
ENV GIT_DOWNLOAD_SHA256=a0c0261df2ce589fe9706617323e06c5bcae70511112eae921681b1169674bc8
# Wed, 15 Jul 2020 21:11:13 GMT
RUN Set-PSDebug -Trace 2
# Wed, 15 Jul 2020 21:13:11 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 15 Jul 2020 21:13:14 GMT
EXPOSE 4222 8222
# Wed, 15 Jul 2020 21:13:15 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 15 Jul 2020 21:13:16 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:802c4beb8b091968ccf1bb4a853ded7955ddb79e6f8775a5155cb5ed07dcbcab`  
		Size: 1.7 GB (1667476199 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3393eecaf56a66035ab178b379bacf81d30373b630b34b2973501f259aadb0f6`  
		Last Modified: Wed, 15 Jul 2020 14:32:38 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1430ee68db5fe3026683f1b7c74f31ae748da71bf8ad611efede726e9e036b1`  
		Last Modified: Wed, 15 Jul 2020 15:10:21 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75bee39dfb46c142a6dd8c7b99236cd36b36ed56346c403d7be4fb8623f9b8d5`  
		Last Modified: Wed, 15 Jul 2020 21:14:20 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b7de9a5c713789f72af564cdc5f28c0dba85d4b95332f815a7d0ba032170616`  
		Last Modified: Wed, 15 Jul 2020 21:14:20 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7ba6847dae4e00016f022ecb49741fecdfb048a3cf945beed074720180415ff`  
		Last Modified: Wed, 15 Jul 2020 21:14:20 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d62e9ba6e0d6f49e9b722408130b963a54818538f1d9f7f3856239f03795f5ab`  
		Last Modified: Wed, 15 Jul 2020 21:14:19 GMT  
		Size: 5.4 MB (5379274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c099f3a69d1984acb328df528418c5d92a1a208d1949990ebaac1b8256e12b9`  
		Last Modified: Wed, 15 Jul 2020 21:14:21 GMT  
		Size: 15.8 MB (15761002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ec2f283e382f964302246e46c7558554d80d222708541d0ad673e912fd538f4`  
		Last Modified: Wed, 15 Jul 2020 21:14:17 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:748659c661458abcab3c6af30d446fd311404a91f63607c45c10b8620a484270`  
		Last Modified: Wed, 15 Jul 2020 21:14:17 GMT  
		Size: 1.1 KB (1136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fed56fa4c13c0af0264cde0de3b1c5c2d040ed6e725662e6b19057481de9dd0f`  
		Last Modified: Wed, 15 Jul 2020 21:14:17 GMT  
		Size: 1.2 KB (1192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
