<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `nats`

-	[`nats:2`](#nats2)
-	[`nats:2-alpine`](#nats2-alpine)
-	[`nats:2-alpine3.15`](#nats2-alpine315)
-	[`nats:2-linux`](#nats2-linux)
-	[`nats:2-nanoserver`](#nats2-nanoserver)
-	[`nats:2-nanoserver-1809`](#nats2-nanoserver-1809)
-	[`nats:2-scratch`](#nats2-scratch)
-	[`nats:2-windowsservercore`](#nats2-windowsservercore)
-	[`nats:2-windowsservercore-1809`](#nats2-windowsservercore-1809)
-	[`nats:2.7`](#nats27)
-	[`nats:2.7-alpine`](#nats27-alpine)
-	[`nats:2.7-alpine3.15`](#nats27-alpine315)
-	[`nats:2.7-linux`](#nats27-linux)
-	[`nats:2.7-nanoserver`](#nats27-nanoserver)
-	[`nats:2.7-nanoserver-1809`](#nats27-nanoserver-1809)
-	[`nats:2.7-scratch`](#nats27-scratch)
-	[`nats:2.7-windowsservercore`](#nats27-windowsservercore)
-	[`nats:2.7-windowsservercore-1809`](#nats27-windowsservercore-1809)
-	[`nats:2.7.3`](#nats273)
-	[`nats:2.7.3-alpine`](#nats273-alpine)
-	[`nats:2.7.3-alpine3.15`](#nats273-alpine315)
-	[`nats:2.7.3-linux`](#nats273-linux)
-	[`nats:2.7.3-nanoserver`](#nats273-nanoserver)
-	[`nats:2.7.3-nanoserver-1809`](#nats273-nanoserver-1809)
-	[`nats:2.7.3-scratch`](#nats273-scratch)
-	[`nats:2.7.3-windowsservercore`](#nats273-windowsservercore)
-	[`nats:2.7.3-windowsservercore-1809`](#nats273-windowsservercore-1809)
-	[`nats:alpine`](#natsalpine)
-	[`nats:alpine3.15`](#natsalpine315)
-	[`nats:latest`](#natslatest)
-	[`nats:linux`](#natslinux)
-	[`nats:nanoserver`](#natsnanoserver)
-	[`nats:nanoserver-1809`](#natsnanoserver-1809)
-	[`nats:scratch`](#natsscratch)
-	[`nats:windowsservercore`](#natswindowsservercore)
-	[`nats:windowsservercore-1809`](#natswindowsservercore-1809)

## `nats:2`

```console
$ docker pull nats@sha256:4fa6d62e36bac738598e6523bb2185b0d57de021331057a538765f518cfd505a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.2565; amd64

### `nats:2` - linux; amd64

```console
$ docker pull nats@sha256:5fd249efa75cf3eb595342175207fdbb390eee3034f7fe49355d7a479fa3ffe2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4499407 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c84de17b17b3458d2b6e6d4264ea6186c82bab718ca058f5d7738e53ca2759ac`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 25 Feb 2022 02:21:13 GMT
COPY file:8a814b0c66a47e63e5a7f4287478948812fe6e03c224d539f37ce3f950d2b6c6 in /nats-server 
# Fri, 25 Feb 2022 02:21:13 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 25 Feb 2022 02:21:14 GMT
EXPOSE 4222 6222 8222
# Fri, 25 Feb 2022 02:21:14 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 25 Feb 2022 02:21:14 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:277fae1baf41821774f7a2e1c3f465b28aa8693ee0cd77e0ad0bace55d9c616e`  
		Last Modified: Fri, 25 Feb 2022 02:22:04 GMT  
		Size: 4.5 MB (4498900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb932b4b3fbc873b56e996c6357055bb7700c701d17d7d87cdec31211142b49a`  
		Last Modified: Fri, 25 Feb 2022 02:22:03 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - linux; arm variant v6

```console
$ docker pull nats@sha256:2e3339e7e8d98e7bbab0613c7b7c3dd6f51fcf33ed3910a2e65e62fba7049337
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4165977 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ddc7bcc78dd550ace4def82e3db227e618d77e136274749f3bf55869e64be264`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 25 Feb 2022 02:50:06 GMT
COPY file:3a951d885f7bcec693f6fbf26a9ffd82b0c6218b6834fc6053e5812f7451b63e in /nats-server 
# Fri, 25 Feb 2022 02:50:06 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 25 Feb 2022 02:50:07 GMT
EXPOSE 4222 6222 8222
# Fri, 25 Feb 2022 02:50:07 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 25 Feb 2022 02:50:07 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:f6de87b4530f922b11edc08be8edeebc6ce0cb666907013348d4e1b9f5d51809`  
		Last Modified: Fri, 25 Feb 2022 02:52:29 GMT  
		Size: 4.2 MB (4165468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5fa68b52226484e5870677184cdc47c93a7d453f334c144b5cb631346bc8111`  
		Last Modified: Fri, 25 Feb 2022 02:52:27 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - linux; arm variant v7

```console
$ docker pull nats@sha256:87cf3f8e33ebf28f35575ea083f8feb460d19fa9380d2622c82567ff3fa9d840
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4157918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4eef99b95e572b23f90d60e6e157be90b05ab2f35dbcb10f83f96ece551945a`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 25 Feb 2022 02:58:34 GMT
COPY file:3ee879939ad264e803dd4d6072181d968c4dd0fe076115159f70479c6309ef45 in /nats-server 
# Fri, 25 Feb 2022 02:58:34 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 25 Feb 2022 02:58:35 GMT
EXPOSE 4222 6222 8222
# Fri, 25 Feb 2022 02:58:35 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 25 Feb 2022 02:58:36 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:67a3d8907097b9caffd9d1720b4fb2b1d2ac9dfda60a1d169abbf5494323d50a`  
		Last Modified: Fri, 25 Feb 2022 03:00:58 GMT  
		Size: 4.2 MB (4157409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73f5577f4846f032b281220b897161962481198ead0a1b9ad1d7c76cdd989747`  
		Last Modified: Fri, 25 Feb 2022 03:00:55 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:e970861a260709ae1e8c892eb36758c14323e81959ff4aaa1e9b7327b91d3e70
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.1 MB (4143805 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4414e48026697a15338f28dcb8e46ace9627ea7332559e1708f36ce62a5e327`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 25 Feb 2022 03:01:42 GMT
COPY file:acd11e9a3a86f6f3da079c5155851337e747c3b31481ec05e2dd1e48e23becb2 in /nats-server 
# Fri, 25 Feb 2022 03:01:43 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 25 Feb 2022 03:01:43 GMT
EXPOSE 4222 6222 8222
# Fri, 25 Feb 2022 03:01:44 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 25 Feb 2022 03:01:45 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6ad9fd47af885b43442590ad2c8171e4b4899caef84921ec73ba0540b9c03284`  
		Last Modified: Fri, 25 Feb 2022 03:02:59 GMT  
		Size: 4.1 MB (4143299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02d7667f81936503f26a5ed657cfffdc9add626da8ae5bb78d691054cd3af7c3`  
		Last Modified: Fri, 25 Feb 2022 03:02:59 GMT  
		Size: 506.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - windows version 10.0.17763.2565; amd64

```console
$ docker pull nats@sha256:d7c795020fd7295382d503ba883e23cf34ca9c53d6e6b91184bc1fd2bb2c990d
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.6 MB (107634881 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6e99776e94a148ebda875656d07e673c65aedb583986faedb3bdc61a2fd7759`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 02 Feb 2022 19:06:51 GMT
RUN Apply image 1809-amd64
# Wed, 09 Feb 2022 18:13:36 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 25 Feb 2022 02:17:30 GMT
RUN cmd /S /C #(nop) COPY file:d5609a37f534b519fa4326428362ea5398f7165ee90493fb7bdc8b810da33b0e in C:\nats-server.exe 
# Fri, 25 Feb 2022 02:17:31 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Fri, 25 Feb 2022 02:17:32 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Fri, 25 Feb 2022 02:17:33 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 25 Feb 2022 02:17:34 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:bd0b37167cd3d731eb15196e123df7156b5a35597874d3016a1a4298c46fac3f`  
		Size: 103.1 MB (103087119 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8bc49c59cde14e3a9ed8fedce001c00fcb5fe0f9b914aa07273e04f23333d180`  
		Last Modified: Wed, 09 Feb 2022 18:14:28 GMT  
		Size: 1.1 KB (1138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b682f8d539489225b7a3859570b80452b497086f57fa4e6908f2b99d213e1a03`  
		Last Modified: Fri, 25 Feb 2022 03:15:32 GMT  
		Size: 4.5 MB (4541735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67997158a056ea601aec06de195ce0251264a6d8d071f8a44a49a545865ce426`  
		Last Modified: Fri, 25 Feb 2022 03:15:27 GMT  
		Size: 1.7 KB (1656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f873036aacce9bbc35378d6a36985e62919c6d2c9ff526011564a861b86240ab`  
		Last Modified: Fri, 25 Feb 2022 03:15:27 GMT  
		Size: 1.0 KB (1039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf1eace4b7f44dce795499001f62baee27fb477865e490b11d05d198c8e80550`  
		Last Modified: Fri, 25 Feb 2022 03:15:27 GMT  
		Size: 1.1 KB (1081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8accc8a69e6317ee43a53e093f2aef25b70ddff625cfa691d7df28e9bf6d94dc`  
		Last Modified: Fri, 25 Feb 2022 03:15:27 GMT  
		Size: 1.1 KB (1113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-alpine`

```console
$ docker pull nats@sha256:6944283c7d430ef4d5e23afb87b2a2d9faf963793bcd94b0461bc12def6c74c2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-alpine` - linux; amd64

```console
$ docker pull nats@sha256:6f8d631c068a9d37845ebee434d2c37606757634b9d8950e8de1035dc68842b4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7591453 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:775ec723ebf4c964b880457f54f66782e850e7121d3264c851da7d58cddb64bc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 24 Nov 2021 20:19:40 GMT
ADD file:9233f6f2237d79659a9521f7e390df217cec49f1a8aa3a12147bbca1956acdb9 in / 
# Wed, 24 Nov 2021 20:19:40 GMT
CMD ["/bin/sh"]
# Fri, 25 Feb 2022 02:21:01 GMT
ENV NATS_SERVER=2.7.3
# Fri, 25 Feb 2022 02:21:04 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='c895169ab34bc21442121f6c885905a254a9351a098402f319b3fbfd1e6225c9' ;; 		armhf) natsArch='arm6'; sha256='1b7e1c5835131825c4007766befd0c96a60edbcc3bc336a6739de5c8affea0c4' ;; 		armv7) natsArch='arm7'; sha256='723290467bc7e95b59ca7238a818932b199b00a21d4e3d7eb0e826b7aba2e0ea' ;; 		x86_64) natsArch='amd64'; sha256='2186c7660cd1d9774421614f6724ad32d7cec2389e39858f227a7991be41b1a7' ;; 		x86) natsArch='386'; sha256='3e8e2841921d555d06c67b1e33fc9bd934e4afec4748f7ddf27c67d707fafea4' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 25 Feb 2022 02:21:04 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 25 Feb 2022 02:21:04 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 25 Feb 2022 02:21:04 GMT
EXPOSE 4222 6222 8222
# Fri, 25 Feb 2022 02:21:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Feb 2022 02:21:05 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:59bf1c3509f33515622619af21ed55bbe26d24913cedbca106468a5fb37a50c3`  
		Last Modified: Wed, 24 Nov 2021 20:20:05 GMT  
		Size: 2.8 MB (2818413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfad251bce41e482876302125c33ef603e0ca99f33d1d274a09af07e1acd1be6`  
		Last Modified: Fri, 25 Feb 2022 02:21:40 GMT  
		Size: 4.8 MB (4772040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8c6f8e0dbab2106f703f51433a684cef43840e5e7443402b474f3c09144a4fe`  
		Last Modified: Fri, 25 Feb 2022 02:21:39 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0d8341c3c348e685617552e338228d15dd937ca0708bd7ab85c3c1b273ed88c`  
		Last Modified: Fri, 25 Feb 2022 02:21:39 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:d6f43ae04309c6115c32d1c71469973712b3e817088a449ce37a9e8cb6b86bf9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7071601 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:846b4c8922b69a90d198633a7b622da89348aa9e3f7f11f58a294e2c4b112a33`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 24 Nov 2021 21:08:16 GMT
ADD file:61137e0aa49ba06f57ac69466fe2fb116f580b5e6159d56f846b1d72c4a3c814 in / 
# Wed, 24 Nov 2021 21:08:16 GMT
CMD ["/bin/sh"]
# Fri, 25 Feb 2022 02:49:34 GMT
ENV NATS_SERVER=2.7.3
# Fri, 25 Feb 2022 02:49:38 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='c895169ab34bc21442121f6c885905a254a9351a098402f319b3fbfd1e6225c9' ;; 		armhf) natsArch='arm6'; sha256='1b7e1c5835131825c4007766befd0c96a60edbcc3bc336a6739de5c8affea0c4' ;; 		armv7) natsArch='arm7'; sha256='723290467bc7e95b59ca7238a818932b199b00a21d4e3d7eb0e826b7aba2e0ea' ;; 		x86_64) natsArch='amd64'; sha256='2186c7660cd1d9774421614f6724ad32d7cec2389e39858f227a7991be41b1a7' ;; 		x86) natsArch='386'; sha256='3e8e2841921d555d06c67b1e33fc9bd934e4afec4748f7ddf27c67d707fafea4' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 25 Feb 2022 02:49:38 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 25 Feb 2022 02:49:39 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 25 Feb 2022 02:49:39 GMT
EXPOSE 4222 6222 8222
# Fri, 25 Feb 2022 02:49:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Feb 2022 02:49:40 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:e4a43de54da9e309482f6762f0c11f5f547cd8fd61a49c5f158453066162023e`  
		Last Modified: Wed, 24 Nov 2021 21:09:46 GMT  
		Size: 2.6 MB (2631421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ecb484648e454aaf42c41938db64a0715cb509a90811b5912192d2e66a2f7fb`  
		Last Modified: Fri, 25 Feb 2022 02:51:52 GMT  
		Size: 4.4 MB (4439176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdd675987846849cf3247fbc41b25505410823bffd30e841e7f663936458e553`  
		Last Modified: Fri, 25 Feb 2022 02:51:49 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ae450e4bdcdcad0dc3e04a43f8855409627f6c7fdecd22f661dbfe3a99530d2`  
		Last Modified: Fri, 25 Feb 2022 02:51:49 GMT  
		Size: 417.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:665c6221a3c009747c340953834a8e1c6e38008d728f3a9d4d4eaab76e8e640d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.9 MB (6865015 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f23f21c3235ba9d61b53aeb161021b62412dc690dd81727439de14a1f9b902eb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 24 Nov 2021 21:42:11 GMT
ADD file:ca436da5b0bfc9c0e2fc685533c6628918000c8fff109fe9a8da625b9a798002 in / 
# Wed, 24 Nov 2021 21:42:11 GMT
CMD ["/bin/sh"]
# Fri, 25 Feb 2022 02:57:52 GMT
ENV NATS_SERVER=2.7.3
# Fri, 25 Feb 2022 02:57:56 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='c895169ab34bc21442121f6c885905a254a9351a098402f319b3fbfd1e6225c9' ;; 		armhf) natsArch='arm6'; sha256='1b7e1c5835131825c4007766befd0c96a60edbcc3bc336a6739de5c8affea0c4' ;; 		armv7) natsArch='arm7'; sha256='723290467bc7e95b59ca7238a818932b199b00a21d4e3d7eb0e826b7aba2e0ea' ;; 		x86_64) natsArch='amd64'; sha256='2186c7660cd1d9774421614f6724ad32d7cec2389e39858f227a7991be41b1a7' ;; 		x86) natsArch='386'; sha256='3e8e2841921d555d06c67b1e33fc9bd934e4afec4748f7ddf27c67d707fafea4' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 25 Feb 2022 02:57:57 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 25 Feb 2022 02:57:57 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 25 Feb 2022 02:57:58 GMT
EXPOSE 4222 6222 8222
# Fri, 25 Feb 2022 02:57:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Feb 2022 02:57:58 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:5480d2ca1740c20ce17652e01ed2265cdc914458acd41256a2b1ccff28f2762c`  
		Last Modified: Wed, 24 Nov 2021 21:43:40 GMT  
		Size: 2.4 MB (2434764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fafd4ba596baa033665a46ce765df0c4a928784832ecc5645944032cfcd9295`  
		Last Modified: Fri, 25 Feb 2022 03:00:20 GMT  
		Size: 4.4 MB (4429250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abb2edff52bc9250fdec4032d39728784d4495539ef65cceed401a8968ec2df5`  
		Last Modified: Fri, 25 Feb 2022 03:00:18 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1047f2aa448d4163e2995aed662d6890fdd3954289a1ff2908edc894450b3d78`  
		Last Modified: Fri, 25 Feb 2022 03:00:18 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:8f79d8af0b084884d2cc9641a33a1274022fc51b99e955d3f13d9c45f47cf6b4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7132810 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e50bb490b2ac0a89152a29fc28e269300b6b83d2a85c0ce5ebe74635c34cdb0d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 24 Nov 2021 20:39:20 GMT
ADD file:df53811312284306901fdaaff0a357a4bf40d631e662fe9ce6d342442e494b6c in / 
# Wed, 24 Nov 2021 20:39:20 GMT
CMD ["/bin/sh"]
# Fri, 25 Feb 2022 03:01:24 GMT
ENV NATS_SERVER=2.7.3
# Fri, 25 Feb 2022 03:01:26 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='c895169ab34bc21442121f6c885905a254a9351a098402f319b3fbfd1e6225c9' ;; 		armhf) natsArch='arm6'; sha256='1b7e1c5835131825c4007766befd0c96a60edbcc3bc336a6739de5c8affea0c4' ;; 		armv7) natsArch='arm7'; sha256='723290467bc7e95b59ca7238a818932b199b00a21d4e3d7eb0e826b7aba2e0ea' ;; 		x86_64) natsArch='amd64'; sha256='2186c7660cd1d9774421614f6724ad32d7cec2389e39858f227a7991be41b1a7' ;; 		x86) natsArch='386'; sha256='3e8e2841921d555d06c67b1e33fc9bd934e4afec4748f7ddf27c67d707fafea4' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 25 Feb 2022 03:01:28 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 25 Feb 2022 03:01:29 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 25 Feb 2022 03:01:29 GMT
EXPOSE 4222 6222 8222
# Fri, 25 Feb 2022 03:01:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Feb 2022 03:01:31 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9b3977197b4f2147bdd31e1271f811319dcd5c2fc595f14e81f5351ab6275b99`  
		Last Modified: Wed, 24 Nov 2021 20:39:59 GMT  
		Size: 2.7 MB (2715434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c75ed4d21bde940c8f5b4d0d82b44c31489bd5a37d46b1f197b7d1baed0b6e8`  
		Last Modified: Fri, 25 Feb 2022 03:02:31 GMT  
		Size: 4.4 MB (4416403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f7dd0d82f2c731b21df156c69326c651274a35eb010b23b5150397309110717`  
		Last Modified: Fri, 25 Feb 2022 03:02:30 GMT  
		Size: 559.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f29d0f81d7bbfb90bc5607be41aabbd3e970b1e74e19a069c23e863092772ba`  
		Last Modified: Fri, 25 Feb 2022 03:02:30 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-alpine3.15`

```console
$ docker pull nats@sha256:6944283c7d430ef4d5e23afb87b2a2d9faf963793bcd94b0461bc12def6c74c2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-alpine3.15` - linux; amd64

```console
$ docker pull nats@sha256:6f8d631c068a9d37845ebee434d2c37606757634b9d8950e8de1035dc68842b4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7591453 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:775ec723ebf4c964b880457f54f66782e850e7121d3264c851da7d58cddb64bc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 24 Nov 2021 20:19:40 GMT
ADD file:9233f6f2237d79659a9521f7e390df217cec49f1a8aa3a12147bbca1956acdb9 in / 
# Wed, 24 Nov 2021 20:19:40 GMT
CMD ["/bin/sh"]
# Fri, 25 Feb 2022 02:21:01 GMT
ENV NATS_SERVER=2.7.3
# Fri, 25 Feb 2022 02:21:04 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='c895169ab34bc21442121f6c885905a254a9351a098402f319b3fbfd1e6225c9' ;; 		armhf) natsArch='arm6'; sha256='1b7e1c5835131825c4007766befd0c96a60edbcc3bc336a6739de5c8affea0c4' ;; 		armv7) natsArch='arm7'; sha256='723290467bc7e95b59ca7238a818932b199b00a21d4e3d7eb0e826b7aba2e0ea' ;; 		x86_64) natsArch='amd64'; sha256='2186c7660cd1d9774421614f6724ad32d7cec2389e39858f227a7991be41b1a7' ;; 		x86) natsArch='386'; sha256='3e8e2841921d555d06c67b1e33fc9bd934e4afec4748f7ddf27c67d707fafea4' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 25 Feb 2022 02:21:04 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 25 Feb 2022 02:21:04 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 25 Feb 2022 02:21:04 GMT
EXPOSE 4222 6222 8222
# Fri, 25 Feb 2022 02:21:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Feb 2022 02:21:05 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:59bf1c3509f33515622619af21ed55bbe26d24913cedbca106468a5fb37a50c3`  
		Last Modified: Wed, 24 Nov 2021 20:20:05 GMT  
		Size: 2.8 MB (2818413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfad251bce41e482876302125c33ef603e0ca99f33d1d274a09af07e1acd1be6`  
		Last Modified: Fri, 25 Feb 2022 02:21:40 GMT  
		Size: 4.8 MB (4772040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8c6f8e0dbab2106f703f51433a684cef43840e5e7443402b474f3c09144a4fe`  
		Last Modified: Fri, 25 Feb 2022 02:21:39 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0d8341c3c348e685617552e338228d15dd937ca0708bd7ab85c3c1b273ed88c`  
		Last Modified: Fri, 25 Feb 2022 02:21:39 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.15` - linux; arm variant v6

```console
$ docker pull nats@sha256:d6f43ae04309c6115c32d1c71469973712b3e817088a449ce37a9e8cb6b86bf9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7071601 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:846b4c8922b69a90d198633a7b622da89348aa9e3f7f11f58a294e2c4b112a33`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 24 Nov 2021 21:08:16 GMT
ADD file:61137e0aa49ba06f57ac69466fe2fb116f580b5e6159d56f846b1d72c4a3c814 in / 
# Wed, 24 Nov 2021 21:08:16 GMT
CMD ["/bin/sh"]
# Fri, 25 Feb 2022 02:49:34 GMT
ENV NATS_SERVER=2.7.3
# Fri, 25 Feb 2022 02:49:38 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='c895169ab34bc21442121f6c885905a254a9351a098402f319b3fbfd1e6225c9' ;; 		armhf) natsArch='arm6'; sha256='1b7e1c5835131825c4007766befd0c96a60edbcc3bc336a6739de5c8affea0c4' ;; 		armv7) natsArch='arm7'; sha256='723290467bc7e95b59ca7238a818932b199b00a21d4e3d7eb0e826b7aba2e0ea' ;; 		x86_64) natsArch='amd64'; sha256='2186c7660cd1d9774421614f6724ad32d7cec2389e39858f227a7991be41b1a7' ;; 		x86) natsArch='386'; sha256='3e8e2841921d555d06c67b1e33fc9bd934e4afec4748f7ddf27c67d707fafea4' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 25 Feb 2022 02:49:38 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 25 Feb 2022 02:49:39 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 25 Feb 2022 02:49:39 GMT
EXPOSE 4222 6222 8222
# Fri, 25 Feb 2022 02:49:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Feb 2022 02:49:40 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:e4a43de54da9e309482f6762f0c11f5f547cd8fd61a49c5f158453066162023e`  
		Last Modified: Wed, 24 Nov 2021 21:09:46 GMT  
		Size: 2.6 MB (2631421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ecb484648e454aaf42c41938db64a0715cb509a90811b5912192d2e66a2f7fb`  
		Last Modified: Fri, 25 Feb 2022 02:51:52 GMT  
		Size: 4.4 MB (4439176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdd675987846849cf3247fbc41b25505410823bffd30e841e7f663936458e553`  
		Last Modified: Fri, 25 Feb 2022 02:51:49 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ae450e4bdcdcad0dc3e04a43f8855409627f6c7fdecd22f661dbfe3a99530d2`  
		Last Modified: Fri, 25 Feb 2022 02:51:49 GMT  
		Size: 417.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.15` - linux; arm variant v7

```console
$ docker pull nats@sha256:665c6221a3c009747c340953834a8e1c6e38008d728f3a9d4d4eaab76e8e640d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.9 MB (6865015 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f23f21c3235ba9d61b53aeb161021b62412dc690dd81727439de14a1f9b902eb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 24 Nov 2021 21:42:11 GMT
ADD file:ca436da5b0bfc9c0e2fc685533c6628918000c8fff109fe9a8da625b9a798002 in / 
# Wed, 24 Nov 2021 21:42:11 GMT
CMD ["/bin/sh"]
# Fri, 25 Feb 2022 02:57:52 GMT
ENV NATS_SERVER=2.7.3
# Fri, 25 Feb 2022 02:57:56 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='c895169ab34bc21442121f6c885905a254a9351a098402f319b3fbfd1e6225c9' ;; 		armhf) natsArch='arm6'; sha256='1b7e1c5835131825c4007766befd0c96a60edbcc3bc336a6739de5c8affea0c4' ;; 		armv7) natsArch='arm7'; sha256='723290467bc7e95b59ca7238a818932b199b00a21d4e3d7eb0e826b7aba2e0ea' ;; 		x86_64) natsArch='amd64'; sha256='2186c7660cd1d9774421614f6724ad32d7cec2389e39858f227a7991be41b1a7' ;; 		x86) natsArch='386'; sha256='3e8e2841921d555d06c67b1e33fc9bd934e4afec4748f7ddf27c67d707fafea4' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 25 Feb 2022 02:57:57 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 25 Feb 2022 02:57:57 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 25 Feb 2022 02:57:58 GMT
EXPOSE 4222 6222 8222
# Fri, 25 Feb 2022 02:57:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Feb 2022 02:57:58 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:5480d2ca1740c20ce17652e01ed2265cdc914458acd41256a2b1ccff28f2762c`  
		Last Modified: Wed, 24 Nov 2021 21:43:40 GMT  
		Size: 2.4 MB (2434764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fafd4ba596baa033665a46ce765df0c4a928784832ecc5645944032cfcd9295`  
		Last Modified: Fri, 25 Feb 2022 03:00:20 GMT  
		Size: 4.4 MB (4429250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abb2edff52bc9250fdec4032d39728784d4495539ef65cceed401a8968ec2df5`  
		Last Modified: Fri, 25 Feb 2022 03:00:18 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1047f2aa448d4163e2995aed662d6890fdd3954289a1ff2908edc894450b3d78`  
		Last Modified: Fri, 25 Feb 2022 03:00:18 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.15` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:8f79d8af0b084884d2cc9641a33a1274022fc51b99e955d3f13d9c45f47cf6b4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7132810 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e50bb490b2ac0a89152a29fc28e269300b6b83d2a85c0ce5ebe74635c34cdb0d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 24 Nov 2021 20:39:20 GMT
ADD file:df53811312284306901fdaaff0a357a4bf40d631e662fe9ce6d342442e494b6c in / 
# Wed, 24 Nov 2021 20:39:20 GMT
CMD ["/bin/sh"]
# Fri, 25 Feb 2022 03:01:24 GMT
ENV NATS_SERVER=2.7.3
# Fri, 25 Feb 2022 03:01:26 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='c895169ab34bc21442121f6c885905a254a9351a098402f319b3fbfd1e6225c9' ;; 		armhf) natsArch='arm6'; sha256='1b7e1c5835131825c4007766befd0c96a60edbcc3bc336a6739de5c8affea0c4' ;; 		armv7) natsArch='arm7'; sha256='723290467bc7e95b59ca7238a818932b199b00a21d4e3d7eb0e826b7aba2e0ea' ;; 		x86_64) natsArch='amd64'; sha256='2186c7660cd1d9774421614f6724ad32d7cec2389e39858f227a7991be41b1a7' ;; 		x86) natsArch='386'; sha256='3e8e2841921d555d06c67b1e33fc9bd934e4afec4748f7ddf27c67d707fafea4' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 25 Feb 2022 03:01:28 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 25 Feb 2022 03:01:29 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 25 Feb 2022 03:01:29 GMT
EXPOSE 4222 6222 8222
# Fri, 25 Feb 2022 03:01:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Feb 2022 03:01:31 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9b3977197b4f2147bdd31e1271f811319dcd5c2fc595f14e81f5351ab6275b99`  
		Last Modified: Wed, 24 Nov 2021 20:39:59 GMT  
		Size: 2.7 MB (2715434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c75ed4d21bde940c8f5b4d0d82b44c31489bd5a37d46b1f197b7d1baed0b6e8`  
		Last Modified: Fri, 25 Feb 2022 03:02:31 GMT  
		Size: 4.4 MB (4416403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f7dd0d82f2c731b21df156c69326c651274a35eb010b23b5150397309110717`  
		Last Modified: Fri, 25 Feb 2022 03:02:30 GMT  
		Size: 559.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f29d0f81d7bbfb90bc5607be41aabbd3e970b1e74e19a069c23e863092772ba`  
		Last Modified: Fri, 25 Feb 2022 03:02:30 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-linux`

```console
$ docker pull nats@sha256:4fe2c16e211795858e7e7538197ec57f67ed6e9ca5d91d06d925e09ec6724d3b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-linux` - linux; amd64

```console
$ docker pull nats@sha256:5fd249efa75cf3eb595342175207fdbb390eee3034f7fe49355d7a479fa3ffe2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4499407 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c84de17b17b3458d2b6e6d4264ea6186c82bab718ca058f5d7738e53ca2759ac`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 25 Feb 2022 02:21:13 GMT
COPY file:8a814b0c66a47e63e5a7f4287478948812fe6e03c224d539f37ce3f950d2b6c6 in /nats-server 
# Fri, 25 Feb 2022 02:21:13 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 25 Feb 2022 02:21:14 GMT
EXPOSE 4222 6222 8222
# Fri, 25 Feb 2022 02:21:14 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 25 Feb 2022 02:21:14 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:277fae1baf41821774f7a2e1c3f465b28aa8693ee0cd77e0ad0bace55d9c616e`  
		Last Modified: Fri, 25 Feb 2022 02:22:04 GMT  
		Size: 4.5 MB (4498900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb932b4b3fbc873b56e996c6357055bb7700c701d17d7d87cdec31211142b49a`  
		Last Modified: Fri, 25 Feb 2022 02:22:03 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:2e3339e7e8d98e7bbab0613c7b7c3dd6f51fcf33ed3910a2e65e62fba7049337
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4165977 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ddc7bcc78dd550ace4def82e3db227e618d77e136274749f3bf55869e64be264`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 25 Feb 2022 02:50:06 GMT
COPY file:3a951d885f7bcec693f6fbf26a9ffd82b0c6218b6834fc6053e5812f7451b63e in /nats-server 
# Fri, 25 Feb 2022 02:50:06 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 25 Feb 2022 02:50:07 GMT
EXPOSE 4222 6222 8222
# Fri, 25 Feb 2022 02:50:07 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 25 Feb 2022 02:50:07 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:f6de87b4530f922b11edc08be8edeebc6ce0cb666907013348d4e1b9f5d51809`  
		Last Modified: Fri, 25 Feb 2022 02:52:29 GMT  
		Size: 4.2 MB (4165468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5fa68b52226484e5870677184cdc47c93a7d453f334c144b5cb631346bc8111`  
		Last Modified: Fri, 25 Feb 2022 02:52:27 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:87cf3f8e33ebf28f35575ea083f8feb460d19fa9380d2622c82567ff3fa9d840
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4157918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4eef99b95e572b23f90d60e6e157be90b05ab2f35dbcb10f83f96ece551945a`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 25 Feb 2022 02:58:34 GMT
COPY file:3ee879939ad264e803dd4d6072181d968c4dd0fe076115159f70479c6309ef45 in /nats-server 
# Fri, 25 Feb 2022 02:58:34 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 25 Feb 2022 02:58:35 GMT
EXPOSE 4222 6222 8222
# Fri, 25 Feb 2022 02:58:35 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 25 Feb 2022 02:58:36 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:67a3d8907097b9caffd9d1720b4fb2b1d2ac9dfda60a1d169abbf5494323d50a`  
		Last Modified: Fri, 25 Feb 2022 03:00:58 GMT  
		Size: 4.2 MB (4157409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73f5577f4846f032b281220b897161962481198ead0a1b9ad1d7c76cdd989747`  
		Last Modified: Fri, 25 Feb 2022 03:00:55 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:e970861a260709ae1e8c892eb36758c14323e81959ff4aaa1e9b7327b91d3e70
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.1 MB (4143805 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4414e48026697a15338f28dcb8e46ace9627ea7332559e1708f36ce62a5e327`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 25 Feb 2022 03:01:42 GMT
COPY file:acd11e9a3a86f6f3da079c5155851337e747c3b31481ec05e2dd1e48e23becb2 in /nats-server 
# Fri, 25 Feb 2022 03:01:43 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 25 Feb 2022 03:01:43 GMT
EXPOSE 4222 6222 8222
# Fri, 25 Feb 2022 03:01:44 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 25 Feb 2022 03:01:45 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6ad9fd47af885b43442590ad2c8171e4b4899caef84921ec73ba0540b9c03284`  
		Last Modified: Fri, 25 Feb 2022 03:02:59 GMT  
		Size: 4.1 MB (4143299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02d7667f81936503f26a5ed657cfffdc9add626da8ae5bb78d691054cd3af7c3`  
		Last Modified: Fri, 25 Feb 2022 03:02:59 GMT  
		Size: 506.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-nanoserver`

```console
$ docker pull nats@sha256:6e43eecf010598596b218f3800a6d052426d875695ead9cdbf074e0653772142
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2565; amd64

### `nats:2-nanoserver` - windows version 10.0.17763.2565; amd64

```console
$ docker pull nats@sha256:d7c795020fd7295382d503ba883e23cf34ca9c53d6e6b91184bc1fd2bb2c990d
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.6 MB (107634881 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6e99776e94a148ebda875656d07e673c65aedb583986faedb3bdc61a2fd7759`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 02 Feb 2022 19:06:51 GMT
RUN Apply image 1809-amd64
# Wed, 09 Feb 2022 18:13:36 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 25 Feb 2022 02:17:30 GMT
RUN cmd /S /C #(nop) COPY file:d5609a37f534b519fa4326428362ea5398f7165ee90493fb7bdc8b810da33b0e in C:\nats-server.exe 
# Fri, 25 Feb 2022 02:17:31 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Fri, 25 Feb 2022 02:17:32 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Fri, 25 Feb 2022 02:17:33 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 25 Feb 2022 02:17:34 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:bd0b37167cd3d731eb15196e123df7156b5a35597874d3016a1a4298c46fac3f`  
		Size: 103.1 MB (103087119 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8bc49c59cde14e3a9ed8fedce001c00fcb5fe0f9b914aa07273e04f23333d180`  
		Last Modified: Wed, 09 Feb 2022 18:14:28 GMT  
		Size: 1.1 KB (1138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b682f8d539489225b7a3859570b80452b497086f57fa4e6908f2b99d213e1a03`  
		Last Modified: Fri, 25 Feb 2022 03:15:32 GMT  
		Size: 4.5 MB (4541735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67997158a056ea601aec06de195ce0251264a6d8d071f8a44a49a545865ce426`  
		Last Modified: Fri, 25 Feb 2022 03:15:27 GMT  
		Size: 1.7 KB (1656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f873036aacce9bbc35378d6a36985e62919c6d2c9ff526011564a861b86240ab`  
		Last Modified: Fri, 25 Feb 2022 03:15:27 GMT  
		Size: 1.0 KB (1039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf1eace4b7f44dce795499001f62baee27fb477865e490b11d05d198c8e80550`  
		Last Modified: Fri, 25 Feb 2022 03:15:27 GMT  
		Size: 1.1 KB (1081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8accc8a69e6317ee43a53e093f2aef25b70ddff625cfa691d7df28e9bf6d94dc`  
		Last Modified: Fri, 25 Feb 2022 03:15:27 GMT  
		Size: 1.1 KB (1113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-nanoserver-1809`

```console
$ docker pull nats@sha256:6e43eecf010598596b218f3800a6d052426d875695ead9cdbf074e0653772142
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2565; amd64

### `nats:2-nanoserver-1809` - windows version 10.0.17763.2565; amd64

```console
$ docker pull nats@sha256:d7c795020fd7295382d503ba883e23cf34ca9c53d6e6b91184bc1fd2bb2c990d
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.6 MB (107634881 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6e99776e94a148ebda875656d07e673c65aedb583986faedb3bdc61a2fd7759`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 02 Feb 2022 19:06:51 GMT
RUN Apply image 1809-amd64
# Wed, 09 Feb 2022 18:13:36 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 25 Feb 2022 02:17:30 GMT
RUN cmd /S /C #(nop) COPY file:d5609a37f534b519fa4326428362ea5398f7165ee90493fb7bdc8b810da33b0e in C:\nats-server.exe 
# Fri, 25 Feb 2022 02:17:31 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Fri, 25 Feb 2022 02:17:32 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Fri, 25 Feb 2022 02:17:33 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 25 Feb 2022 02:17:34 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:bd0b37167cd3d731eb15196e123df7156b5a35597874d3016a1a4298c46fac3f`  
		Size: 103.1 MB (103087119 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8bc49c59cde14e3a9ed8fedce001c00fcb5fe0f9b914aa07273e04f23333d180`  
		Last Modified: Wed, 09 Feb 2022 18:14:28 GMT  
		Size: 1.1 KB (1138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b682f8d539489225b7a3859570b80452b497086f57fa4e6908f2b99d213e1a03`  
		Last Modified: Fri, 25 Feb 2022 03:15:32 GMT  
		Size: 4.5 MB (4541735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67997158a056ea601aec06de195ce0251264a6d8d071f8a44a49a545865ce426`  
		Last Modified: Fri, 25 Feb 2022 03:15:27 GMT  
		Size: 1.7 KB (1656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f873036aacce9bbc35378d6a36985e62919c6d2c9ff526011564a861b86240ab`  
		Last Modified: Fri, 25 Feb 2022 03:15:27 GMT  
		Size: 1.0 KB (1039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf1eace4b7f44dce795499001f62baee27fb477865e490b11d05d198c8e80550`  
		Last Modified: Fri, 25 Feb 2022 03:15:27 GMT  
		Size: 1.1 KB (1081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8accc8a69e6317ee43a53e093f2aef25b70ddff625cfa691d7df28e9bf6d94dc`  
		Last Modified: Fri, 25 Feb 2022 03:15:27 GMT  
		Size: 1.1 KB (1113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-scratch`

```console
$ docker pull nats@sha256:4fe2c16e211795858e7e7538197ec57f67ed6e9ca5d91d06d925e09ec6724d3b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-scratch` - linux; amd64

```console
$ docker pull nats@sha256:5fd249efa75cf3eb595342175207fdbb390eee3034f7fe49355d7a479fa3ffe2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4499407 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c84de17b17b3458d2b6e6d4264ea6186c82bab718ca058f5d7738e53ca2759ac`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 25 Feb 2022 02:21:13 GMT
COPY file:8a814b0c66a47e63e5a7f4287478948812fe6e03c224d539f37ce3f950d2b6c6 in /nats-server 
# Fri, 25 Feb 2022 02:21:13 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 25 Feb 2022 02:21:14 GMT
EXPOSE 4222 6222 8222
# Fri, 25 Feb 2022 02:21:14 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 25 Feb 2022 02:21:14 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:277fae1baf41821774f7a2e1c3f465b28aa8693ee0cd77e0ad0bace55d9c616e`  
		Last Modified: Fri, 25 Feb 2022 02:22:04 GMT  
		Size: 4.5 MB (4498900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb932b4b3fbc873b56e996c6357055bb7700c701d17d7d87cdec31211142b49a`  
		Last Modified: Fri, 25 Feb 2022 02:22:03 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:2e3339e7e8d98e7bbab0613c7b7c3dd6f51fcf33ed3910a2e65e62fba7049337
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4165977 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ddc7bcc78dd550ace4def82e3db227e618d77e136274749f3bf55869e64be264`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 25 Feb 2022 02:50:06 GMT
COPY file:3a951d885f7bcec693f6fbf26a9ffd82b0c6218b6834fc6053e5812f7451b63e in /nats-server 
# Fri, 25 Feb 2022 02:50:06 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 25 Feb 2022 02:50:07 GMT
EXPOSE 4222 6222 8222
# Fri, 25 Feb 2022 02:50:07 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 25 Feb 2022 02:50:07 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:f6de87b4530f922b11edc08be8edeebc6ce0cb666907013348d4e1b9f5d51809`  
		Last Modified: Fri, 25 Feb 2022 02:52:29 GMT  
		Size: 4.2 MB (4165468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5fa68b52226484e5870677184cdc47c93a7d453f334c144b5cb631346bc8111`  
		Last Modified: Fri, 25 Feb 2022 02:52:27 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:87cf3f8e33ebf28f35575ea083f8feb460d19fa9380d2622c82567ff3fa9d840
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4157918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4eef99b95e572b23f90d60e6e157be90b05ab2f35dbcb10f83f96ece551945a`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 25 Feb 2022 02:58:34 GMT
COPY file:3ee879939ad264e803dd4d6072181d968c4dd0fe076115159f70479c6309ef45 in /nats-server 
# Fri, 25 Feb 2022 02:58:34 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 25 Feb 2022 02:58:35 GMT
EXPOSE 4222 6222 8222
# Fri, 25 Feb 2022 02:58:35 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 25 Feb 2022 02:58:36 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:67a3d8907097b9caffd9d1720b4fb2b1d2ac9dfda60a1d169abbf5494323d50a`  
		Last Modified: Fri, 25 Feb 2022 03:00:58 GMT  
		Size: 4.2 MB (4157409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73f5577f4846f032b281220b897161962481198ead0a1b9ad1d7c76cdd989747`  
		Last Modified: Fri, 25 Feb 2022 03:00:55 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:e970861a260709ae1e8c892eb36758c14323e81959ff4aaa1e9b7327b91d3e70
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.1 MB (4143805 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4414e48026697a15338f28dcb8e46ace9627ea7332559e1708f36ce62a5e327`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 25 Feb 2022 03:01:42 GMT
COPY file:acd11e9a3a86f6f3da079c5155851337e747c3b31481ec05e2dd1e48e23becb2 in /nats-server 
# Fri, 25 Feb 2022 03:01:43 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 25 Feb 2022 03:01:43 GMT
EXPOSE 4222 6222 8222
# Fri, 25 Feb 2022 03:01:44 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 25 Feb 2022 03:01:45 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6ad9fd47af885b43442590ad2c8171e4b4899caef84921ec73ba0540b9c03284`  
		Last Modified: Fri, 25 Feb 2022 03:02:59 GMT  
		Size: 4.1 MB (4143299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02d7667f81936503f26a5ed657cfffdc9add626da8ae5bb78d691054cd3af7c3`  
		Last Modified: Fri, 25 Feb 2022 03:02:59 GMT  
		Size: 506.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-windowsservercore`

```console
$ docker pull nats@sha256:2b9c20408baf29df9d8666fc894d8a5c308946331d4310ef5a82b1eed5101db3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2565; amd64

### `nats:2-windowsservercore` - windows version 10.0.17763.2565; amd64

```console
$ docker pull nats@sha256:ac025e7ac0a2786f5807888399f94d317a0636b60e8a37584569d586fb1ac146
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2718991955 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:007419288bb7b16cd78d29d0476687df2d88011775f13b3f565c92414a214c05`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Wed, 02 Feb 2022 19:28:56 GMT
RUN Install update 1809-amd64
# Wed, 09 Feb 2022 15:04:17 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Feb 2022 18:10:54 GMT
ENV NATS_DOCKERIZED=1
# Fri, 25 Feb 2022 02:14:46 GMT
ENV NATS_SERVER=2.7.3
# Fri, 25 Feb 2022 02:14:47 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.7.3/nats-server-v2.7.3-windows-amd64.zip
# Fri, 25 Feb 2022 02:14:48 GMT
ENV NATS_SERVER_SHASUM=ddb372da68741d897006c8d4b160c7f4788603cbaacb3fa105ddf7baada04428
# Fri, 25 Feb 2022 02:15:50 GMT
RUN Set-PSDebug -Trace 2
# Fri, 25 Feb 2022 02:17:14 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 25 Feb 2022 02:17:16 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Fri, 25 Feb 2022 02:17:17 GMT
EXPOSE 4222 6222 8222
# Fri, 25 Feb 2022 02:17:18 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 25 Feb 2022 02:17:19 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:1bd78008c728d8f9e56dc2093e6eb55f0f0b1aa96e5d0c7ccc830c5f60876cdf`  
		Size: 995.4 MB (995381853 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f49d3791198cf2ea875fd54ce3bb715670742d4a58c00252395ad1b74036662a`  
		Last Modified: Wed, 09 Feb 2022 16:39:51 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4235aeeb4e8b577cc7aa26c7994ec94c94dd53a38764fc510b330b77cef4abad`  
		Last Modified: Wed, 09 Feb 2022 18:14:09 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6ed63a799d34b3a151eb2d65afc4a93d028c5308ce305f9059da19083ea4579`  
		Last Modified: Fri, 25 Feb 2022 03:15:11 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fa36020fa0fadcfe9ac785f1bc4cbf6e51ac336a4441d2ea628465f9f1e3832`  
		Last Modified: Fri, 25 Feb 2022 03:15:11 GMT  
		Size: 1.3 KB (1321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58aaa8ed102560150d8bd4fe887000c2789a69df5ae550a8b8058e526d01af34`  
		Last Modified: Fri, 25 Feb 2022 03:15:11 GMT  
		Size: 1.3 KB (1300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e48afd20cc6576c9f831f4166f86f4cd65be8140eda5a57159bba0d62c21b1af`  
		Last Modified: Fri, 25 Feb 2022 03:15:12 GMT  
		Size: 374.3 KB (374309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1eb76be5e45618d5a45f4672ac8e8c8d45d10bf627dc47f3afe45c7909b223b`  
		Last Modified: Fri, 25 Feb 2022 03:15:10 GMT  
		Size: 4.9 MB (4890363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:513928aafbffc4a16807de347507df4019d3096da02f3475f8731f6704a0e75d`  
		Last Modified: Fri, 25 Feb 2022 03:15:09 GMT  
		Size: 1.9 KB (1884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6ba5e5368daffd340a50b6715a6d9d28d2f2c341d694c5d7cdae52e15e46d4d`  
		Last Modified: Fri, 25 Feb 2022 03:15:09 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca864d6530840f9fbdc99b6aaedcd8aa7acf319697677ca480fd220d426cb62f`  
		Last Modified: Fri, 25 Feb 2022 03:15:09 GMT  
		Size: 1.3 KB (1322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e9cb037cabf38f35bdcf375e13b7790bfdc9b4e9761cd2e865cf557a7575e81`  
		Last Modified: Fri, 25 Feb 2022 03:15:09 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-windowsservercore-1809`

```console
$ docker pull nats@sha256:2b9c20408baf29df9d8666fc894d8a5c308946331d4310ef5a82b1eed5101db3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2565; amd64

### `nats:2-windowsservercore-1809` - windows version 10.0.17763.2565; amd64

```console
$ docker pull nats@sha256:ac025e7ac0a2786f5807888399f94d317a0636b60e8a37584569d586fb1ac146
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2718991955 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:007419288bb7b16cd78d29d0476687df2d88011775f13b3f565c92414a214c05`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Wed, 02 Feb 2022 19:28:56 GMT
RUN Install update 1809-amd64
# Wed, 09 Feb 2022 15:04:17 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Feb 2022 18:10:54 GMT
ENV NATS_DOCKERIZED=1
# Fri, 25 Feb 2022 02:14:46 GMT
ENV NATS_SERVER=2.7.3
# Fri, 25 Feb 2022 02:14:47 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.7.3/nats-server-v2.7.3-windows-amd64.zip
# Fri, 25 Feb 2022 02:14:48 GMT
ENV NATS_SERVER_SHASUM=ddb372da68741d897006c8d4b160c7f4788603cbaacb3fa105ddf7baada04428
# Fri, 25 Feb 2022 02:15:50 GMT
RUN Set-PSDebug -Trace 2
# Fri, 25 Feb 2022 02:17:14 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 25 Feb 2022 02:17:16 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Fri, 25 Feb 2022 02:17:17 GMT
EXPOSE 4222 6222 8222
# Fri, 25 Feb 2022 02:17:18 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 25 Feb 2022 02:17:19 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:1bd78008c728d8f9e56dc2093e6eb55f0f0b1aa96e5d0c7ccc830c5f60876cdf`  
		Size: 995.4 MB (995381853 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f49d3791198cf2ea875fd54ce3bb715670742d4a58c00252395ad1b74036662a`  
		Last Modified: Wed, 09 Feb 2022 16:39:51 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4235aeeb4e8b577cc7aa26c7994ec94c94dd53a38764fc510b330b77cef4abad`  
		Last Modified: Wed, 09 Feb 2022 18:14:09 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6ed63a799d34b3a151eb2d65afc4a93d028c5308ce305f9059da19083ea4579`  
		Last Modified: Fri, 25 Feb 2022 03:15:11 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fa36020fa0fadcfe9ac785f1bc4cbf6e51ac336a4441d2ea628465f9f1e3832`  
		Last Modified: Fri, 25 Feb 2022 03:15:11 GMT  
		Size: 1.3 KB (1321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58aaa8ed102560150d8bd4fe887000c2789a69df5ae550a8b8058e526d01af34`  
		Last Modified: Fri, 25 Feb 2022 03:15:11 GMT  
		Size: 1.3 KB (1300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e48afd20cc6576c9f831f4166f86f4cd65be8140eda5a57159bba0d62c21b1af`  
		Last Modified: Fri, 25 Feb 2022 03:15:12 GMT  
		Size: 374.3 KB (374309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1eb76be5e45618d5a45f4672ac8e8c8d45d10bf627dc47f3afe45c7909b223b`  
		Last Modified: Fri, 25 Feb 2022 03:15:10 GMT  
		Size: 4.9 MB (4890363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:513928aafbffc4a16807de347507df4019d3096da02f3475f8731f6704a0e75d`  
		Last Modified: Fri, 25 Feb 2022 03:15:09 GMT  
		Size: 1.9 KB (1884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6ba5e5368daffd340a50b6715a6d9d28d2f2c341d694c5d7cdae52e15e46d4d`  
		Last Modified: Fri, 25 Feb 2022 03:15:09 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca864d6530840f9fbdc99b6aaedcd8aa7acf319697677ca480fd220d426cb62f`  
		Last Modified: Fri, 25 Feb 2022 03:15:09 GMT  
		Size: 1.3 KB (1322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e9cb037cabf38f35bdcf375e13b7790bfdc9b4e9761cd2e865cf557a7575e81`  
		Last Modified: Fri, 25 Feb 2022 03:15:09 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.7`

```console
$ docker pull nats@sha256:4fa6d62e36bac738598e6523bb2185b0d57de021331057a538765f518cfd505a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.2565; amd64

### `nats:2.7` - linux; amd64

```console
$ docker pull nats@sha256:5fd249efa75cf3eb595342175207fdbb390eee3034f7fe49355d7a479fa3ffe2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4499407 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c84de17b17b3458d2b6e6d4264ea6186c82bab718ca058f5d7738e53ca2759ac`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 25 Feb 2022 02:21:13 GMT
COPY file:8a814b0c66a47e63e5a7f4287478948812fe6e03c224d539f37ce3f950d2b6c6 in /nats-server 
# Fri, 25 Feb 2022 02:21:13 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 25 Feb 2022 02:21:14 GMT
EXPOSE 4222 6222 8222
# Fri, 25 Feb 2022 02:21:14 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 25 Feb 2022 02:21:14 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:277fae1baf41821774f7a2e1c3f465b28aa8693ee0cd77e0ad0bace55d9c616e`  
		Last Modified: Fri, 25 Feb 2022 02:22:04 GMT  
		Size: 4.5 MB (4498900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb932b4b3fbc873b56e996c6357055bb7700c701d17d7d87cdec31211142b49a`  
		Last Modified: Fri, 25 Feb 2022 02:22:03 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.7` - linux; arm variant v6

```console
$ docker pull nats@sha256:2e3339e7e8d98e7bbab0613c7b7c3dd6f51fcf33ed3910a2e65e62fba7049337
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4165977 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ddc7bcc78dd550ace4def82e3db227e618d77e136274749f3bf55869e64be264`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 25 Feb 2022 02:50:06 GMT
COPY file:3a951d885f7bcec693f6fbf26a9ffd82b0c6218b6834fc6053e5812f7451b63e in /nats-server 
# Fri, 25 Feb 2022 02:50:06 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 25 Feb 2022 02:50:07 GMT
EXPOSE 4222 6222 8222
# Fri, 25 Feb 2022 02:50:07 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 25 Feb 2022 02:50:07 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:f6de87b4530f922b11edc08be8edeebc6ce0cb666907013348d4e1b9f5d51809`  
		Last Modified: Fri, 25 Feb 2022 02:52:29 GMT  
		Size: 4.2 MB (4165468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5fa68b52226484e5870677184cdc47c93a7d453f334c144b5cb631346bc8111`  
		Last Modified: Fri, 25 Feb 2022 02:52:27 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.7` - linux; arm variant v7

```console
$ docker pull nats@sha256:87cf3f8e33ebf28f35575ea083f8feb460d19fa9380d2622c82567ff3fa9d840
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4157918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4eef99b95e572b23f90d60e6e157be90b05ab2f35dbcb10f83f96ece551945a`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 25 Feb 2022 02:58:34 GMT
COPY file:3ee879939ad264e803dd4d6072181d968c4dd0fe076115159f70479c6309ef45 in /nats-server 
# Fri, 25 Feb 2022 02:58:34 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 25 Feb 2022 02:58:35 GMT
EXPOSE 4222 6222 8222
# Fri, 25 Feb 2022 02:58:35 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 25 Feb 2022 02:58:36 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:67a3d8907097b9caffd9d1720b4fb2b1d2ac9dfda60a1d169abbf5494323d50a`  
		Last Modified: Fri, 25 Feb 2022 03:00:58 GMT  
		Size: 4.2 MB (4157409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73f5577f4846f032b281220b897161962481198ead0a1b9ad1d7c76cdd989747`  
		Last Modified: Fri, 25 Feb 2022 03:00:55 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.7` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:e970861a260709ae1e8c892eb36758c14323e81959ff4aaa1e9b7327b91d3e70
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.1 MB (4143805 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4414e48026697a15338f28dcb8e46ace9627ea7332559e1708f36ce62a5e327`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 25 Feb 2022 03:01:42 GMT
COPY file:acd11e9a3a86f6f3da079c5155851337e747c3b31481ec05e2dd1e48e23becb2 in /nats-server 
# Fri, 25 Feb 2022 03:01:43 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 25 Feb 2022 03:01:43 GMT
EXPOSE 4222 6222 8222
# Fri, 25 Feb 2022 03:01:44 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 25 Feb 2022 03:01:45 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6ad9fd47af885b43442590ad2c8171e4b4899caef84921ec73ba0540b9c03284`  
		Last Modified: Fri, 25 Feb 2022 03:02:59 GMT  
		Size: 4.1 MB (4143299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02d7667f81936503f26a5ed657cfffdc9add626da8ae5bb78d691054cd3af7c3`  
		Last Modified: Fri, 25 Feb 2022 03:02:59 GMT  
		Size: 506.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.7` - windows version 10.0.17763.2565; amd64

```console
$ docker pull nats@sha256:d7c795020fd7295382d503ba883e23cf34ca9c53d6e6b91184bc1fd2bb2c990d
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.6 MB (107634881 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6e99776e94a148ebda875656d07e673c65aedb583986faedb3bdc61a2fd7759`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 02 Feb 2022 19:06:51 GMT
RUN Apply image 1809-amd64
# Wed, 09 Feb 2022 18:13:36 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 25 Feb 2022 02:17:30 GMT
RUN cmd /S /C #(nop) COPY file:d5609a37f534b519fa4326428362ea5398f7165ee90493fb7bdc8b810da33b0e in C:\nats-server.exe 
# Fri, 25 Feb 2022 02:17:31 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Fri, 25 Feb 2022 02:17:32 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Fri, 25 Feb 2022 02:17:33 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 25 Feb 2022 02:17:34 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:bd0b37167cd3d731eb15196e123df7156b5a35597874d3016a1a4298c46fac3f`  
		Size: 103.1 MB (103087119 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8bc49c59cde14e3a9ed8fedce001c00fcb5fe0f9b914aa07273e04f23333d180`  
		Last Modified: Wed, 09 Feb 2022 18:14:28 GMT  
		Size: 1.1 KB (1138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b682f8d539489225b7a3859570b80452b497086f57fa4e6908f2b99d213e1a03`  
		Last Modified: Fri, 25 Feb 2022 03:15:32 GMT  
		Size: 4.5 MB (4541735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67997158a056ea601aec06de195ce0251264a6d8d071f8a44a49a545865ce426`  
		Last Modified: Fri, 25 Feb 2022 03:15:27 GMT  
		Size: 1.7 KB (1656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f873036aacce9bbc35378d6a36985e62919c6d2c9ff526011564a861b86240ab`  
		Last Modified: Fri, 25 Feb 2022 03:15:27 GMT  
		Size: 1.0 KB (1039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf1eace4b7f44dce795499001f62baee27fb477865e490b11d05d198c8e80550`  
		Last Modified: Fri, 25 Feb 2022 03:15:27 GMT  
		Size: 1.1 KB (1081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8accc8a69e6317ee43a53e093f2aef25b70ddff625cfa691d7df28e9bf6d94dc`  
		Last Modified: Fri, 25 Feb 2022 03:15:27 GMT  
		Size: 1.1 KB (1113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.7-alpine`

```console
$ docker pull nats@sha256:6944283c7d430ef4d5e23afb87b2a2d9faf963793bcd94b0461bc12def6c74c2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.7-alpine` - linux; amd64

```console
$ docker pull nats@sha256:6f8d631c068a9d37845ebee434d2c37606757634b9d8950e8de1035dc68842b4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7591453 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:775ec723ebf4c964b880457f54f66782e850e7121d3264c851da7d58cddb64bc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 24 Nov 2021 20:19:40 GMT
ADD file:9233f6f2237d79659a9521f7e390df217cec49f1a8aa3a12147bbca1956acdb9 in / 
# Wed, 24 Nov 2021 20:19:40 GMT
CMD ["/bin/sh"]
# Fri, 25 Feb 2022 02:21:01 GMT
ENV NATS_SERVER=2.7.3
# Fri, 25 Feb 2022 02:21:04 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='c895169ab34bc21442121f6c885905a254a9351a098402f319b3fbfd1e6225c9' ;; 		armhf) natsArch='arm6'; sha256='1b7e1c5835131825c4007766befd0c96a60edbcc3bc336a6739de5c8affea0c4' ;; 		armv7) natsArch='arm7'; sha256='723290467bc7e95b59ca7238a818932b199b00a21d4e3d7eb0e826b7aba2e0ea' ;; 		x86_64) natsArch='amd64'; sha256='2186c7660cd1d9774421614f6724ad32d7cec2389e39858f227a7991be41b1a7' ;; 		x86) natsArch='386'; sha256='3e8e2841921d555d06c67b1e33fc9bd934e4afec4748f7ddf27c67d707fafea4' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 25 Feb 2022 02:21:04 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 25 Feb 2022 02:21:04 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 25 Feb 2022 02:21:04 GMT
EXPOSE 4222 6222 8222
# Fri, 25 Feb 2022 02:21:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Feb 2022 02:21:05 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:59bf1c3509f33515622619af21ed55bbe26d24913cedbca106468a5fb37a50c3`  
		Last Modified: Wed, 24 Nov 2021 20:20:05 GMT  
		Size: 2.8 MB (2818413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfad251bce41e482876302125c33ef603e0ca99f33d1d274a09af07e1acd1be6`  
		Last Modified: Fri, 25 Feb 2022 02:21:40 GMT  
		Size: 4.8 MB (4772040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8c6f8e0dbab2106f703f51433a684cef43840e5e7443402b474f3c09144a4fe`  
		Last Modified: Fri, 25 Feb 2022 02:21:39 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0d8341c3c348e685617552e338228d15dd937ca0708bd7ab85c3c1b273ed88c`  
		Last Modified: Fri, 25 Feb 2022 02:21:39 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.7-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:d6f43ae04309c6115c32d1c71469973712b3e817088a449ce37a9e8cb6b86bf9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7071601 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:846b4c8922b69a90d198633a7b622da89348aa9e3f7f11f58a294e2c4b112a33`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 24 Nov 2021 21:08:16 GMT
ADD file:61137e0aa49ba06f57ac69466fe2fb116f580b5e6159d56f846b1d72c4a3c814 in / 
# Wed, 24 Nov 2021 21:08:16 GMT
CMD ["/bin/sh"]
# Fri, 25 Feb 2022 02:49:34 GMT
ENV NATS_SERVER=2.7.3
# Fri, 25 Feb 2022 02:49:38 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='c895169ab34bc21442121f6c885905a254a9351a098402f319b3fbfd1e6225c9' ;; 		armhf) natsArch='arm6'; sha256='1b7e1c5835131825c4007766befd0c96a60edbcc3bc336a6739de5c8affea0c4' ;; 		armv7) natsArch='arm7'; sha256='723290467bc7e95b59ca7238a818932b199b00a21d4e3d7eb0e826b7aba2e0ea' ;; 		x86_64) natsArch='amd64'; sha256='2186c7660cd1d9774421614f6724ad32d7cec2389e39858f227a7991be41b1a7' ;; 		x86) natsArch='386'; sha256='3e8e2841921d555d06c67b1e33fc9bd934e4afec4748f7ddf27c67d707fafea4' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 25 Feb 2022 02:49:38 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 25 Feb 2022 02:49:39 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 25 Feb 2022 02:49:39 GMT
EXPOSE 4222 6222 8222
# Fri, 25 Feb 2022 02:49:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Feb 2022 02:49:40 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:e4a43de54da9e309482f6762f0c11f5f547cd8fd61a49c5f158453066162023e`  
		Last Modified: Wed, 24 Nov 2021 21:09:46 GMT  
		Size: 2.6 MB (2631421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ecb484648e454aaf42c41938db64a0715cb509a90811b5912192d2e66a2f7fb`  
		Last Modified: Fri, 25 Feb 2022 02:51:52 GMT  
		Size: 4.4 MB (4439176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdd675987846849cf3247fbc41b25505410823bffd30e841e7f663936458e553`  
		Last Modified: Fri, 25 Feb 2022 02:51:49 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ae450e4bdcdcad0dc3e04a43f8855409627f6c7fdecd22f661dbfe3a99530d2`  
		Last Modified: Fri, 25 Feb 2022 02:51:49 GMT  
		Size: 417.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.7-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:665c6221a3c009747c340953834a8e1c6e38008d728f3a9d4d4eaab76e8e640d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.9 MB (6865015 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f23f21c3235ba9d61b53aeb161021b62412dc690dd81727439de14a1f9b902eb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 24 Nov 2021 21:42:11 GMT
ADD file:ca436da5b0bfc9c0e2fc685533c6628918000c8fff109fe9a8da625b9a798002 in / 
# Wed, 24 Nov 2021 21:42:11 GMT
CMD ["/bin/sh"]
# Fri, 25 Feb 2022 02:57:52 GMT
ENV NATS_SERVER=2.7.3
# Fri, 25 Feb 2022 02:57:56 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='c895169ab34bc21442121f6c885905a254a9351a098402f319b3fbfd1e6225c9' ;; 		armhf) natsArch='arm6'; sha256='1b7e1c5835131825c4007766befd0c96a60edbcc3bc336a6739de5c8affea0c4' ;; 		armv7) natsArch='arm7'; sha256='723290467bc7e95b59ca7238a818932b199b00a21d4e3d7eb0e826b7aba2e0ea' ;; 		x86_64) natsArch='amd64'; sha256='2186c7660cd1d9774421614f6724ad32d7cec2389e39858f227a7991be41b1a7' ;; 		x86) natsArch='386'; sha256='3e8e2841921d555d06c67b1e33fc9bd934e4afec4748f7ddf27c67d707fafea4' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 25 Feb 2022 02:57:57 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 25 Feb 2022 02:57:57 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 25 Feb 2022 02:57:58 GMT
EXPOSE 4222 6222 8222
# Fri, 25 Feb 2022 02:57:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Feb 2022 02:57:58 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:5480d2ca1740c20ce17652e01ed2265cdc914458acd41256a2b1ccff28f2762c`  
		Last Modified: Wed, 24 Nov 2021 21:43:40 GMT  
		Size: 2.4 MB (2434764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fafd4ba596baa033665a46ce765df0c4a928784832ecc5645944032cfcd9295`  
		Last Modified: Fri, 25 Feb 2022 03:00:20 GMT  
		Size: 4.4 MB (4429250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abb2edff52bc9250fdec4032d39728784d4495539ef65cceed401a8968ec2df5`  
		Last Modified: Fri, 25 Feb 2022 03:00:18 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1047f2aa448d4163e2995aed662d6890fdd3954289a1ff2908edc894450b3d78`  
		Last Modified: Fri, 25 Feb 2022 03:00:18 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.7-alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:8f79d8af0b084884d2cc9641a33a1274022fc51b99e955d3f13d9c45f47cf6b4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7132810 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e50bb490b2ac0a89152a29fc28e269300b6b83d2a85c0ce5ebe74635c34cdb0d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 24 Nov 2021 20:39:20 GMT
ADD file:df53811312284306901fdaaff0a357a4bf40d631e662fe9ce6d342442e494b6c in / 
# Wed, 24 Nov 2021 20:39:20 GMT
CMD ["/bin/sh"]
# Fri, 25 Feb 2022 03:01:24 GMT
ENV NATS_SERVER=2.7.3
# Fri, 25 Feb 2022 03:01:26 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='c895169ab34bc21442121f6c885905a254a9351a098402f319b3fbfd1e6225c9' ;; 		armhf) natsArch='arm6'; sha256='1b7e1c5835131825c4007766befd0c96a60edbcc3bc336a6739de5c8affea0c4' ;; 		armv7) natsArch='arm7'; sha256='723290467bc7e95b59ca7238a818932b199b00a21d4e3d7eb0e826b7aba2e0ea' ;; 		x86_64) natsArch='amd64'; sha256='2186c7660cd1d9774421614f6724ad32d7cec2389e39858f227a7991be41b1a7' ;; 		x86) natsArch='386'; sha256='3e8e2841921d555d06c67b1e33fc9bd934e4afec4748f7ddf27c67d707fafea4' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 25 Feb 2022 03:01:28 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 25 Feb 2022 03:01:29 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 25 Feb 2022 03:01:29 GMT
EXPOSE 4222 6222 8222
# Fri, 25 Feb 2022 03:01:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Feb 2022 03:01:31 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9b3977197b4f2147bdd31e1271f811319dcd5c2fc595f14e81f5351ab6275b99`  
		Last Modified: Wed, 24 Nov 2021 20:39:59 GMT  
		Size: 2.7 MB (2715434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c75ed4d21bde940c8f5b4d0d82b44c31489bd5a37d46b1f197b7d1baed0b6e8`  
		Last Modified: Fri, 25 Feb 2022 03:02:31 GMT  
		Size: 4.4 MB (4416403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f7dd0d82f2c731b21df156c69326c651274a35eb010b23b5150397309110717`  
		Last Modified: Fri, 25 Feb 2022 03:02:30 GMT  
		Size: 559.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f29d0f81d7bbfb90bc5607be41aabbd3e970b1e74e19a069c23e863092772ba`  
		Last Modified: Fri, 25 Feb 2022 03:02:30 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.7-alpine3.15`

```console
$ docker pull nats@sha256:6944283c7d430ef4d5e23afb87b2a2d9faf963793bcd94b0461bc12def6c74c2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.7-alpine3.15` - linux; amd64

```console
$ docker pull nats@sha256:6f8d631c068a9d37845ebee434d2c37606757634b9d8950e8de1035dc68842b4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7591453 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:775ec723ebf4c964b880457f54f66782e850e7121d3264c851da7d58cddb64bc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 24 Nov 2021 20:19:40 GMT
ADD file:9233f6f2237d79659a9521f7e390df217cec49f1a8aa3a12147bbca1956acdb9 in / 
# Wed, 24 Nov 2021 20:19:40 GMT
CMD ["/bin/sh"]
# Fri, 25 Feb 2022 02:21:01 GMT
ENV NATS_SERVER=2.7.3
# Fri, 25 Feb 2022 02:21:04 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='c895169ab34bc21442121f6c885905a254a9351a098402f319b3fbfd1e6225c9' ;; 		armhf) natsArch='arm6'; sha256='1b7e1c5835131825c4007766befd0c96a60edbcc3bc336a6739de5c8affea0c4' ;; 		armv7) natsArch='arm7'; sha256='723290467bc7e95b59ca7238a818932b199b00a21d4e3d7eb0e826b7aba2e0ea' ;; 		x86_64) natsArch='amd64'; sha256='2186c7660cd1d9774421614f6724ad32d7cec2389e39858f227a7991be41b1a7' ;; 		x86) natsArch='386'; sha256='3e8e2841921d555d06c67b1e33fc9bd934e4afec4748f7ddf27c67d707fafea4' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 25 Feb 2022 02:21:04 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 25 Feb 2022 02:21:04 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 25 Feb 2022 02:21:04 GMT
EXPOSE 4222 6222 8222
# Fri, 25 Feb 2022 02:21:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Feb 2022 02:21:05 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:59bf1c3509f33515622619af21ed55bbe26d24913cedbca106468a5fb37a50c3`  
		Last Modified: Wed, 24 Nov 2021 20:20:05 GMT  
		Size: 2.8 MB (2818413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfad251bce41e482876302125c33ef603e0ca99f33d1d274a09af07e1acd1be6`  
		Last Modified: Fri, 25 Feb 2022 02:21:40 GMT  
		Size: 4.8 MB (4772040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8c6f8e0dbab2106f703f51433a684cef43840e5e7443402b474f3c09144a4fe`  
		Last Modified: Fri, 25 Feb 2022 02:21:39 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0d8341c3c348e685617552e338228d15dd937ca0708bd7ab85c3c1b273ed88c`  
		Last Modified: Fri, 25 Feb 2022 02:21:39 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.7-alpine3.15` - linux; arm variant v6

```console
$ docker pull nats@sha256:d6f43ae04309c6115c32d1c71469973712b3e817088a449ce37a9e8cb6b86bf9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7071601 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:846b4c8922b69a90d198633a7b622da89348aa9e3f7f11f58a294e2c4b112a33`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 24 Nov 2021 21:08:16 GMT
ADD file:61137e0aa49ba06f57ac69466fe2fb116f580b5e6159d56f846b1d72c4a3c814 in / 
# Wed, 24 Nov 2021 21:08:16 GMT
CMD ["/bin/sh"]
# Fri, 25 Feb 2022 02:49:34 GMT
ENV NATS_SERVER=2.7.3
# Fri, 25 Feb 2022 02:49:38 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='c895169ab34bc21442121f6c885905a254a9351a098402f319b3fbfd1e6225c9' ;; 		armhf) natsArch='arm6'; sha256='1b7e1c5835131825c4007766befd0c96a60edbcc3bc336a6739de5c8affea0c4' ;; 		armv7) natsArch='arm7'; sha256='723290467bc7e95b59ca7238a818932b199b00a21d4e3d7eb0e826b7aba2e0ea' ;; 		x86_64) natsArch='amd64'; sha256='2186c7660cd1d9774421614f6724ad32d7cec2389e39858f227a7991be41b1a7' ;; 		x86) natsArch='386'; sha256='3e8e2841921d555d06c67b1e33fc9bd934e4afec4748f7ddf27c67d707fafea4' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 25 Feb 2022 02:49:38 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 25 Feb 2022 02:49:39 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 25 Feb 2022 02:49:39 GMT
EXPOSE 4222 6222 8222
# Fri, 25 Feb 2022 02:49:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Feb 2022 02:49:40 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:e4a43de54da9e309482f6762f0c11f5f547cd8fd61a49c5f158453066162023e`  
		Last Modified: Wed, 24 Nov 2021 21:09:46 GMT  
		Size: 2.6 MB (2631421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ecb484648e454aaf42c41938db64a0715cb509a90811b5912192d2e66a2f7fb`  
		Last Modified: Fri, 25 Feb 2022 02:51:52 GMT  
		Size: 4.4 MB (4439176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdd675987846849cf3247fbc41b25505410823bffd30e841e7f663936458e553`  
		Last Modified: Fri, 25 Feb 2022 02:51:49 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ae450e4bdcdcad0dc3e04a43f8855409627f6c7fdecd22f661dbfe3a99530d2`  
		Last Modified: Fri, 25 Feb 2022 02:51:49 GMT  
		Size: 417.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.7-alpine3.15` - linux; arm variant v7

```console
$ docker pull nats@sha256:665c6221a3c009747c340953834a8e1c6e38008d728f3a9d4d4eaab76e8e640d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.9 MB (6865015 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f23f21c3235ba9d61b53aeb161021b62412dc690dd81727439de14a1f9b902eb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 24 Nov 2021 21:42:11 GMT
ADD file:ca436da5b0bfc9c0e2fc685533c6628918000c8fff109fe9a8da625b9a798002 in / 
# Wed, 24 Nov 2021 21:42:11 GMT
CMD ["/bin/sh"]
# Fri, 25 Feb 2022 02:57:52 GMT
ENV NATS_SERVER=2.7.3
# Fri, 25 Feb 2022 02:57:56 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='c895169ab34bc21442121f6c885905a254a9351a098402f319b3fbfd1e6225c9' ;; 		armhf) natsArch='arm6'; sha256='1b7e1c5835131825c4007766befd0c96a60edbcc3bc336a6739de5c8affea0c4' ;; 		armv7) natsArch='arm7'; sha256='723290467bc7e95b59ca7238a818932b199b00a21d4e3d7eb0e826b7aba2e0ea' ;; 		x86_64) natsArch='amd64'; sha256='2186c7660cd1d9774421614f6724ad32d7cec2389e39858f227a7991be41b1a7' ;; 		x86) natsArch='386'; sha256='3e8e2841921d555d06c67b1e33fc9bd934e4afec4748f7ddf27c67d707fafea4' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 25 Feb 2022 02:57:57 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 25 Feb 2022 02:57:57 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 25 Feb 2022 02:57:58 GMT
EXPOSE 4222 6222 8222
# Fri, 25 Feb 2022 02:57:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Feb 2022 02:57:58 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:5480d2ca1740c20ce17652e01ed2265cdc914458acd41256a2b1ccff28f2762c`  
		Last Modified: Wed, 24 Nov 2021 21:43:40 GMT  
		Size: 2.4 MB (2434764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fafd4ba596baa033665a46ce765df0c4a928784832ecc5645944032cfcd9295`  
		Last Modified: Fri, 25 Feb 2022 03:00:20 GMT  
		Size: 4.4 MB (4429250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abb2edff52bc9250fdec4032d39728784d4495539ef65cceed401a8968ec2df5`  
		Last Modified: Fri, 25 Feb 2022 03:00:18 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1047f2aa448d4163e2995aed662d6890fdd3954289a1ff2908edc894450b3d78`  
		Last Modified: Fri, 25 Feb 2022 03:00:18 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.7-alpine3.15` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:8f79d8af0b084884d2cc9641a33a1274022fc51b99e955d3f13d9c45f47cf6b4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7132810 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e50bb490b2ac0a89152a29fc28e269300b6b83d2a85c0ce5ebe74635c34cdb0d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 24 Nov 2021 20:39:20 GMT
ADD file:df53811312284306901fdaaff0a357a4bf40d631e662fe9ce6d342442e494b6c in / 
# Wed, 24 Nov 2021 20:39:20 GMT
CMD ["/bin/sh"]
# Fri, 25 Feb 2022 03:01:24 GMT
ENV NATS_SERVER=2.7.3
# Fri, 25 Feb 2022 03:01:26 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='c895169ab34bc21442121f6c885905a254a9351a098402f319b3fbfd1e6225c9' ;; 		armhf) natsArch='arm6'; sha256='1b7e1c5835131825c4007766befd0c96a60edbcc3bc336a6739de5c8affea0c4' ;; 		armv7) natsArch='arm7'; sha256='723290467bc7e95b59ca7238a818932b199b00a21d4e3d7eb0e826b7aba2e0ea' ;; 		x86_64) natsArch='amd64'; sha256='2186c7660cd1d9774421614f6724ad32d7cec2389e39858f227a7991be41b1a7' ;; 		x86) natsArch='386'; sha256='3e8e2841921d555d06c67b1e33fc9bd934e4afec4748f7ddf27c67d707fafea4' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 25 Feb 2022 03:01:28 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 25 Feb 2022 03:01:29 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 25 Feb 2022 03:01:29 GMT
EXPOSE 4222 6222 8222
# Fri, 25 Feb 2022 03:01:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Feb 2022 03:01:31 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9b3977197b4f2147bdd31e1271f811319dcd5c2fc595f14e81f5351ab6275b99`  
		Last Modified: Wed, 24 Nov 2021 20:39:59 GMT  
		Size: 2.7 MB (2715434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c75ed4d21bde940c8f5b4d0d82b44c31489bd5a37d46b1f197b7d1baed0b6e8`  
		Last Modified: Fri, 25 Feb 2022 03:02:31 GMT  
		Size: 4.4 MB (4416403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f7dd0d82f2c731b21df156c69326c651274a35eb010b23b5150397309110717`  
		Last Modified: Fri, 25 Feb 2022 03:02:30 GMT  
		Size: 559.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f29d0f81d7bbfb90bc5607be41aabbd3e970b1e74e19a069c23e863092772ba`  
		Last Modified: Fri, 25 Feb 2022 03:02:30 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.7-linux`

```console
$ docker pull nats@sha256:4fe2c16e211795858e7e7538197ec57f67ed6e9ca5d91d06d925e09ec6724d3b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.7-linux` - linux; amd64

```console
$ docker pull nats@sha256:5fd249efa75cf3eb595342175207fdbb390eee3034f7fe49355d7a479fa3ffe2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4499407 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c84de17b17b3458d2b6e6d4264ea6186c82bab718ca058f5d7738e53ca2759ac`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 25 Feb 2022 02:21:13 GMT
COPY file:8a814b0c66a47e63e5a7f4287478948812fe6e03c224d539f37ce3f950d2b6c6 in /nats-server 
# Fri, 25 Feb 2022 02:21:13 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 25 Feb 2022 02:21:14 GMT
EXPOSE 4222 6222 8222
# Fri, 25 Feb 2022 02:21:14 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 25 Feb 2022 02:21:14 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:277fae1baf41821774f7a2e1c3f465b28aa8693ee0cd77e0ad0bace55d9c616e`  
		Last Modified: Fri, 25 Feb 2022 02:22:04 GMT  
		Size: 4.5 MB (4498900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb932b4b3fbc873b56e996c6357055bb7700c701d17d7d87cdec31211142b49a`  
		Last Modified: Fri, 25 Feb 2022 02:22:03 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.7-linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:2e3339e7e8d98e7bbab0613c7b7c3dd6f51fcf33ed3910a2e65e62fba7049337
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4165977 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ddc7bcc78dd550ace4def82e3db227e618d77e136274749f3bf55869e64be264`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 25 Feb 2022 02:50:06 GMT
COPY file:3a951d885f7bcec693f6fbf26a9ffd82b0c6218b6834fc6053e5812f7451b63e in /nats-server 
# Fri, 25 Feb 2022 02:50:06 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 25 Feb 2022 02:50:07 GMT
EXPOSE 4222 6222 8222
# Fri, 25 Feb 2022 02:50:07 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 25 Feb 2022 02:50:07 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:f6de87b4530f922b11edc08be8edeebc6ce0cb666907013348d4e1b9f5d51809`  
		Last Modified: Fri, 25 Feb 2022 02:52:29 GMT  
		Size: 4.2 MB (4165468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5fa68b52226484e5870677184cdc47c93a7d453f334c144b5cb631346bc8111`  
		Last Modified: Fri, 25 Feb 2022 02:52:27 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.7-linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:87cf3f8e33ebf28f35575ea083f8feb460d19fa9380d2622c82567ff3fa9d840
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4157918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4eef99b95e572b23f90d60e6e157be90b05ab2f35dbcb10f83f96ece551945a`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 25 Feb 2022 02:58:34 GMT
COPY file:3ee879939ad264e803dd4d6072181d968c4dd0fe076115159f70479c6309ef45 in /nats-server 
# Fri, 25 Feb 2022 02:58:34 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 25 Feb 2022 02:58:35 GMT
EXPOSE 4222 6222 8222
# Fri, 25 Feb 2022 02:58:35 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 25 Feb 2022 02:58:36 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:67a3d8907097b9caffd9d1720b4fb2b1d2ac9dfda60a1d169abbf5494323d50a`  
		Last Modified: Fri, 25 Feb 2022 03:00:58 GMT  
		Size: 4.2 MB (4157409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73f5577f4846f032b281220b897161962481198ead0a1b9ad1d7c76cdd989747`  
		Last Modified: Fri, 25 Feb 2022 03:00:55 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.7-linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:e970861a260709ae1e8c892eb36758c14323e81959ff4aaa1e9b7327b91d3e70
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.1 MB (4143805 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4414e48026697a15338f28dcb8e46ace9627ea7332559e1708f36ce62a5e327`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 25 Feb 2022 03:01:42 GMT
COPY file:acd11e9a3a86f6f3da079c5155851337e747c3b31481ec05e2dd1e48e23becb2 in /nats-server 
# Fri, 25 Feb 2022 03:01:43 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 25 Feb 2022 03:01:43 GMT
EXPOSE 4222 6222 8222
# Fri, 25 Feb 2022 03:01:44 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 25 Feb 2022 03:01:45 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6ad9fd47af885b43442590ad2c8171e4b4899caef84921ec73ba0540b9c03284`  
		Last Modified: Fri, 25 Feb 2022 03:02:59 GMT  
		Size: 4.1 MB (4143299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02d7667f81936503f26a5ed657cfffdc9add626da8ae5bb78d691054cd3af7c3`  
		Last Modified: Fri, 25 Feb 2022 03:02:59 GMT  
		Size: 506.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.7-nanoserver`

```console
$ docker pull nats@sha256:6e43eecf010598596b218f3800a6d052426d875695ead9cdbf074e0653772142
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2565; amd64

### `nats:2.7-nanoserver` - windows version 10.0.17763.2565; amd64

```console
$ docker pull nats@sha256:d7c795020fd7295382d503ba883e23cf34ca9c53d6e6b91184bc1fd2bb2c990d
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.6 MB (107634881 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6e99776e94a148ebda875656d07e673c65aedb583986faedb3bdc61a2fd7759`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 02 Feb 2022 19:06:51 GMT
RUN Apply image 1809-amd64
# Wed, 09 Feb 2022 18:13:36 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 25 Feb 2022 02:17:30 GMT
RUN cmd /S /C #(nop) COPY file:d5609a37f534b519fa4326428362ea5398f7165ee90493fb7bdc8b810da33b0e in C:\nats-server.exe 
# Fri, 25 Feb 2022 02:17:31 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Fri, 25 Feb 2022 02:17:32 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Fri, 25 Feb 2022 02:17:33 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 25 Feb 2022 02:17:34 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:bd0b37167cd3d731eb15196e123df7156b5a35597874d3016a1a4298c46fac3f`  
		Size: 103.1 MB (103087119 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8bc49c59cde14e3a9ed8fedce001c00fcb5fe0f9b914aa07273e04f23333d180`  
		Last Modified: Wed, 09 Feb 2022 18:14:28 GMT  
		Size: 1.1 KB (1138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b682f8d539489225b7a3859570b80452b497086f57fa4e6908f2b99d213e1a03`  
		Last Modified: Fri, 25 Feb 2022 03:15:32 GMT  
		Size: 4.5 MB (4541735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67997158a056ea601aec06de195ce0251264a6d8d071f8a44a49a545865ce426`  
		Last Modified: Fri, 25 Feb 2022 03:15:27 GMT  
		Size: 1.7 KB (1656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f873036aacce9bbc35378d6a36985e62919c6d2c9ff526011564a861b86240ab`  
		Last Modified: Fri, 25 Feb 2022 03:15:27 GMT  
		Size: 1.0 KB (1039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf1eace4b7f44dce795499001f62baee27fb477865e490b11d05d198c8e80550`  
		Last Modified: Fri, 25 Feb 2022 03:15:27 GMT  
		Size: 1.1 KB (1081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8accc8a69e6317ee43a53e093f2aef25b70ddff625cfa691d7df28e9bf6d94dc`  
		Last Modified: Fri, 25 Feb 2022 03:15:27 GMT  
		Size: 1.1 KB (1113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.7-nanoserver-1809`

```console
$ docker pull nats@sha256:6e43eecf010598596b218f3800a6d052426d875695ead9cdbf074e0653772142
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2565; amd64

### `nats:2.7-nanoserver-1809` - windows version 10.0.17763.2565; amd64

```console
$ docker pull nats@sha256:d7c795020fd7295382d503ba883e23cf34ca9c53d6e6b91184bc1fd2bb2c990d
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.6 MB (107634881 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6e99776e94a148ebda875656d07e673c65aedb583986faedb3bdc61a2fd7759`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 02 Feb 2022 19:06:51 GMT
RUN Apply image 1809-amd64
# Wed, 09 Feb 2022 18:13:36 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 25 Feb 2022 02:17:30 GMT
RUN cmd /S /C #(nop) COPY file:d5609a37f534b519fa4326428362ea5398f7165ee90493fb7bdc8b810da33b0e in C:\nats-server.exe 
# Fri, 25 Feb 2022 02:17:31 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Fri, 25 Feb 2022 02:17:32 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Fri, 25 Feb 2022 02:17:33 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 25 Feb 2022 02:17:34 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:bd0b37167cd3d731eb15196e123df7156b5a35597874d3016a1a4298c46fac3f`  
		Size: 103.1 MB (103087119 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8bc49c59cde14e3a9ed8fedce001c00fcb5fe0f9b914aa07273e04f23333d180`  
		Last Modified: Wed, 09 Feb 2022 18:14:28 GMT  
		Size: 1.1 KB (1138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b682f8d539489225b7a3859570b80452b497086f57fa4e6908f2b99d213e1a03`  
		Last Modified: Fri, 25 Feb 2022 03:15:32 GMT  
		Size: 4.5 MB (4541735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67997158a056ea601aec06de195ce0251264a6d8d071f8a44a49a545865ce426`  
		Last Modified: Fri, 25 Feb 2022 03:15:27 GMT  
		Size: 1.7 KB (1656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f873036aacce9bbc35378d6a36985e62919c6d2c9ff526011564a861b86240ab`  
		Last Modified: Fri, 25 Feb 2022 03:15:27 GMT  
		Size: 1.0 KB (1039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf1eace4b7f44dce795499001f62baee27fb477865e490b11d05d198c8e80550`  
		Last Modified: Fri, 25 Feb 2022 03:15:27 GMT  
		Size: 1.1 KB (1081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8accc8a69e6317ee43a53e093f2aef25b70ddff625cfa691d7df28e9bf6d94dc`  
		Last Modified: Fri, 25 Feb 2022 03:15:27 GMT  
		Size: 1.1 KB (1113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.7-scratch`

```console
$ docker pull nats@sha256:4fe2c16e211795858e7e7538197ec57f67ed6e9ca5d91d06d925e09ec6724d3b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.7-scratch` - linux; amd64

```console
$ docker pull nats@sha256:5fd249efa75cf3eb595342175207fdbb390eee3034f7fe49355d7a479fa3ffe2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4499407 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c84de17b17b3458d2b6e6d4264ea6186c82bab718ca058f5d7738e53ca2759ac`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 25 Feb 2022 02:21:13 GMT
COPY file:8a814b0c66a47e63e5a7f4287478948812fe6e03c224d539f37ce3f950d2b6c6 in /nats-server 
# Fri, 25 Feb 2022 02:21:13 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 25 Feb 2022 02:21:14 GMT
EXPOSE 4222 6222 8222
# Fri, 25 Feb 2022 02:21:14 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 25 Feb 2022 02:21:14 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:277fae1baf41821774f7a2e1c3f465b28aa8693ee0cd77e0ad0bace55d9c616e`  
		Last Modified: Fri, 25 Feb 2022 02:22:04 GMT  
		Size: 4.5 MB (4498900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb932b4b3fbc873b56e996c6357055bb7700c701d17d7d87cdec31211142b49a`  
		Last Modified: Fri, 25 Feb 2022 02:22:03 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.7-scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:2e3339e7e8d98e7bbab0613c7b7c3dd6f51fcf33ed3910a2e65e62fba7049337
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4165977 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ddc7bcc78dd550ace4def82e3db227e618d77e136274749f3bf55869e64be264`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 25 Feb 2022 02:50:06 GMT
COPY file:3a951d885f7bcec693f6fbf26a9ffd82b0c6218b6834fc6053e5812f7451b63e in /nats-server 
# Fri, 25 Feb 2022 02:50:06 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 25 Feb 2022 02:50:07 GMT
EXPOSE 4222 6222 8222
# Fri, 25 Feb 2022 02:50:07 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 25 Feb 2022 02:50:07 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:f6de87b4530f922b11edc08be8edeebc6ce0cb666907013348d4e1b9f5d51809`  
		Last Modified: Fri, 25 Feb 2022 02:52:29 GMT  
		Size: 4.2 MB (4165468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5fa68b52226484e5870677184cdc47c93a7d453f334c144b5cb631346bc8111`  
		Last Modified: Fri, 25 Feb 2022 02:52:27 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.7-scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:87cf3f8e33ebf28f35575ea083f8feb460d19fa9380d2622c82567ff3fa9d840
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4157918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4eef99b95e572b23f90d60e6e157be90b05ab2f35dbcb10f83f96ece551945a`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 25 Feb 2022 02:58:34 GMT
COPY file:3ee879939ad264e803dd4d6072181d968c4dd0fe076115159f70479c6309ef45 in /nats-server 
# Fri, 25 Feb 2022 02:58:34 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 25 Feb 2022 02:58:35 GMT
EXPOSE 4222 6222 8222
# Fri, 25 Feb 2022 02:58:35 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 25 Feb 2022 02:58:36 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:67a3d8907097b9caffd9d1720b4fb2b1d2ac9dfda60a1d169abbf5494323d50a`  
		Last Modified: Fri, 25 Feb 2022 03:00:58 GMT  
		Size: 4.2 MB (4157409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73f5577f4846f032b281220b897161962481198ead0a1b9ad1d7c76cdd989747`  
		Last Modified: Fri, 25 Feb 2022 03:00:55 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.7-scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:e970861a260709ae1e8c892eb36758c14323e81959ff4aaa1e9b7327b91d3e70
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.1 MB (4143805 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4414e48026697a15338f28dcb8e46ace9627ea7332559e1708f36ce62a5e327`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 25 Feb 2022 03:01:42 GMT
COPY file:acd11e9a3a86f6f3da079c5155851337e747c3b31481ec05e2dd1e48e23becb2 in /nats-server 
# Fri, 25 Feb 2022 03:01:43 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 25 Feb 2022 03:01:43 GMT
EXPOSE 4222 6222 8222
# Fri, 25 Feb 2022 03:01:44 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 25 Feb 2022 03:01:45 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6ad9fd47af885b43442590ad2c8171e4b4899caef84921ec73ba0540b9c03284`  
		Last Modified: Fri, 25 Feb 2022 03:02:59 GMT  
		Size: 4.1 MB (4143299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02d7667f81936503f26a5ed657cfffdc9add626da8ae5bb78d691054cd3af7c3`  
		Last Modified: Fri, 25 Feb 2022 03:02:59 GMT  
		Size: 506.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.7-windowsservercore`

```console
$ docker pull nats@sha256:2b9c20408baf29df9d8666fc894d8a5c308946331d4310ef5a82b1eed5101db3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2565; amd64

### `nats:2.7-windowsservercore` - windows version 10.0.17763.2565; amd64

```console
$ docker pull nats@sha256:ac025e7ac0a2786f5807888399f94d317a0636b60e8a37584569d586fb1ac146
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2718991955 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:007419288bb7b16cd78d29d0476687df2d88011775f13b3f565c92414a214c05`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Wed, 02 Feb 2022 19:28:56 GMT
RUN Install update 1809-amd64
# Wed, 09 Feb 2022 15:04:17 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Feb 2022 18:10:54 GMT
ENV NATS_DOCKERIZED=1
# Fri, 25 Feb 2022 02:14:46 GMT
ENV NATS_SERVER=2.7.3
# Fri, 25 Feb 2022 02:14:47 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.7.3/nats-server-v2.7.3-windows-amd64.zip
# Fri, 25 Feb 2022 02:14:48 GMT
ENV NATS_SERVER_SHASUM=ddb372da68741d897006c8d4b160c7f4788603cbaacb3fa105ddf7baada04428
# Fri, 25 Feb 2022 02:15:50 GMT
RUN Set-PSDebug -Trace 2
# Fri, 25 Feb 2022 02:17:14 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 25 Feb 2022 02:17:16 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Fri, 25 Feb 2022 02:17:17 GMT
EXPOSE 4222 6222 8222
# Fri, 25 Feb 2022 02:17:18 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 25 Feb 2022 02:17:19 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:1bd78008c728d8f9e56dc2093e6eb55f0f0b1aa96e5d0c7ccc830c5f60876cdf`  
		Size: 995.4 MB (995381853 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f49d3791198cf2ea875fd54ce3bb715670742d4a58c00252395ad1b74036662a`  
		Last Modified: Wed, 09 Feb 2022 16:39:51 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4235aeeb4e8b577cc7aa26c7994ec94c94dd53a38764fc510b330b77cef4abad`  
		Last Modified: Wed, 09 Feb 2022 18:14:09 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6ed63a799d34b3a151eb2d65afc4a93d028c5308ce305f9059da19083ea4579`  
		Last Modified: Fri, 25 Feb 2022 03:15:11 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fa36020fa0fadcfe9ac785f1bc4cbf6e51ac336a4441d2ea628465f9f1e3832`  
		Last Modified: Fri, 25 Feb 2022 03:15:11 GMT  
		Size: 1.3 KB (1321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58aaa8ed102560150d8bd4fe887000c2789a69df5ae550a8b8058e526d01af34`  
		Last Modified: Fri, 25 Feb 2022 03:15:11 GMT  
		Size: 1.3 KB (1300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e48afd20cc6576c9f831f4166f86f4cd65be8140eda5a57159bba0d62c21b1af`  
		Last Modified: Fri, 25 Feb 2022 03:15:12 GMT  
		Size: 374.3 KB (374309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1eb76be5e45618d5a45f4672ac8e8c8d45d10bf627dc47f3afe45c7909b223b`  
		Last Modified: Fri, 25 Feb 2022 03:15:10 GMT  
		Size: 4.9 MB (4890363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:513928aafbffc4a16807de347507df4019d3096da02f3475f8731f6704a0e75d`  
		Last Modified: Fri, 25 Feb 2022 03:15:09 GMT  
		Size: 1.9 KB (1884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6ba5e5368daffd340a50b6715a6d9d28d2f2c341d694c5d7cdae52e15e46d4d`  
		Last Modified: Fri, 25 Feb 2022 03:15:09 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca864d6530840f9fbdc99b6aaedcd8aa7acf319697677ca480fd220d426cb62f`  
		Last Modified: Fri, 25 Feb 2022 03:15:09 GMT  
		Size: 1.3 KB (1322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e9cb037cabf38f35bdcf375e13b7790bfdc9b4e9761cd2e865cf557a7575e81`  
		Last Modified: Fri, 25 Feb 2022 03:15:09 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.7-windowsservercore-1809`

```console
$ docker pull nats@sha256:2b9c20408baf29df9d8666fc894d8a5c308946331d4310ef5a82b1eed5101db3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2565; amd64

### `nats:2.7-windowsservercore-1809` - windows version 10.0.17763.2565; amd64

```console
$ docker pull nats@sha256:ac025e7ac0a2786f5807888399f94d317a0636b60e8a37584569d586fb1ac146
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2718991955 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:007419288bb7b16cd78d29d0476687df2d88011775f13b3f565c92414a214c05`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Wed, 02 Feb 2022 19:28:56 GMT
RUN Install update 1809-amd64
# Wed, 09 Feb 2022 15:04:17 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Feb 2022 18:10:54 GMT
ENV NATS_DOCKERIZED=1
# Fri, 25 Feb 2022 02:14:46 GMT
ENV NATS_SERVER=2.7.3
# Fri, 25 Feb 2022 02:14:47 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.7.3/nats-server-v2.7.3-windows-amd64.zip
# Fri, 25 Feb 2022 02:14:48 GMT
ENV NATS_SERVER_SHASUM=ddb372da68741d897006c8d4b160c7f4788603cbaacb3fa105ddf7baada04428
# Fri, 25 Feb 2022 02:15:50 GMT
RUN Set-PSDebug -Trace 2
# Fri, 25 Feb 2022 02:17:14 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 25 Feb 2022 02:17:16 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Fri, 25 Feb 2022 02:17:17 GMT
EXPOSE 4222 6222 8222
# Fri, 25 Feb 2022 02:17:18 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 25 Feb 2022 02:17:19 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:1bd78008c728d8f9e56dc2093e6eb55f0f0b1aa96e5d0c7ccc830c5f60876cdf`  
		Size: 995.4 MB (995381853 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f49d3791198cf2ea875fd54ce3bb715670742d4a58c00252395ad1b74036662a`  
		Last Modified: Wed, 09 Feb 2022 16:39:51 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4235aeeb4e8b577cc7aa26c7994ec94c94dd53a38764fc510b330b77cef4abad`  
		Last Modified: Wed, 09 Feb 2022 18:14:09 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6ed63a799d34b3a151eb2d65afc4a93d028c5308ce305f9059da19083ea4579`  
		Last Modified: Fri, 25 Feb 2022 03:15:11 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fa36020fa0fadcfe9ac785f1bc4cbf6e51ac336a4441d2ea628465f9f1e3832`  
		Last Modified: Fri, 25 Feb 2022 03:15:11 GMT  
		Size: 1.3 KB (1321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58aaa8ed102560150d8bd4fe887000c2789a69df5ae550a8b8058e526d01af34`  
		Last Modified: Fri, 25 Feb 2022 03:15:11 GMT  
		Size: 1.3 KB (1300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e48afd20cc6576c9f831f4166f86f4cd65be8140eda5a57159bba0d62c21b1af`  
		Last Modified: Fri, 25 Feb 2022 03:15:12 GMT  
		Size: 374.3 KB (374309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1eb76be5e45618d5a45f4672ac8e8c8d45d10bf627dc47f3afe45c7909b223b`  
		Last Modified: Fri, 25 Feb 2022 03:15:10 GMT  
		Size: 4.9 MB (4890363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:513928aafbffc4a16807de347507df4019d3096da02f3475f8731f6704a0e75d`  
		Last Modified: Fri, 25 Feb 2022 03:15:09 GMT  
		Size: 1.9 KB (1884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6ba5e5368daffd340a50b6715a6d9d28d2f2c341d694c5d7cdae52e15e46d4d`  
		Last Modified: Fri, 25 Feb 2022 03:15:09 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca864d6530840f9fbdc99b6aaedcd8aa7acf319697677ca480fd220d426cb62f`  
		Last Modified: Fri, 25 Feb 2022 03:15:09 GMT  
		Size: 1.3 KB (1322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e9cb037cabf38f35bdcf375e13b7790bfdc9b4e9761cd2e865cf557a7575e81`  
		Last Modified: Fri, 25 Feb 2022 03:15:09 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.7.3`

```console
$ docker pull nats@sha256:4fa6d62e36bac738598e6523bb2185b0d57de021331057a538765f518cfd505a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.2565; amd64

### `nats:2.7.3` - linux; amd64

```console
$ docker pull nats@sha256:5fd249efa75cf3eb595342175207fdbb390eee3034f7fe49355d7a479fa3ffe2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4499407 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c84de17b17b3458d2b6e6d4264ea6186c82bab718ca058f5d7738e53ca2759ac`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 25 Feb 2022 02:21:13 GMT
COPY file:8a814b0c66a47e63e5a7f4287478948812fe6e03c224d539f37ce3f950d2b6c6 in /nats-server 
# Fri, 25 Feb 2022 02:21:13 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 25 Feb 2022 02:21:14 GMT
EXPOSE 4222 6222 8222
# Fri, 25 Feb 2022 02:21:14 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 25 Feb 2022 02:21:14 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:277fae1baf41821774f7a2e1c3f465b28aa8693ee0cd77e0ad0bace55d9c616e`  
		Last Modified: Fri, 25 Feb 2022 02:22:04 GMT  
		Size: 4.5 MB (4498900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb932b4b3fbc873b56e996c6357055bb7700c701d17d7d87cdec31211142b49a`  
		Last Modified: Fri, 25 Feb 2022 02:22:03 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.7.3` - linux; arm variant v6

```console
$ docker pull nats@sha256:2e3339e7e8d98e7bbab0613c7b7c3dd6f51fcf33ed3910a2e65e62fba7049337
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4165977 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ddc7bcc78dd550ace4def82e3db227e618d77e136274749f3bf55869e64be264`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 25 Feb 2022 02:50:06 GMT
COPY file:3a951d885f7bcec693f6fbf26a9ffd82b0c6218b6834fc6053e5812f7451b63e in /nats-server 
# Fri, 25 Feb 2022 02:50:06 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 25 Feb 2022 02:50:07 GMT
EXPOSE 4222 6222 8222
# Fri, 25 Feb 2022 02:50:07 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 25 Feb 2022 02:50:07 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:f6de87b4530f922b11edc08be8edeebc6ce0cb666907013348d4e1b9f5d51809`  
		Last Modified: Fri, 25 Feb 2022 02:52:29 GMT  
		Size: 4.2 MB (4165468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5fa68b52226484e5870677184cdc47c93a7d453f334c144b5cb631346bc8111`  
		Last Modified: Fri, 25 Feb 2022 02:52:27 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.7.3` - linux; arm variant v7

```console
$ docker pull nats@sha256:87cf3f8e33ebf28f35575ea083f8feb460d19fa9380d2622c82567ff3fa9d840
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4157918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4eef99b95e572b23f90d60e6e157be90b05ab2f35dbcb10f83f96ece551945a`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 25 Feb 2022 02:58:34 GMT
COPY file:3ee879939ad264e803dd4d6072181d968c4dd0fe076115159f70479c6309ef45 in /nats-server 
# Fri, 25 Feb 2022 02:58:34 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 25 Feb 2022 02:58:35 GMT
EXPOSE 4222 6222 8222
# Fri, 25 Feb 2022 02:58:35 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 25 Feb 2022 02:58:36 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:67a3d8907097b9caffd9d1720b4fb2b1d2ac9dfda60a1d169abbf5494323d50a`  
		Last Modified: Fri, 25 Feb 2022 03:00:58 GMT  
		Size: 4.2 MB (4157409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73f5577f4846f032b281220b897161962481198ead0a1b9ad1d7c76cdd989747`  
		Last Modified: Fri, 25 Feb 2022 03:00:55 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.7.3` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:e970861a260709ae1e8c892eb36758c14323e81959ff4aaa1e9b7327b91d3e70
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.1 MB (4143805 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4414e48026697a15338f28dcb8e46ace9627ea7332559e1708f36ce62a5e327`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 25 Feb 2022 03:01:42 GMT
COPY file:acd11e9a3a86f6f3da079c5155851337e747c3b31481ec05e2dd1e48e23becb2 in /nats-server 
# Fri, 25 Feb 2022 03:01:43 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 25 Feb 2022 03:01:43 GMT
EXPOSE 4222 6222 8222
# Fri, 25 Feb 2022 03:01:44 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 25 Feb 2022 03:01:45 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6ad9fd47af885b43442590ad2c8171e4b4899caef84921ec73ba0540b9c03284`  
		Last Modified: Fri, 25 Feb 2022 03:02:59 GMT  
		Size: 4.1 MB (4143299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02d7667f81936503f26a5ed657cfffdc9add626da8ae5bb78d691054cd3af7c3`  
		Last Modified: Fri, 25 Feb 2022 03:02:59 GMT  
		Size: 506.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.7.3` - windows version 10.0.17763.2565; amd64

```console
$ docker pull nats@sha256:d7c795020fd7295382d503ba883e23cf34ca9c53d6e6b91184bc1fd2bb2c990d
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.6 MB (107634881 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6e99776e94a148ebda875656d07e673c65aedb583986faedb3bdc61a2fd7759`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 02 Feb 2022 19:06:51 GMT
RUN Apply image 1809-amd64
# Wed, 09 Feb 2022 18:13:36 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 25 Feb 2022 02:17:30 GMT
RUN cmd /S /C #(nop) COPY file:d5609a37f534b519fa4326428362ea5398f7165ee90493fb7bdc8b810da33b0e in C:\nats-server.exe 
# Fri, 25 Feb 2022 02:17:31 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Fri, 25 Feb 2022 02:17:32 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Fri, 25 Feb 2022 02:17:33 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 25 Feb 2022 02:17:34 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:bd0b37167cd3d731eb15196e123df7156b5a35597874d3016a1a4298c46fac3f`  
		Size: 103.1 MB (103087119 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8bc49c59cde14e3a9ed8fedce001c00fcb5fe0f9b914aa07273e04f23333d180`  
		Last Modified: Wed, 09 Feb 2022 18:14:28 GMT  
		Size: 1.1 KB (1138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b682f8d539489225b7a3859570b80452b497086f57fa4e6908f2b99d213e1a03`  
		Last Modified: Fri, 25 Feb 2022 03:15:32 GMT  
		Size: 4.5 MB (4541735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67997158a056ea601aec06de195ce0251264a6d8d071f8a44a49a545865ce426`  
		Last Modified: Fri, 25 Feb 2022 03:15:27 GMT  
		Size: 1.7 KB (1656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f873036aacce9bbc35378d6a36985e62919c6d2c9ff526011564a861b86240ab`  
		Last Modified: Fri, 25 Feb 2022 03:15:27 GMT  
		Size: 1.0 KB (1039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf1eace4b7f44dce795499001f62baee27fb477865e490b11d05d198c8e80550`  
		Last Modified: Fri, 25 Feb 2022 03:15:27 GMT  
		Size: 1.1 KB (1081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8accc8a69e6317ee43a53e093f2aef25b70ddff625cfa691d7df28e9bf6d94dc`  
		Last Modified: Fri, 25 Feb 2022 03:15:27 GMT  
		Size: 1.1 KB (1113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.7.3-alpine`

```console
$ docker pull nats@sha256:6944283c7d430ef4d5e23afb87b2a2d9faf963793bcd94b0461bc12def6c74c2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.7.3-alpine` - linux; amd64

```console
$ docker pull nats@sha256:6f8d631c068a9d37845ebee434d2c37606757634b9d8950e8de1035dc68842b4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7591453 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:775ec723ebf4c964b880457f54f66782e850e7121d3264c851da7d58cddb64bc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 24 Nov 2021 20:19:40 GMT
ADD file:9233f6f2237d79659a9521f7e390df217cec49f1a8aa3a12147bbca1956acdb9 in / 
# Wed, 24 Nov 2021 20:19:40 GMT
CMD ["/bin/sh"]
# Fri, 25 Feb 2022 02:21:01 GMT
ENV NATS_SERVER=2.7.3
# Fri, 25 Feb 2022 02:21:04 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='c895169ab34bc21442121f6c885905a254a9351a098402f319b3fbfd1e6225c9' ;; 		armhf) natsArch='arm6'; sha256='1b7e1c5835131825c4007766befd0c96a60edbcc3bc336a6739de5c8affea0c4' ;; 		armv7) natsArch='arm7'; sha256='723290467bc7e95b59ca7238a818932b199b00a21d4e3d7eb0e826b7aba2e0ea' ;; 		x86_64) natsArch='amd64'; sha256='2186c7660cd1d9774421614f6724ad32d7cec2389e39858f227a7991be41b1a7' ;; 		x86) natsArch='386'; sha256='3e8e2841921d555d06c67b1e33fc9bd934e4afec4748f7ddf27c67d707fafea4' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 25 Feb 2022 02:21:04 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 25 Feb 2022 02:21:04 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 25 Feb 2022 02:21:04 GMT
EXPOSE 4222 6222 8222
# Fri, 25 Feb 2022 02:21:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Feb 2022 02:21:05 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:59bf1c3509f33515622619af21ed55bbe26d24913cedbca106468a5fb37a50c3`  
		Last Modified: Wed, 24 Nov 2021 20:20:05 GMT  
		Size: 2.8 MB (2818413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfad251bce41e482876302125c33ef603e0ca99f33d1d274a09af07e1acd1be6`  
		Last Modified: Fri, 25 Feb 2022 02:21:40 GMT  
		Size: 4.8 MB (4772040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8c6f8e0dbab2106f703f51433a684cef43840e5e7443402b474f3c09144a4fe`  
		Last Modified: Fri, 25 Feb 2022 02:21:39 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0d8341c3c348e685617552e338228d15dd937ca0708bd7ab85c3c1b273ed88c`  
		Last Modified: Fri, 25 Feb 2022 02:21:39 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.7.3-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:d6f43ae04309c6115c32d1c71469973712b3e817088a449ce37a9e8cb6b86bf9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7071601 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:846b4c8922b69a90d198633a7b622da89348aa9e3f7f11f58a294e2c4b112a33`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 24 Nov 2021 21:08:16 GMT
ADD file:61137e0aa49ba06f57ac69466fe2fb116f580b5e6159d56f846b1d72c4a3c814 in / 
# Wed, 24 Nov 2021 21:08:16 GMT
CMD ["/bin/sh"]
# Fri, 25 Feb 2022 02:49:34 GMT
ENV NATS_SERVER=2.7.3
# Fri, 25 Feb 2022 02:49:38 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='c895169ab34bc21442121f6c885905a254a9351a098402f319b3fbfd1e6225c9' ;; 		armhf) natsArch='arm6'; sha256='1b7e1c5835131825c4007766befd0c96a60edbcc3bc336a6739de5c8affea0c4' ;; 		armv7) natsArch='arm7'; sha256='723290467bc7e95b59ca7238a818932b199b00a21d4e3d7eb0e826b7aba2e0ea' ;; 		x86_64) natsArch='amd64'; sha256='2186c7660cd1d9774421614f6724ad32d7cec2389e39858f227a7991be41b1a7' ;; 		x86) natsArch='386'; sha256='3e8e2841921d555d06c67b1e33fc9bd934e4afec4748f7ddf27c67d707fafea4' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 25 Feb 2022 02:49:38 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 25 Feb 2022 02:49:39 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 25 Feb 2022 02:49:39 GMT
EXPOSE 4222 6222 8222
# Fri, 25 Feb 2022 02:49:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Feb 2022 02:49:40 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:e4a43de54da9e309482f6762f0c11f5f547cd8fd61a49c5f158453066162023e`  
		Last Modified: Wed, 24 Nov 2021 21:09:46 GMT  
		Size: 2.6 MB (2631421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ecb484648e454aaf42c41938db64a0715cb509a90811b5912192d2e66a2f7fb`  
		Last Modified: Fri, 25 Feb 2022 02:51:52 GMT  
		Size: 4.4 MB (4439176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdd675987846849cf3247fbc41b25505410823bffd30e841e7f663936458e553`  
		Last Modified: Fri, 25 Feb 2022 02:51:49 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ae450e4bdcdcad0dc3e04a43f8855409627f6c7fdecd22f661dbfe3a99530d2`  
		Last Modified: Fri, 25 Feb 2022 02:51:49 GMT  
		Size: 417.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.7.3-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:665c6221a3c009747c340953834a8e1c6e38008d728f3a9d4d4eaab76e8e640d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.9 MB (6865015 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f23f21c3235ba9d61b53aeb161021b62412dc690dd81727439de14a1f9b902eb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 24 Nov 2021 21:42:11 GMT
ADD file:ca436da5b0bfc9c0e2fc685533c6628918000c8fff109fe9a8da625b9a798002 in / 
# Wed, 24 Nov 2021 21:42:11 GMT
CMD ["/bin/sh"]
# Fri, 25 Feb 2022 02:57:52 GMT
ENV NATS_SERVER=2.7.3
# Fri, 25 Feb 2022 02:57:56 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='c895169ab34bc21442121f6c885905a254a9351a098402f319b3fbfd1e6225c9' ;; 		armhf) natsArch='arm6'; sha256='1b7e1c5835131825c4007766befd0c96a60edbcc3bc336a6739de5c8affea0c4' ;; 		armv7) natsArch='arm7'; sha256='723290467bc7e95b59ca7238a818932b199b00a21d4e3d7eb0e826b7aba2e0ea' ;; 		x86_64) natsArch='amd64'; sha256='2186c7660cd1d9774421614f6724ad32d7cec2389e39858f227a7991be41b1a7' ;; 		x86) natsArch='386'; sha256='3e8e2841921d555d06c67b1e33fc9bd934e4afec4748f7ddf27c67d707fafea4' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 25 Feb 2022 02:57:57 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 25 Feb 2022 02:57:57 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 25 Feb 2022 02:57:58 GMT
EXPOSE 4222 6222 8222
# Fri, 25 Feb 2022 02:57:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Feb 2022 02:57:58 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:5480d2ca1740c20ce17652e01ed2265cdc914458acd41256a2b1ccff28f2762c`  
		Last Modified: Wed, 24 Nov 2021 21:43:40 GMT  
		Size: 2.4 MB (2434764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fafd4ba596baa033665a46ce765df0c4a928784832ecc5645944032cfcd9295`  
		Last Modified: Fri, 25 Feb 2022 03:00:20 GMT  
		Size: 4.4 MB (4429250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abb2edff52bc9250fdec4032d39728784d4495539ef65cceed401a8968ec2df5`  
		Last Modified: Fri, 25 Feb 2022 03:00:18 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1047f2aa448d4163e2995aed662d6890fdd3954289a1ff2908edc894450b3d78`  
		Last Modified: Fri, 25 Feb 2022 03:00:18 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.7.3-alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:8f79d8af0b084884d2cc9641a33a1274022fc51b99e955d3f13d9c45f47cf6b4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7132810 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e50bb490b2ac0a89152a29fc28e269300b6b83d2a85c0ce5ebe74635c34cdb0d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 24 Nov 2021 20:39:20 GMT
ADD file:df53811312284306901fdaaff0a357a4bf40d631e662fe9ce6d342442e494b6c in / 
# Wed, 24 Nov 2021 20:39:20 GMT
CMD ["/bin/sh"]
# Fri, 25 Feb 2022 03:01:24 GMT
ENV NATS_SERVER=2.7.3
# Fri, 25 Feb 2022 03:01:26 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='c895169ab34bc21442121f6c885905a254a9351a098402f319b3fbfd1e6225c9' ;; 		armhf) natsArch='arm6'; sha256='1b7e1c5835131825c4007766befd0c96a60edbcc3bc336a6739de5c8affea0c4' ;; 		armv7) natsArch='arm7'; sha256='723290467bc7e95b59ca7238a818932b199b00a21d4e3d7eb0e826b7aba2e0ea' ;; 		x86_64) natsArch='amd64'; sha256='2186c7660cd1d9774421614f6724ad32d7cec2389e39858f227a7991be41b1a7' ;; 		x86) natsArch='386'; sha256='3e8e2841921d555d06c67b1e33fc9bd934e4afec4748f7ddf27c67d707fafea4' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 25 Feb 2022 03:01:28 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 25 Feb 2022 03:01:29 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 25 Feb 2022 03:01:29 GMT
EXPOSE 4222 6222 8222
# Fri, 25 Feb 2022 03:01:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Feb 2022 03:01:31 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9b3977197b4f2147bdd31e1271f811319dcd5c2fc595f14e81f5351ab6275b99`  
		Last Modified: Wed, 24 Nov 2021 20:39:59 GMT  
		Size: 2.7 MB (2715434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c75ed4d21bde940c8f5b4d0d82b44c31489bd5a37d46b1f197b7d1baed0b6e8`  
		Last Modified: Fri, 25 Feb 2022 03:02:31 GMT  
		Size: 4.4 MB (4416403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f7dd0d82f2c731b21df156c69326c651274a35eb010b23b5150397309110717`  
		Last Modified: Fri, 25 Feb 2022 03:02:30 GMT  
		Size: 559.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f29d0f81d7bbfb90bc5607be41aabbd3e970b1e74e19a069c23e863092772ba`  
		Last Modified: Fri, 25 Feb 2022 03:02:30 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.7.3-alpine3.15`

```console
$ docker pull nats@sha256:6944283c7d430ef4d5e23afb87b2a2d9faf963793bcd94b0461bc12def6c74c2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.7.3-alpine3.15` - linux; amd64

```console
$ docker pull nats@sha256:6f8d631c068a9d37845ebee434d2c37606757634b9d8950e8de1035dc68842b4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7591453 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:775ec723ebf4c964b880457f54f66782e850e7121d3264c851da7d58cddb64bc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 24 Nov 2021 20:19:40 GMT
ADD file:9233f6f2237d79659a9521f7e390df217cec49f1a8aa3a12147bbca1956acdb9 in / 
# Wed, 24 Nov 2021 20:19:40 GMT
CMD ["/bin/sh"]
# Fri, 25 Feb 2022 02:21:01 GMT
ENV NATS_SERVER=2.7.3
# Fri, 25 Feb 2022 02:21:04 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='c895169ab34bc21442121f6c885905a254a9351a098402f319b3fbfd1e6225c9' ;; 		armhf) natsArch='arm6'; sha256='1b7e1c5835131825c4007766befd0c96a60edbcc3bc336a6739de5c8affea0c4' ;; 		armv7) natsArch='arm7'; sha256='723290467bc7e95b59ca7238a818932b199b00a21d4e3d7eb0e826b7aba2e0ea' ;; 		x86_64) natsArch='amd64'; sha256='2186c7660cd1d9774421614f6724ad32d7cec2389e39858f227a7991be41b1a7' ;; 		x86) natsArch='386'; sha256='3e8e2841921d555d06c67b1e33fc9bd934e4afec4748f7ddf27c67d707fafea4' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 25 Feb 2022 02:21:04 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 25 Feb 2022 02:21:04 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 25 Feb 2022 02:21:04 GMT
EXPOSE 4222 6222 8222
# Fri, 25 Feb 2022 02:21:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Feb 2022 02:21:05 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:59bf1c3509f33515622619af21ed55bbe26d24913cedbca106468a5fb37a50c3`  
		Last Modified: Wed, 24 Nov 2021 20:20:05 GMT  
		Size: 2.8 MB (2818413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfad251bce41e482876302125c33ef603e0ca99f33d1d274a09af07e1acd1be6`  
		Last Modified: Fri, 25 Feb 2022 02:21:40 GMT  
		Size: 4.8 MB (4772040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8c6f8e0dbab2106f703f51433a684cef43840e5e7443402b474f3c09144a4fe`  
		Last Modified: Fri, 25 Feb 2022 02:21:39 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0d8341c3c348e685617552e338228d15dd937ca0708bd7ab85c3c1b273ed88c`  
		Last Modified: Fri, 25 Feb 2022 02:21:39 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.7.3-alpine3.15` - linux; arm variant v6

```console
$ docker pull nats@sha256:d6f43ae04309c6115c32d1c71469973712b3e817088a449ce37a9e8cb6b86bf9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7071601 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:846b4c8922b69a90d198633a7b622da89348aa9e3f7f11f58a294e2c4b112a33`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 24 Nov 2021 21:08:16 GMT
ADD file:61137e0aa49ba06f57ac69466fe2fb116f580b5e6159d56f846b1d72c4a3c814 in / 
# Wed, 24 Nov 2021 21:08:16 GMT
CMD ["/bin/sh"]
# Fri, 25 Feb 2022 02:49:34 GMT
ENV NATS_SERVER=2.7.3
# Fri, 25 Feb 2022 02:49:38 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='c895169ab34bc21442121f6c885905a254a9351a098402f319b3fbfd1e6225c9' ;; 		armhf) natsArch='arm6'; sha256='1b7e1c5835131825c4007766befd0c96a60edbcc3bc336a6739de5c8affea0c4' ;; 		armv7) natsArch='arm7'; sha256='723290467bc7e95b59ca7238a818932b199b00a21d4e3d7eb0e826b7aba2e0ea' ;; 		x86_64) natsArch='amd64'; sha256='2186c7660cd1d9774421614f6724ad32d7cec2389e39858f227a7991be41b1a7' ;; 		x86) natsArch='386'; sha256='3e8e2841921d555d06c67b1e33fc9bd934e4afec4748f7ddf27c67d707fafea4' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 25 Feb 2022 02:49:38 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 25 Feb 2022 02:49:39 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 25 Feb 2022 02:49:39 GMT
EXPOSE 4222 6222 8222
# Fri, 25 Feb 2022 02:49:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Feb 2022 02:49:40 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:e4a43de54da9e309482f6762f0c11f5f547cd8fd61a49c5f158453066162023e`  
		Last Modified: Wed, 24 Nov 2021 21:09:46 GMT  
		Size: 2.6 MB (2631421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ecb484648e454aaf42c41938db64a0715cb509a90811b5912192d2e66a2f7fb`  
		Last Modified: Fri, 25 Feb 2022 02:51:52 GMT  
		Size: 4.4 MB (4439176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdd675987846849cf3247fbc41b25505410823bffd30e841e7f663936458e553`  
		Last Modified: Fri, 25 Feb 2022 02:51:49 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ae450e4bdcdcad0dc3e04a43f8855409627f6c7fdecd22f661dbfe3a99530d2`  
		Last Modified: Fri, 25 Feb 2022 02:51:49 GMT  
		Size: 417.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.7.3-alpine3.15` - linux; arm variant v7

```console
$ docker pull nats@sha256:665c6221a3c009747c340953834a8e1c6e38008d728f3a9d4d4eaab76e8e640d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.9 MB (6865015 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f23f21c3235ba9d61b53aeb161021b62412dc690dd81727439de14a1f9b902eb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 24 Nov 2021 21:42:11 GMT
ADD file:ca436da5b0bfc9c0e2fc685533c6628918000c8fff109fe9a8da625b9a798002 in / 
# Wed, 24 Nov 2021 21:42:11 GMT
CMD ["/bin/sh"]
# Fri, 25 Feb 2022 02:57:52 GMT
ENV NATS_SERVER=2.7.3
# Fri, 25 Feb 2022 02:57:56 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='c895169ab34bc21442121f6c885905a254a9351a098402f319b3fbfd1e6225c9' ;; 		armhf) natsArch='arm6'; sha256='1b7e1c5835131825c4007766befd0c96a60edbcc3bc336a6739de5c8affea0c4' ;; 		armv7) natsArch='arm7'; sha256='723290467bc7e95b59ca7238a818932b199b00a21d4e3d7eb0e826b7aba2e0ea' ;; 		x86_64) natsArch='amd64'; sha256='2186c7660cd1d9774421614f6724ad32d7cec2389e39858f227a7991be41b1a7' ;; 		x86) natsArch='386'; sha256='3e8e2841921d555d06c67b1e33fc9bd934e4afec4748f7ddf27c67d707fafea4' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 25 Feb 2022 02:57:57 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 25 Feb 2022 02:57:57 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 25 Feb 2022 02:57:58 GMT
EXPOSE 4222 6222 8222
# Fri, 25 Feb 2022 02:57:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Feb 2022 02:57:58 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:5480d2ca1740c20ce17652e01ed2265cdc914458acd41256a2b1ccff28f2762c`  
		Last Modified: Wed, 24 Nov 2021 21:43:40 GMT  
		Size: 2.4 MB (2434764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fafd4ba596baa033665a46ce765df0c4a928784832ecc5645944032cfcd9295`  
		Last Modified: Fri, 25 Feb 2022 03:00:20 GMT  
		Size: 4.4 MB (4429250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abb2edff52bc9250fdec4032d39728784d4495539ef65cceed401a8968ec2df5`  
		Last Modified: Fri, 25 Feb 2022 03:00:18 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1047f2aa448d4163e2995aed662d6890fdd3954289a1ff2908edc894450b3d78`  
		Last Modified: Fri, 25 Feb 2022 03:00:18 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.7.3-alpine3.15` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:8f79d8af0b084884d2cc9641a33a1274022fc51b99e955d3f13d9c45f47cf6b4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7132810 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e50bb490b2ac0a89152a29fc28e269300b6b83d2a85c0ce5ebe74635c34cdb0d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 24 Nov 2021 20:39:20 GMT
ADD file:df53811312284306901fdaaff0a357a4bf40d631e662fe9ce6d342442e494b6c in / 
# Wed, 24 Nov 2021 20:39:20 GMT
CMD ["/bin/sh"]
# Fri, 25 Feb 2022 03:01:24 GMT
ENV NATS_SERVER=2.7.3
# Fri, 25 Feb 2022 03:01:26 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='c895169ab34bc21442121f6c885905a254a9351a098402f319b3fbfd1e6225c9' ;; 		armhf) natsArch='arm6'; sha256='1b7e1c5835131825c4007766befd0c96a60edbcc3bc336a6739de5c8affea0c4' ;; 		armv7) natsArch='arm7'; sha256='723290467bc7e95b59ca7238a818932b199b00a21d4e3d7eb0e826b7aba2e0ea' ;; 		x86_64) natsArch='amd64'; sha256='2186c7660cd1d9774421614f6724ad32d7cec2389e39858f227a7991be41b1a7' ;; 		x86) natsArch='386'; sha256='3e8e2841921d555d06c67b1e33fc9bd934e4afec4748f7ddf27c67d707fafea4' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 25 Feb 2022 03:01:28 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 25 Feb 2022 03:01:29 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 25 Feb 2022 03:01:29 GMT
EXPOSE 4222 6222 8222
# Fri, 25 Feb 2022 03:01:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Feb 2022 03:01:31 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9b3977197b4f2147bdd31e1271f811319dcd5c2fc595f14e81f5351ab6275b99`  
		Last Modified: Wed, 24 Nov 2021 20:39:59 GMT  
		Size: 2.7 MB (2715434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c75ed4d21bde940c8f5b4d0d82b44c31489bd5a37d46b1f197b7d1baed0b6e8`  
		Last Modified: Fri, 25 Feb 2022 03:02:31 GMT  
		Size: 4.4 MB (4416403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f7dd0d82f2c731b21df156c69326c651274a35eb010b23b5150397309110717`  
		Last Modified: Fri, 25 Feb 2022 03:02:30 GMT  
		Size: 559.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f29d0f81d7bbfb90bc5607be41aabbd3e970b1e74e19a069c23e863092772ba`  
		Last Modified: Fri, 25 Feb 2022 03:02:30 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.7.3-linux`

```console
$ docker pull nats@sha256:4fe2c16e211795858e7e7538197ec57f67ed6e9ca5d91d06d925e09ec6724d3b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.7.3-linux` - linux; amd64

```console
$ docker pull nats@sha256:5fd249efa75cf3eb595342175207fdbb390eee3034f7fe49355d7a479fa3ffe2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4499407 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c84de17b17b3458d2b6e6d4264ea6186c82bab718ca058f5d7738e53ca2759ac`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 25 Feb 2022 02:21:13 GMT
COPY file:8a814b0c66a47e63e5a7f4287478948812fe6e03c224d539f37ce3f950d2b6c6 in /nats-server 
# Fri, 25 Feb 2022 02:21:13 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 25 Feb 2022 02:21:14 GMT
EXPOSE 4222 6222 8222
# Fri, 25 Feb 2022 02:21:14 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 25 Feb 2022 02:21:14 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:277fae1baf41821774f7a2e1c3f465b28aa8693ee0cd77e0ad0bace55d9c616e`  
		Last Modified: Fri, 25 Feb 2022 02:22:04 GMT  
		Size: 4.5 MB (4498900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb932b4b3fbc873b56e996c6357055bb7700c701d17d7d87cdec31211142b49a`  
		Last Modified: Fri, 25 Feb 2022 02:22:03 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.7.3-linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:2e3339e7e8d98e7bbab0613c7b7c3dd6f51fcf33ed3910a2e65e62fba7049337
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4165977 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ddc7bcc78dd550ace4def82e3db227e618d77e136274749f3bf55869e64be264`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 25 Feb 2022 02:50:06 GMT
COPY file:3a951d885f7bcec693f6fbf26a9ffd82b0c6218b6834fc6053e5812f7451b63e in /nats-server 
# Fri, 25 Feb 2022 02:50:06 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 25 Feb 2022 02:50:07 GMT
EXPOSE 4222 6222 8222
# Fri, 25 Feb 2022 02:50:07 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 25 Feb 2022 02:50:07 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:f6de87b4530f922b11edc08be8edeebc6ce0cb666907013348d4e1b9f5d51809`  
		Last Modified: Fri, 25 Feb 2022 02:52:29 GMT  
		Size: 4.2 MB (4165468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5fa68b52226484e5870677184cdc47c93a7d453f334c144b5cb631346bc8111`  
		Last Modified: Fri, 25 Feb 2022 02:52:27 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.7.3-linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:87cf3f8e33ebf28f35575ea083f8feb460d19fa9380d2622c82567ff3fa9d840
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4157918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4eef99b95e572b23f90d60e6e157be90b05ab2f35dbcb10f83f96ece551945a`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 25 Feb 2022 02:58:34 GMT
COPY file:3ee879939ad264e803dd4d6072181d968c4dd0fe076115159f70479c6309ef45 in /nats-server 
# Fri, 25 Feb 2022 02:58:34 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 25 Feb 2022 02:58:35 GMT
EXPOSE 4222 6222 8222
# Fri, 25 Feb 2022 02:58:35 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 25 Feb 2022 02:58:36 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:67a3d8907097b9caffd9d1720b4fb2b1d2ac9dfda60a1d169abbf5494323d50a`  
		Last Modified: Fri, 25 Feb 2022 03:00:58 GMT  
		Size: 4.2 MB (4157409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73f5577f4846f032b281220b897161962481198ead0a1b9ad1d7c76cdd989747`  
		Last Modified: Fri, 25 Feb 2022 03:00:55 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.7.3-linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:e970861a260709ae1e8c892eb36758c14323e81959ff4aaa1e9b7327b91d3e70
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.1 MB (4143805 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4414e48026697a15338f28dcb8e46ace9627ea7332559e1708f36ce62a5e327`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 25 Feb 2022 03:01:42 GMT
COPY file:acd11e9a3a86f6f3da079c5155851337e747c3b31481ec05e2dd1e48e23becb2 in /nats-server 
# Fri, 25 Feb 2022 03:01:43 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 25 Feb 2022 03:01:43 GMT
EXPOSE 4222 6222 8222
# Fri, 25 Feb 2022 03:01:44 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 25 Feb 2022 03:01:45 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6ad9fd47af885b43442590ad2c8171e4b4899caef84921ec73ba0540b9c03284`  
		Last Modified: Fri, 25 Feb 2022 03:02:59 GMT  
		Size: 4.1 MB (4143299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02d7667f81936503f26a5ed657cfffdc9add626da8ae5bb78d691054cd3af7c3`  
		Last Modified: Fri, 25 Feb 2022 03:02:59 GMT  
		Size: 506.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.7.3-nanoserver`

```console
$ docker pull nats@sha256:6e43eecf010598596b218f3800a6d052426d875695ead9cdbf074e0653772142
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2565; amd64

### `nats:2.7.3-nanoserver` - windows version 10.0.17763.2565; amd64

```console
$ docker pull nats@sha256:d7c795020fd7295382d503ba883e23cf34ca9c53d6e6b91184bc1fd2bb2c990d
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.6 MB (107634881 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6e99776e94a148ebda875656d07e673c65aedb583986faedb3bdc61a2fd7759`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 02 Feb 2022 19:06:51 GMT
RUN Apply image 1809-amd64
# Wed, 09 Feb 2022 18:13:36 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 25 Feb 2022 02:17:30 GMT
RUN cmd /S /C #(nop) COPY file:d5609a37f534b519fa4326428362ea5398f7165ee90493fb7bdc8b810da33b0e in C:\nats-server.exe 
# Fri, 25 Feb 2022 02:17:31 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Fri, 25 Feb 2022 02:17:32 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Fri, 25 Feb 2022 02:17:33 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 25 Feb 2022 02:17:34 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:bd0b37167cd3d731eb15196e123df7156b5a35597874d3016a1a4298c46fac3f`  
		Size: 103.1 MB (103087119 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8bc49c59cde14e3a9ed8fedce001c00fcb5fe0f9b914aa07273e04f23333d180`  
		Last Modified: Wed, 09 Feb 2022 18:14:28 GMT  
		Size: 1.1 KB (1138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b682f8d539489225b7a3859570b80452b497086f57fa4e6908f2b99d213e1a03`  
		Last Modified: Fri, 25 Feb 2022 03:15:32 GMT  
		Size: 4.5 MB (4541735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67997158a056ea601aec06de195ce0251264a6d8d071f8a44a49a545865ce426`  
		Last Modified: Fri, 25 Feb 2022 03:15:27 GMT  
		Size: 1.7 KB (1656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f873036aacce9bbc35378d6a36985e62919c6d2c9ff526011564a861b86240ab`  
		Last Modified: Fri, 25 Feb 2022 03:15:27 GMT  
		Size: 1.0 KB (1039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf1eace4b7f44dce795499001f62baee27fb477865e490b11d05d198c8e80550`  
		Last Modified: Fri, 25 Feb 2022 03:15:27 GMT  
		Size: 1.1 KB (1081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8accc8a69e6317ee43a53e093f2aef25b70ddff625cfa691d7df28e9bf6d94dc`  
		Last Modified: Fri, 25 Feb 2022 03:15:27 GMT  
		Size: 1.1 KB (1113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.7.3-nanoserver-1809`

```console
$ docker pull nats@sha256:6e43eecf010598596b218f3800a6d052426d875695ead9cdbf074e0653772142
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2565; amd64

### `nats:2.7.3-nanoserver-1809` - windows version 10.0.17763.2565; amd64

```console
$ docker pull nats@sha256:d7c795020fd7295382d503ba883e23cf34ca9c53d6e6b91184bc1fd2bb2c990d
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.6 MB (107634881 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6e99776e94a148ebda875656d07e673c65aedb583986faedb3bdc61a2fd7759`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 02 Feb 2022 19:06:51 GMT
RUN Apply image 1809-amd64
# Wed, 09 Feb 2022 18:13:36 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 25 Feb 2022 02:17:30 GMT
RUN cmd /S /C #(nop) COPY file:d5609a37f534b519fa4326428362ea5398f7165ee90493fb7bdc8b810da33b0e in C:\nats-server.exe 
# Fri, 25 Feb 2022 02:17:31 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Fri, 25 Feb 2022 02:17:32 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Fri, 25 Feb 2022 02:17:33 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 25 Feb 2022 02:17:34 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:bd0b37167cd3d731eb15196e123df7156b5a35597874d3016a1a4298c46fac3f`  
		Size: 103.1 MB (103087119 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8bc49c59cde14e3a9ed8fedce001c00fcb5fe0f9b914aa07273e04f23333d180`  
		Last Modified: Wed, 09 Feb 2022 18:14:28 GMT  
		Size: 1.1 KB (1138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b682f8d539489225b7a3859570b80452b497086f57fa4e6908f2b99d213e1a03`  
		Last Modified: Fri, 25 Feb 2022 03:15:32 GMT  
		Size: 4.5 MB (4541735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67997158a056ea601aec06de195ce0251264a6d8d071f8a44a49a545865ce426`  
		Last Modified: Fri, 25 Feb 2022 03:15:27 GMT  
		Size: 1.7 KB (1656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f873036aacce9bbc35378d6a36985e62919c6d2c9ff526011564a861b86240ab`  
		Last Modified: Fri, 25 Feb 2022 03:15:27 GMT  
		Size: 1.0 KB (1039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf1eace4b7f44dce795499001f62baee27fb477865e490b11d05d198c8e80550`  
		Last Modified: Fri, 25 Feb 2022 03:15:27 GMT  
		Size: 1.1 KB (1081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8accc8a69e6317ee43a53e093f2aef25b70ddff625cfa691d7df28e9bf6d94dc`  
		Last Modified: Fri, 25 Feb 2022 03:15:27 GMT  
		Size: 1.1 KB (1113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.7.3-scratch`

```console
$ docker pull nats@sha256:4fe2c16e211795858e7e7538197ec57f67ed6e9ca5d91d06d925e09ec6724d3b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.7.3-scratch` - linux; amd64

```console
$ docker pull nats@sha256:5fd249efa75cf3eb595342175207fdbb390eee3034f7fe49355d7a479fa3ffe2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4499407 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c84de17b17b3458d2b6e6d4264ea6186c82bab718ca058f5d7738e53ca2759ac`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 25 Feb 2022 02:21:13 GMT
COPY file:8a814b0c66a47e63e5a7f4287478948812fe6e03c224d539f37ce3f950d2b6c6 in /nats-server 
# Fri, 25 Feb 2022 02:21:13 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 25 Feb 2022 02:21:14 GMT
EXPOSE 4222 6222 8222
# Fri, 25 Feb 2022 02:21:14 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 25 Feb 2022 02:21:14 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:277fae1baf41821774f7a2e1c3f465b28aa8693ee0cd77e0ad0bace55d9c616e`  
		Last Modified: Fri, 25 Feb 2022 02:22:04 GMT  
		Size: 4.5 MB (4498900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb932b4b3fbc873b56e996c6357055bb7700c701d17d7d87cdec31211142b49a`  
		Last Modified: Fri, 25 Feb 2022 02:22:03 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.7.3-scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:2e3339e7e8d98e7bbab0613c7b7c3dd6f51fcf33ed3910a2e65e62fba7049337
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4165977 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ddc7bcc78dd550ace4def82e3db227e618d77e136274749f3bf55869e64be264`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 25 Feb 2022 02:50:06 GMT
COPY file:3a951d885f7bcec693f6fbf26a9ffd82b0c6218b6834fc6053e5812f7451b63e in /nats-server 
# Fri, 25 Feb 2022 02:50:06 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 25 Feb 2022 02:50:07 GMT
EXPOSE 4222 6222 8222
# Fri, 25 Feb 2022 02:50:07 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 25 Feb 2022 02:50:07 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:f6de87b4530f922b11edc08be8edeebc6ce0cb666907013348d4e1b9f5d51809`  
		Last Modified: Fri, 25 Feb 2022 02:52:29 GMT  
		Size: 4.2 MB (4165468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5fa68b52226484e5870677184cdc47c93a7d453f334c144b5cb631346bc8111`  
		Last Modified: Fri, 25 Feb 2022 02:52:27 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.7.3-scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:87cf3f8e33ebf28f35575ea083f8feb460d19fa9380d2622c82567ff3fa9d840
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4157918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4eef99b95e572b23f90d60e6e157be90b05ab2f35dbcb10f83f96ece551945a`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 25 Feb 2022 02:58:34 GMT
COPY file:3ee879939ad264e803dd4d6072181d968c4dd0fe076115159f70479c6309ef45 in /nats-server 
# Fri, 25 Feb 2022 02:58:34 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 25 Feb 2022 02:58:35 GMT
EXPOSE 4222 6222 8222
# Fri, 25 Feb 2022 02:58:35 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 25 Feb 2022 02:58:36 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:67a3d8907097b9caffd9d1720b4fb2b1d2ac9dfda60a1d169abbf5494323d50a`  
		Last Modified: Fri, 25 Feb 2022 03:00:58 GMT  
		Size: 4.2 MB (4157409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73f5577f4846f032b281220b897161962481198ead0a1b9ad1d7c76cdd989747`  
		Last Modified: Fri, 25 Feb 2022 03:00:55 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.7.3-scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:e970861a260709ae1e8c892eb36758c14323e81959ff4aaa1e9b7327b91d3e70
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.1 MB (4143805 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4414e48026697a15338f28dcb8e46ace9627ea7332559e1708f36ce62a5e327`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 25 Feb 2022 03:01:42 GMT
COPY file:acd11e9a3a86f6f3da079c5155851337e747c3b31481ec05e2dd1e48e23becb2 in /nats-server 
# Fri, 25 Feb 2022 03:01:43 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 25 Feb 2022 03:01:43 GMT
EXPOSE 4222 6222 8222
# Fri, 25 Feb 2022 03:01:44 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 25 Feb 2022 03:01:45 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6ad9fd47af885b43442590ad2c8171e4b4899caef84921ec73ba0540b9c03284`  
		Last Modified: Fri, 25 Feb 2022 03:02:59 GMT  
		Size: 4.1 MB (4143299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02d7667f81936503f26a5ed657cfffdc9add626da8ae5bb78d691054cd3af7c3`  
		Last Modified: Fri, 25 Feb 2022 03:02:59 GMT  
		Size: 506.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.7.3-windowsservercore`

```console
$ docker pull nats@sha256:2b9c20408baf29df9d8666fc894d8a5c308946331d4310ef5a82b1eed5101db3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2565; amd64

### `nats:2.7.3-windowsservercore` - windows version 10.0.17763.2565; amd64

```console
$ docker pull nats@sha256:ac025e7ac0a2786f5807888399f94d317a0636b60e8a37584569d586fb1ac146
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2718991955 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:007419288bb7b16cd78d29d0476687df2d88011775f13b3f565c92414a214c05`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Wed, 02 Feb 2022 19:28:56 GMT
RUN Install update 1809-amd64
# Wed, 09 Feb 2022 15:04:17 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Feb 2022 18:10:54 GMT
ENV NATS_DOCKERIZED=1
# Fri, 25 Feb 2022 02:14:46 GMT
ENV NATS_SERVER=2.7.3
# Fri, 25 Feb 2022 02:14:47 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.7.3/nats-server-v2.7.3-windows-amd64.zip
# Fri, 25 Feb 2022 02:14:48 GMT
ENV NATS_SERVER_SHASUM=ddb372da68741d897006c8d4b160c7f4788603cbaacb3fa105ddf7baada04428
# Fri, 25 Feb 2022 02:15:50 GMT
RUN Set-PSDebug -Trace 2
# Fri, 25 Feb 2022 02:17:14 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 25 Feb 2022 02:17:16 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Fri, 25 Feb 2022 02:17:17 GMT
EXPOSE 4222 6222 8222
# Fri, 25 Feb 2022 02:17:18 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 25 Feb 2022 02:17:19 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:1bd78008c728d8f9e56dc2093e6eb55f0f0b1aa96e5d0c7ccc830c5f60876cdf`  
		Size: 995.4 MB (995381853 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f49d3791198cf2ea875fd54ce3bb715670742d4a58c00252395ad1b74036662a`  
		Last Modified: Wed, 09 Feb 2022 16:39:51 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4235aeeb4e8b577cc7aa26c7994ec94c94dd53a38764fc510b330b77cef4abad`  
		Last Modified: Wed, 09 Feb 2022 18:14:09 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6ed63a799d34b3a151eb2d65afc4a93d028c5308ce305f9059da19083ea4579`  
		Last Modified: Fri, 25 Feb 2022 03:15:11 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fa36020fa0fadcfe9ac785f1bc4cbf6e51ac336a4441d2ea628465f9f1e3832`  
		Last Modified: Fri, 25 Feb 2022 03:15:11 GMT  
		Size: 1.3 KB (1321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58aaa8ed102560150d8bd4fe887000c2789a69df5ae550a8b8058e526d01af34`  
		Last Modified: Fri, 25 Feb 2022 03:15:11 GMT  
		Size: 1.3 KB (1300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e48afd20cc6576c9f831f4166f86f4cd65be8140eda5a57159bba0d62c21b1af`  
		Last Modified: Fri, 25 Feb 2022 03:15:12 GMT  
		Size: 374.3 KB (374309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1eb76be5e45618d5a45f4672ac8e8c8d45d10bf627dc47f3afe45c7909b223b`  
		Last Modified: Fri, 25 Feb 2022 03:15:10 GMT  
		Size: 4.9 MB (4890363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:513928aafbffc4a16807de347507df4019d3096da02f3475f8731f6704a0e75d`  
		Last Modified: Fri, 25 Feb 2022 03:15:09 GMT  
		Size: 1.9 KB (1884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6ba5e5368daffd340a50b6715a6d9d28d2f2c341d694c5d7cdae52e15e46d4d`  
		Last Modified: Fri, 25 Feb 2022 03:15:09 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca864d6530840f9fbdc99b6aaedcd8aa7acf319697677ca480fd220d426cb62f`  
		Last Modified: Fri, 25 Feb 2022 03:15:09 GMT  
		Size: 1.3 KB (1322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e9cb037cabf38f35bdcf375e13b7790bfdc9b4e9761cd2e865cf557a7575e81`  
		Last Modified: Fri, 25 Feb 2022 03:15:09 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.7.3-windowsservercore-1809`

```console
$ docker pull nats@sha256:2b9c20408baf29df9d8666fc894d8a5c308946331d4310ef5a82b1eed5101db3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2565; amd64

### `nats:2.7.3-windowsservercore-1809` - windows version 10.0.17763.2565; amd64

```console
$ docker pull nats@sha256:ac025e7ac0a2786f5807888399f94d317a0636b60e8a37584569d586fb1ac146
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2718991955 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:007419288bb7b16cd78d29d0476687df2d88011775f13b3f565c92414a214c05`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Wed, 02 Feb 2022 19:28:56 GMT
RUN Install update 1809-amd64
# Wed, 09 Feb 2022 15:04:17 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Feb 2022 18:10:54 GMT
ENV NATS_DOCKERIZED=1
# Fri, 25 Feb 2022 02:14:46 GMT
ENV NATS_SERVER=2.7.3
# Fri, 25 Feb 2022 02:14:47 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.7.3/nats-server-v2.7.3-windows-amd64.zip
# Fri, 25 Feb 2022 02:14:48 GMT
ENV NATS_SERVER_SHASUM=ddb372da68741d897006c8d4b160c7f4788603cbaacb3fa105ddf7baada04428
# Fri, 25 Feb 2022 02:15:50 GMT
RUN Set-PSDebug -Trace 2
# Fri, 25 Feb 2022 02:17:14 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 25 Feb 2022 02:17:16 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Fri, 25 Feb 2022 02:17:17 GMT
EXPOSE 4222 6222 8222
# Fri, 25 Feb 2022 02:17:18 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 25 Feb 2022 02:17:19 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:1bd78008c728d8f9e56dc2093e6eb55f0f0b1aa96e5d0c7ccc830c5f60876cdf`  
		Size: 995.4 MB (995381853 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f49d3791198cf2ea875fd54ce3bb715670742d4a58c00252395ad1b74036662a`  
		Last Modified: Wed, 09 Feb 2022 16:39:51 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4235aeeb4e8b577cc7aa26c7994ec94c94dd53a38764fc510b330b77cef4abad`  
		Last Modified: Wed, 09 Feb 2022 18:14:09 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6ed63a799d34b3a151eb2d65afc4a93d028c5308ce305f9059da19083ea4579`  
		Last Modified: Fri, 25 Feb 2022 03:15:11 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fa36020fa0fadcfe9ac785f1bc4cbf6e51ac336a4441d2ea628465f9f1e3832`  
		Last Modified: Fri, 25 Feb 2022 03:15:11 GMT  
		Size: 1.3 KB (1321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58aaa8ed102560150d8bd4fe887000c2789a69df5ae550a8b8058e526d01af34`  
		Last Modified: Fri, 25 Feb 2022 03:15:11 GMT  
		Size: 1.3 KB (1300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e48afd20cc6576c9f831f4166f86f4cd65be8140eda5a57159bba0d62c21b1af`  
		Last Modified: Fri, 25 Feb 2022 03:15:12 GMT  
		Size: 374.3 KB (374309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1eb76be5e45618d5a45f4672ac8e8c8d45d10bf627dc47f3afe45c7909b223b`  
		Last Modified: Fri, 25 Feb 2022 03:15:10 GMT  
		Size: 4.9 MB (4890363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:513928aafbffc4a16807de347507df4019d3096da02f3475f8731f6704a0e75d`  
		Last Modified: Fri, 25 Feb 2022 03:15:09 GMT  
		Size: 1.9 KB (1884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6ba5e5368daffd340a50b6715a6d9d28d2f2c341d694c5d7cdae52e15e46d4d`  
		Last Modified: Fri, 25 Feb 2022 03:15:09 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca864d6530840f9fbdc99b6aaedcd8aa7acf319697677ca480fd220d426cb62f`  
		Last Modified: Fri, 25 Feb 2022 03:15:09 GMT  
		Size: 1.3 KB (1322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e9cb037cabf38f35bdcf375e13b7790bfdc9b4e9761cd2e865cf557a7575e81`  
		Last Modified: Fri, 25 Feb 2022 03:15:09 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:alpine`

```console
$ docker pull nats@sha256:6944283c7d430ef4d5e23afb87b2a2d9faf963793bcd94b0461bc12def6c74c2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:alpine` - linux; amd64

```console
$ docker pull nats@sha256:6f8d631c068a9d37845ebee434d2c37606757634b9d8950e8de1035dc68842b4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7591453 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:775ec723ebf4c964b880457f54f66782e850e7121d3264c851da7d58cddb64bc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 24 Nov 2021 20:19:40 GMT
ADD file:9233f6f2237d79659a9521f7e390df217cec49f1a8aa3a12147bbca1956acdb9 in / 
# Wed, 24 Nov 2021 20:19:40 GMT
CMD ["/bin/sh"]
# Fri, 25 Feb 2022 02:21:01 GMT
ENV NATS_SERVER=2.7.3
# Fri, 25 Feb 2022 02:21:04 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='c895169ab34bc21442121f6c885905a254a9351a098402f319b3fbfd1e6225c9' ;; 		armhf) natsArch='arm6'; sha256='1b7e1c5835131825c4007766befd0c96a60edbcc3bc336a6739de5c8affea0c4' ;; 		armv7) natsArch='arm7'; sha256='723290467bc7e95b59ca7238a818932b199b00a21d4e3d7eb0e826b7aba2e0ea' ;; 		x86_64) natsArch='amd64'; sha256='2186c7660cd1d9774421614f6724ad32d7cec2389e39858f227a7991be41b1a7' ;; 		x86) natsArch='386'; sha256='3e8e2841921d555d06c67b1e33fc9bd934e4afec4748f7ddf27c67d707fafea4' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 25 Feb 2022 02:21:04 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 25 Feb 2022 02:21:04 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 25 Feb 2022 02:21:04 GMT
EXPOSE 4222 6222 8222
# Fri, 25 Feb 2022 02:21:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Feb 2022 02:21:05 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:59bf1c3509f33515622619af21ed55bbe26d24913cedbca106468a5fb37a50c3`  
		Last Modified: Wed, 24 Nov 2021 20:20:05 GMT  
		Size: 2.8 MB (2818413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfad251bce41e482876302125c33ef603e0ca99f33d1d274a09af07e1acd1be6`  
		Last Modified: Fri, 25 Feb 2022 02:21:40 GMT  
		Size: 4.8 MB (4772040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8c6f8e0dbab2106f703f51433a684cef43840e5e7443402b474f3c09144a4fe`  
		Last Modified: Fri, 25 Feb 2022 02:21:39 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0d8341c3c348e685617552e338228d15dd937ca0708bd7ab85c3c1b273ed88c`  
		Last Modified: Fri, 25 Feb 2022 02:21:39 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:d6f43ae04309c6115c32d1c71469973712b3e817088a449ce37a9e8cb6b86bf9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7071601 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:846b4c8922b69a90d198633a7b622da89348aa9e3f7f11f58a294e2c4b112a33`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 24 Nov 2021 21:08:16 GMT
ADD file:61137e0aa49ba06f57ac69466fe2fb116f580b5e6159d56f846b1d72c4a3c814 in / 
# Wed, 24 Nov 2021 21:08:16 GMT
CMD ["/bin/sh"]
# Fri, 25 Feb 2022 02:49:34 GMT
ENV NATS_SERVER=2.7.3
# Fri, 25 Feb 2022 02:49:38 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='c895169ab34bc21442121f6c885905a254a9351a098402f319b3fbfd1e6225c9' ;; 		armhf) natsArch='arm6'; sha256='1b7e1c5835131825c4007766befd0c96a60edbcc3bc336a6739de5c8affea0c4' ;; 		armv7) natsArch='arm7'; sha256='723290467bc7e95b59ca7238a818932b199b00a21d4e3d7eb0e826b7aba2e0ea' ;; 		x86_64) natsArch='amd64'; sha256='2186c7660cd1d9774421614f6724ad32d7cec2389e39858f227a7991be41b1a7' ;; 		x86) natsArch='386'; sha256='3e8e2841921d555d06c67b1e33fc9bd934e4afec4748f7ddf27c67d707fafea4' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 25 Feb 2022 02:49:38 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 25 Feb 2022 02:49:39 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 25 Feb 2022 02:49:39 GMT
EXPOSE 4222 6222 8222
# Fri, 25 Feb 2022 02:49:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Feb 2022 02:49:40 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:e4a43de54da9e309482f6762f0c11f5f547cd8fd61a49c5f158453066162023e`  
		Last Modified: Wed, 24 Nov 2021 21:09:46 GMT  
		Size: 2.6 MB (2631421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ecb484648e454aaf42c41938db64a0715cb509a90811b5912192d2e66a2f7fb`  
		Last Modified: Fri, 25 Feb 2022 02:51:52 GMT  
		Size: 4.4 MB (4439176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdd675987846849cf3247fbc41b25505410823bffd30e841e7f663936458e553`  
		Last Modified: Fri, 25 Feb 2022 02:51:49 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ae450e4bdcdcad0dc3e04a43f8855409627f6c7fdecd22f661dbfe3a99530d2`  
		Last Modified: Fri, 25 Feb 2022 02:51:49 GMT  
		Size: 417.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:665c6221a3c009747c340953834a8e1c6e38008d728f3a9d4d4eaab76e8e640d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.9 MB (6865015 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f23f21c3235ba9d61b53aeb161021b62412dc690dd81727439de14a1f9b902eb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 24 Nov 2021 21:42:11 GMT
ADD file:ca436da5b0bfc9c0e2fc685533c6628918000c8fff109fe9a8da625b9a798002 in / 
# Wed, 24 Nov 2021 21:42:11 GMT
CMD ["/bin/sh"]
# Fri, 25 Feb 2022 02:57:52 GMT
ENV NATS_SERVER=2.7.3
# Fri, 25 Feb 2022 02:57:56 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='c895169ab34bc21442121f6c885905a254a9351a098402f319b3fbfd1e6225c9' ;; 		armhf) natsArch='arm6'; sha256='1b7e1c5835131825c4007766befd0c96a60edbcc3bc336a6739de5c8affea0c4' ;; 		armv7) natsArch='arm7'; sha256='723290467bc7e95b59ca7238a818932b199b00a21d4e3d7eb0e826b7aba2e0ea' ;; 		x86_64) natsArch='amd64'; sha256='2186c7660cd1d9774421614f6724ad32d7cec2389e39858f227a7991be41b1a7' ;; 		x86) natsArch='386'; sha256='3e8e2841921d555d06c67b1e33fc9bd934e4afec4748f7ddf27c67d707fafea4' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 25 Feb 2022 02:57:57 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 25 Feb 2022 02:57:57 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 25 Feb 2022 02:57:58 GMT
EXPOSE 4222 6222 8222
# Fri, 25 Feb 2022 02:57:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Feb 2022 02:57:58 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:5480d2ca1740c20ce17652e01ed2265cdc914458acd41256a2b1ccff28f2762c`  
		Last Modified: Wed, 24 Nov 2021 21:43:40 GMT  
		Size: 2.4 MB (2434764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fafd4ba596baa033665a46ce765df0c4a928784832ecc5645944032cfcd9295`  
		Last Modified: Fri, 25 Feb 2022 03:00:20 GMT  
		Size: 4.4 MB (4429250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abb2edff52bc9250fdec4032d39728784d4495539ef65cceed401a8968ec2df5`  
		Last Modified: Fri, 25 Feb 2022 03:00:18 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1047f2aa448d4163e2995aed662d6890fdd3954289a1ff2908edc894450b3d78`  
		Last Modified: Fri, 25 Feb 2022 03:00:18 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:8f79d8af0b084884d2cc9641a33a1274022fc51b99e955d3f13d9c45f47cf6b4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7132810 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e50bb490b2ac0a89152a29fc28e269300b6b83d2a85c0ce5ebe74635c34cdb0d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 24 Nov 2021 20:39:20 GMT
ADD file:df53811312284306901fdaaff0a357a4bf40d631e662fe9ce6d342442e494b6c in / 
# Wed, 24 Nov 2021 20:39:20 GMT
CMD ["/bin/sh"]
# Fri, 25 Feb 2022 03:01:24 GMT
ENV NATS_SERVER=2.7.3
# Fri, 25 Feb 2022 03:01:26 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='c895169ab34bc21442121f6c885905a254a9351a098402f319b3fbfd1e6225c9' ;; 		armhf) natsArch='arm6'; sha256='1b7e1c5835131825c4007766befd0c96a60edbcc3bc336a6739de5c8affea0c4' ;; 		armv7) natsArch='arm7'; sha256='723290467bc7e95b59ca7238a818932b199b00a21d4e3d7eb0e826b7aba2e0ea' ;; 		x86_64) natsArch='amd64'; sha256='2186c7660cd1d9774421614f6724ad32d7cec2389e39858f227a7991be41b1a7' ;; 		x86) natsArch='386'; sha256='3e8e2841921d555d06c67b1e33fc9bd934e4afec4748f7ddf27c67d707fafea4' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 25 Feb 2022 03:01:28 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 25 Feb 2022 03:01:29 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 25 Feb 2022 03:01:29 GMT
EXPOSE 4222 6222 8222
# Fri, 25 Feb 2022 03:01:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Feb 2022 03:01:31 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9b3977197b4f2147bdd31e1271f811319dcd5c2fc595f14e81f5351ab6275b99`  
		Last Modified: Wed, 24 Nov 2021 20:39:59 GMT  
		Size: 2.7 MB (2715434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c75ed4d21bde940c8f5b4d0d82b44c31489bd5a37d46b1f197b7d1baed0b6e8`  
		Last Modified: Fri, 25 Feb 2022 03:02:31 GMT  
		Size: 4.4 MB (4416403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f7dd0d82f2c731b21df156c69326c651274a35eb010b23b5150397309110717`  
		Last Modified: Fri, 25 Feb 2022 03:02:30 GMT  
		Size: 559.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f29d0f81d7bbfb90bc5607be41aabbd3e970b1e74e19a069c23e863092772ba`  
		Last Modified: Fri, 25 Feb 2022 03:02:30 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:alpine3.15`

```console
$ docker pull nats@sha256:6944283c7d430ef4d5e23afb87b2a2d9faf963793bcd94b0461bc12def6c74c2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:alpine3.15` - linux; amd64

```console
$ docker pull nats@sha256:6f8d631c068a9d37845ebee434d2c37606757634b9d8950e8de1035dc68842b4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7591453 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:775ec723ebf4c964b880457f54f66782e850e7121d3264c851da7d58cddb64bc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 24 Nov 2021 20:19:40 GMT
ADD file:9233f6f2237d79659a9521f7e390df217cec49f1a8aa3a12147bbca1956acdb9 in / 
# Wed, 24 Nov 2021 20:19:40 GMT
CMD ["/bin/sh"]
# Fri, 25 Feb 2022 02:21:01 GMT
ENV NATS_SERVER=2.7.3
# Fri, 25 Feb 2022 02:21:04 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='c895169ab34bc21442121f6c885905a254a9351a098402f319b3fbfd1e6225c9' ;; 		armhf) natsArch='arm6'; sha256='1b7e1c5835131825c4007766befd0c96a60edbcc3bc336a6739de5c8affea0c4' ;; 		armv7) natsArch='arm7'; sha256='723290467bc7e95b59ca7238a818932b199b00a21d4e3d7eb0e826b7aba2e0ea' ;; 		x86_64) natsArch='amd64'; sha256='2186c7660cd1d9774421614f6724ad32d7cec2389e39858f227a7991be41b1a7' ;; 		x86) natsArch='386'; sha256='3e8e2841921d555d06c67b1e33fc9bd934e4afec4748f7ddf27c67d707fafea4' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 25 Feb 2022 02:21:04 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 25 Feb 2022 02:21:04 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 25 Feb 2022 02:21:04 GMT
EXPOSE 4222 6222 8222
# Fri, 25 Feb 2022 02:21:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Feb 2022 02:21:05 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:59bf1c3509f33515622619af21ed55bbe26d24913cedbca106468a5fb37a50c3`  
		Last Modified: Wed, 24 Nov 2021 20:20:05 GMT  
		Size: 2.8 MB (2818413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfad251bce41e482876302125c33ef603e0ca99f33d1d274a09af07e1acd1be6`  
		Last Modified: Fri, 25 Feb 2022 02:21:40 GMT  
		Size: 4.8 MB (4772040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8c6f8e0dbab2106f703f51433a684cef43840e5e7443402b474f3c09144a4fe`  
		Last Modified: Fri, 25 Feb 2022 02:21:39 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0d8341c3c348e685617552e338228d15dd937ca0708bd7ab85c3c1b273ed88c`  
		Last Modified: Fri, 25 Feb 2022 02:21:39 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.15` - linux; arm variant v6

```console
$ docker pull nats@sha256:d6f43ae04309c6115c32d1c71469973712b3e817088a449ce37a9e8cb6b86bf9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7071601 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:846b4c8922b69a90d198633a7b622da89348aa9e3f7f11f58a294e2c4b112a33`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 24 Nov 2021 21:08:16 GMT
ADD file:61137e0aa49ba06f57ac69466fe2fb116f580b5e6159d56f846b1d72c4a3c814 in / 
# Wed, 24 Nov 2021 21:08:16 GMT
CMD ["/bin/sh"]
# Fri, 25 Feb 2022 02:49:34 GMT
ENV NATS_SERVER=2.7.3
# Fri, 25 Feb 2022 02:49:38 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='c895169ab34bc21442121f6c885905a254a9351a098402f319b3fbfd1e6225c9' ;; 		armhf) natsArch='arm6'; sha256='1b7e1c5835131825c4007766befd0c96a60edbcc3bc336a6739de5c8affea0c4' ;; 		armv7) natsArch='arm7'; sha256='723290467bc7e95b59ca7238a818932b199b00a21d4e3d7eb0e826b7aba2e0ea' ;; 		x86_64) natsArch='amd64'; sha256='2186c7660cd1d9774421614f6724ad32d7cec2389e39858f227a7991be41b1a7' ;; 		x86) natsArch='386'; sha256='3e8e2841921d555d06c67b1e33fc9bd934e4afec4748f7ddf27c67d707fafea4' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 25 Feb 2022 02:49:38 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 25 Feb 2022 02:49:39 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 25 Feb 2022 02:49:39 GMT
EXPOSE 4222 6222 8222
# Fri, 25 Feb 2022 02:49:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Feb 2022 02:49:40 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:e4a43de54da9e309482f6762f0c11f5f547cd8fd61a49c5f158453066162023e`  
		Last Modified: Wed, 24 Nov 2021 21:09:46 GMT  
		Size: 2.6 MB (2631421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ecb484648e454aaf42c41938db64a0715cb509a90811b5912192d2e66a2f7fb`  
		Last Modified: Fri, 25 Feb 2022 02:51:52 GMT  
		Size: 4.4 MB (4439176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdd675987846849cf3247fbc41b25505410823bffd30e841e7f663936458e553`  
		Last Modified: Fri, 25 Feb 2022 02:51:49 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ae450e4bdcdcad0dc3e04a43f8855409627f6c7fdecd22f661dbfe3a99530d2`  
		Last Modified: Fri, 25 Feb 2022 02:51:49 GMT  
		Size: 417.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.15` - linux; arm variant v7

```console
$ docker pull nats@sha256:665c6221a3c009747c340953834a8e1c6e38008d728f3a9d4d4eaab76e8e640d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.9 MB (6865015 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f23f21c3235ba9d61b53aeb161021b62412dc690dd81727439de14a1f9b902eb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 24 Nov 2021 21:42:11 GMT
ADD file:ca436da5b0bfc9c0e2fc685533c6628918000c8fff109fe9a8da625b9a798002 in / 
# Wed, 24 Nov 2021 21:42:11 GMT
CMD ["/bin/sh"]
# Fri, 25 Feb 2022 02:57:52 GMT
ENV NATS_SERVER=2.7.3
# Fri, 25 Feb 2022 02:57:56 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='c895169ab34bc21442121f6c885905a254a9351a098402f319b3fbfd1e6225c9' ;; 		armhf) natsArch='arm6'; sha256='1b7e1c5835131825c4007766befd0c96a60edbcc3bc336a6739de5c8affea0c4' ;; 		armv7) natsArch='arm7'; sha256='723290467bc7e95b59ca7238a818932b199b00a21d4e3d7eb0e826b7aba2e0ea' ;; 		x86_64) natsArch='amd64'; sha256='2186c7660cd1d9774421614f6724ad32d7cec2389e39858f227a7991be41b1a7' ;; 		x86) natsArch='386'; sha256='3e8e2841921d555d06c67b1e33fc9bd934e4afec4748f7ddf27c67d707fafea4' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 25 Feb 2022 02:57:57 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 25 Feb 2022 02:57:57 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 25 Feb 2022 02:57:58 GMT
EXPOSE 4222 6222 8222
# Fri, 25 Feb 2022 02:57:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Feb 2022 02:57:58 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:5480d2ca1740c20ce17652e01ed2265cdc914458acd41256a2b1ccff28f2762c`  
		Last Modified: Wed, 24 Nov 2021 21:43:40 GMT  
		Size: 2.4 MB (2434764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fafd4ba596baa033665a46ce765df0c4a928784832ecc5645944032cfcd9295`  
		Last Modified: Fri, 25 Feb 2022 03:00:20 GMT  
		Size: 4.4 MB (4429250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abb2edff52bc9250fdec4032d39728784d4495539ef65cceed401a8968ec2df5`  
		Last Modified: Fri, 25 Feb 2022 03:00:18 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1047f2aa448d4163e2995aed662d6890fdd3954289a1ff2908edc894450b3d78`  
		Last Modified: Fri, 25 Feb 2022 03:00:18 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.15` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:8f79d8af0b084884d2cc9641a33a1274022fc51b99e955d3f13d9c45f47cf6b4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7132810 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e50bb490b2ac0a89152a29fc28e269300b6b83d2a85c0ce5ebe74635c34cdb0d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 24 Nov 2021 20:39:20 GMT
ADD file:df53811312284306901fdaaff0a357a4bf40d631e662fe9ce6d342442e494b6c in / 
# Wed, 24 Nov 2021 20:39:20 GMT
CMD ["/bin/sh"]
# Fri, 25 Feb 2022 03:01:24 GMT
ENV NATS_SERVER=2.7.3
# Fri, 25 Feb 2022 03:01:26 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='c895169ab34bc21442121f6c885905a254a9351a098402f319b3fbfd1e6225c9' ;; 		armhf) natsArch='arm6'; sha256='1b7e1c5835131825c4007766befd0c96a60edbcc3bc336a6739de5c8affea0c4' ;; 		armv7) natsArch='arm7'; sha256='723290467bc7e95b59ca7238a818932b199b00a21d4e3d7eb0e826b7aba2e0ea' ;; 		x86_64) natsArch='amd64'; sha256='2186c7660cd1d9774421614f6724ad32d7cec2389e39858f227a7991be41b1a7' ;; 		x86) natsArch='386'; sha256='3e8e2841921d555d06c67b1e33fc9bd934e4afec4748f7ddf27c67d707fafea4' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 25 Feb 2022 03:01:28 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 25 Feb 2022 03:01:29 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 25 Feb 2022 03:01:29 GMT
EXPOSE 4222 6222 8222
# Fri, 25 Feb 2022 03:01:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Feb 2022 03:01:31 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9b3977197b4f2147bdd31e1271f811319dcd5c2fc595f14e81f5351ab6275b99`  
		Last Modified: Wed, 24 Nov 2021 20:39:59 GMT  
		Size: 2.7 MB (2715434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c75ed4d21bde940c8f5b4d0d82b44c31489bd5a37d46b1f197b7d1baed0b6e8`  
		Last Modified: Fri, 25 Feb 2022 03:02:31 GMT  
		Size: 4.4 MB (4416403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f7dd0d82f2c731b21df156c69326c651274a35eb010b23b5150397309110717`  
		Last Modified: Fri, 25 Feb 2022 03:02:30 GMT  
		Size: 559.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f29d0f81d7bbfb90bc5607be41aabbd3e970b1e74e19a069c23e863092772ba`  
		Last Modified: Fri, 25 Feb 2022 03:02:30 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:latest`

```console
$ docker pull nats@sha256:4fa6d62e36bac738598e6523bb2185b0d57de021331057a538765f518cfd505a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.2565; amd64

### `nats:latest` - linux; amd64

```console
$ docker pull nats@sha256:5fd249efa75cf3eb595342175207fdbb390eee3034f7fe49355d7a479fa3ffe2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4499407 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c84de17b17b3458d2b6e6d4264ea6186c82bab718ca058f5d7738e53ca2759ac`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 25 Feb 2022 02:21:13 GMT
COPY file:8a814b0c66a47e63e5a7f4287478948812fe6e03c224d539f37ce3f950d2b6c6 in /nats-server 
# Fri, 25 Feb 2022 02:21:13 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 25 Feb 2022 02:21:14 GMT
EXPOSE 4222 6222 8222
# Fri, 25 Feb 2022 02:21:14 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 25 Feb 2022 02:21:14 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:277fae1baf41821774f7a2e1c3f465b28aa8693ee0cd77e0ad0bace55d9c616e`  
		Last Modified: Fri, 25 Feb 2022 02:22:04 GMT  
		Size: 4.5 MB (4498900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb932b4b3fbc873b56e996c6357055bb7700c701d17d7d87cdec31211142b49a`  
		Last Modified: Fri, 25 Feb 2022 02:22:03 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm variant v6

```console
$ docker pull nats@sha256:2e3339e7e8d98e7bbab0613c7b7c3dd6f51fcf33ed3910a2e65e62fba7049337
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4165977 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ddc7bcc78dd550ace4def82e3db227e618d77e136274749f3bf55869e64be264`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 25 Feb 2022 02:50:06 GMT
COPY file:3a951d885f7bcec693f6fbf26a9ffd82b0c6218b6834fc6053e5812f7451b63e in /nats-server 
# Fri, 25 Feb 2022 02:50:06 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 25 Feb 2022 02:50:07 GMT
EXPOSE 4222 6222 8222
# Fri, 25 Feb 2022 02:50:07 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 25 Feb 2022 02:50:07 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:f6de87b4530f922b11edc08be8edeebc6ce0cb666907013348d4e1b9f5d51809`  
		Last Modified: Fri, 25 Feb 2022 02:52:29 GMT  
		Size: 4.2 MB (4165468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5fa68b52226484e5870677184cdc47c93a7d453f334c144b5cb631346bc8111`  
		Last Modified: Fri, 25 Feb 2022 02:52:27 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm variant v7

```console
$ docker pull nats@sha256:87cf3f8e33ebf28f35575ea083f8feb460d19fa9380d2622c82567ff3fa9d840
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4157918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4eef99b95e572b23f90d60e6e157be90b05ab2f35dbcb10f83f96ece551945a`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 25 Feb 2022 02:58:34 GMT
COPY file:3ee879939ad264e803dd4d6072181d968c4dd0fe076115159f70479c6309ef45 in /nats-server 
# Fri, 25 Feb 2022 02:58:34 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 25 Feb 2022 02:58:35 GMT
EXPOSE 4222 6222 8222
# Fri, 25 Feb 2022 02:58:35 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 25 Feb 2022 02:58:36 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:67a3d8907097b9caffd9d1720b4fb2b1d2ac9dfda60a1d169abbf5494323d50a`  
		Last Modified: Fri, 25 Feb 2022 03:00:58 GMT  
		Size: 4.2 MB (4157409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73f5577f4846f032b281220b897161962481198ead0a1b9ad1d7c76cdd989747`  
		Last Modified: Fri, 25 Feb 2022 03:00:55 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:e970861a260709ae1e8c892eb36758c14323e81959ff4aaa1e9b7327b91d3e70
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.1 MB (4143805 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4414e48026697a15338f28dcb8e46ace9627ea7332559e1708f36ce62a5e327`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 25 Feb 2022 03:01:42 GMT
COPY file:acd11e9a3a86f6f3da079c5155851337e747c3b31481ec05e2dd1e48e23becb2 in /nats-server 
# Fri, 25 Feb 2022 03:01:43 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 25 Feb 2022 03:01:43 GMT
EXPOSE 4222 6222 8222
# Fri, 25 Feb 2022 03:01:44 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 25 Feb 2022 03:01:45 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6ad9fd47af885b43442590ad2c8171e4b4899caef84921ec73ba0540b9c03284`  
		Last Modified: Fri, 25 Feb 2022 03:02:59 GMT  
		Size: 4.1 MB (4143299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02d7667f81936503f26a5ed657cfffdc9add626da8ae5bb78d691054cd3af7c3`  
		Last Modified: Fri, 25 Feb 2022 03:02:59 GMT  
		Size: 506.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - windows version 10.0.17763.2565; amd64

```console
$ docker pull nats@sha256:d7c795020fd7295382d503ba883e23cf34ca9c53d6e6b91184bc1fd2bb2c990d
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.6 MB (107634881 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6e99776e94a148ebda875656d07e673c65aedb583986faedb3bdc61a2fd7759`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 02 Feb 2022 19:06:51 GMT
RUN Apply image 1809-amd64
# Wed, 09 Feb 2022 18:13:36 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 25 Feb 2022 02:17:30 GMT
RUN cmd /S /C #(nop) COPY file:d5609a37f534b519fa4326428362ea5398f7165ee90493fb7bdc8b810da33b0e in C:\nats-server.exe 
# Fri, 25 Feb 2022 02:17:31 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Fri, 25 Feb 2022 02:17:32 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Fri, 25 Feb 2022 02:17:33 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 25 Feb 2022 02:17:34 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:bd0b37167cd3d731eb15196e123df7156b5a35597874d3016a1a4298c46fac3f`  
		Size: 103.1 MB (103087119 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8bc49c59cde14e3a9ed8fedce001c00fcb5fe0f9b914aa07273e04f23333d180`  
		Last Modified: Wed, 09 Feb 2022 18:14:28 GMT  
		Size: 1.1 KB (1138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b682f8d539489225b7a3859570b80452b497086f57fa4e6908f2b99d213e1a03`  
		Last Modified: Fri, 25 Feb 2022 03:15:32 GMT  
		Size: 4.5 MB (4541735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67997158a056ea601aec06de195ce0251264a6d8d071f8a44a49a545865ce426`  
		Last Modified: Fri, 25 Feb 2022 03:15:27 GMT  
		Size: 1.7 KB (1656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f873036aacce9bbc35378d6a36985e62919c6d2c9ff526011564a861b86240ab`  
		Last Modified: Fri, 25 Feb 2022 03:15:27 GMT  
		Size: 1.0 KB (1039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf1eace4b7f44dce795499001f62baee27fb477865e490b11d05d198c8e80550`  
		Last Modified: Fri, 25 Feb 2022 03:15:27 GMT  
		Size: 1.1 KB (1081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8accc8a69e6317ee43a53e093f2aef25b70ddff625cfa691d7df28e9bf6d94dc`  
		Last Modified: Fri, 25 Feb 2022 03:15:27 GMT  
		Size: 1.1 KB (1113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:linux`

```console
$ docker pull nats@sha256:4fe2c16e211795858e7e7538197ec57f67ed6e9ca5d91d06d925e09ec6724d3b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:linux` - linux; amd64

```console
$ docker pull nats@sha256:5fd249efa75cf3eb595342175207fdbb390eee3034f7fe49355d7a479fa3ffe2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4499407 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c84de17b17b3458d2b6e6d4264ea6186c82bab718ca058f5d7738e53ca2759ac`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 25 Feb 2022 02:21:13 GMT
COPY file:8a814b0c66a47e63e5a7f4287478948812fe6e03c224d539f37ce3f950d2b6c6 in /nats-server 
# Fri, 25 Feb 2022 02:21:13 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 25 Feb 2022 02:21:14 GMT
EXPOSE 4222 6222 8222
# Fri, 25 Feb 2022 02:21:14 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 25 Feb 2022 02:21:14 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:277fae1baf41821774f7a2e1c3f465b28aa8693ee0cd77e0ad0bace55d9c616e`  
		Last Modified: Fri, 25 Feb 2022 02:22:04 GMT  
		Size: 4.5 MB (4498900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb932b4b3fbc873b56e996c6357055bb7700c701d17d7d87cdec31211142b49a`  
		Last Modified: Fri, 25 Feb 2022 02:22:03 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:2e3339e7e8d98e7bbab0613c7b7c3dd6f51fcf33ed3910a2e65e62fba7049337
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4165977 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ddc7bcc78dd550ace4def82e3db227e618d77e136274749f3bf55869e64be264`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 25 Feb 2022 02:50:06 GMT
COPY file:3a951d885f7bcec693f6fbf26a9ffd82b0c6218b6834fc6053e5812f7451b63e in /nats-server 
# Fri, 25 Feb 2022 02:50:06 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 25 Feb 2022 02:50:07 GMT
EXPOSE 4222 6222 8222
# Fri, 25 Feb 2022 02:50:07 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 25 Feb 2022 02:50:07 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:f6de87b4530f922b11edc08be8edeebc6ce0cb666907013348d4e1b9f5d51809`  
		Last Modified: Fri, 25 Feb 2022 02:52:29 GMT  
		Size: 4.2 MB (4165468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5fa68b52226484e5870677184cdc47c93a7d453f334c144b5cb631346bc8111`  
		Last Modified: Fri, 25 Feb 2022 02:52:27 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:87cf3f8e33ebf28f35575ea083f8feb460d19fa9380d2622c82567ff3fa9d840
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4157918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4eef99b95e572b23f90d60e6e157be90b05ab2f35dbcb10f83f96ece551945a`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 25 Feb 2022 02:58:34 GMT
COPY file:3ee879939ad264e803dd4d6072181d968c4dd0fe076115159f70479c6309ef45 in /nats-server 
# Fri, 25 Feb 2022 02:58:34 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 25 Feb 2022 02:58:35 GMT
EXPOSE 4222 6222 8222
# Fri, 25 Feb 2022 02:58:35 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 25 Feb 2022 02:58:36 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:67a3d8907097b9caffd9d1720b4fb2b1d2ac9dfda60a1d169abbf5494323d50a`  
		Last Modified: Fri, 25 Feb 2022 03:00:58 GMT  
		Size: 4.2 MB (4157409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73f5577f4846f032b281220b897161962481198ead0a1b9ad1d7c76cdd989747`  
		Last Modified: Fri, 25 Feb 2022 03:00:55 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:e970861a260709ae1e8c892eb36758c14323e81959ff4aaa1e9b7327b91d3e70
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.1 MB (4143805 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4414e48026697a15338f28dcb8e46ace9627ea7332559e1708f36ce62a5e327`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 25 Feb 2022 03:01:42 GMT
COPY file:acd11e9a3a86f6f3da079c5155851337e747c3b31481ec05e2dd1e48e23becb2 in /nats-server 
# Fri, 25 Feb 2022 03:01:43 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 25 Feb 2022 03:01:43 GMT
EXPOSE 4222 6222 8222
# Fri, 25 Feb 2022 03:01:44 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 25 Feb 2022 03:01:45 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6ad9fd47af885b43442590ad2c8171e4b4899caef84921ec73ba0540b9c03284`  
		Last Modified: Fri, 25 Feb 2022 03:02:59 GMT  
		Size: 4.1 MB (4143299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02d7667f81936503f26a5ed657cfffdc9add626da8ae5bb78d691054cd3af7c3`  
		Last Modified: Fri, 25 Feb 2022 03:02:59 GMT  
		Size: 506.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:nanoserver`

```console
$ docker pull nats@sha256:6e43eecf010598596b218f3800a6d052426d875695ead9cdbf074e0653772142
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2565; amd64

### `nats:nanoserver` - windows version 10.0.17763.2565; amd64

```console
$ docker pull nats@sha256:d7c795020fd7295382d503ba883e23cf34ca9c53d6e6b91184bc1fd2bb2c990d
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.6 MB (107634881 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6e99776e94a148ebda875656d07e673c65aedb583986faedb3bdc61a2fd7759`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 02 Feb 2022 19:06:51 GMT
RUN Apply image 1809-amd64
# Wed, 09 Feb 2022 18:13:36 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 25 Feb 2022 02:17:30 GMT
RUN cmd /S /C #(nop) COPY file:d5609a37f534b519fa4326428362ea5398f7165ee90493fb7bdc8b810da33b0e in C:\nats-server.exe 
# Fri, 25 Feb 2022 02:17:31 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Fri, 25 Feb 2022 02:17:32 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Fri, 25 Feb 2022 02:17:33 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 25 Feb 2022 02:17:34 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:bd0b37167cd3d731eb15196e123df7156b5a35597874d3016a1a4298c46fac3f`  
		Size: 103.1 MB (103087119 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8bc49c59cde14e3a9ed8fedce001c00fcb5fe0f9b914aa07273e04f23333d180`  
		Last Modified: Wed, 09 Feb 2022 18:14:28 GMT  
		Size: 1.1 KB (1138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b682f8d539489225b7a3859570b80452b497086f57fa4e6908f2b99d213e1a03`  
		Last Modified: Fri, 25 Feb 2022 03:15:32 GMT  
		Size: 4.5 MB (4541735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67997158a056ea601aec06de195ce0251264a6d8d071f8a44a49a545865ce426`  
		Last Modified: Fri, 25 Feb 2022 03:15:27 GMT  
		Size: 1.7 KB (1656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f873036aacce9bbc35378d6a36985e62919c6d2c9ff526011564a861b86240ab`  
		Last Modified: Fri, 25 Feb 2022 03:15:27 GMT  
		Size: 1.0 KB (1039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf1eace4b7f44dce795499001f62baee27fb477865e490b11d05d198c8e80550`  
		Last Modified: Fri, 25 Feb 2022 03:15:27 GMT  
		Size: 1.1 KB (1081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8accc8a69e6317ee43a53e093f2aef25b70ddff625cfa691d7df28e9bf6d94dc`  
		Last Modified: Fri, 25 Feb 2022 03:15:27 GMT  
		Size: 1.1 KB (1113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:nanoserver-1809`

```console
$ docker pull nats@sha256:6e43eecf010598596b218f3800a6d052426d875695ead9cdbf074e0653772142
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2565; amd64

### `nats:nanoserver-1809` - windows version 10.0.17763.2565; amd64

```console
$ docker pull nats@sha256:d7c795020fd7295382d503ba883e23cf34ca9c53d6e6b91184bc1fd2bb2c990d
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.6 MB (107634881 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6e99776e94a148ebda875656d07e673c65aedb583986faedb3bdc61a2fd7759`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 02 Feb 2022 19:06:51 GMT
RUN Apply image 1809-amd64
# Wed, 09 Feb 2022 18:13:36 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 25 Feb 2022 02:17:30 GMT
RUN cmd /S /C #(nop) COPY file:d5609a37f534b519fa4326428362ea5398f7165ee90493fb7bdc8b810da33b0e in C:\nats-server.exe 
# Fri, 25 Feb 2022 02:17:31 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Fri, 25 Feb 2022 02:17:32 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Fri, 25 Feb 2022 02:17:33 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 25 Feb 2022 02:17:34 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:bd0b37167cd3d731eb15196e123df7156b5a35597874d3016a1a4298c46fac3f`  
		Size: 103.1 MB (103087119 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8bc49c59cde14e3a9ed8fedce001c00fcb5fe0f9b914aa07273e04f23333d180`  
		Last Modified: Wed, 09 Feb 2022 18:14:28 GMT  
		Size: 1.1 KB (1138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b682f8d539489225b7a3859570b80452b497086f57fa4e6908f2b99d213e1a03`  
		Last Modified: Fri, 25 Feb 2022 03:15:32 GMT  
		Size: 4.5 MB (4541735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67997158a056ea601aec06de195ce0251264a6d8d071f8a44a49a545865ce426`  
		Last Modified: Fri, 25 Feb 2022 03:15:27 GMT  
		Size: 1.7 KB (1656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f873036aacce9bbc35378d6a36985e62919c6d2c9ff526011564a861b86240ab`  
		Last Modified: Fri, 25 Feb 2022 03:15:27 GMT  
		Size: 1.0 KB (1039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf1eace4b7f44dce795499001f62baee27fb477865e490b11d05d198c8e80550`  
		Last Modified: Fri, 25 Feb 2022 03:15:27 GMT  
		Size: 1.1 KB (1081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8accc8a69e6317ee43a53e093f2aef25b70ddff625cfa691d7df28e9bf6d94dc`  
		Last Modified: Fri, 25 Feb 2022 03:15:27 GMT  
		Size: 1.1 KB (1113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:scratch`

```console
$ docker pull nats@sha256:4fe2c16e211795858e7e7538197ec57f67ed6e9ca5d91d06d925e09ec6724d3b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:scratch` - linux; amd64

```console
$ docker pull nats@sha256:5fd249efa75cf3eb595342175207fdbb390eee3034f7fe49355d7a479fa3ffe2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4499407 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c84de17b17b3458d2b6e6d4264ea6186c82bab718ca058f5d7738e53ca2759ac`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 25 Feb 2022 02:21:13 GMT
COPY file:8a814b0c66a47e63e5a7f4287478948812fe6e03c224d539f37ce3f950d2b6c6 in /nats-server 
# Fri, 25 Feb 2022 02:21:13 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 25 Feb 2022 02:21:14 GMT
EXPOSE 4222 6222 8222
# Fri, 25 Feb 2022 02:21:14 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 25 Feb 2022 02:21:14 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:277fae1baf41821774f7a2e1c3f465b28aa8693ee0cd77e0ad0bace55d9c616e`  
		Last Modified: Fri, 25 Feb 2022 02:22:04 GMT  
		Size: 4.5 MB (4498900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb932b4b3fbc873b56e996c6357055bb7700c701d17d7d87cdec31211142b49a`  
		Last Modified: Fri, 25 Feb 2022 02:22:03 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:2e3339e7e8d98e7bbab0613c7b7c3dd6f51fcf33ed3910a2e65e62fba7049337
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4165977 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ddc7bcc78dd550ace4def82e3db227e618d77e136274749f3bf55869e64be264`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 25 Feb 2022 02:50:06 GMT
COPY file:3a951d885f7bcec693f6fbf26a9ffd82b0c6218b6834fc6053e5812f7451b63e in /nats-server 
# Fri, 25 Feb 2022 02:50:06 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 25 Feb 2022 02:50:07 GMT
EXPOSE 4222 6222 8222
# Fri, 25 Feb 2022 02:50:07 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 25 Feb 2022 02:50:07 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:f6de87b4530f922b11edc08be8edeebc6ce0cb666907013348d4e1b9f5d51809`  
		Last Modified: Fri, 25 Feb 2022 02:52:29 GMT  
		Size: 4.2 MB (4165468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5fa68b52226484e5870677184cdc47c93a7d453f334c144b5cb631346bc8111`  
		Last Modified: Fri, 25 Feb 2022 02:52:27 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:87cf3f8e33ebf28f35575ea083f8feb460d19fa9380d2622c82567ff3fa9d840
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4157918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4eef99b95e572b23f90d60e6e157be90b05ab2f35dbcb10f83f96ece551945a`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 25 Feb 2022 02:58:34 GMT
COPY file:3ee879939ad264e803dd4d6072181d968c4dd0fe076115159f70479c6309ef45 in /nats-server 
# Fri, 25 Feb 2022 02:58:34 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 25 Feb 2022 02:58:35 GMT
EXPOSE 4222 6222 8222
# Fri, 25 Feb 2022 02:58:35 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 25 Feb 2022 02:58:36 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:67a3d8907097b9caffd9d1720b4fb2b1d2ac9dfda60a1d169abbf5494323d50a`  
		Last Modified: Fri, 25 Feb 2022 03:00:58 GMT  
		Size: 4.2 MB (4157409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73f5577f4846f032b281220b897161962481198ead0a1b9ad1d7c76cdd989747`  
		Last Modified: Fri, 25 Feb 2022 03:00:55 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:e970861a260709ae1e8c892eb36758c14323e81959ff4aaa1e9b7327b91d3e70
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.1 MB (4143805 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4414e48026697a15338f28dcb8e46ace9627ea7332559e1708f36ce62a5e327`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 25 Feb 2022 03:01:42 GMT
COPY file:acd11e9a3a86f6f3da079c5155851337e747c3b31481ec05e2dd1e48e23becb2 in /nats-server 
# Fri, 25 Feb 2022 03:01:43 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 25 Feb 2022 03:01:43 GMT
EXPOSE 4222 6222 8222
# Fri, 25 Feb 2022 03:01:44 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 25 Feb 2022 03:01:45 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6ad9fd47af885b43442590ad2c8171e4b4899caef84921ec73ba0540b9c03284`  
		Last Modified: Fri, 25 Feb 2022 03:02:59 GMT  
		Size: 4.1 MB (4143299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02d7667f81936503f26a5ed657cfffdc9add626da8ae5bb78d691054cd3af7c3`  
		Last Modified: Fri, 25 Feb 2022 03:02:59 GMT  
		Size: 506.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:windowsservercore`

```console
$ docker pull nats@sha256:2b9c20408baf29df9d8666fc894d8a5c308946331d4310ef5a82b1eed5101db3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2565; amd64

### `nats:windowsservercore` - windows version 10.0.17763.2565; amd64

```console
$ docker pull nats@sha256:ac025e7ac0a2786f5807888399f94d317a0636b60e8a37584569d586fb1ac146
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2718991955 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:007419288bb7b16cd78d29d0476687df2d88011775f13b3f565c92414a214c05`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Wed, 02 Feb 2022 19:28:56 GMT
RUN Install update 1809-amd64
# Wed, 09 Feb 2022 15:04:17 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Feb 2022 18:10:54 GMT
ENV NATS_DOCKERIZED=1
# Fri, 25 Feb 2022 02:14:46 GMT
ENV NATS_SERVER=2.7.3
# Fri, 25 Feb 2022 02:14:47 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.7.3/nats-server-v2.7.3-windows-amd64.zip
# Fri, 25 Feb 2022 02:14:48 GMT
ENV NATS_SERVER_SHASUM=ddb372da68741d897006c8d4b160c7f4788603cbaacb3fa105ddf7baada04428
# Fri, 25 Feb 2022 02:15:50 GMT
RUN Set-PSDebug -Trace 2
# Fri, 25 Feb 2022 02:17:14 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 25 Feb 2022 02:17:16 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Fri, 25 Feb 2022 02:17:17 GMT
EXPOSE 4222 6222 8222
# Fri, 25 Feb 2022 02:17:18 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 25 Feb 2022 02:17:19 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:1bd78008c728d8f9e56dc2093e6eb55f0f0b1aa96e5d0c7ccc830c5f60876cdf`  
		Size: 995.4 MB (995381853 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f49d3791198cf2ea875fd54ce3bb715670742d4a58c00252395ad1b74036662a`  
		Last Modified: Wed, 09 Feb 2022 16:39:51 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4235aeeb4e8b577cc7aa26c7994ec94c94dd53a38764fc510b330b77cef4abad`  
		Last Modified: Wed, 09 Feb 2022 18:14:09 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6ed63a799d34b3a151eb2d65afc4a93d028c5308ce305f9059da19083ea4579`  
		Last Modified: Fri, 25 Feb 2022 03:15:11 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fa36020fa0fadcfe9ac785f1bc4cbf6e51ac336a4441d2ea628465f9f1e3832`  
		Last Modified: Fri, 25 Feb 2022 03:15:11 GMT  
		Size: 1.3 KB (1321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58aaa8ed102560150d8bd4fe887000c2789a69df5ae550a8b8058e526d01af34`  
		Last Modified: Fri, 25 Feb 2022 03:15:11 GMT  
		Size: 1.3 KB (1300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e48afd20cc6576c9f831f4166f86f4cd65be8140eda5a57159bba0d62c21b1af`  
		Last Modified: Fri, 25 Feb 2022 03:15:12 GMT  
		Size: 374.3 KB (374309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1eb76be5e45618d5a45f4672ac8e8c8d45d10bf627dc47f3afe45c7909b223b`  
		Last Modified: Fri, 25 Feb 2022 03:15:10 GMT  
		Size: 4.9 MB (4890363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:513928aafbffc4a16807de347507df4019d3096da02f3475f8731f6704a0e75d`  
		Last Modified: Fri, 25 Feb 2022 03:15:09 GMT  
		Size: 1.9 KB (1884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6ba5e5368daffd340a50b6715a6d9d28d2f2c341d694c5d7cdae52e15e46d4d`  
		Last Modified: Fri, 25 Feb 2022 03:15:09 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca864d6530840f9fbdc99b6aaedcd8aa7acf319697677ca480fd220d426cb62f`  
		Last Modified: Fri, 25 Feb 2022 03:15:09 GMT  
		Size: 1.3 KB (1322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e9cb037cabf38f35bdcf375e13b7790bfdc9b4e9761cd2e865cf557a7575e81`  
		Last Modified: Fri, 25 Feb 2022 03:15:09 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:windowsservercore-1809`

```console
$ docker pull nats@sha256:2b9c20408baf29df9d8666fc894d8a5c308946331d4310ef5a82b1eed5101db3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2565; amd64

### `nats:windowsservercore-1809` - windows version 10.0.17763.2565; amd64

```console
$ docker pull nats@sha256:ac025e7ac0a2786f5807888399f94d317a0636b60e8a37584569d586fb1ac146
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2718991955 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:007419288bb7b16cd78d29d0476687df2d88011775f13b3f565c92414a214c05`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Wed, 02 Feb 2022 19:28:56 GMT
RUN Install update 1809-amd64
# Wed, 09 Feb 2022 15:04:17 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Feb 2022 18:10:54 GMT
ENV NATS_DOCKERIZED=1
# Fri, 25 Feb 2022 02:14:46 GMT
ENV NATS_SERVER=2.7.3
# Fri, 25 Feb 2022 02:14:47 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.7.3/nats-server-v2.7.3-windows-amd64.zip
# Fri, 25 Feb 2022 02:14:48 GMT
ENV NATS_SERVER_SHASUM=ddb372da68741d897006c8d4b160c7f4788603cbaacb3fa105ddf7baada04428
# Fri, 25 Feb 2022 02:15:50 GMT
RUN Set-PSDebug -Trace 2
# Fri, 25 Feb 2022 02:17:14 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 25 Feb 2022 02:17:16 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Fri, 25 Feb 2022 02:17:17 GMT
EXPOSE 4222 6222 8222
# Fri, 25 Feb 2022 02:17:18 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 25 Feb 2022 02:17:19 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:1bd78008c728d8f9e56dc2093e6eb55f0f0b1aa96e5d0c7ccc830c5f60876cdf`  
		Size: 995.4 MB (995381853 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f49d3791198cf2ea875fd54ce3bb715670742d4a58c00252395ad1b74036662a`  
		Last Modified: Wed, 09 Feb 2022 16:39:51 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4235aeeb4e8b577cc7aa26c7994ec94c94dd53a38764fc510b330b77cef4abad`  
		Last Modified: Wed, 09 Feb 2022 18:14:09 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6ed63a799d34b3a151eb2d65afc4a93d028c5308ce305f9059da19083ea4579`  
		Last Modified: Fri, 25 Feb 2022 03:15:11 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fa36020fa0fadcfe9ac785f1bc4cbf6e51ac336a4441d2ea628465f9f1e3832`  
		Last Modified: Fri, 25 Feb 2022 03:15:11 GMT  
		Size: 1.3 KB (1321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58aaa8ed102560150d8bd4fe887000c2789a69df5ae550a8b8058e526d01af34`  
		Last Modified: Fri, 25 Feb 2022 03:15:11 GMT  
		Size: 1.3 KB (1300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e48afd20cc6576c9f831f4166f86f4cd65be8140eda5a57159bba0d62c21b1af`  
		Last Modified: Fri, 25 Feb 2022 03:15:12 GMT  
		Size: 374.3 KB (374309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1eb76be5e45618d5a45f4672ac8e8c8d45d10bf627dc47f3afe45c7909b223b`  
		Last Modified: Fri, 25 Feb 2022 03:15:10 GMT  
		Size: 4.9 MB (4890363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:513928aafbffc4a16807de347507df4019d3096da02f3475f8731f6704a0e75d`  
		Last Modified: Fri, 25 Feb 2022 03:15:09 GMT  
		Size: 1.9 KB (1884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6ba5e5368daffd340a50b6715a6d9d28d2f2c341d694c5d7cdae52e15e46d4d`  
		Last Modified: Fri, 25 Feb 2022 03:15:09 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca864d6530840f9fbdc99b6aaedcd8aa7acf319697677ca480fd220d426cb62f`  
		Last Modified: Fri, 25 Feb 2022 03:15:09 GMT  
		Size: 1.3 KB (1322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e9cb037cabf38f35bdcf375e13b7790bfdc9b4e9761cd2e865cf557a7575e81`  
		Last Modified: Fri, 25 Feb 2022 03:15:09 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
