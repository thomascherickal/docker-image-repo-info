<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `nats`

-	[`nats:2`](#nats2)
-	[`nats:2-alpine`](#nats2-alpine)
-	[`nats:2-alpine3.17`](#nats2-alpine317)
-	[`nats:2-linux`](#nats2-linux)
-	[`nats:2-nanoserver`](#nats2-nanoserver)
-	[`nats:2-nanoserver-1809`](#nats2-nanoserver-1809)
-	[`nats:2-scratch`](#nats2-scratch)
-	[`nats:2-windowsservercore`](#nats2-windowsservercore)
-	[`nats:2-windowsservercore-1809`](#nats2-windowsservercore-1809)
-	[`nats:2.9`](#nats29)
-	[`nats:2.9-alpine`](#nats29-alpine)
-	[`nats:2.9-alpine3.17`](#nats29-alpine317)
-	[`nats:2.9-linux`](#nats29-linux)
-	[`nats:2.9-nanoserver`](#nats29-nanoserver)
-	[`nats:2.9-nanoserver-1809`](#nats29-nanoserver-1809)
-	[`nats:2.9-scratch`](#nats29-scratch)
-	[`nats:2.9-windowsservercore`](#nats29-windowsservercore)
-	[`nats:2.9-windowsservercore-1809`](#nats29-windowsservercore-1809)
-	[`nats:2.9.14`](#nats2914)
-	[`nats:2.9.14-alpine`](#nats2914-alpine)
-	[`nats:2.9.14-alpine3.17`](#nats2914-alpine317)
-	[`nats:2.9.14-linux`](#nats2914-linux)
-	[`nats:2.9.14-nanoserver`](#nats2914-nanoserver)
-	[`nats:2.9.14-nanoserver-1809`](#nats2914-nanoserver-1809)
-	[`nats:2.9.14-scratch`](#nats2914-scratch)
-	[`nats:2.9.14-windowsservercore`](#nats2914-windowsservercore)
-	[`nats:2.9.14-windowsservercore-1809`](#nats2914-windowsservercore-1809)
-	[`nats:alpine`](#natsalpine)
-	[`nats:alpine3.17`](#natsalpine317)
-	[`nats:latest`](#natslatest)
-	[`nats:linux`](#natslinux)
-	[`nats:nanoserver`](#natsnanoserver)
-	[`nats:nanoserver-1809`](#natsnanoserver-1809)
-	[`nats:scratch`](#natsscratch)
-	[`nats:windowsservercore`](#natswindowsservercore)
-	[`nats:windowsservercore-1809`](#natswindowsservercore-1809)

## `nats:2`

```console
$ docker pull nats@sha256:f80a2e0337ac068122897636f9f6d686a397ea56f593e0ce0a603cdf41e6e027
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.3887; amd64

### `nats:2` - linux; amd64

```console
$ docker pull nats@sha256:e6916a74a9af2d54502bfa1459a3e0702c00faa14327b3f3b812262e8ada0966
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4933617 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dbb0263a71ad823c35b7c360c016e57737a4367ef1c4909a859acb0ddb4ab19a`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 07 Feb 2023 02:43:58 GMT
COPY file:ac560677dbfad917be71a9245045f536b2801212b542bc63c664d6d11156f4dc in /nats-server 
# Tue, 07 Feb 2023 02:43:58 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 07 Feb 2023 02:43:58 GMT
EXPOSE 4222 6222 8222
# Tue, 07 Feb 2023 02:43:58 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 07 Feb 2023 02:43:59 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 07 Feb 2023 02:43:59 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:5668bc7ee19e1c51e1510bfeee7245e2b2cc66a8b8f8b0f988f4b3bca8729cec`  
		Last Modified: Tue, 07 Feb 2023 02:44:45 GMT  
		Size: 4.9 MB (4933108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93d5b4d77a0e7f6c3fed0f1ae97dbe1b22a3ed4e6af873e7782a0b1d2b992779`  
		Last Modified: Tue, 07 Feb 2023 02:44:44 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - linux; arm variant v6

```console
$ docker pull nats@sha256:b141eec319986960b56193a2de1a779138beb96cb9945ebc12dbbe199ca96382
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4696311 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89f9b13a403b08d651892f330e0f3dd788a5fb00fd1f6338e79860d306d4504d`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 07 Feb 2023 01:52:41 GMT
COPY file:4eee0f78d63bff3b20fac11aaeb64833cd520dac95605f8f9015e670e58a5ef7 in /nats-server 
# Tue, 07 Feb 2023 01:52:41 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 07 Feb 2023 01:52:41 GMT
EXPOSE 4222 6222 8222
# Tue, 07 Feb 2023 01:52:41 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 07 Feb 2023 01:52:41 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 07 Feb 2023 01:52:41 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6a1ef747dccf7d40d061dc4c857fff9b056d8693e427a2f3adaebc1e22066869`  
		Last Modified: Tue, 07 Feb 2023 01:54:10 GMT  
		Size: 4.7 MB (4695803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc7ba083439d0caacde0ad211a483925f47f6ec3916cf261abe491ac5a630aaf`  
		Last Modified: Tue, 07 Feb 2023 01:54:10 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - linux; arm variant v7

```console
$ docker pull nats@sha256:ccb41e1e35bee87bcd6a70e43fd88e284140c67701fb8f639781a7b0b7201eb6
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4691076 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a4d042e0f28cb5cfa1b6a77c7eb4e06d62ffbfd2c681f2ca2f1aa747dc538cf`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 07 Feb 2023 02:00:54 GMT
COPY file:5f0ce15e9664bd3755e850351446cf7719b19193e891220c68a9776456e2700a in /nats-server 
# Tue, 07 Feb 2023 02:00:54 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 07 Feb 2023 02:00:54 GMT
EXPOSE 4222 6222 8222
# Tue, 07 Feb 2023 02:00:54 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 07 Feb 2023 02:00:54 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 07 Feb 2023 02:00:54 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:858d33663bc30713d47f7de008a1659f090a1ab8df117e447c1623a289378d31`  
		Last Modified: Tue, 07 Feb 2023 02:02:24 GMT  
		Size: 4.7 MB (4690568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c4973a38193b2d039d297077dd1451a47493f724dd8283e465313c615bcbbb8`  
		Last Modified: Tue, 07 Feb 2023 02:02:23 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:1689ba4ea78e52511a025fdbe524cf1d62dc69c0c2bb68119fabb955e8513246
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4519578 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:96bb932300dca1eb555905232fe9caf2ee65c6b8285cc68e13cf30bb07bd94d3`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 07 Feb 2023 01:52:13 GMT
COPY file:cc453883d11f3e7a77a5f311e510cb07fee2fd66b31eb11f16a5f8023889f08d in /nats-server 
# Tue, 07 Feb 2023 01:52:13 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 07 Feb 2023 01:52:13 GMT
EXPOSE 4222 6222 8222
# Tue, 07 Feb 2023 01:52:13 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 07 Feb 2023 01:52:13 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 07 Feb 2023 01:52:13 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:cf0e5763ec64b26f959ef78ac3641929a51a1fda6989adfd65f04af6f8b3a53a`  
		Last Modified: Tue, 07 Feb 2023 01:53:02 GMT  
		Size: 4.5 MB (4519070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cb009df287c6f73705947a89031473f06a27171a64409e09c24fc061c1863d5`  
		Last Modified: Tue, 07 Feb 2023 01:53:01 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - windows version 10.0.17763.3887; amd64

```console
$ docker pull nats@sha256:e6a17bb97fb6a291a4bd98d30c3b9099dedbcf70d12fb062efebaabdb1213bbc
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.7 MB (111659596 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:45804cd0005e5185373d2c577a4257391cd004c68b4c440f4678cf10382b2db7`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 07 Jan 2023 05:17:01 GMT
RUN Apply image 10.0.17763.3887
# Thu, 12 Jan 2023 05:01:51 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Tue, 07 Feb 2023 02:18:03 GMT
RUN cmd /S /C #(nop) COPY file:a45a34d252c029bb58fb3b3e2b3592a2d7869806250714c7b6dc3fb0b305c7bd in C:\nats-server.exe 
# Tue, 07 Feb 2023 02:18:04 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Tue, 07 Feb 2023 02:18:05 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Tue, 07 Feb 2023 02:18:06 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 07 Feb 2023 02:18:06 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:e58f9ad3b15a2a4882ab0a845e8e619cc8c3c411ddbe8b50046c1618a95c1397`  
		Last Modified: Thu, 12 Jan 2023 02:40:44 GMT  
		Size: 106.7 MB (106666138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fe88f4c5f9972ffecb9a66b92e75ddfe48bf7d8d451ace7af3527653f67ff9e`  
		Last Modified: Thu, 12 Jan 2023 05:02:42 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6572a3c131299689497339cc59b098f3601ad482ac0828eeaba7e5f78dc21d76`  
		Last Modified: Tue, 07 Feb 2023 02:18:55 GMT  
		Size: 5.0 MB (4987024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d5a625d40bd2eadd9e49c606bd8fad79a2aa73ebcd3313c3de00a12b06738c7`  
		Last Modified: Tue, 07 Feb 2023 02:18:53 GMT  
		Size: 1.8 KB (1788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9650a5245dfd33f33fb4a5df832057f9d0b34cb3febe41b20095202eda9b58f`  
		Last Modified: Tue, 07 Feb 2023 02:18:53 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15ca02e3d157746bd7381b47df24d65195a307dadd09eba9a311c95481d51b4d`  
		Last Modified: Tue, 07 Feb 2023 02:18:53 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efd2be7007de85b1c3f78a02ae15fdfcf679c7378b8d53403ebe90f39cd16418`  
		Last Modified: Tue, 07 Feb 2023 02:18:53 GMT  
		Size: 1.2 KB (1181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-alpine`

```console
$ docker pull nats@sha256:23353a80fc1fecc883623f6b72759544f596be792aed1db01257ac900ca8d47f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-alpine` - linux; amd64

```console
$ docker pull nats@sha256:2a0dd7504f75410d3b3198dbe094b70521260161f86ce9ec6a90b87548e5a22e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.6 MB (8591202 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9082af6bf2d6856d36cfa41bfd118221042916ab5cdf1ea5e886e9b9040cb97`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 09 Jan 2023 17:05:20 GMT
ADD file:e4d600fc4c9c293efe360be7b30ee96579925d1b4634c94332e2ec73f7d8eca1 in / 
# Mon, 09 Jan 2023 17:05:20 GMT
CMD ["/bin/sh"]
# Tue, 07 Feb 2023 02:43:45 GMT
ENV NATS_SERVER=2.9.14
# Tue, 07 Feb 2023 02:43:48 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='6032bc7b2621256e2d9f62f2a987eef490f071bde04dca09786d0270130f9cfd' ;; 		armhf) natsArch='arm6'; sha256='afbee67b87868dc29cf6c382f87813de264572472ac7513a66db6e99fd2a24ac' ;; 		armv7) natsArch='arm7'; sha256='e7e5c019e6cc3d6ef72da80defd5a4f95690b8d108ebb2cfd74fc9c47ac00706' ;; 		x86_64) natsArch='amd64'; sha256='18ac6d0a3956a3d293b85c33822159188b9e75b7597241e2c821e9ded7456601' ;; 		x86) natsArch='386'; sha256='637363cf3ca923c8762ecd083cf83c15cad505ed011ddbbaea857d982a1dadcf' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 07 Feb 2023 02:43:48 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 07 Feb 2023 02:43:48 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 07 Feb 2023 02:43:48 GMT
EXPOSE 4222 6222 8222
# Tue, 07 Feb 2023 02:43:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 07 Feb 2023 02:43:49 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:8921db27df2831fa6eaa85321205a2470c669b855f3ec95d5a3c2b46de0442c9`  
		Last Modified: Mon, 09 Jan 2023 17:05:45 GMT  
		Size: 3.4 MB (3370628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46ba763279c380b62642251deb522cb55e40fe260ab682de35f8f996055711b0`  
		Last Modified: Tue, 07 Feb 2023 02:44:24 GMT  
		Size: 5.2 MB (5219576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bd0bb18636d36c245afe73516ea39a6f261f808f4983639b201ddccacd55b9f`  
		Last Modified: Tue, 07 Feb 2023 02:44:23 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5caf6e5944e57b92eb19acf938c4c61f7b58c8d4504f368ef63e21fafcfcf56`  
		Last Modified: Tue, 07 Feb 2023 02:44:23 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:d12deb5cddef79e53674a91f6a89b5106ed6c362b41c3a4db5ae2a839a149e85
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.1 MB (8092120 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:392d9e6c7555074305ae94233b635d10c0a78887283578e341bcb9dc14be0fd6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 09 Jan 2023 17:04:54 GMT
ADD file:b15fd8e9f996815394e25f20c8459bfb4c2a8c4074592d6f4c75f4fe79ce537e in / 
# Mon, 09 Jan 2023 17:04:55 GMT
CMD ["/bin/sh"]
# Tue, 07 Feb 2023 01:52:29 GMT
ENV NATS_SERVER=2.9.14
# Tue, 07 Feb 2023 01:52:32 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='6032bc7b2621256e2d9f62f2a987eef490f071bde04dca09786d0270130f9cfd' ;; 		armhf) natsArch='arm6'; sha256='afbee67b87868dc29cf6c382f87813de264572472ac7513a66db6e99fd2a24ac' ;; 		armv7) natsArch='arm7'; sha256='e7e5c019e6cc3d6ef72da80defd5a4f95690b8d108ebb2cfd74fc9c47ac00706' ;; 		x86_64) natsArch='amd64'; sha256='18ac6d0a3956a3d293b85c33822159188b9e75b7597241e2c821e9ded7456601' ;; 		x86) natsArch='386'; sha256='637363cf3ca923c8762ecd083cf83c15cad505ed011ddbbaea857d982a1dadcf' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 07 Feb 2023 01:52:32 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 07 Feb 2023 01:52:32 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 07 Feb 2023 01:52:32 GMT
EXPOSE 4222 6222 8222
# Tue, 07 Feb 2023 01:52:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 07 Feb 2023 01:52:32 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:0269c10e600f3a375f36ddabdbd264ce9503a455f0d0969ce8a00f24eaecc032`  
		Last Modified: Mon, 09 Jan 2023 17:05:45 GMT  
		Size: 3.1 MB (3107243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12f12cb76c0f1aaea4b961abed480010a0742a12af14e5a7529fdcfe4ea1596f`  
		Last Modified: Tue, 07 Feb 2023 01:53:39 GMT  
		Size: 5.0 MB (4983903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcefd563896d4e37ea519c76d11d6f56e2cef47a3e47128072ac72293a6ded78`  
		Last Modified: Tue, 07 Feb 2023 01:53:38 GMT  
		Size: 560.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d426ece1d3a7e9fe54a8109d35cb1b0b91fe9823fa677ed49cea88878081269`  
		Last Modified: Tue, 07 Feb 2023 01:53:38 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:296856ae5e1bddb3fe6aebc65ac14b9d7ff5603959982d746d40db9e076eb62f
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.8 MB (7844570 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90e12165abca9e05e0f5ed3ff69b5461a01997b551fef47f8d6c6e910533341b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 09 Jan 2023 17:06:27 GMT
ADD file:4696f25d0f019b27457c55b3b128b70bf153f38e3e4eb5bdfc21058543313e94 in / 
# Mon, 09 Jan 2023 17:06:27 GMT
CMD ["/bin/sh"]
# Tue, 07 Feb 2023 02:00:38 GMT
ENV NATS_SERVER=2.9.14
# Tue, 07 Feb 2023 02:00:41 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='6032bc7b2621256e2d9f62f2a987eef490f071bde04dca09786d0270130f9cfd' ;; 		armhf) natsArch='arm6'; sha256='afbee67b87868dc29cf6c382f87813de264572472ac7513a66db6e99fd2a24ac' ;; 		armv7) natsArch='arm7'; sha256='e7e5c019e6cc3d6ef72da80defd5a4f95690b8d108ebb2cfd74fc9c47ac00706' ;; 		x86_64) natsArch='amd64'; sha256='18ac6d0a3956a3d293b85c33822159188b9e75b7597241e2c821e9ded7456601' ;; 		x86) natsArch='386'; sha256='637363cf3ca923c8762ecd083cf83c15cad505ed011ddbbaea857d982a1dadcf' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 07 Feb 2023 02:00:41 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 07 Feb 2023 02:00:41 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 07 Feb 2023 02:00:41 GMT
EXPOSE 4222 6222 8222
# Tue, 07 Feb 2023 02:00:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 07 Feb 2023 02:00:41 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:c527615e4ffa2d5b9b777fd469b3b5ba7c1b1e9201c065be2c43569de48a3754`  
		Last Modified: Mon, 09 Jan 2023 17:07:17 GMT  
		Size: 2.9 MB (2865208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28862903dec656beb20cc75d923845dc13689200c1e107e37e28f6e46d8a59b8`  
		Last Modified: Tue, 07 Feb 2023 02:01:53 GMT  
		Size: 5.0 MB (4978388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:937488760d17e32d344f2dd241d52b39400c167c419770a9eaafe9d170a14940`  
		Last Modified: Tue, 07 Feb 2023 02:01:52 GMT  
		Size: 560.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90c32128f2b508d07fc45ca73314749d71f9ba9d40869ce3bb81340feb4708a5`  
		Last Modified: Tue, 07 Feb 2023 02:01:52 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:df31ff3432342b1ede316ebcf7b4e73750286be0d7dabdff093432bf8a4ca8d5
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.1 MB (8065142 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e99541fd7b98de2eee799f260881ced37fb28d95d1b53eac7b31cd80dacba1c8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 09 Jan 2023 17:04:48 GMT
ADD file:3080f19f39259a4b77cc53975de0184c78d4335ceb9ffb77a2838d0539ad6f85 in / 
# Mon, 09 Jan 2023 17:04:49 GMT
CMD ["/bin/sh"]
# Tue, 07 Feb 2023 01:51:39 GMT
ENV NATS_SERVER=2.9.14
# Tue, 07 Feb 2023 01:51:42 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='6032bc7b2621256e2d9f62f2a987eef490f071bde04dca09786d0270130f9cfd' ;; 		armhf) natsArch='arm6'; sha256='afbee67b87868dc29cf6c382f87813de264572472ac7513a66db6e99fd2a24ac' ;; 		armv7) natsArch='arm7'; sha256='e7e5c019e6cc3d6ef72da80defd5a4f95690b8d108ebb2cfd74fc9c47ac00706' ;; 		x86_64) natsArch='amd64'; sha256='18ac6d0a3956a3d293b85c33822159188b9e75b7597241e2c821e9ded7456601' ;; 		x86) natsArch='386'; sha256='637363cf3ca923c8762ecd083cf83c15cad505ed011ddbbaea857d982a1dadcf' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 07 Feb 2023 01:51:42 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 07 Feb 2023 01:51:42 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 07 Feb 2023 01:51:42 GMT
EXPOSE 4222 6222 8222
# Tue, 07 Feb 2023 01:51:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 07 Feb 2023 01:51:42 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:a9eaa45ef418e883481a13c7d84fa9904f2ec56789c52a87ba5a9e6483f2b74f`  
		Last Modified: Mon, 09 Jan 2023 17:05:12 GMT  
		Size: 3.3 MB (3259241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed8a4006f1e7c6891cb29af60ba2447250fe63508a68ff60749aacb11c4df66c`  
		Last Modified: Tue, 07 Feb 2023 01:52:41 GMT  
		Size: 4.8 MB (4804903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99c0cd0fbcf84e908f6acb62f30f2c7ad11d4e7a09b697c1978bc272ece880e0`  
		Last Modified: Tue, 07 Feb 2023 01:52:40 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1a1c2bbc32bebff9300f6366e508a8bf0731b9f69074b6defb83f4af3a1411e`  
		Last Modified: Tue, 07 Feb 2023 01:52:40 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-alpine3.17`

```console
$ docker pull nats@sha256:23353a80fc1fecc883623f6b72759544f596be792aed1db01257ac900ca8d47f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-alpine3.17` - linux; amd64

```console
$ docker pull nats@sha256:2a0dd7504f75410d3b3198dbe094b70521260161f86ce9ec6a90b87548e5a22e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.6 MB (8591202 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9082af6bf2d6856d36cfa41bfd118221042916ab5cdf1ea5e886e9b9040cb97`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 09 Jan 2023 17:05:20 GMT
ADD file:e4d600fc4c9c293efe360be7b30ee96579925d1b4634c94332e2ec73f7d8eca1 in / 
# Mon, 09 Jan 2023 17:05:20 GMT
CMD ["/bin/sh"]
# Tue, 07 Feb 2023 02:43:45 GMT
ENV NATS_SERVER=2.9.14
# Tue, 07 Feb 2023 02:43:48 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='6032bc7b2621256e2d9f62f2a987eef490f071bde04dca09786d0270130f9cfd' ;; 		armhf) natsArch='arm6'; sha256='afbee67b87868dc29cf6c382f87813de264572472ac7513a66db6e99fd2a24ac' ;; 		armv7) natsArch='arm7'; sha256='e7e5c019e6cc3d6ef72da80defd5a4f95690b8d108ebb2cfd74fc9c47ac00706' ;; 		x86_64) natsArch='amd64'; sha256='18ac6d0a3956a3d293b85c33822159188b9e75b7597241e2c821e9ded7456601' ;; 		x86) natsArch='386'; sha256='637363cf3ca923c8762ecd083cf83c15cad505ed011ddbbaea857d982a1dadcf' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 07 Feb 2023 02:43:48 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 07 Feb 2023 02:43:48 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 07 Feb 2023 02:43:48 GMT
EXPOSE 4222 6222 8222
# Tue, 07 Feb 2023 02:43:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 07 Feb 2023 02:43:49 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:8921db27df2831fa6eaa85321205a2470c669b855f3ec95d5a3c2b46de0442c9`  
		Last Modified: Mon, 09 Jan 2023 17:05:45 GMT  
		Size: 3.4 MB (3370628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46ba763279c380b62642251deb522cb55e40fe260ab682de35f8f996055711b0`  
		Last Modified: Tue, 07 Feb 2023 02:44:24 GMT  
		Size: 5.2 MB (5219576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bd0bb18636d36c245afe73516ea39a6f261f808f4983639b201ddccacd55b9f`  
		Last Modified: Tue, 07 Feb 2023 02:44:23 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5caf6e5944e57b92eb19acf938c4c61f7b58c8d4504f368ef63e21fafcfcf56`  
		Last Modified: Tue, 07 Feb 2023 02:44:23 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.17` - linux; arm variant v6

```console
$ docker pull nats@sha256:d12deb5cddef79e53674a91f6a89b5106ed6c362b41c3a4db5ae2a839a149e85
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.1 MB (8092120 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:392d9e6c7555074305ae94233b635d10c0a78887283578e341bcb9dc14be0fd6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 09 Jan 2023 17:04:54 GMT
ADD file:b15fd8e9f996815394e25f20c8459bfb4c2a8c4074592d6f4c75f4fe79ce537e in / 
# Mon, 09 Jan 2023 17:04:55 GMT
CMD ["/bin/sh"]
# Tue, 07 Feb 2023 01:52:29 GMT
ENV NATS_SERVER=2.9.14
# Tue, 07 Feb 2023 01:52:32 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='6032bc7b2621256e2d9f62f2a987eef490f071bde04dca09786d0270130f9cfd' ;; 		armhf) natsArch='arm6'; sha256='afbee67b87868dc29cf6c382f87813de264572472ac7513a66db6e99fd2a24ac' ;; 		armv7) natsArch='arm7'; sha256='e7e5c019e6cc3d6ef72da80defd5a4f95690b8d108ebb2cfd74fc9c47ac00706' ;; 		x86_64) natsArch='amd64'; sha256='18ac6d0a3956a3d293b85c33822159188b9e75b7597241e2c821e9ded7456601' ;; 		x86) natsArch='386'; sha256='637363cf3ca923c8762ecd083cf83c15cad505ed011ddbbaea857d982a1dadcf' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 07 Feb 2023 01:52:32 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 07 Feb 2023 01:52:32 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 07 Feb 2023 01:52:32 GMT
EXPOSE 4222 6222 8222
# Tue, 07 Feb 2023 01:52:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 07 Feb 2023 01:52:32 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:0269c10e600f3a375f36ddabdbd264ce9503a455f0d0969ce8a00f24eaecc032`  
		Last Modified: Mon, 09 Jan 2023 17:05:45 GMT  
		Size: 3.1 MB (3107243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12f12cb76c0f1aaea4b961abed480010a0742a12af14e5a7529fdcfe4ea1596f`  
		Last Modified: Tue, 07 Feb 2023 01:53:39 GMT  
		Size: 5.0 MB (4983903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcefd563896d4e37ea519c76d11d6f56e2cef47a3e47128072ac72293a6ded78`  
		Last Modified: Tue, 07 Feb 2023 01:53:38 GMT  
		Size: 560.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d426ece1d3a7e9fe54a8109d35cb1b0b91fe9823fa677ed49cea88878081269`  
		Last Modified: Tue, 07 Feb 2023 01:53:38 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.17` - linux; arm variant v7

```console
$ docker pull nats@sha256:296856ae5e1bddb3fe6aebc65ac14b9d7ff5603959982d746d40db9e076eb62f
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.8 MB (7844570 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90e12165abca9e05e0f5ed3ff69b5461a01997b551fef47f8d6c6e910533341b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 09 Jan 2023 17:06:27 GMT
ADD file:4696f25d0f019b27457c55b3b128b70bf153f38e3e4eb5bdfc21058543313e94 in / 
# Mon, 09 Jan 2023 17:06:27 GMT
CMD ["/bin/sh"]
# Tue, 07 Feb 2023 02:00:38 GMT
ENV NATS_SERVER=2.9.14
# Tue, 07 Feb 2023 02:00:41 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='6032bc7b2621256e2d9f62f2a987eef490f071bde04dca09786d0270130f9cfd' ;; 		armhf) natsArch='arm6'; sha256='afbee67b87868dc29cf6c382f87813de264572472ac7513a66db6e99fd2a24ac' ;; 		armv7) natsArch='arm7'; sha256='e7e5c019e6cc3d6ef72da80defd5a4f95690b8d108ebb2cfd74fc9c47ac00706' ;; 		x86_64) natsArch='amd64'; sha256='18ac6d0a3956a3d293b85c33822159188b9e75b7597241e2c821e9ded7456601' ;; 		x86) natsArch='386'; sha256='637363cf3ca923c8762ecd083cf83c15cad505ed011ddbbaea857d982a1dadcf' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 07 Feb 2023 02:00:41 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 07 Feb 2023 02:00:41 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 07 Feb 2023 02:00:41 GMT
EXPOSE 4222 6222 8222
# Tue, 07 Feb 2023 02:00:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 07 Feb 2023 02:00:41 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:c527615e4ffa2d5b9b777fd469b3b5ba7c1b1e9201c065be2c43569de48a3754`  
		Last Modified: Mon, 09 Jan 2023 17:07:17 GMT  
		Size: 2.9 MB (2865208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28862903dec656beb20cc75d923845dc13689200c1e107e37e28f6e46d8a59b8`  
		Last Modified: Tue, 07 Feb 2023 02:01:53 GMT  
		Size: 5.0 MB (4978388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:937488760d17e32d344f2dd241d52b39400c167c419770a9eaafe9d170a14940`  
		Last Modified: Tue, 07 Feb 2023 02:01:52 GMT  
		Size: 560.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90c32128f2b508d07fc45ca73314749d71f9ba9d40869ce3bb81340feb4708a5`  
		Last Modified: Tue, 07 Feb 2023 02:01:52 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.17` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:df31ff3432342b1ede316ebcf7b4e73750286be0d7dabdff093432bf8a4ca8d5
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.1 MB (8065142 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e99541fd7b98de2eee799f260881ced37fb28d95d1b53eac7b31cd80dacba1c8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 09 Jan 2023 17:04:48 GMT
ADD file:3080f19f39259a4b77cc53975de0184c78d4335ceb9ffb77a2838d0539ad6f85 in / 
# Mon, 09 Jan 2023 17:04:49 GMT
CMD ["/bin/sh"]
# Tue, 07 Feb 2023 01:51:39 GMT
ENV NATS_SERVER=2.9.14
# Tue, 07 Feb 2023 01:51:42 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='6032bc7b2621256e2d9f62f2a987eef490f071bde04dca09786d0270130f9cfd' ;; 		armhf) natsArch='arm6'; sha256='afbee67b87868dc29cf6c382f87813de264572472ac7513a66db6e99fd2a24ac' ;; 		armv7) natsArch='arm7'; sha256='e7e5c019e6cc3d6ef72da80defd5a4f95690b8d108ebb2cfd74fc9c47ac00706' ;; 		x86_64) natsArch='amd64'; sha256='18ac6d0a3956a3d293b85c33822159188b9e75b7597241e2c821e9ded7456601' ;; 		x86) natsArch='386'; sha256='637363cf3ca923c8762ecd083cf83c15cad505ed011ddbbaea857d982a1dadcf' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 07 Feb 2023 01:51:42 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 07 Feb 2023 01:51:42 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 07 Feb 2023 01:51:42 GMT
EXPOSE 4222 6222 8222
# Tue, 07 Feb 2023 01:51:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 07 Feb 2023 01:51:42 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:a9eaa45ef418e883481a13c7d84fa9904f2ec56789c52a87ba5a9e6483f2b74f`  
		Last Modified: Mon, 09 Jan 2023 17:05:12 GMT  
		Size: 3.3 MB (3259241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed8a4006f1e7c6891cb29af60ba2447250fe63508a68ff60749aacb11c4df66c`  
		Last Modified: Tue, 07 Feb 2023 01:52:41 GMT  
		Size: 4.8 MB (4804903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99c0cd0fbcf84e908f6acb62f30f2c7ad11d4e7a09b697c1978bc272ece880e0`  
		Last Modified: Tue, 07 Feb 2023 01:52:40 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1a1c2bbc32bebff9300f6366e508a8bf0731b9f69074b6defb83f4af3a1411e`  
		Last Modified: Tue, 07 Feb 2023 01:52:40 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-linux`

```console
$ docker pull nats@sha256:eb248ee016566129be55f099933db3c2daa1b235a9831eab265fb9b8324cd269
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-linux` - linux; amd64

```console
$ docker pull nats@sha256:e6916a74a9af2d54502bfa1459a3e0702c00faa14327b3f3b812262e8ada0966
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4933617 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dbb0263a71ad823c35b7c360c016e57737a4367ef1c4909a859acb0ddb4ab19a`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 07 Feb 2023 02:43:58 GMT
COPY file:ac560677dbfad917be71a9245045f536b2801212b542bc63c664d6d11156f4dc in /nats-server 
# Tue, 07 Feb 2023 02:43:58 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 07 Feb 2023 02:43:58 GMT
EXPOSE 4222 6222 8222
# Tue, 07 Feb 2023 02:43:58 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 07 Feb 2023 02:43:59 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 07 Feb 2023 02:43:59 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:5668bc7ee19e1c51e1510bfeee7245e2b2cc66a8b8f8b0f988f4b3bca8729cec`  
		Last Modified: Tue, 07 Feb 2023 02:44:45 GMT  
		Size: 4.9 MB (4933108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93d5b4d77a0e7f6c3fed0f1ae97dbe1b22a3ed4e6af873e7782a0b1d2b992779`  
		Last Modified: Tue, 07 Feb 2023 02:44:44 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:b141eec319986960b56193a2de1a779138beb96cb9945ebc12dbbe199ca96382
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4696311 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89f9b13a403b08d651892f330e0f3dd788a5fb00fd1f6338e79860d306d4504d`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 07 Feb 2023 01:52:41 GMT
COPY file:4eee0f78d63bff3b20fac11aaeb64833cd520dac95605f8f9015e670e58a5ef7 in /nats-server 
# Tue, 07 Feb 2023 01:52:41 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 07 Feb 2023 01:52:41 GMT
EXPOSE 4222 6222 8222
# Tue, 07 Feb 2023 01:52:41 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 07 Feb 2023 01:52:41 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 07 Feb 2023 01:52:41 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6a1ef747dccf7d40d061dc4c857fff9b056d8693e427a2f3adaebc1e22066869`  
		Last Modified: Tue, 07 Feb 2023 01:54:10 GMT  
		Size: 4.7 MB (4695803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc7ba083439d0caacde0ad211a483925f47f6ec3916cf261abe491ac5a630aaf`  
		Last Modified: Tue, 07 Feb 2023 01:54:10 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:ccb41e1e35bee87bcd6a70e43fd88e284140c67701fb8f639781a7b0b7201eb6
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4691076 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a4d042e0f28cb5cfa1b6a77c7eb4e06d62ffbfd2c681f2ca2f1aa747dc538cf`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 07 Feb 2023 02:00:54 GMT
COPY file:5f0ce15e9664bd3755e850351446cf7719b19193e891220c68a9776456e2700a in /nats-server 
# Tue, 07 Feb 2023 02:00:54 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 07 Feb 2023 02:00:54 GMT
EXPOSE 4222 6222 8222
# Tue, 07 Feb 2023 02:00:54 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 07 Feb 2023 02:00:54 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 07 Feb 2023 02:00:54 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:858d33663bc30713d47f7de008a1659f090a1ab8df117e447c1623a289378d31`  
		Last Modified: Tue, 07 Feb 2023 02:02:24 GMT  
		Size: 4.7 MB (4690568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c4973a38193b2d039d297077dd1451a47493f724dd8283e465313c615bcbbb8`  
		Last Modified: Tue, 07 Feb 2023 02:02:23 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:1689ba4ea78e52511a025fdbe524cf1d62dc69c0c2bb68119fabb955e8513246
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4519578 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:96bb932300dca1eb555905232fe9caf2ee65c6b8285cc68e13cf30bb07bd94d3`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 07 Feb 2023 01:52:13 GMT
COPY file:cc453883d11f3e7a77a5f311e510cb07fee2fd66b31eb11f16a5f8023889f08d in /nats-server 
# Tue, 07 Feb 2023 01:52:13 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 07 Feb 2023 01:52:13 GMT
EXPOSE 4222 6222 8222
# Tue, 07 Feb 2023 01:52:13 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 07 Feb 2023 01:52:13 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 07 Feb 2023 01:52:13 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:cf0e5763ec64b26f959ef78ac3641929a51a1fda6989adfd65f04af6f8b3a53a`  
		Last Modified: Tue, 07 Feb 2023 01:53:02 GMT  
		Size: 4.5 MB (4519070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cb009df287c6f73705947a89031473f06a27171a64409e09c24fc061c1863d5`  
		Last Modified: Tue, 07 Feb 2023 01:53:01 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-nanoserver`

```console
$ docker pull nats@sha256:cf75db15a7a309da40d820366d4ca9bbf4f39bc06a401a060ccbc7f0618eea1f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3887; amd64

### `nats:2-nanoserver` - windows version 10.0.17763.3887; amd64

```console
$ docker pull nats@sha256:e6a17bb97fb6a291a4bd98d30c3b9099dedbcf70d12fb062efebaabdb1213bbc
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.7 MB (111659596 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:45804cd0005e5185373d2c577a4257391cd004c68b4c440f4678cf10382b2db7`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 07 Jan 2023 05:17:01 GMT
RUN Apply image 10.0.17763.3887
# Thu, 12 Jan 2023 05:01:51 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Tue, 07 Feb 2023 02:18:03 GMT
RUN cmd /S /C #(nop) COPY file:a45a34d252c029bb58fb3b3e2b3592a2d7869806250714c7b6dc3fb0b305c7bd in C:\nats-server.exe 
# Tue, 07 Feb 2023 02:18:04 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Tue, 07 Feb 2023 02:18:05 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Tue, 07 Feb 2023 02:18:06 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 07 Feb 2023 02:18:06 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:e58f9ad3b15a2a4882ab0a845e8e619cc8c3c411ddbe8b50046c1618a95c1397`  
		Last Modified: Thu, 12 Jan 2023 02:40:44 GMT  
		Size: 106.7 MB (106666138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fe88f4c5f9972ffecb9a66b92e75ddfe48bf7d8d451ace7af3527653f67ff9e`  
		Last Modified: Thu, 12 Jan 2023 05:02:42 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6572a3c131299689497339cc59b098f3601ad482ac0828eeaba7e5f78dc21d76`  
		Last Modified: Tue, 07 Feb 2023 02:18:55 GMT  
		Size: 5.0 MB (4987024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d5a625d40bd2eadd9e49c606bd8fad79a2aa73ebcd3313c3de00a12b06738c7`  
		Last Modified: Tue, 07 Feb 2023 02:18:53 GMT  
		Size: 1.8 KB (1788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9650a5245dfd33f33fb4a5df832057f9d0b34cb3febe41b20095202eda9b58f`  
		Last Modified: Tue, 07 Feb 2023 02:18:53 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15ca02e3d157746bd7381b47df24d65195a307dadd09eba9a311c95481d51b4d`  
		Last Modified: Tue, 07 Feb 2023 02:18:53 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efd2be7007de85b1c3f78a02ae15fdfcf679c7378b8d53403ebe90f39cd16418`  
		Last Modified: Tue, 07 Feb 2023 02:18:53 GMT  
		Size: 1.2 KB (1181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-nanoserver-1809`

```console
$ docker pull nats@sha256:cf75db15a7a309da40d820366d4ca9bbf4f39bc06a401a060ccbc7f0618eea1f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3887; amd64

### `nats:2-nanoserver-1809` - windows version 10.0.17763.3887; amd64

```console
$ docker pull nats@sha256:e6a17bb97fb6a291a4bd98d30c3b9099dedbcf70d12fb062efebaabdb1213bbc
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.7 MB (111659596 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:45804cd0005e5185373d2c577a4257391cd004c68b4c440f4678cf10382b2db7`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 07 Jan 2023 05:17:01 GMT
RUN Apply image 10.0.17763.3887
# Thu, 12 Jan 2023 05:01:51 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Tue, 07 Feb 2023 02:18:03 GMT
RUN cmd /S /C #(nop) COPY file:a45a34d252c029bb58fb3b3e2b3592a2d7869806250714c7b6dc3fb0b305c7bd in C:\nats-server.exe 
# Tue, 07 Feb 2023 02:18:04 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Tue, 07 Feb 2023 02:18:05 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Tue, 07 Feb 2023 02:18:06 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 07 Feb 2023 02:18:06 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:e58f9ad3b15a2a4882ab0a845e8e619cc8c3c411ddbe8b50046c1618a95c1397`  
		Last Modified: Thu, 12 Jan 2023 02:40:44 GMT  
		Size: 106.7 MB (106666138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fe88f4c5f9972ffecb9a66b92e75ddfe48bf7d8d451ace7af3527653f67ff9e`  
		Last Modified: Thu, 12 Jan 2023 05:02:42 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6572a3c131299689497339cc59b098f3601ad482ac0828eeaba7e5f78dc21d76`  
		Last Modified: Tue, 07 Feb 2023 02:18:55 GMT  
		Size: 5.0 MB (4987024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d5a625d40bd2eadd9e49c606bd8fad79a2aa73ebcd3313c3de00a12b06738c7`  
		Last Modified: Tue, 07 Feb 2023 02:18:53 GMT  
		Size: 1.8 KB (1788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9650a5245dfd33f33fb4a5df832057f9d0b34cb3febe41b20095202eda9b58f`  
		Last Modified: Tue, 07 Feb 2023 02:18:53 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15ca02e3d157746bd7381b47df24d65195a307dadd09eba9a311c95481d51b4d`  
		Last Modified: Tue, 07 Feb 2023 02:18:53 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efd2be7007de85b1c3f78a02ae15fdfcf679c7378b8d53403ebe90f39cd16418`  
		Last Modified: Tue, 07 Feb 2023 02:18:53 GMT  
		Size: 1.2 KB (1181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-scratch`

```console
$ docker pull nats@sha256:eb248ee016566129be55f099933db3c2daa1b235a9831eab265fb9b8324cd269
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-scratch` - linux; amd64

```console
$ docker pull nats@sha256:e6916a74a9af2d54502bfa1459a3e0702c00faa14327b3f3b812262e8ada0966
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4933617 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dbb0263a71ad823c35b7c360c016e57737a4367ef1c4909a859acb0ddb4ab19a`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 07 Feb 2023 02:43:58 GMT
COPY file:ac560677dbfad917be71a9245045f536b2801212b542bc63c664d6d11156f4dc in /nats-server 
# Tue, 07 Feb 2023 02:43:58 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 07 Feb 2023 02:43:58 GMT
EXPOSE 4222 6222 8222
# Tue, 07 Feb 2023 02:43:58 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 07 Feb 2023 02:43:59 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 07 Feb 2023 02:43:59 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:5668bc7ee19e1c51e1510bfeee7245e2b2cc66a8b8f8b0f988f4b3bca8729cec`  
		Last Modified: Tue, 07 Feb 2023 02:44:45 GMT  
		Size: 4.9 MB (4933108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93d5b4d77a0e7f6c3fed0f1ae97dbe1b22a3ed4e6af873e7782a0b1d2b992779`  
		Last Modified: Tue, 07 Feb 2023 02:44:44 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:b141eec319986960b56193a2de1a779138beb96cb9945ebc12dbbe199ca96382
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4696311 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89f9b13a403b08d651892f330e0f3dd788a5fb00fd1f6338e79860d306d4504d`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 07 Feb 2023 01:52:41 GMT
COPY file:4eee0f78d63bff3b20fac11aaeb64833cd520dac95605f8f9015e670e58a5ef7 in /nats-server 
# Tue, 07 Feb 2023 01:52:41 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 07 Feb 2023 01:52:41 GMT
EXPOSE 4222 6222 8222
# Tue, 07 Feb 2023 01:52:41 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 07 Feb 2023 01:52:41 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 07 Feb 2023 01:52:41 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6a1ef747dccf7d40d061dc4c857fff9b056d8693e427a2f3adaebc1e22066869`  
		Last Modified: Tue, 07 Feb 2023 01:54:10 GMT  
		Size: 4.7 MB (4695803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc7ba083439d0caacde0ad211a483925f47f6ec3916cf261abe491ac5a630aaf`  
		Last Modified: Tue, 07 Feb 2023 01:54:10 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:ccb41e1e35bee87bcd6a70e43fd88e284140c67701fb8f639781a7b0b7201eb6
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4691076 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a4d042e0f28cb5cfa1b6a77c7eb4e06d62ffbfd2c681f2ca2f1aa747dc538cf`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 07 Feb 2023 02:00:54 GMT
COPY file:5f0ce15e9664bd3755e850351446cf7719b19193e891220c68a9776456e2700a in /nats-server 
# Tue, 07 Feb 2023 02:00:54 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 07 Feb 2023 02:00:54 GMT
EXPOSE 4222 6222 8222
# Tue, 07 Feb 2023 02:00:54 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 07 Feb 2023 02:00:54 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 07 Feb 2023 02:00:54 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:858d33663bc30713d47f7de008a1659f090a1ab8df117e447c1623a289378d31`  
		Last Modified: Tue, 07 Feb 2023 02:02:24 GMT  
		Size: 4.7 MB (4690568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c4973a38193b2d039d297077dd1451a47493f724dd8283e465313c615bcbbb8`  
		Last Modified: Tue, 07 Feb 2023 02:02:23 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:1689ba4ea78e52511a025fdbe524cf1d62dc69c0c2bb68119fabb955e8513246
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4519578 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:96bb932300dca1eb555905232fe9caf2ee65c6b8285cc68e13cf30bb07bd94d3`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 07 Feb 2023 01:52:13 GMT
COPY file:cc453883d11f3e7a77a5f311e510cb07fee2fd66b31eb11f16a5f8023889f08d in /nats-server 
# Tue, 07 Feb 2023 01:52:13 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 07 Feb 2023 01:52:13 GMT
EXPOSE 4222 6222 8222
# Tue, 07 Feb 2023 01:52:13 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 07 Feb 2023 01:52:13 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 07 Feb 2023 01:52:13 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:cf0e5763ec64b26f959ef78ac3641929a51a1fda6989adfd65f04af6f8b3a53a`  
		Last Modified: Tue, 07 Feb 2023 01:53:02 GMT  
		Size: 4.5 MB (4519070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cb009df287c6f73705947a89031473f06a27171a64409e09c24fc061c1863d5`  
		Last Modified: Tue, 07 Feb 2023 01:53:01 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-windowsservercore`

```console
$ docker pull nats@sha256:2f83133d0acce8f6e25329cfa1448835465a15f6f6080d3dea01f044b04cdb6f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3887; amd64

### `nats:2-windowsservercore` - windows version 10.0.17763.3887; amd64

```console
$ docker pull nats@sha256:e0c232bf30691b8afe55af261d4a01f8639efc585516e1eb09940bb851eb8833
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.7 GB (1713683278 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0382d02f9daa152fcd1c45024249998399b9334f6099f446e931d98f771aef58`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Thu, 12 Jan 2023 04:04:12 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Thu, 12 Jan 2023 04:59:53 GMT
ENV NATS_DOCKERIZED=1
# Tue, 07 Feb 2023 02:16:03 GMT
ENV NATS_SERVER=2.9.14
# Tue, 07 Feb 2023 02:16:05 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.9.14/nats-server-v2.9.14-windows-amd64.zip
# Tue, 07 Feb 2023 02:16:05 GMT
ENV NATS_SERVER_SHASUM=b47ca5d88b1a74934145aba3afd6a3b0eee0e543638000cee82b468b8dfbcb3c
# Tue, 07 Feb 2023 02:16:36 GMT
RUN Set-PSDebug -Trace 2
# Tue, 07 Feb 2023 02:17:45 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Tue, 07 Feb 2023 02:17:46 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Tue, 07 Feb 2023 02:17:47 GMT
EXPOSE 4222 6222 8222
# Tue, 07 Feb 2023 02:17:47 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 07 Feb 2023 02:17:48 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f99eee4cf5f23d13a762e719b10916801f19f9df4bd7ff9b4c5cf57133b3dc04`  
		Last Modified: Thu, 12 Jan 2023 04:39:02 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fda92ec365568291ec0ef873b055a8b13d2c46244c129bc4cdf81f0e43e1ec8c`  
		Last Modified: Thu, 12 Jan 2023 05:02:27 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddda27c0ef4ad351d1295efe578196d2003caa62b54a6dee81e4765decf322c9`  
		Last Modified: Tue, 07 Feb 2023 02:18:39 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6375d8bcf5bfd121917c9066a7fc47758ed54929693e46c124d8b34cd701c29`  
		Last Modified: Tue, 07 Feb 2023 02:18:39 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ed0fe5c6e734a1bb638b4e36f3d8cea012a04915c4408581da282286dc6b9ec`  
		Last Modified: Tue, 07 Feb 2023 02:18:39 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83d9c44c9456dd05617593616f2a49404163b5d832e2eb53dda03b1e8b59aec7`  
		Last Modified: Tue, 07 Feb 2023 02:18:39 GMT  
		Size: 382.7 KB (382704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7bcd7fc2e88df50e426c8b75e75d6578f5f036d2f228ed98719dea90187c5db`  
		Last Modified: Tue, 07 Feb 2023 02:18:39 GMT  
		Size: 5.3 MB (5343352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49c9175c6ac4001ff4bc634962943cd35c9bbb984cf1b92653a90a892d15a1bd`  
		Last Modified: Tue, 07 Feb 2023 02:18:37 GMT  
		Size: 2.0 KB (1963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5172837be3b8edccf67687c538bbdc1bfb717ff392a6e6f146469c063e54c0b5`  
		Last Modified: Tue, 07 Feb 2023 02:18:37 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:791a5a7bac5f0d37232a1b86033fb3be57356d147b1c8293d8128faf6ac70c63`  
		Last Modified: Tue, 07 Feb 2023 02:18:37 GMT  
		Size: 1.4 KB (1442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2de08797cefe4c85eb6dd724a5a14d0c72406c8fce9d081ccf86b41210c6171f`  
		Last Modified: Tue, 07 Feb 2023 02:18:37 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-windowsservercore-1809`

```console
$ docker pull nats@sha256:2f83133d0acce8f6e25329cfa1448835465a15f6f6080d3dea01f044b04cdb6f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3887; amd64

### `nats:2-windowsservercore-1809` - windows version 10.0.17763.3887; amd64

```console
$ docker pull nats@sha256:e0c232bf30691b8afe55af261d4a01f8639efc585516e1eb09940bb851eb8833
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.7 GB (1713683278 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0382d02f9daa152fcd1c45024249998399b9334f6099f446e931d98f771aef58`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Thu, 12 Jan 2023 04:04:12 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Thu, 12 Jan 2023 04:59:53 GMT
ENV NATS_DOCKERIZED=1
# Tue, 07 Feb 2023 02:16:03 GMT
ENV NATS_SERVER=2.9.14
# Tue, 07 Feb 2023 02:16:05 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.9.14/nats-server-v2.9.14-windows-amd64.zip
# Tue, 07 Feb 2023 02:16:05 GMT
ENV NATS_SERVER_SHASUM=b47ca5d88b1a74934145aba3afd6a3b0eee0e543638000cee82b468b8dfbcb3c
# Tue, 07 Feb 2023 02:16:36 GMT
RUN Set-PSDebug -Trace 2
# Tue, 07 Feb 2023 02:17:45 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Tue, 07 Feb 2023 02:17:46 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Tue, 07 Feb 2023 02:17:47 GMT
EXPOSE 4222 6222 8222
# Tue, 07 Feb 2023 02:17:47 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 07 Feb 2023 02:17:48 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f99eee4cf5f23d13a762e719b10916801f19f9df4bd7ff9b4c5cf57133b3dc04`  
		Last Modified: Thu, 12 Jan 2023 04:39:02 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fda92ec365568291ec0ef873b055a8b13d2c46244c129bc4cdf81f0e43e1ec8c`  
		Last Modified: Thu, 12 Jan 2023 05:02:27 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddda27c0ef4ad351d1295efe578196d2003caa62b54a6dee81e4765decf322c9`  
		Last Modified: Tue, 07 Feb 2023 02:18:39 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6375d8bcf5bfd121917c9066a7fc47758ed54929693e46c124d8b34cd701c29`  
		Last Modified: Tue, 07 Feb 2023 02:18:39 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ed0fe5c6e734a1bb638b4e36f3d8cea012a04915c4408581da282286dc6b9ec`  
		Last Modified: Tue, 07 Feb 2023 02:18:39 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83d9c44c9456dd05617593616f2a49404163b5d832e2eb53dda03b1e8b59aec7`  
		Last Modified: Tue, 07 Feb 2023 02:18:39 GMT  
		Size: 382.7 KB (382704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7bcd7fc2e88df50e426c8b75e75d6578f5f036d2f228ed98719dea90187c5db`  
		Last Modified: Tue, 07 Feb 2023 02:18:39 GMT  
		Size: 5.3 MB (5343352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49c9175c6ac4001ff4bc634962943cd35c9bbb984cf1b92653a90a892d15a1bd`  
		Last Modified: Tue, 07 Feb 2023 02:18:37 GMT  
		Size: 2.0 KB (1963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5172837be3b8edccf67687c538bbdc1bfb717ff392a6e6f146469c063e54c0b5`  
		Last Modified: Tue, 07 Feb 2023 02:18:37 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:791a5a7bac5f0d37232a1b86033fb3be57356d147b1c8293d8128faf6ac70c63`  
		Last Modified: Tue, 07 Feb 2023 02:18:37 GMT  
		Size: 1.4 KB (1442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2de08797cefe4c85eb6dd724a5a14d0c72406c8fce9d081ccf86b41210c6171f`  
		Last Modified: Tue, 07 Feb 2023 02:18:37 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9`

```console
$ docker pull nats@sha256:f80a2e0337ac068122897636f9f6d686a397ea56f593e0ce0a603cdf41e6e027
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.3887; amd64

### `nats:2.9` - linux; amd64

```console
$ docker pull nats@sha256:e6916a74a9af2d54502bfa1459a3e0702c00faa14327b3f3b812262e8ada0966
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4933617 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dbb0263a71ad823c35b7c360c016e57737a4367ef1c4909a859acb0ddb4ab19a`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 07 Feb 2023 02:43:58 GMT
COPY file:ac560677dbfad917be71a9245045f536b2801212b542bc63c664d6d11156f4dc in /nats-server 
# Tue, 07 Feb 2023 02:43:58 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 07 Feb 2023 02:43:58 GMT
EXPOSE 4222 6222 8222
# Tue, 07 Feb 2023 02:43:58 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 07 Feb 2023 02:43:59 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 07 Feb 2023 02:43:59 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:5668bc7ee19e1c51e1510bfeee7245e2b2cc66a8b8f8b0f988f4b3bca8729cec`  
		Last Modified: Tue, 07 Feb 2023 02:44:45 GMT  
		Size: 4.9 MB (4933108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93d5b4d77a0e7f6c3fed0f1ae97dbe1b22a3ed4e6af873e7782a0b1d2b992779`  
		Last Modified: Tue, 07 Feb 2023 02:44:44 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9` - linux; arm variant v6

```console
$ docker pull nats@sha256:b141eec319986960b56193a2de1a779138beb96cb9945ebc12dbbe199ca96382
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4696311 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89f9b13a403b08d651892f330e0f3dd788a5fb00fd1f6338e79860d306d4504d`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 07 Feb 2023 01:52:41 GMT
COPY file:4eee0f78d63bff3b20fac11aaeb64833cd520dac95605f8f9015e670e58a5ef7 in /nats-server 
# Tue, 07 Feb 2023 01:52:41 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 07 Feb 2023 01:52:41 GMT
EXPOSE 4222 6222 8222
# Tue, 07 Feb 2023 01:52:41 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 07 Feb 2023 01:52:41 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 07 Feb 2023 01:52:41 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6a1ef747dccf7d40d061dc4c857fff9b056d8693e427a2f3adaebc1e22066869`  
		Last Modified: Tue, 07 Feb 2023 01:54:10 GMT  
		Size: 4.7 MB (4695803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc7ba083439d0caacde0ad211a483925f47f6ec3916cf261abe491ac5a630aaf`  
		Last Modified: Tue, 07 Feb 2023 01:54:10 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9` - linux; arm variant v7

```console
$ docker pull nats@sha256:ccb41e1e35bee87bcd6a70e43fd88e284140c67701fb8f639781a7b0b7201eb6
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4691076 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a4d042e0f28cb5cfa1b6a77c7eb4e06d62ffbfd2c681f2ca2f1aa747dc538cf`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 07 Feb 2023 02:00:54 GMT
COPY file:5f0ce15e9664bd3755e850351446cf7719b19193e891220c68a9776456e2700a in /nats-server 
# Tue, 07 Feb 2023 02:00:54 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 07 Feb 2023 02:00:54 GMT
EXPOSE 4222 6222 8222
# Tue, 07 Feb 2023 02:00:54 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 07 Feb 2023 02:00:54 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 07 Feb 2023 02:00:54 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:858d33663bc30713d47f7de008a1659f090a1ab8df117e447c1623a289378d31`  
		Last Modified: Tue, 07 Feb 2023 02:02:24 GMT  
		Size: 4.7 MB (4690568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c4973a38193b2d039d297077dd1451a47493f724dd8283e465313c615bcbbb8`  
		Last Modified: Tue, 07 Feb 2023 02:02:23 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:1689ba4ea78e52511a025fdbe524cf1d62dc69c0c2bb68119fabb955e8513246
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4519578 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:96bb932300dca1eb555905232fe9caf2ee65c6b8285cc68e13cf30bb07bd94d3`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 07 Feb 2023 01:52:13 GMT
COPY file:cc453883d11f3e7a77a5f311e510cb07fee2fd66b31eb11f16a5f8023889f08d in /nats-server 
# Tue, 07 Feb 2023 01:52:13 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 07 Feb 2023 01:52:13 GMT
EXPOSE 4222 6222 8222
# Tue, 07 Feb 2023 01:52:13 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 07 Feb 2023 01:52:13 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 07 Feb 2023 01:52:13 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:cf0e5763ec64b26f959ef78ac3641929a51a1fda6989adfd65f04af6f8b3a53a`  
		Last Modified: Tue, 07 Feb 2023 01:53:02 GMT  
		Size: 4.5 MB (4519070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cb009df287c6f73705947a89031473f06a27171a64409e09c24fc061c1863d5`  
		Last Modified: Tue, 07 Feb 2023 01:53:01 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9` - windows version 10.0.17763.3887; amd64

```console
$ docker pull nats@sha256:e6a17bb97fb6a291a4bd98d30c3b9099dedbcf70d12fb062efebaabdb1213bbc
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.7 MB (111659596 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:45804cd0005e5185373d2c577a4257391cd004c68b4c440f4678cf10382b2db7`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 07 Jan 2023 05:17:01 GMT
RUN Apply image 10.0.17763.3887
# Thu, 12 Jan 2023 05:01:51 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Tue, 07 Feb 2023 02:18:03 GMT
RUN cmd /S /C #(nop) COPY file:a45a34d252c029bb58fb3b3e2b3592a2d7869806250714c7b6dc3fb0b305c7bd in C:\nats-server.exe 
# Tue, 07 Feb 2023 02:18:04 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Tue, 07 Feb 2023 02:18:05 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Tue, 07 Feb 2023 02:18:06 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 07 Feb 2023 02:18:06 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:e58f9ad3b15a2a4882ab0a845e8e619cc8c3c411ddbe8b50046c1618a95c1397`  
		Last Modified: Thu, 12 Jan 2023 02:40:44 GMT  
		Size: 106.7 MB (106666138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fe88f4c5f9972ffecb9a66b92e75ddfe48bf7d8d451ace7af3527653f67ff9e`  
		Last Modified: Thu, 12 Jan 2023 05:02:42 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6572a3c131299689497339cc59b098f3601ad482ac0828eeaba7e5f78dc21d76`  
		Last Modified: Tue, 07 Feb 2023 02:18:55 GMT  
		Size: 5.0 MB (4987024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d5a625d40bd2eadd9e49c606bd8fad79a2aa73ebcd3313c3de00a12b06738c7`  
		Last Modified: Tue, 07 Feb 2023 02:18:53 GMT  
		Size: 1.8 KB (1788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9650a5245dfd33f33fb4a5df832057f9d0b34cb3febe41b20095202eda9b58f`  
		Last Modified: Tue, 07 Feb 2023 02:18:53 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15ca02e3d157746bd7381b47df24d65195a307dadd09eba9a311c95481d51b4d`  
		Last Modified: Tue, 07 Feb 2023 02:18:53 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efd2be7007de85b1c3f78a02ae15fdfcf679c7378b8d53403ebe90f39cd16418`  
		Last Modified: Tue, 07 Feb 2023 02:18:53 GMT  
		Size: 1.2 KB (1181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-alpine`

```console
$ docker pull nats@sha256:23353a80fc1fecc883623f6b72759544f596be792aed1db01257ac900ca8d47f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9-alpine` - linux; amd64

```console
$ docker pull nats@sha256:2a0dd7504f75410d3b3198dbe094b70521260161f86ce9ec6a90b87548e5a22e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.6 MB (8591202 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9082af6bf2d6856d36cfa41bfd118221042916ab5cdf1ea5e886e9b9040cb97`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 09 Jan 2023 17:05:20 GMT
ADD file:e4d600fc4c9c293efe360be7b30ee96579925d1b4634c94332e2ec73f7d8eca1 in / 
# Mon, 09 Jan 2023 17:05:20 GMT
CMD ["/bin/sh"]
# Tue, 07 Feb 2023 02:43:45 GMT
ENV NATS_SERVER=2.9.14
# Tue, 07 Feb 2023 02:43:48 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='6032bc7b2621256e2d9f62f2a987eef490f071bde04dca09786d0270130f9cfd' ;; 		armhf) natsArch='arm6'; sha256='afbee67b87868dc29cf6c382f87813de264572472ac7513a66db6e99fd2a24ac' ;; 		armv7) natsArch='arm7'; sha256='e7e5c019e6cc3d6ef72da80defd5a4f95690b8d108ebb2cfd74fc9c47ac00706' ;; 		x86_64) natsArch='amd64'; sha256='18ac6d0a3956a3d293b85c33822159188b9e75b7597241e2c821e9ded7456601' ;; 		x86) natsArch='386'; sha256='637363cf3ca923c8762ecd083cf83c15cad505ed011ddbbaea857d982a1dadcf' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 07 Feb 2023 02:43:48 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 07 Feb 2023 02:43:48 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 07 Feb 2023 02:43:48 GMT
EXPOSE 4222 6222 8222
# Tue, 07 Feb 2023 02:43:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 07 Feb 2023 02:43:49 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:8921db27df2831fa6eaa85321205a2470c669b855f3ec95d5a3c2b46de0442c9`  
		Last Modified: Mon, 09 Jan 2023 17:05:45 GMT  
		Size: 3.4 MB (3370628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46ba763279c380b62642251deb522cb55e40fe260ab682de35f8f996055711b0`  
		Last Modified: Tue, 07 Feb 2023 02:44:24 GMT  
		Size: 5.2 MB (5219576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bd0bb18636d36c245afe73516ea39a6f261f808f4983639b201ddccacd55b9f`  
		Last Modified: Tue, 07 Feb 2023 02:44:23 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5caf6e5944e57b92eb19acf938c4c61f7b58c8d4504f368ef63e21fafcfcf56`  
		Last Modified: Tue, 07 Feb 2023 02:44:23 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:d12deb5cddef79e53674a91f6a89b5106ed6c362b41c3a4db5ae2a839a149e85
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.1 MB (8092120 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:392d9e6c7555074305ae94233b635d10c0a78887283578e341bcb9dc14be0fd6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 09 Jan 2023 17:04:54 GMT
ADD file:b15fd8e9f996815394e25f20c8459bfb4c2a8c4074592d6f4c75f4fe79ce537e in / 
# Mon, 09 Jan 2023 17:04:55 GMT
CMD ["/bin/sh"]
# Tue, 07 Feb 2023 01:52:29 GMT
ENV NATS_SERVER=2.9.14
# Tue, 07 Feb 2023 01:52:32 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='6032bc7b2621256e2d9f62f2a987eef490f071bde04dca09786d0270130f9cfd' ;; 		armhf) natsArch='arm6'; sha256='afbee67b87868dc29cf6c382f87813de264572472ac7513a66db6e99fd2a24ac' ;; 		armv7) natsArch='arm7'; sha256='e7e5c019e6cc3d6ef72da80defd5a4f95690b8d108ebb2cfd74fc9c47ac00706' ;; 		x86_64) natsArch='amd64'; sha256='18ac6d0a3956a3d293b85c33822159188b9e75b7597241e2c821e9ded7456601' ;; 		x86) natsArch='386'; sha256='637363cf3ca923c8762ecd083cf83c15cad505ed011ddbbaea857d982a1dadcf' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 07 Feb 2023 01:52:32 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 07 Feb 2023 01:52:32 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 07 Feb 2023 01:52:32 GMT
EXPOSE 4222 6222 8222
# Tue, 07 Feb 2023 01:52:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 07 Feb 2023 01:52:32 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:0269c10e600f3a375f36ddabdbd264ce9503a455f0d0969ce8a00f24eaecc032`  
		Last Modified: Mon, 09 Jan 2023 17:05:45 GMT  
		Size: 3.1 MB (3107243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12f12cb76c0f1aaea4b961abed480010a0742a12af14e5a7529fdcfe4ea1596f`  
		Last Modified: Tue, 07 Feb 2023 01:53:39 GMT  
		Size: 5.0 MB (4983903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcefd563896d4e37ea519c76d11d6f56e2cef47a3e47128072ac72293a6ded78`  
		Last Modified: Tue, 07 Feb 2023 01:53:38 GMT  
		Size: 560.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d426ece1d3a7e9fe54a8109d35cb1b0b91fe9823fa677ed49cea88878081269`  
		Last Modified: Tue, 07 Feb 2023 01:53:38 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:296856ae5e1bddb3fe6aebc65ac14b9d7ff5603959982d746d40db9e076eb62f
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.8 MB (7844570 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90e12165abca9e05e0f5ed3ff69b5461a01997b551fef47f8d6c6e910533341b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 09 Jan 2023 17:06:27 GMT
ADD file:4696f25d0f019b27457c55b3b128b70bf153f38e3e4eb5bdfc21058543313e94 in / 
# Mon, 09 Jan 2023 17:06:27 GMT
CMD ["/bin/sh"]
# Tue, 07 Feb 2023 02:00:38 GMT
ENV NATS_SERVER=2.9.14
# Tue, 07 Feb 2023 02:00:41 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='6032bc7b2621256e2d9f62f2a987eef490f071bde04dca09786d0270130f9cfd' ;; 		armhf) natsArch='arm6'; sha256='afbee67b87868dc29cf6c382f87813de264572472ac7513a66db6e99fd2a24ac' ;; 		armv7) natsArch='arm7'; sha256='e7e5c019e6cc3d6ef72da80defd5a4f95690b8d108ebb2cfd74fc9c47ac00706' ;; 		x86_64) natsArch='amd64'; sha256='18ac6d0a3956a3d293b85c33822159188b9e75b7597241e2c821e9ded7456601' ;; 		x86) natsArch='386'; sha256='637363cf3ca923c8762ecd083cf83c15cad505ed011ddbbaea857d982a1dadcf' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 07 Feb 2023 02:00:41 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 07 Feb 2023 02:00:41 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 07 Feb 2023 02:00:41 GMT
EXPOSE 4222 6222 8222
# Tue, 07 Feb 2023 02:00:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 07 Feb 2023 02:00:41 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:c527615e4ffa2d5b9b777fd469b3b5ba7c1b1e9201c065be2c43569de48a3754`  
		Last Modified: Mon, 09 Jan 2023 17:07:17 GMT  
		Size: 2.9 MB (2865208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28862903dec656beb20cc75d923845dc13689200c1e107e37e28f6e46d8a59b8`  
		Last Modified: Tue, 07 Feb 2023 02:01:53 GMT  
		Size: 5.0 MB (4978388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:937488760d17e32d344f2dd241d52b39400c167c419770a9eaafe9d170a14940`  
		Last Modified: Tue, 07 Feb 2023 02:01:52 GMT  
		Size: 560.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90c32128f2b508d07fc45ca73314749d71f9ba9d40869ce3bb81340feb4708a5`  
		Last Modified: Tue, 07 Feb 2023 02:01:52 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:df31ff3432342b1ede316ebcf7b4e73750286be0d7dabdff093432bf8a4ca8d5
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.1 MB (8065142 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e99541fd7b98de2eee799f260881ced37fb28d95d1b53eac7b31cd80dacba1c8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 09 Jan 2023 17:04:48 GMT
ADD file:3080f19f39259a4b77cc53975de0184c78d4335ceb9ffb77a2838d0539ad6f85 in / 
# Mon, 09 Jan 2023 17:04:49 GMT
CMD ["/bin/sh"]
# Tue, 07 Feb 2023 01:51:39 GMT
ENV NATS_SERVER=2.9.14
# Tue, 07 Feb 2023 01:51:42 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='6032bc7b2621256e2d9f62f2a987eef490f071bde04dca09786d0270130f9cfd' ;; 		armhf) natsArch='arm6'; sha256='afbee67b87868dc29cf6c382f87813de264572472ac7513a66db6e99fd2a24ac' ;; 		armv7) natsArch='arm7'; sha256='e7e5c019e6cc3d6ef72da80defd5a4f95690b8d108ebb2cfd74fc9c47ac00706' ;; 		x86_64) natsArch='amd64'; sha256='18ac6d0a3956a3d293b85c33822159188b9e75b7597241e2c821e9ded7456601' ;; 		x86) natsArch='386'; sha256='637363cf3ca923c8762ecd083cf83c15cad505ed011ddbbaea857d982a1dadcf' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 07 Feb 2023 01:51:42 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 07 Feb 2023 01:51:42 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 07 Feb 2023 01:51:42 GMT
EXPOSE 4222 6222 8222
# Tue, 07 Feb 2023 01:51:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 07 Feb 2023 01:51:42 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:a9eaa45ef418e883481a13c7d84fa9904f2ec56789c52a87ba5a9e6483f2b74f`  
		Last Modified: Mon, 09 Jan 2023 17:05:12 GMT  
		Size: 3.3 MB (3259241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed8a4006f1e7c6891cb29af60ba2447250fe63508a68ff60749aacb11c4df66c`  
		Last Modified: Tue, 07 Feb 2023 01:52:41 GMT  
		Size: 4.8 MB (4804903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99c0cd0fbcf84e908f6acb62f30f2c7ad11d4e7a09b697c1978bc272ece880e0`  
		Last Modified: Tue, 07 Feb 2023 01:52:40 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1a1c2bbc32bebff9300f6366e508a8bf0731b9f69074b6defb83f4af3a1411e`  
		Last Modified: Tue, 07 Feb 2023 01:52:40 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-alpine3.17`

```console
$ docker pull nats@sha256:23353a80fc1fecc883623f6b72759544f596be792aed1db01257ac900ca8d47f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9-alpine3.17` - linux; amd64

```console
$ docker pull nats@sha256:2a0dd7504f75410d3b3198dbe094b70521260161f86ce9ec6a90b87548e5a22e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.6 MB (8591202 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9082af6bf2d6856d36cfa41bfd118221042916ab5cdf1ea5e886e9b9040cb97`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 09 Jan 2023 17:05:20 GMT
ADD file:e4d600fc4c9c293efe360be7b30ee96579925d1b4634c94332e2ec73f7d8eca1 in / 
# Mon, 09 Jan 2023 17:05:20 GMT
CMD ["/bin/sh"]
# Tue, 07 Feb 2023 02:43:45 GMT
ENV NATS_SERVER=2.9.14
# Tue, 07 Feb 2023 02:43:48 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='6032bc7b2621256e2d9f62f2a987eef490f071bde04dca09786d0270130f9cfd' ;; 		armhf) natsArch='arm6'; sha256='afbee67b87868dc29cf6c382f87813de264572472ac7513a66db6e99fd2a24ac' ;; 		armv7) natsArch='arm7'; sha256='e7e5c019e6cc3d6ef72da80defd5a4f95690b8d108ebb2cfd74fc9c47ac00706' ;; 		x86_64) natsArch='amd64'; sha256='18ac6d0a3956a3d293b85c33822159188b9e75b7597241e2c821e9ded7456601' ;; 		x86) natsArch='386'; sha256='637363cf3ca923c8762ecd083cf83c15cad505ed011ddbbaea857d982a1dadcf' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 07 Feb 2023 02:43:48 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 07 Feb 2023 02:43:48 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 07 Feb 2023 02:43:48 GMT
EXPOSE 4222 6222 8222
# Tue, 07 Feb 2023 02:43:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 07 Feb 2023 02:43:49 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:8921db27df2831fa6eaa85321205a2470c669b855f3ec95d5a3c2b46de0442c9`  
		Last Modified: Mon, 09 Jan 2023 17:05:45 GMT  
		Size: 3.4 MB (3370628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46ba763279c380b62642251deb522cb55e40fe260ab682de35f8f996055711b0`  
		Last Modified: Tue, 07 Feb 2023 02:44:24 GMT  
		Size: 5.2 MB (5219576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bd0bb18636d36c245afe73516ea39a6f261f808f4983639b201ddccacd55b9f`  
		Last Modified: Tue, 07 Feb 2023 02:44:23 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5caf6e5944e57b92eb19acf938c4c61f7b58c8d4504f368ef63e21fafcfcf56`  
		Last Modified: Tue, 07 Feb 2023 02:44:23 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-alpine3.17` - linux; arm variant v6

```console
$ docker pull nats@sha256:d12deb5cddef79e53674a91f6a89b5106ed6c362b41c3a4db5ae2a839a149e85
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.1 MB (8092120 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:392d9e6c7555074305ae94233b635d10c0a78887283578e341bcb9dc14be0fd6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 09 Jan 2023 17:04:54 GMT
ADD file:b15fd8e9f996815394e25f20c8459bfb4c2a8c4074592d6f4c75f4fe79ce537e in / 
# Mon, 09 Jan 2023 17:04:55 GMT
CMD ["/bin/sh"]
# Tue, 07 Feb 2023 01:52:29 GMT
ENV NATS_SERVER=2.9.14
# Tue, 07 Feb 2023 01:52:32 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='6032bc7b2621256e2d9f62f2a987eef490f071bde04dca09786d0270130f9cfd' ;; 		armhf) natsArch='arm6'; sha256='afbee67b87868dc29cf6c382f87813de264572472ac7513a66db6e99fd2a24ac' ;; 		armv7) natsArch='arm7'; sha256='e7e5c019e6cc3d6ef72da80defd5a4f95690b8d108ebb2cfd74fc9c47ac00706' ;; 		x86_64) natsArch='amd64'; sha256='18ac6d0a3956a3d293b85c33822159188b9e75b7597241e2c821e9ded7456601' ;; 		x86) natsArch='386'; sha256='637363cf3ca923c8762ecd083cf83c15cad505ed011ddbbaea857d982a1dadcf' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 07 Feb 2023 01:52:32 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 07 Feb 2023 01:52:32 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 07 Feb 2023 01:52:32 GMT
EXPOSE 4222 6222 8222
# Tue, 07 Feb 2023 01:52:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 07 Feb 2023 01:52:32 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:0269c10e600f3a375f36ddabdbd264ce9503a455f0d0969ce8a00f24eaecc032`  
		Last Modified: Mon, 09 Jan 2023 17:05:45 GMT  
		Size: 3.1 MB (3107243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12f12cb76c0f1aaea4b961abed480010a0742a12af14e5a7529fdcfe4ea1596f`  
		Last Modified: Tue, 07 Feb 2023 01:53:39 GMT  
		Size: 5.0 MB (4983903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcefd563896d4e37ea519c76d11d6f56e2cef47a3e47128072ac72293a6ded78`  
		Last Modified: Tue, 07 Feb 2023 01:53:38 GMT  
		Size: 560.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d426ece1d3a7e9fe54a8109d35cb1b0b91fe9823fa677ed49cea88878081269`  
		Last Modified: Tue, 07 Feb 2023 01:53:38 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-alpine3.17` - linux; arm variant v7

```console
$ docker pull nats@sha256:296856ae5e1bddb3fe6aebc65ac14b9d7ff5603959982d746d40db9e076eb62f
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.8 MB (7844570 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90e12165abca9e05e0f5ed3ff69b5461a01997b551fef47f8d6c6e910533341b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 09 Jan 2023 17:06:27 GMT
ADD file:4696f25d0f019b27457c55b3b128b70bf153f38e3e4eb5bdfc21058543313e94 in / 
# Mon, 09 Jan 2023 17:06:27 GMT
CMD ["/bin/sh"]
# Tue, 07 Feb 2023 02:00:38 GMT
ENV NATS_SERVER=2.9.14
# Tue, 07 Feb 2023 02:00:41 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='6032bc7b2621256e2d9f62f2a987eef490f071bde04dca09786d0270130f9cfd' ;; 		armhf) natsArch='arm6'; sha256='afbee67b87868dc29cf6c382f87813de264572472ac7513a66db6e99fd2a24ac' ;; 		armv7) natsArch='arm7'; sha256='e7e5c019e6cc3d6ef72da80defd5a4f95690b8d108ebb2cfd74fc9c47ac00706' ;; 		x86_64) natsArch='amd64'; sha256='18ac6d0a3956a3d293b85c33822159188b9e75b7597241e2c821e9ded7456601' ;; 		x86) natsArch='386'; sha256='637363cf3ca923c8762ecd083cf83c15cad505ed011ddbbaea857d982a1dadcf' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 07 Feb 2023 02:00:41 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 07 Feb 2023 02:00:41 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 07 Feb 2023 02:00:41 GMT
EXPOSE 4222 6222 8222
# Tue, 07 Feb 2023 02:00:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 07 Feb 2023 02:00:41 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:c527615e4ffa2d5b9b777fd469b3b5ba7c1b1e9201c065be2c43569de48a3754`  
		Last Modified: Mon, 09 Jan 2023 17:07:17 GMT  
		Size: 2.9 MB (2865208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28862903dec656beb20cc75d923845dc13689200c1e107e37e28f6e46d8a59b8`  
		Last Modified: Tue, 07 Feb 2023 02:01:53 GMT  
		Size: 5.0 MB (4978388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:937488760d17e32d344f2dd241d52b39400c167c419770a9eaafe9d170a14940`  
		Last Modified: Tue, 07 Feb 2023 02:01:52 GMT  
		Size: 560.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90c32128f2b508d07fc45ca73314749d71f9ba9d40869ce3bb81340feb4708a5`  
		Last Modified: Tue, 07 Feb 2023 02:01:52 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-alpine3.17` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:df31ff3432342b1ede316ebcf7b4e73750286be0d7dabdff093432bf8a4ca8d5
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.1 MB (8065142 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e99541fd7b98de2eee799f260881ced37fb28d95d1b53eac7b31cd80dacba1c8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 09 Jan 2023 17:04:48 GMT
ADD file:3080f19f39259a4b77cc53975de0184c78d4335ceb9ffb77a2838d0539ad6f85 in / 
# Mon, 09 Jan 2023 17:04:49 GMT
CMD ["/bin/sh"]
# Tue, 07 Feb 2023 01:51:39 GMT
ENV NATS_SERVER=2.9.14
# Tue, 07 Feb 2023 01:51:42 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='6032bc7b2621256e2d9f62f2a987eef490f071bde04dca09786d0270130f9cfd' ;; 		armhf) natsArch='arm6'; sha256='afbee67b87868dc29cf6c382f87813de264572472ac7513a66db6e99fd2a24ac' ;; 		armv7) natsArch='arm7'; sha256='e7e5c019e6cc3d6ef72da80defd5a4f95690b8d108ebb2cfd74fc9c47ac00706' ;; 		x86_64) natsArch='amd64'; sha256='18ac6d0a3956a3d293b85c33822159188b9e75b7597241e2c821e9ded7456601' ;; 		x86) natsArch='386'; sha256='637363cf3ca923c8762ecd083cf83c15cad505ed011ddbbaea857d982a1dadcf' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 07 Feb 2023 01:51:42 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 07 Feb 2023 01:51:42 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 07 Feb 2023 01:51:42 GMT
EXPOSE 4222 6222 8222
# Tue, 07 Feb 2023 01:51:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 07 Feb 2023 01:51:42 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:a9eaa45ef418e883481a13c7d84fa9904f2ec56789c52a87ba5a9e6483f2b74f`  
		Last Modified: Mon, 09 Jan 2023 17:05:12 GMT  
		Size: 3.3 MB (3259241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed8a4006f1e7c6891cb29af60ba2447250fe63508a68ff60749aacb11c4df66c`  
		Last Modified: Tue, 07 Feb 2023 01:52:41 GMT  
		Size: 4.8 MB (4804903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99c0cd0fbcf84e908f6acb62f30f2c7ad11d4e7a09b697c1978bc272ece880e0`  
		Last Modified: Tue, 07 Feb 2023 01:52:40 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1a1c2bbc32bebff9300f6366e508a8bf0731b9f69074b6defb83f4af3a1411e`  
		Last Modified: Tue, 07 Feb 2023 01:52:40 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-linux`

```console
$ docker pull nats@sha256:eb248ee016566129be55f099933db3c2daa1b235a9831eab265fb9b8324cd269
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9-linux` - linux; amd64

```console
$ docker pull nats@sha256:e6916a74a9af2d54502bfa1459a3e0702c00faa14327b3f3b812262e8ada0966
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4933617 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dbb0263a71ad823c35b7c360c016e57737a4367ef1c4909a859acb0ddb4ab19a`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 07 Feb 2023 02:43:58 GMT
COPY file:ac560677dbfad917be71a9245045f536b2801212b542bc63c664d6d11156f4dc in /nats-server 
# Tue, 07 Feb 2023 02:43:58 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 07 Feb 2023 02:43:58 GMT
EXPOSE 4222 6222 8222
# Tue, 07 Feb 2023 02:43:58 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 07 Feb 2023 02:43:59 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 07 Feb 2023 02:43:59 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:5668bc7ee19e1c51e1510bfeee7245e2b2cc66a8b8f8b0f988f4b3bca8729cec`  
		Last Modified: Tue, 07 Feb 2023 02:44:45 GMT  
		Size: 4.9 MB (4933108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93d5b4d77a0e7f6c3fed0f1ae97dbe1b22a3ed4e6af873e7782a0b1d2b992779`  
		Last Modified: Tue, 07 Feb 2023 02:44:44 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:b141eec319986960b56193a2de1a779138beb96cb9945ebc12dbbe199ca96382
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4696311 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89f9b13a403b08d651892f330e0f3dd788a5fb00fd1f6338e79860d306d4504d`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 07 Feb 2023 01:52:41 GMT
COPY file:4eee0f78d63bff3b20fac11aaeb64833cd520dac95605f8f9015e670e58a5ef7 in /nats-server 
# Tue, 07 Feb 2023 01:52:41 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 07 Feb 2023 01:52:41 GMT
EXPOSE 4222 6222 8222
# Tue, 07 Feb 2023 01:52:41 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 07 Feb 2023 01:52:41 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 07 Feb 2023 01:52:41 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6a1ef747dccf7d40d061dc4c857fff9b056d8693e427a2f3adaebc1e22066869`  
		Last Modified: Tue, 07 Feb 2023 01:54:10 GMT  
		Size: 4.7 MB (4695803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc7ba083439d0caacde0ad211a483925f47f6ec3916cf261abe491ac5a630aaf`  
		Last Modified: Tue, 07 Feb 2023 01:54:10 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:ccb41e1e35bee87bcd6a70e43fd88e284140c67701fb8f639781a7b0b7201eb6
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4691076 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a4d042e0f28cb5cfa1b6a77c7eb4e06d62ffbfd2c681f2ca2f1aa747dc538cf`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 07 Feb 2023 02:00:54 GMT
COPY file:5f0ce15e9664bd3755e850351446cf7719b19193e891220c68a9776456e2700a in /nats-server 
# Tue, 07 Feb 2023 02:00:54 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 07 Feb 2023 02:00:54 GMT
EXPOSE 4222 6222 8222
# Tue, 07 Feb 2023 02:00:54 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 07 Feb 2023 02:00:54 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 07 Feb 2023 02:00:54 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:858d33663bc30713d47f7de008a1659f090a1ab8df117e447c1623a289378d31`  
		Last Modified: Tue, 07 Feb 2023 02:02:24 GMT  
		Size: 4.7 MB (4690568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c4973a38193b2d039d297077dd1451a47493f724dd8283e465313c615bcbbb8`  
		Last Modified: Tue, 07 Feb 2023 02:02:23 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:1689ba4ea78e52511a025fdbe524cf1d62dc69c0c2bb68119fabb955e8513246
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4519578 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:96bb932300dca1eb555905232fe9caf2ee65c6b8285cc68e13cf30bb07bd94d3`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 07 Feb 2023 01:52:13 GMT
COPY file:cc453883d11f3e7a77a5f311e510cb07fee2fd66b31eb11f16a5f8023889f08d in /nats-server 
# Tue, 07 Feb 2023 01:52:13 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 07 Feb 2023 01:52:13 GMT
EXPOSE 4222 6222 8222
# Tue, 07 Feb 2023 01:52:13 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 07 Feb 2023 01:52:13 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 07 Feb 2023 01:52:13 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:cf0e5763ec64b26f959ef78ac3641929a51a1fda6989adfd65f04af6f8b3a53a`  
		Last Modified: Tue, 07 Feb 2023 01:53:02 GMT  
		Size: 4.5 MB (4519070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cb009df287c6f73705947a89031473f06a27171a64409e09c24fc061c1863d5`  
		Last Modified: Tue, 07 Feb 2023 01:53:01 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-nanoserver`

```console
$ docker pull nats@sha256:cf75db15a7a309da40d820366d4ca9bbf4f39bc06a401a060ccbc7f0618eea1f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3887; amd64

### `nats:2.9-nanoserver` - windows version 10.0.17763.3887; amd64

```console
$ docker pull nats@sha256:e6a17bb97fb6a291a4bd98d30c3b9099dedbcf70d12fb062efebaabdb1213bbc
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.7 MB (111659596 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:45804cd0005e5185373d2c577a4257391cd004c68b4c440f4678cf10382b2db7`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 07 Jan 2023 05:17:01 GMT
RUN Apply image 10.0.17763.3887
# Thu, 12 Jan 2023 05:01:51 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Tue, 07 Feb 2023 02:18:03 GMT
RUN cmd /S /C #(nop) COPY file:a45a34d252c029bb58fb3b3e2b3592a2d7869806250714c7b6dc3fb0b305c7bd in C:\nats-server.exe 
# Tue, 07 Feb 2023 02:18:04 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Tue, 07 Feb 2023 02:18:05 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Tue, 07 Feb 2023 02:18:06 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 07 Feb 2023 02:18:06 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:e58f9ad3b15a2a4882ab0a845e8e619cc8c3c411ddbe8b50046c1618a95c1397`  
		Last Modified: Thu, 12 Jan 2023 02:40:44 GMT  
		Size: 106.7 MB (106666138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fe88f4c5f9972ffecb9a66b92e75ddfe48bf7d8d451ace7af3527653f67ff9e`  
		Last Modified: Thu, 12 Jan 2023 05:02:42 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6572a3c131299689497339cc59b098f3601ad482ac0828eeaba7e5f78dc21d76`  
		Last Modified: Tue, 07 Feb 2023 02:18:55 GMT  
		Size: 5.0 MB (4987024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d5a625d40bd2eadd9e49c606bd8fad79a2aa73ebcd3313c3de00a12b06738c7`  
		Last Modified: Tue, 07 Feb 2023 02:18:53 GMT  
		Size: 1.8 KB (1788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9650a5245dfd33f33fb4a5df832057f9d0b34cb3febe41b20095202eda9b58f`  
		Last Modified: Tue, 07 Feb 2023 02:18:53 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15ca02e3d157746bd7381b47df24d65195a307dadd09eba9a311c95481d51b4d`  
		Last Modified: Tue, 07 Feb 2023 02:18:53 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efd2be7007de85b1c3f78a02ae15fdfcf679c7378b8d53403ebe90f39cd16418`  
		Last Modified: Tue, 07 Feb 2023 02:18:53 GMT  
		Size: 1.2 KB (1181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-nanoserver-1809`

```console
$ docker pull nats@sha256:cf75db15a7a309da40d820366d4ca9bbf4f39bc06a401a060ccbc7f0618eea1f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3887; amd64

### `nats:2.9-nanoserver-1809` - windows version 10.0.17763.3887; amd64

```console
$ docker pull nats@sha256:e6a17bb97fb6a291a4bd98d30c3b9099dedbcf70d12fb062efebaabdb1213bbc
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.7 MB (111659596 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:45804cd0005e5185373d2c577a4257391cd004c68b4c440f4678cf10382b2db7`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 07 Jan 2023 05:17:01 GMT
RUN Apply image 10.0.17763.3887
# Thu, 12 Jan 2023 05:01:51 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Tue, 07 Feb 2023 02:18:03 GMT
RUN cmd /S /C #(nop) COPY file:a45a34d252c029bb58fb3b3e2b3592a2d7869806250714c7b6dc3fb0b305c7bd in C:\nats-server.exe 
# Tue, 07 Feb 2023 02:18:04 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Tue, 07 Feb 2023 02:18:05 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Tue, 07 Feb 2023 02:18:06 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 07 Feb 2023 02:18:06 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:e58f9ad3b15a2a4882ab0a845e8e619cc8c3c411ddbe8b50046c1618a95c1397`  
		Last Modified: Thu, 12 Jan 2023 02:40:44 GMT  
		Size: 106.7 MB (106666138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fe88f4c5f9972ffecb9a66b92e75ddfe48bf7d8d451ace7af3527653f67ff9e`  
		Last Modified: Thu, 12 Jan 2023 05:02:42 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6572a3c131299689497339cc59b098f3601ad482ac0828eeaba7e5f78dc21d76`  
		Last Modified: Tue, 07 Feb 2023 02:18:55 GMT  
		Size: 5.0 MB (4987024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d5a625d40bd2eadd9e49c606bd8fad79a2aa73ebcd3313c3de00a12b06738c7`  
		Last Modified: Tue, 07 Feb 2023 02:18:53 GMT  
		Size: 1.8 KB (1788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9650a5245dfd33f33fb4a5df832057f9d0b34cb3febe41b20095202eda9b58f`  
		Last Modified: Tue, 07 Feb 2023 02:18:53 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15ca02e3d157746bd7381b47df24d65195a307dadd09eba9a311c95481d51b4d`  
		Last Modified: Tue, 07 Feb 2023 02:18:53 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efd2be7007de85b1c3f78a02ae15fdfcf679c7378b8d53403ebe90f39cd16418`  
		Last Modified: Tue, 07 Feb 2023 02:18:53 GMT  
		Size: 1.2 KB (1181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-scratch`

```console
$ docker pull nats@sha256:eb248ee016566129be55f099933db3c2daa1b235a9831eab265fb9b8324cd269
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9-scratch` - linux; amd64

```console
$ docker pull nats@sha256:e6916a74a9af2d54502bfa1459a3e0702c00faa14327b3f3b812262e8ada0966
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4933617 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dbb0263a71ad823c35b7c360c016e57737a4367ef1c4909a859acb0ddb4ab19a`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 07 Feb 2023 02:43:58 GMT
COPY file:ac560677dbfad917be71a9245045f536b2801212b542bc63c664d6d11156f4dc in /nats-server 
# Tue, 07 Feb 2023 02:43:58 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 07 Feb 2023 02:43:58 GMT
EXPOSE 4222 6222 8222
# Tue, 07 Feb 2023 02:43:58 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 07 Feb 2023 02:43:59 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 07 Feb 2023 02:43:59 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:5668bc7ee19e1c51e1510bfeee7245e2b2cc66a8b8f8b0f988f4b3bca8729cec`  
		Last Modified: Tue, 07 Feb 2023 02:44:45 GMT  
		Size: 4.9 MB (4933108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93d5b4d77a0e7f6c3fed0f1ae97dbe1b22a3ed4e6af873e7782a0b1d2b992779`  
		Last Modified: Tue, 07 Feb 2023 02:44:44 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:b141eec319986960b56193a2de1a779138beb96cb9945ebc12dbbe199ca96382
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4696311 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89f9b13a403b08d651892f330e0f3dd788a5fb00fd1f6338e79860d306d4504d`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 07 Feb 2023 01:52:41 GMT
COPY file:4eee0f78d63bff3b20fac11aaeb64833cd520dac95605f8f9015e670e58a5ef7 in /nats-server 
# Tue, 07 Feb 2023 01:52:41 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 07 Feb 2023 01:52:41 GMT
EXPOSE 4222 6222 8222
# Tue, 07 Feb 2023 01:52:41 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 07 Feb 2023 01:52:41 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 07 Feb 2023 01:52:41 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6a1ef747dccf7d40d061dc4c857fff9b056d8693e427a2f3adaebc1e22066869`  
		Last Modified: Tue, 07 Feb 2023 01:54:10 GMT  
		Size: 4.7 MB (4695803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc7ba083439d0caacde0ad211a483925f47f6ec3916cf261abe491ac5a630aaf`  
		Last Modified: Tue, 07 Feb 2023 01:54:10 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:ccb41e1e35bee87bcd6a70e43fd88e284140c67701fb8f639781a7b0b7201eb6
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4691076 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a4d042e0f28cb5cfa1b6a77c7eb4e06d62ffbfd2c681f2ca2f1aa747dc538cf`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 07 Feb 2023 02:00:54 GMT
COPY file:5f0ce15e9664bd3755e850351446cf7719b19193e891220c68a9776456e2700a in /nats-server 
# Tue, 07 Feb 2023 02:00:54 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 07 Feb 2023 02:00:54 GMT
EXPOSE 4222 6222 8222
# Tue, 07 Feb 2023 02:00:54 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 07 Feb 2023 02:00:54 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 07 Feb 2023 02:00:54 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:858d33663bc30713d47f7de008a1659f090a1ab8df117e447c1623a289378d31`  
		Last Modified: Tue, 07 Feb 2023 02:02:24 GMT  
		Size: 4.7 MB (4690568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c4973a38193b2d039d297077dd1451a47493f724dd8283e465313c615bcbbb8`  
		Last Modified: Tue, 07 Feb 2023 02:02:23 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:1689ba4ea78e52511a025fdbe524cf1d62dc69c0c2bb68119fabb955e8513246
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4519578 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:96bb932300dca1eb555905232fe9caf2ee65c6b8285cc68e13cf30bb07bd94d3`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 07 Feb 2023 01:52:13 GMT
COPY file:cc453883d11f3e7a77a5f311e510cb07fee2fd66b31eb11f16a5f8023889f08d in /nats-server 
# Tue, 07 Feb 2023 01:52:13 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 07 Feb 2023 01:52:13 GMT
EXPOSE 4222 6222 8222
# Tue, 07 Feb 2023 01:52:13 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 07 Feb 2023 01:52:13 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 07 Feb 2023 01:52:13 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:cf0e5763ec64b26f959ef78ac3641929a51a1fda6989adfd65f04af6f8b3a53a`  
		Last Modified: Tue, 07 Feb 2023 01:53:02 GMT  
		Size: 4.5 MB (4519070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cb009df287c6f73705947a89031473f06a27171a64409e09c24fc061c1863d5`  
		Last Modified: Tue, 07 Feb 2023 01:53:01 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-windowsservercore`

```console
$ docker pull nats@sha256:2f83133d0acce8f6e25329cfa1448835465a15f6f6080d3dea01f044b04cdb6f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3887; amd64

### `nats:2.9-windowsservercore` - windows version 10.0.17763.3887; amd64

```console
$ docker pull nats@sha256:e0c232bf30691b8afe55af261d4a01f8639efc585516e1eb09940bb851eb8833
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.7 GB (1713683278 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0382d02f9daa152fcd1c45024249998399b9334f6099f446e931d98f771aef58`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Thu, 12 Jan 2023 04:04:12 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Thu, 12 Jan 2023 04:59:53 GMT
ENV NATS_DOCKERIZED=1
# Tue, 07 Feb 2023 02:16:03 GMT
ENV NATS_SERVER=2.9.14
# Tue, 07 Feb 2023 02:16:05 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.9.14/nats-server-v2.9.14-windows-amd64.zip
# Tue, 07 Feb 2023 02:16:05 GMT
ENV NATS_SERVER_SHASUM=b47ca5d88b1a74934145aba3afd6a3b0eee0e543638000cee82b468b8dfbcb3c
# Tue, 07 Feb 2023 02:16:36 GMT
RUN Set-PSDebug -Trace 2
# Tue, 07 Feb 2023 02:17:45 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Tue, 07 Feb 2023 02:17:46 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Tue, 07 Feb 2023 02:17:47 GMT
EXPOSE 4222 6222 8222
# Tue, 07 Feb 2023 02:17:47 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 07 Feb 2023 02:17:48 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f99eee4cf5f23d13a762e719b10916801f19f9df4bd7ff9b4c5cf57133b3dc04`  
		Last Modified: Thu, 12 Jan 2023 04:39:02 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fda92ec365568291ec0ef873b055a8b13d2c46244c129bc4cdf81f0e43e1ec8c`  
		Last Modified: Thu, 12 Jan 2023 05:02:27 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddda27c0ef4ad351d1295efe578196d2003caa62b54a6dee81e4765decf322c9`  
		Last Modified: Tue, 07 Feb 2023 02:18:39 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6375d8bcf5bfd121917c9066a7fc47758ed54929693e46c124d8b34cd701c29`  
		Last Modified: Tue, 07 Feb 2023 02:18:39 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ed0fe5c6e734a1bb638b4e36f3d8cea012a04915c4408581da282286dc6b9ec`  
		Last Modified: Tue, 07 Feb 2023 02:18:39 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83d9c44c9456dd05617593616f2a49404163b5d832e2eb53dda03b1e8b59aec7`  
		Last Modified: Tue, 07 Feb 2023 02:18:39 GMT  
		Size: 382.7 KB (382704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7bcd7fc2e88df50e426c8b75e75d6578f5f036d2f228ed98719dea90187c5db`  
		Last Modified: Tue, 07 Feb 2023 02:18:39 GMT  
		Size: 5.3 MB (5343352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49c9175c6ac4001ff4bc634962943cd35c9bbb984cf1b92653a90a892d15a1bd`  
		Last Modified: Tue, 07 Feb 2023 02:18:37 GMT  
		Size: 2.0 KB (1963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5172837be3b8edccf67687c538bbdc1bfb717ff392a6e6f146469c063e54c0b5`  
		Last Modified: Tue, 07 Feb 2023 02:18:37 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:791a5a7bac5f0d37232a1b86033fb3be57356d147b1c8293d8128faf6ac70c63`  
		Last Modified: Tue, 07 Feb 2023 02:18:37 GMT  
		Size: 1.4 KB (1442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2de08797cefe4c85eb6dd724a5a14d0c72406c8fce9d081ccf86b41210c6171f`  
		Last Modified: Tue, 07 Feb 2023 02:18:37 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-windowsservercore-1809`

```console
$ docker pull nats@sha256:2f83133d0acce8f6e25329cfa1448835465a15f6f6080d3dea01f044b04cdb6f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3887; amd64

### `nats:2.9-windowsservercore-1809` - windows version 10.0.17763.3887; amd64

```console
$ docker pull nats@sha256:e0c232bf30691b8afe55af261d4a01f8639efc585516e1eb09940bb851eb8833
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.7 GB (1713683278 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0382d02f9daa152fcd1c45024249998399b9334f6099f446e931d98f771aef58`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Thu, 12 Jan 2023 04:04:12 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Thu, 12 Jan 2023 04:59:53 GMT
ENV NATS_DOCKERIZED=1
# Tue, 07 Feb 2023 02:16:03 GMT
ENV NATS_SERVER=2.9.14
# Tue, 07 Feb 2023 02:16:05 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.9.14/nats-server-v2.9.14-windows-amd64.zip
# Tue, 07 Feb 2023 02:16:05 GMT
ENV NATS_SERVER_SHASUM=b47ca5d88b1a74934145aba3afd6a3b0eee0e543638000cee82b468b8dfbcb3c
# Tue, 07 Feb 2023 02:16:36 GMT
RUN Set-PSDebug -Trace 2
# Tue, 07 Feb 2023 02:17:45 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Tue, 07 Feb 2023 02:17:46 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Tue, 07 Feb 2023 02:17:47 GMT
EXPOSE 4222 6222 8222
# Tue, 07 Feb 2023 02:17:47 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 07 Feb 2023 02:17:48 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f99eee4cf5f23d13a762e719b10916801f19f9df4bd7ff9b4c5cf57133b3dc04`  
		Last Modified: Thu, 12 Jan 2023 04:39:02 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fda92ec365568291ec0ef873b055a8b13d2c46244c129bc4cdf81f0e43e1ec8c`  
		Last Modified: Thu, 12 Jan 2023 05:02:27 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddda27c0ef4ad351d1295efe578196d2003caa62b54a6dee81e4765decf322c9`  
		Last Modified: Tue, 07 Feb 2023 02:18:39 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6375d8bcf5bfd121917c9066a7fc47758ed54929693e46c124d8b34cd701c29`  
		Last Modified: Tue, 07 Feb 2023 02:18:39 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ed0fe5c6e734a1bb638b4e36f3d8cea012a04915c4408581da282286dc6b9ec`  
		Last Modified: Tue, 07 Feb 2023 02:18:39 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83d9c44c9456dd05617593616f2a49404163b5d832e2eb53dda03b1e8b59aec7`  
		Last Modified: Tue, 07 Feb 2023 02:18:39 GMT  
		Size: 382.7 KB (382704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7bcd7fc2e88df50e426c8b75e75d6578f5f036d2f228ed98719dea90187c5db`  
		Last Modified: Tue, 07 Feb 2023 02:18:39 GMT  
		Size: 5.3 MB (5343352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49c9175c6ac4001ff4bc634962943cd35c9bbb984cf1b92653a90a892d15a1bd`  
		Last Modified: Tue, 07 Feb 2023 02:18:37 GMT  
		Size: 2.0 KB (1963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5172837be3b8edccf67687c538bbdc1bfb717ff392a6e6f146469c063e54c0b5`  
		Last Modified: Tue, 07 Feb 2023 02:18:37 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:791a5a7bac5f0d37232a1b86033fb3be57356d147b1c8293d8128faf6ac70c63`  
		Last Modified: Tue, 07 Feb 2023 02:18:37 GMT  
		Size: 1.4 KB (1442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2de08797cefe4c85eb6dd724a5a14d0c72406c8fce9d081ccf86b41210c6171f`  
		Last Modified: Tue, 07 Feb 2023 02:18:37 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.14`

```console
$ docker pull nats@sha256:f80a2e0337ac068122897636f9f6d686a397ea56f593e0ce0a603cdf41e6e027
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.3887; amd64

### `nats:2.9.14` - linux; amd64

```console
$ docker pull nats@sha256:e6916a74a9af2d54502bfa1459a3e0702c00faa14327b3f3b812262e8ada0966
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4933617 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dbb0263a71ad823c35b7c360c016e57737a4367ef1c4909a859acb0ddb4ab19a`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 07 Feb 2023 02:43:58 GMT
COPY file:ac560677dbfad917be71a9245045f536b2801212b542bc63c664d6d11156f4dc in /nats-server 
# Tue, 07 Feb 2023 02:43:58 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 07 Feb 2023 02:43:58 GMT
EXPOSE 4222 6222 8222
# Tue, 07 Feb 2023 02:43:58 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 07 Feb 2023 02:43:59 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 07 Feb 2023 02:43:59 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:5668bc7ee19e1c51e1510bfeee7245e2b2cc66a8b8f8b0f988f4b3bca8729cec`  
		Last Modified: Tue, 07 Feb 2023 02:44:45 GMT  
		Size: 4.9 MB (4933108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93d5b4d77a0e7f6c3fed0f1ae97dbe1b22a3ed4e6af873e7782a0b1d2b992779`  
		Last Modified: Tue, 07 Feb 2023 02:44:44 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.14` - linux; arm variant v6

```console
$ docker pull nats@sha256:b141eec319986960b56193a2de1a779138beb96cb9945ebc12dbbe199ca96382
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4696311 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89f9b13a403b08d651892f330e0f3dd788a5fb00fd1f6338e79860d306d4504d`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 07 Feb 2023 01:52:41 GMT
COPY file:4eee0f78d63bff3b20fac11aaeb64833cd520dac95605f8f9015e670e58a5ef7 in /nats-server 
# Tue, 07 Feb 2023 01:52:41 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 07 Feb 2023 01:52:41 GMT
EXPOSE 4222 6222 8222
# Tue, 07 Feb 2023 01:52:41 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 07 Feb 2023 01:52:41 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 07 Feb 2023 01:52:41 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6a1ef747dccf7d40d061dc4c857fff9b056d8693e427a2f3adaebc1e22066869`  
		Last Modified: Tue, 07 Feb 2023 01:54:10 GMT  
		Size: 4.7 MB (4695803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc7ba083439d0caacde0ad211a483925f47f6ec3916cf261abe491ac5a630aaf`  
		Last Modified: Tue, 07 Feb 2023 01:54:10 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.14` - linux; arm variant v7

```console
$ docker pull nats@sha256:ccb41e1e35bee87bcd6a70e43fd88e284140c67701fb8f639781a7b0b7201eb6
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4691076 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a4d042e0f28cb5cfa1b6a77c7eb4e06d62ffbfd2c681f2ca2f1aa747dc538cf`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 07 Feb 2023 02:00:54 GMT
COPY file:5f0ce15e9664bd3755e850351446cf7719b19193e891220c68a9776456e2700a in /nats-server 
# Tue, 07 Feb 2023 02:00:54 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 07 Feb 2023 02:00:54 GMT
EXPOSE 4222 6222 8222
# Tue, 07 Feb 2023 02:00:54 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 07 Feb 2023 02:00:54 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 07 Feb 2023 02:00:54 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:858d33663bc30713d47f7de008a1659f090a1ab8df117e447c1623a289378d31`  
		Last Modified: Tue, 07 Feb 2023 02:02:24 GMT  
		Size: 4.7 MB (4690568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c4973a38193b2d039d297077dd1451a47493f724dd8283e465313c615bcbbb8`  
		Last Modified: Tue, 07 Feb 2023 02:02:23 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.14` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:1689ba4ea78e52511a025fdbe524cf1d62dc69c0c2bb68119fabb955e8513246
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4519578 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:96bb932300dca1eb555905232fe9caf2ee65c6b8285cc68e13cf30bb07bd94d3`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 07 Feb 2023 01:52:13 GMT
COPY file:cc453883d11f3e7a77a5f311e510cb07fee2fd66b31eb11f16a5f8023889f08d in /nats-server 
# Tue, 07 Feb 2023 01:52:13 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 07 Feb 2023 01:52:13 GMT
EXPOSE 4222 6222 8222
# Tue, 07 Feb 2023 01:52:13 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 07 Feb 2023 01:52:13 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 07 Feb 2023 01:52:13 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:cf0e5763ec64b26f959ef78ac3641929a51a1fda6989adfd65f04af6f8b3a53a`  
		Last Modified: Tue, 07 Feb 2023 01:53:02 GMT  
		Size: 4.5 MB (4519070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cb009df287c6f73705947a89031473f06a27171a64409e09c24fc061c1863d5`  
		Last Modified: Tue, 07 Feb 2023 01:53:01 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.14` - windows version 10.0.17763.3887; amd64

```console
$ docker pull nats@sha256:e6a17bb97fb6a291a4bd98d30c3b9099dedbcf70d12fb062efebaabdb1213bbc
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.7 MB (111659596 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:45804cd0005e5185373d2c577a4257391cd004c68b4c440f4678cf10382b2db7`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 07 Jan 2023 05:17:01 GMT
RUN Apply image 10.0.17763.3887
# Thu, 12 Jan 2023 05:01:51 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Tue, 07 Feb 2023 02:18:03 GMT
RUN cmd /S /C #(nop) COPY file:a45a34d252c029bb58fb3b3e2b3592a2d7869806250714c7b6dc3fb0b305c7bd in C:\nats-server.exe 
# Tue, 07 Feb 2023 02:18:04 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Tue, 07 Feb 2023 02:18:05 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Tue, 07 Feb 2023 02:18:06 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 07 Feb 2023 02:18:06 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:e58f9ad3b15a2a4882ab0a845e8e619cc8c3c411ddbe8b50046c1618a95c1397`  
		Last Modified: Thu, 12 Jan 2023 02:40:44 GMT  
		Size: 106.7 MB (106666138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fe88f4c5f9972ffecb9a66b92e75ddfe48bf7d8d451ace7af3527653f67ff9e`  
		Last Modified: Thu, 12 Jan 2023 05:02:42 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6572a3c131299689497339cc59b098f3601ad482ac0828eeaba7e5f78dc21d76`  
		Last Modified: Tue, 07 Feb 2023 02:18:55 GMT  
		Size: 5.0 MB (4987024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d5a625d40bd2eadd9e49c606bd8fad79a2aa73ebcd3313c3de00a12b06738c7`  
		Last Modified: Tue, 07 Feb 2023 02:18:53 GMT  
		Size: 1.8 KB (1788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9650a5245dfd33f33fb4a5df832057f9d0b34cb3febe41b20095202eda9b58f`  
		Last Modified: Tue, 07 Feb 2023 02:18:53 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15ca02e3d157746bd7381b47df24d65195a307dadd09eba9a311c95481d51b4d`  
		Last Modified: Tue, 07 Feb 2023 02:18:53 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efd2be7007de85b1c3f78a02ae15fdfcf679c7378b8d53403ebe90f39cd16418`  
		Last Modified: Tue, 07 Feb 2023 02:18:53 GMT  
		Size: 1.2 KB (1181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.14-alpine`

```console
$ docker pull nats@sha256:23353a80fc1fecc883623f6b72759544f596be792aed1db01257ac900ca8d47f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9.14-alpine` - linux; amd64

```console
$ docker pull nats@sha256:2a0dd7504f75410d3b3198dbe094b70521260161f86ce9ec6a90b87548e5a22e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.6 MB (8591202 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9082af6bf2d6856d36cfa41bfd118221042916ab5cdf1ea5e886e9b9040cb97`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 09 Jan 2023 17:05:20 GMT
ADD file:e4d600fc4c9c293efe360be7b30ee96579925d1b4634c94332e2ec73f7d8eca1 in / 
# Mon, 09 Jan 2023 17:05:20 GMT
CMD ["/bin/sh"]
# Tue, 07 Feb 2023 02:43:45 GMT
ENV NATS_SERVER=2.9.14
# Tue, 07 Feb 2023 02:43:48 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='6032bc7b2621256e2d9f62f2a987eef490f071bde04dca09786d0270130f9cfd' ;; 		armhf) natsArch='arm6'; sha256='afbee67b87868dc29cf6c382f87813de264572472ac7513a66db6e99fd2a24ac' ;; 		armv7) natsArch='arm7'; sha256='e7e5c019e6cc3d6ef72da80defd5a4f95690b8d108ebb2cfd74fc9c47ac00706' ;; 		x86_64) natsArch='amd64'; sha256='18ac6d0a3956a3d293b85c33822159188b9e75b7597241e2c821e9ded7456601' ;; 		x86) natsArch='386'; sha256='637363cf3ca923c8762ecd083cf83c15cad505ed011ddbbaea857d982a1dadcf' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 07 Feb 2023 02:43:48 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 07 Feb 2023 02:43:48 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 07 Feb 2023 02:43:48 GMT
EXPOSE 4222 6222 8222
# Tue, 07 Feb 2023 02:43:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 07 Feb 2023 02:43:49 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:8921db27df2831fa6eaa85321205a2470c669b855f3ec95d5a3c2b46de0442c9`  
		Last Modified: Mon, 09 Jan 2023 17:05:45 GMT  
		Size: 3.4 MB (3370628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46ba763279c380b62642251deb522cb55e40fe260ab682de35f8f996055711b0`  
		Last Modified: Tue, 07 Feb 2023 02:44:24 GMT  
		Size: 5.2 MB (5219576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bd0bb18636d36c245afe73516ea39a6f261f808f4983639b201ddccacd55b9f`  
		Last Modified: Tue, 07 Feb 2023 02:44:23 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5caf6e5944e57b92eb19acf938c4c61f7b58c8d4504f368ef63e21fafcfcf56`  
		Last Modified: Tue, 07 Feb 2023 02:44:23 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.14-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:d12deb5cddef79e53674a91f6a89b5106ed6c362b41c3a4db5ae2a839a149e85
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.1 MB (8092120 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:392d9e6c7555074305ae94233b635d10c0a78887283578e341bcb9dc14be0fd6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 09 Jan 2023 17:04:54 GMT
ADD file:b15fd8e9f996815394e25f20c8459bfb4c2a8c4074592d6f4c75f4fe79ce537e in / 
# Mon, 09 Jan 2023 17:04:55 GMT
CMD ["/bin/sh"]
# Tue, 07 Feb 2023 01:52:29 GMT
ENV NATS_SERVER=2.9.14
# Tue, 07 Feb 2023 01:52:32 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='6032bc7b2621256e2d9f62f2a987eef490f071bde04dca09786d0270130f9cfd' ;; 		armhf) natsArch='arm6'; sha256='afbee67b87868dc29cf6c382f87813de264572472ac7513a66db6e99fd2a24ac' ;; 		armv7) natsArch='arm7'; sha256='e7e5c019e6cc3d6ef72da80defd5a4f95690b8d108ebb2cfd74fc9c47ac00706' ;; 		x86_64) natsArch='amd64'; sha256='18ac6d0a3956a3d293b85c33822159188b9e75b7597241e2c821e9ded7456601' ;; 		x86) natsArch='386'; sha256='637363cf3ca923c8762ecd083cf83c15cad505ed011ddbbaea857d982a1dadcf' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 07 Feb 2023 01:52:32 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 07 Feb 2023 01:52:32 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 07 Feb 2023 01:52:32 GMT
EXPOSE 4222 6222 8222
# Tue, 07 Feb 2023 01:52:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 07 Feb 2023 01:52:32 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:0269c10e600f3a375f36ddabdbd264ce9503a455f0d0969ce8a00f24eaecc032`  
		Last Modified: Mon, 09 Jan 2023 17:05:45 GMT  
		Size: 3.1 MB (3107243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12f12cb76c0f1aaea4b961abed480010a0742a12af14e5a7529fdcfe4ea1596f`  
		Last Modified: Tue, 07 Feb 2023 01:53:39 GMT  
		Size: 5.0 MB (4983903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcefd563896d4e37ea519c76d11d6f56e2cef47a3e47128072ac72293a6ded78`  
		Last Modified: Tue, 07 Feb 2023 01:53:38 GMT  
		Size: 560.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d426ece1d3a7e9fe54a8109d35cb1b0b91fe9823fa677ed49cea88878081269`  
		Last Modified: Tue, 07 Feb 2023 01:53:38 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.14-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:296856ae5e1bddb3fe6aebc65ac14b9d7ff5603959982d746d40db9e076eb62f
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.8 MB (7844570 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90e12165abca9e05e0f5ed3ff69b5461a01997b551fef47f8d6c6e910533341b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 09 Jan 2023 17:06:27 GMT
ADD file:4696f25d0f019b27457c55b3b128b70bf153f38e3e4eb5bdfc21058543313e94 in / 
# Mon, 09 Jan 2023 17:06:27 GMT
CMD ["/bin/sh"]
# Tue, 07 Feb 2023 02:00:38 GMT
ENV NATS_SERVER=2.9.14
# Tue, 07 Feb 2023 02:00:41 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='6032bc7b2621256e2d9f62f2a987eef490f071bde04dca09786d0270130f9cfd' ;; 		armhf) natsArch='arm6'; sha256='afbee67b87868dc29cf6c382f87813de264572472ac7513a66db6e99fd2a24ac' ;; 		armv7) natsArch='arm7'; sha256='e7e5c019e6cc3d6ef72da80defd5a4f95690b8d108ebb2cfd74fc9c47ac00706' ;; 		x86_64) natsArch='amd64'; sha256='18ac6d0a3956a3d293b85c33822159188b9e75b7597241e2c821e9ded7456601' ;; 		x86) natsArch='386'; sha256='637363cf3ca923c8762ecd083cf83c15cad505ed011ddbbaea857d982a1dadcf' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 07 Feb 2023 02:00:41 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 07 Feb 2023 02:00:41 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 07 Feb 2023 02:00:41 GMT
EXPOSE 4222 6222 8222
# Tue, 07 Feb 2023 02:00:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 07 Feb 2023 02:00:41 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:c527615e4ffa2d5b9b777fd469b3b5ba7c1b1e9201c065be2c43569de48a3754`  
		Last Modified: Mon, 09 Jan 2023 17:07:17 GMT  
		Size: 2.9 MB (2865208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28862903dec656beb20cc75d923845dc13689200c1e107e37e28f6e46d8a59b8`  
		Last Modified: Tue, 07 Feb 2023 02:01:53 GMT  
		Size: 5.0 MB (4978388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:937488760d17e32d344f2dd241d52b39400c167c419770a9eaafe9d170a14940`  
		Last Modified: Tue, 07 Feb 2023 02:01:52 GMT  
		Size: 560.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90c32128f2b508d07fc45ca73314749d71f9ba9d40869ce3bb81340feb4708a5`  
		Last Modified: Tue, 07 Feb 2023 02:01:52 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.14-alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:df31ff3432342b1ede316ebcf7b4e73750286be0d7dabdff093432bf8a4ca8d5
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.1 MB (8065142 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e99541fd7b98de2eee799f260881ced37fb28d95d1b53eac7b31cd80dacba1c8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 09 Jan 2023 17:04:48 GMT
ADD file:3080f19f39259a4b77cc53975de0184c78d4335ceb9ffb77a2838d0539ad6f85 in / 
# Mon, 09 Jan 2023 17:04:49 GMT
CMD ["/bin/sh"]
# Tue, 07 Feb 2023 01:51:39 GMT
ENV NATS_SERVER=2.9.14
# Tue, 07 Feb 2023 01:51:42 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='6032bc7b2621256e2d9f62f2a987eef490f071bde04dca09786d0270130f9cfd' ;; 		armhf) natsArch='arm6'; sha256='afbee67b87868dc29cf6c382f87813de264572472ac7513a66db6e99fd2a24ac' ;; 		armv7) natsArch='arm7'; sha256='e7e5c019e6cc3d6ef72da80defd5a4f95690b8d108ebb2cfd74fc9c47ac00706' ;; 		x86_64) natsArch='amd64'; sha256='18ac6d0a3956a3d293b85c33822159188b9e75b7597241e2c821e9ded7456601' ;; 		x86) natsArch='386'; sha256='637363cf3ca923c8762ecd083cf83c15cad505ed011ddbbaea857d982a1dadcf' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 07 Feb 2023 01:51:42 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 07 Feb 2023 01:51:42 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 07 Feb 2023 01:51:42 GMT
EXPOSE 4222 6222 8222
# Tue, 07 Feb 2023 01:51:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 07 Feb 2023 01:51:42 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:a9eaa45ef418e883481a13c7d84fa9904f2ec56789c52a87ba5a9e6483f2b74f`  
		Last Modified: Mon, 09 Jan 2023 17:05:12 GMT  
		Size: 3.3 MB (3259241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed8a4006f1e7c6891cb29af60ba2447250fe63508a68ff60749aacb11c4df66c`  
		Last Modified: Tue, 07 Feb 2023 01:52:41 GMT  
		Size: 4.8 MB (4804903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99c0cd0fbcf84e908f6acb62f30f2c7ad11d4e7a09b697c1978bc272ece880e0`  
		Last Modified: Tue, 07 Feb 2023 01:52:40 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1a1c2bbc32bebff9300f6366e508a8bf0731b9f69074b6defb83f4af3a1411e`  
		Last Modified: Tue, 07 Feb 2023 01:52:40 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.14-alpine3.17`

```console
$ docker pull nats@sha256:23353a80fc1fecc883623f6b72759544f596be792aed1db01257ac900ca8d47f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9.14-alpine3.17` - linux; amd64

```console
$ docker pull nats@sha256:2a0dd7504f75410d3b3198dbe094b70521260161f86ce9ec6a90b87548e5a22e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.6 MB (8591202 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9082af6bf2d6856d36cfa41bfd118221042916ab5cdf1ea5e886e9b9040cb97`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 09 Jan 2023 17:05:20 GMT
ADD file:e4d600fc4c9c293efe360be7b30ee96579925d1b4634c94332e2ec73f7d8eca1 in / 
# Mon, 09 Jan 2023 17:05:20 GMT
CMD ["/bin/sh"]
# Tue, 07 Feb 2023 02:43:45 GMT
ENV NATS_SERVER=2.9.14
# Tue, 07 Feb 2023 02:43:48 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='6032bc7b2621256e2d9f62f2a987eef490f071bde04dca09786d0270130f9cfd' ;; 		armhf) natsArch='arm6'; sha256='afbee67b87868dc29cf6c382f87813de264572472ac7513a66db6e99fd2a24ac' ;; 		armv7) natsArch='arm7'; sha256='e7e5c019e6cc3d6ef72da80defd5a4f95690b8d108ebb2cfd74fc9c47ac00706' ;; 		x86_64) natsArch='amd64'; sha256='18ac6d0a3956a3d293b85c33822159188b9e75b7597241e2c821e9ded7456601' ;; 		x86) natsArch='386'; sha256='637363cf3ca923c8762ecd083cf83c15cad505ed011ddbbaea857d982a1dadcf' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 07 Feb 2023 02:43:48 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 07 Feb 2023 02:43:48 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 07 Feb 2023 02:43:48 GMT
EXPOSE 4222 6222 8222
# Tue, 07 Feb 2023 02:43:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 07 Feb 2023 02:43:49 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:8921db27df2831fa6eaa85321205a2470c669b855f3ec95d5a3c2b46de0442c9`  
		Last Modified: Mon, 09 Jan 2023 17:05:45 GMT  
		Size: 3.4 MB (3370628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46ba763279c380b62642251deb522cb55e40fe260ab682de35f8f996055711b0`  
		Last Modified: Tue, 07 Feb 2023 02:44:24 GMT  
		Size: 5.2 MB (5219576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bd0bb18636d36c245afe73516ea39a6f261f808f4983639b201ddccacd55b9f`  
		Last Modified: Tue, 07 Feb 2023 02:44:23 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5caf6e5944e57b92eb19acf938c4c61f7b58c8d4504f368ef63e21fafcfcf56`  
		Last Modified: Tue, 07 Feb 2023 02:44:23 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.14-alpine3.17` - linux; arm variant v6

```console
$ docker pull nats@sha256:d12deb5cddef79e53674a91f6a89b5106ed6c362b41c3a4db5ae2a839a149e85
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.1 MB (8092120 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:392d9e6c7555074305ae94233b635d10c0a78887283578e341bcb9dc14be0fd6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 09 Jan 2023 17:04:54 GMT
ADD file:b15fd8e9f996815394e25f20c8459bfb4c2a8c4074592d6f4c75f4fe79ce537e in / 
# Mon, 09 Jan 2023 17:04:55 GMT
CMD ["/bin/sh"]
# Tue, 07 Feb 2023 01:52:29 GMT
ENV NATS_SERVER=2.9.14
# Tue, 07 Feb 2023 01:52:32 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='6032bc7b2621256e2d9f62f2a987eef490f071bde04dca09786d0270130f9cfd' ;; 		armhf) natsArch='arm6'; sha256='afbee67b87868dc29cf6c382f87813de264572472ac7513a66db6e99fd2a24ac' ;; 		armv7) natsArch='arm7'; sha256='e7e5c019e6cc3d6ef72da80defd5a4f95690b8d108ebb2cfd74fc9c47ac00706' ;; 		x86_64) natsArch='amd64'; sha256='18ac6d0a3956a3d293b85c33822159188b9e75b7597241e2c821e9ded7456601' ;; 		x86) natsArch='386'; sha256='637363cf3ca923c8762ecd083cf83c15cad505ed011ddbbaea857d982a1dadcf' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 07 Feb 2023 01:52:32 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 07 Feb 2023 01:52:32 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 07 Feb 2023 01:52:32 GMT
EXPOSE 4222 6222 8222
# Tue, 07 Feb 2023 01:52:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 07 Feb 2023 01:52:32 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:0269c10e600f3a375f36ddabdbd264ce9503a455f0d0969ce8a00f24eaecc032`  
		Last Modified: Mon, 09 Jan 2023 17:05:45 GMT  
		Size: 3.1 MB (3107243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12f12cb76c0f1aaea4b961abed480010a0742a12af14e5a7529fdcfe4ea1596f`  
		Last Modified: Tue, 07 Feb 2023 01:53:39 GMT  
		Size: 5.0 MB (4983903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcefd563896d4e37ea519c76d11d6f56e2cef47a3e47128072ac72293a6ded78`  
		Last Modified: Tue, 07 Feb 2023 01:53:38 GMT  
		Size: 560.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d426ece1d3a7e9fe54a8109d35cb1b0b91fe9823fa677ed49cea88878081269`  
		Last Modified: Tue, 07 Feb 2023 01:53:38 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.14-alpine3.17` - linux; arm variant v7

```console
$ docker pull nats@sha256:296856ae5e1bddb3fe6aebc65ac14b9d7ff5603959982d746d40db9e076eb62f
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.8 MB (7844570 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90e12165abca9e05e0f5ed3ff69b5461a01997b551fef47f8d6c6e910533341b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 09 Jan 2023 17:06:27 GMT
ADD file:4696f25d0f019b27457c55b3b128b70bf153f38e3e4eb5bdfc21058543313e94 in / 
# Mon, 09 Jan 2023 17:06:27 GMT
CMD ["/bin/sh"]
# Tue, 07 Feb 2023 02:00:38 GMT
ENV NATS_SERVER=2.9.14
# Tue, 07 Feb 2023 02:00:41 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='6032bc7b2621256e2d9f62f2a987eef490f071bde04dca09786d0270130f9cfd' ;; 		armhf) natsArch='arm6'; sha256='afbee67b87868dc29cf6c382f87813de264572472ac7513a66db6e99fd2a24ac' ;; 		armv7) natsArch='arm7'; sha256='e7e5c019e6cc3d6ef72da80defd5a4f95690b8d108ebb2cfd74fc9c47ac00706' ;; 		x86_64) natsArch='amd64'; sha256='18ac6d0a3956a3d293b85c33822159188b9e75b7597241e2c821e9ded7456601' ;; 		x86) natsArch='386'; sha256='637363cf3ca923c8762ecd083cf83c15cad505ed011ddbbaea857d982a1dadcf' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 07 Feb 2023 02:00:41 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 07 Feb 2023 02:00:41 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 07 Feb 2023 02:00:41 GMT
EXPOSE 4222 6222 8222
# Tue, 07 Feb 2023 02:00:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 07 Feb 2023 02:00:41 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:c527615e4ffa2d5b9b777fd469b3b5ba7c1b1e9201c065be2c43569de48a3754`  
		Last Modified: Mon, 09 Jan 2023 17:07:17 GMT  
		Size: 2.9 MB (2865208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28862903dec656beb20cc75d923845dc13689200c1e107e37e28f6e46d8a59b8`  
		Last Modified: Tue, 07 Feb 2023 02:01:53 GMT  
		Size: 5.0 MB (4978388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:937488760d17e32d344f2dd241d52b39400c167c419770a9eaafe9d170a14940`  
		Last Modified: Tue, 07 Feb 2023 02:01:52 GMT  
		Size: 560.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90c32128f2b508d07fc45ca73314749d71f9ba9d40869ce3bb81340feb4708a5`  
		Last Modified: Tue, 07 Feb 2023 02:01:52 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.14-alpine3.17` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:df31ff3432342b1ede316ebcf7b4e73750286be0d7dabdff093432bf8a4ca8d5
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.1 MB (8065142 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e99541fd7b98de2eee799f260881ced37fb28d95d1b53eac7b31cd80dacba1c8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 09 Jan 2023 17:04:48 GMT
ADD file:3080f19f39259a4b77cc53975de0184c78d4335ceb9ffb77a2838d0539ad6f85 in / 
# Mon, 09 Jan 2023 17:04:49 GMT
CMD ["/bin/sh"]
# Tue, 07 Feb 2023 01:51:39 GMT
ENV NATS_SERVER=2.9.14
# Tue, 07 Feb 2023 01:51:42 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='6032bc7b2621256e2d9f62f2a987eef490f071bde04dca09786d0270130f9cfd' ;; 		armhf) natsArch='arm6'; sha256='afbee67b87868dc29cf6c382f87813de264572472ac7513a66db6e99fd2a24ac' ;; 		armv7) natsArch='arm7'; sha256='e7e5c019e6cc3d6ef72da80defd5a4f95690b8d108ebb2cfd74fc9c47ac00706' ;; 		x86_64) natsArch='amd64'; sha256='18ac6d0a3956a3d293b85c33822159188b9e75b7597241e2c821e9ded7456601' ;; 		x86) natsArch='386'; sha256='637363cf3ca923c8762ecd083cf83c15cad505ed011ddbbaea857d982a1dadcf' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 07 Feb 2023 01:51:42 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 07 Feb 2023 01:51:42 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 07 Feb 2023 01:51:42 GMT
EXPOSE 4222 6222 8222
# Tue, 07 Feb 2023 01:51:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 07 Feb 2023 01:51:42 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:a9eaa45ef418e883481a13c7d84fa9904f2ec56789c52a87ba5a9e6483f2b74f`  
		Last Modified: Mon, 09 Jan 2023 17:05:12 GMT  
		Size: 3.3 MB (3259241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed8a4006f1e7c6891cb29af60ba2447250fe63508a68ff60749aacb11c4df66c`  
		Last Modified: Tue, 07 Feb 2023 01:52:41 GMT  
		Size: 4.8 MB (4804903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99c0cd0fbcf84e908f6acb62f30f2c7ad11d4e7a09b697c1978bc272ece880e0`  
		Last Modified: Tue, 07 Feb 2023 01:52:40 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1a1c2bbc32bebff9300f6366e508a8bf0731b9f69074b6defb83f4af3a1411e`  
		Last Modified: Tue, 07 Feb 2023 01:52:40 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.14-linux`

```console
$ docker pull nats@sha256:eb248ee016566129be55f099933db3c2daa1b235a9831eab265fb9b8324cd269
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9.14-linux` - linux; amd64

```console
$ docker pull nats@sha256:e6916a74a9af2d54502bfa1459a3e0702c00faa14327b3f3b812262e8ada0966
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4933617 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dbb0263a71ad823c35b7c360c016e57737a4367ef1c4909a859acb0ddb4ab19a`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 07 Feb 2023 02:43:58 GMT
COPY file:ac560677dbfad917be71a9245045f536b2801212b542bc63c664d6d11156f4dc in /nats-server 
# Tue, 07 Feb 2023 02:43:58 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 07 Feb 2023 02:43:58 GMT
EXPOSE 4222 6222 8222
# Tue, 07 Feb 2023 02:43:58 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 07 Feb 2023 02:43:59 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 07 Feb 2023 02:43:59 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:5668bc7ee19e1c51e1510bfeee7245e2b2cc66a8b8f8b0f988f4b3bca8729cec`  
		Last Modified: Tue, 07 Feb 2023 02:44:45 GMT  
		Size: 4.9 MB (4933108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93d5b4d77a0e7f6c3fed0f1ae97dbe1b22a3ed4e6af873e7782a0b1d2b992779`  
		Last Modified: Tue, 07 Feb 2023 02:44:44 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.14-linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:b141eec319986960b56193a2de1a779138beb96cb9945ebc12dbbe199ca96382
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4696311 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89f9b13a403b08d651892f330e0f3dd788a5fb00fd1f6338e79860d306d4504d`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 07 Feb 2023 01:52:41 GMT
COPY file:4eee0f78d63bff3b20fac11aaeb64833cd520dac95605f8f9015e670e58a5ef7 in /nats-server 
# Tue, 07 Feb 2023 01:52:41 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 07 Feb 2023 01:52:41 GMT
EXPOSE 4222 6222 8222
# Tue, 07 Feb 2023 01:52:41 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 07 Feb 2023 01:52:41 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 07 Feb 2023 01:52:41 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6a1ef747dccf7d40d061dc4c857fff9b056d8693e427a2f3adaebc1e22066869`  
		Last Modified: Tue, 07 Feb 2023 01:54:10 GMT  
		Size: 4.7 MB (4695803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc7ba083439d0caacde0ad211a483925f47f6ec3916cf261abe491ac5a630aaf`  
		Last Modified: Tue, 07 Feb 2023 01:54:10 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.14-linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:ccb41e1e35bee87bcd6a70e43fd88e284140c67701fb8f639781a7b0b7201eb6
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4691076 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a4d042e0f28cb5cfa1b6a77c7eb4e06d62ffbfd2c681f2ca2f1aa747dc538cf`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 07 Feb 2023 02:00:54 GMT
COPY file:5f0ce15e9664bd3755e850351446cf7719b19193e891220c68a9776456e2700a in /nats-server 
# Tue, 07 Feb 2023 02:00:54 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 07 Feb 2023 02:00:54 GMT
EXPOSE 4222 6222 8222
# Tue, 07 Feb 2023 02:00:54 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 07 Feb 2023 02:00:54 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 07 Feb 2023 02:00:54 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:858d33663bc30713d47f7de008a1659f090a1ab8df117e447c1623a289378d31`  
		Last Modified: Tue, 07 Feb 2023 02:02:24 GMT  
		Size: 4.7 MB (4690568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c4973a38193b2d039d297077dd1451a47493f724dd8283e465313c615bcbbb8`  
		Last Modified: Tue, 07 Feb 2023 02:02:23 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.14-linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:1689ba4ea78e52511a025fdbe524cf1d62dc69c0c2bb68119fabb955e8513246
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4519578 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:96bb932300dca1eb555905232fe9caf2ee65c6b8285cc68e13cf30bb07bd94d3`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 07 Feb 2023 01:52:13 GMT
COPY file:cc453883d11f3e7a77a5f311e510cb07fee2fd66b31eb11f16a5f8023889f08d in /nats-server 
# Tue, 07 Feb 2023 01:52:13 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 07 Feb 2023 01:52:13 GMT
EXPOSE 4222 6222 8222
# Tue, 07 Feb 2023 01:52:13 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 07 Feb 2023 01:52:13 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 07 Feb 2023 01:52:13 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:cf0e5763ec64b26f959ef78ac3641929a51a1fda6989adfd65f04af6f8b3a53a`  
		Last Modified: Tue, 07 Feb 2023 01:53:02 GMT  
		Size: 4.5 MB (4519070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cb009df287c6f73705947a89031473f06a27171a64409e09c24fc061c1863d5`  
		Last Modified: Tue, 07 Feb 2023 01:53:01 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.14-nanoserver`

```console
$ docker pull nats@sha256:cf75db15a7a309da40d820366d4ca9bbf4f39bc06a401a060ccbc7f0618eea1f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3887; amd64

### `nats:2.9.14-nanoserver` - windows version 10.0.17763.3887; amd64

```console
$ docker pull nats@sha256:e6a17bb97fb6a291a4bd98d30c3b9099dedbcf70d12fb062efebaabdb1213bbc
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.7 MB (111659596 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:45804cd0005e5185373d2c577a4257391cd004c68b4c440f4678cf10382b2db7`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 07 Jan 2023 05:17:01 GMT
RUN Apply image 10.0.17763.3887
# Thu, 12 Jan 2023 05:01:51 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Tue, 07 Feb 2023 02:18:03 GMT
RUN cmd /S /C #(nop) COPY file:a45a34d252c029bb58fb3b3e2b3592a2d7869806250714c7b6dc3fb0b305c7bd in C:\nats-server.exe 
# Tue, 07 Feb 2023 02:18:04 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Tue, 07 Feb 2023 02:18:05 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Tue, 07 Feb 2023 02:18:06 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 07 Feb 2023 02:18:06 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:e58f9ad3b15a2a4882ab0a845e8e619cc8c3c411ddbe8b50046c1618a95c1397`  
		Last Modified: Thu, 12 Jan 2023 02:40:44 GMT  
		Size: 106.7 MB (106666138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fe88f4c5f9972ffecb9a66b92e75ddfe48bf7d8d451ace7af3527653f67ff9e`  
		Last Modified: Thu, 12 Jan 2023 05:02:42 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6572a3c131299689497339cc59b098f3601ad482ac0828eeaba7e5f78dc21d76`  
		Last Modified: Tue, 07 Feb 2023 02:18:55 GMT  
		Size: 5.0 MB (4987024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d5a625d40bd2eadd9e49c606bd8fad79a2aa73ebcd3313c3de00a12b06738c7`  
		Last Modified: Tue, 07 Feb 2023 02:18:53 GMT  
		Size: 1.8 KB (1788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9650a5245dfd33f33fb4a5df832057f9d0b34cb3febe41b20095202eda9b58f`  
		Last Modified: Tue, 07 Feb 2023 02:18:53 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15ca02e3d157746bd7381b47df24d65195a307dadd09eba9a311c95481d51b4d`  
		Last Modified: Tue, 07 Feb 2023 02:18:53 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efd2be7007de85b1c3f78a02ae15fdfcf679c7378b8d53403ebe90f39cd16418`  
		Last Modified: Tue, 07 Feb 2023 02:18:53 GMT  
		Size: 1.2 KB (1181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.14-nanoserver-1809`

```console
$ docker pull nats@sha256:cf75db15a7a309da40d820366d4ca9bbf4f39bc06a401a060ccbc7f0618eea1f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3887; amd64

### `nats:2.9.14-nanoserver-1809` - windows version 10.0.17763.3887; amd64

```console
$ docker pull nats@sha256:e6a17bb97fb6a291a4bd98d30c3b9099dedbcf70d12fb062efebaabdb1213bbc
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.7 MB (111659596 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:45804cd0005e5185373d2c577a4257391cd004c68b4c440f4678cf10382b2db7`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 07 Jan 2023 05:17:01 GMT
RUN Apply image 10.0.17763.3887
# Thu, 12 Jan 2023 05:01:51 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Tue, 07 Feb 2023 02:18:03 GMT
RUN cmd /S /C #(nop) COPY file:a45a34d252c029bb58fb3b3e2b3592a2d7869806250714c7b6dc3fb0b305c7bd in C:\nats-server.exe 
# Tue, 07 Feb 2023 02:18:04 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Tue, 07 Feb 2023 02:18:05 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Tue, 07 Feb 2023 02:18:06 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 07 Feb 2023 02:18:06 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:e58f9ad3b15a2a4882ab0a845e8e619cc8c3c411ddbe8b50046c1618a95c1397`  
		Last Modified: Thu, 12 Jan 2023 02:40:44 GMT  
		Size: 106.7 MB (106666138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fe88f4c5f9972ffecb9a66b92e75ddfe48bf7d8d451ace7af3527653f67ff9e`  
		Last Modified: Thu, 12 Jan 2023 05:02:42 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6572a3c131299689497339cc59b098f3601ad482ac0828eeaba7e5f78dc21d76`  
		Last Modified: Tue, 07 Feb 2023 02:18:55 GMT  
		Size: 5.0 MB (4987024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d5a625d40bd2eadd9e49c606bd8fad79a2aa73ebcd3313c3de00a12b06738c7`  
		Last Modified: Tue, 07 Feb 2023 02:18:53 GMT  
		Size: 1.8 KB (1788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9650a5245dfd33f33fb4a5df832057f9d0b34cb3febe41b20095202eda9b58f`  
		Last Modified: Tue, 07 Feb 2023 02:18:53 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15ca02e3d157746bd7381b47df24d65195a307dadd09eba9a311c95481d51b4d`  
		Last Modified: Tue, 07 Feb 2023 02:18:53 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efd2be7007de85b1c3f78a02ae15fdfcf679c7378b8d53403ebe90f39cd16418`  
		Last Modified: Tue, 07 Feb 2023 02:18:53 GMT  
		Size: 1.2 KB (1181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.14-scratch`

```console
$ docker pull nats@sha256:eb248ee016566129be55f099933db3c2daa1b235a9831eab265fb9b8324cd269
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9.14-scratch` - linux; amd64

```console
$ docker pull nats@sha256:e6916a74a9af2d54502bfa1459a3e0702c00faa14327b3f3b812262e8ada0966
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4933617 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dbb0263a71ad823c35b7c360c016e57737a4367ef1c4909a859acb0ddb4ab19a`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 07 Feb 2023 02:43:58 GMT
COPY file:ac560677dbfad917be71a9245045f536b2801212b542bc63c664d6d11156f4dc in /nats-server 
# Tue, 07 Feb 2023 02:43:58 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 07 Feb 2023 02:43:58 GMT
EXPOSE 4222 6222 8222
# Tue, 07 Feb 2023 02:43:58 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 07 Feb 2023 02:43:59 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 07 Feb 2023 02:43:59 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:5668bc7ee19e1c51e1510bfeee7245e2b2cc66a8b8f8b0f988f4b3bca8729cec`  
		Last Modified: Tue, 07 Feb 2023 02:44:45 GMT  
		Size: 4.9 MB (4933108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93d5b4d77a0e7f6c3fed0f1ae97dbe1b22a3ed4e6af873e7782a0b1d2b992779`  
		Last Modified: Tue, 07 Feb 2023 02:44:44 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.14-scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:b141eec319986960b56193a2de1a779138beb96cb9945ebc12dbbe199ca96382
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4696311 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89f9b13a403b08d651892f330e0f3dd788a5fb00fd1f6338e79860d306d4504d`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 07 Feb 2023 01:52:41 GMT
COPY file:4eee0f78d63bff3b20fac11aaeb64833cd520dac95605f8f9015e670e58a5ef7 in /nats-server 
# Tue, 07 Feb 2023 01:52:41 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 07 Feb 2023 01:52:41 GMT
EXPOSE 4222 6222 8222
# Tue, 07 Feb 2023 01:52:41 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 07 Feb 2023 01:52:41 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 07 Feb 2023 01:52:41 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6a1ef747dccf7d40d061dc4c857fff9b056d8693e427a2f3adaebc1e22066869`  
		Last Modified: Tue, 07 Feb 2023 01:54:10 GMT  
		Size: 4.7 MB (4695803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc7ba083439d0caacde0ad211a483925f47f6ec3916cf261abe491ac5a630aaf`  
		Last Modified: Tue, 07 Feb 2023 01:54:10 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.14-scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:ccb41e1e35bee87bcd6a70e43fd88e284140c67701fb8f639781a7b0b7201eb6
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4691076 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a4d042e0f28cb5cfa1b6a77c7eb4e06d62ffbfd2c681f2ca2f1aa747dc538cf`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 07 Feb 2023 02:00:54 GMT
COPY file:5f0ce15e9664bd3755e850351446cf7719b19193e891220c68a9776456e2700a in /nats-server 
# Tue, 07 Feb 2023 02:00:54 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 07 Feb 2023 02:00:54 GMT
EXPOSE 4222 6222 8222
# Tue, 07 Feb 2023 02:00:54 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 07 Feb 2023 02:00:54 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 07 Feb 2023 02:00:54 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:858d33663bc30713d47f7de008a1659f090a1ab8df117e447c1623a289378d31`  
		Last Modified: Tue, 07 Feb 2023 02:02:24 GMT  
		Size: 4.7 MB (4690568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c4973a38193b2d039d297077dd1451a47493f724dd8283e465313c615bcbbb8`  
		Last Modified: Tue, 07 Feb 2023 02:02:23 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.14-scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:1689ba4ea78e52511a025fdbe524cf1d62dc69c0c2bb68119fabb955e8513246
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4519578 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:96bb932300dca1eb555905232fe9caf2ee65c6b8285cc68e13cf30bb07bd94d3`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 07 Feb 2023 01:52:13 GMT
COPY file:cc453883d11f3e7a77a5f311e510cb07fee2fd66b31eb11f16a5f8023889f08d in /nats-server 
# Tue, 07 Feb 2023 01:52:13 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 07 Feb 2023 01:52:13 GMT
EXPOSE 4222 6222 8222
# Tue, 07 Feb 2023 01:52:13 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 07 Feb 2023 01:52:13 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 07 Feb 2023 01:52:13 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:cf0e5763ec64b26f959ef78ac3641929a51a1fda6989adfd65f04af6f8b3a53a`  
		Last Modified: Tue, 07 Feb 2023 01:53:02 GMT  
		Size: 4.5 MB (4519070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cb009df287c6f73705947a89031473f06a27171a64409e09c24fc061c1863d5`  
		Last Modified: Tue, 07 Feb 2023 01:53:01 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.14-windowsservercore`

```console
$ docker pull nats@sha256:2f83133d0acce8f6e25329cfa1448835465a15f6f6080d3dea01f044b04cdb6f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3887; amd64

### `nats:2.9.14-windowsservercore` - windows version 10.0.17763.3887; amd64

```console
$ docker pull nats@sha256:e0c232bf30691b8afe55af261d4a01f8639efc585516e1eb09940bb851eb8833
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.7 GB (1713683278 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0382d02f9daa152fcd1c45024249998399b9334f6099f446e931d98f771aef58`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Thu, 12 Jan 2023 04:04:12 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Thu, 12 Jan 2023 04:59:53 GMT
ENV NATS_DOCKERIZED=1
# Tue, 07 Feb 2023 02:16:03 GMT
ENV NATS_SERVER=2.9.14
# Tue, 07 Feb 2023 02:16:05 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.9.14/nats-server-v2.9.14-windows-amd64.zip
# Tue, 07 Feb 2023 02:16:05 GMT
ENV NATS_SERVER_SHASUM=b47ca5d88b1a74934145aba3afd6a3b0eee0e543638000cee82b468b8dfbcb3c
# Tue, 07 Feb 2023 02:16:36 GMT
RUN Set-PSDebug -Trace 2
# Tue, 07 Feb 2023 02:17:45 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Tue, 07 Feb 2023 02:17:46 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Tue, 07 Feb 2023 02:17:47 GMT
EXPOSE 4222 6222 8222
# Tue, 07 Feb 2023 02:17:47 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 07 Feb 2023 02:17:48 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f99eee4cf5f23d13a762e719b10916801f19f9df4bd7ff9b4c5cf57133b3dc04`  
		Last Modified: Thu, 12 Jan 2023 04:39:02 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fda92ec365568291ec0ef873b055a8b13d2c46244c129bc4cdf81f0e43e1ec8c`  
		Last Modified: Thu, 12 Jan 2023 05:02:27 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddda27c0ef4ad351d1295efe578196d2003caa62b54a6dee81e4765decf322c9`  
		Last Modified: Tue, 07 Feb 2023 02:18:39 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6375d8bcf5bfd121917c9066a7fc47758ed54929693e46c124d8b34cd701c29`  
		Last Modified: Tue, 07 Feb 2023 02:18:39 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ed0fe5c6e734a1bb638b4e36f3d8cea012a04915c4408581da282286dc6b9ec`  
		Last Modified: Tue, 07 Feb 2023 02:18:39 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83d9c44c9456dd05617593616f2a49404163b5d832e2eb53dda03b1e8b59aec7`  
		Last Modified: Tue, 07 Feb 2023 02:18:39 GMT  
		Size: 382.7 KB (382704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7bcd7fc2e88df50e426c8b75e75d6578f5f036d2f228ed98719dea90187c5db`  
		Last Modified: Tue, 07 Feb 2023 02:18:39 GMT  
		Size: 5.3 MB (5343352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49c9175c6ac4001ff4bc634962943cd35c9bbb984cf1b92653a90a892d15a1bd`  
		Last Modified: Tue, 07 Feb 2023 02:18:37 GMT  
		Size: 2.0 KB (1963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5172837be3b8edccf67687c538bbdc1bfb717ff392a6e6f146469c063e54c0b5`  
		Last Modified: Tue, 07 Feb 2023 02:18:37 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:791a5a7bac5f0d37232a1b86033fb3be57356d147b1c8293d8128faf6ac70c63`  
		Last Modified: Tue, 07 Feb 2023 02:18:37 GMT  
		Size: 1.4 KB (1442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2de08797cefe4c85eb6dd724a5a14d0c72406c8fce9d081ccf86b41210c6171f`  
		Last Modified: Tue, 07 Feb 2023 02:18:37 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.14-windowsservercore-1809`

```console
$ docker pull nats@sha256:2f83133d0acce8f6e25329cfa1448835465a15f6f6080d3dea01f044b04cdb6f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3887; amd64

### `nats:2.9.14-windowsservercore-1809` - windows version 10.0.17763.3887; amd64

```console
$ docker pull nats@sha256:e0c232bf30691b8afe55af261d4a01f8639efc585516e1eb09940bb851eb8833
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.7 GB (1713683278 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0382d02f9daa152fcd1c45024249998399b9334f6099f446e931d98f771aef58`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Thu, 12 Jan 2023 04:04:12 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Thu, 12 Jan 2023 04:59:53 GMT
ENV NATS_DOCKERIZED=1
# Tue, 07 Feb 2023 02:16:03 GMT
ENV NATS_SERVER=2.9.14
# Tue, 07 Feb 2023 02:16:05 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.9.14/nats-server-v2.9.14-windows-amd64.zip
# Tue, 07 Feb 2023 02:16:05 GMT
ENV NATS_SERVER_SHASUM=b47ca5d88b1a74934145aba3afd6a3b0eee0e543638000cee82b468b8dfbcb3c
# Tue, 07 Feb 2023 02:16:36 GMT
RUN Set-PSDebug -Trace 2
# Tue, 07 Feb 2023 02:17:45 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Tue, 07 Feb 2023 02:17:46 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Tue, 07 Feb 2023 02:17:47 GMT
EXPOSE 4222 6222 8222
# Tue, 07 Feb 2023 02:17:47 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 07 Feb 2023 02:17:48 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f99eee4cf5f23d13a762e719b10916801f19f9df4bd7ff9b4c5cf57133b3dc04`  
		Last Modified: Thu, 12 Jan 2023 04:39:02 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fda92ec365568291ec0ef873b055a8b13d2c46244c129bc4cdf81f0e43e1ec8c`  
		Last Modified: Thu, 12 Jan 2023 05:02:27 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddda27c0ef4ad351d1295efe578196d2003caa62b54a6dee81e4765decf322c9`  
		Last Modified: Tue, 07 Feb 2023 02:18:39 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6375d8bcf5bfd121917c9066a7fc47758ed54929693e46c124d8b34cd701c29`  
		Last Modified: Tue, 07 Feb 2023 02:18:39 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ed0fe5c6e734a1bb638b4e36f3d8cea012a04915c4408581da282286dc6b9ec`  
		Last Modified: Tue, 07 Feb 2023 02:18:39 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83d9c44c9456dd05617593616f2a49404163b5d832e2eb53dda03b1e8b59aec7`  
		Last Modified: Tue, 07 Feb 2023 02:18:39 GMT  
		Size: 382.7 KB (382704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7bcd7fc2e88df50e426c8b75e75d6578f5f036d2f228ed98719dea90187c5db`  
		Last Modified: Tue, 07 Feb 2023 02:18:39 GMT  
		Size: 5.3 MB (5343352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49c9175c6ac4001ff4bc634962943cd35c9bbb984cf1b92653a90a892d15a1bd`  
		Last Modified: Tue, 07 Feb 2023 02:18:37 GMT  
		Size: 2.0 KB (1963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5172837be3b8edccf67687c538bbdc1bfb717ff392a6e6f146469c063e54c0b5`  
		Last Modified: Tue, 07 Feb 2023 02:18:37 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:791a5a7bac5f0d37232a1b86033fb3be57356d147b1c8293d8128faf6ac70c63`  
		Last Modified: Tue, 07 Feb 2023 02:18:37 GMT  
		Size: 1.4 KB (1442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2de08797cefe4c85eb6dd724a5a14d0c72406c8fce9d081ccf86b41210c6171f`  
		Last Modified: Tue, 07 Feb 2023 02:18:37 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:alpine`

```console
$ docker pull nats@sha256:23353a80fc1fecc883623f6b72759544f596be792aed1db01257ac900ca8d47f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:alpine` - linux; amd64

```console
$ docker pull nats@sha256:2a0dd7504f75410d3b3198dbe094b70521260161f86ce9ec6a90b87548e5a22e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.6 MB (8591202 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9082af6bf2d6856d36cfa41bfd118221042916ab5cdf1ea5e886e9b9040cb97`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 09 Jan 2023 17:05:20 GMT
ADD file:e4d600fc4c9c293efe360be7b30ee96579925d1b4634c94332e2ec73f7d8eca1 in / 
# Mon, 09 Jan 2023 17:05:20 GMT
CMD ["/bin/sh"]
# Tue, 07 Feb 2023 02:43:45 GMT
ENV NATS_SERVER=2.9.14
# Tue, 07 Feb 2023 02:43:48 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='6032bc7b2621256e2d9f62f2a987eef490f071bde04dca09786d0270130f9cfd' ;; 		armhf) natsArch='arm6'; sha256='afbee67b87868dc29cf6c382f87813de264572472ac7513a66db6e99fd2a24ac' ;; 		armv7) natsArch='arm7'; sha256='e7e5c019e6cc3d6ef72da80defd5a4f95690b8d108ebb2cfd74fc9c47ac00706' ;; 		x86_64) natsArch='amd64'; sha256='18ac6d0a3956a3d293b85c33822159188b9e75b7597241e2c821e9ded7456601' ;; 		x86) natsArch='386'; sha256='637363cf3ca923c8762ecd083cf83c15cad505ed011ddbbaea857d982a1dadcf' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 07 Feb 2023 02:43:48 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 07 Feb 2023 02:43:48 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 07 Feb 2023 02:43:48 GMT
EXPOSE 4222 6222 8222
# Tue, 07 Feb 2023 02:43:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 07 Feb 2023 02:43:49 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:8921db27df2831fa6eaa85321205a2470c669b855f3ec95d5a3c2b46de0442c9`  
		Last Modified: Mon, 09 Jan 2023 17:05:45 GMT  
		Size: 3.4 MB (3370628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46ba763279c380b62642251deb522cb55e40fe260ab682de35f8f996055711b0`  
		Last Modified: Tue, 07 Feb 2023 02:44:24 GMT  
		Size: 5.2 MB (5219576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bd0bb18636d36c245afe73516ea39a6f261f808f4983639b201ddccacd55b9f`  
		Last Modified: Tue, 07 Feb 2023 02:44:23 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5caf6e5944e57b92eb19acf938c4c61f7b58c8d4504f368ef63e21fafcfcf56`  
		Last Modified: Tue, 07 Feb 2023 02:44:23 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:d12deb5cddef79e53674a91f6a89b5106ed6c362b41c3a4db5ae2a839a149e85
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.1 MB (8092120 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:392d9e6c7555074305ae94233b635d10c0a78887283578e341bcb9dc14be0fd6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 09 Jan 2023 17:04:54 GMT
ADD file:b15fd8e9f996815394e25f20c8459bfb4c2a8c4074592d6f4c75f4fe79ce537e in / 
# Mon, 09 Jan 2023 17:04:55 GMT
CMD ["/bin/sh"]
# Tue, 07 Feb 2023 01:52:29 GMT
ENV NATS_SERVER=2.9.14
# Tue, 07 Feb 2023 01:52:32 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='6032bc7b2621256e2d9f62f2a987eef490f071bde04dca09786d0270130f9cfd' ;; 		armhf) natsArch='arm6'; sha256='afbee67b87868dc29cf6c382f87813de264572472ac7513a66db6e99fd2a24ac' ;; 		armv7) natsArch='arm7'; sha256='e7e5c019e6cc3d6ef72da80defd5a4f95690b8d108ebb2cfd74fc9c47ac00706' ;; 		x86_64) natsArch='amd64'; sha256='18ac6d0a3956a3d293b85c33822159188b9e75b7597241e2c821e9ded7456601' ;; 		x86) natsArch='386'; sha256='637363cf3ca923c8762ecd083cf83c15cad505ed011ddbbaea857d982a1dadcf' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 07 Feb 2023 01:52:32 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 07 Feb 2023 01:52:32 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 07 Feb 2023 01:52:32 GMT
EXPOSE 4222 6222 8222
# Tue, 07 Feb 2023 01:52:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 07 Feb 2023 01:52:32 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:0269c10e600f3a375f36ddabdbd264ce9503a455f0d0969ce8a00f24eaecc032`  
		Last Modified: Mon, 09 Jan 2023 17:05:45 GMT  
		Size: 3.1 MB (3107243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12f12cb76c0f1aaea4b961abed480010a0742a12af14e5a7529fdcfe4ea1596f`  
		Last Modified: Tue, 07 Feb 2023 01:53:39 GMT  
		Size: 5.0 MB (4983903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcefd563896d4e37ea519c76d11d6f56e2cef47a3e47128072ac72293a6ded78`  
		Last Modified: Tue, 07 Feb 2023 01:53:38 GMT  
		Size: 560.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d426ece1d3a7e9fe54a8109d35cb1b0b91fe9823fa677ed49cea88878081269`  
		Last Modified: Tue, 07 Feb 2023 01:53:38 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:296856ae5e1bddb3fe6aebc65ac14b9d7ff5603959982d746d40db9e076eb62f
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.8 MB (7844570 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90e12165abca9e05e0f5ed3ff69b5461a01997b551fef47f8d6c6e910533341b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 09 Jan 2023 17:06:27 GMT
ADD file:4696f25d0f019b27457c55b3b128b70bf153f38e3e4eb5bdfc21058543313e94 in / 
# Mon, 09 Jan 2023 17:06:27 GMT
CMD ["/bin/sh"]
# Tue, 07 Feb 2023 02:00:38 GMT
ENV NATS_SERVER=2.9.14
# Tue, 07 Feb 2023 02:00:41 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='6032bc7b2621256e2d9f62f2a987eef490f071bde04dca09786d0270130f9cfd' ;; 		armhf) natsArch='arm6'; sha256='afbee67b87868dc29cf6c382f87813de264572472ac7513a66db6e99fd2a24ac' ;; 		armv7) natsArch='arm7'; sha256='e7e5c019e6cc3d6ef72da80defd5a4f95690b8d108ebb2cfd74fc9c47ac00706' ;; 		x86_64) natsArch='amd64'; sha256='18ac6d0a3956a3d293b85c33822159188b9e75b7597241e2c821e9ded7456601' ;; 		x86) natsArch='386'; sha256='637363cf3ca923c8762ecd083cf83c15cad505ed011ddbbaea857d982a1dadcf' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 07 Feb 2023 02:00:41 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 07 Feb 2023 02:00:41 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 07 Feb 2023 02:00:41 GMT
EXPOSE 4222 6222 8222
# Tue, 07 Feb 2023 02:00:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 07 Feb 2023 02:00:41 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:c527615e4ffa2d5b9b777fd469b3b5ba7c1b1e9201c065be2c43569de48a3754`  
		Last Modified: Mon, 09 Jan 2023 17:07:17 GMT  
		Size: 2.9 MB (2865208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28862903dec656beb20cc75d923845dc13689200c1e107e37e28f6e46d8a59b8`  
		Last Modified: Tue, 07 Feb 2023 02:01:53 GMT  
		Size: 5.0 MB (4978388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:937488760d17e32d344f2dd241d52b39400c167c419770a9eaafe9d170a14940`  
		Last Modified: Tue, 07 Feb 2023 02:01:52 GMT  
		Size: 560.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90c32128f2b508d07fc45ca73314749d71f9ba9d40869ce3bb81340feb4708a5`  
		Last Modified: Tue, 07 Feb 2023 02:01:52 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:df31ff3432342b1ede316ebcf7b4e73750286be0d7dabdff093432bf8a4ca8d5
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.1 MB (8065142 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e99541fd7b98de2eee799f260881ced37fb28d95d1b53eac7b31cd80dacba1c8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 09 Jan 2023 17:04:48 GMT
ADD file:3080f19f39259a4b77cc53975de0184c78d4335ceb9ffb77a2838d0539ad6f85 in / 
# Mon, 09 Jan 2023 17:04:49 GMT
CMD ["/bin/sh"]
# Tue, 07 Feb 2023 01:51:39 GMT
ENV NATS_SERVER=2.9.14
# Tue, 07 Feb 2023 01:51:42 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='6032bc7b2621256e2d9f62f2a987eef490f071bde04dca09786d0270130f9cfd' ;; 		armhf) natsArch='arm6'; sha256='afbee67b87868dc29cf6c382f87813de264572472ac7513a66db6e99fd2a24ac' ;; 		armv7) natsArch='arm7'; sha256='e7e5c019e6cc3d6ef72da80defd5a4f95690b8d108ebb2cfd74fc9c47ac00706' ;; 		x86_64) natsArch='amd64'; sha256='18ac6d0a3956a3d293b85c33822159188b9e75b7597241e2c821e9ded7456601' ;; 		x86) natsArch='386'; sha256='637363cf3ca923c8762ecd083cf83c15cad505ed011ddbbaea857d982a1dadcf' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 07 Feb 2023 01:51:42 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 07 Feb 2023 01:51:42 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 07 Feb 2023 01:51:42 GMT
EXPOSE 4222 6222 8222
# Tue, 07 Feb 2023 01:51:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 07 Feb 2023 01:51:42 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:a9eaa45ef418e883481a13c7d84fa9904f2ec56789c52a87ba5a9e6483f2b74f`  
		Last Modified: Mon, 09 Jan 2023 17:05:12 GMT  
		Size: 3.3 MB (3259241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed8a4006f1e7c6891cb29af60ba2447250fe63508a68ff60749aacb11c4df66c`  
		Last Modified: Tue, 07 Feb 2023 01:52:41 GMT  
		Size: 4.8 MB (4804903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99c0cd0fbcf84e908f6acb62f30f2c7ad11d4e7a09b697c1978bc272ece880e0`  
		Last Modified: Tue, 07 Feb 2023 01:52:40 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1a1c2bbc32bebff9300f6366e508a8bf0731b9f69074b6defb83f4af3a1411e`  
		Last Modified: Tue, 07 Feb 2023 01:52:40 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:alpine3.17`

```console
$ docker pull nats@sha256:23353a80fc1fecc883623f6b72759544f596be792aed1db01257ac900ca8d47f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:alpine3.17` - linux; amd64

```console
$ docker pull nats@sha256:2a0dd7504f75410d3b3198dbe094b70521260161f86ce9ec6a90b87548e5a22e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.6 MB (8591202 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9082af6bf2d6856d36cfa41bfd118221042916ab5cdf1ea5e886e9b9040cb97`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 09 Jan 2023 17:05:20 GMT
ADD file:e4d600fc4c9c293efe360be7b30ee96579925d1b4634c94332e2ec73f7d8eca1 in / 
# Mon, 09 Jan 2023 17:05:20 GMT
CMD ["/bin/sh"]
# Tue, 07 Feb 2023 02:43:45 GMT
ENV NATS_SERVER=2.9.14
# Tue, 07 Feb 2023 02:43:48 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='6032bc7b2621256e2d9f62f2a987eef490f071bde04dca09786d0270130f9cfd' ;; 		armhf) natsArch='arm6'; sha256='afbee67b87868dc29cf6c382f87813de264572472ac7513a66db6e99fd2a24ac' ;; 		armv7) natsArch='arm7'; sha256='e7e5c019e6cc3d6ef72da80defd5a4f95690b8d108ebb2cfd74fc9c47ac00706' ;; 		x86_64) natsArch='amd64'; sha256='18ac6d0a3956a3d293b85c33822159188b9e75b7597241e2c821e9ded7456601' ;; 		x86) natsArch='386'; sha256='637363cf3ca923c8762ecd083cf83c15cad505ed011ddbbaea857d982a1dadcf' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 07 Feb 2023 02:43:48 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 07 Feb 2023 02:43:48 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 07 Feb 2023 02:43:48 GMT
EXPOSE 4222 6222 8222
# Tue, 07 Feb 2023 02:43:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 07 Feb 2023 02:43:49 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:8921db27df2831fa6eaa85321205a2470c669b855f3ec95d5a3c2b46de0442c9`  
		Last Modified: Mon, 09 Jan 2023 17:05:45 GMT  
		Size: 3.4 MB (3370628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46ba763279c380b62642251deb522cb55e40fe260ab682de35f8f996055711b0`  
		Last Modified: Tue, 07 Feb 2023 02:44:24 GMT  
		Size: 5.2 MB (5219576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bd0bb18636d36c245afe73516ea39a6f261f808f4983639b201ddccacd55b9f`  
		Last Modified: Tue, 07 Feb 2023 02:44:23 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5caf6e5944e57b92eb19acf938c4c61f7b58c8d4504f368ef63e21fafcfcf56`  
		Last Modified: Tue, 07 Feb 2023 02:44:23 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.17` - linux; arm variant v6

```console
$ docker pull nats@sha256:d12deb5cddef79e53674a91f6a89b5106ed6c362b41c3a4db5ae2a839a149e85
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.1 MB (8092120 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:392d9e6c7555074305ae94233b635d10c0a78887283578e341bcb9dc14be0fd6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 09 Jan 2023 17:04:54 GMT
ADD file:b15fd8e9f996815394e25f20c8459bfb4c2a8c4074592d6f4c75f4fe79ce537e in / 
# Mon, 09 Jan 2023 17:04:55 GMT
CMD ["/bin/sh"]
# Tue, 07 Feb 2023 01:52:29 GMT
ENV NATS_SERVER=2.9.14
# Tue, 07 Feb 2023 01:52:32 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='6032bc7b2621256e2d9f62f2a987eef490f071bde04dca09786d0270130f9cfd' ;; 		armhf) natsArch='arm6'; sha256='afbee67b87868dc29cf6c382f87813de264572472ac7513a66db6e99fd2a24ac' ;; 		armv7) natsArch='arm7'; sha256='e7e5c019e6cc3d6ef72da80defd5a4f95690b8d108ebb2cfd74fc9c47ac00706' ;; 		x86_64) natsArch='amd64'; sha256='18ac6d0a3956a3d293b85c33822159188b9e75b7597241e2c821e9ded7456601' ;; 		x86) natsArch='386'; sha256='637363cf3ca923c8762ecd083cf83c15cad505ed011ddbbaea857d982a1dadcf' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 07 Feb 2023 01:52:32 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 07 Feb 2023 01:52:32 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 07 Feb 2023 01:52:32 GMT
EXPOSE 4222 6222 8222
# Tue, 07 Feb 2023 01:52:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 07 Feb 2023 01:52:32 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:0269c10e600f3a375f36ddabdbd264ce9503a455f0d0969ce8a00f24eaecc032`  
		Last Modified: Mon, 09 Jan 2023 17:05:45 GMT  
		Size: 3.1 MB (3107243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12f12cb76c0f1aaea4b961abed480010a0742a12af14e5a7529fdcfe4ea1596f`  
		Last Modified: Tue, 07 Feb 2023 01:53:39 GMT  
		Size: 5.0 MB (4983903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcefd563896d4e37ea519c76d11d6f56e2cef47a3e47128072ac72293a6ded78`  
		Last Modified: Tue, 07 Feb 2023 01:53:38 GMT  
		Size: 560.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d426ece1d3a7e9fe54a8109d35cb1b0b91fe9823fa677ed49cea88878081269`  
		Last Modified: Tue, 07 Feb 2023 01:53:38 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.17` - linux; arm variant v7

```console
$ docker pull nats@sha256:296856ae5e1bddb3fe6aebc65ac14b9d7ff5603959982d746d40db9e076eb62f
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.8 MB (7844570 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90e12165abca9e05e0f5ed3ff69b5461a01997b551fef47f8d6c6e910533341b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 09 Jan 2023 17:06:27 GMT
ADD file:4696f25d0f019b27457c55b3b128b70bf153f38e3e4eb5bdfc21058543313e94 in / 
# Mon, 09 Jan 2023 17:06:27 GMT
CMD ["/bin/sh"]
# Tue, 07 Feb 2023 02:00:38 GMT
ENV NATS_SERVER=2.9.14
# Tue, 07 Feb 2023 02:00:41 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='6032bc7b2621256e2d9f62f2a987eef490f071bde04dca09786d0270130f9cfd' ;; 		armhf) natsArch='arm6'; sha256='afbee67b87868dc29cf6c382f87813de264572472ac7513a66db6e99fd2a24ac' ;; 		armv7) natsArch='arm7'; sha256='e7e5c019e6cc3d6ef72da80defd5a4f95690b8d108ebb2cfd74fc9c47ac00706' ;; 		x86_64) natsArch='amd64'; sha256='18ac6d0a3956a3d293b85c33822159188b9e75b7597241e2c821e9ded7456601' ;; 		x86) natsArch='386'; sha256='637363cf3ca923c8762ecd083cf83c15cad505ed011ddbbaea857d982a1dadcf' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 07 Feb 2023 02:00:41 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 07 Feb 2023 02:00:41 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 07 Feb 2023 02:00:41 GMT
EXPOSE 4222 6222 8222
# Tue, 07 Feb 2023 02:00:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 07 Feb 2023 02:00:41 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:c527615e4ffa2d5b9b777fd469b3b5ba7c1b1e9201c065be2c43569de48a3754`  
		Last Modified: Mon, 09 Jan 2023 17:07:17 GMT  
		Size: 2.9 MB (2865208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28862903dec656beb20cc75d923845dc13689200c1e107e37e28f6e46d8a59b8`  
		Last Modified: Tue, 07 Feb 2023 02:01:53 GMT  
		Size: 5.0 MB (4978388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:937488760d17e32d344f2dd241d52b39400c167c419770a9eaafe9d170a14940`  
		Last Modified: Tue, 07 Feb 2023 02:01:52 GMT  
		Size: 560.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90c32128f2b508d07fc45ca73314749d71f9ba9d40869ce3bb81340feb4708a5`  
		Last Modified: Tue, 07 Feb 2023 02:01:52 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.17` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:df31ff3432342b1ede316ebcf7b4e73750286be0d7dabdff093432bf8a4ca8d5
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.1 MB (8065142 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e99541fd7b98de2eee799f260881ced37fb28d95d1b53eac7b31cd80dacba1c8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 09 Jan 2023 17:04:48 GMT
ADD file:3080f19f39259a4b77cc53975de0184c78d4335ceb9ffb77a2838d0539ad6f85 in / 
# Mon, 09 Jan 2023 17:04:49 GMT
CMD ["/bin/sh"]
# Tue, 07 Feb 2023 01:51:39 GMT
ENV NATS_SERVER=2.9.14
# Tue, 07 Feb 2023 01:51:42 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='6032bc7b2621256e2d9f62f2a987eef490f071bde04dca09786d0270130f9cfd' ;; 		armhf) natsArch='arm6'; sha256='afbee67b87868dc29cf6c382f87813de264572472ac7513a66db6e99fd2a24ac' ;; 		armv7) natsArch='arm7'; sha256='e7e5c019e6cc3d6ef72da80defd5a4f95690b8d108ebb2cfd74fc9c47ac00706' ;; 		x86_64) natsArch='amd64'; sha256='18ac6d0a3956a3d293b85c33822159188b9e75b7597241e2c821e9ded7456601' ;; 		x86) natsArch='386'; sha256='637363cf3ca923c8762ecd083cf83c15cad505ed011ddbbaea857d982a1dadcf' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 07 Feb 2023 01:51:42 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 07 Feb 2023 01:51:42 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 07 Feb 2023 01:51:42 GMT
EXPOSE 4222 6222 8222
# Tue, 07 Feb 2023 01:51:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 07 Feb 2023 01:51:42 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:a9eaa45ef418e883481a13c7d84fa9904f2ec56789c52a87ba5a9e6483f2b74f`  
		Last Modified: Mon, 09 Jan 2023 17:05:12 GMT  
		Size: 3.3 MB (3259241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed8a4006f1e7c6891cb29af60ba2447250fe63508a68ff60749aacb11c4df66c`  
		Last Modified: Tue, 07 Feb 2023 01:52:41 GMT  
		Size: 4.8 MB (4804903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99c0cd0fbcf84e908f6acb62f30f2c7ad11d4e7a09b697c1978bc272ece880e0`  
		Last Modified: Tue, 07 Feb 2023 01:52:40 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1a1c2bbc32bebff9300f6366e508a8bf0731b9f69074b6defb83f4af3a1411e`  
		Last Modified: Tue, 07 Feb 2023 01:52:40 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:latest`

```console
$ docker pull nats@sha256:f80a2e0337ac068122897636f9f6d686a397ea56f593e0ce0a603cdf41e6e027
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.3887; amd64

### `nats:latest` - linux; amd64

```console
$ docker pull nats@sha256:e6916a74a9af2d54502bfa1459a3e0702c00faa14327b3f3b812262e8ada0966
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4933617 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dbb0263a71ad823c35b7c360c016e57737a4367ef1c4909a859acb0ddb4ab19a`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 07 Feb 2023 02:43:58 GMT
COPY file:ac560677dbfad917be71a9245045f536b2801212b542bc63c664d6d11156f4dc in /nats-server 
# Tue, 07 Feb 2023 02:43:58 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 07 Feb 2023 02:43:58 GMT
EXPOSE 4222 6222 8222
# Tue, 07 Feb 2023 02:43:58 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 07 Feb 2023 02:43:59 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 07 Feb 2023 02:43:59 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:5668bc7ee19e1c51e1510bfeee7245e2b2cc66a8b8f8b0f988f4b3bca8729cec`  
		Last Modified: Tue, 07 Feb 2023 02:44:45 GMT  
		Size: 4.9 MB (4933108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93d5b4d77a0e7f6c3fed0f1ae97dbe1b22a3ed4e6af873e7782a0b1d2b992779`  
		Last Modified: Tue, 07 Feb 2023 02:44:44 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm variant v6

```console
$ docker pull nats@sha256:b141eec319986960b56193a2de1a779138beb96cb9945ebc12dbbe199ca96382
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4696311 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89f9b13a403b08d651892f330e0f3dd788a5fb00fd1f6338e79860d306d4504d`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 07 Feb 2023 01:52:41 GMT
COPY file:4eee0f78d63bff3b20fac11aaeb64833cd520dac95605f8f9015e670e58a5ef7 in /nats-server 
# Tue, 07 Feb 2023 01:52:41 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 07 Feb 2023 01:52:41 GMT
EXPOSE 4222 6222 8222
# Tue, 07 Feb 2023 01:52:41 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 07 Feb 2023 01:52:41 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 07 Feb 2023 01:52:41 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6a1ef747dccf7d40d061dc4c857fff9b056d8693e427a2f3adaebc1e22066869`  
		Last Modified: Tue, 07 Feb 2023 01:54:10 GMT  
		Size: 4.7 MB (4695803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc7ba083439d0caacde0ad211a483925f47f6ec3916cf261abe491ac5a630aaf`  
		Last Modified: Tue, 07 Feb 2023 01:54:10 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm variant v7

```console
$ docker pull nats@sha256:ccb41e1e35bee87bcd6a70e43fd88e284140c67701fb8f639781a7b0b7201eb6
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4691076 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a4d042e0f28cb5cfa1b6a77c7eb4e06d62ffbfd2c681f2ca2f1aa747dc538cf`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 07 Feb 2023 02:00:54 GMT
COPY file:5f0ce15e9664bd3755e850351446cf7719b19193e891220c68a9776456e2700a in /nats-server 
# Tue, 07 Feb 2023 02:00:54 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 07 Feb 2023 02:00:54 GMT
EXPOSE 4222 6222 8222
# Tue, 07 Feb 2023 02:00:54 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 07 Feb 2023 02:00:54 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 07 Feb 2023 02:00:54 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:858d33663bc30713d47f7de008a1659f090a1ab8df117e447c1623a289378d31`  
		Last Modified: Tue, 07 Feb 2023 02:02:24 GMT  
		Size: 4.7 MB (4690568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c4973a38193b2d039d297077dd1451a47493f724dd8283e465313c615bcbbb8`  
		Last Modified: Tue, 07 Feb 2023 02:02:23 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:1689ba4ea78e52511a025fdbe524cf1d62dc69c0c2bb68119fabb955e8513246
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4519578 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:96bb932300dca1eb555905232fe9caf2ee65c6b8285cc68e13cf30bb07bd94d3`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 07 Feb 2023 01:52:13 GMT
COPY file:cc453883d11f3e7a77a5f311e510cb07fee2fd66b31eb11f16a5f8023889f08d in /nats-server 
# Tue, 07 Feb 2023 01:52:13 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 07 Feb 2023 01:52:13 GMT
EXPOSE 4222 6222 8222
# Tue, 07 Feb 2023 01:52:13 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 07 Feb 2023 01:52:13 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 07 Feb 2023 01:52:13 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:cf0e5763ec64b26f959ef78ac3641929a51a1fda6989adfd65f04af6f8b3a53a`  
		Last Modified: Tue, 07 Feb 2023 01:53:02 GMT  
		Size: 4.5 MB (4519070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cb009df287c6f73705947a89031473f06a27171a64409e09c24fc061c1863d5`  
		Last Modified: Tue, 07 Feb 2023 01:53:01 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - windows version 10.0.17763.3887; amd64

```console
$ docker pull nats@sha256:e6a17bb97fb6a291a4bd98d30c3b9099dedbcf70d12fb062efebaabdb1213bbc
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.7 MB (111659596 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:45804cd0005e5185373d2c577a4257391cd004c68b4c440f4678cf10382b2db7`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 07 Jan 2023 05:17:01 GMT
RUN Apply image 10.0.17763.3887
# Thu, 12 Jan 2023 05:01:51 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Tue, 07 Feb 2023 02:18:03 GMT
RUN cmd /S /C #(nop) COPY file:a45a34d252c029bb58fb3b3e2b3592a2d7869806250714c7b6dc3fb0b305c7bd in C:\nats-server.exe 
# Tue, 07 Feb 2023 02:18:04 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Tue, 07 Feb 2023 02:18:05 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Tue, 07 Feb 2023 02:18:06 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 07 Feb 2023 02:18:06 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:e58f9ad3b15a2a4882ab0a845e8e619cc8c3c411ddbe8b50046c1618a95c1397`  
		Last Modified: Thu, 12 Jan 2023 02:40:44 GMT  
		Size: 106.7 MB (106666138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fe88f4c5f9972ffecb9a66b92e75ddfe48bf7d8d451ace7af3527653f67ff9e`  
		Last Modified: Thu, 12 Jan 2023 05:02:42 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6572a3c131299689497339cc59b098f3601ad482ac0828eeaba7e5f78dc21d76`  
		Last Modified: Tue, 07 Feb 2023 02:18:55 GMT  
		Size: 5.0 MB (4987024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d5a625d40bd2eadd9e49c606bd8fad79a2aa73ebcd3313c3de00a12b06738c7`  
		Last Modified: Tue, 07 Feb 2023 02:18:53 GMT  
		Size: 1.8 KB (1788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9650a5245dfd33f33fb4a5df832057f9d0b34cb3febe41b20095202eda9b58f`  
		Last Modified: Tue, 07 Feb 2023 02:18:53 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15ca02e3d157746bd7381b47df24d65195a307dadd09eba9a311c95481d51b4d`  
		Last Modified: Tue, 07 Feb 2023 02:18:53 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efd2be7007de85b1c3f78a02ae15fdfcf679c7378b8d53403ebe90f39cd16418`  
		Last Modified: Tue, 07 Feb 2023 02:18:53 GMT  
		Size: 1.2 KB (1181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:linux`

```console
$ docker pull nats@sha256:eb248ee016566129be55f099933db3c2daa1b235a9831eab265fb9b8324cd269
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:linux` - linux; amd64

```console
$ docker pull nats@sha256:e6916a74a9af2d54502bfa1459a3e0702c00faa14327b3f3b812262e8ada0966
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4933617 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dbb0263a71ad823c35b7c360c016e57737a4367ef1c4909a859acb0ddb4ab19a`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 07 Feb 2023 02:43:58 GMT
COPY file:ac560677dbfad917be71a9245045f536b2801212b542bc63c664d6d11156f4dc in /nats-server 
# Tue, 07 Feb 2023 02:43:58 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 07 Feb 2023 02:43:58 GMT
EXPOSE 4222 6222 8222
# Tue, 07 Feb 2023 02:43:58 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 07 Feb 2023 02:43:59 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 07 Feb 2023 02:43:59 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:5668bc7ee19e1c51e1510bfeee7245e2b2cc66a8b8f8b0f988f4b3bca8729cec`  
		Last Modified: Tue, 07 Feb 2023 02:44:45 GMT  
		Size: 4.9 MB (4933108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93d5b4d77a0e7f6c3fed0f1ae97dbe1b22a3ed4e6af873e7782a0b1d2b992779`  
		Last Modified: Tue, 07 Feb 2023 02:44:44 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:b141eec319986960b56193a2de1a779138beb96cb9945ebc12dbbe199ca96382
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4696311 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89f9b13a403b08d651892f330e0f3dd788a5fb00fd1f6338e79860d306d4504d`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 07 Feb 2023 01:52:41 GMT
COPY file:4eee0f78d63bff3b20fac11aaeb64833cd520dac95605f8f9015e670e58a5ef7 in /nats-server 
# Tue, 07 Feb 2023 01:52:41 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 07 Feb 2023 01:52:41 GMT
EXPOSE 4222 6222 8222
# Tue, 07 Feb 2023 01:52:41 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 07 Feb 2023 01:52:41 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 07 Feb 2023 01:52:41 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6a1ef747dccf7d40d061dc4c857fff9b056d8693e427a2f3adaebc1e22066869`  
		Last Modified: Tue, 07 Feb 2023 01:54:10 GMT  
		Size: 4.7 MB (4695803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc7ba083439d0caacde0ad211a483925f47f6ec3916cf261abe491ac5a630aaf`  
		Last Modified: Tue, 07 Feb 2023 01:54:10 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:ccb41e1e35bee87bcd6a70e43fd88e284140c67701fb8f639781a7b0b7201eb6
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4691076 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a4d042e0f28cb5cfa1b6a77c7eb4e06d62ffbfd2c681f2ca2f1aa747dc538cf`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 07 Feb 2023 02:00:54 GMT
COPY file:5f0ce15e9664bd3755e850351446cf7719b19193e891220c68a9776456e2700a in /nats-server 
# Tue, 07 Feb 2023 02:00:54 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 07 Feb 2023 02:00:54 GMT
EXPOSE 4222 6222 8222
# Tue, 07 Feb 2023 02:00:54 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 07 Feb 2023 02:00:54 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 07 Feb 2023 02:00:54 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:858d33663bc30713d47f7de008a1659f090a1ab8df117e447c1623a289378d31`  
		Last Modified: Tue, 07 Feb 2023 02:02:24 GMT  
		Size: 4.7 MB (4690568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c4973a38193b2d039d297077dd1451a47493f724dd8283e465313c615bcbbb8`  
		Last Modified: Tue, 07 Feb 2023 02:02:23 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:1689ba4ea78e52511a025fdbe524cf1d62dc69c0c2bb68119fabb955e8513246
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4519578 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:96bb932300dca1eb555905232fe9caf2ee65c6b8285cc68e13cf30bb07bd94d3`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 07 Feb 2023 01:52:13 GMT
COPY file:cc453883d11f3e7a77a5f311e510cb07fee2fd66b31eb11f16a5f8023889f08d in /nats-server 
# Tue, 07 Feb 2023 01:52:13 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 07 Feb 2023 01:52:13 GMT
EXPOSE 4222 6222 8222
# Tue, 07 Feb 2023 01:52:13 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 07 Feb 2023 01:52:13 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 07 Feb 2023 01:52:13 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:cf0e5763ec64b26f959ef78ac3641929a51a1fda6989adfd65f04af6f8b3a53a`  
		Last Modified: Tue, 07 Feb 2023 01:53:02 GMT  
		Size: 4.5 MB (4519070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cb009df287c6f73705947a89031473f06a27171a64409e09c24fc061c1863d5`  
		Last Modified: Tue, 07 Feb 2023 01:53:01 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:nanoserver`

```console
$ docker pull nats@sha256:cf75db15a7a309da40d820366d4ca9bbf4f39bc06a401a060ccbc7f0618eea1f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3887; amd64

### `nats:nanoserver` - windows version 10.0.17763.3887; amd64

```console
$ docker pull nats@sha256:e6a17bb97fb6a291a4bd98d30c3b9099dedbcf70d12fb062efebaabdb1213bbc
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.7 MB (111659596 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:45804cd0005e5185373d2c577a4257391cd004c68b4c440f4678cf10382b2db7`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 07 Jan 2023 05:17:01 GMT
RUN Apply image 10.0.17763.3887
# Thu, 12 Jan 2023 05:01:51 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Tue, 07 Feb 2023 02:18:03 GMT
RUN cmd /S /C #(nop) COPY file:a45a34d252c029bb58fb3b3e2b3592a2d7869806250714c7b6dc3fb0b305c7bd in C:\nats-server.exe 
# Tue, 07 Feb 2023 02:18:04 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Tue, 07 Feb 2023 02:18:05 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Tue, 07 Feb 2023 02:18:06 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 07 Feb 2023 02:18:06 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:e58f9ad3b15a2a4882ab0a845e8e619cc8c3c411ddbe8b50046c1618a95c1397`  
		Last Modified: Thu, 12 Jan 2023 02:40:44 GMT  
		Size: 106.7 MB (106666138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fe88f4c5f9972ffecb9a66b92e75ddfe48bf7d8d451ace7af3527653f67ff9e`  
		Last Modified: Thu, 12 Jan 2023 05:02:42 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6572a3c131299689497339cc59b098f3601ad482ac0828eeaba7e5f78dc21d76`  
		Last Modified: Tue, 07 Feb 2023 02:18:55 GMT  
		Size: 5.0 MB (4987024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d5a625d40bd2eadd9e49c606bd8fad79a2aa73ebcd3313c3de00a12b06738c7`  
		Last Modified: Tue, 07 Feb 2023 02:18:53 GMT  
		Size: 1.8 KB (1788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9650a5245dfd33f33fb4a5df832057f9d0b34cb3febe41b20095202eda9b58f`  
		Last Modified: Tue, 07 Feb 2023 02:18:53 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15ca02e3d157746bd7381b47df24d65195a307dadd09eba9a311c95481d51b4d`  
		Last Modified: Tue, 07 Feb 2023 02:18:53 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efd2be7007de85b1c3f78a02ae15fdfcf679c7378b8d53403ebe90f39cd16418`  
		Last Modified: Tue, 07 Feb 2023 02:18:53 GMT  
		Size: 1.2 KB (1181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:nanoserver-1809`

```console
$ docker pull nats@sha256:cf75db15a7a309da40d820366d4ca9bbf4f39bc06a401a060ccbc7f0618eea1f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3887; amd64

### `nats:nanoserver-1809` - windows version 10.0.17763.3887; amd64

```console
$ docker pull nats@sha256:e6a17bb97fb6a291a4bd98d30c3b9099dedbcf70d12fb062efebaabdb1213bbc
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.7 MB (111659596 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:45804cd0005e5185373d2c577a4257391cd004c68b4c440f4678cf10382b2db7`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 07 Jan 2023 05:17:01 GMT
RUN Apply image 10.0.17763.3887
# Thu, 12 Jan 2023 05:01:51 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Tue, 07 Feb 2023 02:18:03 GMT
RUN cmd /S /C #(nop) COPY file:a45a34d252c029bb58fb3b3e2b3592a2d7869806250714c7b6dc3fb0b305c7bd in C:\nats-server.exe 
# Tue, 07 Feb 2023 02:18:04 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Tue, 07 Feb 2023 02:18:05 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Tue, 07 Feb 2023 02:18:06 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 07 Feb 2023 02:18:06 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:e58f9ad3b15a2a4882ab0a845e8e619cc8c3c411ddbe8b50046c1618a95c1397`  
		Last Modified: Thu, 12 Jan 2023 02:40:44 GMT  
		Size: 106.7 MB (106666138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fe88f4c5f9972ffecb9a66b92e75ddfe48bf7d8d451ace7af3527653f67ff9e`  
		Last Modified: Thu, 12 Jan 2023 05:02:42 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6572a3c131299689497339cc59b098f3601ad482ac0828eeaba7e5f78dc21d76`  
		Last Modified: Tue, 07 Feb 2023 02:18:55 GMT  
		Size: 5.0 MB (4987024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d5a625d40bd2eadd9e49c606bd8fad79a2aa73ebcd3313c3de00a12b06738c7`  
		Last Modified: Tue, 07 Feb 2023 02:18:53 GMT  
		Size: 1.8 KB (1788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9650a5245dfd33f33fb4a5df832057f9d0b34cb3febe41b20095202eda9b58f`  
		Last Modified: Tue, 07 Feb 2023 02:18:53 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15ca02e3d157746bd7381b47df24d65195a307dadd09eba9a311c95481d51b4d`  
		Last Modified: Tue, 07 Feb 2023 02:18:53 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efd2be7007de85b1c3f78a02ae15fdfcf679c7378b8d53403ebe90f39cd16418`  
		Last Modified: Tue, 07 Feb 2023 02:18:53 GMT  
		Size: 1.2 KB (1181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:scratch`

```console
$ docker pull nats@sha256:eb248ee016566129be55f099933db3c2daa1b235a9831eab265fb9b8324cd269
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:scratch` - linux; amd64

```console
$ docker pull nats@sha256:e6916a74a9af2d54502bfa1459a3e0702c00faa14327b3f3b812262e8ada0966
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4933617 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dbb0263a71ad823c35b7c360c016e57737a4367ef1c4909a859acb0ddb4ab19a`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 07 Feb 2023 02:43:58 GMT
COPY file:ac560677dbfad917be71a9245045f536b2801212b542bc63c664d6d11156f4dc in /nats-server 
# Tue, 07 Feb 2023 02:43:58 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 07 Feb 2023 02:43:58 GMT
EXPOSE 4222 6222 8222
# Tue, 07 Feb 2023 02:43:58 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 07 Feb 2023 02:43:59 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 07 Feb 2023 02:43:59 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:5668bc7ee19e1c51e1510bfeee7245e2b2cc66a8b8f8b0f988f4b3bca8729cec`  
		Last Modified: Tue, 07 Feb 2023 02:44:45 GMT  
		Size: 4.9 MB (4933108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93d5b4d77a0e7f6c3fed0f1ae97dbe1b22a3ed4e6af873e7782a0b1d2b992779`  
		Last Modified: Tue, 07 Feb 2023 02:44:44 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:b141eec319986960b56193a2de1a779138beb96cb9945ebc12dbbe199ca96382
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4696311 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89f9b13a403b08d651892f330e0f3dd788a5fb00fd1f6338e79860d306d4504d`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 07 Feb 2023 01:52:41 GMT
COPY file:4eee0f78d63bff3b20fac11aaeb64833cd520dac95605f8f9015e670e58a5ef7 in /nats-server 
# Tue, 07 Feb 2023 01:52:41 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 07 Feb 2023 01:52:41 GMT
EXPOSE 4222 6222 8222
# Tue, 07 Feb 2023 01:52:41 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 07 Feb 2023 01:52:41 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 07 Feb 2023 01:52:41 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6a1ef747dccf7d40d061dc4c857fff9b056d8693e427a2f3adaebc1e22066869`  
		Last Modified: Tue, 07 Feb 2023 01:54:10 GMT  
		Size: 4.7 MB (4695803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc7ba083439d0caacde0ad211a483925f47f6ec3916cf261abe491ac5a630aaf`  
		Last Modified: Tue, 07 Feb 2023 01:54:10 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:ccb41e1e35bee87bcd6a70e43fd88e284140c67701fb8f639781a7b0b7201eb6
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4691076 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a4d042e0f28cb5cfa1b6a77c7eb4e06d62ffbfd2c681f2ca2f1aa747dc538cf`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 07 Feb 2023 02:00:54 GMT
COPY file:5f0ce15e9664bd3755e850351446cf7719b19193e891220c68a9776456e2700a in /nats-server 
# Tue, 07 Feb 2023 02:00:54 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 07 Feb 2023 02:00:54 GMT
EXPOSE 4222 6222 8222
# Tue, 07 Feb 2023 02:00:54 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 07 Feb 2023 02:00:54 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 07 Feb 2023 02:00:54 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:858d33663bc30713d47f7de008a1659f090a1ab8df117e447c1623a289378d31`  
		Last Modified: Tue, 07 Feb 2023 02:02:24 GMT  
		Size: 4.7 MB (4690568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c4973a38193b2d039d297077dd1451a47493f724dd8283e465313c615bcbbb8`  
		Last Modified: Tue, 07 Feb 2023 02:02:23 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:1689ba4ea78e52511a025fdbe524cf1d62dc69c0c2bb68119fabb955e8513246
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4519578 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:96bb932300dca1eb555905232fe9caf2ee65c6b8285cc68e13cf30bb07bd94d3`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 07 Feb 2023 01:52:13 GMT
COPY file:cc453883d11f3e7a77a5f311e510cb07fee2fd66b31eb11f16a5f8023889f08d in /nats-server 
# Tue, 07 Feb 2023 01:52:13 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 07 Feb 2023 01:52:13 GMT
EXPOSE 4222 6222 8222
# Tue, 07 Feb 2023 01:52:13 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 07 Feb 2023 01:52:13 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 07 Feb 2023 01:52:13 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:cf0e5763ec64b26f959ef78ac3641929a51a1fda6989adfd65f04af6f8b3a53a`  
		Last Modified: Tue, 07 Feb 2023 01:53:02 GMT  
		Size: 4.5 MB (4519070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cb009df287c6f73705947a89031473f06a27171a64409e09c24fc061c1863d5`  
		Last Modified: Tue, 07 Feb 2023 01:53:01 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:windowsservercore`

```console
$ docker pull nats@sha256:2f83133d0acce8f6e25329cfa1448835465a15f6f6080d3dea01f044b04cdb6f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3887; amd64

### `nats:windowsservercore` - windows version 10.0.17763.3887; amd64

```console
$ docker pull nats@sha256:e0c232bf30691b8afe55af261d4a01f8639efc585516e1eb09940bb851eb8833
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.7 GB (1713683278 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0382d02f9daa152fcd1c45024249998399b9334f6099f446e931d98f771aef58`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Thu, 12 Jan 2023 04:04:12 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Thu, 12 Jan 2023 04:59:53 GMT
ENV NATS_DOCKERIZED=1
# Tue, 07 Feb 2023 02:16:03 GMT
ENV NATS_SERVER=2.9.14
# Tue, 07 Feb 2023 02:16:05 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.9.14/nats-server-v2.9.14-windows-amd64.zip
# Tue, 07 Feb 2023 02:16:05 GMT
ENV NATS_SERVER_SHASUM=b47ca5d88b1a74934145aba3afd6a3b0eee0e543638000cee82b468b8dfbcb3c
# Tue, 07 Feb 2023 02:16:36 GMT
RUN Set-PSDebug -Trace 2
# Tue, 07 Feb 2023 02:17:45 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Tue, 07 Feb 2023 02:17:46 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Tue, 07 Feb 2023 02:17:47 GMT
EXPOSE 4222 6222 8222
# Tue, 07 Feb 2023 02:17:47 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 07 Feb 2023 02:17:48 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f99eee4cf5f23d13a762e719b10916801f19f9df4bd7ff9b4c5cf57133b3dc04`  
		Last Modified: Thu, 12 Jan 2023 04:39:02 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fda92ec365568291ec0ef873b055a8b13d2c46244c129bc4cdf81f0e43e1ec8c`  
		Last Modified: Thu, 12 Jan 2023 05:02:27 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddda27c0ef4ad351d1295efe578196d2003caa62b54a6dee81e4765decf322c9`  
		Last Modified: Tue, 07 Feb 2023 02:18:39 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6375d8bcf5bfd121917c9066a7fc47758ed54929693e46c124d8b34cd701c29`  
		Last Modified: Tue, 07 Feb 2023 02:18:39 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ed0fe5c6e734a1bb638b4e36f3d8cea012a04915c4408581da282286dc6b9ec`  
		Last Modified: Tue, 07 Feb 2023 02:18:39 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83d9c44c9456dd05617593616f2a49404163b5d832e2eb53dda03b1e8b59aec7`  
		Last Modified: Tue, 07 Feb 2023 02:18:39 GMT  
		Size: 382.7 KB (382704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7bcd7fc2e88df50e426c8b75e75d6578f5f036d2f228ed98719dea90187c5db`  
		Last Modified: Tue, 07 Feb 2023 02:18:39 GMT  
		Size: 5.3 MB (5343352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49c9175c6ac4001ff4bc634962943cd35c9bbb984cf1b92653a90a892d15a1bd`  
		Last Modified: Tue, 07 Feb 2023 02:18:37 GMT  
		Size: 2.0 KB (1963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5172837be3b8edccf67687c538bbdc1bfb717ff392a6e6f146469c063e54c0b5`  
		Last Modified: Tue, 07 Feb 2023 02:18:37 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:791a5a7bac5f0d37232a1b86033fb3be57356d147b1c8293d8128faf6ac70c63`  
		Last Modified: Tue, 07 Feb 2023 02:18:37 GMT  
		Size: 1.4 KB (1442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2de08797cefe4c85eb6dd724a5a14d0c72406c8fce9d081ccf86b41210c6171f`  
		Last Modified: Tue, 07 Feb 2023 02:18:37 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:windowsservercore-1809`

```console
$ docker pull nats@sha256:2f83133d0acce8f6e25329cfa1448835465a15f6f6080d3dea01f044b04cdb6f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3887; amd64

### `nats:windowsservercore-1809` - windows version 10.0.17763.3887; amd64

```console
$ docker pull nats@sha256:e0c232bf30691b8afe55af261d4a01f8639efc585516e1eb09940bb851eb8833
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.7 GB (1713683278 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0382d02f9daa152fcd1c45024249998399b9334f6099f446e931d98f771aef58`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Thu, 12 Jan 2023 04:04:12 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Thu, 12 Jan 2023 04:59:53 GMT
ENV NATS_DOCKERIZED=1
# Tue, 07 Feb 2023 02:16:03 GMT
ENV NATS_SERVER=2.9.14
# Tue, 07 Feb 2023 02:16:05 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.9.14/nats-server-v2.9.14-windows-amd64.zip
# Tue, 07 Feb 2023 02:16:05 GMT
ENV NATS_SERVER_SHASUM=b47ca5d88b1a74934145aba3afd6a3b0eee0e543638000cee82b468b8dfbcb3c
# Tue, 07 Feb 2023 02:16:36 GMT
RUN Set-PSDebug -Trace 2
# Tue, 07 Feb 2023 02:17:45 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Tue, 07 Feb 2023 02:17:46 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Tue, 07 Feb 2023 02:17:47 GMT
EXPOSE 4222 6222 8222
# Tue, 07 Feb 2023 02:17:47 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 07 Feb 2023 02:17:48 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f99eee4cf5f23d13a762e719b10916801f19f9df4bd7ff9b4c5cf57133b3dc04`  
		Last Modified: Thu, 12 Jan 2023 04:39:02 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fda92ec365568291ec0ef873b055a8b13d2c46244c129bc4cdf81f0e43e1ec8c`  
		Last Modified: Thu, 12 Jan 2023 05:02:27 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddda27c0ef4ad351d1295efe578196d2003caa62b54a6dee81e4765decf322c9`  
		Last Modified: Tue, 07 Feb 2023 02:18:39 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6375d8bcf5bfd121917c9066a7fc47758ed54929693e46c124d8b34cd701c29`  
		Last Modified: Tue, 07 Feb 2023 02:18:39 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ed0fe5c6e734a1bb638b4e36f3d8cea012a04915c4408581da282286dc6b9ec`  
		Last Modified: Tue, 07 Feb 2023 02:18:39 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83d9c44c9456dd05617593616f2a49404163b5d832e2eb53dda03b1e8b59aec7`  
		Last Modified: Tue, 07 Feb 2023 02:18:39 GMT  
		Size: 382.7 KB (382704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7bcd7fc2e88df50e426c8b75e75d6578f5f036d2f228ed98719dea90187c5db`  
		Last Modified: Tue, 07 Feb 2023 02:18:39 GMT  
		Size: 5.3 MB (5343352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49c9175c6ac4001ff4bc634962943cd35c9bbb984cf1b92653a90a892d15a1bd`  
		Last Modified: Tue, 07 Feb 2023 02:18:37 GMT  
		Size: 2.0 KB (1963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5172837be3b8edccf67687c538bbdc1bfb717ff392a6e6f146469c063e54c0b5`  
		Last Modified: Tue, 07 Feb 2023 02:18:37 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:791a5a7bac5f0d37232a1b86033fb3be57356d147b1c8293d8128faf6ac70c63`  
		Last Modified: Tue, 07 Feb 2023 02:18:37 GMT  
		Size: 1.4 KB (1442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2de08797cefe4c85eb6dd724a5a14d0c72406c8fce9d081ccf86b41210c6171f`  
		Last Modified: Tue, 07 Feb 2023 02:18:37 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
