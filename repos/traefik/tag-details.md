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
$ docker pull traefik@sha256:d6d776c62575fb3b396cb467234e0dd247bf254533323118bf98d5369ce399e3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:2.10` - linux; amd64

```console
$ docker pull traefik@sha256:e14a97009734c3ac7f7fbabc18cc5a068143c4e25d0d072a0d10bee2c1c7312c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.0 MB (40990699 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:75f6529f13bb8557fa01f41f878e79f3714d703f4ae52d6d5c700a580877da90`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 14 Jun 2023 20:42:04 GMT
ADD file:828b07e74c184e7f251ed992ff195cdc50fdca345f13ff484e258851d928d950 in / 
# Wed, 14 Jun 2023 20:42:04 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 06:27:35 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 15 Jun 2023 06:27:38 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.1/traefik_v2.10.1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 15 Jun 2023 06:27:38 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 15 Jun 2023 06:27:38 GMT
EXPOSE 80
# Thu, 15 Jun 2023 06:27:38 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 15 Jun 2023 06:27:39 GMT
CMD ["traefik"]
# Thu, 15 Jun 2023 06:27:39 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4db1b89c0bd13344176ddce2d093b9da2ae58336823ffed2009a7ea4b62d2a95`  
		Last Modified: Wed, 14 Jun 2023 20:42:37 GMT  
		Size: 3.4 MB (3374713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d68693d54c11729ff385d1eebbcf2d487268fe3d0030be219f32ad8c717664c`  
		Last Modified: Thu, 15 Jun 2023 06:28:09 GMT  
		Size: 622.4 KB (622389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e2a95bcf565f364a3b5f9a4b04e21d5327717fc8241186142ea0072d1a33a84`  
		Last Modified: Thu, 15 Jun 2023 06:28:15 GMT  
		Size: 37.0 MB (36993228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0bec7d4cba02c558bc5f947fbe89df277f46e49d8874185ea227323660f6ebd`  
		Last Modified: Thu, 15 Jun 2023 06:28:09 GMT  
		Size: 369.0 B  
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
$ docker pull traefik@sha256:6f25e308d9878b8e8bbf8e6dafe2c14d63603407bea656519f8edc23314e9afe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4499; amd64

### `traefik:2.10-windowsservercore-1809` - windows version 10.0.17763.4499; amd64

```console
$ docker pull traefik@sha256:38c05bc5d5b1fed6f46d49c436c6799455aaf44d4ebe5761ca0f4ce80b0484a2
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.7 GB (1688053125 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0296470c640092d32d47853bb9ce910aea86f173c2e6b99c928d414fca68dd74`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Wed, 14 Jun 2023 17:39:58 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Jun 2023 23:21:07 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.10.1/traefik_v2.10.1_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Wed, 14 Jun 2023 23:21:07 GMT
EXPOSE 80
# Wed, 14 Jun 2023 23:21:08 GMT
ENTRYPOINT ["/traefik"]
# Wed, 14 Jun 2023 23:21:09 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b712a9a082fd391beaa9ca7c8e6c3fda37b0ad8d29cc4663173ed973b961d342`  
		Last Modified: Wed, 14 Jun 2023 18:21:55 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1239fe21d714ec31d2c97dd138856e2047eb2e7f3dd5af11dcbb909150bca6a4`  
		Last Modified: Wed, 14 Jun 2023 23:22:04 GMT  
		Size: 37.4 MB (37427190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8ca5d47e1e4a4fb8896368092bad8dc75a36016da70c433a7748adc078f3bac`  
		Last Modified: Wed, 14 Jun 2023 23:21:56 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6387bbce68fc59152ba2d4c40d6156cc95d2f175b730a7378000bbda5097369f`  
		Last Modified: Wed, 14 Jun 2023 23:21:56 GMT  
		Size: 1.4 KB (1380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adda4c788527d598ef60970509366fa8b5675941cde2de8afab18bf0cf4d7f7b`  
		Last Modified: Wed, 14 Jun 2023 23:21:56 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:2.10.1`

```console
$ docker pull traefik@sha256:d6d776c62575fb3b396cb467234e0dd247bf254533323118bf98d5369ce399e3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:2.10.1` - linux; amd64

```console
$ docker pull traefik@sha256:e14a97009734c3ac7f7fbabc18cc5a068143c4e25d0d072a0d10bee2c1c7312c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.0 MB (40990699 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:75f6529f13bb8557fa01f41f878e79f3714d703f4ae52d6d5c700a580877da90`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 14 Jun 2023 20:42:04 GMT
ADD file:828b07e74c184e7f251ed992ff195cdc50fdca345f13ff484e258851d928d950 in / 
# Wed, 14 Jun 2023 20:42:04 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 06:27:35 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 15 Jun 2023 06:27:38 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.1/traefik_v2.10.1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 15 Jun 2023 06:27:38 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 15 Jun 2023 06:27:38 GMT
EXPOSE 80
# Thu, 15 Jun 2023 06:27:38 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 15 Jun 2023 06:27:39 GMT
CMD ["traefik"]
# Thu, 15 Jun 2023 06:27:39 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4db1b89c0bd13344176ddce2d093b9da2ae58336823ffed2009a7ea4b62d2a95`  
		Last Modified: Wed, 14 Jun 2023 20:42:37 GMT  
		Size: 3.4 MB (3374713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d68693d54c11729ff385d1eebbcf2d487268fe3d0030be219f32ad8c717664c`  
		Last Modified: Thu, 15 Jun 2023 06:28:09 GMT  
		Size: 622.4 KB (622389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e2a95bcf565f364a3b5f9a4b04e21d5327717fc8241186142ea0072d1a33a84`  
		Last Modified: Thu, 15 Jun 2023 06:28:15 GMT  
		Size: 37.0 MB (36993228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0bec7d4cba02c558bc5f947fbe89df277f46e49d8874185ea227323660f6ebd`  
		Last Modified: Thu, 15 Jun 2023 06:28:09 GMT  
		Size: 369.0 B  
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
$ docker pull traefik@sha256:6f25e308d9878b8e8bbf8e6dafe2c14d63603407bea656519f8edc23314e9afe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4499; amd64

### `traefik:2.10.1-windowsservercore-1809` - windows version 10.0.17763.4499; amd64

```console
$ docker pull traefik@sha256:38c05bc5d5b1fed6f46d49c436c6799455aaf44d4ebe5761ca0f4ce80b0484a2
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.7 GB (1688053125 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0296470c640092d32d47853bb9ce910aea86f173c2e6b99c928d414fca68dd74`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Wed, 14 Jun 2023 17:39:58 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Jun 2023 23:21:07 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.10.1/traefik_v2.10.1_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Wed, 14 Jun 2023 23:21:07 GMT
EXPOSE 80
# Wed, 14 Jun 2023 23:21:08 GMT
ENTRYPOINT ["/traefik"]
# Wed, 14 Jun 2023 23:21:09 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b712a9a082fd391beaa9ca7c8e6c3fda37b0ad8d29cc4663173ed973b961d342`  
		Last Modified: Wed, 14 Jun 2023 18:21:55 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1239fe21d714ec31d2c97dd138856e2047eb2e7f3dd5af11dcbb909150bca6a4`  
		Last Modified: Wed, 14 Jun 2023 23:22:04 GMT  
		Size: 37.4 MB (37427190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8ca5d47e1e4a4fb8896368092bad8dc75a36016da70c433a7748adc078f3bac`  
		Last Modified: Wed, 14 Jun 2023 23:21:56 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6387bbce68fc59152ba2d4c40d6156cc95d2f175b730a7378000bbda5097369f`  
		Last Modified: Wed, 14 Jun 2023 23:21:56 GMT  
		Size: 1.4 KB (1380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adda4c788527d598ef60970509366fa8b5675941cde2de8afab18bf0cf4d7f7b`  
		Last Modified: Wed, 14 Jun 2023 23:21:56 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:3.0`

```console
$ docker pull traefik@sha256:ed47de5df8e31883b51a0b8d7add5a4732195d49f416065049d552a8c089dff1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:3.0` - linux; amd64

```console
$ docker pull traefik@sha256:5f3e471200c36a65618b50719f8f467530a9895a61f87bda0bb437b5718ac327
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.6 MB (40562366 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c08e518a729607ef1142c8a57a82ab9df16bcd47e4e5a6874d07467e07a87dd0`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 14 Jun 2023 20:42:13 GMT
ADD file:4fa8e307f595ecff485113fb0ec6e2320979eaa6fb3eb467d2433771a6f016e6 in / 
# Wed, 14 Jun 2023 20:42:13 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 06:27:27 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 15 Jun 2023 06:27:31 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta2/traefik_v3.0.0-beta2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 15 Jun 2023 06:27:31 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 15 Jun 2023 06:27:31 GMT
EXPOSE 80
# Thu, 15 Jun 2023 06:27:31 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 15 Jun 2023 06:27:31 GMT
CMD ["traefik"]
# Thu, 15 Jun 2023 06:27:31 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:0cdfa0c98ed79707cd91c5dd7ebd282aa2b976d86a9e699d7fc188cdb6be390e`  
		Last Modified: Wed, 14 Jun 2023 20:42:58 GMT  
		Size: 2.8 MB (2825916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75174169df6666c22d9a3c3085ea1eacd10478e79c70bbd53abc6cf647134b86`  
		Last Modified: Thu, 15 Jun 2023 06:27:51 GMT  
		Size: 661.2 KB (661203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4920635d165c3cb67e2ee3fd37aec68049e9730086d72999c5d926fd5a2b5bdb`  
		Last Modified: Thu, 15 Jun 2023 06:27:56 GMT  
		Size: 37.1 MB (37074878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:133801879169abc43871a5a32c77fb651e1ae90c3233a0cce11b6ead5c526c79`  
		Last Modified: Thu, 15 Jun 2023 06:27:50 GMT  
		Size: 369.0 B  
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
$ docker pull traefik@sha256:468282899a6f9b06f9fca5ebb1a3a5bf030b45e63e0508f36f75ad7792100318
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4499; amd64

### `traefik:3.0-windowsservercore-1809` - windows version 10.0.17763.4499; amd64

```console
$ docker pull traefik@sha256:58a44dc3d5c4e9816d6873d753a6074c23aa7a462052f72f8fb60172ae00773b
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.7 GB (1688143673 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:01f1804410c439a02c3fbb603e3dc9c1a10922016750389db87aed22db51adb2`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Wed, 14 Jun 2023 17:39:58 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Jun 2023 23:20:14 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v3.0.0-beta2/traefik_v3.0.0-beta2_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Wed, 14 Jun 2023 23:20:15 GMT
EXPOSE 80
# Wed, 14 Jun 2023 23:20:15 GMT
ENTRYPOINT ["/traefik"]
# Wed, 14 Jun 2023 23:20:16 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b712a9a082fd391beaa9ca7c8e6c3fda37b0ad8d29cc4663173ed973b961d342`  
		Last Modified: Wed, 14 Jun 2023 18:21:55 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a9b4e4d63720e53bc602ec5afd594ae87dc8d306b5873781d0fd3055f818c16`  
		Last Modified: Wed, 14 Jun 2023 23:21:42 GMT  
		Size: 37.5 MB (37517697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef864bbe2da9a6fc6aba62dc459a1b659d3d46ada2e3a1a04ee8b7c02a6f4e92`  
		Last Modified: Wed, 14 Jun 2023 23:21:33 GMT  
		Size: 1.4 KB (1377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2213ec09fd524be95c6a826c50e14f52e9e639e66c3572d56f438bac3cf98bab`  
		Last Modified: Wed, 14 Jun 2023 23:21:33 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58cd9c99e4865330e999c8136c9600504c563b6c37779e28663ff1421a7ac516`  
		Last Modified: Wed, 14 Jun 2023 23:21:33 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:3.0.0-beta2`

```console
$ docker pull traefik@sha256:ed47de5df8e31883b51a0b8d7add5a4732195d49f416065049d552a8c089dff1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:3.0.0-beta2` - linux; amd64

```console
$ docker pull traefik@sha256:5f3e471200c36a65618b50719f8f467530a9895a61f87bda0bb437b5718ac327
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.6 MB (40562366 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c08e518a729607ef1142c8a57a82ab9df16bcd47e4e5a6874d07467e07a87dd0`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 14 Jun 2023 20:42:13 GMT
ADD file:4fa8e307f595ecff485113fb0ec6e2320979eaa6fb3eb467d2433771a6f016e6 in / 
# Wed, 14 Jun 2023 20:42:13 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 06:27:27 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 15 Jun 2023 06:27:31 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta2/traefik_v3.0.0-beta2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 15 Jun 2023 06:27:31 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 15 Jun 2023 06:27:31 GMT
EXPOSE 80
# Thu, 15 Jun 2023 06:27:31 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 15 Jun 2023 06:27:31 GMT
CMD ["traefik"]
# Thu, 15 Jun 2023 06:27:31 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:0cdfa0c98ed79707cd91c5dd7ebd282aa2b976d86a9e699d7fc188cdb6be390e`  
		Last Modified: Wed, 14 Jun 2023 20:42:58 GMT  
		Size: 2.8 MB (2825916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75174169df6666c22d9a3c3085ea1eacd10478e79c70bbd53abc6cf647134b86`  
		Last Modified: Thu, 15 Jun 2023 06:27:51 GMT  
		Size: 661.2 KB (661203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4920635d165c3cb67e2ee3fd37aec68049e9730086d72999c5d926fd5a2b5bdb`  
		Last Modified: Thu, 15 Jun 2023 06:27:56 GMT  
		Size: 37.1 MB (37074878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:133801879169abc43871a5a32c77fb651e1ae90c3233a0cce11b6ead5c526c79`  
		Last Modified: Thu, 15 Jun 2023 06:27:50 GMT  
		Size: 369.0 B  
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
$ docker pull traefik@sha256:468282899a6f9b06f9fca5ebb1a3a5bf030b45e63e0508f36f75ad7792100318
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4499; amd64

### `traefik:3.0.0-beta2-windowsservercore-1809` - windows version 10.0.17763.4499; amd64

```console
$ docker pull traefik@sha256:58a44dc3d5c4e9816d6873d753a6074c23aa7a462052f72f8fb60172ae00773b
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.7 GB (1688143673 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:01f1804410c439a02c3fbb603e3dc9c1a10922016750389db87aed22db51adb2`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Wed, 14 Jun 2023 17:39:58 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Jun 2023 23:20:14 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v3.0.0-beta2/traefik_v3.0.0-beta2_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Wed, 14 Jun 2023 23:20:15 GMT
EXPOSE 80
# Wed, 14 Jun 2023 23:20:15 GMT
ENTRYPOINT ["/traefik"]
# Wed, 14 Jun 2023 23:20:16 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b712a9a082fd391beaa9ca7c8e6c3fda37b0ad8d29cc4663173ed973b961d342`  
		Last Modified: Wed, 14 Jun 2023 18:21:55 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a9b4e4d63720e53bc602ec5afd594ae87dc8d306b5873781d0fd3055f818c16`  
		Last Modified: Wed, 14 Jun 2023 23:21:42 GMT  
		Size: 37.5 MB (37517697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef864bbe2da9a6fc6aba62dc459a1b659d3d46ada2e3a1a04ee8b7c02a6f4e92`  
		Last Modified: Wed, 14 Jun 2023 23:21:33 GMT  
		Size: 1.4 KB (1377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2213ec09fd524be95c6a826c50e14f52e9e639e66c3572d56f438bac3cf98bab`  
		Last Modified: Wed, 14 Jun 2023 23:21:33 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58cd9c99e4865330e999c8136c9600504c563b6c37779e28663ff1421a7ac516`  
		Last Modified: Wed, 14 Jun 2023 23:21:33 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:beaufort`

```console
$ docker pull traefik@sha256:ed47de5df8e31883b51a0b8d7add5a4732195d49f416065049d552a8c089dff1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:beaufort` - linux; amd64

```console
$ docker pull traefik@sha256:5f3e471200c36a65618b50719f8f467530a9895a61f87bda0bb437b5718ac327
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.6 MB (40562366 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c08e518a729607ef1142c8a57a82ab9df16bcd47e4e5a6874d07467e07a87dd0`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 14 Jun 2023 20:42:13 GMT
ADD file:4fa8e307f595ecff485113fb0ec6e2320979eaa6fb3eb467d2433771a6f016e6 in / 
# Wed, 14 Jun 2023 20:42:13 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 06:27:27 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 15 Jun 2023 06:27:31 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta2/traefik_v3.0.0-beta2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 15 Jun 2023 06:27:31 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 15 Jun 2023 06:27:31 GMT
EXPOSE 80
# Thu, 15 Jun 2023 06:27:31 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 15 Jun 2023 06:27:31 GMT
CMD ["traefik"]
# Thu, 15 Jun 2023 06:27:31 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:0cdfa0c98ed79707cd91c5dd7ebd282aa2b976d86a9e699d7fc188cdb6be390e`  
		Last Modified: Wed, 14 Jun 2023 20:42:58 GMT  
		Size: 2.8 MB (2825916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75174169df6666c22d9a3c3085ea1eacd10478e79c70bbd53abc6cf647134b86`  
		Last Modified: Thu, 15 Jun 2023 06:27:51 GMT  
		Size: 661.2 KB (661203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4920635d165c3cb67e2ee3fd37aec68049e9730086d72999c5d926fd5a2b5bdb`  
		Last Modified: Thu, 15 Jun 2023 06:27:56 GMT  
		Size: 37.1 MB (37074878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:133801879169abc43871a5a32c77fb651e1ae90c3233a0cce11b6ead5c526c79`  
		Last Modified: Thu, 15 Jun 2023 06:27:50 GMT  
		Size: 369.0 B  
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
$ docker pull traefik@sha256:468282899a6f9b06f9fca5ebb1a3a5bf030b45e63e0508f36f75ad7792100318
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4499; amd64

### `traefik:beaufort-windowsservercore-1809` - windows version 10.0.17763.4499; amd64

```console
$ docker pull traefik@sha256:58a44dc3d5c4e9816d6873d753a6074c23aa7a462052f72f8fb60172ae00773b
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.7 GB (1688143673 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:01f1804410c439a02c3fbb603e3dc9c1a10922016750389db87aed22db51adb2`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Wed, 14 Jun 2023 17:39:58 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Jun 2023 23:20:14 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v3.0.0-beta2/traefik_v3.0.0-beta2_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Wed, 14 Jun 2023 23:20:15 GMT
EXPOSE 80
# Wed, 14 Jun 2023 23:20:15 GMT
ENTRYPOINT ["/traefik"]
# Wed, 14 Jun 2023 23:20:16 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b712a9a082fd391beaa9ca7c8e6c3fda37b0ad8d29cc4663173ed973b961d342`  
		Last Modified: Wed, 14 Jun 2023 18:21:55 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a9b4e4d63720e53bc602ec5afd594ae87dc8d306b5873781d0fd3055f818c16`  
		Last Modified: Wed, 14 Jun 2023 23:21:42 GMT  
		Size: 37.5 MB (37517697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef864bbe2da9a6fc6aba62dc459a1b659d3d46ada2e3a1a04ee8b7c02a6f4e92`  
		Last Modified: Wed, 14 Jun 2023 23:21:33 GMT  
		Size: 1.4 KB (1377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2213ec09fd524be95c6a826c50e14f52e9e639e66c3572d56f438bac3cf98bab`  
		Last Modified: Wed, 14 Jun 2023 23:21:33 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58cd9c99e4865330e999c8136c9600504c563b6c37779e28663ff1421a7ac516`  
		Last Modified: Wed, 14 Jun 2023 23:21:33 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:latest`

```console
$ docker pull traefik@sha256:d6d776c62575fb3b396cb467234e0dd247bf254533323118bf98d5369ce399e3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:latest` - linux; amd64

```console
$ docker pull traefik@sha256:e14a97009734c3ac7f7fbabc18cc5a068143c4e25d0d072a0d10bee2c1c7312c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.0 MB (40990699 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:75f6529f13bb8557fa01f41f878e79f3714d703f4ae52d6d5c700a580877da90`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 14 Jun 2023 20:42:04 GMT
ADD file:828b07e74c184e7f251ed992ff195cdc50fdca345f13ff484e258851d928d950 in / 
# Wed, 14 Jun 2023 20:42:04 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 06:27:35 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 15 Jun 2023 06:27:38 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.1/traefik_v2.10.1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 15 Jun 2023 06:27:38 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 15 Jun 2023 06:27:38 GMT
EXPOSE 80
# Thu, 15 Jun 2023 06:27:38 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 15 Jun 2023 06:27:39 GMT
CMD ["traefik"]
# Thu, 15 Jun 2023 06:27:39 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4db1b89c0bd13344176ddce2d093b9da2ae58336823ffed2009a7ea4b62d2a95`  
		Last Modified: Wed, 14 Jun 2023 20:42:37 GMT  
		Size: 3.4 MB (3374713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d68693d54c11729ff385d1eebbcf2d487268fe3d0030be219f32ad8c717664c`  
		Last Modified: Thu, 15 Jun 2023 06:28:09 GMT  
		Size: 622.4 KB (622389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e2a95bcf565f364a3b5f9a4b04e21d5327717fc8241186142ea0072d1a33a84`  
		Last Modified: Thu, 15 Jun 2023 06:28:15 GMT  
		Size: 37.0 MB (36993228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0bec7d4cba02c558bc5f947fbe89df277f46e49d8874185ea227323660f6ebd`  
		Last Modified: Thu, 15 Jun 2023 06:28:09 GMT  
		Size: 369.0 B  
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
$ docker pull traefik@sha256:d6d776c62575fb3b396cb467234e0dd247bf254533323118bf98d5369ce399e3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:saintmarcelin` - linux; amd64

```console
$ docker pull traefik@sha256:e14a97009734c3ac7f7fbabc18cc5a068143c4e25d0d072a0d10bee2c1c7312c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.0 MB (40990699 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:75f6529f13bb8557fa01f41f878e79f3714d703f4ae52d6d5c700a580877da90`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 14 Jun 2023 20:42:04 GMT
ADD file:828b07e74c184e7f251ed992ff195cdc50fdca345f13ff484e258851d928d950 in / 
# Wed, 14 Jun 2023 20:42:04 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 06:27:35 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 15 Jun 2023 06:27:38 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.1/traefik_v2.10.1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 15 Jun 2023 06:27:38 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 15 Jun 2023 06:27:38 GMT
EXPOSE 80
# Thu, 15 Jun 2023 06:27:38 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 15 Jun 2023 06:27:39 GMT
CMD ["traefik"]
# Thu, 15 Jun 2023 06:27:39 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4db1b89c0bd13344176ddce2d093b9da2ae58336823ffed2009a7ea4b62d2a95`  
		Last Modified: Wed, 14 Jun 2023 20:42:37 GMT  
		Size: 3.4 MB (3374713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d68693d54c11729ff385d1eebbcf2d487268fe3d0030be219f32ad8c717664c`  
		Last Modified: Thu, 15 Jun 2023 06:28:09 GMT  
		Size: 622.4 KB (622389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e2a95bcf565f364a3b5f9a4b04e21d5327717fc8241186142ea0072d1a33a84`  
		Last Modified: Thu, 15 Jun 2023 06:28:15 GMT  
		Size: 37.0 MB (36993228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0bec7d4cba02c558bc5f947fbe89df277f46e49d8874185ea227323660f6ebd`  
		Last Modified: Thu, 15 Jun 2023 06:28:09 GMT  
		Size: 369.0 B  
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
$ docker pull traefik@sha256:6f25e308d9878b8e8bbf8e6dafe2c14d63603407bea656519f8edc23314e9afe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4499; amd64

### `traefik:saintmarcelin-windowsservercore-1809` - windows version 10.0.17763.4499; amd64

```console
$ docker pull traefik@sha256:38c05bc5d5b1fed6f46d49c436c6799455aaf44d4ebe5761ca0f4ce80b0484a2
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.7 GB (1688053125 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0296470c640092d32d47853bb9ce910aea86f173c2e6b99c928d414fca68dd74`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Wed, 14 Jun 2023 17:39:58 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Jun 2023 23:21:07 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.10.1/traefik_v2.10.1_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Wed, 14 Jun 2023 23:21:07 GMT
EXPOSE 80
# Wed, 14 Jun 2023 23:21:08 GMT
ENTRYPOINT ["/traefik"]
# Wed, 14 Jun 2023 23:21:09 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b712a9a082fd391beaa9ca7c8e6c3fda37b0ad8d29cc4663173ed973b961d342`  
		Last Modified: Wed, 14 Jun 2023 18:21:55 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1239fe21d714ec31d2c97dd138856e2047eb2e7f3dd5af11dcbb909150bca6a4`  
		Last Modified: Wed, 14 Jun 2023 23:22:04 GMT  
		Size: 37.4 MB (37427190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8ca5d47e1e4a4fb8896368092bad8dc75a36016da70c433a7748adc078f3bac`  
		Last Modified: Wed, 14 Jun 2023 23:21:56 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6387bbce68fc59152ba2d4c40d6156cc95d2f175b730a7378000bbda5097369f`  
		Last Modified: Wed, 14 Jun 2023 23:21:56 GMT  
		Size: 1.4 KB (1380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adda4c788527d598ef60970509366fa8b5675941cde2de8afab18bf0cf4d7f7b`  
		Last Modified: Wed, 14 Jun 2023 23:21:56 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.10`

```console
$ docker pull traefik@sha256:d6d776c62575fb3b396cb467234e0dd247bf254533323118bf98d5369ce399e3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:v2.10` - linux; amd64

```console
$ docker pull traefik@sha256:e14a97009734c3ac7f7fbabc18cc5a068143c4e25d0d072a0d10bee2c1c7312c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.0 MB (40990699 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:75f6529f13bb8557fa01f41f878e79f3714d703f4ae52d6d5c700a580877da90`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 14 Jun 2023 20:42:04 GMT
ADD file:828b07e74c184e7f251ed992ff195cdc50fdca345f13ff484e258851d928d950 in / 
# Wed, 14 Jun 2023 20:42:04 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 06:27:35 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 15 Jun 2023 06:27:38 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.1/traefik_v2.10.1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 15 Jun 2023 06:27:38 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 15 Jun 2023 06:27:38 GMT
EXPOSE 80
# Thu, 15 Jun 2023 06:27:38 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 15 Jun 2023 06:27:39 GMT
CMD ["traefik"]
# Thu, 15 Jun 2023 06:27:39 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4db1b89c0bd13344176ddce2d093b9da2ae58336823ffed2009a7ea4b62d2a95`  
		Last Modified: Wed, 14 Jun 2023 20:42:37 GMT  
		Size: 3.4 MB (3374713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d68693d54c11729ff385d1eebbcf2d487268fe3d0030be219f32ad8c717664c`  
		Last Modified: Thu, 15 Jun 2023 06:28:09 GMT  
		Size: 622.4 KB (622389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e2a95bcf565f364a3b5f9a4b04e21d5327717fc8241186142ea0072d1a33a84`  
		Last Modified: Thu, 15 Jun 2023 06:28:15 GMT  
		Size: 37.0 MB (36993228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0bec7d4cba02c558bc5f947fbe89df277f46e49d8874185ea227323660f6ebd`  
		Last Modified: Thu, 15 Jun 2023 06:28:09 GMT  
		Size: 369.0 B  
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
$ docker pull traefik@sha256:6f25e308d9878b8e8bbf8e6dafe2c14d63603407bea656519f8edc23314e9afe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4499; amd64

### `traefik:v2.10-windowsservercore-1809` - windows version 10.0.17763.4499; amd64

```console
$ docker pull traefik@sha256:38c05bc5d5b1fed6f46d49c436c6799455aaf44d4ebe5761ca0f4ce80b0484a2
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.7 GB (1688053125 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0296470c640092d32d47853bb9ce910aea86f173c2e6b99c928d414fca68dd74`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Wed, 14 Jun 2023 17:39:58 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Jun 2023 23:21:07 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.10.1/traefik_v2.10.1_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Wed, 14 Jun 2023 23:21:07 GMT
EXPOSE 80
# Wed, 14 Jun 2023 23:21:08 GMT
ENTRYPOINT ["/traefik"]
# Wed, 14 Jun 2023 23:21:09 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b712a9a082fd391beaa9ca7c8e6c3fda37b0ad8d29cc4663173ed973b961d342`  
		Last Modified: Wed, 14 Jun 2023 18:21:55 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1239fe21d714ec31d2c97dd138856e2047eb2e7f3dd5af11dcbb909150bca6a4`  
		Last Modified: Wed, 14 Jun 2023 23:22:04 GMT  
		Size: 37.4 MB (37427190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8ca5d47e1e4a4fb8896368092bad8dc75a36016da70c433a7748adc078f3bac`  
		Last Modified: Wed, 14 Jun 2023 23:21:56 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6387bbce68fc59152ba2d4c40d6156cc95d2f175b730a7378000bbda5097369f`  
		Last Modified: Wed, 14 Jun 2023 23:21:56 GMT  
		Size: 1.4 KB (1380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adda4c788527d598ef60970509366fa8b5675941cde2de8afab18bf0cf4d7f7b`  
		Last Modified: Wed, 14 Jun 2023 23:21:56 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.10.1`

```console
$ docker pull traefik@sha256:d6d776c62575fb3b396cb467234e0dd247bf254533323118bf98d5369ce399e3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:v2.10.1` - linux; amd64

```console
$ docker pull traefik@sha256:e14a97009734c3ac7f7fbabc18cc5a068143c4e25d0d072a0d10bee2c1c7312c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.0 MB (40990699 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:75f6529f13bb8557fa01f41f878e79f3714d703f4ae52d6d5c700a580877da90`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 14 Jun 2023 20:42:04 GMT
ADD file:828b07e74c184e7f251ed992ff195cdc50fdca345f13ff484e258851d928d950 in / 
# Wed, 14 Jun 2023 20:42:04 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 06:27:35 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 15 Jun 2023 06:27:38 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.10.1/traefik_v2.10.1_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 15 Jun 2023 06:27:38 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 15 Jun 2023 06:27:38 GMT
EXPOSE 80
# Thu, 15 Jun 2023 06:27:38 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 15 Jun 2023 06:27:39 GMT
CMD ["traefik"]
# Thu, 15 Jun 2023 06:27:39 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:4db1b89c0bd13344176ddce2d093b9da2ae58336823ffed2009a7ea4b62d2a95`  
		Last Modified: Wed, 14 Jun 2023 20:42:37 GMT  
		Size: 3.4 MB (3374713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d68693d54c11729ff385d1eebbcf2d487268fe3d0030be219f32ad8c717664c`  
		Last Modified: Thu, 15 Jun 2023 06:28:09 GMT  
		Size: 622.4 KB (622389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e2a95bcf565f364a3b5f9a4b04e21d5327717fc8241186142ea0072d1a33a84`  
		Last Modified: Thu, 15 Jun 2023 06:28:15 GMT  
		Size: 37.0 MB (36993228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0bec7d4cba02c558bc5f947fbe89df277f46e49d8874185ea227323660f6ebd`  
		Last Modified: Thu, 15 Jun 2023 06:28:09 GMT  
		Size: 369.0 B  
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
$ docker pull traefik@sha256:6f25e308d9878b8e8bbf8e6dafe2c14d63603407bea656519f8edc23314e9afe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4499; amd64

### `traefik:v2.10.1-windowsservercore-1809` - windows version 10.0.17763.4499; amd64

```console
$ docker pull traefik@sha256:38c05bc5d5b1fed6f46d49c436c6799455aaf44d4ebe5761ca0f4ce80b0484a2
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.7 GB (1688053125 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0296470c640092d32d47853bb9ce910aea86f173c2e6b99c928d414fca68dd74`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Wed, 14 Jun 2023 17:39:58 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Jun 2023 23:21:07 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.10.1/traefik_v2.10.1_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Wed, 14 Jun 2023 23:21:07 GMT
EXPOSE 80
# Wed, 14 Jun 2023 23:21:08 GMT
ENTRYPOINT ["/traefik"]
# Wed, 14 Jun 2023 23:21:09 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b712a9a082fd391beaa9ca7c8e6c3fda37b0ad8d29cc4663173ed973b961d342`  
		Last Modified: Wed, 14 Jun 2023 18:21:55 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1239fe21d714ec31d2c97dd138856e2047eb2e7f3dd5af11dcbb909150bca6a4`  
		Last Modified: Wed, 14 Jun 2023 23:22:04 GMT  
		Size: 37.4 MB (37427190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8ca5d47e1e4a4fb8896368092bad8dc75a36016da70c433a7748adc078f3bac`  
		Last Modified: Wed, 14 Jun 2023 23:21:56 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6387bbce68fc59152ba2d4c40d6156cc95d2f175b730a7378000bbda5097369f`  
		Last Modified: Wed, 14 Jun 2023 23:21:56 GMT  
		Size: 1.4 KB (1380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adda4c788527d598ef60970509366fa8b5675941cde2de8afab18bf0cf4d7f7b`  
		Last Modified: Wed, 14 Jun 2023 23:21:56 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v3.0`

```console
$ docker pull traefik@sha256:ed47de5df8e31883b51a0b8d7add5a4732195d49f416065049d552a8c089dff1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:v3.0` - linux; amd64

```console
$ docker pull traefik@sha256:5f3e471200c36a65618b50719f8f467530a9895a61f87bda0bb437b5718ac327
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.6 MB (40562366 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c08e518a729607ef1142c8a57a82ab9df16bcd47e4e5a6874d07467e07a87dd0`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 14 Jun 2023 20:42:13 GMT
ADD file:4fa8e307f595ecff485113fb0ec6e2320979eaa6fb3eb467d2433771a6f016e6 in / 
# Wed, 14 Jun 2023 20:42:13 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 06:27:27 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 15 Jun 2023 06:27:31 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta2/traefik_v3.0.0-beta2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 15 Jun 2023 06:27:31 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 15 Jun 2023 06:27:31 GMT
EXPOSE 80
# Thu, 15 Jun 2023 06:27:31 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 15 Jun 2023 06:27:31 GMT
CMD ["traefik"]
# Thu, 15 Jun 2023 06:27:31 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:0cdfa0c98ed79707cd91c5dd7ebd282aa2b976d86a9e699d7fc188cdb6be390e`  
		Last Modified: Wed, 14 Jun 2023 20:42:58 GMT  
		Size: 2.8 MB (2825916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75174169df6666c22d9a3c3085ea1eacd10478e79c70bbd53abc6cf647134b86`  
		Last Modified: Thu, 15 Jun 2023 06:27:51 GMT  
		Size: 661.2 KB (661203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4920635d165c3cb67e2ee3fd37aec68049e9730086d72999c5d926fd5a2b5bdb`  
		Last Modified: Thu, 15 Jun 2023 06:27:56 GMT  
		Size: 37.1 MB (37074878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:133801879169abc43871a5a32c77fb651e1ae90c3233a0cce11b6ead5c526c79`  
		Last Modified: Thu, 15 Jun 2023 06:27:50 GMT  
		Size: 369.0 B  
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
$ docker pull traefik@sha256:468282899a6f9b06f9fca5ebb1a3a5bf030b45e63e0508f36f75ad7792100318
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4499; amd64

### `traefik:v3.0-windowsservercore-1809` - windows version 10.0.17763.4499; amd64

```console
$ docker pull traefik@sha256:58a44dc3d5c4e9816d6873d753a6074c23aa7a462052f72f8fb60172ae00773b
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.7 GB (1688143673 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:01f1804410c439a02c3fbb603e3dc9c1a10922016750389db87aed22db51adb2`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Wed, 14 Jun 2023 17:39:58 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Jun 2023 23:20:14 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v3.0.0-beta2/traefik_v3.0.0-beta2_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Wed, 14 Jun 2023 23:20:15 GMT
EXPOSE 80
# Wed, 14 Jun 2023 23:20:15 GMT
ENTRYPOINT ["/traefik"]
# Wed, 14 Jun 2023 23:20:16 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b712a9a082fd391beaa9ca7c8e6c3fda37b0ad8d29cc4663173ed973b961d342`  
		Last Modified: Wed, 14 Jun 2023 18:21:55 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a9b4e4d63720e53bc602ec5afd594ae87dc8d306b5873781d0fd3055f818c16`  
		Last Modified: Wed, 14 Jun 2023 23:21:42 GMT  
		Size: 37.5 MB (37517697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef864bbe2da9a6fc6aba62dc459a1b659d3d46ada2e3a1a04ee8b7c02a6f4e92`  
		Last Modified: Wed, 14 Jun 2023 23:21:33 GMT  
		Size: 1.4 KB (1377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2213ec09fd524be95c6a826c50e14f52e9e639e66c3572d56f438bac3cf98bab`  
		Last Modified: Wed, 14 Jun 2023 23:21:33 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58cd9c99e4865330e999c8136c9600504c563b6c37779e28663ff1421a7ac516`  
		Last Modified: Wed, 14 Jun 2023 23:21:33 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v3.0.0-beta2`

```console
$ docker pull traefik@sha256:ed47de5df8e31883b51a0b8d7add5a4732195d49f416065049d552a8c089dff1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:v3.0.0-beta2` - linux; amd64

```console
$ docker pull traefik@sha256:5f3e471200c36a65618b50719f8f467530a9895a61f87bda0bb437b5718ac327
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.6 MB (40562366 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c08e518a729607ef1142c8a57a82ab9df16bcd47e4e5a6874d07467e07a87dd0`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Wed, 14 Jun 2023 20:42:13 GMT
ADD file:4fa8e307f595ecff485113fb0ec6e2320979eaa6fb3eb467d2433771a6f016e6 in / 
# Wed, 14 Jun 2023 20:42:13 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 06:27:27 GMT
RUN apk --no-cache add ca-certificates tzdata
# Thu, 15 Jun 2023 06:27:31 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta2/traefik_v3.0.0-beta2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Thu, 15 Jun 2023 06:27:31 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Thu, 15 Jun 2023 06:27:31 GMT
EXPOSE 80
# Thu, 15 Jun 2023 06:27:31 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 15 Jun 2023 06:27:31 GMT
CMD ["traefik"]
# Thu, 15 Jun 2023 06:27:31 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:0cdfa0c98ed79707cd91c5dd7ebd282aa2b976d86a9e699d7fc188cdb6be390e`  
		Last Modified: Wed, 14 Jun 2023 20:42:58 GMT  
		Size: 2.8 MB (2825916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75174169df6666c22d9a3c3085ea1eacd10478e79c70bbd53abc6cf647134b86`  
		Last Modified: Thu, 15 Jun 2023 06:27:51 GMT  
		Size: 661.2 KB (661203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4920635d165c3cb67e2ee3fd37aec68049e9730086d72999c5d926fd5a2b5bdb`  
		Last Modified: Thu, 15 Jun 2023 06:27:56 GMT  
		Size: 37.1 MB (37074878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:133801879169abc43871a5a32c77fb651e1ae90c3233a0cce11b6ead5c526c79`  
		Last Modified: Thu, 15 Jun 2023 06:27:50 GMT  
		Size: 369.0 B  
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
$ docker pull traefik@sha256:468282899a6f9b06f9fca5ebb1a3a5bf030b45e63e0508f36f75ad7792100318
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4499; amd64

### `traefik:v3.0.0-beta2-windowsservercore-1809` - windows version 10.0.17763.4499; amd64

```console
$ docker pull traefik@sha256:58a44dc3d5c4e9816d6873d753a6074c23aa7a462052f72f8fb60172ae00773b
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.7 GB (1688143673 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:01f1804410c439a02c3fbb603e3dc9c1a10922016750389db87aed22db51adb2`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Wed, 14 Jun 2023 17:39:58 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Jun 2023 23:20:14 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v3.0.0-beta2/traefik_v3.0.0-beta2_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Wed, 14 Jun 2023 23:20:15 GMT
EXPOSE 80
# Wed, 14 Jun 2023 23:20:15 GMT
ENTRYPOINT ["/traefik"]
# Wed, 14 Jun 2023 23:20:16 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b712a9a082fd391beaa9ca7c8e6c3fda37b0ad8d29cc4663173ed973b961d342`  
		Last Modified: Wed, 14 Jun 2023 18:21:55 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a9b4e4d63720e53bc602ec5afd594ae87dc8d306b5873781d0fd3055f818c16`  
		Last Modified: Wed, 14 Jun 2023 23:21:42 GMT  
		Size: 37.5 MB (37517697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef864bbe2da9a6fc6aba62dc459a1b659d3d46ada2e3a1a04ee8b7c02a6f4e92`  
		Last Modified: Wed, 14 Jun 2023 23:21:33 GMT  
		Size: 1.4 KB (1377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2213ec09fd524be95c6a826c50e14f52e9e639e66c3572d56f438bac3cf98bab`  
		Last Modified: Wed, 14 Jun 2023 23:21:33 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58cd9c99e4865330e999c8136c9600504c563b6c37779e28663ff1421a7ac516`  
		Last Modified: Wed, 14 Jun 2023 23:21:33 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:windowsservercore-1809`

```console
$ docker pull traefik@sha256:6f25e308d9878b8e8bbf8e6dafe2c14d63603407bea656519f8edc23314e9afe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4499; amd64

### `traefik:windowsservercore-1809` - windows version 10.0.17763.4499; amd64

```console
$ docker pull traefik@sha256:38c05bc5d5b1fed6f46d49c436c6799455aaf44d4ebe5761ca0f4ce80b0484a2
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.7 GB (1688053125 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0296470c640092d32d47853bb9ce910aea86f173c2e6b99c928d414fca68dd74`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Wed, 14 Jun 2023 17:39:58 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Jun 2023 23:21:07 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.10.1/traefik_v2.10.1_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Wed, 14 Jun 2023 23:21:07 GMT
EXPOSE 80
# Wed, 14 Jun 2023 23:21:08 GMT
ENTRYPOINT ["/traefik"]
# Wed, 14 Jun 2023 23:21:09 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.10.1 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b712a9a082fd391beaa9ca7c8e6c3fda37b0ad8d29cc4663173ed973b961d342`  
		Last Modified: Wed, 14 Jun 2023 18:21:55 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1239fe21d714ec31d2c97dd138856e2047eb2e7f3dd5af11dcbb909150bca6a4`  
		Last Modified: Wed, 14 Jun 2023 23:22:04 GMT  
		Size: 37.4 MB (37427190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8ca5d47e1e4a4fb8896368092bad8dc75a36016da70c433a7748adc078f3bac`  
		Last Modified: Wed, 14 Jun 2023 23:21:56 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6387bbce68fc59152ba2d4c40d6156cc95d2f175b730a7378000bbda5097369f`  
		Last Modified: Wed, 14 Jun 2023 23:21:56 GMT  
		Size: 1.4 KB (1380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adda4c788527d598ef60970509366fa8b5675941cde2de8afab18bf0cf4d7f7b`  
		Last Modified: Wed, 14 Jun 2023 23:21:56 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
