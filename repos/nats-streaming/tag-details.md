<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `nats-streaming`

-	[`nats-streaming:0.19`](#nats-streaming019)
-	[`nats-streaming:0.19.0`](#nats-streaming0190)
-	[`nats-streaming:0.19.0-alpine`](#nats-streaming0190-alpine)
-	[`nats-streaming:0.19.0-alpine3.12`](#nats-streaming0190-alpine312)
-	[`nats-streaming:0.19.0-linux`](#nats-streaming0190-linux)
-	[`nats-streaming:0.19.0-nanoserver`](#nats-streaming0190-nanoserver)
-	[`nats-streaming:0.19.0-nanoserver-1809`](#nats-streaming0190-nanoserver-1809)
-	[`nats-streaming:0.19.0-scratch`](#nats-streaming0190-scratch)
-	[`nats-streaming:0.19.0-windowsservercore`](#nats-streaming0190-windowsservercore)
-	[`nats-streaming:0.19.0-windowsservercore-1809`](#nats-streaming0190-windowsservercore-1809)
-	[`nats-streaming:0.19.0-windowsservercore-ltsc2016`](#nats-streaming0190-windowsservercore-ltsc2016)
-	[`nats-streaming:0.19-alpine`](#nats-streaming019-alpine)
-	[`nats-streaming:0.19-alpine3.12`](#nats-streaming019-alpine312)
-	[`nats-streaming:0.19-linux`](#nats-streaming019-linux)
-	[`nats-streaming:0.19-nanoserver`](#nats-streaming019-nanoserver)
-	[`nats-streaming:0.19-nanoserver-1809`](#nats-streaming019-nanoserver-1809)
-	[`nats-streaming:0.19-scratch`](#nats-streaming019-scratch)
-	[`nats-streaming:0.19-windowsservercore`](#nats-streaming019-windowsservercore)
-	[`nats-streaming:0.19-windowsservercore-1809`](#nats-streaming019-windowsservercore-1809)
-	[`nats-streaming:0.19-windowsservercore-ltsc2016`](#nats-streaming019-windowsservercore-ltsc2016)
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

## `nats-streaming:0.19`

```console
$ docker pull nats-streaming@sha256:c8bb32720403c22b091541677c2cdd4e827e65bcf1f25ecf5aaa3acfda90f7d5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.1637; amd64

### `nats-streaming:0.19` - linux; amd64

```console
$ docker pull nats-streaming@sha256:053a4ca3955b9c5036e48bafb96c83003fe86c34c6928934e3fd1db0529a889c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 MB (6487259 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:993a204b53252cabfc16952c1d2dc014dc6518d1a08d00bda1bc5008a139e37a`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 03 Nov 2020 00:33:13 GMT
COPY file:3ed83d1497b0535960e452435cb8b27e347f48da12693aa27ebaf9bff94d82de in /nats-streaming-server 
# Tue, 03 Nov 2020 00:33:13 GMT
EXPOSE 4222 8222
# Tue, 03 Nov 2020 00:33:14 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 03 Nov 2020 00:33:14 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:57ac21f890a508f609eabea265197b18ce9dfe3e694034c7a06d37b536a707b2`  
		Last Modified: Tue, 03 Nov 2020 00:33:37 GMT  
		Size: 6.5 MB (6487259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.19` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:f334d10ef2a4663d8d7d920d96321cd97f050b82a5d55d588192f074f60dd814
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 MB (6049845 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9eecfd5ab4178a65e952a7cf1d248a556a6ae2c328ac8b68923146d64734db03`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 02 Nov 2020 23:56:28 GMT
COPY file:d6896b1c93dcd497494c972f9274fcc634a4f4a8d63a0191bdb87f6336aec0d7 in /nats-streaming-server 
# Mon, 02 Nov 2020 23:56:28 GMT
EXPOSE 4222 8222
# Mon, 02 Nov 2020 23:56:29 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 02 Nov 2020 23:56:29 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:7f165fb71ab77e8081dbfa13656cdf9e5e005002d6c3afa0aac40667a0f97af8`  
		Last Modified: Mon, 02 Nov 2020 23:57:04 GMT  
		Size: 6.0 MB (6049845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.19` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:5fd0943909d8aedafb888e099c9f64d234023ad780805ed7c939692ebfd8304d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 MB (6043163 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f37071e856ae40dc3c8c5e10b359d1640fd67a6110741c0957af2031032ed6ce`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 03 Nov 2020 00:05:23 GMT
COPY file:d232132ddff1d85d3a2f5c80a91c80023cbc103d816387e06d604cf97238e52c in /nats-streaming-server 
# Tue, 03 Nov 2020 00:05:24 GMT
EXPOSE 4222 8222
# Tue, 03 Nov 2020 00:05:24 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 03 Nov 2020 00:05:25 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:9c7227cc1040d04ca7763cfb53ab58bc32ae54921990516adf8e13374ac9ef29`  
		Last Modified: Tue, 03 Nov 2020 00:05:57 GMT  
		Size: 6.0 MB (6043163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.19` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:c058fd3e9a8ac44263bf53fa2f6f1e8e8cb3e95cd223f8353fdafc50fe57e417
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 MB (5978846 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7c915a80bd440362bd4a6743fee8134a3caf6271e3258e449fb106b19c050a3b`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 03 Nov 2020 00:43:38 GMT
COPY file:55e70ee826cd5a662497337a2488e22833672bd031d85b4ee39556ab1e80df08 in /nats-streaming-server 
# Tue, 03 Nov 2020 00:43:40 GMT
EXPOSE 4222 8222
# Tue, 03 Nov 2020 00:43:42 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 03 Nov 2020 00:43:43 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:3dc58a59de8a6ed19e9144b0189eb3b637a9e7fcd76ec6c6dc47561b2740a3a2`  
		Last Modified: Tue, 03 Nov 2020 00:44:19 GMT  
		Size: 6.0 MB (5978846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.19` - windows version 10.0.17763.1637; amd64

```console
$ docker pull nats-streaming@sha256:9444afab14740d43bfd213340272edcfaa96f83b2ae24d586333398cc089a858
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.8 MB (107783475 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:85bdcab4235f3b70b1671972c4154790bde79e33644ae254ae48efa965b2b3cb`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 03 Dec 2020 08:05:47 GMT
RUN Apply image 1809-amd64
# Wed, 09 Dec 2020 17:38:01 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 09 Dec 2020 23:04:19 GMT
RUN cmd /S /C #(nop) COPY file:cc6bae0f50b6e35b12e8233f240d95e093f7e44257bc87e06aed691866ec1477 in C:\nats-streaming-server.exe 
# Wed, 09 Dec 2020 23:04:21 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 09 Dec 2020 23:04:21 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 09 Dec 2020 23:04:22 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:21be49aa856f07be4e0a677b988e43c04bd595a3c858e58b6c364477bbbf7222`  
		Size: 101.3 MB (101264827 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8a3891744a5ba41f01e625a0a70d755ffe93de4d4f124ad6d069420d5c7956d4`  
		Last Modified: Wed, 09 Dec 2020 17:42:32 GMT  
		Size: 893.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab2cf2a7f92a640dc1125e539b41a28abc6b4e2df892f67cbc0072f90bb65509`  
		Last Modified: Wed, 09 Dec 2020 23:08:42 GMT  
		Size: 6.5 MB (6515155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf561da2a706a067845b617e3efccdaf8257da5fb1ae53c383e29559f5220612`  
		Last Modified: Wed, 09 Dec 2020 23:08:41 GMT  
		Size: 869.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1e5e4a71ea08fded20e3471625c1c06c12540fd3c7f4e12eeaee288bf6e5377`  
		Last Modified: Wed, 09 Dec 2020 23:08:39 GMT  
		Size: 864.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5d7a7dbf47aa9dfd9ed44ec162d12b58d6751c6d5f129c4e65250e21fde3631`  
		Last Modified: Wed, 09 Dec 2020 23:08:41 GMT  
		Size: 867.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.19.0`

```console
$ docker pull nats-streaming@sha256:c8bb32720403c22b091541677c2cdd4e827e65bcf1f25ecf5aaa3acfda90f7d5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.1637; amd64

### `nats-streaming:0.19.0` - linux; amd64

```console
$ docker pull nats-streaming@sha256:053a4ca3955b9c5036e48bafb96c83003fe86c34c6928934e3fd1db0529a889c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 MB (6487259 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:993a204b53252cabfc16952c1d2dc014dc6518d1a08d00bda1bc5008a139e37a`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 03 Nov 2020 00:33:13 GMT
COPY file:3ed83d1497b0535960e452435cb8b27e347f48da12693aa27ebaf9bff94d82de in /nats-streaming-server 
# Tue, 03 Nov 2020 00:33:13 GMT
EXPOSE 4222 8222
# Tue, 03 Nov 2020 00:33:14 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 03 Nov 2020 00:33:14 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:57ac21f890a508f609eabea265197b18ce9dfe3e694034c7a06d37b536a707b2`  
		Last Modified: Tue, 03 Nov 2020 00:33:37 GMT  
		Size: 6.5 MB (6487259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.19.0` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:f334d10ef2a4663d8d7d920d96321cd97f050b82a5d55d588192f074f60dd814
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 MB (6049845 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9eecfd5ab4178a65e952a7cf1d248a556a6ae2c328ac8b68923146d64734db03`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 02 Nov 2020 23:56:28 GMT
COPY file:d6896b1c93dcd497494c972f9274fcc634a4f4a8d63a0191bdb87f6336aec0d7 in /nats-streaming-server 
# Mon, 02 Nov 2020 23:56:28 GMT
EXPOSE 4222 8222
# Mon, 02 Nov 2020 23:56:29 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 02 Nov 2020 23:56:29 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:7f165fb71ab77e8081dbfa13656cdf9e5e005002d6c3afa0aac40667a0f97af8`  
		Last Modified: Mon, 02 Nov 2020 23:57:04 GMT  
		Size: 6.0 MB (6049845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.19.0` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:5fd0943909d8aedafb888e099c9f64d234023ad780805ed7c939692ebfd8304d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 MB (6043163 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f37071e856ae40dc3c8c5e10b359d1640fd67a6110741c0957af2031032ed6ce`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 03 Nov 2020 00:05:23 GMT
COPY file:d232132ddff1d85d3a2f5c80a91c80023cbc103d816387e06d604cf97238e52c in /nats-streaming-server 
# Tue, 03 Nov 2020 00:05:24 GMT
EXPOSE 4222 8222
# Tue, 03 Nov 2020 00:05:24 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 03 Nov 2020 00:05:25 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:9c7227cc1040d04ca7763cfb53ab58bc32ae54921990516adf8e13374ac9ef29`  
		Last Modified: Tue, 03 Nov 2020 00:05:57 GMT  
		Size: 6.0 MB (6043163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.19.0` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:c058fd3e9a8ac44263bf53fa2f6f1e8e8cb3e95cd223f8353fdafc50fe57e417
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 MB (5978846 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7c915a80bd440362bd4a6743fee8134a3caf6271e3258e449fb106b19c050a3b`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 03 Nov 2020 00:43:38 GMT
COPY file:55e70ee826cd5a662497337a2488e22833672bd031d85b4ee39556ab1e80df08 in /nats-streaming-server 
# Tue, 03 Nov 2020 00:43:40 GMT
EXPOSE 4222 8222
# Tue, 03 Nov 2020 00:43:42 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 03 Nov 2020 00:43:43 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:3dc58a59de8a6ed19e9144b0189eb3b637a9e7fcd76ec6c6dc47561b2740a3a2`  
		Last Modified: Tue, 03 Nov 2020 00:44:19 GMT  
		Size: 6.0 MB (5978846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.19.0` - windows version 10.0.17763.1637; amd64

```console
$ docker pull nats-streaming@sha256:9444afab14740d43bfd213340272edcfaa96f83b2ae24d586333398cc089a858
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.8 MB (107783475 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:85bdcab4235f3b70b1671972c4154790bde79e33644ae254ae48efa965b2b3cb`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 03 Dec 2020 08:05:47 GMT
RUN Apply image 1809-amd64
# Wed, 09 Dec 2020 17:38:01 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 09 Dec 2020 23:04:19 GMT
RUN cmd /S /C #(nop) COPY file:cc6bae0f50b6e35b12e8233f240d95e093f7e44257bc87e06aed691866ec1477 in C:\nats-streaming-server.exe 
# Wed, 09 Dec 2020 23:04:21 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 09 Dec 2020 23:04:21 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 09 Dec 2020 23:04:22 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:21be49aa856f07be4e0a677b988e43c04bd595a3c858e58b6c364477bbbf7222`  
		Size: 101.3 MB (101264827 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8a3891744a5ba41f01e625a0a70d755ffe93de4d4f124ad6d069420d5c7956d4`  
		Last Modified: Wed, 09 Dec 2020 17:42:32 GMT  
		Size: 893.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab2cf2a7f92a640dc1125e539b41a28abc6b4e2df892f67cbc0072f90bb65509`  
		Last Modified: Wed, 09 Dec 2020 23:08:42 GMT  
		Size: 6.5 MB (6515155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf561da2a706a067845b617e3efccdaf8257da5fb1ae53c383e29559f5220612`  
		Last Modified: Wed, 09 Dec 2020 23:08:41 GMT  
		Size: 869.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1e5e4a71ea08fded20e3471625c1c06c12540fd3c7f4e12eeaee288bf6e5377`  
		Last Modified: Wed, 09 Dec 2020 23:08:39 GMT  
		Size: 864.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5d7a7dbf47aa9dfd9ed44ec162d12b58d6751c6d5f129c4e65250e21fde3631`  
		Last Modified: Wed, 09 Dec 2020 23:08:41 GMT  
		Size: 867.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.19.0-alpine`

```console
$ docker pull nats-streaming@sha256:5f15b51b2b447004408633f8f9458106fadad8f21393b1ed531071731e1ddb00
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.19.0-alpine` - linux; amd64

```console
$ docker pull nats-streaming@sha256:a8fcf986c14ae3ad60206bd6ebde23999c28f9967f05b9c81a760054539a683d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.6 MB (9567595 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b20b4ccbdde21c3fb61f4bd7fa3e83384f7e9d7f32f5bb86c88cd162a41403c0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Thu, 22 Oct 2020 02:19:24 GMT
ADD file:f17f65714f703db9012f00e5ec98d0b2541ff6147c2633f7ab9ba659d0c507f4 in / 
# Thu, 22 Oct 2020 02:19:24 GMT
CMD ["/bin/sh"]
# Tue, 03 Nov 2020 00:33:01 GMT
ENV NATS_STREAMING_SERVER=0.19.0
# Tue, 03 Nov 2020 00:33:03 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='d582023b8f9fe33b98f0faa6396aae8d5366ecade7e56cde912e21e5b93ea670' ;; 		armhf) natsArch='arm6'; sha256='f4af03e6cbb19f3ad9ea57217607dcf4b68018e1879859c847e2680917fc7139' ;; 		armv7) natsArch='arm7'; sha256='ec8c5ca693344e8b24de9ac955c38de757af8c5760658fc29ed2fbd804803fad' ;; 		x86_64) natsArch='amd64'; sha256='fc15530faec66b61de5140c2b99927c5839caff1c4c17f8bffbf4432fab83017' ;; 		x86) natsArch='386'; sha256='655f0f7cebf727317974006ad4a13ddacd3520f15266e854c2b01681e499bf80' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Tue, 03 Nov 2020 00:33:03 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Tue, 03 Nov 2020 00:33:04 GMT
EXPOSE 4222 8222
# Tue, 03 Nov 2020 00:33:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 03 Nov 2020 00:33:04 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:188c0c94c7c576fff0792aca7ec73d67a2f7f4cb3a6e53a84559337260b36964`  
		Last Modified: Thu, 22 Oct 2020 02:19:57 GMT  
		Size: 2.8 MB (2796860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f211ef5561f154a9a5957cdf08a625861df698594add9ba490a54259e9a01cb1`  
		Last Modified: Tue, 03 Nov 2020 00:33:28 GMT  
		Size: 6.8 MB (6770312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5eef7e98823e252892036fb4b7e5ccf695c556028fa2f7dd6dc314f625ba9eb9`  
		Last Modified: Tue, 03 Nov 2020 00:33:27 GMT  
		Size: 423.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.19.0-alpine` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:2a58d6644e94cc17212ec6a604029ebe9f855ceeee7fa66171bdc8aa6c7113ba
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.9 MB (8932203 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b8391afd58a04ec8cf1ab166357c9495c5aa4d32bc4bb4472e577874f42fe55d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Thu, 22 Oct 2020 02:01:09 GMT
ADD file:dec4d3b6cf21c59820d1d74a554d0a193b5f4859e00b932f31ffe73f554d5afb in / 
# Thu, 22 Oct 2020 02:01:12 GMT
CMD ["/bin/sh"]
# Mon, 02 Nov 2020 23:56:13 GMT
ENV NATS_STREAMING_SERVER=0.19.0
# Mon, 02 Nov 2020 23:56:17 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='d582023b8f9fe33b98f0faa6396aae8d5366ecade7e56cde912e21e5b93ea670' ;; 		armhf) natsArch='arm6'; sha256='f4af03e6cbb19f3ad9ea57217607dcf4b68018e1879859c847e2680917fc7139' ;; 		armv7) natsArch='arm7'; sha256='ec8c5ca693344e8b24de9ac955c38de757af8c5760658fc29ed2fbd804803fad' ;; 		x86_64) natsArch='amd64'; sha256='fc15530faec66b61de5140c2b99927c5839caff1c4c17f8bffbf4432fab83017' ;; 		x86) natsArch='386'; sha256='655f0f7cebf727317974006ad4a13ddacd3520f15266e854c2b01681e499bf80' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Mon, 02 Nov 2020 23:56:17 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Mon, 02 Nov 2020 23:56:18 GMT
EXPOSE 4222 8222
# Mon, 02 Nov 2020 23:56:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 02 Nov 2020 23:56:19 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:bad30e7b45c14f784ef29a828b5fc69db0ebdefebcde6a7c98f4f77ffc93a546`  
		Last Modified: Thu, 22 Oct 2020 02:01:42 GMT  
		Size: 2.6 MB (2601912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21cba1ed5b5094a02c017d654b758674905ec0bb2535d3311fcdd61dce32b319`  
		Last Modified: Mon, 02 Nov 2020 23:56:50 GMT  
		Size: 6.3 MB (6329871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3992f15ff4c1a7660c4a81854ec33d3e4973405c7095ceb0bd8a7865fff21c9f`  
		Last Modified: Mon, 02 Nov 2020 23:56:47 GMT  
		Size: 420.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.19.0-alpine` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:6a6c52fc272b91cff878ca25bddc432f19583a2e41e5e92288f0e64d0c649896
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.7 MB (8730479 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b4347330ee2d9b26f7fafaadc370627e71670505b340c9e4b54d791afcb3a6b2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Thu, 22 Oct 2020 01:58:13 GMT
ADD file:46f89172426e9f5b1d669a2ca7ab218fc2deaef1caeeab88f2b5bd443ac9773d in / 
# Thu, 22 Oct 2020 01:58:14 GMT
CMD ["/bin/sh"]
# Tue, 03 Nov 2020 00:05:05 GMT
ENV NATS_STREAMING_SERVER=0.19.0
# Tue, 03 Nov 2020 00:05:09 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='d582023b8f9fe33b98f0faa6396aae8d5366ecade7e56cde912e21e5b93ea670' ;; 		armhf) natsArch='arm6'; sha256='f4af03e6cbb19f3ad9ea57217607dcf4b68018e1879859c847e2680917fc7139' ;; 		armv7) natsArch='arm7'; sha256='ec8c5ca693344e8b24de9ac955c38de757af8c5760658fc29ed2fbd804803fad' ;; 		x86_64) natsArch='amd64'; sha256='fc15530faec66b61de5140c2b99927c5839caff1c4c17f8bffbf4432fab83017' ;; 		x86) natsArch='386'; sha256='655f0f7cebf727317974006ad4a13ddacd3520f15266e854c2b01681e499bf80' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Tue, 03 Nov 2020 00:05:09 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Tue, 03 Nov 2020 00:05:10 GMT
EXPOSE 4222 8222
# Tue, 03 Nov 2020 00:05:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 03 Nov 2020 00:05:11 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:5f2023fd85a4e68f37fe41421fd89f30e69b98a645613521c57c01317561eee3`  
		Last Modified: Thu, 22 Oct 2020 01:58:45 GMT  
		Size: 2.4 MB (2405675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34033d6dabe9c0f77f765bf2fce39f1eef24c163cfa802ec78f0e2e1bea9da7c`  
		Last Modified: Tue, 03 Nov 2020 00:05:43 GMT  
		Size: 6.3 MB (6324384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b0a98c9d7b5d859df80140920031b236b38ff88a4ff09d3bf8cfc5b9776e436`  
		Last Modified: Tue, 03 Nov 2020 00:05:40 GMT  
		Size: 420.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.19.0-alpine` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:36be57b574502addd00c81caaffedb9030eec583dbf4e3011a95aa7f998834aa
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.0 MB (8969159 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b947ac7936fa0250ecf3f1aaa6e22a928bdb3cdd8f0dcbbc3b8912a0678290c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Thu, 22 Oct 2020 02:01:01 GMT
ADD file:55c4e9752146061a2b5f76027221329f423687987c0744ef577130c60ff0ba42 in / 
# Thu, 22 Oct 2020 02:01:06 GMT
CMD ["/bin/sh"]
# Tue, 03 Nov 2020 00:43:12 GMT
ENV NATS_STREAMING_SERVER=0.19.0
# Tue, 03 Nov 2020 00:43:20 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='d582023b8f9fe33b98f0faa6396aae8d5366ecade7e56cde912e21e5b93ea670' ;; 		armhf) natsArch='arm6'; sha256='f4af03e6cbb19f3ad9ea57217607dcf4b68018e1879859c847e2680917fc7139' ;; 		armv7) natsArch='arm7'; sha256='ec8c5ca693344e8b24de9ac955c38de757af8c5760658fc29ed2fbd804803fad' ;; 		x86_64) natsArch='amd64'; sha256='fc15530faec66b61de5140c2b99927c5839caff1c4c17f8bffbf4432fab83017' ;; 		x86) natsArch='386'; sha256='655f0f7cebf727317974006ad4a13ddacd3520f15266e854c2b01681e499bf80' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Tue, 03 Nov 2020 00:43:21 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Tue, 03 Nov 2020 00:43:23 GMT
EXPOSE 4222 8222
# Tue, 03 Nov 2020 00:43:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 03 Nov 2020 00:43:27 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:5f621e34cdf485f410766dc9a0fc7855d17916d0f6583b58cbdce7c28831f527`  
		Last Modified: Thu, 22 Oct 2020 02:01:38 GMT  
		Size: 2.7 MB (2706555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfea83a41655c390ae2bea2fd6f2a83188ecb9c82e60ebde8040109e79a2eba5`  
		Last Modified: Tue, 03 Nov 2020 00:44:06 GMT  
		Size: 6.3 MB (6262183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0eca3d16e3b7142a6392c550b0efad91076053f222028892a3ae01e63f58dec`  
		Last Modified: Tue, 03 Nov 2020 00:44:05 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.19.0-alpine3.12`

```console
$ docker pull nats-streaming@sha256:5f15b51b2b447004408633f8f9458106fadad8f21393b1ed531071731e1ddb00
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.19.0-alpine3.12` - linux; amd64

```console
$ docker pull nats-streaming@sha256:a8fcf986c14ae3ad60206bd6ebde23999c28f9967f05b9c81a760054539a683d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.6 MB (9567595 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b20b4ccbdde21c3fb61f4bd7fa3e83384f7e9d7f32f5bb86c88cd162a41403c0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Thu, 22 Oct 2020 02:19:24 GMT
ADD file:f17f65714f703db9012f00e5ec98d0b2541ff6147c2633f7ab9ba659d0c507f4 in / 
# Thu, 22 Oct 2020 02:19:24 GMT
CMD ["/bin/sh"]
# Tue, 03 Nov 2020 00:33:01 GMT
ENV NATS_STREAMING_SERVER=0.19.0
# Tue, 03 Nov 2020 00:33:03 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='d582023b8f9fe33b98f0faa6396aae8d5366ecade7e56cde912e21e5b93ea670' ;; 		armhf) natsArch='arm6'; sha256='f4af03e6cbb19f3ad9ea57217607dcf4b68018e1879859c847e2680917fc7139' ;; 		armv7) natsArch='arm7'; sha256='ec8c5ca693344e8b24de9ac955c38de757af8c5760658fc29ed2fbd804803fad' ;; 		x86_64) natsArch='amd64'; sha256='fc15530faec66b61de5140c2b99927c5839caff1c4c17f8bffbf4432fab83017' ;; 		x86) natsArch='386'; sha256='655f0f7cebf727317974006ad4a13ddacd3520f15266e854c2b01681e499bf80' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Tue, 03 Nov 2020 00:33:03 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Tue, 03 Nov 2020 00:33:04 GMT
EXPOSE 4222 8222
# Tue, 03 Nov 2020 00:33:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 03 Nov 2020 00:33:04 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:188c0c94c7c576fff0792aca7ec73d67a2f7f4cb3a6e53a84559337260b36964`  
		Last Modified: Thu, 22 Oct 2020 02:19:57 GMT  
		Size: 2.8 MB (2796860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f211ef5561f154a9a5957cdf08a625861df698594add9ba490a54259e9a01cb1`  
		Last Modified: Tue, 03 Nov 2020 00:33:28 GMT  
		Size: 6.8 MB (6770312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5eef7e98823e252892036fb4b7e5ccf695c556028fa2f7dd6dc314f625ba9eb9`  
		Last Modified: Tue, 03 Nov 2020 00:33:27 GMT  
		Size: 423.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.19.0-alpine3.12` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:2a58d6644e94cc17212ec6a604029ebe9f855ceeee7fa66171bdc8aa6c7113ba
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.9 MB (8932203 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b8391afd58a04ec8cf1ab166357c9495c5aa4d32bc4bb4472e577874f42fe55d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Thu, 22 Oct 2020 02:01:09 GMT
ADD file:dec4d3b6cf21c59820d1d74a554d0a193b5f4859e00b932f31ffe73f554d5afb in / 
# Thu, 22 Oct 2020 02:01:12 GMT
CMD ["/bin/sh"]
# Mon, 02 Nov 2020 23:56:13 GMT
ENV NATS_STREAMING_SERVER=0.19.0
# Mon, 02 Nov 2020 23:56:17 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='d582023b8f9fe33b98f0faa6396aae8d5366ecade7e56cde912e21e5b93ea670' ;; 		armhf) natsArch='arm6'; sha256='f4af03e6cbb19f3ad9ea57217607dcf4b68018e1879859c847e2680917fc7139' ;; 		armv7) natsArch='arm7'; sha256='ec8c5ca693344e8b24de9ac955c38de757af8c5760658fc29ed2fbd804803fad' ;; 		x86_64) natsArch='amd64'; sha256='fc15530faec66b61de5140c2b99927c5839caff1c4c17f8bffbf4432fab83017' ;; 		x86) natsArch='386'; sha256='655f0f7cebf727317974006ad4a13ddacd3520f15266e854c2b01681e499bf80' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Mon, 02 Nov 2020 23:56:17 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Mon, 02 Nov 2020 23:56:18 GMT
EXPOSE 4222 8222
# Mon, 02 Nov 2020 23:56:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 02 Nov 2020 23:56:19 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:bad30e7b45c14f784ef29a828b5fc69db0ebdefebcde6a7c98f4f77ffc93a546`  
		Last Modified: Thu, 22 Oct 2020 02:01:42 GMT  
		Size: 2.6 MB (2601912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21cba1ed5b5094a02c017d654b758674905ec0bb2535d3311fcdd61dce32b319`  
		Last Modified: Mon, 02 Nov 2020 23:56:50 GMT  
		Size: 6.3 MB (6329871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3992f15ff4c1a7660c4a81854ec33d3e4973405c7095ceb0bd8a7865fff21c9f`  
		Last Modified: Mon, 02 Nov 2020 23:56:47 GMT  
		Size: 420.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.19.0-alpine3.12` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:6a6c52fc272b91cff878ca25bddc432f19583a2e41e5e92288f0e64d0c649896
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.7 MB (8730479 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b4347330ee2d9b26f7fafaadc370627e71670505b340c9e4b54d791afcb3a6b2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Thu, 22 Oct 2020 01:58:13 GMT
ADD file:46f89172426e9f5b1d669a2ca7ab218fc2deaef1caeeab88f2b5bd443ac9773d in / 
# Thu, 22 Oct 2020 01:58:14 GMT
CMD ["/bin/sh"]
# Tue, 03 Nov 2020 00:05:05 GMT
ENV NATS_STREAMING_SERVER=0.19.0
# Tue, 03 Nov 2020 00:05:09 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='d582023b8f9fe33b98f0faa6396aae8d5366ecade7e56cde912e21e5b93ea670' ;; 		armhf) natsArch='arm6'; sha256='f4af03e6cbb19f3ad9ea57217607dcf4b68018e1879859c847e2680917fc7139' ;; 		armv7) natsArch='arm7'; sha256='ec8c5ca693344e8b24de9ac955c38de757af8c5760658fc29ed2fbd804803fad' ;; 		x86_64) natsArch='amd64'; sha256='fc15530faec66b61de5140c2b99927c5839caff1c4c17f8bffbf4432fab83017' ;; 		x86) natsArch='386'; sha256='655f0f7cebf727317974006ad4a13ddacd3520f15266e854c2b01681e499bf80' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Tue, 03 Nov 2020 00:05:09 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Tue, 03 Nov 2020 00:05:10 GMT
EXPOSE 4222 8222
# Tue, 03 Nov 2020 00:05:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 03 Nov 2020 00:05:11 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:5f2023fd85a4e68f37fe41421fd89f30e69b98a645613521c57c01317561eee3`  
		Last Modified: Thu, 22 Oct 2020 01:58:45 GMT  
		Size: 2.4 MB (2405675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34033d6dabe9c0f77f765bf2fce39f1eef24c163cfa802ec78f0e2e1bea9da7c`  
		Last Modified: Tue, 03 Nov 2020 00:05:43 GMT  
		Size: 6.3 MB (6324384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b0a98c9d7b5d859df80140920031b236b38ff88a4ff09d3bf8cfc5b9776e436`  
		Last Modified: Tue, 03 Nov 2020 00:05:40 GMT  
		Size: 420.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.19.0-alpine3.12` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:36be57b574502addd00c81caaffedb9030eec583dbf4e3011a95aa7f998834aa
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.0 MB (8969159 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b947ac7936fa0250ecf3f1aaa6e22a928bdb3cdd8f0dcbbc3b8912a0678290c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Thu, 22 Oct 2020 02:01:01 GMT
ADD file:55c4e9752146061a2b5f76027221329f423687987c0744ef577130c60ff0ba42 in / 
# Thu, 22 Oct 2020 02:01:06 GMT
CMD ["/bin/sh"]
# Tue, 03 Nov 2020 00:43:12 GMT
ENV NATS_STREAMING_SERVER=0.19.0
# Tue, 03 Nov 2020 00:43:20 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='d582023b8f9fe33b98f0faa6396aae8d5366ecade7e56cde912e21e5b93ea670' ;; 		armhf) natsArch='arm6'; sha256='f4af03e6cbb19f3ad9ea57217607dcf4b68018e1879859c847e2680917fc7139' ;; 		armv7) natsArch='arm7'; sha256='ec8c5ca693344e8b24de9ac955c38de757af8c5760658fc29ed2fbd804803fad' ;; 		x86_64) natsArch='amd64'; sha256='fc15530faec66b61de5140c2b99927c5839caff1c4c17f8bffbf4432fab83017' ;; 		x86) natsArch='386'; sha256='655f0f7cebf727317974006ad4a13ddacd3520f15266e854c2b01681e499bf80' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Tue, 03 Nov 2020 00:43:21 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Tue, 03 Nov 2020 00:43:23 GMT
EXPOSE 4222 8222
# Tue, 03 Nov 2020 00:43:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 03 Nov 2020 00:43:27 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:5f621e34cdf485f410766dc9a0fc7855d17916d0f6583b58cbdce7c28831f527`  
		Last Modified: Thu, 22 Oct 2020 02:01:38 GMT  
		Size: 2.7 MB (2706555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfea83a41655c390ae2bea2fd6f2a83188ecb9c82e60ebde8040109e79a2eba5`  
		Last Modified: Tue, 03 Nov 2020 00:44:06 GMT  
		Size: 6.3 MB (6262183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0eca3d16e3b7142a6392c550b0efad91076053f222028892a3ae01e63f58dec`  
		Last Modified: Tue, 03 Nov 2020 00:44:05 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.19.0-linux`

```console
$ docker pull nats-streaming@sha256:8001e4db36785bd692d9ae1c9ed3857d972692b385e36c08994794a5254bb78a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.19.0-linux` - linux; amd64

```console
$ docker pull nats-streaming@sha256:053a4ca3955b9c5036e48bafb96c83003fe86c34c6928934e3fd1db0529a889c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 MB (6487259 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:993a204b53252cabfc16952c1d2dc014dc6518d1a08d00bda1bc5008a139e37a`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 03 Nov 2020 00:33:13 GMT
COPY file:3ed83d1497b0535960e452435cb8b27e347f48da12693aa27ebaf9bff94d82de in /nats-streaming-server 
# Tue, 03 Nov 2020 00:33:13 GMT
EXPOSE 4222 8222
# Tue, 03 Nov 2020 00:33:14 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 03 Nov 2020 00:33:14 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:57ac21f890a508f609eabea265197b18ce9dfe3e694034c7a06d37b536a707b2`  
		Last Modified: Tue, 03 Nov 2020 00:33:37 GMT  
		Size: 6.5 MB (6487259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.19.0-linux` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:f334d10ef2a4663d8d7d920d96321cd97f050b82a5d55d588192f074f60dd814
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 MB (6049845 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9eecfd5ab4178a65e952a7cf1d248a556a6ae2c328ac8b68923146d64734db03`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 02 Nov 2020 23:56:28 GMT
COPY file:d6896b1c93dcd497494c972f9274fcc634a4f4a8d63a0191bdb87f6336aec0d7 in /nats-streaming-server 
# Mon, 02 Nov 2020 23:56:28 GMT
EXPOSE 4222 8222
# Mon, 02 Nov 2020 23:56:29 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 02 Nov 2020 23:56:29 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:7f165fb71ab77e8081dbfa13656cdf9e5e005002d6c3afa0aac40667a0f97af8`  
		Last Modified: Mon, 02 Nov 2020 23:57:04 GMT  
		Size: 6.0 MB (6049845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.19.0-linux` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:5fd0943909d8aedafb888e099c9f64d234023ad780805ed7c939692ebfd8304d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 MB (6043163 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f37071e856ae40dc3c8c5e10b359d1640fd67a6110741c0957af2031032ed6ce`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 03 Nov 2020 00:05:23 GMT
COPY file:d232132ddff1d85d3a2f5c80a91c80023cbc103d816387e06d604cf97238e52c in /nats-streaming-server 
# Tue, 03 Nov 2020 00:05:24 GMT
EXPOSE 4222 8222
# Tue, 03 Nov 2020 00:05:24 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 03 Nov 2020 00:05:25 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:9c7227cc1040d04ca7763cfb53ab58bc32ae54921990516adf8e13374ac9ef29`  
		Last Modified: Tue, 03 Nov 2020 00:05:57 GMT  
		Size: 6.0 MB (6043163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.19.0-linux` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:c058fd3e9a8ac44263bf53fa2f6f1e8e8cb3e95cd223f8353fdafc50fe57e417
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 MB (5978846 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7c915a80bd440362bd4a6743fee8134a3caf6271e3258e449fb106b19c050a3b`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 03 Nov 2020 00:43:38 GMT
COPY file:55e70ee826cd5a662497337a2488e22833672bd031d85b4ee39556ab1e80df08 in /nats-streaming-server 
# Tue, 03 Nov 2020 00:43:40 GMT
EXPOSE 4222 8222
# Tue, 03 Nov 2020 00:43:42 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 03 Nov 2020 00:43:43 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:3dc58a59de8a6ed19e9144b0189eb3b637a9e7fcd76ec6c6dc47561b2740a3a2`  
		Last Modified: Tue, 03 Nov 2020 00:44:19 GMT  
		Size: 6.0 MB (5978846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.19.0-nanoserver`

```console
$ docker pull nats-streaming@sha256:4a013f6e621b040ed030861cb0bd02d96ef23c7a5fbf2019841921e255379ebf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1637; amd64

### `nats-streaming:0.19.0-nanoserver` - windows version 10.0.17763.1637; amd64

```console
$ docker pull nats-streaming@sha256:9444afab14740d43bfd213340272edcfaa96f83b2ae24d586333398cc089a858
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.8 MB (107783475 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:85bdcab4235f3b70b1671972c4154790bde79e33644ae254ae48efa965b2b3cb`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 03 Dec 2020 08:05:47 GMT
RUN Apply image 1809-amd64
# Wed, 09 Dec 2020 17:38:01 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 09 Dec 2020 23:04:19 GMT
RUN cmd /S /C #(nop) COPY file:cc6bae0f50b6e35b12e8233f240d95e093f7e44257bc87e06aed691866ec1477 in C:\nats-streaming-server.exe 
# Wed, 09 Dec 2020 23:04:21 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 09 Dec 2020 23:04:21 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 09 Dec 2020 23:04:22 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:21be49aa856f07be4e0a677b988e43c04bd595a3c858e58b6c364477bbbf7222`  
		Size: 101.3 MB (101264827 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8a3891744a5ba41f01e625a0a70d755ffe93de4d4f124ad6d069420d5c7956d4`  
		Last Modified: Wed, 09 Dec 2020 17:42:32 GMT  
		Size: 893.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab2cf2a7f92a640dc1125e539b41a28abc6b4e2df892f67cbc0072f90bb65509`  
		Last Modified: Wed, 09 Dec 2020 23:08:42 GMT  
		Size: 6.5 MB (6515155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf561da2a706a067845b617e3efccdaf8257da5fb1ae53c383e29559f5220612`  
		Last Modified: Wed, 09 Dec 2020 23:08:41 GMT  
		Size: 869.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1e5e4a71ea08fded20e3471625c1c06c12540fd3c7f4e12eeaee288bf6e5377`  
		Last Modified: Wed, 09 Dec 2020 23:08:39 GMT  
		Size: 864.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5d7a7dbf47aa9dfd9ed44ec162d12b58d6751c6d5f129c4e65250e21fde3631`  
		Last Modified: Wed, 09 Dec 2020 23:08:41 GMT  
		Size: 867.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.19.0-nanoserver-1809`

```console
$ docker pull nats-streaming@sha256:4a013f6e621b040ed030861cb0bd02d96ef23c7a5fbf2019841921e255379ebf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1637; amd64

### `nats-streaming:0.19.0-nanoserver-1809` - windows version 10.0.17763.1637; amd64

```console
$ docker pull nats-streaming@sha256:9444afab14740d43bfd213340272edcfaa96f83b2ae24d586333398cc089a858
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.8 MB (107783475 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:85bdcab4235f3b70b1671972c4154790bde79e33644ae254ae48efa965b2b3cb`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 03 Dec 2020 08:05:47 GMT
RUN Apply image 1809-amd64
# Wed, 09 Dec 2020 17:38:01 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 09 Dec 2020 23:04:19 GMT
RUN cmd /S /C #(nop) COPY file:cc6bae0f50b6e35b12e8233f240d95e093f7e44257bc87e06aed691866ec1477 in C:\nats-streaming-server.exe 
# Wed, 09 Dec 2020 23:04:21 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 09 Dec 2020 23:04:21 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 09 Dec 2020 23:04:22 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:21be49aa856f07be4e0a677b988e43c04bd595a3c858e58b6c364477bbbf7222`  
		Size: 101.3 MB (101264827 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8a3891744a5ba41f01e625a0a70d755ffe93de4d4f124ad6d069420d5c7956d4`  
		Last Modified: Wed, 09 Dec 2020 17:42:32 GMT  
		Size: 893.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab2cf2a7f92a640dc1125e539b41a28abc6b4e2df892f67cbc0072f90bb65509`  
		Last Modified: Wed, 09 Dec 2020 23:08:42 GMT  
		Size: 6.5 MB (6515155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf561da2a706a067845b617e3efccdaf8257da5fb1ae53c383e29559f5220612`  
		Last Modified: Wed, 09 Dec 2020 23:08:41 GMT  
		Size: 869.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1e5e4a71ea08fded20e3471625c1c06c12540fd3c7f4e12eeaee288bf6e5377`  
		Last Modified: Wed, 09 Dec 2020 23:08:39 GMT  
		Size: 864.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5d7a7dbf47aa9dfd9ed44ec162d12b58d6751c6d5f129c4e65250e21fde3631`  
		Last Modified: Wed, 09 Dec 2020 23:08:41 GMT  
		Size: 867.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.19.0-scratch`

```console
$ docker pull nats-streaming@sha256:8001e4db36785bd692d9ae1c9ed3857d972692b385e36c08994794a5254bb78a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.19.0-scratch` - linux; amd64

```console
$ docker pull nats-streaming@sha256:053a4ca3955b9c5036e48bafb96c83003fe86c34c6928934e3fd1db0529a889c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 MB (6487259 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:993a204b53252cabfc16952c1d2dc014dc6518d1a08d00bda1bc5008a139e37a`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 03 Nov 2020 00:33:13 GMT
COPY file:3ed83d1497b0535960e452435cb8b27e347f48da12693aa27ebaf9bff94d82de in /nats-streaming-server 
# Tue, 03 Nov 2020 00:33:13 GMT
EXPOSE 4222 8222
# Tue, 03 Nov 2020 00:33:14 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 03 Nov 2020 00:33:14 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:57ac21f890a508f609eabea265197b18ce9dfe3e694034c7a06d37b536a707b2`  
		Last Modified: Tue, 03 Nov 2020 00:33:37 GMT  
		Size: 6.5 MB (6487259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.19.0-scratch` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:f334d10ef2a4663d8d7d920d96321cd97f050b82a5d55d588192f074f60dd814
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 MB (6049845 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9eecfd5ab4178a65e952a7cf1d248a556a6ae2c328ac8b68923146d64734db03`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 02 Nov 2020 23:56:28 GMT
COPY file:d6896b1c93dcd497494c972f9274fcc634a4f4a8d63a0191bdb87f6336aec0d7 in /nats-streaming-server 
# Mon, 02 Nov 2020 23:56:28 GMT
EXPOSE 4222 8222
# Mon, 02 Nov 2020 23:56:29 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 02 Nov 2020 23:56:29 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:7f165fb71ab77e8081dbfa13656cdf9e5e005002d6c3afa0aac40667a0f97af8`  
		Last Modified: Mon, 02 Nov 2020 23:57:04 GMT  
		Size: 6.0 MB (6049845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.19.0-scratch` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:5fd0943909d8aedafb888e099c9f64d234023ad780805ed7c939692ebfd8304d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 MB (6043163 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f37071e856ae40dc3c8c5e10b359d1640fd67a6110741c0957af2031032ed6ce`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 03 Nov 2020 00:05:23 GMT
COPY file:d232132ddff1d85d3a2f5c80a91c80023cbc103d816387e06d604cf97238e52c in /nats-streaming-server 
# Tue, 03 Nov 2020 00:05:24 GMT
EXPOSE 4222 8222
# Tue, 03 Nov 2020 00:05:24 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 03 Nov 2020 00:05:25 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:9c7227cc1040d04ca7763cfb53ab58bc32ae54921990516adf8e13374ac9ef29`  
		Last Modified: Tue, 03 Nov 2020 00:05:57 GMT  
		Size: 6.0 MB (6043163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.19.0-scratch` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:c058fd3e9a8ac44263bf53fa2f6f1e8e8cb3e95cd223f8353fdafc50fe57e417
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 MB (5978846 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7c915a80bd440362bd4a6743fee8134a3caf6271e3258e449fb106b19c050a3b`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 03 Nov 2020 00:43:38 GMT
COPY file:55e70ee826cd5a662497337a2488e22833672bd031d85b4ee39556ab1e80df08 in /nats-streaming-server 
# Tue, 03 Nov 2020 00:43:40 GMT
EXPOSE 4222 8222
# Tue, 03 Nov 2020 00:43:42 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 03 Nov 2020 00:43:43 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:3dc58a59de8a6ed19e9144b0189eb3b637a9e7fcd76ec6c6dc47561b2740a3a2`  
		Last Modified: Tue, 03 Nov 2020 00:44:19 GMT  
		Size: 6.0 MB (5978846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.19.0-windowsservercore`

```console
$ docker pull nats-streaming@sha256:78cddd38d3c26f2a74454532132969b5fbc9fbff9cc8708cf338c1b33a80c17b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1637; amd64
	-	windows version 10.0.14393.4104; amd64

### `nats-streaming:0.19.0-windowsservercore` - windows version 10.0.17763.1637; amd64

```console
$ docker pull nats-streaming@sha256:7a8ab0956821d178ef84f6f10c399d44005ca86dd75378d41a5980979ed24409
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2411449594 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0146757e90d9c2df66c7933b807c71d62de612813d33a32f15c8d7fdd710ddae`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 04 Dec 2020 02:13:01 GMT
RUN Install update 1809-amd64
# Wed, 09 Dec 2020 14:02:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Dec 2020 17:36:04 GMT
ENV NATS_DOCKERIZED=1
# Wed, 09 Dec 2020 23:02:20 GMT
ENV NATS_STREAMING_SERVER=0.19.0
# Wed, 09 Dec 2020 23:02:21 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.19.0/nats-streaming-server-v0.19.0-windows-amd64.zip
# Wed, 09 Dec 2020 23:02:22 GMT
ENV GIT_DOWNLOAD_SHA256=edafd6482bd71f3d6035d7f6871df1fd4c53acf0ac19e88b85e08a2c7ab1cec5
# Wed, 09 Dec 2020 23:02:52 GMT
RUN Set-PSDebug -Trace 2
# Wed, 09 Dec 2020 23:04:09 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 09 Dec 2020 23:04:10 GMT
EXPOSE 4222 8222
# Wed, 09 Dec 2020 23:04:12 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 09 Dec 2020 23:04:13 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:aa4f58cd6da1aaf1a0b44d443bd88e7fbe5b0a6f193995a1a61d6bd63990f314`  
		Size: 672.5 MB (672541583 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:240407eb82b6591b0574396ec829a4a5cd9a75257a4663f9876942995275965d`  
		Last Modified: Wed, 09 Dec 2020 17:10:14 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82b9257be76bd37cad15d45905ec5910266409794a9dbd8a0428174f8b2f352a`  
		Last Modified: Wed, 09 Dec 2020 17:42:00 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36644685392e418bf32ab96db81c8f6a861b913256c244637d9d3ee45098a9cb`  
		Last Modified: Wed, 09 Dec 2020 23:08:22 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9469bed00eb5f6a5b7c050a1aaee856134ec78bab6076cc793e26dc52ec71fa`  
		Last Modified: Wed, 09 Dec 2020 23:08:21 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94e9d451908e3e8ec10448e052cf25767a282312e49e29d2a0b42652cf217e28`  
		Last Modified: Wed, 09 Dec 2020 23:08:21 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:870e3bb830bd8ad9b84a928d2b858be730dcdba8016206ee4aeda623d98754b3`  
		Last Modified: Wed, 09 Dec 2020 23:08:20 GMT  
		Size: 4.8 MB (4843348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14d24c0a2fc2b3ecd1b0467794ae95667a29e1bd550bf2bf9c455499839253bc`  
		Last Modified: Wed, 09 Dec 2020 23:08:23 GMT  
		Size: 15.7 MB (15722612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09371bf015245c95ce8d5db6b8d7f90fc6d8527f83101535c8c6af719b628e79`  
		Last Modified: Wed, 09 Dec 2020 23:08:18 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76ff8db511e98efbde9cbbf6ecd2d9bd2b73565c7c4e0d24dddeb6edfa2a1875`  
		Last Modified: Wed, 09 Dec 2020 23:08:18 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13217bf3886546791bd6c26ab23636f9bc595fd80abf1e7d6ab6f10f8613cdee`  
		Last Modified: Wed, 09 Dec 2020 23:08:18 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.19.0-windowsservercore` - windows version 10.0.14393.4104; amd64

```console
$ docker pull nats-streaming@sha256:33a909f6239f294532f68e91f94655aa881f2c8701293c9963e4b1c85b1a1a52
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5790922042 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:74e094a16d960a68e3691347bc7923c1f94b7db31dedb2ef74b9d87436170384`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 02 Dec 2020 17:42:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 09 Dec 2020 14:41:21 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Dec 2020 17:38:10 GMT
ENV NATS_DOCKERIZED=1
# Wed, 09 Dec 2020 23:04:27 GMT
ENV NATS_STREAMING_SERVER=0.19.0
# Wed, 09 Dec 2020 23:04:28 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.19.0/nats-streaming-server-v0.19.0-windows-amd64.zip
# Wed, 09 Dec 2020 23:04:28 GMT
ENV GIT_DOWNLOAD_SHA256=edafd6482bd71f3d6035d7f6871df1fd4c53acf0ac19e88b85e08a2c7ab1cec5
# Wed, 09 Dec 2020 23:05:39 GMT
RUN Set-PSDebug -Trace 2
# Wed, 09 Dec 2020 23:07:44 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 09 Dec 2020 23:07:45 GMT
EXPOSE 4222 8222
# Wed, 09 Dec 2020 23:07:46 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 09 Dec 2020 23:07:47 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d2696dc2a40dc121fc5acaa02242817ac416c69d17c113e2ac5136d21a3942d8`  
		Size: 1.7 GB (1698858125 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b5a79f8be42bf1c358ccc82f32c1481de95c393ef97e712a321c1440d132fda9`  
		Last Modified: Wed, 09 Dec 2020 17:11:03 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56d972336c8bcee0026c76e8f199cef405112a70aeef9917f07d2859f15162c1`  
		Last Modified: Wed, 09 Dec 2020 17:42:56 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e4f52064be159ebf6d7d967a842e39ae04b53dcf15dd8b582a77af431f81df7`  
		Last Modified: Wed, 09 Dec 2020 23:09:02 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54d1ecc24d286c8499d1698affa71481762f11bb3d4fdd9d35763dcbe94e9e9a`  
		Last Modified: Wed, 09 Dec 2020 23:09:00 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:649366889ec5703d27a79142f0331f2a462858d6d6ee2a7c1bd8e426bece4236`  
		Last Modified: Wed, 09 Dec 2020 23:08:59 GMT  
		Size: 1.1 KB (1139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9916349c9d6afe29e7418ee0e8f0454bb37038070600eaef872fb7356c1147d0`  
		Last Modified: Wed, 09 Dec 2020 23:08:59 GMT  
		Size: 5.5 MB (5528923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:838e032e6db488d413de3f4681555d2b57bb4472c3b16ed16a5c07f2e921f1ed`  
		Last Modified: Wed, 09 Dec 2020 23:09:01 GMT  
		Size: 16.5 MB (16540005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96a5c8ab334a9fbf340bbb2d213d16e91599eee98aafa72f7f8fbb6d4d147b27`  
		Last Modified: Wed, 09 Dec 2020 23:08:56 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09db5c24070ad330bcb0f078a2325aba107a3a8615fc004248d02e8e828fa8ce`  
		Last Modified: Wed, 09 Dec 2020 23:08:58 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21108015f9c4f2ee78087806b4ca0582f2618489ed4899b07b6290d743b8ef3d`  
		Last Modified: Wed, 09 Dec 2020 23:08:57 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.19.0-windowsservercore-1809`

```console
$ docker pull nats-streaming@sha256:3a285fa7c8c148aad627e61b6848554ccc223cb30a1eb3293a5a5fb89af016c6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1637; amd64

### `nats-streaming:0.19.0-windowsservercore-1809` - windows version 10.0.17763.1637; amd64

```console
$ docker pull nats-streaming@sha256:7a8ab0956821d178ef84f6f10c399d44005ca86dd75378d41a5980979ed24409
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2411449594 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0146757e90d9c2df66c7933b807c71d62de612813d33a32f15c8d7fdd710ddae`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 04 Dec 2020 02:13:01 GMT
RUN Install update 1809-amd64
# Wed, 09 Dec 2020 14:02:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Dec 2020 17:36:04 GMT
ENV NATS_DOCKERIZED=1
# Wed, 09 Dec 2020 23:02:20 GMT
ENV NATS_STREAMING_SERVER=0.19.0
# Wed, 09 Dec 2020 23:02:21 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.19.0/nats-streaming-server-v0.19.0-windows-amd64.zip
# Wed, 09 Dec 2020 23:02:22 GMT
ENV GIT_DOWNLOAD_SHA256=edafd6482bd71f3d6035d7f6871df1fd4c53acf0ac19e88b85e08a2c7ab1cec5
# Wed, 09 Dec 2020 23:02:52 GMT
RUN Set-PSDebug -Trace 2
# Wed, 09 Dec 2020 23:04:09 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 09 Dec 2020 23:04:10 GMT
EXPOSE 4222 8222
# Wed, 09 Dec 2020 23:04:12 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 09 Dec 2020 23:04:13 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:aa4f58cd6da1aaf1a0b44d443bd88e7fbe5b0a6f193995a1a61d6bd63990f314`  
		Size: 672.5 MB (672541583 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:240407eb82b6591b0574396ec829a4a5cd9a75257a4663f9876942995275965d`  
		Last Modified: Wed, 09 Dec 2020 17:10:14 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82b9257be76bd37cad15d45905ec5910266409794a9dbd8a0428174f8b2f352a`  
		Last Modified: Wed, 09 Dec 2020 17:42:00 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36644685392e418bf32ab96db81c8f6a861b913256c244637d9d3ee45098a9cb`  
		Last Modified: Wed, 09 Dec 2020 23:08:22 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9469bed00eb5f6a5b7c050a1aaee856134ec78bab6076cc793e26dc52ec71fa`  
		Last Modified: Wed, 09 Dec 2020 23:08:21 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94e9d451908e3e8ec10448e052cf25767a282312e49e29d2a0b42652cf217e28`  
		Last Modified: Wed, 09 Dec 2020 23:08:21 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:870e3bb830bd8ad9b84a928d2b858be730dcdba8016206ee4aeda623d98754b3`  
		Last Modified: Wed, 09 Dec 2020 23:08:20 GMT  
		Size: 4.8 MB (4843348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14d24c0a2fc2b3ecd1b0467794ae95667a29e1bd550bf2bf9c455499839253bc`  
		Last Modified: Wed, 09 Dec 2020 23:08:23 GMT  
		Size: 15.7 MB (15722612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09371bf015245c95ce8d5db6b8d7f90fc6d8527f83101535c8c6af719b628e79`  
		Last Modified: Wed, 09 Dec 2020 23:08:18 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76ff8db511e98efbde9cbbf6ecd2d9bd2b73565c7c4e0d24dddeb6edfa2a1875`  
		Last Modified: Wed, 09 Dec 2020 23:08:18 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13217bf3886546791bd6c26ab23636f9bc595fd80abf1e7d6ab6f10f8613cdee`  
		Last Modified: Wed, 09 Dec 2020 23:08:18 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.19.0-windowsservercore-ltsc2016`

```console
$ docker pull nats-streaming@sha256:da877310cb87d1822f44a79a76b57af2eceb3e15aa82ab406a47d32bc0de9f47
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4104; amd64

### `nats-streaming:0.19.0-windowsservercore-ltsc2016` - windows version 10.0.14393.4104; amd64

```console
$ docker pull nats-streaming@sha256:33a909f6239f294532f68e91f94655aa881f2c8701293c9963e4b1c85b1a1a52
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5790922042 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:74e094a16d960a68e3691347bc7923c1f94b7db31dedb2ef74b9d87436170384`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 02 Dec 2020 17:42:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 09 Dec 2020 14:41:21 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Dec 2020 17:38:10 GMT
ENV NATS_DOCKERIZED=1
# Wed, 09 Dec 2020 23:04:27 GMT
ENV NATS_STREAMING_SERVER=0.19.0
# Wed, 09 Dec 2020 23:04:28 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.19.0/nats-streaming-server-v0.19.0-windows-amd64.zip
# Wed, 09 Dec 2020 23:04:28 GMT
ENV GIT_DOWNLOAD_SHA256=edafd6482bd71f3d6035d7f6871df1fd4c53acf0ac19e88b85e08a2c7ab1cec5
# Wed, 09 Dec 2020 23:05:39 GMT
RUN Set-PSDebug -Trace 2
# Wed, 09 Dec 2020 23:07:44 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 09 Dec 2020 23:07:45 GMT
EXPOSE 4222 8222
# Wed, 09 Dec 2020 23:07:46 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 09 Dec 2020 23:07:47 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d2696dc2a40dc121fc5acaa02242817ac416c69d17c113e2ac5136d21a3942d8`  
		Size: 1.7 GB (1698858125 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b5a79f8be42bf1c358ccc82f32c1481de95c393ef97e712a321c1440d132fda9`  
		Last Modified: Wed, 09 Dec 2020 17:11:03 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56d972336c8bcee0026c76e8f199cef405112a70aeef9917f07d2859f15162c1`  
		Last Modified: Wed, 09 Dec 2020 17:42:56 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e4f52064be159ebf6d7d967a842e39ae04b53dcf15dd8b582a77af431f81df7`  
		Last Modified: Wed, 09 Dec 2020 23:09:02 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54d1ecc24d286c8499d1698affa71481762f11bb3d4fdd9d35763dcbe94e9e9a`  
		Last Modified: Wed, 09 Dec 2020 23:09:00 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:649366889ec5703d27a79142f0331f2a462858d6d6ee2a7c1bd8e426bece4236`  
		Last Modified: Wed, 09 Dec 2020 23:08:59 GMT  
		Size: 1.1 KB (1139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9916349c9d6afe29e7418ee0e8f0454bb37038070600eaef872fb7356c1147d0`  
		Last Modified: Wed, 09 Dec 2020 23:08:59 GMT  
		Size: 5.5 MB (5528923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:838e032e6db488d413de3f4681555d2b57bb4472c3b16ed16a5c07f2e921f1ed`  
		Last Modified: Wed, 09 Dec 2020 23:09:01 GMT  
		Size: 16.5 MB (16540005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96a5c8ab334a9fbf340bbb2d213d16e91599eee98aafa72f7f8fbb6d4d147b27`  
		Last Modified: Wed, 09 Dec 2020 23:08:56 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09db5c24070ad330bcb0f078a2325aba107a3a8615fc004248d02e8e828fa8ce`  
		Last Modified: Wed, 09 Dec 2020 23:08:58 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21108015f9c4f2ee78087806b4ca0582f2618489ed4899b07b6290d743b8ef3d`  
		Last Modified: Wed, 09 Dec 2020 23:08:57 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.19-alpine`

```console
$ docker pull nats-streaming@sha256:5f15b51b2b447004408633f8f9458106fadad8f21393b1ed531071731e1ddb00
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.19-alpine` - linux; amd64

```console
$ docker pull nats-streaming@sha256:a8fcf986c14ae3ad60206bd6ebde23999c28f9967f05b9c81a760054539a683d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.6 MB (9567595 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b20b4ccbdde21c3fb61f4bd7fa3e83384f7e9d7f32f5bb86c88cd162a41403c0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Thu, 22 Oct 2020 02:19:24 GMT
ADD file:f17f65714f703db9012f00e5ec98d0b2541ff6147c2633f7ab9ba659d0c507f4 in / 
# Thu, 22 Oct 2020 02:19:24 GMT
CMD ["/bin/sh"]
# Tue, 03 Nov 2020 00:33:01 GMT
ENV NATS_STREAMING_SERVER=0.19.0
# Tue, 03 Nov 2020 00:33:03 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='d582023b8f9fe33b98f0faa6396aae8d5366ecade7e56cde912e21e5b93ea670' ;; 		armhf) natsArch='arm6'; sha256='f4af03e6cbb19f3ad9ea57217607dcf4b68018e1879859c847e2680917fc7139' ;; 		armv7) natsArch='arm7'; sha256='ec8c5ca693344e8b24de9ac955c38de757af8c5760658fc29ed2fbd804803fad' ;; 		x86_64) natsArch='amd64'; sha256='fc15530faec66b61de5140c2b99927c5839caff1c4c17f8bffbf4432fab83017' ;; 		x86) natsArch='386'; sha256='655f0f7cebf727317974006ad4a13ddacd3520f15266e854c2b01681e499bf80' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Tue, 03 Nov 2020 00:33:03 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Tue, 03 Nov 2020 00:33:04 GMT
EXPOSE 4222 8222
# Tue, 03 Nov 2020 00:33:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 03 Nov 2020 00:33:04 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:188c0c94c7c576fff0792aca7ec73d67a2f7f4cb3a6e53a84559337260b36964`  
		Last Modified: Thu, 22 Oct 2020 02:19:57 GMT  
		Size: 2.8 MB (2796860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f211ef5561f154a9a5957cdf08a625861df698594add9ba490a54259e9a01cb1`  
		Last Modified: Tue, 03 Nov 2020 00:33:28 GMT  
		Size: 6.8 MB (6770312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5eef7e98823e252892036fb4b7e5ccf695c556028fa2f7dd6dc314f625ba9eb9`  
		Last Modified: Tue, 03 Nov 2020 00:33:27 GMT  
		Size: 423.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.19-alpine` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:2a58d6644e94cc17212ec6a604029ebe9f855ceeee7fa66171bdc8aa6c7113ba
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.9 MB (8932203 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b8391afd58a04ec8cf1ab166357c9495c5aa4d32bc4bb4472e577874f42fe55d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Thu, 22 Oct 2020 02:01:09 GMT
ADD file:dec4d3b6cf21c59820d1d74a554d0a193b5f4859e00b932f31ffe73f554d5afb in / 
# Thu, 22 Oct 2020 02:01:12 GMT
CMD ["/bin/sh"]
# Mon, 02 Nov 2020 23:56:13 GMT
ENV NATS_STREAMING_SERVER=0.19.0
# Mon, 02 Nov 2020 23:56:17 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='d582023b8f9fe33b98f0faa6396aae8d5366ecade7e56cde912e21e5b93ea670' ;; 		armhf) natsArch='arm6'; sha256='f4af03e6cbb19f3ad9ea57217607dcf4b68018e1879859c847e2680917fc7139' ;; 		armv7) natsArch='arm7'; sha256='ec8c5ca693344e8b24de9ac955c38de757af8c5760658fc29ed2fbd804803fad' ;; 		x86_64) natsArch='amd64'; sha256='fc15530faec66b61de5140c2b99927c5839caff1c4c17f8bffbf4432fab83017' ;; 		x86) natsArch='386'; sha256='655f0f7cebf727317974006ad4a13ddacd3520f15266e854c2b01681e499bf80' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Mon, 02 Nov 2020 23:56:17 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Mon, 02 Nov 2020 23:56:18 GMT
EXPOSE 4222 8222
# Mon, 02 Nov 2020 23:56:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 02 Nov 2020 23:56:19 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:bad30e7b45c14f784ef29a828b5fc69db0ebdefebcde6a7c98f4f77ffc93a546`  
		Last Modified: Thu, 22 Oct 2020 02:01:42 GMT  
		Size: 2.6 MB (2601912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21cba1ed5b5094a02c017d654b758674905ec0bb2535d3311fcdd61dce32b319`  
		Last Modified: Mon, 02 Nov 2020 23:56:50 GMT  
		Size: 6.3 MB (6329871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3992f15ff4c1a7660c4a81854ec33d3e4973405c7095ceb0bd8a7865fff21c9f`  
		Last Modified: Mon, 02 Nov 2020 23:56:47 GMT  
		Size: 420.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.19-alpine` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:6a6c52fc272b91cff878ca25bddc432f19583a2e41e5e92288f0e64d0c649896
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.7 MB (8730479 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b4347330ee2d9b26f7fafaadc370627e71670505b340c9e4b54d791afcb3a6b2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Thu, 22 Oct 2020 01:58:13 GMT
ADD file:46f89172426e9f5b1d669a2ca7ab218fc2deaef1caeeab88f2b5bd443ac9773d in / 
# Thu, 22 Oct 2020 01:58:14 GMT
CMD ["/bin/sh"]
# Tue, 03 Nov 2020 00:05:05 GMT
ENV NATS_STREAMING_SERVER=0.19.0
# Tue, 03 Nov 2020 00:05:09 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='d582023b8f9fe33b98f0faa6396aae8d5366ecade7e56cde912e21e5b93ea670' ;; 		armhf) natsArch='arm6'; sha256='f4af03e6cbb19f3ad9ea57217607dcf4b68018e1879859c847e2680917fc7139' ;; 		armv7) natsArch='arm7'; sha256='ec8c5ca693344e8b24de9ac955c38de757af8c5760658fc29ed2fbd804803fad' ;; 		x86_64) natsArch='amd64'; sha256='fc15530faec66b61de5140c2b99927c5839caff1c4c17f8bffbf4432fab83017' ;; 		x86) natsArch='386'; sha256='655f0f7cebf727317974006ad4a13ddacd3520f15266e854c2b01681e499bf80' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Tue, 03 Nov 2020 00:05:09 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Tue, 03 Nov 2020 00:05:10 GMT
EXPOSE 4222 8222
# Tue, 03 Nov 2020 00:05:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 03 Nov 2020 00:05:11 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:5f2023fd85a4e68f37fe41421fd89f30e69b98a645613521c57c01317561eee3`  
		Last Modified: Thu, 22 Oct 2020 01:58:45 GMT  
		Size: 2.4 MB (2405675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34033d6dabe9c0f77f765bf2fce39f1eef24c163cfa802ec78f0e2e1bea9da7c`  
		Last Modified: Tue, 03 Nov 2020 00:05:43 GMT  
		Size: 6.3 MB (6324384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b0a98c9d7b5d859df80140920031b236b38ff88a4ff09d3bf8cfc5b9776e436`  
		Last Modified: Tue, 03 Nov 2020 00:05:40 GMT  
		Size: 420.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.19-alpine` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:36be57b574502addd00c81caaffedb9030eec583dbf4e3011a95aa7f998834aa
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.0 MB (8969159 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b947ac7936fa0250ecf3f1aaa6e22a928bdb3cdd8f0dcbbc3b8912a0678290c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Thu, 22 Oct 2020 02:01:01 GMT
ADD file:55c4e9752146061a2b5f76027221329f423687987c0744ef577130c60ff0ba42 in / 
# Thu, 22 Oct 2020 02:01:06 GMT
CMD ["/bin/sh"]
# Tue, 03 Nov 2020 00:43:12 GMT
ENV NATS_STREAMING_SERVER=0.19.0
# Tue, 03 Nov 2020 00:43:20 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='d582023b8f9fe33b98f0faa6396aae8d5366ecade7e56cde912e21e5b93ea670' ;; 		armhf) natsArch='arm6'; sha256='f4af03e6cbb19f3ad9ea57217607dcf4b68018e1879859c847e2680917fc7139' ;; 		armv7) natsArch='arm7'; sha256='ec8c5ca693344e8b24de9ac955c38de757af8c5760658fc29ed2fbd804803fad' ;; 		x86_64) natsArch='amd64'; sha256='fc15530faec66b61de5140c2b99927c5839caff1c4c17f8bffbf4432fab83017' ;; 		x86) natsArch='386'; sha256='655f0f7cebf727317974006ad4a13ddacd3520f15266e854c2b01681e499bf80' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Tue, 03 Nov 2020 00:43:21 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Tue, 03 Nov 2020 00:43:23 GMT
EXPOSE 4222 8222
# Tue, 03 Nov 2020 00:43:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 03 Nov 2020 00:43:27 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:5f621e34cdf485f410766dc9a0fc7855d17916d0f6583b58cbdce7c28831f527`  
		Last Modified: Thu, 22 Oct 2020 02:01:38 GMT  
		Size: 2.7 MB (2706555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfea83a41655c390ae2bea2fd6f2a83188ecb9c82e60ebde8040109e79a2eba5`  
		Last Modified: Tue, 03 Nov 2020 00:44:06 GMT  
		Size: 6.3 MB (6262183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0eca3d16e3b7142a6392c550b0efad91076053f222028892a3ae01e63f58dec`  
		Last Modified: Tue, 03 Nov 2020 00:44:05 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.19-alpine3.12`

```console
$ docker pull nats-streaming@sha256:5f15b51b2b447004408633f8f9458106fadad8f21393b1ed531071731e1ddb00
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.19-alpine3.12` - linux; amd64

```console
$ docker pull nats-streaming@sha256:a8fcf986c14ae3ad60206bd6ebde23999c28f9967f05b9c81a760054539a683d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.6 MB (9567595 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b20b4ccbdde21c3fb61f4bd7fa3e83384f7e9d7f32f5bb86c88cd162a41403c0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Thu, 22 Oct 2020 02:19:24 GMT
ADD file:f17f65714f703db9012f00e5ec98d0b2541ff6147c2633f7ab9ba659d0c507f4 in / 
# Thu, 22 Oct 2020 02:19:24 GMT
CMD ["/bin/sh"]
# Tue, 03 Nov 2020 00:33:01 GMT
ENV NATS_STREAMING_SERVER=0.19.0
# Tue, 03 Nov 2020 00:33:03 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='d582023b8f9fe33b98f0faa6396aae8d5366ecade7e56cde912e21e5b93ea670' ;; 		armhf) natsArch='arm6'; sha256='f4af03e6cbb19f3ad9ea57217607dcf4b68018e1879859c847e2680917fc7139' ;; 		armv7) natsArch='arm7'; sha256='ec8c5ca693344e8b24de9ac955c38de757af8c5760658fc29ed2fbd804803fad' ;; 		x86_64) natsArch='amd64'; sha256='fc15530faec66b61de5140c2b99927c5839caff1c4c17f8bffbf4432fab83017' ;; 		x86) natsArch='386'; sha256='655f0f7cebf727317974006ad4a13ddacd3520f15266e854c2b01681e499bf80' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Tue, 03 Nov 2020 00:33:03 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Tue, 03 Nov 2020 00:33:04 GMT
EXPOSE 4222 8222
# Tue, 03 Nov 2020 00:33:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 03 Nov 2020 00:33:04 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:188c0c94c7c576fff0792aca7ec73d67a2f7f4cb3a6e53a84559337260b36964`  
		Last Modified: Thu, 22 Oct 2020 02:19:57 GMT  
		Size: 2.8 MB (2796860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f211ef5561f154a9a5957cdf08a625861df698594add9ba490a54259e9a01cb1`  
		Last Modified: Tue, 03 Nov 2020 00:33:28 GMT  
		Size: 6.8 MB (6770312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5eef7e98823e252892036fb4b7e5ccf695c556028fa2f7dd6dc314f625ba9eb9`  
		Last Modified: Tue, 03 Nov 2020 00:33:27 GMT  
		Size: 423.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.19-alpine3.12` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:2a58d6644e94cc17212ec6a604029ebe9f855ceeee7fa66171bdc8aa6c7113ba
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.9 MB (8932203 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b8391afd58a04ec8cf1ab166357c9495c5aa4d32bc4bb4472e577874f42fe55d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Thu, 22 Oct 2020 02:01:09 GMT
ADD file:dec4d3b6cf21c59820d1d74a554d0a193b5f4859e00b932f31ffe73f554d5afb in / 
# Thu, 22 Oct 2020 02:01:12 GMT
CMD ["/bin/sh"]
# Mon, 02 Nov 2020 23:56:13 GMT
ENV NATS_STREAMING_SERVER=0.19.0
# Mon, 02 Nov 2020 23:56:17 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='d582023b8f9fe33b98f0faa6396aae8d5366ecade7e56cde912e21e5b93ea670' ;; 		armhf) natsArch='arm6'; sha256='f4af03e6cbb19f3ad9ea57217607dcf4b68018e1879859c847e2680917fc7139' ;; 		armv7) natsArch='arm7'; sha256='ec8c5ca693344e8b24de9ac955c38de757af8c5760658fc29ed2fbd804803fad' ;; 		x86_64) natsArch='amd64'; sha256='fc15530faec66b61de5140c2b99927c5839caff1c4c17f8bffbf4432fab83017' ;; 		x86) natsArch='386'; sha256='655f0f7cebf727317974006ad4a13ddacd3520f15266e854c2b01681e499bf80' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Mon, 02 Nov 2020 23:56:17 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Mon, 02 Nov 2020 23:56:18 GMT
EXPOSE 4222 8222
# Mon, 02 Nov 2020 23:56:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 02 Nov 2020 23:56:19 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:bad30e7b45c14f784ef29a828b5fc69db0ebdefebcde6a7c98f4f77ffc93a546`  
		Last Modified: Thu, 22 Oct 2020 02:01:42 GMT  
		Size: 2.6 MB (2601912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21cba1ed5b5094a02c017d654b758674905ec0bb2535d3311fcdd61dce32b319`  
		Last Modified: Mon, 02 Nov 2020 23:56:50 GMT  
		Size: 6.3 MB (6329871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3992f15ff4c1a7660c4a81854ec33d3e4973405c7095ceb0bd8a7865fff21c9f`  
		Last Modified: Mon, 02 Nov 2020 23:56:47 GMT  
		Size: 420.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.19-alpine3.12` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:6a6c52fc272b91cff878ca25bddc432f19583a2e41e5e92288f0e64d0c649896
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.7 MB (8730479 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b4347330ee2d9b26f7fafaadc370627e71670505b340c9e4b54d791afcb3a6b2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Thu, 22 Oct 2020 01:58:13 GMT
ADD file:46f89172426e9f5b1d669a2ca7ab218fc2deaef1caeeab88f2b5bd443ac9773d in / 
# Thu, 22 Oct 2020 01:58:14 GMT
CMD ["/bin/sh"]
# Tue, 03 Nov 2020 00:05:05 GMT
ENV NATS_STREAMING_SERVER=0.19.0
# Tue, 03 Nov 2020 00:05:09 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='d582023b8f9fe33b98f0faa6396aae8d5366ecade7e56cde912e21e5b93ea670' ;; 		armhf) natsArch='arm6'; sha256='f4af03e6cbb19f3ad9ea57217607dcf4b68018e1879859c847e2680917fc7139' ;; 		armv7) natsArch='arm7'; sha256='ec8c5ca693344e8b24de9ac955c38de757af8c5760658fc29ed2fbd804803fad' ;; 		x86_64) natsArch='amd64'; sha256='fc15530faec66b61de5140c2b99927c5839caff1c4c17f8bffbf4432fab83017' ;; 		x86) natsArch='386'; sha256='655f0f7cebf727317974006ad4a13ddacd3520f15266e854c2b01681e499bf80' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Tue, 03 Nov 2020 00:05:09 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Tue, 03 Nov 2020 00:05:10 GMT
EXPOSE 4222 8222
# Tue, 03 Nov 2020 00:05:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 03 Nov 2020 00:05:11 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:5f2023fd85a4e68f37fe41421fd89f30e69b98a645613521c57c01317561eee3`  
		Last Modified: Thu, 22 Oct 2020 01:58:45 GMT  
		Size: 2.4 MB (2405675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34033d6dabe9c0f77f765bf2fce39f1eef24c163cfa802ec78f0e2e1bea9da7c`  
		Last Modified: Tue, 03 Nov 2020 00:05:43 GMT  
		Size: 6.3 MB (6324384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b0a98c9d7b5d859df80140920031b236b38ff88a4ff09d3bf8cfc5b9776e436`  
		Last Modified: Tue, 03 Nov 2020 00:05:40 GMT  
		Size: 420.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.19-alpine3.12` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:36be57b574502addd00c81caaffedb9030eec583dbf4e3011a95aa7f998834aa
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.0 MB (8969159 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b947ac7936fa0250ecf3f1aaa6e22a928bdb3cdd8f0dcbbc3b8912a0678290c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Thu, 22 Oct 2020 02:01:01 GMT
ADD file:55c4e9752146061a2b5f76027221329f423687987c0744ef577130c60ff0ba42 in / 
# Thu, 22 Oct 2020 02:01:06 GMT
CMD ["/bin/sh"]
# Tue, 03 Nov 2020 00:43:12 GMT
ENV NATS_STREAMING_SERVER=0.19.0
# Tue, 03 Nov 2020 00:43:20 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='d582023b8f9fe33b98f0faa6396aae8d5366ecade7e56cde912e21e5b93ea670' ;; 		armhf) natsArch='arm6'; sha256='f4af03e6cbb19f3ad9ea57217607dcf4b68018e1879859c847e2680917fc7139' ;; 		armv7) natsArch='arm7'; sha256='ec8c5ca693344e8b24de9ac955c38de757af8c5760658fc29ed2fbd804803fad' ;; 		x86_64) natsArch='amd64'; sha256='fc15530faec66b61de5140c2b99927c5839caff1c4c17f8bffbf4432fab83017' ;; 		x86) natsArch='386'; sha256='655f0f7cebf727317974006ad4a13ddacd3520f15266e854c2b01681e499bf80' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Tue, 03 Nov 2020 00:43:21 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Tue, 03 Nov 2020 00:43:23 GMT
EXPOSE 4222 8222
# Tue, 03 Nov 2020 00:43:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 03 Nov 2020 00:43:27 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:5f621e34cdf485f410766dc9a0fc7855d17916d0f6583b58cbdce7c28831f527`  
		Last Modified: Thu, 22 Oct 2020 02:01:38 GMT  
		Size: 2.7 MB (2706555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfea83a41655c390ae2bea2fd6f2a83188ecb9c82e60ebde8040109e79a2eba5`  
		Last Modified: Tue, 03 Nov 2020 00:44:06 GMT  
		Size: 6.3 MB (6262183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0eca3d16e3b7142a6392c550b0efad91076053f222028892a3ae01e63f58dec`  
		Last Modified: Tue, 03 Nov 2020 00:44:05 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.19-linux`

```console
$ docker pull nats-streaming@sha256:8001e4db36785bd692d9ae1c9ed3857d972692b385e36c08994794a5254bb78a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.19-linux` - linux; amd64

```console
$ docker pull nats-streaming@sha256:053a4ca3955b9c5036e48bafb96c83003fe86c34c6928934e3fd1db0529a889c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 MB (6487259 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:993a204b53252cabfc16952c1d2dc014dc6518d1a08d00bda1bc5008a139e37a`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 03 Nov 2020 00:33:13 GMT
COPY file:3ed83d1497b0535960e452435cb8b27e347f48da12693aa27ebaf9bff94d82de in /nats-streaming-server 
# Tue, 03 Nov 2020 00:33:13 GMT
EXPOSE 4222 8222
# Tue, 03 Nov 2020 00:33:14 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 03 Nov 2020 00:33:14 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:57ac21f890a508f609eabea265197b18ce9dfe3e694034c7a06d37b536a707b2`  
		Last Modified: Tue, 03 Nov 2020 00:33:37 GMT  
		Size: 6.5 MB (6487259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.19-linux` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:f334d10ef2a4663d8d7d920d96321cd97f050b82a5d55d588192f074f60dd814
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 MB (6049845 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9eecfd5ab4178a65e952a7cf1d248a556a6ae2c328ac8b68923146d64734db03`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 02 Nov 2020 23:56:28 GMT
COPY file:d6896b1c93dcd497494c972f9274fcc634a4f4a8d63a0191bdb87f6336aec0d7 in /nats-streaming-server 
# Mon, 02 Nov 2020 23:56:28 GMT
EXPOSE 4222 8222
# Mon, 02 Nov 2020 23:56:29 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 02 Nov 2020 23:56:29 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:7f165fb71ab77e8081dbfa13656cdf9e5e005002d6c3afa0aac40667a0f97af8`  
		Last Modified: Mon, 02 Nov 2020 23:57:04 GMT  
		Size: 6.0 MB (6049845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.19-linux` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:5fd0943909d8aedafb888e099c9f64d234023ad780805ed7c939692ebfd8304d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 MB (6043163 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f37071e856ae40dc3c8c5e10b359d1640fd67a6110741c0957af2031032ed6ce`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 03 Nov 2020 00:05:23 GMT
COPY file:d232132ddff1d85d3a2f5c80a91c80023cbc103d816387e06d604cf97238e52c in /nats-streaming-server 
# Tue, 03 Nov 2020 00:05:24 GMT
EXPOSE 4222 8222
# Tue, 03 Nov 2020 00:05:24 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 03 Nov 2020 00:05:25 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:9c7227cc1040d04ca7763cfb53ab58bc32ae54921990516adf8e13374ac9ef29`  
		Last Modified: Tue, 03 Nov 2020 00:05:57 GMT  
		Size: 6.0 MB (6043163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.19-linux` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:c058fd3e9a8ac44263bf53fa2f6f1e8e8cb3e95cd223f8353fdafc50fe57e417
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 MB (5978846 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7c915a80bd440362bd4a6743fee8134a3caf6271e3258e449fb106b19c050a3b`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 03 Nov 2020 00:43:38 GMT
COPY file:55e70ee826cd5a662497337a2488e22833672bd031d85b4ee39556ab1e80df08 in /nats-streaming-server 
# Tue, 03 Nov 2020 00:43:40 GMT
EXPOSE 4222 8222
# Tue, 03 Nov 2020 00:43:42 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 03 Nov 2020 00:43:43 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:3dc58a59de8a6ed19e9144b0189eb3b637a9e7fcd76ec6c6dc47561b2740a3a2`  
		Last Modified: Tue, 03 Nov 2020 00:44:19 GMT  
		Size: 6.0 MB (5978846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.19-nanoserver`

```console
$ docker pull nats-streaming@sha256:4a013f6e621b040ed030861cb0bd02d96ef23c7a5fbf2019841921e255379ebf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1637; amd64

### `nats-streaming:0.19-nanoserver` - windows version 10.0.17763.1637; amd64

```console
$ docker pull nats-streaming@sha256:9444afab14740d43bfd213340272edcfaa96f83b2ae24d586333398cc089a858
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.8 MB (107783475 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:85bdcab4235f3b70b1671972c4154790bde79e33644ae254ae48efa965b2b3cb`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 03 Dec 2020 08:05:47 GMT
RUN Apply image 1809-amd64
# Wed, 09 Dec 2020 17:38:01 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 09 Dec 2020 23:04:19 GMT
RUN cmd /S /C #(nop) COPY file:cc6bae0f50b6e35b12e8233f240d95e093f7e44257bc87e06aed691866ec1477 in C:\nats-streaming-server.exe 
# Wed, 09 Dec 2020 23:04:21 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 09 Dec 2020 23:04:21 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 09 Dec 2020 23:04:22 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:21be49aa856f07be4e0a677b988e43c04bd595a3c858e58b6c364477bbbf7222`  
		Size: 101.3 MB (101264827 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8a3891744a5ba41f01e625a0a70d755ffe93de4d4f124ad6d069420d5c7956d4`  
		Last Modified: Wed, 09 Dec 2020 17:42:32 GMT  
		Size: 893.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab2cf2a7f92a640dc1125e539b41a28abc6b4e2df892f67cbc0072f90bb65509`  
		Last Modified: Wed, 09 Dec 2020 23:08:42 GMT  
		Size: 6.5 MB (6515155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf561da2a706a067845b617e3efccdaf8257da5fb1ae53c383e29559f5220612`  
		Last Modified: Wed, 09 Dec 2020 23:08:41 GMT  
		Size: 869.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1e5e4a71ea08fded20e3471625c1c06c12540fd3c7f4e12eeaee288bf6e5377`  
		Last Modified: Wed, 09 Dec 2020 23:08:39 GMT  
		Size: 864.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5d7a7dbf47aa9dfd9ed44ec162d12b58d6751c6d5f129c4e65250e21fde3631`  
		Last Modified: Wed, 09 Dec 2020 23:08:41 GMT  
		Size: 867.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.19-nanoserver-1809`

```console
$ docker pull nats-streaming@sha256:4a013f6e621b040ed030861cb0bd02d96ef23c7a5fbf2019841921e255379ebf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1637; amd64

### `nats-streaming:0.19-nanoserver-1809` - windows version 10.0.17763.1637; amd64

```console
$ docker pull nats-streaming@sha256:9444afab14740d43bfd213340272edcfaa96f83b2ae24d586333398cc089a858
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.8 MB (107783475 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:85bdcab4235f3b70b1671972c4154790bde79e33644ae254ae48efa965b2b3cb`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 03 Dec 2020 08:05:47 GMT
RUN Apply image 1809-amd64
# Wed, 09 Dec 2020 17:38:01 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 09 Dec 2020 23:04:19 GMT
RUN cmd /S /C #(nop) COPY file:cc6bae0f50b6e35b12e8233f240d95e093f7e44257bc87e06aed691866ec1477 in C:\nats-streaming-server.exe 
# Wed, 09 Dec 2020 23:04:21 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 09 Dec 2020 23:04:21 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 09 Dec 2020 23:04:22 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:21be49aa856f07be4e0a677b988e43c04bd595a3c858e58b6c364477bbbf7222`  
		Size: 101.3 MB (101264827 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8a3891744a5ba41f01e625a0a70d755ffe93de4d4f124ad6d069420d5c7956d4`  
		Last Modified: Wed, 09 Dec 2020 17:42:32 GMT  
		Size: 893.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab2cf2a7f92a640dc1125e539b41a28abc6b4e2df892f67cbc0072f90bb65509`  
		Last Modified: Wed, 09 Dec 2020 23:08:42 GMT  
		Size: 6.5 MB (6515155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf561da2a706a067845b617e3efccdaf8257da5fb1ae53c383e29559f5220612`  
		Last Modified: Wed, 09 Dec 2020 23:08:41 GMT  
		Size: 869.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1e5e4a71ea08fded20e3471625c1c06c12540fd3c7f4e12eeaee288bf6e5377`  
		Last Modified: Wed, 09 Dec 2020 23:08:39 GMT  
		Size: 864.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5d7a7dbf47aa9dfd9ed44ec162d12b58d6751c6d5f129c4e65250e21fde3631`  
		Last Modified: Wed, 09 Dec 2020 23:08:41 GMT  
		Size: 867.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.19-scratch`

```console
$ docker pull nats-streaming@sha256:8001e4db36785bd692d9ae1c9ed3857d972692b385e36c08994794a5254bb78a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.19-scratch` - linux; amd64

```console
$ docker pull nats-streaming@sha256:053a4ca3955b9c5036e48bafb96c83003fe86c34c6928934e3fd1db0529a889c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 MB (6487259 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:993a204b53252cabfc16952c1d2dc014dc6518d1a08d00bda1bc5008a139e37a`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 03 Nov 2020 00:33:13 GMT
COPY file:3ed83d1497b0535960e452435cb8b27e347f48da12693aa27ebaf9bff94d82de in /nats-streaming-server 
# Tue, 03 Nov 2020 00:33:13 GMT
EXPOSE 4222 8222
# Tue, 03 Nov 2020 00:33:14 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 03 Nov 2020 00:33:14 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:57ac21f890a508f609eabea265197b18ce9dfe3e694034c7a06d37b536a707b2`  
		Last Modified: Tue, 03 Nov 2020 00:33:37 GMT  
		Size: 6.5 MB (6487259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.19-scratch` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:f334d10ef2a4663d8d7d920d96321cd97f050b82a5d55d588192f074f60dd814
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 MB (6049845 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9eecfd5ab4178a65e952a7cf1d248a556a6ae2c328ac8b68923146d64734db03`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 02 Nov 2020 23:56:28 GMT
COPY file:d6896b1c93dcd497494c972f9274fcc634a4f4a8d63a0191bdb87f6336aec0d7 in /nats-streaming-server 
# Mon, 02 Nov 2020 23:56:28 GMT
EXPOSE 4222 8222
# Mon, 02 Nov 2020 23:56:29 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 02 Nov 2020 23:56:29 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:7f165fb71ab77e8081dbfa13656cdf9e5e005002d6c3afa0aac40667a0f97af8`  
		Last Modified: Mon, 02 Nov 2020 23:57:04 GMT  
		Size: 6.0 MB (6049845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.19-scratch` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:5fd0943909d8aedafb888e099c9f64d234023ad780805ed7c939692ebfd8304d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 MB (6043163 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f37071e856ae40dc3c8c5e10b359d1640fd67a6110741c0957af2031032ed6ce`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 03 Nov 2020 00:05:23 GMT
COPY file:d232132ddff1d85d3a2f5c80a91c80023cbc103d816387e06d604cf97238e52c in /nats-streaming-server 
# Tue, 03 Nov 2020 00:05:24 GMT
EXPOSE 4222 8222
# Tue, 03 Nov 2020 00:05:24 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 03 Nov 2020 00:05:25 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:9c7227cc1040d04ca7763cfb53ab58bc32ae54921990516adf8e13374ac9ef29`  
		Last Modified: Tue, 03 Nov 2020 00:05:57 GMT  
		Size: 6.0 MB (6043163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.19-scratch` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:c058fd3e9a8ac44263bf53fa2f6f1e8e8cb3e95cd223f8353fdafc50fe57e417
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 MB (5978846 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7c915a80bd440362bd4a6743fee8134a3caf6271e3258e449fb106b19c050a3b`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 03 Nov 2020 00:43:38 GMT
COPY file:55e70ee826cd5a662497337a2488e22833672bd031d85b4ee39556ab1e80df08 in /nats-streaming-server 
# Tue, 03 Nov 2020 00:43:40 GMT
EXPOSE 4222 8222
# Tue, 03 Nov 2020 00:43:42 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 03 Nov 2020 00:43:43 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:3dc58a59de8a6ed19e9144b0189eb3b637a9e7fcd76ec6c6dc47561b2740a3a2`  
		Last Modified: Tue, 03 Nov 2020 00:44:19 GMT  
		Size: 6.0 MB (5978846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.19-windowsservercore`

```console
$ docker pull nats-streaming@sha256:78cddd38d3c26f2a74454532132969b5fbc9fbff9cc8708cf338c1b33a80c17b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1637; amd64
	-	windows version 10.0.14393.4104; amd64

### `nats-streaming:0.19-windowsservercore` - windows version 10.0.17763.1637; amd64

```console
$ docker pull nats-streaming@sha256:7a8ab0956821d178ef84f6f10c399d44005ca86dd75378d41a5980979ed24409
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2411449594 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0146757e90d9c2df66c7933b807c71d62de612813d33a32f15c8d7fdd710ddae`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 04 Dec 2020 02:13:01 GMT
RUN Install update 1809-amd64
# Wed, 09 Dec 2020 14:02:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Dec 2020 17:36:04 GMT
ENV NATS_DOCKERIZED=1
# Wed, 09 Dec 2020 23:02:20 GMT
ENV NATS_STREAMING_SERVER=0.19.0
# Wed, 09 Dec 2020 23:02:21 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.19.0/nats-streaming-server-v0.19.0-windows-amd64.zip
# Wed, 09 Dec 2020 23:02:22 GMT
ENV GIT_DOWNLOAD_SHA256=edafd6482bd71f3d6035d7f6871df1fd4c53acf0ac19e88b85e08a2c7ab1cec5
# Wed, 09 Dec 2020 23:02:52 GMT
RUN Set-PSDebug -Trace 2
# Wed, 09 Dec 2020 23:04:09 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 09 Dec 2020 23:04:10 GMT
EXPOSE 4222 8222
# Wed, 09 Dec 2020 23:04:12 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 09 Dec 2020 23:04:13 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:aa4f58cd6da1aaf1a0b44d443bd88e7fbe5b0a6f193995a1a61d6bd63990f314`  
		Size: 672.5 MB (672541583 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:240407eb82b6591b0574396ec829a4a5cd9a75257a4663f9876942995275965d`  
		Last Modified: Wed, 09 Dec 2020 17:10:14 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82b9257be76bd37cad15d45905ec5910266409794a9dbd8a0428174f8b2f352a`  
		Last Modified: Wed, 09 Dec 2020 17:42:00 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36644685392e418bf32ab96db81c8f6a861b913256c244637d9d3ee45098a9cb`  
		Last Modified: Wed, 09 Dec 2020 23:08:22 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9469bed00eb5f6a5b7c050a1aaee856134ec78bab6076cc793e26dc52ec71fa`  
		Last Modified: Wed, 09 Dec 2020 23:08:21 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94e9d451908e3e8ec10448e052cf25767a282312e49e29d2a0b42652cf217e28`  
		Last Modified: Wed, 09 Dec 2020 23:08:21 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:870e3bb830bd8ad9b84a928d2b858be730dcdba8016206ee4aeda623d98754b3`  
		Last Modified: Wed, 09 Dec 2020 23:08:20 GMT  
		Size: 4.8 MB (4843348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14d24c0a2fc2b3ecd1b0467794ae95667a29e1bd550bf2bf9c455499839253bc`  
		Last Modified: Wed, 09 Dec 2020 23:08:23 GMT  
		Size: 15.7 MB (15722612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09371bf015245c95ce8d5db6b8d7f90fc6d8527f83101535c8c6af719b628e79`  
		Last Modified: Wed, 09 Dec 2020 23:08:18 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76ff8db511e98efbde9cbbf6ecd2d9bd2b73565c7c4e0d24dddeb6edfa2a1875`  
		Last Modified: Wed, 09 Dec 2020 23:08:18 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13217bf3886546791bd6c26ab23636f9bc595fd80abf1e7d6ab6f10f8613cdee`  
		Last Modified: Wed, 09 Dec 2020 23:08:18 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.19-windowsservercore` - windows version 10.0.14393.4104; amd64

```console
$ docker pull nats-streaming@sha256:33a909f6239f294532f68e91f94655aa881f2c8701293c9963e4b1c85b1a1a52
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5790922042 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:74e094a16d960a68e3691347bc7923c1f94b7db31dedb2ef74b9d87436170384`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 02 Dec 2020 17:42:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 09 Dec 2020 14:41:21 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Dec 2020 17:38:10 GMT
ENV NATS_DOCKERIZED=1
# Wed, 09 Dec 2020 23:04:27 GMT
ENV NATS_STREAMING_SERVER=0.19.0
# Wed, 09 Dec 2020 23:04:28 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.19.0/nats-streaming-server-v0.19.0-windows-amd64.zip
# Wed, 09 Dec 2020 23:04:28 GMT
ENV GIT_DOWNLOAD_SHA256=edafd6482bd71f3d6035d7f6871df1fd4c53acf0ac19e88b85e08a2c7ab1cec5
# Wed, 09 Dec 2020 23:05:39 GMT
RUN Set-PSDebug -Trace 2
# Wed, 09 Dec 2020 23:07:44 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 09 Dec 2020 23:07:45 GMT
EXPOSE 4222 8222
# Wed, 09 Dec 2020 23:07:46 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 09 Dec 2020 23:07:47 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d2696dc2a40dc121fc5acaa02242817ac416c69d17c113e2ac5136d21a3942d8`  
		Size: 1.7 GB (1698858125 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b5a79f8be42bf1c358ccc82f32c1481de95c393ef97e712a321c1440d132fda9`  
		Last Modified: Wed, 09 Dec 2020 17:11:03 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56d972336c8bcee0026c76e8f199cef405112a70aeef9917f07d2859f15162c1`  
		Last Modified: Wed, 09 Dec 2020 17:42:56 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e4f52064be159ebf6d7d967a842e39ae04b53dcf15dd8b582a77af431f81df7`  
		Last Modified: Wed, 09 Dec 2020 23:09:02 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54d1ecc24d286c8499d1698affa71481762f11bb3d4fdd9d35763dcbe94e9e9a`  
		Last Modified: Wed, 09 Dec 2020 23:09:00 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:649366889ec5703d27a79142f0331f2a462858d6d6ee2a7c1bd8e426bece4236`  
		Last Modified: Wed, 09 Dec 2020 23:08:59 GMT  
		Size: 1.1 KB (1139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9916349c9d6afe29e7418ee0e8f0454bb37038070600eaef872fb7356c1147d0`  
		Last Modified: Wed, 09 Dec 2020 23:08:59 GMT  
		Size: 5.5 MB (5528923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:838e032e6db488d413de3f4681555d2b57bb4472c3b16ed16a5c07f2e921f1ed`  
		Last Modified: Wed, 09 Dec 2020 23:09:01 GMT  
		Size: 16.5 MB (16540005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96a5c8ab334a9fbf340bbb2d213d16e91599eee98aafa72f7f8fbb6d4d147b27`  
		Last Modified: Wed, 09 Dec 2020 23:08:56 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09db5c24070ad330bcb0f078a2325aba107a3a8615fc004248d02e8e828fa8ce`  
		Last Modified: Wed, 09 Dec 2020 23:08:58 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21108015f9c4f2ee78087806b4ca0582f2618489ed4899b07b6290d743b8ef3d`  
		Last Modified: Wed, 09 Dec 2020 23:08:57 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.19-windowsservercore-1809`

```console
$ docker pull nats-streaming@sha256:3a285fa7c8c148aad627e61b6848554ccc223cb30a1eb3293a5a5fb89af016c6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1637; amd64

### `nats-streaming:0.19-windowsservercore-1809` - windows version 10.0.17763.1637; amd64

```console
$ docker pull nats-streaming@sha256:7a8ab0956821d178ef84f6f10c399d44005ca86dd75378d41a5980979ed24409
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2411449594 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0146757e90d9c2df66c7933b807c71d62de612813d33a32f15c8d7fdd710ddae`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 04 Dec 2020 02:13:01 GMT
RUN Install update 1809-amd64
# Wed, 09 Dec 2020 14:02:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Dec 2020 17:36:04 GMT
ENV NATS_DOCKERIZED=1
# Wed, 09 Dec 2020 23:02:20 GMT
ENV NATS_STREAMING_SERVER=0.19.0
# Wed, 09 Dec 2020 23:02:21 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.19.0/nats-streaming-server-v0.19.0-windows-amd64.zip
# Wed, 09 Dec 2020 23:02:22 GMT
ENV GIT_DOWNLOAD_SHA256=edafd6482bd71f3d6035d7f6871df1fd4c53acf0ac19e88b85e08a2c7ab1cec5
# Wed, 09 Dec 2020 23:02:52 GMT
RUN Set-PSDebug -Trace 2
# Wed, 09 Dec 2020 23:04:09 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 09 Dec 2020 23:04:10 GMT
EXPOSE 4222 8222
# Wed, 09 Dec 2020 23:04:12 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 09 Dec 2020 23:04:13 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:aa4f58cd6da1aaf1a0b44d443bd88e7fbe5b0a6f193995a1a61d6bd63990f314`  
		Size: 672.5 MB (672541583 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:240407eb82b6591b0574396ec829a4a5cd9a75257a4663f9876942995275965d`  
		Last Modified: Wed, 09 Dec 2020 17:10:14 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82b9257be76bd37cad15d45905ec5910266409794a9dbd8a0428174f8b2f352a`  
		Last Modified: Wed, 09 Dec 2020 17:42:00 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36644685392e418bf32ab96db81c8f6a861b913256c244637d9d3ee45098a9cb`  
		Last Modified: Wed, 09 Dec 2020 23:08:22 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9469bed00eb5f6a5b7c050a1aaee856134ec78bab6076cc793e26dc52ec71fa`  
		Last Modified: Wed, 09 Dec 2020 23:08:21 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94e9d451908e3e8ec10448e052cf25767a282312e49e29d2a0b42652cf217e28`  
		Last Modified: Wed, 09 Dec 2020 23:08:21 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:870e3bb830bd8ad9b84a928d2b858be730dcdba8016206ee4aeda623d98754b3`  
		Last Modified: Wed, 09 Dec 2020 23:08:20 GMT  
		Size: 4.8 MB (4843348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14d24c0a2fc2b3ecd1b0467794ae95667a29e1bd550bf2bf9c455499839253bc`  
		Last Modified: Wed, 09 Dec 2020 23:08:23 GMT  
		Size: 15.7 MB (15722612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09371bf015245c95ce8d5db6b8d7f90fc6d8527f83101535c8c6af719b628e79`  
		Last Modified: Wed, 09 Dec 2020 23:08:18 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76ff8db511e98efbde9cbbf6ecd2d9bd2b73565c7c4e0d24dddeb6edfa2a1875`  
		Last Modified: Wed, 09 Dec 2020 23:08:18 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13217bf3886546791bd6c26ab23636f9bc595fd80abf1e7d6ab6f10f8613cdee`  
		Last Modified: Wed, 09 Dec 2020 23:08:18 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.19-windowsservercore-ltsc2016`

```console
$ docker pull nats-streaming@sha256:da877310cb87d1822f44a79a76b57af2eceb3e15aa82ab406a47d32bc0de9f47
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4104; amd64

### `nats-streaming:0.19-windowsservercore-ltsc2016` - windows version 10.0.14393.4104; amd64

```console
$ docker pull nats-streaming@sha256:33a909f6239f294532f68e91f94655aa881f2c8701293c9963e4b1c85b1a1a52
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5790922042 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:74e094a16d960a68e3691347bc7923c1f94b7db31dedb2ef74b9d87436170384`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 02 Dec 2020 17:42:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 09 Dec 2020 14:41:21 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Dec 2020 17:38:10 GMT
ENV NATS_DOCKERIZED=1
# Wed, 09 Dec 2020 23:04:27 GMT
ENV NATS_STREAMING_SERVER=0.19.0
# Wed, 09 Dec 2020 23:04:28 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.19.0/nats-streaming-server-v0.19.0-windows-amd64.zip
# Wed, 09 Dec 2020 23:04:28 GMT
ENV GIT_DOWNLOAD_SHA256=edafd6482bd71f3d6035d7f6871df1fd4c53acf0ac19e88b85e08a2c7ab1cec5
# Wed, 09 Dec 2020 23:05:39 GMT
RUN Set-PSDebug -Trace 2
# Wed, 09 Dec 2020 23:07:44 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 09 Dec 2020 23:07:45 GMT
EXPOSE 4222 8222
# Wed, 09 Dec 2020 23:07:46 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 09 Dec 2020 23:07:47 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d2696dc2a40dc121fc5acaa02242817ac416c69d17c113e2ac5136d21a3942d8`  
		Size: 1.7 GB (1698858125 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b5a79f8be42bf1c358ccc82f32c1481de95c393ef97e712a321c1440d132fda9`  
		Last Modified: Wed, 09 Dec 2020 17:11:03 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56d972336c8bcee0026c76e8f199cef405112a70aeef9917f07d2859f15162c1`  
		Last Modified: Wed, 09 Dec 2020 17:42:56 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e4f52064be159ebf6d7d967a842e39ae04b53dcf15dd8b582a77af431f81df7`  
		Last Modified: Wed, 09 Dec 2020 23:09:02 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54d1ecc24d286c8499d1698affa71481762f11bb3d4fdd9d35763dcbe94e9e9a`  
		Last Modified: Wed, 09 Dec 2020 23:09:00 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:649366889ec5703d27a79142f0331f2a462858d6d6ee2a7c1bd8e426bece4236`  
		Last Modified: Wed, 09 Dec 2020 23:08:59 GMT  
		Size: 1.1 KB (1139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9916349c9d6afe29e7418ee0e8f0454bb37038070600eaef872fb7356c1147d0`  
		Last Modified: Wed, 09 Dec 2020 23:08:59 GMT  
		Size: 5.5 MB (5528923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:838e032e6db488d413de3f4681555d2b57bb4472c3b16ed16a5c07f2e921f1ed`  
		Last Modified: Wed, 09 Dec 2020 23:09:01 GMT  
		Size: 16.5 MB (16540005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96a5c8ab334a9fbf340bbb2d213d16e91599eee98aafa72f7f8fbb6d4d147b27`  
		Last Modified: Wed, 09 Dec 2020 23:08:56 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09db5c24070ad330bcb0f078a2325aba107a3a8615fc004248d02e8e828fa8ce`  
		Last Modified: Wed, 09 Dec 2020 23:08:58 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21108015f9c4f2ee78087806b4ca0582f2618489ed4899b07b6290d743b8ef3d`  
		Last Modified: Wed, 09 Dec 2020 23:08:57 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:alpine`

```console
$ docker pull nats-streaming@sha256:5f15b51b2b447004408633f8f9458106fadad8f21393b1ed531071731e1ddb00
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:alpine` - linux; amd64

```console
$ docker pull nats-streaming@sha256:a8fcf986c14ae3ad60206bd6ebde23999c28f9967f05b9c81a760054539a683d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.6 MB (9567595 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b20b4ccbdde21c3fb61f4bd7fa3e83384f7e9d7f32f5bb86c88cd162a41403c0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Thu, 22 Oct 2020 02:19:24 GMT
ADD file:f17f65714f703db9012f00e5ec98d0b2541ff6147c2633f7ab9ba659d0c507f4 in / 
# Thu, 22 Oct 2020 02:19:24 GMT
CMD ["/bin/sh"]
# Tue, 03 Nov 2020 00:33:01 GMT
ENV NATS_STREAMING_SERVER=0.19.0
# Tue, 03 Nov 2020 00:33:03 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='d582023b8f9fe33b98f0faa6396aae8d5366ecade7e56cde912e21e5b93ea670' ;; 		armhf) natsArch='arm6'; sha256='f4af03e6cbb19f3ad9ea57217607dcf4b68018e1879859c847e2680917fc7139' ;; 		armv7) natsArch='arm7'; sha256='ec8c5ca693344e8b24de9ac955c38de757af8c5760658fc29ed2fbd804803fad' ;; 		x86_64) natsArch='amd64'; sha256='fc15530faec66b61de5140c2b99927c5839caff1c4c17f8bffbf4432fab83017' ;; 		x86) natsArch='386'; sha256='655f0f7cebf727317974006ad4a13ddacd3520f15266e854c2b01681e499bf80' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Tue, 03 Nov 2020 00:33:03 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Tue, 03 Nov 2020 00:33:04 GMT
EXPOSE 4222 8222
# Tue, 03 Nov 2020 00:33:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 03 Nov 2020 00:33:04 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:188c0c94c7c576fff0792aca7ec73d67a2f7f4cb3a6e53a84559337260b36964`  
		Last Modified: Thu, 22 Oct 2020 02:19:57 GMT  
		Size: 2.8 MB (2796860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f211ef5561f154a9a5957cdf08a625861df698594add9ba490a54259e9a01cb1`  
		Last Modified: Tue, 03 Nov 2020 00:33:28 GMT  
		Size: 6.8 MB (6770312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5eef7e98823e252892036fb4b7e5ccf695c556028fa2f7dd6dc314f625ba9eb9`  
		Last Modified: Tue, 03 Nov 2020 00:33:27 GMT  
		Size: 423.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:2a58d6644e94cc17212ec6a604029ebe9f855ceeee7fa66171bdc8aa6c7113ba
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.9 MB (8932203 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b8391afd58a04ec8cf1ab166357c9495c5aa4d32bc4bb4472e577874f42fe55d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Thu, 22 Oct 2020 02:01:09 GMT
ADD file:dec4d3b6cf21c59820d1d74a554d0a193b5f4859e00b932f31ffe73f554d5afb in / 
# Thu, 22 Oct 2020 02:01:12 GMT
CMD ["/bin/sh"]
# Mon, 02 Nov 2020 23:56:13 GMT
ENV NATS_STREAMING_SERVER=0.19.0
# Mon, 02 Nov 2020 23:56:17 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='d582023b8f9fe33b98f0faa6396aae8d5366ecade7e56cde912e21e5b93ea670' ;; 		armhf) natsArch='arm6'; sha256='f4af03e6cbb19f3ad9ea57217607dcf4b68018e1879859c847e2680917fc7139' ;; 		armv7) natsArch='arm7'; sha256='ec8c5ca693344e8b24de9ac955c38de757af8c5760658fc29ed2fbd804803fad' ;; 		x86_64) natsArch='amd64'; sha256='fc15530faec66b61de5140c2b99927c5839caff1c4c17f8bffbf4432fab83017' ;; 		x86) natsArch='386'; sha256='655f0f7cebf727317974006ad4a13ddacd3520f15266e854c2b01681e499bf80' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Mon, 02 Nov 2020 23:56:17 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Mon, 02 Nov 2020 23:56:18 GMT
EXPOSE 4222 8222
# Mon, 02 Nov 2020 23:56:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 02 Nov 2020 23:56:19 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:bad30e7b45c14f784ef29a828b5fc69db0ebdefebcde6a7c98f4f77ffc93a546`  
		Last Modified: Thu, 22 Oct 2020 02:01:42 GMT  
		Size: 2.6 MB (2601912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21cba1ed5b5094a02c017d654b758674905ec0bb2535d3311fcdd61dce32b319`  
		Last Modified: Mon, 02 Nov 2020 23:56:50 GMT  
		Size: 6.3 MB (6329871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3992f15ff4c1a7660c4a81854ec33d3e4973405c7095ceb0bd8a7865fff21c9f`  
		Last Modified: Mon, 02 Nov 2020 23:56:47 GMT  
		Size: 420.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:6a6c52fc272b91cff878ca25bddc432f19583a2e41e5e92288f0e64d0c649896
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.7 MB (8730479 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b4347330ee2d9b26f7fafaadc370627e71670505b340c9e4b54d791afcb3a6b2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Thu, 22 Oct 2020 01:58:13 GMT
ADD file:46f89172426e9f5b1d669a2ca7ab218fc2deaef1caeeab88f2b5bd443ac9773d in / 
# Thu, 22 Oct 2020 01:58:14 GMT
CMD ["/bin/sh"]
# Tue, 03 Nov 2020 00:05:05 GMT
ENV NATS_STREAMING_SERVER=0.19.0
# Tue, 03 Nov 2020 00:05:09 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='d582023b8f9fe33b98f0faa6396aae8d5366ecade7e56cde912e21e5b93ea670' ;; 		armhf) natsArch='arm6'; sha256='f4af03e6cbb19f3ad9ea57217607dcf4b68018e1879859c847e2680917fc7139' ;; 		armv7) natsArch='arm7'; sha256='ec8c5ca693344e8b24de9ac955c38de757af8c5760658fc29ed2fbd804803fad' ;; 		x86_64) natsArch='amd64'; sha256='fc15530faec66b61de5140c2b99927c5839caff1c4c17f8bffbf4432fab83017' ;; 		x86) natsArch='386'; sha256='655f0f7cebf727317974006ad4a13ddacd3520f15266e854c2b01681e499bf80' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Tue, 03 Nov 2020 00:05:09 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Tue, 03 Nov 2020 00:05:10 GMT
EXPOSE 4222 8222
# Tue, 03 Nov 2020 00:05:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 03 Nov 2020 00:05:11 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:5f2023fd85a4e68f37fe41421fd89f30e69b98a645613521c57c01317561eee3`  
		Last Modified: Thu, 22 Oct 2020 01:58:45 GMT  
		Size: 2.4 MB (2405675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34033d6dabe9c0f77f765bf2fce39f1eef24c163cfa802ec78f0e2e1bea9da7c`  
		Last Modified: Tue, 03 Nov 2020 00:05:43 GMT  
		Size: 6.3 MB (6324384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b0a98c9d7b5d859df80140920031b236b38ff88a4ff09d3bf8cfc5b9776e436`  
		Last Modified: Tue, 03 Nov 2020 00:05:40 GMT  
		Size: 420.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:36be57b574502addd00c81caaffedb9030eec583dbf4e3011a95aa7f998834aa
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.0 MB (8969159 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b947ac7936fa0250ecf3f1aaa6e22a928bdb3cdd8f0dcbbc3b8912a0678290c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Thu, 22 Oct 2020 02:01:01 GMT
ADD file:55c4e9752146061a2b5f76027221329f423687987c0744ef577130c60ff0ba42 in / 
# Thu, 22 Oct 2020 02:01:06 GMT
CMD ["/bin/sh"]
# Tue, 03 Nov 2020 00:43:12 GMT
ENV NATS_STREAMING_SERVER=0.19.0
# Tue, 03 Nov 2020 00:43:20 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='d582023b8f9fe33b98f0faa6396aae8d5366ecade7e56cde912e21e5b93ea670' ;; 		armhf) natsArch='arm6'; sha256='f4af03e6cbb19f3ad9ea57217607dcf4b68018e1879859c847e2680917fc7139' ;; 		armv7) natsArch='arm7'; sha256='ec8c5ca693344e8b24de9ac955c38de757af8c5760658fc29ed2fbd804803fad' ;; 		x86_64) natsArch='amd64'; sha256='fc15530faec66b61de5140c2b99927c5839caff1c4c17f8bffbf4432fab83017' ;; 		x86) natsArch='386'; sha256='655f0f7cebf727317974006ad4a13ddacd3520f15266e854c2b01681e499bf80' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Tue, 03 Nov 2020 00:43:21 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Tue, 03 Nov 2020 00:43:23 GMT
EXPOSE 4222 8222
# Tue, 03 Nov 2020 00:43:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 03 Nov 2020 00:43:27 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:5f621e34cdf485f410766dc9a0fc7855d17916d0f6583b58cbdce7c28831f527`  
		Last Modified: Thu, 22 Oct 2020 02:01:38 GMT  
		Size: 2.7 MB (2706555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfea83a41655c390ae2bea2fd6f2a83188ecb9c82e60ebde8040109e79a2eba5`  
		Last Modified: Tue, 03 Nov 2020 00:44:06 GMT  
		Size: 6.3 MB (6262183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0eca3d16e3b7142a6392c550b0efad91076053f222028892a3ae01e63f58dec`  
		Last Modified: Tue, 03 Nov 2020 00:44:05 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:alpine3.12`

```console
$ docker pull nats-streaming@sha256:5f15b51b2b447004408633f8f9458106fadad8f21393b1ed531071731e1ddb00
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:alpine3.12` - linux; amd64

```console
$ docker pull nats-streaming@sha256:a8fcf986c14ae3ad60206bd6ebde23999c28f9967f05b9c81a760054539a683d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.6 MB (9567595 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b20b4ccbdde21c3fb61f4bd7fa3e83384f7e9d7f32f5bb86c88cd162a41403c0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Thu, 22 Oct 2020 02:19:24 GMT
ADD file:f17f65714f703db9012f00e5ec98d0b2541ff6147c2633f7ab9ba659d0c507f4 in / 
# Thu, 22 Oct 2020 02:19:24 GMT
CMD ["/bin/sh"]
# Tue, 03 Nov 2020 00:33:01 GMT
ENV NATS_STREAMING_SERVER=0.19.0
# Tue, 03 Nov 2020 00:33:03 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='d582023b8f9fe33b98f0faa6396aae8d5366ecade7e56cde912e21e5b93ea670' ;; 		armhf) natsArch='arm6'; sha256='f4af03e6cbb19f3ad9ea57217607dcf4b68018e1879859c847e2680917fc7139' ;; 		armv7) natsArch='arm7'; sha256='ec8c5ca693344e8b24de9ac955c38de757af8c5760658fc29ed2fbd804803fad' ;; 		x86_64) natsArch='amd64'; sha256='fc15530faec66b61de5140c2b99927c5839caff1c4c17f8bffbf4432fab83017' ;; 		x86) natsArch='386'; sha256='655f0f7cebf727317974006ad4a13ddacd3520f15266e854c2b01681e499bf80' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Tue, 03 Nov 2020 00:33:03 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Tue, 03 Nov 2020 00:33:04 GMT
EXPOSE 4222 8222
# Tue, 03 Nov 2020 00:33:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 03 Nov 2020 00:33:04 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:188c0c94c7c576fff0792aca7ec73d67a2f7f4cb3a6e53a84559337260b36964`  
		Last Modified: Thu, 22 Oct 2020 02:19:57 GMT  
		Size: 2.8 MB (2796860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f211ef5561f154a9a5957cdf08a625861df698594add9ba490a54259e9a01cb1`  
		Last Modified: Tue, 03 Nov 2020 00:33:28 GMT  
		Size: 6.8 MB (6770312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5eef7e98823e252892036fb4b7e5ccf695c556028fa2f7dd6dc314f625ba9eb9`  
		Last Modified: Tue, 03 Nov 2020 00:33:27 GMT  
		Size: 423.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine3.12` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:2a58d6644e94cc17212ec6a604029ebe9f855ceeee7fa66171bdc8aa6c7113ba
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.9 MB (8932203 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b8391afd58a04ec8cf1ab166357c9495c5aa4d32bc4bb4472e577874f42fe55d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Thu, 22 Oct 2020 02:01:09 GMT
ADD file:dec4d3b6cf21c59820d1d74a554d0a193b5f4859e00b932f31ffe73f554d5afb in / 
# Thu, 22 Oct 2020 02:01:12 GMT
CMD ["/bin/sh"]
# Mon, 02 Nov 2020 23:56:13 GMT
ENV NATS_STREAMING_SERVER=0.19.0
# Mon, 02 Nov 2020 23:56:17 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='d582023b8f9fe33b98f0faa6396aae8d5366ecade7e56cde912e21e5b93ea670' ;; 		armhf) natsArch='arm6'; sha256='f4af03e6cbb19f3ad9ea57217607dcf4b68018e1879859c847e2680917fc7139' ;; 		armv7) natsArch='arm7'; sha256='ec8c5ca693344e8b24de9ac955c38de757af8c5760658fc29ed2fbd804803fad' ;; 		x86_64) natsArch='amd64'; sha256='fc15530faec66b61de5140c2b99927c5839caff1c4c17f8bffbf4432fab83017' ;; 		x86) natsArch='386'; sha256='655f0f7cebf727317974006ad4a13ddacd3520f15266e854c2b01681e499bf80' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Mon, 02 Nov 2020 23:56:17 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Mon, 02 Nov 2020 23:56:18 GMT
EXPOSE 4222 8222
# Mon, 02 Nov 2020 23:56:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 02 Nov 2020 23:56:19 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:bad30e7b45c14f784ef29a828b5fc69db0ebdefebcde6a7c98f4f77ffc93a546`  
		Last Modified: Thu, 22 Oct 2020 02:01:42 GMT  
		Size: 2.6 MB (2601912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21cba1ed5b5094a02c017d654b758674905ec0bb2535d3311fcdd61dce32b319`  
		Last Modified: Mon, 02 Nov 2020 23:56:50 GMT  
		Size: 6.3 MB (6329871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3992f15ff4c1a7660c4a81854ec33d3e4973405c7095ceb0bd8a7865fff21c9f`  
		Last Modified: Mon, 02 Nov 2020 23:56:47 GMT  
		Size: 420.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine3.12` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:6a6c52fc272b91cff878ca25bddc432f19583a2e41e5e92288f0e64d0c649896
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.7 MB (8730479 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b4347330ee2d9b26f7fafaadc370627e71670505b340c9e4b54d791afcb3a6b2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Thu, 22 Oct 2020 01:58:13 GMT
ADD file:46f89172426e9f5b1d669a2ca7ab218fc2deaef1caeeab88f2b5bd443ac9773d in / 
# Thu, 22 Oct 2020 01:58:14 GMT
CMD ["/bin/sh"]
# Tue, 03 Nov 2020 00:05:05 GMT
ENV NATS_STREAMING_SERVER=0.19.0
# Tue, 03 Nov 2020 00:05:09 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='d582023b8f9fe33b98f0faa6396aae8d5366ecade7e56cde912e21e5b93ea670' ;; 		armhf) natsArch='arm6'; sha256='f4af03e6cbb19f3ad9ea57217607dcf4b68018e1879859c847e2680917fc7139' ;; 		armv7) natsArch='arm7'; sha256='ec8c5ca693344e8b24de9ac955c38de757af8c5760658fc29ed2fbd804803fad' ;; 		x86_64) natsArch='amd64'; sha256='fc15530faec66b61de5140c2b99927c5839caff1c4c17f8bffbf4432fab83017' ;; 		x86) natsArch='386'; sha256='655f0f7cebf727317974006ad4a13ddacd3520f15266e854c2b01681e499bf80' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Tue, 03 Nov 2020 00:05:09 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Tue, 03 Nov 2020 00:05:10 GMT
EXPOSE 4222 8222
# Tue, 03 Nov 2020 00:05:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 03 Nov 2020 00:05:11 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:5f2023fd85a4e68f37fe41421fd89f30e69b98a645613521c57c01317561eee3`  
		Last Modified: Thu, 22 Oct 2020 01:58:45 GMT  
		Size: 2.4 MB (2405675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34033d6dabe9c0f77f765bf2fce39f1eef24c163cfa802ec78f0e2e1bea9da7c`  
		Last Modified: Tue, 03 Nov 2020 00:05:43 GMT  
		Size: 6.3 MB (6324384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b0a98c9d7b5d859df80140920031b236b38ff88a4ff09d3bf8cfc5b9776e436`  
		Last Modified: Tue, 03 Nov 2020 00:05:40 GMT  
		Size: 420.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine3.12` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:36be57b574502addd00c81caaffedb9030eec583dbf4e3011a95aa7f998834aa
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.0 MB (8969159 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b947ac7936fa0250ecf3f1aaa6e22a928bdb3cdd8f0dcbbc3b8912a0678290c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Thu, 22 Oct 2020 02:01:01 GMT
ADD file:55c4e9752146061a2b5f76027221329f423687987c0744ef577130c60ff0ba42 in / 
# Thu, 22 Oct 2020 02:01:06 GMT
CMD ["/bin/sh"]
# Tue, 03 Nov 2020 00:43:12 GMT
ENV NATS_STREAMING_SERVER=0.19.0
# Tue, 03 Nov 2020 00:43:20 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='d582023b8f9fe33b98f0faa6396aae8d5366ecade7e56cde912e21e5b93ea670' ;; 		armhf) natsArch='arm6'; sha256='f4af03e6cbb19f3ad9ea57217607dcf4b68018e1879859c847e2680917fc7139' ;; 		armv7) natsArch='arm7'; sha256='ec8c5ca693344e8b24de9ac955c38de757af8c5760658fc29ed2fbd804803fad' ;; 		x86_64) natsArch='amd64'; sha256='fc15530faec66b61de5140c2b99927c5839caff1c4c17f8bffbf4432fab83017' ;; 		x86) natsArch='386'; sha256='655f0f7cebf727317974006ad4a13ddacd3520f15266e854c2b01681e499bf80' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Tue, 03 Nov 2020 00:43:21 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Tue, 03 Nov 2020 00:43:23 GMT
EXPOSE 4222 8222
# Tue, 03 Nov 2020 00:43:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 03 Nov 2020 00:43:27 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:5f621e34cdf485f410766dc9a0fc7855d17916d0f6583b58cbdce7c28831f527`  
		Last Modified: Thu, 22 Oct 2020 02:01:38 GMT  
		Size: 2.7 MB (2706555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfea83a41655c390ae2bea2fd6f2a83188ecb9c82e60ebde8040109e79a2eba5`  
		Last Modified: Tue, 03 Nov 2020 00:44:06 GMT  
		Size: 6.3 MB (6262183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0eca3d16e3b7142a6392c550b0efad91076053f222028892a3ae01e63f58dec`  
		Last Modified: Tue, 03 Nov 2020 00:44:05 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:latest`

```console
$ docker pull nats-streaming@sha256:c8bb32720403c22b091541677c2cdd4e827e65bcf1f25ecf5aaa3acfda90f7d5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.1637; amd64

### `nats-streaming:latest` - linux; amd64

```console
$ docker pull nats-streaming@sha256:053a4ca3955b9c5036e48bafb96c83003fe86c34c6928934e3fd1db0529a889c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 MB (6487259 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:993a204b53252cabfc16952c1d2dc014dc6518d1a08d00bda1bc5008a139e37a`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 03 Nov 2020 00:33:13 GMT
COPY file:3ed83d1497b0535960e452435cb8b27e347f48da12693aa27ebaf9bff94d82de in /nats-streaming-server 
# Tue, 03 Nov 2020 00:33:13 GMT
EXPOSE 4222 8222
# Tue, 03 Nov 2020 00:33:14 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 03 Nov 2020 00:33:14 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:57ac21f890a508f609eabea265197b18ce9dfe3e694034c7a06d37b536a707b2`  
		Last Modified: Tue, 03 Nov 2020 00:33:37 GMT  
		Size: 6.5 MB (6487259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:latest` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:f334d10ef2a4663d8d7d920d96321cd97f050b82a5d55d588192f074f60dd814
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 MB (6049845 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9eecfd5ab4178a65e952a7cf1d248a556a6ae2c328ac8b68923146d64734db03`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 02 Nov 2020 23:56:28 GMT
COPY file:d6896b1c93dcd497494c972f9274fcc634a4f4a8d63a0191bdb87f6336aec0d7 in /nats-streaming-server 
# Mon, 02 Nov 2020 23:56:28 GMT
EXPOSE 4222 8222
# Mon, 02 Nov 2020 23:56:29 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 02 Nov 2020 23:56:29 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:7f165fb71ab77e8081dbfa13656cdf9e5e005002d6c3afa0aac40667a0f97af8`  
		Last Modified: Mon, 02 Nov 2020 23:57:04 GMT  
		Size: 6.0 MB (6049845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:latest` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:5fd0943909d8aedafb888e099c9f64d234023ad780805ed7c939692ebfd8304d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 MB (6043163 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f37071e856ae40dc3c8c5e10b359d1640fd67a6110741c0957af2031032ed6ce`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 03 Nov 2020 00:05:23 GMT
COPY file:d232132ddff1d85d3a2f5c80a91c80023cbc103d816387e06d604cf97238e52c in /nats-streaming-server 
# Tue, 03 Nov 2020 00:05:24 GMT
EXPOSE 4222 8222
# Tue, 03 Nov 2020 00:05:24 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 03 Nov 2020 00:05:25 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:9c7227cc1040d04ca7763cfb53ab58bc32ae54921990516adf8e13374ac9ef29`  
		Last Modified: Tue, 03 Nov 2020 00:05:57 GMT  
		Size: 6.0 MB (6043163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:latest` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:c058fd3e9a8ac44263bf53fa2f6f1e8e8cb3e95cd223f8353fdafc50fe57e417
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 MB (5978846 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7c915a80bd440362bd4a6743fee8134a3caf6271e3258e449fb106b19c050a3b`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 03 Nov 2020 00:43:38 GMT
COPY file:55e70ee826cd5a662497337a2488e22833672bd031d85b4ee39556ab1e80df08 in /nats-streaming-server 
# Tue, 03 Nov 2020 00:43:40 GMT
EXPOSE 4222 8222
# Tue, 03 Nov 2020 00:43:42 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 03 Nov 2020 00:43:43 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:3dc58a59de8a6ed19e9144b0189eb3b637a9e7fcd76ec6c6dc47561b2740a3a2`  
		Last Modified: Tue, 03 Nov 2020 00:44:19 GMT  
		Size: 6.0 MB (5978846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:latest` - windows version 10.0.17763.1637; amd64

```console
$ docker pull nats-streaming@sha256:9444afab14740d43bfd213340272edcfaa96f83b2ae24d586333398cc089a858
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.8 MB (107783475 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:85bdcab4235f3b70b1671972c4154790bde79e33644ae254ae48efa965b2b3cb`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 03 Dec 2020 08:05:47 GMT
RUN Apply image 1809-amd64
# Wed, 09 Dec 2020 17:38:01 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 09 Dec 2020 23:04:19 GMT
RUN cmd /S /C #(nop) COPY file:cc6bae0f50b6e35b12e8233f240d95e093f7e44257bc87e06aed691866ec1477 in C:\nats-streaming-server.exe 
# Wed, 09 Dec 2020 23:04:21 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 09 Dec 2020 23:04:21 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 09 Dec 2020 23:04:22 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:21be49aa856f07be4e0a677b988e43c04bd595a3c858e58b6c364477bbbf7222`  
		Size: 101.3 MB (101264827 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8a3891744a5ba41f01e625a0a70d755ffe93de4d4f124ad6d069420d5c7956d4`  
		Last Modified: Wed, 09 Dec 2020 17:42:32 GMT  
		Size: 893.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab2cf2a7f92a640dc1125e539b41a28abc6b4e2df892f67cbc0072f90bb65509`  
		Last Modified: Wed, 09 Dec 2020 23:08:42 GMT  
		Size: 6.5 MB (6515155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf561da2a706a067845b617e3efccdaf8257da5fb1ae53c383e29559f5220612`  
		Last Modified: Wed, 09 Dec 2020 23:08:41 GMT  
		Size: 869.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1e5e4a71ea08fded20e3471625c1c06c12540fd3c7f4e12eeaee288bf6e5377`  
		Last Modified: Wed, 09 Dec 2020 23:08:39 GMT  
		Size: 864.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5d7a7dbf47aa9dfd9ed44ec162d12b58d6751c6d5f129c4e65250e21fde3631`  
		Last Modified: Wed, 09 Dec 2020 23:08:41 GMT  
		Size: 867.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:linux`

```console
$ docker pull nats-streaming@sha256:8001e4db36785bd692d9ae1c9ed3857d972692b385e36c08994794a5254bb78a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:linux` - linux; amd64

```console
$ docker pull nats-streaming@sha256:053a4ca3955b9c5036e48bafb96c83003fe86c34c6928934e3fd1db0529a889c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 MB (6487259 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:993a204b53252cabfc16952c1d2dc014dc6518d1a08d00bda1bc5008a139e37a`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 03 Nov 2020 00:33:13 GMT
COPY file:3ed83d1497b0535960e452435cb8b27e347f48da12693aa27ebaf9bff94d82de in /nats-streaming-server 
# Tue, 03 Nov 2020 00:33:13 GMT
EXPOSE 4222 8222
# Tue, 03 Nov 2020 00:33:14 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 03 Nov 2020 00:33:14 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:57ac21f890a508f609eabea265197b18ce9dfe3e694034c7a06d37b536a707b2`  
		Last Modified: Tue, 03 Nov 2020 00:33:37 GMT  
		Size: 6.5 MB (6487259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:linux` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:f334d10ef2a4663d8d7d920d96321cd97f050b82a5d55d588192f074f60dd814
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 MB (6049845 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9eecfd5ab4178a65e952a7cf1d248a556a6ae2c328ac8b68923146d64734db03`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 02 Nov 2020 23:56:28 GMT
COPY file:d6896b1c93dcd497494c972f9274fcc634a4f4a8d63a0191bdb87f6336aec0d7 in /nats-streaming-server 
# Mon, 02 Nov 2020 23:56:28 GMT
EXPOSE 4222 8222
# Mon, 02 Nov 2020 23:56:29 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 02 Nov 2020 23:56:29 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:7f165fb71ab77e8081dbfa13656cdf9e5e005002d6c3afa0aac40667a0f97af8`  
		Last Modified: Mon, 02 Nov 2020 23:57:04 GMT  
		Size: 6.0 MB (6049845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:linux` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:5fd0943909d8aedafb888e099c9f64d234023ad780805ed7c939692ebfd8304d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 MB (6043163 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f37071e856ae40dc3c8c5e10b359d1640fd67a6110741c0957af2031032ed6ce`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 03 Nov 2020 00:05:23 GMT
COPY file:d232132ddff1d85d3a2f5c80a91c80023cbc103d816387e06d604cf97238e52c in /nats-streaming-server 
# Tue, 03 Nov 2020 00:05:24 GMT
EXPOSE 4222 8222
# Tue, 03 Nov 2020 00:05:24 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 03 Nov 2020 00:05:25 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:9c7227cc1040d04ca7763cfb53ab58bc32ae54921990516adf8e13374ac9ef29`  
		Last Modified: Tue, 03 Nov 2020 00:05:57 GMT  
		Size: 6.0 MB (6043163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:linux` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:c058fd3e9a8ac44263bf53fa2f6f1e8e8cb3e95cd223f8353fdafc50fe57e417
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 MB (5978846 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7c915a80bd440362bd4a6743fee8134a3caf6271e3258e449fb106b19c050a3b`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 03 Nov 2020 00:43:38 GMT
COPY file:55e70ee826cd5a662497337a2488e22833672bd031d85b4ee39556ab1e80df08 in /nats-streaming-server 
# Tue, 03 Nov 2020 00:43:40 GMT
EXPOSE 4222 8222
# Tue, 03 Nov 2020 00:43:42 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 03 Nov 2020 00:43:43 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:3dc58a59de8a6ed19e9144b0189eb3b637a9e7fcd76ec6c6dc47561b2740a3a2`  
		Last Modified: Tue, 03 Nov 2020 00:44:19 GMT  
		Size: 6.0 MB (5978846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:nanoserver`

```console
$ docker pull nats-streaming@sha256:4a013f6e621b040ed030861cb0bd02d96ef23c7a5fbf2019841921e255379ebf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1637; amd64

### `nats-streaming:nanoserver` - windows version 10.0.17763.1637; amd64

```console
$ docker pull nats-streaming@sha256:9444afab14740d43bfd213340272edcfaa96f83b2ae24d586333398cc089a858
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.8 MB (107783475 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:85bdcab4235f3b70b1671972c4154790bde79e33644ae254ae48efa965b2b3cb`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 03 Dec 2020 08:05:47 GMT
RUN Apply image 1809-amd64
# Wed, 09 Dec 2020 17:38:01 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 09 Dec 2020 23:04:19 GMT
RUN cmd /S /C #(nop) COPY file:cc6bae0f50b6e35b12e8233f240d95e093f7e44257bc87e06aed691866ec1477 in C:\nats-streaming-server.exe 
# Wed, 09 Dec 2020 23:04:21 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 09 Dec 2020 23:04:21 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 09 Dec 2020 23:04:22 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:21be49aa856f07be4e0a677b988e43c04bd595a3c858e58b6c364477bbbf7222`  
		Size: 101.3 MB (101264827 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8a3891744a5ba41f01e625a0a70d755ffe93de4d4f124ad6d069420d5c7956d4`  
		Last Modified: Wed, 09 Dec 2020 17:42:32 GMT  
		Size: 893.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab2cf2a7f92a640dc1125e539b41a28abc6b4e2df892f67cbc0072f90bb65509`  
		Last Modified: Wed, 09 Dec 2020 23:08:42 GMT  
		Size: 6.5 MB (6515155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf561da2a706a067845b617e3efccdaf8257da5fb1ae53c383e29559f5220612`  
		Last Modified: Wed, 09 Dec 2020 23:08:41 GMT  
		Size: 869.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1e5e4a71ea08fded20e3471625c1c06c12540fd3c7f4e12eeaee288bf6e5377`  
		Last Modified: Wed, 09 Dec 2020 23:08:39 GMT  
		Size: 864.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5d7a7dbf47aa9dfd9ed44ec162d12b58d6751c6d5f129c4e65250e21fde3631`  
		Last Modified: Wed, 09 Dec 2020 23:08:41 GMT  
		Size: 867.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:nanoserver-1809`

```console
$ docker pull nats-streaming@sha256:4a013f6e621b040ed030861cb0bd02d96ef23c7a5fbf2019841921e255379ebf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1637; amd64

### `nats-streaming:nanoserver-1809` - windows version 10.0.17763.1637; amd64

```console
$ docker pull nats-streaming@sha256:9444afab14740d43bfd213340272edcfaa96f83b2ae24d586333398cc089a858
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.8 MB (107783475 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:85bdcab4235f3b70b1671972c4154790bde79e33644ae254ae48efa965b2b3cb`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 03 Dec 2020 08:05:47 GMT
RUN Apply image 1809-amd64
# Wed, 09 Dec 2020 17:38:01 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 09 Dec 2020 23:04:19 GMT
RUN cmd /S /C #(nop) COPY file:cc6bae0f50b6e35b12e8233f240d95e093f7e44257bc87e06aed691866ec1477 in C:\nats-streaming-server.exe 
# Wed, 09 Dec 2020 23:04:21 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 09 Dec 2020 23:04:21 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 09 Dec 2020 23:04:22 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:21be49aa856f07be4e0a677b988e43c04bd595a3c858e58b6c364477bbbf7222`  
		Size: 101.3 MB (101264827 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8a3891744a5ba41f01e625a0a70d755ffe93de4d4f124ad6d069420d5c7956d4`  
		Last Modified: Wed, 09 Dec 2020 17:42:32 GMT  
		Size: 893.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab2cf2a7f92a640dc1125e539b41a28abc6b4e2df892f67cbc0072f90bb65509`  
		Last Modified: Wed, 09 Dec 2020 23:08:42 GMT  
		Size: 6.5 MB (6515155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf561da2a706a067845b617e3efccdaf8257da5fb1ae53c383e29559f5220612`  
		Last Modified: Wed, 09 Dec 2020 23:08:41 GMT  
		Size: 869.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1e5e4a71ea08fded20e3471625c1c06c12540fd3c7f4e12eeaee288bf6e5377`  
		Last Modified: Wed, 09 Dec 2020 23:08:39 GMT  
		Size: 864.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5d7a7dbf47aa9dfd9ed44ec162d12b58d6751c6d5f129c4e65250e21fde3631`  
		Last Modified: Wed, 09 Dec 2020 23:08:41 GMT  
		Size: 867.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:scratch`

```console
$ docker pull nats-streaming@sha256:8001e4db36785bd692d9ae1c9ed3857d972692b385e36c08994794a5254bb78a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:scratch` - linux; amd64

```console
$ docker pull nats-streaming@sha256:053a4ca3955b9c5036e48bafb96c83003fe86c34c6928934e3fd1db0529a889c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 MB (6487259 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:993a204b53252cabfc16952c1d2dc014dc6518d1a08d00bda1bc5008a139e37a`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 03 Nov 2020 00:33:13 GMT
COPY file:3ed83d1497b0535960e452435cb8b27e347f48da12693aa27ebaf9bff94d82de in /nats-streaming-server 
# Tue, 03 Nov 2020 00:33:13 GMT
EXPOSE 4222 8222
# Tue, 03 Nov 2020 00:33:14 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 03 Nov 2020 00:33:14 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:57ac21f890a508f609eabea265197b18ce9dfe3e694034c7a06d37b536a707b2`  
		Last Modified: Tue, 03 Nov 2020 00:33:37 GMT  
		Size: 6.5 MB (6487259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:scratch` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:f334d10ef2a4663d8d7d920d96321cd97f050b82a5d55d588192f074f60dd814
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 MB (6049845 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9eecfd5ab4178a65e952a7cf1d248a556a6ae2c328ac8b68923146d64734db03`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 02 Nov 2020 23:56:28 GMT
COPY file:d6896b1c93dcd497494c972f9274fcc634a4f4a8d63a0191bdb87f6336aec0d7 in /nats-streaming-server 
# Mon, 02 Nov 2020 23:56:28 GMT
EXPOSE 4222 8222
# Mon, 02 Nov 2020 23:56:29 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 02 Nov 2020 23:56:29 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:7f165fb71ab77e8081dbfa13656cdf9e5e005002d6c3afa0aac40667a0f97af8`  
		Last Modified: Mon, 02 Nov 2020 23:57:04 GMT  
		Size: 6.0 MB (6049845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:scratch` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:5fd0943909d8aedafb888e099c9f64d234023ad780805ed7c939692ebfd8304d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 MB (6043163 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f37071e856ae40dc3c8c5e10b359d1640fd67a6110741c0957af2031032ed6ce`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 03 Nov 2020 00:05:23 GMT
COPY file:d232132ddff1d85d3a2f5c80a91c80023cbc103d816387e06d604cf97238e52c in /nats-streaming-server 
# Tue, 03 Nov 2020 00:05:24 GMT
EXPOSE 4222 8222
# Tue, 03 Nov 2020 00:05:24 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 03 Nov 2020 00:05:25 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:9c7227cc1040d04ca7763cfb53ab58bc32ae54921990516adf8e13374ac9ef29`  
		Last Modified: Tue, 03 Nov 2020 00:05:57 GMT  
		Size: 6.0 MB (6043163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:scratch` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:c058fd3e9a8ac44263bf53fa2f6f1e8e8cb3e95cd223f8353fdafc50fe57e417
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 MB (5978846 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7c915a80bd440362bd4a6743fee8134a3caf6271e3258e449fb106b19c050a3b`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 03 Nov 2020 00:43:38 GMT
COPY file:55e70ee826cd5a662497337a2488e22833672bd031d85b4ee39556ab1e80df08 in /nats-streaming-server 
# Tue, 03 Nov 2020 00:43:40 GMT
EXPOSE 4222 8222
# Tue, 03 Nov 2020 00:43:42 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 03 Nov 2020 00:43:43 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:3dc58a59de8a6ed19e9144b0189eb3b637a9e7fcd76ec6c6dc47561b2740a3a2`  
		Last Modified: Tue, 03 Nov 2020 00:44:19 GMT  
		Size: 6.0 MB (5978846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:windowsservercore`

```console
$ docker pull nats-streaming@sha256:78cddd38d3c26f2a74454532132969b5fbc9fbff9cc8708cf338c1b33a80c17b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1637; amd64
	-	windows version 10.0.14393.4104; amd64

### `nats-streaming:windowsservercore` - windows version 10.0.17763.1637; amd64

```console
$ docker pull nats-streaming@sha256:7a8ab0956821d178ef84f6f10c399d44005ca86dd75378d41a5980979ed24409
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2411449594 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0146757e90d9c2df66c7933b807c71d62de612813d33a32f15c8d7fdd710ddae`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 04 Dec 2020 02:13:01 GMT
RUN Install update 1809-amd64
# Wed, 09 Dec 2020 14:02:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Dec 2020 17:36:04 GMT
ENV NATS_DOCKERIZED=1
# Wed, 09 Dec 2020 23:02:20 GMT
ENV NATS_STREAMING_SERVER=0.19.0
# Wed, 09 Dec 2020 23:02:21 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.19.0/nats-streaming-server-v0.19.0-windows-amd64.zip
# Wed, 09 Dec 2020 23:02:22 GMT
ENV GIT_DOWNLOAD_SHA256=edafd6482bd71f3d6035d7f6871df1fd4c53acf0ac19e88b85e08a2c7ab1cec5
# Wed, 09 Dec 2020 23:02:52 GMT
RUN Set-PSDebug -Trace 2
# Wed, 09 Dec 2020 23:04:09 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 09 Dec 2020 23:04:10 GMT
EXPOSE 4222 8222
# Wed, 09 Dec 2020 23:04:12 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 09 Dec 2020 23:04:13 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:aa4f58cd6da1aaf1a0b44d443bd88e7fbe5b0a6f193995a1a61d6bd63990f314`  
		Size: 672.5 MB (672541583 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:240407eb82b6591b0574396ec829a4a5cd9a75257a4663f9876942995275965d`  
		Last Modified: Wed, 09 Dec 2020 17:10:14 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82b9257be76bd37cad15d45905ec5910266409794a9dbd8a0428174f8b2f352a`  
		Last Modified: Wed, 09 Dec 2020 17:42:00 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36644685392e418bf32ab96db81c8f6a861b913256c244637d9d3ee45098a9cb`  
		Last Modified: Wed, 09 Dec 2020 23:08:22 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9469bed00eb5f6a5b7c050a1aaee856134ec78bab6076cc793e26dc52ec71fa`  
		Last Modified: Wed, 09 Dec 2020 23:08:21 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94e9d451908e3e8ec10448e052cf25767a282312e49e29d2a0b42652cf217e28`  
		Last Modified: Wed, 09 Dec 2020 23:08:21 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:870e3bb830bd8ad9b84a928d2b858be730dcdba8016206ee4aeda623d98754b3`  
		Last Modified: Wed, 09 Dec 2020 23:08:20 GMT  
		Size: 4.8 MB (4843348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14d24c0a2fc2b3ecd1b0467794ae95667a29e1bd550bf2bf9c455499839253bc`  
		Last Modified: Wed, 09 Dec 2020 23:08:23 GMT  
		Size: 15.7 MB (15722612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09371bf015245c95ce8d5db6b8d7f90fc6d8527f83101535c8c6af719b628e79`  
		Last Modified: Wed, 09 Dec 2020 23:08:18 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76ff8db511e98efbde9cbbf6ecd2d9bd2b73565c7c4e0d24dddeb6edfa2a1875`  
		Last Modified: Wed, 09 Dec 2020 23:08:18 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13217bf3886546791bd6c26ab23636f9bc595fd80abf1e7d6ab6f10f8613cdee`  
		Last Modified: Wed, 09 Dec 2020 23:08:18 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:windowsservercore` - windows version 10.0.14393.4104; amd64

```console
$ docker pull nats-streaming@sha256:33a909f6239f294532f68e91f94655aa881f2c8701293c9963e4b1c85b1a1a52
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5790922042 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:74e094a16d960a68e3691347bc7923c1f94b7db31dedb2ef74b9d87436170384`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 02 Dec 2020 17:42:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 09 Dec 2020 14:41:21 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Dec 2020 17:38:10 GMT
ENV NATS_DOCKERIZED=1
# Wed, 09 Dec 2020 23:04:27 GMT
ENV NATS_STREAMING_SERVER=0.19.0
# Wed, 09 Dec 2020 23:04:28 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.19.0/nats-streaming-server-v0.19.0-windows-amd64.zip
# Wed, 09 Dec 2020 23:04:28 GMT
ENV GIT_DOWNLOAD_SHA256=edafd6482bd71f3d6035d7f6871df1fd4c53acf0ac19e88b85e08a2c7ab1cec5
# Wed, 09 Dec 2020 23:05:39 GMT
RUN Set-PSDebug -Trace 2
# Wed, 09 Dec 2020 23:07:44 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 09 Dec 2020 23:07:45 GMT
EXPOSE 4222 8222
# Wed, 09 Dec 2020 23:07:46 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 09 Dec 2020 23:07:47 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d2696dc2a40dc121fc5acaa02242817ac416c69d17c113e2ac5136d21a3942d8`  
		Size: 1.7 GB (1698858125 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b5a79f8be42bf1c358ccc82f32c1481de95c393ef97e712a321c1440d132fda9`  
		Last Modified: Wed, 09 Dec 2020 17:11:03 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56d972336c8bcee0026c76e8f199cef405112a70aeef9917f07d2859f15162c1`  
		Last Modified: Wed, 09 Dec 2020 17:42:56 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e4f52064be159ebf6d7d967a842e39ae04b53dcf15dd8b582a77af431f81df7`  
		Last Modified: Wed, 09 Dec 2020 23:09:02 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54d1ecc24d286c8499d1698affa71481762f11bb3d4fdd9d35763dcbe94e9e9a`  
		Last Modified: Wed, 09 Dec 2020 23:09:00 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:649366889ec5703d27a79142f0331f2a462858d6d6ee2a7c1bd8e426bece4236`  
		Last Modified: Wed, 09 Dec 2020 23:08:59 GMT  
		Size: 1.1 KB (1139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9916349c9d6afe29e7418ee0e8f0454bb37038070600eaef872fb7356c1147d0`  
		Last Modified: Wed, 09 Dec 2020 23:08:59 GMT  
		Size: 5.5 MB (5528923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:838e032e6db488d413de3f4681555d2b57bb4472c3b16ed16a5c07f2e921f1ed`  
		Last Modified: Wed, 09 Dec 2020 23:09:01 GMT  
		Size: 16.5 MB (16540005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96a5c8ab334a9fbf340bbb2d213d16e91599eee98aafa72f7f8fbb6d4d147b27`  
		Last Modified: Wed, 09 Dec 2020 23:08:56 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09db5c24070ad330bcb0f078a2325aba107a3a8615fc004248d02e8e828fa8ce`  
		Last Modified: Wed, 09 Dec 2020 23:08:58 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21108015f9c4f2ee78087806b4ca0582f2618489ed4899b07b6290d743b8ef3d`  
		Last Modified: Wed, 09 Dec 2020 23:08:57 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:windowsservercore-1809`

```console
$ docker pull nats-streaming@sha256:3a285fa7c8c148aad627e61b6848554ccc223cb30a1eb3293a5a5fb89af016c6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1637; amd64

### `nats-streaming:windowsservercore-1809` - windows version 10.0.17763.1637; amd64

```console
$ docker pull nats-streaming@sha256:7a8ab0956821d178ef84f6f10c399d44005ca86dd75378d41a5980979ed24409
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2411449594 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0146757e90d9c2df66c7933b807c71d62de612813d33a32f15c8d7fdd710ddae`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 04 Dec 2020 02:13:01 GMT
RUN Install update 1809-amd64
# Wed, 09 Dec 2020 14:02:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Dec 2020 17:36:04 GMT
ENV NATS_DOCKERIZED=1
# Wed, 09 Dec 2020 23:02:20 GMT
ENV NATS_STREAMING_SERVER=0.19.0
# Wed, 09 Dec 2020 23:02:21 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.19.0/nats-streaming-server-v0.19.0-windows-amd64.zip
# Wed, 09 Dec 2020 23:02:22 GMT
ENV GIT_DOWNLOAD_SHA256=edafd6482bd71f3d6035d7f6871df1fd4c53acf0ac19e88b85e08a2c7ab1cec5
# Wed, 09 Dec 2020 23:02:52 GMT
RUN Set-PSDebug -Trace 2
# Wed, 09 Dec 2020 23:04:09 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 09 Dec 2020 23:04:10 GMT
EXPOSE 4222 8222
# Wed, 09 Dec 2020 23:04:12 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 09 Dec 2020 23:04:13 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:aa4f58cd6da1aaf1a0b44d443bd88e7fbe5b0a6f193995a1a61d6bd63990f314`  
		Size: 672.5 MB (672541583 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:240407eb82b6591b0574396ec829a4a5cd9a75257a4663f9876942995275965d`  
		Last Modified: Wed, 09 Dec 2020 17:10:14 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82b9257be76bd37cad15d45905ec5910266409794a9dbd8a0428174f8b2f352a`  
		Last Modified: Wed, 09 Dec 2020 17:42:00 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36644685392e418bf32ab96db81c8f6a861b913256c244637d9d3ee45098a9cb`  
		Last Modified: Wed, 09 Dec 2020 23:08:22 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9469bed00eb5f6a5b7c050a1aaee856134ec78bab6076cc793e26dc52ec71fa`  
		Last Modified: Wed, 09 Dec 2020 23:08:21 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94e9d451908e3e8ec10448e052cf25767a282312e49e29d2a0b42652cf217e28`  
		Last Modified: Wed, 09 Dec 2020 23:08:21 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:870e3bb830bd8ad9b84a928d2b858be730dcdba8016206ee4aeda623d98754b3`  
		Last Modified: Wed, 09 Dec 2020 23:08:20 GMT  
		Size: 4.8 MB (4843348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14d24c0a2fc2b3ecd1b0467794ae95667a29e1bd550bf2bf9c455499839253bc`  
		Last Modified: Wed, 09 Dec 2020 23:08:23 GMT  
		Size: 15.7 MB (15722612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09371bf015245c95ce8d5db6b8d7f90fc6d8527f83101535c8c6af719b628e79`  
		Last Modified: Wed, 09 Dec 2020 23:08:18 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76ff8db511e98efbde9cbbf6ecd2d9bd2b73565c7c4e0d24dddeb6edfa2a1875`  
		Last Modified: Wed, 09 Dec 2020 23:08:18 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13217bf3886546791bd6c26ab23636f9bc595fd80abf1e7d6ab6f10f8613cdee`  
		Last Modified: Wed, 09 Dec 2020 23:08:18 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:windowsservercore-ltsc2016`

```console
$ docker pull nats-streaming@sha256:da877310cb87d1822f44a79a76b57af2eceb3e15aa82ab406a47d32bc0de9f47
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4104; amd64

### `nats-streaming:windowsservercore-ltsc2016` - windows version 10.0.14393.4104; amd64

```console
$ docker pull nats-streaming@sha256:33a909f6239f294532f68e91f94655aa881f2c8701293c9963e4b1c85b1a1a52
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5790922042 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:74e094a16d960a68e3691347bc7923c1f94b7db31dedb2ef74b9d87436170384`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 02 Dec 2020 17:42:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 09 Dec 2020 14:41:21 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Dec 2020 17:38:10 GMT
ENV NATS_DOCKERIZED=1
# Wed, 09 Dec 2020 23:04:27 GMT
ENV NATS_STREAMING_SERVER=0.19.0
# Wed, 09 Dec 2020 23:04:28 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.19.0/nats-streaming-server-v0.19.0-windows-amd64.zip
# Wed, 09 Dec 2020 23:04:28 GMT
ENV GIT_DOWNLOAD_SHA256=edafd6482bd71f3d6035d7f6871df1fd4c53acf0ac19e88b85e08a2c7ab1cec5
# Wed, 09 Dec 2020 23:05:39 GMT
RUN Set-PSDebug -Trace 2
# Wed, 09 Dec 2020 23:07:44 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 09 Dec 2020 23:07:45 GMT
EXPOSE 4222 8222
# Wed, 09 Dec 2020 23:07:46 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 09 Dec 2020 23:07:47 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d2696dc2a40dc121fc5acaa02242817ac416c69d17c113e2ac5136d21a3942d8`  
		Size: 1.7 GB (1698858125 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b5a79f8be42bf1c358ccc82f32c1481de95c393ef97e712a321c1440d132fda9`  
		Last Modified: Wed, 09 Dec 2020 17:11:03 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56d972336c8bcee0026c76e8f199cef405112a70aeef9917f07d2859f15162c1`  
		Last Modified: Wed, 09 Dec 2020 17:42:56 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e4f52064be159ebf6d7d967a842e39ae04b53dcf15dd8b582a77af431f81df7`  
		Last Modified: Wed, 09 Dec 2020 23:09:02 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54d1ecc24d286c8499d1698affa71481762f11bb3d4fdd9d35763dcbe94e9e9a`  
		Last Modified: Wed, 09 Dec 2020 23:09:00 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:649366889ec5703d27a79142f0331f2a462858d6d6ee2a7c1bd8e426bece4236`  
		Last Modified: Wed, 09 Dec 2020 23:08:59 GMT  
		Size: 1.1 KB (1139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9916349c9d6afe29e7418ee0e8f0454bb37038070600eaef872fb7356c1147d0`  
		Last Modified: Wed, 09 Dec 2020 23:08:59 GMT  
		Size: 5.5 MB (5528923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:838e032e6db488d413de3f4681555d2b57bb4472c3b16ed16a5c07f2e921f1ed`  
		Last Modified: Wed, 09 Dec 2020 23:09:01 GMT  
		Size: 16.5 MB (16540005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96a5c8ab334a9fbf340bbb2d213d16e91599eee98aafa72f7f8fbb6d4d147b27`  
		Last Modified: Wed, 09 Dec 2020 23:08:56 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09db5c24070ad330bcb0f078a2325aba107a3a8615fc004248d02e8e828fa8ce`  
		Last Modified: Wed, 09 Dec 2020 23:08:58 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21108015f9c4f2ee78087806b4ca0582f2618489ed4899b07b6290d743b8ef3d`  
		Last Modified: Wed, 09 Dec 2020 23:08:57 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
