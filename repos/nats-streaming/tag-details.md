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
$ docker pull nats-streaming@sha256:75a03d7b41efbfe88ad632319a99ec0a93c546d202c7caa3481d07cd8ea559c2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.1697; amd64

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

### `nats-streaming:0.20` - windows version 10.0.17763.1697; amd64

```console
$ docker pull nats-streaming@sha256:131f9c39ac29e11d0dc81c1c26cc0fbbb50b832eaba8715c6504d1dac8418435
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.4 MB (107365498 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef855a422d4be3f13d838208fd85955fd7768b3567bd89861a6d67df15122d4a`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 07 Jan 2021 16:14:35 GMT
RUN Apply image 1809-amd64
# Wed, 13 Jan 2021 19:06:01 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Thu, 14 Jan 2021 00:16:51 GMT
RUN cmd /S /C #(nop) COPY file:f2450ffeda74e33f820191eccf78b6647ce56865170e966bfa8e72afe6e46c36 in C:\nats-streaming-server.exe 
# Thu, 14 Jan 2021 00:16:52 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Thu, 14 Jan 2021 00:16:53 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Thu, 14 Jan 2021 00:16:54 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:62239e9aa1a352a20b0d4969c2b508b8a18d10e799d4db72e6f24ccbb2c724d9`  
		Size: 101.3 MB (101340070 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:0a89b73109217060f51d51b7d3a7eda3a9ac0de9c5f76db54addb98b7f1c24c1`  
		Last Modified: Wed, 13 Jan 2021 19:10:49 GMT  
		Size: 885.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65b689a2a270a9c8e1ec741a7297ca14c2001e9a7ab5c9ea3d06f4cf834b8261`  
		Last Modified: Thu, 14 Jan 2021 00:21:28 GMT  
		Size: 6.0 MB (6021918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9339c8634418d855b08dc20f472d3906160f6010ee4b4f1c803e0e9cc4f6d6e3`  
		Last Modified: Thu, 14 Jan 2021 00:21:23 GMT  
		Size: 877.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1de47275056946f9394ba060e89e9ab1710aa73977d6485df317ed346a3c6ed1`  
		Last Modified: Thu, 14 Jan 2021 00:21:25 GMT  
		Size: 865.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4b4ebb72cdd066de0407bdd35275fc5528023c450322d57a92f6527fc42b931`  
		Last Modified: Thu, 14 Jan 2021 00:21:24 GMT  
		Size: 883.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.20.0`

```console
$ docker pull nats-streaming@sha256:75a03d7b41efbfe88ad632319a99ec0a93c546d202c7caa3481d07cd8ea559c2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.1697; amd64

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

### `nats-streaming:0.20.0` - windows version 10.0.17763.1697; amd64

```console
$ docker pull nats-streaming@sha256:131f9c39ac29e11d0dc81c1c26cc0fbbb50b832eaba8715c6504d1dac8418435
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.4 MB (107365498 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef855a422d4be3f13d838208fd85955fd7768b3567bd89861a6d67df15122d4a`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 07 Jan 2021 16:14:35 GMT
RUN Apply image 1809-amd64
# Wed, 13 Jan 2021 19:06:01 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Thu, 14 Jan 2021 00:16:51 GMT
RUN cmd /S /C #(nop) COPY file:f2450ffeda74e33f820191eccf78b6647ce56865170e966bfa8e72afe6e46c36 in C:\nats-streaming-server.exe 
# Thu, 14 Jan 2021 00:16:52 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Thu, 14 Jan 2021 00:16:53 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Thu, 14 Jan 2021 00:16:54 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:62239e9aa1a352a20b0d4969c2b508b8a18d10e799d4db72e6f24ccbb2c724d9`  
		Size: 101.3 MB (101340070 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:0a89b73109217060f51d51b7d3a7eda3a9ac0de9c5f76db54addb98b7f1c24c1`  
		Last Modified: Wed, 13 Jan 2021 19:10:49 GMT  
		Size: 885.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65b689a2a270a9c8e1ec741a7297ca14c2001e9a7ab5c9ea3d06f4cf834b8261`  
		Last Modified: Thu, 14 Jan 2021 00:21:28 GMT  
		Size: 6.0 MB (6021918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9339c8634418d855b08dc20f472d3906160f6010ee4b4f1c803e0e9cc4f6d6e3`  
		Last Modified: Thu, 14 Jan 2021 00:21:23 GMT  
		Size: 877.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1de47275056946f9394ba060e89e9ab1710aa73977d6485df317ed346a3c6ed1`  
		Last Modified: Thu, 14 Jan 2021 00:21:25 GMT  
		Size: 865.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4b4ebb72cdd066de0407bdd35275fc5528023c450322d57a92f6527fc42b931`  
		Last Modified: Thu, 14 Jan 2021 00:21:24 GMT  
		Size: 883.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.20.0-alpine`

```console
$ docker pull nats-streaming@sha256:54ee921908bc93e1deb621ad5b769a4b1e66fd99781595cacb1e1f526cae5670
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.20.0-alpine` - linux; amd64

```console
$ docker pull nats-streaming@sha256:ee383fab395fb79ad35d3663e31ba2c1556e67dd1ae42c9a314b14f66d80afa6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.0 MB (8997281 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c2217d4d7856bf852cbd735ef2587447e243436346788e6acaf5f102bcfbf28`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:41 GMT
ADD file:ec475c2abb2d46435286b5ae5efacf5b50b1a9e3b6293b69db3c0172b5b9658b in / 
# Thu, 17 Dec 2020 00:19:42 GMT
CMD ["/bin/sh"]
# Tue, 12 Jan 2021 00:48:03 GMT
ENV NATS_STREAMING_SERVER=0.20.0
# Tue, 12 Jan 2021 00:48:05 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='618008a4902916b6bdb26022343ab91313d4f7fc90b31d0c71ad9e75dc8299e4' ;; 		armhf) natsArch='arm6'; sha256='144b04f8f42793aee1b2deb3f6eb187648c37dcc32d526c607a0af99a847260d' ;; 		armv7) natsArch='arm7'; sha256='720f4a90d1dd536bc04639ae31c70ab46fb3e10556f0f261eb038fdce941f20c' ;; 		x86_64) natsArch='amd64'; sha256='098e2293cce5d457b92f3df35127789422562f1414427c406ffd03ea3bd687c9' ;; 		x86) natsArch='386'; sha256='322a290f4706f14d6ff8160ec437202bd282f61f0607741d0e4c38ef89b83451' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Tue, 12 Jan 2021 00:48:05 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Tue, 12 Jan 2021 00:48:06 GMT
EXPOSE 4222 8222
# Tue, 12 Jan 2021 00:48:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 12 Jan 2021 00:48:06 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:801bfaa63ef2094d770c809815b9e2b9c1194728e5e754ef7bc764030e140cea`  
		Last Modified: Wed, 16 Dec 2020 19:34:50 GMT  
		Size: 2.8 MB (2799066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f9b99285c9495350a993a87920ea4ccf0c2c560a7047d0076af2648f08b7bea`  
		Last Modified: Tue, 12 Jan 2021 00:48:48 GMT  
		Size: 6.2 MB (6197794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:244241c08cee6b44b104d2b942ec81d0a48351c78496d12ee991024881132576`  
		Last Modified: Tue, 12 Jan 2021 00:48:46 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.20.0-alpine` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:18fd3ddc15d5b65b6ad1171abf76e359cca31b60730750546e0dc0368a805750
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.3 MB (8330755 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0322ce6374b271fc98c0e0a12b42c00a722465006d75394c2ab41bbb47d50c46`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 16 Dec 2020 23:49:43 GMT
ADD file:0a16715e2d0e5811c3c578945d618db0e269847a799340248f9ba8d393c9eec2 in / 
# Wed, 16 Dec 2020 23:49:45 GMT
CMD ["/bin/sh"]
# Mon, 11 Jan 2021 23:53:38 GMT
ENV NATS_STREAMING_SERVER=0.20.0
# Mon, 11 Jan 2021 23:53:42 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='618008a4902916b6bdb26022343ab91313d4f7fc90b31d0c71ad9e75dc8299e4' ;; 		armhf) natsArch='arm6'; sha256='144b04f8f42793aee1b2deb3f6eb187648c37dcc32d526c607a0af99a847260d' ;; 		armv7) natsArch='arm7'; sha256='720f4a90d1dd536bc04639ae31c70ab46fb3e10556f0f261eb038fdce941f20c' ;; 		x86_64) natsArch='amd64'; sha256='098e2293cce5d457b92f3df35127789422562f1414427c406ffd03ea3bd687c9' ;; 		x86) natsArch='386'; sha256='322a290f4706f14d6ff8160ec437202bd282f61f0607741d0e4c38ef89b83451' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Mon, 11 Jan 2021 23:53:43 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Mon, 11 Jan 2021 23:53:44 GMT
EXPOSE 4222 8222
# Mon, 11 Jan 2021 23:53:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 11 Jan 2021 23:53:45 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:93247449aef3c56eb4f7ab7b3fed95743c974b823def6dd86ec84008126e7903`  
		Last Modified: Wed, 16 Dec 2020 23:50:24 GMT  
		Size: 2.6 MB (2604163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d54831e858eddfe2c245e8c154d4422ad61bc9a30c1cfe612ec35f7a12b1e529`  
		Last Modified: Mon, 11 Jan 2021 23:54:22 GMT  
		Size: 5.7 MB (5726171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:412a9e8bb4d16b7ddec81004c2205411fc7b8830d0d2a0f3054a2fe0dc4664cd`  
		Last Modified: Mon, 11 Jan 2021 23:54:20 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.20.0-alpine` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:b41e2afb428f6345393616c70c1a9d2221db86ab84c6e37be6c252bebf974203
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.1 MB (8125466 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8cfc9155e69d8a79c164c6c96d01ea612fb88e955066a7f2803d0054801875da`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 16 Dec 2020 23:58:14 GMT
ADD file:bd07f77a2b2741ca6bda80d9203be9c7274cf73145bff778cf000db0d8d4e903 in / 
# Wed, 16 Dec 2020 23:58:15 GMT
CMD ["/bin/sh"]
# Tue, 12 Jan 2021 00:18:41 GMT
ENV NATS_STREAMING_SERVER=0.20.0
# Tue, 12 Jan 2021 00:18:51 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='618008a4902916b6bdb26022343ab91313d4f7fc90b31d0c71ad9e75dc8299e4' ;; 		armhf) natsArch='arm6'; sha256='144b04f8f42793aee1b2deb3f6eb187648c37dcc32d526c607a0af99a847260d' ;; 		armv7) natsArch='arm7'; sha256='720f4a90d1dd536bc04639ae31c70ab46fb3e10556f0f261eb038fdce941f20c' ;; 		x86_64) natsArch='amd64'; sha256='098e2293cce5d457b92f3df35127789422562f1414427c406ffd03ea3bd687c9' ;; 		x86) natsArch='386'; sha256='322a290f4706f14d6ff8160ec437202bd282f61f0607741d0e4c38ef89b83451' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Tue, 12 Jan 2021 00:18:54 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Tue, 12 Jan 2021 00:18:57 GMT
EXPOSE 4222 8222
# Tue, 12 Jan 2021 00:18:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 12 Jan 2021 00:18:59 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:c58e8a26a8407acc3ead776f6526efa889fda03270a8d05109208d9f59159420`  
		Last Modified: Wed, 16 Dec 2020 23:58:59 GMT  
		Size: 2.4 MB (2407555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9290155f6f3b723d2522ebaa0d1e2038dcd4f4c978c086bc43fd55a4d8284659`  
		Last Modified: Tue, 12 Jan 2021 00:19:43 GMT  
		Size: 5.7 MB (5717488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4715986f280e125e74cc7b430caa19329b3de9fcfcd40ae588f422be68c37ca`  
		Last Modified: Tue, 12 Jan 2021 00:19:42 GMT  
		Size: 423.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.20.0-alpine` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:ae8f52346c3d26a49ae885bf56785f3952c14c8622a97e18288ae0abedd51660
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.4 MB (8377876 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5f79e7574653a33192a8af07510cf1a7f03f5c02a77b49072304e701cf514cf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 16 Dec 2020 23:40:26 GMT
ADD file:a4845c3840a3fd0e41e4635a179cce20c81afc6c02e34e3fd5bd2d535698918b in / 
# Wed, 16 Dec 2020 23:40:29 GMT
CMD ["/bin/sh"]
# Mon, 11 Jan 2021 23:47:10 GMT
ENV NATS_STREAMING_SERVER=0.20.0
# Mon, 11 Jan 2021 23:47:14 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='618008a4902916b6bdb26022343ab91313d4f7fc90b31d0c71ad9e75dc8299e4' ;; 		armhf) natsArch='arm6'; sha256='144b04f8f42793aee1b2deb3f6eb187648c37dcc32d526c607a0af99a847260d' ;; 		armv7) natsArch='arm7'; sha256='720f4a90d1dd536bc04639ae31c70ab46fb3e10556f0f261eb038fdce941f20c' ;; 		x86_64) natsArch='amd64'; sha256='098e2293cce5d457b92f3df35127789422562f1414427c406ffd03ea3bd687c9' ;; 		x86) natsArch='386'; sha256='322a290f4706f14d6ff8160ec437202bd282f61f0607741d0e4c38ef89b83451' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Mon, 11 Jan 2021 23:47:15 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Mon, 11 Jan 2021 23:47:15 GMT
EXPOSE 4222 8222
# Mon, 11 Jan 2021 23:47:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 11 Jan 2021 23:47:17 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:159e5727ea618dfe8b08811112e2c51f5bd2b9ae7db9eb214914a65249f70ca0`  
		Last Modified: Wed, 16 Dec 2020 23:41:08 GMT  
		Size: 2.7 MB (2709048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e424273d6cedd00225b67fa1b47e0dd8bf4b2abfa19fbc27f7763f096aeb138`  
		Last Modified: Mon, 11 Jan 2021 23:47:54 GMT  
		Size: 5.7 MB (5668408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33979e718e15555239006f224ba6d995cf9d6d044a7f25493196839d4d5aed73`  
		Last Modified: Mon, 11 Jan 2021 23:47:53 GMT  
		Size: 420.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.20.0-alpine3.12`

```console
$ docker pull nats-streaming@sha256:54ee921908bc93e1deb621ad5b769a4b1e66fd99781595cacb1e1f526cae5670
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.20.0-alpine3.12` - linux; amd64

```console
$ docker pull nats-streaming@sha256:ee383fab395fb79ad35d3663e31ba2c1556e67dd1ae42c9a314b14f66d80afa6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.0 MB (8997281 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c2217d4d7856bf852cbd735ef2587447e243436346788e6acaf5f102bcfbf28`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:41 GMT
ADD file:ec475c2abb2d46435286b5ae5efacf5b50b1a9e3b6293b69db3c0172b5b9658b in / 
# Thu, 17 Dec 2020 00:19:42 GMT
CMD ["/bin/sh"]
# Tue, 12 Jan 2021 00:48:03 GMT
ENV NATS_STREAMING_SERVER=0.20.0
# Tue, 12 Jan 2021 00:48:05 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='618008a4902916b6bdb26022343ab91313d4f7fc90b31d0c71ad9e75dc8299e4' ;; 		armhf) natsArch='arm6'; sha256='144b04f8f42793aee1b2deb3f6eb187648c37dcc32d526c607a0af99a847260d' ;; 		armv7) natsArch='arm7'; sha256='720f4a90d1dd536bc04639ae31c70ab46fb3e10556f0f261eb038fdce941f20c' ;; 		x86_64) natsArch='amd64'; sha256='098e2293cce5d457b92f3df35127789422562f1414427c406ffd03ea3bd687c9' ;; 		x86) natsArch='386'; sha256='322a290f4706f14d6ff8160ec437202bd282f61f0607741d0e4c38ef89b83451' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Tue, 12 Jan 2021 00:48:05 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Tue, 12 Jan 2021 00:48:06 GMT
EXPOSE 4222 8222
# Tue, 12 Jan 2021 00:48:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 12 Jan 2021 00:48:06 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:801bfaa63ef2094d770c809815b9e2b9c1194728e5e754ef7bc764030e140cea`  
		Last Modified: Wed, 16 Dec 2020 19:34:50 GMT  
		Size: 2.8 MB (2799066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f9b99285c9495350a993a87920ea4ccf0c2c560a7047d0076af2648f08b7bea`  
		Last Modified: Tue, 12 Jan 2021 00:48:48 GMT  
		Size: 6.2 MB (6197794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:244241c08cee6b44b104d2b942ec81d0a48351c78496d12ee991024881132576`  
		Last Modified: Tue, 12 Jan 2021 00:48:46 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.20.0-alpine3.12` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:18fd3ddc15d5b65b6ad1171abf76e359cca31b60730750546e0dc0368a805750
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.3 MB (8330755 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0322ce6374b271fc98c0e0a12b42c00a722465006d75394c2ab41bbb47d50c46`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 16 Dec 2020 23:49:43 GMT
ADD file:0a16715e2d0e5811c3c578945d618db0e269847a799340248f9ba8d393c9eec2 in / 
# Wed, 16 Dec 2020 23:49:45 GMT
CMD ["/bin/sh"]
# Mon, 11 Jan 2021 23:53:38 GMT
ENV NATS_STREAMING_SERVER=0.20.0
# Mon, 11 Jan 2021 23:53:42 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='618008a4902916b6bdb26022343ab91313d4f7fc90b31d0c71ad9e75dc8299e4' ;; 		armhf) natsArch='arm6'; sha256='144b04f8f42793aee1b2deb3f6eb187648c37dcc32d526c607a0af99a847260d' ;; 		armv7) natsArch='arm7'; sha256='720f4a90d1dd536bc04639ae31c70ab46fb3e10556f0f261eb038fdce941f20c' ;; 		x86_64) natsArch='amd64'; sha256='098e2293cce5d457b92f3df35127789422562f1414427c406ffd03ea3bd687c9' ;; 		x86) natsArch='386'; sha256='322a290f4706f14d6ff8160ec437202bd282f61f0607741d0e4c38ef89b83451' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Mon, 11 Jan 2021 23:53:43 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Mon, 11 Jan 2021 23:53:44 GMT
EXPOSE 4222 8222
# Mon, 11 Jan 2021 23:53:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 11 Jan 2021 23:53:45 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:93247449aef3c56eb4f7ab7b3fed95743c974b823def6dd86ec84008126e7903`  
		Last Modified: Wed, 16 Dec 2020 23:50:24 GMT  
		Size: 2.6 MB (2604163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d54831e858eddfe2c245e8c154d4422ad61bc9a30c1cfe612ec35f7a12b1e529`  
		Last Modified: Mon, 11 Jan 2021 23:54:22 GMT  
		Size: 5.7 MB (5726171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:412a9e8bb4d16b7ddec81004c2205411fc7b8830d0d2a0f3054a2fe0dc4664cd`  
		Last Modified: Mon, 11 Jan 2021 23:54:20 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.20.0-alpine3.12` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:b41e2afb428f6345393616c70c1a9d2221db86ab84c6e37be6c252bebf974203
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.1 MB (8125466 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8cfc9155e69d8a79c164c6c96d01ea612fb88e955066a7f2803d0054801875da`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 16 Dec 2020 23:58:14 GMT
ADD file:bd07f77a2b2741ca6bda80d9203be9c7274cf73145bff778cf000db0d8d4e903 in / 
# Wed, 16 Dec 2020 23:58:15 GMT
CMD ["/bin/sh"]
# Tue, 12 Jan 2021 00:18:41 GMT
ENV NATS_STREAMING_SERVER=0.20.0
# Tue, 12 Jan 2021 00:18:51 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='618008a4902916b6bdb26022343ab91313d4f7fc90b31d0c71ad9e75dc8299e4' ;; 		armhf) natsArch='arm6'; sha256='144b04f8f42793aee1b2deb3f6eb187648c37dcc32d526c607a0af99a847260d' ;; 		armv7) natsArch='arm7'; sha256='720f4a90d1dd536bc04639ae31c70ab46fb3e10556f0f261eb038fdce941f20c' ;; 		x86_64) natsArch='amd64'; sha256='098e2293cce5d457b92f3df35127789422562f1414427c406ffd03ea3bd687c9' ;; 		x86) natsArch='386'; sha256='322a290f4706f14d6ff8160ec437202bd282f61f0607741d0e4c38ef89b83451' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Tue, 12 Jan 2021 00:18:54 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Tue, 12 Jan 2021 00:18:57 GMT
EXPOSE 4222 8222
# Tue, 12 Jan 2021 00:18:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 12 Jan 2021 00:18:59 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:c58e8a26a8407acc3ead776f6526efa889fda03270a8d05109208d9f59159420`  
		Last Modified: Wed, 16 Dec 2020 23:58:59 GMT  
		Size: 2.4 MB (2407555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9290155f6f3b723d2522ebaa0d1e2038dcd4f4c978c086bc43fd55a4d8284659`  
		Last Modified: Tue, 12 Jan 2021 00:19:43 GMT  
		Size: 5.7 MB (5717488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4715986f280e125e74cc7b430caa19329b3de9fcfcd40ae588f422be68c37ca`  
		Last Modified: Tue, 12 Jan 2021 00:19:42 GMT  
		Size: 423.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.20.0-alpine3.12` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:ae8f52346c3d26a49ae885bf56785f3952c14c8622a97e18288ae0abedd51660
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.4 MB (8377876 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5f79e7574653a33192a8af07510cf1a7f03f5c02a77b49072304e701cf514cf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 16 Dec 2020 23:40:26 GMT
ADD file:a4845c3840a3fd0e41e4635a179cce20c81afc6c02e34e3fd5bd2d535698918b in / 
# Wed, 16 Dec 2020 23:40:29 GMT
CMD ["/bin/sh"]
# Mon, 11 Jan 2021 23:47:10 GMT
ENV NATS_STREAMING_SERVER=0.20.0
# Mon, 11 Jan 2021 23:47:14 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='618008a4902916b6bdb26022343ab91313d4f7fc90b31d0c71ad9e75dc8299e4' ;; 		armhf) natsArch='arm6'; sha256='144b04f8f42793aee1b2deb3f6eb187648c37dcc32d526c607a0af99a847260d' ;; 		armv7) natsArch='arm7'; sha256='720f4a90d1dd536bc04639ae31c70ab46fb3e10556f0f261eb038fdce941f20c' ;; 		x86_64) natsArch='amd64'; sha256='098e2293cce5d457b92f3df35127789422562f1414427c406ffd03ea3bd687c9' ;; 		x86) natsArch='386'; sha256='322a290f4706f14d6ff8160ec437202bd282f61f0607741d0e4c38ef89b83451' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Mon, 11 Jan 2021 23:47:15 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Mon, 11 Jan 2021 23:47:15 GMT
EXPOSE 4222 8222
# Mon, 11 Jan 2021 23:47:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 11 Jan 2021 23:47:17 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:159e5727ea618dfe8b08811112e2c51f5bd2b9ae7db9eb214914a65249f70ca0`  
		Last Modified: Wed, 16 Dec 2020 23:41:08 GMT  
		Size: 2.7 MB (2709048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e424273d6cedd00225b67fa1b47e0dd8bf4b2abfa19fbc27f7763f096aeb138`  
		Last Modified: Mon, 11 Jan 2021 23:47:54 GMT  
		Size: 5.7 MB (5668408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33979e718e15555239006f224ba6d995cf9d6d044a7f25493196839d4d5aed73`  
		Last Modified: Mon, 11 Jan 2021 23:47:53 GMT  
		Size: 420.0 B  
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
$ docker pull nats-streaming@sha256:c7b60cb7eb50b0454d787676660cbb52ebc25457d367cc91f7f6219eb3cdc861
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1697; amd64

### `nats-streaming:0.20.0-nanoserver` - windows version 10.0.17763.1697; amd64

```console
$ docker pull nats-streaming@sha256:131f9c39ac29e11d0dc81c1c26cc0fbbb50b832eaba8715c6504d1dac8418435
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.4 MB (107365498 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef855a422d4be3f13d838208fd85955fd7768b3567bd89861a6d67df15122d4a`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 07 Jan 2021 16:14:35 GMT
RUN Apply image 1809-amd64
# Wed, 13 Jan 2021 19:06:01 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Thu, 14 Jan 2021 00:16:51 GMT
RUN cmd /S /C #(nop) COPY file:f2450ffeda74e33f820191eccf78b6647ce56865170e966bfa8e72afe6e46c36 in C:\nats-streaming-server.exe 
# Thu, 14 Jan 2021 00:16:52 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Thu, 14 Jan 2021 00:16:53 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Thu, 14 Jan 2021 00:16:54 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:62239e9aa1a352a20b0d4969c2b508b8a18d10e799d4db72e6f24ccbb2c724d9`  
		Size: 101.3 MB (101340070 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:0a89b73109217060f51d51b7d3a7eda3a9ac0de9c5f76db54addb98b7f1c24c1`  
		Last Modified: Wed, 13 Jan 2021 19:10:49 GMT  
		Size: 885.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65b689a2a270a9c8e1ec741a7297ca14c2001e9a7ab5c9ea3d06f4cf834b8261`  
		Last Modified: Thu, 14 Jan 2021 00:21:28 GMT  
		Size: 6.0 MB (6021918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9339c8634418d855b08dc20f472d3906160f6010ee4b4f1c803e0e9cc4f6d6e3`  
		Last Modified: Thu, 14 Jan 2021 00:21:23 GMT  
		Size: 877.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1de47275056946f9394ba060e89e9ab1710aa73977d6485df317ed346a3c6ed1`  
		Last Modified: Thu, 14 Jan 2021 00:21:25 GMT  
		Size: 865.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4b4ebb72cdd066de0407bdd35275fc5528023c450322d57a92f6527fc42b931`  
		Last Modified: Thu, 14 Jan 2021 00:21:24 GMT  
		Size: 883.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.20.0-nanoserver-1809`

```console
$ docker pull nats-streaming@sha256:c7b60cb7eb50b0454d787676660cbb52ebc25457d367cc91f7f6219eb3cdc861
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1697; amd64

### `nats-streaming:0.20.0-nanoserver-1809` - windows version 10.0.17763.1697; amd64

```console
$ docker pull nats-streaming@sha256:131f9c39ac29e11d0dc81c1c26cc0fbbb50b832eaba8715c6504d1dac8418435
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.4 MB (107365498 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef855a422d4be3f13d838208fd85955fd7768b3567bd89861a6d67df15122d4a`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 07 Jan 2021 16:14:35 GMT
RUN Apply image 1809-amd64
# Wed, 13 Jan 2021 19:06:01 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Thu, 14 Jan 2021 00:16:51 GMT
RUN cmd /S /C #(nop) COPY file:f2450ffeda74e33f820191eccf78b6647ce56865170e966bfa8e72afe6e46c36 in C:\nats-streaming-server.exe 
# Thu, 14 Jan 2021 00:16:52 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Thu, 14 Jan 2021 00:16:53 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Thu, 14 Jan 2021 00:16:54 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:62239e9aa1a352a20b0d4969c2b508b8a18d10e799d4db72e6f24ccbb2c724d9`  
		Size: 101.3 MB (101340070 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:0a89b73109217060f51d51b7d3a7eda3a9ac0de9c5f76db54addb98b7f1c24c1`  
		Last Modified: Wed, 13 Jan 2021 19:10:49 GMT  
		Size: 885.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65b689a2a270a9c8e1ec741a7297ca14c2001e9a7ab5c9ea3d06f4cf834b8261`  
		Last Modified: Thu, 14 Jan 2021 00:21:28 GMT  
		Size: 6.0 MB (6021918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9339c8634418d855b08dc20f472d3906160f6010ee4b4f1c803e0e9cc4f6d6e3`  
		Last Modified: Thu, 14 Jan 2021 00:21:23 GMT  
		Size: 877.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1de47275056946f9394ba060e89e9ab1710aa73977d6485df317ed346a3c6ed1`  
		Last Modified: Thu, 14 Jan 2021 00:21:25 GMT  
		Size: 865.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4b4ebb72cdd066de0407bdd35275fc5528023c450322d57a92f6527fc42b931`  
		Last Modified: Thu, 14 Jan 2021 00:21:24 GMT  
		Size: 883.0 B  
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
$ docker pull nats-streaming@sha256:11ad0d1e03a1ff4fb65d386c0a006568d4734fef5df4dc9b3c62766ce61ac698
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1697; amd64
	-	windows version 10.0.14393.4169; amd64

### `nats-streaming:0.20.0-windowsservercore` - windows version 10.0.17763.1697; amd64

```console
$ docker pull nats-streaming@sha256:d2daab4b8bc283cf1ddc2ddf53f4f222917ea9e9a1bc67de348a775962c269a0
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2456125476 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c5292ad84e88614d976356e7ff8e6f7e7b2649d2a22528459d8728ba63779a4`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 08 Jan 2021 08:50:52 GMT
RUN Install update 1809-amd64
# Wed, 13 Jan 2021 15:20:56 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 Jan 2021 19:04:04 GMT
ENV NATS_DOCKERIZED=1
# Thu, 14 Jan 2021 00:14:52 GMT
ENV NATS_STREAMING_SERVER=0.20.0
# Thu, 14 Jan 2021 00:14:53 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.20.0/nats-streaming-server-v0.20.0-windows-amd64.zip
# Thu, 14 Jan 2021 00:14:54 GMT
ENV GIT_DOWNLOAD_SHA256=26ae310d3ec11617d380106a769236a6dc2209769c0c36d15cb6736db1b589cb
# Thu, 14 Jan 2021 00:15:24 GMT
RUN Set-PSDebug -Trace 2
# Thu, 14 Jan 2021 00:16:41 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Thu, 14 Jan 2021 00:16:42 GMT
EXPOSE 4222 8222
# Thu, 14 Jan 2021 00:16:43 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Thu, 14 Jan 2021 00:16:44 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4dcc9a9b9e680514ef3fdfcc2ce08a3768f9e412703faa137f4a7c8297600052`  
		Size: 717.4 MB (717439216 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:9f84df50d9e20cf852bfd3555d4e56feabf7b9c735e48c613fc461146876bc03`  
		Last Modified: Wed, 13 Jan 2021 18:31:55 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eff779c93810f460e9728c49a995f9cdd81c09b10ffc6e842f2272d19bf4389c`  
		Last Modified: Wed, 13 Jan 2021 19:10:22 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db50a98331abb7193615377c607d4cc7ea1627e30627f5082cc2a05a1e8cb428`  
		Last Modified: Thu, 14 Jan 2021 00:21:00 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79b5d06af7ef1e49206abf1d378dada3faab78554537f7634ec7b5ecf32c6c6a`  
		Last Modified: Thu, 14 Jan 2021 00:20:59 GMT  
		Size: 1.2 KB (1195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12b88e14e5a7930afc8de8e320c13370e618c24fcad06cd1c1f780c5c8384511`  
		Last Modified: Thu, 14 Jan 2021 00:20:59 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5edc2474a0a8a163a2a2a5cf7f87653f8139b5502f6feb6f6498659f23a0aab3`  
		Last Modified: Thu, 14 Jan 2021 00:21:03 GMT  
		Size: 5.0 MB (4995134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7618255c64c34d36a87a9d6f8651060d3039ff15997db8d45ae63784a1033029`  
		Last Modified: Thu, 14 Jan 2021 00:20:59 GMT  
		Size: 15.3 MB (15349122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c31f9a9cb9ee775a576ab8b2965a6e6519cf8a3204d86fab292f4ef3e4812da`  
		Last Modified: Thu, 14 Jan 2021 00:20:55 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:970ac1da377a92447bf6c7fc7fdb9e99090419dda91b090699f888b52e668f6e`  
		Last Modified: Thu, 14 Jan 2021 00:20:57 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bf641cd6f551e1da67ddae43c327f9d50e79f84861fdbbd5b4fd106bede1abc`  
		Last Modified: Thu, 14 Jan 2021 00:20:55 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.20.0-windowsservercore` - windows version 10.0.14393.4169; amd64

```console
$ docker pull nats-streaming@sha256:c367ca4a4a285c082ea86a36e7756fa5fb8bdcb26e0d672d001a6c8705665ce4
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5815695855 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a029a9ad083d7eb1f30e9786dd41f47c2e77080d9e9021766804fc0be81a012`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Thu, 07 Jan 2021 11:30:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 13 Jan 2021 15:29:26 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 Jan 2021 19:06:11 GMT
ENV NATS_DOCKERIZED=1
# Thu, 14 Jan 2021 00:16:59 GMT
ENV NATS_STREAMING_SERVER=0.20.0
# Thu, 14 Jan 2021 00:16:59 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.20.0/nats-streaming-server-v0.20.0-windows-amd64.zip
# Thu, 14 Jan 2021 00:17:00 GMT
ENV GIT_DOWNLOAD_SHA256=26ae310d3ec11617d380106a769236a6dc2209769c0c36d15cb6736db1b589cb
# Thu, 14 Jan 2021 00:18:09 GMT
RUN Set-PSDebug -Trace 2
# Thu, 14 Jan 2021 00:20:06 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Thu, 14 Jan 2021 00:20:07 GMT
EXPOSE 4222 8222
# Thu, 14 Jan 2021 00:20:08 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Thu, 14 Jan 2021 00:20:09 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bd091f41e44cabc11504b7e130c74a7ef654f58840ba102e3507c4fdf2bae994`  
		Size: 1.7 GB (1723908142 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3b5ee02f83739eef6745d432d63363ce5f490820d4b3e39ae83aa4e3771c4073`  
		Last Modified: Wed, 13 Jan 2021 18:32:39 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acd1c346230e9eaf41e5c8f582c16f531efe65ddbc7fad4e748dd41227e0bbbb`  
		Last Modified: Wed, 13 Jan 2021 19:11:23 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f108152877e2db7ec4dd6c6de8d00482b91437643ebd0dd7cf43e42190c2890`  
		Last Modified: Thu, 14 Jan 2021 00:21:53 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6e3520bde1739f1c73952b8e57fe35000dbac521a22f348e3a0371d914a1937`  
		Last Modified: Thu, 14 Jan 2021 00:21:53 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:585f9330c9a3eebe8d5e6a286b47d58f468a4450072ff1d43f5e7789c82bc66c`  
		Last Modified: Thu, 14 Jan 2021 00:21:51 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39283eaf29b89a60733eeee6ef01dd8db391eef6ce38d43af691e2ad029afc47`  
		Last Modified: Thu, 14 Jan 2021 00:21:48 GMT  
		Size: 5.6 MB (5634422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e3dbd237456a9c1256853ea1c674bc29dac8a8c889e44cccd2dd5407c865abd`  
		Last Modified: Thu, 14 Jan 2021 00:22:07 GMT  
		Size: 16.2 MB (16158244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55dd8e327b6c1be0b8ef8fc2d1abf1d797ecb1f920126d8eb22725259e09587b`  
		Last Modified: Thu, 14 Jan 2021 00:21:48 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d4d27bf34acd3738303a71be66064e609fe0401657f123b818f3acff11d1144`  
		Last Modified: Thu, 14 Jan 2021 00:21:48 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c0acd7c0d45157eb23fcbcbb981ac80d8c0a013e5feb807d40f8b1d85ae1d30`  
		Last Modified: Thu, 14 Jan 2021 00:21:48 GMT  
		Size: 1.1 KB (1139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.20.0-windowsservercore-1809`

```console
$ docker pull nats-streaming@sha256:5a3c9931a73fd83aa5cdaef3d876f63dd8265212a5b22c1502fbc38f6c43c94c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1697; amd64

### `nats-streaming:0.20.0-windowsservercore-1809` - windows version 10.0.17763.1697; amd64

```console
$ docker pull nats-streaming@sha256:d2daab4b8bc283cf1ddc2ddf53f4f222917ea9e9a1bc67de348a775962c269a0
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2456125476 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c5292ad84e88614d976356e7ff8e6f7e7b2649d2a22528459d8728ba63779a4`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 08 Jan 2021 08:50:52 GMT
RUN Install update 1809-amd64
# Wed, 13 Jan 2021 15:20:56 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 Jan 2021 19:04:04 GMT
ENV NATS_DOCKERIZED=1
# Thu, 14 Jan 2021 00:14:52 GMT
ENV NATS_STREAMING_SERVER=0.20.0
# Thu, 14 Jan 2021 00:14:53 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.20.0/nats-streaming-server-v0.20.0-windows-amd64.zip
# Thu, 14 Jan 2021 00:14:54 GMT
ENV GIT_DOWNLOAD_SHA256=26ae310d3ec11617d380106a769236a6dc2209769c0c36d15cb6736db1b589cb
# Thu, 14 Jan 2021 00:15:24 GMT
RUN Set-PSDebug -Trace 2
# Thu, 14 Jan 2021 00:16:41 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Thu, 14 Jan 2021 00:16:42 GMT
EXPOSE 4222 8222
# Thu, 14 Jan 2021 00:16:43 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Thu, 14 Jan 2021 00:16:44 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4dcc9a9b9e680514ef3fdfcc2ce08a3768f9e412703faa137f4a7c8297600052`  
		Size: 717.4 MB (717439216 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:9f84df50d9e20cf852bfd3555d4e56feabf7b9c735e48c613fc461146876bc03`  
		Last Modified: Wed, 13 Jan 2021 18:31:55 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eff779c93810f460e9728c49a995f9cdd81c09b10ffc6e842f2272d19bf4389c`  
		Last Modified: Wed, 13 Jan 2021 19:10:22 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db50a98331abb7193615377c607d4cc7ea1627e30627f5082cc2a05a1e8cb428`  
		Last Modified: Thu, 14 Jan 2021 00:21:00 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79b5d06af7ef1e49206abf1d378dada3faab78554537f7634ec7b5ecf32c6c6a`  
		Last Modified: Thu, 14 Jan 2021 00:20:59 GMT  
		Size: 1.2 KB (1195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12b88e14e5a7930afc8de8e320c13370e618c24fcad06cd1c1f780c5c8384511`  
		Last Modified: Thu, 14 Jan 2021 00:20:59 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5edc2474a0a8a163a2a2a5cf7f87653f8139b5502f6feb6f6498659f23a0aab3`  
		Last Modified: Thu, 14 Jan 2021 00:21:03 GMT  
		Size: 5.0 MB (4995134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7618255c64c34d36a87a9d6f8651060d3039ff15997db8d45ae63784a1033029`  
		Last Modified: Thu, 14 Jan 2021 00:20:59 GMT  
		Size: 15.3 MB (15349122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c31f9a9cb9ee775a576ab8b2965a6e6519cf8a3204d86fab292f4ef3e4812da`  
		Last Modified: Thu, 14 Jan 2021 00:20:55 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:970ac1da377a92447bf6c7fc7fdb9e99090419dda91b090699f888b52e668f6e`  
		Last Modified: Thu, 14 Jan 2021 00:20:57 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bf641cd6f551e1da67ddae43c327f9d50e79f84861fdbbd5b4fd106bede1abc`  
		Last Modified: Thu, 14 Jan 2021 00:20:55 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.20.0-windowsservercore-ltsc2016`

```console
$ docker pull nats-streaming@sha256:69f55054852b78b108077f2c54bbeb3e546b35558384bf8179be11ad1a8766e2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4169; amd64

### `nats-streaming:0.20.0-windowsservercore-ltsc2016` - windows version 10.0.14393.4169; amd64

```console
$ docker pull nats-streaming@sha256:c367ca4a4a285c082ea86a36e7756fa5fb8bdcb26e0d672d001a6c8705665ce4
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5815695855 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a029a9ad083d7eb1f30e9786dd41f47c2e77080d9e9021766804fc0be81a012`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Thu, 07 Jan 2021 11:30:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 13 Jan 2021 15:29:26 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 Jan 2021 19:06:11 GMT
ENV NATS_DOCKERIZED=1
# Thu, 14 Jan 2021 00:16:59 GMT
ENV NATS_STREAMING_SERVER=0.20.0
# Thu, 14 Jan 2021 00:16:59 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.20.0/nats-streaming-server-v0.20.0-windows-amd64.zip
# Thu, 14 Jan 2021 00:17:00 GMT
ENV GIT_DOWNLOAD_SHA256=26ae310d3ec11617d380106a769236a6dc2209769c0c36d15cb6736db1b589cb
# Thu, 14 Jan 2021 00:18:09 GMT
RUN Set-PSDebug -Trace 2
# Thu, 14 Jan 2021 00:20:06 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Thu, 14 Jan 2021 00:20:07 GMT
EXPOSE 4222 8222
# Thu, 14 Jan 2021 00:20:08 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Thu, 14 Jan 2021 00:20:09 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bd091f41e44cabc11504b7e130c74a7ef654f58840ba102e3507c4fdf2bae994`  
		Size: 1.7 GB (1723908142 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3b5ee02f83739eef6745d432d63363ce5f490820d4b3e39ae83aa4e3771c4073`  
		Last Modified: Wed, 13 Jan 2021 18:32:39 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acd1c346230e9eaf41e5c8f582c16f531efe65ddbc7fad4e748dd41227e0bbbb`  
		Last Modified: Wed, 13 Jan 2021 19:11:23 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f108152877e2db7ec4dd6c6de8d00482b91437643ebd0dd7cf43e42190c2890`  
		Last Modified: Thu, 14 Jan 2021 00:21:53 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6e3520bde1739f1c73952b8e57fe35000dbac521a22f348e3a0371d914a1937`  
		Last Modified: Thu, 14 Jan 2021 00:21:53 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:585f9330c9a3eebe8d5e6a286b47d58f468a4450072ff1d43f5e7789c82bc66c`  
		Last Modified: Thu, 14 Jan 2021 00:21:51 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39283eaf29b89a60733eeee6ef01dd8db391eef6ce38d43af691e2ad029afc47`  
		Last Modified: Thu, 14 Jan 2021 00:21:48 GMT  
		Size: 5.6 MB (5634422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e3dbd237456a9c1256853ea1c674bc29dac8a8c889e44cccd2dd5407c865abd`  
		Last Modified: Thu, 14 Jan 2021 00:22:07 GMT  
		Size: 16.2 MB (16158244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55dd8e327b6c1be0b8ef8fc2d1abf1d797ecb1f920126d8eb22725259e09587b`  
		Last Modified: Thu, 14 Jan 2021 00:21:48 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d4d27bf34acd3738303a71be66064e609fe0401657f123b818f3acff11d1144`  
		Last Modified: Thu, 14 Jan 2021 00:21:48 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c0acd7c0d45157eb23fcbcbb981ac80d8c0a013e5feb807d40f8b1d85ae1d30`  
		Last Modified: Thu, 14 Jan 2021 00:21:48 GMT  
		Size: 1.1 KB (1139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.20-alpine`

```console
$ docker pull nats-streaming@sha256:54ee921908bc93e1deb621ad5b769a4b1e66fd99781595cacb1e1f526cae5670
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.20-alpine` - linux; amd64

```console
$ docker pull nats-streaming@sha256:ee383fab395fb79ad35d3663e31ba2c1556e67dd1ae42c9a314b14f66d80afa6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.0 MB (8997281 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c2217d4d7856bf852cbd735ef2587447e243436346788e6acaf5f102bcfbf28`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:41 GMT
ADD file:ec475c2abb2d46435286b5ae5efacf5b50b1a9e3b6293b69db3c0172b5b9658b in / 
# Thu, 17 Dec 2020 00:19:42 GMT
CMD ["/bin/sh"]
# Tue, 12 Jan 2021 00:48:03 GMT
ENV NATS_STREAMING_SERVER=0.20.0
# Tue, 12 Jan 2021 00:48:05 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='618008a4902916b6bdb26022343ab91313d4f7fc90b31d0c71ad9e75dc8299e4' ;; 		armhf) natsArch='arm6'; sha256='144b04f8f42793aee1b2deb3f6eb187648c37dcc32d526c607a0af99a847260d' ;; 		armv7) natsArch='arm7'; sha256='720f4a90d1dd536bc04639ae31c70ab46fb3e10556f0f261eb038fdce941f20c' ;; 		x86_64) natsArch='amd64'; sha256='098e2293cce5d457b92f3df35127789422562f1414427c406ffd03ea3bd687c9' ;; 		x86) natsArch='386'; sha256='322a290f4706f14d6ff8160ec437202bd282f61f0607741d0e4c38ef89b83451' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Tue, 12 Jan 2021 00:48:05 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Tue, 12 Jan 2021 00:48:06 GMT
EXPOSE 4222 8222
# Tue, 12 Jan 2021 00:48:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 12 Jan 2021 00:48:06 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:801bfaa63ef2094d770c809815b9e2b9c1194728e5e754ef7bc764030e140cea`  
		Last Modified: Wed, 16 Dec 2020 19:34:50 GMT  
		Size: 2.8 MB (2799066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f9b99285c9495350a993a87920ea4ccf0c2c560a7047d0076af2648f08b7bea`  
		Last Modified: Tue, 12 Jan 2021 00:48:48 GMT  
		Size: 6.2 MB (6197794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:244241c08cee6b44b104d2b942ec81d0a48351c78496d12ee991024881132576`  
		Last Modified: Tue, 12 Jan 2021 00:48:46 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.20-alpine` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:18fd3ddc15d5b65b6ad1171abf76e359cca31b60730750546e0dc0368a805750
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.3 MB (8330755 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0322ce6374b271fc98c0e0a12b42c00a722465006d75394c2ab41bbb47d50c46`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 16 Dec 2020 23:49:43 GMT
ADD file:0a16715e2d0e5811c3c578945d618db0e269847a799340248f9ba8d393c9eec2 in / 
# Wed, 16 Dec 2020 23:49:45 GMT
CMD ["/bin/sh"]
# Mon, 11 Jan 2021 23:53:38 GMT
ENV NATS_STREAMING_SERVER=0.20.0
# Mon, 11 Jan 2021 23:53:42 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='618008a4902916b6bdb26022343ab91313d4f7fc90b31d0c71ad9e75dc8299e4' ;; 		armhf) natsArch='arm6'; sha256='144b04f8f42793aee1b2deb3f6eb187648c37dcc32d526c607a0af99a847260d' ;; 		armv7) natsArch='arm7'; sha256='720f4a90d1dd536bc04639ae31c70ab46fb3e10556f0f261eb038fdce941f20c' ;; 		x86_64) natsArch='amd64'; sha256='098e2293cce5d457b92f3df35127789422562f1414427c406ffd03ea3bd687c9' ;; 		x86) natsArch='386'; sha256='322a290f4706f14d6ff8160ec437202bd282f61f0607741d0e4c38ef89b83451' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Mon, 11 Jan 2021 23:53:43 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Mon, 11 Jan 2021 23:53:44 GMT
EXPOSE 4222 8222
# Mon, 11 Jan 2021 23:53:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 11 Jan 2021 23:53:45 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:93247449aef3c56eb4f7ab7b3fed95743c974b823def6dd86ec84008126e7903`  
		Last Modified: Wed, 16 Dec 2020 23:50:24 GMT  
		Size: 2.6 MB (2604163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d54831e858eddfe2c245e8c154d4422ad61bc9a30c1cfe612ec35f7a12b1e529`  
		Last Modified: Mon, 11 Jan 2021 23:54:22 GMT  
		Size: 5.7 MB (5726171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:412a9e8bb4d16b7ddec81004c2205411fc7b8830d0d2a0f3054a2fe0dc4664cd`  
		Last Modified: Mon, 11 Jan 2021 23:54:20 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.20-alpine` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:b41e2afb428f6345393616c70c1a9d2221db86ab84c6e37be6c252bebf974203
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.1 MB (8125466 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8cfc9155e69d8a79c164c6c96d01ea612fb88e955066a7f2803d0054801875da`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 16 Dec 2020 23:58:14 GMT
ADD file:bd07f77a2b2741ca6bda80d9203be9c7274cf73145bff778cf000db0d8d4e903 in / 
# Wed, 16 Dec 2020 23:58:15 GMT
CMD ["/bin/sh"]
# Tue, 12 Jan 2021 00:18:41 GMT
ENV NATS_STREAMING_SERVER=0.20.0
# Tue, 12 Jan 2021 00:18:51 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='618008a4902916b6bdb26022343ab91313d4f7fc90b31d0c71ad9e75dc8299e4' ;; 		armhf) natsArch='arm6'; sha256='144b04f8f42793aee1b2deb3f6eb187648c37dcc32d526c607a0af99a847260d' ;; 		armv7) natsArch='arm7'; sha256='720f4a90d1dd536bc04639ae31c70ab46fb3e10556f0f261eb038fdce941f20c' ;; 		x86_64) natsArch='amd64'; sha256='098e2293cce5d457b92f3df35127789422562f1414427c406ffd03ea3bd687c9' ;; 		x86) natsArch='386'; sha256='322a290f4706f14d6ff8160ec437202bd282f61f0607741d0e4c38ef89b83451' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Tue, 12 Jan 2021 00:18:54 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Tue, 12 Jan 2021 00:18:57 GMT
EXPOSE 4222 8222
# Tue, 12 Jan 2021 00:18:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 12 Jan 2021 00:18:59 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:c58e8a26a8407acc3ead776f6526efa889fda03270a8d05109208d9f59159420`  
		Last Modified: Wed, 16 Dec 2020 23:58:59 GMT  
		Size: 2.4 MB (2407555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9290155f6f3b723d2522ebaa0d1e2038dcd4f4c978c086bc43fd55a4d8284659`  
		Last Modified: Tue, 12 Jan 2021 00:19:43 GMT  
		Size: 5.7 MB (5717488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4715986f280e125e74cc7b430caa19329b3de9fcfcd40ae588f422be68c37ca`  
		Last Modified: Tue, 12 Jan 2021 00:19:42 GMT  
		Size: 423.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.20-alpine` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:ae8f52346c3d26a49ae885bf56785f3952c14c8622a97e18288ae0abedd51660
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.4 MB (8377876 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5f79e7574653a33192a8af07510cf1a7f03f5c02a77b49072304e701cf514cf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 16 Dec 2020 23:40:26 GMT
ADD file:a4845c3840a3fd0e41e4635a179cce20c81afc6c02e34e3fd5bd2d535698918b in / 
# Wed, 16 Dec 2020 23:40:29 GMT
CMD ["/bin/sh"]
# Mon, 11 Jan 2021 23:47:10 GMT
ENV NATS_STREAMING_SERVER=0.20.0
# Mon, 11 Jan 2021 23:47:14 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='618008a4902916b6bdb26022343ab91313d4f7fc90b31d0c71ad9e75dc8299e4' ;; 		armhf) natsArch='arm6'; sha256='144b04f8f42793aee1b2deb3f6eb187648c37dcc32d526c607a0af99a847260d' ;; 		armv7) natsArch='arm7'; sha256='720f4a90d1dd536bc04639ae31c70ab46fb3e10556f0f261eb038fdce941f20c' ;; 		x86_64) natsArch='amd64'; sha256='098e2293cce5d457b92f3df35127789422562f1414427c406ffd03ea3bd687c9' ;; 		x86) natsArch='386'; sha256='322a290f4706f14d6ff8160ec437202bd282f61f0607741d0e4c38ef89b83451' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Mon, 11 Jan 2021 23:47:15 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Mon, 11 Jan 2021 23:47:15 GMT
EXPOSE 4222 8222
# Mon, 11 Jan 2021 23:47:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 11 Jan 2021 23:47:17 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:159e5727ea618dfe8b08811112e2c51f5bd2b9ae7db9eb214914a65249f70ca0`  
		Last Modified: Wed, 16 Dec 2020 23:41:08 GMT  
		Size: 2.7 MB (2709048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e424273d6cedd00225b67fa1b47e0dd8bf4b2abfa19fbc27f7763f096aeb138`  
		Last Modified: Mon, 11 Jan 2021 23:47:54 GMT  
		Size: 5.7 MB (5668408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33979e718e15555239006f224ba6d995cf9d6d044a7f25493196839d4d5aed73`  
		Last Modified: Mon, 11 Jan 2021 23:47:53 GMT  
		Size: 420.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.20-alpine3.12`

```console
$ docker pull nats-streaming@sha256:54ee921908bc93e1deb621ad5b769a4b1e66fd99781595cacb1e1f526cae5670
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.20-alpine3.12` - linux; amd64

```console
$ docker pull nats-streaming@sha256:ee383fab395fb79ad35d3663e31ba2c1556e67dd1ae42c9a314b14f66d80afa6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.0 MB (8997281 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c2217d4d7856bf852cbd735ef2587447e243436346788e6acaf5f102bcfbf28`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:41 GMT
ADD file:ec475c2abb2d46435286b5ae5efacf5b50b1a9e3b6293b69db3c0172b5b9658b in / 
# Thu, 17 Dec 2020 00:19:42 GMT
CMD ["/bin/sh"]
# Tue, 12 Jan 2021 00:48:03 GMT
ENV NATS_STREAMING_SERVER=0.20.0
# Tue, 12 Jan 2021 00:48:05 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='618008a4902916b6bdb26022343ab91313d4f7fc90b31d0c71ad9e75dc8299e4' ;; 		armhf) natsArch='arm6'; sha256='144b04f8f42793aee1b2deb3f6eb187648c37dcc32d526c607a0af99a847260d' ;; 		armv7) natsArch='arm7'; sha256='720f4a90d1dd536bc04639ae31c70ab46fb3e10556f0f261eb038fdce941f20c' ;; 		x86_64) natsArch='amd64'; sha256='098e2293cce5d457b92f3df35127789422562f1414427c406ffd03ea3bd687c9' ;; 		x86) natsArch='386'; sha256='322a290f4706f14d6ff8160ec437202bd282f61f0607741d0e4c38ef89b83451' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Tue, 12 Jan 2021 00:48:05 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Tue, 12 Jan 2021 00:48:06 GMT
EXPOSE 4222 8222
# Tue, 12 Jan 2021 00:48:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 12 Jan 2021 00:48:06 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:801bfaa63ef2094d770c809815b9e2b9c1194728e5e754ef7bc764030e140cea`  
		Last Modified: Wed, 16 Dec 2020 19:34:50 GMT  
		Size: 2.8 MB (2799066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f9b99285c9495350a993a87920ea4ccf0c2c560a7047d0076af2648f08b7bea`  
		Last Modified: Tue, 12 Jan 2021 00:48:48 GMT  
		Size: 6.2 MB (6197794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:244241c08cee6b44b104d2b942ec81d0a48351c78496d12ee991024881132576`  
		Last Modified: Tue, 12 Jan 2021 00:48:46 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.20-alpine3.12` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:18fd3ddc15d5b65b6ad1171abf76e359cca31b60730750546e0dc0368a805750
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.3 MB (8330755 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0322ce6374b271fc98c0e0a12b42c00a722465006d75394c2ab41bbb47d50c46`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 16 Dec 2020 23:49:43 GMT
ADD file:0a16715e2d0e5811c3c578945d618db0e269847a799340248f9ba8d393c9eec2 in / 
# Wed, 16 Dec 2020 23:49:45 GMT
CMD ["/bin/sh"]
# Mon, 11 Jan 2021 23:53:38 GMT
ENV NATS_STREAMING_SERVER=0.20.0
# Mon, 11 Jan 2021 23:53:42 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='618008a4902916b6bdb26022343ab91313d4f7fc90b31d0c71ad9e75dc8299e4' ;; 		armhf) natsArch='arm6'; sha256='144b04f8f42793aee1b2deb3f6eb187648c37dcc32d526c607a0af99a847260d' ;; 		armv7) natsArch='arm7'; sha256='720f4a90d1dd536bc04639ae31c70ab46fb3e10556f0f261eb038fdce941f20c' ;; 		x86_64) natsArch='amd64'; sha256='098e2293cce5d457b92f3df35127789422562f1414427c406ffd03ea3bd687c9' ;; 		x86) natsArch='386'; sha256='322a290f4706f14d6ff8160ec437202bd282f61f0607741d0e4c38ef89b83451' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Mon, 11 Jan 2021 23:53:43 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Mon, 11 Jan 2021 23:53:44 GMT
EXPOSE 4222 8222
# Mon, 11 Jan 2021 23:53:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 11 Jan 2021 23:53:45 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:93247449aef3c56eb4f7ab7b3fed95743c974b823def6dd86ec84008126e7903`  
		Last Modified: Wed, 16 Dec 2020 23:50:24 GMT  
		Size: 2.6 MB (2604163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d54831e858eddfe2c245e8c154d4422ad61bc9a30c1cfe612ec35f7a12b1e529`  
		Last Modified: Mon, 11 Jan 2021 23:54:22 GMT  
		Size: 5.7 MB (5726171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:412a9e8bb4d16b7ddec81004c2205411fc7b8830d0d2a0f3054a2fe0dc4664cd`  
		Last Modified: Mon, 11 Jan 2021 23:54:20 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.20-alpine3.12` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:b41e2afb428f6345393616c70c1a9d2221db86ab84c6e37be6c252bebf974203
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.1 MB (8125466 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8cfc9155e69d8a79c164c6c96d01ea612fb88e955066a7f2803d0054801875da`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 16 Dec 2020 23:58:14 GMT
ADD file:bd07f77a2b2741ca6bda80d9203be9c7274cf73145bff778cf000db0d8d4e903 in / 
# Wed, 16 Dec 2020 23:58:15 GMT
CMD ["/bin/sh"]
# Tue, 12 Jan 2021 00:18:41 GMT
ENV NATS_STREAMING_SERVER=0.20.0
# Tue, 12 Jan 2021 00:18:51 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='618008a4902916b6bdb26022343ab91313d4f7fc90b31d0c71ad9e75dc8299e4' ;; 		armhf) natsArch='arm6'; sha256='144b04f8f42793aee1b2deb3f6eb187648c37dcc32d526c607a0af99a847260d' ;; 		armv7) natsArch='arm7'; sha256='720f4a90d1dd536bc04639ae31c70ab46fb3e10556f0f261eb038fdce941f20c' ;; 		x86_64) natsArch='amd64'; sha256='098e2293cce5d457b92f3df35127789422562f1414427c406ffd03ea3bd687c9' ;; 		x86) natsArch='386'; sha256='322a290f4706f14d6ff8160ec437202bd282f61f0607741d0e4c38ef89b83451' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Tue, 12 Jan 2021 00:18:54 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Tue, 12 Jan 2021 00:18:57 GMT
EXPOSE 4222 8222
# Tue, 12 Jan 2021 00:18:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 12 Jan 2021 00:18:59 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:c58e8a26a8407acc3ead776f6526efa889fda03270a8d05109208d9f59159420`  
		Last Modified: Wed, 16 Dec 2020 23:58:59 GMT  
		Size: 2.4 MB (2407555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9290155f6f3b723d2522ebaa0d1e2038dcd4f4c978c086bc43fd55a4d8284659`  
		Last Modified: Tue, 12 Jan 2021 00:19:43 GMT  
		Size: 5.7 MB (5717488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4715986f280e125e74cc7b430caa19329b3de9fcfcd40ae588f422be68c37ca`  
		Last Modified: Tue, 12 Jan 2021 00:19:42 GMT  
		Size: 423.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.20-alpine3.12` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:ae8f52346c3d26a49ae885bf56785f3952c14c8622a97e18288ae0abedd51660
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.4 MB (8377876 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5f79e7574653a33192a8af07510cf1a7f03f5c02a77b49072304e701cf514cf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 16 Dec 2020 23:40:26 GMT
ADD file:a4845c3840a3fd0e41e4635a179cce20c81afc6c02e34e3fd5bd2d535698918b in / 
# Wed, 16 Dec 2020 23:40:29 GMT
CMD ["/bin/sh"]
# Mon, 11 Jan 2021 23:47:10 GMT
ENV NATS_STREAMING_SERVER=0.20.0
# Mon, 11 Jan 2021 23:47:14 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='618008a4902916b6bdb26022343ab91313d4f7fc90b31d0c71ad9e75dc8299e4' ;; 		armhf) natsArch='arm6'; sha256='144b04f8f42793aee1b2deb3f6eb187648c37dcc32d526c607a0af99a847260d' ;; 		armv7) natsArch='arm7'; sha256='720f4a90d1dd536bc04639ae31c70ab46fb3e10556f0f261eb038fdce941f20c' ;; 		x86_64) natsArch='amd64'; sha256='098e2293cce5d457b92f3df35127789422562f1414427c406ffd03ea3bd687c9' ;; 		x86) natsArch='386'; sha256='322a290f4706f14d6ff8160ec437202bd282f61f0607741d0e4c38ef89b83451' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Mon, 11 Jan 2021 23:47:15 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Mon, 11 Jan 2021 23:47:15 GMT
EXPOSE 4222 8222
# Mon, 11 Jan 2021 23:47:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 11 Jan 2021 23:47:17 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:159e5727ea618dfe8b08811112e2c51f5bd2b9ae7db9eb214914a65249f70ca0`  
		Last Modified: Wed, 16 Dec 2020 23:41:08 GMT  
		Size: 2.7 MB (2709048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e424273d6cedd00225b67fa1b47e0dd8bf4b2abfa19fbc27f7763f096aeb138`  
		Last Modified: Mon, 11 Jan 2021 23:47:54 GMT  
		Size: 5.7 MB (5668408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33979e718e15555239006f224ba6d995cf9d6d044a7f25493196839d4d5aed73`  
		Last Modified: Mon, 11 Jan 2021 23:47:53 GMT  
		Size: 420.0 B  
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
$ docker pull nats-streaming@sha256:c7b60cb7eb50b0454d787676660cbb52ebc25457d367cc91f7f6219eb3cdc861
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1697; amd64

### `nats-streaming:0.20-nanoserver` - windows version 10.0.17763.1697; amd64

```console
$ docker pull nats-streaming@sha256:131f9c39ac29e11d0dc81c1c26cc0fbbb50b832eaba8715c6504d1dac8418435
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.4 MB (107365498 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef855a422d4be3f13d838208fd85955fd7768b3567bd89861a6d67df15122d4a`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 07 Jan 2021 16:14:35 GMT
RUN Apply image 1809-amd64
# Wed, 13 Jan 2021 19:06:01 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Thu, 14 Jan 2021 00:16:51 GMT
RUN cmd /S /C #(nop) COPY file:f2450ffeda74e33f820191eccf78b6647ce56865170e966bfa8e72afe6e46c36 in C:\nats-streaming-server.exe 
# Thu, 14 Jan 2021 00:16:52 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Thu, 14 Jan 2021 00:16:53 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Thu, 14 Jan 2021 00:16:54 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:62239e9aa1a352a20b0d4969c2b508b8a18d10e799d4db72e6f24ccbb2c724d9`  
		Size: 101.3 MB (101340070 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:0a89b73109217060f51d51b7d3a7eda3a9ac0de9c5f76db54addb98b7f1c24c1`  
		Last Modified: Wed, 13 Jan 2021 19:10:49 GMT  
		Size: 885.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65b689a2a270a9c8e1ec741a7297ca14c2001e9a7ab5c9ea3d06f4cf834b8261`  
		Last Modified: Thu, 14 Jan 2021 00:21:28 GMT  
		Size: 6.0 MB (6021918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9339c8634418d855b08dc20f472d3906160f6010ee4b4f1c803e0e9cc4f6d6e3`  
		Last Modified: Thu, 14 Jan 2021 00:21:23 GMT  
		Size: 877.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1de47275056946f9394ba060e89e9ab1710aa73977d6485df317ed346a3c6ed1`  
		Last Modified: Thu, 14 Jan 2021 00:21:25 GMT  
		Size: 865.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4b4ebb72cdd066de0407bdd35275fc5528023c450322d57a92f6527fc42b931`  
		Last Modified: Thu, 14 Jan 2021 00:21:24 GMT  
		Size: 883.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.20-nanoserver-1809`

```console
$ docker pull nats-streaming@sha256:c7b60cb7eb50b0454d787676660cbb52ebc25457d367cc91f7f6219eb3cdc861
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1697; amd64

### `nats-streaming:0.20-nanoserver-1809` - windows version 10.0.17763.1697; amd64

```console
$ docker pull nats-streaming@sha256:131f9c39ac29e11d0dc81c1c26cc0fbbb50b832eaba8715c6504d1dac8418435
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.4 MB (107365498 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef855a422d4be3f13d838208fd85955fd7768b3567bd89861a6d67df15122d4a`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 07 Jan 2021 16:14:35 GMT
RUN Apply image 1809-amd64
# Wed, 13 Jan 2021 19:06:01 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Thu, 14 Jan 2021 00:16:51 GMT
RUN cmd /S /C #(nop) COPY file:f2450ffeda74e33f820191eccf78b6647ce56865170e966bfa8e72afe6e46c36 in C:\nats-streaming-server.exe 
# Thu, 14 Jan 2021 00:16:52 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Thu, 14 Jan 2021 00:16:53 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Thu, 14 Jan 2021 00:16:54 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:62239e9aa1a352a20b0d4969c2b508b8a18d10e799d4db72e6f24ccbb2c724d9`  
		Size: 101.3 MB (101340070 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:0a89b73109217060f51d51b7d3a7eda3a9ac0de9c5f76db54addb98b7f1c24c1`  
		Last Modified: Wed, 13 Jan 2021 19:10:49 GMT  
		Size: 885.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65b689a2a270a9c8e1ec741a7297ca14c2001e9a7ab5c9ea3d06f4cf834b8261`  
		Last Modified: Thu, 14 Jan 2021 00:21:28 GMT  
		Size: 6.0 MB (6021918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9339c8634418d855b08dc20f472d3906160f6010ee4b4f1c803e0e9cc4f6d6e3`  
		Last Modified: Thu, 14 Jan 2021 00:21:23 GMT  
		Size: 877.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1de47275056946f9394ba060e89e9ab1710aa73977d6485df317ed346a3c6ed1`  
		Last Modified: Thu, 14 Jan 2021 00:21:25 GMT  
		Size: 865.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4b4ebb72cdd066de0407bdd35275fc5528023c450322d57a92f6527fc42b931`  
		Last Modified: Thu, 14 Jan 2021 00:21:24 GMT  
		Size: 883.0 B  
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
$ docker pull nats-streaming@sha256:11ad0d1e03a1ff4fb65d386c0a006568d4734fef5df4dc9b3c62766ce61ac698
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1697; amd64
	-	windows version 10.0.14393.4169; amd64

### `nats-streaming:0.20-windowsservercore` - windows version 10.0.17763.1697; amd64

```console
$ docker pull nats-streaming@sha256:d2daab4b8bc283cf1ddc2ddf53f4f222917ea9e9a1bc67de348a775962c269a0
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2456125476 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c5292ad84e88614d976356e7ff8e6f7e7b2649d2a22528459d8728ba63779a4`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 08 Jan 2021 08:50:52 GMT
RUN Install update 1809-amd64
# Wed, 13 Jan 2021 15:20:56 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 Jan 2021 19:04:04 GMT
ENV NATS_DOCKERIZED=1
# Thu, 14 Jan 2021 00:14:52 GMT
ENV NATS_STREAMING_SERVER=0.20.0
# Thu, 14 Jan 2021 00:14:53 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.20.0/nats-streaming-server-v0.20.0-windows-amd64.zip
# Thu, 14 Jan 2021 00:14:54 GMT
ENV GIT_DOWNLOAD_SHA256=26ae310d3ec11617d380106a769236a6dc2209769c0c36d15cb6736db1b589cb
# Thu, 14 Jan 2021 00:15:24 GMT
RUN Set-PSDebug -Trace 2
# Thu, 14 Jan 2021 00:16:41 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Thu, 14 Jan 2021 00:16:42 GMT
EXPOSE 4222 8222
# Thu, 14 Jan 2021 00:16:43 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Thu, 14 Jan 2021 00:16:44 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4dcc9a9b9e680514ef3fdfcc2ce08a3768f9e412703faa137f4a7c8297600052`  
		Size: 717.4 MB (717439216 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:9f84df50d9e20cf852bfd3555d4e56feabf7b9c735e48c613fc461146876bc03`  
		Last Modified: Wed, 13 Jan 2021 18:31:55 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eff779c93810f460e9728c49a995f9cdd81c09b10ffc6e842f2272d19bf4389c`  
		Last Modified: Wed, 13 Jan 2021 19:10:22 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db50a98331abb7193615377c607d4cc7ea1627e30627f5082cc2a05a1e8cb428`  
		Last Modified: Thu, 14 Jan 2021 00:21:00 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79b5d06af7ef1e49206abf1d378dada3faab78554537f7634ec7b5ecf32c6c6a`  
		Last Modified: Thu, 14 Jan 2021 00:20:59 GMT  
		Size: 1.2 KB (1195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12b88e14e5a7930afc8de8e320c13370e618c24fcad06cd1c1f780c5c8384511`  
		Last Modified: Thu, 14 Jan 2021 00:20:59 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5edc2474a0a8a163a2a2a5cf7f87653f8139b5502f6feb6f6498659f23a0aab3`  
		Last Modified: Thu, 14 Jan 2021 00:21:03 GMT  
		Size: 5.0 MB (4995134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7618255c64c34d36a87a9d6f8651060d3039ff15997db8d45ae63784a1033029`  
		Last Modified: Thu, 14 Jan 2021 00:20:59 GMT  
		Size: 15.3 MB (15349122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c31f9a9cb9ee775a576ab8b2965a6e6519cf8a3204d86fab292f4ef3e4812da`  
		Last Modified: Thu, 14 Jan 2021 00:20:55 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:970ac1da377a92447bf6c7fc7fdb9e99090419dda91b090699f888b52e668f6e`  
		Last Modified: Thu, 14 Jan 2021 00:20:57 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bf641cd6f551e1da67ddae43c327f9d50e79f84861fdbbd5b4fd106bede1abc`  
		Last Modified: Thu, 14 Jan 2021 00:20:55 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.20-windowsservercore` - windows version 10.0.14393.4169; amd64

```console
$ docker pull nats-streaming@sha256:c367ca4a4a285c082ea86a36e7756fa5fb8bdcb26e0d672d001a6c8705665ce4
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5815695855 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a029a9ad083d7eb1f30e9786dd41f47c2e77080d9e9021766804fc0be81a012`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Thu, 07 Jan 2021 11:30:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 13 Jan 2021 15:29:26 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 Jan 2021 19:06:11 GMT
ENV NATS_DOCKERIZED=1
# Thu, 14 Jan 2021 00:16:59 GMT
ENV NATS_STREAMING_SERVER=0.20.0
# Thu, 14 Jan 2021 00:16:59 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.20.0/nats-streaming-server-v0.20.0-windows-amd64.zip
# Thu, 14 Jan 2021 00:17:00 GMT
ENV GIT_DOWNLOAD_SHA256=26ae310d3ec11617d380106a769236a6dc2209769c0c36d15cb6736db1b589cb
# Thu, 14 Jan 2021 00:18:09 GMT
RUN Set-PSDebug -Trace 2
# Thu, 14 Jan 2021 00:20:06 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Thu, 14 Jan 2021 00:20:07 GMT
EXPOSE 4222 8222
# Thu, 14 Jan 2021 00:20:08 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Thu, 14 Jan 2021 00:20:09 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bd091f41e44cabc11504b7e130c74a7ef654f58840ba102e3507c4fdf2bae994`  
		Size: 1.7 GB (1723908142 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3b5ee02f83739eef6745d432d63363ce5f490820d4b3e39ae83aa4e3771c4073`  
		Last Modified: Wed, 13 Jan 2021 18:32:39 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acd1c346230e9eaf41e5c8f582c16f531efe65ddbc7fad4e748dd41227e0bbbb`  
		Last Modified: Wed, 13 Jan 2021 19:11:23 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f108152877e2db7ec4dd6c6de8d00482b91437643ebd0dd7cf43e42190c2890`  
		Last Modified: Thu, 14 Jan 2021 00:21:53 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6e3520bde1739f1c73952b8e57fe35000dbac521a22f348e3a0371d914a1937`  
		Last Modified: Thu, 14 Jan 2021 00:21:53 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:585f9330c9a3eebe8d5e6a286b47d58f468a4450072ff1d43f5e7789c82bc66c`  
		Last Modified: Thu, 14 Jan 2021 00:21:51 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39283eaf29b89a60733eeee6ef01dd8db391eef6ce38d43af691e2ad029afc47`  
		Last Modified: Thu, 14 Jan 2021 00:21:48 GMT  
		Size: 5.6 MB (5634422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e3dbd237456a9c1256853ea1c674bc29dac8a8c889e44cccd2dd5407c865abd`  
		Last Modified: Thu, 14 Jan 2021 00:22:07 GMT  
		Size: 16.2 MB (16158244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55dd8e327b6c1be0b8ef8fc2d1abf1d797ecb1f920126d8eb22725259e09587b`  
		Last Modified: Thu, 14 Jan 2021 00:21:48 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d4d27bf34acd3738303a71be66064e609fe0401657f123b818f3acff11d1144`  
		Last Modified: Thu, 14 Jan 2021 00:21:48 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c0acd7c0d45157eb23fcbcbb981ac80d8c0a013e5feb807d40f8b1d85ae1d30`  
		Last Modified: Thu, 14 Jan 2021 00:21:48 GMT  
		Size: 1.1 KB (1139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.20-windowsservercore-1809`

```console
$ docker pull nats-streaming@sha256:5a3c9931a73fd83aa5cdaef3d876f63dd8265212a5b22c1502fbc38f6c43c94c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1697; amd64

### `nats-streaming:0.20-windowsservercore-1809` - windows version 10.0.17763.1697; amd64

```console
$ docker pull nats-streaming@sha256:d2daab4b8bc283cf1ddc2ddf53f4f222917ea9e9a1bc67de348a775962c269a0
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2456125476 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c5292ad84e88614d976356e7ff8e6f7e7b2649d2a22528459d8728ba63779a4`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 08 Jan 2021 08:50:52 GMT
RUN Install update 1809-amd64
# Wed, 13 Jan 2021 15:20:56 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 Jan 2021 19:04:04 GMT
ENV NATS_DOCKERIZED=1
# Thu, 14 Jan 2021 00:14:52 GMT
ENV NATS_STREAMING_SERVER=0.20.0
# Thu, 14 Jan 2021 00:14:53 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.20.0/nats-streaming-server-v0.20.0-windows-amd64.zip
# Thu, 14 Jan 2021 00:14:54 GMT
ENV GIT_DOWNLOAD_SHA256=26ae310d3ec11617d380106a769236a6dc2209769c0c36d15cb6736db1b589cb
# Thu, 14 Jan 2021 00:15:24 GMT
RUN Set-PSDebug -Trace 2
# Thu, 14 Jan 2021 00:16:41 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Thu, 14 Jan 2021 00:16:42 GMT
EXPOSE 4222 8222
# Thu, 14 Jan 2021 00:16:43 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Thu, 14 Jan 2021 00:16:44 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4dcc9a9b9e680514ef3fdfcc2ce08a3768f9e412703faa137f4a7c8297600052`  
		Size: 717.4 MB (717439216 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:9f84df50d9e20cf852bfd3555d4e56feabf7b9c735e48c613fc461146876bc03`  
		Last Modified: Wed, 13 Jan 2021 18:31:55 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eff779c93810f460e9728c49a995f9cdd81c09b10ffc6e842f2272d19bf4389c`  
		Last Modified: Wed, 13 Jan 2021 19:10:22 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db50a98331abb7193615377c607d4cc7ea1627e30627f5082cc2a05a1e8cb428`  
		Last Modified: Thu, 14 Jan 2021 00:21:00 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79b5d06af7ef1e49206abf1d378dada3faab78554537f7634ec7b5ecf32c6c6a`  
		Last Modified: Thu, 14 Jan 2021 00:20:59 GMT  
		Size: 1.2 KB (1195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12b88e14e5a7930afc8de8e320c13370e618c24fcad06cd1c1f780c5c8384511`  
		Last Modified: Thu, 14 Jan 2021 00:20:59 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5edc2474a0a8a163a2a2a5cf7f87653f8139b5502f6feb6f6498659f23a0aab3`  
		Last Modified: Thu, 14 Jan 2021 00:21:03 GMT  
		Size: 5.0 MB (4995134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7618255c64c34d36a87a9d6f8651060d3039ff15997db8d45ae63784a1033029`  
		Last Modified: Thu, 14 Jan 2021 00:20:59 GMT  
		Size: 15.3 MB (15349122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c31f9a9cb9ee775a576ab8b2965a6e6519cf8a3204d86fab292f4ef3e4812da`  
		Last Modified: Thu, 14 Jan 2021 00:20:55 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:970ac1da377a92447bf6c7fc7fdb9e99090419dda91b090699f888b52e668f6e`  
		Last Modified: Thu, 14 Jan 2021 00:20:57 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bf641cd6f551e1da67ddae43c327f9d50e79f84861fdbbd5b4fd106bede1abc`  
		Last Modified: Thu, 14 Jan 2021 00:20:55 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.20-windowsservercore-ltsc2016`

```console
$ docker pull nats-streaming@sha256:69f55054852b78b108077f2c54bbeb3e546b35558384bf8179be11ad1a8766e2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4169; amd64

### `nats-streaming:0.20-windowsservercore-ltsc2016` - windows version 10.0.14393.4169; amd64

```console
$ docker pull nats-streaming@sha256:c367ca4a4a285c082ea86a36e7756fa5fb8bdcb26e0d672d001a6c8705665ce4
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5815695855 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a029a9ad083d7eb1f30e9786dd41f47c2e77080d9e9021766804fc0be81a012`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Thu, 07 Jan 2021 11:30:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 13 Jan 2021 15:29:26 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 Jan 2021 19:06:11 GMT
ENV NATS_DOCKERIZED=1
# Thu, 14 Jan 2021 00:16:59 GMT
ENV NATS_STREAMING_SERVER=0.20.0
# Thu, 14 Jan 2021 00:16:59 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.20.0/nats-streaming-server-v0.20.0-windows-amd64.zip
# Thu, 14 Jan 2021 00:17:00 GMT
ENV GIT_DOWNLOAD_SHA256=26ae310d3ec11617d380106a769236a6dc2209769c0c36d15cb6736db1b589cb
# Thu, 14 Jan 2021 00:18:09 GMT
RUN Set-PSDebug -Trace 2
# Thu, 14 Jan 2021 00:20:06 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Thu, 14 Jan 2021 00:20:07 GMT
EXPOSE 4222 8222
# Thu, 14 Jan 2021 00:20:08 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Thu, 14 Jan 2021 00:20:09 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bd091f41e44cabc11504b7e130c74a7ef654f58840ba102e3507c4fdf2bae994`  
		Size: 1.7 GB (1723908142 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3b5ee02f83739eef6745d432d63363ce5f490820d4b3e39ae83aa4e3771c4073`  
		Last Modified: Wed, 13 Jan 2021 18:32:39 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acd1c346230e9eaf41e5c8f582c16f531efe65ddbc7fad4e748dd41227e0bbbb`  
		Last Modified: Wed, 13 Jan 2021 19:11:23 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f108152877e2db7ec4dd6c6de8d00482b91437643ebd0dd7cf43e42190c2890`  
		Last Modified: Thu, 14 Jan 2021 00:21:53 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6e3520bde1739f1c73952b8e57fe35000dbac521a22f348e3a0371d914a1937`  
		Last Modified: Thu, 14 Jan 2021 00:21:53 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:585f9330c9a3eebe8d5e6a286b47d58f468a4450072ff1d43f5e7789c82bc66c`  
		Last Modified: Thu, 14 Jan 2021 00:21:51 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39283eaf29b89a60733eeee6ef01dd8db391eef6ce38d43af691e2ad029afc47`  
		Last Modified: Thu, 14 Jan 2021 00:21:48 GMT  
		Size: 5.6 MB (5634422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e3dbd237456a9c1256853ea1c674bc29dac8a8c889e44cccd2dd5407c865abd`  
		Last Modified: Thu, 14 Jan 2021 00:22:07 GMT  
		Size: 16.2 MB (16158244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55dd8e327b6c1be0b8ef8fc2d1abf1d797ecb1f920126d8eb22725259e09587b`  
		Last Modified: Thu, 14 Jan 2021 00:21:48 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d4d27bf34acd3738303a71be66064e609fe0401657f123b818f3acff11d1144`  
		Last Modified: Thu, 14 Jan 2021 00:21:48 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c0acd7c0d45157eb23fcbcbb981ac80d8c0a013e5feb807d40f8b1d85ae1d30`  
		Last Modified: Thu, 14 Jan 2021 00:21:48 GMT  
		Size: 1.1 KB (1139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:alpine`

```console
$ docker pull nats-streaming@sha256:54ee921908bc93e1deb621ad5b769a4b1e66fd99781595cacb1e1f526cae5670
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:alpine` - linux; amd64

```console
$ docker pull nats-streaming@sha256:ee383fab395fb79ad35d3663e31ba2c1556e67dd1ae42c9a314b14f66d80afa6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.0 MB (8997281 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c2217d4d7856bf852cbd735ef2587447e243436346788e6acaf5f102bcfbf28`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:41 GMT
ADD file:ec475c2abb2d46435286b5ae5efacf5b50b1a9e3b6293b69db3c0172b5b9658b in / 
# Thu, 17 Dec 2020 00:19:42 GMT
CMD ["/bin/sh"]
# Tue, 12 Jan 2021 00:48:03 GMT
ENV NATS_STREAMING_SERVER=0.20.0
# Tue, 12 Jan 2021 00:48:05 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='618008a4902916b6bdb26022343ab91313d4f7fc90b31d0c71ad9e75dc8299e4' ;; 		armhf) natsArch='arm6'; sha256='144b04f8f42793aee1b2deb3f6eb187648c37dcc32d526c607a0af99a847260d' ;; 		armv7) natsArch='arm7'; sha256='720f4a90d1dd536bc04639ae31c70ab46fb3e10556f0f261eb038fdce941f20c' ;; 		x86_64) natsArch='amd64'; sha256='098e2293cce5d457b92f3df35127789422562f1414427c406ffd03ea3bd687c9' ;; 		x86) natsArch='386'; sha256='322a290f4706f14d6ff8160ec437202bd282f61f0607741d0e4c38ef89b83451' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Tue, 12 Jan 2021 00:48:05 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Tue, 12 Jan 2021 00:48:06 GMT
EXPOSE 4222 8222
# Tue, 12 Jan 2021 00:48:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 12 Jan 2021 00:48:06 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:801bfaa63ef2094d770c809815b9e2b9c1194728e5e754ef7bc764030e140cea`  
		Last Modified: Wed, 16 Dec 2020 19:34:50 GMT  
		Size: 2.8 MB (2799066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f9b99285c9495350a993a87920ea4ccf0c2c560a7047d0076af2648f08b7bea`  
		Last Modified: Tue, 12 Jan 2021 00:48:48 GMT  
		Size: 6.2 MB (6197794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:244241c08cee6b44b104d2b942ec81d0a48351c78496d12ee991024881132576`  
		Last Modified: Tue, 12 Jan 2021 00:48:46 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:18fd3ddc15d5b65b6ad1171abf76e359cca31b60730750546e0dc0368a805750
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.3 MB (8330755 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0322ce6374b271fc98c0e0a12b42c00a722465006d75394c2ab41bbb47d50c46`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 16 Dec 2020 23:49:43 GMT
ADD file:0a16715e2d0e5811c3c578945d618db0e269847a799340248f9ba8d393c9eec2 in / 
# Wed, 16 Dec 2020 23:49:45 GMT
CMD ["/bin/sh"]
# Mon, 11 Jan 2021 23:53:38 GMT
ENV NATS_STREAMING_SERVER=0.20.0
# Mon, 11 Jan 2021 23:53:42 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='618008a4902916b6bdb26022343ab91313d4f7fc90b31d0c71ad9e75dc8299e4' ;; 		armhf) natsArch='arm6'; sha256='144b04f8f42793aee1b2deb3f6eb187648c37dcc32d526c607a0af99a847260d' ;; 		armv7) natsArch='arm7'; sha256='720f4a90d1dd536bc04639ae31c70ab46fb3e10556f0f261eb038fdce941f20c' ;; 		x86_64) natsArch='amd64'; sha256='098e2293cce5d457b92f3df35127789422562f1414427c406ffd03ea3bd687c9' ;; 		x86) natsArch='386'; sha256='322a290f4706f14d6ff8160ec437202bd282f61f0607741d0e4c38ef89b83451' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Mon, 11 Jan 2021 23:53:43 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Mon, 11 Jan 2021 23:53:44 GMT
EXPOSE 4222 8222
# Mon, 11 Jan 2021 23:53:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 11 Jan 2021 23:53:45 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:93247449aef3c56eb4f7ab7b3fed95743c974b823def6dd86ec84008126e7903`  
		Last Modified: Wed, 16 Dec 2020 23:50:24 GMT  
		Size: 2.6 MB (2604163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d54831e858eddfe2c245e8c154d4422ad61bc9a30c1cfe612ec35f7a12b1e529`  
		Last Modified: Mon, 11 Jan 2021 23:54:22 GMT  
		Size: 5.7 MB (5726171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:412a9e8bb4d16b7ddec81004c2205411fc7b8830d0d2a0f3054a2fe0dc4664cd`  
		Last Modified: Mon, 11 Jan 2021 23:54:20 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:b41e2afb428f6345393616c70c1a9d2221db86ab84c6e37be6c252bebf974203
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.1 MB (8125466 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8cfc9155e69d8a79c164c6c96d01ea612fb88e955066a7f2803d0054801875da`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 16 Dec 2020 23:58:14 GMT
ADD file:bd07f77a2b2741ca6bda80d9203be9c7274cf73145bff778cf000db0d8d4e903 in / 
# Wed, 16 Dec 2020 23:58:15 GMT
CMD ["/bin/sh"]
# Tue, 12 Jan 2021 00:18:41 GMT
ENV NATS_STREAMING_SERVER=0.20.0
# Tue, 12 Jan 2021 00:18:51 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='618008a4902916b6bdb26022343ab91313d4f7fc90b31d0c71ad9e75dc8299e4' ;; 		armhf) natsArch='arm6'; sha256='144b04f8f42793aee1b2deb3f6eb187648c37dcc32d526c607a0af99a847260d' ;; 		armv7) natsArch='arm7'; sha256='720f4a90d1dd536bc04639ae31c70ab46fb3e10556f0f261eb038fdce941f20c' ;; 		x86_64) natsArch='amd64'; sha256='098e2293cce5d457b92f3df35127789422562f1414427c406ffd03ea3bd687c9' ;; 		x86) natsArch='386'; sha256='322a290f4706f14d6ff8160ec437202bd282f61f0607741d0e4c38ef89b83451' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Tue, 12 Jan 2021 00:18:54 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Tue, 12 Jan 2021 00:18:57 GMT
EXPOSE 4222 8222
# Tue, 12 Jan 2021 00:18:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 12 Jan 2021 00:18:59 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:c58e8a26a8407acc3ead776f6526efa889fda03270a8d05109208d9f59159420`  
		Last Modified: Wed, 16 Dec 2020 23:58:59 GMT  
		Size: 2.4 MB (2407555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9290155f6f3b723d2522ebaa0d1e2038dcd4f4c978c086bc43fd55a4d8284659`  
		Last Modified: Tue, 12 Jan 2021 00:19:43 GMT  
		Size: 5.7 MB (5717488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4715986f280e125e74cc7b430caa19329b3de9fcfcd40ae588f422be68c37ca`  
		Last Modified: Tue, 12 Jan 2021 00:19:42 GMT  
		Size: 423.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:ae8f52346c3d26a49ae885bf56785f3952c14c8622a97e18288ae0abedd51660
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.4 MB (8377876 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5f79e7574653a33192a8af07510cf1a7f03f5c02a77b49072304e701cf514cf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 16 Dec 2020 23:40:26 GMT
ADD file:a4845c3840a3fd0e41e4635a179cce20c81afc6c02e34e3fd5bd2d535698918b in / 
# Wed, 16 Dec 2020 23:40:29 GMT
CMD ["/bin/sh"]
# Mon, 11 Jan 2021 23:47:10 GMT
ENV NATS_STREAMING_SERVER=0.20.0
# Mon, 11 Jan 2021 23:47:14 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='618008a4902916b6bdb26022343ab91313d4f7fc90b31d0c71ad9e75dc8299e4' ;; 		armhf) natsArch='arm6'; sha256='144b04f8f42793aee1b2deb3f6eb187648c37dcc32d526c607a0af99a847260d' ;; 		armv7) natsArch='arm7'; sha256='720f4a90d1dd536bc04639ae31c70ab46fb3e10556f0f261eb038fdce941f20c' ;; 		x86_64) natsArch='amd64'; sha256='098e2293cce5d457b92f3df35127789422562f1414427c406ffd03ea3bd687c9' ;; 		x86) natsArch='386'; sha256='322a290f4706f14d6ff8160ec437202bd282f61f0607741d0e4c38ef89b83451' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Mon, 11 Jan 2021 23:47:15 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Mon, 11 Jan 2021 23:47:15 GMT
EXPOSE 4222 8222
# Mon, 11 Jan 2021 23:47:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 11 Jan 2021 23:47:17 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:159e5727ea618dfe8b08811112e2c51f5bd2b9ae7db9eb214914a65249f70ca0`  
		Last Modified: Wed, 16 Dec 2020 23:41:08 GMT  
		Size: 2.7 MB (2709048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e424273d6cedd00225b67fa1b47e0dd8bf4b2abfa19fbc27f7763f096aeb138`  
		Last Modified: Mon, 11 Jan 2021 23:47:54 GMT  
		Size: 5.7 MB (5668408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33979e718e15555239006f224ba6d995cf9d6d044a7f25493196839d4d5aed73`  
		Last Modified: Mon, 11 Jan 2021 23:47:53 GMT  
		Size: 420.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:alpine3.12`

```console
$ docker pull nats-streaming@sha256:54ee921908bc93e1deb621ad5b769a4b1e66fd99781595cacb1e1f526cae5670
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:alpine3.12` - linux; amd64

```console
$ docker pull nats-streaming@sha256:ee383fab395fb79ad35d3663e31ba2c1556e67dd1ae42c9a314b14f66d80afa6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.0 MB (8997281 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c2217d4d7856bf852cbd735ef2587447e243436346788e6acaf5f102bcfbf28`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:41 GMT
ADD file:ec475c2abb2d46435286b5ae5efacf5b50b1a9e3b6293b69db3c0172b5b9658b in / 
# Thu, 17 Dec 2020 00:19:42 GMT
CMD ["/bin/sh"]
# Tue, 12 Jan 2021 00:48:03 GMT
ENV NATS_STREAMING_SERVER=0.20.0
# Tue, 12 Jan 2021 00:48:05 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='618008a4902916b6bdb26022343ab91313d4f7fc90b31d0c71ad9e75dc8299e4' ;; 		armhf) natsArch='arm6'; sha256='144b04f8f42793aee1b2deb3f6eb187648c37dcc32d526c607a0af99a847260d' ;; 		armv7) natsArch='arm7'; sha256='720f4a90d1dd536bc04639ae31c70ab46fb3e10556f0f261eb038fdce941f20c' ;; 		x86_64) natsArch='amd64'; sha256='098e2293cce5d457b92f3df35127789422562f1414427c406ffd03ea3bd687c9' ;; 		x86) natsArch='386'; sha256='322a290f4706f14d6ff8160ec437202bd282f61f0607741d0e4c38ef89b83451' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Tue, 12 Jan 2021 00:48:05 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Tue, 12 Jan 2021 00:48:06 GMT
EXPOSE 4222 8222
# Tue, 12 Jan 2021 00:48:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 12 Jan 2021 00:48:06 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:801bfaa63ef2094d770c809815b9e2b9c1194728e5e754ef7bc764030e140cea`  
		Last Modified: Wed, 16 Dec 2020 19:34:50 GMT  
		Size: 2.8 MB (2799066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f9b99285c9495350a993a87920ea4ccf0c2c560a7047d0076af2648f08b7bea`  
		Last Modified: Tue, 12 Jan 2021 00:48:48 GMT  
		Size: 6.2 MB (6197794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:244241c08cee6b44b104d2b942ec81d0a48351c78496d12ee991024881132576`  
		Last Modified: Tue, 12 Jan 2021 00:48:46 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine3.12` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:18fd3ddc15d5b65b6ad1171abf76e359cca31b60730750546e0dc0368a805750
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.3 MB (8330755 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0322ce6374b271fc98c0e0a12b42c00a722465006d75394c2ab41bbb47d50c46`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 16 Dec 2020 23:49:43 GMT
ADD file:0a16715e2d0e5811c3c578945d618db0e269847a799340248f9ba8d393c9eec2 in / 
# Wed, 16 Dec 2020 23:49:45 GMT
CMD ["/bin/sh"]
# Mon, 11 Jan 2021 23:53:38 GMT
ENV NATS_STREAMING_SERVER=0.20.0
# Mon, 11 Jan 2021 23:53:42 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='618008a4902916b6bdb26022343ab91313d4f7fc90b31d0c71ad9e75dc8299e4' ;; 		armhf) natsArch='arm6'; sha256='144b04f8f42793aee1b2deb3f6eb187648c37dcc32d526c607a0af99a847260d' ;; 		armv7) natsArch='arm7'; sha256='720f4a90d1dd536bc04639ae31c70ab46fb3e10556f0f261eb038fdce941f20c' ;; 		x86_64) natsArch='amd64'; sha256='098e2293cce5d457b92f3df35127789422562f1414427c406ffd03ea3bd687c9' ;; 		x86) natsArch='386'; sha256='322a290f4706f14d6ff8160ec437202bd282f61f0607741d0e4c38ef89b83451' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Mon, 11 Jan 2021 23:53:43 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Mon, 11 Jan 2021 23:53:44 GMT
EXPOSE 4222 8222
# Mon, 11 Jan 2021 23:53:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 11 Jan 2021 23:53:45 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:93247449aef3c56eb4f7ab7b3fed95743c974b823def6dd86ec84008126e7903`  
		Last Modified: Wed, 16 Dec 2020 23:50:24 GMT  
		Size: 2.6 MB (2604163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d54831e858eddfe2c245e8c154d4422ad61bc9a30c1cfe612ec35f7a12b1e529`  
		Last Modified: Mon, 11 Jan 2021 23:54:22 GMT  
		Size: 5.7 MB (5726171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:412a9e8bb4d16b7ddec81004c2205411fc7b8830d0d2a0f3054a2fe0dc4664cd`  
		Last Modified: Mon, 11 Jan 2021 23:54:20 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine3.12` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:b41e2afb428f6345393616c70c1a9d2221db86ab84c6e37be6c252bebf974203
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.1 MB (8125466 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8cfc9155e69d8a79c164c6c96d01ea612fb88e955066a7f2803d0054801875da`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 16 Dec 2020 23:58:14 GMT
ADD file:bd07f77a2b2741ca6bda80d9203be9c7274cf73145bff778cf000db0d8d4e903 in / 
# Wed, 16 Dec 2020 23:58:15 GMT
CMD ["/bin/sh"]
# Tue, 12 Jan 2021 00:18:41 GMT
ENV NATS_STREAMING_SERVER=0.20.0
# Tue, 12 Jan 2021 00:18:51 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='618008a4902916b6bdb26022343ab91313d4f7fc90b31d0c71ad9e75dc8299e4' ;; 		armhf) natsArch='arm6'; sha256='144b04f8f42793aee1b2deb3f6eb187648c37dcc32d526c607a0af99a847260d' ;; 		armv7) natsArch='arm7'; sha256='720f4a90d1dd536bc04639ae31c70ab46fb3e10556f0f261eb038fdce941f20c' ;; 		x86_64) natsArch='amd64'; sha256='098e2293cce5d457b92f3df35127789422562f1414427c406ffd03ea3bd687c9' ;; 		x86) natsArch='386'; sha256='322a290f4706f14d6ff8160ec437202bd282f61f0607741d0e4c38ef89b83451' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Tue, 12 Jan 2021 00:18:54 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Tue, 12 Jan 2021 00:18:57 GMT
EXPOSE 4222 8222
# Tue, 12 Jan 2021 00:18:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 12 Jan 2021 00:18:59 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:c58e8a26a8407acc3ead776f6526efa889fda03270a8d05109208d9f59159420`  
		Last Modified: Wed, 16 Dec 2020 23:58:59 GMT  
		Size: 2.4 MB (2407555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9290155f6f3b723d2522ebaa0d1e2038dcd4f4c978c086bc43fd55a4d8284659`  
		Last Modified: Tue, 12 Jan 2021 00:19:43 GMT  
		Size: 5.7 MB (5717488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4715986f280e125e74cc7b430caa19329b3de9fcfcd40ae588f422be68c37ca`  
		Last Modified: Tue, 12 Jan 2021 00:19:42 GMT  
		Size: 423.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine3.12` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:ae8f52346c3d26a49ae885bf56785f3952c14c8622a97e18288ae0abedd51660
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.4 MB (8377876 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5f79e7574653a33192a8af07510cf1a7f03f5c02a77b49072304e701cf514cf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 16 Dec 2020 23:40:26 GMT
ADD file:a4845c3840a3fd0e41e4635a179cce20c81afc6c02e34e3fd5bd2d535698918b in / 
# Wed, 16 Dec 2020 23:40:29 GMT
CMD ["/bin/sh"]
# Mon, 11 Jan 2021 23:47:10 GMT
ENV NATS_STREAMING_SERVER=0.20.0
# Mon, 11 Jan 2021 23:47:14 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='618008a4902916b6bdb26022343ab91313d4f7fc90b31d0c71ad9e75dc8299e4' ;; 		armhf) natsArch='arm6'; sha256='144b04f8f42793aee1b2deb3f6eb187648c37dcc32d526c607a0af99a847260d' ;; 		armv7) natsArch='arm7'; sha256='720f4a90d1dd536bc04639ae31c70ab46fb3e10556f0f261eb038fdce941f20c' ;; 		x86_64) natsArch='amd64'; sha256='098e2293cce5d457b92f3df35127789422562f1414427c406ffd03ea3bd687c9' ;; 		x86) natsArch='386'; sha256='322a290f4706f14d6ff8160ec437202bd282f61f0607741d0e4c38ef89b83451' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Mon, 11 Jan 2021 23:47:15 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Mon, 11 Jan 2021 23:47:15 GMT
EXPOSE 4222 8222
# Mon, 11 Jan 2021 23:47:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 11 Jan 2021 23:47:17 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:159e5727ea618dfe8b08811112e2c51f5bd2b9ae7db9eb214914a65249f70ca0`  
		Last Modified: Wed, 16 Dec 2020 23:41:08 GMT  
		Size: 2.7 MB (2709048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e424273d6cedd00225b67fa1b47e0dd8bf4b2abfa19fbc27f7763f096aeb138`  
		Last Modified: Mon, 11 Jan 2021 23:47:54 GMT  
		Size: 5.7 MB (5668408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33979e718e15555239006f224ba6d995cf9d6d044a7f25493196839d4d5aed73`  
		Last Modified: Mon, 11 Jan 2021 23:47:53 GMT  
		Size: 420.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:latest`

```console
$ docker pull nats-streaming@sha256:75a03d7b41efbfe88ad632319a99ec0a93c546d202c7caa3481d07cd8ea559c2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.1697; amd64

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

### `nats-streaming:latest` - windows version 10.0.17763.1697; amd64

```console
$ docker pull nats-streaming@sha256:131f9c39ac29e11d0dc81c1c26cc0fbbb50b832eaba8715c6504d1dac8418435
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.4 MB (107365498 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef855a422d4be3f13d838208fd85955fd7768b3567bd89861a6d67df15122d4a`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 07 Jan 2021 16:14:35 GMT
RUN Apply image 1809-amd64
# Wed, 13 Jan 2021 19:06:01 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Thu, 14 Jan 2021 00:16:51 GMT
RUN cmd /S /C #(nop) COPY file:f2450ffeda74e33f820191eccf78b6647ce56865170e966bfa8e72afe6e46c36 in C:\nats-streaming-server.exe 
# Thu, 14 Jan 2021 00:16:52 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Thu, 14 Jan 2021 00:16:53 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Thu, 14 Jan 2021 00:16:54 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:62239e9aa1a352a20b0d4969c2b508b8a18d10e799d4db72e6f24ccbb2c724d9`  
		Size: 101.3 MB (101340070 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:0a89b73109217060f51d51b7d3a7eda3a9ac0de9c5f76db54addb98b7f1c24c1`  
		Last Modified: Wed, 13 Jan 2021 19:10:49 GMT  
		Size: 885.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65b689a2a270a9c8e1ec741a7297ca14c2001e9a7ab5c9ea3d06f4cf834b8261`  
		Last Modified: Thu, 14 Jan 2021 00:21:28 GMT  
		Size: 6.0 MB (6021918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9339c8634418d855b08dc20f472d3906160f6010ee4b4f1c803e0e9cc4f6d6e3`  
		Last Modified: Thu, 14 Jan 2021 00:21:23 GMT  
		Size: 877.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1de47275056946f9394ba060e89e9ab1710aa73977d6485df317ed346a3c6ed1`  
		Last Modified: Thu, 14 Jan 2021 00:21:25 GMT  
		Size: 865.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4b4ebb72cdd066de0407bdd35275fc5528023c450322d57a92f6527fc42b931`  
		Last Modified: Thu, 14 Jan 2021 00:21:24 GMT  
		Size: 883.0 B  
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
$ docker pull nats-streaming@sha256:c7b60cb7eb50b0454d787676660cbb52ebc25457d367cc91f7f6219eb3cdc861
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1697; amd64

### `nats-streaming:nanoserver` - windows version 10.0.17763.1697; amd64

```console
$ docker pull nats-streaming@sha256:131f9c39ac29e11d0dc81c1c26cc0fbbb50b832eaba8715c6504d1dac8418435
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.4 MB (107365498 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef855a422d4be3f13d838208fd85955fd7768b3567bd89861a6d67df15122d4a`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 07 Jan 2021 16:14:35 GMT
RUN Apply image 1809-amd64
# Wed, 13 Jan 2021 19:06:01 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Thu, 14 Jan 2021 00:16:51 GMT
RUN cmd /S /C #(nop) COPY file:f2450ffeda74e33f820191eccf78b6647ce56865170e966bfa8e72afe6e46c36 in C:\nats-streaming-server.exe 
# Thu, 14 Jan 2021 00:16:52 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Thu, 14 Jan 2021 00:16:53 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Thu, 14 Jan 2021 00:16:54 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:62239e9aa1a352a20b0d4969c2b508b8a18d10e799d4db72e6f24ccbb2c724d9`  
		Size: 101.3 MB (101340070 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:0a89b73109217060f51d51b7d3a7eda3a9ac0de9c5f76db54addb98b7f1c24c1`  
		Last Modified: Wed, 13 Jan 2021 19:10:49 GMT  
		Size: 885.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65b689a2a270a9c8e1ec741a7297ca14c2001e9a7ab5c9ea3d06f4cf834b8261`  
		Last Modified: Thu, 14 Jan 2021 00:21:28 GMT  
		Size: 6.0 MB (6021918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9339c8634418d855b08dc20f472d3906160f6010ee4b4f1c803e0e9cc4f6d6e3`  
		Last Modified: Thu, 14 Jan 2021 00:21:23 GMT  
		Size: 877.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1de47275056946f9394ba060e89e9ab1710aa73977d6485df317ed346a3c6ed1`  
		Last Modified: Thu, 14 Jan 2021 00:21:25 GMT  
		Size: 865.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4b4ebb72cdd066de0407bdd35275fc5528023c450322d57a92f6527fc42b931`  
		Last Modified: Thu, 14 Jan 2021 00:21:24 GMT  
		Size: 883.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:nanoserver-1809`

```console
$ docker pull nats-streaming@sha256:c7b60cb7eb50b0454d787676660cbb52ebc25457d367cc91f7f6219eb3cdc861
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1697; amd64

### `nats-streaming:nanoserver-1809` - windows version 10.0.17763.1697; amd64

```console
$ docker pull nats-streaming@sha256:131f9c39ac29e11d0dc81c1c26cc0fbbb50b832eaba8715c6504d1dac8418435
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.4 MB (107365498 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef855a422d4be3f13d838208fd85955fd7768b3567bd89861a6d67df15122d4a`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 07 Jan 2021 16:14:35 GMT
RUN Apply image 1809-amd64
# Wed, 13 Jan 2021 19:06:01 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Thu, 14 Jan 2021 00:16:51 GMT
RUN cmd /S /C #(nop) COPY file:f2450ffeda74e33f820191eccf78b6647ce56865170e966bfa8e72afe6e46c36 in C:\nats-streaming-server.exe 
# Thu, 14 Jan 2021 00:16:52 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Thu, 14 Jan 2021 00:16:53 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Thu, 14 Jan 2021 00:16:54 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:62239e9aa1a352a20b0d4969c2b508b8a18d10e799d4db72e6f24ccbb2c724d9`  
		Size: 101.3 MB (101340070 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:0a89b73109217060f51d51b7d3a7eda3a9ac0de9c5f76db54addb98b7f1c24c1`  
		Last Modified: Wed, 13 Jan 2021 19:10:49 GMT  
		Size: 885.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65b689a2a270a9c8e1ec741a7297ca14c2001e9a7ab5c9ea3d06f4cf834b8261`  
		Last Modified: Thu, 14 Jan 2021 00:21:28 GMT  
		Size: 6.0 MB (6021918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9339c8634418d855b08dc20f472d3906160f6010ee4b4f1c803e0e9cc4f6d6e3`  
		Last Modified: Thu, 14 Jan 2021 00:21:23 GMT  
		Size: 877.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1de47275056946f9394ba060e89e9ab1710aa73977d6485df317ed346a3c6ed1`  
		Last Modified: Thu, 14 Jan 2021 00:21:25 GMT  
		Size: 865.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4b4ebb72cdd066de0407bdd35275fc5528023c450322d57a92f6527fc42b931`  
		Last Modified: Thu, 14 Jan 2021 00:21:24 GMT  
		Size: 883.0 B  
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
$ docker pull nats-streaming@sha256:11ad0d1e03a1ff4fb65d386c0a006568d4734fef5df4dc9b3c62766ce61ac698
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1697; amd64
	-	windows version 10.0.14393.4169; amd64

### `nats-streaming:windowsservercore` - windows version 10.0.17763.1697; amd64

```console
$ docker pull nats-streaming@sha256:d2daab4b8bc283cf1ddc2ddf53f4f222917ea9e9a1bc67de348a775962c269a0
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2456125476 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c5292ad84e88614d976356e7ff8e6f7e7b2649d2a22528459d8728ba63779a4`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 08 Jan 2021 08:50:52 GMT
RUN Install update 1809-amd64
# Wed, 13 Jan 2021 15:20:56 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 Jan 2021 19:04:04 GMT
ENV NATS_DOCKERIZED=1
# Thu, 14 Jan 2021 00:14:52 GMT
ENV NATS_STREAMING_SERVER=0.20.0
# Thu, 14 Jan 2021 00:14:53 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.20.0/nats-streaming-server-v0.20.0-windows-amd64.zip
# Thu, 14 Jan 2021 00:14:54 GMT
ENV GIT_DOWNLOAD_SHA256=26ae310d3ec11617d380106a769236a6dc2209769c0c36d15cb6736db1b589cb
# Thu, 14 Jan 2021 00:15:24 GMT
RUN Set-PSDebug -Trace 2
# Thu, 14 Jan 2021 00:16:41 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Thu, 14 Jan 2021 00:16:42 GMT
EXPOSE 4222 8222
# Thu, 14 Jan 2021 00:16:43 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Thu, 14 Jan 2021 00:16:44 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4dcc9a9b9e680514ef3fdfcc2ce08a3768f9e412703faa137f4a7c8297600052`  
		Size: 717.4 MB (717439216 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:9f84df50d9e20cf852bfd3555d4e56feabf7b9c735e48c613fc461146876bc03`  
		Last Modified: Wed, 13 Jan 2021 18:31:55 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eff779c93810f460e9728c49a995f9cdd81c09b10ffc6e842f2272d19bf4389c`  
		Last Modified: Wed, 13 Jan 2021 19:10:22 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db50a98331abb7193615377c607d4cc7ea1627e30627f5082cc2a05a1e8cb428`  
		Last Modified: Thu, 14 Jan 2021 00:21:00 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79b5d06af7ef1e49206abf1d378dada3faab78554537f7634ec7b5ecf32c6c6a`  
		Last Modified: Thu, 14 Jan 2021 00:20:59 GMT  
		Size: 1.2 KB (1195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12b88e14e5a7930afc8de8e320c13370e618c24fcad06cd1c1f780c5c8384511`  
		Last Modified: Thu, 14 Jan 2021 00:20:59 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5edc2474a0a8a163a2a2a5cf7f87653f8139b5502f6feb6f6498659f23a0aab3`  
		Last Modified: Thu, 14 Jan 2021 00:21:03 GMT  
		Size: 5.0 MB (4995134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7618255c64c34d36a87a9d6f8651060d3039ff15997db8d45ae63784a1033029`  
		Last Modified: Thu, 14 Jan 2021 00:20:59 GMT  
		Size: 15.3 MB (15349122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c31f9a9cb9ee775a576ab8b2965a6e6519cf8a3204d86fab292f4ef3e4812da`  
		Last Modified: Thu, 14 Jan 2021 00:20:55 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:970ac1da377a92447bf6c7fc7fdb9e99090419dda91b090699f888b52e668f6e`  
		Last Modified: Thu, 14 Jan 2021 00:20:57 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bf641cd6f551e1da67ddae43c327f9d50e79f84861fdbbd5b4fd106bede1abc`  
		Last Modified: Thu, 14 Jan 2021 00:20:55 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:windowsservercore` - windows version 10.0.14393.4169; amd64

```console
$ docker pull nats-streaming@sha256:c367ca4a4a285c082ea86a36e7756fa5fb8bdcb26e0d672d001a6c8705665ce4
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5815695855 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a029a9ad083d7eb1f30e9786dd41f47c2e77080d9e9021766804fc0be81a012`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Thu, 07 Jan 2021 11:30:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 13 Jan 2021 15:29:26 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 Jan 2021 19:06:11 GMT
ENV NATS_DOCKERIZED=1
# Thu, 14 Jan 2021 00:16:59 GMT
ENV NATS_STREAMING_SERVER=0.20.0
# Thu, 14 Jan 2021 00:16:59 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.20.0/nats-streaming-server-v0.20.0-windows-amd64.zip
# Thu, 14 Jan 2021 00:17:00 GMT
ENV GIT_DOWNLOAD_SHA256=26ae310d3ec11617d380106a769236a6dc2209769c0c36d15cb6736db1b589cb
# Thu, 14 Jan 2021 00:18:09 GMT
RUN Set-PSDebug -Trace 2
# Thu, 14 Jan 2021 00:20:06 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Thu, 14 Jan 2021 00:20:07 GMT
EXPOSE 4222 8222
# Thu, 14 Jan 2021 00:20:08 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Thu, 14 Jan 2021 00:20:09 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bd091f41e44cabc11504b7e130c74a7ef654f58840ba102e3507c4fdf2bae994`  
		Size: 1.7 GB (1723908142 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3b5ee02f83739eef6745d432d63363ce5f490820d4b3e39ae83aa4e3771c4073`  
		Last Modified: Wed, 13 Jan 2021 18:32:39 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acd1c346230e9eaf41e5c8f582c16f531efe65ddbc7fad4e748dd41227e0bbbb`  
		Last Modified: Wed, 13 Jan 2021 19:11:23 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f108152877e2db7ec4dd6c6de8d00482b91437643ebd0dd7cf43e42190c2890`  
		Last Modified: Thu, 14 Jan 2021 00:21:53 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6e3520bde1739f1c73952b8e57fe35000dbac521a22f348e3a0371d914a1937`  
		Last Modified: Thu, 14 Jan 2021 00:21:53 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:585f9330c9a3eebe8d5e6a286b47d58f468a4450072ff1d43f5e7789c82bc66c`  
		Last Modified: Thu, 14 Jan 2021 00:21:51 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39283eaf29b89a60733eeee6ef01dd8db391eef6ce38d43af691e2ad029afc47`  
		Last Modified: Thu, 14 Jan 2021 00:21:48 GMT  
		Size: 5.6 MB (5634422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e3dbd237456a9c1256853ea1c674bc29dac8a8c889e44cccd2dd5407c865abd`  
		Last Modified: Thu, 14 Jan 2021 00:22:07 GMT  
		Size: 16.2 MB (16158244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55dd8e327b6c1be0b8ef8fc2d1abf1d797ecb1f920126d8eb22725259e09587b`  
		Last Modified: Thu, 14 Jan 2021 00:21:48 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d4d27bf34acd3738303a71be66064e609fe0401657f123b818f3acff11d1144`  
		Last Modified: Thu, 14 Jan 2021 00:21:48 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c0acd7c0d45157eb23fcbcbb981ac80d8c0a013e5feb807d40f8b1d85ae1d30`  
		Last Modified: Thu, 14 Jan 2021 00:21:48 GMT  
		Size: 1.1 KB (1139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:windowsservercore-1809`

```console
$ docker pull nats-streaming@sha256:5a3c9931a73fd83aa5cdaef3d876f63dd8265212a5b22c1502fbc38f6c43c94c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1697; amd64

### `nats-streaming:windowsservercore-1809` - windows version 10.0.17763.1697; amd64

```console
$ docker pull nats-streaming@sha256:d2daab4b8bc283cf1ddc2ddf53f4f222917ea9e9a1bc67de348a775962c269a0
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2456125476 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c5292ad84e88614d976356e7ff8e6f7e7b2649d2a22528459d8728ba63779a4`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 08 Jan 2021 08:50:52 GMT
RUN Install update 1809-amd64
# Wed, 13 Jan 2021 15:20:56 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 Jan 2021 19:04:04 GMT
ENV NATS_DOCKERIZED=1
# Thu, 14 Jan 2021 00:14:52 GMT
ENV NATS_STREAMING_SERVER=0.20.0
# Thu, 14 Jan 2021 00:14:53 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.20.0/nats-streaming-server-v0.20.0-windows-amd64.zip
# Thu, 14 Jan 2021 00:14:54 GMT
ENV GIT_DOWNLOAD_SHA256=26ae310d3ec11617d380106a769236a6dc2209769c0c36d15cb6736db1b589cb
# Thu, 14 Jan 2021 00:15:24 GMT
RUN Set-PSDebug -Trace 2
# Thu, 14 Jan 2021 00:16:41 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Thu, 14 Jan 2021 00:16:42 GMT
EXPOSE 4222 8222
# Thu, 14 Jan 2021 00:16:43 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Thu, 14 Jan 2021 00:16:44 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4dcc9a9b9e680514ef3fdfcc2ce08a3768f9e412703faa137f4a7c8297600052`  
		Size: 717.4 MB (717439216 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:9f84df50d9e20cf852bfd3555d4e56feabf7b9c735e48c613fc461146876bc03`  
		Last Modified: Wed, 13 Jan 2021 18:31:55 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eff779c93810f460e9728c49a995f9cdd81c09b10ffc6e842f2272d19bf4389c`  
		Last Modified: Wed, 13 Jan 2021 19:10:22 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db50a98331abb7193615377c607d4cc7ea1627e30627f5082cc2a05a1e8cb428`  
		Last Modified: Thu, 14 Jan 2021 00:21:00 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79b5d06af7ef1e49206abf1d378dada3faab78554537f7634ec7b5ecf32c6c6a`  
		Last Modified: Thu, 14 Jan 2021 00:20:59 GMT  
		Size: 1.2 KB (1195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12b88e14e5a7930afc8de8e320c13370e618c24fcad06cd1c1f780c5c8384511`  
		Last Modified: Thu, 14 Jan 2021 00:20:59 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5edc2474a0a8a163a2a2a5cf7f87653f8139b5502f6feb6f6498659f23a0aab3`  
		Last Modified: Thu, 14 Jan 2021 00:21:03 GMT  
		Size: 5.0 MB (4995134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7618255c64c34d36a87a9d6f8651060d3039ff15997db8d45ae63784a1033029`  
		Last Modified: Thu, 14 Jan 2021 00:20:59 GMT  
		Size: 15.3 MB (15349122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c31f9a9cb9ee775a576ab8b2965a6e6519cf8a3204d86fab292f4ef3e4812da`  
		Last Modified: Thu, 14 Jan 2021 00:20:55 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:970ac1da377a92447bf6c7fc7fdb9e99090419dda91b090699f888b52e668f6e`  
		Last Modified: Thu, 14 Jan 2021 00:20:57 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bf641cd6f551e1da67ddae43c327f9d50e79f84861fdbbd5b4fd106bede1abc`  
		Last Modified: Thu, 14 Jan 2021 00:20:55 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:windowsservercore-ltsc2016`

```console
$ docker pull nats-streaming@sha256:69f55054852b78b108077f2c54bbeb3e546b35558384bf8179be11ad1a8766e2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4169; amd64

### `nats-streaming:windowsservercore-ltsc2016` - windows version 10.0.14393.4169; amd64

```console
$ docker pull nats-streaming@sha256:c367ca4a4a285c082ea86a36e7756fa5fb8bdcb26e0d672d001a6c8705665ce4
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5815695855 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a029a9ad083d7eb1f30e9786dd41f47c2e77080d9e9021766804fc0be81a012`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Thu, 07 Jan 2021 11:30:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 13 Jan 2021 15:29:26 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 Jan 2021 19:06:11 GMT
ENV NATS_DOCKERIZED=1
# Thu, 14 Jan 2021 00:16:59 GMT
ENV NATS_STREAMING_SERVER=0.20.0
# Thu, 14 Jan 2021 00:16:59 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.20.0/nats-streaming-server-v0.20.0-windows-amd64.zip
# Thu, 14 Jan 2021 00:17:00 GMT
ENV GIT_DOWNLOAD_SHA256=26ae310d3ec11617d380106a769236a6dc2209769c0c36d15cb6736db1b589cb
# Thu, 14 Jan 2021 00:18:09 GMT
RUN Set-PSDebug -Trace 2
# Thu, 14 Jan 2021 00:20:06 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Thu, 14 Jan 2021 00:20:07 GMT
EXPOSE 4222 8222
# Thu, 14 Jan 2021 00:20:08 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Thu, 14 Jan 2021 00:20:09 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bd091f41e44cabc11504b7e130c74a7ef654f58840ba102e3507c4fdf2bae994`  
		Size: 1.7 GB (1723908142 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3b5ee02f83739eef6745d432d63363ce5f490820d4b3e39ae83aa4e3771c4073`  
		Last Modified: Wed, 13 Jan 2021 18:32:39 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acd1c346230e9eaf41e5c8f582c16f531efe65ddbc7fad4e748dd41227e0bbbb`  
		Last Modified: Wed, 13 Jan 2021 19:11:23 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f108152877e2db7ec4dd6c6de8d00482b91437643ebd0dd7cf43e42190c2890`  
		Last Modified: Thu, 14 Jan 2021 00:21:53 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6e3520bde1739f1c73952b8e57fe35000dbac521a22f348e3a0371d914a1937`  
		Last Modified: Thu, 14 Jan 2021 00:21:53 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:585f9330c9a3eebe8d5e6a286b47d58f468a4450072ff1d43f5e7789c82bc66c`  
		Last Modified: Thu, 14 Jan 2021 00:21:51 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39283eaf29b89a60733eeee6ef01dd8db391eef6ce38d43af691e2ad029afc47`  
		Last Modified: Thu, 14 Jan 2021 00:21:48 GMT  
		Size: 5.6 MB (5634422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e3dbd237456a9c1256853ea1c674bc29dac8a8c889e44cccd2dd5407c865abd`  
		Last Modified: Thu, 14 Jan 2021 00:22:07 GMT  
		Size: 16.2 MB (16158244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55dd8e327b6c1be0b8ef8fc2d1abf1d797ecb1f920126d8eb22725259e09587b`  
		Last Modified: Thu, 14 Jan 2021 00:21:48 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d4d27bf34acd3738303a71be66064e609fe0401657f123b818f3acff11d1144`  
		Last Modified: Thu, 14 Jan 2021 00:21:48 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c0acd7c0d45157eb23fcbcbb981ac80d8c0a013e5feb807d40f8b1d85ae1d30`  
		Last Modified: Thu, 14 Jan 2021 00:21:48 GMT  
		Size: 1.1 KB (1139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
