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
$ docker pull nats-streaming@sha256:e57ac5c71fefaa523ccdb5432772f28a784c2a429be3d0a4939ef3666d79f32c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.1457; amd64

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

### `nats-streaming:0.18` - windows version 10.0.17763.1457; amd64

```console
$ docker pull nats-streaming@sha256:633ee41bf90856c425664d464d0bbde7c719a8d684aae2a4c4aa8c688b273c2f
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.2 MB (107186820 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:800961c202be6010a686406b705d7a401c822eb61b250ae466a82f207e1962cc`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Wed, 02 Sep 2020 12:08:18 GMT
RUN Apply image 1809-amd64
# Wed, 09 Sep 2020 17:12:30 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 09 Sep 2020 20:33:07 GMT
RUN cmd /S /C #(nop) COPY file:4a858ac4da943f868519572e3fb6817fd379875f2bff0bcb5f03c5bdddc496a8 in C:\nats-streaming-server.exe 
# Wed, 09 Sep 2020 20:33:09 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 09 Sep 2020 20:33:10 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 09 Sep 2020 20:33:10 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:ecf9bb62dc6eedea9fd367628f8715dea75b7d2053afa4b5121e7809aa692139`  
		Size: 101.2 MB (101239122 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a993e00682bb4be271d74c200e8e9d454b07999d7ab172f3b14fe72883380722`  
		Last Modified: Wed, 09 Sep 2020 17:16:30 GMT  
		Size: 929.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e73f351ef78c90a784ebe68be1d18a90b8d3d96b4bc34c7a0eef484d8c1dffa`  
		Last Modified: Wed, 09 Sep 2020 20:37:08 GMT  
		Size: 5.9 MB (5944140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b597a9018de11dec33432a01c58c1c8a0b34a109943149eea36418113bb3947d`  
		Last Modified: Wed, 09 Sep 2020 20:37:06 GMT  
		Size: 896.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aafa4807abd9e0fb29a3ea7b8de9201357fe0888234631d6f1b2d19586e85f2f`  
		Last Modified: Wed, 09 Sep 2020 20:37:06 GMT  
		Size: 869.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fd0e0805a30ff0bebf0e1377a6ee0c68cb6a8f23df9fba6c9443e9940ae24e9`  
		Last Modified: Wed, 09 Sep 2020 20:37:06 GMT  
		Size: 864.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.18.0`

```console
$ docker pull nats-streaming@sha256:e57ac5c71fefaa523ccdb5432772f28a784c2a429be3d0a4939ef3666d79f32c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.1457; amd64

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

### `nats-streaming:0.18.0` - windows version 10.0.17763.1457; amd64

```console
$ docker pull nats-streaming@sha256:633ee41bf90856c425664d464d0bbde7c719a8d684aae2a4c4aa8c688b273c2f
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.2 MB (107186820 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:800961c202be6010a686406b705d7a401c822eb61b250ae466a82f207e1962cc`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Wed, 02 Sep 2020 12:08:18 GMT
RUN Apply image 1809-amd64
# Wed, 09 Sep 2020 17:12:30 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 09 Sep 2020 20:33:07 GMT
RUN cmd /S /C #(nop) COPY file:4a858ac4da943f868519572e3fb6817fd379875f2bff0bcb5f03c5bdddc496a8 in C:\nats-streaming-server.exe 
# Wed, 09 Sep 2020 20:33:09 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 09 Sep 2020 20:33:10 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 09 Sep 2020 20:33:10 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:ecf9bb62dc6eedea9fd367628f8715dea75b7d2053afa4b5121e7809aa692139`  
		Size: 101.2 MB (101239122 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a993e00682bb4be271d74c200e8e9d454b07999d7ab172f3b14fe72883380722`  
		Last Modified: Wed, 09 Sep 2020 17:16:30 GMT  
		Size: 929.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e73f351ef78c90a784ebe68be1d18a90b8d3d96b4bc34c7a0eef484d8c1dffa`  
		Last Modified: Wed, 09 Sep 2020 20:37:08 GMT  
		Size: 5.9 MB (5944140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b597a9018de11dec33432a01c58c1c8a0b34a109943149eea36418113bb3947d`  
		Last Modified: Wed, 09 Sep 2020 20:37:06 GMT  
		Size: 896.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aafa4807abd9e0fb29a3ea7b8de9201357fe0888234631d6f1b2d19586e85f2f`  
		Last Modified: Wed, 09 Sep 2020 20:37:06 GMT  
		Size: 869.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fd0e0805a30ff0bebf0e1377a6ee0c68cb6a8f23df9fba6c9443e9940ae24e9`  
		Last Modified: Wed, 09 Sep 2020 20:37:06 GMT  
		Size: 864.0 B  
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
$ docker pull nats-streaming@sha256:80efa6dd34a9994a256f9c60c778702e05691f8fa5405967c4d48d63d64e734f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1457; amd64

### `nats-streaming:0.18.0-nanoserver` - windows version 10.0.17763.1457; amd64

```console
$ docker pull nats-streaming@sha256:633ee41bf90856c425664d464d0bbde7c719a8d684aae2a4c4aa8c688b273c2f
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.2 MB (107186820 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:800961c202be6010a686406b705d7a401c822eb61b250ae466a82f207e1962cc`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Wed, 02 Sep 2020 12:08:18 GMT
RUN Apply image 1809-amd64
# Wed, 09 Sep 2020 17:12:30 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 09 Sep 2020 20:33:07 GMT
RUN cmd /S /C #(nop) COPY file:4a858ac4da943f868519572e3fb6817fd379875f2bff0bcb5f03c5bdddc496a8 in C:\nats-streaming-server.exe 
# Wed, 09 Sep 2020 20:33:09 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 09 Sep 2020 20:33:10 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 09 Sep 2020 20:33:10 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:ecf9bb62dc6eedea9fd367628f8715dea75b7d2053afa4b5121e7809aa692139`  
		Size: 101.2 MB (101239122 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a993e00682bb4be271d74c200e8e9d454b07999d7ab172f3b14fe72883380722`  
		Last Modified: Wed, 09 Sep 2020 17:16:30 GMT  
		Size: 929.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e73f351ef78c90a784ebe68be1d18a90b8d3d96b4bc34c7a0eef484d8c1dffa`  
		Last Modified: Wed, 09 Sep 2020 20:37:08 GMT  
		Size: 5.9 MB (5944140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b597a9018de11dec33432a01c58c1c8a0b34a109943149eea36418113bb3947d`  
		Last Modified: Wed, 09 Sep 2020 20:37:06 GMT  
		Size: 896.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aafa4807abd9e0fb29a3ea7b8de9201357fe0888234631d6f1b2d19586e85f2f`  
		Last Modified: Wed, 09 Sep 2020 20:37:06 GMT  
		Size: 869.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fd0e0805a30ff0bebf0e1377a6ee0c68cb6a8f23df9fba6c9443e9940ae24e9`  
		Last Modified: Wed, 09 Sep 2020 20:37:06 GMT  
		Size: 864.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.18.0-nanoserver-1809`

```console
$ docker pull nats-streaming@sha256:80efa6dd34a9994a256f9c60c778702e05691f8fa5405967c4d48d63d64e734f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1457; amd64

### `nats-streaming:0.18.0-nanoserver-1809` - windows version 10.0.17763.1457; amd64

```console
$ docker pull nats-streaming@sha256:633ee41bf90856c425664d464d0bbde7c719a8d684aae2a4c4aa8c688b273c2f
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.2 MB (107186820 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:800961c202be6010a686406b705d7a401c822eb61b250ae466a82f207e1962cc`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Wed, 02 Sep 2020 12:08:18 GMT
RUN Apply image 1809-amd64
# Wed, 09 Sep 2020 17:12:30 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 09 Sep 2020 20:33:07 GMT
RUN cmd /S /C #(nop) COPY file:4a858ac4da943f868519572e3fb6817fd379875f2bff0bcb5f03c5bdddc496a8 in C:\nats-streaming-server.exe 
# Wed, 09 Sep 2020 20:33:09 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 09 Sep 2020 20:33:10 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 09 Sep 2020 20:33:10 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:ecf9bb62dc6eedea9fd367628f8715dea75b7d2053afa4b5121e7809aa692139`  
		Size: 101.2 MB (101239122 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a993e00682bb4be271d74c200e8e9d454b07999d7ab172f3b14fe72883380722`  
		Last Modified: Wed, 09 Sep 2020 17:16:30 GMT  
		Size: 929.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e73f351ef78c90a784ebe68be1d18a90b8d3d96b4bc34c7a0eef484d8c1dffa`  
		Last Modified: Wed, 09 Sep 2020 20:37:08 GMT  
		Size: 5.9 MB (5944140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b597a9018de11dec33432a01c58c1c8a0b34a109943149eea36418113bb3947d`  
		Last Modified: Wed, 09 Sep 2020 20:37:06 GMT  
		Size: 896.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aafa4807abd9e0fb29a3ea7b8de9201357fe0888234631d6f1b2d19586e85f2f`  
		Last Modified: Wed, 09 Sep 2020 20:37:06 GMT  
		Size: 869.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fd0e0805a30ff0bebf0e1377a6ee0c68cb6a8f23df9fba6c9443e9940ae24e9`  
		Last Modified: Wed, 09 Sep 2020 20:37:06 GMT  
		Size: 864.0 B  
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
$ docker pull nats-streaming@sha256:e8c22bffec8b2ced3d9bef1570fb45f1e168091ad1c5ac8ad284885876ec44d1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1457; amd64
	-	windows version 10.0.14393.3930; amd64

### `nats-streaming:0.18.0-windowsservercore` - windows version 10.0.17763.1457; amd64

```console
$ docker pull nats-streaming@sha256:c94cf73a46b625f0d88728e07a7d2f1f2d5449d2ca74f6aff19065231283599b
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2371111653 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ef12f072c15e6d5c505dec4022a33399d1b1eb10c10968261006daca91e4ce0`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 03 Sep 2020 05:59:01 GMT
RUN Install update 1809-amd64
# Wed, 09 Sep 2020 13:15:06 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Sep 2020 17:10:34 GMT
ENV NATS_DOCKERIZED=1
# Wed, 09 Sep 2020 20:31:10 GMT
ENV NATS_STREAMING_SERVER=0.18.0
# Wed, 09 Sep 2020 20:31:10 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.18.0/nats-streaming-server-v0.18.0-windows-amd64.zip
# Wed, 09 Sep 2020 20:31:11 GMT
ENV GIT_DOWNLOAD_SHA256=a0c0261df2ce589fe9706617323e06c5bcae70511112eae921681b1169674bc8
# Wed, 09 Sep 2020 20:31:40 GMT
RUN Set-PSDebug -Trace 2
# Wed, 09 Sep 2020 20:32:54 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 09 Sep 2020 20:32:55 GMT
EXPOSE 4222 8222
# Wed, 09 Sep 2020 20:32:56 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 09 Sep 2020 20:32:57 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c3aff44502467b94164764856a6feb805fc5c79ff66012eebdd7da3f180e3138`  
		Size: 632.9 MB (632939341 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:1df31adcc7026c3bf0cb32832a3f307dd6e1e54b8b3e050f8a73b5caee674d88`  
		Last Modified: Wed, 09 Sep 2020 16:48:51 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a005485001c0802bc2ee93661375bfb4c868e16c3f5678debf00f29a8bb26386`  
		Last Modified: Wed, 09 Sep 2020 17:16:08 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8694028d86dd4c393914d2d297dd6869064d3eebb0e37f4fbf118b0220e54462`  
		Last Modified: Wed, 09 Sep 2020 20:36:51 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13620d5ec186fd18ae4469cf269f141b543dcf10f69a6f3b154054b096394a12`  
		Last Modified: Wed, 09 Sep 2020 20:36:51 GMT  
		Size: 1.1 KB (1140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:085e5f4e037f4da34b0d4adb9c9895fb6d02e3e157acb4adc891fa27cef8d3bb`  
		Last Modified: Wed, 09 Sep 2020 20:36:51 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0321f95de34d68601a758a932a003b5e3cf6e0e45077ee0b524100c7d08a381f`  
		Last Modified: Wed, 09 Sep 2020 20:36:50 GMT  
		Size: 4.8 MB (4784319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa831bb560296cb990cd36699b5efa30aa0537885f70827a16d14db6c9777901`  
		Last Modified: Wed, 09 Sep 2020 20:36:52 GMT  
		Size: 15.0 MB (15045992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2cd5f57708b2d773c1ece864eab14ba8a4c9a8ed13882e5aeeda9cb66ec0586`  
		Last Modified: Wed, 09 Sep 2020 20:36:48 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c35decd3f52c0519150414ac9c188b632ca4fb591eb4adca28d95b5bf12b9fa0`  
		Last Modified: Wed, 09 Sep 2020 20:36:49 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97f0407c16bfc68dbc3501cf3e406dc1a256a093ed77043eec98317f272e0017`  
		Last Modified: Wed, 09 Sep 2020 20:36:48 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.18.0-windowsservercore` - windows version 10.0.14393.3930; amd64

```console
$ docker pull nats-streaming@sha256:981ef599a734b64a66cac4f2d5cba055451854d765898f9993fec7811ca1c394
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5760484146 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86d2337b5310038c6b37fadf4c91e7e441252a28e8a77576f9140384a4f4672f`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 01 Sep 2020 19:14:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 09 Sep 2020 13:23:04 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Sep 2020 17:12:41 GMT
ENV NATS_DOCKERIZED=1
# Wed, 09 Sep 2020 20:33:15 GMT
ENV NATS_STREAMING_SERVER=0.18.0
# Wed, 09 Sep 2020 20:33:16 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.18.0/nats-streaming-server-v0.18.0-windows-amd64.zip
# Wed, 09 Sep 2020 20:33:16 GMT
ENV GIT_DOWNLOAD_SHA256=a0c0261df2ce589fe9706617323e06c5bcae70511112eae921681b1169674bc8
# Wed, 09 Sep 2020 20:34:26 GMT
RUN Set-PSDebug -Trace 2
# Wed, 09 Sep 2020 20:36:11 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 09 Sep 2020 20:36:11 GMT
EXPOSE 4222 8222
# Wed, 09 Sep 2020 20:36:12 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 09 Sep 2020 20:36:14 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bc202b498d589027cc702b23cf959b8842907508b3465b9d6ff739c9668e5134`  
		Size: 1.7 GB (1669268544 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c1d56eeebea105bba2dd1879a89adb012f98cf42708c0f36ca4af683db7162a2`  
		Last Modified: Wed, 09 Sep 2020 16:49:22 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae4d96d0f21f7d823b426589ab2a404cd548354f8d03ceb98ed43812aa4ea498`  
		Last Modified: Wed, 09 Sep 2020 17:16:52 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd2d7de21675e6a7b359d125e71a443d18e04e40860dec675c44d37c7361ed62`  
		Last Modified: Wed, 09 Sep 2020 20:37:23 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae08ee6b7fee5f9fffc78e4c7f2f4c89dcbf18422a72fbe3a79bafdf7bd44640`  
		Last Modified: Wed, 09 Sep 2020 20:37:23 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80ebec154bb3a413d80d85884bf30c098fdc5ca1bb89bed4101a5a8461ff6301`  
		Last Modified: Wed, 09 Sep 2020 20:37:23 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a4c2d3b77c41d8255a747b40d4ca2979be47b74ed08ce2599a2995eef1b613b`  
		Last Modified: Wed, 09 Sep 2020 20:37:22 GMT  
		Size: 5.4 MB (5378060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ca76e108efd6235186de526ff5505988de6cff23592026dd8760d11aeea5bdd`  
		Last Modified: Wed, 09 Sep 2020 20:37:38 GMT  
		Size: 15.8 MB (15842566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdcd8c348d7e661add432378d1a17026e0ca4b65a205cb77cc3b9df060dc0cdf`  
		Last Modified: Wed, 09 Sep 2020 20:37:20 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c55596ce0711ce624d77dfd64a752d31630a12a964365db81412beabdf0ae0ea`  
		Last Modified: Wed, 09 Sep 2020 20:37:20 GMT  
		Size: 1.1 KB (1140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3b82f600ad3dd8623c8638a813ae0eb243b2a9f9c0fa6f3a8b3b3d9bd5b47db`  
		Last Modified: Wed, 09 Sep 2020 20:37:21 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.18.0-windowsservercore-1809`

```console
$ docker pull nats-streaming@sha256:31da8c5a6f0efbee7be5dac0e9851ab6d38d6548d1c2521d6b22b17554ac7660
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1457; amd64

### `nats-streaming:0.18.0-windowsservercore-1809` - windows version 10.0.17763.1457; amd64

```console
$ docker pull nats-streaming@sha256:c94cf73a46b625f0d88728e07a7d2f1f2d5449d2ca74f6aff19065231283599b
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2371111653 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ef12f072c15e6d5c505dec4022a33399d1b1eb10c10968261006daca91e4ce0`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 03 Sep 2020 05:59:01 GMT
RUN Install update 1809-amd64
# Wed, 09 Sep 2020 13:15:06 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Sep 2020 17:10:34 GMT
ENV NATS_DOCKERIZED=1
# Wed, 09 Sep 2020 20:31:10 GMT
ENV NATS_STREAMING_SERVER=0.18.0
# Wed, 09 Sep 2020 20:31:10 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.18.0/nats-streaming-server-v0.18.0-windows-amd64.zip
# Wed, 09 Sep 2020 20:31:11 GMT
ENV GIT_DOWNLOAD_SHA256=a0c0261df2ce589fe9706617323e06c5bcae70511112eae921681b1169674bc8
# Wed, 09 Sep 2020 20:31:40 GMT
RUN Set-PSDebug -Trace 2
# Wed, 09 Sep 2020 20:32:54 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 09 Sep 2020 20:32:55 GMT
EXPOSE 4222 8222
# Wed, 09 Sep 2020 20:32:56 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 09 Sep 2020 20:32:57 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c3aff44502467b94164764856a6feb805fc5c79ff66012eebdd7da3f180e3138`  
		Size: 632.9 MB (632939341 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:1df31adcc7026c3bf0cb32832a3f307dd6e1e54b8b3e050f8a73b5caee674d88`  
		Last Modified: Wed, 09 Sep 2020 16:48:51 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a005485001c0802bc2ee93661375bfb4c868e16c3f5678debf00f29a8bb26386`  
		Last Modified: Wed, 09 Sep 2020 17:16:08 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8694028d86dd4c393914d2d297dd6869064d3eebb0e37f4fbf118b0220e54462`  
		Last Modified: Wed, 09 Sep 2020 20:36:51 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13620d5ec186fd18ae4469cf269f141b543dcf10f69a6f3b154054b096394a12`  
		Last Modified: Wed, 09 Sep 2020 20:36:51 GMT  
		Size: 1.1 KB (1140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:085e5f4e037f4da34b0d4adb9c9895fb6d02e3e157acb4adc891fa27cef8d3bb`  
		Last Modified: Wed, 09 Sep 2020 20:36:51 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0321f95de34d68601a758a932a003b5e3cf6e0e45077ee0b524100c7d08a381f`  
		Last Modified: Wed, 09 Sep 2020 20:36:50 GMT  
		Size: 4.8 MB (4784319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa831bb560296cb990cd36699b5efa30aa0537885f70827a16d14db6c9777901`  
		Last Modified: Wed, 09 Sep 2020 20:36:52 GMT  
		Size: 15.0 MB (15045992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2cd5f57708b2d773c1ece864eab14ba8a4c9a8ed13882e5aeeda9cb66ec0586`  
		Last Modified: Wed, 09 Sep 2020 20:36:48 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c35decd3f52c0519150414ac9c188b632ca4fb591eb4adca28d95b5bf12b9fa0`  
		Last Modified: Wed, 09 Sep 2020 20:36:49 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97f0407c16bfc68dbc3501cf3e406dc1a256a093ed77043eec98317f272e0017`  
		Last Modified: Wed, 09 Sep 2020 20:36:48 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.18.0-windowsservercore-ltsc2016`

```console
$ docker pull nats-streaming@sha256:702f25fac8d3eff9cf2716c95681b464c2d7e7c6a741a1e3e7df31177ff08cc8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3930; amd64

### `nats-streaming:0.18.0-windowsservercore-ltsc2016` - windows version 10.0.14393.3930; amd64

```console
$ docker pull nats-streaming@sha256:981ef599a734b64a66cac4f2d5cba055451854d765898f9993fec7811ca1c394
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5760484146 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86d2337b5310038c6b37fadf4c91e7e441252a28e8a77576f9140384a4f4672f`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 01 Sep 2020 19:14:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 09 Sep 2020 13:23:04 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Sep 2020 17:12:41 GMT
ENV NATS_DOCKERIZED=1
# Wed, 09 Sep 2020 20:33:15 GMT
ENV NATS_STREAMING_SERVER=0.18.0
# Wed, 09 Sep 2020 20:33:16 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.18.0/nats-streaming-server-v0.18.0-windows-amd64.zip
# Wed, 09 Sep 2020 20:33:16 GMT
ENV GIT_DOWNLOAD_SHA256=a0c0261df2ce589fe9706617323e06c5bcae70511112eae921681b1169674bc8
# Wed, 09 Sep 2020 20:34:26 GMT
RUN Set-PSDebug -Trace 2
# Wed, 09 Sep 2020 20:36:11 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 09 Sep 2020 20:36:11 GMT
EXPOSE 4222 8222
# Wed, 09 Sep 2020 20:36:12 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 09 Sep 2020 20:36:14 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bc202b498d589027cc702b23cf959b8842907508b3465b9d6ff739c9668e5134`  
		Size: 1.7 GB (1669268544 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c1d56eeebea105bba2dd1879a89adb012f98cf42708c0f36ca4af683db7162a2`  
		Last Modified: Wed, 09 Sep 2020 16:49:22 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae4d96d0f21f7d823b426589ab2a404cd548354f8d03ceb98ed43812aa4ea498`  
		Last Modified: Wed, 09 Sep 2020 17:16:52 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd2d7de21675e6a7b359d125e71a443d18e04e40860dec675c44d37c7361ed62`  
		Last Modified: Wed, 09 Sep 2020 20:37:23 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae08ee6b7fee5f9fffc78e4c7f2f4c89dcbf18422a72fbe3a79bafdf7bd44640`  
		Last Modified: Wed, 09 Sep 2020 20:37:23 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80ebec154bb3a413d80d85884bf30c098fdc5ca1bb89bed4101a5a8461ff6301`  
		Last Modified: Wed, 09 Sep 2020 20:37:23 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a4c2d3b77c41d8255a747b40d4ca2979be47b74ed08ce2599a2995eef1b613b`  
		Last Modified: Wed, 09 Sep 2020 20:37:22 GMT  
		Size: 5.4 MB (5378060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ca76e108efd6235186de526ff5505988de6cff23592026dd8760d11aeea5bdd`  
		Last Modified: Wed, 09 Sep 2020 20:37:38 GMT  
		Size: 15.8 MB (15842566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdcd8c348d7e661add432378d1a17026e0ca4b65a205cb77cc3b9df060dc0cdf`  
		Last Modified: Wed, 09 Sep 2020 20:37:20 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c55596ce0711ce624d77dfd64a752d31630a12a964365db81412beabdf0ae0ea`  
		Last Modified: Wed, 09 Sep 2020 20:37:20 GMT  
		Size: 1.1 KB (1140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3b82f600ad3dd8623c8638a813ae0eb243b2a9f9c0fa6f3a8b3b3d9bd5b47db`  
		Last Modified: Wed, 09 Sep 2020 20:37:21 GMT  
		Size: 1.1 KB (1150 bytes)  
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
$ docker pull nats-streaming@sha256:80efa6dd34a9994a256f9c60c778702e05691f8fa5405967c4d48d63d64e734f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1457; amd64

### `nats-streaming:0.18-nanoserver` - windows version 10.0.17763.1457; amd64

```console
$ docker pull nats-streaming@sha256:633ee41bf90856c425664d464d0bbde7c719a8d684aae2a4c4aa8c688b273c2f
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.2 MB (107186820 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:800961c202be6010a686406b705d7a401c822eb61b250ae466a82f207e1962cc`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Wed, 02 Sep 2020 12:08:18 GMT
RUN Apply image 1809-amd64
# Wed, 09 Sep 2020 17:12:30 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 09 Sep 2020 20:33:07 GMT
RUN cmd /S /C #(nop) COPY file:4a858ac4da943f868519572e3fb6817fd379875f2bff0bcb5f03c5bdddc496a8 in C:\nats-streaming-server.exe 
# Wed, 09 Sep 2020 20:33:09 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 09 Sep 2020 20:33:10 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 09 Sep 2020 20:33:10 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:ecf9bb62dc6eedea9fd367628f8715dea75b7d2053afa4b5121e7809aa692139`  
		Size: 101.2 MB (101239122 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a993e00682bb4be271d74c200e8e9d454b07999d7ab172f3b14fe72883380722`  
		Last Modified: Wed, 09 Sep 2020 17:16:30 GMT  
		Size: 929.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e73f351ef78c90a784ebe68be1d18a90b8d3d96b4bc34c7a0eef484d8c1dffa`  
		Last Modified: Wed, 09 Sep 2020 20:37:08 GMT  
		Size: 5.9 MB (5944140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b597a9018de11dec33432a01c58c1c8a0b34a109943149eea36418113bb3947d`  
		Last Modified: Wed, 09 Sep 2020 20:37:06 GMT  
		Size: 896.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aafa4807abd9e0fb29a3ea7b8de9201357fe0888234631d6f1b2d19586e85f2f`  
		Last Modified: Wed, 09 Sep 2020 20:37:06 GMT  
		Size: 869.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fd0e0805a30ff0bebf0e1377a6ee0c68cb6a8f23df9fba6c9443e9940ae24e9`  
		Last Modified: Wed, 09 Sep 2020 20:37:06 GMT  
		Size: 864.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.18-nanoserver-1809`

```console
$ docker pull nats-streaming@sha256:80efa6dd34a9994a256f9c60c778702e05691f8fa5405967c4d48d63d64e734f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1457; amd64

### `nats-streaming:0.18-nanoserver-1809` - windows version 10.0.17763.1457; amd64

```console
$ docker pull nats-streaming@sha256:633ee41bf90856c425664d464d0bbde7c719a8d684aae2a4c4aa8c688b273c2f
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.2 MB (107186820 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:800961c202be6010a686406b705d7a401c822eb61b250ae466a82f207e1962cc`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Wed, 02 Sep 2020 12:08:18 GMT
RUN Apply image 1809-amd64
# Wed, 09 Sep 2020 17:12:30 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 09 Sep 2020 20:33:07 GMT
RUN cmd /S /C #(nop) COPY file:4a858ac4da943f868519572e3fb6817fd379875f2bff0bcb5f03c5bdddc496a8 in C:\nats-streaming-server.exe 
# Wed, 09 Sep 2020 20:33:09 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 09 Sep 2020 20:33:10 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 09 Sep 2020 20:33:10 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:ecf9bb62dc6eedea9fd367628f8715dea75b7d2053afa4b5121e7809aa692139`  
		Size: 101.2 MB (101239122 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a993e00682bb4be271d74c200e8e9d454b07999d7ab172f3b14fe72883380722`  
		Last Modified: Wed, 09 Sep 2020 17:16:30 GMT  
		Size: 929.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e73f351ef78c90a784ebe68be1d18a90b8d3d96b4bc34c7a0eef484d8c1dffa`  
		Last Modified: Wed, 09 Sep 2020 20:37:08 GMT  
		Size: 5.9 MB (5944140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b597a9018de11dec33432a01c58c1c8a0b34a109943149eea36418113bb3947d`  
		Last Modified: Wed, 09 Sep 2020 20:37:06 GMT  
		Size: 896.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aafa4807abd9e0fb29a3ea7b8de9201357fe0888234631d6f1b2d19586e85f2f`  
		Last Modified: Wed, 09 Sep 2020 20:37:06 GMT  
		Size: 869.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fd0e0805a30ff0bebf0e1377a6ee0c68cb6a8f23df9fba6c9443e9940ae24e9`  
		Last Modified: Wed, 09 Sep 2020 20:37:06 GMT  
		Size: 864.0 B  
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
$ docker pull nats-streaming@sha256:e8c22bffec8b2ced3d9bef1570fb45f1e168091ad1c5ac8ad284885876ec44d1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1457; amd64
	-	windows version 10.0.14393.3930; amd64

### `nats-streaming:0.18-windowsservercore` - windows version 10.0.17763.1457; amd64

```console
$ docker pull nats-streaming@sha256:c94cf73a46b625f0d88728e07a7d2f1f2d5449d2ca74f6aff19065231283599b
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2371111653 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ef12f072c15e6d5c505dec4022a33399d1b1eb10c10968261006daca91e4ce0`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 03 Sep 2020 05:59:01 GMT
RUN Install update 1809-amd64
# Wed, 09 Sep 2020 13:15:06 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Sep 2020 17:10:34 GMT
ENV NATS_DOCKERIZED=1
# Wed, 09 Sep 2020 20:31:10 GMT
ENV NATS_STREAMING_SERVER=0.18.0
# Wed, 09 Sep 2020 20:31:10 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.18.0/nats-streaming-server-v0.18.0-windows-amd64.zip
# Wed, 09 Sep 2020 20:31:11 GMT
ENV GIT_DOWNLOAD_SHA256=a0c0261df2ce589fe9706617323e06c5bcae70511112eae921681b1169674bc8
# Wed, 09 Sep 2020 20:31:40 GMT
RUN Set-PSDebug -Trace 2
# Wed, 09 Sep 2020 20:32:54 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 09 Sep 2020 20:32:55 GMT
EXPOSE 4222 8222
# Wed, 09 Sep 2020 20:32:56 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 09 Sep 2020 20:32:57 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c3aff44502467b94164764856a6feb805fc5c79ff66012eebdd7da3f180e3138`  
		Size: 632.9 MB (632939341 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:1df31adcc7026c3bf0cb32832a3f307dd6e1e54b8b3e050f8a73b5caee674d88`  
		Last Modified: Wed, 09 Sep 2020 16:48:51 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a005485001c0802bc2ee93661375bfb4c868e16c3f5678debf00f29a8bb26386`  
		Last Modified: Wed, 09 Sep 2020 17:16:08 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8694028d86dd4c393914d2d297dd6869064d3eebb0e37f4fbf118b0220e54462`  
		Last Modified: Wed, 09 Sep 2020 20:36:51 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13620d5ec186fd18ae4469cf269f141b543dcf10f69a6f3b154054b096394a12`  
		Last Modified: Wed, 09 Sep 2020 20:36:51 GMT  
		Size: 1.1 KB (1140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:085e5f4e037f4da34b0d4adb9c9895fb6d02e3e157acb4adc891fa27cef8d3bb`  
		Last Modified: Wed, 09 Sep 2020 20:36:51 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0321f95de34d68601a758a932a003b5e3cf6e0e45077ee0b524100c7d08a381f`  
		Last Modified: Wed, 09 Sep 2020 20:36:50 GMT  
		Size: 4.8 MB (4784319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa831bb560296cb990cd36699b5efa30aa0537885f70827a16d14db6c9777901`  
		Last Modified: Wed, 09 Sep 2020 20:36:52 GMT  
		Size: 15.0 MB (15045992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2cd5f57708b2d773c1ece864eab14ba8a4c9a8ed13882e5aeeda9cb66ec0586`  
		Last Modified: Wed, 09 Sep 2020 20:36:48 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c35decd3f52c0519150414ac9c188b632ca4fb591eb4adca28d95b5bf12b9fa0`  
		Last Modified: Wed, 09 Sep 2020 20:36:49 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97f0407c16bfc68dbc3501cf3e406dc1a256a093ed77043eec98317f272e0017`  
		Last Modified: Wed, 09 Sep 2020 20:36:48 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.18-windowsservercore` - windows version 10.0.14393.3930; amd64

```console
$ docker pull nats-streaming@sha256:981ef599a734b64a66cac4f2d5cba055451854d765898f9993fec7811ca1c394
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5760484146 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86d2337b5310038c6b37fadf4c91e7e441252a28e8a77576f9140384a4f4672f`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 01 Sep 2020 19:14:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 09 Sep 2020 13:23:04 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Sep 2020 17:12:41 GMT
ENV NATS_DOCKERIZED=1
# Wed, 09 Sep 2020 20:33:15 GMT
ENV NATS_STREAMING_SERVER=0.18.0
# Wed, 09 Sep 2020 20:33:16 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.18.0/nats-streaming-server-v0.18.0-windows-amd64.zip
# Wed, 09 Sep 2020 20:33:16 GMT
ENV GIT_DOWNLOAD_SHA256=a0c0261df2ce589fe9706617323e06c5bcae70511112eae921681b1169674bc8
# Wed, 09 Sep 2020 20:34:26 GMT
RUN Set-PSDebug -Trace 2
# Wed, 09 Sep 2020 20:36:11 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 09 Sep 2020 20:36:11 GMT
EXPOSE 4222 8222
# Wed, 09 Sep 2020 20:36:12 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 09 Sep 2020 20:36:14 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bc202b498d589027cc702b23cf959b8842907508b3465b9d6ff739c9668e5134`  
		Size: 1.7 GB (1669268544 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c1d56eeebea105bba2dd1879a89adb012f98cf42708c0f36ca4af683db7162a2`  
		Last Modified: Wed, 09 Sep 2020 16:49:22 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae4d96d0f21f7d823b426589ab2a404cd548354f8d03ceb98ed43812aa4ea498`  
		Last Modified: Wed, 09 Sep 2020 17:16:52 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd2d7de21675e6a7b359d125e71a443d18e04e40860dec675c44d37c7361ed62`  
		Last Modified: Wed, 09 Sep 2020 20:37:23 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae08ee6b7fee5f9fffc78e4c7f2f4c89dcbf18422a72fbe3a79bafdf7bd44640`  
		Last Modified: Wed, 09 Sep 2020 20:37:23 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80ebec154bb3a413d80d85884bf30c098fdc5ca1bb89bed4101a5a8461ff6301`  
		Last Modified: Wed, 09 Sep 2020 20:37:23 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a4c2d3b77c41d8255a747b40d4ca2979be47b74ed08ce2599a2995eef1b613b`  
		Last Modified: Wed, 09 Sep 2020 20:37:22 GMT  
		Size: 5.4 MB (5378060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ca76e108efd6235186de526ff5505988de6cff23592026dd8760d11aeea5bdd`  
		Last Modified: Wed, 09 Sep 2020 20:37:38 GMT  
		Size: 15.8 MB (15842566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdcd8c348d7e661add432378d1a17026e0ca4b65a205cb77cc3b9df060dc0cdf`  
		Last Modified: Wed, 09 Sep 2020 20:37:20 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c55596ce0711ce624d77dfd64a752d31630a12a964365db81412beabdf0ae0ea`  
		Last Modified: Wed, 09 Sep 2020 20:37:20 GMT  
		Size: 1.1 KB (1140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3b82f600ad3dd8623c8638a813ae0eb243b2a9f9c0fa6f3a8b3b3d9bd5b47db`  
		Last Modified: Wed, 09 Sep 2020 20:37:21 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.18-windowsservercore-1809`

```console
$ docker pull nats-streaming@sha256:31da8c5a6f0efbee7be5dac0e9851ab6d38d6548d1c2521d6b22b17554ac7660
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1457; amd64

### `nats-streaming:0.18-windowsservercore-1809` - windows version 10.0.17763.1457; amd64

```console
$ docker pull nats-streaming@sha256:c94cf73a46b625f0d88728e07a7d2f1f2d5449d2ca74f6aff19065231283599b
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2371111653 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ef12f072c15e6d5c505dec4022a33399d1b1eb10c10968261006daca91e4ce0`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 03 Sep 2020 05:59:01 GMT
RUN Install update 1809-amd64
# Wed, 09 Sep 2020 13:15:06 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Sep 2020 17:10:34 GMT
ENV NATS_DOCKERIZED=1
# Wed, 09 Sep 2020 20:31:10 GMT
ENV NATS_STREAMING_SERVER=0.18.0
# Wed, 09 Sep 2020 20:31:10 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.18.0/nats-streaming-server-v0.18.0-windows-amd64.zip
# Wed, 09 Sep 2020 20:31:11 GMT
ENV GIT_DOWNLOAD_SHA256=a0c0261df2ce589fe9706617323e06c5bcae70511112eae921681b1169674bc8
# Wed, 09 Sep 2020 20:31:40 GMT
RUN Set-PSDebug -Trace 2
# Wed, 09 Sep 2020 20:32:54 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 09 Sep 2020 20:32:55 GMT
EXPOSE 4222 8222
# Wed, 09 Sep 2020 20:32:56 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 09 Sep 2020 20:32:57 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c3aff44502467b94164764856a6feb805fc5c79ff66012eebdd7da3f180e3138`  
		Size: 632.9 MB (632939341 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:1df31adcc7026c3bf0cb32832a3f307dd6e1e54b8b3e050f8a73b5caee674d88`  
		Last Modified: Wed, 09 Sep 2020 16:48:51 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a005485001c0802bc2ee93661375bfb4c868e16c3f5678debf00f29a8bb26386`  
		Last Modified: Wed, 09 Sep 2020 17:16:08 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8694028d86dd4c393914d2d297dd6869064d3eebb0e37f4fbf118b0220e54462`  
		Last Modified: Wed, 09 Sep 2020 20:36:51 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13620d5ec186fd18ae4469cf269f141b543dcf10f69a6f3b154054b096394a12`  
		Last Modified: Wed, 09 Sep 2020 20:36:51 GMT  
		Size: 1.1 KB (1140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:085e5f4e037f4da34b0d4adb9c9895fb6d02e3e157acb4adc891fa27cef8d3bb`  
		Last Modified: Wed, 09 Sep 2020 20:36:51 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0321f95de34d68601a758a932a003b5e3cf6e0e45077ee0b524100c7d08a381f`  
		Last Modified: Wed, 09 Sep 2020 20:36:50 GMT  
		Size: 4.8 MB (4784319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa831bb560296cb990cd36699b5efa30aa0537885f70827a16d14db6c9777901`  
		Last Modified: Wed, 09 Sep 2020 20:36:52 GMT  
		Size: 15.0 MB (15045992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2cd5f57708b2d773c1ece864eab14ba8a4c9a8ed13882e5aeeda9cb66ec0586`  
		Last Modified: Wed, 09 Sep 2020 20:36:48 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c35decd3f52c0519150414ac9c188b632ca4fb591eb4adca28d95b5bf12b9fa0`  
		Last Modified: Wed, 09 Sep 2020 20:36:49 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97f0407c16bfc68dbc3501cf3e406dc1a256a093ed77043eec98317f272e0017`  
		Last Modified: Wed, 09 Sep 2020 20:36:48 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.18-windowsservercore-ltsc2016`

```console
$ docker pull nats-streaming@sha256:702f25fac8d3eff9cf2716c95681b464c2d7e7c6a741a1e3e7df31177ff08cc8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3930; amd64

### `nats-streaming:0.18-windowsservercore-ltsc2016` - windows version 10.0.14393.3930; amd64

```console
$ docker pull nats-streaming@sha256:981ef599a734b64a66cac4f2d5cba055451854d765898f9993fec7811ca1c394
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5760484146 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86d2337b5310038c6b37fadf4c91e7e441252a28e8a77576f9140384a4f4672f`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 01 Sep 2020 19:14:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 09 Sep 2020 13:23:04 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Sep 2020 17:12:41 GMT
ENV NATS_DOCKERIZED=1
# Wed, 09 Sep 2020 20:33:15 GMT
ENV NATS_STREAMING_SERVER=0.18.0
# Wed, 09 Sep 2020 20:33:16 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.18.0/nats-streaming-server-v0.18.0-windows-amd64.zip
# Wed, 09 Sep 2020 20:33:16 GMT
ENV GIT_DOWNLOAD_SHA256=a0c0261df2ce589fe9706617323e06c5bcae70511112eae921681b1169674bc8
# Wed, 09 Sep 2020 20:34:26 GMT
RUN Set-PSDebug -Trace 2
# Wed, 09 Sep 2020 20:36:11 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 09 Sep 2020 20:36:11 GMT
EXPOSE 4222 8222
# Wed, 09 Sep 2020 20:36:12 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 09 Sep 2020 20:36:14 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bc202b498d589027cc702b23cf959b8842907508b3465b9d6ff739c9668e5134`  
		Size: 1.7 GB (1669268544 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c1d56eeebea105bba2dd1879a89adb012f98cf42708c0f36ca4af683db7162a2`  
		Last Modified: Wed, 09 Sep 2020 16:49:22 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae4d96d0f21f7d823b426589ab2a404cd548354f8d03ceb98ed43812aa4ea498`  
		Last Modified: Wed, 09 Sep 2020 17:16:52 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd2d7de21675e6a7b359d125e71a443d18e04e40860dec675c44d37c7361ed62`  
		Last Modified: Wed, 09 Sep 2020 20:37:23 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae08ee6b7fee5f9fffc78e4c7f2f4c89dcbf18422a72fbe3a79bafdf7bd44640`  
		Last Modified: Wed, 09 Sep 2020 20:37:23 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80ebec154bb3a413d80d85884bf30c098fdc5ca1bb89bed4101a5a8461ff6301`  
		Last Modified: Wed, 09 Sep 2020 20:37:23 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a4c2d3b77c41d8255a747b40d4ca2979be47b74ed08ce2599a2995eef1b613b`  
		Last Modified: Wed, 09 Sep 2020 20:37:22 GMT  
		Size: 5.4 MB (5378060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ca76e108efd6235186de526ff5505988de6cff23592026dd8760d11aeea5bdd`  
		Last Modified: Wed, 09 Sep 2020 20:37:38 GMT  
		Size: 15.8 MB (15842566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdcd8c348d7e661add432378d1a17026e0ca4b65a205cb77cc3b9df060dc0cdf`  
		Last Modified: Wed, 09 Sep 2020 20:37:20 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c55596ce0711ce624d77dfd64a752d31630a12a964365db81412beabdf0ae0ea`  
		Last Modified: Wed, 09 Sep 2020 20:37:20 GMT  
		Size: 1.1 KB (1140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3b82f600ad3dd8623c8638a813ae0eb243b2a9f9c0fa6f3a8b3b3d9bd5b47db`  
		Last Modified: Wed, 09 Sep 2020 20:37:21 GMT  
		Size: 1.1 KB (1150 bytes)  
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
$ docker pull nats-streaming@sha256:e57ac5c71fefaa523ccdb5432772f28a784c2a429be3d0a4939ef3666d79f32c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.1457; amd64

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

### `nats-streaming:latest` - windows version 10.0.17763.1457; amd64

```console
$ docker pull nats-streaming@sha256:633ee41bf90856c425664d464d0bbde7c719a8d684aae2a4c4aa8c688b273c2f
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.2 MB (107186820 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:800961c202be6010a686406b705d7a401c822eb61b250ae466a82f207e1962cc`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Wed, 02 Sep 2020 12:08:18 GMT
RUN Apply image 1809-amd64
# Wed, 09 Sep 2020 17:12:30 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 09 Sep 2020 20:33:07 GMT
RUN cmd /S /C #(nop) COPY file:4a858ac4da943f868519572e3fb6817fd379875f2bff0bcb5f03c5bdddc496a8 in C:\nats-streaming-server.exe 
# Wed, 09 Sep 2020 20:33:09 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 09 Sep 2020 20:33:10 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 09 Sep 2020 20:33:10 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:ecf9bb62dc6eedea9fd367628f8715dea75b7d2053afa4b5121e7809aa692139`  
		Size: 101.2 MB (101239122 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a993e00682bb4be271d74c200e8e9d454b07999d7ab172f3b14fe72883380722`  
		Last Modified: Wed, 09 Sep 2020 17:16:30 GMT  
		Size: 929.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e73f351ef78c90a784ebe68be1d18a90b8d3d96b4bc34c7a0eef484d8c1dffa`  
		Last Modified: Wed, 09 Sep 2020 20:37:08 GMT  
		Size: 5.9 MB (5944140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b597a9018de11dec33432a01c58c1c8a0b34a109943149eea36418113bb3947d`  
		Last Modified: Wed, 09 Sep 2020 20:37:06 GMT  
		Size: 896.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aafa4807abd9e0fb29a3ea7b8de9201357fe0888234631d6f1b2d19586e85f2f`  
		Last Modified: Wed, 09 Sep 2020 20:37:06 GMT  
		Size: 869.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fd0e0805a30ff0bebf0e1377a6ee0c68cb6a8f23df9fba6c9443e9940ae24e9`  
		Last Modified: Wed, 09 Sep 2020 20:37:06 GMT  
		Size: 864.0 B  
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
$ docker pull nats-streaming@sha256:80efa6dd34a9994a256f9c60c778702e05691f8fa5405967c4d48d63d64e734f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1457; amd64

### `nats-streaming:nanoserver` - windows version 10.0.17763.1457; amd64

```console
$ docker pull nats-streaming@sha256:633ee41bf90856c425664d464d0bbde7c719a8d684aae2a4c4aa8c688b273c2f
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.2 MB (107186820 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:800961c202be6010a686406b705d7a401c822eb61b250ae466a82f207e1962cc`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Wed, 02 Sep 2020 12:08:18 GMT
RUN Apply image 1809-amd64
# Wed, 09 Sep 2020 17:12:30 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 09 Sep 2020 20:33:07 GMT
RUN cmd /S /C #(nop) COPY file:4a858ac4da943f868519572e3fb6817fd379875f2bff0bcb5f03c5bdddc496a8 in C:\nats-streaming-server.exe 
# Wed, 09 Sep 2020 20:33:09 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 09 Sep 2020 20:33:10 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 09 Sep 2020 20:33:10 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:ecf9bb62dc6eedea9fd367628f8715dea75b7d2053afa4b5121e7809aa692139`  
		Size: 101.2 MB (101239122 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a993e00682bb4be271d74c200e8e9d454b07999d7ab172f3b14fe72883380722`  
		Last Modified: Wed, 09 Sep 2020 17:16:30 GMT  
		Size: 929.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e73f351ef78c90a784ebe68be1d18a90b8d3d96b4bc34c7a0eef484d8c1dffa`  
		Last Modified: Wed, 09 Sep 2020 20:37:08 GMT  
		Size: 5.9 MB (5944140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b597a9018de11dec33432a01c58c1c8a0b34a109943149eea36418113bb3947d`  
		Last Modified: Wed, 09 Sep 2020 20:37:06 GMT  
		Size: 896.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aafa4807abd9e0fb29a3ea7b8de9201357fe0888234631d6f1b2d19586e85f2f`  
		Last Modified: Wed, 09 Sep 2020 20:37:06 GMT  
		Size: 869.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fd0e0805a30ff0bebf0e1377a6ee0c68cb6a8f23df9fba6c9443e9940ae24e9`  
		Last Modified: Wed, 09 Sep 2020 20:37:06 GMT  
		Size: 864.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:nanoserver-1809`

```console
$ docker pull nats-streaming@sha256:80efa6dd34a9994a256f9c60c778702e05691f8fa5405967c4d48d63d64e734f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1457; amd64

### `nats-streaming:nanoserver-1809` - windows version 10.0.17763.1457; amd64

```console
$ docker pull nats-streaming@sha256:633ee41bf90856c425664d464d0bbde7c719a8d684aae2a4c4aa8c688b273c2f
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.2 MB (107186820 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:800961c202be6010a686406b705d7a401c822eb61b250ae466a82f207e1962cc`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Wed, 02 Sep 2020 12:08:18 GMT
RUN Apply image 1809-amd64
# Wed, 09 Sep 2020 17:12:30 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 09 Sep 2020 20:33:07 GMT
RUN cmd /S /C #(nop) COPY file:4a858ac4da943f868519572e3fb6817fd379875f2bff0bcb5f03c5bdddc496a8 in C:\nats-streaming-server.exe 
# Wed, 09 Sep 2020 20:33:09 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 09 Sep 2020 20:33:10 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 09 Sep 2020 20:33:10 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:ecf9bb62dc6eedea9fd367628f8715dea75b7d2053afa4b5121e7809aa692139`  
		Size: 101.2 MB (101239122 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a993e00682bb4be271d74c200e8e9d454b07999d7ab172f3b14fe72883380722`  
		Last Modified: Wed, 09 Sep 2020 17:16:30 GMT  
		Size: 929.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e73f351ef78c90a784ebe68be1d18a90b8d3d96b4bc34c7a0eef484d8c1dffa`  
		Last Modified: Wed, 09 Sep 2020 20:37:08 GMT  
		Size: 5.9 MB (5944140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b597a9018de11dec33432a01c58c1c8a0b34a109943149eea36418113bb3947d`  
		Last Modified: Wed, 09 Sep 2020 20:37:06 GMT  
		Size: 896.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aafa4807abd9e0fb29a3ea7b8de9201357fe0888234631d6f1b2d19586e85f2f`  
		Last Modified: Wed, 09 Sep 2020 20:37:06 GMT  
		Size: 869.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fd0e0805a30ff0bebf0e1377a6ee0c68cb6a8f23df9fba6c9443e9940ae24e9`  
		Last Modified: Wed, 09 Sep 2020 20:37:06 GMT  
		Size: 864.0 B  
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
$ docker pull nats-streaming@sha256:e8c22bffec8b2ced3d9bef1570fb45f1e168091ad1c5ac8ad284885876ec44d1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1457; amd64
	-	windows version 10.0.14393.3930; amd64

### `nats-streaming:windowsservercore` - windows version 10.0.17763.1457; amd64

```console
$ docker pull nats-streaming@sha256:c94cf73a46b625f0d88728e07a7d2f1f2d5449d2ca74f6aff19065231283599b
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2371111653 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ef12f072c15e6d5c505dec4022a33399d1b1eb10c10968261006daca91e4ce0`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 03 Sep 2020 05:59:01 GMT
RUN Install update 1809-amd64
# Wed, 09 Sep 2020 13:15:06 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Sep 2020 17:10:34 GMT
ENV NATS_DOCKERIZED=1
# Wed, 09 Sep 2020 20:31:10 GMT
ENV NATS_STREAMING_SERVER=0.18.0
# Wed, 09 Sep 2020 20:31:10 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.18.0/nats-streaming-server-v0.18.0-windows-amd64.zip
# Wed, 09 Sep 2020 20:31:11 GMT
ENV GIT_DOWNLOAD_SHA256=a0c0261df2ce589fe9706617323e06c5bcae70511112eae921681b1169674bc8
# Wed, 09 Sep 2020 20:31:40 GMT
RUN Set-PSDebug -Trace 2
# Wed, 09 Sep 2020 20:32:54 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 09 Sep 2020 20:32:55 GMT
EXPOSE 4222 8222
# Wed, 09 Sep 2020 20:32:56 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 09 Sep 2020 20:32:57 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c3aff44502467b94164764856a6feb805fc5c79ff66012eebdd7da3f180e3138`  
		Size: 632.9 MB (632939341 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:1df31adcc7026c3bf0cb32832a3f307dd6e1e54b8b3e050f8a73b5caee674d88`  
		Last Modified: Wed, 09 Sep 2020 16:48:51 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a005485001c0802bc2ee93661375bfb4c868e16c3f5678debf00f29a8bb26386`  
		Last Modified: Wed, 09 Sep 2020 17:16:08 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8694028d86dd4c393914d2d297dd6869064d3eebb0e37f4fbf118b0220e54462`  
		Last Modified: Wed, 09 Sep 2020 20:36:51 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13620d5ec186fd18ae4469cf269f141b543dcf10f69a6f3b154054b096394a12`  
		Last Modified: Wed, 09 Sep 2020 20:36:51 GMT  
		Size: 1.1 KB (1140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:085e5f4e037f4da34b0d4adb9c9895fb6d02e3e157acb4adc891fa27cef8d3bb`  
		Last Modified: Wed, 09 Sep 2020 20:36:51 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0321f95de34d68601a758a932a003b5e3cf6e0e45077ee0b524100c7d08a381f`  
		Last Modified: Wed, 09 Sep 2020 20:36:50 GMT  
		Size: 4.8 MB (4784319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa831bb560296cb990cd36699b5efa30aa0537885f70827a16d14db6c9777901`  
		Last Modified: Wed, 09 Sep 2020 20:36:52 GMT  
		Size: 15.0 MB (15045992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2cd5f57708b2d773c1ece864eab14ba8a4c9a8ed13882e5aeeda9cb66ec0586`  
		Last Modified: Wed, 09 Sep 2020 20:36:48 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c35decd3f52c0519150414ac9c188b632ca4fb591eb4adca28d95b5bf12b9fa0`  
		Last Modified: Wed, 09 Sep 2020 20:36:49 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97f0407c16bfc68dbc3501cf3e406dc1a256a093ed77043eec98317f272e0017`  
		Last Modified: Wed, 09 Sep 2020 20:36:48 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:windowsservercore` - windows version 10.0.14393.3930; amd64

```console
$ docker pull nats-streaming@sha256:981ef599a734b64a66cac4f2d5cba055451854d765898f9993fec7811ca1c394
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5760484146 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86d2337b5310038c6b37fadf4c91e7e441252a28e8a77576f9140384a4f4672f`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 01 Sep 2020 19:14:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 09 Sep 2020 13:23:04 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Sep 2020 17:12:41 GMT
ENV NATS_DOCKERIZED=1
# Wed, 09 Sep 2020 20:33:15 GMT
ENV NATS_STREAMING_SERVER=0.18.0
# Wed, 09 Sep 2020 20:33:16 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.18.0/nats-streaming-server-v0.18.0-windows-amd64.zip
# Wed, 09 Sep 2020 20:33:16 GMT
ENV GIT_DOWNLOAD_SHA256=a0c0261df2ce589fe9706617323e06c5bcae70511112eae921681b1169674bc8
# Wed, 09 Sep 2020 20:34:26 GMT
RUN Set-PSDebug -Trace 2
# Wed, 09 Sep 2020 20:36:11 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 09 Sep 2020 20:36:11 GMT
EXPOSE 4222 8222
# Wed, 09 Sep 2020 20:36:12 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 09 Sep 2020 20:36:14 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bc202b498d589027cc702b23cf959b8842907508b3465b9d6ff739c9668e5134`  
		Size: 1.7 GB (1669268544 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c1d56eeebea105bba2dd1879a89adb012f98cf42708c0f36ca4af683db7162a2`  
		Last Modified: Wed, 09 Sep 2020 16:49:22 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae4d96d0f21f7d823b426589ab2a404cd548354f8d03ceb98ed43812aa4ea498`  
		Last Modified: Wed, 09 Sep 2020 17:16:52 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd2d7de21675e6a7b359d125e71a443d18e04e40860dec675c44d37c7361ed62`  
		Last Modified: Wed, 09 Sep 2020 20:37:23 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae08ee6b7fee5f9fffc78e4c7f2f4c89dcbf18422a72fbe3a79bafdf7bd44640`  
		Last Modified: Wed, 09 Sep 2020 20:37:23 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80ebec154bb3a413d80d85884bf30c098fdc5ca1bb89bed4101a5a8461ff6301`  
		Last Modified: Wed, 09 Sep 2020 20:37:23 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a4c2d3b77c41d8255a747b40d4ca2979be47b74ed08ce2599a2995eef1b613b`  
		Last Modified: Wed, 09 Sep 2020 20:37:22 GMT  
		Size: 5.4 MB (5378060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ca76e108efd6235186de526ff5505988de6cff23592026dd8760d11aeea5bdd`  
		Last Modified: Wed, 09 Sep 2020 20:37:38 GMT  
		Size: 15.8 MB (15842566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdcd8c348d7e661add432378d1a17026e0ca4b65a205cb77cc3b9df060dc0cdf`  
		Last Modified: Wed, 09 Sep 2020 20:37:20 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c55596ce0711ce624d77dfd64a752d31630a12a964365db81412beabdf0ae0ea`  
		Last Modified: Wed, 09 Sep 2020 20:37:20 GMT  
		Size: 1.1 KB (1140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3b82f600ad3dd8623c8638a813ae0eb243b2a9f9c0fa6f3a8b3b3d9bd5b47db`  
		Last Modified: Wed, 09 Sep 2020 20:37:21 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:windowsservercore-1809`

```console
$ docker pull nats-streaming@sha256:31da8c5a6f0efbee7be5dac0e9851ab6d38d6548d1c2521d6b22b17554ac7660
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1457; amd64

### `nats-streaming:windowsservercore-1809` - windows version 10.0.17763.1457; amd64

```console
$ docker pull nats-streaming@sha256:c94cf73a46b625f0d88728e07a7d2f1f2d5449d2ca74f6aff19065231283599b
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2371111653 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ef12f072c15e6d5c505dec4022a33399d1b1eb10c10968261006daca91e4ce0`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 03 Sep 2020 05:59:01 GMT
RUN Install update 1809-amd64
# Wed, 09 Sep 2020 13:15:06 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Sep 2020 17:10:34 GMT
ENV NATS_DOCKERIZED=1
# Wed, 09 Sep 2020 20:31:10 GMT
ENV NATS_STREAMING_SERVER=0.18.0
# Wed, 09 Sep 2020 20:31:10 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.18.0/nats-streaming-server-v0.18.0-windows-amd64.zip
# Wed, 09 Sep 2020 20:31:11 GMT
ENV GIT_DOWNLOAD_SHA256=a0c0261df2ce589fe9706617323e06c5bcae70511112eae921681b1169674bc8
# Wed, 09 Sep 2020 20:31:40 GMT
RUN Set-PSDebug -Trace 2
# Wed, 09 Sep 2020 20:32:54 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 09 Sep 2020 20:32:55 GMT
EXPOSE 4222 8222
# Wed, 09 Sep 2020 20:32:56 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 09 Sep 2020 20:32:57 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c3aff44502467b94164764856a6feb805fc5c79ff66012eebdd7da3f180e3138`  
		Size: 632.9 MB (632939341 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:1df31adcc7026c3bf0cb32832a3f307dd6e1e54b8b3e050f8a73b5caee674d88`  
		Last Modified: Wed, 09 Sep 2020 16:48:51 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a005485001c0802bc2ee93661375bfb4c868e16c3f5678debf00f29a8bb26386`  
		Last Modified: Wed, 09 Sep 2020 17:16:08 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8694028d86dd4c393914d2d297dd6869064d3eebb0e37f4fbf118b0220e54462`  
		Last Modified: Wed, 09 Sep 2020 20:36:51 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13620d5ec186fd18ae4469cf269f141b543dcf10f69a6f3b154054b096394a12`  
		Last Modified: Wed, 09 Sep 2020 20:36:51 GMT  
		Size: 1.1 KB (1140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:085e5f4e037f4da34b0d4adb9c9895fb6d02e3e157acb4adc891fa27cef8d3bb`  
		Last Modified: Wed, 09 Sep 2020 20:36:51 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0321f95de34d68601a758a932a003b5e3cf6e0e45077ee0b524100c7d08a381f`  
		Last Modified: Wed, 09 Sep 2020 20:36:50 GMT  
		Size: 4.8 MB (4784319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa831bb560296cb990cd36699b5efa30aa0537885f70827a16d14db6c9777901`  
		Last Modified: Wed, 09 Sep 2020 20:36:52 GMT  
		Size: 15.0 MB (15045992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2cd5f57708b2d773c1ece864eab14ba8a4c9a8ed13882e5aeeda9cb66ec0586`  
		Last Modified: Wed, 09 Sep 2020 20:36:48 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c35decd3f52c0519150414ac9c188b632ca4fb591eb4adca28d95b5bf12b9fa0`  
		Last Modified: Wed, 09 Sep 2020 20:36:49 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97f0407c16bfc68dbc3501cf3e406dc1a256a093ed77043eec98317f272e0017`  
		Last Modified: Wed, 09 Sep 2020 20:36:48 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:windowsservercore-ltsc2016`

```console
$ docker pull nats-streaming@sha256:702f25fac8d3eff9cf2716c95681b464c2d7e7c6a741a1e3e7df31177ff08cc8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3930; amd64

### `nats-streaming:windowsservercore-ltsc2016` - windows version 10.0.14393.3930; amd64

```console
$ docker pull nats-streaming@sha256:981ef599a734b64a66cac4f2d5cba055451854d765898f9993fec7811ca1c394
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5760484146 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86d2337b5310038c6b37fadf4c91e7e441252a28e8a77576f9140384a4f4672f`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 01 Sep 2020 19:14:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 09 Sep 2020 13:23:04 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Sep 2020 17:12:41 GMT
ENV NATS_DOCKERIZED=1
# Wed, 09 Sep 2020 20:33:15 GMT
ENV NATS_STREAMING_SERVER=0.18.0
# Wed, 09 Sep 2020 20:33:16 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.18.0/nats-streaming-server-v0.18.0-windows-amd64.zip
# Wed, 09 Sep 2020 20:33:16 GMT
ENV GIT_DOWNLOAD_SHA256=a0c0261df2ce589fe9706617323e06c5bcae70511112eae921681b1169674bc8
# Wed, 09 Sep 2020 20:34:26 GMT
RUN Set-PSDebug -Trace 2
# Wed, 09 Sep 2020 20:36:11 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 09 Sep 2020 20:36:11 GMT
EXPOSE 4222 8222
# Wed, 09 Sep 2020 20:36:12 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 09 Sep 2020 20:36:14 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bc202b498d589027cc702b23cf959b8842907508b3465b9d6ff739c9668e5134`  
		Size: 1.7 GB (1669268544 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c1d56eeebea105bba2dd1879a89adb012f98cf42708c0f36ca4af683db7162a2`  
		Last Modified: Wed, 09 Sep 2020 16:49:22 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae4d96d0f21f7d823b426589ab2a404cd548354f8d03ceb98ed43812aa4ea498`  
		Last Modified: Wed, 09 Sep 2020 17:16:52 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd2d7de21675e6a7b359d125e71a443d18e04e40860dec675c44d37c7361ed62`  
		Last Modified: Wed, 09 Sep 2020 20:37:23 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae08ee6b7fee5f9fffc78e4c7f2f4c89dcbf18422a72fbe3a79bafdf7bd44640`  
		Last Modified: Wed, 09 Sep 2020 20:37:23 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80ebec154bb3a413d80d85884bf30c098fdc5ca1bb89bed4101a5a8461ff6301`  
		Last Modified: Wed, 09 Sep 2020 20:37:23 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a4c2d3b77c41d8255a747b40d4ca2979be47b74ed08ce2599a2995eef1b613b`  
		Last Modified: Wed, 09 Sep 2020 20:37:22 GMT  
		Size: 5.4 MB (5378060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ca76e108efd6235186de526ff5505988de6cff23592026dd8760d11aeea5bdd`  
		Last Modified: Wed, 09 Sep 2020 20:37:38 GMT  
		Size: 15.8 MB (15842566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdcd8c348d7e661add432378d1a17026e0ca4b65a205cb77cc3b9df060dc0cdf`  
		Last Modified: Wed, 09 Sep 2020 20:37:20 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c55596ce0711ce624d77dfd64a752d31630a12a964365db81412beabdf0ae0ea`  
		Last Modified: Wed, 09 Sep 2020 20:37:20 GMT  
		Size: 1.1 KB (1140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3b82f600ad3dd8623c8638a813ae0eb243b2a9f9c0fa6f3a8b3b3d9bd5b47db`  
		Last Modified: Wed, 09 Sep 2020 20:37:21 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
