<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `traefik`

-	[`traefik:2.10`](#traefik210)
-	[`traefik:2.10-windowsservercore-1809`](#traefik210-windowsservercore-1809)
-	[`traefik:2.10.1`](#traefik2101)
-	[`traefik:2.10.1-windowsservercore-1809`](#traefik2101-windowsservercore-1809)
-	[`traefik:3.0`](#traefik30)
-	[`traefik:3.0-windowsservercore-1809`](#traefik30-windowsservercore-1809)
-	[`traefik:3.0.0-beta2`](#traefik300-beta2)
-	[`traefik:3.0.0-beta2-windowsservercore-1809`](#traefik300-beta2-windowsservercore-1809)
-	[`traefik:beaufort`](#traefikbeaufort)
-	[`traefik:beaufort-windowsservercore-1809`](#traefikbeaufort-windowsservercore-1809)
-	[`traefik:latest`](#traefiklatest)
-	[`traefik:saintmarcelin`](#traefiksaintmarcelin)
-	[`traefik:saintmarcelin-windowsservercore-1809`](#traefiksaintmarcelin-windowsservercore-1809)
-	[`traefik:v2.10`](#traefikv210)
-	[`traefik:v2.10-windowsservercore-1809`](#traefikv210-windowsservercore-1809)
-	[`traefik:v2.10.1`](#traefikv2101)
-	[`traefik:v2.10.1-windowsservercore-1809`](#traefikv2101-windowsservercore-1809)
-	[`traefik:v3.0`](#traefikv30)
-	[`traefik:v3.0-windowsservercore-1809`](#traefikv30-windowsservercore-1809)
-	[`traefik:v3.0.0-beta2`](#traefikv300-beta2)
-	[`traefik:v3.0.0-beta2-windowsservercore-1809`](#traefikv300-beta2-windowsservercore-1809)
-	[`traefik:windowsservercore-1809`](#traefikwindowsservercore-1809)

## `traefik:2.10`

```console
$ docker pull traefik@sha256:aae49c77988f065f91948477368475be36d74f46e7eb7b25ab1a8444266d2b0e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:2.10` - linux; amd64

```console
$ docker pull traefik@sha256:e01d05a30cfed0f79a9ecfb4942662c654ff2d8a39a80f030d4d58d9eb9ec0d1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.0 MB (40990396 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:63d7224eb30e1c2f2976e0043c6cb6f4f7f9bebb820253dc65998bbd747fcc85`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:24 GMT
ADD file:9a4f77dfaba7fd2aa78186e4ef0e7486ad55101cefc1fabbc1b385601bb38920 in / 
# Wed, 29 Mar 2023 18:19:24 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 02:37:38 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 27 Apr 2023 19:23:59 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.1/traefik_v2.10.1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 27 Apr 2023 19:24:00 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 27 Apr 2023 19:24:00 GMT
EXPOSE 80
# Thu, 27 Apr 2023 19:24:00 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 27 Apr 2023 19:24:00 GMT
CMD ["traefik"]
# Thu, 27 Apr 2023 19:24:00 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:f56be85fc22e46face30e2c3de3f7fe7c15f8fd7c4e5add29d7f64b87abdaa09`  
		Last Modified: Wed, 29 Mar 2023 18:19:57 GMT  
		Size: 3.4 MB (3374563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d055169f9c6f7e08b88a6ef90eba203750fcc51761ecb994e40aa2aaa640ff72`  
		Last Modified: Thu, 30 Mar 2023 02:38:35 GMT  
		Size: 622.2 KB (622239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56d2f042306d84d6b5581bdb96cc47a568cd2c8f18c778d4bdd4289f10ad8955`  
		Last Modified: Thu, 27 Apr 2023 19:24:26 GMT  
		Size: 37.0 MB (36993226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06c7eaf9711b1292ae5a5c1d70177cba7f0aeba30e0d974832bc5729ae07708a`  
		Last Modified: Thu, 27 Apr 2023 19:24:20 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.10` - linux; arm variant v6

```console
$ docker pull traefik@sha256:f67d07c8c40f742e8fd5b071bf8804690f631b28e9ccef7ecb9b0b6e8e3fc76c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.6 MB (38551154 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d02830f09811f97f72174cd791d4a3781bbafe3452c20d6fcd5ed0bc09fdcfd`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 14 Jun 2023 18:49:25 GMT
ADD file:07e668ef139dce7f076143a30b89ff57885c8539d8b5764ac1bd5277d9936702 in / 
# Wed, 14 Jun 2023 18:49:25 GMT
CMD ["/bin/sh"]
# Wed, 14 Jun 2023 20:12:29 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 14 Jun 2023 20:12:34 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.1/traefik_v2.10.1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 14 Jun 2023 20:12:34 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 14 Jun 2023 20:12:34 GMT
EXPOSE 80
# Wed, 14 Jun 2023 20:12:34 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 14 Jun 2023 20:12:35 GMT
CMD ["traefik"]
# Wed, 14 Jun 2023 20:12:35 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:33ec62e98ceea71d24212ee03e239c2d5538dbe7c98f41c42e8b2693fedf58fb`  
		Last Modified: Wed, 14 Jun 2023 18:50:00 GMT  
		Size: 3.1 MB (3110916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3456aa2bab6b1577d1ef938c6047142d2661cfa237d7988bc621c795148c4f9`  
		Last Modified: Wed, 14 Jun 2023 20:13:06 GMT  
		Size: 624.6 KB (624561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e1f88f7ccafe6c44c30bccec04fdf7523c60284c5bfc2184f657e61bea7b410`  
		Last Modified: Wed, 14 Jun 2023 20:13:12 GMT  
		Size: 34.8 MB (34815309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ae5708ba9c2b61ea7f0086f0ef7438f9a4db8e6abbedf44bd6898d2e9ed465b`  
		Last Modified: Wed, 14 Jun 2023 20:13:06 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.10` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:38ad4f0cffc281d86fd8512f384d194e24d0e47788c96d2402f243c62d655fb1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.7 MB (37747171 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:28c2c5ecdf8f6666c38b75756b057e2f96002102211ee1d2b5df7615bcf2c106`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:18 GMT
ADD file:e51d4089e73ad6dee52b31f0c8059a00c17df6e23f6741fe11b43bd84cc99008 in / 
# Wed, 29 Mar 2023 17:39:18 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 03:26:37 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 27 Apr 2023 18:50:16 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.1/traefik_v2.10.1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 27 Apr 2023 18:50:16 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 27 Apr 2023 18:50:16 GMT
EXPOSE 80
# Thu, 27 Apr 2023 18:50:16 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 27 Apr 2023 18:50:16 GMT
CMD ["traefik"]
# Thu, 27 Apr 2023 18:50:16 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:c41833b44d910632b415cd89a9cdaa4d62c9725dc56c99a7ddadafd6719960f9`  
		Last Modified: Wed, 29 Mar 2023 17:39:44 GMT  
		Size: 3.3 MB (3261854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4336eee5b1b811f9668d2251fb67e6099c4089ef7b26ade14aacd2f5f0982e06`  
		Last Modified: Thu, 30 Mar 2023 03:27:34 GMT  
		Size: 624.2 KB (624204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb3006acbb0f5f363c1104c94bf762bb2252f9b7f29d8c5b2f74412630c4af33`  
		Last Modified: Thu, 27 Apr 2023 18:50:38 GMT  
		Size: 33.9 MB (33860745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6ecd274862a81d7d04859e42c5c35cd1f4851afcd0aaa61e481abe26bbfb6ca`  
		Last Modified: Thu, 27 Apr 2023 18:50:34 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.10` - linux; s390x

```console
$ docker pull traefik@sha256:5fed19f3ecb9f6c2438c022696eb56228cfadaccee43a52b0a2bdb4d701925cd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.7 MB (39660993 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7634a95de667e3145cb226864ab946f751a613a045b069611e2db5e078083589`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 29 Mar 2023 17:41:57 GMT
ADD file:675ad8acf4b076e34aeeba26dd482be7640df5912b1ec5e3183b7eb69c01e83e in / 
# Wed, 29 Mar 2023 17:41:57 GMT
CMD ["/bin/sh"]
# Tue, 09 May 2023 23:57:51 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 09 May 2023 23:57:55 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.1/traefik_v2.10.1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Tue, 09 May 2023 23:57:57 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 09 May 2023 23:57:57 GMT
EXPOSE 80
# Tue, 09 May 2023 23:57:57 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 09 May 2023 23:57:57 GMT
CMD ["traefik"]
# Tue, 09 May 2023 23:57:57 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:a76f78d8854217635d8049ec8501edb806f961e72989cfff8503982e6ff2579d`  
		Last Modified: Wed, 29 Mar 2023 17:42:31 GMT  
		Size: 3.2 MB (3175187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aa8506383024e4e72ae2aa2e28d39f346912e8002e883f12c16c3e78b076687`  
		Last Modified: Tue, 09 May 2023 23:58:26 GMT  
		Size: 622.8 KB (622785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71f308ec932ffa02b0679ce4a37a19c241bbf0edffeb07c562c81096e2da38ca`  
		Last Modified: Tue, 09 May 2023 23:58:32 GMT  
		Size: 35.9 MB (35862652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58531206b398f1e9bcb368c1a724cc336a6100fc764fb28153ba3f97f79c78a8`  
		Last Modified: Tue, 09 May 2023 23:58:26 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:2.10-windowsservercore-1809`

```console
$ docker pull traefik@sha256:f16636d4d18fea046d66cb57fa0e90feaeb8ecbf1ca8f4182848481259f07eed
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4377; amd64

### `traefik:2.10-windowsservercore-1809` - windows version 10.0.17763.4377; amd64

```console
$ docker pull traefik@sha256:c888963af81054ac8c158404fbacff203fc05de699fd77ef99fdb276b0e742e0
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2109597280 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4493990f99f036c842802ae6b9593cf761ac18dbc67fd5cd1a322a84c2697c5e`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Fri, 05 May 2023 12:05:28 GMT
RUN Install update 10.0.17763.4377
# Wed, 10 May 2023 00:36:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 May 2023 06:31:45 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.10.1/traefik_v2.10.1_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Wed, 10 May 2023 06:31:46 GMT
EXPOSE 80
# Wed, 10 May 2023 06:31:47 GMT
ENTRYPOINT ["/traefik"]
# Wed, 10 May 2023 06:31:48 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e01de39a0c44e24aa1912078d32ee54389b71154e509138cc4f5d1de42e7a32a`  
		Last Modified: Wed, 10 May 2023 01:47:41 GMT  
		Size: 364.1 MB (364091294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15a238e462da347b2e29386c9883c0ec93c8dbce311782ea1c5abbec2a31d884`  
		Last Modified: Wed, 10 May 2023 01:46:46 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df6b1b568e48ea9b9c1126801eb055cc1d9aa1e21270219140c58f2e1253a636`  
		Last Modified: Wed, 10 May 2023 07:14:51 GMT  
		Size: 37.6 MB (37556455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f754667a3def555298e795f9f84b666f44e7d683178bc69b2765cc10fa741ec1`  
		Last Modified: Wed, 10 May 2023 07:14:44 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:269055700abc29f93e7940722c0a8c7c9423dd04dd3dcbf84caac07612d4b1cc`  
		Last Modified: Wed, 10 May 2023 07:14:44 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdc6c3594a8fea61840c387597d673ca691a7633347d397c73b3b0b849a173d1`  
		Last Modified: Wed, 10 May 2023 07:14:44 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:2.10.1`

```console
$ docker pull traefik@sha256:aae49c77988f065f91948477368475be36d74f46e7eb7b25ab1a8444266d2b0e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:2.10.1` - linux; amd64

```console
$ docker pull traefik@sha256:e01d05a30cfed0f79a9ecfb4942662c654ff2d8a39a80f030d4d58d9eb9ec0d1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.0 MB (40990396 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:63d7224eb30e1c2f2976e0043c6cb6f4f7f9bebb820253dc65998bbd747fcc85`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:24 GMT
ADD file:9a4f77dfaba7fd2aa78186e4ef0e7486ad55101cefc1fabbc1b385601bb38920 in / 
# Wed, 29 Mar 2023 18:19:24 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 02:37:38 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 27 Apr 2023 19:23:59 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.1/traefik_v2.10.1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 27 Apr 2023 19:24:00 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 27 Apr 2023 19:24:00 GMT
EXPOSE 80
# Thu, 27 Apr 2023 19:24:00 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 27 Apr 2023 19:24:00 GMT
CMD ["traefik"]
# Thu, 27 Apr 2023 19:24:00 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:f56be85fc22e46face30e2c3de3f7fe7c15f8fd7c4e5add29d7f64b87abdaa09`  
		Last Modified: Wed, 29 Mar 2023 18:19:57 GMT  
		Size: 3.4 MB (3374563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d055169f9c6f7e08b88a6ef90eba203750fcc51761ecb994e40aa2aaa640ff72`  
		Last Modified: Thu, 30 Mar 2023 02:38:35 GMT  
		Size: 622.2 KB (622239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56d2f042306d84d6b5581bdb96cc47a568cd2c8f18c778d4bdd4289f10ad8955`  
		Last Modified: Thu, 27 Apr 2023 19:24:26 GMT  
		Size: 37.0 MB (36993226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06c7eaf9711b1292ae5a5c1d70177cba7f0aeba30e0d974832bc5729ae07708a`  
		Last Modified: Thu, 27 Apr 2023 19:24:20 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.10.1` - linux; arm variant v6

```console
$ docker pull traefik@sha256:f67d07c8c40f742e8fd5b071bf8804690f631b28e9ccef7ecb9b0b6e8e3fc76c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.6 MB (38551154 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d02830f09811f97f72174cd791d4a3781bbafe3452c20d6fcd5ed0bc09fdcfd`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 14 Jun 2023 18:49:25 GMT
ADD file:07e668ef139dce7f076143a30b89ff57885c8539d8b5764ac1bd5277d9936702 in / 
# Wed, 14 Jun 2023 18:49:25 GMT
CMD ["/bin/sh"]
# Wed, 14 Jun 2023 20:12:29 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 14 Jun 2023 20:12:34 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.1/traefik_v2.10.1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 14 Jun 2023 20:12:34 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 14 Jun 2023 20:12:34 GMT
EXPOSE 80
# Wed, 14 Jun 2023 20:12:34 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 14 Jun 2023 20:12:35 GMT
CMD ["traefik"]
# Wed, 14 Jun 2023 20:12:35 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:33ec62e98ceea71d24212ee03e239c2d5538dbe7c98f41c42e8b2693fedf58fb`  
		Last Modified: Wed, 14 Jun 2023 18:50:00 GMT  
		Size: 3.1 MB (3110916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3456aa2bab6b1577d1ef938c6047142d2661cfa237d7988bc621c795148c4f9`  
		Last Modified: Wed, 14 Jun 2023 20:13:06 GMT  
		Size: 624.6 KB (624561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e1f88f7ccafe6c44c30bccec04fdf7523c60284c5bfc2184f657e61bea7b410`  
		Last Modified: Wed, 14 Jun 2023 20:13:12 GMT  
		Size: 34.8 MB (34815309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ae5708ba9c2b61ea7f0086f0ef7438f9a4db8e6abbedf44bd6898d2e9ed465b`  
		Last Modified: Wed, 14 Jun 2023 20:13:06 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.10.1` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:38ad4f0cffc281d86fd8512f384d194e24d0e47788c96d2402f243c62d655fb1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.7 MB (37747171 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:28c2c5ecdf8f6666c38b75756b057e2f96002102211ee1d2b5df7615bcf2c106`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:18 GMT
ADD file:e51d4089e73ad6dee52b31f0c8059a00c17df6e23f6741fe11b43bd84cc99008 in / 
# Wed, 29 Mar 2023 17:39:18 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 03:26:37 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 27 Apr 2023 18:50:16 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.1/traefik_v2.10.1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 27 Apr 2023 18:50:16 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 27 Apr 2023 18:50:16 GMT
EXPOSE 80
# Thu, 27 Apr 2023 18:50:16 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 27 Apr 2023 18:50:16 GMT
CMD ["traefik"]
# Thu, 27 Apr 2023 18:50:16 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:c41833b44d910632b415cd89a9cdaa4d62c9725dc56c99a7ddadafd6719960f9`  
		Last Modified: Wed, 29 Mar 2023 17:39:44 GMT  
		Size: 3.3 MB (3261854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4336eee5b1b811f9668d2251fb67e6099c4089ef7b26ade14aacd2f5f0982e06`  
		Last Modified: Thu, 30 Mar 2023 03:27:34 GMT  
		Size: 624.2 KB (624204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb3006acbb0f5f363c1104c94bf762bb2252f9b7f29d8c5b2f74412630c4af33`  
		Last Modified: Thu, 27 Apr 2023 18:50:38 GMT  
		Size: 33.9 MB (33860745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6ecd274862a81d7d04859e42c5c35cd1f4851afcd0aaa61e481abe26bbfb6ca`  
		Last Modified: Thu, 27 Apr 2023 18:50:34 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.10.1` - linux; s390x

```console
$ docker pull traefik@sha256:5fed19f3ecb9f6c2438c022696eb56228cfadaccee43a52b0a2bdb4d701925cd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.7 MB (39660993 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7634a95de667e3145cb226864ab946f751a613a045b069611e2db5e078083589`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 29 Mar 2023 17:41:57 GMT
ADD file:675ad8acf4b076e34aeeba26dd482be7640df5912b1ec5e3183b7eb69c01e83e in / 
# Wed, 29 Mar 2023 17:41:57 GMT
CMD ["/bin/sh"]
# Tue, 09 May 2023 23:57:51 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 09 May 2023 23:57:55 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.1/traefik_v2.10.1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Tue, 09 May 2023 23:57:57 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 09 May 2023 23:57:57 GMT
EXPOSE 80
# Tue, 09 May 2023 23:57:57 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 09 May 2023 23:57:57 GMT
CMD ["traefik"]
# Tue, 09 May 2023 23:57:57 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:a76f78d8854217635d8049ec8501edb806f961e72989cfff8503982e6ff2579d`  
		Last Modified: Wed, 29 Mar 2023 17:42:31 GMT  
		Size: 3.2 MB (3175187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aa8506383024e4e72ae2aa2e28d39f346912e8002e883f12c16c3e78b076687`  
		Last Modified: Tue, 09 May 2023 23:58:26 GMT  
		Size: 622.8 KB (622785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71f308ec932ffa02b0679ce4a37a19c241bbf0edffeb07c562c81096e2da38ca`  
		Last Modified: Tue, 09 May 2023 23:58:32 GMT  
		Size: 35.9 MB (35862652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58531206b398f1e9bcb368c1a724cc336a6100fc764fb28153ba3f97f79c78a8`  
		Last Modified: Tue, 09 May 2023 23:58:26 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:2.10.1-windowsservercore-1809`

```console
$ docker pull traefik@sha256:f16636d4d18fea046d66cb57fa0e90feaeb8ecbf1ca8f4182848481259f07eed
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4377; amd64

### `traefik:2.10.1-windowsservercore-1809` - windows version 10.0.17763.4377; amd64

```console
$ docker pull traefik@sha256:c888963af81054ac8c158404fbacff203fc05de699fd77ef99fdb276b0e742e0
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2109597280 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4493990f99f036c842802ae6b9593cf761ac18dbc67fd5cd1a322a84c2697c5e`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Fri, 05 May 2023 12:05:28 GMT
RUN Install update 10.0.17763.4377
# Wed, 10 May 2023 00:36:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 May 2023 06:31:45 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.10.1/traefik_v2.10.1_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Wed, 10 May 2023 06:31:46 GMT
EXPOSE 80
# Wed, 10 May 2023 06:31:47 GMT
ENTRYPOINT ["/traefik"]
# Wed, 10 May 2023 06:31:48 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e01de39a0c44e24aa1912078d32ee54389b71154e509138cc4f5d1de42e7a32a`  
		Last Modified: Wed, 10 May 2023 01:47:41 GMT  
		Size: 364.1 MB (364091294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15a238e462da347b2e29386c9883c0ec93c8dbce311782ea1c5abbec2a31d884`  
		Last Modified: Wed, 10 May 2023 01:46:46 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df6b1b568e48ea9b9c1126801eb055cc1d9aa1e21270219140c58f2e1253a636`  
		Last Modified: Wed, 10 May 2023 07:14:51 GMT  
		Size: 37.6 MB (37556455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f754667a3def555298e795f9f84b666f44e7d683178bc69b2765cc10fa741ec1`  
		Last Modified: Wed, 10 May 2023 07:14:44 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:269055700abc29f93e7940722c0a8c7c9423dd04dd3dcbf84caac07612d4b1cc`  
		Last Modified: Wed, 10 May 2023 07:14:44 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdc6c3594a8fea61840c387597d673ca691a7633347d397c73b3b0b849a173d1`  
		Last Modified: Wed, 10 May 2023 07:14:44 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:3.0`

```console
$ docker pull traefik@sha256:83e7b36fbe4096887d144ba82c51b891893ad3eb5f891daf300f5cf49b9d61d3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:3.0` - linux; amd64

```console
$ docker pull traefik@sha256:a239deca1c7682fe9bb6a32e54364c7ff460205fa0e87c02bfeb66efb3f3a3d1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.6 MB (40562953 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:42fc5a7c2d34a752fce6439cf3dc08ac747649d7712bc265c7dd7d1b38a2a45b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:33 GMT
ADD file:08ad6c1c886a26e30ae4ab103ff377ee6cfbc1be2437fa227ec28a335c63d78a in / 
# Wed, 29 Mar 2023 18:19:33 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 02:37:32 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 30 Mar 2023 02:37:35 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta2/traefik_v3.0.0-beta2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 30 Mar 2023 02:37:35 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 30 Mar 2023 02:37:35 GMT
EXPOSE 80
# Thu, 30 Mar 2023 02:37:35 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 30 Mar 2023 02:37:35 GMT
CMD ["traefik"]
# Thu, 30 Mar 2023 02:37:36 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:0ce1dd7918a48990ab749aab2e805c26f691a3a8103495530e7ea5a1d168af4a`  
		Last Modified: Wed, 29 Mar 2023 18:20:17 GMT  
		Size: 2.8 MB (2826596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c11624eb8d0cca298aa32848e39318bbc75ab1c404423d1d47c670fa60354e3`  
		Last Modified: Thu, 30 Mar 2023 02:38:16 GMT  
		Size: 661.1 KB (661099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a9d40a9765a3ede8e4ec67030b20d484fedcea2ad98ee2b231ec3d86e6fd1b6`  
		Last Modified: Thu, 30 Mar 2023 02:38:21 GMT  
		Size: 37.1 MB (37074890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fca61e22e5a1dbbdeea08d3e394601c2c5492fc65d19af813ef66cc36a7d582`  
		Last Modified: Thu, 30 Mar 2023 02:38:15 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:3.0` - linux; arm variant v6

```console
$ docker pull traefik@sha256:0e010dd7b60c3960f903b07854cae707e691496f1491f0447ca2635b5a374a6d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.3 MB (38289085 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ee0012c6d54cfd4da66d0da5e01f3dc4f70609eec928ce429e71a5efa02c96b3`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 14 Jun 2023 18:49:32 GMT
ADD file:b987db82fa4ce6e623de49a50612c1fd91c5ab2209a62a5727ab3436c2923e91 in / 
# Wed, 14 Jun 2023 18:49:32 GMT
CMD ["/bin/sh"]
# Wed, 14 Jun 2023 20:12:22 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 14 Jun 2023 20:12:26 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta2/traefik_v3.0.0-beta2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 14 Jun 2023 20:12:26 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 14 Jun 2023 20:12:26 GMT
EXPOSE 80
# Wed, 14 Jun 2023 20:12:26 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 14 Jun 2023 20:12:26 GMT
CMD ["traefik"]
# Wed, 14 Jun 2023 20:12:26 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:41c5c5b38e13af18def277385607129664fb24993d262d4b601a381e776482a9`  
		Last Modified: Wed, 14 Jun 2023 18:50:19 GMT  
		Size: 2.6 MB (2633060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:718cfe2cb66c053a8fdb09adf88b20a52f260f22abd38cba68cc2838ee33e73d`  
		Last Modified: Wed, 14 Jun 2023 20:12:46 GMT  
		Size: 666.3 KB (666349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47b2cef5f2c79471c563b3c10376140084b51c097de00e9be0b758219ab95e5c`  
		Last Modified: Wed, 14 Jun 2023 20:12:52 GMT  
		Size: 35.0 MB (34989308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66078e59ed6730404193e57cea654480d0731663c7a068349344e0a681d1c660`  
		Last Modified: Wed, 14 Jun 2023 20:12:46 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:3.0` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:529410986a68c6e7989a5a08afa53d087795a2f1406977d5d6b183bfdfab65dd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.4 MB (37408212 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e4bfdbd12bed1c2e46296bb16021a1eea4269055e03fdf9e30c035e5f9e8dc4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:22 GMT
ADD file:4acfda16c71abce07068ed23839e9de60c1d1145ab8002b3a92c15b1e80d4356 in / 
# Wed, 29 Mar 2023 17:39:23 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 03:26:31 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 30 Mar 2023 03:26:34 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta2/traefik_v3.0.0-beta2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 30 Mar 2023 03:26:35 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 30 Mar 2023 03:26:35 GMT
EXPOSE 80
# Thu, 30 Mar 2023 03:26:35 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 30 Mar 2023 03:26:35 GMT
CMD ["traefik"]
# Thu, 30 Mar 2023 03:26:35 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:60a00c11adf5202a365ec8215b889c3390d67fa295ab79940e1c5dc4cbed9db1`  
		Last Modified: Wed, 29 Mar 2023 17:40:04 GMT  
		Size: 2.7 MB (2722002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d019fab0470c352dfa2ff6c01be8f1d0344d43e9431a28656e78c5cabd03e67f`  
		Last Modified: Thu, 30 Mar 2023 03:27:17 GMT  
		Size: 662.3 KB (662323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d82ed46bb3966bf021d56f3bfda66ada1ddde7199ee9d3446ebcbeffec692004`  
		Last Modified: Thu, 30 Mar 2023 03:27:20 GMT  
		Size: 34.0 MB (34023520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07a93ddfbde23c1aa20ccac6b7cd3dcbda52d11c2b1627d41dc7fa169bd46430`  
		Last Modified: Thu, 30 Mar 2023 03:27:16 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:3.0` - linux; s390x

```console
$ docker pull traefik@sha256:bbf1710b9a47f8ec5a04c849b5eabca1601d8c3d14771376db863d4bfb11267c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.1 MB (39132224 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a7797b8a6b1786adb45fd822e034429307f0e6d9835934dff30e1685c3d7253`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 29 Mar 2023 17:42:07 GMT
ADD file:5cf392863cd9a0735de88f9e7dab93c9e74aca59ca05b792943cf3b621ea2c59 in / 
# Wed, 29 Mar 2023 17:42:07 GMT
CMD ["/bin/sh"]
# Tue, 09 May 2023 23:57:38 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 09 May 2023 23:57:42 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta2/traefik_v3.0.0-beta2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Tue, 09 May 2023 23:57:44 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 09 May 2023 23:57:44 GMT
EXPOSE 80
# Tue, 09 May 2023 23:57:44 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 09 May 2023 23:57:44 GMT
CMD ["traefik"]
# Tue, 09 May 2023 23:57:44 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:1536575ac9c5f5fff4522c60d4610af0a52be584c36e652080c6c0ad169d4f27`  
		Last Modified: Wed, 29 Mar 2023 17:42:42 GMT  
		Size: 2.6 MB (2610636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa7a4deefee64d3e0ac000d06c44544635381ead6c9ce624aad695fd76bdde33`  
		Last Modified: Tue, 09 May 2023 23:58:12 GMT  
		Size: 665.8 KB (665799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a2ced6eac60c1c9707c57590d27e69315354f9d304ec2af3e7f07d5a2bec0b4`  
		Last Modified: Tue, 09 May 2023 23:58:18 GMT  
		Size: 35.9 MB (35855421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b58a1e76f2b69535b5f8ea9cdfda36f79ee2e5fd3194ee2e9ce12fd841672a09`  
		Last Modified: Tue, 09 May 2023 23:58:12 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:3.0-windowsservercore-1809`

```console
$ docker pull traefik@sha256:a029ead52682acc7e61cd89a8807ddebd7d1d5df26f9249c3dd1003991a1c8da
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4377; amd64

### `traefik:3.0-windowsservercore-1809` - windows version 10.0.17763.4377; amd64

```console
$ docker pull traefik@sha256:78a79fdcd7524d1a0efa1937dd822c5018cae9333ceace3ea65fd9e9f8673847
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2109691146 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e40512720c63bc941384872c5997d1356d112a9a09d42b25f64e228937c02ba7`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Fri, 05 May 2023 12:05:28 GMT
RUN Install update 10.0.17763.4377
# Wed, 10 May 2023 00:36:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 May 2023 06:30:17 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v3.0.0-beta2/traefik_v3.0.0-beta2_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Wed, 10 May 2023 06:30:18 GMT
EXPOSE 80
# Wed, 10 May 2023 06:30:19 GMT
ENTRYPOINT ["/traefik"]
# Wed, 10 May 2023 06:30:20 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e01de39a0c44e24aa1912078d32ee54389b71154e509138cc4f5d1de42e7a32a`  
		Last Modified: Wed, 10 May 2023 01:47:41 GMT  
		Size: 364.1 MB (364091294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15a238e462da347b2e29386c9883c0ec93c8dbce311782ea1c5abbec2a31d884`  
		Last Modified: Wed, 10 May 2023 01:46:46 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f5d58d623c979fa789cd0569f498ae640679c8c40d6aa12ba6f0714a8524a8b`  
		Last Modified: Wed, 10 May 2023 07:14:30 GMT  
		Size: 37.7 MB (37650316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69d5e987e1a63a8e5472dafacad7b03bd1ceebc572fdfdec77bcd778030bfd30`  
		Last Modified: Wed, 10 May 2023 07:14:22 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1e4c1a5897d7faefb9bb9c57c4b06244db88d7039610fc61a720f24e98b8108`  
		Last Modified: Wed, 10 May 2023 07:14:22 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9def7bdf656e22544902494ac6ffb34aef316d5f2d2b5cd77f1d7b9fe5174bed`  
		Last Modified: Wed, 10 May 2023 07:14:22 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:3.0.0-beta2`

```console
$ docker pull traefik@sha256:83e7b36fbe4096887d144ba82c51b891893ad3eb5f891daf300f5cf49b9d61d3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:3.0.0-beta2` - linux; amd64

```console
$ docker pull traefik@sha256:a239deca1c7682fe9bb6a32e54364c7ff460205fa0e87c02bfeb66efb3f3a3d1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.6 MB (40562953 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:42fc5a7c2d34a752fce6439cf3dc08ac747649d7712bc265c7dd7d1b38a2a45b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:33 GMT
ADD file:08ad6c1c886a26e30ae4ab103ff377ee6cfbc1be2437fa227ec28a335c63d78a in / 
# Wed, 29 Mar 2023 18:19:33 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 02:37:32 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 30 Mar 2023 02:37:35 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta2/traefik_v3.0.0-beta2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 30 Mar 2023 02:37:35 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 30 Mar 2023 02:37:35 GMT
EXPOSE 80
# Thu, 30 Mar 2023 02:37:35 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 30 Mar 2023 02:37:35 GMT
CMD ["traefik"]
# Thu, 30 Mar 2023 02:37:36 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:0ce1dd7918a48990ab749aab2e805c26f691a3a8103495530e7ea5a1d168af4a`  
		Last Modified: Wed, 29 Mar 2023 18:20:17 GMT  
		Size: 2.8 MB (2826596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c11624eb8d0cca298aa32848e39318bbc75ab1c404423d1d47c670fa60354e3`  
		Last Modified: Thu, 30 Mar 2023 02:38:16 GMT  
		Size: 661.1 KB (661099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a9d40a9765a3ede8e4ec67030b20d484fedcea2ad98ee2b231ec3d86e6fd1b6`  
		Last Modified: Thu, 30 Mar 2023 02:38:21 GMT  
		Size: 37.1 MB (37074890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fca61e22e5a1dbbdeea08d3e394601c2c5492fc65d19af813ef66cc36a7d582`  
		Last Modified: Thu, 30 Mar 2023 02:38:15 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:3.0.0-beta2` - linux; arm variant v6

```console
$ docker pull traefik@sha256:0e010dd7b60c3960f903b07854cae707e691496f1491f0447ca2635b5a374a6d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.3 MB (38289085 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ee0012c6d54cfd4da66d0da5e01f3dc4f70609eec928ce429e71a5efa02c96b3`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 14 Jun 2023 18:49:32 GMT
ADD file:b987db82fa4ce6e623de49a50612c1fd91c5ab2209a62a5727ab3436c2923e91 in / 
# Wed, 14 Jun 2023 18:49:32 GMT
CMD ["/bin/sh"]
# Wed, 14 Jun 2023 20:12:22 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 14 Jun 2023 20:12:26 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta2/traefik_v3.0.0-beta2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 14 Jun 2023 20:12:26 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 14 Jun 2023 20:12:26 GMT
EXPOSE 80
# Wed, 14 Jun 2023 20:12:26 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 14 Jun 2023 20:12:26 GMT
CMD ["traefik"]
# Wed, 14 Jun 2023 20:12:26 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:41c5c5b38e13af18def277385607129664fb24993d262d4b601a381e776482a9`  
		Last Modified: Wed, 14 Jun 2023 18:50:19 GMT  
		Size: 2.6 MB (2633060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:718cfe2cb66c053a8fdb09adf88b20a52f260f22abd38cba68cc2838ee33e73d`  
		Last Modified: Wed, 14 Jun 2023 20:12:46 GMT  
		Size: 666.3 KB (666349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47b2cef5f2c79471c563b3c10376140084b51c097de00e9be0b758219ab95e5c`  
		Last Modified: Wed, 14 Jun 2023 20:12:52 GMT  
		Size: 35.0 MB (34989308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66078e59ed6730404193e57cea654480d0731663c7a068349344e0a681d1c660`  
		Last Modified: Wed, 14 Jun 2023 20:12:46 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:3.0.0-beta2` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:529410986a68c6e7989a5a08afa53d087795a2f1406977d5d6b183bfdfab65dd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.4 MB (37408212 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e4bfdbd12bed1c2e46296bb16021a1eea4269055e03fdf9e30c035e5f9e8dc4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:22 GMT
ADD file:4acfda16c71abce07068ed23839e9de60c1d1145ab8002b3a92c15b1e80d4356 in / 
# Wed, 29 Mar 2023 17:39:23 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 03:26:31 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 30 Mar 2023 03:26:34 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta2/traefik_v3.0.0-beta2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 30 Mar 2023 03:26:35 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 30 Mar 2023 03:26:35 GMT
EXPOSE 80
# Thu, 30 Mar 2023 03:26:35 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 30 Mar 2023 03:26:35 GMT
CMD ["traefik"]
# Thu, 30 Mar 2023 03:26:35 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:60a00c11adf5202a365ec8215b889c3390d67fa295ab79940e1c5dc4cbed9db1`  
		Last Modified: Wed, 29 Mar 2023 17:40:04 GMT  
		Size: 2.7 MB (2722002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d019fab0470c352dfa2ff6c01be8f1d0344d43e9431a28656e78c5cabd03e67f`  
		Last Modified: Thu, 30 Mar 2023 03:27:17 GMT  
		Size: 662.3 KB (662323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d82ed46bb3966bf021d56f3bfda66ada1ddde7199ee9d3446ebcbeffec692004`  
		Last Modified: Thu, 30 Mar 2023 03:27:20 GMT  
		Size: 34.0 MB (34023520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07a93ddfbde23c1aa20ccac6b7cd3dcbda52d11c2b1627d41dc7fa169bd46430`  
		Last Modified: Thu, 30 Mar 2023 03:27:16 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:3.0.0-beta2` - linux; s390x

```console
$ docker pull traefik@sha256:bbf1710b9a47f8ec5a04c849b5eabca1601d8c3d14771376db863d4bfb11267c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.1 MB (39132224 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a7797b8a6b1786adb45fd822e034429307f0e6d9835934dff30e1685c3d7253`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 29 Mar 2023 17:42:07 GMT
ADD file:5cf392863cd9a0735de88f9e7dab93c9e74aca59ca05b792943cf3b621ea2c59 in / 
# Wed, 29 Mar 2023 17:42:07 GMT
CMD ["/bin/sh"]
# Tue, 09 May 2023 23:57:38 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 09 May 2023 23:57:42 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta2/traefik_v3.0.0-beta2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Tue, 09 May 2023 23:57:44 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 09 May 2023 23:57:44 GMT
EXPOSE 80
# Tue, 09 May 2023 23:57:44 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 09 May 2023 23:57:44 GMT
CMD ["traefik"]
# Tue, 09 May 2023 23:57:44 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:1536575ac9c5f5fff4522c60d4610af0a52be584c36e652080c6c0ad169d4f27`  
		Last Modified: Wed, 29 Mar 2023 17:42:42 GMT  
		Size: 2.6 MB (2610636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa7a4deefee64d3e0ac000d06c44544635381ead6c9ce624aad695fd76bdde33`  
		Last Modified: Tue, 09 May 2023 23:58:12 GMT  
		Size: 665.8 KB (665799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a2ced6eac60c1c9707c57590d27e69315354f9d304ec2af3e7f07d5a2bec0b4`  
		Last Modified: Tue, 09 May 2023 23:58:18 GMT  
		Size: 35.9 MB (35855421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b58a1e76f2b69535b5f8ea9cdfda36f79ee2e5fd3194ee2e9ce12fd841672a09`  
		Last Modified: Tue, 09 May 2023 23:58:12 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:3.0.0-beta2-windowsservercore-1809`

```console
$ docker pull traefik@sha256:a029ead52682acc7e61cd89a8807ddebd7d1d5df26f9249c3dd1003991a1c8da
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4377; amd64

### `traefik:3.0.0-beta2-windowsservercore-1809` - windows version 10.0.17763.4377; amd64

```console
$ docker pull traefik@sha256:78a79fdcd7524d1a0efa1937dd822c5018cae9333ceace3ea65fd9e9f8673847
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2109691146 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e40512720c63bc941384872c5997d1356d112a9a09d42b25f64e228937c02ba7`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Fri, 05 May 2023 12:05:28 GMT
RUN Install update 10.0.17763.4377
# Wed, 10 May 2023 00:36:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 May 2023 06:30:17 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v3.0.0-beta2/traefik_v3.0.0-beta2_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Wed, 10 May 2023 06:30:18 GMT
EXPOSE 80
# Wed, 10 May 2023 06:30:19 GMT
ENTRYPOINT ["/traefik"]
# Wed, 10 May 2023 06:30:20 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e01de39a0c44e24aa1912078d32ee54389b71154e509138cc4f5d1de42e7a32a`  
		Last Modified: Wed, 10 May 2023 01:47:41 GMT  
		Size: 364.1 MB (364091294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15a238e462da347b2e29386c9883c0ec93c8dbce311782ea1c5abbec2a31d884`  
		Last Modified: Wed, 10 May 2023 01:46:46 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f5d58d623c979fa789cd0569f498ae640679c8c40d6aa12ba6f0714a8524a8b`  
		Last Modified: Wed, 10 May 2023 07:14:30 GMT  
		Size: 37.7 MB (37650316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69d5e987e1a63a8e5472dafacad7b03bd1ceebc572fdfdec77bcd778030bfd30`  
		Last Modified: Wed, 10 May 2023 07:14:22 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1e4c1a5897d7faefb9bb9c57c4b06244db88d7039610fc61a720f24e98b8108`  
		Last Modified: Wed, 10 May 2023 07:14:22 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9def7bdf656e22544902494ac6ffb34aef316d5f2d2b5cd77f1d7b9fe5174bed`  
		Last Modified: Wed, 10 May 2023 07:14:22 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:beaufort`

```console
$ docker pull traefik@sha256:83e7b36fbe4096887d144ba82c51b891893ad3eb5f891daf300f5cf49b9d61d3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:beaufort` - linux; amd64

```console
$ docker pull traefik@sha256:a239deca1c7682fe9bb6a32e54364c7ff460205fa0e87c02bfeb66efb3f3a3d1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.6 MB (40562953 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:42fc5a7c2d34a752fce6439cf3dc08ac747649d7712bc265c7dd7d1b38a2a45b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:33 GMT
ADD file:08ad6c1c886a26e30ae4ab103ff377ee6cfbc1be2437fa227ec28a335c63d78a in / 
# Wed, 29 Mar 2023 18:19:33 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 02:37:32 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 30 Mar 2023 02:37:35 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta2/traefik_v3.0.0-beta2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 30 Mar 2023 02:37:35 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 30 Mar 2023 02:37:35 GMT
EXPOSE 80
# Thu, 30 Mar 2023 02:37:35 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 30 Mar 2023 02:37:35 GMT
CMD ["traefik"]
# Thu, 30 Mar 2023 02:37:36 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:0ce1dd7918a48990ab749aab2e805c26f691a3a8103495530e7ea5a1d168af4a`  
		Last Modified: Wed, 29 Mar 2023 18:20:17 GMT  
		Size: 2.8 MB (2826596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c11624eb8d0cca298aa32848e39318bbc75ab1c404423d1d47c670fa60354e3`  
		Last Modified: Thu, 30 Mar 2023 02:38:16 GMT  
		Size: 661.1 KB (661099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a9d40a9765a3ede8e4ec67030b20d484fedcea2ad98ee2b231ec3d86e6fd1b6`  
		Last Modified: Thu, 30 Mar 2023 02:38:21 GMT  
		Size: 37.1 MB (37074890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fca61e22e5a1dbbdeea08d3e394601c2c5492fc65d19af813ef66cc36a7d582`  
		Last Modified: Thu, 30 Mar 2023 02:38:15 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:beaufort` - linux; arm variant v6

```console
$ docker pull traefik@sha256:0e010dd7b60c3960f903b07854cae707e691496f1491f0447ca2635b5a374a6d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.3 MB (38289085 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ee0012c6d54cfd4da66d0da5e01f3dc4f70609eec928ce429e71a5efa02c96b3`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 14 Jun 2023 18:49:32 GMT
ADD file:b987db82fa4ce6e623de49a50612c1fd91c5ab2209a62a5727ab3436c2923e91 in / 
# Wed, 14 Jun 2023 18:49:32 GMT
CMD ["/bin/sh"]
# Wed, 14 Jun 2023 20:12:22 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 14 Jun 2023 20:12:26 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta2/traefik_v3.0.0-beta2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 14 Jun 2023 20:12:26 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 14 Jun 2023 20:12:26 GMT
EXPOSE 80
# Wed, 14 Jun 2023 20:12:26 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 14 Jun 2023 20:12:26 GMT
CMD ["traefik"]
# Wed, 14 Jun 2023 20:12:26 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:41c5c5b38e13af18def277385607129664fb24993d262d4b601a381e776482a9`  
		Last Modified: Wed, 14 Jun 2023 18:50:19 GMT  
		Size: 2.6 MB (2633060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:718cfe2cb66c053a8fdb09adf88b20a52f260f22abd38cba68cc2838ee33e73d`  
		Last Modified: Wed, 14 Jun 2023 20:12:46 GMT  
		Size: 666.3 KB (666349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47b2cef5f2c79471c563b3c10376140084b51c097de00e9be0b758219ab95e5c`  
		Last Modified: Wed, 14 Jun 2023 20:12:52 GMT  
		Size: 35.0 MB (34989308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66078e59ed6730404193e57cea654480d0731663c7a068349344e0a681d1c660`  
		Last Modified: Wed, 14 Jun 2023 20:12:46 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:beaufort` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:529410986a68c6e7989a5a08afa53d087795a2f1406977d5d6b183bfdfab65dd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.4 MB (37408212 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e4bfdbd12bed1c2e46296bb16021a1eea4269055e03fdf9e30c035e5f9e8dc4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:22 GMT
ADD file:4acfda16c71abce07068ed23839e9de60c1d1145ab8002b3a92c15b1e80d4356 in / 
# Wed, 29 Mar 2023 17:39:23 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 03:26:31 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 30 Mar 2023 03:26:34 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta2/traefik_v3.0.0-beta2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 30 Mar 2023 03:26:35 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 30 Mar 2023 03:26:35 GMT
EXPOSE 80
# Thu, 30 Mar 2023 03:26:35 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 30 Mar 2023 03:26:35 GMT
CMD ["traefik"]
# Thu, 30 Mar 2023 03:26:35 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:60a00c11adf5202a365ec8215b889c3390d67fa295ab79940e1c5dc4cbed9db1`  
		Last Modified: Wed, 29 Mar 2023 17:40:04 GMT  
		Size: 2.7 MB (2722002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d019fab0470c352dfa2ff6c01be8f1d0344d43e9431a28656e78c5cabd03e67f`  
		Last Modified: Thu, 30 Mar 2023 03:27:17 GMT  
		Size: 662.3 KB (662323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d82ed46bb3966bf021d56f3bfda66ada1ddde7199ee9d3446ebcbeffec692004`  
		Last Modified: Thu, 30 Mar 2023 03:27:20 GMT  
		Size: 34.0 MB (34023520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07a93ddfbde23c1aa20ccac6b7cd3dcbda52d11c2b1627d41dc7fa169bd46430`  
		Last Modified: Thu, 30 Mar 2023 03:27:16 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:beaufort` - linux; s390x

```console
$ docker pull traefik@sha256:bbf1710b9a47f8ec5a04c849b5eabca1601d8c3d14771376db863d4bfb11267c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.1 MB (39132224 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a7797b8a6b1786adb45fd822e034429307f0e6d9835934dff30e1685c3d7253`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 29 Mar 2023 17:42:07 GMT
ADD file:5cf392863cd9a0735de88f9e7dab93c9e74aca59ca05b792943cf3b621ea2c59 in / 
# Wed, 29 Mar 2023 17:42:07 GMT
CMD ["/bin/sh"]
# Tue, 09 May 2023 23:57:38 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 09 May 2023 23:57:42 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta2/traefik_v3.0.0-beta2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Tue, 09 May 2023 23:57:44 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 09 May 2023 23:57:44 GMT
EXPOSE 80
# Tue, 09 May 2023 23:57:44 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 09 May 2023 23:57:44 GMT
CMD ["traefik"]
# Tue, 09 May 2023 23:57:44 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:1536575ac9c5f5fff4522c60d4610af0a52be584c36e652080c6c0ad169d4f27`  
		Last Modified: Wed, 29 Mar 2023 17:42:42 GMT  
		Size: 2.6 MB (2610636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa7a4deefee64d3e0ac000d06c44544635381ead6c9ce624aad695fd76bdde33`  
		Last Modified: Tue, 09 May 2023 23:58:12 GMT  
		Size: 665.8 KB (665799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a2ced6eac60c1c9707c57590d27e69315354f9d304ec2af3e7f07d5a2bec0b4`  
		Last Modified: Tue, 09 May 2023 23:58:18 GMT  
		Size: 35.9 MB (35855421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b58a1e76f2b69535b5f8ea9cdfda36f79ee2e5fd3194ee2e9ce12fd841672a09`  
		Last Modified: Tue, 09 May 2023 23:58:12 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:beaufort-windowsservercore-1809`

```console
$ docker pull traefik@sha256:a029ead52682acc7e61cd89a8807ddebd7d1d5df26f9249c3dd1003991a1c8da
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4377; amd64

### `traefik:beaufort-windowsservercore-1809` - windows version 10.0.17763.4377; amd64

```console
$ docker pull traefik@sha256:78a79fdcd7524d1a0efa1937dd822c5018cae9333ceace3ea65fd9e9f8673847
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2109691146 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e40512720c63bc941384872c5997d1356d112a9a09d42b25f64e228937c02ba7`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Fri, 05 May 2023 12:05:28 GMT
RUN Install update 10.0.17763.4377
# Wed, 10 May 2023 00:36:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 May 2023 06:30:17 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v3.0.0-beta2/traefik_v3.0.0-beta2_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Wed, 10 May 2023 06:30:18 GMT
EXPOSE 80
# Wed, 10 May 2023 06:30:19 GMT
ENTRYPOINT ["/traefik"]
# Wed, 10 May 2023 06:30:20 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e01de39a0c44e24aa1912078d32ee54389b71154e509138cc4f5d1de42e7a32a`  
		Last Modified: Wed, 10 May 2023 01:47:41 GMT  
		Size: 364.1 MB (364091294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15a238e462da347b2e29386c9883c0ec93c8dbce311782ea1c5abbec2a31d884`  
		Last Modified: Wed, 10 May 2023 01:46:46 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f5d58d623c979fa789cd0569f498ae640679c8c40d6aa12ba6f0714a8524a8b`  
		Last Modified: Wed, 10 May 2023 07:14:30 GMT  
		Size: 37.7 MB (37650316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69d5e987e1a63a8e5472dafacad7b03bd1ceebc572fdfdec77bcd778030bfd30`  
		Last Modified: Wed, 10 May 2023 07:14:22 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1e4c1a5897d7faefb9bb9c57c4b06244db88d7039610fc61a720f24e98b8108`  
		Last Modified: Wed, 10 May 2023 07:14:22 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9def7bdf656e22544902494ac6ffb34aef316d5f2d2b5cd77f1d7b9fe5174bed`  
		Last Modified: Wed, 10 May 2023 07:14:22 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:latest`

```console
$ docker pull traefik@sha256:aae49c77988f065f91948477368475be36d74f46e7eb7b25ab1a8444266d2b0e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:latest` - linux; amd64

```console
$ docker pull traefik@sha256:e01d05a30cfed0f79a9ecfb4942662c654ff2d8a39a80f030d4d58d9eb9ec0d1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.0 MB (40990396 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:63d7224eb30e1c2f2976e0043c6cb6f4f7f9bebb820253dc65998bbd747fcc85`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:24 GMT
ADD file:9a4f77dfaba7fd2aa78186e4ef0e7486ad55101cefc1fabbc1b385601bb38920 in / 
# Wed, 29 Mar 2023 18:19:24 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 02:37:38 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 27 Apr 2023 19:23:59 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.1/traefik_v2.10.1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 27 Apr 2023 19:24:00 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 27 Apr 2023 19:24:00 GMT
EXPOSE 80
# Thu, 27 Apr 2023 19:24:00 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 27 Apr 2023 19:24:00 GMT
CMD ["traefik"]
# Thu, 27 Apr 2023 19:24:00 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:f56be85fc22e46face30e2c3de3f7fe7c15f8fd7c4e5add29d7f64b87abdaa09`  
		Last Modified: Wed, 29 Mar 2023 18:19:57 GMT  
		Size: 3.4 MB (3374563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d055169f9c6f7e08b88a6ef90eba203750fcc51761ecb994e40aa2aaa640ff72`  
		Last Modified: Thu, 30 Mar 2023 02:38:35 GMT  
		Size: 622.2 KB (622239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56d2f042306d84d6b5581bdb96cc47a568cd2c8f18c778d4bdd4289f10ad8955`  
		Last Modified: Thu, 27 Apr 2023 19:24:26 GMT  
		Size: 37.0 MB (36993226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06c7eaf9711b1292ae5a5c1d70177cba7f0aeba30e0d974832bc5729ae07708a`  
		Last Modified: Thu, 27 Apr 2023 19:24:20 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:latest` - linux; arm variant v6

```console
$ docker pull traefik@sha256:f67d07c8c40f742e8fd5b071bf8804690f631b28e9ccef7ecb9b0b6e8e3fc76c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.6 MB (38551154 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d02830f09811f97f72174cd791d4a3781bbafe3452c20d6fcd5ed0bc09fdcfd`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 14 Jun 2023 18:49:25 GMT
ADD file:07e668ef139dce7f076143a30b89ff57885c8539d8b5764ac1bd5277d9936702 in / 
# Wed, 14 Jun 2023 18:49:25 GMT
CMD ["/bin/sh"]
# Wed, 14 Jun 2023 20:12:29 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 14 Jun 2023 20:12:34 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.1/traefik_v2.10.1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 14 Jun 2023 20:12:34 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 14 Jun 2023 20:12:34 GMT
EXPOSE 80
# Wed, 14 Jun 2023 20:12:34 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 14 Jun 2023 20:12:35 GMT
CMD ["traefik"]
# Wed, 14 Jun 2023 20:12:35 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:33ec62e98ceea71d24212ee03e239c2d5538dbe7c98f41c42e8b2693fedf58fb`  
		Last Modified: Wed, 14 Jun 2023 18:50:00 GMT  
		Size: 3.1 MB (3110916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3456aa2bab6b1577d1ef938c6047142d2661cfa237d7988bc621c795148c4f9`  
		Last Modified: Wed, 14 Jun 2023 20:13:06 GMT  
		Size: 624.6 KB (624561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e1f88f7ccafe6c44c30bccec04fdf7523c60284c5bfc2184f657e61bea7b410`  
		Last Modified: Wed, 14 Jun 2023 20:13:12 GMT  
		Size: 34.8 MB (34815309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ae5708ba9c2b61ea7f0086f0ef7438f9a4db8e6abbedf44bd6898d2e9ed465b`  
		Last Modified: Wed, 14 Jun 2023 20:13:06 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:latest` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:38ad4f0cffc281d86fd8512f384d194e24d0e47788c96d2402f243c62d655fb1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.7 MB (37747171 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:28c2c5ecdf8f6666c38b75756b057e2f96002102211ee1d2b5df7615bcf2c106`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:18 GMT
ADD file:e51d4089e73ad6dee52b31f0c8059a00c17df6e23f6741fe11b43bd84cc99008 in / 
# Wed, 29 Mar 2023 17:39:18 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 03:26:37 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 27 Apr 2023 18:50:16 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.1/traefik_v2.10.1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 27 Apr 2023 18:50:16 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 27 Apr 2023 18:50:16 GMT
EXPOSE 80
# Thu, 27 Apr 2023 18:50:16 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 27 Apr 2023 18:50:16 GMT
CMD ["traefik"]
# Thu, 27 Apr 2023 18:50:16 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:c41833b44d910632b415cd89a9cdaa4d62c9725dc56c99a7ddadafd6719960f9`  
		Last Modified: Wed, 29 Mar 2023 17:39:44 GMT  
		Size: 3.3 MB (3261854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4336eee5b1b811f9668d2251fb67e6099c4089ef7b26ade14aacd2f5f0982e06`  
		Last Modified: Thu, 30 Mar 2023 03:27:34 GMT  
		Size: 624.2 KB (624204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb3006acbb0f5f363c1104c94bf762bb2252f9b7f29d8c5b2f74412630c4af33`  
		Last Modified: Thu, 27 Apr 2023 18:50:38 GMT  
		Size: 33.9 MB (33860745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6ecd274862a81d7d04859e42c5c35cd1f4851afcd0aaa61e481abe26bbfb6ca`  
		Last Modified: Thu, 27 Apr 2023 18:50:34 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:latest` - linux; s390x

```console
$ docker pull traefik@sha256:5fed19f3ecb9f6c2438c022696eb56228cfadaccee43a52b0a2bdb4d701925cd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.7 MB (39660993 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7634a95de667e3145cb226864ab946f751a613a045b069611e2db5e078083589`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 29 Mar 2023 17:41:57 GMT
ADD file:675ad8acf4b076e34aeeba26dd482be7640df5912b1ec5e3183b7eb69c01e83e in / 
# Wed, 29 Mar 2023 17:41:57 GMT
CMD ["/bin/sh"]
# Tue, 09 May 2023 23:57:51 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 09 May 2023 23:57:55 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.1/traefik_v2.10.1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Tue, 09 May 2023 23:57:57 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 09 May 2023 23:57:57 GMT
EXPOSE 80
# Tue, 09 May 2023 23:57:57 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 09 May 2023 23:57:57 GMT
CMD ["traefik"]
# Tue, 09 May 2023 23:57:57 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:a76f78d8854217635d8049ec8501edb806f961e72989cfff8503982e6ff2579d`  
		Last Modified: Wed, 29 Mar 2023 17:42:31 GMT  
		Size: 3.2 MB (3175187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aa8506383024e4e72ae2aa2e28d39f346912e8002e883f12c16c3e78b076687`  
		Last Modified: Tue, 09 May 2023 23:58:26 GMT  
		Size: 622.8 KB (622785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71f308ec932ffa02b0679ce4a37a19c241bbf0edffeb07c562c81096e2da38ca`  
		Last Modified: Tue, 09 May 2023 23:58:32 GMT  
		Size: 35.9 MB (35862652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58531206b398f1e9bcb368c1a724cc336a6100fc764fb28153ba3f97f79c78a8`  
		Last Modified: Tue, 09 May 2023 23:58:26 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:saintmarcelin`

```console
$ docker pull traefik@sha256:aae49c77988f065f91948477368475be36d74f46e7eb7b25ab1a8444266d2b0e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:saintmarcelin` - linux; amd64

```console
$ docker pull traefik@sha256:e01d05a30cfed0f79a9ecfb4942662c654ff2d8a39a80f030d4d58d9eb9ec0d1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.0 MB (40990396 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:63d7224eb30e1c2f2976e0043c6cb6f4f7f9bebb820253dc65998bbd747fcc85`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:24 GMT
ADD file:9a4f77dfaba7fd2aa78186e4ef0e7486ad55101cefc1fabbc1b385601bb38920 in / 
# Wed, 29 Mar 2023 18:19:24 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 02:37:38 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 27 Apr 2023 19:23:59 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.1/traefik_v2.10.1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 27 Apr 2023 19:24:00 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 27 Apr 2023 19:24:00 GMT
EXPOSE 80
# Thu, 27 Apr 2023 19:24:00 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 27 Apr 2023 19:24:00 GMT
CMD ["traefik"]
# Thu, 27 Apr 2023 19:24:00 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:f56be85fc22e46face30e2c3de3f7fe7c15f8fd7c4e5add29d7f64b87abdaa09`  
		Last Modified: Wed, 29 Mar 2023 18:19:57 GMT  
		Size: 3.4 MB (3374563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d055169f9c6f7e08b88a6ef90eba203750fcc51761ecb994e40aa2aaa640ff72`  
		Last Modified: Thu, 30 Mar 2023 02:38:35 GMT  
		Size: 622.2 KB (622239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56d2f042306d84d6b5581bdb96cc47a568cd2c8f18c778d4bdd4289f10ad8955`  
		Last Modified: Thu, 27 Apr 2023 19:24:26 GMT  
		Size: 37.0 MB (36993226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06c7eaf9711b1292ae5a5c1d70177cba7f0aeba30e0d974832bc5729ae07708a`  
		Last Modified: Thu, 27 Apr 2023 19:24:20 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:saintmarcelin` - linux; arm variant v6

```console
$ docker pull traefik@sha256:f67d07c8c40f742e8fd5b071bf8804690f631b28e9ccef7ecb9b0b6e8e3fc76c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.6 MB (38551154 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d02830f09811f97f72174cd791d4a3781bbafe3452c20d6fcd5ed0bc09fdcfd`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 14 Jun 2023 18:49:25 GMT
ADD file:07e668ef139dce7f076143a30b89ff57885c8539d8b5764ac1bd5277d9936702 in / 
# Wed, 14 Jun 2023 18:49:25 GMT
CMD ["/bin/sh"]
# Wed, 14 Jun 2023 20:12:29 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 14 Jun 2023 20:12:34 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.1/traefik_v2.10.1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 14 Jun 2023 20:12:34 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 14 Jun 2023 20:12:34 GMT
EXPOSE 80
# Wed, 14 Jun 2023 20:12:34 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 14 Jun 2023 20:12:35 GMT
CMD ["traefik"]
# Wed, 14 Jun 2023 20:12:35 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:33ec62e98ceea71d24212ee03e239c2d5538dbe7c98f41c42e8b2693fedf58fb`  
		Last Modified: Wed, 14 Jun 2023 18:50:00 GMT  
		Size: 3.1 MB (3110916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3456aa2bab6b1577d1ef938c6047142d2661cfa237d7988bc621c795148c4f9`  
		Last Modified: Wed, 14 Jun 2023 20:13:06 GMT  
		Size: 624.6 KB (624561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e1f88f7ccafe6c44c30bccec04fdf7523c60284c5bfc2184f657e61bea7b410`  
		Last Modified: Wed, 14 Jun 2023 20:13:12 GMT  
		Size: 34.8 MB (34815309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ae5708ba9c2b61ea7f0086f0ef7438f9a4db8e6abbedf44bd6898d2e9ed465b`  
		Last Modified: Wed, 14 Jun 2023 20:13:06 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:saintmarcelin` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:38ad4f0cffc281d86fd8512f384d194e24d0e47788c96d2402f243c62d655fb1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.7 MB (37747171 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:28c2c5ecdf8f6666c38b75756b057e2f96002102211ee1d2b5df7615bcf2c106`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:18 GMT
ADD file:e51d4089e73ad6dee52b31f0c8059a00c17df6e23f6741fe11b43bd84cc99008 in / 
# Wed, 29 Mar 2023 17:39:18 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 03:26:37 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 27 Apr 2023 18:50:16 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.1/traefik_v2.10.1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 27 Apr 2023 18:50:16 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 27 Apr 2023 18:50:16 GMT
EXPOSE 80
# Thu, 27 Apr 2023 18:50:16 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 27 Apr 2023 18:50:16 GMT
CMD ["traefik"]
# Thu, 27 Apr 2023 18:50:16 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:c41833b44d910632b415cd89a9cdaa4d62c9725dc56c99a7ddadafd6719960f9`  
		Last Modified: Wed, 29 Mar 2023 17:39:44 GMT  
		Size: 3.3 MB (3261854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4336eee5b1b811f9668d2251fb67e6099c4089ef7b26ade14aacd2f5f0982e06`  
		Last Modified: Thu, 30 Mar 2023 03:27:34 GMT  
		Size: 624.2 KB (624204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb3006acbb0f5f363c1104c94bf762bb2252f9b7f29d8c5b2f74412630c4af33`  
		Last Modified: Thu, 27 Apr 2023 18:50:38 GMT  
		Size: 33.9 MB (33860745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6ecd274862a81d7d04859e42c5c35cd1f4851afcd0aaa61e481abe26bbfb6ca`  
		Last Modified: Thu, 27 Apr 2023 18:50:34 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:saintmarcelin` - linux; s390x

```console
$ docker pull traefik@sha256:5fed19f3ecb9f6c2438c022696eb56228cfadaccee43a52b0a2bdb4d701925cd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.7 MB (39660993 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7634a95de667e3145cb226864ab946f751a613a045b069611e2db5e078083589`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 29 Mar 2023 17:41:57 GMT
ADD file:675ad8acf4b076e34aeeba26dd482be7640df5912b1ec5e3183b7eb69c01e83e in / 
# Wed, 29 Mar 2023 17:41:57 GMT
CMD ["/bin/sh"]
# Tue, 09 May 2023 23:57:51 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 09 May 2023 23:57:55 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.1/traefik_v2.10.1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Tue, 09 May 2023 23:57:57 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 09 May 2023 23:57:57 GMT
EXPOSE 80
# Tue, 09 May 2023 23:57:57 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 09 May 2023 23:57:57 GMT
CMD ["traefik"]
# Tue, 09 May 2023 23:57:57 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:a76f78d8854217635d8049ec8501edb806f961e72989cfff8503982e6ff2579d`  
		Last Modified: Wed, 29 Mar 2023 17:42:31 GMT  
		Size: 3.2 MB (3175187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aa8506383024e4e72ae2aa2e28d39f346912e8002e883f12c16c3e78b076687`  
		Last Modified: Tue, 09 May 2023 23:58:26 GMT  
		Size: 622.8 KB (622785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71f308ec932ffa02b0679ce4a37a19c241bbf0edffeb07c562c81096e2da38ca`  
		Last Modified: Tue, 09 May 2023 23:58:32 GMT  
		Size: 35.9 MB (35862652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58531206b398f1e9bcb368c1a724cc336a6100fc764fb28153ba3f97f79c78a8`  
		Last Modified: Tue, 09 May 2023 23:58:26 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:saintmarcelin-windowsservercore-1809`

```console
$ docker pull traefik@sha256:f16636d4d18fea046d66cb57fa0e90feaeb8ecbf1ca8f4182848481259f07eed
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4377; amd64

### `traefik:saintmarcelin-windowsservercore-1809` - windows version 10.0.17763.4377; amd64

```console
$ docker pull traefik@sha256:c888963af81054ac8c158404fbacff203fc05de699fd77ef99fdb276b0e742e0
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2109597280 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4493990f99f036c842802ae6b9593cf761ac18dbc67fd5cd1a322a84c2697c5e`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Fri, 05 May 2023 12:05:28 GMT
RUN Install update 10.0.17763.4377
# Wed, 10 May 2023 00:36:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 May 2023 06:31:45 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.10.1/traefik_v2.10.1_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Wed, 10 May 2023 06:31:46 GMT
EXPOSE 80
# Wed, 10 May 2023 06:31:47 GMT
ENTRYPOINT ["/traefik"]
# Wed, 10 May 2023 06:31:48 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e01de39a0c44e24aa1912078d32ee54389b71154e509138cc4f5d1de42e7a32a`  
		Last Modified: Wed, 10 May 2023 01:47:41 GMT  
		Size: 364.1 MB (364091294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15a238e462da347b2e29386c9883c0ec93c8dbce311782ea1c5abbec2a31d884`  
		Last Modified: Wed, 10 May 2023 01:46:46 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df6b1b568e48ea9b9c1126801eb055cc1d9aa1e21270219140c58f2e1253a636`  
		Last Modified: Wed, 10 May 2023 07:14:51 GMT  
		Size: 37.6 MB (37556455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f754667a3def555298e795f9f84b666f44e7d683178bc69b2765cc10fa741ec1`  
		Last Modified: Wed, 10 May 2023 07:14:44 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:269055700abc29f93e7940722c0a8c7c9423dd04dd3dcbf84caac07612d4b1cc`  
		Last Modified: Wed, 10 May 2023 07:14:44 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdc6c3594a8fea61840c387597d673ca691a7633347d397c73b3b0b849a173d1`  
		Last Modified: Wed, 10 May 2023 07:14:44 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.10`

```console
$ docker pull traefik@sha256:aae49c77988f065f91948477368475be36d74f46e7eb7b25ab1a8444266d2b0e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:v2.10` - linux; amd64

```console
$ docker pull traefik@sha256:e01d05a30cfed0f79a9ecfb4942662c654ff2d8a39a80f030d4d58d9eb9ec0d1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.0 MB (40990396 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:63d7224eb30e1c2f2976e0043c6cb6f4f7f9bebb820253dc65998bbd747fcc85`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:24 GMT
ADD file:9a4f77dfaba7fd2aa78186e4ef0e7486ad55101cefc1fabbc1b385601bb38920 in / 
# Wed, 29 Mar 2023 18:19:24 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 02:37:38 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 27 Apr 2023 19:23:59 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.1/traefik_v2.10.1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 27 Apr 2023 19:24:00 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 27 Apr 2023 19:24:00 GMT
EXPOSE 80
# Thu, 27 Apr 2023 19:24:00 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 27 Apr 2023 19:24:00 GMT
CMD ["traefik"]
# Thu, 27 Apr 2023 19:24:00 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:f56be85fc22e46face30e2c3de3f7fe7c15f8fd7c4e5add29d7f64b87abdaa09`  
		Last Modified: Wed, 29 Mar 2023 18:19:57 GMT  
		Size: 3.4 MB (3374563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d055169f9c6f7e08b88a6ef90eba203750fcc51761ecb994e40aa2aaa640ff72`  
		Last Modified: Thu, 30 Mar 2023 02:38:35 GMT  
		Size: 622.2 KB (622239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56d2f042306d84d6b5581bdb96cc47a568cd2c8f18c778d4bdd4289f10ad8955`  
		Last Modified: Thu, 27 Apr 2023 19:24:26 GMT  
		Size: 37.0 MB (36993226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06c7eaf9711b1292ae5a5c1d70177cba7f0aeba30e0d974832bc5729ae07708a`  
		Last Modified: Thu, 27 Apr 2023 19:24:20 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.10` - linux; arm variant v6

```console
$ docker pull traefik@sha256:f67d07c8c40f742e8fd5b071bf8804690f631b28e9ccef7ecb9b0b6e8e3fc76c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.6 MB (38551154 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d02830f09811f97f72174cd791d4a3781bbafe3452c20d6fcd5ed0bc09fdcfd`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 14 Jun 2023 18:49:25 GMT
ADD file:07e668ef139dce7f076143a30b89ff57885c8539d8b5764ac1bd5277d9936702 in / 
# Wed, 14 Jun 2023 18:49:25 GMT
CMD ["/bin/sh"]
# Wed, 14 Jun 2023 20:12:29 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 14 Jun 2023 20:12:34 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.1/traefik_v2.10.1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 14 Jun 2023 20:12:34 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 14 Jun 2023 20:12:34 GMT
EXPOSE 80
# Wed, 14 Jun 2023 20:12:34 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 14 Jun 2023 20:12:35 GMT
CMD ["traefik"]
# Wed, 14 Jun 2023 20:12:35 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:33ec62e98ceea71d24212ee03e239c2d5538dbe7c98f41c42e8b2693fedf58fb`  
		Last Modified: Wed, 14 Jun 2023 18:50:00 GMT  
		Size: 3.1 MB (3110916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3456aa2bab6b1577d1ef938c6047142d2661cfa237d7988bc621c795148c4f9`  
		Last Modified: Wed, 14 Jun 2023 20:13:06 GMT  
		Size: 624.6 KB (624561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e1f88f7ccafe6c44c30bccec04fdf7523c60284c5bfc2184f657e61bea7b410`  
		Last Modified: Wed, 14 Jun 2023 20:13:12 GMT  
		Size: 34.8 MB (34815309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ae5708ba9c2b61ea7f0086f0ef7438f9a4db8e6abbedf44bd6898d2e9ed465b`  
		Last Modified: Wed, 14 Jun 2023 20:13:06 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.10` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:38ad4f0cffc281d86fd8512f384d194e24d0e47788c96d2402f243c62d655fb1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.7 MB (37747171 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:28c2c5ecdf8f6666c38b75756b057e2f96002102211ee1d2b5df7615bcf2c106`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:18 GMT
ADD file:e51d4089e73ad6dee52b31f0c8059a00c17df6e23f6741fe11b43bd84cc99008 in / 
# Wed, 29 Mar 2023 17:39:18 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 03:26:37 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 27 Apr 2023 18:50:16 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.1/traefik_v2.10.1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 27 Apr 2023 18:50:16 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 27 Apr 2023 18:50:16 GMT
EXPOSE 80
# Thu, 27 Apr 2023 18:50:16 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 27 Apr 2023 18:50:16 GMT
CMD ["traefik"]
# Thu, 27 Apr 2023 18:50:16 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:c41833b44d910632b415cd89a9cdaa4d62c9725dc56c99a7ddadafd6719960f9`  
		Last Modified: Wed, 29 Mar 2023 17:39:44 GMT  
		Size: 3.3 MB (3261854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4336eee5b1b811f9668d2251fb67e6099c4089ef7b26ade14aacd2f5f0982e06`  
		Last Modified: Thu, 30 Mar 2023 03:27:34 GMT  
		Size: 624.2 KB (624204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb3006acbb0f5f363c1104c94bf762bb2252f9b7f29d8c5b2f74412630c4af33`  
		Last Modified: Thu, 27 Apr 2023 18:50:38 GMT  
		Size: 33.9 MB (33860745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6ecd274862a81d7d04859e42c5c35cd1f4851afcd0aaa61e481abe26bbfb6ca`  
		Last Modified: Thu, 27 Apr 2023 18:50:34 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.10` - linux; s390x

```console
$ docker pull traefik@sha256:5fed19f3ecb9f6c2438c022696eb56228cfadaccee43a52b0a2bdb4d701925cd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.7 MB (39660993 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7634a95de667e3145cb226864ab946f751a613a045b069611e2db5e078083589`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 29 Mar 2023 17:41:57 GMT
ADD file:675ad8acf4b076e34aeeba26dd482be7640df5912b1ec5e3183b7eb69c01e83e in / 
# Wed, 29 Mar 2023 17:41:57 GMT
CMD ["/bin/sh"]
# Tue, 09 May 2023 23:57:51 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 09 May 2023 23:57:55 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.1/traefik_v2.10.1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Tue, 09 May 2023 23:57:57 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 09 May 2023 23:57:57 GMT
EXPOSE 80
# Tue, 09 May 2023 23:57:57 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 09 May 2023 23:57:57 GMT
CMD ["traefik"]
# Tue, 09 May 2023 23:57:57 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:a76f78d8854217635d8049ec8501edb806f961e72989cfff8503982e6ff2579d`  
		Last Modified: Wed, 29 Mar 2023 17:42:31 GMT  
		Size: 3.2 MB (3175187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aa8506383024e4e72ae2aa2e28d39f346912e8002e883f12c16c3e78b076687`  
		Last Modified: Tue, 09 May 2023 23:58:26 GMT  
		Size: 622.8 KB (622785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71f308ec932ffa02b0679ce4a37a19c241bbf0edffeb07c562c81096e2da38ca`  
		Last Modified: Tue, 09 May 2023 23:58:32 GMT  
		Size: 35.9 MB (35862652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58531206b398f1e9bcb368c1a724cc336a6100fc764fb28153ba3f97f79c78a8`  
		Last Modified: Tue, 09 May 2023 23:58:26 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.10-windowsservercore-1809`

```console
$ docker pull traefik@sha256:f16636d4d18fea046d66cb57fa0e90feaeb8ecbf1ca8f4182848481259f07eed
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4377; amd64

### `traefik:v2.10-windowsservercore-1809` - windows version 10.0.17763.4377; amd64

```console
$ docker pull traefik@sha256:c888963af81054ac8c158404fbacff203fc05de699fd77ef99fdb276b0e742e0
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2109597280 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4493990f99f036c842802ae6b9593cf761ac18dbc67fd5cd1a322a84c2697c5e`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Fri, 05 May 2023 12:05:28 GMT
RUN Install update 10.0.17763.4377
# Wed, 10 May 2023 00:36:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 May 2023 06:31:45 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.10.1/traefik_v2.10.1_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Wed, 10 May 2023 06:31:46 GMT
EXPOSE 80
# Wed, 10 May 2023 06:31:47 GMT
ENTRYPOINT ["/traefik"]
# Wed, 10 May 2023 06:31:48 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e01de39a0c44e24aa1912078d32ee54389b71154e509138cc4f5d1de42e7a32a`  
		Last Modified: Wed, 10 May 2023 01:47:41 GMT  
		Size: 364.1 MB (364091294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15a238e462da347b2e29386c9883c0ec93c8dbce311782ea1c5abbec2a31d884`  
		Last Modified: Wed, 10 May 2023 01:46:46 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df6b1b568e48ea9b9c1126801eb055cc1d9aa1e21270219140c58f2e1253a636`  
		Last Modified: Wed, 10 May 2023 07:14:51 GMT  
		Size: 37.6 MB (37556455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f754667a3def555298e795f9f84b666f44e7d683178bc69b2765cc10fa741ec1`  
		Last Modified: Wed, 10 May 2023 07:14:44 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:269055700abc29f93e7940722c0a8c7c9423dd04dd3dcbf84caac07612d4b1cc`  
		Last Modified: Wed, 10 May 2023 07:14:44 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdc6c3594a8fea61840c387597d673ca691a7633347d397c73b3b0b849a173d1`  
		Last Modified: Wed, 10 May 2023 07:14:44 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.10.1`

```console
$ docker pull traefik@sha256:aae49c77988f065f91948477368475be36d74f46e7eb7b25ab1a8444266d2b0e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:v2.10.1` - linux; amd64

```console
$ docker pull traefik@sha256:e01d05a30cfed0f79a9ecfb4942662c654ff2d8a39a80f030d4d58d9eb9ec0d1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.0 MB (40990396 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:63d7224eb30e1c2f2976e0043c6cb6f4f7f9bebb820253dc65998bbd747fcc85`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:24 GMT
ADD file:9a4f77dfaba7fd2aa78186e4ef0e7486ad55101cefc1fabbc1b385601bb38920 in / 
# Wed, 29 Mar 2023 18:19:24 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 02:37:38 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 27 Apr 2023 19:23:59 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.1/traefik_v2.10.1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 27 Apr 2023 19:24:00 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 27 Apr 2023 19:24:00 GMT
EXPOSE 80
# Thu, 27 Apr 2023 19:24:00 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 27 Apr 2023 19:24:00 GMT
CMD ["traefik"]
# Thu, 27 Apr 2023 19:24:00 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:f56be85fc22e46face30e2c3de3f7fe7c15f8fd7c4e5add29d7f64b87abdaa09`  
		Last Modified: Wed, 29 Mar 2023 18:19:57 GMT  
		Size: 3.4 MB (3374563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d055169f9c6f7e08b88a6ef90eba203750fcc51761ecb994e40aa2aaa640ff72`  
		Last Modified: Thu, 30 Mar 2023 02:38:35 GMT  
		Size: 622.2 KB (622239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56d2f042306d84d6b5581bdb96cc47a568cd2c8f18c778d4bdd4289f10ad8955`  
		Last Modified: Thu, 27 Apr 2023 19:24:26 GMT  
		Size: 37.0 MB (36993226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06c7eaf9711b1292ae5a5c1d70177cba7f0aeba30e0d974832bc5729ae07708a`  
		Last Modified: Thu, 27 Apr 2023 19:24:20 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.10.1` - linux; arm variant v6

```console
$ docker pull traefik@sha256:f67d07c8c40f742e8fd5b071bf8804690f631b28e9ccef7ecb9b0b6e8e3fc76c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.6 MB (38551154 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d02830f09811f97f72174cd791d4a3781bbafe3452c20d6fcd5ed0bc09fdcfd`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 14 Jun 2023 18:49:25 GMT
ADD file:07e668ef139dce7f076143a30b89ff57885c8539d8b5764ac1bd5277d9936702 in / 
# Wed, 14 Jun 2023 18:49:25 GMT
CMD ["/bin/sh"]
# Wed, 14 Jun 2023 20:12:29 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 14 Jun 2023 20:12:34 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.1/traefik_v2.10.1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 14 Jun 2023 20:12:34 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 14 Jun 2023 20:12:34 GMT
EXPOSE 80
# Wed, 14 Jun 2023 20:12:34 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 14 Jun 2023 20:12:35 GMT
CMD ["traefik"]
# Wed, 14 Jun 2023 20:12:35 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:33ec62e98ceea71d24212ee03e239c2d5538dbe7c98f41c42e8b2693fedf58fb`  
		Last Modified: Wed, 14 Jun 2023 18:50:00 GMT  
		Size: 3.1 MB (3110916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3456aa2bab6b1577d1ef938c6047142d2661cfa237d7988bc621c795148c4f9`  
		Last Modified: Wed, 14 Jun 2023 20:13:06 GMT  
		Size: 624.6 KB (624561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e1f88f7ccafe6c44c30bccec04fdf7523c60284c5bfc2184f657e61bea7b410`  
		Last Modified: Wed, 14 Jun 2023 20:13:12 GMT  
		Size: 34.8 MB (34815309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ae5708ba9c2b61ea7f0086f0ef7438f9a4db8e6abbedf44bd6898d2e9ed465b`  
		Last Modified: Wed, 14 Jun 2023 20:13:06 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.10.1` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:38ad4f0cffc281d86fd8512f384d194e24d0e47788c96d2402f243c62d655fb1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.7 MB (37747171 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:28c2c5ecdf8f6666c38b75756b057e2f96002102211ee1d2b5df7615bcf2c106`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:18 GMT
ADD file:e51d4089e73ad6dee52b31f0c8059a00c17df6e23f6741fe11b43bd84cc99008 in / 
# Wed, 29 Mar 2023 17:39:18 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 03:26:37 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 27 Apr 2023 18:50:16 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.1/traefik_v2.10.1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 27 Apr 2023 18:50:16 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 27 Apr 2023 18:50:16 GMT
EXPOSE 80
# Thu, 27 Apr 2023 18:50:16 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 27 Apr 2023 18:50:16 GMT
CMD ["traefik"]
# Thu, 27 Apr 2023 18:50:16 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:c41833b44d910632b415cd89a9cdaa4d62c9725dc56c99a7ddadafd6719960f9`  
		Last Modified: Wed, 29 Mar 2023 17:39:44 GMT  
		Size: 3.3 MB (3261854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4336eee5b1b811f9668d2251fb67e6099c4089ef7b26ade14aacd2f5f0982e06`  
		Last Modified: Thu, 30 Mar 2023 03:27:34 GMT  
		Size: 624.2 KB (624204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb3006acbb0f5f363c1104c94bf762bb2252f9b7f29d8c5b2f74412630c4af33`  
		Last Modified: Thu, 27 Apr 2023 18:50:38 GMT  
		Size: 33.9 MB (33860745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6ecd274862a81d7d04859e42c5c35cd1f4851afcd0aaa61e481abe26bbfb6ca`  
		Last Modified: Thu, 27 Apr 2023 18:50:34 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.10.1` - linux; s390x

```console
$ docker pull traefik@sha256:5fed19f3ecb9f6c2438c022696eb56228cfadaccee43a52b0a2bdb4d701925cd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.7 MB (39660993 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7634a95de667e3145cb226864ab946f751a613a045b069611e2db5e078083589`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 29 Mar 2023 17:41:57 GMT
ADD file:675ad8acf4b076e34aeeba26dd482be7640df5912b1ec5e3183b7eb69c01e83e in / 
# Wed, 29 Mar 2023 17:41:57 GMT
CMD ["/bin/sh"]
# Tue, 09 May 2023 23:57:51 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 09 May 2023 23:57:55 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.1/traefik_v2.10.1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Tue, 09 May 2023 23:57:57 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 09 May 2023 23:57:57 GMT
EXPOSE 80
# Tue, 09 May 2023 23:57:57 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 09 May 2023 23:57:57 GMT
CMD ["traefik"]
# Tue, 09 May 2023 23:57:57 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:a76f78d8854217635d8049ec8501edb806f961e72989cfff8503982e6ff2579d`  
		Last Modified: Wed, 29 Mar 2023 17:42:31 GMT  
		Size: 3.2 MB (3175187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aa8506383024e4e72ae2aa2e28d39f346912e8002e883f12c16c3e78b076687`  
		Last Modified: Tue, 09 May 2023 23:58:26 GMT  
		Size: 622.8 KB (622785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71f308ec932ffa02b0679ce4a37a19c241bbf0edffeb07c562c81096e2da38ca`  
		Last Modified: Tue, 09 May 2023 23:58:32 GMT  
		Size: 35.9 MB (35862652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58531206b398f1e9bcb368c1a724cc336a6100fc764fb28153ba3f97f79c78a8`  
		Last Modified: Tue, 09 May 2023 23:58:26 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.10.1-windowsservercore-1809`

```console
$ docker pull traefik@sha256:f16636d4d18fea046d66cb57fa0e90feaeb8ecbf1ca8f4182848481259f07eed
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4377; amd64

### `traefik:v2.10.1-windowsservercore-1809` - windows version 10.0.17763.4377; amd64

```console
$ docker pull traefik@sha256:c888963af81054ac8c158404fbacff203fc05de699fd77ef99fdb276b0e742e0
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2109597280 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4493990f99f036c842802ae6b9593cf761ac18dbc67fd5cd1a322a84c2697c5e`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Fri, 05 May 2023 12:05:28 GMT
RUN Install update 10.0.17763.4377
# Wed, 10 May 2023 00:36:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 May 2023 06:31:45 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.10.1/traefik_v2.10.1_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Wed, 10 May 2023 06:31:46 GMT
EXPOSE 80
# Wed, 10 May 2023 06:31:47 GMT
ENTRYPOINT ["/traefik"]
# Wed, 10 May 2023 06:31:48 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e01de39a0c44e24aa1912078d32ee54389b71154e509138cc4f5d1de42e7a32a`  
		Last Modified: Wed, 10 May 2023 01:47:41 GMT  
		Size: 364.1 MB (364091294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15a238e462da347b2e29386c9883c0ec93c8dbce311782ea1c5abbec2a31d884`  
		Last Modified: Wed, 10 May 2023 01:46:46 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df6b1b568e48ea9b9c1126801eb055cc1d9aa1e21270219140c58f2e1253a636`  
		Last Modified: Wed, 10 May 2023 07:14:51 GMT  
		Size: 37.6 MB (37556455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f754667a3def555298e795f9f84b666f44e7d683178bc69b2765cc10fa741ec1`  
		Last Modified: Wed, 10 May 2023 07:14:44 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:269055700abc29f93e7940722c0a8c7c9423dd04dd3dcbf84caac07612d4b1cc`  
		Last Modified: Wed, 10 May 2023 07:14:44 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdc6c3594a8fea61840c387597d673ca691a7633347d397c73b3b0b849a173d1`  
		Last Modified: Wed, 10 May 2023 07:14:44 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v3.0`

```console
$ docker pull traefik@sha256:83e7b36fbe4096887d144ba82c51b891893ad3eb5f891daf300f5cf49b9d61d3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:v3.0` - linux; amd64

```console
$ docker pull traefik@sha256:a239deca1c7682fe9bb6a32e54364c7ff460205fa0e87c02bfeb66efb3f3a3d1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.6 MB (40562953 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:42fc5a7c2d34a752fce6439cf3dc08ac747649d7712bc265c7dd7d1b38a2a45b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:33 GMT
ADD file:08ad6c1c886a26e30ae4ab103ff377ee6cfbc1be2437fa227ec28a335c63d78a in / 
# Wed, 29 Mar 2023 18:19:33 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 02:37:32 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 30 Mar 2023 02:37:35 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta2/traefik_v3.0.0-beta2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 30 Mar 2023 02:37:35 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 30 Mar 2023 02:37:35 GMT
EXPOSE 80
# Thu, 30 Mar 2023 02:37:35 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 30 Mar 2023 02:37:35 GMT
CMD ["traefik"]
# Thu, 30 Mar 2023 02:37:36 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:0ce1dd7918a48990ab749aab2e805c26f691a3a8103495530e7ea5a1d168af4a`  
		Last Modified: Wed, 29 Mar 2023 18:20:17 GMT  
		Size: 2.8 MB (2826596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c11624eb8d0cca298aa32848e39318bbc75ab1c404423d1d47c670fa60354e3`  
		Last Modified: Thu, 30 Mar 2023 02:38:16 GMT  
		Size: 661.1 KB (661099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a9d40a9765a3ede8e4ec67030b20d484fedcea2ad98ee2b231ec3d86e6fd1b6`  
		Last Modified: Thu, 30 Mar 2023 02:38:21 GMT  
		Size: 37.1 MB (37074890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fca61e22e5a1dbbdeea08d3e394601c2c5492fc65d19af813ef66cc36a7d582`  
		Last Modified: Thu, 30 Mar 2023 02:38:15 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v3.0` - linux; arm variant v6

```console
$ docker pull traefik@sha256:0e010dd7b60c3960f903b07854cae707e691496f1491f0447ca2635b5a374a6d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.3 MB (38289085 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ee0012c6d54cfd4da66d0da5e01f3dc4f70609eec928ce429e71a5efa02c96b3`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 14 Jun 2023 18:49:32 GMT
ADD file:b987db82fa4ce6e623de49a50612c1fd91c5ab2209a62a5727ab3436c2923e91 in / 
# Wed, 14 Jun 2023 18:49:32 GMT
CMD ["/bin/sh"]
# Wed, 14 Jun 2023 20:12:22 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 14 Jun 2023 20:12:26 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta2/traefik_v3.0.0-beta2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 14 Jun 2023 20:12:26 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 14 Jun 2023 20:12:26 GMT
EXPOSE 80
# Wed, 14 Jun 2023 20:12:26 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 14 Jun 2023 20:12:26 GMT
CMD ["traefik"]
# Wed, 14 Jun 2023 20:12:26 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:41c5c5b38e13af18def277385607129664fb24993d262d4b601a381e776482a9`  
		Last Modified: Wed, 14 Jun 2023 18:50:19 GMT  
		Size: 2.6 MB (2633060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:718cfe2cb66c053a8fdb09adf88b20a52f260f22abd38cba68cc2838ee33e73d`  
		Last Modified: Wed, 14 Jun 2023 20:12:46 GMT  
		Size: 666.3 KB (666349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47b2cef5f2c79471c563b3c10376140084b51c097de00e9be0b758219ab95e5c`  
		Last Modified: Wed, 14 Jun 2023 20:12:52 GMT  
		Size: 35.0 MB (34989308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66078e59ed6730404193e57cea654480d0731663c7a068349344e0a681d1c660`  
		Last Modified: Wed, 14 Jun 2023 20:12:46 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v3.0` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:529410986a68c6e7989a5a08afa53d087795a2f1406977d5d6b183bfdfab65dd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.4 MB (37408212 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e4bfdbd12bed1c2e46296bb16021a1eea4269055e03fdf9e30c035e5f9e8dc4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:22 GMT
ADD file:4acfda16c71abce07068ed23839e9de60c1d1145ab8002b3a92c15b1e80d4356 in / 
# Wed, 29 Mar 2023 17:39:23 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 03:26:31 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 30 Mar 2023 03:26:34 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta2/traefik_v3.0.0-beta2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 30 Mar 2023 03:26:35 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 30 Mar 2023 03:26:35 GMT
EXPOSE 80
# Thu, 30 Mar 2023 03:26:35 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 30 Mar 2023 03:26:35 GMT
CMD ["traefik"]
# Thu, 30 Mar 2023 03:26:35 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:60a00c11adf5202a365ec8215b889c3390d67fa295ab79940e1c5dc4cbed9db1`  
		Last Modified: Wed, 29 Mar 2023 17:40:04 GMT  
		Size: 2.7 MB (2722002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d019fab0470c352dfa2ff6c01be8f1d0344d43e9431a28656e78c5cabd03e67f`  
		Last Modified: Thu, 30 Mar 2023 03:27:17 GMT  
		Size: 662.3 KB (662323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d82ed46bb3966bf021d56f3bfda66ada1ddde7199ee9d3446ebcbeffec692004`  
		Last Modified: Thu, 30 Mar 2023 03:27:20 GMT  
		Size: 34.0 MB (34023520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07a93ddfbde23c1aa20ccac6b7cd3dcbda52d11c2b1627d41dc7fa169bd46430`  
		Last Modified: Thu, 30 Mar 2023 03:27:16 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v3.0` - linux; s390x

```console
$ docker pull traefik@sha256:bbf1710b9a47f8ec5a04c849b5eabca1601d8c3d14771376db863d4bfb11267c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.1 MB (39132224 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a7797b8a6b1786adb45fd822e034429307f0e6d9835934dff30e1685c3d7253`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 29 Mar 2023 17:42:07 GMT
ADD file:5cf392863cd9a0735de88f9e7dab93c9e74aca59ca05b792943cf3b621ea2c59 in / 
# Wed, 29 Mar 2023 17:42:07 GMT
CMD ["/bin/sh"]
# Tue, 09 May 2023 23:57:38 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 09 May 2023 23:57:42 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta2/traefik_v3.0.0-beta2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Tue, 09 May 2023 23:57:44 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 09 May 2023 23:57:44 GMT
EXPOSE 80
# Tue, 09 May 2023 23:57:44 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 09 May 2023 23:57:44 GMT
CMD ["traefik"]
# Tue, 09 May 2023 23:57:44 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:1536575ac9c5f5fff4522c60d4610af0a52be584c36e652080c6c0ad169d4f27`  
		Last Modified: Wed, 29 Mar 2023 17:42:42 GMT  
		Size: 2.6 MB (2610636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa7a4deefee64d3e0ac000d06c44544635381ead6c9ce624aad695fd76bdde33`  
		Last Modified: Tue, 09 May 2023 23:58:12 GMT  
		Size: 665.8 KB (665799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a2ced6eac60c1c9707c57590d27e69315354f9d304ec2af3e7f07d5a2bec0b4`  
		Last Modified: Tue, 09 May 2023 23:58:18 GMT  
		Size: 35.9 MB (35855421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b58a1e76f2b69535b5f8ea9cdfda36f79ee2e5fd3194ee2e9ce12fd841672a09`  
		Last Modified: Tue, 09 May 2023 23:58:12 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v3.0-windowsservercore-1809`

```console
$ docker pull traefik@sha256:a029ead52682acc7e61cd89a8807ddebd7d1d5df26f9249c3dd1003991a1c8da
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4377; amd64

### `traefik:v3.0-windowsservercore-1809` - windows version 10.0.17763.4377; amd64

```console
$ docker pull traefik@sha256:78a79fdcd7524d1a0efa1937dd822c5018cae9333ceace3ea65fd9e9f8673847
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2109691146 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e40512720c63bc941384872c5997d1356d112a9a09d42b25f64e228937c02ba7`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Fri, 05 May 2023 12:05:28 GMT
RUN Install update 10.0.17763.4377
# Wed, 10 May 2023 00:36:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 May 2023 06:30:17 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v3.0.0-beta2/traefik_v3.0.0-beta2_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Wed, 10 May 2023 06:30:18 GMT
EXPOSE 80
# Wed, 10 May 2023 06:30:19 GMT
ENTRYPOINT ["/traefik"]
# Wed, 10 May 2023 06:30:20 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e01de39a0c44e24aa1912078d32ee54389b71154e509138cc4f5d1de42e7a32a`  
		Last Modified: Wed, 10 May 2023 01:47:41 GMT  
		Size: 364.1 MB (364091294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15a238e462da347b2e29386c9883c0ec93c8dbce311782ea1c5abbec2a31d884`  
		Last Modified: Wed, 10 May 2023 01:46:46 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f5d58d623c979fa789cd0569f498ae640679c8c40d6aa12ba6f0714a8524a8b`  
		Last Modified: Wed, 10 May 2023 07:14:30 GMT  
		Size: 37.7 MB (37650316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69d5e987e1a63a8e5472dafacad7b03bd1ceebc572fdfdec77bcd778030bfd30`  
		Last Modified: Wed, 10 May 2023 07:14:22 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1e4c1a5897d7faefb9bb9c57c4b06244db88d7039610fc61a720f24e98b8108`  
		Last Modified: Wed, 10 May 2023 07:14:22 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9def7bdf656e22544902494ac6ffb34aef316d5f2d2b5cd77f1d7b9fe5174bed`  
		Last Modified: Wed, 10 May 2023 07:14:22 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v3.0.0-beta2`

```console
$ docker pull traefik@sha256:83e7b36fbe4096887d144ba82c51b891893ad3eb5f891daf300f5cf49b9d61d3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:v3.0.0-beta2` - linux; amd64

```console
$ docker pull traefik@sha256:a239deca1c7682fe9bb6a32e54364c7ff460205fa0e87c02bfeb66efb3f3a3d1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.6 MB (40562953 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:42fc5a7c2d34a752fce6439cf3dc08ac747649d7712bc265c7dd7d1b38a2a45b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:33 GMT
ADD file:08ad6c1c886a26e30ae4ab103ff377ee6cfbc1be2437fa227ec28a335c63d78a in / 
# Wed, 29 Mar 2023 18:19:33 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 02:37:32 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 30 Mar 2023 02:37:35 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta2/traefik_v3.0.0-beta2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 30 Mar 2023 02:37:35 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 30 Mar 2023 02:37:35 GMT
EXPOSE 80
# Thu, 30 Mar 2023 02:37:35 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 30 Mar 2023 02:37:35 GMT
CMD ["traefik"]
# Thu, 30 Mar 2023 02:37:36 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:0ce1dd7918a48990ab749aab2e805c26f691a3a8103495530e7ea5a1d168af4a`  
		Last Modified: Wed, 29 Mar 2023 18:20:17 GMT  
		Size: 2.8 MB (2826596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c11624eb8d0cca298aa32848e39318bbc75ab1c404423d1d47c670fa60354e3`  
		Last Modified: Thu, 30 Mar 2023 02:38:16 GMT  
		Size: 661.1 KB (661099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a9d40a9765a3ede8e4ec67030b20d484fedcea2ad98ee2b231ec3d86e6fd1b6`  
		Last Modified: Thu, 30 Mar 2023 02:38:21 GMT  
		Size: 37.1 MB (37074890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fca61e22e5a1dbbdeea08d3e394601c2c5492fc65d19af813ef66cc36a7d582`  
		Last Modified: Thu, 30 Mar 2023 02:38:15 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v3.0.0-beta2` - linux; arm variant v6

```console
$ docker pull traefik@sha256:0e010dd7b60c3960f903b07854cae707e691496f1491f0447ca2635b5a374a6d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.3 MB (38289085 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ee0012c6d54cfd4da66d0da5e01f3dc4f70609eec928ce429e71a5efa02c96b3`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 14 Jun 2023 18:49:32 GMT
ADD file:b987db82fa4ce6e623de49a50612c1fd91c5ab2209a62a5727ab3436c2923e91 in / 
# Wed, 14 Jun 2023 18:49:32 GMT
CMD ["/bin/sh"]
# Wed, 14 Jun 2023 20:12:22 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 14 Jun 2023 20:12:26 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta2/traefik_v3.0.0-beta2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 14 Jun 2023 20:12:26 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 14 Jun 2023 20:12:26 GMT
EXPOSE 80
# Wed, 14 Jun 2023 20:12:26 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 14 Jun 2023 20:12:26 GMT
CMD ["traefik"]
# Wed, 14 Jun 2023 20:12:26 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:41c5c5b38e13af18def277385607129664fb24993d262d4b601a381e776482a9`  
		Last Modified: Wed, 14 Jun 2023 18:50:19 GMT  
		Size: 2.6 MB (2633060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:718cfe2cb66c053a8fdb09adf88b20a52f260f22abd38cba68cc2838ee33e73d`  
		Last Modified: Wed, 14 Jun 2023 20:12:46 GMT  
		Size: 666.3 KB (666349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47b2cef5f2c79471c563b3c10376140084b51c097de00e9be0b758219ab95e5c`  
		Last Modified: Wed, 14 Jun 2023 20:12:52 GMT  
		Size: 35.0 MB (34989308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66078e59ed6730404193e57cea654480d0731663c7a068349344e0a681d1c660`  
		Last Modified: Wed, 14 Jun 2023 20:12:46 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v3.0.0-beta2` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:529410986a68c6e7989a5a08afa53d087795a2f1406977d5d6b183bfdfab65dd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.4 MB (37408212 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e4bfdbd12bed1c2e46296bb16021a1eea4269055e03fdf9e30c035e5f9e8dc4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:22 GMT
ADD file:4acfda16c71abce07068ed23839e9de60c1d1145ab8002b3a92c15b1e80d4356 in / 
# Wed, 29 Mar 2023 17:39:23 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 03:26:31 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 30 Mar 2023 03:26:34 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta2/traefik_v3.0.0-beta2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 30 Mar 2023 03:26:35 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 30 Mar 2023 03:26:35 GMT
EXPOSE 80
# Thu, 30 Mar 2023 03:26:35 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 30 Mar 2023 03:26:35 GMT
CMD ["traefik"]
# Thu, 30 Mar 2023 03:26:35 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:60a00c11adf5202a365ec8215b889c3390d67fa295ab79940e1c5dc4cbed9db1`  
		Last Modified: Wed, 29 Mar 2023 17:40:04 GMT  
		Size: 2.7 MB (2722002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d019fab0470c352dfa2ff6c01be8f1d0344d43e9431a28656e78c5cabd03e67f`  
		Last Modified: Thu, 30 Mar 2023 03:27:17 GMT  
		Size: 662.3 KB (662323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d82ed46bb3966bf021d56f3bfda66ada1ddde7199ee9d3446ebcbeffec692004`  
		Last Modified: Thu, 30 Mar 2023 03:27:20 GMT  
		Size: 34.0 MB (34023520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07a93ddfbde23c1aa20ccac6b7cd3dcbda52d11c2b1627d41dc7fa169bd46430`  
		Last Modified: Thu, 30 Mar 2023 03:27:16 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v3.0.0-beta2` - linux; s390x

```console
$ docker pull traefik@sha256:bbf1710b9a47f8ec5a04c849b5eabca1601d8c3d14771376db863d4bfb11267c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.1 MB (39132224 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a7797b8a6b1786adb45fd822e034429307f0e6d9835934dff30e1685c3d7253`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 29 Mar 2023 17:42:07 GMT
ADD file:5cf392863cd9a0735de88f9e7dab93c9e74aca59ca05b792943cf3b621ea2c59 in / 
# Wed, 29 Mar 2023 17:42:07 GMT
CMD ["/bin/sh"]
# Tue, 09 May 2023 23:57:38 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 09 May 2023 23:57:42 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta2/traefik_v3.0.0-beta2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Tue, 09 May 2023 23:57:44 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 09 May 2023 23:57:44 GMT
EXPOSE 80
# Tue, 09 May 2023 23:57:44 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 09 May 2023 23:57:44 GMT
CMD ["traefik"]
# Tue, 09 May 2023 23:57:44 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:1536575ac9c5f5fff4522c60d4610af0a52be584c36e652080c6c0ad169d4f27`  
		Last Modified: Wed, 29 Mar 2023 17:42:42 GMT  
		Size: 2.6 MB (2610636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa7a4deefee64d3e0ac000d06c44544635381ead6c9ce624aad695fd76bdde33`  
		Last Modified: Tue, 09 May 2023 23:58:12 GMT  
		Size: 665.8 KB (665799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a2ced6eac60c1c9707c57590d27e69315354f9d304ec2af3e7f07d5a2bec0b4`  
		Last Modified: Tue, 09 May 2023 23:58:18 GMT  
		Size: 35.9 MB (35855421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b58a1e76f2b69535b5f8ea9cdfda36f79ee2e5fd3194ee2e9ce12fd841672a09`  
		Last Modified: Tue, 09 May 2023 23:58:12 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v3.0.0-beta2-windowsservercore-1809`

```console
$ docker pull traefik@sha256:a029ead52682acc7e61cd89a8807ddebd7d1d5df26f9249c3dd1003991a1c8da
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4377; amd64

### `traefik:v3.0.0-beta2-windowsservercore-1809` - windows version 10.0.17763.4377; amd64

```console
$ docker pull traefik@sha256:78a79fdcd7524d1a0efa1937dd822c5018cae9333ceace3ea65fd9e9f8673847
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2109691146 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e40512720c63bc941384872c5997d1356d112a9a09d42b25f64e228937c02ba7`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Fri, 05 May 2023 12:05:28 GMT
RUN Install update 10.0.17763.4377
# Wed, 10 May 2023 00:36:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 May 2023 06:30:17 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v3.0.0-beta2/traefik_v3.0.0-beta2_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Wed, 10 May 2023 06:30:18 GMT
EXPOSE 80
# Wed, 10 May 2023 06:30:19 GMT
ENTRYPOINT ["/traefik"]
# Wed, 10 May 2023 06:30:20 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e01de39a0c44e24aa1912078d32ee54389b71154e509138cc4f5d1de42e7a32a`  
		Last Modified: Wed, 10 May 2023 01:47:41 GMT  
		Size: 364.1 MB (364091294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15a238e462da347b2e29386c9883c0ec93c8dbce311782ea1c5abbec2a31d884`  
		Last Modified: Wed, 10 May 2023 01:46:46 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f5d58d623c979fa789cd0569f498ae640679c8c40d6aa12ba6f0714a8524a8b`  
		Last Modified: Wed, 10 May 2023 07:14:30 GMT  
		Size: 37.7 MB (37650316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69d5e987e1a63a8e5472dafacad7b03bd1ceebc572fdfdec77bcd778030bfd30`  
		Last Modified: Wed, 10 May 2023 07:14:22 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1e4c1a5897d7faefb9bb9c57c4b06244db88d7039610fc61a720f24e98b8108`  
		Last Modified: Wed, 10 May 2023 07:14:22 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9def7bdf656e22544902494ac6ffb34aef316d5f2d2b5cd77f1d7b9fe5174bed`  
		Last Modified: Wed, 10 May 2023 07:14:22 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:windowsservercore-1809`

```console
$ docker pull traefik@sha256:f16636d4d18fea046d66cb57fa0e90feaeb8ecbf1ca8f4182848481259f07eed
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4377; amd64

### `traefik:windowsservercore-1809` - windows version 10.0.17763.4377; amd64

```console
$ docker pull traefik@sha256:c888963af81054ac8c158404fbacff203fc05de699fd77ef99fdb276b0e742e0
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2109597280 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4493990f99f036c842802ae6b9593cf761ac18dbc67fd5cd1a322a84c2697c5e`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Fri, 05 May 2023 12:05:28 GMT
RUN Install update 10.0.17763.4377
# Wed, 10 May 2023 00:36:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 May 2023 06:31:45 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.10.1/traefik_v2.10.1_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Wed, 10 May 2023 06:31:46 GMT
EXPOSE 80
# Wed, 10 May 2023 06:31:47 GMT
ENTRYPOINT ["/traefik"]
# Wed, 10 May 2023 06:31:48 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e01de39a0c44e24aa1912078d32ee54389b71154e509138cc4f5d1de42e7a32a`  
		Last Modified: Wed, 10 May 2023 01:47:41 GMT  
		Size: 364.1 MB (364091294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15a238e462da347b2e29386c9883c0ec93c8dbce311782ea1c5abbec2a31d884`  
		Last Modified: Wed, 10 May 2023 01:46:46 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df6b1b568e48ea9b9c1126801eb055cc1d9aa1e21270219140c58f2e1253a636`  
		Last Modified: Wed, 10 May 2023 07:14:51 GMT  
		Size: 37.6 MB (37556455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f754667a3def555298e795f9f84b666f44e7d683178bc69b2765cc10fa741ec1`  
		Last Modified: Wed, 10 May 2023 07:14:44 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:269055700abc29f93e7940722c0a8c7c9423dd04dd3dcbf84caac07612d4b1cc`  
		Last Modified: Wed, 10 May 2023 07:14:44 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdc6c3594a8fea61840c387597d673ca691a7633347d397c73b3b0b849a173d1`  
		Last Modified: Wed, 10 May 2023 07:14:44 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
