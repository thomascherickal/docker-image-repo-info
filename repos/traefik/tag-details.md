<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `traefik`

-	[`traefik:2.10`](#traefik210)
-	[`traefik:2.10-windowsservercore-1809`](#traefik210-windowsservercore-1809)
-	[`traefik:2.10.6`](#traefik2106)
-	[`traefik:2.10.6-windowsservercore-1809`](#traefik2106-windowsservercore-1809)
-	[`traefik:3.0`](#traefik30)
-	[`traefik:3.0-windowsservercore-1809`](#traefik30-windowsservercore-1809)
-	[`traefik:3.0.0-beta5`](#traefik300-beta5)
-	[`traefik:3.0.0-beta5-windowsservercore-1809`](#traefik300-beta5-windowsservercore-1809)
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
-	[`traefik:v3.0.0-beta5`](#traefikv300-beta5)
-	[`traefik:v3.0.0-beta5-windowsservercore-1809`](#traefikv300-beta5-windowsservercore-1809)
-	[`traefik:windowsservercore-1809`](#traefikwindowsservercore-1809)

## `traefik:2.10`

```console
$ docker pull traefik@sha256:5f99d9c100d5e9e7ff7f88f5312ae3fe47c28a4a81993f2c876975ed70f0cef5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:2.10` - linux; amd64

```console
$ docker pull traefik@sha256:b24c16c9e07f7966fa7053dc1f5cbab55a52d7ebc27b1b47f06ffbf6e74300c4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.2 MB (43229578 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:59cdefb2f44dc58b68182898241a11cdd0d1f42e8f4f0b751c3d65a9afb197af`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 28 Sep 2023 21:19:27 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Thu, 28 Sep 2023 21:19:27 GMT
CMD ["/bin/sh"]
# Wed, 29 Nov 2023 06:31:16 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 29 Nov 2023 06:31:27 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.6/traefik_v2.10.6_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 29 Nov 2023 06:31:27 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 29 Nov 2023 06:31:27 GMT
EXPOSE 80
# Wed, 29 Nov 2023 06:31:28 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 29 Nov 2023 06:31:28 GMT
CMD ["traefik"]
# Wed, 29 Nov 2023 06:31:28 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.6 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:550423c3d1314ff5c8a13904f583e11da40f2e6a9cb9178d6a9ddaf589a41779`  
		Last Modified: Wed, 29 Nov 2023 06:31:39 GMT  
		Size: 622.3 KB (622306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4a7e7be3ff2eb024c7b69ac4a43c4a4bd889658719c1d44a047a23093de50d0`  
		Last Modified: Wed, 29 Nov 2023 06:32:05 GMT  
		Size: 39.2 MB (39204936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0eedc6a01b11648a3ef09decd0f5fe7dc77d79f1f423fbf694e5e72bf0aad727`  
		Last Modified: Wed, 29 Nov 2023 06:31:59 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.10` - linux; arm variant v6

```console
$ docker pull traefik@sha256:ee4c9390ec239d494e291a1c287e0446ef7c3bc65bf44f8149129be679fb0ea2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.8 MB (40819799 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fb69008e6b5ca4b2e9f8fac574fc302587f6484159604be6b60b67ef18c6b12d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 28 Sep 2023 20:49:16 GMT
ADD file:2222b03381ff0fce22edd647f5c60529ec6a72202f8d3cb1d6e4648ebcd19a1e in / 
# Thu, 28 Sep 2023 20:49:16 GMT
CMD ["/bin/sh"]
# Wed, 29 Nov 2023 06:08:47 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 29 Nov 2023 06:09:00 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.6/traefik_v2.10.6_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 29 Nov 2023 06:09:00 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 29 Nov 2023 06:09:00 GMT
EXPOSE 80
# Wed, 29 Nov 2023 06:09:00 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 29 Nov 2023 06:09:00 GMT
CMD ["traefik"]
# Wed, 29 Nov 2023 06:09:01 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.6 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:91cb83b91ee16f1ee0d588fccef56ab5dbb5689a64e5373caf33d7e4fe52ceb4`  
		Last Modified: Thu, 28 Sep 2023 20:51:25 GMT  
		Size: 3.1 MB (3145291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c560ac1492fab77141400f65ad727f721927e8b6e900b4ac28c26f979bca126b`  
		Last Modified: Wed, 29 Nov 2023 06:09:13 GMT  
		Size: 622.7 KB (622724 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f4c2cd2ed2db68cde60fea11fadd614e21b54715f4b187d262a44adaaeea0ba`  
		Last Modified: Wed, 29 Nov 2023 06:09:41 GMT  
		Size: 37.1 MB (37051415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1feb4d81d2128391f399b4a113650a73713d9043fe0bd8610d60416461a8f08d`  
		Last Modified: Wed, 29 Nov 2023 06:09:34 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.10` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:fb2b2d4ba7fa84d4df30aa7f39d24d990da97c8a89edc95fae0a13db29c5eacc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.2 MB (40217109 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc6cf9d511ec323b99dc8a36da0d4ecee3682321b430cd66db33b7524584039a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 28 Sep 2023 20:39:33 GMT
ADD file:ff3112828967e8004a3264d7ece3f81c88e6a1d44d360b9b5613caab15b41717 in / 
# Thu, 28 Sep 2023 20:39:34 GMT
CMD ["/bin/sh"]
# Wed, 29 Nov 2023 05:46:15 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 29 Nov 2023 05:46:25 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.6/traefik_v2.10.6_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 29 Nov 2023 05:46:25 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 29 Nov 2023 05:46:25 GMT
EXPOSE 80
# Wed, 29 Nov 2023 05:46:25 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 29 Nov 2023 05:46:25 GMT
CMD ["traefik"]
# Wed, 29 Nov 2023 05:46:26 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.6 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:579b34f0a95bb83b3acd6b3249ddc52c3d80f5c84b13c944e9e324feb86dd329`  
		Last Modified: Thu, 28 Sep 2023 20:40:08 GMT  
		Size: 3.3 MB (3331831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e3e1d74d27dfa82cc4925dee376ed0ba2c7017bfbd86256a39cd43e067564f2`  
		Last Modified: Wed, 29 Nov 2023 05:46:38 GMT  
		Size: 624.5 KB (624518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95059fa99e09dbde33cb526d541164644a28542b49d664a19f2b9a31249481df`  
		Last Modified: Wed, 29 Nov 2023 05:47:01 GMT  
		Size: 36.3 MB (36260392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0095e4c4a053c89641ac5307d800208b58cd7675ac891d827f18addb52c9d870`  
		Last Modified: Wed, 29 Nov 2023 05:46:57 GMT  
		Size: 368.0 B  
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
$ docker pull traefik@sha256:4009a9c08e8ff3f3a8215cfc2bcce0355913c9800985c58828d1c7cba68572d6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.5122; amd64

### `traefik:2.10-windowsservercore-1809` - windows version 10.0.17763.5122; amd64

```console
$ docker pull traefik@sha256:3f007c45153ec0b2e3abe2b3c7c09b093532d0e198ef4b673e4ddd07bf87ea62
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2098146309 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:84386f59fd9c10dc0607ccebed700b43ed3f66ebfbc4b235398ca2a53bb6dce2`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Thu, 09 Nov 2023 17:56:40 GMT
RUN Install update 10.0.17763.5122
# Thu, 16 Nov 2023 01:37:58 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 29 Nov 2023 02:37:05 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.10.6/traefik_v2.10.6_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Wed, 29 Nov 2023 02:37:06 GMT
EXPOSE 80
# Wed, 29 Nov 2023 02:37:07 GMT
ENTRYPOINT ["/traefik"]
# Wed, 29 Nov 2023 02:37:08 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.6 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:fba9e80c0146453b6de8f35aea2ae18481cf6436bd532c51c90bd2e049433406`  
		Last Modified: Wed, 29 Nov 2023 02:37:46 GMT  
		Size: 40.7 MB (40709104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b54955fdd93b60b49068aadb447e1dbe066720ae5efaa7a315e4592abdd138b0`  
		Last Modified: Wed, 29 Nov 2023 02:37:37 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:463cbb8cb23bb46d13942b85ea410666ef2e97489fb170a77eeaa91dd2f7ae9f`  
		Last Modified: Wed, 29 Nov 2023 02:37:37 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fb9c1cd767d2004163dd2c4b6bb806605d40ff4f8fa90589edef410642f5e41`  
		Last Modified: Wed, 29 Nov 2023 02:37:37 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:2.10.6`

```console
$ docker pull traefik@sha256:5f99d9c100d5e9e7ff7f88f5312ae3fe47c28a4a81993f2c876975ed70f0cef5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:2.10.6` - linux; amd64

```console
$ docker pull traefik@sha256:b24c16c9e07f7966fa7053dc1f5cbab55a52d7ebc27b1b47f06ffbf6e74300c4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.2 MB (43229578 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:59cdefb2f44dc58b68182898241a11cdd0d1f42e8f4f0b751c3d65a9afb197af`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 28 Sep 2023 21:19:27 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Thu, 28 Sep 2023 21:19:27 GMT
CMD ["/bin/sh"]
# Wed, 29 Nov 2023 06:31:16 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 29 Nov 2023 06:31:27 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.6/traefik_v2.10.6_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 29 Nov 2023 06:31:27 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 29 Nov 2023 06:31:27 GMT
EXPOSE 80
# Wed, 29 Nov 2023 06:31:28 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 29 Nov 2023 06:31:28 GMT
CMD ["traefik"]
# Wed, 29 Nov 2023 06:31:28 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.6 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:550423c3d1314ff5c8a13904f583e11da40f2e6a9cb9178d6a9ddaf589a41779`  
		Last Modified: Wed, 29 Nov 2023 06:31:39 GMT  
		Size: 622.3 KB (622306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4a7e7be3ff2eb024c7b69ac4a43c4a4bd889658719c1d44a047a23093de50d0`  
		Last Modified: Wed, 29 Nov 2023 06:32:05 GMT  
		Size: 39.2 MB (39204936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0eedc6a01b11648a3ef09decd0f5fe7dc77d79f1f423fbf694e5e72bf0aad727`  
		Last Modified: Wed, 29 Nov 2023 06:31:59 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.10.6` - linux; arm variant v6

```console
$ docker pull traefik@sha256:ee4c9390ec239d494e291a1c287e0446ef7c3bc65bf44f8149129be679fb0ea2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.8 MB (40819799 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fb69008e6b5ca4b2e9f8fac574fc302587f6484159604be6b60b67ef18c6b12d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 28 Sep 2023 20:49:16 GMT
ADD file:2222b03381ff0fce22edd647f5c60529ec6a72202f8d3cb1d6e4648ebcd19a1e in / 
# Thu, 28 Sep 2023 20:49:16 GMT
CMD ["/bin/sh"]
# Wed, 29 Nov 2023 06:08:47 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 29 Nov 2023 06:09:00 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.6/traefik_v2.10.6_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 29 Nov 2023 06:09:00 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 29 Nov 2023 06:09:00 GMT
EXPOSE 80
# Wed, 29 Nov 2023 06:09:00 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 29 Nov 2023 06:09:00 GMT
CMD ["traefik"]
# Wed, 29 Nov 2023 06:09:01 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.6 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:91cb83b91ee16f1ee0d588fccef56ab5dbb5689a64e5373caf33d7e4fe52ceb4`  
		Last Modified: Thu, 28 Sep 2023 20:51:25 GMT  
		Size: 3.1 MB (3145291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c560ac1492fab77141400f65ad727f721927e8b6e900b4ac28c26f979bca126b`  
		Last Modified: Wed, 29 Nov 2023 06:09:13 GMT  
		Size: 622.7 KB (622724 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f4c2cd2ed2db68cde60fea11fadd614e21b54715f4b187d262a44adaaeea0ba`  
		Last Modified: Wed, 29 Nov 2023 06:09:41 GMT  
		Size: 37.1 MB (37051415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1feb4d81d2128391f399b4a113650a73713d9043fe0bd8610d60416461a8f08d`  
		Last Modified: Wed, 29 Nov 2023 06:09:34 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.10.6` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:fb2b2d4ba7fa84d4df30aa7f39d24d990da97c8a89edc95fae0a13db29c5eacc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.2 MB (40217109 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc6cf9d511ec323b99dc8a36da0d4ecee3682321b430cd66db33b7524584039a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 28 Sep 2023 20:39:33 GMT
ADD file:ff3112828967e8004a3264d7ece3f81c88e6a1d44d360b9b5613caab15b41717 in / 
# Thu, 28 Sep 2023 20:39:34 GMT
CMD ["/bin/sh"]
# Wed, 29 Nov 2023 05:46:15 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 29 Nov 2023 05:46:25 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.6/traefik_v2.10.6_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 29 Nov 2023 05:46:25 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 29 Nov 2023 05:46:25 GMT
EXPOSE 80
# Wed, 29 Nov 2023 05:46:25 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 29 Nov 2023 05:46:25 GMT
CMD ["traefik"]
# Wed, 29 Nov 2023 05:46:26 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.6 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:579b34f0a95bb83b3acd6b3249ddc52c3d80f5c84b13c944e9e324feb86dd329`  
		Last Modified: Thu, 28 Sep 2023 20:40:08 GMT  
		Size: 3.3 MB (3331831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e3e1d74d27dfa82cc4925dee376ed0ba2c7017bfbd86256a39cd43e067564f2`  
		Last Modified: Wed, 29 Nov 2023 05:46:38 GMT  
		Size: 624.5 KB (624518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95059fa99e09dbde33cb526d541164644a28542b49d664a19f2b9a31249481df`  
		Last Modified: Wed, 29 Nov 2023 05:47:01 GMT  
		Size: 36.3 MB (36260392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0095e4c4a053c89641ac5307d800208b58cd7675ac891d827f18addb52c9d870`  
		Last Modified: Wed, 29 Nov 2023 05:46:57 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

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
$ docker pull traefik@sha256:4009a9c08e8ff3f3a8215cfc2bcce0355913c9800985c58828d1c7cba68572d6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.5122; amd64

### `traefik:2.10.6-windowsservercore-1809` - windows version 10.0.17763.5122; amd64

```console
$ docker pull traefik@sha256:3f007c45153ec0b2e3abe2b3c7c09b093532d0e198ef4b673e4ddd07bf87ea62
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2098146309 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:84386f59fd9c10dc0607ccebed700b43ed3f66ebfbc4b235398ca2a53bb6dce2`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Thu, 09 Nov 2023 17:56:40 GMT
RUN Install update 10.0.17763.5122
# Thu, 16 Nov 2023 01:37:58 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 29 Nov 2023 02:37:05 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.10.6/traefik_v2.10.6_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Wed, 29 Nov 2023 02:37:06 GMT
EXPOSE 80
# Wed, 29 Nov 2023 02:37:07 GMT
ENTRYPOINT ["/traefik"]
# Wed, 29 Nov 2023 02:37:08 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.6 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:fba9e80c0146453b6de8f35aea2ae18481cf6436bd532c51c90bd2e049433406`  
		Last Modified: Wed, 29 Nov 2023 02:37:46 GMT  
		Size: 40.7 MB (40709104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b54955fdd93b60b49068aadb447e1dbe066720ae5efaa7a315e4592abdd138b0`  
		Last Modified: Wed, 29 Nov 2023 02:37:37 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:463cbb8cb23bb46d13942b85ea410666ef2e97489fb170a77eeaa91dd2f7ae9f`  
		Last Modified: Wed, 29 Nov 2023 02:37:37 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fb9c1cd767d2004163dd2c4b6bb806605d40ff4f8fa90589edef410642f5e41`  
		Last Modified: Wed, 29 Nov 2023 02:37:37 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:3.0`

```console
$ docker pull traefik@sha256:c7dd4749369c7f39b77b65b460dd10f1d530773121d8974517ab8c7fc335f291
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:3.0` - linux; amd64

```console
$ docker pull traefik@sha256:b465cb7fc3feacd73bf2bd911028cb05bedc79b07df77d2a719da68ae3b5e5b6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.3 MB (44344741 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:35e1b781adcd223ab4008abd81961ada3091446d5d2b9669df1959fc2a919a87`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 28 Sep 2023 21:19:27 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Thu, 28 Sep 2023 21:19:27 GMT
CMD ["/bin/sh"]
# Wed, 29 Nov 2023 06:31:16 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 30 Nov 2023 00:02:08 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta5/traefik_v3.0.0-beta5_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 30 Nov 2023 00:02:08 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 30 Nov 2023 00:02:08 GMT
EXPOSE 80
# Thu, 30 Nov 2023 00:02:08 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 30 Nov 2023 00:02:09 GMT
CMD ["traefik"]
# Thu, 30 Nov 2023 00:02:09 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta5 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:550423c3d1314ff5c8a13904f583e11da40f2e6a9cb9178d6a9ddaf589a41779`  
		Last Modified: Wed, 29 Nov 2023 06:31:39 GMT  
		Size: 622.3 KB (622306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:741f1395c35daaf5c16544c9ca9f71066acf45ac91579688d8533b75542423fd`  
		Last Modified: Thu, 30 Nov 2023 00:02:28 GMT  
		Size: 40.3 MB (40320100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ecf90d6107e9b586f52047ef11e34660f723b57d37b533fec167340b088ddec`  
		Last Modified: Thu, 30 Nov 2023 00:02:22 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:3.0` - linux; arm variant v6

```console
$ docker pull traefik@sha256:730a28168695c9e4f202b004aa278b26ae2504494947ffc13846142bb44602be
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.9 MB (41865413 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:176fa9d73dddf00c2db003aba07c3352d35b433ea46fd3f9ddbcde57f80d490b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 28 Sep 2023 20:49:16 GMT
ADD file:2222b03381ff0fce22edd647f5c60529ec6a72202f8d3cb1d6e4648ebcd19a1e in / 
# Thu, 28 Sep 2023 20:49:16 GMT
CMD ["/bin/sh"]
# Wed, 29 Nov 2023 06:08:47 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 29 Nov 2023 22:49:33 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta5/traefik_v3.0.0-beta5_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 29 Nov 2023 22:49:33 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 29 Nov 2023 22:49:34 GMT
EXPOSE 80
# Wed, 29 Nov 2023 22:49:34 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 29 Nov 2023 22:49:34 GMT
CMD ["traefik"]
# Wed, 29 Nov 2023 22:49:34 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta5 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:91cb83b91ee16f1ee0d588fccef56ab5dbb5689a64e5373caf33d7e4fe52ceb4`  
		Last Modified: Thu, 28 Sep 2023 20:51:25 GMT  
		Size: 3.1 MB (3145291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c560ac1492fab77141400f65ad727f721927e8b6e900b4ac28c26f979bca126b`  
		Last Modified: Wed, 29 Nov 2023 06:09:13 GMT  
		Size: 622.7 KB (622724 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3ea4dc694d9a9830abd0465ed7686827423371b3ddcc9129febf7295c698c40`  
		Last Modified: Wed, 29 Nov 2023 22:49:53 GMT  
		Size: 38.1 MB (38097030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:328ec46c597684cc8bea8abbf2df51f928c0b8a3838e5f979bf8d299bb144ef4`  
		Last Modified: Wed, 29 Nov 2023 22:49:46 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:3.0` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:17b54c18b6b963425c24742d6bfd9ce3391d4fb095a817d63a39f6f45aaa5183
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.3 MB (41267281 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:159c3ccccdd343c97de569516c8d1182f59f01126287a00986447a312ed1ffda`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 28 Sep 2023 20:39:33 GMT
ADD file:ff3112828967e8004a3264d7ece3f81c88e6a1d44d360b9b5613caab15b41717 in / 
# Thu, 28 Sep 2023 20:39:34 GMT
CMD ["/bin/sh"]
# Wed, 29 Nov 2023 05:46:15 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 29 Nov 2023 22:53:58 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta5/traefik_v3.0.0-beta5_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 29 Nov 2023 22:53:59 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 29 Nov 2023 22:53:59 GMT
EXPOSE 80
# Wed, 29 Nov 2023 22:53:59 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 29 Nov 2023 22:53:59 GMT
CMD ["traefik"]
# Wed, 29 Nov 2023 22:53:59 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta5 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:579b34f0a95bb83b3acd6b3249ddc52c3d80f5c84b13c944e9e324feb86dd329`  
		Last Modified: Thu, 28 Sep 2023 20:40:08 GMT  
		Size: 3.3 MB (3331831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e3e1d74d27dfa82cc4925dee376ed0ba2c7017bfbd86256a39cd43e067564f2`  
		Last Modified: Wed, 29 Nov 2023 05:46:38 GMT  
		Size: 624.5 KB (624518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f3f0b4b45dbeb83877a4f4095a9a5460b444bedf0cd771bf7354644dae4d14c`  
		Last Modified: Wed, 29 Nov 2023 22:54:15 GMT  
		Size: 37.3 MB (37310564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61d780b5de6c3e10c3823156c8acc1ce059c97806eb9c5ffbc1e1028ed6665f9`  
		Last Modified: Wed, 29 Nov 2023 22:54:10 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:3.0` - linux; s390x

```console
$ docker pull traefik@sha256:805865463ddea5963049677b95df8521ed93a6497f007fbbaed71f8485565994
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.1 MB (43094242 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d78c5cf9b705fb3a6fa5542b75143d30c439a510c1d26ce8f879f7336d4beddc`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 28 Sep 2023 20:41:43 GMT
ADD file:fd3808a676fc56c1380e55b2ddbf4014d9371346cf789860b336bc9f00729ed0 in / 
# Thu, 28 Sep 2023 20:41:44 GMT
CMD ["/bin/sh"]
# Wed, 29 Nov 2023 00:45:49 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 29 Nov 2023 22:53:24 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta5/traefik_v3.0.0-beta5_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 29 Nov 2023 22:53:32 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 29 Nov 2023 22:53:33 GMT
EXPOSE 80
# Wed, 29 Nov 2023 22:53:33 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 29 Nov 2023 22:53:34 GMT
CMD ["traefik"]
# Wed, 29 Nov 2023 22:53:34 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta5 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:aec19fdf7945578e14db6e95447a4eed13b34bf6e12bca9914059a24956ce655`  
		Last Modified: Wed, 29 Nov 2023 22:54:05 GMT  
		Size: 39.3 MB (39255926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c055557912fa6e42461929b6795eb5fa848b1ab0b5e46ba75ab2b34dc7a17f66`  
		Last Modified: Wed, 29 Nov 2023 22:53:59 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:3.0-windowsservercore-1809`

```console
$ docker pull traefik@sha256:b0c7a98486b0ac8e13a2e2320d452a7464533382cbc252abd449cbb6150737a8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.5122; amd64

### `traefik:3.0-windowsservercore-1809` - windows version 10.0.17763.5122; amd64

```console
$ docker pull traefik@sha256:7e85e697df9033b16fc2f80a00efcb8ac1f717d482f4759a1896ea82b46a1f06
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2099262676 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c790457d2785c38271eccfb5d1a985e2f189d84763d92a8980f1a889f90694f8`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Thu, 09 Nov 2023 17:56:40 GMT
RUN Install update 10.0.17763.5122
# Thu, 16 Nov 2023 01:37:58 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 29 Nov 2023 23:16:56 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v3.0.0-beta5/traefik_v3.0.0-beta5_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Wed, 29 Nov 2023 23:16:58 GMT
EXPOSE 80
# Wed, 29 Nov 2023 23:16:58 GMT
ENTRYPOINT ["/traefik"]
# Wed, 29 Nov 2023 23:16:59 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta5 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:65d3a54963132deb3b7e269bda91707f12702256902f4c90d487ccb21b9d558a`  
		Last Modified: Wed, 29 Nov 2023 23:17:45 GMT  
		Size: 41.8 MB (41825821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbce753338c510a600c4f528fabd498bd13a6342d0cd4f58552ee481c98faf41`  
		Last Modified: Wed, 29 Nov 2023 23:17:35 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41c981bb20ef7dfa9d3f71feb1f2448764c30f56e450431f1c52686bdd4b87de`  
		Last Modified: Wed, 29 Nov 2023 23:17:36 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b828c19e9a4c0fd32592a6e14895b39c96566702494253d5f316348902749062`  
		Last Modified: Wed, 29 Nov 2023 23:17:35 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:3.0.0-beta5`

```console
$ docker pull traefik@sha256:c7dd4749369c7f39b77b65b460dd10f1d530773121d8974517ab8c7fc335f291
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:3.0.0-beta5` - linux; amd64

```console
$ docker pull traefik@sha256:b465cb7fc3feacd73bf2bd911028cb05bedc79b07df77d2a719da68ae3b5e5b6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.3 MB (44344741 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:35e1b781adcd223ab4008abd81961ada3091446d5d2b9669df1959fc2a919a87`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 28 Sep 2023 21:19:27 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Thu, 28 Sep 2023 21:19:27 GMT
CMD ["/bin/sh"]
# Wed, 29 Nov 2023 06:31:16 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 30 Nov 2023 00:02:08 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta5/traefik_v3.0.0-beta5_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 30 Nov 2023 00:02:08 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 30 Nov 2023 00:02:08 GMT
EXPOSE 80
# Thu, 30 Nov 2023 00:02:08 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 30 Nov 2023 00:02:09 GMT
CMD ["traefik"]
# Thu, 30 Nov 2023 00:02:09 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta5 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:550423c3d1314ff5c8a13904f583e11da40f2e6a9cb9178d6a9ddaf589a41779`  
		Last Modified: Wed, 29 Nov 2023 06:31:39 GMT  
		Size: 622.3 KB (622306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:741f1395c35daaf5c16544c9ca9f71066acf45ac91579688d8533b75542423fd`  
		Last Modified: Thu, 30 Nov 2023 00:02:28 GMT  
		Size: 40.3 MB (40320100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ecf90d6107e9b586f52047ef11e34660f723b57d37b533fec167340b088ddec`  
		Last Modified: Thu, 30 Nov 2023 00:02:22 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:3.0.0-beta5` - linux; arm variant v6

```console
$ docker pull traefik@sha256:730a28168695c9e4f202b004aa278b26ae2504494947ffc13846142bb44602be
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.9 MB (41865413 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:176fa9d73dddf00c2db003aba07c3352d35b433ea46fd3f9ddbcde57f80d490b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 28 Sep 2023 20:49:16 GMT
ADD file:2222b03381ff0fce22edd647f5c60529ec6a72202f8d3cb1d6e4648ebcd19a1e in / 
# Thu, 28 Sep 2023 20:49:16 GMT
CMD ["/bin/sh"]
# Wed, 29 Nov 2023 06:08:47 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 29 Nov 2023 22:49:33 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta5/traefik_v3.0.0-beta5_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 29 Nov 2023 22:49:33 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 29 Nov 2023 22:49:34 GMT
EXPOSE 80
# Wed, 29 Nov 2023 22:49:34 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 29 Nov 2023 22:49:34 GMT
CMD ["traefik"]
# Wed, 29 Nov 2023 22:49:34 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta5 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:91cb83b91ee16f1ee0d588fccef56ab5dbb5689a64e5373caf33d7e4fe52ceb4`  
		Last Modified: Thu, 28 Sep 2023 20:51:25 GMT  
		Size: 3.1 MB (3145291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c560ac1492fab77141400f65ad727f721927e8b6e900b4ac28c26f979bca126b`  
		Last Modified: Wed, 29 Nov 2023 06:09:13 GMT  
		Size: 622.7 KB (622724 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3ea4dc694d9a9830abd0465ed7686827423371b3ddcc9129febf7295c698c40`  
		Last Modified: Wed, 29 Nov 2023 22:49:53 GMT  
		Size: 38.1 MB (38097030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:328ec46c597684cc8bea8abbf2df51f928c0b8a3838e5f979bf8d299bb144ef4`  
		Last Modified: Wed, 29 Nov 2023 22:49:46 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:3.0.0-beta5` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:17b54c18b6b963425c24742d6bfd9ce3391d4fb095a817d63a39f6f45aaa5183
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.3 MB (41267281 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:159c3ccccdd343c97de569516c8d1182f59f01126287a00986447a312ed1ffda`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 28 Sep 2023 20:39:33 GMT
ADD file:ff3112828967e8004a3264d7ece3f81c88e6a1d44d360b9b5613caab15b41717 in / 
# Thu, 28 Sep 2023 20:39:34 GMT
CMD ["/bin/sh"]
# Wed, 29 Nov 2023 05:46:15 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 29 Nov 2023 22:53:58 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta5/traefik_v3.0.0-beta5_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 29 Nov 2023 22:53:59 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 29 Nov 2023 22:53:59 GMT
EXPOSE 80
# Wed, 29 Nov 2023 22:53:59 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 29 Nov 2023 22:53:59 GMT
CMD ["traefik"]
# Wed, 29 Nov 2023 22:53:59 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta5 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:579b34f0a95bb83b3acd6b3249ddc52c3d80f5c84b13c944e9e324feb86dd329`  
		Last Modified: Thu, 28 Sep 2023 20:40:08 GMT  
		Size: 3.3 MB (3331831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e3e1d74d27dfa82cc4925dee376ed0ba2c7017bfbd86256a39cd43e067564f2`  
		Last Modified: Wed, 29 Nov 2023 05:46:38 GMT  
		Size: 624.5 KB (624518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f3f0b4b45dbeb83877a4f4095a9a5460b444bedf0cd771bf7354644dae4d14c`  
		Last Modified: Wed, 29 Nov 2023 22:54:15 GMT  
		Size: 37.3 MB (37310564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61d780b5de6c3e10c3823156c8acc1ce059c97806eb9c5ffbc1e1028ed6665f9`  
		Last Modified: Wed, 29 Nov 2023 22:54:10 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:3.0.0-beta5` - linux; s390x

```console
$ docker pull traefik@sha256:805865463ddea5963049677b95df8521ed93a6497f007fbbaed71f8485565994
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.1 MB (43094242 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d78c5cf9b705fb3a6fa5542b75143d30c439a510c1d26ce8f879f7336d4beddc`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 28 Sep 2023 20:41:43 GMT
ADD file:fd3808a676fc56c1380e55b2ddbf4014d9371346cf789860b336bc9f00729ed0 in / 
# Thu, 28 Sep 2023 20:41:44 GMT
CMD ["/bin/sh"]
# Wed, 29 Nov 2023 00:45:49 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 29 Nov 2023 22:53:24 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta5/traefik_v3.0.0-beta5_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 29 Nov 2023 22:53:32 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 29 Nov 2023 22:53:33 GMT
EXPOSE 80
# Wed, 29 Nov 2023 22:53:33 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 29 Nov 2023 22:53:34 GMT
CMD ["traefik"]
# Wed, 29 Nov 2023 22:53:34 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta5 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:aec19fdf7945578e14db6e95447a4eed13b34bf6e12bca9914059a24956ce655`  
		Last Modified: Wed, 29 Nov 2023 22:54:05 GMT  
		Size: 39.3 MB (39255926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c055557912fa6e42461929b6795eb5fa848b1ab0b5e46ba75ab2b34dc7a17f66`  
		Last Modified: Wed, 29 Nov 2023 22:53:59 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:3.0.0-beta5-windowsservercore-1809`

```console
$ docker pull traefik@sha256:b0c7a98486b0ac8e13a2e2320d452a7464533382cbc252abd449cbb6150737a8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.5122; amd64

### `traefik:3.0.0-beta5-windowsservercore-1809` - windows version 10.0.17763.5122; amd64

```console
$ docker pull traefik@sha256:7e85e697df9033b16fc2f80a00efcb8ac1f717d482f4759a1896ea82b46a1f06
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2099262676 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c790457d2785c38271eccfb5d1a985e2f189d84763d92a8980f1a889f90694f8`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Thu, 09 Nov 2023 17:56:40 GMT
RUN Install update 10.0.17763.5122
# Thu, 16 Nov 2023 01:37:58 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 29 Nov 2023 23:16:56 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v3.0.0-beta5/traefik_v3.0.0-beta5_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Wed, 29 Nov 2023 23:16:58 GMT
EXPOSE 80
# Wed, 29 Nov 2023 23:16:58 GMT
ENTRYPOINT ["/traefik"]
# Wed, 29 Nov 2023 23:16:59 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta5 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:65d3a54963132deb3b7e269bda91707f12702256902f4c90d487ccb21b9d558a`  
		Last Modified: Wed, 29 Nov 2023 23:17:45 GMT  
		Size: 41.8 MB (41825821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbce753338c510a600c4f528fabd498bd13a6342d0cd4f58552ee481c98faf41`  
		Last Modified: Wed, 29 Nov 2023 23:17:35 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41c981bb20ef7dfa9d3f71feb1f2448764c30f56e450431f1c52686bdd4b87de`  
		Last Modified: Wed, 29 Nov 2023 23:17:36 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b828c19e9a4c0fd32592a6e14895b39c96566702494253d5f316348902749062`  
		Last Modified: Wed, 29 Nov 2023 23:17:35 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:beaufort`

```console
$ docker pull traefik@sha256:c7dd4749369c7f39b77b65b460dd10f1d530773121d8974517ab8c7fc335f291
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:beaufort` - linux; amd64

```console
$ docker pull traefik@sha256:b465cb7fc3feacd73bf2bd911028cb05bedc79b07df77d2a719da68ae3b5e5b6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.3 MB (44344741 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:35e1b781adcd223ab4008abd81961ada3091446d5d2b9669df1959fc2a919a87`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 28 Sep 2023 21:19:27 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Thu, 28 Sep 2023 21:19:27 GMT
CMD ["/bin/sh"]
# Wed, 29 Nov 2023 06:31:16 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 30 Nov 2023 00:02:08 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta5/traefik_v3.0.0-beta5_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 30 Nov 2023 00:02:08 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 30 Nov 2023 00:02:08 GMT
EXPOSE 80
# Thu, 30 Nov 2023 00:02:08 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 30 Nov 2023 00:02:09 GMT
CMD ["traefik"]
# Thu, 30 Nov 2023 00:02:09 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta5 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:550423c3d1314ff5c8a13904f583e11da40f2e6a9cb9178d6a9ddaf589a41779`  
		Last Modified: Wed, 29 Nov 2023 06:31:39 GMT  
		Size: 622.3 KB (622306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:741f1395c35daaf5c16544c9ca9f71066acf45ac91579688d8533b75542423fd`  
		Last Modified: Thu, 30 Nov 2023 00:02:28 GMT  
		Size: 40.3 MB (40320100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ecf90d6107e9b586f52047ef11e34660f723b57d37b533fec167340b088ddec`  
		Last Modified: Thu, 30 Nov 2023 00:02:22 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:beaufort` - linux; arm variant v6

```console
$ docker pull traefik@sha256:730a28168695c9e4f202b004aa278b26ae2504494947ffc13846142bb44602be
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.9 MB (41865413 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:176fa9d73dddf00c2db003aba07c3352d35b433ea46fd3f9ddbcde57f80d490b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 28 Sep 2023 20:49:16 GMT
ADD file:2222b03381ff0fce22edd647f5c60529ec6a72202f8d3cb1d6e4648ebcd19a1e in / 
# Thu, 28 Sep 2023 20:49:16 GMT
CMD ["/bin/sh"]
# Wed, 29 Nov 2023 06:08:47 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 29 Nov 2023 22:49:33 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta5/traefik_v3.0.0-beta5_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 29 Nov 2023 22:49:33 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 29 Nov 2023 22:49:34 GMT
EXPOSE 80
# Wed, 29 Nov 2023 22:49:34 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 29 Nov 2023 22:49:34 GMT
CMD ["traefik"]
# Wed, 29 Nov 2023 22:49:34 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta5 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:91cb83b91ee16f1ee0d588fccef56ab5dbb5689a64e5373caf33d7e4fe52ceb4`  
		Last Modified: Thu, 28 Sep 2023 20:51:25 GMT  
		Size: 3.1 MB (3145291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c560ac1492fab77141400f65ad727f721927e8b6e900b4ac28c26f979bca126b`  
		Last Modified: Wed, 29 Nov 2023 06:09:13 GMT  
		Size: 622.7 KB (622724 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3ea4dc694d9a9830abd0465ed7686827423371b3ddcc9129febf7295c698c40`  
		Last Modified: Wed, 29 Nov 2023 22:49:53 GMT  
		Size: 38.1 MB (38097030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:328ec46c597684cc8bea8abbf2df51f928c0b8a3838e5f979bf8d299bb144ef4`  
		Last Modified: Wed, 29 Nov 2023 22:49:46 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:beaufort` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:17b54c18b6b963425c24742d6bfd9ce3391d4fb095a817d63a39f6f45aaa5183
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.3 MB (41267281 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:159c3ccccdd343c97de569516c8d1182f59f01126287a00986447a312ed1ffda`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 28 Sep 2023 20:39:33 GMT
ADD file:ff3112828967e8004a3264d7ece3f81c88e6a1d44d360b9b5613caab15b41717 in / 
# Thu, 28 Sep 2023 20:39:34 GMT
CMD ["/bin/sh"]
# Wed, 29 Nov 2023 05:46:15 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 29 Nov 2023 22:53:58 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta5/traefik_v3.0.0-beta5_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 29 Nov 2023 22:53:59 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 29 Nov 2023 22:53:59 GMT
EXPOSE 80
# Wed, 29 Nov 2023 22:53:59 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 29 Nov 2023 22:53:59 GMT
CMD ["traefik"]
# Wed, 29 Nov 2023 22:53:59 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta5 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:579b34f0a95bb83b3acd6b3249ddc52c3d80f5c84b13c944e9e324feb86dd329`  
		Last Modified: Thu, 28 Sep 2023 20:40:08 GMT  
		Size: 3.3 MB (3331831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e3e1d74d27dfa82cc4925dee376ed0ba2c7017bfbd86256a39cd43e067564f2`  
		Last Modified: Wed, 29 Nov 2023 05:46:38 GMT  
		Size: 624.5 KB (624518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f3f0b4b45dbeb83877a4f4095a9a5460b444bedf0cd771bf7354644dae4d14c`  
		Last Modified: Wed, 29 Nov 2023 22:54:15 GMT  
		Size: 37.3 MB (37310564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61d780b5de6c3e10c3823156c8acc1ce059c97806eb9c5ffbc1e1028ed6665f9`  
		Last Modified: Wed, 29 Nov 2023 22:54:10 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:beaufort` - linux; s390x

```console
$ docker pull traefik@sha256:805865463ddea5963049677b95df8521ed93a6497f007fbbaed71f8485565994
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.1 MB (43094242 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d78c5cf9b705fb3a6fa5542b75143d30c439a510c1d26ce8f879f7336d4beddc`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 28 Sep 2023 20:41:43 GMT
ADD file:fd3808a676fc56c1380e55b2ddbf4014d9371346cf789860b336bc9f00729ed0 in / 
# Thu, 28 Sep 2023 20:41:44 GMT
CMD ["/bin/sh"]
# Wed, 29 Nov 2023 00:45:49 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 29 Nov 2023 22:53:24 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta5/traefik_v3.0.0-beta5_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 29 Nov 2023 22:53:32 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 29 Nov 2023 22:53:33 GMT
EXPOSE 80
# Wed, 29 Nov 2023 22:53:33 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 29 Nov 2023 22:53:34 GMT
CMD ["traefik"]
# Wed, 29 Nov 2023 22:53:34 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta5 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:aec19fdf7945578e14db6e95447a4eed13b34bf6e12bca9914059a24956ce655`  
		Last Modified: Wed, 29 Nov 2023 22:54:05 GMT  
		Size: 39.3 MB (39255926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c055557912fa6e42461929b6795eb5fa848b1ab0b5e46ba75ab2b34dc7a17f66`  
		Last Modified: Wed, 29 Nov 2023 22:53:59 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:beaufort-windowsservercore-1809`

```console
$ docker pull traefik@sha256:b0c7a98486b0ac8e13a2e2320d452a7464533382cbc252abd449cbb6150737a8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.5122; amd64

### `traefik:beaufort-windowsservercore-1809` - windows version 10.0.17763.5122; amd64

```console
$ docker pull traefik@sha256:7e85e697df9033b16fc2f80a00efcb8ac1f717d482f4759a1896ea82b46a1f06
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2099262676 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c790457d2785c38271eccfb5d1a985e2f189d84763d92a8980f1a889f90694f8`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Thu, 09 Nov 2023 17:56:40 GMT
RUN Install update 10.0.17763.5122
# Thu, 16 Nov 2023 01:37:58 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 29 Nov 2023 23:16:56 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v3.0.0-beta5/traefik_v3.0.0-beta5_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Wed, 29 Nov 2023 23:16:58 GMT
EXPOSE 80
# Wed, 29 Nov 2023 23:16:58 GMT
ENTRYPOINT ["/traefik"]
# Wed, 29 Nov 2023 23:16:59 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta5 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:65d3a54963132deb3b7e269bda91707f12702256902f4c90d487ccb21b9d558a`  
		Last Modified: Wed, 29 Nov 2023 23:17:45 GMT  
		Size: 41.8 MB (41825821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbce753338c510a600c4f528fabd498bd13a6342d0cd4f58552ee481c98faf41`  
		Last Modified: Wed, 29 Nov 2023 23:17:35 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41c981bb20ef7dfa9d3f71feb1f2448764c30f56e450431f1c52686bdd4b87de`  
		Last Modified: Wed, 29 Nov 2023 23:17:36 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b828c19e9a4c0fd32592a6e14895b39c96566702494253d5f316348902749062`  
		Last Modified: Wed, 29 Nov 2023 23:17:35 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:latest`

```console
$ docker pull traefik@sha256:5f99d9c100d5e9e7ff7f88f5312ae3fe47c28a4a81993f2c876975ed70f0cef5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:latest` - linux; amd64

```console
$ docker pull traefik@sha256:b24c16c9e07f7966fa7053dc1f5cbab55a52d7ebc27b1b47f06ffbf6e74300c4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.2 MB (43229578 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:59cdefb2f44dc58b68182898241a11cdd0d1f42e8f4f0b751c3d65a9afb197af`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 28 Sep 2023 21:19:27 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Thu, 28 Sep 2023 21:19:27 GMT
CMD ["/bin/sh"]
# Wed, 29 Nov 2023 06:31:16 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 29 Nov 2023 06:31:27 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.6/traefik_v2.10.6_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 29 Nov 2023 06:31:27 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 29 Nov 2023 06:31:27 GMT
EXPOSE 80
# Wed, 29 Nov 2023 06:31:28 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 29 Nov 2023 06:31:28 GMT
CMD ["traefik"]
# Wed, 29 Nov 2023 06:31:28 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.6 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:550423c3d1314ff5c8a13904f583e11da40f2e6a9cb9178d6a9ddaf589a41779`  
		Last Modified: Wed, 29 Nov 2023 06:31:39 GMT  
		Size: 622.3 KB (622306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4a7e7be3ff2eb024c7b69ac4a43c4a4bd889658719c1d44a047a23093de50d0`  
		Last Modified: Wed, 29 Nov 2023 06:32:05 GMT  
		Size: 39.2 MB (39204936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0eedc6a01b11648a3ef09decd0f5fe7dc77d79f1f423fbf694e5e72bf0aad727`  
		Last Modified: Wed, 29 Nov 2023 06:31:59 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:latest` - linux; arm variant v6

```console
$ docker pull traefik@sha256:ee4c9390ec239d494e291a1c287e0446ef7c3bc65bf44f8149129be679fb0ea2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.8 MB (40819799 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fb69008e6b5ca4b2e9f8fac574fc302587f6484159604be6b60b67ef18c6b12d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 28 Sep 2023 20:49:16 GMT
ADD file:2222b03381ff0fce22edd647f5c60529ec6a72202f8d3cb1d6e4648ebcd19a1e in / 
# Thu, 28 Sep 2023 20:49:16 GMT
CMD ["/bin/sh"]
# Wed, 29 Nov 2023 06:08:47 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 29 Nov 2023 06:09:00 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.6/traefik_v2.10.6_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 29 Nov 2023 06:09:00 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 29 Nov 2023 06:09:00 GMT
EXPOSE 80
# Wed, 29 Nov 2023 06:09:00 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 29 Nov 2023 06:09:00 GMT
CMD ["traefik"]
# Wed, 29 Nov 2023 06:09:01 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.6 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:91cb83b91ee16f1ee0d588fccef56ab5dbb5689a64e5373caf33d7e4fe52ceb4`  
		Last Modified: Thu, 28 Sep 2023 20:51:25 GMT  
		Size: 3.1 MB (3145291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c560ac1492fab77141400f65ad727f721927e8b6e900b4ac28c26f979bca126b`  
		Last Modified: Wed, 29 Nov 2023 06:09:13 GMT  
		Size: 622.7 KB (622724 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f4c2cd2ed2db68cde60fea11fadd614e21b54715f4b187d262a44adaaeea0ba`  
		Last Modified: Wed, 29 Nov 2023 06:09:41 GMT  
		Size: 37.1 MB (37051415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1feb4d81d2128391f399b4a113650a73713d9043fe0bd8610d60416461a8f08d`  
		Last Modified: Wed, 29 Nov 2023 06:09:34 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:latest` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:fb2b2d4ba7fa84d4df30aa7f39d24d990da97c8a89edc95fae0a13db29c5eacc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.2 MB (40217109 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc6cf9d511ec323b99dc8a36da0d4ecee3682321b430cd66db33b7524584039a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 28 Sep 2023 20:39:33 GMT
ADD file:ff3112828967e8004a3264d7ece3f81c88e6a1d44d360b9b5613caab15b41717 in / 
# Thu, 28 Sep 2023 20:39:34 GMT
CMD ["/bin/sh"]
# Wed, 29 Nov 2023 05:46:15 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 29 Nov 2023 05:46:25 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.6/traefik_v2.10.6_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 29 Nov 2023 05:46:25 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 29 Nov 2023 05:46:25 GMT
EXPOSE 80
# Wed, 29 Nov 2023 05:46:25 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 29 Nov 2023 05:46:25 GMT
CMD ["traefik"]
# Wed, 29 Nov 2023 05:46:26 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.6 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:579b34f0a95bb83b3acd6b3249ddc52c3d80f5c84b13c944e9e324feb86dd329`  
		Last Modified: Thu, 28 Sep 2023 20:40:08 GMT  
		Size: 3.3 MB (3331831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e3e1d74d27dfa82cc4925dee376ed0ba2c7017bfbd86256a39cd43e067564f2`  
		Last Modified: Wed, 29 Nov 2023 05:46:38 GMT  
		Size: 624.5 KB (624518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95059fa99e09dbde33cb526d541164644a28542b49d664a19f2b9a31249481df`  
		Last Modified: Wed, 29 Nov 2023 05:47:01 GMT  
		Size: 36.3 MB (36260392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0095e4c4a053c89641ac5307d800208b58cd7675ac891d827f18addb52c9d870`  
		Last Modified: Wed, 29 Nov 2023 05:46:57 GMT  
		Size: 368.0 B  
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
$ docker pull traefik@sha256:5f99d9c100d5e9e7ff7f88f5312ae3fe47c28a4a81993f2c876975ed70f0cef5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:saintmarcelin` - linux; amd64

```console
$ docker pull traefik@sha256:b24c16c9e07f7966fa7053dc1f5cbab55a52d7ebc27b1b47f06ffbf6e74300c4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.2 MB (43229578 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:59cdefb2f44dc58b68182898241a11cdd0d1f42e8f4f0b751c3d65a9afb197af`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 28 Sep 2023 21:19:27 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Thu, 28 Sep 2023 21:19:27 GMT
CMD ["/bin/sh"]
# Wed, 29 Nov 2023 06:31:16 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 29 Nov 2023 06:31:27 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.6/traefik_v2.10.6_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 29 Nov 2023 06:31:27 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 29 Nov 2023 06:31:27 GMT
EXPOSE 80
# Wed, 29 Nov 2023 06:31:28 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 29 Nov 2023 06:31:28 GMT
CMD ["traefik"]
# Wed, 29 Nov 2023 06:31:28 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.6 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:550423c3d1314ff5c8a13904f583e11da40f2e6a9cb9178d6a9ddaf589a41779`  
		Last Modified: Wed, 29 Nov 2023 06:31:39 GMT  
		Size: 622.3 KB (622306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4a7e7be3ff2eb024c7b69ac4a43c4a4bd889658719c1d44a047a23093de50d0`  
		Last Modified: Wed, 29 Nov 2023 06:32:05 GMT  
		Size: 39.2 MB (39204936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0eedc6a01b11648a3ef09decd0f5fe7dc77d79f1f423fbf694e5e72bf0aad727`  
		Last Modified: Wed, 29 Nov 2023 06:31:59 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:saintmarcelin` - linux; arm variant v6

```console
$ docker pull traefik@sha256:ee4c9390ec239d494e291a1c287e0446ef7c3bc65bf44f8149129be679fb0ea2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.8 MB (40819799 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fb69008e6b5ca4b2e9f8fac574fc302587f6484159604be6b60b67ef18c6b12d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 28 Sep 2023 20:49:16 GMT
ADD file:2222b03381ff0fce22edd647f5c60529ec6a72202f8d3cb1d6e4648ebcd19a1e in / 
# Thu, 28 Sep 2023 20:49:16 GMT
CMD ["/bin/sh"]
# Wed, 29 Nov 2023 06:08:47 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 29 Nov 2023 06:09:00 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.6/traefik_v2.10.6_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 29 Nov 2023 06:09:00 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 29 Nov 2023 06:09:00 GMT
EXPOSE 80
# Wed, 29 Nov 2023 06:09:00 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 29 Nov 2023 06:09:00 GMT
CMD ["traefik"]
# Wed, 29 Nov 2023 06:09:01 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.6 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:91cb83b91ee16f1ee0d588fccef56ab5dbb5689a64e5373caf33d7e4fe52ceb4`  
		Last Modified: Thu, 28 Sep 2023 20:51:25 GMT  
		Size: 3.1 MB (3145291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c560ac1492fab77141400f65ad727f721927e8b6e900b4ac28c26f979bca126b`  
		Last Modified: Wed, 29 Nov 2023 06:09:13 GMT  
		Size: 622.7 KB (622724 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f4c2cd2ed2db68cde60fea11fadd614e21b54715f4b187d262a44adaaeea0ba`  
		Last Modified: Wed, 29 Nov 2023 06:09:41 GMT  
		Size: 37.1 MB (37051415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1feb4d81d2128391f399b4a113650a73713d9043fe0bd8610d60416461a8f08d`  
		Last Modified: Wed, 29 Nov 2023 06:09:34 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:saintmarcelin` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:fb2b2d4ba7fa84d4df30aa7f39d24d990da97c8a89edc95fae0a13db29c5eacc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.2 MB (40217109 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc6cf9d511ec323b99dc8a36da0d4ecee3682321b430cd66db33b7524584039a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 28 Sep 2023 20:39:33 GMT
ADD file:ff3112828967e8004a3264d7ece3f81c88e6a1d44d360b9b5613caab15b41717 in / 
# Thu, 28 Sep 2023 20:39:34 GMT
CMD ["/bin/sh"]
# Wed, 29 Nov 2023 05:46:15 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 29 Nov 2023 05:46:25 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.6/traefik_v2.10.6_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 29 Nov 2023 05:46:25 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 29 Nov 2023 05:46:25 GMT
EXPOSE 80
# Wed, 29 Nov 2023 05:46:25 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 29 Nov 2023 05:46:25 GMT
CMD ["traefik"]
# Wed, 29 Nov 2023 05:46:26 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.6 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:579b34f0a95bb83b3acd6b3249ddc52c3d80f5c84b13c944e9e324feb86dd329`  
		Last Modified: Thu, 28 Sep 2023 20:40:08 GMT  
		Size: 3.3 MB (3331831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e3e1d74d27dfa82cc4925dee376ed0ba2c7017bfbd86256a39cd43e067564f2`  
		Last Modified: Wed, 29 Nov 2023 05:46:38 GMT  
		Size: 624.5 KB (624518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95059fa99e09dbde33cb526d541164644a28542b49d664a19f2b9a31249481df`  
		Last Modified: Wed, 29 Nov 2023 05:47:01 GMT  
		Size: 36.3 MB (36260392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0095e4c4a053c89641ac5307d800208b58cd7675ac891d827f18addb52c9d870`  
		Last Modified: Wed, 29 Nov 2023 05:46:57 GMT  
		Size: 368.0 B  
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
$ docker pull traefik@sha256:4009a9c08e8ff3f3a8215cfc2bcce0355913c9800985c58828d1c7cba68572d6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.5122; amd64

### `traefik:saintmarcelin-windowsservercore-1809` - windows version 10.0.17763.5122; amd64

```console
$ docker pull traefik@sha256:3f007c45153ec0b2e3abe2b3c7c09b093532d0e198ef4b673e4ddd07bf87ea62
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2098146309 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:84386f59fd9c10dc0607ccebed700b43ed3f66ebfbc4b235398ca2a53bb6dce2`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Thu, 09 Nov 2023 17:56:40 GMT
RUN Install update 10.0.17763.5122
# Thu, 16 Nov 2023 01:37:58 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 29 Nov 2023 02:37:05 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.10.6/traefik_v2.10.6_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Wed, 29 Nov 2023 02:37:06 GMT
EXPOSE 80
# Wed, 29 Nov 2023 02:37:07 GMT
ENTRYPOINT ["/traefik"]
# Wed, 29 Nov 2023 02:37:08 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.6 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:fba9e80c0146453b6de8f35aea2ae18481cf6436bd532c51c90bd2e049433406`  
		Last Modified: Wed, 29 Nov 2023 02:37:46 GMT  
		Size: 40.7 MB (40709104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b54955fdd93b60b49068aadb447e1dbe066720ae5efaa7a315e4592abdd138b0`  
		Last Modified: Wed, 29 Nov 2023 02:37:37 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:463cbb8cb23bb46d13942b85ea410666ef2e97489fb170a77eeaa91dd2f7ae9f`  
		Last Modified: Wed, 29 Nov 2023 02:37:37 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fb9c1cd767d2004163dd2c4b6bb806605d40ff4f8fa90589edef410642f5e41`  
		Last Modified: Wed, 29 Nov 2023 02:37:37 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.10`

```console
$ docker pull traefik@sha256:5f99d9c100d5e9e7ff7f88f5312ae3fe47c28a4a81993f2c876975ed70f0cef5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:v2.10` - linux; amd64

```console
$ docker pull traefik@sha256:b24c16c9e07f7966fa7053dc1f5cbab55a52d7ebc27b1b47f06ffbf6e74300c4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.2 MB (43229578 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:59cdefb2f44dc58b68182898241a11cdd0d1f42e8f4f0b751c3d65a9afb197af`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 28 Sep 2023 21:19:27 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Thu, 28 Sep 2023 21:19:27 GMT
CMD ["/bin/sh"]
# Wed, 29 Nov 2023 06:31:16 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 29 Nov 2023 06:31:27 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.6/traefik_v2.10.6_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 29 Nov 2023 06:31:27 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 29 Nov 2023 06:31:27 GMT
EXPOSE 80
# Wed, 29 Nov 2023 06:31:28 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 29 Nov 2023 06:31:28 GMT
CMD ["traefik"]
# Wed, 29 Nov 2023 06:31:28 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.6 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:550423c3d1314ff5c8a13904f583e11da40f2e6a9cb9178d6a9ddaf589a41779`  
		Last Modified: Wed, 29 Nov 2023 06:31:39 GMT  
		Size: 622.3 KB (622306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4a7e7be3ff2eb024c7b69ac4a43c4a4bd889658719c1d44a047a23093de50d0`  
		Last Modified: Wed, 29 Nov 2023 06:32:05 GMT  
		Size: 39.2 MB (39204936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0eedc6a01b11648a3ef09decd0f5fe7dc77d79f1f423fbf694e5e72bf0aad727`  
		Last Modified: Wed, 29 Nov 2023 06:31:59 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.10` - linux; arm variant v6

```console
$ docker pull traefik@sha256:ee4c9390ec239d494e291a1c287e0446ef7c3bc65bf44f8149129be679fb0ea2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.8 MB (40819799 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fb69008e6b5ca4b2e9f8fac574fc302587f6484159604be6b60b67ef18c6b12d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 28 Sep 2023 20:49:16 GMT
ADD file:2222b03381ff0fce22edd647f5c60529ec6a72202f8d3cb1d6e4648ebcd19a1e in / 
# Thu, 28 Sep 2023 20:49:16 GMT
CMD ["/bin/sh"]
# Wed, 29 Nov 2023 06:08:47 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 29 Nov 2023 06:09:00 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.6/traefik_v2.10.6_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 29 Nov 2023 06:09:00 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 29 Nov 2023 06:09:00 GMT
EXPOSE 80
# Wed, 29 Nov 2023 06:09:00 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 29 Nov 2023 06:09:00 GMT
CMD ["traefik"]
# Wed, 29 Nov 2023 06:09:01 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.6 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:91cb83b91ee16f1ee0d588fccef56ab5dbb5689a64e5373caf33d7e4fe52ceb4`  
		Last Modified: Thu, 28 Sep 2023 20:51:25 GMT  
		Size: 3.1 MB (3145291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c560ac1492fab77141400f65ad727f721927e8b6e900b4ac28c26f979bca126b`  
		Last Modified: Wed, 29 Nov 2023 06:09:13 GMT  
		Size: 622.7 KB (622724 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f4c2cd2ed2db68cde60fea11fadd614e21b54715f4b187d262a44adaaeea0ba`  
		Last Modified: Wed, 29 Nov 2023 06:09:41 GMT  
		Size: 37.1 MB (37051415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1feb4d81d2128391f399b4a113650a73713d9043fe0bd8610d60416461a8f08d`  
		Last Modified: Wed, 29 Nov 2023 06:09:34 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.10` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:fb2b2d4ba7fa84d4df30aa7f39d24d990da97c8a89edc95fae0a13db29c5eacc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.2 MB (40217109 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc6cf9d511ec323b99dc8a36da0d4ecee3682321b430cd66db33b7524584039a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 28 Sep 2023 20:39:33 GMT
ADD file:ff3112828967e8004a3264d7ece3f81c88e6a1d44d360b9b5613caab15b41717 in / 
# Thu, 28 Sep 2023 20:39:34 GMT
CMD ["/bin/sh"]
# Wed, 29 Nov 2023 05:46:15 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 29 Nov 2023 05:46:25 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.6/traefik_v2.10.6_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 29 Nov 2023 05:46:25 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 29 Nov 2023 05:46:25 GMT
EXPOSE 80
# Wed, 29 Nov 2023 05:46:25 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 29 Nov 2023 05:46:25 GMT
CMD ["traefik"]
# Wed, 29 Nov 2023 05:46:26 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.6 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:579b34f0a95bb83b3acd6b3249ddc52c3d80f5c84b13c944e9e324feb86dd329`  
		Last Modified: Thu, 28 Sep 2023 20:40:08 GMT  
		Size: 3.3 MB (3331831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e3e1d74d27dfa82cc4925dee376ed0ba2c7017bfbd86256a39cd43e067564f2`  
		Last Modified: Wed, 29 Nov 2023 05:46:38 GMT  
		Size: 624.5 KB (624518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95059fa99e09dbde33cb526d541164644a28542b49d664a19f2b9a31249481df`  
		Last Modified: Wed, 29 Nov 2023 05:47:01 GMT  
		Size: 36.3 MB (36260392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0095e4c4a053c89641ac5307d800208b58cd7675ac891d827f18addb52c9d870`  
		Last Modified: Wed, 29 Nov 2023 05:46:57 GMT  
		Size: 368.0 B  
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
$ docker pull traefik@sha256:4009a9c08e8ff3f3a8215cfc2bcce0355913c9800985c58828d1c7cba68572d6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.5122; amd64

### `traefik:v2.10-windowsservercore-1809` - windows version 10.0.17763.5122; amd64

```console
$ docker pull traefik@sha256:3f007c45153ec0b2e3abe2b3c7c09b093532d0e198ef4b673e4ddd07bf87ea62
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2098146309 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:84386f59fd9c10dc0607ccebed700b43ed3f66ebfbc4b235398ca2a53bb6dce2`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Thu, 09 Nov 2023 17:56:40 GMT
RUN Install update 10.0.17763.5122
# Thu, 16 Nov 2023 01:37:58 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 29 Nov 2023 02:37:05 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.10.6/traefik_v2.10.6_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Wed, 29 Nov 2023 02:37:06 GMT
EXPOSE 80
# Wed, 29 Nov 2023 02:37:07 GMT
ENTRYPOINT ["/traefik"]
# Wed, 29 Nov 2023 02:37:08 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.6 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:fba9e80c0146453b6de8f35aea2ae18481cf6436bd532c51c90bd2e049433406`  
		Last Modified: Wed, 29 Nov 2023 02:37:46 GMT  
		Size: 40.7 MB (40709104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b54955fdd93b60b49068aadb447e1dbe066720ae5efaa7a315e4592abdd138b0`  
		Last Modified: Wed, 29 Nov 2023 02:37:37 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:463cbb8cb23bb46d13942b85ea410666ef2e97489fb170a77eeaa91dd2f7ae9f`  
		Last Modified: Wed, 29 Nov 2023 02:37:37 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fb9c1cd767d2004163dd2c4b6bb806605d40ff4f8fa90589edef410642f5e41`  
		Last Modified: Wed, 29 Nov 2023 02:37:37 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.10.6`

```console
$ docker pull traefik@sha256:5f99d9c100d5e9e7ff7f88f5312ae3fe47c28a4a81993f2c876975ed70f0cef5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:v2.10.6` - linux; amd64

```console
$ docker pull traefik@sha256:b24c16c9e07f7966fa7053dc1f5cbab55a52d7ebc27b1b47f06ffbf6e74300c4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.2 MB (43229578 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:59cdefb2f44dc58b68182898241a11cdd0d1f42e8f4f0b751c3d65a9afb197af`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 28 Sep 2023 21:19:27 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Thu, 28 Sep 2023 21:19:27 GMT
CMD ["/bin/sh"]
# Wed, 29 Nov 2023 06:31:16 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 29 Nov 2023 06:31:27 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.6/traefik_v2.10.6_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 29 Nov 2023 06:31:27 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 29 Nov 2023 06:31:27 GMT
EXPOSE 80
# Wed, 29 Nov 2023 06:31:28 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 29 Nov 2023 06:31:28 GMT
CMD ["traefik"]
# Wed, 29 Nov 2023 06:31:28 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.6 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:550423c3d1314ff5c8a13904f583e11da40f2e6a9cb9178d6a9ddaf589a41779`  
		Last Modified: Wed, 29 Nov 2023 06:31:39 GMT  
		Size: 622.3 KB (622306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4a7e7be3ff2eb024c7b69ac4a43c4a4bd889658719c1d44a047a23093de50d0`  
		Last Modified: Wed, 29 Nov 2023 06:32:05 GMT  
		Size: 39.2 MB (39204936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0eedc6a01b11648a3ef09decd0f5fe7dc77d79f1f423fbf694e5e72bf0aad727`  
		Last Modified: Wed, 29 Nov 2023 06:31:59 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.10.6` - linux; arm variant v6

```console
$ docker pull traefik@sha256:ee4c9390ec239d494e291a1c287e0446ef7c3bc65bf44f8149129be679fb0ea2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.8 MB (40819799 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fb69008e6b5ca4b2e9f8fac574fc302587f6484159604be6b60b67ef18c6b12d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 28 Sep 2023 20:49:16 GMT
ADD file:2222b03381ff0fce22edd647f5c60529ec6a72202f8d3cb1d6e4648ebcd19a1e in / 
# Thu, 28 Sep 2023 20:49:16 GMT
CMD ["/bin/sh"]
# Wed, 29 Nov 2023 06:08:47 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 29 Nov 2023 06:09:00 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.6/traefik_v2.10.6_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 29 Nov 2023 06:09:00 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 29 Nov 2023 06:09:00 GMT
EXPOSE 80
# Wed, 29 Nov 2023 06:09:00 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 29 Nov 2023 06:09:00 GMT
CMD ["traefik"]
# Wed, 29 Nov 2023 06:09:01 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.6 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:91cb83b91ee16f1ee0d588fccef56ab5dbb5689a64e5373caf33d7e4fe52ceb4`  
		Last Modified: Thu, 28 Sep 2023 20:51:25 GMT  
		Size: 3.1 MB (3145291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c560ac1492fab77141400f65ad727f721927e8b6e900b4ac28c26f979bca126b`  
		Last Modified: Wed, 29 Nov 2023 06:09:13 GMT  
		Size: 622.7 KB (622724 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f4c2cd2ed2db68cde60fea11fadd614e21b54715f4b187d262a44adaaeea0ba`  
		Last Modified: Wed, 29 Nov 2023 06:09:41 GMT  
		Size: 37.1 MB (37051415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1feb4d81d2128391f399b4a113650a73713d9043fe0bd8610d60416461a8f08d`  
		Last Modified: Wed, 29 Nov 2023 06:09:34 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.10.6` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:fb2b2d4ba7fa84d4df30aa7f39d24d990da97c8a89edc95fae0a13db29c5eacc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.2 MB (40217109 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc6cf9d511ec323b99dc8a36da0d4ecee3682321b430cd66db33b7524584039a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 28 Sep 2023 20:39:33 GMT
ADD file:ff3112828967e8004a3264d7ece3f81c88e6a1d44d360b9b5613caab15b41717 in / 
# Thu, 28 Sep 2023 20:39:34 GMT
CMD ["/bin/sh"]
# Wed, 29 Nov 2023 05:46:15 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 29 Nov 2023 05:46:25 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.6/traefik_v2.10.6_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 29 Nov 2023 05:46:25 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 29 Nov 2023 05:46:25 GMT
EXPOSE 80
# Wed, 29 Nov 2023 05:46:25 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 29 Nov 2023 05:46:25 GMT
CMD ["traefik"]
# Wed, 29 Nov 2023 05:46:26 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.6 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:579b34f0a95bb83b3acd6b3249ddc52c3d80f5c84b13c944e9e324feb86dd329`  
		Last Modified: Thu, 28 Sep 2023 20:40:08 GMT  
		Size: 3.3 MB (3331831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e3e1d74d27dfa82cc4925dee376ed0ba2c7017bfbd86256a39cd43e067564f2`  
		Last Modified: Wed, 29 Nov 2023 05:46:38 GMT  
		Size: 624.5 KB (624518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95059fa99e09dbde33cb526d541164644a28542b49d664a19f2b9a31249481df`  
		Last Modified: Wed, 29 Nov 2023 05:47:01 GMT  
		Size: 36.3 MB (36260392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0095e4c4a053c89641ac5307d800208b58cd7675ac891d827f18addb52c9d870`  
		Last Modified: Wed, 29 Nov 2023 05:46:57 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

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
$ docker pull traefik@sha256:4009a9c08e8ff3f3a8215cfc2bcce0355913c9800985c58828d1c7cba68572d6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.5122; amd64

### `traefik:v2.10.6-windowsservercore-1809` - windows version 10.0.17763.5122; amd64

```console
$ docker pull traefik@sha256:3f007c45153ec0b2e3abe2b3c7c09b093532d0e198ef4b673e4ddd07bf87ea62
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2098146309 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:84386f59fd9c10dc0607ccebed700b43ed3f66ebfbc4b235398ca2a53bb6dce2`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Thu, 09 Nov 2023 17:56:40 GMT
RUN Install update 10.0.17763.5122
# Thu, 16 Nov 2023 01:37:58 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 29 Nov 2023 02:37:05 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.10.6/traefik_v2.10.6_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Wed, 29 Nov 2023 02:37:06 GMT
EXPOSE 80
# Wed, 29 Nov 2023 02:37:07 GMT
ENTRYPOINT ["/traefik"]
# Wed, 29 Nov 2023 02:37:08 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.6 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:fba9e80c0146453b6de8f35aea2ae18481cf6436bd532c51c90bd2e049433406`  
		Last Modified: Wed, 29 Nov 2023 02:37:46 GMT  
		Size: 40.7 MB (40709104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b54955fdd93b60b49068aadb447e1dbe066720ae5efaa7a315e4592abdd138b0`  
		Last Modified: Wed, 29 Nov 2023 02:37:37 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:463cbb8cb23bb46d13942b85ea410666ef2e97489fb170a77eeaa91dd2f7ae9f`  
		Last Modified: Wed, 29 Nov 2023 02:37:37 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fb9c1cd767d2004163dd2c4b6bb806605d40ff4f8fa90589edef410642f5e41`  
		Last Modified: Wed, 29 Nov 2023 02:37:37 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v3.0`

```console
$ docker pull traefik@sha256:c7dd4749369c7f39b77b65b460dd10f1d530773121d8974517ab8c7fc335f291
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:v3.0` - linux; amd64

```console
$ docker pull traefik@sha256:b465cb7fc3feacd73bf2bd911028cb05bedc79b07df77d2a719da68ae3b5e5b6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.3 MB (44344741 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:35e1b781adcd223ab4008abd81961ada3091446d5d2b9669df1959fc2a919a87`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 28 Sep 2023 21:19:27 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Thu, 28 Sep 2023 21:19:27 GMT
CMD ["/bin/sh"]
# Wed, 29 Nov 2023 06:31:16 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 30 Nov 2023 00:02:08 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta5/traefik_v3.0.0-beta5_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 30 Nov 2023 00:02:08 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 30 Nov 2023 00:02:08 GMT
EXPOSE 80
# Thu, 30 Nov 2023 00:02:08 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 30 Nov 2023 00:02:09 GMT
CMD ["traefik"]
# Thu, 30 Nov 2023 00:02:09 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta5 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:550423c3d1314ff5c8a13904f583e11da40f2e6a9cb9178d6a9ddaf589a41779`  
		Last Modified: Wed, 29 Nov 2023 06:31:39 GMT  
		Size: 622.3 KB (622306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:741f1395c35daaf5c16544c9ca9f71066acf45ac91579688d8533b75542423fd`  
		Last Modified: Thu, 30 Nov 2023 00:02:28 GMT  
		Size: 40.3 MB (40320100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ecf90d6107e9b586f52047ef11e34660f723b57d37b533fec167340b088ddec`  
		Last Modified: Thu, 30 Nov 2023 00:02:22 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v3.0` - linux; arm variant v6

```console
$ docker pull traefik@sha256:730a28168695c9e4f202b004aa278b26ae2504494947ffc13846142bb44602be
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.9 MB (41865413 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:176fa9d73dddf00c2db003aba07c3352d35b433ea46fd3f9ddbcde57f80d490b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 28 Sep 2023 20:49:16 GMT
ADD file:2222b03381ff0fce22edd647f5c60529ec6a72202f8d3cb1d6e4648ebcd19a1e in / 
# Thu, 28 Sep 2023 20:49:16 GMT
CMD ["/bin/sh"]
# Wed, 29 Nov 2023 06:08:47 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 29 Nov 2023 22:49:33 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta5/traefik_v3.0.0-beta5_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 29 Nov 2023 22:49:33 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 29 Nov 2023 22:49:34 GMT
EXPOSE 80
# Wed, 29 Nov 2023 22:49:34 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 29 Nov 2023 22:49:34 GMT
CMD ["traefik"]
# Wed, 29 Nov 2023 22:49:34 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta5 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:91cb83b91ee16f1ee0d588fccef56ab5dbb5689a64e5373caf33d7e4fe52ceb4`  
		Last Modified: Thu, 28 Sep 2023 20:51:25 GMT  
		Size: 3.1 MB (3145291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c560ac1492fab77141400f65ad727f721927e8b6e900b4ac28c26f979bca126b`  
		Last Modified: Wed, 29 Nov 2023 06:09:13 GMT  
		Size: 622.7 KB (622724 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3ea4dc694d9a9830abd0465ed7686827423371b3ddcc9129febf7295c698c40`  
		Last Modified: Wed, 29 Nov 2023 22:49:53 GMT  
		Size: 38.1 MB (38097030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:328ec46c597684cc8bea8abbf2df51f928c0b8a3838e5f979bf8d299bb144ef4`  
		Last Modified: Wed, 29 Nov 2023 22:49:46 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v3.0` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:17b54c18b6b963425c24742d6bfd9ce3391d4fb095a817d63a39f6f45aaa5183
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.3 MB (41267281 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:159c3ccccdd343c97de569516c8d1182f59f01126287a00986447a312ed1ffda`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 28 Sep 2023 20:39:33 GMT
ADD file:ff3112828967e8004a3264d7ece3f81c88e6a1d44d360b9b5613caab15b41717 in / 
# Thu, 28 Sep 2023 20:39:34 GMT
CMD ["/bin/sh"]
# Wed, 29 Nov 2023 05:46:15 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 29 Nov 2023 22:53:58 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta5/traefik_v3.0.0-beta5_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 29 Nov 2023 22:53:59 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 29 Nov 2023 22:53:59 GMT
EXPOSE 80
# Wed, 29 Nov 2023 22:53:59 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 29 Nov 2023 22:53:59 GMT
CMD ["traefik"]
# Wed, 29 Nov 2023 22:53:59 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta5 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:579b34f0a95bb83b3acd6b3249ddc52c3d80f5c84b13c944e9e324feb86dd329`  
		Last Modified: Thu, 28 Sep 2023 20:40:08 GMT  
		Size: 3.3 MB (3331831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e3e1d74d27dfa82cc4925dee376ed0ba2c7017bfbd86256a39cd43e067564f2`  
		Last Modified: Wed, 29 Nov 2023 05:46:38 GMT  
		Size: 624.5 KB (624518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f3f0b4b45dbeb83877a4f4095a9a5460b444bedf0cd771bf7354644dae4d14c`  
		Last Modified: Wed, 29 Nov 2023 22:54:15 GMT  
		Size: 37.3 MB (37310564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61d780b5de6c3e10c3823156c8acc1ce059c97806eb9c5ffbc1e1028ed6665f9`  
		Last Modified: Wed, 29 Nov 2023 22:54:10 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v3.0` - linux; s390x

```console
$ docker pull traefik@sha256:805865463ddea5963049677b95df8521ed93a6497f007fbbaed71f8485565994
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.1 MB (43094242 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d78c5cf9b705fb3a6fa5542b75143d30c439a510c1d26ce8f879f7336d4beddc`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 28 Sep 2023 20:41:43 GMT
ADD file:fd3808a676fc56c1380e55b2ddbf4014d9371346cf789860b336bc9f00729ed0 in / 
# Thu, 28 Sep 2023 20:41:44 GMT
CMD ["/bin/sh"]
# Wed, 29 Nov 2023 00:45:49 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 29 Nov 2023 22:53:24 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta5/traefik_v3.0.0-beta5_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 29 Nov 2023 22:53:32 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 29 Nov 2023 22:53:33 GMT
EXPOSE 80
# Wed, 29 Nov 2023 22:53:33 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 29 Nov 2023 22:53:34 GMT
CMD ["traefik"]
# Wed, 29 Nov 2023 22:53:34 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta5 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:aec19fdf7945578e14db6e95447a4eed13b34bf6e12bca9914059a24956ce655`  
		Last Modified: Wed, 29 Nov 2023 22:54:05 GMT  
		Size: 39.3 MB (39255926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c055557912fa6e42461929b6795eb5fa848b1ab0b5e46ba75ab2b34dc7a17f66`  
		Last Modified: Wed, 29 Nov 2023 22:53:59 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v3.0-windowsservercore-1809`

```console
$ docker pull traefik@sha256:b0c7a98486b0ac8e13a2e2320d452a7464533382cbc252abd449cbb6150737a8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.5122; amd64

### `traefik:v3.0-windowsservercore-1809` - windows version 10.0.17763.5122; amd64

```console
$ docker pull traefik@sha256:7e85e697df9033b16fc2f80a00efcb8ac1f717d482f4759a1896ea82b46a1f06
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2099262676 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c790457d2785c38271eccfb5d1a985e2f189d84763d92a8980f1a889f90694f8`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Thu, 09 Nov 2023 17:56:40 GMT
RUN Install update 10.0.17763.5122
# Thu, 16 Nov 2023 01:37:58 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 29 Nov 2023 23:16:56 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v3.0.0-beta5/traefik_v3.0.0-beta5_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Wed, 29 Nov 2023 23:16:58 GMT
EXPOSE 80
# Wed, 29 Nov 2023 23:16:58 GMT
ENTRYPOINT ["/traefik"]
# Wed, 29 Nov 2023 23:16:59 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta5 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:65d3a54963132deb3b7e269bda91707f12702256902f4c90d487ccb21b9d558a`  
		Last Modified: Wed, 29 Nov 2023 23:17:45 GMT  
		Size: 41.8 MB (41825821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbce753338c510a600c4f528fabd498bd13a6342d0cd4f58552ee481c98faf41`  
		Last Modified: Wed, 29 Nov 2023 23:17:35 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41c981bb20ef7dfa9d3f71feb1f2448764c30f56e450431f1c52686bdd4b87de`  
		Last Modified: Wed, 29 Nov 2023 23:17:36 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b828c19e9a4c0fd32592a6e14895b39c96566702494253d5f316348902749062`  
		Last Modified: Wed, 29 Nov 2023 23:17:35 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v3.0.0-beta5`

```console
$ docker pull traefik@sha256:c7dd4749369c7f39b77b65b460dd10f1d530773121d8974517ab8c7fc335f291
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:v3.0.0-beta5` - linux; amd64

```console
$ docker pull traefik@sha256:b465cb7fc3feacd73bf2bd911028cb05bedc79b07df77d2a719da68ae3b5e5b6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.3 MB (44344741 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:35e1b781adcd223ab4008abd81961ada3091446d5d2b9669df1959fc2a919a87`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 28 Sep 2023 21:19:27 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Thu, 28 Sep 2023 21:19:27 GMT
CMD ["/bin/sh"]
# Wed, 29 Nov 2023 06:31:16 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 30 Nov 2023 00:02:08 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta5/traefik_v3.0.0-beta5_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 30 Nov 2023 00:02:08 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 30 Nov 2023 00:02:08 GMT
EXPOSE 80
# Thu, 30 Nov 2023 00:02:08 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 30 Nov 2023 00:02:09 GMT
CMD ["traefik"]
# Thu, 30 Nov 2023 00:02:09 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta5 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:550423c3d1314ff5c8a13904f583e11da40f2e6a9cb9178d6a9ddaf589a41779`  
		Last Modified: Wed, 29 Nov 2023 06:31:39 GMT  
		Size: 622.3 KB (622306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:741f1395c35daaf5c16544c9ca9f71066acf45ac91579688d8533b75542423fd`  
		Last Modified: Thu, 30 Nov 2023 00:02:28 GMT  
		Size: 40.3 MB (40320100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ecf90d6107e9b586f52047ef11e34660f723b57d37b533fec167340b088ddec`  
		Last Modified: Thu, 30 Nov 2023 00:02:22 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v3.0.0-beta5` - linux; arm variant v6

```console
$ docker pull traefik@sha256:730a28168695c9e4f202b004aa278b26ae2504494947ffc13846142bb44602be
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.9 MB (41865413 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:176fa9d73dddf00c2db003aba07c3352d35b433ea46fd3f9ddbcde57f80d490b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 28 Sep 2023 20:49:16 GMT
ADD file:2222b03381ff0fce22edd647f5c60529ec6a72202f8d3cb1d6e4648ebcd19a1e in / 
# Thu, 28 Sep 2023 20:49:16 GMT
CMD ["/bin/sh"]
# Wed, 29 Nov 2023 06:08:47 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 29 Nov 2023 22:49:33 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta5/traefik_v3.0.0-beta5_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 29 Nov 2023 22:49:33 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 29 Nov 2023 22:49:34 GMT
EXPOSE 80
# Wed, 29 Nov 2023 22:49:34 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 29 Nov 2023 22:49:34 GMT
CMD ["traefik"]
# Wed, 29 Nov 2023 22:49:34 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta5 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:91cb83b91ee16f1ee0d588fccef56ab5dbb5689a64e5373caf33d7e4fe52ceb4`  
		Last Modified: Thu, 28 Sep 2023 20:51:25 GMT  
		Size: 3.1 MB (3145291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c560ac1492fab77141400f65ad727f721927e8b6e900b4ac28c26f979bca126b`  
		Last Modified: Wed, 29 Nov 2023 06:09:13 GMT  
		Size: 622.7 KB (622724 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3ea4dc694d9a9830abd0465ed7686827423371b3ddcc9129febf7295c698c40`  
		Last Modified: Wed, 29 Nov 2023 22:49:53 GMT  
		Size: 38.1 MB (38097030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:328ec46c597684cc8bea8abbf2df51f928c0b8a3838e5f979bf8d299bb144ef4`  
		Last Modified: Wed, 29 Nov 2023 22:49:46 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v3.0.0-beta5` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:17b54c18b6b963425c24742d6bfd9ce3391d4fb095a817d63a39f6f45aaa5183
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.3 MB (41267281 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:159c3ccccdd343c97de569516c8d1182f59f01126287a00986447a312ed1ffda`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 28 Sep 2023 20:39:33 GMT
ADD file:ff3112828967e8004a3264d7ece3f81c88e6a1d44d360b9b5613caab15b41717 in / 
# Thu, 28 Sep 2023 20:39:34 GMT
CMD ["/bin/sh"]
# Wed, 29 Nov 2023 05:46:15 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 29 Nov 2023 22:53:58 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta5/traefik_v3.0.0-beta5_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 29 Nov 2023 22:53:59 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 29 Nov 2023 22:53:59 GMT
EXPOSE 80
# Wed, 29 Nov 2023 22:53:59 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 29 Nov 2023 22:53:59 GMT
CMD ["traefik"]
# Wed, 29 Nov 2023 22:53:59 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta5 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:579b34f0a95bb83b3acd6b3249ddc52c3d80f5c84b13c944e9e324feb86dd329`  
		Last Modified: Thu, 28 Sep 2023 20:40:08 GMT  
		Size: 3.3 MB (3331831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e3e1d74d27dfa82cc4925dee376ed0ba2c7017bfbd86256a39cd43e067564f2`  
		Last Modified: Wed, 29 Nov 2023 05:46:38 GMT  
		Size: 624.5 KB (624518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f3f0b4b45dbeb83877a4f4095a9a5460b444bedf0cd771bf7354644dae4d14c`  
		Last Modified: Wed, 29 Nov 2023 22:54:15 GMT  
		Size: 37.3 MB (37310564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61d780b5de6c3e10c3823156c8acc1ce059c97806eb9c5ffbc1e1028ed6665f9`  
		Last Modified: Wed, 29 Nov 2023 22:54:10 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v3.0.0-beta5` - linux; s390x

```console
$ docker pull traefik@sha256:805865463ddea5963049677b95df8521ed93a6497f007fbbaed71f8485565994
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.1 MB (43094242 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d78c5cf9b705fb3a6fa5542b75143d30c439a510c1d26ce8f879f7336d4beddc`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 28 Sep 2023 20:41:43 GMT
ADD file:fd3808a676fc56c1380e55b2ddbf4014d9371346cf789860b336bc9f00729ed0 in / 
# Thu, 28 Sep 2023 20:41:44 GMT
CMD ["/bin/sh"]
# Wed, 29 Nov 2023 00:45:49 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 29 Nov 2023 22:53:24 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta5/traefik_v3.0.0-beta5_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 29 Nov 2023 22:53:32 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 29 Nov 2023 22:53:33 GMT
EXPOSE 80
# Wed, 29 Nov 2023 22:53:33 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 29 Nov 2023 22:53:34 GMT
CMD ["traefik"]
# Wed, 29 Nov 2023 22:53:34 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta5 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:aec19fdf7945578e14db6e95447a4eed13b34bf6e12bca9914059a24956ce655`  
		Last Modified: Wed, 29 Nov 2023 22:54:05 GMT  
		Size: 39.3 MB (39255926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c055557912fa6e42461929b6795eb5fa848b1ab0b5e46ba75ab2b34dc7a17f66`  
		Last Modified: Wed, 29 Nov 2023 22:53:59 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v3.0.0-beta5-windowsservercore-1809`

```console
$ docker pull traefik@sha256:b0c7a98486b0ac8e13a2e2320d452a7464533382cbc252abd449cbb6150737a8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.5122; amd64

### `traefik:v3.0.0-beta5-windowsservercore-1809` - windows version 10.0.17763.5122; amd64

```console
$ docker pull traefik@sha256:7e85e697df9033b16fc2f80a00efcb8ac1f717d482f4759a1896ea82b46a1f06
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2099262676 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c790457d2785c38271eccfb5d1a985e2f189d84763d92a8980f1a889f90694f8`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Thu, 09 Nov 2023 17:56:40 GMT
RUN Install update 10.0.17763.5122
# Thu, 16 Nov 2023 01:37:58 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 29 Nov 2023 23:16:56 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v3.0.0-beta5/traefik_v3.0.0-beta5_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Wed, 29 Nov 2023 23:16:58 GMT
EXPOSE 80
# Wed, 29 Nov 2023 23:16:58 GMT
ENTRYPOINT ["/traefik"]
# Wed, 29 Nov 2023 23:16:59 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta5 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:65d3a54963132deb3b7e269bda91707f12702256902f4c90d487ccb21b9d558a`  
		Last Modified: Wed, 29 Nov 2023 23:17:45 GMT  
		Size: 41.8 MB (41825821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbce753338c510a600c4f528fabd498bd13a6342d0cd4f58552ee481c98faf41`  
		Last Modified: Wed, 29 Nov 2023 23:17:35 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41c981bb20ef7dfa9d3f71feb1f2448764c30f56e450431f1c52686bdd4b87de`  
		Last Modified: Wed, 29 Nov 2023 23:17:36 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b828c19e9a4c0fd32592a6e14895b39c96566702494253d5f316348902749062`  
		Last Modified: Wed, 29 Nov 2023 23:17:35 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:windowsservercore-1809`

```console
$ docker pull traefik@sha256:4009a9c08e8ff3f3a8215cfc2bcce0355913c9800985c58828d1c7cba68572d6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.5122; amd64

### `traefik:windowsservercore-1809` - windows version 10.0.17763.5122; amd64

```console
$ docker pull traefik@sha256:3f007c45153ec0b2e3abe2b3c7c09b093532d0e198ef4b673e4ddd07bf87ea62
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2098146309 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:84386f59fd9c10dc0607ccebed700b43ed3f66ebfbc4b235398ca2a53bb6dce2`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Thu, 09 Nov 2023 17:56:40 GMT
RUN Install update 10.0.17763.5122
# Thu, 16 Nov 2023 01:37:58 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 29 Nov 2023 02:37:05 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.10.6/traefik_v2.10.6_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Wed, 29 Nov 2023 02:37:06 GMT
EXPOSE 80
# Wed, 29 Nov 2023 02:37:07 GMT
ENTRYPOINT ["/traefik"]
# Wed, 29 Nov 2023 02:37:08 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.6 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:fba9e80c0146453b6de8f35aea2ae18481cf6436bd532c51c90bd2e049433406`  
		Last Modified: Wed, 29 Nov 2023 02:37:46 GMT  
		Size: 40.7 MB (40709104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b54955fdd93b60b49068aadb447e1dbe066720ae5efaa7a315e4592abdd138b0`  
		Last Modified: Wed, 29 Nov 2023 02:37:37 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:463cbb8cb23bb46d13942b85ea410666ef2e97489fb170a77eeaa91dd2f7ae9f`  
		Last Modified: Wed, 29 Nov 2023 02:37:37 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fb9c1cd767d2004163dd2c4b6bb806605d40ff4f8fa90589edef410642f5e41`  
		Last Modified: Wed, 29 Nov 2023 02:37:37 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
