<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `nats-streaming`

-	[`nats-streaming:0.20`](#nats-streaming020)
-	[`nats-streaming:0.20.0`](#nats-streaming0200)
-	[`nats-streaming:0.20.0-alpine`](#nats-streaming0200-alpine)
-	[`nats-streaming:0.20.0-alpine3.12`](#nats-streaming0200-alpine312)
-	[`nats-streaming:0.20.0-linux`](#nats-streaming0200-linux)
-	[`nats-streaming:0.20.0-nanoserver`](#nats-streaming0200-nanoserver)
-	[`nats-streaming:0.20.0-nanoserver-1809`](#nats-streaming0200-nanoserver-1809)
-	[`nats-streaming:0.20.0-scratch`](#nats-streaming0200-scratch)
-	[`nats-streaming:0.20.0-windowsservercore`](#nats-streaming0200-windowsservercore)
-	[`nats-streaming:0.20.0-windowsservercore-1809`](#nats-streaming0200-windowsservercore-1809)
-	[`nats-streaming:0.20.0-windowsservercore-ltsc2016`](#nats-streaming0200-windowsservercore-ltsc2016)
-	[`nats-streaming:0.20-alpine`](#nats-streaming020-alpine)
-	[`nats-streaming:0.20-alpine3.12`](#nats-streaming020-alpine312)
-	[`nats-streaming:0.20-linux`](#nats-streaming020-linux)
-	[`nats-streaming:0.20-nanoserver`](#nats-streaming020-nanoserver)
-	[`nats-streaming:0.20-nanoserver-1809`](#nats-streaming020-nanoserver-1809)
-	[`nats-streaming:0.20-scratch`](#nats-streaming020-scratch)
-	[`nats-streaming:0.20-windowsservercore`](#nats-streaming020-windowsservercore)
-	[`nats-streaming:0.20-windowsservercore-1809`](#nats-streaming020-windowsservercore-1809)
-	[`nats-streaming:0.20-windowsservercore-ltsc2016`](#nats-streaming020-windowsservercore-ltsc2016)
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

## `nats-streaming:0.20`

```console
$ docker pull nats-streaming@sha256:83e5a79191091b9dfcacc7305ade7103ae29b443f06a973104196aea8b7fb931
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.1757; amd64

### `nats-streaming:0.20` - linux; amd64

```console
$ docker pull nats-streaming@sha256:cd0162a7232de1eabe982554c8740e7edbac4747af3e99fa9bc38a480b4a4243
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 MB (5914730 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1544c1524919e1458186fefae5f5ff415c37055742e531010fc2660b11db2339`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 12 Jan 2021 00:48:24 GMT
COPY file:acbca3cec2dc5172f21984b614cbcd90e6e4cf0bd9848c5ddcffb94615a02436 in /nats-streaming-server 
# Tue, 12 Jan 2021 00:48:24 GMT
EXPOSE 4222 8222
# Tue, 12 Jan 2021 00:48:24 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 12 Jan 2021 00:48:24 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:0d51fde6ce3492f397e8a85dad354a9a45ab91310cf4abd6275101f3ef823587`  
		Last Modified: Tue, 12 Jan 2021 00:49:07 GMT  
		Size: 5.9 MB (5914730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.20` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:bbb3d771f9232932017b9cb9b501734367bc3560eed790695be682d94a8f3573
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.4 MB (5444243 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ed880c2955fd126b0ce38471e90c9467c9c739f55b4c789cec1a4575a41d36f`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 11 Jan 2021 23:53:53 GMT
COPY file:617b9b5366d0d437ce471ad0763bdd7d350496612583dc2c7044dcde4d32257e in /nats-streaming-server 
# Mon, 11 Jan 2021 23:53:54 GMT
EXPOSE 4222 8222
# Mon, 11 Jan 2021 23:53:54 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 11 Jan 2021 23:53:55 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:7cffcff2c5b4913dac660d7456365492a0393b1aa6f1812f6b7b46b250e1970d`  
		Last Modified: Mon, 11 Jan 2021 23:54:39 GMT  
		Size: 5.4 MB (5444243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.20` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:b2d9250f9a4e3b25b2212f4e8c27c693cc5cfa0f83ca82a8005c90ae8372ab86
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.4 MB (5439328 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:35f1d3c5a1d429a3e2b1fc71f5bc023980c41d34ccb0a0482aca07b6cbb4d6f1`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 12 Jan 2021 00:19:09 GMT
COPY file:2b3fc04f11d3cc7cdfa09f93a79d8efe0889d24324b831fb35126470165c9027 in /nats-streaming-server 
# Tue, 12 Jan 2021 00:19:14 GMT
EXPOSE 4222 8222
# Tue, 12 Jan 2021 00:19:16 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 12 Jan 2021 00:19:17 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:bf50122b11c4b5e2fa295a9456a93489ad25dd1e9bfefda1d572da1a57418205`  
		Last Modified: Tue, 12 Jan 2021 00:20:01 GMT  
		Size: 5.4 MB (5439328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.20` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:0f315491d4d14e634f971591c7f8bd0eb9aad59975fcdf867a51294df2e5efb2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.4 MB (5388538 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:22dba974517468c29a982c1b4a0b7744a93825122145a1dcc5f7e53c96119efa`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 11 Jan 2021 23:47:25 GMT
COPY file:5a251d4e6bafc9d9ea6f25cd37fd44252da405176da94cc580cdd663abecffa5 in /nats-streaming-server 
# Mon, 11 Jan 2021 23:47:26 GMT
EXPOSE 4222 8222
# Mon, 11 Jan 2021 23:47:26 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 11 Jan 2021 23:47:27 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:58239a1ea6494e431645c7ad156ed917333a248edbe6be76af8b7384d9339f07`  
		Last Modified: Mon, 11 Jan 2021 23:48:09 GMT  
		Size: 5.4 MB (5388538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.20` - windows version 10.0.17763.1757; amd64

```console
$ docker pull nats-streaming@sha256:d13b43d591f725a510ae54f0f2efa114399a0a0c9e85f0652bc802e7e8d45187
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.4 MB (107432722 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc67b6d7f9c859b2a9e9272dfda84571744e233c3ada49fdd3505d40e586c859`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 02 Feb 2021 13:06:30 GMT
RUN Apply image 1809-amd64
# Wed, 10 Feb 2021 16:02:26 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 10 Feb 2021 20:00:55 GMT
RUN cmd /S /C #(nop) COPY file:f2450ffeda74e33f820191eccf78b6647ce56865170e966bfa8e72afe6e46c36 in C:\nats-streaming-server.exe 
# Wed, 10 Feb 2021 20:00:56 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 10 Feb 2021 20:00:57 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 10 Feb 2021 20:00:57 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:ba17af31b9276ee11fdf859681b442db50979a39eff4cea2a559a5755cedbe01`  
		Size: 101.4 MB (101406193 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:23b613036f8aee9066e712b3aa58f10f2fde093623511a5658867f53a6d01b18`  
		Last Modified: Wed, 10 Feb 2021 16:06:34 GMT  
		Size: 1.1 KB (1071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:546c4d75ec4cbc867ea01774757b0a9303906569a30157fd804f8c1bc5d4e63e`  
		Last Modified: Wed, 10 Feb 2021 20:06:15 GMT  
		Size: 6.0 MB (6022164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d942fdcd6082f7ac407761ffc6d739677d6fe08f0f51db38d32d33398e9073f`  
		Last Modified: Wed, 10 Feb 2021 20:06:07 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2c29c3e2255d5f0292ecd161299cb57afc896ff1c7002836b53577f1d57e6fe`  
		Last Modified: Wed, 10 Feb 2021 20:06:07 GMT  
		Size: 1.1 KB (1097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12923e759dcf1b0d858f5bfacd7f73cffa442500803639aa349428d981cd881f`  
		Last Modified: Wed, 10 Feb 2021 20:06:07 GMT  
		Size: 1.1 KB (1072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.20.0`

```console
$ docker pull nats-streaming@sha256:83e5a79191091b9dfcacc7305ade7103ae29b443f06a973104196aea8b7fb931
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.1757; amd64

### `nats-streaming:0.20.0` - linux; amd64

```console
$ docker pull nats-streaming@sha256:cd0162a7232de1eabe982554c8740e7edbac4747af3e99fa9bc38a480b4a4243
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 MB (5914730 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1544c1524919e1458186fefae5f5ff415c37055742e531010fc2660b11db2339`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 12 Jan 2021 00:48:24 GMT
COPY file:acbca3cec2dc5172f21984b614cbcd90e6e4cf0bd9848c5ddcffb94615a02436 in /nats-streaming-server 
# Tue, 12 Jan 2021 00:48:24 GMT
EXPOSE 4222 8222
# Tue, 12 Jan 2021 00:48:24 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 12 Jan 2021 00:48:24 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:0d51fde6ce3492f397e8a85dad354a9a45ab91310cf4abd6275101f3ef823587`  
		Last Modified: Tue, 12 Jan 2021 00:49:07 GMT  
		Size: 5.9 MB (5914730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.20.0` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:bbb3d771f9232932017b9cb9b501734367bc3560eed790695be682d94a8f3573
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.4 MB (5444243 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ed880c2955fd126b0ce38471e90c9467c9c739f55b4c789cec1a4575a41d36f`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 11 Jan 2021 23:53:53 GMT
COPY file:617b9b5366d0d437ce471ad0763bdd7d350496612583dc2c7044dcde4d32257e in /nats-streaming-server 
# Mon, 11 Jan 2021 23:53:54 GMT
EXPOSE 4222 8222
# Mon, 11 Jan 2021 23:53:54 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 11 Jan 2021 23:53:55 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:7cffcff2c5b4913dac660d7456365492a0393b1aa6f1812f6b7b46b250e1970d`  
		Last Modified: Mon, 11 Jan 2021 23:54:39 GMT  
		Size: 5.4 MB (5444243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.20.0` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:b2d9250f9a4e3b25b2212f4e8c27c693cc5cfa0f83ca82a8005c90ae8372ab86
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.4 MB (5439328 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:35f1d3c5a1d429a3e2b1fc71f5bc023980c41d34ccb0a0482aca07b6cbb4d6f1`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 12 Jan 2021 00:19:09 GMT
COPY file:2b3fc04f11d3cc7cdfa09f93a79d8efe0889d24324b831fb35126470165c9027 in /nats-streaming-server 
# Tue, 12 Jan 2021 00:19:14 GMT
EXPOSE 4222 8222
# Tue, 12 Jan 2021 00:19:16 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 12 Jan 2021 00:19:17 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:bf50122b11c4b5e2fa295a9456a93489ad25dd1e9bfefda1d572da1a57418205`  
		Last Modified: Tue, 12 Jan 2021 00:20:01 GMT  
		Size: 5.4 MB (5439328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.20.0` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:0f315491d4d14e634f971591c7f8bd0eb9aad59975fcdf867a51294df2e5efb2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.4 MB (5388538 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:22dba974517468c29a982c1b4a0b7744a93825122145a1dcc5f7e53c96119efa`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 11 Jan 2021 23:47:25 GMT
COPY file:5a251d4e6bafc9d9ea6f25cd37fd44252da405176da94cc580cdd663abecffa5 in /nats-streaming-server 
# Mon, 11 Jan 2021 23:47:26 GMT
EXPOSE 4222 8222
# Mon, 11 Jan 2021 23:47:26 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 11 Jan 2021 23:47:27 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:58239a1ea6494e431645c7ad156ed917333a248edbe6be76af8b7384d9339f07`  
		Last Modified: Mon, 11 Jan 2021 23:48:09 GMT  
		Size: 5.4 MB (5388538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.20.0` - windows version 10.0.17763.1757; amd64

```console
$ docker pull nats-streaming@sha256:d13b43d591f725a510ae54f0f2efa114399a0a0c9e85f0652bc802e7e8d45187
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.4 MB (107432722 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc67b6d7f9c859b2a9e9272dfda84571744e233c3ada49fdd3505d40e586c859`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 02 Feb 2021 13:06:30 GMT
RUN Apply image 1809-amd64
# Wed, 10 Feb 2021 16:02:26 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 10 Feb 2021 20:00:55 GMT
RUN cmd /S /C #(nop) COPY file:f2450ffeda74e33f820191eccf78b6647ce56865170e966bfa8e72afe6e46c36 in C:\nats-streaming-server.exe 
# Wed, 10 Feb 2021 20:00:56 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 10 Feb 2021 20:00:57 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 10 Feb 2021 20:00:57 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:ba17af31b9276ee11fdf859681b442db50979a39eff4cea2a559a5755cedbe01`  
		Size: 101.4 MB (101406193 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:23b613036f8aee9066e712b3aa58f10f2fde093623511a5658867f53a6d01b18`  
		Last Modified: Wed, 10 Feb 2021 16:06:34 GMT  
		Size: 1.1 KB (1071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:546c4d75ec4cbc867ea01774757b0a9303906569a30157fd804f8c1bc5d4e63e`  
		Last Modified: Wed, 10 Feb 2021 20:06:15 GMT  
		Size: 6.0 MB (6022164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d942fdcd6082f7ac407761ffc6d739677d6fe08f0f51db38d32d33398e9073f`  
		Last Modified: Wed, 10 Feb 2021 20:06:07 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2c29c3e2255d5f0292ecd161299cb57afc896ff1c7002836b53577f1d57e6fe`  
		Last Modified: Wed, 10 Feb 2021 20:06:07 GMT  
		Size: 1.1 KB (1097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12923e759dcf1b0d858f5bfacd7f73cffa442500803639aa349428d981cd881f`  
		Last Modified: Wed, 10 Feb 2021 20:06:07 GMT  
		Size: 1.1 KB (1072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.20.0-alpine`

```console
$ docker pull nats-streaming@sha256:3e79d8fb911870f1333bc6bfed2fcd3af9e3090434a40d85c5b2747ad2b33ece
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.20.0-alpine` - linux; amd64

```console
$ docker pull nats-streaming@sha256:7e2837da130ab6208e927ba254dd3e66cf3e51c232bff758fdcd6f177e8e4cba
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.0 MB (8997694 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df0e4bfed7e10f0725503851ba4a32fa19cc88f189c2a7bc34d4348b5083e184`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 24 Feb 2021 20:20:03 GMT
ADD file:0dbb1cd66f708f54f7e6663eabf24095fcd53747bfb09912a118a77e737d9617 in / 
# Wed, 24 Feb 2021 20:20:03 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 21:16:41 GMT
ENV NATS_STREAMING_SERVER=0.20.0
# Wed, 24 Feb 2021 21:16:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='618008a4902916b6bdb26022343ab91313d4f7fc90b31d0c71ad9e75dc8299e4' ;; 		armhf) natsArch='arm6'; sha256='144b04f8f42793aee1b2deb3f6eb187648c37dcc32d526c607a0af99a847260d' ;; 		armv7) natsArch='arm7'; sha256='720f4a90d1dd536bc04639ae31c70ab46fb3e10556f0f261eb038fdce941f20c' ;; 		x86_64) natsArch='amd64'; sha256='098e2293cce5d457b92f3df35127789422562f1414427c406ffd03ea3bd687c9' ;; 		x86) natsArch='386'; sha256='322a290f4706f14d6ff8160ec437202bd282f61f0607741d0e4c38ef89b83451' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 24 Feb 2021 21:16:44 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Wed, 24 Feb 2021 21:16:44 GMT
EXPOSE 4222 8222
# Wed, 24 Feb 2021 21:16:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 24 Feb 2021 21:16:45 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:f84cab65f19f5d625a4b5f895cdf37ad9f21e160bf201ec59a48d95b2a430145`  
		Last Modified: Wed, 24 Feb 2021 20:20:39 GMT  
		Size: 2.8 MB (2799493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32044508a232eda00968bedd206428d2540ce9b818a3382269486238d731550c`  
		Last Modified: Wed, 24 Feb 2021 21:17:24 GMT  
		Size: 6.2 MB (6197781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ebefc07ccecb4605491ec038d76ed03335e0a0b0e033be052987c817d713cc0`  
		Last Modified: Wed, 24 Feb 2021 21:17:23 GMT  
		Size: 420.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.20.0-alpine` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:71a3dda1dc2ddabf1f7d58456851bb20b66a176c7df12844dd00777365754351
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.3 MB (8331130 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:481fb1c587fe44cb52065c781076c4d64bbe18c9d2856305f951d92d3d564c67`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 24 Feb 2021 20:50:34 GMT
ADD file:8bbb59eeaad0cbcf11559bc6e2b4492aadf6822d1935ed50c710f8bed858b7b5 in / 
# Wed, 24 Feb 2021 20:50:35 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 21:35:57 GMT
ENV NATS_STREAMING_SERVER=0.20.0
# Wed, 24 Feb 2021 21:36:02 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='618008a4902916b6bdb26022343ab91313d4f7fc90b31d0c71ad9e75dc8299e4' ;; 		armhf) natsArch='arm6'; sha256='144b04f8f42793aee1b2deb3f6eb187648c37dcc32d526c607a0af99a847260d' ;; 		armv7) natsArch='arm7'; sha256='720f4a90d1dd536bc04639ae31c70ab46fb3e10556f0f261eb038fdce941f20c' ;; 		x86_64) natsArch='amd64'; sha256='098e2293cce5d457b92f3df35127789422562f1414427c406ffd03ea3bd687c9' ;; 		x86) natsArch='386'; sha256='322a290f4706f14d6ff8160ec437202bd282f61f0607741d0e4c38ef89b83451' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 24 Feb 2021 21:36:03 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Wed, 24 Feb 2021 21:36:04 GMT
EXPOSE 4222 8222
# Wed, 24 Feb 2021 21:36:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 24 Feb 2021 21:36:05 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:55242616b0494f68f44470d864da746cd2a8f8f2d1ffca698114de64032247ef`  
		Last Modified: Wed, 24 Feb 2021 20:51:17 GMT  
		Size: 2.6 MB (2604518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cdc5b3ef2d08f12a32b4290648ce4ccaf53c62b831c0035a86f5f7934af51c5`  
		Last Modified: Wed, 24 Feb 2021 21:36:38 GMT  
		Size: 5.7 MB (5726190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:300ae63bdaa97a87286e7cd46df7562ee6d65fc79d1c59789b077a6efc5a04aa`  
		Last Modified: Wed, 24 Feb 2021 21:36:34 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.20.0-alpine` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:5ade3cc881349db3662cc2a32166b001c22214e0c79c0f2f99d0cb785f78cdab
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.1 MB (8125937 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3003c551e23e6c957b25e7c9db011e1cd8170bb14193c185bad20b6f639047f2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 24 Feb 2021 21:03:35 GMT
ADD file:2632f48dd643f8927da2b1af8365b3edb484bd6b7d9fee4009e69f6cf3310e91 in / 
# Wed, 24 Feb 2021 21:03:36 GMT
CMD ["/bin/sh"]
# Thu, 25 Feb 2021 02:03:00 GMT
ENV NATS_STREAMING_SERVER=0.20.0
# Thu, 25 Feb 2021 02:03:07 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='618008a4902916b6bdb26022343ab91313d4f7fc90b31d0c71ad9e75dc8299e4' ;; 		armhf) natsArch='arm6'; sha256='144b04f8f42793aee1b2deb3f6eb187648c37dcc32d526c607a0af99a847260d' ;; 		armv7) natsArch='arm7'; sha256='720f4a90d1dd536bc04639ae31c70ab46fb3e10556f0f261eb038fdce941f20c' ;; 		x86_64) natsArch='amd64'; sha256='098e2293cce5d457b92f3df35127789422562f1414427c406ffd03ea3bd687c9' ;; 		x86) natsArch='386'; sha256='322a290f4706f14d6ff8160ec437202bd282f61f0607741d0e4c38ef89b83451' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 25 Feb 2021 02:03:09 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Thu, 25 Feb 2021 02:03:10 GMT
EXPOSE 4222 8222
# Thu, 25 Feb 2021 02:03:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 25 Feb 2021 02:03:13 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:8e85c7428c31ea48b47424ca0e4663106c54591c83545d32b66a77093f90ffd0`  
		Last Modified: Wed, 24 Feb 2021 21:04:23 GMT  
		Size: 2.4 MB (2408004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e73e11681aeadb2d31fa3245a2d356980142a629503b54745e3dac74b4c6ccb`  
		Last Modified: Thu, 25 Feb 2021 02:04:13 GMT  
		Size: 5.7 MB (5717512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a07ffd0ec2224fc48e7d5a98c442b6a4a4b46730ed88e95871d2d6397f4c9d8`  
		Last Modified: Thu, 25 Feb 2021 02:04:06 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.20.0-alpine` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:bd39a673070144b75764fb3a0aad84cdbe8a7c16c9393b294da3d7bdddc223f9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.4 MB (8378716 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:72a01c0cbdeefc26cfc81137d93311ff33253f7d914cd42ffacbcd45725a4ab1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 24 Feb 2021 20:39:39 GMT
ADD file:7e82858ef85f6db90c131ed835a390d736cfdbd1a0cf8bccaeed8f7e30172ddb in / 
# Wed, 24 Feb 2021 20:39:40 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 23:54:22 GMT
ENV NATS_STREAMING_SERVER=0.20.0
# Wed, 24 Feb 2021 23:54:26 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='618008a4902916b6bdb26022343ab91313d4f7fc90b31d0c71ad9e75dc8299e4' ;; 		armhf) natsArch='arm6'; sha256='144b04f8f42793aee1b2deb3f6eb187648c37dcc32d526c607a0af99a847260d' ;; 		armv7) natsArch='arm7'; sha256='720f4a90d1dd536bc04639ae31c70ab46fb3e10556f0f261eb038fdce941f20c' ;; 		x86_64) natsArch='amd64'; sha256='098e2293cce5d457b92f3df35127789422562f1414427c406ffd03ea3bd687c9' ;; 		x86) natsArch='386'; sha256='322a290f4706f14d6ff8160ec437202bd282f61f0607741d0e4c38ef89b83451' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 24 Feb 2021 23:54:27 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Wed, 24 Feb 2021 23:54:28 GMT
EXPOSE 4222 8222
# Wed, 24 Feb 2021 23:54:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 24 Feb 2021 23:54:29 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:dce8679b510e95d136241d02ababff86469dd14220812a7ce9202833c0e32f66`  
		Last Modified: Wed, 24 Feb 2021 20:40:26 GMT  
		Size: 2.7 MB (2709880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64d185e50c4f0cdc2dc88a9f750ebea1210da17133d4339466bd454a3d2d3b5c`  
		Last Modified: Wed, 24 Feb 2021 23:55:03 GMT  
		Size: 5.7 MB (5668417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d70ce809390466c98565d0da9060e5d2d21974101f9ed8caf6bae1982e9cf71`  
		Last Modified: Wed, 24 Feb 2021 23:55:02 GMT  
		Size: 419.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.20.0-alpine3.12`

```console
$ docker pull nats-streaming@sha256:3e79d8fb911870f1333bc6bfed2fcd3af9e3090434a40d85c5b2747ad2b33ece
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.20.0-alpine3.12` - linux; amd64

```console
$ docker pull nats-streaming@sha256:7e2837da130ab6208e927ba254dd3e66cf3e51c232bff758fdcd6f177e8e4cba
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.0 MB (8997694 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df0e4bfed7e10f0725503851ba4a32fa19cc88f189c2a7bc34d4348b5083e184`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 24 Feb 2021 20:20:03 GMT
ADD file:0dbb1cd66f708f54f7e6663eabf24095fcd53747bfb09912a118a77e737d9617 in / 
# Wed, 24 Feb 2021 20:20:03 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 21:16:41 GMT
ENV NATS_STREAMING_SERVER=0.20.0
# Wed, 24 Feb 2021 21:16:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='618008a4902916b6bdb26022343ab91313d4f7fc90b31d0c71ad9e75dc8299e4' ;; 		armhf) natsArch='arm6'; sha256='144b04f8f42793aee1b2deb3f6eb187648c37dcc32d526c607a0af99a847260d' ;; 		armv7) natsArch='arm7'; sha256='720f4a90d1dd536bc04639ae31c70ab46fb3e10556f0f261eb038fdce941f20c' ;; 		x86_64) natsArch='amd64'; sha256='098e2293cce5d457b92f3df35127789422562f1414427c406ffd03ea3bd687c9' ;; 		x86) natsArch='386'; sha256='322a290f4706f14d6ff8160ec437202bd282f61f0607741d0e4c38ef89b83451' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 24 Feb 2021 21:16:44 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Wed, 24 Feb 2021 21:16:44 GMT
EXPOSE 4222 8222
# Wed, 24 Feb 2021 21:16:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 24 Feb 2021 21:16:45 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:f84cab65f19f5d625a4b5f895cdf37ad9f21e160bf201ec59a48d95b2a430145`  
		Last Modified: Wed, 24 Feb 2021 20:20:39 GMT  
		Size: 2.8 MB (2799493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32044508a232eda00968bedd206428d2540ce9b818a3382269486238d731550c`  
		Last Modified: Wed, 24 Feb 2021 21:17:24 GMT  
		Size: 6.2 MB (6197781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ebefc07ccecb4605491ec038d76ed03335e0a0b0e033be052987c817d713cc0`  
		Last Modified: Wed, 24 Feb 2021 21:17:23 GMT  
		Size: 420.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.20.0-alpine3.12` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:71a3dda1dc2ddabf1f7d58456851bb20b66a176c7df12844dd00777365754351
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.3 MB (8331130 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:481fb1c587fe44cb52065c781076c4d64bbe18c9d2856305f951d92d3d564c67`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 24 Feb 2021 20:50:34 GMT
ADD file:8bbb59eeaad0cbcf11559bc6e2b4492aadf6822d1935ed50c710f8bed858b7b5 in / 
# Wed, 24 Feb 2021 20:50:35 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 21:35:57 GMT
ENV NATS_STREAMING_SERVER=0.20.0
# Wed, 24 Feb 2021 21:36:02 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='618008a4902916b6bdb26022343ab91313d4f7fc90b31d0c71ad9e75dc8299e4' ;; 		armhf) natsArch='arm6'; sha256='144b04f8f42793aee1b2deb3f6eb187648c37dcc32d526c607a0af99a847260d' ;; 		armv7) natsArch='arm7'; sha256='720f4a90d1dd536bc04639ae31c70ab46fb3e10556f0f261eb038fdce941f20c' ;; 		x86_64) natsArch='amd64'; sha256='098e2293cce5d457b92f3df35127789422562f1414427c406ffd03ea3bd687c9' ;; 		x86) natsArch='386'; sha256='322a290f4706f14d6ff8160ec437202bd282f61f0607741d0e4c38ef89b83451' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 24 Feb 2021 21:36:03 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Wed, 24 Feb 2021 21:36:04 GMT
EXPOSE 4222 8222
# Wed, 24 Feb 2021 21:36:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 24 Feb 2021 21:36:05 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:55242616b0494f68f44470d864da746cd2a8f8f2d1ffca698114de64032247ef`  
		Last Modified: Wed, 24 Feb 2021 20:51:17 GMT  
		Size: 2.6 MB (2604518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cdc5b3ef2d08f12a32b4290648ce4ccaf53c62b831c0035a86f5f7934af51c5`  
		Last Modified: Wed, 24 Feb 2021 21:36:38 GMT  
		Size: 5.7 MB (5726190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:300ae63bdaa97a87286e7cd46df7562ee6d65fc79d1c59789b077a6efc5a04aa`  
		Last Modified: Wed, 24 Feb 2021 21:36:34 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.20.0-alpine3.12` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:5ade3cc881349db3662cc2a32166b001c22214e0c79c0f2f99d0cb785f78cdab
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.1 MB (8125937 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3003c551e23e6c957b25e7c9db011e1cd8170bb14193c185bad20b6f639047f2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 24 Feb 2021 21:03:35 GMT
ADD file:2632f48dd643f8927da2b1af8365b3edb484bd6b7d9fee4009e69f6cf3310e91 in / 
# Wed, 24 Feb 2021 21:03:36 GMT
CMD ["/bin/sh"]
# Thu, 25 Feb 2021 02:03:00 GMT
ENV NATS_STREAMING_SERVER=0.20.0
# Thu, 25 Feb 2021 02:03:07 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='618008a4902916b6bdb26022343ab91313d4f7fc90b31d0c71ad9e75dc8299e4' ;; 		armhf) natsArch='arm6'; sha256='144b04f8f42793aee1b2deb3f6eb187648c37dcc32d526c607a0af99a847260d' ;; 		armv7) natsArch='arm7'; sha256='720f4a90d1dd536bc04639ae31c70ab46fb3e10556f0f261eb038fdce941f20c' ;; 		x86_64) natsArch='amd64'; sha256='098e2293cce5d457b92f3df35127789422562f1414427c406ffd03ea3bd687c9' ;; 		x86) natsArch='386'; sha256='322a290f4706f14d6ff8160ec437202bd282f61f0607741d0e4c38ef89b83451' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 25 Feb 2021 02:03:09 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Thu, 25 Feb 2021 02:03:10 GMT
EXPOSE 4222 8222
# Thu, 25 Feb 2021 02:03:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 25 Feb 2021 02:03:13 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:8e85c7428c31ea48b47424ca0e4663106c54591c83545d32b66a77093f90ffd0`  
		Last Modified: Wed, 24 Feb 2021 21:04:23 GMT  
		Size: 2.4 MB (2408004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e73e11681aeadb2d31fa3245a2d356980142a629503b54745e3dac74b4c6ccb`  
		Last Modified: Thu, 25 Feb 2021 02:04:13 GMT  
		Size: 5.7 MB (5717512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a07ffd0ec2224fc48e7d5a98c442b6a4a4b46730ed88e95871d2d6397f4c9d8`  
		Last Modified: Thu, 25 Feb 2021 02:04:06 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.20.0-alpine3.12` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:bd39a673070144b75764fb3a0aad84cdbe8a7c16c9393b294da3d7bdddc223f9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.4 MB (8378716 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:72a01c0cbdeefc26cfc81137d93311ff33253f7d914cd42ffacbcd45725a4ab1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 24 Feb 2021 20:39:39 GMT
ADD file:7e82858ef85f6db90c131ed835a390d736cfdbd1a0cf8bccaeed8f7e30172ddb in / 
# Wed, 24 Feb 2021 20:39:40 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 23:54:22 GMT
ENV NATS_STREAMING_SERVER=0.20.0
# Wed, 24 Feb 2021 23:54:26 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='618008a4902916b6bdb26022343ab91313d4f7fc90b31d0c71ad9e75dc8299e4' ;; 		armhf) natsArch='arm6'; sha256='144b04f8f42793aee1b2deb3f6eb187648c37dcc32d526c607a0af99a847260d' ;; 		armv7) natsArch='arm7'; sha256='720f4a90d1dd536bc04639ae31c70ab46fb3e10556f0f261eb038fdce941f20c' ;; 		x86_64) natsArch='amd64'; sha256='098e2293cce5d457b92f3df35127789422562f1414427c406ffd03ea3bd687c9' ;; 		x86) natsArch='386'; sha256='322a290f4706f14d6ff8160ec437202bd282f61f0607741d0e4c38ef89b83451' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 24 Feb 2021 23:54:27 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Wed, 24 Feb 2021 23:54:28 GMT
EXPOSE 4222 8222
# Wed, 24 Feb 2021 23:54:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 24 Feb 2021 23:54:29 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:dce8679b510e95d136241d02ababff86469dd14220812a7ce9202833c0e32f66`  
		Last Modified: Wed, 24 Feb 2021 20:40:26 GMT  
		Size: 2.7 MB (2709880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64d185e50c4f0cdc2dc88a9f750ebea1210da17133d4339466bd454a3d2d3b5c`  
		Last Modified: Wed, 24 Feb 2021 23:55:03 GMT  
		Size: 5.7 MB (5668417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d70ce809390466c98565d0da9060e5d2d21974101f9ed8caf6bae1982e9cf71`  
		Last Modified: Wed, 24 Feb 2021 23:55:02 GMT  
		Size: 419.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.20.0-linux`

```console
$ docker pull nats-streaming@sha256:f46b63443b02bc0089e72301ae260b1ef32ff25e755e67b633169945585ca12d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.20.0-linux` - linux; amd64

```console
$ docker pull nats-streaming@sha256:cd0162a7232de1eabe982554c8740e7edbac4747af3e99fa9bc38a480b4a4243
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 MB (5914730 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1544c1524919e1458186fefae5f5ff415c37055742e531010fc2660b11db2339`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 12 Jan 2021 00:48:24 GMT
COPY file:acbca3cec2dc5172f21984b614cbcd90e6e4cf0bd9848c5ddcffb94615a02436 in /nats-streaming-server 
# Tue, 12 Jan 2021 00:48:24 GMT
EXPOSE 4222 8222
# Tue, 12 Jan 2021 00:48:24 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 12 Jan 2021 00:48:24 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:0d51fde6ce3492f397e8a85dad354a9a45ab91310cf4abd6275101f3ef823587`  
		Last Modified: Tue, 12 Jan 2021 00:49:07 GMT  
		Size: 5.9 MB (5914730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.20.0-linux` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:bbb3d771f9232932017b9cb9b501734367bc3560eed790695be682d94a8f3573
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.4 MB (5444243 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ed880c2955fd126b0ce38471e90c9467c9c739f55b4c789cec1a4575a41d36f`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 11 Jan 2021 23:53:53 GMT
COPY file:617b9b5366d0d437ce471ad0763bdd7d350496612583dc2c7044dcde4d32257e in /nats-streaming-server 
# Mon, 11 Jan 2021 23:53:54 GMT
EXPOSE 4222 8222
# Mon, 11 Jan 2021 23:53:54 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 11 Jan 2021 23:53:55 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:7cffcff2c5b4913dac660d7456365492a0393b1aa6f1812f6b7b46b250e1970d`  
		Last Modified: Mon, 11 Jan 2021 23:54:39 GMT  
		Size: 5.4 MB (5444243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.20.0-linux` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:b2d9250f9a4e3b25b2212f4e8c27c693cc5cfa0f83ca82a8005c90ae8372ab86
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.4 MB (5439328 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:35f1d3c5a1d429a3e2b1fc71f5bc023980c41d34ccb0a0482aca07b6cbb4d6f1`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 12 Jan 2021 00:19:09 GMT
COPY file:2b3fc04f11d3cc7cdfa09f93a79d8efe0889d24324b831fb35126470165c9027 in /nats-streaming-server 
# Tue, 12 Jan 2021 00:19:14 GMT
EXPOSE 4222 8222
# Tue, 12 Jan 2021 00:19:16 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 12 Jan 2021 00:19:17 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:bf50122b11c4b5e2fa295a9456a93489ad25dd1e9bfefda1d572da1a57418205`  
		Last Modified: Tue, 12 Jan 2021 00:20:01 GMT  
		Size: 5.4 MB (5439328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.20.0-linux` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:0f315491d4d14e634f971591c7f8bd0eb9aad59975fcdf867a51294df2e5efb2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.4 MB (5388538 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:22dba974517468c29a982c1b4a0b7744a93825122145a1dcc5f7e53c96119efa`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 11 Jan 2021 23:47:25 GMT
COPY file:5a251d4e6bafc9d9ea6f25cd37fd44252da405176da94cc580cdd663abecffa5 in /nats-streaming-server 
# Mon, 11 Jan 2021 23:47:26 GMT
EXPOSE 4222 8222
# Mon, 11 Jan 2021 23:47:26 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 11 Jan 2021 23:47:27 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:58239a1ea6494e431645c7ad156ed917333a248edbe6be76af8b7384d9339f07`  
		Last Modified: Mon, 11 Jan 2021 23:48:09 GMT  
		Size: 5.4 MB (5388538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.20.0-nanoserver`

```console
$ docker pull nats-streaming@sha256:b89cba5cf792b4be014bbb1be1a2fbca1c0019946c989c8a903c7ed865c0e7d8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1757; amd64

### `nats-streaming:0.20.0-nanoserver` - windows version 10.0.17763.1757; amd64

```console
$ docker pull nats-streaming@sha256:d13b43d591f725a510ae54f0f2efa114399a0a0c9e85f0652bc802e7e8d45187
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.4 MB (107432722 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc67b6d7f9c859b2a9e9272dfda84571744e233c3ada49fdd3505d40e586c859`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 02 Feb 2021 13:06:30 GMT
RUN Apply image 1809-amd64
# Wed, 10 Feb 2021 16:02:26 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 10 Feb 2021 20:00:55 GMT
RUN cmd /S /C #(nop) COPY file:f2450ffeda74e33f820191eccf78b6647ce56865170e966bfa8e72afe6e46c36 in C:\nats-streaming-server.exe 
# Wed, 10 Feb 2021 20:00:56 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 10 Feb 2021 20:00:57 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 10 Feb 2021 20:00:57 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:ba17af31b9276ee11fdf859681b442db50979a39eff4cea2a559a5755cedbe01`  
		Size: 101.4 MB (101406193 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:23b613036f8aee9066e712b3aa58f10f2fde093623511a5658867f53a6d01b18`  
		Last Modified: Wed, 10 Feb 2021 16:06:34 GMT  
		Size: 1.1 KB (1071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:546c4d75ec4cbc867ea01774757b0a9303906569a30157fd804f8c1bc5d4e63e`  
		Last Modified: Wed, 10 Feb 2021 20:06:15 GMT  
		Size: 6.0 MB (6022164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d942fdcd6082f7ac407761ffc6d739677d6fe08f0f51db38d32d33398e9073f`  
		Last Modified: Wed, 10 Feb 2021 20:06:07 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2c29c3e2255d5f0292ecd161299cb57afc896ff1c7002836b53577f1d57e6fe`  
		Last Modified: Wed, 10 Feb 2021 20:06:07 GMT  
		Size: 1.1 KB (1097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12923e759dcf1b0d858f5bfacd7f73cffa442500803639aa349428d981cd881f`  
		Last Modified: Wed, 10 Feb 2021 20:06:07 GMT  
		Size: 1.1 KB (1072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.20.0-nanoserver-1809`

```console
$ docker pull nats-streaming@sha256:b89cba5cf792b4be014bbb1be1a2fbca1c0019946c989c8a903c7ed865c0e7d8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1757; amd64

### `nats-streaming:0.20.0-nanoserver-1809` - windows version 10.0.17763.1757; amd64

```console
$ docker pull nats-streaming@sha256:d13b43d591f725a510ae54f0f2efa114399a0a0c9e85f0652bc802e7e8d45187
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.4 MB (107432722 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc67b6d7f9c859b2a9e9272dfda84571744e233c3ada49fdd3505d40e586c859`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 02 Feb 2021 13:06:30 GMT
RUN Apply image 1809-amd64
# Wed, 10 Feb 2021 16:02:26 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 10 Feb 2021 20:00:55 GMT
RUN cmd /S /C #(nop) COPY file:f2450ffeda74e33f820191eccf78b6647ce56865170e966bfa8e72afe6e46c36 in C:\nats-streaming-server.exe 
# Wed, 10 Feb 2021 20:00:56 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 10 Feb 2021 20:00:57 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 10 Feb 2021 20:00:57 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:ba17af31b9276ee11fdf859681b442db50979a39eff4cea2a559a5755cedbe01`  
		Size: 101.4 MB (101406193 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:23b613036f8aee9066e712b3aa58f10f2fde093623511a5658867f53a6d01b18`  
		Last Modified: Wed, 10 Feb 2021 16:06:34 GMT  
		Size: 1.1 KB (1071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:546c4d75ec4cbc867ea01774757b0a9303906569a30157fd804f8c1bc5d4e63e`  
		Last Modified: Wed, 10 Feb 2021 20:06:15 GMT  
		Size: 6.0 MB (6022164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d942fdcd6082f7ac407761ffc6d739677d6fe08f0f51db38d32d33398e9073f`  
		Last Modified: Wed, 10 Feb 2021 20:06:07 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2c29c3e2255d5f0292ecd161299cb57afc896ff1c7002836b53577f1d57e6fe`  
		Last Modified: Wed, 10 Feb 2021 20:06:07 GMT  
		Size: 1.1 KB (1097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12923e759dcf1b0d858f5bfacd7f73cffa442500803639aa349428d981cd881f`  
		Last Modified: Wed, 10 Feb 2021 20:06:07 GMT  
		Size: 1.1 KB (1072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.20.0-scratch`

```console
$ docker pull nats-streaming@sha256:f46b63443b02bc0089e72301ae260b1ef32ff25e755e67b633169945585ca12d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.20.0-scratch` - linux; amd64

```console
$ docker pull nats-streaming@sha256:cd0162a7232de1eabe982554c8740e7edbac4747af3e99fa9bc38a480b4a4243
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 MB (5914730 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1544c1524919e1458186fefae5f5ff415c37055742e531010fc2660b11db2339`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 12 Jan 2021 00:48:24 GMT
COPY file:acbca3cec2dc5172f21984b614cbcd90e6e4cf0bd9848c5ddcffb94615a02436 in /nats-streaming-server 
# Tue, 12 Jan 2021 00:48:24 GMT
EXPOSE 4222 8222
# Tue, 12 Jan 2021 00:48:24 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 12 Jan 2021 00:48:24 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:0d51fde6ce3492f397e8a85dad354a9a45ab91310cf4abd6275101f3ef823587`  
		Last Modified: Tue, 12 Jan 2021 00:49:07 GMT  
		Size: 5.9 MB (5914730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.20.0-scratch` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:bbb3d771f9232932017b9cb9b501734367bc3560eed790695be682d94a8f3573
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.4 MB (5444243 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ed880c2955fd126b0ce38471e90c9467c9c739f55b4c789cec1a4575a41d36f`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 11 Jan 2021 23:53:53 GMT
COPY file:617b9b5366d0d437ce471ad0763bdd7d350496612583dc2c7044dcde4d32257e in /nats-streaming-server 
# Mon, 11 Jan 2021 23:53:54 GMT
EXPOSE 4222 8222
# Mon, 11 Jan 2021 23:53:54 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 11 Jan 2021 23:53:55 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:7cffcff2c5b4913dac660d7456365492a0393b1aa6f1812f6b7b46b250e1970d`  
		Last Modified: Mon, 11 Jan 2021 23:54:39 GMT  
		Size: 5.4 MB (5444243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.20.0-scratch` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:b2d9250f9a4e3b25b2212f4e8c27c693cc5cfa0f83ca82a8005c90ae8372ab86
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.4 MB (5439328 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:35f1d3c5a1d429a3e2b1fc71f5bc023980c41d34ccb0a0482aca07b6cbb4d6f1`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 12 Jan 2021 00:19:09 GMT
COPY file:2b3fc04f11d3cc7cdfa09f93a79d8efe0889d24324b831fb35126470165c9027 in /nats-streaming-server 
# Tue, 12 Jan 2021 00:19:14 GMT
EXPOSE 4222 8222
# Tue, 12 Jan 2021 00:19:16 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 12 Jan 2021 00:19:17 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:bf50122b11c4b5e2fa295a9456a93489ad25dd1e9bfefda1d572da1a57418205`  
		Last Modified: Tue, 12 Jan 2021 00:20:01 GMT  
		Size: 5.4 MB (5439328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.20.0-scratch` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:0f315491d4d14e634f971591c7f8bd0eb9aad59975fcdf867a51294df2e5efb2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.4 MB (5388538 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:22dba974517468c29a982c1b4a0b7744a93825122145a1dcc5f7e53c96119efa`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 11 Jan 2021 23:47:25 GMT
COPY file:5a251d4e6bafc9d9ea6f25cd37fd44252da405176da94cc580cdd663abecffa5 in /nats-streaming-server 
# Mon, 11 Jan 2021 23:47:26 GMT
EXPOSE 4222 8222
# Mon, 11 Jan 2021 23:47:26 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 11 Jan 2021 23:47:27 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:58239a1ea6494e431645c7ad156ed917333a248edbe6be76af8b7384d9339f07`  
		Last Modified: Mon, 11 Jan 2021 23:48:09 GMT  
		Size: 5.4 MB (5388538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.20.0-windowsservercore`

```console
$ docker pull nats-streaming@sha256:f5c17fa3628e9e6d4f4a960b80c4f905b48409dc7f7227d9b2b53652d5e03311
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1757; amd64
	-	windows version 10.0.14393.4225; amd64

### `nats-streaming:0.20.0-windowsservercore` - windows version 10.0.17763.1757; amd64

```console
$ docker pull nats-streaming@sha256:54ce906f88c84ed2e364f31fcda6fb3c162926540ce48e90f579231a6abfb48f
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2459695608 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6680b77bb43567b839fdc0da0fafd3fba6903bb3e96f903ac356ba5a31f4556`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 06 Feb 2021 05:03:14 GMT
RUN Install update 1809-amd64
# Tue, 09 Feb 2021 20:26:38 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Feb 2021 16:00:30 GMT
ENV NATS_DOCKERIZED=1
# Wed, 10 Feb 2021 19:58:59 GMT
ENV NATS_STREAMING_SERVER=0.20.0
# Wed, 10 Feb 2021 19:58:59 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.20.0/nats-streaming-server-v0.20.0-windows-amd64.zip
# Wed, 10 Feb 2021 19:59:00 GMT
ENV GIT_DOWNLOAD_SHA256=26ae310d3ec11617d380106a769236a6dc2209769c0c36d15cb6736db1b589cb
# Wed, 10 Feb 2021 19:59:29 GMT
RUN Set-PSDebug -Trace 2
# Wed, 10 Feb 2021 20:00:45 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 10 Feb 2021 20:00:45 GMT
EXPOSE 4222 8222
# Wed, 10 Feb 2021 20:00:46 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 10 Feb 2021 20:00:47 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:db4edcf0861ff3fdc41851a5a218965ecb2ab6cf4ec9448fb80cc4b6792fd46c`  
		Size: 720.9 MB (720933935 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:751b8860e89a7e6999d74a11dc393620b118057ad881cb87f1d6e3653cb2db43`  
		Last Modified: Tue, 09 Feb 2021 20:48:09 GMT  
		Size: 1.3 KB (1337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7f01e717591f83c73890556e7a4c77e53caed8daf6c9b0150f497e094a4a698`  
		Last Modified: Wed, 10 Feb 2021 16:06:05 GMT  
		Size: 1.4 KB (1361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58b9fd76bfcc3923f270750c61e7e97a3aef114253089eaa76dc10c9646d423e`  
		Last Modified: Wed, 10 Feb 2021 20:04:42 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dedbaf4d01c80583ca29d8dbe57d676028feb67a3a05585bb4a6023db1e594d`  
		Last Modified: Wed, 10 Feb 2021 20:04:42 GMT  
		Size: 1.4 KB (1356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b3c1ad5a715163ac2b7a339e423a01f3f4f0b15a573766d89a61ba55a986ad0`  
		Last Modified: Wed, 10 Feb 2021 20:04:42 GMT  
		Size: 1.3 KB (1329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db42b5fd63b27df3e466b97a15dc186ad636cbdd8329490877acd12f3ea19d79`  
		Last Modified: Wed, 10 Feb 2021 20:04:41 GMT  
		Size: 5.0 MB (5027472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b65ae3b9922d83438f901016cdfc11b6b3a61c6b9e808c96d2d2e05680ea042`  
		Last Modified: Wed, 10 Feb 2021 20:04:44 GMT  
		Size: 15.4 MB (15390555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:019886058fe88defbb509d8045d2f7a5d345e2dfefec33c626894401ca5bb5b7`  
		Last Modified: Wed, 10 Feb 2021 20:04:40 GMT  
		Size: 1.3 KB (1335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98167084c5ae01ebb43d46418db9814ab5794cf8c2295f38c6def03ddc1427d9`  
		Last Modified: Wed, 10 Feb 2021 20:04:40 GMT  
		Size: 1.3 KB (1326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ef3dff4857898fe4a1c9877ddf0c7173d892e69faa0e651a99be642cfb57790`  
		Last Modified: Wed, 10 Feb 2021 20:04:40 GMT  
		Size: 1.4 KB (1361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.20.0-windowsservercore` - windows version 10.0.14393.4225; amd64

```console
$ docker pull nats-streaming@sha256:51668710b962ea70261499d873828a7b752f13c47a599f71e9199c0e1a7bf9a9
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5816886127 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a297d5a9a88f97d8c01f02171e4e2b9a45cb7e428c1e45796b3f80622ba1dfa8`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 27 Jan 2021 18:11:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 09 Feb 2021 20:28:50 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Feb 2021 16:02:35 GMT
ENV NATS_DOCKERIZED=1
# Wed, 10 Feb 2021 20:01:03 GMT
ENV NATS_STREAMING_SERVER=0.20.0
# Wed, 10 Feb 2021 20:01:03 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.20.0/nats-streaming-server-v0.20.0-windows-amd64.zip
# Wed, 10 Feb 2021 20:01:04 GMT
ENV GIT_DOWNLOAD_SHA256=26ae310d3ec11617d380106a769236a6dc2209769c0c36d15cb6736db1b589cb
# Wed, 10 Feb 2021 20:02:12 GMT
RUN Set-PSDebug -Trace 2
# Wed, 10 Feb 2021 20:04:03 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 10 Feb 2021 20:04:04 GMT
EXPOSE 4222 8222
# Wed, 10 Feb 2021 20:04:04 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 10 Feb 2021 20:04:05 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:62c48323ed8ac695b8cbe0ecedcc28ba185a234673ad9241df2b151dd00f9181`  
		Size: 1.7 GB (1725027107 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ac4a230905430e1aea27172a9432f576cc4a530e72bea516a2b304d2b7e9c101`  
		Last Modified: Tue, 09 Feb 2021 20:49:11 GMT  
		Size: 1.4 KB (1356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cc28e30e89dab2d0b2b2f6c3114771d9d803d5942c730de78d2dd457ad4ac40`  
		Last Modified: Wed, 10 Feb 2021 16:06:59 GMT  
		Size: 1.4 KB (1361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05764ae13ea6854b6abb1163dedcdbec24b30ea512599f3b60542072b923f063`  
		Last Modified: Wed, 10 Feb 2021 20:06:35 GMT  
		Size: 1.4 KB (1356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14a0242de998d983dbd8cb540a0928e5d89da6be0e231d561adba835f166061a`  
		Last Modified: Wed, 10 Feb 2021 20:06:34 GMT  
		Size: 1.3 KB (1342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c60afc4477c8f67e49cc93415eea7dab8759b9682360b8c9ec52886870a603a`  
		Last Modified: Wed, 10 Feb 2021 20:06:34 GMT  
		Size: 1.4 KB (1354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca406b9360ad583b7e00b3cd19f865b72ed7cb994b2de91a0611a44ebe20fa4a`  
		Last Modified: Wed, 10 Feb 2021 20:06:32 GMT  
		Size: 5.7 MB (5656542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0319e1b15ceaaa34e58bfb5a047c9330bf2c36c0daff41d260ca00046a68e2f7`  
		Last Modified: Wed, 10 Feb 2021 20:06:35 GMT  
		Size: 16.2 MB (16205763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d04607dfd13c95014c417374cea53b46af10028ac7816011f611e530442564f`  
		Last Modified: Wed, 10 Feb 2021 20:06:31 GMT  
		Size: 1.3 KB (1333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f6fb81a24254dafc4514d4692cf0d4f651294223ab39d2b07a7c69e738e5e32`  
		Last Modified: Wed, 10 Feb 2021 20:06:32 GMT  
		Size: 1.4 KB (1351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:042f35c5ee10f438bce2ba60b486efa0cb59d803951cdd7e833fcb2b306e8e8e`  
		Last Modified: Wed, 10 Feb 2021 20:06:31 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.20.0-windowsservercore-1809`

```console
$ docker pull nats-streaming@sha256:d484366d41ec5afe4c5f2dc2ad3f47e3a800a56d86ee682115591711827aebfd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1757; amd64

### `nats-streaming:0.20.0-windowsservercore-1809` - windows version 10.0.17763.1757; amd64

```console
$ docker pull nats-streaming@sha256:54ce906f88c84ed2e364f31fcda6fb3c162926540ce48e90f579231a6abfb48f
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2459695608 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6680b77bb43567b839fdc0da0fafd3fba6903bb3e96f903ac356ba5a31f4556`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 06 Feb 2021 05:03:14 GMT
RUN Install update 1809-amd64
# Tue, 09 Feb 2021 20:26:38 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Feb 2021 16:00:30 GMT
ENV NATS_DOCKERIZED=1
# Wed, 10 Feb 2021 19:58:59 GMT
ENV NATS_STREAMING_SERVER=0.20.0
# Wed, 10 Feb 2021 19:58:59 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.20.0/nats-streaming-server-v0.20.0-windows-amd64.zip
# Wed, 10 Feb 2021 19:59:00 GMT
ENV GIT_DOWNLOAD_SHA256=26ae310d3ec11617d380106a769236a6dc2209769c0c36d15cb6736db1b589cb
# Wed, 10 Feb 2021 19:59:29 GMT
RUN Set-PSDebug -Trace 2
# Wed, 10 Feb 2021 20:00:45 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 10 Feb 2021 20:00:45 GMT
EXPOSE 4222 8222
# Wed, 10 Feb 2021 20:00:46 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 10 Feb 2021 20:00:47 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:db4edcf0861ff3fdc41851a5a218965ecb2ab6cf4ec9448fb80cc4b6792fd46c`  
		Size: 720.9 MB (720933935 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:751b8860e89a7e6999d74a11dc393620b118057ad881cb87f1d6e3653cb2db43`  
		Last Modified: Tue, 09 Feb 2021 20:48:09 GMT  
		Size: 1.3 KB (1337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7f01e717591f83c73890556e7a4c77e53caed8daf6c9b0150f497e094a4a698`  
		Last Modified: Wed, 10 Feb 2021 16:06:05 GMT  
		Size: 1.4 KB (1361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58b9fd76bfcc3923f270750c61e7e97a3aef114253089eaa76dc10c9646d423e`  
		Last Modified: Wed, 10 Feb 2021 20:04:42 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dedbaf4d01c80583ca29d8dbe57d676028feb67a3a05585bb4a6023db1e594d`  
		Last Modified: Wed, 10 Feb 2021 20:04:42 GMT  
		Size: 1.4 KB (1356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b3c1ad5a715163ac2b7a339e423a01f3f4f0b15a573766d89a61ba55a986ad0`  
		Last Modified: Wed, 10 Feb 2021 20:04:42 GMT  
		Size: 1.3 KB (1329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db42b5fd63b27df3e466b97a15dc186ad636cbdd8329490877acd12f3ea19d79`  
		Last Modified: Wed, 10 Feb 2021 20:04:41 GMT  
		Size: 5.0 MB (5027472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b65ae3b9922d83438f901016cdfc11b6b3a61c6b9e808c96d2d2e05680ea042`  
		Last Modified: Wed, 10 Feb 2021 20:04:44 GMT  
		Size: 15.4 MB (15390555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:019886058fe88defbb509d8045d2f7a5d345e2dfefec33c626894401ca5bb5b7`  
		Last Modified: Wed, 10 Feb 2021 20:04:40 GMT  
		Size: 1.3 KB (1335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98167084c5ae01ebb43d46418db9814ab5794cf8c2295f38c6def03ddc1427d9`  
		Last Modified: Wed, 10 Feb 2021 20:04:40 GMT  
		Size: 1.3 KB (1326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ef3dff4857898fe4a1c9877ddf0c7173d892e69faa0e651a99be642cfb57790`  
		Last Modified: Wed, 10 Feb 2021 20:04:40 GMT  
		Size: 1.4 KB (1361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.20.0-windowsservercore-ltsc2016`

```console
$ docker pull nats-streaming@sha256:b84cb6e0d77ade20c0cde41401c881134555257e2b94afedbf2b7bf93a05bdbe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4225; amd64

### `nats-streaming:0.20.0-windowsservercore-ltsc2016` - windows version 10.0.14393.4225; amd64

```console
$ docker pull nats-streaming@sha256:51668710b962ea70261499d873828a7b752f13c47a599f71e9199c0e1a7bf9a9
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5816886127 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a297d5a9a88f97d8c01f02171e4e2b9a45cb7e428c1e45796b3f80622ba1dfa8`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 27 Jan 2021 18:11:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 09 Feb 2021 20:28:50 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Feb 2021 16:02:35 GMT
ENV NATS_DOCKERIZED=1
# Wed, 10 Feb 2021 20:01:03 GMT
ENV NATS_STREAMING_SERVER=0.20.0
# Wed, 10 Feb 2021 20:01:03 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.20.0/nats-streaming-server-v0.20.0-windows-amd64.zip
# Wed, 10 Feb 2021 20:01:04 GMT
ENV GIT_DOWNLOAD_SHA256=26ae310d3ec11617d380106a769236a6dc2209769c0c36d15cb6736db1b589cb
# Wed, 10 Feb 2021 20:02:12 GMT
RUN Set-PSDebug -Trace 2
# Wed, 10 Feb 2021 20:04:03 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 10 Feb 2021 20:04:04 GMT
EXPOSE 4222 8222
# Wed, 10 Feb 2021 20:04:04 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 10 Feb 2021 20:04:05 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:62c48323ed8ac695b8cbe0ecedcc28ba185a234673ad9241df2b151dd00f9181`  
		Size: 1.7 GB (1725027107 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ac4a230905430e1aea27172a9432f576cc4a530e72bea516a2b304d2b7e9c101`  
		Last Modified: Tue, 09 Feb 2021 20:49:11 GMT  
		Size: 1.4 KB (1356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cc28e30e89dab2d0b2b2f6c3114771d9d803d5942c730de78d2dd457ad4ac40`  
		Last Modified: Wed, 10 Feb 2021 16:06:59 GMT  
		Size: 1.4 KB (1361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05764ae13ea6854b6abb1163dedcdbec24b30ea512599f3b60542072b923f063`  
		Last Modified: Wed, 10 Feb 2021 20:06:35 GMT  
		Size: 1.4 KB (1356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14a0242de998d983dbd8cb540a0928e5d89da6be0e231d561adba835f166061a`  
		Last Modified: Wed, 10 Feb 2021 20:06:34 GMT  
		Size: 1.3 KB (1342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c60afc4477c8f67e49cc93415eea7dab8759b9682360b8c9ec52886870a603a`  
		Last Modified: Wed, 10 Feb 2021 20:06:34 GMT  
		Size: 1.4 KB (1354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca406b9360ad583b7e00b3cd19f865b72ed7cb994b2de91a0611a44ebe20fa4a`  
		Last Modified: Wed, 10 Feb 2021 20:06:32 GMT  
		Size: 5.7 MB (5656542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0319e1b15ceaaa34e58bfb5a047c9330bf2c36c0daff41d260ca00046a68e2f7`  
		Last Modified: Wed, 10 Feb 2021 20:06:35 GMT  
		Size: 16.2 MB (16205763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d04607dfd13c95014c417374cea53b46af10028ac7816011f611e530442564f`  
		Last Modified: Wed, 10 Feb 2021 20:06:31 GMT  
		Size: 1.3 KB (1333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f6fb81a24254dafc4514d4692cf0d4f651294223ab39d2b07a7c69e738e5e32`  
		Last Modified: Wed, 10 Feb 2021 20:06:32 GMT  
		Size: 1.4 KB (1351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:042f35c5ee10f438bce2ba60b486efa0cb59d803951cdd7e833fcb2b306e8e8e`  
		Last Modified: Wed, 10 Feb 2021 20:06:31 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.20-alpine`

```console
$ docker pull nats-streaming@sha256:3e79d8fb911870f1333bc6bfed2fcd3af9e3090434a40d85c5b2747ad2b33ece
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.20-alpine` - linux; amd64

```console
$ docker pull nats-streaming@sha256:7e2837da130ab6208e927ba254dd3e66cf3e51c232bff758fdcd6f177e8e4cba
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.0 MB (8997694 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df0e4bfed7e10f0725503851ba4a32fa19cc88f189c2a7bc34d4348b5083e184`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 24 Feb 2021 20:20:03 GMT
ADD file:0dbb1cd66f708f54f7e6663eabf24095fcd53747bfb09912a118a77e737d9617 in / 
# Wed, 24 Feb 2021 20:20:03 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 21:16:41 GMT
ENV NATS_STREAMING_SERVER=0.20.0
# Wed, 24 Feb 2021 21:16:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='618008a4902916b6bdb26022343ab91313d4f7fc90b31d0c71ad9e75dc8299e4' ;; 		armhf) natsArch='arm6'; sha256='144b04f8f42793aee1b2deb3f6eb187648c37dcc32d526c607a0af99a847260d' ;; 		armv7) natsArch='arm7'; sha256='720f4a90d1dd536bc04639ae31c70ab46fb3e10556f0f261eb038fdce941f20c' ;; 		x86_64) natsArch='amd64'; sha256='098e2293cce5d457b92f3df35127789422562f1414427c406ffd03ea3bd687c9' ;; 		x86) natsArch='386'; sha256='322a290f4706f14d6ff8160ec437202bd282f61f0607741d0e4c38ef89b83451' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 24 Feb 2021 21:16:44 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Wed, 24 Feb 2021 21:16:44 GMT
EXPOSE 4222 8222
# Wed, 24 Feb 2021 21:16:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 24 Feb 2021 21:16:45 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:f84cab65f19f5d625a4b5f895cdf37ad9f21e160bf201ec59a48d95b2a430145`  
		Last Modified: Wed, 24 Feb 2021 20:20:39 GMT  
		Size: 2.8 MB (2799493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32044508a232eda00968bedd206428d2540ce9b818a3382269486238d731550c`  
		Last Modified: Wed, 24 Feb 2021 21:17:24 GMT  
		Size: 6.2 MB (6197781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ebefc07ccecb4605491ec038d76ed03335e0a0b0e033be052987c817d713cc0`  
		Last Modified: Wed, 24 Feb 2021 21:17:23 GMT  
		Size: 420.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.20-alpine` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:71a3dda1dc2ddabf1f7d58456851bb20b66a176c7df12844dd00777365754351
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.3 MB (8331130 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:481fb1c587fe44cb52065c781076c4d64bbe18c9d2856305f951d92d3d564c67`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 24 Feb 2021 20:50:34 GMT
ADD file:8bbb59eeaad0cbcf11559bc6e2b4492aadf6822d1935ed50c710f8bed858b7b5 in / 
# Wed, 24 Feb 2021 20:50:35 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 21:35:57 GMT
ENV NATS_STREAMING_SERVER=0.20.0
# Wed, 24 Feb 2021 21:36:02 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='618008a4902916b6bdb26022343ab91313d4f7fc90b31d0c71ad9e75dc8299e4' ;; 		armhf) natsArch='arm6'; sha256='144b04f8f42793aee1b2deb3f6eb187648c37dcc32d526c607a0af99a847260d' ;; 		armv7) natsArch='arm7'; sha256='720f4a90d1dd536bc04639ae31c70ab46fb3e10556f0f261eb038fdce941f20c' ;; 		x86_64) natsArch='amd64'; sha256='098e2293cce5d457b92f3df35127789422562f1414427c406ffd03ea3bd687c9' ;; 		x86) natsArch='386'; sha256='322a290f4706f14d6ff8160ec437202bd282f61f0607741d0e4c38ef89b83451' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 24 Feb 2021 21:36:03 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Wed, 24 Feb 2021 21:36:04 GMT
EXPOSE 4222 8222
# Wed, 24 Feb 2021 21:36:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 24 Feb 2021 21:36:05 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:55242616b0494f68f44470d864da746cd2a8f8f2d1ffca698114de64032247ef`  
		Last Modified: Wed, 24 Feb 2021 20:51:17 GMT  
		Size: 2.6 MB (2604518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cdc5b3ef2d08f12a32b4290648ce4ccaf53c62b831c0035a86f5f7934af51c5`  
		Last Modified: Wed, 24 Feb 2021 21:36:38 GMT  
		Size: 5.7 MB (5726190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:300ae63bdaa97a87286e7cd46df7562ee6d65fc79d1c59789b077a6efc5a04aa`  
		Last Modified: Wed, 24 Feb 2021 21:36:34 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.20-alpine` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:5ade3cc881349db3662cc2a32166b001c22214e0c79c0f2f99d0cb785f78cdab
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.1 MB (8125937 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3003c551e23e6c957b25e7c9db011e1cd8170bb14193c185bad20b6f639047f2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 24 Feb 2021 21:03:35 GMT
ADD file:2632f48dd643f8927da2b1af8365b3edb484bd6b7d9fee4009e69f6cf3310e91 in / 
# Wed, 24 Feb 2021 21:03:36 GMT
CMD ["/bin/sh"]
# Thu, 25 Feb 2021 02:03:00 GMT
ENV NATS_STREAMING_SERVER=0.20.0
# Thu, 25 Feb 2021 02:03:07 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='618008a4902916b6bdb26022343ab91313d4f7fc90b31d0c71ad9e75dc8299e4' ;; 		armhf) natsArch='arm6'; sha256='144b04f8f42793aee1b2deb3f6eb187648c37dcc32d526c607a0af99a847260d' ;; 		armv7) natsArch='arm7'; sha256='720f4a90d1dd536bc04639ae31c70ab46fb3e10556f0f261eb038fdce941f20c' ;; 		x86_64) natsArch='amd64'; sha256='098e2293cce5d457b92f3df35127789422562f1414427c406ffd03ea3bd687c9' ;; 		x86) natsArch='386'; sha256='322a290f4706f14d6ff8160ec437202bd282f61f0607741d0e4c38ef89b83451' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 25 Feb 2021 02:03:09 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Thu, 25 Feb 2021 02:03:10 GMT
EXPOSE 4222 8222
# Thu, 25 Feb 2021 02:03:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 25 Feb 2021 02:03:13 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:8e85c7428c31ea48b47424ca0e4663106c54591c83545d32b66a77093f90ffd0`  
		Last Modified: Wed, 24 Feb 2021 21:04:23 GMT  
		Size: 2.4 MB (2408004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e73e11681aeadb2d31fa3245a2d356980142a629503b54745e3dac74b4c6ccb`  
		Last Modified: Thu, 25 Feb 2021 02:04:13 GMT  
		Size: 5.7 MB (5717512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a07ffd0ec2224fc48e7d5a98c442b6a4a4b46730ed88e95871d2d6397f4c9d8`  
		Last Modified: Thu, 25 Feb 2021 02:04:06 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.20-alpine` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:bd39a673070144b75764fb3a0aad84cdbe8a7c16c9393b294da3d7bdddc223f9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.4 MB (8378716 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:72a01c0cbdeefc26cfc81137d93311ff33253f7d914cd42ffacbcd45725a4ab1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 24 Feb 2021 20:39:39 GMT
ADD file:7e82858ef85f6db90c131ed835a390d736cfdbd1a0cf8bccaeed8f7e30172ddb in / 
# Wed, 24 Feb 2021 20:39:40 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 23:54:22 GMT
ENV NATS_STREAMING_SERVER=0.20.0
# Wed, 24 Feb 2021 23:54:26 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='618008a4902916b6bdb26022343ab91313d4f7fc90b31d0c71ad9e75dc8299e4' ;; 		armhf) natsArch='arm6'; sha256='144b04f8f42793aee1b2deb3f6eb187648c37dcc32d526c607a0af99a847260d' ;; 		armv7) natsArch='arm7'; sha256='720f4a90d1dd536bc04639ae31c70ab46fb3e10556f0f261eb038fdce941f20c' ;; 		x86_64) natsArch='amd64'; sha256='098e2293cce5d457b92f3df35127789422562f1414427c406ffd03ea3bd687c9' ;; 		x86) natsArch='386'; sha256='322a290f4706f14d6ff8160ec437202bd282f61f0607741d0e4c38ef89b83451' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 24 Feb 2021 23:54:27 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Wed, 24 Feb 2021 23:54:28 GMT
EXPOSE 4222 8222
# Wed, 24 Feb 2021 23:54:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 24 Feb 2021 23:54:29 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:dce8679b510e95d136241d02ababff86469dd14220812a7ce9202833c0e32f66`  
		Last Modified: Wed, 24 Feb 2021 20:40:26 GMT  
		Size: 2.7 MB (2709880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64d185e50c4f0cdc2dc88a9f750ebea1210da17133d4339466bd454a3d2d3b5c`  
		Last Modified: Wed, 24 Feb 2021 23:55:03 GMT  
		Size: 5.7 MB (5668417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d70ce809390466c98565d0da9060e5d2d21974101f9ed8caf6bae1982e9cf71`  
		Last Modified: Wed, 24 Feb 2021 23:55:02 GMT  
		Size: 419.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.20-alpine3.12`

```console
$ docker pull nats-streaming@sha256:3e79d8fb911870f1333bc6bfed2fcd3af9e3090434a40d85c5b2747ad2b33ece
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.20-alpine3.12` - linux; amd64

```console
$ docker pull nats-streaming@sha256:7e2837da130ab6208e927ba254dd3e66cf3e51c232bff758fdcd6f177e8e4cba
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.0 MB (8997694 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df0e4bfed7e10f0725503851ba4a32fa19cc88f189c2a7bc34d4348b5083e184`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 24 Feb 2021 20:20:03 GMT
ADD file:0dbb1cd66f708f54f7e6663eabf24095fcd53747bfb09912a118a77e737d9617 in / 
# Wed, 24 Feb 2021 20:20:03 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 21:16:41 GMT
ENV NATS_STREAMING_SERVER=0.20.0
# Wed, 24 Feb 2021 21:16:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='618008a4902916b6bdb26022343ab91313d4f7fc90b31d0c71ad9e75dc8299e4' ;; 		armhf) natsArch='arm6'; sha256='144b04f8f42793aee1b2deb3f6eb187648c37dcc32d526c607a0af99a847260d' ;; 		armv7) natsArch='arm7'; sha256='720f4a90d1dd536bc04639ae31c70ab46fb3e10556f0f261eb038fdce941f20c' ;; 		x86_64) natsArch='amd64'; sha256='098e2293cce5d457b92f3df35127789422562f1414427c406ffd03ea3bd687c9' ;; 		x86) natsArch='386'; sha256='322a290f4706f14d6ff8160ec437202bd282f61f0607741d0e4c38ef89b83451' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 24 Feb 2021 21:16:44 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Wed, 24 Feb 2021 21:16:44 GMT
EXPOSE 4222 8222
# Wed, 24 Feb 2021 21:16:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 24 Feb 2021 21:16:45 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:f84cab65f19f5d625a4b5f895cdf37ad9f21e160bf201ec59a48d95b2a430145`  
		Last Modified: Wed, 24 Feb 2021 20:20:39 GMT  
		Size: 2.8 MB (2799493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32044508a232eda00968bedd206428d2540ce9b818a3382269486238d731550c`  
		Last Modified: Wed, 24 Feb 2021 21:17:24 GMT  
		Size: 6.2 MB (6197781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ebefc07ccecb4605491ec038d76ed03335e0a0b0e033be052987c817d713cc0`  
		Last Modified: Wed, 24 Feb 2021 21:17:23 GMT  
		Size: 420.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.20-alpine3.12` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:71a3dda1dc2ddabf1f7d58456851bb20b66a176c7df12844dd00777365754351
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.3 MB (8331130 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:481fb1c587fe44cb52065c781076c4d64bbe18c9d2856305f951d92d3d564c67`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 24 Feb 2021 20:50:34 GMT
ADD file:8bbb59eeaad0cbcf11559bc6e2b4492aadf6822d1935ed50c710f8bed858b7b5 in / 
# Wed, 24 Feb 2021 20:50:35 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 21:35:57 GMT
ENV NATS_STREAMING_SERVER=0.20.0
# Wed, 24 Feb 2021 21:36:02 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='618008a4902916b6bdb26022343ab91313d4f7fc90b31d0c71ad9e75dc8299e4' ;; 		armhf) natsArch='arm6'; sha256='144b04f8f42793aee1b2deb3f6eb187648c37dcc32d526c607a0af99a847260d' ;; 		armv7) natsArch='arm7'; sha256='720f4a90d1dd536bc04639ae31c70ab46fb3e10556f0f261eb038fdce941f20c' ;; 		x86_64) natsArch='amd64'; sha256='098e2293cce5d457b92f3df35127789422562f1414427c406ffd03ea3bd687c9' ;; 		x86) natsArch='386'; sha256='322a290f4706f14d6ff8160ec437202bd282f61f0607741d0e4c38ef89b83451' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 24 Feb 2021 21:36:03 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Wed, 24 Feb 2021 21:36:04 GMT
EXPOSE 4222 8222
# Wed, 24 Feb 2021 21:36:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 24 Feb 2021 21:36:05 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:55242616b0494f68f44470d864da746cd2a8f8f2d1ffca698114de64032247ef`  
		Last Modified: Wed, 24 Feb 2021 20:51:17 GMT  
		Size: 2.6 MB (2604518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cdc5b3ef2d08f12a32b4290648ce4ccaf53c62b831c0035a86f5f7934af51c5`  
		Last Modified: Wed, 24 Feb 2021 21:36:38 GMT  
		Size: 5.7 MB (5726190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:300ae63bdaa97a87286e7cd46df7562ee6d65fc79d1c59789b077a6efc5a04aa`  
		Last Modified: Wed, 24 Feb 2021 21:36:34 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.20-alpine3.12` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:5ade3cc881349db3662cc2a32166b001c22214e0c79c0f2f99d0cb785f78cdab
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.1 MB (8125937 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3003c551e23e6c957b25e7c9db011e1cd8170bb14193c185bad20b6f639047f2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 24 Feb 2021 21:03:35 GMT
ADD file:2632f48dd643f8927da2b1af8365b3edb484bd6b7d9fee4009e69f6cf3310e91 in / 
# Wed, 24 Feb 2021 21:03:36 GMT
CMD ["/bin/sh"]
# Thu, 25 Feb 2021 02:03:00 GMT
ENV NATS_STREAMING_SERVER=0.20.0
# Thu, 25 Feb 2021 02:03:07 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='618008a4902916b6bdb26022343ab91313d4f7fc90b31d0c71ad9e75dc8299e4' ;; 		armhf) natsArch='arm6'; sha256='144b04f8f42793aee1b2deb3f6eb187648c37dcc32d526c607a0af99a847260d' ;; 		armv7) natsArch='arm7'; sha256='720f4a90d1dd536bc04639ae31c70ab46fb3e10556f0f261eb038fdce941f20c' ;; 		x86_64) natsArch='amd64'; sha256='098e2293cce5d457b92f3df35127789422562f1414427c406ffd03ea3bd687c9' ;; 		x86) natsArch='386'; sha256='322a290f4706f14d6ff8160ec437202bd282f61f0607741d0e4c38ef89b83451' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 25 Feb 2021 02:03:09 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Thu, 25 Feb 2021 02:03:10 GMT
EXPOSE 4222 8222
# Thu, 25 Feb 2021 02:03:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 25 Feb 2021 02:03:13 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:8e85c7428c31ea48b47424ca0e4663106c54591c83545d32b66a77093f90ffd0`  
		Last Modified: Wed, 24 Feb 2021 21:04:23 GMT  
		Size: 2.4 MB (2408004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e73e11681aeadb2d31fa3245a2d356980142a629503b54745e3dac74b4c6ccb`  
		Last Modified: Thu, 25 Feb 2021 02:04:13 GMT  
		Size: 5.7 MB (5717512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a07ffd0ec2224fc48e7d5a98c442b6a4a4b46730ed88e95871d2d6397f4c9d8`  
		Last Modified: Thu, 25 Feb 2021 02:04:06 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.20-alpine3.12` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:bd39a673070144b75764fb3a0aad84cdbe8a7c16c9393b294da3d7bdddc223f9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.4 MB (8378716 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:72a01c0cbdeefc26cfc81137d93311ff33253f7d914cd42ffacbcd45725a4ab1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 24 Feb 2021 20:39:39 GMT
ADD file:7e82858ef85f6db90c131ed835a390d736cfdbd1a0cf8bccaeed8f7e30172ddb in / 
# Wed, 24 Feb 2021 20:39:40 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 23:54:22 GMT
ENV NATS_STREAMING_SERVER=0.20.0
# Wed, 24 Feb 2021 23:54:26 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='618008a4902916b6bdb26022343ab91313d4f7fc90b31d0c71ad9e75dc8299e4' ;; 		armhf) natsArch='arm6'; sha256='144b04f8f42793aee1b2deb3f6eb187648c37dcc32d526c607a0af99a847260d' ;; 		armv7) natsArch='arm7'; sha256='720f4a90d1dd536bc04639ae31c70ab46fb3e10556f0f261eb038fdce941f20c' ;; 		x86_64) natsArch='amd64'; sha256='098e2293cce5d457b92f3df35127789422562f1414427c406ffd03ea3bd687c9' ;; 		x86) natsArch='386'; sha256='322a290f4706f14d6ff8160ec437202bd282f61f0607741d0e4c38ef89b83451' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 24 Feb 2021 23:54:27 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Wed, 24 Feb 2021 23:54:28 GMT
EXPOSE 4222 8222
# Wed, 24 Feb 2021 23:54:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 24 Feb 2021 23:54:29 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:dce8679b510e95d136241d02ababff86469dd14220812a7ce9202833c0e32f66`  
		Last Modified: Wed, 24 Feb 2021 20:40:26 GMT  
		Size: 2.7 MB (2709880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64d185e50c4f0cdc2dc88a9f750ebea1210da17133d4339466bd454a3d2d3b5c`  
		Last Modified: Wed, 24 Feb 2021 23:55:03 GMT  
		Size: 5.7 MB (5668417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d70ce809390466c98565d0da9060e5d2d21974101f9ed8caf6bae1982e9cf71`  
		Last Modified: Wed, 24 Feb 2021 23:55:02 GMT  
		Size: 419.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.20-linux`

```console
$ docker pull nats-streaming@sha256:f46b63443b02bc0089e72301ae260b1ef32ff25e755e67b633169945585ca12d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.20-linux` - linux; amd64

```console
$ docker pull nats-streaming@sha256:cd0162a7232de1eabe982554c8740e7edbac4747af3e99fa9bc38a480b4a4243
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 MB (5914730 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1544c1524919e1458186fefae5f5ff415c37055742e531010fc2660b11db2339`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 12 Jan 2021 00:48:24 GMT
COPY file:acbca3cec2dc5172f21984b614cbcd90e6e4cf0bd9848c5ddcffb94615a02436 in /nats-streaming-server 
# Tue, 12 Jan 2021 00:48:24 GMT
EXPOSE 4222 8222
# Tue, 12 Jan 2021 00:48:24 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 12 Jan 2021 00:48:24 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:0d51fde6ce3492f397e8a85dad354a9a45ab91310cf4abd6275101f3ef823587`  
		Last Modified: Tue, 12 Jan 2021 00:49:07 GMT  
		Size: 5.9 MB (5914730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.20-linux` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:bbb3d771f9232932017b9cb9b501734367bc3560eed790695be682d94a8f3573
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.4 MB (5444243 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ed880c2955fd126b0ce38471e90c9467c9c739f55b4c789cec1a4575a41d36f`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 11 Jan 2021 23:53:53 GMT
COPY file:617b9b5366d0d437ce471ad0763bdd7d350496612583dc2c7044dcde4d32257e in /nats-streaming-server 
# Mon, 11 Jan 2021 23:53:54 GMT
EXPOSE 4222 8222
# Mon, 11 Jan 2021 23:53:54 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 11 Jan 2021 23:53:55 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:7cffcff2c5b4913dac660d7456365492a0393b1aa6f1812f6b7b46b250e1970d`  
		Last Modified: Mon, 11 Jan 2021 23:54:39 GMT  
		Size: 5.4 MB (5444243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.20-linux` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:b2d9250f9a4e3b25b2212f4e8c27c693cc5cfa0f83ca82a8005c90ae8372ab86
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.4 MB (5439328 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:35f1d3c5a1d429a3e2b1fc71f5bc023980c41d34ccb0a0482aca07b6cbb4d6f1`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 12 Jan 2021 00:19:09 GMT
COPY file:2b3fc04f11d3cc7cdfa09f93a79d8efe0889d24324b831fb35126470165c9027 in /nats-streaming-server 
# Tue, 12 Jan 2021 00:19:14 GMT
EXPOSE 4222 8222
# Tue, 12 Jan 2021 00:19:16 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 12 Jan 2021 00:19:17 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:bf50122b11c4b5e2fa295a9456a93489ad25dd1e9bfefda1d572da1a57418205`  
		Last Modified: Tue, 12 Jan 2021 00:20:01 GMT  
		Size: 5.4 MB (5439328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.20-linux` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:0f315491d4d14e634f971591c7f8bd0eb9aad59975fcdf867a51294df2e5efb2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.4 MB (5388538 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:22dba974517468c29a982c1b4a0b7744a93825122145a1dcc5f7e53c96119efa`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 11 Jan 2021 23:47:25 GMT
COPY file:5a251d4e6bafc9d9ea6f25cd37fd44252da405176da94cc580cdd663abecffa5 in /nats-streaming-server 
# Mon, 11 Jan 2021 23:47:26 GMT
EXPOSE 4222 8222
# Mon, 11 Jan 2021 23:47:26 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 11 Jan 2021 23:47:27 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:58239a1ea6494e431645c7ad156ed917333a248edbe6be76af8b7384d9339f07`  
		Last Modified: Mon, 11 Jan 2021 23:48:09 GMT  
		Size: 5.4 MB (5388538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.20-nanoserver`

```console
$ docker pull nats-streaming@sha256:b89cba5cf792b4be014bbb1be1a2fbca1c0019946c989c8a903c7ed865c0e7d8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1757; amd64

### `nats-streaming:0.20-nanoserver` - windows version 10.0.17763.1757; amd64

```console
$ docker pull nats-streaming@sha256:d13b43d591f725a510ae54f0f2efa114399a0a0c9e85f0652bc802e7e8d45187
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.4 MB (107432722 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc67b6d7f9c859b2a9e9272dfda84571744e233c3ada49fdd3505d40e586c859`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 02 Feb 2021 13:06:30 GMT
RUN Apply image 1809-amd64
# Wed, 10 Feb 2021 16:02:26 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 10 Feb 2021 20:00:55 GMT
RUN cmd /S /C #(nop) COPY file:f2450ffeda74e33f820191eccf78b6647ce56865170e966bfa8e72afe6e46c36 in C:\nats-streaming-server.exe 
# Wed, 10 Feb 2021 20:00:56 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 10 Feb 2021 20:00:57 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 10 Feb 2021 20:00:57 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:ba17af31b9276ee11fdf859681b442db50979a39eff4cea2a559a5755cedbe01`  
		Size: 101.4 MB (101406193 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:23b613036f8aee9066e712b3aa58f10f2fde093623511a5658867f53a6d01b18`  
		Last Modified: Wed, 10 Feb 2021 16:06:34 GMT  
		Size: 1.1 KB (1071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:546c4d75ec4cbc867ea01774757b0a9303906569a30157fd804f8c1bc5d4e63e`  
		Last Modified: Wed, 10 Feb 2021 20:06:15 GMT  
		Size: 6.0 MB (6022164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d942fdcd6082f7ac407761ffc6d739677d6fe08f0f51db38d32d33398e9073f`  
		Last Modified: Wed, 10 Feb 2021 20:06:07 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2c29c3e2255d5f0292ecd161299cb57afc896ff1c7002836b53577f1d57e6fe`  
		Last Modified: Wed, 10 Feb 2021 20:06:07 GMT  
		Size: 1.1 KB (1097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12923e759dcf1b0d858f5bfacd7f73cffa442500803639aa349428d981cd881f`  
		Last Modified: Wed, 10 Feb 2021 20:06:07 GMT  
		Size: 1.1 KB (1072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.20-nanoserver-1809`

```console
$ docker pull nats-streaming@sha256:b89cba5cf792b4be014bbb1be1a2fbca1c0019946c989c8a903c7ed865c0e7d8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1757; amd64

### `nats-streaming:0.20-nanoserver-1809` - windows version 10.0.17763.1757; amd64

```console
$ docker pull nats-streaming@sha256:d13b43d591f725a510ae54f0f2efa114399a0a0c9e85f0652bc802e7e8d45187
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.4 MB (107432722 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc67b6d7f9c859b2a9e9272dfda84571744e233c3ada49fdd3505d40e586c859`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 02 Feb 2021 13:06:30 GMT
RUN Apply image 1809-amd64
# Wed, 10 Feb 2021 16:02:26 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 10 Feb 2021 20:00:55 GMT
RUN cmd /S /C #(nop) COPY file:f2450ffeda74e33f820191eccf78b6647ce56865170e966bfa8e72afe6e46c36 in C:\nats-streaming-server.exe 
# Wed, 10 Feb 2021 20:00:56 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 10 Feb 2021 20:00:57 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 10 Feb 2021 20:00:57 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:ba17af31b9276ee11fdf859681b442db50979a39eff4cea2a559a5755cedbe01`  
		Size: 101.4 MB (101406193 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:23b613036f8aee9066e712b3aa58f10f2fde093623511a5658867f53a6d01b18`  
		Last Modified: Wed, 10 Feb 2021 16:06:34 GMT  
		Size: 1.1 KB (1071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:546c4d75ec4cbc867ea01774757b0a9303906569a30157fd804f8c1bc5d4e63e`  
		Last Modified: Wed, 10 Feb 2021 20:06:15 GMT  
		Size: 6.0 MB (6022164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d942fdcd6082f7ac407761ffc6d739677d6fe08f0f51db38d32d33398e9073f`  
		Last Modified: Wed, 10 Feb 2021 20:06:07 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2c29c3e2255d5f0292ecd161299cb57afc896ff1c7002836b53577f1d57e6fe`  
		Last Modified: Wed, 10 Feb 2021 20:06:07 GMT  
		Size: 1.1 KB (1097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12923e759dcf1b0d858f5bfacd7f73cffa442500803639aa349428d981cd881f`  
		Last Modified: Wed, 10 Feb 2021 20:06:07 GMT  
		Size: 1.1 KB (1072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.20-scratch`

```console
$ docker pull nats-streaming@sha256:f46b63443b02bc0089e72301ae260b1ef32ff25e755e67b633169945585ca12d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.20-scratch` - linux; amd64

```console
$ docker pull nats-streaming@sha256:cd0162a7232de1eabe982554c8740e7edbac4747af3e99fa9bc38a480b4a4243
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 MB (5914730 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1544c1524919e1458186fefae5f5ff415c37055742e531010fc2660b11db2339`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 12 Jan 2021 00:48:24 GMT
COPY file:acbca3cec2dc5172f21984b614cbcd90e6e4cf0bd9848c5ddcffb94615a02436 in /nats-streaming-server 
# Tue, 12 Jan 2021 00:48:24 GMT
EXPOSE 4222 8222
# Tue, 12 Jan 2021 00:48:24 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 12 Jan 2021 00:48:24 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:0d51fde6ce3492f397e8a85dad354a9a45ab91310cf4abd6275101f3ef823587`  
		Last Modified: Tue, 12 Jan 2021 00:49:07 GMT  
		Size: 5.9 MB (5914730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.20-scratch` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:bbb3d771f9232932017b9cb9b501734367bc3560eed790695be682d94a8f3573
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.4 MB (5444243 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ed880c2955fd126b0ce38471e90c9467c9c739f55b4c789cec1a4575a41d36f`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 11 Jan 2021 23:53:53 GMT
COPY file:617b9b5366d0d437ce471ad0763bdd7d350496612583dc2c7044dcde4d32257e in /nats-streaming-server 
# Mon, 11 Jan 2021 23:53:54 GMT
EXPOSE 4222 8222
# Mon, 11 Jan 2021 23:53:54 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 11 Jan 2021 23:53:55 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:7cffcff2c5b4913dac660d7456365492a0393b1aa6f1812f6b7b46b250e1970d`  
		Last Modified: Mon, 11 Jan 2021 23:54:39 GMT  
		Size: 5.4 MB (5444243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.20-scratch` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:b2d9250f9a4e3b25b2212f4e8c27c693cc5cfa0f83ca82a8005c90ae8372ab86
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.4 MB (5439328 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:35f1d3c5a1d429a3e2b1fc71f5bc023980c41d34ccb0a0482aca07b6cbb4d6f1`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 12 Jan 2021 00:19:09 GMT
COPY file:2b3fc04f11d3cc7cdfa09f93a79d8efe0889d24324b831fb35126470165c9027 in /nats-streaming-server 
# Tue, 12 Jan 2021 00:19:14 GMT
EXPOSE 4222 8222
# Tue, 12 Jan 2021 00:19:16 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 12 Jan 2021 00:19:17 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:bf50122b11c4b5e2fa295a9456a93489ad25dd1e9bfefda1d572da1a57418205`  
		Last Modified: Tue, 12 Jan 2021 00:20:01 GMT  
		Size: 5.4 MB (5439328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.20-scratch` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:0f315491d4d14e634f971591c7f8bd0eb9aad59975fcdf867a51294df2e5efb2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.4 MB (5388538 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:22dba974517468c29a982c1b4a0b7744a93825122145a1dcc5f7e53c96119efa`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 11 Jan 2021 23:47:25 GMT
COPY file:5a251d4e6bafc9d9ea6f25cd37fd44252da405176da94cc580cdd663abecffa5 in /nats-streaming-server 
# Mon, 11 Jan 2021 23:47:26 GMT
EXPOSE 4222 8222
# Mon, 11 Jan 2021 23:47:26 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 11 Jan 2021 23:47:27 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:58239a1ea6494e431645c7ad156ed917333a248edbe6be76af8b7384d9339f07`  
		Last Modified: Mon, 11 Jan 2021 23:48:09 GMT  
		Size: 5.4 MB (5388538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.20-windowsservercore`

```console
$ docker pull nats-streaming@sha256:f5c17fa3628e9e6d4f4a960b80c4f905b48409dc7f7227d9b2b53652d5e03311
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1757; amd64
	-	windows version 10.0.14393.4225; amd64

### `nats-streaming:0.20-windowsservercore` - windows version 10.0.17763.1757; amd64

```console
$ docker pull nats-streaming@sha256:54ce906f88c84ed2e364f31fcda6fb3c162926540ce48e90f579231a6abfb48f
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2459695608 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6680b77bb43567b839fdc0da0fafd3fba6903bb3e96f903ac356ba5a31f4556`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 06 Feb 2021 05:03:14 GMT
RUN Install update 1809-amd64
# Tue, 09 Feb 2021 20:26:38 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Feb 2021 16:00:30 GMT
ENV NATS_DOCKERIZED=1
# Wed, 10 Feb 2021 19:58:59 GMT
ENV NATS_STREAMING_SERVER=0.20.0
# Wed, 10 Feb 2021 19:58:59 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.20.0/nats-streaming-server-v0.20.0-windows-amd64.zip
# Wed, 10 Feb 2021 19:59:00 GMT
ENV GIT_DOWNLOAD_SHA256=26ae310d3ec11617d380106a769236a6dc2209769c0c36d15cb6736db1b589cb
# Wed, 10 Feb 2021 19:59:29 GMT
RUN Set-PSDebug -Trace 2
# Wed, 10 Feb 2021 20:00:45 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 10 Feb 2021 20:00:45 GMT
EXPOSE 4222 8222
# Wed, 10 Feb 2021 20:00:46 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 10 Feb 2021 20:00:47 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:db4edcf0861ff3fdc41851a5a218965ecb2ab6cf4ec9448fb80cc4b6792fd46c`  
		Size: 720.9 MB (720933935 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:751b8860e89a7e6999d74a11dc393620b118057ad881cb87f1d6e3653cb2db43`  
		Last Modified: Tue, 09 Feb 2021 20:48:09 GMT  
		Size: 1.3 KB (1337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7f01e717591f83c73890556e7a4c77e53caed8daf6c9b0150f497e094a4a698`  
		Last Modified: Wed, 10 Feb 2021 16:06:05 GMT  
		Size: 1.4 KB (1361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58b9fd76bfcc3923f270750c61e7e97a3aef114253089eaa76dc10c9646d423e`  
		Last Modified: Wed, 10 Feb 2021 20:04:42 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dedbaf4d01c80583ca29d8dbe57d676028feb67a3a05585bb4a6023db1e594d`  
		Last Modified: Wed, 10 Feb 2021 20:04:42 GMT  
		Size: 1.4 KB (1356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b3c1ad5a715163ac2b7a339e423a01f3f4f0b15a573766d89a61ba55a986ad0`  
		Last Modified: Wed, 10 Feb 2021 20:04:42 GMT  
		Size: 1.3 KB (1329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db42b5fd63b27df3e466b97a15dc186ad636cbdd8329490877acd12f3ea19d79`  
		Last Modified: Wed, 10 Feb 2021 20:04:41 GMT  
		Size: 5.0 MB (5027472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b65ae3b9922d83438f901016cdfc11b6b3a61c6b9e808c96d2d2e05680ea042`  
		Last Modified: Wed, 10 Feb 2021 20:04:44 GMT  
		Size: 15.4 MB (15390555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:019886058fe88defbb509d8045d2f7a5d345e2dfefec33c626894401ca5bb5b7`  
		Last Modified: Wed, 10 Feb 2021 20:04:40 GMT  
		Size: 1.3 KB (1335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98167084c5ae01ebb43d46418db9814ab5794cf8c2295f38c6def03ddc1427d9`  
		Last Modified: Wed, 10 Feb 2021 20:04:40 GMT  
		Size: 1.3 KB (1326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ef3dff4857898fe4a1c9877ddf0c7173d892e69faa0e651a99be642cfb57790`  
		Last Modified: Wed, 10 Feb 2021 20:04:40 GMT  
		Size: 1.4 KB (1361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.20-windowsservercore` - windows version 10.0.14393.4225; amd64

```console
$ docker pull nats-streaming@sha256:51668710b962ea70261499d873828a7b752f13c47a599f71e9199c0e1a7bf9a9
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5816886127 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a297d5a9a88f97d8c01f02171e4e2b9a45cb7e428c1e45796b3f80622ba1dfa8`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 27 Jan 2021 18:11:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 09 Feb 2021 20:28:50 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Feb 2021 16:02:35 GMT
ENV NATS_DOCKERIZED=1
# Wed, 10 Feb 2021 20:01:03 GMT
ENV NATS_STREAMING_SERVER=0.20.0
# Wed, 10 Feb 2021 20:01:03 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.20.0/nats-streaming-server-v0.20.0-windows-amd64.zip
# Wed, 10 Feb 2021 20:01:04 GMT
ENV GIT_DOWNLOAD_SHA256=26ae310d3ec11617d380106a769236a6dc2209769c0c36d15cb6736db1b589cb
# Wed, 10 Feb 2021 20:02:12 GMT
RUN Set-PSDebug -Trace 2
# Wed, 10 Feb 2021 20:04:03 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 10 Feb 2021 20:04:04 GMT
EXPOSE 4222 8222
# Wed, 10 Feb 2021 20:04:04 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 10 Feb 2021 20:04:05 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:62c48323ed8ac695b8cbe0ecedcc28ba185a234673ad9241df2b151dd00f9181`  
		Size: 1.7 GB (1725027107 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ac4a230905430e1aea27172a9432f576cc4a530e72bea516a2b304d2b7e9c101`  
		Last Modified: Tue, 09 Feb 2021 20:49:11 GMT  
		Size: 1.4 KB (1356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cc28e30e89dab2d0b2b2f6c3114771d9d803d5942c730de78d2dd457ad4ac40`  
		Last Modified: Wed, 10 Feb 2021 16:06:59 GMT  
		Size: 1.4 KB (1361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05764ae13ea6854b6abb1163dedcdbec24b30ea512599f3b60542072b923f063`  
		Last Modified: Wed, 10 Feb 2021 20:06:35 GMT  
		Size: 1.4 KB (1356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14a0242de998d983dbd8cb540a0928e5d89da6be0e231d561adba835f166061a`  
		Last Modified: Wed, 10 Feb 2021 20:06:34 GMT  
		Size: 1.3 KB (1342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c60afc4477c8f67e49cc93415eea7dab8759b9682360b8c9ec52886870a603a`  
		Last Modified: Wed, 10 Feb 2021 20:06:34 GMT  
		Size: 1.4 KB (1354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca406b9360ad583b7e00b3cd19f865b72ed7cb994b2de91a0611a44ebe20fa4a`  
		Last Modified: Wed, 10 Feb 2021 20:06:32 GMT  
		Size: 5.7 MB (5656542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0319e1b15ceaaa34e58bfb5a047c9330bf2c36c0daff41d260ca00046a68e2f7`  
		Last Modified: Wed, 10 Feb 2021 20:06:35 GMT  
		Size: 16.2 MB (16205763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d04607dfd13c95014c417374cea53b46af10028ac7816011f611e530442564f`  
		Last Modified: Wed, 10 Feb 2021 20:06:31 GMT  
		Size: 1.3 KB (1333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f6fb81a24254dafc4514d4692cf0d4f651294223ab39d2b07a7c69e738e5e32`  
		Last Modified: Wed, 10 Feb 2021 20:06:32 GMT  
		Size: 1.4 KB (1351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:042f35c5ee10f438bce2ba60b486efa0cb59d803951cdd7e833fcb2b306e8e8e`  
		Last Modified: Wed, 10 Feb 2021 20:06:31 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.20-windowsservercore-1809`

```console
$ docker pull nats-streaming@sha256:d484366d41ec5afe4c5f2dc2ad3f47e3a800a56d86ee682115591711827aebfd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1757; amd64

### `nats-streaming:0.20-windowsservercore-1809` - windows version 10.0.17763.1757; amd64

```console
$ docker pull nats-streaming@sha256:54ce906f88c84ed2e364f31fcda6fb3c162926540ce48e90f579231a6abfb48f
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2459695608 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6680b77bb43567b839fdc0da0fafd3fba6903bb3e96f903ac356ba5a31f4556`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 06 Feb 2021 05:03:14 GMT
RUN Install update 1809-amd64
# Tue, 09 Feb 2021 20:26:38 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Feb 2021 16:00:30 GMT
ENV NATS_DOCKERIZED=1
# Wed, 10 Feb 2021 19:58:59 GMT
ENV NATS_STREAMING_SERVER=0.20.0
# Wed, 10 Feb 2021 19:58:59 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.20.0/nats-streaming-server-v0.20.0-windows-amd64.zip
# Wed, 10 Feb 2021 19:59:00 GMT
ENV GIT_DOWNLOAD_SHA256=26ae310d3ec11617d380106a769236a6dc2209769c0c36d15cb6736db1b589cb
# Wed, 10 Feb 2021 19:59:29 GMT
RUN Set-PSDebug -Trace 2
# Wed, 10 Feb 2021 20:00:45 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 10 Feb 2021 20:00:45 GMT
EXPOSE 4222 8222
# Wed, 10 Feb 2021 20:00:46 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 10 Feb 2021 20:00:47 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:db4edcf0861ff3fdc41851a5a218965ecb2ab6cf4ec9448fb80cc4b6792fd46c`  
		Size: 720.9 MB (720933935 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:751b8860e89a7e6999d74a11dc393620b118057ad881cb87f1d6e3653cb2db43`  
		Last Modified: Tue, 09 Feb 2021 20:48:09 GMT  
		Size: 1.3 KB (1337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7f01e717591f83c73890556e7a4c77e53caed8daf6c9b0150f497e094a4a698`  
		Last Modified: Wed, 10 Feb 2021 16:06:05 GMT  
		Size: 1.4 KB (1361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58b9fd76bfcc3923f270750c61e7e97a3aef114253089eaa76dc10c9646d423e`  
		Last Modified: Wed, 10 Feb 2021 20:04:42 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dedbaf4d01c80583ca29d8dbe57d676028feb67a3a05585bb4a6023db1e594d`  
		Last Modified: Wed, 10 Feb 2021 20:04:42 GMT  
		Size: 1.4 KB (1356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b3c1ad5a715163ac2b7a339e423a01f3f4f0b15a573766d89a61ba55a986ad0`  
		Last Modified: Wed, 10 Feb 2021 20:04:42 GMT  
		Size: 1.3 KB (1329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db42b5fd63b27df3e466b97a15dc186ad636cbdd8329490877acd12f3ea19d79`  
		Last Modified: Wed, 10 Feb 2021 20:04:41 GMT  
		Size: 5.0 MB (5027472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b65ae3b9922d83438f901016cdfc11b6b3a61c6b9e808c96d2d2e05680ea042`  
		Last Modified: Wed, 10 Feb 2021 20:04:44 GMT  
		Size: 15.4 MB (15390555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:019886058fe88defbb509d8045d2f7a5d345e2dfefec33c626894401ca5bb5b7`  
		Last Modified: Wed, 10 Feb 2021 20:04:40 GMT  
		Size: 1.3 KB (1335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98167084c5ae01ebb43d46418db9814ab5794cf8c2295f38c6def03ddc1427d9`  
		Last Modified: Wed, 10 Feb 2021 20:04:40 GMT  
		Size: 1.3 KB (1326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ef3dff4857898fe4a1c9877ddf0c7173d892e69faa0e651a99be642cfb57790`  
		Last Modified: Wed, 10 Feb 2021 20:04:40 GMT  
		Size: 1.4 KB (1361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.20-windowsservercore-ltsc2016`

```console
$ docker pull nats-streaming@sha256:b84cb6e0d77ade20c0cde41401c881134555257e2b94afedbf2b7bf93a05bdbe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4225; amd64

### `nats-streaming:0.20-windowsservercore-ltsc2016` - windows version 10.0.14393.4225; amd64

```console
$ docker pull nats-streaming@sha256:51668710b962ea70261499d873828a7b752f13c47a599f71e9199c0e1a7bf9a9
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5816886127 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a297d5a9a88f97d8c01f02171e4e2b9a45cb7e428c1e45796b3f80622ba1dfa8`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 27 Jan 2021 18:11:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 09 Feb 2021 20:28:50 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Feb 2021 16:02:35 GMT
ENV NATS_DOCKERIZED=1
# Wed, 10 Feb 2021 20:01:03 GMT
ENV NATS_STREAMING_SERVER=0.20.0
# Wed, 10 Feb 2021 20:01:03 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.20.0/nats-streaming-server-v0.20.0-windows-amd64.zip
# Wed, 10 Feb 2021 20:01:04 GMT
ENV GIT_DOWNLOAD_SHA256=26ae310d3ec11617d380106a769236a6dc2209769c0c36d15cb6736db1b589cb
# Wed, 10 Feb 2021 20:02:12 GMT
RUN Set-PSDebug -Trace 2
# Wed, 10 Feb 2021 20:04:03 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 10 Feb 2021 20:04:04 GMT
EXPOSE 4222 8222
# Wed, 10 Feb 2021 20:04:04 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 10 Feb 2021 20:04:05 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:62c48323ed8ac695b8cbe0ecedcc28ba185a234673ad9241df2b151dd00f9181`  
		Size: 1.7 GB (1725027107 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ac4a230905430e1aea27172a9432f576cc4a530e72bea516a2b304d2b7e9c101`  
		Last Modified: Tue, 09 Feb 2021 20:49:11 GMT  
		Size: 1.4 KB (1356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cc28e30e89dab2d0b2b2f6c3114771d9d803d5942c730de78d2dd457ad4ac40`  
		Last Modified: Wed, 10 Feb 2021 16:06:59 GMT  
		Size: 1.4 KB (1361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05764ae13ea6854b6abb1163dedcdbec24b30ea512599f3b60542072b923f063`  
		Last Modified: Wed, 10 Feb 2021 20:06:35 GMT  
		Size: 1.4 KB (1356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14a0242de998d983dbd8cb540a0928e5d89da6be0e231d561adba835f166061a`  
		Last Modified: Wed, 10 Feb 2021 20:06:34 GMT  
		Size: 1.3 KB (1342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c60afc4477c8f67e49cc93415eea7dab8759b9682360b8c9ec52886870a603a`  
		Last Modified: Wed, 10 Feb 2021 20:06:34 GMT  
		Size: 1.4 KB (1354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca406b9360ad583b7e00b3cd19f865b72ed7cb994b2de91a0611a44ebe20fa4a`  
		Last Modified: Wed, 10 Feb 2021 20:06:32 GMT  
		Size: 5.7 MB (5656542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0319e1b15ceaaa34e58bfb5a047c9330bf2c36c0daff41d260ca00046a68e2f7`  
		Last Modified: Wed, 10 Feb 2021 20:06:35 GMT  
		Size: 16.2 MB (16205763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d04607dfd13c95014c417374cea53b46af10028ac7816011f611e530442564f`  
		Last Modified: Wed, 10 Feb 2021 20:06:31 GMT  
		Size: 1.3 KB (1333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f6fb81a24254dafc4514d4692cf0d4f651294223ab39d2b07a7c69e738e5e32`  
		Last Modified: Wed, 10 Feb 2021 20:06:32 GMT  
		Size: 1.4 KB (1351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:042f35c5ee10f438bce2ba60b486efa0cb59d803951cdd7e833fcb2b306e8e8e`  
		Last Modified: Wed, 10 Feb 2021 20:06:31 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:alpine`

```console
$ docker pull nats-streaming@sha256:3e79d8fb911870f1333bc6bfed2fcd3af9e3090434a40d85c5b2747ad2b33ece
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:alpine` - linux; amd64

```console
$ docker pull nats-streaming@sha256:7e2837da130ab6208e927ba254dd3e66cf3e51c232bff758fdcd6f177e8e4cba
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.0 MB (8997694 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df0e4bfed7e10f0725503851ba4a32fa19cc88f189c2a7bc34d4348b5083e184`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 24 Feb 2021 20:20:03 GMT
ADD file:0dbb1cd66f708f54f7e6663eabf24095fcd53747bfb09912a118a77e737d9617 in / 
# Wed, 24 Feb 2021 20:20:03 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 21:16:41 GMT
ENV NATS_STREAMING_SERVER=0.20.0
# Wed, 24 Feb 2021 21:16:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='618008a4902916b6bdb26022343ab91313d4f7fc90b31d0c71ad9e75dc8299e4' ;; 		armhf) natsArch='arm6'; sha256='144b04f8f42793aee1b2deb3f6eb187648c37dcc32d526c607a0af99a847260d' ;; 		armv7) natsArch='arm7'; sha256='720f4a90d1dd536bc04639ae31c70ab46fb3e10556f0f261eb038fdce941f20c' ;; 		x86_64) natsArch='amd64'; sha256='098e2293cce5d457b92f3df35127789422562f1414427c406ffd03ea3bd687c9' ;; 		x86) natsArch='386'; sha256='322a290f4706f14d6ff8160ec437202bd282f61f0607741d0e4c38ef89b83451' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 24 Feb 2021 21:16:44 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Wed, 24 Feb 2021 21:16:44 GMT
EXPOSE 4222 8222
# Wed, 24 Feb 2021 21:16:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 24 Feb 2021 21:16:45 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:f84cab65f19f5d625a4b5f895cdf37ad9f21e160bf201ec59a48d95b2a430145`  
		Last Modified: Wed, 24 Feb 2021 20:20:39 GMT  
		Size: 2.8 MB (2799493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32044508a232eda00968bedd206428d2540ce9b818a3382269486238d731550c`  
		Last Modified: Wed, 24 Feb 2021 21:17:24 GMT  
		Size: 6.2 MB (6197781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ebefc07ccecb4605491ec038d76ed03335e0a0b0e033be052987c817d713cc0`  
		Last Modified: Wed, 24 Feb 2021 21:17:23 GMT  
		Size: 420.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:71a3dda1dc2ddabf1f7d58456851bb20b66a176c7df12844dd00777365754351
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.3 MB (8331130 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:481fb1c587fe44cb52065c781076c4d64bbe18c9d2856305f951d92d3d564c67`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 24 Feb 2021 20:50:34 GMT
ADD file:8bbb59eeaad0cbcf11559bc6e2b4492aadf6822d1935ed50c710f8bed858b7b5 in / 
# Wed, 24 Feb 2021 20:50:35 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 21:35:57 GMT
ENV NATS_STREAMING_SERVER=0.20.0
# Wed, 24 Feb 2021 21:36:02 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='618008a4902916b6bdb26022343ab91313d4f7fc90b31d0c71ad9e75dc8299e4' ;; 		armhf) natsArch='arm6'; sha256='144b04f8f42793aee1b2deb3f6eb187648c37dcc32d526c607a0af99a847260d' ;; 		armv7) natsArch='arm7'; sha256='720f4a90d1dd536bc04639ae31c70ab46fb3e10556f0f261eb038fdce941f20c' ;; 		x86_64) natsArch='amd64'; sha256='098e2293cce5d457b92f3df35127789422562f1414427c406ffd03ea3bd687c9' ;; 		x86) natsArch='386'; sha256='322a290f4706f14d6ff8160ec437202bd282f61f0607741d0e4c38ef89b83451' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 24 Feb 2021 21:36:03 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Wed, 24 Feb 2021 21:36:04 GMT
EXPOSE 4222 8222
# Wed, 24 Feb 2021 21:36:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 24 Feb 2021 21:36:05 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:55242616b0494f68f44470d864da746cd2a8f8f2d1ffca698114de64032247ef`  
		Last Modified: Wed, 24 Feb 2021 20:51:17 GMT  
		Size: 2.6 MB (2604518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cdc5b3ef2d08f12a32b4290648ce4ccaf53c62b831c0035a86f5f7934af51c5`  
		Last Modified: Wed, 24 Feb 2021 21:36:38 GMT  
		Size: 5.7 MB (5726190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:300ae63bdaa97a87286e7cd46df7562ee6d65fc79d1c59789b077a6efc5a04aa`  
		Last Modified: Wed, 24 Feb 2021 21:36:34 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:5ade3cc881349db3662cc2a32166b001c22214e0c79c0f2f99d0cb785f78cdab
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.1 MB (8125937 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3003c551e23e6c957b25e7c9db011e1cd8170bb14193c185bad20b6f639047f2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 24 Feb 2021 21:03:35 GMT
ADD file:2632f48dd643f8927da2b1af8365b3edb484bd6b7d9fee4009e69f6cf3310e91 in / 
# Wed, 24 Feb 2021 21:03:36 GMT
CMD ["/bin/sh"]
# Thu, 25 Feb 2021 02:03:00 GMT
ENV NATS_STREAMING_SERVER=0.20.0
# Thu, 25 Feb 2021 02:03:07 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='618008a4902916b6bdb26022343ab91313d4f7fc90b31d0c71ad9e75dc8299e4' ;; 		armhf) natsArch='arm6'; sha256='144b04f8f42793aee1b2deb3f6eb187648c37dcc32d526c607a0af99a847260d' ;; 		armv7) natsArch='arm7'; sha256='720f4a90d1dd536bc04639ae31c70ab46fb3e10556f0f261eb038fdce941f20c' ;; 		x86_64) natsArch='amd64'; sha256='098e2293cce5d457b92f3df35127789422562f1414427c406ffd03ea3bd687c9' ;; 		x86) natsArch='386'; sha256='322a290f4706f14d6ff8160ec437202bd282f61f0607741d0e4c38ef89b83451' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 25 Feb 2021 02:03:09 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Thu, 25 Feb 2021 02:03:10 GMT
EXPOSE 4222 8222
# Thu, 25 Feb 2021 02:03:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 25 Feb 2021 02:03:13 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:8e85c7428c31ea48b47424ca0e4663106c54591c83545d32b66a77093f90ffd0`  
		Last Modified: Wed, 24 Feb 2021 21:04:23 GMT  
		Size: 2.4 MB (2408004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e73e11681aeadb2d31fa3245a2d356980142a629503b54745e3dac74b4c6ccb`  
		Last Modified: Thu, 25 Feb 2021 02:04:13 GMT  
		Size: 5.7 MB (5717512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a07ffd0ec2224fc48e7d5a98c442b6a4a4b46730ed88e95871d2d6397f4c9d8`  
		Last Modified: Thu, 25 Feb 2021 02:04:06 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:bd39a673070144b75764fb3a0aad84cdbe8a7c16c9393b294da3d7bdddc223f9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.4 MB (8378716 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:72a01c0cbdeefc26cfc81137d93311ff33253f7d914cd42ffacbcd45725a4ab1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 24 Feb 2021 20:39:39 GMT
ADD file:7e82858ef85f6db90c131ed835a390d736cfdbd1a0cf8bccaeed8f7e30172ddb in / 
# Wed, 24 Feb 2021 20:39:40 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 23:54:22 GMT
ENV NATS_STREAMING_SERVER=0.20.0
# Wed, 24 Feb 2021 23:54:26 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='618008a4902916b6bdb26022343ab91313d4f7fc90b31d0c71ad9e75dc8299e4' ;; 		armhf) natsArch='arm6'; sha256='144b04f8f42793aee1b2deb3f6eb187648c37dcc32d526c607a0af99a847260d' ;; 		armv7) natsArch='arm7'; sha256='720f4a90d1dd536bc04639ae31c70ab46fb3e10556f0f261eb038fdce941f20c' ;; 		x86_64) natsArch='amd64'; sha256='098e2293cce5d457b92f3df35127789422562f1414427c406ffd03ea3bd687c9' ;; 		x86) natsArch='386'; sha256='322a290f4706f14d6ff8160ec437202bd282f61f0607741d0e4c38ef89b83451' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 24 Feb 2021 23:54:27 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Wed, 24 Feb 2021 23:54:28 GMT
EXPOSE 4222 8222
# Wed, 24 Feb 2021 23:54:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 24 Feb 2021 23:54:29 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:dce8679b510e95d136241d02ababff86469dd14220812a7ce9202833c0e32f66`  
		Last Modified: Wed, 24 Feb 2021 20:40:26 GMT  
		Size: 2.7 MB (2709880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64d185e50c4f0cdc2dc88a9f750ebea1210da17133d4339466bd454a3d2d3b5c`  
		Last Modified: Wed, 24 Feb 2021 23:55:03 GMT  
		Size: 5.7 MB (5668417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d70ce809390466c98565d0da9060e5d2d21974101f9ed8caf6bae1982e9cf71`  
		Last Modified: Wed, 24 Feb 2021 23:55:02 GMT  
		Size: 419.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:alpine3.12`

```console
$ docker pull nats-streaming@sha256:3e79d8fb911870f1333bc6bfed2fcd3af9e3090434a40d85c5b2747ad2b33ece
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:alpine3.12` - linux; amd64

```console
$ docker pull nats-streaming@sha256:7e2837da130ab6208e927ba254dd3e66cf3e51c232bff758fdcd6f177e8e4cba
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.0 MB (8997694 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df0e4bfed7e10f0725503851ba4a32fa19cc88f189c2a7bc34d4348b5083e184`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 24 Feb 2021 20:20:03 GMT
ADD file:0dbb1cd66f708f54f7e6663eabf24095fcd53747bfb09912a118a77e737d9617 in / 
# Wed, 24 Feb 2021 20:20:03 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 21:16:41 GMT
ENV NATS_STREAMING_SERVER=0.20.0
# Wed, 24 Feb 2021 21:16:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='618008a4902916b6bdb26022343ab91313d4f7fc90b31d0c71ad9e75dc8299e4' ;; 		armhf) natsArch='arm6'; sha256='144b04f8f42793aee1b2deb3f6eb187648c37dcc32d526c607a0af99a847260d' ;; 		armv7) natsArch='arm7'; sha256='720f4a90d1dd536bc04639ae31c70ab46fb3e10556f0f261eb038fdce941f20c' ;; 		x86_64) natsArch='amd64'; sha256='098e2293cce5d457b92f3df35127789422562f1414427c406ffd03ea3bd687c9' ;; 		x86) natsArch='386'; sha256='322a290f4706f14d6ff8160ec437202bd282f61f0607741d0e4c38ef89b83451' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 24 Feb 2021 21:16:44 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Wed, 24 Feb 2021 21:16:44 GMT
EXPOSE 4222 8222
# Wed, 24 Feb 2021 21:16:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 24 Feb 2021 21:16:45 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:f84cab65f19f5d625a4b5f895cdf37ad9f21e160bf201ec59a48d95b2a430145`  
		Last Modified: Wed, 24 Feb 2021 20:20:39 GMT  
		Size: 2.8 MB (2799493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32044508a232eda00968bedd206428d2540ce9b818a3382269486238d731550c`  
		Last Modified: Wed, 24 Feb 2021 21:17:24 GMT  
		Size: 6.2 MB (6197781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ebefc07ccecb4605491ec038d76ed03335e0a0b0e033be052987c817d713cc0`  
		Last Modified: Wed, 24 Feb 2021 21:17:23 GMT  
		Size: 420.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine3.12` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:71a3dda1dc2ddabf1f7d58456851bb20b66a176c7df12844dd00777365754351
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.3 MB (8331130 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:481fb1c587fe44cb52065c781076c4d64bbe18c9d2856305f951d92d3d564c67`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 24 Feb 2021 20:50:34 GMT
ADD file:8bbb59eeaad0cbcf11559bc6e2b4492aadf6822d1935ed50c710f8bed858b7b5 in / 
# Wed, 24 Feb 2021 20:50:35 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 21:35:57 GMT
ENV NATS_STREAMING_SERVER=0.20.0
# Wed, 24 Feb 2021 21:36:02 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='618008a4902916b6bdb26022343ab91313d4f7fc90b31d0c71ad9e75dc8299e4' ;; 		armhf) natsArch='arm6'; sha256='144b04f8f42793aee1b2deb3f6eb187648c37dcc32d526c607a0af99a847260d' ;; 		armv7) natsArch='arm7'; sha256='720f4a90d1dd536bc04639ae31c70ab46fb3e10556f0f261eb038fdce941f20c' ;; 		x86_64) natsArch='amd64'; sha256='098e2293cce5d457b92f3df35127789422562f1414427c406ffd03ea3bd687c9' ;; 		x86) natsArch='386'; sha256='322a290f4706f14d6ff8160ec437202bd282f61f0607741d0e4c38ef89b83451' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 24 Feb 2021 21:36:03 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Wed, 24 Feb 2021 21:36:04 GMT
EXPOSE 4222 8222
# Wed, 24 Feb 2021 21:36:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 24 Feb 2021 21:36:05 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:55242616b0494f68f44470d864da746cd2a8f8f2d1ffca698114de64032247ef`  
		Last Modified: Wed, 24 Feb 2021 20:51:17 GMT  
		Size: 2.6 MB (2604518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cdc5b3ef2d08f12a32b4290648ce4ccaf53c62b831c0035a86f5f7934af51c5`  
		Last Modified: Wed, 24 Feb 2021 21:36:38 GMT  
		Size: 5.7 MB (5726190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:300ae63bdaa97a87286e7cd46df7562ee6d65fc79d1c59789b077a6efc5a04aa`  
		Last Modified: Wed, 24 Feb 2021 21:36:34 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine3.12` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:5ade3cc881349db3662cc2a32166b001c22214e0c79c0f2f99d0cb785f78cdab
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.1 MB (8125937 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3003c551e23e6c957b25e7c9db011e1cd8170bb14193c185bad20b6f639047f2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 24 Feb 2021 21:03:35 GMT
ADD file:2632f48dd643f8927da2b1af8365b3edb484bd6b7d9fee4009e69f6cf3310e91 in / 
# Wed, 24 Feb 2021 21:03:36 GMT
CMD ["/bin/sh"]
# Thu, 25 Feb 2021 02:03:00 GMT
ENV NATS_STREAMING_SERVER=0.20.0
# Thu, 25 Feb 2021 02:03:07 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='618008a4902916b6bdb26022343ab91313d4f7fc90b31d0c71ad9e75dc8299e4' ;; 		armhf) natsArch='arm6'; sha256='144b04f8f42793aee1b2deb3f6eb187648c37dcc32d526c607a0af99a847260d' ;; 		armv7) natsArch='arm7'; sha256='720f4a90d1dd536bc04639ae31c70ab46fb3e10556f0f261eb038fdce941f20c' ;; 		x86_64) natsArch='amd64'; sha256='098e2293cce5d457b92f3df35127789422562f1414427c406ffd03ea3bd687c9' ;; 		x86) natsArch='386'; sha256='322a290f4706f14d6ff8160ec437202bd282f61f0607741d0e4c38ef89b83451' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 25 Feb 2021 02:03:09 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Thu, 25 Feb 2021 02:03:10 GMT
EXPOSE 4222 8222
# Thu, 25 Feb 2021 02:03:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 25 Feb 2021 02:03:13 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:8e85c7428c31ea48b47424ca0e4663106c54591c83545d32b66a77093f90ffd0`  
		Last Modified: Wed, 24 Feb 2021 21:04:23 GMT  
		Size: 2.4 MB (2408004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e73e11681aeadb2d31fa3245a2d356980142a629503b54745e3dac74b4c6ccb`  
		Last Modified: Thu, 25 Feb 2021 02:04:13 GMT  
		Size: 5.7 MB (5717512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a07ffd0ec2224fc48e7d5a98c442b6a4a4b46730ed88e95871d2d6397f4c9d8`  
		Last Modified: Thu, 25 Feb 2021 02:04:06 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine3.12` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:bd39a673070144b75764fb3a0aad84cdbe8a7c16c9393b294da3d7bdddc223f9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.4 MB (8378716 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:72a01c0cbdeefc26cfc81137d93311ff33253f7d914cd42ffacbcd45725a4ab1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 24 Feb 2021 20:39:39 GMT
ADD file:7e82858ef85f6db90c131ed835a390d736cfdbd1a0cf8bccaeed8f7e30172ddb in / 
# Wed, 24 Feb 2021 20:39:40 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 23:54:22 GMT
ENV NATS_STREAMING_SERVER=0.20.0
# Wed, 24 Feb 2021 23:54:26 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='618008a4902916b6bdb26022343ab91313d4f7fc90b31d0c71ad9e75dc8299e4' ;; 		armhf) natsArch='arm6'; sha256='144b04f8f42793aee1b2deb3f6eb187648c37dcc32d526c607a0af99a847260d' ;; 		armv7) natsArch='arm7'; sha256='720f4a90d1dd536bc04639ae31c70ab46fb3e10556f0f261eb038fdce941f20c' ;; 		x86_64) natsArch='amd64'; sha256='098e2293cce5d457b92f3df35127789422562f1414427c406ffd03ea3bd687c9' ;; 		x86) natsArch='386'; sha256='322a290f4706f14d6ff8160ec437202bd282f61f0607741d0e4c38ef89b83451' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 24 Feb 2021 23:54:27 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Wed, 24 Feb 2021 23:54:28 GMT
EXPOSE 4222 8222
# Wed, 24 Feb 2021 23:54:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 24 Feb 2021 23:54:29 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:dce8679b510e95d136241d02ababff86469dd14220812a7ce9202833c0e32f66`  
		Last Modified: Wed, 24 Feb 2021 20:40:26 GMT  
		Size: 2.7 MB (2709880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64d185e50c4f0cdc2dc88a9f750ebea1210da17133d4339466bd454a3d2d3b5c`  
		Last Modified: Wed, 24 Feb 2021 23:55:03 GMT  
		Size: 5.7 MB (5668417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d70ce809390466c98565d0da9060e5d2d21974101f9ed8caf6bae1982e9cf71`  
		Last Modified: Wed, 24 Feb 2021 23:55:02 GMT  
		Size: 419.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:latest`

```console
$ docker pull nats-streaming@sha256:83e5a79191091b9dfcacc7305ade7103ae29b443f06a973104196aea8b7fb931
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.1757; amd64

### `nats-streaming:latest` - linux; amd64

```console
$ docker pull nats-streaming@sha256:cd0162a7232de1eabe982554c8740e7edbac4747af3e99fa9bc38a480b4a4243
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 MB (5914730 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1544c1524919e1458186fefae5f5ff415c37055742e531010fc2660b11db2339`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 12 Jan 2021 00:48:24 GMT
COPY file:acbca3cec2dc5172f21984b614cbcd90e6e4cf0bd9848c5ddcffb94615a02436 in /nats-streaming-server 
# Tue, 12 Jan 2021 00:48:24 GMT
EXPOSE 4222 8222
# Tue, 12 Jan 2021 00:48:24 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 12 Jan 2021 00:48:24 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:0d51fde6ce3492f397e8a85dad354a9a45ab91310cf4abd6275101f3ef823587`  
		Last Modified: Tue, 12 Jan 2021 00:49:07 GMT  
		Size: 5.9 MB (5914730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:latest` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:bbb3d771f9232932017b9cb9b501734367bc3560eed790695be682d94a8f3573
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.4 MB (5444243 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ed880c2955fd126b0ce38471e90c9467c9c739f55b4c789cec1a4575a41d36f`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 11 Jan 2021 23:53:53 GMT
COPY file:617b9b5366d0d437ce471ad0763bdd7d350496612583dc2c7044dcde4d32257e in /nats-streaming-server 
# Mon, 11 Jan 2021 23:53:54 GMT
EXPOSE 4222 8222
# Mon, 11 Jan 2021 23:53:54 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 11 Jan 2021 23:53:55 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:7cffcff2c5b4913dac660d7456365492a0393b1aa6f1812f6b7b46b250e1970d`  
		Last Modified: Mon, 11 Jan 2021 23:54:39 GMT  
		Size: 5.4 MB (5444243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:latest` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:b2d9250f9a4e3b25b2212f4e8c27c693cc5cfa0f83ca82a8005c90ae8372ab86
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.4 MB (5439328 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:35f1d3c5a1d429a3e2b1fc71f5bc023980c41d34ccb0a0482aca07b6cbb4d6f1`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 12 Jan 2021 00:19:09 GMT
COPY file:2b3fc04f11d3cc7cdfa09f93a79d8efe0889d24324b831fb35126470165c9027 in /nats-streaming-server 
# Tue, 12 Jan 2021 00:19:14 GMT
EXPOSE 4222 8222
# Tue, 12 Jan 2021 00:19:16 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 12 Jan 2021 00:19:17 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:bf50122b11c4b5e2fa295a9456a93489ad25dd1e9bfefda1d572da1a57418205`  
		Last Modified: Tue, 12 Jan 2021 00:20:01 GMT  
		Size: 5.4 MB (5439328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:latest` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:0f315491d4d14e634f971591c7f8bd0eb9aad59975fcdf867a51294df2e5efb2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.4 MB (5388538 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:22dba974517468c29a982c1b4a0b7744a93825122145a1dcc5f7e53c96119efa`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 11 Jan 2021 23:47:25 GMT
COPY file:5a251d4e6bafc9d9ea6f25cd37fd44252da405176da94cc580cdd663abecffa5 in /nats-streaming-server 
# Mon, 11 Jan 2021 23:47:26 GMT
EXPOSE 4222 8222
# Mon, 11 Jan 2021 23:47:26 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 11 Jan 2021 23:47:27 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:58239a1ea6494e431645c7ad156ed917333a248edbe6be76af8b7384d9339f07`  
		Last Modified: Mon, 11 Jan 2021 23:48:09 GMT  
		Size: 5.4 MB (5388538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:latest` - windows version 10.0.17763.1757; amd64

```console
$ docker pull nats-streaming@sha256:d13b43d591f725a510ae54f0f2efa114399a0a0c9e85f0652bc802e7e8d45187
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.4 MB (107432722 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc67b6d7f9c859b2a9e9272dfda84571744e233c3ada49fdd3505d40e586c859`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 02 Feb 2021 13:06:30 GMT
RUN Apply image 1809-amd64
# Wed, 10 Feb 2021 16:02:26 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 10 Feb 2021 20:00:55 GMT
RUN cmd /S /C #(nop) COPY file:f2450ffeda74e33f820191eccf78b6647ce56865170e966bfa8e72afe6e46c36 in C:\nats-streaming-server.exe 
# Wed, 10 Feb 2021 20:00:56 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 10 Feb 2021 20:00:57 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 10 Feb 2021 20:00:57 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:ba17af31b9276ee11fdf859681b442db50979a39eff4cea2a559a5755cedbe01`  
		Size: 101.4 MB (101406193 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:23b613036f8aee9066e712b3aa58f10f2fde093623511a5658867f53a6d01b18`  
		Last Modified: Wed, 10 Feb 2021 16:06:34 GMT  
		Size: 1.1 KB (1071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:546c4d75ec4cbc867ea01774757b0a9303906569a30157fd804f8c1bc5d4e63e`  
		Last Modified: Wed, 10 Feb 2021 20:06:15 GMT  
		Size: 6.0 MB (6022164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d942fdcd6082f7ac407761ffc6d739677d6fe08f0f51db38d32d33398e9073f`  
		Last Modified: Wed, 10 Feb 2021 20:06:07 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2c29c3e2255d5f0292ecd161299cb57afc896ff1c7002836b53577f1d57e6fe`  
		Last Modified: Wed, 10 Feb 2021 20:06:07 GMT  
		Size: 1.1 KB (1097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12923e759dcf1b0d858f5bfacd7f73cffa442500803639aa349428d981cd881f`  
		Last Modified: Wed, 10 Feb 2021 20:06:07 GMT  
		Size: 1.1 KB (1072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:linux`

```console
$ docker pull nats-streaming@sha256:f46b63443b02bc0089e72301ae260b1ef32ff25e755e67b633169945585ca12d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:linux` - linux; amd64

```console
$ docker pull nats-streaming@sha256:cd0162a7232de1eabe982554c8740e7edbac4747af3e99fa9bc38a480b4a4243
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 MB (5914730 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1544c1524919e1458186fefae5f5ff415c37055742e531010fc2660b11db2339`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 12 Jan 2021 00:48:24 GMT
COPY file:acbca3cec2dc5172f21984b614cbcd90e6e4cf0bd9848c5ddcffb94615a02436 in /nats-streaming-server 
# Tue, 12 Jan 2021 00:48:24 GMT
EXPOSE 4222 8222
# Tue, 12 Jan 2021 00:48:24 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 12 Jan 2021 00:48:24 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:0d51fde6ce3492f397e8a85dad354a9a45ab91310cf4abd6275101f3ef823587`  
		Last Modified: Tue, 12 Jan 2021 00:49:07 GMT  
		Size: 5.9 MB (5914730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:linux` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:bbb3d771f9232932017b9cb9b501734367bc3560eed790695be682d94a8f3573
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.4 MB (5444243 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ed880c2955fd126b0ce38471e90c9467c9c739f55b4c789cec1a4575a41d36f`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 11 Jan 2021 23:53:53 GMT
COPY file:617b9b5366d0d437ce471ad0763bdd7d350496612583dc2c7044dcde4d32257e in /nats-streaming-server 
# Mon, 11 Jan 2021 23:53:54 GMT
EXPOSE 4222 8222
# Mon, 11 Jan 2021 23:53:54 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 11 Jan 2021 23:53:55 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:7cffcff2c5b4913dac660d7456365492a0393b1aa6f1812f6b7b46b250e1970d`  
		Last Modified: Mon, 11 Jan 2021 23:54:39 GMT  
		Size: 5.4 MB (5444243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:linux` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:b2d9250f9a4e3b25b2212f4e8c27c693cc5cfa0f83ca82a8005c90ae8372ab86
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.4 MB (5439328 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:35f1d3c5a1d429a3e2b1fc71f5bc023980c41d34ccb0a0482aca07b6cbb4d6f1`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 12 Jan 2021 00:19:09 GMT
COPY file:2b3fc04f11d3cc7cdfa09f93a79d8efe0889d24324b831fb35126470165c9027 in /nats-streaming-server 
# Tue, 12 Jan 2021 00:19:14 GMT
EXPOSE 4222 8222
# Tue, 12 Jan 2021 00:19:16 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 12 Jan 2021 00:19:17 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:bf50122b11c4b5e2fa295a9456a93489ad25dd1e9bfefda1d572da1a57418205`  
		Last Modified: Tue, 12 Jan 2021 00:20:01 GMT  
		Size: 5.4 MB (5439328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:linux` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:0f315491d4d14e634f971591c7f8bd0eb9aad59975fcdf867a51294df2e5efb2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.4 MB (5388538 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:22dba974517468c29a982c1b4a0b7744a93825122145a1dcc5f7e53c96119efa`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 11 Jan 2021 23:47:25 GMT
COPY file:5a251d4e6bafc9d9ea6f25cd37fd44252da405176da94cc580cdd663abecffa5 in /nats-streaming-server 
# Mon, 11 Jan 2021 23:47:26 GMT
EXPOSE 4222 8222
# Mon, 11 Jan 2021 23:47:26 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 11 Jan 2021 23:47:27 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:58239a1ea6494e431645c7ad156ed917333a248edbe6be76af8b7384d9339f07`  
		Last Modified: Mon, 11 Jan 2021 23:48:09 GMT  
		Size: 5.4 MB (5388538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:nanoserver`

```console
$ docker pull nats-streaming@sha256:b89cba5cf792b4be014bbb1be1a2fbca1c0019946c989c8a903c7ed865c0e7d8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1757; amd64

### `nats-streaming:nanoserver` - windows version 10.0.17763.1757; amd64

```console
$ docker pull nats-streaming@sha256:d13b43d591f725a510ae54f0f2efa114399a0a0c9e85f0652bc802e7e8d45187
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.4 MB (107432722 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc67b6d7f9c859b2a9e9272dfda84571744e233c3ada49fdd3505d40e586c859`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 02 Feb 2021 13:06:30 GMT
RUN Apply image 1809-amd64
# Wed, 10 Feb 2021 16:02:26 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 10 Feb 2021 20:00:55 GMT
RUN cmd /S /C #(nop) COPY file:f2450ffeda74e33f820191eccf78b6647ce56865170e966bfa8e72afe6e46c36 in C:\nats-streaming-server.exe 
# Wed, 10 Feb 2021 20:00:56 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 10 Feb 2021 20:00:57 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 10 Feb 2021 20:00:57 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:ba17af31b9276ee11fdf859681b442db50979a39eff4cea2a559a5755cedbe01`  
		Size: 101.4 MB (101406193 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:23b613036f8aee9066e712b3aa58f10f2fde093623511a5658867f53a6d01b18`  
		Last Modified: Wed, 10 Feb 2021 16:06:34 GMT  
		Size: 1.1 KB (1071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:546c4d75ec4cbc867ea01774757b0a9303906569a30157fd804f8c1bc5d4e63e`  
		Last Modified: Wed, 10 Feb 2021 20:06:15 GMT  
		Size: 6.0 MB (6022164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d942fdcd6082f7ac407761ffc6d739677d6fe08f0f51db38d32d33398e9073f`  
		Last Modified: Wed, 10 Feb 2021 20:06:07 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2c29c3e2255d5f0292ecd161299cb57afc896ff1c7002836b53577f1d57e6fe`  
		Last Modified: Wed, 10 Feb 2021 20:06:07 GMT  
		Size: 1.1 KB (1097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12923e759dcf1b0d858f5bfacd7f73cffa442500803639aa349428d981cd881f`  
		Last Modified: Wed, 10 Feb 2021 20:06:07 GMT  
		Size: 1.1 KB (1072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:nanoserver-1809`

```console
$ docker pull nats-streaming@sha256:b89cba5cf792b4be014bbb1be1a2fbca1c0019946c989c8a903c7ed865c0e7d8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1757; amd64

### `nats-streaming:nanoserver-1809` - windows version 10.0.17763.1757; amd64

```console
$ docker pull nats-streaming@sha256:d13b43d591f725a510ae54f0f2efa114399a0a0c9e85f0652bc802e7e8d45187
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.4 MB (107432722 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc67b6d7f9c859b2a9e9272dfda84571744e233c3ada49fdd3505d40e586c859`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 02 Feb 2021 13:06:30 GMT
RUN Apply image 1809-amd64
# Wed, 10 Feb 2021 16:02:26 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 10 Feb 2021 20:00:55 GMT
RUN cmd /S /C #(nop) COPY file:f2450ffeda74e33f820191eccf78b6647ce56865170e966bfa8e72afe6e46c36 in C:\nats-streaming-server.exe 
# Wed, 10 Feb 2021 20:00:56 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 10 Feb 2021 20:00:57 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 10 Feb 2021 20:00:57 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:ba17af31b9276ee11fdf859681b442db50979a39eff4cea2a559a5755cedbe01`  
		Size: 101.4 MB (101406193 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:23b613036f8aee9066e712b3aa58f10f2fde093623511a5658867f53a6d01b18`  
		Last Modified: Wed, 10 Feb 2021 16:06:34 GMT  
		Size: 1.1 KB (1071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:546c4d75ec4cbc867ea01774757b0a9303906569a30157fd804f8c1bc5d4e63e`  
		Last Modified: Wed, 10 Feb 2021 20:06:15 GMT  
		Size: 6.0 MB (6022164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d942fdcd6082f7ac407761ffc6d739677d6fe08f0f51db38d32d33398e9073f`  
		Last Modified: Wed, 10 Feb 2021 20:06:07 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2c29c3e2255d5f0292ecd161299cb57afc896ff1c7002836b53577f1d57e6fe`  
		Last Modified: Wed, 10 Feb 2021 20:06:07 GMT  
		Size: 1.1 KB (1097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12923e759dcf1b0d858f5bfacd7f73cffa442500803639aa349428d981cd881f`  
		Last Modified: Wed, 10 Feb 2021 20:06:07 GMT  
		Size: 1.1 KB (1072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:scratch`

```console
$ docker pull nats-streaming@sha256:f46b63443b02bc0089e72301ae260b1ef32ff25e755e67b633169945585ca12d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:scratch` - linux; amd64

```console
$ docker pull nats-streaming@sha256:cd0162a7232de1eabe982554c8740e7edbac4747af3e99fa9bc38a480b4a4243
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 MB (5914730 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1544c1524919e1458186fefae5f5ff415c37055742e531010fc2660b11db2339`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 12 Jan 2021 00:48:24 GMT
COPY file:acbca3cec2dc5172f21984b614cbcd90e6e4cf0bd9848c5ddcffb94615a02436 in /nats-streaming-server 
# Tue, 12 Jan 2021 00:48:24 GMT
EXPOSE 4222 8222
# Tue, 12 Jan 2021 00:48:24 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 12 Jan 2021 00:48:24 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:0d51fde6ce3492f397e8a85dad354a9a45ab91310cf4abd6275101f3ef823587`  
		Last Modified: Tue, 12 Jan 2021 00:49:07 GMT  
		Size: 5.9 MB (5914730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:scratch` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:bbb3d771f9232932017b9cb9b501734367bc3560eed790695be682d94a8f3573
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.4 MB (5444243 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ed880c2955fd126b0ce38471e90c9467c9c739f55b4c789cec1a4575a41d36f`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 11 Jan 2021 23:53:53 GMT
COPY file:617b9b5366d0d437ce471ad0763bdd7d350496612583dc2c7044dcde4d32257e in /nats-streaming-server 
# Mon, 11 Jan 2021 23:53:54 GMT
EXPOSE 4222 8222
# Mon, 11 Jan 2021 23:53:54 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 11 Jan 2021 23:53:55 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:7cffcff2c5b4913dac660d7456365492a0393b1aa6f1812f6b7b46b250e1970d`  
		Last Modified: Mon, 11 Jan 2021 23:54:39 GMT  
		Size: 5.4 MB (5444243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:scratch` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:b2d9250f9a4e3b25b2212f4e8c27c693cc5cfa0f83ca82a8005c90ae8372ab86
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.4 MB (5439328 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:35f1d3c5a1d429a3e2b1fc71f5bc023980c41d34ccb0a0482aca07b6cbb4d6f1`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 12 Jan 2021 00:19:09 GMT
COPY file:2b3fc04f11d3cc7cdfa09f93a79d8efe0889d24324b831fb35126470165c9027 in /nats-streaming-server 
# Tue, 12 Jan 2021 00:19:14 GMT
EXPOSE 4222 8222
# Tue, 12 Jan 2021 00:19:16 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 12 Jan 2021 00:19:17 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:bf50122b11c4b5e2fa295a9456a93489ad25dd1e9bfefda1d572da1a57418205`  
		Last Modified: Tue, 12 Jan 2021 00:20:01 GMT  
		Size: 5.4 MB (5439328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:scratch` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:0f315491d4d14e634f971591c7f8bd0eb9aad59975fcdf867a51294df2e5efb2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.4 MB (5388538 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:22dba974517468c29a982c1b4a0b7744a93825122145a1dcc5f7e53c96119efa`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 11 Jan 2021 23:47:25 GMT
COPY file:5a251d4e6bafc9d9ea6f25cd37fd44252da405176da94cc580cdd663abecffa5 in /nats-streaming-server 
# Mon, 11 Jan 2021 23:47:26 GMT
EXPOSE 4222 8222
# Mon, 11 Jan 2021 23:47:26 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 11 Jan 2021 23:47:27 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:58239a1ea6494e431645c7ad156ed917333a248edbe6be76af8b7384d9339f07`  
		Last Modified: Mon, 11 Jan 2021 23:48:09 GMT  
		Size: 5.4 MB (5388538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:windowsservercore`

```console
$ docker pull nats-streaming@sha256:f5c17fa3628e9e6d4f4a960b80c4f905b48409dc7f7227d9b2b53652d5e03311
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1757; amd64
	-	windows version 10.0.14393.4225; amd64

### `nats-streaming:windowsservercore` - windows version 10.0.17763.1757; amd64

```console
$ docker pull nats-streaming@sha256:54ce906f88c84ed2e364f31fcda6fb3c162926540ce48e90f579231a6abfb48f
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2459695608 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6680b77bb43567b839fdc0da0fafd3fba6903bb3e96f903ac356ba5a31f4556`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 06 Feb 2021 05:03:14 GMT
RUN Install update 1809-amd64
# Tue, 09 Feb 2021 20:26:38 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Feb 2021 16:00:30 GMT
ENV NATS_DOCKERIZED=1
# Wed, 10 Feb 2021 19:58:59 GMT
ENV NATS_STREAMING_SERVER=0.20.0
# Wed, 10 Feb 2021 19:58:59 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.20.0/nats-streaming-server-v0.20.0-windows-amd64.zip
# Wed, 10 Feb 2021 19:59:00 GMT
ENV GIT_DOWNLOAD_SHA256=26ae310d3ec11617d380106a769236a6dc2209769c0c36d15cb6736db1b589cb
# Wed, 10 Feb 2021 19:59:29 GMT
RUN Set-PSDebug -Trace 2
# Wed, 10 Feb 2021 20:00:45 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 10 Feb 2021 20:00:45 GMT
EXPOSE 4222 8222
# Wed, 10 Feb 2021 20:00:46 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 10 Feb 2021 20:00:47 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:db4edcf0861ff3fdc41851a5a218965ecb2ab6cf4ec9448fb80cc4b6792fd46c`  
		Size: 720.9 MB (720933935 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:751b8860e89a7e6999d74a11dc393620b118057ad881cb87f1d6e3653cb2db43`  
		Last Modified: Tue, 09 Feb 2021 20:48:09 GMT  
		Size: 1.3 KB (1337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7f01e717591f83c73890556e7a4c77e53caed8daf6c9b0150f497e094a4a698`  
		Last Modified: Wed, 10 Feb 2021 16:06:05 GMT  
		Size: 1.4 KB (1361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58b9fd76bfcc3923f270750c61e7e97a3aef114253089eaa76dc10c9646d423e`  
		Last Modified: Wed, 10 Feb 2021 20:04:42 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dedbaf4d01c80583ca29d8dbe57d676028feb67a3a05585bb4a6023db1e594d`  
		Last Modified: Wed, 10 Feb 2021 20:04:42 GMT  
		Size: 1.4 KB (1356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b3c1ad5a715163ac2b7a339e423a01f3f4f0b15a573766d89a61ba55a986ad0`  
		Last Modified: Wed, 10 Feb 2021 20:04:42 GMT  
		Size: 1.3 KB (1329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db42b5fd63b27df3e466b97a15dc186ad636cbdd8329490877acd12f3ea19d79`  
		Last Modified: Wed, 10 Feb 2021 20:04:41 GMT  
		Size: 5.0 MB (5027472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b65ae3b9922d83438f901016cdfc11b6b3a61c6b9e808c96d2d2e05680ea042`  
		Last Modified: Wed, 10 Feb 2021 20:04:44 GMT  
		Size: 15.4 MB (15390555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:019886058fe88defbb509d8045d2f7a5d345e2dfefec33c626894401ca5bb5b7`  
		Last Modified: Wed, 10 Feb 2021 20:04:40 GMT  
		Size: 1.3 KB (1335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98167084c5ae01ebb43d46418db9814ab5794cf8c2295f38c6def03ddc1427d9`  
		Last Modified: Wed, 10 Feb 2021 20:04:40 GMT  
		Size: 1.3 KB (1326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ef3dff4857898fe4a1c9877ddf0c7173d892e69faa0e651a99be642cfb57790`  
		Last Modified: Wed, 10 Feb 2021 20:04:40 GMT  
		Size: 1.4 KB (1361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:windowsservercore` - windows version 10.0.14393.4225; amd64

```console
$ docker pull nats-streaming@sha256:51668710b962ea70261499d873828a7b752f13c47a599f71e9199c0e1a7bf9a9
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5816886127 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a297d5a9a88f97d8c01f02171e4e2b9a45cb7e428c1e45796b3f80622ba1dfa8`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 27 Jan 2021 18:11:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 09 Feb 2021 20:28:50 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Feb 2021 16:02:35 GMT
ENV NATS_DOCKERIZED=1
# Wed, 10 Feb 2021 20:01:03 GMT
ENV NATS_STREAMING_SERVER=0.20.0
# Wed, 10 Feb 2021 20:01:03 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.20.0/nats-streaming-server-v0.20.0-windows-amd64.zip
# Wed, 10 Feb 2021 20:01:04 GMT
ENV GIT_DOWNLOAD_SHA256=26ae310d3ec11617d380106a769236a6dc2209769c0c36d15cb6736db1b589cb
# Wed, 10 Feb 2021 20:02:12 GMT
RUN Set-PSDebug -Trace 2
# Wed, 10 Feb 2021 20:04:03 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 10 Feb 2021 20:04:04 GMT
EXPOSE 4222 8222
# Wed, 10 Feb 2021 20:04:04 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 10 Feb 2021 20:04:05 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:62c48323ed8ac695b8cbe0ecedcc28ba185a234673ad9241df2b151dd00f9181`  
		Size: 1.7 GB (1725027107 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ac4a230905430e1aea27172a9432f576cc4a530e72bea516a2b304d2b7e9c101`  
		Last Modified: Tue, 09 Feb 2021 20:49:11 GMT  
		Size: 1.4 KB (1356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cc28e30e89dab2d0b2b2f6c3114771d9d803d5942c730de78d2dd457ad4ac40`  
		Last Modified: Wed, 10 Feb 2021 16:06:59 GMT  
		Size: 1.4 KB (1361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05764ae13ea6854b6abb1163dedcdbec24b30ea512599f3b60542072b923f063`  
		Last Modified: Wed, 10 Feb 2021 20:06:35 GMT  
		Size: 1.4 KB (1356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14a0242de998d983dbd8cb540a0928e5d89da6be0e231d561adba835f166061a`  
		Last Modified: Wed, 10 Feb 2021 20:06:34 GMT  
		Size: 1.3 KB (1342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c60afc4477c8f67e49cc93415eea7dab8759b9682360b8c9ec52886870a603a`  
		Last Modified: Wed, 10 Feb 2021 20:06:34 GMT  
		Size: 1.4 KB (1354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca406b9360ad583b7e00b3cd19f865b72ed7cb994b2de91a0611a44ebe20fa4a`  
		Last Modified: Wed, 10 Feb 2021 20:06:32 GMT  
		Size: 5.7 MB (5656542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0319e1b15ceaaa34e58bfb5a047c9330bf2c36c0daff41d260ca00046a68e2f7`  
		Last Modified: Wed, 10 Feb 2021 20:06:35 GMT  
		Size: 16.2 MB (16205763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d04607dfd13c95014c417374cea53b46af10028ac7816011f611e530442564f`  
		Last Modified: Wed, 10 Feb 2021 20:06:31 GMT  
		Size: 1.3 KB (1333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f6fb81a24254dafc4514d4692cf0d4f651294223ab39d2b07a7c69e738e5e32`  
		Last Modified: Wed, 10 Feb 2021 20:06:32 GMT  
		Size: 1.4 KB (1351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:042f35c5ee10f438bce2ba60b486efa0cb59d803951cdd7e833fcb2b306e8e8e`  
		Last Modified: Wed, 10 Feb 2021 20:06:31 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:windowsservercore-1809`

```console
$ docker pull nats-streaming@sha256:d484366d41ec5afe4c5f2dc2ad3f47e3a800a56d86ee682115591711827aebfd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1757; amd64

### `nats-streaming:windowsservercore-1809` - windows version 10.0.17763.1757; amd64

```console
$ docker pull nats-streaming@sha256:54ce906f88c84ed2e364f31fcda6fb3c162926540ce48e90f579231a6abfb48f
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2459695608 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6680b77bb43567b839fdc0da0fafd3fba6903bb3e96f903ac356ba5a31f4556`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 06 Feb 2021 05:03:14 GMT
RUN Install update 1809-amd64
# Tue, 09 Feb 2021 20:26:38 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Feb 2021 16:00:30 GMT
ENV NATS_DOCKERIZED=1
# Wed, 10 Feb 2021 19:58:59 GMT
ENV NATS_STREAMING_SERVER=0.20.0
# Wed, 10 Feb 2021 19:58:59 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.20.0/nats-streaming-server-v0.20.0-windows-amd64.zip
# Wed, 10 Feb 2021 19:59:00 GMT
ENV GIT_DOWNLOAD_SHA256=26ae310d3ec11617d380106a769236a6dc2209769c0c36d15cb6736db1b589cb
# Wed, 10 Feb 2021 19:59:29 GMT
RUN Set-PSDebug -Trace 2
# Wed, 10 Feb 2021 20:00:45 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 10 Feb 2021 20:00:45 GMT
EXPOSE 4222 8222
# Wed, 10 Feb 2021 20:00:46 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 10 Feb 2021 20:00:47 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:db4edcf0861ff3fdc41851a5a218965ecb2ab6cf4ec9448fb80cc4b6792fd46c`  
		Size: 720.9 MB (720933935 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:751b8860e89a7e6999d74a11dc393620b118057ad881cb87f1d6e3653cb2db43`  
		Last Modified: Tue, 09 Feb 2021 20:48:09 GMT  
		Size: 1.3 KB (1337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7f01e717591f83c73890556e7a4c77e53caed8daf6c9b0150f497e094a4a698`  
		Last Modified: Wed, 10 Feb 2021 16:06:05 GMT  
		Size: 1.4 KB (1361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58b9fd76bfcc3923f270750c61e7e97a3aef114253089eaa76dc10c9646d423e`  
		Last Modified: Wed, 10 Feb 2021 20:04:42 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dedbaf4d01c80583ca29d8dbe57d676028feb67a3a05585bb4a6023db1e594d`  
		Last Modified: Wed, 10 Feb 2021 20:04:42 GMT  
		Size: 1.4 KB (1356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b3c1ad5a715163ac2b7a339e423a01f3f4f0b15a573766d89a61ba55a986ad0`  
		Last Modified: Wed, 10 Feb 2021 20:04:42 GMT  
		Size: 1.3 KB (1329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db42b5fd63b27df3e466b97a15dc186ad636cbdd8329490877acd12f3ea19d79`  
		Last Modified: Wed, 10 Feb 2021 20:04:41 GMT  
		Size: 5.0 MB (5027472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b65ae3b9922d83438f901016cdfc11b6b3a61c6b9e808c96d2d2e05680ea042`  
		Last Modified: Wed, 10 Feb 2021 20:04:44 GMT  
		Size: 15.4 MB (15390555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:019886058fe88defbb509d8045d2f7a5d345e2dfefec33c626894401ca5bb5b7`  
		Last Modified: Wed, 10 Feb 2021 20:04:40 GMT  
		Size: 1.3 KB (1335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98167084c5ae01ebb43d46418db9814ab5794cf8c2295f38c6def03ddc1427d9`  
		Last Modified: Wed, 10 Feb 2021 20:04:40 GMT  
		Size: 1.3 KB (1326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ef3dff4857898fe4a1c9877ddf0c7173d892e69faa0e651a99be642cfb57790`  
		Last Modified: Wed, 10 Feb 2021 20:04:40 GMT  
		Size: 1.4 KB (1361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:windowsservercore-ltsc2016`

```console
$ docker pull nats-streaming@sha256:b84cb6e0d77ade20c0cde41401c881134555257e2b94afedbf2b7bf93a05bdbe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4225; amd64

### `nats-streaming:windowsservercore-ltsc2016` - windows version 10.0.14393.4225; amd64

```console
$ docker pull nats-streaming@sha256:51668710b962ea70261499d873828a7b752f13c47a599f71e9199c0e1a7bf9a9
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5816886127 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a297d5a9a88f97d8c01f02171e4e2b9a45cb7e428c1e45796b3f80622ba1dfa8`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 27 Jan 2021 18:11:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 09 Feb 2021 20:28:50 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Feb 2021 16:02:35 GMT
ENV NATS_DOCKERIZED=1
# Wed, 10 Feb 2021 20:01:03 GMT
ENV NATS_STREAMING_SERVER=0.20.0
# Wed, 10 Feb 2021 20:01:03 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.20.0/nats-streaming-server-v0.20.0-windows-amd64.zip
# Wed, 10 Feb 2021 20:01:04 GMT
ENV GIT_DOWNLOAD_SHA256=26ae310d3ec11617d380106a769236a6dc2209769c0c36d15cb6736db1b589cb
# Wed, 10 Feb 2021 20:02:12 GMT
RUN Set-PSDebug -Trace 2
# Wed, 10 Feb 2021 20:04:03 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 10 Feb 2021 20:04:04 GMT
EXPOSE 4222 8222
# Wed, 10 Feb 2021 20:04:04 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 10 Feb 2021 20:04:05 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:62c48323ed8ac695b8cbe0ecedcc28ba185a234673ad9241df2b151dd00f9181`  
		Size: 1.7 GB (1725027107 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ac4a230905430e1aea27172a9432f576cc4a530e72bea516a2b304d2b7e9c101`  
		Last Modified: Tue, 09 Feb 2021 20:49:11 GMT  
		Size: 1.4 KB (1356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cc28e30e89dab2d0b2b2f6c3114771d9d803d5942c730de78d2dd457ad4ac40`  
		Last Modified: Wed, 10 Feb 2021 16:06:59 GMT  
		Size: 1.4 KB (1361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05764ae13ea6854b6abb1163dedcdbec24b30ea512599f3b60542072b923f063`  
		Last Modified: Wed, 10 Feb 2021 20:06:35 GMT  
		Size: 1.4 KB (1356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14a0242de998d983dbd8cb540a0928e5d89da6be0e231d561adba835f166061a`  
		Last Modified: Wed, 10 Feb 2021 20:06:34 GMT  
		Size: 1.3 KB (1342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c60afc4477c8f67e49cc93415eea7dab8759b9682360b8c9ec52886870a603a`  
		Last Modified: Wed, 10 Feb 2021 20:06:34 GMT  
		Size: 1.4 KB (1354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca406b9360ad583b7e00b3cd19f865b72ed7cb994b2de91a0611a44ebe20fa4a`  
		Last Modified: Wed, 10 Feb 2021 20:06:32 GMT  
		Size: 5.7 MB (5656542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0319e1b15ceaaa34e58bfb5a047c9330bf2c36c0daff41d260ca00046a68e2f7`  
		Last Modified: Wed, 10 Feb 2021 20:06:35 GMT  
		Size: 16.2 MB (16205763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d04607dfd13c95014c417374cea53b46af10028ac7816011f611e530442564f`  
		Last Modified: Wed, 10 Feb 2021 20:06:31 GMT  
		Size: 1.3 KB (1333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f6fb81a24254dafc4514d4692cf0d4f651294223ab39d2b07a7c69e738e5e32`  
		Last Modified: Wed, 10 Feb 2021 20:06:32 GMT  
		Size: 1.4 KB (1351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:042f35c5ee10f438bce2ba60b486efa0cb59d803951cdd7e833fcb2b306e8e8e`  
		Last Modified: Wed, 10 Feb 2021 20:06:31 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
