<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `traefik`

-	[`traefik:2.10`](#traefik210)
-	[`traefik:2.10-windowsservercore-1809`](#traefik210-windowsservercore-1809)
-	[`traefik:2.10.5`](#traefik2105)
-	[`traefik:2.10.5-windowsservercore-1809`](#traefik2105-windowsservercore-1809)
-	[`traefik:3.0`](#traefik30)
-	[`traefik:3.0-windowsservercore-1809`](#traefik30-windowsservercore-1809)
-	[`traefik:3.0.0-beta4`](#traefik300-beta4)
-	[`traefik:3.0.0-beta4-windowsservercore-1809`](#traefik300-beta4-windowsservercore-1809)
-	[`traefik:beaufort`](#traefikbeaufort)
-	[`traefik:beaufort-windowsservercore-1809`](#traefikbeaufort-windowsservercore-1809)
-	[`traefik:latest`](#traefiklatest)
-	[`traefik:saintmarcelin`](#traefiksaintmarcelin)
-	[`traefik:saintmarcelin-windowsservercore-1809`](#traefiksaintmarcelin-windowsservercore-1809)
-	[`traefik:v2.10`](#traefikv210)
-	[`traefik:v2.10-windowsservercore-1809`](#traefikv210-windowsservercore-1809)
-	[`traefik:v2.10.5`](#traefikv2105)
-	[`traefik:v2.10.5-windowsservercore-1809`](#traefikv2105-windowsservercore-1809)
-	[`traefik:v3.0`](#traefikv30)
-	[`traefik:v3.0-windowsservercore-1809`](#traefikv30-windowsservercore-1809)
-	[`traefik:v3.0.0-beta4`](#traefikv300-beta4)
-	[`traefik:v3.0.0-beta4-windowsservercore-1809`](#traefikv300-beta4-windowsservercore-1809)
-	[`traefik:windowsservercore-1809`](#traefikwindowsservercore-1809)

## `traefik:2.10`

```console
$ docker pull traefik@sha256:948978f7ec62f137a79f8af7044a1785bd7868706ef2c8cba9c88db688d08661
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:2.10` - linux; amd64

```console
$ docker pull traefik@sha256:9701f2c228e65fbaced54478b24f3953502192d396823ebdb2aa9b9e37b0e647
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.1 MB (43135183 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cc365cbb0397b708abc260501574769de3891d756c7a2e43c3839e9126cf9aec`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 28 Sep 2023 21:19:27 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Thu, 28 Sep 2023 21:19:27 GMT
CMD ["/bin/sh"]
# Fri, 29 Sep 2023 03:23:55 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 11 Oct 2023 18:19:24 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.5/traefik_v2.10.5_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 11 Oct 2023 18:19:24 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 11 Oct 2023 18:19:24 GMT
EXPOSE 80
# Wed, 11 Oct 2023 18:19:24 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 11 Oct 2023 18:19:25 GMT
CMD ["traefik"]
# Wed, 11 Oct 2023 18:19:25 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.5 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eeed05813ad6dab5b7d0156cab3e4976cd245786d76cc19071687bf8232d0683`  
		Last Modified: Fri, 29 Sep 2023 03:24:23 GMT  
		Size: 622.3 KB (622285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86ea8083d7bce4dd990c2ea838f2c04ab7fcc56a861c000ae0094825b6912661`  
		Last Modified: Wed, 11 Oct 2023 18:19:48 GMT  
		Size: 39.1 MB (39110563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cea349f5f8a775924119f640676ef0b55a652143545b75c966e52dccc0b25a3b`  
		Last Modified: Wed, 11 Oct 2023 18:19:42 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.10` - linux; arm variant v6

```console
$ docker pull traefik@sha256:dc00301f748218be762305628990942becd6157e6e3e5cfe75a13fdd3fdb76bb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.7 MB (40720959 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4ec390e620b8982f8897b4224718a34eaf67f26bbedf3c0925701a7b61036b6`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 28 Sep 2023 20:49:16 GMT
ADD file:2222b03381ff0fce22edd647f5c60529ec6a72202f8d3cb1d6e4648ebcd19a1e in / 
# Thu, 28 Sep 2023 20:49:16 GMT
CMD ["/bin/sh"]
# Fri, 29 Sep 2023 02:07:55 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 11 Oct 2023 17:33:52 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.5/traefik_v2.10.5_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 11 Oct 2023 17:33:52 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 11 Oct 2023 17:33:52 GMT
EXPOSE 80
# Wed, 11 Oct 2023 17:33:52 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 11 Oct 2023 17:33:53 GMT
CMD ["traefik"]
# Wed, 11 Oct 2023 17:33:53 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.5 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:91cb83b91ee16f1ee0d588fccef56ab5dbb5689a64e5373caf33d7e4fe52ceb4`  
		Last Modified: Thu, 28 Sep 2023 20:51:25 GMT  
		Size: 3.1 MB (3145291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:145b6a121fb4926fc8535cfa17caa1e1cd475fcc89a18cc9ecabe5da99ff5462`  
		Last Modified: Fri, 29 Sep 2023 02:08:23 GMT  
		Size: 622.7 KB (622716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aabde1aa4d1522179691248f83aa55c1242b3d42e4523b43ecfc956b07a45441`  
		Last Modified: Wed, 11 Oct 2023 17:34:13 GMT  
		Size: 37.0 MB (36952584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f16736147d14f3ed928c692cce1e4373ddceb0416d08c37aeeda8f6ddc58f2f`  
		Last Modified: Wed, 11 Oct 2023 17:34:07 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.10` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:4d7c60c1d882dafc8f0148231d836f7d1e2fef0d732daf1cd16f37d711afe689
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.1 MB (40122097 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1bdddb248186d54fa971abe0cc8f4e1b8a05579d6e129cef0cd8e4aace2cdec`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 28 Sep 2023 20:39:33 GMT
ADD file:ff3112828967e8004a3264d7ece3f81c88e6a1d44d360b9b5613caab15b41717 in / 
# Thu, 28 Sep 2023 20:39:34 GMT
CMD ["/bin/sh"]
# Fri, 29 Sep 2023 02:23:59 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 11 Oct 2023 18:23:41 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.5/traefik_v2.10.5_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 11 Oct 2023 18:23:41 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 11 Oct 2023 18:23:41 GMT
EXPOSE 80
# Wed, 11 Oct 2023 18:23:42 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 11 Oct 2023 18:23:42 GMT
CMD ["traefik"]
# Wed, 11 Oct 2023 18:23:42 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.5 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:579b34f0a95bb83b3acd6b3249ddc52c3d80f5c84b13c944e9e324feb86dd329`  
		Last Modified: Thu, 28 Sep 2023 20:40:08 GMT  
		Size: 3.3 MB (3331831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38b59e422640e276d23497c5544f7d98d0d1a6eed46644029a75b232afc0e4dc`  
		Last Modified: Fri, 29 Sep 2023 02:24:21 GMT  
		Size: 624.5 KB (624514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27163b2644a7f56bc248f42f0002375480295665c372ec73a52045dbd137a1a0`  
		Last Modified: Wed, 11 Oct 2023 18:24:02 GMT  
		Size: 36.2 MB (36165385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:043f01742e9c079f76aa4524a7f55f153a6d0ced946663371b8e157c333c8afa`  
		Last Modified: Wed, 11 Oct 2023 18:23:58 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.10` - linux; s390x

```console
$ docker pull traefik@sha256:0ac60f2c2f4a9564d06dfe1b9f68d47457142d947714c6367d6e2063346c79f9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.0 MB (41958288 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7556291a63d1e75251705523cef1799f2e878e85a4cab148bbc5443b1808c259`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 28 Sep 2023 20:41:43 GMT
ADD file:fd3808a676fc56c1380e55b2ddbf4014d9371346cf789860b336bc9f00729ed0 in / 
# Thu, 28 Sep 2023 20:41:44 GMT
CMD ["/bin/sh"]
# Fri, 29 Sep 2023 00:15:10 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 11 Oct 2023 17:48:05 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.5/traefik_v2.10.5_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 11 Oct 2023 17:48:07 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 11 Oct 2023 17:48:07 GMT
EXPOSE 80
# Wed, 11 Oct 2023 17:48:07 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 11 Oct 2023 17:48:08 GMT
CMD ["traefik"]
# Wed, 11 Oct 2023 17:48:08 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.5 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:47539bffe0f44273ec7731d86be2a6171359b3847c9b60c6ac74c4875c3264af`  
		Last Modified: Thu, 28 Sep 2023 20:43:18 GMT  
		Size: 3.2 MB (3215103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37af407ac96c8e70e35ccb675ba932c1f6a441da5da4bff25fdfee4b8037205c`  
		Last Modified: Fri, 29 Sep 2023 00:15:51 GMT  
		Size: 622.8 KB (622839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fd9a3520d22d271d14445ac3488b3a3c1243ee5a36456303253061f65b58fbf`  
		Last Modified: Wed, 11 Oct 2023 17:48:39 GMT  
		Size: 38.1 MB (38119978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b98e142b7086bf0349c6782eac90d799f78fa452d198cbecd8fdfae62181704f`  
		Last Modified: Wed, 11 Oct 2023 17:48:32 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:2.10-windowsservercore-1809`

```console
$ docker pull traefik@sha256:e48ea53ba59577bef28d3ceb8dd82d512802fc92bba0ea8730217ca65bb7a400
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4974; amd64

### `traefik:2.10-windowsservercore-1809` - windows version 10.0.17763.4974; amd64

```console
$ docker pull traefik@sha256:6ddb17d74fd90ba6dd250de9179642d6b9578d6d56be82327b31f0817eb5f195
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2072188607 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:781a8b280451eba384580300e40e1a90f21b2bce4bebedde69d5c87b66476b17`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Mon, 02 Oct 2023 08:29:38 GMT
RUN Install update 10.0.17763.4974
# Wed, 11 Oct 2023 01:36:38 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Oct 2023 17:53:25 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.10.5/traefik_v2.10.5_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Wed, 11 Oct 2023 17:53:26 GMT
EXPOSE 80
# Wed, 11 Oct 2023 17:53:27 GMT
ENTRYPOINT ["/traefik"]
# Wed, 11 Oct 2023 17:53:28 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.5 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1af2bcb37edaec1dd87fc4a6f7c9129ca37bf1f91b65eb365ba9d4c70473beea`  
		Last Modified: Tue, 10 Oct 2023 17:51:10 GMT  
		Size: 381.0 MB (380970130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0814e4a0bb8c615854a85a2b60cd043cfd20ad5a5d755acab1b30b18e4bfad3c`  
		Last Modified: Wed, 11 Oct 2023 02:46:41 GMT  
		Size: 1.3 KB (1324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f15241f4df03f5eed76e4442d2b3f7a498d9144f1297714e03b04a513bddc8c`  
		Last Modified: Wed, 11 Oct 2023 17:53:58 GMT  
		Size: 40.6 MB (40592559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d40acdeea4d8136d5f835b8e319e6a7d4bc818c64267537a59a2076fb38cd0a8`  
		Last Modified: Wed, 11 Oct 2023 17:53:49 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:289c14de3f4bf9beef5623344f1de08243e9ed0e48c8293aad5c67e937f006b1`  
		Last Modified: Wed, 11 Oct 2023 17:53:49 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a066414845489fe46ce720ac765d0b3b8ad3727c9c622c21223676eed2a8906`  
		Last Modified: Wed, 11 Oct 2023 17:53:49 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:2.10.5`

```console
$ docker pull traefik@sha256:948978f7ec62f137a79f8af7044a1785bd7868706ef2c8cba9c88db688d08661
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:2.10.5` - linux; amd64

```console
$ docker pull traefik@sha256:9701f2c228e65fbaced54478b24f3953502192d396823ebdb2aa9b9e37b0e647
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.1 MB (43135183 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cc365cbb0397b708abc260501574769de3891d756c7a2e43c3839e9126cf9aec`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 28 Sep 2023 21:19:27 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Thu, 28 Sep 2023 21:19:27 GMT
CMD ["/bin/sh"]
# Fri, 29 Sep 2023 03:23:55 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 11 Oct 2023 18:19:24 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.5/traefik_v2.10.5_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 11 Oct 2023 18:19:24 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 11 Oct 2023 18:19:24 GMT
EXPOSE 80
# Wed, 11 Oct 2023 18:19:24 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 11 Oct 2023 18:19:25 GMT
CMD ["traefik"]
# Wed, 11 Oct 2023 18:19:25 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.5 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eeed05813ad6dab5b7d0156cab3e4976cd245786d76cc19071687bf8232d0683`  
		Last Modified: Fri, 29 Sep 2023 03:24:23 GMT  
		Size: 622.3 KB (622285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86ea8083d7bce4dd990c2ea838f2c04ab7fcc56a861c000ae0094825b6912661`  
		Last Modified: Wed, 11 Oct 2023 18:19:48 GMT  
		Size: 39.1 MB (39110563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cea349f5f8a775924119f640676ef0b55a652143545b75c966e52dccc0b25a3b`  
		Last Modified: Wed, 11 Oct 2023 18:19:42 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.10.5` - linux; arm variant v6

```console
$ docker pull traefik@sha256:dc00301f748218be762305628990942becd6157e6e3e5cfe75a13fdd3fdb76bb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.7 MB (40720959 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4ec390e620b8982f8897b4224718a34eaf67f26bbedf3c0925701a7b61036b6`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 28 Sep 2023 20:49:16 GMT
ADD file:2222b03381ff0fce22edd647f5c60529ec6a72202f8d3cb1d6e4648ebcd19a1e in / 
# Thu, 28 Sep 2023 20:49:16 GMT
CMD ["/bin/sh"]
# Fri, 29 Sep 2023 02:07:55 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 11 Oct 2023 17:33:52 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.5/traefik_v2.10.5_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 11 Oct 2023 17:33:52 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 11 Oct 2023 17:33:52 GMT
EXPOSE 80
# Wed, 11 Oct 2023 17:33:52 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 11 Oct 2023 17:33:53 GMT
CMD ["traefik"]
# Wed, 11 Oct 2023 17:33:53 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.5 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:91cb83b91ee16f1ee0d588fccef56ab5dbb5689a64e5373caf33d7e4fe52ceb4`  
		Last Modified: Thu, 28 Sep 2023 20:51:25 GMT  
		Size: 3.1 MB (3145291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:145b6a121fb4926fc8535cfa17caa1e1cd475fcc89a18cc9ecabe5da99ff5462`  
		Last Modified: Fri, 29 Sep 2023 02:08:23 GMT  
		Size: 622.7 KB (622716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aabde1aa4d1522179691248f83aa55c1242b3d42e4523b43ecfc956b07a45441`  
		Last Modified: Wed, 11 Oct 2023 17:34:13 GMT  
		Size: 37.0 MB (36952584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f16736147d14f3ed928c692cce1e4373ddceb0416d08c37aeeda8f6ddc58f2f`  
		Last Modified: Wed, 11 Oct 2023 17:34:07 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.10.5` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:4d7c60c1d882dafc8f0148231d836f7d1e2fef0d732daf1cd16f37d711afe689
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.1 MB (40122097 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1bdddb248186d54fa971abe0cc8f4e1b8a05579d6e129cef0cd8e4aace2cdec`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 28 Sep 2023 20:39:33 GMT
ADD file:ff3112828967e8004a3264d7ece3f81c88e6a1d44d360b9b5613caab15b41717 in / 
# Thu, 28 Sep 2023 20:39:34 GMT
CMD ["/bin/sh"]
# Fri, 29 Sep 2023 02:23:59 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 11 Oct 2023 18:23:41 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.5/traefik_v2.10.5_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 11 Oct 2023 18:23:41 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 11 Oct 2023 18:23:41 GMT
EXPOSE 80
# Wed, 11 Oct 2023 18:23:42 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 11 Oct 2023 18:23:42 GMT
CMD ["traefik"]
# Wed, 11 Oct 2023 18:23:42 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.5 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:579b34f0a95bb83b3acd6b3249ddc52c3d80f5c84b13c944e9e324feb86dd329`  
		Last Modified: Thu, 28 Sep 2023 20:40:08 GMT  
		Size: 3.3 MB (3331831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38b59e422640e276d23497c5544f7d98d0d1a6eed46644029a75b232afc0e4dc`  
		Last Modified: Fri, 29 Sep 2023 02:24:21 GMT  
		Size: 624.5 KB (624514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27163b2644a7f56bc248f42f0002375480295665c372ec73a52045dbd137a1a0`  
		Last Modified: Wed, 11 Oct 2023 18:24:02 GMT  
		Size: 36.2 MB (36165385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:043f01742e9c079f76aa4524a7f55f153a6d0ced946663371b8e157c333c8afa`  
		Last Modified: Wed, 11 Oct 2023 18:23:58 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.10.5` - linux; s390x

```console
$ docker pull traefik@sha256:0ac60f2c2f4a9564d06dfe1b9f68d47457142d947714c6367d6e2063346c79f9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.0 MB (41958288 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7556291a63d1e75251705523cef1799f2e878e85a4cab148bbc5443b1808c259`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 28 Sep 2023 20:41:43 GMT
ADD file:fd3808a676fc56c1380e55b2ddbf4014d9371346cf789860b336bc9f00729ed0 in / 
# Thu, 28 Sep 2023 20:41:44 GMT
CMD ["/bin/sh"]
# Fri, 29 Sep 2023 00:15:10 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 11 Oct 2023 17:48:05 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.5/traefik_v2.10.5_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 11 Oct 2023 17:48:07 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 11 Oct 2023 17:48:07 GMT
EXPOSE 80
# Wed, 11 Oct 2023 17:48:07 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 11 Oct 2023 17:48:08 GMT
CMD ["traefik"]
# Wed, 11 Oct 2023 17:48:08 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.5 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:47539bffe0f44273ec7731d86be2a6171359b3847c9b60c6ac74c4875c3264af`  
		Last Modified: Thu, 28 Sep 2023 20:43:18 GMT  
		Size: 3.2 MB (3215103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37af407ac96c8e70e35ccb675ba932c1f6a441da5da4bff25fdfee4b8037205c`  
		Last Modified: Fri, 29 Sep 2023 00:15:51 GMT  
		Size: 622.8 KB (622839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fd9a3520d22d271d14445ac3488b3a3c1243ee5a36456303253061f65b58fbf`  
		Last Modified: Wed, 11 Oct 2023 17:48:39 GMT  
		Size: 38.1 MB (38119978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b98e142b7086bf0349c6782eac90d799f78fa452d198cbecd8fdfae62181704f`  
		Last Modified: Wed, 11 Oct 2023 17:48:32 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:2.10.5-windowsservercore-1809`

```console
$ docker pull traefik@sha256:e48ea53ba59577bef28d3ceb8dd82d512802fc92bba0ea8730217ca65bb7a400
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4974; amd64

### `traefik:2.10.5-windowsservercore-1809` - windows version 10.0.17763.4974; amd64

```console
$ docker pull traefik@sha256:6ddb17d74fd90ba6dd250de9179642d6b9578d6d56be82327b31f0817eb5f195
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2072188607 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:781a8b280451eba384580300e40e1a90f21b2bce4bebedde69d5c87b66476b17`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Mon, 02 Oct 2023 08:29:38 GMT
RUN Install update 10.0.17763.4974
# Wed, 11 Oct 2023 01:36:38 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Oct 2023 17:53:25 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.10.5/traefik_v2.10.5_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Wed, 11 Oct 2023 17:53:26 GMT
EXPOSE 80
# Wed, 11 Oct 2023 17:53:27 GMT
ENTRYPOINT ["/traefik"]
# Wed, 11 Oct 2023 17:53:28 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.5 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1af2bcb37edaec1dd87fc4a6f7c9129ca37bf1f91b65eb365ba9d4c70473beea`  
		Last Modified: Tue, 10 Oct 2023 17:51:10 GMT  
		Size: 381.0 MB (380970130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0814e4a0bb8c615854a85a2b60cd043cfd20ad5a5d755acab1b30b18e4bfad3c`  
		Last Modified: Wed, 11 Oct 2023 02:46:41 GMT  
		Size: 1.3 KB (1324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f15241f4df03f5eed76e4442d2b3f7a498d9144f1297714e03b04a513bddc8c`  
		Last Modified: Wed, 11 Oct 2023 17:53:58 GMT  
		Size: 40.6 MB (40592559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d40acdeea4d8136d5f835b8e319e6a7d4bc818c64267537a59a2076fb38cd0a8`  
		Last Modified: Wed, 11 Oct 2023 17:53:49 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:289c14de3f4bf9beef5623344f1de08243e9ed0e48c8293aad5c67e937f006b1`  
		Last Modified: Wed, 11 Oct 2023 17:53:49 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a066414845489fe46ce720ac765d0b3b8ad3727c9c622c21223676eed2a8906`  
		Last Modified: Wed, 11 Oct 2023 17:53:49 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:3.0`

```console
$ docker pull traefik@sha256:ecd743980ec721fefff4d983f017854c18b2e8e01095c1da5aa2c977e5d55d23
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:3.0` - linux; amd64

```console
$ docker pull traefik@sha256:e65c9806dbee1c695306e888d8314fe1bb0cb4ed641fd1390ce7d6592db71bf9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.2 MB (44177073 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c559431d3551e6491ecd951a03ffbed34ad158c6a8c37361fa399d3bb9d824cf`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 28 Sep 2023 21:19:27 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Thu, 28 Sep 2023 21:19:27 GMT
CMD ["/bin/sh"]
# Fri, 29 Sep 2023 03:23:55 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 12 Oct 2023 22:42:42 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta4/traefik_v3.0.0-beta4_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 12 Oct 2023 22:42:42 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 12 Oct 2023 22:42:42 GMT
EXPOSE 80
# Thu, 12 Oct 2023 22:42:42 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 12 Oct 2023 22:42:42 GMT
CMD ["traefik"]
# Thu, 12 Oct 2023 22:42:42 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta4 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eeed05813ad6dab5b7d0156cab3e4976cd245786d76cc19071687bf8232d0683`  
		Last Modified: Fri, 29 Sep 2023 03:24:23 GMT  
		Size: 622.3 KB (622285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7da63c1e2f94cf3655890da7139b612aea1df85a9e10e85fc70427395a2e142e`  
		Last Modified: Thu, 12 Oct 2023 22:43:03 GMT  
		Size: 40.2 MB (40152453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c71a61b6f5a53b4c9e40f554b0d6e2edf1b69156bcd5a34c881578434c8902f`  
		Last Modified: Thu, 12 Oct 2023 22:42:57 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:3.0` - linux; arm variant v6

```console
$ docker pull traefik@sha256:cde351e72497d598de95a302d15c4bb703c4bce0753ec130f86b13e7855ff261
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.7 MB (41679316 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10b293ef5e3303917b1db7a28cacab688a12a46f9bf39ca87d304e08ff1f59d8`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 28 Sep 2023 20:49:16 GMT
ADD file:2222b03381ff0fce22edd647f5c60529ec6a72202f8d3cb1d6e4648ebcd19a1e in / 
# Thu, 28 Sep 2023 20:49:16 GMT
CMD ["/bin/sh"]
# Fri, 29 Sep 2023 02:07:55 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 12 Oct 2023 23:20:15 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta4/traefik_v3.0.0-beta4_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 12 Oct 2023 23:20:16 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 12 Oct 2023 23:20:16 GMT
EXPOSE 80
# Thu, 12 Oct 2023 23:20:16 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 12 Oct 2023 23:20:16 GMT
CMD ["traefik"]
# Thu, 12 Oct 2023 23:20:16 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta4 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:91cb83b91ee16f1ee0d588fccef56ab5dbb5689a64e5373caf33d7e4fe52ceb4`  
		Last Modified: Thu, 28 Sep 2023 20:51:25 GMT  
		Size: 3.1 MB (3145291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:145b6a121fb4926fc8535cfa17caa1e1cd475fcc89a18cc9ecabe5da99ff5462`  
		Last Modified: Fri, 29 Sep 2023 02:08:23 GMT  
		Size: 622.7 KB (622716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8e7cef19935c6e70917acf5c35f145ddc59f9d893c60290b5f72226a0e3d3c4`  
		Last Modified: Thu, 12 Oct 2023 23:20:37 GMT  
		Size: 37.9 MB (37910941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a73af842f798a0a1c648809b16b0bfb4f9f96ecb88b164d0d6dc29d444af157`  
		Last Modified: Thu, 12 Oct 2023 23:20:30 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:3.0` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:3083de26eab790353a8adb50cf1e2425f5a3957b55354c62df5b8b87f781ebee
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.1 MB (41118829 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:666c449e445fb3157f27a542d34acfb5fc0a26b2d72686c11a9ca242e54f904f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 28 Sep 2023 20:39:33 GMT
ADD file:ff3112828967e8004a3264d7ece3f81c88e6a1d44d360b9b5613caab15b41717 in / 
# Thu, 28 Sep 2023 20:39:34 GMT
CMD ["/bin/sh"]
# Fri, 29 Sep 2023 02:23:59 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 12 Oct 2023 22:27:17 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta4/traefik_v3.0.0-beta4_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 12 Oct 2023 22:27:17 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 12 Oct 2023 22:27:18 GMT
EXPOSE 80
# Thu, 12 Oct 2023 22:27:18 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 12 Oct 2023 22:27:18 GMT
CMD ["traefik"]
# Thu, 12 Oct 2023 22:27:18 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta4 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:579b34f0a95bb83b3acd6b3249ddc52c3d80f5c84b13c944e9e324feb86dd329`  
		Last Modified: Thu, 28 Sep 2023 20:40:08 GMT  
		Size: 3.3 MB (3331831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38b59e422640e276d23497c5544f7d98d0d1a6eed46644029a75b232afc0e4dc`  
		Last Modified: Fri, 29 Sep 2023 02:24:21 GMT  
		Size: 624.5 KB (624514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cccecd1037de20ee480b6f08472b24eb9c4993915a69e638e5943b5a205b13be`  
		Last Modified: Thu, 12 Oct 2023 22:27:36 GMT  
		Size: 37.2 MB (37162116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7c2919404f38247327ec35fae754a6dbe8c3125a35184df27c2568b51333270`  
		Last Modified: Thu, 12 Oct 2023 22:27:31 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:3.0` - linux; s390x

```console
$ docker pull traefik@sha256:79ff1827a0fe4f8236b39ea8728144a7d9ad9c20443fab8bcaaa7421d2267ca6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.0 MB (40951344 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc99842a54f239f3e13715141e6cfe726560cd79fee4167a72ff71c25219b5f2`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 28 Sep 2023 20:41:43 GMT
ADD file:fd3808a676fc56c1380e55b2ddbf4014d9371346cf789860b336bc9f00729ed0 in / 
# Thu, 28 Sep 2023 20:41:44 GMT
CMD ["/bin/sh"]
# Fri, 29 Sep 2023 00:15:10 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 29 Sep 2023 00:15:16 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta3/traefik_v3.0.0-beta3_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 29 Sep 2023 00:15:18 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 29 Sep 2023 00:15:18 GMT
EXPOSE 80
# Fri, 29 Sep 2023 00:15:18 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 29 Sep 2023 00:15:18 GMT
CMD ["traefik"]
# Fri, 29 Sep 2023 00:15:18 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta3 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:47539bffe0f44273ec7731d86be2a6171359b3847c9b60c6ac74c4875c3264af`  
		Last Modified: Thu, 28 Sep 2023 20:43:18 GMT  
		Size: 3.2 MB (3215103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37af407ac96c8e70e35ccb675ba932c1f6a441da5da4bff25fdfee4b8037205c`  
		Last Modified: Fri, 29 Sep 2023 00:15:51 GMT  
		Size: 622.8 KB (622839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2e08d6b62d3329493d6a6ead807303f1c265143bbda714fdef9382ae8c27a8d`  
		Last Modified: Fri, 29 Sep 2023 00:15:57 GMT  
		Size: 37.1 MB (37113034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b7fa0850e9af9b35eca14f9c7eaaf6b8fcc591d1c20fca9d47ecaacb3e1b314`  
		Last Modified: Fri, 29 Sep 2023 00:15:51 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:3.0-windowsservercore-1809`

```console
$ docker pull traefik@sha256:ea7055531ed953009a0e9425d7282b6430513a06f8ae8e0ab01a317180ace17e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4974; amd64

### `traefik:3.0-windowsservercore-1809` - windows version 10.0.17763.4974; amd64

```console
$ docker pull traefik@sha256:6bbe10dec34e310f581af3d2f4b1bca020b4b4d097063e77a5301e74af5a0196
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2073250916 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07c75757a6015ce6028f3f4a0dd5feb644a793030aa74cc2385d596f907b668f`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Mon, 02 Oct 2023 08:29:38 GMT
RUN Install update 10.0.17763.4974
# Wed, 11 Oct 2023 01:36:38 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 12 Oct 2023 22:54:05 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v3.0.0-beta4/traefik_v3.0.0-beta4_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Thu, 12 Oct 2023 22:54:06 GMT
EXPOSE 80
# Thu, 12 Oct 2023 22:54:07 GMT
ENTRYPOINT ["/traefik"]
# Thu, 12 Oct 2023 22:54:08 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta4 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1af2bcb37edaec1dd87fc4a6f7c9129ca37bf1f91b65eb365ba9d4c70473beea`  
		Last Modified: Tue, 10 Oct 2023 17:51:10 GMT  
		Size: 381.0 MB (380970130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0814e4a0bb8c615854a85a2b60cd043cfd20ad5a5d755acab1b30b18e4bfad3c`  
		Last Modified: Wed, 11 Oct 2023 02:46:41 GMT  
		Size: 1.3 KB (1324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e84a2fdaa00ff0a807b62824299a31186cefe7c718ff5ec7c1ba82e841bdd06a`  
		Last Modified: Thu, 12 Oct 2023 22:54:53 GMT  
		Size: 41.7 MB (41654848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b1c76c44d5bf228448de203ad236d89e22156c9847b987be33407eab8a858fb`  
		Last Modified: Thu, 12 Oct 2023 22:54:44 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f19674d9d87c8f6940731e95e09ae18c975e4adee1aac63919a490b394304a74`  
		Last Modified: Thu, 12 Oct 2023 22:54:44 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2fdb2e4268e4ef7e76c81493e498aa6848b3b5d7f56dffc399cbf07f42b5341`  
		Last Modified: Thu, 12 Oct 2023 22:54:44 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:3.0.0-beta4`

```console
$ docker pull traefik@sha256:da111b19ade88559f80eb7317f94a89e15bb80c7f3d9f53425246b4d8b901b4a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:3.0.0-beta4` - linux; amd64

```console
$ docker pull traefik@sha256:e65c9806dbee1c695306e888d8314fe1bb0cb4ed641fd1390ce7d6592db71bf9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.2 MB (44177073 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c559431d3551e6491ecd951a03ffbed34ad158c6a8c37361fa399d3bb9d824cf`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 28 Sep 2023 21:19:27 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Thu, 28 Sep 2023 21:19:27 GMT
CMD ["/bin/sh"]
# Fri, 29 Sep 2023 03:23:55 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 12 Oct 2023 22:42:42 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta4/traefik_v3.0.0-beta4_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 12 Oct 2023 22:42:42 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 12 Oct 2023 22:42:42 GMT
EXPOSE 80
# Thu, 12 Oct 2023 22:42:42 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 12 Oct 2023 22:42:42 GMT
CMD ["traefik"]
# Thu, 12 Oct 2023 22:42:42 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta4 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eeed05813ad6dab5b7d0156cab3e4976cd245786d76cc19071687bf8232d0683`  
		Last Modified: Fri, 29 Sep 2023 03:24:23 GMT  
		Size: 622.3 KB (622285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7da63c1e2f94cf3655890da7139b612aea1df85a9e10e85fc70427395a2e142e`  
		Last Modified: Thu, 12 Oct 2023 22:43:03 GMT  
		Size: 40.2 MB (40152453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c71a61b6f5a53b4c9e40f554b0d6e2edf1b69156bcd5a34c881578434c8902f`  
		Last Modified: Thu, 12 Oct 2023 22:42:57 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:3.0.0-beta4` - linux; arm variant v6

```console
$ docker pull traefik@sha256:cde351e72497d598de95a302d15c4bb703c4bce0753ec130f86b13e7855ff261
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.7 MB (41679316 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10b293ef5e3303917b1db7a28cacab688a12a46f9bf39ca87d304e08ff1f59d8`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 28 Sep 2023 20:49:16 GMT
ADD file:2222b03381ff0fce22edd647f5c60529ec6a72202f8d3cb1d6e4648ebcd19a1e in / 
# Thu, 28 Sep 2023 20:49:16 GMT
CMD ["/bin/sh"]
# Fri, 29 Sep 2023 02:07:55 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 12 Oct 2023 23:20:15 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta4/traefik_v3.0.0-beta4_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 12 Oct 2023 23:20:16 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 12 Oct 2023 23:20:16 GMT
EXPOSE 80
# Thu, 12 Oct 2023 23:20:16 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 12 Oct 2023 23:20:16 GMT
CMD ["traefik"]
# Thu, 12 Oct 2023 23:20:16 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta4 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:91cb83b91ee16f1ee0d588fccef56ab5dbb5689a64e5373caf33d7e4fe52ceb4`  
		Last Modified: Thu, 28 Sep 2023 20:51:25 GMT  
		Size: 3.1 MB (3145291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:145b6a121fb4926fc8535cfa17caa1e1cd475fcc89a18cc9ecabe5da99ff5462`  
		Last Modified: Fri, 29 Sep 2023 02:08:23 GMT  
		Size: 622.7 KB (622716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8e7cef19935c6e70917acf5c35f145ddc59f9d893c60290b5f72226a0e3d3c4`  
		Last Modified: Thu, 12 Oct 2023 23:20:37 GMT  
		Size: 37.9 MB (37910941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a73af842f798a0a1c648809b16b0bfb4f9f96ecb88b164d0d6dc29d444af157`  
		Last Modified: Thu, 12 Oct 2023 23:20:30 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:3.0.0-beta4` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:3083de26eab790353a8adb50cf1e2425f5a3957b55354c62df5b8b87f781ebee
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.1 MB (41118829 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:666c449e445fb3157f27a542d34acfb5fc0a26b2d72686c11a9ca242e54f904f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 28 Sep 2023 20:39:33 GMT
ADD file:ff3112828967e8004a3264d7ece3f81c88e6a1d44d360b9b5613caab15b41717 in / 
# Thu, 28 Sep 2023 20:39:34 GMT
CMD ["/bin/sh"]
# Fri, 29 Sep 2023 02:23:59 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 12 Oct 2023 22:27:17 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta4/traefik_v3.0.0-beta4_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 12 Oct 2023 22:27:17 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 12 Oct 2023 22:27:18 GMT
EXPOSE 80
# Thu, 12 Oct 2023 22:27:18 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 12 Oct 2023 22:27:18 GMT
CMD ["traefik"]
# Thu, 12 Oct 2023 22:27:18 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta4 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:579b34f0a95bb83b3acd6b3249ddc52c3d80f5c84b13c944e9e324feb86dd329`  
		Last Modified: Thu, 28 Sep 2023 20:40:08 GMT  
		Size: 3.3 MB (3331831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38b59e422640e276d23497c5544f7d98d0d1a6eed46644029a75b232afc0e4dc`  
		Last Modified: Fri, 29 Sep 2023 02:24:21 GMT  
		Size: 624.5 KB (624514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cccecd1037de20ee480b6f08472b24eb9c4993915a69e638e5943b5a205b13be`  
		Last Modified: Thu, 12 Oct 2023 22:27:36 GMT  
		Size: 37.2 MB (37162116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7c2919404f38247327ec35fae754a6dbe8c3125a35184df27c2568b51333270`  
		Last Modified: Thu, 12 Oct 2023 22:27:31 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:3.0.0-beta4-windowsservercore-1809`

```console
$ docker pull traefik@sha256:ea7055531ed953009a0e9425d7282b6430513a06f8ae8e0ab01a317180ace17e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4974; amd64

### `traefik:3.0.0-beta4-windowsservercore-1809` - windows version 10.0.17763.4974; amd64

```console
$ docker pull traefik@sha256:6bbe10dec34e310f581af3d2f4b1bca020b4b4d097063e77a5301e74af5a0196
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2073250916 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07c75757a6015ce6028f3f4a0dd5feb644a793030aa74cc2385d596f907b668f`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Mon, 02 Oct 2023 08:29:38 GMT
RUN Install update 10.0.17763.4974
# Wed, 11 Oct 2023 01:36:38 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 12 Oct 2023 22:54:05 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v3.0.0-beta4/traefik_v3.0.0-beta4_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Thu, 12 Oct 2023 22:54:06 GMT
EXPOSE 80
# Thu, 12 Oct 2023 22:54:07 GMT
ENTRYPOINT ["/traefik"]
# Thu, 12 Oct 2023 22:54:08 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta4 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1af2bcb37edaec1dd87fc4a6f7c9129ca37bf1f91b65eb365ba9d4c70473beea`  
		Last Modified: Tue, 10 Oct 2023 17:51:10 GMT  
		Size: 381.0 MB (380970130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0814e4a0bb8c615854a85a2b60cd043cfd20ad5a5d755acab1b30b18e4bfad3c`  
		Last Modified: Wed, 11 Oct 2023 02:46:41 GMT  
		Size: 1.3 KB (1324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e84a2fdaa00ff0a807b62824299a31186cefe7c718ff5ec7c1ba82e841bdd06a`  
		Last Modified: Thu, 12 Oct 2023 22:54:53 GMT  
		Size: 41.7 MB (41654848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b1c76c44d5bf228448de203ad236d89e22156c9847b987be33407eab8a858fb`  
		Last Modified: Thu, 12 Oct 2023 22:54:44 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f19674d9d87c8f6940731e95e09ae18c975e4adee1aac63919a490b394304a74`  
		Last Modified: Thu, 12 Oct 2023 22:54:44 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2fdb2e4268e4ef7e76c81493e498aa6848b3b5d7f56dffc399cbf07f42b5341`  
		Last Modified: Thu, 12 Oct 2023 22:54:44 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:beaufort`

```console
$ docker pull traefik@sha256:ecd743980ec721fefff4d983f017854c18b2e8e01095c1da5aa2c977e5d55d23
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:beaufort` - linux; amd64

```console
$ docker pull traefik@sha256:e65c9806dbee1c695306e888d8314fe1bb0cb4ed641fd1390ce7d6592db71bf9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.2 MB (44177073 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c559431d3551e6491ecd951a03ffbed34ad158c6a8c37361fa399d3bb9d824cf`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 28 Sep 2023 21:19:27 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Thu, 28 Sep 2023 21:19:27 GMT
CMD ["/bin/sh"]
# Fri, 29 Sep 2023 03:23:55 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 12 Oct 2023 22:42:42 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta4/traefik_v3.0.0-beta4_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 12 Oct 2023 22:42:42 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 12 Oct 2023 22:42:42 GMT
EXPOSE 80
# Thu, 12 Oct 2023 22:42:42 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 12 Oct 2023 22:42:42 GMT
CMD ["traefik"]
# Thu, 12 Oct 2023 22:42:42 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta4 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eeed05813ad6dab5b7d0156cab3e4976cd245786d76cc19071687bf8232d0683`  
		Last Modified: Fri, 29 Sep 2023 03:24:23 GMT  
		Size: 622.3 KB (622285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7da63c1e2f94cf3655890da7139b612aea1df85a9e10e85fc70427395a2e142e`  
		Last Modified: Thu, 12 Oct 2023 22:43:03 GMT  
		Size: 40.2 MB (40152453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c71a61b6f5a53b4c9e40f554b0d6e2edf1b69156bcd5a34c881578434c8902f`  
		Last Modified: Thu, 12 Oct 2023 22:42:57 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:beaufort` - linux; arm variant v6

```console
$ docker pull traefik@sha256:cde351e72497d598de95a302d15c4bb703c4bce0753ec130f86b13e7855ff261
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.7 MB (41679316 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10b293ef5e3303917b1db7a28cacab688a12a46f9bf39ca87d304e08ff1f59d8`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 28 Sep 2023 20:49:16 GMT
ADD file:2222b03381ff0fce22edd647f5c60529ec6a72202f8d3cb1d6e4648ebcd19a1e in / 
# Thu, 28 Sep 2023 20:49:16 GMT
CMD ["/bin/sh"]
# Fri, 29 Sep 2023 02:07:55 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 12 Oct 2023 23:20:15 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta4/traefik_v3.0.0-beta4_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 12 Oct 2023 23:20:16 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 12 Oct 2023 23:20:16 GMT
EXPOSE 80
# Thu, 12 Oct 2023 23:20:16 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 12 Oct 2023 23:20:16 GMT
CMD ["traefik"]
# Thu, 12 Oct 2023 23:20:16 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta4 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:91cb83b91ee16f1ee0d588fccef56ab5dbb5689a64e5373caf33d7e4fe52ceb4`  
		Last Modified: Thu, 28 Sep 2023 20:51:25 GMT  
		Size: 3.1 MB (3145291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:145b6a121fb4926fc8535cfa17caa1e1cd475fcc89a18cc9ecabe5da99ff5462`  
		Last Modified: Fri, 29 Sep 2023 02:08:23 GMT  
		Size: 622.7 KB (622716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8e7cef19935c6e70917acf5c35f145ddc59f9d893c60290b5f72226a0e3d3c4`  
		Last Modified: Thu, 12 Oct 2023 23:20:37 GMT  
		Size: 37.9 MB (37910941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a73af842f798a0a1c648809b16b0bfb4f9f96ecb88b164d0d6dc29d444af157`  
		Last Modified: Thu, 12 Oct 2023 23:20:30 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:beaufort` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:3083de26eab790353a8adb50cf1e2425f5a3957b55354c62df5b8b87f781ebee
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.1 MB (41118829 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:666c449e445fb3157f27a542d34acfb5fc0a26b2d72686c11a9ca242e54f904f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 28 Sep 2023 20:39:33 GMT
ADD file:ff3112828967e8004a3264d7ece3f81c88e6a1d44d360b9b5613caab15b41717 in / 
# Thu, 28 Sep 2023 20:39:34 GMT
CMD ["/bin/sh"]
# Fri, 29 Sep 2023 02:23:59 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 12 Oct 2023 22:27:17 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta4/traefik_v3.0.0-beta4_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 12 Oct 2023 22:27:17 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 12 Oct 2023 22:27:18 GMT
EXPOSE 80
# Thu, 12 Oct 2023 22:27:18 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 12 Oct 2023 22:27:18 GMT
CMD ["traefik"]
# Thu, 12 Oct 2023 22:27:18 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta4 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:579b34f0a95bb83b3acd6b3249ddc52c3d80f5c84b13c944e9e324feb86dd329`  
		Last Modified: Thu, 28 Sep 2023 20:40:08 GMT  
		Size: 3.3 MB (3331831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38b59e422640e276d23497c5544f7d98d0d1a6eed46644029a75b232afc0e4dc`  
		Last Modified: Fri, 29 Sep 2023 02:24:21 GMT  
		Size: 624.5 KB (624514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cccecd1037de20ee480b6f08472b24eb9c4993915a69e638e5943b5a205b13be`  
		Last Modified: Thu, 12 Oct 2023 22:27:36 GMT  
		Size: 37.2 MB (37162116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7c2919404f38247327ec35fae754a6dbe8c3125a35184df27c2568b51333270`  
		Last Modified: Thu, 12 Oct 2023 22:27:31 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:beaufort` - linux; s390x

```console
$ docker pull traefik@sha256:79ff1827a0fe4f8236b39ea8728144a7d9ad9c20443fab8bcaaa7421d2267ca6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.0 MB (40951344 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc99842a54f239f3e13715141e6cfe726560cd79fee4167a72ff71c25219b5f2`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 28 Sep 2023 20:41:43 GMT
ADD file:fd3808a676fc56c1380e55b2ddbf4014d9371346cf789860b336bc9f00729ed0 in / 
# Thu, 28 Sep 2023 20:41:44 GMT
CMD ["/bin/sh"]
# Fri, 29 Sep 2023 00:15:10 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 29 Sep 2023 00:15:16 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta3/traefik_v3.0.0-beta3_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 29 Sep 2023 00:15:18 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 29 Sep 2023 00:15:18 GMT
EXPOSE 80
# Fri, 29 Sep 2023 00:15:18 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 29 Sep 2023 00:15:18 GMT
CMD ["traefik"]
# Fri, 29 Sep 2023 00:15:18 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta3 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:47539bffe0f44273ec7731d86be2a6171359b3847c9b60c6ac74c4875c3264af`  
		Last Modified: Thu, 28 Sep 2023 20:43:18 GMT  
		Size: 3.2 MB (3215103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37af407ac96c8e70e35ccb675ba932c1f6a441da5da4bff25fdfee4b8037205c`  
		Last Modified: Fri, 29 Sep 2023 00:15:51 GMT  
		Size: 622.8 KB (622839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2e08d6b62d3329493d6a6ead807303f1c265143bbda714fdef9382ae8c27a8d`  
		Last Modified: Fri, 29 Sep 2023 00:15:57 GMT  
		Size: 37.1 MB (37113034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b7fa0850e9af9b35eca14f9c7eaaf6b8fcc591d1c20fca9d47ecaacb3e1b314`  
		Last Modified: Fri, 29 Sep 2023 00:15:51 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:beaufort-windowsservercore-1809`

```console
$ docker pull traefik@sha256:ea7055531ed953009a0e9425d7282b6430513a06f8ae8e0ab01a317180ace17e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4974; amd64

### `traefik:beaufort-windowsservercore-1809` - windows version 10.0.17763.4974; amd64

```console
$ docker pull traefik@sha256:6bbe10dec34e310f581af3d2f4b1bca020b4b4d097063e77a5301e74af5a0196
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2073250916 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07c75757a6015ce6028f3f4a0dd5feb644a793030aa74cc2385d596f907b668f`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Mon, 02 Oct 2023 08:29:38 GMT
RUN Install update 10.0.17763.4974
# Wed, 11 Oct 2023 01:36:38 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 12 Oct 2023 22:54:05 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v3.0.0-beta4/traefik_v3.0.0-beta4_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Thu, 12 Oct 2023 22:54:06 GMT
EXPOSE 80
# Thu, 12 Oct 2023 22:54:07 GMT
ENTRYPOINT ["/traefik"]
# Thu, 12 Oct 2023 22:54:08 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta4 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1af2bcb37edaec1dd87fc4a6f7c9129ca37bf1f91b65eb365ba9d4c70473beea`  
		Last Modified: Tue, 10 Oct 2023 17:51:10 GMT  
		Size: 381.0 MB (380970130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0814e4a0bb8c615854a85a2b60cd043cfd20ad5a5d755acab1b30b18e4bfad3c`  
		Last Modified: Wed, 11 Oct 2023 02:46:41 GMT  
		Size: 1.3 KB (1324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e84a2fdaa00ff0a807b62824299a31186cefe7c718ff5ec7c1ba82e841bdd06a`  
		Last Modified: Thu, 12 Oct 2023 22:54:53 GMT  
		Size: 41.7 MB (41654848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b1c76c44d5bf228448de203ad236d89e22156c9847b987be33407eab8a858fb`  
		Last Modified: Thu, 12 Oct 2023 22:54:44 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f19674d9d87c8f6940731e95e09ae18c975e4adee1aac63919a490b394304a74`  
		Last Modified: Thu, 12 Oct 2023 22:54:44 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2fdb2e4268e4ef7e76c81493e498aa6848b3b5d7f56dffc399cbf07f42b5341`  
		Last Modified: Thu, 12 Oct 2023 22:54:44 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:latest`

```console
$ docker pull traefik@sha256:948978f7ec62f137a79f8af7044a1785bd7868706ef2c8cba9c88db688d08661
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:latest` - linux; amd64

```console
$ docker pull traefik@sha256:9701f2c228e65fbaced54478b24f3953502192d396823ebdb2aa9b9e37b0e647
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.1 MB (43135183 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cc365cbb0397b708abc260501574769de3891d756c7a2e43c3839e9126cf9aec`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 28 Sep 2023 21:19:27 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Thu, 28 Sep 2023 21:19:27 GMT
CMD ["/bin/sh"]
# Fri, 29 Sep 2023 03:23:55 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 11 Oct 2023 18:19:24 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.5/traefik_v2.10.5_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 11 Oct 2023 18:19:24 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 11 Oct 2023 18:19:24 GMT
EXPOSE 80
# Wed, 11 Oct 2023 18:19:24 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 11 Oct 2023 18:19:25 GMT
CMD ["traefik"]
# Wed, 11 Oct 2023 18:19:25 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.5 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eeed05813ad6dab5b7d0156cab3e4976cd245786d76cc19071687bf8232d0683`  
		Last Modified: Fri, 29 Sep 2023 03:24:23 GMT  
		Size: 622.3 KB (622285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86ea8083d7bce4dd990c2ea838f2c04ab7fcc56a861c000ae0094825b6912661`  
		Last Modified: Wed, 11 Oct 2023 18:19:48 GMT  
		Size: 39.1 MB (39110563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cea349f5f8a775924119f640676ef0b55a652143545b75c966e52dccc0b25a3b`  
		Last Modified: Wed, 11 Oct 2023 18:19:42 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:latest` - linux; arm variant v6

```console
$ docker pull traefik@sha256:dc00301f748218be762305628990942becd6157e6e3e5cfe75a13fdd3fdb76bb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.7 MB (40720959 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4ec390e620b8982f8897b4224718a34eaf67f26bbedf3c0925701a7b61036b6`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 28 Sep 2023 20:49:16 GMT
ADD file:2222b03381ff0fce22edd647f5c60529ec6a72202f8d3cb1d6e4648ebcd19a1e in / 
# Thu, 28 Sep 2023 20:49:16 GMT
CMD ["/bin/sh"]
# Fri, 29 Sep 2023 02:07:55 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 11 Oct 2023 17:33:52 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.5/traefik_v2.10.5_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 11 Oct 2023 17:33:52 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 11 Oct 2023 17:33:52 GMT
EXPOSE 80
# Wed, 11 Oct 2023 17:33:52 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 11 Oct 2023 17:33:53 GMT
CMD ["traefik"]
# Wed, 11 Oct 2023 17:33:53 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.5 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:91cb83b91ee16f1ee0d588fccef56ab5dbb5689a64e5373caf33d7e4fe52ceb4`  
		Last Modified: Thu, 28 Sep 2023 20:51:25 GMT  
		Size: 3.1 MB (3145291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:145b6a121fb4926fc8535cfa17caa1e1cd475fcc89a18cc9ecabe5da99ff5462`  
		Last Modified: Fri, 29 Sep 2023 02:08:23 GMT  
		Size: 622.7 KB (622716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aabde1aa4d1522179691248f83aa55c1242b3d42e4523b43ecfc956b07a45441`  
		Last Modified: Wed, 11 Oct 2023 17:34:13 GMT  
		Size: 37.0 MB (36952584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f16736147d14f3ed928c692cce1e4373ddceb0416d08c37aeeda8f6ddc58f2f`  
		Last Modified: Wed, 11 Oct 2023 17:34:07 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:latest` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:4d7c60c1d882dafc8f0148231d836f7d1e2fef0d732daf1cd16f37d711afe689
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.1 MB (40122097 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1bdddb248186d54fa971abe0cc8f4e1b8a05579d6e129cef0cd8e4aace2cdec`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 28 Sep 2023 20:39:33 GMT
ADD file:ff3112828967e8004a3264d7ece3f81c88e6a1d44d360b9b5613caab15b41717 in / 
# Thu, 28 Sep 2023 20:39:34 GMT
CMD ["/bin/sh"]
# Fri, 29 Sep 2023 02:23:59 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 11 Oct 2023 18:23:41 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.5/traefik_v2.10.5_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 11 Oct 2023 18:23:41 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 11 Oct 2023 18:23:41 GMT
EXPOSE 80
# Wed, 11 Oct 2023 18:23:42 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 11 Oct 2023 18:23:42 GMT
CMD ["traefik"]
# Wed, 11 Oct 2023 18:23:42 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.5 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:579b34f0a95bb83b3acd6b3249ddc52c3d80f5c84b13c944e9e324feb86dd329`  
		Last Modified: Thu, 28 Sep 2023 20:40:08 GMT  
		Size: 3.3 MB (3331831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38b59e422640e276d23497c5544f7d98d0d1a6eed46644029a75b232afc0e4dc`  
		Last Modified: Fri, 29 Sep 2023 02:24:21 GMT  
		Size: 624.5 KB (624514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27163b2644a7f56bc248f42f0002375480295665c372ec73a52045dbd137a1a0`  
		Last Modified: Wed, 11 Oct 2023 18:24:02 GMT  
		Size: 36.2 MB (36165385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:043f01742e9c079f76aa4524a7f55f153a6d0ced946663371b8e157c333c8afa`  
		Last Modified: Wed, 11 Oct 2023 18:23:58 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:latest` - linux; s390x

```console
$ docker pull traefik@sha256:0ac60f2c2f4a9564d06dfe1b9f68d47457142d947714c6367d6e2063346c79f9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.0 MB (41958288 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7556291a63d1e75251705523cef1799f2e878e85a4cab148bbc5443b1808c259`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 28 Sep 2023 20:41:43 GMT
ADD file:fd3808a676fc56c1380e55b2ddbf4014d9371346cf789860b336bc9f00729ed0 in / 
# Thu, 28 Sep 2023 20:41:44 GMT
CMD ["/bin/sh"]
# Fri, 29 Sep 2023 00:15:10 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 11 Oct 2023 17:48:05 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.5/traefik_v2.10.5_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 11 Oct 2023 17:48:07 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 11 Oct 2023 17:48:07 GMT
EXPOSE 80
# Wed, 11 Oct 2023 17:48:07 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 11 Oct 2023 17:48:08 GMT
CMD ["traefik"]
# Wed, 11 Oct 2023 17:48:08 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.5 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:47539bffe0f44273ec7731d86be2a6171359b3847c9b60c6ac74c4875c3264af`  
		Last Modified: Thu, 28 Sep 2023 20:43:18 GMT  
		Size: 3.2 MB (3215103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37af407ac96c8e70e35ccb675ba932c1f6a441da5da4bff25fdfee4b8037205c`  
		Last Modified: Fri, 29 Sep 2023 00:15:51 GMT  
		Size: 622.8 KB (622839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fd9a3520d22d271d14445ac3488b3a3c1243ee5a36456303253061f65b58fbf`  
		Last Modified: Wed, 11 Oct 2023 17:48:39 GMT  
		Size: 38.1 MB (38119978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b98e142b7086bf0349c6782eac90d799f78fa452d198cbecd8fdfae62181704f`  
		Last Modified: Wed, 11 Oct 2023 17:48:32 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:saintmarcelin`

```console
$ docker pull traefik@sha256:948978f7ec62f137a79f8af7044a1785bd7868706ef2c8cba9c88db688d08661
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:saintmarcelin` - linux; amd64

```console
$ docker pull traefik@sha256:9701f2c228e65fbaced54478b24f3953502192d396823ebdb2aa9b9e37b0e647
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.1 MB (43135183 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cc365cbb0397b708abc260501574769de3891d756c7a2e43c3839e9126cf9aec`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 28 Sep 2023 21:19:27 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Thu, 28 Sep 2023 21:19:27 GMT
CMD ["/bin/sh"]
# Fri, 29 Sep 2023 03:23:55 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 11 Oct 2023 18:19:24 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.5/traefik_v2.10.5_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 11 Oct 2023 18:19:24 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 11 Oct 2023 18:19:24 GMT
EXPOSE 80
# Wed, 11 Oct 2023 18:19:24 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 11 Oct 2023 18:19:25 GMT
CMD ["traefik"]
# Wed, 11 Oct 2023 18:19:25 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.5 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eeed05813ad6dab5b7d0156cab3e4976cd245786d76cc19071687bf8232d0683`  
		Last Modified: Fri, 29 Sep 2023 03:24:23 GMT  
		Size: 622.3 KB (622285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86ea8083d7bce4dd990c2ea838f2c04ab7fcc56a861c000ae0094825b6912661`  
		Last Modified: Wed, 11 Oct 2023 18:19:48 GMT  
		Size: 39.1 MB (39110563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cea349f5f8a775924119f640676ef0b55a652143545b75c966e52dccc0b25a3b`  
		Last Modified: Wed, 11 Oct 2023 18:19:42 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:saintmarcelin` - linux; arm variant v6

```console
$ docker pull traefik@sha256:dc00301f748218be762305628990942becd6157e6e3e5cfe75a13fdd3fdb76bb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.7 MB (40720959 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4ec390e620b8982f8897b4224718a34eaf67f26bbedf3c0925701a7b61036b6`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 28 Sep 2023 20:49:16 GMT
ADD file:2222b03381ff0fce22edd647f5c60529ec6a72202f8d3cb1d6e4648ebcd19a1e in / 
# Thu, 28 Sep 2023 20:49:16 GMT
CMD ["/bin/sh"]
# Fri, 29 Sep 2023 02:07:55 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 11 Oct 2023 17:33:52 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.5/traefik_v2.10.5_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 11 Oct 2023 17:33:52 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 11 Oct 2023 17:33:52 GMT
EXPOSE 80
# Wed, 11 Oct 2023 17:33:52 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 11 Oct 2023 17:33:53 GMT
CMD ["traefik"]
# Wed, 11 Oct 2023 17:33:53 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.5 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:91cb83b91ee16f1ee0d588fccef56ab5dbb5689a64e5373caf33d7e4fe52ceb4`  
		Last Modified: Thu, 28 Sep 2023 20:51:25 GMT  
		Size: 3.1 MB (3145291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:145b6a121fb4926fc8535cfa17caa1e1cd475fcc89a18cc9ecabe5da99ff5462`  
		Last Modified: Fri, 29 Sep 2023 02:08:23 GMT  
		Size: 622.7 KB (622716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aabde1aa4d1522179691248f83aa55c1242b3d42e4523b43ecfc956b07a45441`  
		Last Modified: Wed, 11 Oct 2023 17:34:13 GMT  
		Size: 37.0 MB (36952584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f16736147d14f3ed928c692cce1e4373ddceb0416d08c37aeeda8f6ddc58f2f`  
		Last Modified: Wed, 11 Oct 2023 17:34:07 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:saintmarcelin` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:4d7c60c1d882dafc8f0148231d836f7d1e2fef0d732daf1cd16f37d711afe689
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.1 MB (40122097 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1bdddb248186d54fa971abe0cc8f4e1b8a05579d6e129cef0cd8e4aace2cdec`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 28 Sep 2023 20:39:33 GMT
ADD file:ff3112828967e8004a3264d7ece3f81c88e6a1d44d360b9b5613caab15b41717 in / 
# Thu, 28 Sep 2023 20:39:34 GMT
CMD ["/bin/sh"]
# Fri, 29 Sep 2023 02:23:59 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 11 Oct 2023 18:23:41 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.5/traefik_v2.10.5_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 11 Oct 2023 18:23:41 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 11 Oct 2023 18:23:41 GMT
EXPOSE 80
# Wed, 11 Oct 2023 18:23:42 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 11 Oct 2023 18:23:42 GMT
CMD ["traefik"]
# Wed, 11 Oct 2023 18:23:42 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.5 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:579b34f0a95bb83b3acd6b3249ddc52c3d80f5c84b13c944e9e324feb86dd329`  
		Last Modified: Thu, 28 Sep 2023 20:40:08 GMT  
		Size: 3.3 MB (3331831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38b59e422640e276d23497c5544f7d98d0d1a6eed46644029a75b232afc0e4dc`  
		Last Modified: Fri, 29 Sep 2023 02:24:21 GMT  
		Size: 624.5 KB (624514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27163b2644a7f56bc248f42f0002375480295665c372ec73a52045dbd137a1a0`  
		Last Modified: Wed, 11 Oct 2023 18:24:02 GMT  
		Size: 36.2 MB (36165385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:043f01742e9c079f76aa4524a7f55f153a6d0ced946663371b8e157c333c8afa`  
		Last Modified: Wed, 11 Oct 2023 18:23:58 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:saintmarcelin` - linux; s390x

```console
$ docker pull traefik@sha256:0ac60f2c2f4a9564d06dfe1b9f68d47457142d947714c6367d6e2063346c79f9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.0 MB (41958288 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7556291a63d1e75251705523cef1799f2e878e85a4cab148bbc5443b1808c259`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 28 Sep 2023 20:41:43 GMT
ADD file:fd3808a676fc56c1380e55b2ddbf4014d9371346cf789860b336bc9f00729ed0 in / 
# Thu, 28 Sep 2023 20:41:44 GMT
CMD ["/bin/sh"]
# Fri, 29 Sep 2023 00:15:10 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 11 Oct 2023 17:48:05 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.5/traefik_v2.10.5_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 11 Oct 2023 17:48:07 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 11 Oct 2023 17:48:07 GMT
EXPOSE 80
# Wed, 11 Oct 2023 17:48:07 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 11 Oct 2023 17:48:08 GMT
CMD ["traefik"]
# Wed, 11 Oct 2023 17:48:08 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.5 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:47539bffe0f44273ec7731d86be2a6171359b3847c9b60c6ac74c4875c3264af`  
		Last Modified: Thu, 28 Sep 2023 20:43:18 GMT  
		Size: 3.2 MB (3215103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37af407ac96c8e70e35ccb675ba932c1f6a441da5da4bff25fdfee4b8037205c`  
		Last Modified: Fri, 29 Sep 2023 00:15:51 GMT  
		Size: 622.8 KB (622839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fd9a3520d22d271d14445ac3488b3a3c1243ee5a36456303253061f65b58fbf`  
		Last Modified: Wed, 11 Oct 2023 17:48:39 GMT  
		Size: 38.1 MB (38119978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b98e142b7086bf0349c6782eac90d799f78fa452d198cbecd8fdfae62181704f`  
		Last Modified: Wed, 11 Oct 2023 17:48:32 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:saintmarcelin-windowsservercore-1809`

```console
$ docker pull traefik@sha256:e48ea53ba59577bef28d3ceb8dd82d512802fc92bba0ea8730217ca65bb7a400
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4974; amd64

### `traefik:saintmarcelin-windowsservercore-1809` - windows version 10.0.17763.4974; amd64

```console
$ docker pull traefik@sha256:6ddb17d74fd90ba6dd250de9179642d6b9578d6d56be82327b31f0817eb5f195
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2072188607 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:781a8b280451eba384580300e40e1a90f21b2bce4bebedde69d5c87b66476b17`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Mon, 02 Oct 2023 08:29:38 GMT
RUN Install update 10.0.17763.4974
# Wed, 11 Oct 2023 01:36:38 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Oct 2023 17:53:25 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.10.5/traefik_v2.10.5_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Wed, 11 Oct 2023 17:53:26 GMT
EXPOSE 80
# Wed, 11 Oct 2023 17:53:27 GMT
ENTRYPOINT ["/traefik"]
# Wed, 11 Oct 2023 17:53:28 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.5 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1af2bcb37edaec1dd87fc4a6f7c9129ca37bf1f91b65eb365ba9d4c70473beea`  
		Last Modified: Tue, 10 Oct 2023 17:51:10 GMT  
		Size: 381.0 MB (380970130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0814e4a0bb8c615854a85a2b60cd043cfd20ad5a5d755acab1b30b18e4bfad3c`  
		Last Modified: Wed, 11 Oct 2023 02:46:41 GMT  
		Size: 1.3 KB (1324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f15241f4df03f5eed76e4442d2b3f7a498d9144f1297714e03b04a513bddc8c`  
		Last Modified: Wed, 11 Oct 2023 17:53:58 GMT  
		Size: 40.6 MB (40592559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d40acdeea4d8136d5f835b8e319e6a7d4bc818c64267537a59a2076fb38cd0a8`  
		Last Modified: Wed, 11 Oct 2023 17:53:49 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:289c14de3f4bf9beef5623344f1de08243e9ed0e48c8293aad5c67e937f006b1`  
		Last Modified: Wed, 11 Oct 2023 17:53:49 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a066414845489fe46ce720ac765d0b3b8ad3727c9c622c21223676eed2a8906`  
		Last Modified: Wed, 11 Oct 2023 17:53:49 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.10`

```console
$ docker pull traefik@sha256:948978f7ec62f137a79f8af7044a1785bd7868706ef2c8cba9c88db688d08661
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:v2.10` - linux; amd64

```console
$ docker pull traefik@sha256:9701f2c228e65fbaced54478b24f3953502192d396823ebdb2aa9b9e37b0e647
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.1 MB (43135183 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cc365cbb0397b708abc260501574769de3891d756c7a2e43c3839e9126cf9aec`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 28 Sep 2023 21:19:27 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Thu, 28 Sep 2023 21:19:27 GMT
CMD ["/bin/sh"]
# Fri, 29 Sep 2023 03:23:55 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 11 Oct 2023 18:19:24 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.5/traefik_v2.10.5_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 11 Oct 2023 18:19:24 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 11 Oct 2023 18:19:24 GMT
EXPOSE 80
# Wed, 11 Oct 2023 18:19:24 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 11 Oct 2023 18:19:25 GMT
CMD ["traefik"]
# Wed, 11 Oct 2023 18:19:25 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.5 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eeed05813ad6dab5b7d0156cab3e4976cd245786d76cc19071687bf8232d0683`  
		Last Modified: Fri, 29 Sep 2023 03:24:23 GMT  
		Size: 622.3 KB (622285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86ea8083d7bce4dd990c2ea838f2c04ab7fcc56a861c000ae0094825b6912661`  
		Last Modified: Wed, 11 Oct 2023 18:19:48 GMT  
		Size: 39.1 MB (39110563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cea349f5f8a775924119f640676ef0b55a652143545b75c966e52dccc0b25a3b`  
		Last Modified: Wed, 11 Oct 2023 18:19:42 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.10` - linux; arm variant v6

```console
$ docker pull traefik@sha256:dc00301f748218be762305628990942becd6157e6e3e5cfe75a13fdd3fdb76bb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.7 MB (40720959 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4ec390e620b8982f8897b4224718a34eaf67f26bbedf3c0925701a7b61036b6`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 28 Sep 2023 20:49:16 GMT
ADD file:2222b03381ff0fce22edd647f5c60529ec6a72202f8d3cb1d6e4648ebcd19a1e in / 
# Thu, 28 Sep 2023 20:49:16 GMT
CMD ["/bin/sh"]
# Fri, 29 Sep 2023 02:07:55 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 11 Oct 2023 17:33:52 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.5/traefik_v2.10.5_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 11 Oct 2023 17:33:52 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 11 Oct 2023 17:33:52 GMT
EXPOSE 80
# Wed, 11 Oct 2023 17:33:52 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 11 Oct 2023 17:33:53 GMT
CMD ["traefik"]
# Wed, 11 Oct 2023 17:33:53 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.5 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:91cb83b91ee16f1ee0d588fccef56ab5dbb5689a64e5373caf33d7e4fe52ceb4`  
		Last Modified: Thu, 28 Sep 2023 20:51:25 GMT  
		Size: 3.1 MB (3145291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:145b6a121fb4926fc8535cfa17caa1e1cd475fcc89a18cc9ecabe5da99ff5462`  
		Last Modified: Fri, 29 Sep 2023 02:08:23 GMT  
		Size: 622.7 KB (622716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aabde1aa4d1522179691248f83aa55c1242b3d42e4523b43ecfc956b07a45441`  
		Last Modified: Wed, 11 Oct 2023 17:34:13 GMT  
		Size: 37.0 MB (36952584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f16736147d14f3ed928c692cce1e4373ddceb0416d08c37aeeda8f6ddc58f2f`  
		Last Modified: Wed, 11 Oct 2023 17:34:07 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.10` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:4d7c60c1d882dafc8f0148231d836f7d1e2fef0d732daf1cd16f37d711afe689
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.1 MB (40122097 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1bdddb248186d54fa971abe0cc8f4e1b8a05579d6e129cef0cd8e4aace2cdec`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 28 Sep 2023 20:39:33 GMT
ADD file:ff3112828967e8004a3264d7ece3f81c88e6a1d44d360b9b5613caab15b41717 in / 
# Thu, 28 Sep 2023 20:39:34 GMT
CMD ["/bin/sh"]
# Fri, 29 Sep 2023 02:23:59 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 11 Oct 2023 18:23:41 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.5/traefik_v2.10.5_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 11 Oct 2023 18:23:41 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 11 Oct 2023 18:23:41 GMT
EXPOSE 80
# Wed, 11 Oct 2023 18:23:42 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 11 Oct 2023 18:23:42 GMT
CMD ["traefik"]
# Wed, 11 Oct 2023 18:23:42 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.5 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:579b34f0a95bb83b3acd6b3249ddc52c3d80f5c84b13c944e9e324feb86dd329`  
		Last Modified: Thu, 28 Sep 2023 20:40:08 GMT  
		Size: 3.3 MB (3331831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38b59e422640e276d23497c5544f7d98d0d1a6eed46644029a75b232afc0e4dc`  
		Last Modified: Fri, 29 Sep 2023 02:24:21 GMT  
		Size: 624.5 KB (624514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27163b2644a7f56bc248f42f0002375480295665c372ec73a52045dbd137a1a0`  
		Last Modified: Wed, 11 Oct 2023 18:24:02 GMT  
		Size: 36.2 MB (36165385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:043f01742e9c079f76aa4524a7f55f153a6d0ced946663371b8e157c333c8afa`  
		Last Modified: Wed, 11 Oct 2023 18:23:58 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.10` - linux; s390x

```console
$ docker pull traefik@sha256:0ac60f2c2f4a9564d06dfe1b9f68d47457142d947714c6367d6e2063346c79f9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.0 MB (41958288 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7556291a63d1e75251705523cef1799f2e878e85a4cab148bbc5443b1808c259`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 28 Sep 2023 20:41:43 GMT
ADD file:fd3808a676fc56c1380e55b2ddbf4014d9371346cf789860b336bc9f00729ed0 in / 
# Thu, 28 Sep 2023 20:41:44 GMT
CMD ["/bin/sh"]
# Fri, 29 Sep 2023 00:15:10 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 11 Oct 2023 17:48:05 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.5/traefik_v2.10.5_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 11 Oct 2023 17:48:07 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 11 Oct 2023 17:48:07 GMT
EXPOSE 80
# Wed, 11 Oct 2023 17:48:07 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 11 Oct 2023 17:48:08 GMT
CMD ["traefik"]
# Wed, 11 Oct 2023 17:48:08 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.5 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:47539bffe0f44273ec7731d86be2a6171359b3847c9b60c6ac74c4875c3264af`  
		Last Modified: Thu, 28 Sep 2023 20:43:18 GMT  
		Size: 3.2 MB (3215103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37af407ac96c8e70e35ccb675ba932c1f6a441da5da4bff25fdfee4b8037205c`  
		Last Modified: Fri, 29 Sep 2023 00:15:51 GMT  
		Size: 622.8 KB (622839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fd9a3520d22d271d14445ac3488b3a3c1243ee5a36456303253061f65b58fbf`  
		Last Modified: Wed, 11 Oct 2023 17:48:39 GMT  
		Size: 38.1 MB (38119978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b98e142b7086bf0349c6782eac90d799f78fa452d198cbecd8fdfae62181704f`  
		Last Modified: Wed, 11 Oct 2023 17:48:32 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.10-windowsservercore-1809`

```console
$ docker pull traefik@sha256:e48ea53ba59577bef28d3ceb8dd82d512802fc92bba0ea8730217ca65bb7a400
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4974; amd64

### `traefik:v2.10-windowsservercore-1809` - windows version 10.0.17763.4974; amd64

```console
$ docker pull traefik@sha256:6ddb17d74fd90ba6dd250de9179642d6b9578d6d56be82327b31f0817eb5f195
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2072188607 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:781a8b280451eba384580300e40e1a90f21b2bce4bebedde69d5c87b66476b17`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Mon, 02 Oct 2023 08:29:38 GMT
RUN Install update 10.0.17763.4974
# Wed, 11 Oct 2023 01:36:38 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Oct 2023 17:53:25 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.10.5/traefik_v2.10.5_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Wed, 11 Oct 2023 17:53:26 GMT
EXPOSE 80
# Wed, 11 Oct 2023 17:53:27 GMT
ENTRYPOINT ["/traefik"]
# Wed, 11 Oct 2023 17:53:28 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.5 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1af2bcb37edaec1dd87fc4a6f7c9129ca37bf1f91b65eb365ba9d4c70473beea`  
		Last Modified: Tue, 10 Oct 2023 17:51:10 GMT  
		Size: 381.0 MB (380970130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0814e4a0bb8c615854a85a2b60cd043cfd20ad5a5d755acab1b30b18e4bfad3c`  
		Last Modified: Wed, 11 Oct 2023 02:46:41 GMT  
		Size: 1.3 KB (1324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f15241f4df03f5eed76e4442d2b3f7a498d9144f1297714e03b04a513bddc8c`  
		Last Modified: Wed, 11 Oct 2023 17:53:58 GMT  
		Size: 40.6 MB (40592559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d40acdeea4d8136d5f835b8e319e6a7d4bc818c64267537a59a2076fb38cd0a8`  
		Last Modified: Wed, 11 Oct 2023 17:53:49 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:289c14de3f4bf9beef5623344f1de08243e9ed0e48c8293aad5c67e937f006b1`  
		Last Modified: Wed, 11 Oct 2023 17:53:49 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a066414845489fe46ce720ac765d0b3b8ad3727c9c622c21223676eed2a8906`  
		Last Modified: Wed, 11 Oct 2023 17:53:49 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.10.5`

```console
$ docker pull traefik@sha256:948978f7ec62f137a79f8af7044a1785bd7868706ef2c8cba9c88db688d08661
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:v2.10.5` - linux; amd64

```console
$ docker pull traefik@sha256:9701f2c228e65fbaced54478b24f3953502192d396823ebdb2aa9b9e37b0e647
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.1 MB (43135183 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cc365cbb0397b708abc260501574769de3891d756c7a2e43c3839e9126cf9aec`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 28 Sep 2023 21:19:27 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Thu, 28 Sep 2023 21:19:27 GMT
CMD ["/bin/sh"]
# Fri, 29 Sep 2023 03:23:55 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 11 Oct 2023 18:19:24 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.5/traefik_v2.10.5_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 11 Oct 2023 18:19:24 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 11 Oct 2023 18:19:24 GMT
EXPOSE 80
# Wed, 11 Oct 2023 18:19:24 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 11 Oct 2023 18:19:25 GMT
CMD ["traefik"]
# Wed, 11 Oct 2023 18:19:25 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.5 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eeed05813ad6dab5b7d0156cab3e4976cd245786d76cc19071687bf8232d0683`  
		Last Modified: Fri, 29 Sep 2023 03:24:23 GMT  
		Size: 622.3 KB (622285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86ea8083d7bce4dd990c2ea838f2c04ab7fcc56a861c000ae0094825b6912661`  
		Last Modified: Wed, 11 Oct 2023 18:19:48 GMT  
		Size: 39.1 MB (39110563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cea349f5f8a775924119f640676ef0b55a652143545b75c966e52dccc0b25a3b`  
		Last Modified: Wed, 11 Oct 2023 18:19:42 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.10.5` - linux; arm variant v6

```console
$ docker pull traefik@sha256:dc00301f748218be762305628990942becd6157e6e3e5cfe75a13fdd3fdb76bb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.7 MB (40720959 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4ec390e620b8982f8897b4224718a34eaf67f26bbedf3c0925701a7b61036b6`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 28 Sep 2023 20:49:16 GMT
ADD file:2222b03381ff0fce22edd647f5c60529ec6a72202f8d3cb1d6e4648ebcd19a1e in / 
# Thu, 28 Sep 2023 20:49:16 GMT
CMD ["/bin/sh"]
# Fri, 29 Sep 2023 02:07:55 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 11 Oct 2023 17:33:52 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.5/traefik_v2.10.5_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 11 Oct 2023 17:33:52 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 11 Oct 2023 17:33:52 GMT
EXPOSE 80
# Wed, 11 Oct 2023 17:33:52 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 11 Oct 2023 17:33:53 GMT
CMD ["traefik"]
# Wed, 11 Oct 2023 17:33:53 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.5 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:91cb83b91ee16f1ee0d588fccef56ab5dbb5689a64e5373caf33d7e4fe52ceb4`  
		Last Modified: Thu, 28 Sep 2023 20:51:25 GMT  
		Size: 3.1 MB (3145291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:145b6a121fb4926fc8535cfa17caa1e1cd475fcc89a18cc9ecabe5da99ff5462`  
		Last Modified: Fri, 29 Sep 2023 02:08:23 GMT  
		Size: 622.7 KB (622716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aabde1aa4d1522179691248f83aa55c1242b3d42e4523b43ecfc956b07a45441`  
		Last Modified: Wed, 11 Oct 2023 17:34:13 GMT  
		Size: 37.0 MB (36952584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f16736147d14f3ed928c692cce1e4373ddceb0416d08c37aeeda8f6ddc58f2f`  
		Last Modified: Wed, 11 Oct 2023 17:34:07 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.10.5` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:4d7c60c1d882dafc8f0148231d836f7d1e2fef0d732daf1cd16f37d711afe689
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.1 MB (40122097 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1bdddb248186d54fa971abe0cc8f4e1b8a05579d6e129cef0cd8e4aace2cdec`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 28 Sep 2023 20:39:33 GMT
ADD file:ff3112828967e8004a3264d7ece3f81c88e6a1d44d360b9b5613caab15b41717 in / 
# Thu, 28 Sep 2023 20:39:34 GMT
CMD ["/bin/sh"]
# Fri, 29 Sep 2023 02:23:59 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 11 Oct 2023 18:23:41 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.5/traefik_v2.10.5_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 11 Oct 2023 18:23:41 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 11 Oct 2023 18:23:41 GMT
EXPOSE 80
# Wed, 11 Oct 2023 18:23:42 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 11 Oct 2023 18:23:42 GMT
CMD ["traefik"]
# Wed, 11 Oct 2023 18:23:42 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.5 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:579b34f0a95bb83b3acd6b3249ddc52c3d80f5c84b13c944e9e324feb86dd329`  
		Last Modified: Thu, 28 Sep 2023 20:40:08 GMT  
		Size: 3.3 MB (3331831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38b59e422640e276d23497c5544f7d98d0d1a6eed46644029a75b232afc0e4dc`  
		Last Modified: Fri, 29 Sep 2023 02:24:21 GMT  
		Size: 624.5 KB (624514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27163b2644a7f56bc248f42f0002375480295665c372ec73a52045dbd137a1a0`  
		Last Modified: Wed, 11 Oct 2023 18:24:02 GMT  
		Size: 36.2 MB (36165385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:043f01742e9c079f76aa4524a7f55f153a6d0ced946663371b8e157c333c8afa`  
		Last Modified: Wed, 11 Oct 2023 18:23:58 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.10.5` - linux; s390x

```console
$ docker pull traefik@sha256:0ac60f2c2f4a9564d06dfe1b9f68d47457142d947714c6367d6e2063346c79f9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.0 MB (41958288 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7556291a63d1e75251705523cef1799f2e878e85a4cab148bbc5443b1808c259`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 28 Sep 2023 20:41:43 GMT
ADD file:fd3808a676fc56c1380e55b2ddbf4014d9371346cf789860b336bc9f00729ed0 in / 
# Thu, 28 Sep 2023 20:41:44 GMT
CMD ["/bin/sh"]
# Fri, 29 Sep 2023 00:15:10 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 11 Oct 2023 17:48:05 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.5/traefik_v2.10.5_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 11 Oct 2023 17:48:07 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 11 Oct 2023 17:48:07 GMT
EXPOSE 80
# Wed, 11 Oct 2023 17:48:07 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 11 Oct 2023 17:48:08 GMT
CMD ["traefik"]
# Wed, 11 Oct 2023 17:48:08 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.5 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:47539bffe0f44273ec7731d86be2a6171359b3847c9b60c6ac74c4875c3264af`  
		Last Modified: Thu, 28 Sep 2023 20:43:18 GMT  
		Size: 3.2 MB (3215103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37af407ac96c8e70e35ccb675ba932c1f6a441da5da4bff25fdfee4b8037205c`  
		Last Modified: Fri, 29 Sep 2023 00:15:51 GMT  
		Size: 622.8 KB (622839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fd9a3520d22d271d14445ac3488b3a3c1243ee5a36456303253061f65b58fbf`  
		Last Modified: Wed, 11 Oct 2023 17:48:39 GMT  
		Size: 38.1 MB (38119978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b98e142b7086bf0349c6782eac90d799f78fa452d198cbecd8fdfae62181704f`  
		Last Modified: Wed, 11 Oct 2023 17:48:32 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.10.5-windowsservercore-1809`

```console
$ docker pull traefik@sha256:e48ea53ba59577bef28d3ceb8dd82d512802fc92bba0ea8730217ca65bb7a400
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4974; amd64

### `traefik:v2.10.5-windowsservercore-1809` - windows version 10.0.17763.4974; amd64

```console
$ docker pull traefik@sha256:6ddb17d74fd90ba6dd250de9179642d6b9578d6d56be82327b31f0817eb5f195
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2072188607 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:781a8b280451eba384580300e40e1a90f21b2bce4bebedde69d5c87b66476b17`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Mon, 02 Oct 2023 08:29:38 GMT
RUN Install update 10.0.17763.4974
# Wed, 11 Oct 2023 01:36:38 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Oct 2023 17:53:25 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.10.5/traefik_v2.10.5_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Wed, 11 Oct 2023 17:53:26 GMT
EXPOSE 80
# Wed, 11 Oct 2023 17:53:27 GMT
ENTRYPOINT ["/traefik"]
# Wed, 11 Oct 2023 17:53:28 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.5 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1af2bcb37edaec1dd87fc4a6f7c9129ca37bf1f91b65eb365ba9d4c70473beea`  
		Last Modified: Tue, 10 Oct 2023 17:51:10 GMT  
		Size: 381.0 MB (380970130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0814e4a0bb8c615854a85a2b60cd043cfd20ad5a5d755acab1b30b18e4bfad3c`  
		Last Modified: Wed, 11 Oct 2023 02:46:41 GMT  
		Size: 1.3 KB (1324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f15241f4df03f5eed76e4442d2b3f7a498d9144f1297714e03b04a513bddc8c`  
		Last Modified: Wed, 11 Oct 2023 17:53:58 GMT  
		Size: 40.6 MB (40592559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d40acdeea4d8136d5f835b8e319e6a7d4bc818c64267537a59a2076fb38cd0a8`  
		Last Modified: Wed, 11 Oct 2023 17:53:49 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:289c14de3f4bf9beef5623344f1de08243e9ed0e48c8293aad5c67e937f006b1`  
		Last Modified: Wed, 11 Oct 2023 17:53:49 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a066414845489fe46ce720ac765d0b3b8ad3727c9c622c21223676eed2a8906`  
		Last Modified: Wed, 11 Oct 2023 17:53:49 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v3.0`

```console
$ docker pull traefik@sha256:ecd743980ec721fefff4d983f017854c18b2e8e01095c1da5aa2c977e5d55d23
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:v3.0` - linux; amd64

```console
$ docker pull traefik@sha256:e65c9806dbee1c695306e888d8314fe1bb0cb4ed641fd1390ce7d6592db71bf9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.2 MB (44177073 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c559431d3551e6491ecd951a03ffbed34ad158c6a8c37361fa399d3bb9d824cf`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 28 Sep 2023 21:19:27 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Thu, 28 Sep 2023 21:19:27 GMT
CMD ["/bin/sh"]
# Fri, 29 Sep 2023 03:23:55 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 12 Oct 2023 22:42:42 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta4/traefik_v3.0.0-beta4_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 12 Oct 2023 22:42:42 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 12 Oct 2023 22:42:42 GMT
EXPOSE 80
# Thu, 12 Oct 2023 22:42:42 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 12 Oct 2023 22:42:42 GMT
CMD ["traefik"]
# Thu, 12 Oct 2023 22:42:42 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta4 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eeed05813ad6dab5b7d0156cab3e4976cd245786d76cc19071687bf8232d0683`  
		Last Modified: Fri, 29 Sep 2023 03:24:23 GMT  
		Size: 622.3 KB (622285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7da63c1e2f94cf3655890da7139b612aea1df85a9e10e85fc70427395a2e142e`  
		Last Modified: Thu, 12 Oct 2023 22:43:03 GMT  
		Size: 40.2 MB (40152453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c71a61b6f5a53b4c9e40f554b0d6e2edf1b69156bcd5a34c881578434c8902f`  
		Last Modified: Thu, 12 Oct 2023 22:42:57 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v3.0` - linux; arm variant v6

```console
$ docker pull traefik@sha256:cde351e72497d598de95a302d15c4bb703c4bce0753ec130f86b13e7855ff261
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.7 MB (41679316 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10b293ef5e3303917b1db7a28cacab688a12a46f9bf39ca87d304e08ff1f59d8`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 28 Sep 2023 20:49:16 GMT
ADD file:2222b03381ff0fce22edd647f5c60529ec6a72202f8d3cb1d6e4648ebcd19a1e in / 
# Thu, 28 Sep 2023 20:49:16 GMT
CMD ["/bin/sh"]
# Fri, 29 Sep 2023 02:07:55 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 12 Oct 2023 23:20:15 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta4/traefik_v3.0.0-beta4_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 12 Oct 2023 23:20:16 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 12 Oct 2023 23:20:16 GMT
EXPOSE 80
# Thu, 12 Oct 2023 23:20:16 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 12 Oct 2023 23:20:16 GMT
CMD ["traefik"]
# Thu, 12 Oct 2023 23:20:16 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta4 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:91cb83b91ee16f1ee0d588fccef56ab5dbb5689a64e5373caf33d7e4fe52ceb4`  
		Last Modified: Thu, 28 Sep 2023 20:51:25 GMT  
		Size: 3.1 MB (3145291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:145b6a121fb4926fc8535cfa17caa1e1cd475fcc89a18cc9ecabe5da99ff5462`  
		Last Modified: Fri, 29 Sep 2023 02:08:23 GMT  
		Size: 622.7 KB (622716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8e7cef19935c6e70917acf5c35f145ddc59f9d893c60290b5f72226a0e3d3c4`  
		Last Modified: Thu, 12 Oct 2023 23:20:37 GMT  
		Size: 37.9 MB (37910941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a73af842f798a0a1c648809b16b0bfb4f9f96ecb88b164d0d6dc29d444af157`  
		Last Modified: Thu, 12 Oct 2023 23:20:30 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v3.0` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:3083de26eab790353a8adb50cf1e2425f5a3957b55354c62df5b8b87f781ebee
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.1 MB (41118829 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:666c449e445fb3157f27a542d34acfb5fc0a26b2d72686c11a9ca242e54f904f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 28 Sep 2023 20:39:33 GMT
ADD file:ff3112828967e8004a3264d7ece3f81c88e6a1d44d360b9b5613caab15b41717 in / 
# Thu, 28 Sep 2023 20:39:34 GMT
CMD ["/bin/sh"]
# Fri, 29 Sep 2023 02:23:59 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 12 Oct 2023 22:27:17 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta4/traefik_v3.0.0-beta4_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 12 Oct 2023 22:27:17 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 12 Oct 2023 22:27:18 GMT
EXPOSE 80
# Thu, 12 Oct 2023 22:27:18 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 12 Oct 2023 22:27:18 GMT
CMD ["traefik"]
# Thu, 12 Oct 2023 22:27:18 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta4 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:579b34f0a95bb83b3acd6b3249ddc52c3d80f5c84b13c944e9e324feb86dd329`  
		Last Modified: Thu, 28 Sep 2023 20:40:08 GMT  
		Size: 3.3 MB (3331831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38b59e422640e276d23497c5544f7d98d0d1a6eed46644029a75b232afc0e4dc`  
		Last Modified: Fri, 29 Sep 2023 02:24:21 GMT  
		Size: 624.5 KB (624514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cccecd1037de20ee480b6f08472b24eb9c4993915a69e638e5943b5a205b13be`  
		Last Modified: Thu, 12 Oct 2023 22:27:36 GMT  
		Size: 37.2 MB (37162116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7c2919404f38247327ec35fae754a6dbe8c3125a35184df27c2568b51333270`  
		Last Modified: Thu, 12 Oct 2023 22:27:31 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v3.0` - linux; s390x

```console
$ docker pull traefik@sha256:79ff1827a0fe4f8236b39ea8728144a7d9ad9c20443fab8bcaaa7421d2267ca6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.0 MB (40951344 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc99842a54f239f3e13715141e6cfe726560cd79fee4167a72ff71c25219b5f2`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 28 Sep 2023 20:41:43 GMT
ADD file:fd3808a676fc56c1380e55b2ddbf4014d9371346cf789860b336bc9f00729ed0 in / 
# Thu, 28 Sep 2023 20:41:44 GMT
CMD ["/bin/sh"]
# Fri, 29 Sep 2023 00:15:10 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 29 Sep 2023 00:15:16 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta3/traefik_v3.0.0-beta3_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 29 Sep 2023 00:15:18 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 29 Sep 2023 00:15:18 GMT
EXPOSE 80
# Fri, 29 Sep 2023 00:15:18 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 29 Sep 2023 00:15:18 GMT
CMD ["traefik"]
# Fri, 29 Sep 2023 00:15:18 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta3 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:47539bffe0f44273ec7731d86be2a6171359b3847c9b60c6ac74c4875c3264af`  
		Last Modified: Thu, 28 Sep 2023 20:43:18 GMT  
		Size: 3.2 MB (3215103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37af407ac96c8e70e35ccb675ba932c1f6a441da5da4bff25fdfee4b8037205c`  
		Last Modified: Fri, 29 Sep 2023 00:15:51 GMT  
		Size: 622.8 KB (622839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2e08d6b62d3329493d6a6ead807303f1c265143bbda714fdef9382ae8c27a8d`  
		Last Modified: Fri, 29 Sep 2023 00:15:57 GMT  
		Size: 37.1 MB (37113034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b7fa0850e9af9b35eca14f9c7eaaf6b8fcc591d1c20fca9d47ecaacb3e1b314`  
		Last Modified: Fri, 29 Sep 2023 00:15:51 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v3.0-windowsservercore-1809`

```console
$ docker pull traefik@sha256:ea7055531ed953009a0e9425d7282b6430513a06f8ae8e0ab01a317180ace17e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4974; amd64

### `traefik:v3.0-windowsservercore-1809` - windows version 10.0.17763.4974; amd64

```console
$ docker pull traefik@sha256:6bbe10dec34e310f581af3d2f4b1bca020b4b4d097063e77a5301e74af5a0196
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2073250916 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07c75757a6015ce6028f3f4a0dd5feb644a793030aa74cc2385d596f907b668f`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Mon, 02 Oct 2023 08:29:38 GMT
RUN Install update 10.0.17763.4974
# Wed, 11 Oct 2023 01:36:38 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 12 Oct 2023 22:54:05 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v3.0.0-beta4/traefik_v3.0.0-beta4_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Thu, 12 Oct 2023 22:54:06 GMT
EXPOSE 80
# Thu, 12 Oct 2023 22:54:07 GMT
ENTRYPOINT ["/traefik"]
# Thu, 12 Oct 2023 22:54:08 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta4 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1af2bcb37edaec1dd87fc4a6f7c9129ca37bf1f91b65eb365ba9d4c70473beea`  
		Last Modified: Tue, 10 Oct 2023 17:51:10 GMT  
		Size: 381.0 MB (380970130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0814e4a0bb8c615854a85a2b60cd043cfd20ad5a5d755acab1b30b18e4bfad3c`  
		Last Modified: Wed, 11 Oct 2023 02:46:41 GMT  
		Size: 1.3 KB (1324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e84a2fdaa00ff0a807b62824299a31186cefe7c718ff5ec7c1ba82e841bdd06a`  
		Last Modified: Thu, 12 Oct 2023 22:54:53 GMT  
		Size: 41.7 MB (41654848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b1c76c44d5bf228448de203ad236d89e22156c9847b987be33407eab8a858fb`  
		Last Modified: Thu, 12 Oct 2023 22:54:44 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f19674d9d87c8f6940731e95e09ae18c975e4adee1aac63919a490b394304a74`  
		Last Modified: Thu, 12 Oct 2023 22:54:44 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2fdb2e4268e4ef7e76c81493e498aa6848b3b5d7f56dffc399cbf07f42b5341`  
		Last Modified: Thu, 12 Oct 2023 22:54:44 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v3.0.0-beta4`

```console
$ docker pull traefik@sha256:da111b19ade88559f80eb7317f94a89e15bb80c7f3d9f53425246b4d8b901b4a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:v3.0.0-beta4` - linux; amd64

```console
$ docker pull traefik@sha256:e65c9806dbee1c695306e888d8314fe1bb0cb4ed641fd1390ce7d6592db71bf9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.2 MB (44177073 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c559431d3551e6491ecd951a03ffbed34ad158c6a8c37361fa399d3bb9d824cf`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 28 Sep 2023 21:19:27 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Thu, 28 Sep 2023 21:19:27 GMT
CMD ["/bin/sh"]
# Fri, 29 Sep 2023 03:23:55 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 12 Oct 2023 22:42:42 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta4/traefik_v3.0.0-beta4_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 12 Oct 2023 22:42:42 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 12 Oct 2023 22:42:42 GMT
EXPOSE 80
# Thu, 12 Oct 2023 22:42:42 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 12 Oct 2023 22:42:42 GMT
CMD ["traefik"]
# Thu, 12 Oct 2023 22:42:42 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta4 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eeed05813ad6dab5b7d0156cab3e4976cd245786d76cc19071687bf8232d0683`  
		Last Modified: Fri, 29 Sep 2023 03:24:23 GMT  
		Size: 622.3 KB (622285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7da63c1e2f94cf3655890da7139b612aea1df85a9e10e85fc70427395a2e142e`  
		Last Modified: Thu, 12 Oct 2023 22:43:03 GMT  
		Size: 40.2 MB (40152453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c71a61b6f5a53b4c9e40f554b0d6e2edf1b69156bcd5a34c881578434c8902f`  
		Last Modified: Thu, 12 Oct 2023 22:42:57 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v3.0.0-beta4` - linux; arm variant v6

```console
$ docker pull traefik@sha256:cde351e72497d598de95a302d15c4bb703c4bce0753ec130f86b13e7855ff261
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.7 MB (41679316 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10b293ef5e3303917b1db7a28cacab688a12a46f9bf39ca87d304e08ff1f59d8`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 28 Sep 2023 20:49:16 GMT
ADD file:2222b03381ff0fce22edd647f5c60529ec6a72202f8d3cb1d6e4648ebcd19a1e in / 
# Thu, 28 Sep 2023 20:49:16 GMT
CMD ["/bin/sh"]
# Fri, 29 Sep 2023 02:07:55 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 12 Oct 2023 23:20:15 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta4/traefik_v3.0.0-beta4_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 12 Oct 2023 23:20:16 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 12 Oct 2023 23:20:16 GMT
EXPOSE 80
# Thu, 12 Oct 2023 23:20:16 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 12 Oct 2023 23:20:16 GMT
CMD ["traefik"]
# Thu, 12 Oct 2023 23:20:16 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta4 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:91cb83b91ee16f1ee0d588fccef56ab5dbb5689a64e5373caf33d7e4fe52ceb4`  
		Last Modified: Thu, 28 Sep 2023 20:51:25 GMT  
		Size: 3.1 MB (3145291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:145b6a121fb4926fc8535cfa17caa1e1cd475fcc89a18cc9ecabe5da99ff5462`  
		Last Modified: Fri, 29 Sep 2023 02:08:23 GMT  
		Size: 622.7 KB (622716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8e7cef19935c6e70917acf5c35f145ddc59f9d893c60290b5f72226a0e3d3c4`  
		Last Modified: Thu, 12 Oct 2023 23:20:37 GMT  
		Size: 37.9 MB (37910941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a73af842f798a0a1c648809b16b0bfb4f9f96ecb88b164d0d6dc29d444af157`  
		Last Modified: Thu, 12 Oct 2023 23:20:30 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v3.0.0-beta4` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:3083de26eab790353a8adb50cf1e2425f5a3957b55354c62df5b8b87f781ebee
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.1 MB (41118829 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:666c449e445fb3157f27a542d34acfb5fc0a26b2d72686c11a9ca242e54f904f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 28 Sep 2023 20:39:33 GMT
ADD file:ff3112828967e8004a3264d7ece3f81c88e6a1d44d360b9b5613caab15b41717 in / 
# Thu, 28 Sep 2023 20:39:34 GMT
CMD ["/bin/sh"]
# Fri, 29 Sep 2023 02:23:59 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 12 Oct 2023 22:27:17 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta4/traefik_v3.0.0-beta4_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 12 Oct 2023 22:27:17 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 12 Oct 2023 22:27:18 GMT
EXPOSE 80
# Thu, 12 Oct 2023 22:27:18 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 12 Oct 2023 22:27:18 GMT
CMD ["traefik"]
# Thu, 12 Oct 2023 22:27:18 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta4 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:579b34f0a95bb83b3acd6b3249ddc52c3d80f5c84b13c944e9e324feb86dd329`  
		Last Modified: Thu, 28 Sep 2023 20:40:08 GMT  
		Size: 3.3 MB (3331831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38b59e422640e276d23497c5544f7d98d0d1a6eed46644029a75b232afc0e4dc`  
		Last Modified: Fri, 29 Sep 2023 02:24:21 GMT  
		Size: 624.5 KB (624514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cccecd1037de20ee480b6f08472b24eb9c4993915a69e638e5943b5a205b13be`  
		Last Modified: Thu, 12 Oct 2023 22:27:36 GMT  
		Size: 37.2 MB (37162116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7c2919404f38247327ec35fae754a6dbe8c3125a35184df27c2568b51333270`  
		Last Modified: Thu, 12 Oct 2023 22:27:31 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v3.0.0-beta4-windowsservercore-1809`

```console
$ docker pull traefik@sha256:ea7055531ed953009a0e9425d7282b6430513a06f8ae8e0ab01a317180ace17e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4974; amd64

### `traefik:v3.0.0-beta4-windowsservercore-1809` - windows version 10.0.17763.4974; amd64

```console
$ docker pull traefik@sha256:6bbe10dec34e310f581af3d2f4b1bca020b4b4d097063e77a5301e74af5a0196
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2073250916 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07c75757a6015ce6028f3f4a0dd5feb644a793030aa74cc2385d596f907b668f`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Mon, 02 Oct 2023 08:29:38 GMT
RUN Install update 10.0.17763.4974
# Wed, 11 Oct 2023 01:36:38 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 12 Oct 2023 22:54:05 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v3.0.0-beta4/traefik_v3.0.0-beta4_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Thu, 12 Oct 2023 22:54:06 GMT
EXPOSE 80
# Thu, 12 Oct 2023 22:54:07 GMT
ENTRYPOINT ["/traefik"]
# Thu, 12 Oct 2023 22:54:08 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta4 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1af2bcb37edaec1dd87fc4a6f7c9129ca37bf1f91b65eb365ba9d4c70473beea`  
		Last Modified: Tue, 10 Oct 2023 17:51:10 GMT  
		Size: 381.0 MB (380970130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0814e4a0bb8c615854a85a2b60cd043cfd20ad5a5d755acab1b30b18e4bfad3c`  
		Last Modified: Wed, 11 Oct 2023 02:46:41 GMT  
		Size: 1.3 KB (1324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e84a2fdaa00ff0a807b62824299a31186cefe7c718ff5ec7c1ba82e841bdd06a`  
		Last Modified: Thu, 12 Oct 2023 22:54:53 GMT  
		Size: 41.7 MB (41654848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b1c76c44d5bf228448de203ad236d89e22156c9847b987be33407eab8a858fb`  
		Last Modified: Thu, 12 Oct 2023 22:54:44 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f19674d9d87c8f6940731e95e09ae18c975e4adee1aac63919a490b394304a74`  
		Last Modified: Thu, 12 Oct 2023 22:54:44 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2fdb2e4268e4ef7e76c81493e498aa6848b3b5d7f56dffc399cbf07f42b5341`  
		Last Modified: Thu, 12 Oct 2023 22:54:44 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:windowsservercore-1809`

```console
$ docker pull traefik@sha256:e48ea53ba59577bef28d3ceb8dd82d512802fc92bba0ea8730217ca65bb7a400
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4974; amd64

### `traefik:windowsservercore-1809` - windows version 10.0.17763.4974; amd64

```console
$ docker pull traefik@sha256:6ddb17d74fd90ba6dd250de9179642d6b9578d6d56be82327b31f0817eb5f195
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2072188607 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:781a8b280451eba384580300e40e1a90f21b2bce4bebedde69d5c87b66476b17`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Mon, 02 Oct 2023 08:29:38 GMT
RUN Install update 10.0.17763.4974
# Wed, 11 Oct 2023 01:36:38 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Oct 2023 17:53:25 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.10.5/traefik_v2.10.5_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Wed, 11 Oct 2023 17:53:26 GMT
EXPOSE 80
# Wed, 11 Oct 2023 17:53:27 GMT
ENTRYPOINT ["/traefik"]
# Wed, 11 Oct 2023 17:53:28 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.5 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1af2bcb37edaec1dd87fc4a6f7c9129ca37bf1f91b65eb365ba9d4c70473beea`  
		Last Modified: Tue, 10 Oct 2023 17:51:10 GMT  
		Size: 381.0 MB (380970130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0814e4a0bb8c615854a85a2b60cd043cfd20ad5a5d755acab1b30b18e4bfad3c`  
		Last Modified: Wed, 11 Oct 2023 02:46:41 GMT  
		Size: 1.3 KB (1324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f15241f4df03f5eed76e4442d2b3f7a498d9144f1297714e03b04a513bddc8c`  
		Last Modified: Wed, 11 Oct 2023 17:53:58 GMT  
		Size: 40.6 MB (40592559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d40acdeea4d8136d5f835b8e319e6a7d4bc818c64267537a59a2076fb38cd0a8`  
		Last Modified: Wed, 11 Oct 2023 17:53:49 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:289c14de3f4bf9beef5623344f1de08243e9ed0e48c8293aad5c67e937f006b1`  
		Last Modified: Wed, 11 Oct 2023 17:53:49 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a066414845489fe46ce720ac765d0b3b8ad3727c9c622c21223676eed2a8906`  
		Last Modified: Wed, 11 Oct 2023 17:53:49 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
