<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `traefik`

-	[`traefik:2.10`](#traefik210)
-	[`traefik:2.10-windowsservercore-1809`](#traefik210-windowsservercore-1809)
-	[`traefik:2.10.4`](#traefik2104)
-	[`traefik:2.10.4-windowsservercore-1809`](#traefik2104-windowsservercore-1809)
-	[`traefik:3.0`](#traefik30)
-	[`traefik:3.0-windowsservercore-1809`](#traefik30-windowsservercore-1809)
-	[`traefik:3.0.0-beta3`](#traefik300-beta3)
-	[`traefik:3.0.0-beta3-windowsservercore-1809`](#traefik300-beta3-windowsservercore-1809)
-	[`traefik:beaufort`](#traefikbeaufort)
-	[`traefik:beaufort-windowsservercore-1809`](#traefikbeaufort-windowsservercore-1809)
-	[`traefik:latest`](#traefiklatest)
-	[`traefik:saintmarcelin`](#traefiksaintmarcelin)
-	[`traefik:saintmarcelin-windowsservercore-1809`](#traefiksaintmarcelin-windowsservercore-1809)
-	[`traefik:v2.10`](#traefikv210)
-	[`traefik:v2.10-windowsservercore-1809`](#traefikv210-windowsservercore-1809)
-	[`traefik:v2.10.4`](#traefikv2104)
-	[`traefik:v2.10.4-windowsservercore-1809`](#traefikv2104-windowsservercore-1809)
-	[`traefik:v3.0`](#traefikv30)
-	[`traefik:v3.0-windowsservercore-1809`](#traefikv30-windowsservercore-1809)
-	[`traefik:v3.0.0-beta3`](#traefikv300-beta3)
-	[`traefik:v3.0.0-beta3-windowsservercore-1809`](#traefikv300-beta3-windowsservercore-1809)
-	[`traefik:windowsservercore-1809`](#traefikwindowsservercore-1809)

## `traefik:2.10`

```console
$ docker pull traefik@sha256:50168bc91ccb8f44db127d6fbd45fba8e72dd704e1ac0c850406dd377a4ae140
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:2.10` - linux; amd64

```console
$ docker pull traefik@sha256:57b2516b7549c4f59531bb09311a54a05af237670676529249c3c0b8e58ad0f3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.4 MB (42384635 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ae1addee1b2f3bd2ff67edf06e8cf028e1ca44f99a6fbf51dfb0b2eec546949`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:20 GMT
ADD file:32ff5e7a78b890996ee4681cc0a26185d3e9acdb4eb1e2aaccb2411f922fed6b in / 
# Mon, 07 Aug 2023 19:20:20 GMT
CMD ["/bin/sh"]
# Wed, 09 Aug 2023 04:06:24 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 09 Aug 2023 04:06:36 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.4/traefik_v2.10.4_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 09 Aug 2023 04:06:36 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 09 Aug 2023 04:06:36 GMT
EXPOSE 80
# Wed, 09 Aug 2023 04:06:36 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 09 Aug 2023 04:06:36 GMT
CMD ["traefik"]
# Wed, 09 Aug 2023 04:06:36 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.4 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:7264a8db6415046d36d16ba98b79778e18accee6ffa71850405994cffa9be7de`  
		Last Modified: Mon, 07 Aug 2023 19:20:54 GMT  
		Size: 3.4 MB (3401613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af32133391e63d8b260bd5a6dca0e380b088a7c2cfe9b6882dd7567b97bf5c84`  
		Last Modified: Wed, 09 Aug 2023 04:06:50 GMT  
		Size: 622.3 KB (622281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1022d3e6eb6de11e14cfcea2b297e20657615293e82e4c1a28cc6888c3727fc6`  
		Last Modified: Wed, 09 Aug 2023 04:07:16 GMT  
		Size: 38.4 MB (38360374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef9401db61432baa70472973f37408025b1240d1762e184bf6ab77f1ea68c85b`  
		Last Modified: Wed, 09 Aug 2023 04:07:10 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.10` - linux; arm variant v6

```console
$ docker pull traefik@sha256:bcf37f90bb3c148ecc6c642f0a5ef7ecca69c107f5055a24e94de6b178038ee3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.9 MB (39897744 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b470a25273a17965c4195798705c8c434dec9e1dcb8bed0e25cd4afd15e5a1df`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 07 Aug 2023 19:49:14 GMT
ADD file:9882e99e5f94ab2db05c029648ac5be7cf0f063a8701394fcbb543a7ef5d4b90 in / 
# Mon, 07 Aug 2023 19:49:15 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 23:36:43 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 08 Aug 2023 23:36:56 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.4/traefik_v2.10.4_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Tue, 08 Aug 2023 23:36:56 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 08 Aug 2023 23:36:56 GMT
EXPOSE 80
# Tue, 08 Aug 2023 23:36:56 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 08 Aug 2023 23:36:56 GMT
CMD ["traefik"]
# Tue, 08 Aug 2023 23:36:56 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.4 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:af09961d4a43b504efc76e38b50918977c28be73eeb8b926247783a00e8b9f2f`  
		Last Modified: Mon, 07 Aug 2023 19:49:38 GMT  
		Size: 3.1 MB (3144809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f8cc6c7cf0fb882727ce9bdded1e9477cf9f51f27f262ddd2837ce010c75546`  
		Last Modified: Tue, 08 Aug 2023 23:37:08 GMT  
		Size: 622.7 KB (622688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53f350ea2c1577d6f498d27752f1efc8de8aea15ad9cc2c8ac411a406fc06474`  
		Last Modified: Tue, 08 Aug 2023 23:37:34 GMT  
		Size: 36.1 MB (36129878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbc4c23d6ff9206d00fa66fef11f0d9010dd364ced1cff33b54909008c2add1a`  
		Last Modified: Tue, 08 Aug 2023 23:37:28 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.10` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:a56dcbeb82281b0ac99297d226195215f747242daa5a2213de02d8a09a6d9cfd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.1 MB (39136580 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0791754faa9d789eea8f305cf76a58f17b97c6b2fc5a2a32bfeb7bf3cf1ee8e2`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:19 GMT
ADD file:b2e7eaa7e41f08853dbe08d84439a7f9fd32fc58c3aa1e298f3f60343b2b683a in / 
# Mon, 07 Aug 2023 19:39:19 GMT
CMD ["/bin/sh"]
# Wed, 09 Aug 2023 04:26:52 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 09 Aug 2023 04:27:02 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.4/traefik_v2.10.4_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 09 Aug 2023 04:27:02 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 09 Aug 2023 04:27:02 GMT
EXPOSE 80
# Wed, 09 Aug 2023 04:27:02 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 09 Aug 2023 04:27:02 GMT
CMD ["traefik"]
# Wed, 09 Aug 2023 04:27:02 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.4 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:9fda8d8052c61740409c4bea888859c141fd8cc3f58ac61943144ff6d1681b2d`  
		Last Modified: Mon, 07 Aug 2023 19:39:45 GMT  
		Size: 3.3 MB (3330767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dffff58315ee746797a9f6d4ec2d858fca66532fa8ec5993ab228e70ec0dda7d`  
		Last Modified: Wed, 09 Aug 2023 04:27:14 GMT  
		Size: 624.5 KB (624509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3973374f4924c913ca3c30a39dd6be20f06314a673c7607d4d43b90643d7e21d`  
		Last Modified: Wed, 09 Aug 2023 04:27:39 GMT  
		Size: 35.2 MB (35180936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b4e902bb4f65830c8bcefc8a4ca424e5cce78a9f8843454b0194b9f7080c140`  
		Last Modified: Wed, 09 Aug 2023 04:27:34 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.10` - linux; s390x

```console
$ docker pull traefik@sha256:755c4c3891db8f6b955c25fe3e19442bd0792ca28459f10fc3005e79776683e9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.0 MB (41034756 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:49fb49ad4398f43080e4b15ecb86663f7b9d33fd3394c2dbe5b85a61eea53998`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 28 Sep 2023 20:41:43 GMT
ADD file:fd3808a676fc56c1380e55b2ddbf4014d9371346cf789860b336bc9f00729ed0 in / 
# Thu, 28 Sep 2023 20:41:44 GMT
CMD ["/bin/sh"]
# Fri, 29 Sep 2023 00:15:10 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 29 Sep 2023 00:15:31 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.4/traefik_v2.10.4_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 29 Sep 2023 00:15:33 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 29 Sep 2023 00:15:33 GMT
EXPOSE 80
# Fri, 29 Sep 2023 00:15:34 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 29 Sep 2023 00:15:34 GMT
CMD ["traefik"]
# Fri, 29 Sep 2023 00:15:34 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.4 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:ddc123c7bae83a141fb0dc9f96de9910cfa54eb022ebb63bc8d191aec93dc97c`  
		Last Modified: Fri, 29 Sep 2023 00:16:13 GMT  
		Size: 37.2 MB (37196446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1ddc7c72004c2240bdeb82301ae59b70bacbd4aa31b3c18768ba03db4a96b8b`  
		Last Modified: Fri, 29 Sep 2023 00:16:07 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:2.10-windowsservercore-1809`

```console
$ docker pull traefik@sha256:8c809f2d7759cb331e6787e80637611f0df573ae584057252a404949d93176c6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4851; amd64

### `traefik:2.10-windowsservercore-1809` - windows version 10.0.17763.4851; amd64

```console
$ docker pull traefik@sha256:162622cb7682b3e6f3274106c7920c71adb69ea58ca89fa282e2ab7c33275f26
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2055286197 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:96ca8a25a6214a37c560d4a7e85db466ec7af762962f6ebe1350bb0e0ffeb03c`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Tue, 29 Aug 2023 17:09:18 GMT
RUN Install update 10.0.17763.4851
# Wed, 13 Sep 2023 01:39:13 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Sep 2023 08:35:18 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.10.4/traefik_v2.10.4_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Wed, 13 Sep 2023 08:35:19 GMT
EXPOSE 80
# Wed, 13 Sep 2023 08:35:20 GMT
ENTRYPOINT ["/traefik"]
# Wed, 13 Sep 2023 08:35:21 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.4 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:179757339e051b99f9a62375fed8f87ffcc4df0eeedb984d20b485bdd089ad08`  
		Last Modified: Tue, 12 Sep 2023 19:41:25 GMT  
		Size: 365.7 MB (365709508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdc14cbf6230cebb55cabf885ef8606e63f571dd05f37d899d95bca34972a44a`  
		Last Modified: Wed, 13 Sep 2023 02:16:50 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f02f28ba2ad38d851b3d6f506b4a28243717438129c2627a3492d29c08c6d5d`  
		Last Modified: Wed, 13 Sep 2023 08:36:16 GMT  
		Size: 39.0 MB (38950677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcf8cada8a7cfe4fa87db7be051abb4ec4a26637f91f6404bfce2664ea81dc64`  
		Last Modified: Wed, 13 Sep 2023 08:36:07 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2528ac6fcf0f3b42b632849e634ea6b05511b961bee203c0f893835f04664e6c`  
		Last Modified: Wed, 13 Sep 2023 08:36:08 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6487c7270b3462ca9295dd9a569d4ed3b821aa3f7be16a73d895e3483a3165f5`  
		Last Modified: Wed, 13 Sep 2023 08:36:07 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:2.10.4`

```console
$ docker pull traefik@sha256:50168bc91ccb8f44db127d6fbd45fba8e72dd704e1ac0c850406dd377a4ae140
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:2.10.4` - linux; amd64

```console
$ docker pull traefik@sha256:57b2516b7549c4f59531bb09311a54a05af237670676529249c3c0b8e58ad0f3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.4 MB (42384635 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ae1addee1b2f3bd2ff67edf06e8cf028e1ca44f99a6fbf51dfb0b2eec546949`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:20 GMT
ADD file:32ff5e7a78b890996ee4681cc0a26185d3e9acdb4eb1e2aaccb2411f922fed6b in / 
# Mon, 07 Aug 2023 19:20:20 GMT
CMD ["/bin/sh"]
# Wed, 09 Aug 2023 04:06:24 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 09 Aug 2023 04:06:36 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.4/traefik_v2.10.4_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 09 Aug 2023 04:06:36 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 09 Aug 2023 04:06:36 GMT
EXPOSE 80
# Wed, 09 Aug 2023 04:06:36 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 09 Aug 2023 04:06:36 GMT
CMD ["traefik"]
# Wed, 09 Aug 2023 04:06:36 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.4 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:7264a8db6415046d36d16ba98b79778e18accee6ffa71850405994cffa9be7de`  
		Last Modified: Mon, 07 Aug 2023 19:20:54 GMT  
		Size: 3.4 MB (3401613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af32133391e63d8b260bd5a6dca0e380b088a7c2cfe9b6882dd7567b97bf5c84`  
		Last Modified: Wed, 09 Aug 2023 04:06:50 GMT  
		Size: 622.3 KB (622281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1022d3e6eb6de11e14cfcea2b297e20657615293e82e4c1a28cc6888c3727fc6`  
		Last Modified: Wed, 09 Aug 2023 04:07:16 GMT  
		Size: 38.4 MB (38360374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef9401db61432baa70472973f37408025b1240d1762e184bf6ab77f1ea68c85b`  
		Last Modified: Wed, 09 Aug 2023 04:07:10 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.10.4` - linux; arm variant v6

```console
$ docker pull traefik@sha256:bcf37f90bb3c148ecc6c642f0a5ef7ecca69c107f5055a24e94de6b178038ee3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.9 MB (39897744 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b470a25273a17965c4195798705c8c434dec9e1dcb8bed0e25cd4afd15e5a1df`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 07 Aug 2023 19:49:14 GMT
ADD file:9882e99e5f94ab2db05c029648ac5be7cf0f063a8701394fcbb543a7ef5d4b90 in / 
# Mon, 07 Aug 2023 19:49:15 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 23:36:43 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 08 Aug 2023 23:36:56 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.4/traefik_v2.10.4_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Tue, 08 Aug 2023 23:36:56 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 08 Aug 2023 23:36:56 GMT
EXPOSE 80
# Tue, 08 Aug 2023 23:36:56 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 08 Aug 2023 23:36:56 GMT
CMD ["traefik"]
# Tue, 08 Aug 2023 23:36:56 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.4 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:af09961d4a43b504efc76e38b50918977c28be73eeb8b926247783a00e8b9f2f`  
		Last Modified: Mon, 07 Aug 2023 19:49:38 GMT  
		Size: 3.1 MB (3144809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f8cc6c7cf0fb882727ce9bdded1e9477cf9f51f27f262ddd2837ce010c75546`  
		Last Modified: Tue, 08 Aug 2023 23:37:08 GMT  
		Size: 622.7 KB (622688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53f350ea2c1577d6f498d27752f1efc8de8aea15ad9cc2c8ac411a406fc06474`  
		Last Modified: Tue, 08 Aug 2023 23:37:34 GMT  
		Size: 36.1 MB (36129878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbc4c23d6ff9206d00fa66fef11f0d9010dd364ced1cff33b54909008c2add1a`  
		Last Modified: Tue, 08 Aug 2023 23:37:28 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.10.4` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:a56dcbeb82281b0ac99297d226195215f747242daa5a2213de02d8a09a6d9cfd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.1 MB (39136580 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0791754faa9d789eea8f305cf76a58f17b97c6b2fc5a2a32bfeb7bf3cf1ee8e2`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:19 GMT
ADD file:b2e7eaa7e41f08853dbe08d84439a7f9fd32fc58c3aa1e298f3f60343b2b683a in / 
# Mon, 07 Aug 2023 19:39:19 GMT
CMD ["/bin/sh"]
# Wed, 09 Aug 2023 04:26:52 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 09 Aug 2023 04:27:02 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.4/traefik_v2.10.4_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 09 Aug 2023 04:27:02 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 09 Aug 2023 04:27:02 GMT
EXPOSE 80
# Wed, 09 Aug 2023 04:27:02 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 09 Aug 2023 04:27:02 GMT
CMD ["traefik"]
# Wed, 09 Aug 2023 04:27:02 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.4 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:9fda8d8052c61740409c4bea888859c141fd8cc3f58ac61943144ff6d1681b2d`  
		Last Modified: Mon, 07 Aug 2023 19:39:45 GMT  
		Size: 3.3 MB (3330767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dffff58315ee746797a9f6d4ec2d858fca66532fa8ec5993ab228e70ec0dda7d`  
		Last Modified: Wed, 09 Aug 2023 04:27:14 GMT  
		Size: 624.5 KB (624509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3973374f4924c913ca3c30a39dd6be20f06314a673c7607d4d43b90643d7e21d`  
		Last Modified: Wed, 09 Aug 2023 04:27:39 GMT  
		Size: 35.2 MB (35180936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b4e902bb4f65830c8bcefc8a4ca424e5cce78a9f8843454b0194b9f7080c140`  
		Last Modified: Wed, 09 Aug 2023 04:27:34 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.10.4` - linux; s390x

```console
$ docker pull traefik@sha256:755c4c3891db8f6b955c25fe3e19442bd0792ca28459f10fc3005e79776683e9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.0 MB (41034756 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:49fb49ad4398f43080e4b15ecb86663f7b9d33fd3394c2dbe5b85a61eea53998`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 28 Sep 2023 20:41:43 GMT
ADD file:fd3808a676fc56c1380e55b2ddbf4014d9371346cf789860b336bc9f00729ed0 in / 
# Thu, 28 Sep 2023 20:41:44 GMT
CMD ["/bin/sh"]
# Fri, 29 Sep 2023 00:15:10 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 29 Sep 2023 00:15:31 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.4/traefik_v2.10.4_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 29 Sep 2023 00:15:33 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 29 Sep 2023 00:15:33 GMT
EXPOSE 80
# Fri, 29 Sep 2023 00:15:34 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 29 Sep 2023 00:15:34 GMT
CMD ["traefik"]
# Fri, 29 Sep 2023 00:15:34 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.4 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:ddc123c7bae83a141fb0dc9f96de9910cfa54eb022ebb63bc8d191aec93dc97c`  
		Last Modified: Fri, 29 Sep 2023 00:16:13 GMT  
		Size: 37.2 MB (37196446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1ddc7c72004c2240bdeb82301ae59b70bacbd4aa31b3c18768ba03db4a96b8b`  
		Last Modified: Fri, 29 Sep 2023 00:16:07 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:2.10.4-windowsservercore-1809`

```console
$ docker pull traefik@sha256:8c809f2d7759cb331e6787e80637611f0df573ae584057252a404949d93176c6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4851; amd64

### `traefik:2.10.4-windowsservercore-1809` - windows version 10.0.17763.4851; amd64

```console
$ docker pull traefik@sha256:162622cb7682b3e6f3274106c7920c71adb69ea58ca89fa282e2ab7c33275f26
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2055286197 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:96ca8a25a6214a37c560d4a7e85db466ec7af762962f6ebe1350bb0e0ffeb03c`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Tue, 29 Aug 2023 17:09:18 GMT
RUN Install update 10.0.17763.4851
# Wed, 13 Sep 2023 01:39:13 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Sep 2023 08:35:18 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.10.4/traefik_v2.10.4_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Wed, 13 Sep 2023 08:35:19 GMT
EXPOSE 80
# Wed, 13 Sep 2023 08:35:20 GMT
ENTRYPOINT ["/traefik"]
# Wed, 13 Sep 2023 08:35:21 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.4 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:179757339e051b99f9a62375fed8f87ffcc4df0eeedb984d20b485bdd089ad08`  
		Last Modified: Tue, 12 Sep 2023 19:41:25 GMT  
		Size: 365.7 MB (365709508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdc14cbf6230cebb55cabf885ef8606e63f571dd05f37d899d95bca34972a44a`  
		Last Modified: Wed, 13 Sep 2023 02:16:50 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f02f28ba2ad38d851b3d6f506b4a28243717438129c2627a3492d29c08c6d5d`  
		Last Modified: Wed, 13 Sep 2023 08:36:16 GMT  
		Size: 39.0 MB (38950677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcf8cada8a7cfe4fa87db7be051abb4ec4a26637f91f6404bfce2664ea81dc64`  
		Last Modified: Wed, 13 Sep 2023 08:36:07 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2528ac6fcf0f3b42b632849e634ea6b05511b961bee203c0f893835f04664e6c`  
		Last Modified: Wed, 13 Sep 2023 08:36:08 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6487c7270b3462ca9295dd9a569d4ed3b821aa3f7be16a73d895e3483a3165f5`  
		Last Modified: Wed, 13 Sep 2023 08:36:07 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:3.0`

```console
$ docker pull traefik@sha256:5c18ddd7402cf0a0dfffd4e8b451e5b09018116ee06010d0e9a243e6c3e80cea
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:3.0` - linux; amd64

```console
$ docker pull traefik@sha256:db21af65fb9edaa04542efe69bb6ba74afa04231874b0240fcccb059547fbf24
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.3 MB (42339283 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99d2af65616272cb94e6157ff2c162b2949d831dfe72e5de461e32db2f458951`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:20 GMT
ADD file:32ff5e7a78b890996ee4681cc0a26185d3e9acdb4eb1e2aaccb2411f922fed6b in / 
# Mon, 07 Aug 2023 19:20:20 GMT
CMD ["/bin/sh"]
# Wed, 09 Aug 2023 04:06:24 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 09 Aug 2023 04:06:28 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta3/traefik_v3.0.0-beta3_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 09 Aug 2023 04:06:28 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 09 Aug 2023 04:06:28 GMT
EXPOSE 80
# Wed, 09 Aug 2023 04:06:28 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 09 Aug 2023 04:06:28 GMT
CMD ["traefik"]
# Wed, 09 Aug 2023 04:06:28 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta3 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:7264a8db6415046d36d16ba98b79778e18accee6ffa71850405994cffa9be7de`  
		Last Modified: Mon, 07 Aug 2023 19:20:54 GMT  
		Size: 3.4 MB (3401613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af32133391e63d8b260bd5a6dca0e380b088a7c2cfe9b6882dd7567b97bf5c84`  
		Last Modified: Wed, 09 Aug 2023 04:06:50 GMT  
		Size: 622.3 KB (622281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a3fb410d5ad92d4b790c3aeff36ea3d4e6d1768c3d58cd9fadb8f574f8eb24a`  
		Last Modified: Wed, 09 Aug 2023 04:06:55 GMT  
		Size: 38.3 MB (38315021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25020b7f93004e310f3a03e903db4f1ba8ae45d9a5b5b3a594da55f18b0bc663`  
		Last Modified: Wed, 09 Aug 2023 04:06:50 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:3.0` - linux; arm variant v6

```console
$ docker pull traefik@sha256:4610ad0a08abfd441d5efea592fc370ab772915d5d62a4fe1b6ad57f5b1f7a17
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.8 MB (39834746 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14c7857053ace4e793ccb85ef5e4f7039d5b2d69ef3bba2091533f1eac50eb57`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 07 Aug 2023 19:49:14 GMT
ADD file:9882e99e5f94ab2db05c029648ac5be7cf0f063a8701394fcbb543a7ef5d4b90 in / 
# Mon, 07 Aug 2023 19:49:15 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 23:36:43 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 08 Aug 2023 23:36:47 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta3/traefik_v3.0.0-beta3_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Tue, 08 Aug 2023 23:36:48 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 08 Aug 2023 23:36:48 GMT
EXPOSE 80
# Tue, 08 Aug 2023 23:36:48 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 08 Aug 2023 23:36:48 GMT
CMD ["traefik"]
# Tue, 08 Aug 2023 23:36:48 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta3 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:af09961d4a43b504efc76e38b50918977c28be73eeb8b926247783a00e8b9f2f`  
		Last Modified: Mon, 07 Aug 2023 19:49:38 GMT  
		Size: 3.1 MB (3144809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f8cc6c7cf0fb882727ce9bdded1e9477cf9f51f27f262ddd2837ce010c75546`  
		Last Modified: Tue, 08 Aug 2023 23:37:08 GMT  
		Size: 622.7 KB (622688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13a56f8f3e28824e8aeed3179006a8bacb5ea8697429ecdcf4b3313a11531872`  
		Last Modified: Tue, 08 Aug 2023 23:37:14 GMT  
		Size: 36.1 MB (36066881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b4c24374a077bea1e909f5b61e43515993be1be29aacd3aef10a445d1447b70`  
		Last Modified: Tue, 08 Aug 2023 23:37:08 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:3.0` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:a4ccc52aa5d73f85d580e98cccd048575c4dd1cb3f4903a81e5f370edeb13845
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.1 MB (39098171 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8be29ac05708d11224070a2badc6d648a7b7494276deafffa559dece31419b37`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:19 GMT
ADD file:b2e7eaa7e41f08853dbe08d84439a7f9fd32fc58c3aa1e298f3f60343b2b683a in / 
# Mon, 07 Aug 2023 19:39:19 GMT
CMD ["/bin/sh"]
# Wed, 09 Aug 2023 04:26:52 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 09 Aug 2023 04:26:55 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta3/traefik_v3.0.0-beta3_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 09 Aug 2023 04:26:56 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 09 Aug 2023 04:26:56 GMT
EXPOSE 80
# Wed, 09 Aug 2023 04:26:56 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 09 Aug 2023 04:26:56 GMT
CMD ["traefik"]
# Wed, 09 Aug 2023 04:26:56 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta3 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:9fda8d8052c61740409c4bea888859c141fd8cc3f58ac61943144ff6d1681b2d`  
		Last Modified: Mon, 07 Aug 2023 19:39:45 GMT  
		Size: 3.3 MB (3330767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dffff58315ee746797a9f6d4ec2d858fca66532fa8ec5993ab228e70ec0dda7d`  
		Last Modified: Wed, 09 Aug 2023 04:27:14 GMT  
		Size: 624.5 KB (624509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdeef0a315984700bca8a1be11d88d1531de6244904ee7fd95bf207f107a61a7`  
		Last Modified: Wed, 09 Aug 2023 04:27:18 GMT  
		Size: 35.1 MB (35142527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f464f3b71f2555dfe7d1254a4847862866df2628d5e79e21597c596903c530ec`  
		Last Modified: Wed, 09 Aug 2023 04:27:13 GMT  
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
$ docker pull traefik@sha256:dab2b4b52465d429b1bf5b84ffa38c085ea1c00af3121846acd69ab445b4083e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4851; amd64

### `traefik:3.0-windowsservercore-1809` - windows version 10.0.17763.4851; amd64

```console
$ docker pull traefik@sha256:dee2708e034f9398d1df57ca83b286b95a461705193b858a5b845bb5eec8a7b4
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2055247019 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a29344f9d48c4d86ae52a026fbef4ef800a05ecf2a4fe72457d759dd3615d0b`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Tue, 29 Aug 2023 17:09:18 GMT
RUN Install update 10.0.17763.4851
# Wed, 13 Sep 2023 01:39:13 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Sep 2023 08:33:49 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v3.0.0-beta3/traefik_v3.0.0-beta3_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Wed, 13 Sep 2023 08:33:50 GMT
EXPOSE 80
# Wed, 13 Sep 2023 08:33:50 GMT
ENTRYPOINT ["/traefik"]
# Wed, 13 Sep 2023 08:33:51 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta3 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:179757339e051b99f9a62375fed8f87ffcc4df0eeedb984d20b485bdd089ad08`  
		Last Modified: Tue, 12 Sep 2023 19:41:25 GMT  
		Size: 365.7 MB (365709508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdc14cbf6230cebb55cabf885ef8606e63f571dd05f37d899d95bca34972a44a`  
		Last Modified: Wed, 13 Sep 2023 02:16:50 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4761997e52cfb63512b90853905a746fd9fd54e41674e2d4bcbb1cb8201dd8e6`  
		Last Modified: Wed, 13 Sep 2023 08:35:53 GMT  
		Size: 38.9 MB (38911475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68336a56fcbfa87a1c489e6104360ab265abb53897306e3d4b09b6a7649bcc28`  
		Last Modified: Wed, 13 Sep 2023 08:35:44 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25e209029cdcd07d20e5a87b03da02a4e8a0c69006f4837fb0d0eb73571be80d`  
		Last Modified: Wed, 13 Sep 2023 08:35:44 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00a7cd492baf3537340fe6d001aa41f13f04e92943dc5fc877ffb6a51926b4db`  
		Last Modified: Wed, 13 Sep 2023 08:35:43 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:3.0.0-beta3`

```console
$ docker pull traefik@sha256:5c18ddd7402cf0a0dfffd4e8b451e5b09018116ee06010d0e9a243e6c3e80cea
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:3.0.0-beta3` - linux; amd64

```console
$ docker pull traefik@sha256:db21af65fb9edaa04542efe69bb6ba74afa04231874b0240fcccb059547fbf24
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.3 MB (42339283 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99d2af65616272cb94e6157ff2c162b2949d831dfe72e5de461e32db2f458951`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:20 GMT
ADD file:32ff5e7a78b890996ee4681cc0a26185d3e9acdb4eb1e2aaccb2411f922fed6b in / 
# Mon, 07 Aug 2023 19:20:20 GMT
CMD ["/bin/sh"]
# Wed, 09 Aug 2023 04:06:24 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 09 Aug 2023 04:06:28 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta3/traefik_v3.0.0-beta3_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 09 Aug 2023 04:06:28 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 09 Aug 2023 04:06:28 GMT
EXPOSE 80
# Wed, 09 Aug 2023 04:06:28 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 09 Aug 2023 04:06:28 GMT
CMD ["traefik"]
# Wed, 09 Aug 2023 04:06:28 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta3 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:7264a8db6415046d36d16ba98b79778e18accee6ffa71850405994cffa9be7de`  
		Last Modified: Mon, 07 Aug 2023 19:20:54 GMT  
		Size: 3.4 MB (3401613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af32133391e63d8b260bd5a6dca0e380b088a7c2cfe9b6882dd7567b97bf5c84`  
		Last Modified: Wed, 09 Aug 2023 04:06:50 GMT  
		Size: 622.3 KB (622281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a3fb410d5ad92d4b790c3aeff36ea3d4e6d1768c3d58cd9fadb8f574f8eb24a`  
		Last Modified: Wed, 09 Aug 2023 04:06:55 GMT  
		Size: 38.3 MB (38315021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25020b7f93004e310f3a03e903db4f1ba8ae45d9a5b5b3a594da55f18b0bc663`  
		Last Modified: Wed, 09 Aug 2023 04:06:50 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:3.0.0-beta3` - linux; arm variant v6

```console
$ docker pull traefik@sha256:4610ad0a08abfd441d5efea592fc370ab772915d5d62a4fe1b6ad57f5b1f7a17
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.8 MB (39834746 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14c7857053ace4e793ccb85ef5e4f7039d5b2d69ef3bba2091533f1eac50eb57`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 07 Aug 2023 19:49:14 GMT
ADD file:9882e99e5f94ab2db05c029648ac5be7cf0f063a8701394fcbb543a7ef5d4b90 in / 
# Mon, 07 Aug 2023 19:49:15 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 23:36:43 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 08 Aug 2023 23:36:47 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta3/traefik_v3.0.0-beta3_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Tue, 08 Aug 2023 23:36:48 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 08 Aug 2023 23:36:48 GMT
EXPOSE 80
# Tue, 08 Aug 2023 23:36:48 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 08 Aug 2023 23:36:48 GMT
CMD ["traefik"]
# Tue, 08 Aug 2023 23:36:48 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta3 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:af09961d4a43b504efc76e38b50918977c28be73eeb8b926247783a00e8b9f2f`  
		Last Modified: Mon, 07 Aug 2023 19:49:38 GMT  
		Size: 3.1 MB (3144809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f8cc6c7cf0fb882727ce9bdded1e9477cf9f51f27f262ddd2837ce010c75546`  
		Last Modified: Tue, 08 Aug 2023 23:37:08 GMT  
		Size: 622.7 KB (622688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13a56f8f3e28824e8aeed3179006a8bacb5ea8697429ecdcf4b3313a11531872`  
		Last Modified: Tue, 08 Aug 2023 23:37:14 GMT  
		Size: 36.1 MB (36066881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b4c24374a077bea1e909f5b61e43515993be1be29aacd3aef10a445d1447b70`  
		Last Modified: Tue, 08 Aug 2023 23:37:08 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:3.0.0-beta3` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:a4ccc52aa5d73f85d580e98cccd048575c4dd1cb3f4903a81e5f370edeb13845
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.1 MB (39098171 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8be29ac05708d11224070a2badc6d648a7b7494276deafffa559dece31419b37`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:19 GMT
ADD file:b2e7eaa7e41f08853dbe08d84439a7f9fd32fc58c3aa1e298f3f60343b2b683a in / 
# Mon, 07 Aug 2023 19:39:19 GMT
CMD ["/bin/sh"]
# Wed, 09 Aug 2023 04:26:52 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 09 Aug 2023 04:26:55 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta3/traefik_v3.0.0-beta3_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 09 Aug 2023 04:26:56 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 09 Aug 2023 04:26:56 GMT
EXPOSE 80
# Wed, 09 Aug 2023 04:26:56 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 09 Aug 2023 04:26:56 GMT
CMD ["traefik"]
# Wed, 09 Aug 2023 04:26:56 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta3 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:9fda8d8052c61740409c4bea888859c141fd8cc3f58ac61943144ff6d1681b2d`  
		Last Modified: Mon, 07 Aug 2023 19:39:45 GMT  
		Size: 3.3 MB (3330767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dffff58315ee746797a9f6d4ec2d858fca66532fa8ec5993ab228e70ec0dda7d`  
		Last Modified: Wed, 09 Aug 2023 04:27:14 GMT  
		Size: 624.5 KB (624509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdeef0a315984700bca8a1be11d88d1531de6244904ee7fd95bf207f107a61a7`  
		Last Modified: Wed, 09 Aug 2023 04:27:18 GMT  
		Size: 35.1 MB (35142527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f464f3b71f2555dfe7d1254a4847862866df2628d5e79e21597c596903c530ec`  
		Last Modified: Wed, 09 Aug 2023 04:27:13 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:3.0.0-beta3` - linux; s390x

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

## `traefik:3.0.0-beta3-windowsservercore-1809`

```console
$ docker pull traefik@sha256:dab2b4b52465d429b1bf5b84ffa38c085ea1c00af3121846acd69ab445b4083e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4851; amd64

### `traefik:3.0.0-beta3-windowsservercore-1809` - windows version 10.0.17763.4851; amd64

```console
$ docker pull traefik@sha256:dee2708e034f9398d1df57ca83b286b95a461705193b858a5b845bb5eec8a7b4
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2055247019 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a29344f9d48c4d86ae52a026fbef4ef800a05ecf2a4fe72457d759dd3615d0b`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Tue, 29 Aug 2023 17:09:18 GMT
RUN Install update 10.0.17763.4851
# Wed, 13 Sep 2023 01:39:13 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Sep 2023 08:33:49 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v3.0.0-beta3/traefik_v3.0.0-beta3_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Wed, 13 Sep 2023 08:33:50 GMT
EXPOSE 80
# Wed, 13 Sep 2023 08:33:50 GMT
ENTRYPOINT ["/traefik"]
# Wed, 13 Sep 2023 08:33:51 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta3 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:179757339e051b99f9a62375fed8f87ffcc4df0eeedb984d20b485bdd089ad08`  
		Last Modified: Tue, 12 Sep 2023 19:41:25 GMT  
		Size: 365.7 MB (365709508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdc14cbf6230cebb55cabf885ef8606e63f571dd05f37d899d95bca34972a44a`  
		Last Modified: Wed, 13 Sep 2023 02:16:50 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4761997e52cfb63512b90853905a746fd9fd54e41674e2d4bcbb1cb8201dd8e6`  
		Last Modified: Wed, 13 Sep 2023 08:35:53 GMT  
		Size: 38.9 MB (38911475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68336a56fcbfa87a1c489e6104360ab265abb53897306e3d4b09b6a7649bcc28`  
		Last Modified: Wed, 13 Sep 2023 08:35:44 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25e209029cdcd07d20e5a87b03da02a4e8a0c69006f4837fb0d0eb73571be80d`  
		Last Modified: Wed, 13 Sep 2023 08:35:44 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00a7cd492baf3537340fe6d001aa41f13f04e92943dc5fc877ffb6a51926b4db`  
		Last Modified: Wed, 13 Sep 2023 08:35:43 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:beaufort`

```console
$ docker pull traefik@sha256:5c18ddd7402cf0a0dfffd4e8b451e5b09018116ee06010d0e9a243e6c3e80cea
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:beaufort` - linux; amd64

```console
$ docker pull traefik@sha256:db21af65fb9edaa04542efe69bb6ba74afa04231874b0240fcccb059547fbf24
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.3 MB (42339283 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99d2af65616272cb94e6157ff2c162b2949d831dfe72e5de461e32db2f458951`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:20 GMT
ADD file:32ff5e7a78b890996ee4681cc0a26185d3e9acdb4eb1e2aaccb2411f922fed6b in / 
# Mon, 07 Aug 2023 19:20:20 GMT
CMD ["/bin/sh"]
# Wed, 09 Aug 2023 04:06:24 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 09 Aug 2023 04:06:28 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta3/traefik_v3.0.0-beta3_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 09 Aug 2023 04:06:28 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 09 Aug 2023 04:06:28 GMT
EXPOSE 80
# Wed, 09 Aug 2023 04:06:28 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 09 Aug 2023 04:06:28 GMT
CMD ["traefik"]
# Wed, 09 Aug 2023 04:06:28 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta3 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:7264a8db6415046d36d16ba98b79778e18accee6ffa71850405994cffa9be7de`  
		Last Modified: Mon, 07 Aug 2023 19:20:54 GMT  
		Size: 3.4 MB (3401613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af32133391e63d8b260bd5a6dca0e380b088a7c2cfe9b6882dd7567b97bf5c84`  
		Last Modified: Wed, 09 Aug 2023 04:06:50 GMT  
		Size: 622.3 KB (622281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a3fb410d5ad92d4b790c3aeff36ea3d4e6d1768c3d58cd9fadb8f574f8eb24a`  
		Last Modified: Wed, 09 Aug 2023 04:06:55 GMT  
		Size: 38.3 MB (38315021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25020b7f93004e310f3a03e903db4f1ba8ae45d9a5b5b3a594da55f18b0bc663`  
		Last Modified: Wed, 09 Aug 2023 04:06:50 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:beaufort` - linux; arm variant v6

```console
$ docker pull traefik@sha256:4610ad0a08abfd441d5efea592fc370ab772915d5d62a4fe1b6ad57f5b1f7a17
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.8 MB (39834746 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14c7857053ace4e793ccb85ef5e4f7039d5b2d69ef3bba2091533f1eac50eb57`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 07 Aug 2023 19:49:14 GMT
ADD file:9882e99e5f94ab2db05c029648ac5be7cf0f063a8701394fcbb543a7ef5d4b90 in / 
# Mon, 07 Aug 2023 19:49:15 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 23:36:43 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 08 Aug 2023 23:36:47 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta3/traefik_v3.0.0-beta3_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Tue, 08 Aug 2023 23:36:48 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 08 Aug 2023 23:36:48 GMT
EXPOSE 80
# Tue, 08 Aug 2023 23:36:48 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 08 Aug 2023 23:36:48 GMT
CMD ["traefik"]
# Tue, 08 Aug 2023 23:36:48 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta3 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:af09961d4a43b504efc76e38b50918977c28be73eeb8b926247783a00e8b9f2f`  
		Last Modified: Mon, 07 Aug 2023 19:49:38 GMT  
		Size: 3.1 MB (3144809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f8cc6c7cf0fb882727ce9bdded1e9477cf9f51f27f262ddd2837ce010c75546`  
		Last Modified: Tue, 08 Aug 2023 23:37:08 GMT  
		Size: 622.7 KB (622688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13a56f8f3e28824e8aeed3179006a8bacb5ea8697429ecdcf4b3313a11531872`  
		Last Modified: Tue, 08 Aug 2023 23:37:14 GMT  
		Size: 36.1 MB (36066881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b4c24374a077bea1e909f5b61e43515993be1be29aacd3aef10a445d1447b70`  
		Last Modified: Tue, 08 Aug 2023 23:37:08 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:beaufort` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:a4ccc52aa5d73f85d580e98cccd048575c4dd1cb3f4903a81e5f370edeb13845
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.1 MB (39098171 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8be29ac05708d11224070a2badc6d648a7b7494276deafffa559dece31419b37`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:19 GMT
ADD file:b2e7eaa7e41f08853dbe08d84439a7f9fd32fc58c3aa1e298f3f60343b2b683a in / 
# Mon, 07 Aug 2023 19:39:19 GMT
CMD ["/bin/sh"]
# Wed, 09 Aug 2023 04:26:52 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 09 Aug 2023 04:26:55 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta3/traefik_v3.0.0-beta3_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 09 Aug 2023 04:26:56 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 09 Aug 2023 04:26:56 GMT
EXPOSE 80
# Wed, 09 Aug 2023 04:26:56 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 09 Aug 2023 04:26:56 GMT
CMD ["traefik"]
# Wed, 09 Aug 2023 04:26:56 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta3 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:9fda8d8052c61740409c4bea888859c141fd8cc3f58ac61943144ff6d1681b2d`  
		Last Modified: Mon, 07 Aug 2023 19:39:45 GMT  
		Size: 3.3 MB (3330767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dffff58315ee746797a9f6d4ec2d858fca66532fa8ec5993ab228e70ec0dda7d`  
		Last Modified: Wed, 09 Aug 2023 04:27:14 GMT  
		Size: 624.5 KB (624509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdeef0a315984700bca8a1be11d88d1531de6244904ee7fd95bf207f107a61a7`  
		Last Modified: Wed, 09 Aug 2023 04:27:18 GMT  
		Size: 35.1 MB (35142527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f464f3b71f2555dfe7d1254a4847862866df2628d5e79e21597c596903c530ec`  
		Last Modified: Wed, 09 Aug 2023 04:27:13 GMT  
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
$ docker pull traefik@sha256:dab2b4b52465d429b1bf5b84ffa38c085ea1c00af3121846acd69ab445b4083e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4851; amd64

### `traefik:beaufort-windowsservercore-1809` - windows version 10.0.17763.4851; amd64

```console
$ docker pull traefik@sha256:dee2708e034f9398d1df57ca83b286b95a461705193b858a5b845bb5eec8a7b4
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2055247019 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a29344f9d48c4d86ae52a026fbef4ef800a05ecf2a4fe72457d759dd3615d0b`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Tue, 29 Aug 2023 17:09:18 GMT
RUN Install update 10.0.17763.4851
# Wed, 13 Sep 2023 01:39:13 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Sep 2023 08:33:49 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v3.0.0-beta3/traefik_v3.0.0-beta3_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Wed, 13 Sep 2023 08:33:50 GMT
EXPOSE 80
# Wed, 13 Sep 2023 08:33:50 GMT
ENTRYPOINT ["/traefik"]
# Wed, 13 Sep 2023 08:33:51 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta3 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:179757339e051b99f9a62375fed8f87ffcc4df0eeedb984d20b485bdd089ad08`  
		Last Modified: Tue, 12 Sep 2023 19:41:25 GMT  
		Size: 365.7 MB (365709508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdc14cbf6230cebb55cabf885ef8606e63f571dd05f37d899d95bca34972a44a`  
		Last Modified: Wed, 13 Sep 2023 02:16:50 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4761997e52cfb63512b90853905a746fd9fd54e41674e2d4bcbb1cb8201dd8e6`  
		Last Modified: Wed, 13 Sep 2023 08:35:53 GMT  
		Size: 38.9 MB (38911475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68336a56fcbfa87a1c489e6104360ab265abb53897306e3d4b09b6a7649bcc28`  
		Last Modified: Wed, 13 Sep 2023 08:35:44 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25e209029cdcd07d20e5a87b03da02a4e8a0c69006f4837fb0d0eb73571be80d`  
		Last Modified: Wed, 13 Sep 2023 08:35:44 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00a7cd492baf3537340fe6d001aa41f13f04e92943dc5fc877ffb6a51926b4db`  
		Last Modified: Wed, 13 Sep 2023 08:35:43 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:latest`

```console
$ docker pull traefik@sha256:50168bc91ccb8f44db127d6fbd45fba8e72dd704e1ac0c850406dd377a4ae140
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:latest` - linux; amd64

```console
$ docker pull traefik@sha256:57b2516b7549c4f59531bb09311a54a05af237670676529249c3c0b8e58ad0f3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.4 MB (42384635 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ae1addee1b2f3bd2ff67edf06e8cf028e1ca44f99a6fbf51dfb0b2eec546949`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:20 GMT
ADD file:32ff5e7a78b890996ee4681cc0a26185d3e9acdb4eb1e2aaccb2411f922fed6b in / 
# Mon, 07 Aug 2023 19:20:20 GMT
CMD ["/bin/sh"]
# Wed, 09 Aug 2023 04:06:24 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 09 Aug 2023 04:06:36 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.4/traefik_v2.10.4_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 09 Aug 2023 04:06:36 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 09 Aug 2023 04:06:36 GMT
EXPOSE 80
# Wed, 09 Aug 2023 04:06:36 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 09 Aug 2023 04:06:36 GMT
CMD ["traefik"]
# Wed, 09 Aug 2023 04:06:36 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.4 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:7264a8db6415046d36d16ba98b79778e18accee6ffa71850405994cffa9be7de`  
		Last Modified: Mon, 07 Aug 2023 19:20:54 GMT  
		Size: 3.4 MB (3401613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af32133391e63d8b260bd5a6dca0e380b088a7c2cfe9b6882dd7567b97bf5c84`  
		Last Modified: Wed, 09 Aug 2023 04:06:50 GMT  
		Size: 622.3 KB (622281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1022d3e6eb6de11e14cfcea2b297e20657615293e82e4c1a28cc6888c3727fc6`  
		Last Modified: Wed, 09 Aug 2023 04:07:16 GMT  
		Size: 38.4 MB (38360374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef9401db61432baa70472973f37408025b1240d1762e184bf6ab77f1ea68c85b`  
		Last Modified: Wed, 09 Aug 2023 04:07:10 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:latest` - linux; arm variant v6

```console
$ docker pull traefik@sha256:bcf37f90bb3c148ecc6c642f0a5ef7ecca69c107f5055a24e94de6b178038ee3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.9 MB (39897744 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b470a25273a17965c4195798705c8c434dec9e1dcb8bed0e25cd4afd15e5a1df`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 07 Aug 2023 19:49:14 GMT
ADD file:9882e99e5f94ab2db05c029648ac5be7cf0f063a8701394fcbb543a7ef5d4b90 in / 
# Mon, 07 Aug 2023 19:49:15 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 23:36:43 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 08 Aug 2023 23:36:56 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.4/traefik_v2.10.4_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Tue, 08 Aug 2023 23:36:56 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 08 Aug 2023 23:36:56 GMT
EXPOSE 80
# Tue, 08 Aug 2023 23:36:56 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 08 Aug 2023 23:36:56 GMT
CMD ["traefik"]
# Tue, 08 Aug 2023 23:36:56 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.4 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:af09961d4a43b504efc76e38b50918977c28be73eeb8b926247783a00e8b9f2f`  
		Last Modified: Mon, 07 Aug 2023 19:49:38 GMT  
		Size: 3.1 MB (3144809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f8cc6c7cf0fb882727ce9bdded1e9477cf9f51f27f262ddd2837ce010c75546`  
		Last Modified: Tue, 08 Aug 2023 23:37:08 GMT  
		Size: 622.7 KB (622688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53f350ea2c1577d6f498d27752f1efc8de8aea15ad9cc2c8ac411a406fc06474`  
		Last Modified: Tue, 08 Aug 2023 23:37:34 GMT  
		Size: 36.1 MB (36129878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbc4c23d6ff9206d00fa66fef11f0d9010dd364ced1cff33b54909008c2add1a`  
		Last Modified: Tue, 08 Aug 2023 23:37:28 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:latest` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:a56dcbeb82281b0ac99297d226195215f747242daa5a2213de02d8a09a6d9cfd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.1 MB (39136580 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0791754faa9d789eea8f305cf76a58f17b97c6b2fc5a2a32bfeb7bf3cf1ee8e2`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:19 GMT
ADD file:b2e7eaa7e41f08853dbe08d84439a7f9fd32fc58c3aa1e298f3f60343b2b683a in / 
# Mon, 07 Aug 2023 19:39:19 GMT
CMD ["/bin/sh"]
# Wed, 09 Aug 2023 04:26:52 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 09 Aug 2023 04:27:02 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.4/traefik_v2.10.4_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 09 Aug 2023 04:27:02 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 09 Aug 2023 04:27:02 GMT
EXPOSE 80
# Wed, 09 Aug 2023 04:27:02 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 09 Aug 2023 04:27:02 GMT
CMD ["traefik"]
# Wed, 09 Aug 2023 04:27:02 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.4 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:9fda8d8052c61740409c4bea888859c141fd8cc3f58ac61943144ff6d1681b2d`  
		Last Modified: Mon, 07 Aug 2023 19:39:45 GMT  
		Size: 3.3 MB (3330767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dffff58315ee746797a9f6d4ec2d858fca66532fa8ec5993ab228e70ec0dda7d`  
		Last Modified: Wed, 09 Aug 2023 04:27:14 GMT  
		Size: 624.5 KB (624509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3973374f4924c913ca3c30a39dd6be20f06314a673c7607d4d43b90643d7e21d`  
		Last Modified: Wed, 09 Aug 2023 04:27:39 GMT  
		Size: 35.2 MB (35180936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b4e902bb4f65830c8bcefc8a4ca424e5cce78a9f8843454b0194b9f7080c140`  
		Last Modified: Wed, 09 Aug 2023 04:27:34 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:latest` - linux; s390x

```console
$ docker pull traefik@sha256:755c4c3891db8f6b955c25fe3e19442bd0792ca28459f10fc3005e79776683e9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.0 MB (41034756 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:49fb49ad4398f43080e4b15ecb86663f7b9d33fd3394c2dbe5b85a61eea53998`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 28 Sep 2023 20:41:43 GMT
ADD file:fd3808a676fc56c1380e55b2ddbf4014d9371346cf789860b336bc9f00729ed0 in / 
# Thu, 28 Sep 2023 20:41:44 GMT
CMD ["/bin/sh"]
# Fri, 29 Sep 2023 00:15:10 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 29 Sep 2023 00:15:31 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.4/traefik_v2.10.4_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 29 Sep 2023 00:15:33 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 29 Sep 2023 00:15:33 GMT
EXPOSE 80
# Fri, 29 Sep 2023 00:15:34 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 29 Sep 2023 00:15:34 GMT
CMD ["traefik"]
# Fri, 29 Sep 2023 00:15:34 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.4 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:ddc123c7bae83a141fb0dc9f96de9910cfa54eb022ebb63bc8d191aec93dc97c`  
		Last Modified: Fri, 29 Sep 2023 00:16:13 GMT  
		Size: 37.2 MB (37196446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1ddc7c72004c2240bdeb82301ae59b70bacbd4aa31b3c18768ba03db4a96b8b`  
		Last Modified: Fri, 29 Sep 2023 00:16:07 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:saintmarcelin`

```console
$ docker pull traefik@sha256:50168bc91ccb8f44db127d6fbd45fba8e72dd704e1ac0c850406dd377a4ae140
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:saintmarcelin` - linux; amd64

```console
$ docker pull traefik@sha256:57b2516b7549c4f59531bb09311a54a05af237670676529249c3c0b8e58ad0f3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.4 MB (42384635 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ae1addee1b2f3bd2ff67edf06e8cf028e1ca44f99a6fbf51dfb0b2eec546949`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:20 GMT
ADD file:32ff5e7a78b890996ee4681cc0a26185d3e9acdb4eb1e2aaccb2411f922fed6b in / 
# Mon, 07 Aug 2023 19:20:20 GMT
CMD ["/bin/sh"]
# Wed, 09 Aug 2023 04:06:24 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 09 Aug 2023 04:06:36 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.4/traefik_v2.10.4_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 09 Aug 2023 04:06:36 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 09 Aug 2023 04:06:36 GMT
EXPOSE 80
# Wed, 09 Aug 2023 04:06:36 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 09 Aug 2023 04:06:36 GMT
CMD ["traefik"]
# Wed, 09 Aug 2023 04:06:36 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.4 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:7264a8db6415046d36d16ba98b79778e18accee6ffa71850405994cffa9be7de`  
		Last Modified: Mon, 07 Aug 2023 19:20:54 GMT  
		Size: 3.4 MB (3401613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af32133391e63d8b260bd5a6dca0e380b088a7c2cfe9b6882dd7567b97bf5c84`  
		Last Modified: Wed, 09 Aug 2023 04:06:50 GMT  
		Size: 622.3 KB (622281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1022d3e6eb6de11e14cfcea2b297e20657615293e82e4c1a28cc6888c3727fc6`  
		Last Modified: Wed, 09 Aug 2023 04:07:16 GMT  
		Size: 38.4 MB (38360374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef9401db61432baa70472973f37408025b1240d1762e184bf6ab77f1ea68c85b`  
		Last Modified: Wed, 09 Aug 2023 04:07:10 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:saintmarcelin` - linux; arm variant v6

```console
$ docker pull traefik@sha256:bcf37f90bb3c148ecc6c642f0a5ef7ecca69c107f5055a24e94de6b178038ee3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.9 MB (39897744 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b470a25273a17965c4195798705c8c434dec9e1dcb8bed0e25cd4afd15e5a1df`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 07 Aug 2023 19:49:14 GMT
ADD file:9882e99e5f94ab2db05c029648ac5be7cf0f063a8701394fcbb543a7ef5d4b90 in / 
# Mon, 07 Aug 2023 19:49:15 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 23:36:43 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 08 Aug 2023 23:36:56 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.4/traefik_v2.10.4_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Tue, 08 Aug 2023 23:36:56 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 08 Aug 2023 23:36:56 GMT
EXPOSE 80
# Tue, 08 Aug 2023 23:36:56 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 08 Aug 2023 23:36:56 GMT
CMD ["traefik"]
# Tue, 08 Aug 2023 23:36:56 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.4 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:af09961d4a43b504efc76e38b50918977c28be73eeb8b926247783a00e8b9f2f`  
		Last Modified: Mon, 07 Aug 2023 19:49:38 GMT  
		Size: 3.1 MB (3144809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f8cc6c7cf0fb882727ce9bdded1e9477cf9f51f27f262ddd2837ce010c75546`  
		Last Modified: Tue, 08 Aug 2023 23:37:08 GMT  
		Size: 622.7 KB (622688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53f350ea2c1577d6f498d27752f1efc8de8aea15ad9cc2c8ac411a406fc06474`  
		Last Modified: Tue, 08 Aug 2023 23:37:34 GMT  
		Size: 36.1 MB (36129878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbc4c23d6ff9206d00fa66fef11f0d9010dd364ced1cff33b54909008c2add1a`  
		Last Modified: Tue, 08 Aug 2023 23:37:28 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:saintmarcelin` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:a56dcbeb82281b0ac99297d226195215f747242daa5a2213de02d8a09a6d9cfd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.1 MB (39136580 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0791754faa9d789eea8f305cf76a58f17b97c6b2fc5a2a32bfeb7bf3cf1ee8e2`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:19 GMT
ADD file:b2e7eaa7e41f08853dbe08d84439a7f9fd32fc58c3aa1e298f3f60343b2b683a in / 
# Mon, 07 Aug 2023 19:39:19 GMT
CMD ["/bin/sh"]
# Wed, 09 Aug 2023 04:26:52 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 09 Aug 2023 04:27:02 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.4/traefik_v2.10.4_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 09 Aug 2023 04:27:02 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 09 Aug 2023 04:27:02 GMT
EXPOSE 80
# Wed, 09 Aug 2023 04:27:02 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 09 Aug 2023 04:27:02 GMT
CMD ["traefik"]
# Wed, 09 Aug 2023 04:27:02 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.4 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:9fda8d8052c61740409c4bea888859c141fd8cc3f58ac61943144ff6d1681b2d`  
		Last Modified: Mon, 07 Aug 2023 19:39:45 GMT  
		Size: 3.3 MB (3330767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dffff58315ee746797a9f6d4ec2d858fca66532fa8ec5993ab228e70ec0dda7d`  
		Last Modified: Wed, 09 Aug 2023 04:27:14 GMT  
		Size: 624.5 KB (624509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3973374f4924c913ca3c30a39dd6be20f06314a673c7607d4d43b90643d7e21d`  
		Last Modified: Wed, 09 Aug 2023 04:27:39 GMT  
		Size: 35.2 MB (35180936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b4e902bb4f65830c8bcefc8a4ca424e5cce78a9f8843454b0194b9f7080c140`  
		Last Modified: Wed, 09 Aug 2023 04:27:34 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:saintmarcelin` - linux; s390x

```console
$ docker pull traefik@sha256:755c4c3891db8f6b955c25fe3e19442bd0792ca28459f10fc3005e79776683e9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.0 MB (41034756 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:49fb49ad4398f43080e4b15ecb86663f7b9d33fd3394c2dbe5b85a61eea53998`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 28 Sep 2023 20:41:43 GMT
ADD file:fd3808a676fc56c1380e55b2ddbf4014d9371346cf789860b336bc9f00729ed0 in / 
# Thu, 28 Sep 2023 20:41:44 GMT
CMD ["/bin/sh"]
# Fri, 29 Sep 2023 00:15:10 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 29 Sep 2023 00:15:31 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.4/traefik_v2.10.4_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 29 Sep 2023 00:15:33 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 29 Sep 2023 00:15:33 GMT
EXPOSE 80
# Fri, 29 Sep 2023 00:15:34 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 29 Sep 2023 00:15:34 GMT
CMD ["traefik"]
# Fri, 29 Sep 2023 00:15:34 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.4 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:ddc123c7bae83a141fb0dc9f96de9910cfa54eb022ebb63bc8d191aec93dc97c`  
		Last Modified: Fri, 29 Sep 2023 00:16:13 GMT  
		Size: 37.2 MB (37196446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1ddc7c72004c2240bdeb82301ae59b70bacbd4aa31b3c18768ba03db4a96b8b`  
		Last Modified: Fri, 29 Sep 2023 00:16:07 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:saintmarcelin-windowsservercore-1809`

```console
$ docker pull traefik@sha256:8c809f2d7759cb331e6787e80637611f0df573ae584057252a404949d93176c6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4851; amd64

### `traefik:saintmarcelin-windowsservercore-1809` - windows version 10.0.17763.4851; amd64

```console
$ docker pull traefik@sha256:162622cb7682b3e6f3274106c7920c71adb69ea58ca89fa282e2ab7c33275f26
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2055286197 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:96ca8a25a6214a37c560d4a7e85db466ec7af762962f6ebe1350bb0e0ffeb03c`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Tue, 29 Aug 2023 17:09:18 GMT
RUN Install update 10.0.17763.4851
# Wed, 13 Sep 2023 01:39:13 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Sep 2023 08:35:18 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.10.4/traefik_v2.10.4_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Wed, 13 Sep 2023 08:35:19 GMT
EXPOSE 80
# Wed, 13 Sep 2023 08:35:20 GMT
ENTRYPOINT ["/traefik"]
# Wed, 13 Sep 2023 08:35:21 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.4 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:179757339e051b99f9a62375fed8f87ffcc4df0eeedb984d20b485bdd089ad08`  
		Last Modified: Tue, 12 Sep 2023 19:41:25 GMT  
		Size: 365.7 MB (365709508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdc14cbf6230cebb55cabf885ef8606e63f571dd05f37d899d95bca34972a44a`  
		Last Modified: Wed, 13 Sep 2023 02:16:50 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f02f28ba2ad38d851b3d6f506b4a28243717438129c2627a3492d29c08c6d5d`  
		Last Modified: Wed, 13 Sep 2023 08:36:16 GMT  
		Size: 39.0 MB (38950677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcf8cada8a7cfe4fa87db7be051abb4ec4a26637f91f6404bfce2664ea81dc64`  
		Last Modified: Wed, 13 Sep 2023 08:36:07 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2528ac6fcf0f3b42b632849e634ea6b05511b961bee203c0f893835f04664e6c`  
		Last Modified: Wed, 13 Sep 2023 08:36:08 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6487c7270b3462ca9295dd9a569d4ed3b821aa3f7be16a73d895e3483a3165f5`  
		Last Modified: Wed, 13 Sep 2023 08:36:07 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.10`

```console
$ docker pull traefik@sha256:50168bc91ccb8f44db127d6fbd45fba8e72dd704e1ac0c850406dd377a4ae140
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:v2.10` - linux; amd64

```console
$ docker pull traefik@sha256:57b2516b7549c4f59531bb09311a54a05af237670676529249c3c0b8e58ad0f3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.4 MB (42384635 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ae1addee1b2f3bd2ff67edf06e8cf028e1ca44f99a6fbf51dfb0b2eec546949`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:20 GMT
ADD file:32ff5e7a78b890996ee4681cc0a26185d3e9acdb4eb1e2aaccb2411f922fed6b in / 
# Mon, 07 Aug 2023 19:20:20 GMT
CMD ["/bin/sh"]
# Wed, 09 Aug 2023 04:06:24 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 09 Aug 2023 04:06:36 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.4/traefik_v2.10.4_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 09 Aug 2023 04:06:36 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 09 Aug 2023 04:06:36 GMT
EXPOSE 80
# Wed, 09 Aug 2023 04:06:36 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 09 Aug 2023 04:06:36 GMT
CMD ["traefik"]
# Wed, 09 Aug 2023 04:06:36 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.4 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:7264a8db6415046d36d16ba98b79778e18accee6ffa71850405994cffa9be7de`  
		Last Modified: Mon, 07 Aug 2023 19:20:54 GMT  
		Size: 3.4 MB (3401613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af32133391e63d8b260bd5a6dca0e380b088a7c2cfe9b6882dd7567b97bf5c84`  
		Last Modified: Wed, 09 Aug 2023 04:06:50 GMT  
		Size: 622.3 KB (622281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1022d3e6eb6de11e14cfcea2b297e20657615293e82e4c1a28cc6888c3727fc6`  
		Last Modified: Wed, 09 Aug 2023 04:07:16 GMT  
		Size: 38.4 MB (38360374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef9401db61432baa70472973f37408025b1240d1762e184bf6ab77f1ea68c85b`  
		Last Modified: Wed, 09 Aug 2023 04:07:10 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.10` - linux; arm variant v6

```console
$ docker pull traefik@sha256:bcf37f90bb3c148ecc6c642f0a5ef7ecca69c107f5055a24e94de6b178038ee3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.9 MB (39897744 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b470a25273a17965c4195798705c8c434dec9e1dcb8bed0e25cd4afd15e5a1df`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 07 Aug 2023 19:49:14 GMT
ADD file:9882e99e5f94ab2db05c029648ac5be7cf0f063a8701394fcbb543a7ef5d4b90 in / 
# Mon, 07 Aug 2023 19:49:15 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 23:36:43 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 08 Aug 2023 23:36:56 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.4/traefik_v2.10.4_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Tue, 08 Aug 2023 23:36:56 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 08 Aug 2023 23:36:56 GMT
EXPOSE 80
# Tue, 08 Aug 2023 23:36:56 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 08 Aug 2023 23:36:56 GMT
CMD ["traefik"]
# Tue, 08 Aug 2023 23:36:56 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.4 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:af09961d4a43b504efc76e38b50918977c28be73eeb8b926247783a00e8b9f2f`  
		Last Modified: Mon, 07 Aug 2023 19:49:38 GMT  
		Size: 3.1 MB (3144809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f8cc6c7cf0fb882727ce9bdded1e9477cf9f51f27f262ddd2837ce010c75546`  
		Last Modified: Tue, 08 Aug 2023 23:37:08 GMT  
		Size: 622.7 KB (622688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53f350ea2c1577d6f498d27752f1efc8de8aea15ad9cc2c8ac411a406fc06474`  
		Last Modified: Tue, 08 Aug 2023 23:37:34 GMT  
		Size: 36.1 MB (36129878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbc4c23d6ff9206d00fa66fef11f0d9010dd364ced1cff33b54909008c2add1a`  
		Last Modified: Tue, 08 Aug 2023 23:37:28 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.10` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:a56dcbeb82281b0ac99297d226195215f747242daa5a2213de02d8a09a6d9cfd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.1 MB (39136580 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0791754faa9d789eea8f305cf76a58f17b97c6b2fc5a2a32bfeb7bf3cf1ee8e2`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:19 GMT
ADD file:b2e7eaa7e41f08853dbe08d84439a7f9fd32fc58c3aa1e298f3f60343b2b683a in / 
# Mon, 07 Aug 2023 19:39:19 GMT
CMD ["/bin/sh"]
# Wed, 09 Aug 2023 04:26:52 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 09 Aug 2023 04:27:02 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.4/traefik_v2.10.4_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 09 Aug 2023 04:27:02 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 09 Aug 2023 04:27:02 GMT
EXPOSE 80
# Wed, 09 Aug 2023 04:27:02 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 09 Aug 2023 04:27:02 GMT
CMD ["traefik"]
# Wed, 09 Aug 2023 04:27:02 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.4 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:9fda8d8052c61740409c4bea888859c141fd8cc3f58ac61943144ff6d1681b2d`  
		Last Modified: Mon, 07 Aug 2023 19:39:45 GMT  
		Size: 3.3 MB (3330767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dffff58315ee746797a9f6d4ec2d858fca66532fa8ec5993ab228e70ec0dda7d`  
		Last Modified: Wed, 09 Aug 2023 04:27:14 GMT  
		Size: 624.5 KB (624509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3973374f4924c913ca3c30a39dd6be20f06314a673c7607d4d43b90643d7e21d`  
		Last Modified: Wed, 09 Aug 2023 04:27:39 GMT  
		Size: 35.2 MB (35180936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b4e902bb4f65830c8bcefc8a4ca424e5cce78a9f8843454b0194b9f7080c140`  
		Last Modified: Wed, 09 Aug 2023 04:27:34 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.10` - linux; s390x

```console
$ docker pull traefik@sha256:755c4c3891db8f6b955c25fe3e19442bd0792ca28459f10fc3005e79776683e9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.0 MB (41034756 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:49fb49ad4398f43080e4b15ecb86663f7b9d33fd3394c2dbe5b85a61eea53998`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 28 Sep 2023 20:41:43 GMT
ADD file:fd3808a676fc56c1380e55b2ddbf4014d9371346cf789860b336bc9f00729ed0 in / 
# Thu, 28 Sep 2023 20:41:44 GMT
CMD ["/bin/sh"]
# Fri, 29 Sep 2023 00:15:10 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 29 Sep 2023 00:15:31 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.4/traefik_v2.10.4_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 29 Sep 2023 00:15:33 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 29 Sep 2023 00:15:33 GMT
EXPOSE 80
# Fri, 29 Sep 2023 00:15:34 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 29 Sep 2023 00:15:34 GMT
CMD ["traefik"]
# Fri, 29 Sep 2023 00:15:34 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.4 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:ddc123c7bae83a141fb0dc9f96de9910cfa54eb022ebb63bc8d191aec93dc97c`  
		Last Modified: Fri, 29 Sep 2023 00:16:13 GMT  
		Size: 37.2 MB (37196446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1ddc7c72004c2240bdeb82301ae59b70bacbd4aa31b3c18768ba03db4a96b8b`  
		Last Modified: Fri, 29 Sep 2023 00:16:07 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.10-windowsservercore-1809`

```console
$ docker pull traefik@sha256:8c809f2d7759cb331e6787e80637611f0df573ae584057252a404949d93176c6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4851; amd64

### `traefik:v2.10-windowsservercore-1809` - windows version 10.0.17763.4851; amd64

```console
$ docker pull traefik@sha256:162622cb7682b3e6f3274106c7920c71adb69ea58ca89fa282e2ab7c33275f26
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2055286197 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:96ca8a25a6214a37c560d4a7e85db466ec7af762962f6ebe1350bb0e0ffeb03c`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Tue, 29 Aug 2023 17:09:18 GMT
RUN Install update 10.0.17763.4851
# Wed, 13 Sep 2023 01:39:13 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Sep 2023 08:35:18 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.10.4/traefik_v2.10.4_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Wed, 13 Sep 2023 08:35:19 GMT
EXPOSE 80
# Wed, 13 Sep 2023 08:35:20 GMT
ENTRYPOINT ["/traefik"]
# Wed, 13 Sep 2023 08:35:21 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.4 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:179757339e051b99f9a62375fed8f87ffcc4df0eeedb984d20b485bdd089ad08`  
		Last Modified: Tue, 12 Sep 2023 19:41:25 GMT  
		Size: 365.7 MB (365709508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdc14cbf6230cebb55cabf885ef8606e63f571dd05f37d899d95bca34972a44a`  
		Last Modified: Wed, 13 Sep 2023 02:16:50 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f02f28ba2ad38d851b3d6f506b4a28243717438129c2627a3492d29c08c6d5d`  
		Last Modified: Wed, 13 Sep 2023 08:36:16 GMT  
		Size: 39.0 MB (38950677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcf8cada8a7cfe4fa87db7be051abb4ec4a26637f91f6404bfce2664ea81dc64`  
		Last Modified: Wed, 13 Sep 2023 08:36:07 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2528ac6fcf0f3b42b632849e634ea6b05511b961bee203c0f893835f04664e6c`  
		Last Modified: Wed, 13 Sep 2023 08:36:08 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6487c7270b3462ca9295dd9a569d4ed3b821aa3f7be16a73d895e3483a3165f5`  
		Last Modified: Wed, 13 Sep 2023 08:36:07 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.10.4`

```console
$ docker pull traefik@sha256:50168bc91ccb8f44db127d6fbd45fba8e72dd704e1ac0c850406dd377a4ae140
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:v2.10.4` - linux; amd64

```console
$ docker pull traefik@sha256:57b2516b7549c4f59531bb09311a54a05af237670676529249c3c0b8e58ad0f3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.4 MB (42384635 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ae1addee1b2f3bd2ff67edf06e8cf028e1ca44f99a6fbf51dfb0b2eec546949`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:20 GMT
ADD file:32ff5e7a78b890996ee4681cc0a26185d3e9acdb4eb1e2aaccb2411f922fed6b in / 
# Mon, 07 Aug 2023 19:20:20 GMT
CMD ["/bin/sh"]
# Wed, 09 Aug 2023 04:06:24 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 09 Aug 2023 04:06:36 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.4/traefik_v2.10.4_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 09 Aug 2023 04:06:36 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 09 Aug 2023 04:06:36 GMT
EXPOSE 80
# Wed, 09 Aug 2023 04:06:36 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 09 Aug 2023 04:06:36 GMT
CMD ["traefik"]
# Wed, 09 Aug 2023 04:06:36 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.4 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:7264a8db6415046d36d16ba98b79778e18accee6ffa71850405994cffa9be7de`  
		Last Modified: Mon, 07 Aug 2023 19:20:54 GMT  
		Size: 3.4 MB (3401613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af32133391e63d8b260bd5a6dca0e380b088a7c2cfe9b6882dd7567b97bf5c84`  
		Last Modified: Wed, 09 Aug 2023 04:06:50 GMT  
		Size: 622.3 KB (622281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1022d3e6eb6de11e14cfcea2b297e20657615293e82e4c1a28cc6888c3727fc6`  
		Last Modified: Wed, 09 Aug 2023 04:07:16 GMT  
		Size: 38.4 MB (38360374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef9401db61432baa70472973f37408025b1240d1762e184bf6ab77f1ea68c85b`  
		Last Modified: Wed, 09 Aug 2023 04:07:10 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.10.4` - linux; arm variant v6

```console
$ docker pull traefik@sha256:bcf37f90bb3c148ecc6c642f0a5ef7ecca69c107f5055a24e94de6b178038ee3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.9 MB (39897744 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b470a25273a17965c4195798705c8c434dec9e1dcb8bed0e25cd4afd15e5a1df`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 07 Aug 2023 19:49:14 GMT
ADD file:9882e99e5f94ab2db05c029648ac5be7cf0f063a8701394fcbb543a7ef5d4b90 in / 
# Mon, 07 Aug 2023 19:49:15 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 23:36:43 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 08 Aug 2023 23:36:56 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.4/traefik_v2.10.4_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Tue, 08 Aug 2023 23:36:56 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 08 Aug 2023 23:36:56 GMT
EXPOSE 80
# Tue, 08 Aug 2023 23:36:56 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 08 Aug 2023 23:36:56 GMT
CMD ["traefik"]
# Tue, 08 Aug 2023 23:36:56 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.4 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:af09961d4a43b504efc76e38b50918977c28be73eeb8b926247783a00e8b9f2f`  
		Last Modified: Mon, 07 Aug 2023 19:49:38 GMT  
		Size: 3.1 MB (3144809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f8cc6c7cf0fb882727ce9bdded1e9477cf9f51f27f262ddd2837ce010c75546`  
		Last Modified: Tue, 08 Aug 2023 23:37:08 GMT  
		Size: 622.7 KB (622688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53f350ea2c1577d6f498d27752f1efc8de8aea15ad9cc2c8ac411a406fc06474`  
		Last Modified: Tue, 08 Aug 2023 23:37:34 GMT  
		Size: 36.1 MB (36129878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbc4c23d6ff9206d00fa66fef11f0d9010dd364ced1cff33b54909008c2add1a`  
		Last Modified: Tue, 08 Aug 2023 23:37:28 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.10.4` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:a56dcbeb82281b0ac99297d226195215f747242daa5a2213de02d8a09a6d9cfd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.1 MB (39136580 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0791754faa9d789eea8f305cf76a58f17b97c6b2fc5a2a32bfeb7bf3cf1ee8e2`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:19 GMT
ADD file:b2e7eaa7e41f08853dbe08d84439a7f9fd32fc58c3aa1e298f3f60343b2b683a in / 
# Mon, 07 Aug 2023 19:39:19 GMT
CMD ["/bin/sh"]
# Wed, 09 Aug 2023 04:26:52 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 09 Aug 2023 04:27:02 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.4/traefik_v2.10.4_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 09 Aug 2023 04:27:02 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 09 Aug 2023 04:27:02 GMT
EXPOSE 80
# Wed, 09 Aug 2023 04:27:02 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 09 Aug 2023 04:27:02 GMT
CMD ["traefik"]
# Wed, 09 Aug 2023 04:27:02 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.4 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:9fda8d8052c61740409c4bea888859c141fd8cc3f58ac61943144ff6d1681b2d`  
		Last Modified: Mon, 07 Aug 2023 19:39:45 GMT  
		Size: 3.3 MB (3330767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dffff58315ee746797a9f6d4ec2d858fca66532fa8ec5993ab228e70ec0dda7d`  
		Last Modified: Wed, 09 Aug 2023 04:27:14 GMT  
		Size: 624.5 KB (624509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3973374f4924c913ca3c30a39dd6be20f06314a673c7607d4d43b90643d7e21d`  
		Last Modified: Wed, 09 Aug 2023 04:27:39 GMT  
		Size: 35.2 MB (35180936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b4e902bb4f65830c8bcefc8a4ca424e5cce78a9f8843454b0194b9f7080c140`  
		Last Modified: Wed, 09 Aug 2023 04:27:34 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.10.4` - linux; s390x

```console
$ docker pull traefik@sha256:755c4c3891db8f6b955c25fe3e19442bd0792ca28459f10fc3005e79776683e9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.0 MB (41034756 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:49fb49ad4398f43080e4b15ecb86663f7b9d33fd3394c2dbe5b85a61eea53998`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Thu, 28 Sep 2023 20:41:43 GMT
ADD file:fd3808a676fc56c1380e55b2ddbf4014d9371346cf789860b336bc9f00729ed0 in / 
# Thu, 28 Sep 2023 20:41:44 GMT
CMD ["/bin/sh"]
# Fri, 29 Sep 2023 00:15:10 GMT
RUN apk --no-cache add ca-certificates tzdata
# Fri, 29 Sep 2023 00:15:31 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.4/traefik_v2.10.4_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Fri, 29 Sep 2023 00:15:33 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Fri, 29 Sep 2023 00:15:33 GMT
EXPOSE 80
# Fri, 29 Sep 2023 00:15:34 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 29 Sep 2023 00:15:34 GMT
CMD ["traefik"]
# Fri, 29 Sep 2023 00:15:34 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.4 org.opencontainers.image.documentation=https://docs.traefik.io
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
	-	`sha256:ddc123c7bae83a141fb0dc9f96de9910cfa54eb022ebb63bc8d191aec93dc97c`  
		Last Modified: Fri, 29 Sep 2023 00:16:13 GMT  
		Size: 37.2 MB (37196446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1ddc7c72004c2240bdeb82301ae59b70bacbd4aa31b3c18768ba03db4a96b8b`  
		Last Modified: Fri, 29 Sep 2023 00:16:07 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.10.4-windowsservercore-1809`

```console
$ docker pull traefik@sha256:8c809f2d7759cb331e6787e80637611f0df573ae584057252a404949d93176c6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4851; amd64

### `traefik:v2.10.4-windowsservercore-1809` - windows version 10.0.17763.4851; amd64

```console
$ docker pull traefik@sha256:162622cb7682b3e6f3274106c7920c71adb69ea58ca89fa282e2ab7c33275f26
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2055286197 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:96ca8a25a6214a37c560d4a7e85db466ec7af762962f6ebe1350bb0e0ffeb03c`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Tue, 29 Aug 2023 17:09:18 GMT
RUN Install update 10.0.17763.4851
# Wed, 13 Sep 2023 01:39:13 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Sep 2023 08:35:18 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.10.4/traefik_v2.10.4_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Wed, 13 Sep 2023 08:35:19 GMT
EXPOSE 80
# Wed, 13 Sep 2023 08:35:20 GMT
ENTRYPOINT ["/traefik"]
# Wed, 13 Sep 2023 08:35:21 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.4 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:179757339e051b99f9a62375fed8f87ffcc4df0eeedb984d20b485bdd089ad08`  
		Last Modified: Tue, 12 Sep 2023 19:41:25 GMT  
		Size: 365.7 MB (365709508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdc14cbf6230cebb55cabf885ef8606e63f571dd05f37d899d95bca34972a44a`  
		Last Modified: Wed, 13 Sep 2023 02:16:50 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f02f28ba2ad38d851b3d6f506b4a28243717438129c2627a3492d29c08c6d5d`  
		Last Modified: Wed, 13 Sep 2023 08:36:16 GMT  
		Size: 39.0 MB (38950677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcf8cada8a7cfe4fa87db7be051abb4ec4a26637f91f6404bfce2664ea81dc64`  
		Last Modified: Wed, 13 Sep 2023 08:36:07 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2528ac6fcf0f3b42b632849e634ea6b05511b961bee203c0f893835f04664e6c`  
		Last Modified: Wed, 13 Sep 2023 08:36:08 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6487c7270b3462ca9295dd9a569d4ed3b821aa3f7be16a73d895e3483a3165f5`  
		Last Modified: Wed, 13 Sep 2023 08:36:07 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v3.0`

```console
$ docker pull traefik@sha256:5c18ddd7402cf0a0dfffd4e8b451e5b09018116ee06010d0e9a243e6c3e80cea
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:v3.0` - linux; amd64

```console
$ docker pull traefik@sha256:db21af65fb9edaa04542efe69bb6ba74afa04231874b0240fcccb059547fbf24
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.3 MB (42339283 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99d2af65616272cb94e6157ff2c162b2949d831dfe72e5de461e32db2f458951`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:20 GMT
ADD file:32ff5e7a78b890996ee4681cc0a26185d3e9acdb4eb1e2aaccb2411f922fed6b in / 
# Mon, 07 Aug 2023 19:20:20 GMT
CMD ["/bin/sh"]
# Wed, 09 Aug 2023 04:06:24 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 09 Aug 2023 04:06:28 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta3/traefik_v3.0.0-beta3_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 09 Aug 2023 04:06:28 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 09 Aug 2023 04:06:28 GMT
EXPOSE 80
# Wed, 09 Aug 2023 04:06:28 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 09 Aug 2023 04:06:28 GMT
CMD ["traefik"]
# Wed, 09 Aug 2023 04:06:28 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta3 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:7264a8db6415046d36d16ba98b79778e18accee6ffa71850405994cffa9be7de`  
		Last Modified: Mon, 07 Aug 2023 19:20:54 GMT  
		Size: 3.4 MB (3401613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af32133391e63d8b260bd5a6dca0e380b088a7c2cfe9b6882dd7567b97bf5c84`  
		Last Modified: Wed, 09 Aug 2023 04:06:50 GMT  
		Size: 622.3 KB (622281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a3fb410d5ad92d4b790c3aeff36ea3d4e6d1768c3d58cd9fadb8f574f8eb24a`  
		Last Modified: Wed, 09 Aug 2023 04:06:55 GMT  
		Size: 38.3 MB (38315021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25020b7f93004e310f3a03e903db4f1ba8ae45d9a5b5b3a594da55f18b0bc663`  
		Last Modified: Wed, 09 Aug 2023 04:06:50 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v3.0` - linux; arm variant v6

```console
$ docker pull traefik@sha256:4610ad0a08abfd441d5efea592fc370ab772915d5d62a4fe1b6ad57f5b1f7a17
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.8 MB (39834746 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14c7857053ace4e793ccb85ef5e4f7039d5b2d69ef3bba2091533f1eac50eb57`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 07 Aug 2023 19:49:14 GMT
ADD file:9882e99e5f94ab2db05c029648ac5be7cf0f063a8701394fcbb543a7ef5d4b90 in / 
# Mon, 07 Aug 2023 19:49:15 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 23:36:43 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 08 Aug 2023 23:36:47 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta3/traefik_v3.0.0-beta3_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Tue, 08 Aug 2023 23:36:48 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 08 Aug 2023 23:36:48 GMT
EXPOSE 80
# Tue, 08 Aug 2023 23:36:48 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 08 Aug 2023 23:36:48 GMT
CMD ["traefik"]
# Tue, 08 Aug 2023 23:36:48 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta3 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:af09961d4a43b504efc76e38b50918977c28be73eeb8b926247783a00e8b9f2f`  
		Last Modified: Mon, 07 Aug 2023 19:49:38 GMT  
		Size: 3.1 MB (3144809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f8cc6c7cf0fb882727ce9bdded1e9477cf9f51f27f262ddd2837ce010c75546`  
		Last Modified: Tue, 08 Aug 2023 23:37:08 GMT  
		Size: 622.7 KB (622688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13a56f8f3e28824e8aeed3179006a8bacb5ea8697429ecdcf4b3313a11531872`  
		Last Modified: Tue, 08 Aug 2023 23:37:14 GMT  
		Size: 36.1 MB (36066881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b4c24374a077bea1e909f5b61e43515993be1be29aacd3aef10a445d1447b70`  
		Last Modified: Tue, 08 Aug 2023 23:37:08 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v3.0` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:a4ccc52aa5d73f85d580e98cccd048575c4dd1cb3f4903a81e5f370edeb13845
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.1 MB (39098171 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8be29ac05708d11224070a2badc6d648a7b7494276deafffa559dece31419b37`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:19 GMT
ADD file:b2e7eaa7e41f08853dbe08d84439a7f9fd32fc58c3aa1e298f3f60343b2b683a in / 
# Mon, 07 Aug 2023 19:39:19 GMT
CMD ["/bin/sh"]
# Wed, 09 Aug 2023 04:26:52 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 09 Aug 2023 04:26:55 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta3/traefik_v3.0.0-beta3_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 09 Aug 2023 04:26:56 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 09 Aug 2023 04:26:56 GMT
EXPOSE 80
# Wed, 09 Aug 2023 04:26:56 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 09 Aug 2023 04:26:56 GMT
CMD ["traefik"]
# Wed, 09 Aug 2023 04:26:56 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta3 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:9fda8d8052c61740409c4bea888859c141fd8cc3f58ac61943144ff6d1681b2d`  
		Last Modified: Mon, 07 Aug 2023 19:39:45 GMT  
		Size: 3.3 MB (3330767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dffff58315ee746797a9f6d4ec2d858fca66532fa8ec5993ab228e70ec0dda7d`  
		Last Modified: Wed, 09 Aug 2023 04:27:14 GMT  
		Size: 624.5 KB (624509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdeef0a315984700bca8a1be11d88d1531de6244904ee7fd95bf207f107a61a7`  
		Last Modified: Wed, 09 Aug 2023 04:27:18 GMT  
		Size: 35.1 MB (35142527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f464f3b71f2555dfe7d1254a4847862866df2628d5e79e21597c596903c530ec`  
		Last Modified: Wed, 09 Aug 2023 04:27:13 GMT  
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
$ docker pull traefik@sha256:dab2b4b52465d429b1bf5b84ffa38c085ea1c00af3121846acd69ab445b4083e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4851; amd64

### `traefik:v3.0-windowsservercore-1809` - windows version 10.0.17763.4851; amd64

```console
$ docker pull traefik@sha256:dee2708e034f9398d1df57ca83b286b95a461705193b858a5b845bb5eec8a7b4
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2055247019 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a29344f9d48c4d86ae52a026fbef4ef800a05ecf2a4fe72457d759dd3615d0b`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Tue, 29 Aug 2023 17:09:18 GMT
RUN Install update 10.0.17763.4851
# Wed, 13 Sep 2023 01:39:13 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Sep 2023 08:33:49 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v3.0.0-beta3/traefik_v3.0.0-beta3_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Wed, 13 Sep 2023 08:33:50 GMT
EXPOSE 80
# Wed, 13 Sep 2023 08:33:50 GMT
ENTRYPOINT ["/traefik"]
# Wed, 13 Sep 2023 08:33:51 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta3 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:179757339e051b99f9a62375fed8f87ffcc4df0eeedb984d20b485bdd089ad08`  
		Last Modified: Tue, 12 Sep 2023 19:41:25 GMT  
		Size: 365.7 MB (365709508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdc14cbf6230cebb55cabf885ef8606e63f571dd05f37d899d95bca34972a44a`  
		Last Modified: Wed, 13 Sep 2023 02:16:50 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4761997e52cfb63512b90853905a746fd9fd54e41674e2d4bcbb1cb8201dd8e6`  
		Last Modified: Wed, 13 Sep 2023 08:35:53 GMT  
		Size: 38.9 MB (38911475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68336a56fcbfa87a1c489e6104360ab265abb53897306e3d4b09b6a7649bcc28`  
		Last Modified: Wed, 13 Sep 2023 08:35:44 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25e209029cdcd07d20e5a87b03da02a4e8a0c69006f4837fb0d0eb73571be80d`  
		Last Modified: Wed, 13 Sep 2023 08:35:44 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00a7cd492baf3537340fe6d001aa41f13f04e92943dc5fc877ffb6a51926b4db`  
		Last Modified: Wed, 13 Sep 2023 08:35:43 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v3.0.0-beta3`

```console
$ docker pull traefik@sha256:5c18ddd7402cf0a0dfffd4e8b451e5b09018116ee06010d0e9a243e6c3e80cea
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:v3.0.0-beta3` - linux; amd64

```console
$ docker pull traefik@sha256:db21af65fb9edaa04542efe69bb6ba74afa04231874b0240fcccb059547fbf24
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.3 MB (42339283 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99d2af65616272cb94e6157ff2c162b2949d831dfe72e5de461e32db2f458951`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:20 GMT
ADD file:32ff5e7a78b890996ee4681cc0a26185d3e9acdb4eb1e2aaccb2411f922fed6b in / 
# Mon, 07 Aug 2023 19:20:20 GMT
CMD ["/bin/sh"]
# Wed, 09 Aug 2023 04:06:24 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 09 Aug 2023 04:06:28 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta3/traefik_v3.0.0-beta3_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 09 Aug 2023 04:06:28 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 09 Aug 2023 04:06:28 GMT
EXPOSE 80
# Wed, 09 Aug 2023 04:06:28 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 09 Aug 2023 04:06:28 GMT
CMD ["traefik"]
# Wed, 09 Aug 2023 04:06:28 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta3 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:7264a8db6415046d36d16ba98b79778e18accee6ffa71850405994cffa9be7de`  
		Last Modified: Mon, 07 Aug 2023 19:20:54 GMT  
		Size: 3.4 MB (3401613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af32133391e63d8b260bd5a6dca0e380b088a7c2cfe9b6882dd7567b97bf5c84`  
		Last Modified: Wed, 09 Aug 2023 04:06:50 GMT  
		Size: 622.3 KB (622281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a3fb410d5ad92d4b790c3aeff36ea3d4e6d1768c3d58cd9fadb8f574f8eb24a`  
		Last Modified: Wed, 09 Aug 2023 04:06:55 GMT  
		Size: 38.3 MB (38315021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25020b7f93004e310f3a03e903db4f1ba8ae45d9a5b5b3a594da55f18b0bc663`  
		Last Modified: Wed, 09 Aug 2023 04:06:50 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v3.0.0-beta3` - linux; arm variant v6

```console
$ docker pull traefik@sha256:4610ad0a08abfd441d5efea592fc370ab772915d5d62a4fe1b6ad57f5b1f7a17
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.8 MB (39834746 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14c7857053ace4e793ccb85ef5e4f7039d5b2d69ef3bba2091533f1eac50eb57`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 07 Aug 2023 19:49:14 GMT
ADD file:9882e99e5f94ab2db05c029648ac5be7cf0f063a8701394fcbb543a7ef5d4b90 in / 
# Mon, 07 Aug 2023 19:49:15 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 23:36:43 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 08 Aug 2023 23:36:47 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta3/traefik_v3.0.0-beta3_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Tue, 08 Aug 2023 23:36:48 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 08 Aug 2023 23:36:48 GMT
EXPOSE 80
# Tue, 08 Aug 2023 23:36:48 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 08 Aug 2023 23:36:48 GMT
CMD ["traefik"]
# Tue, 08 Aug 2023 23:36:48 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta3 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:af09961d4a43b504efc76e38b50918977c28be73eeb8b926247783a00e8b9f2f`  
		Last Modified: Mon, 07 Aug 2023 19:49:38 GMT  
		Size: 3.1 MB (3144809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f8cc6c7cf0fb882727ce9bdded1e9477cf9f51f27f262ddd2837ce010c75546`  
		Last Modified: Tue, 08 Aug 2023 23:37:08 GMT  
		Size: 622.7 KB (622688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13a56f8f3e28824e8aeed3179006a8bacb5ea8697429ecdcf4b3313a11531872`  
		Last Modified: Tue, 08 Aug 2023 23:37:14 GMT  
		Size: 36.1 MB (36066881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b4c24374a077bea1e909f5b61e43515993be1be29aacd3aef10a445d1447b70`  
		Last Modified: Tue, 08 Aug 2023 23:37:08 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v3.0.0-beta3` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:a4ccc52aa5d73f85d580e98cccd048575c4dd1cb3f4903a81e5f370edeb13845
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.1 MB (39098171 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8be29ac05708d11224070a2badc6d648a7b7494276deafffa559dece31419b37`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:19 GMT
ADD file:b2e7eaa7e41f08853dbe08d84439a7f9fd32fc58c3aa1e298f3f60343b2b683a in / 
# Mon, 07 Aug 2023 19:39:19 GMT
CMD ["/bin/sh"]
# Wed, 09 Aug 2023 04:26:52 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 09 Aug 2023 04:26:55 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta3/traefik_v3.0.0-beta3_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 09 Aug 2023 04:26:56 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 09 Aug 2023 04:26:56 GMT
EXPOSE 80
# Wed, 09 Aug 2023 04:26:56 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 09 Aug 2023 04:26:56 GMT
CMD ["traefik"]
# Wed, 09 Aug 2023 04:26:56 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta3 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:9fda8d8052c61740409c4bea888859c141fd8cc3f58ac61943144ff6d1681b2d`  
		Last Modified: Mon, 07 Aug 2023 19:39:45 GMT  
		Size: 3.3 MB (3330767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dffff58315ee746797a9f6d4ec2d858fca66532fa8ec5993ab228e70ec0dda7d`  
		Last Modified: Wed, 09 Aug 2023 04:27:14 GMT  
		Size: 624.5 KB (624509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdeef0a315984700bca8a1be11d88d1531de6244904ee7fd95bf207f107a61a7`  
		Last Modified: Wed, 09 Aug 2023 04:27:18 GMT  
		Size: 35.1 MB (35142527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f464f3b71f2555dfe7d1254a4847862866df2628d5e79e21597c596903c530ec`  
		Last Modified: Wed, 09 Aug 2023 04:27:13 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v3.0.0-beta3` - linux; s390x

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

## `traefik:v3.0.0-beta3-windowsservercore-1809`

```console
$ docker pull traefik@sha256:dab2b4b52465d429b1bf5b84ffa38c085ea1c00af3121846acd69ab445b4083e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4851; amd64

### `traefik:v3.0.0-beta3-windowsservercore-1809` - windows version 10.0.17763.4851; amd64

```console
$ docker pull traefik@sha256:dee2708e034f9398d1df57ca83b286b95a461705193b858a5b845bb5eec8a7b4
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2055247019 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a29344f9d48c4d86ae52a026fbef4ef800a05ecf2a4fe72457d759dd3615d0b`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Tue, 29 Aug 2023 17:09:18 GMT
RUN Install update 10.0.17763.4851
# Wed, 13 Sep 2023 01:39:13 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Sep 2023 08:33:49 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v3.0.0-beta3/traefik_v3.0.0-beta3_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Wed, 13 Sep 2023 08:33:50 GMT
EXPOSE 80
# Wed, 13 Sep 2023 08:33:50 GMT
ENTRYPOINT ["/traefik"]
# Wed, 13 Sep 2023 08:33:51 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta3 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:179757339e051b99f9a62375fed8f87ffcc4df0eeedb984d20b485bdd089ad08`  
		Last Modified: Tue, 12 Sep 2023 19:41:25 GMT  
		Size: 365.7 MB (365709508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdc14cbf6230cebb55cabf885ef8606e63f571dd05f37d899d95bca34972a44a`  
		Last Modified: Wed, 13 Sep 2023 02:16:50 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4761997e52cfb63512b90853905a746fd9fd54e41674e2d4bcbb1cb8201dd8e6`  
		Last Modified: Wed, 13 Sep 2023 08:35:53 GMT  
		Size: 38.9 MB (38911475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68336a56fcbfa87a1c489e6104360ab265abb53897306e3d4b09b6a7649bcc28`  
		Last Modified: Wed, 13 Sep 2023 08:35:44 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25e209029cdcd07d20e5a87b03da02a4e8a0c69006f4837fb0d0eb73571be80d`  
		Last Modified: Wed, 13 Sep 2023 08:35:44 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00a7cd492baf3537340fe6d001aa41f13f04e92943dc5fc877ffb6a51926b4db`  
		Last Modified: Wed, 13 Sep 2023 08:35:43 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:windowsservercore-1809`

```console
$ docker pull traefik@sha256:8c809f2d7759cb331e6787e80637611f0df573ae584057252a404949d93176c6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4851; amd64

### `traefik:windowsservercore-1809` - windows version 10.0.17763.4851; amd64

```console
$ docker pull traefik@sha256:162622cb7682b3e6f3274106c7920c71adb69ea58ca89fa282e2ab7c33275f26
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2055286197 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:96ca8a25a6214a37c560d4a7e85db466ec7af762962f6ebe1350bb0e0ffeb03c`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Tue, 29 Aug 2023 17:09:18 GMT
RUN Install update 10.0.17763.4851
# Wed, 13 Sep 2023 01:39:13 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Sep 2023 08:35:18 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.10.4/traefik_v2.10.4_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Wed, 13 Sep 2023 08:35:19 GMT
EXPOSE 80
# Wed, 13 Sep 2023 08:35:20 GMT
ENTRYPOINT ["/traefik"]
# Wed, 13 Sep 2023 08:35:21 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.4 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:179757339e051b99f9a62375fed8f87ffcc4df0eeedb984d20b485bdd089ad08`  
		Last Modified: Tue, 12 Sep 2023 19:41:25 GMT  
		Size: 365.7 MB (365709508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdc14cbf6230cebb55cabf885ef8606e63f571dd05f37d899d95bca34972a44a`  
		Last Modified: Wed, 13 Sep 2023 02:16:50 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f02f28ba2ad38d851b3d6f506b4a28243717438129c2627a3492d29c08c6d5d`  
		Last Modified: Wed, 13 Sep 2023 08:36:16 GMT  
		Size: 39.0 MB (38950677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcf8cada8a7cfe4fa87db7be051abb4ec4a26637f91f6404bfce2664ea81dc64`  
		Last Modified: Wed, 13 Sep 2023 08:36:07 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2528ac6fcf0f3b42b632849e634ea6b05511b961bee203c0f893835f04664e6c`  
		Last Modified: Wed, 13 Sep 2023 08:36:08 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6487c7270b3462ca9295dd9a569d4ed3b821aa3f7be16a73d895e3483a3165f5`  
		Last Modified: Wed, 13 Sep 2023 08:36:07 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
