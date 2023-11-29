<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `traefik`

-	[`traefik:2.10`](#traefik210)
-	[`traefik:2.10-windowsservercore-1809`](#traefik210-windowsservercore-1809)
-	[`traefik:2.10.6`](#traefik2106)
-	[`traefik:2.10.6-windowsservercore-1809`](#traefik2106-windowsservercore-1809)
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
-	[`traefik:v2.10.6`](#traefikv2106)
-	[`traefik:v2.10.6-windowsservercore-1809`](#traefikv2106-windowsservercore-1809)
-	[`traefik:v3.0`](#traefikv30)
-	[`traefik:v3.0-windowsservercore-1809`](#traefikv30-windowsservercore-1809)
-	[`traefik:v3.0.0-beta4`](#traefikv300-beta4)
-	[`traefik:v3.0.0-beta4-windowsservercore-1809`](#traefikv300-beta4-windowsservercore-1809)
-	[`traefik:windowsservercore-1809`](#traefikwindowsservercore-1809)

## `traefik:2.10`

```console
$ docker pull traefik@sha256:8b507326e4cf156eb56057f0019b3919520add3867e126cbc24914acbc0cb653
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
$ docker pull traefik@sha256:1f73a129ceb164fcee414c47e2eeb8166b950ef30728bb86a4142d2fcba75360
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.1 MB (42050681 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:43753aaf21fdf5d7a44475c270504fe5cd018c9a10995cc3bc63defd17ed8661`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 28 Sep 2023 20:41:43 GMT
ADD file:fd3808a676fc56c1380e55b2ddbf4014d9371346cf789860b336bc9f00729ed0 in / 
# Thu, 28 Sep 2023 20:41:44 GMT
CMD ["/bin/sh"]
# Wed, 29 Nov 2023 00:45:49 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 29 Nov 2023 00:46:23 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.6/traefik_v2.10.6_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 29 Nov 2023 00:46:29 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 29 Nov 2023 00:46:30 GMT
EXPOSE 80
# Wed, 29 Nov 2023 00:46:30 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 29 Nov 2023 00:46:30 GMT
CMD ["traefik"]
# Wed, 29 Nov 2023 00:46:30 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.6 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:47539bffe0f44273ec7731d86be2a6171359b3847c9b60c6ac74c4875c3264af`  
		Last Modified: Thu, 28 Sep 2023 20:43:18 GMT  
		Size: 3.2 MB (3215103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef466f0f3a71ca493d3026cd1c1e85592db97303a55121345c9626424dd0d941`  
		Last Modified: Wed, 29 Nov 2023 00:47:25 GMT  
		Size: 622.8 KB (622844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a0bf7a3ef99bf94af2497d00978f85d1009602ec9ec764aa643647e5e5bc653`  
		Last Modified: Wed, 29 Nov 2023 00:47:50 GMT  
		Size: 38.2 MB (38212366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1bd88c0a01deb2371f3822ce3181d55c12b4f33668758d93f9de2a85e812fe4`  
		Last Modified: Wed, 29 Nov 2023 00:47:44 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:2.10-windowsservercore-1809`

```console
$ docker pull traefik@sha256:0171555d49032d3e9a8143f92d75bb773bd1d02d0c6ab5c1ce038e1b9d8a97fb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.5122; amd64

### `traefik:2.10-windowsservercore-1809` - windows version 10.0.17763.5122; amd64

```console
$ docker pull traefik@sha256:7d9e986b167fd6a6e8caf0d270cff4848f68e67d615789d5072359dfaae4658c
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2098008476 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fef5097a6081d1124f5e62b4a0cb1e6f2798c0be3bf4b2ac534172dac2e4aa73`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Thu, 09 Nov 2023 17:56:40 GMT
RUN Install update 10.0.17763.5122
# Thu, 16 Nov 2023 01:37:58 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Nov 2023 08:34:25 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.10.5/traefik_v2.10.5_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Thu, 16 Nov 2023 08:34:26 GMT
EXPOSE 80
# Thu, 16 Nov 2023 08:34:27 GMT
ENTRYPOINT ["/traefik"]
# Thu, 16 Nov 2023 08:34:28 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.5 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f7bb9e009deb881cb90e8b4318258e03882de9bc9b312b763654b59cd13d0bb`  
		Last Modified: Tue, 14 Nov 2023 19:53:30 GMT  
		Size: 406.8 MB (406811201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce7a1cc914f0f5e059bfdf02906a6e052b1c97cebaf91eb6c2fd835cfddebda2`  
		Last Modified: Thu, 16 Nov 2023 02:26:46 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5364859be3494bde67293ec5e752ce6710eb84de075e56586e9dc1a05b9a4953`  
		Last Modified: Thu, 16 Nov 2023 08:35:34 GMT  
		Size: 40.6 MB (40571250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd8773eae2563ee25a1f20ece298456e74f874c3ae705b5516b5f0c51fb4df1a`  
		Last Modified: Thu, 16 Nov 2023 08:35:24 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:676bd9e03c6916f67ddb80177e5dbcb9ba48e2a02aa73990f4a3ca84e314b1e1`  
		Last Modified: Thu, 16 Nov 2023 08:35:24 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d97aade365ce6ad0e88dbeacf46d6d4848438afe9098c42f9d45cb56c3d5889`  
		Last Modified: Thu, 16 Nov 2023 08:35:24 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:2.10.6`

```console
$ docker pull traefik@sha256:b783fbdefa18618b1e5b071872f30dbfdd6e55a30b63430f80b3028463229d80
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; s390x

### `traefik:2.10.6` - linux; s390x

```console
$ docker pull traefik@sha256:1f73a129ceb164fcee414c47e2eeb8166b950ef30728bb86a4142d2fcba75360
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.1 MB (42050681 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:43753aaf21fdf5d7a44475c270504fe5cd018c9a10995cc3bc63defd17ed8661`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 28 Sep 2023 20:41:43 GMT
ADD file:fd3808a676fc56c1380e55b2ddbf4014d9371346cf789860b336bc9f00729ed0 in / 
# Thu, 28 Sep 2023 20:41:44 GMT
CMD ["/bin/sh"]
# Wed, 29 Nov 2023 00:45:49 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 29 Nov 2023 00:46:23 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.6/traefik_v2.10.6_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 29 Nov 2023 00:46:29 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 29 Nov 2023 00:46:30 GMT
EXPOSE 80
# Wed, 29 Nov 2023 00:46:30 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 29 Nov 2023 00:46:30 GMT
CMD ["traefik"]
# Wed, 29 Nov 2023 00:46:30 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.6 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:47539bffe0f44273ec7731d86be2a6171359b3847c9b60c6ac74c4875c3264af`  
		Last Modified: Thu, 28 Sep 2023 20:43:18 GMT  
		Size: 3.2 MB (3215103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef466f0f3a71ca493d3026cd1c1e85592db97303a55121345c9626424dd0d941`  
		Last Modified: Wed, 29 Nov 2023 00:47:25 GMT  
		Size: 622.8 KB (622844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a0bf7a3ef99bf94af2497d00978f85d1009602ec9ec764aa643647e5e5bc653`  
		Last Modified: Wed, 29 Nov 2023 00:47:50 GMT  
		Size: 38.2 MB (38212366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1bd88c0a01deb2371f3822ce3181d55c12b4f33668758d93f9de2a85e812fe4`  
		Last Modified: Wed, 29 Nov 2023 00:47:44 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:2.10.6-windowsservercore-1809`

```console
$ docker pull traefik@sha256:eb37f58646a901dc7727cf448cae36daaefaba79de33b5058dab79aa4c04aefb
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 0

## `traefik:3.0`

```console
$ docker pull traefik@sha256:37fdd705af6341d654a926ea3a22bcd5b7673a171e2917e3613627bdf00902b0
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
$ docker pull traefik@sha256:c0cacfc13537e3e300c438622b3f4f3d968b8acc064b1279af34f468464050cd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.9 MB (42933408 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b49a44fc7d35b2e9c02a3d2d3ff65a2052b7ac11b6b3bfa116c5eabeb6d8f3d8`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 28 Sep 2023 20:41:43 GMT
ADD file:fd3808a676fc56c1380e55b2ddbf4014d9371346cf789860b336bc9f00729ed0 in / 
# Thu, 28 Sep 2023 20:41:44 GMT
CMD ["/bin/sh"]
# Wed, 29 Nov 2023 00:45:49 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 29 Nov 2023 00:45:59 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta4/traefik_v3.0.0-beta4_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 29 Nov 2023 00:46:04 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 29 Nov 2023 00:46:05 GMT
EXPOSE 80
# Wed, 29 Nov 2023 00:46:05 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 29 Nov 2023 00:46:05 GMT
CMD ["traefik"]
# Wed, 29 Nov 2023 00:46:05 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta4 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:47539bffe0f44273ec7731d86be2a6171359b3847c9b60c6ac74c4875c3264af`  
		Last Modified: Thu, 28 Sep 2023 20:43:18 GMT  
		Size: 3.2 MB (3215103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef466f0f3a71ca493d3026cd1c1e85592db97303a55121345c9626424dd0d941`  
		Last Modified: Wed, 29 Nov 2023 00:47:25 GMT  
		Size: 622.8 KB (622844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3404ca1a348f82a1bfe6d8b39b3c42a238f2c9403145bb90d9a7af5443cfd1b`  
		Last Modified: Wed, 29 Nov 2023 00:47:32 GMT  
		Size: 39.1 MB (39095092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47211580b30f098dab76d62b8918df76e1c68707987440c7d112557c5780b9d2`  
		Last Modified: Wed, 29 Nov 2023 00:47:25 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:3.0-windowsservercore-1809`

```console
$ docker pull traefik@sha256:19630807862f87484e67cb4ee380dc6b4c9d23b693e339472b48d45e98a6695a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.5122; amd64

### `traefik:3.0-windowsservercore-1809` - windows version 10.0.17763.5122; amd64

```console
$ docker pull traefik@sha256:2ac02e64d356daa1dc8fd1301b6f2a67b6e5681094cab384fcde2008bec02b5d
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2099063656 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99c6022b519d40f6afa656a268503f5487de25ab4599c5fe32953f7385e93caa`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Thu, 09 Nov 2023 17:56:40 GMT
RUN Install update 10.0.17763.5122
# Thu, 16 Nov 2023 01:37:58 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Nov 2023 08:32:53 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v3.0.0-beta4/traefik_v3.0.0-beta4_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Thu, 16 Nov 2023 08:32:54 GMT
EXPOSE 80
# Thu, 16 Nov 2023 08:32:55 GMT
ENTRYPOINT ["/traefik"]
# Thu, 16 Nov 2023 08:32:56 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta4 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f7bb9e009deb881cb90e8b4318258e03882de9bc9b312b763654b59cd13d0bb`  
		Last Modified: Tue, 14 Nov 2023 19:53:30 GMT  
		Size: 406.8 MB (406811201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce7a1cc914f0f5e059bfdf02906a6e052b1c97cebaf91eb6c2fd835cfddebda2`  
		Last Modified: Thu, 16 Nov 2023 02:26:46 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8577447714f894136f8dcad02f5144f013700f52a7e4a8b77322663ae827843d`  
		Last Modified: Thu, 16 Nov 2023 08:35:07 GMT  
		Size: 41.6 MB (41626426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61adfc07856bba95f19fddcd43601f7dd9190e96e276d19c73bae90e35447f22`  
		Last Modified: Thu, 16 Nov 2023 08:34:57 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c215667b5b3d0976317192c1b9badaec9fe636ab5d80c144142c473f59478d4a`  
		Last Modified: Thu, 16 Nov 2023 08:34:57 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b163722bd41e08e30b2a76118757ac999944507ea8852fc449f7f1bccb147e0e`  
		Last Modified: Thu, 16 Nov 2023 08:34:57 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:3.0.0-beta4`

```console
$ docker pull traefik@sha256:37fdd705af6341d654a926ea3a22bcd5b7673a171e2917e3613627bdf00902b0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

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

### `traefik:3.0.0-beta4` - linux; s390x

```console
$ docker pull traefik@sha256:c0cacfc13537e3e300c438622b3f4f3d968b8acc064b1279af34f468464050cd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.9 MB (42933408 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b49a44fc7d35b2e9c02a3d2d3ff65a2052b7ac11b6b3bfa116c5eabeb6d8f3d8`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 28 Sep 2023 20:41:43 GMT
ADD file:fd3808a676fc56c1380e55b2ddbf4014d9371346cf789860b336bc9f00729ed0 in / 
# Thu, 28 Sep 2023 20:41:44 GMT
CMD ["/bin/sh"]
# Wed, 29 Nov 2023 00:45:49 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 29 Nov 2023 00:45:59 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta4/traefik_v3.0.0-beta4_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 29 Nov 2023 00:46:04 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 29 Nov 2023 00:46:05 GMT
EXPOSE 80
# Wed, 29 Nov 2023 00:46:05 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 29 Nov 2023 00:46:05 GMT
CMD ["traefik"]
# Wed, 29 Nov 2023 00:46:05 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta4 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:47539bffe0f44273ec7731d86be2a6171359b3847c9b60c6ac74c4875c3264af`  
		Last Modified: Thu, 28 Sep 2023 20:43:18 GMT  
		Size: 3.2 MB (3215103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef466f0f3a71ca493d3026cd1c1e85592db97303a55121345c9626424dd0d941`  
		Last Modified: Wed, 29 Nov 2023 00:47:25 GMT  
		Size: 622.8 KB (622844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3404ca1a348f82a1bfe6d8b39b3c42a238f2c9403145bb90d9a7af5443cfd1b`  
		Last Modified: Wed, 29 Nov 2023 00:47:32 GMT  
		Size: 39.1 MB (39095092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47211580b30f098dab76d62b8918df76e1c68707987440c7d112557c5780b9d2`  
		Last Modified: Wed, 29 Nov 2023 00:47:25 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:3.0.0-beta4-windowsservercore-1809`

```console
$ docker pull traefik@sha256:19630807862f87484e67cb4ee380dc6b4c9d23b693e339472b48d45e98a6695a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.5122; amd64

### `traefik:3.0.0-beta4-windowsservercore-1809` - windows version 10.0.17763.5122; amd64

```console
$ docker pull traefik@sha256:2ac02e64d356daa1dc8fd1301b6f2a67b6e5681094cab384fcde2008bec02b5d
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2099063656 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99c6022b519d40f6afa656a268503f5487de25ab4599c5fe32953f7385e93caa`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Thu, 09 Nov 2023 17:56:40 GMT
RUN Install update 10.0.17763.5122
# Thu, 16 Nov 2023 01:37:58 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Nov 2023 08:32:53 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v3.0.0-beta4/traefik_v3.0.0-beta4_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Thu, 16 Nov 2023 08:32:54 GMT
EXPOSE 80
# Thu, 16 Nov 2023 08:32:55 GMT
ENTRYPOINT ["/traefik"]
# Thu, 16 Nov 2023 08:32:56 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta4 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f7bb9e009deb881cb90e8b4318258e03882de9bc9b312b763654b59cd13d0bb`  
		Last Modified: Tue, 14 Nov 2023 19:53:30 GMT  
		Size: 406.8 MB (406811201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce7a1cc914f0f5e059bfdf02906a6e052b1c97cebaf91eb6c2fd835cfddebda2`  
		Last Modified: Thu, 16 Nov 2023 02:26:46 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8577447714f894136f8dcad02f5144f013700f52a7e4a8b77322663ae827843d`  
		Last Modified: Thu, 16 Nov 2023 08:35:07 GMT  
		Size: 41.6 MB (41626426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61adfc07856bba95f19fddcd43601f7dd9190e96e276d19c73bae90e35447f22`  
		Last Modified: Thu, 16 Nov 2023 08:34:57 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c215667b5b3d0976317192c1b9badaec9fe636ab5d80c144142c473f59478d4a`  
		Last Modified: Thu, 16 Nov 2023 08:34:57 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b163722bd41e08e30b2a76118757ac999944507ea8852fc449f7f1bccb147e0e`  
		Last Modified: Thu, 16 Nov 2023 08:34:57 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:beaufort`

```console
$ docker pull traefik@sha256:37fdd705af6341d654a926ea3a22bcd5b7673a171e2917e3613627bdf00902b0
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
$ docker pull traefik@sha256:c0cacfc13537e3e300c438622b3f4f3d968b8acc064b1279af34f468464050cd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.9 MB (42933408 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b49a44fc7d35b2e9c02a3d2d3ff65a2052b7ac11b6b3bfa116c5eabeb6d8f3d8`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 28 Sep 2023 20:41:43 GMT
ADD file:fd3808a676fc56c1380e55b2ddbf4014d9371346cf789860b336bc9f00729ed0 in / 
# Thu, 28 Sep 2023 20:41:44 GMT
CMD ["/bin/sh"]
# Wed, 29 Nov 2023 00:45:49 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 29 Nov 2023 00:45:59 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta4/traefik_v3.0.0-beta4_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 29 Nov 2023 00:46:04 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 29 Nov 2023 00:46:05 GMT
EXPOSE 80
# Wed, 29 Nov 2023 00:46:05 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 29 Nov 2023 00:46:05 GMT
CMD ["traefik"]
# Wed, 29 Nov 2023 00:46:05 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta4 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:47539bffe0f44273ec7731d86be2a6171359b3847c9b60c6ac74c4875c3264af`  
		Last Modified: Thu, 28 Sep 2023 20:43:18 GMT  
		Size: 3.2 MB (3215103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef466f0f3a71ca493d3026cd1c1e85592db97303a55121345c9626424dd0d941`  
		Last Modified: Wed, 29 Nov 2023 00:47:25 GMT  
		Size: 622.8 KB (622844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3404ca1a348f82a1bfe6d8b39b3c42a238f2c9403145bb90d9a7af5443cfd1b`  
		Last Modified: Wed, 29 Nov 2023 00:47:32 GMT  
		Size: 39.1 MB (39095092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47211580b30f098dab76d62b8918df76e1c68707987440c7d112557c5780b9d2`  
		Last Modified: Wed, 29 Nov 2023 00:47:25 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:beaufort-windowsservercore-1809`

```console
$ docker pull traefik@sha256:19630807862f87484e67cb4ee380dc6b4c9d23b693e339472b48d45e98a6695a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.5122; amd64

### `traefik:beaufort-windowsservercore-1809` - windows version 10.0.17763.5122; amd64

```console
$ docker pull traefik@sha256:2ac02e64d356daa1dc8fd1301b6f2a67b6e5681094cab384fcde2008bec02b5d
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2099063656 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99c6022b519d40f6afa656a268503f5487de25ab4599c5fe32953f7385e93caa`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Thu, 09 Nov 2023 17:56:40 GMT
RUN Install update 10.0.17763.5122
# Thu, 16 Nov 2023 01:37:58 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Nov 2023 08:32:53 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v3.0.0-beta4/traefik_v3.0.0-beta4_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Thu, 16 Nov 2023 08:32:54 GMT
EXPOSE 80
# Thu, 16 Nov 2023 08:32:55 GMT
ENTRYPOINT ["/traefik"]
# Thu, 16 Nov 2023 08:32:56 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta4 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f7bb9e009deb881cb90e8b4318258e03882de9bc9b312b763654b59cd13d0bb`  
		Last Modified: Tue, 14 Nov 2023 19:53:30 GMT  
		Size: 406.8 MB (406811201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce7a1cc914f0f5e059bfdf02906a6e052b1c97cebaf91eb6c2fd835cfddebda2`  
		Last Modified: Thu, 16 Nov 2023 02:26:46 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8577447714f894136f8dcad02f5144f013700f52a7e4a8b77322663ae827843d`  
		Last Modified: Thu, 16 Nov 2023 08:35:07 GMT  
		Size: 41.6 MB (41626426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61adfc07856bba95f19fddcd43601f7dd9190e96e276d19c73bae90e35447f22`  
		Last Modified: Thu, 16 Nov 2023 08:34:57 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c215667b5b3d0976317192c1b9badaec9fe636ab5d80c144142c473f59478d4a`  
		Last Modified: Thu, 16 Nov 2023 08:34:57 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b163722bd41e08e30b2a76118757ac999944507ea8852fc449f7f1bccb147e0e`  
		Last Modified: Thu, 16 Nov 2023 08:34:57 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:latest`

```console
$ docker pull traefik@sha256:8b507326e4cf156eb56057f0019b3919520add3867e126cbc24914acbc0cb653
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
$ docker pull traefik@sha256:1f73a129ceb164fcee414c47e2eeb8166b950ef30728bb86a4142d2fcba75360
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.1 MB (42050681 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:43753aaf21fdf5d7a44475c270504fe5cd018c9a10995cc3bc63defd17ed8661`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 28 Sep 2023 20:41:43 GMT
ADD file:fd3808a676fc56c1380e55b2ddbf4014d9371346cf789860b336bc9f00729ed0 in / 
# Thu, 28 Sep 2023 20:41:44 GMT
CMD ["/bin/sh"]
# Wed, 29 Nov 2023 00:45:49 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 29 Nov 2023 00:46:23 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.6/traefik_v2.10.6_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 29 Nov 2023 00:46:29 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 29 Nov 2023 00:46:30 GMT
EXPOSE 80
# Wed, 29 Nov 2023 00:46:30 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 29 Nov 2023 00:46:30 GMT
CMD ["traefik"]
# Wed, 29 Nov 2023 00:46:30 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.6 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:47539bffe0f44273ec7731d86be2a6171359b3847c9b60c6ac74c4875c3264af`  
		Last Modified: Thu, 28 Sep 2023 20:43:18 GMT  
		Size: 3.2 MB (3215103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef466f0f3a71ca493d3026cd1c1e85592db97303a55121345c9626424dd0d941`  
		Last Modified: Wed, 29 Nov 2023 00:47:25 GMT  
		Size: 622.8 KB (622844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a0bf7a3ef99bf94af2497d00978f85d1009602ec9ec764aa643647e5e5bc653`  
		Last Modified: Wed, 29 Nov 2023 00:47:50 GMT  
		Size: 38.2 MB (38212366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1bd88c0a01deb2371f3822ce3181d55c12b4f33668758d93f9de2a85e812fe4`  
		Last Modified: Wed, 29 Nov 2023 00:47:44 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:saintmarcelin`

```console
$ docker pull traefik@sha256:8b507326e4cf156eb56057f0019b3919520add3867e126cbc24914acbc0cb653
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
$ docker pull traefik@sha256:1f73a129ceb164fcee414c47e2eeb8166b950ef30728bb86a4142d2fcba75360
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.1 MB (42050681 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:43753aaf21fdf5d7a44475c270504fe5cd018c9a10995cc3bc63defd17ed8661`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 28 Sep 2023 20:41:43 GMT
ADD file:fd3808a676fc56c1380e55b2ddbf4014d9371346cf789860b336bc9f00729ed0 in / 
# Thu, 28 Sep 2023 20:41:44 GMT
CMD ["/bin/sh"]
# Wed, 29 Nov 2023 00:45:49 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 29 Nov 2023 00:46:23 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.6/traefik_v2.10.6_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 29 Nov 2023 00:46:29 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 29 Nov 2023 00:46:30 GMT
EXPOSE 80
# Wed, 29 Nov 2023 00:46:30 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 29 Nov 2023 00:46:30 GMT
CMD ["traefik"]
# Wed, 29 Nov 2023 00:46:30 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.6 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:47539bffe0f44273ec7731d86be2a6171359b3847c9b60c6ac74c4875c3264af`  
		Last Modified: Thu, 28 Sep 2023 20:43:18 GMT  
		Size: 3.2 MB (3215103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef466f0f3a71ca493d3026cd1c1e85592db97303a55121345c9626424dd0d941`  
		Last Modified: Wed, 29 Nov 2023 00:47:25 GMT  
		Size: 622.8 KB (622844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a0bf7a3ef99bf94af2497d00978f85d1009602ec9ec764aa643647e5e5bc653`  
		Last Modified: Wed, 29 Nov 2023 00:47:50 GMT  
		Size: 38.2 MB (38212366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1bd88c0a01deb2371f3822ce3181d55c12b4f33668758d93f9de2a85e812fe4`  
		Last Modified: Wed, 29 Nov 2023 00:47:44 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:saintmarcelin-windowsservercore-1809`

```console
$ docker pull traefik@sha256:0171555d49032d3e9a8143f92d75bb773bd1d02d0c6ab5c1ce038e1b9d8a97fb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.5122; amd64

### `traefik:saintmarcelin-windowsservercore-1809` - windows version 10.0.17763.5122; amd64

```console
$ docker pull traefik@sha256:7d9e986b167fd6a6e8caf0d270cff4848f68e67d615789d5072359dfaae4658c
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2098008476 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fef5097a6081d1124f5e62b4a0cb1e6f2798c0be3bf4b2ac534172dac2e4aa73`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Thu, 09 Nov 2023 17:56:40 GMT
RUN Install update 10.0.17763.5122
# Thu, 16 Nov 2023 01:37:58 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Nov 2023 08:34:25 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.10.5/traefik_v2.10.5_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Thu, 16 Nov 2023 08:34:26 GMT
EXPOSE 80
# Thu, 16 Nov 2023 08:34:27 GMT
ENTRYPOINT ["/traefik"]
# Thu, 16 Nov 2023 08:34:28 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.5 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f7bb9e009deb881cb90e8b4318258e03882de9bc9b312b763654b59cd13d0bb`  
		Last Modified: Tue, 14 Nov 2023 19:53:30 GMT  
		Size: 406.8 MB (406811201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce7a1cc914f0f5e059bfdf02906a6e052b1c97cebaf91eb6c2fd835cfddebda2`  
		Last Modified: Thu, 16 Nov 2023 02:26:46 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5364859be3494bde67293ec5e752ce6710eb84de075e56586e9dc1a05b9a4953`  
		Last Modified: Thu, 16 Nov 2023 08:35:34 GMT  
		Size: 40.6 MB (40571250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd8773eae2563ee25a1f20ece298456e74f874c3ae705b5516b5f0c51fb4df1a`  
		Last Modified: Thu, 16 Nov 2023 08:35:24 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:676bd9e03c6916f67ddb80177e5dbcb9ba48e2a02aa73990f4a3ca84e314b1e1`  
		Last Modified: Thu, 16 Nov 2023 08:35:24 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d97aade365ce6ad0e88dbeacf46d6d4848438afe9098c42f9d45cb56c3d5889`  
		Last Modified: Thu, 16 Nov 2023 08:35:24 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.10`

```console
$ docker pull traefik@sha256:8b507326e4cf156eb56057f0019b3919520add3867e126cbc24914acbc0cb653
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
$ docker pull traefik@sha256:1f73a129ceb164fcee414c47e2eeb8166b950ef30728bb86a4142d2fcba75360
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.1 MB (42050681 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:43753aaf21fdf5d7a44475c270504fe5cd018c9a10995cc3bc63defd17ed8661`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 28 Sep 2023 20:41:43 GMT
ADD file:fd3808a676fc56c1380e55b2ddbf4014d9371346cf789860b336bc9f00729ed0 in / 
# Thu, 28 Sep 2023 20:41:44 GMT
CMD ["/bin/sh"]
# Wed, 29 Nov 2023 00:45:49 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 29 Nov 2023 00:46:23 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.6/traefik_v2.10.6_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 29 Nov 2023 00:46:29 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 29 Nov 2023 00:46:30 GMT
EXPOSE 80
# Wed, 29 Nov 2023 00:46:30 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 29 Nov 2023 00:46:30 GMT
CMD ["traefik"]
# Wed, 29 Nov 2023 00:46:30 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.6 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:47539bffe0f44273ec7731d86be2a6171359b3847c9b60c6ac74c4875c3264af`  
		Last Modified: Thu, 28 Sep 2023 20:43:18 GMT  
		Size: 3.2 MB (3215103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef466f0f3a71ca493d3026cd1c1e85592db97303a55121345c9626424dd0d941`  
		Last Modified: Wed, 29 Nov 2023 00:47:25 GMT  
		Size: 622.8 KB (622844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a0bf7a3ef99bf94af2497d00978f85d1009602ec9ec764aa643647e5e5bc653`  
		Last Modified: Wed, 29 Nov 2023 00:47:50 GMT  
		Size: 38.2 MB (38212366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1bd88c0a01deb2371f3822ce3181d55c12b4f33668758d93f9de2a85e812fe4`  
		Last Modified: Wed, 29 Nov 2023 00:47:44 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.10-windowsservercore-1809`

```console
$ docker pull traefik@sha256:0171555d49032d3e9a8143f92d75bb773bd1d02d0c6ab5c1ce038e1b9d8a97fb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.5122; amd64

### `traefik:v2.10-windowsservercore-1809` - windows version 10.0.17763.5122; amd64

```console
$ docker pull traefik@sha256:7d9e986b167fd6a6e8caf0d270cff4848f68e67d615789d5072359dfaae4658c
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2098008476 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fef5097a6081d1124f5e62b4a0cb1e6f2798c0be3bf4b2ac534172dac2e4aa73`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Thu, 09 Nov 2023 17:56:40 GMT
RUN Install update 10.0.17763.5122
# Thu, 16 Nov 2023 01:37:58 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Nov 2023 08:34:25 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.10.5/traefik_v2.10.5_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Thu, 16 Nov 2023 08:34:26 GMT
EXPOSE 80
# Thu, 16 Nov 2023 08:34:27 GMT
ENTRYPOINT ["/traefik"]
# Thu, 16 Nov 2023 08:34:28 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.5 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f7bb9e009deb881cb90e8b4318258e03882de9bc9b312b763654b59cd13d0bb`  
		Last Modified: Tue, 14 Nov 2023 19:53:30 GMT  
		Size: 406.8 MB (406811201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce7a1cc914f0f5e059bfdf02906a6e052b1c97cebaf91eb6c2fd835cfddebda2`  
		Last Modified: Thu, 16 Nov 2023 02:26:46 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5364859be3494bde67293ec5e752ce6710eb84de075e56586e9dc1a05b9a4953`  
		Last Modified: Thu, 16 Nov 2023 08:35:34 GMT  
		Size: 40.6 MB (40571250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd8773eae2563ee25a1f20ece298456e74f874c3ae705b5516b5f0c51fb4df1a`  
		Last Modified: Thu, 16 Nov 2023 08:35:24 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:676bd9e03c6916f67ddb80177e5dbcb9ba48e2a02aa73990f4a3ca84e314b1e1`  
		Last Modified: Thu, 16 Nov 2023 08:35:24 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d97aade365ce6ad0e88dbeacf46d6d4848438afe9098c42f9d45cb56c3d5889`  
		Last Modified: Thu, 16 Nov 2023 08:35:24 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.10.6`

```console
$ docker pull traefik@sha256:b783fbdefa18618b1e5b071872f30dbfdd6e55a30b63430f80b3028463229d80
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; s390x

### `traefik:v2.10.6` - linux; s390x

```console
$ docker pull traefik@sha256:1f73a129ceb164fcee414c47e2eeb8166b950ef30728bb86a4142d2fcba75360
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.1 MB (42050681 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:43753aaf21fdf5d7a44475c270504fe5cd018c9a10995cc3bc63defd17ed8661`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 28 Sep 2023 20:41:43 GMT
ADD file:fd3808a676fc56c1380e55b2ddbf4014d9371346cf789860b336bc9f00729ed0 in / 
# Thu, 28 Sep 2023 20:41:44 GMT
CMD ["/bin/sh"]
# Wed, 29 Nov 2023 00:45:49 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 29 Nov 2023 00:46:23 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.6/traefik_v2.10.6_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 29 Nov 2023 00:46:29 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 29 Nov 2023 00:46:30 GMT
EXPOSE 80
# Wed, 29 Nov 2023 00:46:30 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 29 Nov 2023 00:46:30 GMT
CMD ["traefik"]
# Wed, 29 Nov 2023 00:46:30 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.6 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:47539bffe0f44273ec7731d86be2a6171359b3847c9b60c6ac74c4875c3264af`  
		Last Modified: Thu, 28 Sep 2023 20:43:18 GMT  
		Size: 3.2 MB (3215103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef466f0f3a71ca493d3026cd1c1e85592db97303a55121345c9626424dd0d941`  
		Last Modified: Wed, 29 Nov 2023 00:47:25 GMT  
		Size: 622.8 KB (622844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a0bf7a3ef99bf94af2497d00978f85d1009602ec9ec764aa643647e5e5bc653`  
		Last Modified: Wed, 29 Nov 2023 00:47:50 GMT  
		Size: 38.2 MB (38212366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1bd88c0a01deb2371f3822ce3181d55c12b4f33668758d93f9de2a85e812fe4`  
		Last Modified: Wed, 29 Nov 2023 00:47:44 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.10.6-windowsservercore-1809`

```console
$ docker pull traefik@sha256:eb37f58646a901dc7727cf448cae36daaefaba79de33b5058dab79aa4c04aefb
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 0

## `traefik:v3.0`

```console
$ docker pull traefik@sha256:37fdd705af6341d654a926ea3a22bcd5b7673a171e2917e3613627bdf00902b0
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
$ docker pull traefik@sha256:c0cacfc13537e3e300c438622b3f4f3d968b8acc064b1279af34f468464050cd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.9 MB (42933408 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b49a44fc7d35b2e9c02a3d2d3ff65a2052b7ac11b6b3bfa116c5eabeb6d8f3d8`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 28 Sep 2023 20:41:43 GMT
ADD file:fd3808a676fc56c1380e55b2ddbf4014d9371346cf789860b336bc9f00729ed0 in / 
# Thu, 28 Sep 2023 20:41:44 GMT
CMD ["/bin/sh"]
# Wed, 29 Nov 2023 00:45:49 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 29 Nov 2023 00:45:59 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta4/traefik_v3.0.0-beta4_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 29 Nov 2023 00:46:04 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 29 Nov 2023 00:46:05 GMT
EXPOSE 80
# Wed, 29 Nov 2023 00:46:05 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 29 Nov 2023 00:46:05 GMT
CMD ["traefik"]
# Wed, 29 Nov 2023 00:46:05 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta4 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:47539bffe0f44273ec7731d86be2a6171359b3847c9b60c6ac74c4875c3264af`  
		Last Modified: Thu, 28 Sep 2023 20:43:18 GMT  
		Size: 3.2 MB (3215103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef466f0f3a71ca493d3026cd1c1e85592db97303a55121345c9626424dd0d941`  
		Last Modified: Wed, 29 Nov 2023 00:47:25 GMT  
		Size: 622.8 KB (622844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3404ca1a348f82a1bfe6d8b39b3c42a238f2c9403145bb90d9a7af5443cfd1b`  
		Last Modified: Wed, 29 Nov 2023 00:47:32 GMT  
		Size: 39.1 MB (39095092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47211580b30f098dab76d62b8918df76e1c68707987440c7d112557c5780b9d2`  
		Last Modified: Wed, 29 Nov 2023 00:47:25 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v3.0-windowsservercore-1809`

```console
$ docker pull traefik@sha256:19630807862f87484e67cb4ee380dc6b4c9d23b693e339472b48d45e98a6695a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.5122; amd64

### `traefik:v3.0-windowsservercore-1809` - windows version 10.0.17763.5122; amd64

```console
$ docker pull traefik@sha256:2ac02e64d356daa1dc8fd1301b6f2a67b6e5681094cab384fcde2008bec02b5d
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2099063656 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99c6022b519d40f6afa656a268503f5487de25ab4599c5fe32953f7385e93caa`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Thu, 09 Nov 2023 17:56:40 GMT
RUN Install update 10.0.17763.5122
# Thu, 16 Nov 2023 01:37:58 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Nov 2023 08:32:53 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v3.0.0-beta4/traefik_v3.0.0-beta4_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Thu, 16 Nov 2023 08:32:54 GMT
EXPOSE 80
# Thu, 16 Nov 2023 08:32:55 GMT
ENTRYPOINT ["/traefik"]
# Thu, 16 Nov 2023 08:32:56 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta4 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f7bb9e009deb881cb90e8b4318258e03882de9bc9b312b763654b59cd13d0bb`  
		Last Modified: Tue, 14 Nov 2023 19:53:30 GMT  
		Size: 406.8 MB (406811201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce7a1cc914f0f5e059bfdf02906a6e052b1c97cebaf91eb6c2fd835cfddebda2`  
		Last Modified: Thu, 16 Nov 2023 02:26:46 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8577447714f894136f8dcad02f5144f013700f52a7e4a8b77322663ae827843d`  
		Last Modified: Thu, 16 Nov 2023 08:35:07 GMT  
		Size: 41.6 MB (41626426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61adfc07856bba95f19fddcd43601f7dd9190e96e276d19c73bae90e35447f22`  
		Last Modified: Thu, 16 Nov 2023 08:34:57 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c215667b5b3d0976317192c1b9badaec9fe636ab5d80c144142c473f59478d4a`  
		Last Modified: Thu, 16 Nov 2023 08:34:57 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b163722bd41e08e30b2a76118757ac999944507ea8852fc449f7f1bccb147e0e`  
		Last Modified: Thu, 16 Nov 2023 08:34:57 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v3.0.0-beta4`

```console
$ docker pull traefik@sha256:37fdd705af6341d654a926ea3a22bcd5b7673a171e2917e3613627bdf00902b0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

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

### `traefik:v3.0.0-beta4` - linux; s390x

```console
$ docker pull traefik@sha256:c0cacfc13537e3e300c438622b3f4f3d968b8acc064b1279af34f468464050cd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.9 MB (42933408 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b49a44fc7d35b2e9c02a3d2d3ff65a2052b7ac11b6b3bfa116c5eabeb6d8f3d8`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 28 Sep 2023 20:41:43 GMT
ADD file:fd3808a676fc56c1380e55b2ddbf4014d9371346cf789860b336bc9f00729ed0 in / 
# Thu, 28 Sep 2023 20:41:44 GMT
CMD ["/bin/sh"]
# Wed, 29 Nov 2023 00:45:49 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 29 Nov 2023 00:45:59 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta4/traefik_v3.0.0-beta4_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 29 Nov 2023 00:46:04 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 29 Nov 2023 00:46:05 GMT
EXPOSE 80
# Wed, 29 Nov 2023 00:46:05 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 29 Nov 2023 00:46:05 GMT
CMD ["traefik"]
# Wed, 29 Nov 2023 00:46:05 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta4 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:47539bffe0f44273ec7731d86be2a6171359b3847c9b60c6ac74c4875c3264af`  
		Last Modified: Thu, 28 Sep 2023 20:43:18 GMT  
		Size: 3.2 MB (3215103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef466f0f3a71ca493d3026cd1c1e85592db97303a55121345c9626424dd0d941`  
		Last Modified: Wed, 29 Nov 2023 00:47:25 GMT  
		Size: 622.8 KB (622844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3404ca1a348f82a1bfe6d8b39b3c42a238f2c9403145bb90d9a7af5443cfd1b`  
		Last Modified: Wed, 29 Nov 2023 00:47:32 GMT  
		Size: 39.1 MB (39095092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47211580b30f098dab76d62b8918df76e1c68707987440c7d112557c5780b9d2`  
		Last Modified: Wed, 29 Nov 2023 00:47:25 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v3.0.0-beta4-windowsservercore-1809`

```console
$ docker pull traefik@sha256:19630807862f87484e67cb4ee380dc6b4c9d23b693e339472b48d45e98a6695a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.5122; amd64

### `traefik:v3.0.0-beta4-windowsservercore-1809` - windows version 10.0.17763.5122; amd64

```console
$ docker pull traefik@sha256:2ac02e64d356daa1dc8fd1301b6f2a67b6e5681094cab384fcde2008bec02b5d
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2099063656 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99c6022b519d40f6afa656a268503f5487de25ab4599c5fe32953f7385e93caa`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Thu, 09 Nov 2023 17:56:40 GMT
RUN Install update 10.0.17763.5122
# Thu, 16 Nov 2023 01:37:58 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Nov 2023 08:32:53 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v3.0.0-beta4/traefik_v3.0.0-beta4_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Thu, 16 Nov 2023 08:32:54 GMT
EXPOSE 80
# Thu, 16 Nov 2023 08:32:55 GMT
ENTRYPOINT ["/traefik"]
# Thu, 16 Nov 2023 08:32:56 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta4 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f7bb9e009deb881cb90e8b4318258e03882de9bc9b312b763654b59cd13d0bb`  
		Last Modified: Tue, 14 Nov 2023 19:53:30 GMT  
		Size: 406.8 MB (406811201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce7a1cc914f0f5e059bfdf02906a6e052b1c97cebaf91eb6c2fd835cfddebda2`  
		Last Modified: Thu, 16 Nov 2023 02:26:46 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8577447714f894136f8dcad02f5144f013700f52a7e4a8b77322663ae827843d`  
		Last Modified: Thu, 16 Nov 2023 08:35:07 GMT  
		Size: 41.6 MB (41626426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61adfc07856bba95f19fddcd43601f7dd9190e96e276d19c73bae90e35447f22`  
		Last Modified: Thu, 16 Nov 2023 08:34:57 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c215667b5b3d0976317192c1b9badaec9fe636ab5d80c144142c473f59478d4a`  
		Last Modified: Thu, 16 Nov 2023 08:34:57 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b163722bd41e08e30b2a76118757ac999944507ea8852fc449f7f1bccb147e0e`  
		Last Modified: Thu, 16 Nov 2023 08:34:57 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:windowsservercore-1809`

```console
$ docker pull traefik@sha256:0171555d49032d3e9a8143f92d75bb773bd1d02d0c6ab5c1ce038e1b9d8a97fb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.5122; amd64

### `traefik:windowsservercore-1809` - windows version 10.0.17763.5122; amd64

```console
$ docker pull traefik@sha256:7d9e986b167fd6a6e8caf0d270cff4848f68e67d615789d5072359dfaae4658c
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2098008476 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fef5097a6081d1124f5e62b4a0cb1e6f2798c0be3bf4b2ac534172dac2e4aa73`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Thu, 09 Nov 2023 17:56:40 GMT
RUN Install update 10.0.17763.5122
# Thu, 16 Nov 2023 01:37:58 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Nov 2023 08:34:25 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.10.5/traefik_v2.10.5_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Thu, 16 Nov 2023 08:34:26 GMT
EXPOSE 80
# Thu, 16 Nov 2023 08:34:27 GMT
ENTRYPOINT ["/traefik"]
# Thu, 16 Nov 2023 08:34:28 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.5 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f7bb9e009deb881cb90e8b4318258e03882de9bc9b312b763654b59cd13d0bb`  
		Last Modified: Tue, 14 Nov 2023 19:53:30 GMT  
		Size: 406.8 MB (406811201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce7a1cc914f0f5e059bfdf02906a6e052b1c97cebaf91eb6c2fd835cfddebda2`  
		Last Modified: Thu, 16 Nov 2023 02:26:46 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5364859be3494bde67293ec5e752ce6710eb84de075e56586e9dc1a05b9a4953`  
		Last Modified: Thu, 16 Nov 2023 08:35:34 GMT  
		Size: 40.6 MB (40571250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd8773eae2563ee25a1f20ece298456e74f874c3ae705b5516b5f0c51fb4df1a`  
		Last Modified: Thu, 16 Nov 2023 08:35:24 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:676bd9e03c6916f67ddb80177e5dbcb9ba48e2a02aa73990f4a3ca84e314b1e1`  
		Last Modified: Thu, 16 Nov 2023 08:35:24 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d97aade365ce6ad0e88dbeacf46d6d4848438afe9098c42f9d45cb56c3d5889`  
		Last Modified: Thu, 16 Nov 2023 08:35:24 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
