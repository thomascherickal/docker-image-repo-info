<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `nats`

-	[`nats:2`](#nats2)
-	[`nats:2-alpine`](#nats2-alpine)
-	[`nats:2-alpine3.16`](#nats2-alpine316)
-	[`nats:2-linux`](#nats2-linux)
-	[`nats:2-nanoserver`](#nats2-nanoserver)
-	[`nats:2-nanoserver-1809`](#nats2-nanoserver-1809)
-	[`nats:2-scratch`](#nats2-scratch)
-	[`nats:2-windowsservercore`](#nats2-windowsservercore)
-	[`nats:2-windowsservercore-1809`](#nats2-windowsservercore-1809)
-	[`nats:2.9`](#nats29)
-	[`nats:2.9-alpine`](#nats29-alpine)
-	[`nats:2.9-alpine3.16`](#nats29-alpine316)
-	[`nats:2.9-linux`](#nats29-linux)
-	[`nats:2.9-nanoserver`](#nats29-nanoserver)
-	[`nats:2.9-nanoserver-1809`](#nats29-nanoserver-1809)
-	[`nats:2.9-scratch`](#nats29-scratch)
-	[`nats:2.9-windowsservercore`](#nats29-windowsservercore)
-	[`nats:2.9-windowsservercore-1809`](#nats29-windowsservercore-1809)
-	[`nats:2.9.2`](#nats292)
-	[`nats:2.9.2-alpine`](#nats292-alpine)
-	[`nats:2.9.2-alpine3.16`](#nats292-alpine316)
-	[`nats:2.9.2-linux`](#nats292-linux)
-	[`nats:2.9.2-nanoserver`](#nats292-nanoserver)
-	[`nats:2.9.2-nanoserver-1809`](#nats292-nanoserver-1809)
-	[`nats:2.9.2-scratch`](#nats292-scratch)
-	[`nats:2.9.2-windowsservercore`](#nats292-windowsservercore)
-	[`nats:2.9.2-windowsservercore-1809`](#nats292-windowsservercore-1809)
-	[`nats:alpine`](#natsalpine)
-	[`nats:alpine3.16`](#natsalpine316)
-	[`nats:latest`](#natslatest)
-	[`nats:linux`](#natslinux)
-	[`nats:nanoserver`](#natsnanoserver)
-	[`nats:nanoserver-1809`](#natsnanoserver-1809)
-	[`nats:scratch`](#natsscratch)
-	[`nats:windowsservercore`](#natswindowsservercore)
-	[`nats:windowsservercore-1809`](#natswindowsservercore-1809)

## `nats:2`

```console
$ docker pull nats@sha256:2a333e9f7d50ba4dd450e435b65a5b038af6988ab4c19c858cf85c6733667c28
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.3406; amd64

### `nats:2` - linux; amd64

```console
$ docker pull nats@sha256:73a511425369d8e883fc5784023028b7ed02c252e6db030e776b2e6a76bb90ca
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4907513 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf3ba31eb02c938f2ab28c2b60358ef903503ce4a2fb5e2df6f4714d04e74619`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 30 Sep 2022 00:25:01 GMT
COPY file:ef7d265008705c7f8da964d29a2883d21303aab4d4520c3327ca6ce57348e137 in /nats-server 
# Fri, 30 Sep 2022 00:25:01 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 30 Sep 2022 00:25:01 GMT
EXPOSE 4222 6222 8222
# Fri, 30 Sep 2022 00:25:01 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 30 Sep 2022 00:25:01 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 30 Sep 2022 00:25:01 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:325d5a714be1f0303eebb8d34c9b23e1b15c5e7e46eb29d0f90511112fb86894`  
		Last Modified: Fri, 30 Sep 2022 00:25:50 GMT  
		Size: 4.9 MB (4907005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06b03a363308e84c4fc60d5ac2d5b9374e811456edecdb1e302e59198bfb1ca4`  
		Last Modified: Fri, 30 Sep 2022 00:25:49 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - linux; arm variant v6

```console
$ docker pull nats@sha256:22be654fd606d7db5e28383ce35794c881f25b77908c6f981c2442b117d7df19
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4671534 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1eeeee00c7520737eb3766018dde7f3dd63c971938d98ff49cca225f0e6c6990`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 30 Sep 2022 00:15:17 GMT
COPY file:2de52eed8721a4ef1e4c8adb2f046a7ffa8e689d614c704b329ef2bafc7dfe5c in /nats-server 
# Fri, 30 Sep 2022 00:15:17 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 30 Sep 2022 00:15:17 GMT
EXPOSE 4222 6222 8222
# Fri, 30 Sep 2022 00:15:18 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 30 Sep 2022 00:15:18 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 30 Sep 2022 00:15:18 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:948e55d9b8c745ce1f9007c64a6da65d66c0d554fa7e5808a04081a1d0754a6c`  
		Last Modified: Fri, 30 Sep 2022 00:16:49 GMT  
		Size: 4.7 MB (4671025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14bdee3fcf17688810034aff56b746397e799579ff11654f2a2ec59274a9e161`  
		Last Modified: Fri, 30 Sep 2022 00:16:48 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - linux; arm variant v7

```console
$ docker pull nats@sha256:dce0b0ef268b27c6417ee879c4f500273d8eabe0f3347ed2ac19b28a166085e2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4661683 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93f043be0120df37adc5618c50a4eb09f405d9a23f0794314f36c76be8bda597`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 30 Sep 2022 12:21:44 GMT
COPY file:e57d6f6c709cd7f891a48782c812655546ed7ed7194710fb4ff95d3225a8cb24 in /nats-server 
# Fri, 30 Sep 2022 12:21:44 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 30 Sep 2022 12:21:44 GMT
EXPOSE 4222 6222 8222
# Fri, 30 Sep 2022 12:21:44 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 30 Sep 2022 12:21:44 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 30 Sep 2022 12:21:44 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6709a2d5812e1f5aabc828977b23e9033fb28dd6d79bad682b986bfeaf468265`  
		Last Modified: Fri, 30 Sep 2022 12:23:13 GMT  
		Size: 4.7 MB (4661175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:913a6877bd39f71d19820c3493253d22c565656c7058ca6e5deb8e20280f8ad6`  
		Last Modified: Fri, 30 Sep 2022 12:23:12 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:6d0d5cfcf4b908ca419719473183dd4000ebe2e77e9fb1088f51f2195324d865
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4495540 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7069cf895c76381ff91ad174ed58ca07743ca741317f4a2c20ea3b1f1bae44ce`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 30 Sep 2022 01:50:11 GMT
COPY file:06300839e6ae56288247488999d2e96ee71c9bb64453bfa88faa4cbfc85a23e2 in /nats-server 
# Fri, 30 Sep 2022 01:50:12 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 30 Sep 2022 01:50:12 GMT
EXPOSE 4222 6222 8222
# Fri, 30 Sep 2022 01:50:13 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 30 Sep 2022 01:50:14 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 30 Sep 2022 01:50:15 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:71fcb6de35d4d1378bd805b642a59de493c8957d351b1f521d05492db21c54d6`  
		Last Modified: Fri, 30 Sep 2022 01:51:31 GMT  
		Size: 4.5 MB (4495032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3be89d1242837970f7157774c5188f9046677dfb8c676155f7b2d268758d504`  
		Last Modified: Fri, 30 Sep 2022 01:51:30 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - windows version 10.0.17763.3406; amd64

```console
$ docker pull nats@sha256:2861931a21dd96bdbd1686faf3a14c6927dc24203b8c04d30b2116ef4d670e64
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **108.3 MB (108299212 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc0fee332755f830a4cef70df70da46a2cb2c28daadd327e68b97dbf22b35166`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 09 Sep 2022 22:22:51 GMT
RUN Apply image 10.0.17763.3406
# Wed, 14 Sep 2022 15:41:36 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 30 Sep 2022 00:18:47 GMT
RUN cmd /S /C #(nop) COPY file:da89208003aed19cb9852334329c2f8b4dfdfe3218c3f05bba8fcb3247acc400 in C:\nats-server.exe 
# Fri, 30 Sep 2022 00:18:48 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Fri, 30 Sep 2022 00:18:49 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Fri, 30 Sep 2022 00:18:50 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 30 Sep 2022 00:18:51 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:bcd4ab6c304faa0a7f4e183705a7f6e4545b728788221d17886d2a507ea0a06d`  
		Size: 103.3 MB (103334221 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b6bda313a93b8c355d5adf6e15f4b805f705c3741b235a7e4644bbffe6a6af3d`  
		Last Modified: Wed, 14 Sep 2022 15:42:30 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c046270960bff604e9be6498c1c0ee8367958198004e91286a8252366f7185c`  
		Last Modified: Fri, 30 Sep 2022 00:19:41 GMT  
		Size: 5.0 MB (4958572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1087232c1623e24e6883cc4c33bb9ff4926cfc24df9f4909f09db53185f2fe15`  
		Last Modified: Fri, 30 Sep 2022 00:19:40 GMT  
		Size: 1.8 KB (1774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83e77ee18b12423f469199b766a08c031324d15169a9f2e690bf77ccbb796ecd`  
		Last Modified: Fri, 30 Sep 2022 00:19:40 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4549b9baa74eb7ff07539b979f0966c66afb35858810779ec9d7572da5777e49`  
		Last Modified: Fri, 30 Sep 2022 00:19:40 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ee9032ad08c565fc85469a687bbaddfa40a6066692a113da46c758c5d591e4a`  
		Last Modified: Fri, 30 Sep 2022 00:19:40 GMT  
		Size: 1.2 KB (1176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-alpine`

```console
$ docker pull nats@sha256:7b0816d59fbc8f00c834f53bc067bdbb35f27b79cef23e555ecd98496c9c9420
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-alpine` - linux; amd64

```console
$ docker pull nats@sha256:93b6c178034659b624ec39316bec9daeb14b38f690a531eaf5687c8f9a6420f6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.0 MB (7998419 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5068a20fcd0f44c75cc992b50a0c9406d62900af1d7756407b98f67a5aff6049`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Fri, 30 Sep 2022 00:24:33 GMT
ENV NATS_SERVER=2.9.2
# Fri, 30 Sep 2022 00:24:35 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='a2c6ff2c7342198ed61136658310a8f3c336426b07062ed0a073c617ddf4b503' ;; 		armhf) natsArch='arm6'; sha256='918ee03dbc6ab17339f7510940945cdbb07fb15e5599b08961b17e732de0308e' ;; 		armv7) natsArch='arm7'; sha256='2de2669cd17d8c5ad118d7b1b45dbf84fd2ea2baad728cca971df09715086760' ;; 		x86_64) natsArch='amd64'; sha256='7f8f9397247ed5c69eb1ecee25ef5181be822eb85645451389f11dfc9680ed6e' ;; 		x86) natsArch='386'; sha256='dc8793a9778fecd44d71837ecd52174aec79d2115eb895373cc9dd7797d8b6a0' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 30 Sep 2022 00:24:35 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 30 Sep 2022 00:24:35 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 30 Sep 2022 00:24:35 GMT
EXPOSE 4222 6222 8222
# Fri, 30 Sep 2022 00:24:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 30 Sep 2022 00:24:35 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf1cfb9d9ea4605961cdb87b6f9e44cdcfdf68501e6502197a61ba80d7fa2cf3`  
		Last Modified: Fri, 30 Sep 2022 00:25:27 GMT  
		Size: 5.2 MB (5191367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f19aac431077ee9634be9f5879d95e018b853fe9f4355edfb009578928af4a8b`  
		Last Modified: Fri, 30 Sep 2022 00:25:26 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d803ce9173785ad956d0980594d07b7c002d401ec4f7038696cea1a816f8eeba`  
		Last Modified: Fri, 30 Sep 2022 00:25:26 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:1b1b13874064770ee71ee054d372744f61509858d4e2f0e728f4f7e3d0c96979
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7569288 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca1a0478849efea10188e490a19d87485a7e44be7adeb5a71abc150e21ad71b4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:22 GMT
ADD file:e8733e8cc0a81e15ca4041760b6e27392c34171512d34405a9b262b1fff5c687 in / 
# Tue, 09 Aug 2022 17:49:22 GMT
CMD ["/bin/sh"]
# Fri, 30 Sep 2022 00:15:00 GMT
ENV NATS_SERVER=2.9.2
# Fri, 30 Sep 2022 00:15:03 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='a2c6ff2c7342198ed61136658310a8f3c336426b07062ed0a073c617ddf4b503' ;; 		armhf) natsArch='arm6'; sha256='918ee03dbc6ab17339f7510940945cdbb07fb15e5599b08961b17e732de0308e' ;; 		armv7) natsArch='arm7'; sha256='2de2669cd17d8c5ad118d7b1b45dbf84fd2ea2baad728cca971df09715086760' ;; 		x86_64) natsArch='amd64'; sha256='7f8f9397247ed5c69eb1ecee25ef5181be822eb85645451389f11dfc9680ed6e' ;; 		x86) natsArch='386'; sha256='dc8793a9778fecd44d71837ecd52174aec79d2115eb895373cc9dd7797d8b6a0' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 30 Sep 2022 00:15:03 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 30 Sep 2022 00:15:03 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 30 Sep 2022 00:15:03 GMT
EXPOSE 4222 6222 8222
# Fri, 30 Sep 2022 00:15:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 30 Sep 2022 00:15:03 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9506b835437abb4d8ba1683e00c500b8f77e1975e930b356fbb72f2dbdc274d9`  
		Last Modified: Tue, 09 Aug 2022 17:50:33 GMT  
		Size: 2.6 MB (2613965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70e3a299d439ca160a2da5bc72a2fbdfe0d669e0251c6c9ca166ab1f6572234f`  
		Last Modified: Fri, 30 Sep 2022 00:16:18 GMT  
		Size: 5.0 MB (4954323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c2c24ad6cbf82b17aa717ce52a3630fce897bdc317f1cd90fa28a0b18ec0132`  
		Last Modified: Fri, 30 Sep 2022 00:16:17 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8569952349d4aaee564b407fc4a769f8afee1973b746dbc535f7ec1d82ee711f`  
		Last Modified: Fri, 30 Sep 2022 00:16:17 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:2acfd2cdc64cbd116f1f26fd834f476761f9bd485105fc5e9bf4e56596077414
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.4 MB (7369328 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:71027a1b3accd3e7e548dd995f0f20adb3aac785ca9a3f8e122b085367eef6be`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 16:57:44 GMT
ADD file:75521fe16320b193092588f6f31052c85e736965ceb11673de18bd14965a45e6 in / 
# Tue, 09 Aug 2022 16:57:44 GMT
CMD ["/bin/sh"]
# Fri, 30 Sep 2022 12:21:21 GMT
ENV NATS_SERVER=2.9.2
# Fri, 30 Sep 2022 12:21:23 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='a2c6ff2c7342198ed61136658310a8f3c336426b07062ed0a073c617ddf4b503' ;; 		armhf) natsArch='arm6'; sha256='918ee03dbc6ab17339f7510940945cdbb07fb15e5599b08961b17e732de0308e' ;; 		armv7) natsArch='arm7'; sha256='2de2669cd17d8c5ad118d7b1b45dbf84fd2ea2baad728cca971df09715086760' ;; 		x86_64) natsArch='amd64'; sha256='7f8f9397247ed5c69eb1ecee25ef5181be822eb85645451389f11dfc9680ed6e' ;; 		x86) natsArch='386'; sha256='dc8793a9778fecd44d71837ecd52174aec79d2115eb895373cc9dd7797d8b6a0' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 30 Sep 2022 12:21:23 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 30 Sep 2022 12:21:23 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 30 Sep 2022 12:21:23 GMT
EXPOSE 4222 6222 8222
# Fri, 30 Sep 2022 12:21:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 30 Sep 2022 12:21:23 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:c6556b3b6858c6fa1e328377cc2c4becdc9cd1bc3e7302aa7299936522cf93ba`  
		Last Modified: Tue, 09 Aug 2022 16:58:55 GMT  
		Size: 2.4 MB (2417065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce37993864155926f403118474bfe7f519e53160887c3676f0cb079b2da279fd`  
		Last Modified: Fri, 30 Sep 2022 12:22:41 GMT  
		Size: 5.0 MB (4951267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:404500b58d5dc1fd3cb248fe12df440b55e9c3ab7d8671bd898e861be2f61927`  
		Last Modified: Fri, 30 Sep 2022 12:22:40 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04c6d22f211806f08bc6bc9690b5aff62e8fd42fe73b976a1d18dee96b17d9eb`  
		Last Modified: Fri, 30 Sep 2022 12:22:40 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:63f1ff386adae53c49382ca5b6587c2dea35fc1af28e97033450cae49cfdcdab
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.5 MB (7485211 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6bf9a9bbea015857fed1ac343d2011fbc4ad3bfdc076c1963bd616875d0e0c88`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Fri, 30 Sep 2022 01:49:52 GMT
ENV NATS_SERVER=2.9.2
# Fri, 30 Sep 2022 01:49:55 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='a2c6ff2c7342198ed61136658310a8f3c336426b07062ed0a073c617ddf4b503' ;; 		armhf) natsArch='arm6'; sha256='918ee03dbc6ab17339f7510940945cdbb07fb15e5599b08961b17e732de0308e' ;; 		armv7) natsArch='arm7'; sha256='2de2669cd17d8c5ad118d7b1b45dbf84fd2ea2baad728cca971df09715086760' ;; 		x86_64) natsArch='amd64'; sha256='7f8f9397247ed5c69eb1ecee25ef5181be822eb85645451389f11dfc9680ed6e' ;; 		x86) natsArch='386'; sha256='dc8793a9778fecd44d71837ecd52174aec79d2115eb895373cc9dd7797d8b6a0' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 30 Sep 2022 01:49:57 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 30 Sep 2022 01:49:58 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 30 Sep 2022 01:49:58 GMT
EXPOSE 4222 6222 8222
# Fri, 30 Sep 2022 01:49:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 30 Sep 2022 01:50:00 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e30b79a866266b8c14d92afcced6bb4ffc32f152bafd6a4725eb24f2e5308da`  
		Last Modified: Fri, 30 Sep 2022 01:51:03 GMT  
		Size: 4.8 MB (4776577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d4ccb803f2d84c949447676b42f6b097337ce63fc73b9ff1b71715829193bb3`  
		Last Modified: Fri, 30 Sep 2022 01:51:02 GMT  
		Size: 559.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3baeeddb056b5f80c9eaf6dea17b085fd4b29d71b71ab6a68165224637f280da`  
		Last Modified: Fri, 30 Sep 2022 01:51:02 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-alpine3.16`

```console
$ docker pull nats@sha256:7b0816d59fbc8f00c834f53bc067bdbb35f27b79cef23e555ecd98496c9c9420
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-alpine3.16` - linux; amd64

```console
$ docker pull nats@sha256:93b6c178034659b624ec39316bec9daeb14b38f690a531eaf5687c8f9a6420f6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.0 MB (7998419 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5068a20fcd0f44c75cc992b50a0c9406d62900af1d7756407b98f67a5aff6049`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Fri, 30 Sep 2022 00:24:33 GMT
ENV NATS_SERVER=2.9.2
# Fri, 30 Sep 2022 00:24:35 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='a2c6ff2c7342198ed61136658310a8f3c336426b07062ed0a073c617ddf4b503' ;; 		armhf) natsArch='arm6'; sha256='918ee03dbc6ab17339f7510940945cdbb07fb15e5599b08961b17e732de0308e' ;; 		armv7) natsArch='arm7'; sha256='2de2669cd17d8c5ad118d7b1b45dbf84fd2ea2baad728cca971df09715086760' ;; 		x86_64) natsArch='amd64'; sha256='7f8f9397247ed5c69eb1ecee25ef5181be822eb85645451389f11dfc9680ed6e' ;; 		x86) natsArch='386'; sha256='dc8793a9778fecd44d71837ecd52174aec79d2115eb895373cc9dd7797d8b6a0' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 30 Sep 2022 00:24:35 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 30 Sep 2022 00:24:35 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 30 Sep 2022 00:24:35 GMT
EXPOSE 4222 6222 8222
# Fri, 30 Sep 2022 00:24:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 30 Sep 2022 00:24:35 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf1cfb9d9ea4605961cdb87b6f9e44cdcfdf68501e6502197a61ba80d7fa2cf3`  
		Last Modified: Fri, 30 Sep 2022 00:25:27 GMT  
		Size: 5.2 MB (5191367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f19aac431077ee9634be9f5879d95e018b853fe9f4355edfb009578928af4a8b`  
		Last Modified: Fri, 30 Sep 2022 00:25:26 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d803ce9173785ad956d0980594d07b7c002d401ec4f7038696cea1a816f8eeba`  
		Last Modified: Fri, 30 Sep 2022 00:25:26 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.16` - linux; arm variant v6

```console
$ docker pull nats@sha256:1b1b13874064770ee71ee054d372744f61509858d4e2f0e728f4f7e3d0c96979
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7569288 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca1a0478849efea10188e490a19d87485a7e44be7adeb5a71abc150e21ad71b4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:22 GMT
ADD file:e8733e8cc0a81e15ca4041760b6e27392c34171512d34405a9b262b1fff5c687 in / 
# Tue, 09 Aug 2022 17:49:22 GMT
CMD ["/bin/sh"]
# Fri, 30 Sep 2022 00:15:00 GMT
ENV NATS_SERVER=2.9.2
# Fri, 30 Sep 2022 00:15:03 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='a2c6ff2c7342198ed61136658310a8f3c336426b07062ed0a073c617ddf4b503' ;; 		armhf) natsArch='arm6'; sha256='918ee03dbc6ab17339f7510940945cdbb07fb15e5599b08961b17e732de0308e' ;; 		armv7) natsArch='arm7'; sha256='2de2669cd17d8c5ad118d7b1b45dbf84fd2ea2baad728cca971df09715086760' ;; 		x86_64) natsArch='amd64'; sha256='7f8f9397247ed5c69eb1ecee25ef5181be822eb85645451389f11dfc9680ed6e' ;; 		x86) natsArch='386'; sha256='dc8793a9778fecd44d71837ecd52174aec79d2115eb895373cc9dd7797d8b6a0' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 30 Sep 2022 00:15:03 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 30 Sep 2022 00:15:03 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 30 Sep 2022 00:15:03 GMT
EXPOSE 4222 6222 8222
# Fri, 30 Sep 2022 00:15:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 30 Sep 2022 00:15:03 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9506b835437abb4d8ba1683e00c500b8f77e1975e930b356fbb72f2dbdc274d9`  
		Last Modified: Tue, 09 Aug 2022 17:50:33 GMT  
		Size: 2.6 MB (2613965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70e3a299d439ca160a2da5bc72a2fbdfe0d669e0251c6c9ca166ab1f6572234f`  
		Last Modified: Fri, 30 Sep 2022 00:16:18 GMT  
		Size: 5.0 MB (4954323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c2c24ad6cbf82b17aa717ce52a3630fce897bdc317f1cd90fa28a0b18ec0132`  
		Last Modified: Fri, 30 Sep 2022 00:16:17 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8569952349d4aaee564b407fc4a769f8afee1973b746dbc535f7ec1d82ee711f`  
		Last Modified: Fri, 30 Sep 2022 00:16:17 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.16` - linux; arm variant v7

```console
$ docker pull nats@sha256:2acfd2cdc64cbd116f1f26fd834f476761f9bd485105fc5e9bf4e56596077414
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.4 MB (7369328 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:71027a1b3accd3e7e548dd995f0f20adb3aac785ca9a3f8e122b085367eef6be`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 16:57:44 GMT
ADD file:75521fe16320b193092588f6f31052c85e736965ceb11673de18bd14965a45e6 in / 
# Tue, 09 Aug 2022 16:57:44 GMT
CMD ["/bin/sh"]
# Fri, 30 Sep 2022 12:21:21 GMT
ENV NATS_SERVER=2.9.2
# Fri, 30 Sep 2022 12:21:23 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='a2c6ff2c7342198ed61136658310a8f3c336426b07062ed0a073c617ddf4b503' ;; 		armhf) natsArch='arm6'; sha256='918ee03dbc6ab17339f7510940945cdbb07fb15e5599b08961b17e732de0308e' ;; 		armv7) natsArch='arm7'; sha256='2de2669cd17d8c5ad118d7b1b45dbf84fd2ea2baad728cca971df09715086760' ;; 		x86_64) natsArch='amd64'; sha256='7f8f9397247ed5c69eb1ecee25ef5181be822eb85645451389f11dfc9680ed6e' ;; 		x86) natsArch='386'; sha256='dc8793a9778fecd44d71837ecd52174aec79d2115eb895373cc9dd7797d8b6a0' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 30 Sep 2022 12:21:23 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 30 Sep 2022 12:21:23 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 30 Sep 2022 12:21:23 GMT
EXPOSE 4222 6222 8222
# Fri, 30 Sep 2022 12:21:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 30 Sep 2022 12:21:23 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:c6556b3b6858c6fa1e328377cc2c4becdc9cd1bc3e7302aa7299936522cf93ba`  
		Last Modified: Tue, 09 Aug 2022 16:58:55 GMT  
		Size: 2.4 MB (2417065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce37993864155926f403118474bfe7f519e53160887c3676f0cb079b2da279fd`  
		Last Modified: Fri, 30 Sep 2022 12:22:41 GMT  
		Size: 5.0 MB (4951267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:404500b58d5dc1fd3cb248fe12df440b55e9c3ab7d8671bd898e861be2f61927`  
		Last Modified: Fri, 30 Sep 2022 12:22:40 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04c6d22f211806f08bc6bc9690b5aff62e8fd42fe73b976a1d18dee96b17d9eb`  
		Last Modified: Fri, 30 Sep 2022 12:22:40 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.16` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:63f1ff386adae53c49382ca5b6587c2dea35fc1af28e97033450cae49cfdcdab
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.5 MB (7485211 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6bf9a9bbea015857fed1ac343d2011fbc4ad3bfdc076c1963bd616875d0e0c88`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Fri, 30 Sep 2022 01:49:52 GMT
ENV NATS_SERVER=2.9.2
# Fri, 30 Sep 2022 01:49:55 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='a2c6ff2c7342198ed61136658310a8f3c336426b07062ed0a073c617ddf4b503' ;; 		armhf) natsArch='arm6'; sha256='918ee03dbc6ab17339f7510940945cdbb07fb15e5599b08961b17e732de0308e' ;; 		armv7) natsArch='arm7'; sha256='2de2669cd17d8c5ad118d7b1b45dbf84fd2ea2baad728cca971df09715086760' ;; 		x86_64) natsArch='amd64'; sha256='7f8f9397247ed5c69eb1ecee25ef5181be822eb85645451389f11dfc9680ed6e' ;; 		x86) natsArch='386'; sha256='dc8793a9778fecd44d71837ecd52174aec79d2115eb895373cc9dd7797d8b6a0' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 30 Sep 2022 01:49:57 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 30 Sep 2022 01:49:58 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 30 Sep 2022 01:49:58 GMT
EXPOSE 4222 6222 8222
# Fri, 30 Sep 2022 01:49:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 30 Sep 2022 01:50:00 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e30b79a866266b8c14d92afcced6bb4ffc32f152bafd6a4725eb24f2e5308da`  
		Last Modified: Fri, 30 Sep 2022 01:51:03 GMT  
		Size: 4.8 MB (4776577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d4ccb803f2d84c949447676b42f6b097337ce63fc73b9ff1b71715829193bb3`  
		Last Modified: Fri, 30 Sep 2022 01:51:02 GMT  
		Size: 559.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3baeeddb056b5f80c9eaf6dea17b085fd4b29d71b71ab6a68165224637f280da`  
		Last Modified: Fri, 30 Sep 2022 01:51:02 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-linux`

```console
$ docker pull nats@sha256:5f9faa293f743a8c78944dc1827132cc658e8ffcb2746d00e6ea69316a9fe3d9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-linux` - linux; amd64

```console
$ docker pull nats@sha256:73a511425369d8e883fc5784023028b7ed02c252e6db030e776b2e6a76bb90ca
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4907513 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf3ba31eb02c938f2ab28c2b60358ef903503ce4a2fb5e2df6f4714d04e74619`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 30 Sep 2022 00:25:01 GMT
COPY file:ef7d265008705c7f8da964d29a2883d21303aab4d4520c3327ca6ce57348e137 in /nats-server 
# Fri, 30 Sep 2022 00:25:01 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 30 Sep 2022 00:25:01 GMT
EXPOSE 4222 6222 8222
# Fri, 30 Sep 2022 00:25:01 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 30 Sep 2022 00:25:01 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 30 Sep 2022 00:25:01 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:325d5a714be1f0303eebb8d34c9b23e1b15c5e7e46eb29d0f90511112fb86894`  
		Last Modified: Fri, 30 Sep 2022 00:25:50 GMT  
		Size: 4.9 MB (4907005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06b03a363308e84c4fc60d5ac2d5b9374e811456edecdb1e302e59198bfb1ca4`  
		Last Modified: Fri, 30 Sep 2022 00:25:49 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:22be654fd606d7db5e28383ce35794c881f25b77908c6f981c2442b117d7df19
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4671534 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1eeeee00c7520737eb3766018dde7f3dd63c971938d98ff49cca225f0e6c6990`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 30 Sep 2022 00:15:17 GMT
COPY file:2de52eed8721a4ef1e4c8adb2f046a7ffa8e689d614c704b329ef2bafc7dfe5c in /nats-server 
# Fri, 30 Sep 2022 00:15:17 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 30 Sep 2022 00:15:17 GMT
EXPOSE 4222 6222 8222
# Fri, 30 Sep 2022 00:15:18 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 30 Sep 2022 00:15:18 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 30 Sep 2022 00:15:18 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:948e55d9b8c745ce1f9007c64a6da65d66c0d554fa7e5808a04081a1d0754a6c`  
		Last Modified: Fri, 30 Sep 2022 00:16:49 GMT  
		Size: 4.7 MB (4671025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14bdee3fcf17688810034aff56b746397e799579ff11654f2a2ec59274a9e161`  
		Last Modified: Fri, 30 Sep 2022 00:16:48 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:dce0b0ef268b27c6417ee879c4f500273d8eabe0f3347ed2ac19b28a166085e2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4661683 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93f043be0120df37adc5618c50a4eb09f405d9a23f0794314f36c76be8bda597`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 30 Sep 2022 12:21:44 GMT
COPY file:e57d6f6c709cd7f891a48782c812655546ed7ed7194710fb4ff95d3225a8cb24 in /nats-server 
# Fri, 30 Sep 2022 12:21:44 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 30 Sep 2022 12:21:44 GMT
EXPOSE 4222 6222 8222
# Fri, 30 Sep 2022 12:21:44 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 30 Sep 2022 12:21:44 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 30 Sep 2022 12:21:44 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6709a2d5812e1f5aabc828977b23e9033fb28dd6d79bad682b986bfeaf468265`  
		Last Modified: Fri, 30 Sep 2022 12:23:13 GMT  
		Size: 4.7 MB (4661175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:913a6877bd39f71d19820c3493253d22c565656c7058ca6e5deb8e20280f8ad6`  
		Last Modified: Fri, 30 Sep 2022 12:23:12 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:6d0d5cfcf4b908ca419719473183dd4000ebe2e77e9fb1088f51f2195324d865
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4495540 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7069cf895c76381ff91ad174ed58ca07743ca741317f4a2c20ea3b1f1bae44ce`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 30 Sep 2022 01:50:11 GMT
COPY file:06300839e6ae56288247488999d2e96ee71c9bb64453bfa88faa4cbfc85a23e2 in /nats-server 
# Fri, 30 Sep 2022 01:50:12 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 30 Sep 2022 01:50:12 GMT
EXPOSE 4222 6222 8222
# Fri, 30 Sep 2022 01:50:13 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 30 Sep 2022 01:50:14 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 30 Sep 2022 01:50:15 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:71fcb6de35d4d1378bd805b642a59de493c8957d351b1f521d05492db21c54d6`  
		Last Modified: Fri, 30 Sep 2022 01:51:31 GMT  
		Size: 4.5 MB (4495032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3be89d1242837970f7157774c5188f9046677dfb8c676155f7b2d268758d504`  
		Last Modified: Fri, 30 Sep 2022 01:51:30 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-nanoserver`

```console
$ docker pull nats@sha256:679b0d8e5bafa2c6893078adf595ebd301d9df9258ca22d088788c40d6ca5d28
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3406; amd64

### `nats:2-nanoserver` - windows version 10.0.17763.3406; amd64

```console
$ docker pull nats@sha256:2861931a21dd96bdbd1686faf3a14c6927dc24203b8c04d30b2116ef4d670e64
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **108.3 MB (108299212 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc0fee332755f830a4cef70df70da46a2cb2c28daadd327e68b97dbf22b35166`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 09 Sep 2022 22:22:51 GMT
RUN Apply image 10.0.17763.3406
# Wed, 14 Sep 2022 15:41:36 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 30 Sep 2022 00:18:47 GMT
RUN cmd /S /C #(nop) COPY file:da89208003aed19cb9852334329c2f8b4dfdfe3218c3f05bba8fcb3247acc400 in C:\nats-server.exe 
# Fri, 30 Sep 2022 00:18:48 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Fri, 30 Sep 2022 00:18:49 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Fri, 30 Sep 2022 00:18:50 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 30 Sep 2022 00:18:51 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:bcd4ab6c304faa0a7f4e183705a7f6e4545b728788221d17886d2a507ea0a06d`  
		Size: 103.3 MB (103334221 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b6bda313a93b8c355d5adf6e15f4b805f705c3741b235a7e4644bbffe6a6af3d`  
		Last Modified: Wed, 14 Sep 2022 15:42:30 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c046270960bff604e9be6498c1c0ee8367958198004e91286a8252366f7185c`  
		Last Modified: Fri, 30 Sep 2022 00:19:41 GMT  
		Size: 5.0 MB (4958572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1087232c1623e24e6883cc4c33bb9ff4926cfc24df9f4909f09db53185f2fe15`  
		Last Modified: Fri, 30 Sep 2022 00:19:40 GMT  
		Size: 1.8 KB (1774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83e77ee18b12423f469199b766a08c031324d15169a9f2e690bf77ccbb796ecd`  
		Last Modified: Fri, 30 Sep 2022 00:19:40 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4549b9baa74eb7ff07539b979f0966c66afb35858810779ec9d7572da5777e49`  
		Last Modified: Fri, 30 Sep 2022 00:19:40 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ee9032ad08c565fc85469a687bbaddfa40a6066692a113da46c758c5d591e4a`  
		Last Modified: Fri, 30 Sep 2022 00:19:40 GMT  
		Size: 1.2 KB (1176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-nanoserver-1809`

```console
$ docker pull nats@sha256:679b0d8e5bafa2c6893078adf595ebd301d9df9258ca22d088788c40d6ca5d28
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3406; amd64

### `nats:2-nanoserver-1809` - windows version 10.0.17763.3406; amd64

```console
$ docker pull nats@sha256:2861931a21dd96bdbd1686faf3a14c6927dc24203b8c04d30b2116ef4d670e64
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **108.3 MB (108299212 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc0fee332755f830a4cef70df70da46a2cb2c28daadd327e68b97dbf22b35166`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 09 Sep 2022 22:22:51 GMT
RUN Apply image 10.0.17763.3406
# Wed, 14 Sep 2022 15:41:36 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 30 Sep 2022 00:18:47 GMT
RUN cmd /S /C #(nop) COPY file:da89208003aed19cb9852334329c2f8b4dfdfe3218c3f05bba8fcb3247acc400 in C:\nats-server.exe 
# Fri, 30 Sep 2022 00:18:48 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Fri, 30 Sep 2022 00:18:49 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Fri, 30 Sep 2022 00:18:50 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 30 Sep 2022 00:18:51 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:bcd4ab6c304faa0a7f4e183705a7f6e4545b728788221d17886d2a507ea0a06d`  
		Size: 103.3 MB (103334221 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b6bda313a93b8c355d5adf6e15f4b805f705c3741b235a7e4644bbffe6a6af3d`  
		Last Modified: Wed, 14 Sep 2022 15:42:30 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c046270960bff604e9be6498c1c0ee8367958198004e91286a8252366f7185c`  
		Last Modified: Fri, 30 Sep 2022 00:19:41 GMT  
		Size: 5.0 MB (4958572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1087232c1623e24e6883cc4c33bb9ff4926cfc24df9f4909f09db53185f2fe15`  
		Last Modified: Fri, 30 Sep 2022 00:19:40 GMT  
		Size: 1.8 KB (1774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83e77ee18b12423f469199b766a08c031324d15169a9f2e690bf77ccbb796ecd`  
		Last Modified: Fri, 30 Sep 2022 00:19:40 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4549b9baa74eb7ff07539b979f0966c66afb35858810779ec9d7572da5777e49`  
		Last Modified: Fri, 30 Sep 2022 00:19:40 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ee9032ad08c565fc85469a687bbaddfa40a6066692a113da46c758c5d591e4a`  
		Last Modified: Fri, 30 Sep 2022 00:19:40 GMT  
		Size: 1.2 KB (1176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-scratch`

```console
$ docker pull nats@sha256:5f9faa293f743a8c78944dc1827132cc658e8ffcb2746d00e6ea69316a9fe3d9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-scratch` - linux; amd64

```console
$ docker pull nats@sha256:73a511425369d8e883fc5784023028b7ed02c252e6db030e776b2e6a76bb90ca
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4907513 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf3ba31eb02c938f2ab28c2b60358ef903503ce4a2fb5e2df6f4714d04e74619`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 30 Sep 2022 00:25:01 GMT
COPY file:ef7d265008705c7f8da964d29a2883d21303aab4d4520c3327ca6ce57348e137 in /nats-server 
# Fri, 30 Sep 2022 00:25:01 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 30 Sep 2022 00:25:01 GMT
EXPOSE 4222 6222 8222
# Fri, 30 Sep 2022 00:25:01 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 30 Sep 2022 00:25:01 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 30 Sep 2022 00:25:01 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:325d5a714be1f0303eebb8d34c9b23e1b15c5e7e46eb29d0f90511112fb86894`  
		Last Modified: Fri, 30 Sep 2022 00:25:50 GMT  
		Size: 4.9 MB (4907005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06b03a363308e84c4fc60d5ac2d5b9374e811456edecdb1e302e59198bfb1ca4`  
		Last Modified: Fri, 30 Sep 2022 00:25:49 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:22be654fd606d7db5e28383ce35794c881f25b77908c6f981c2442b117d7df19
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4671534 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1eeeee00c7520737eb3766018dde7f3dd63c971938d98ff49cca225f0e6c6990`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 30 Sep 2022 00:15:17 GMT
COPY file:2de52eed8721a4ef1e4c8adb2f046a7ffa8e689d614c704b329ef2bafc7dfe5c in /nats-server 
# Fri, 30 Sep 2022 00:15:17 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 30 Sep 2022 00:15:17 GMT
EXPOSE 4222 6222 8222
# Fri, 30 Sep 2022 00:15:18 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 30 Sep 2022 00:15:18 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 30 Sep 2022 00:15:18 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:948e55d9b8c745ce1f9007c64a6da65d66c0d554fa7e5808a04081a1d0754a6c`  
		Last Modified: Fri, 30 Sep 2022 00:16:49 GMT  
		Size: 4.7 MB (4671025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14bdee3fcf17688810034aff56b746397e799579ff11654f2a2ec59274a9e161`  
		Last Modified: Fri, 30 Sep 2022 00:16:48 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:dce0b0ef268b27c6417ee879c4f500273d8eabe0f3347ed2ac19b28a166085e2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4661683 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93f043be0120df37adc5618c50a4eb09f405d9a23f0794314f36c76be8bda597`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 30 Sep 2022 12:21:44 GMT
COPY file:e57d6f6c709cd7f891a48782c812655546ed7ed7194710fb4ff95d3225a8cb24 in /nats-server 
# Fri, 30 Sep 2022 12:21:44 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 30 Sep 2022 12:21:44 GMT
EXPOSE 4222 6222 8222
# Fri, 30 Sep 2022 12:21:44 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 30 Sep 2022 12:21:44 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 30 Sep 2022 12:21:44 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6709a2d5812e1f5aabc828977b23e9033fb28dd6d79bad682b986bfeaf468265`  
		Last Modified: Fri, 30 Sep 2022 12:23:13 GMT  
		Size: 4.7 MB (4661175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:913a6877bd39f71d19820c3493253d22c565656c7058ca6e5deb8e20280f8ad6`  
		Last Modified: Fri, 30 Sep 2022 12:23:12 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:6d0d5cfcf4b908ca419719473183dd4000ebe2e77e9fb1088f51f2195324d865
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4495540 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7069cf895c76381ff91ad174ed58ca07743ca741317f4a2c20ea3b1f1bae44ce`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 30 Sep 2022 01:50:11 GMT
COPY file:06300839e6ae56288247488999d2e96ee71c9bb64453bfa88faa4cbfc85a23e2 in /nats-server 
# Fri, 30 Sep 2022 01:50:12 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 30 Sep 2022 01:50:12 GMT
EXPOSE 4222 6222 8222
# Fri, 30 Sep 2022 01:50:13 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 30 Sep 2022 01:50:14 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 30 Sep 2022 01:50:15 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:71fcb6de35d4d1378bd805b642a59de493c8957d351b1f521d05492db21c54d6`  
		Last Modified: Fri, 30 Sep 2022 01:51:31 GMT  
		Size: 4.5 MB (4495032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3be89d1242837970f7157774c5188f9046677dfb8c676155f7b2d268758d504`  
		Last Modified: Fri, 30 Sep 2022 01:51:30 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-windowsservercore`

```console
$ docker pull nats@sha256:3357d7889ebcb10a163ba56eff66f60ff010e161b38e1f401cc136e7a6879baf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3406; amd64

### `nats:2-windowsservercore` - windows version 10.0.17763.3406; amd64

```console
$ docker pull nats@sha256:214e04a7dc77ff783ac336d010ba64eb98f2c8722d522260bf340c2df3d521e7
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2709236645 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:30cb30cff6676167599e8b4fd9f6b053b3e6fa2f5418a7a419e631956a014e9e`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Fri, 09 Sep 2022 22:43:02 GMT
RUN Install update 10.0.17763.3406
# Wed, 14 Sep 2022 13:39:18 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 14 Sep 2022 15:38:54 GMT
ENV NATS_DOCKERIZED=1
# Fri, 30 Sep 2022 00:15:50 GMT
ENV NATS_SERVER=2.9.2
# Fri, 30 Sep 2022 00:15:51 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.9.2/nats-server-v2.9.2-windows-amd64.zip
# Fri, 30 Sep 2022 00:15:52 GMT
ENV NATS_SERVER_SHASUM=cd3d2a9d78c235292afc27f812baee7817180fcfe5ebba662e72f0cc821d04fb
# Fri, 30 Sep 2022 00:16:59 GMT
RUN Set-PSDebug -Trace 2
# Fri, 30 Sep 2022 00:18:30 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 30 Sep 2022 00:18:31 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Fri, 30 Sep 2022 00:18:31 GMT
EXPOSE 4222 6222 8222
# Fri, 30 Sep 2022 00:18:32 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 30 Sep 2022 00:18:33 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:cee64bf279e2ca8e924884a10ecb98bfa79c7f0cc8d25e73039b9aeb940815b6`  
		Size: 826.4 MB (826398623 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3c428406510f0a47ed60f28060a7d625d42344a95fdcb7c4f5746fb8857c3328`  
		Last Modified: Wed, 14 Sep 2022 15:42:13 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf4bba85c5cc970a66b01ed6f4cabffa7705a0bdbc18907894f94c09b5ee2618`  
		Last Modified: Wed, 14 Sep 2022 15:42:12 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a29319534b1836908aab29077ce165236693f20e5abbb69a70639c6cce19223b`  
		Last Modified: Fri, 30 Sep 2022 00:19:24 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d34f7b3a98b75cbb6f21f33118a7f43b9efe7d7d8ef5d9f47b5ca73470abd339`  
		Last Modified: Fri, 30 Sep 2022 00:19:24 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2119397eb3051d4784ced2882a1c0f1d2995cec67f5954fd5f33fde4b6ab4c3a`  
		Last Modified: Fri, 30 Sep 2022 00:19:24 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cdecf001ef7e4a9db54aa1a639bf5036f69cfc71a2d6b1b9089c1a3810373aa`  
		Last Modified: Fri, 30 Sep 2022 00:19:24 GMT  
		Size: 358.1 KB (358089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4a5a2ffe352520814f5794422903ec9e717d37294931ca81f856257a419ee1f`  
		Last Modified: Fri, 30 Sep 2022 00:19:23 GMT  
		Size: 5.3 MB (5300456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b80c11ae75a170747a9206d993fe059c9cda9f34c08c9f2eb90bedaef90f322e`  
		Last Modified: Fri, 30 Sep 2022 00:19:22 GMT  
		Size: 2.0 KB (2012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e8020be63ec6ec39f4443bc78e114caf9c24c5686fcf3f84a8c74f38f61b864`  
		Last Modified: Fri, 30 Sep 2022 00:19:22 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50d3d068429b4966cc13e153bdbf220b0259eb72a6a3f507fc5172a963499566`  
		Last Modified: Fri, 30 Sep 2022 00:19:22 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f588edee9a48a943744711d7d4dea00d9e842180f05a759c2edf3e50ee10e06c`  
		Last Modified: Fri, 30 Sep 2022 00:19:22 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-windowsservercore-1809`

```console
$ docker pull nats@sha256:3357d7889ebcb10a163ba56eff66f60ff010e161b38e1f401cc136e7a6879baf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3406; amd64

### `nats:2-windowsservercore-1809` - windows version 10.0.17763.3406; amd64

```console
$ docker pull nats@sha256:214e04a7dc77ff783ac336d010ba64eb98f2c8722d522260bf340c2df3d521e7
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2709236645 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:30cb30cff6676167599e8b4fd9f6b053b3e6fa2f5418a7a419e631956a014e9e`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Fri, 09 Sep 2022 22:43:02 GMT
RUN Install update 10.0.17763.3406
# Wed, 14 Sep 2022 13:39:18 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 14 Sep 2022 15:38:54 GMT
ENV NATS_DOCKERIZED=1
# Fri, 30 Sep 2022 00:15:50 GMT
ENV NATS_SERVER=2.9.2
# Fri, 30 Sep 2022 00:15:51 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.9.2/nats-server-v2.9.2-windows-amd64.zip
# Fri, 30 Sep 2022 00:15:52 GMT
ENV NATS_SERVER_SHASUM=cd3d2a9d78c235292afc27f812baee7817180fcfe5ebba662e72f0cc821d04fb
# Fri, 30 Sep 2022 00:16:59 GMT
RUN Set-PSDebug -Trace 2
# Fri, 30 Sep 2022 00:18:30 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 30 Sep 2022 00:18:31 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Fri, 30 Sep 2022 00:18:31 GMT
EXPOSE 4222 6222 8222
# Fri, 30 Sep 2022 00:18:32 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 30 Sep 2022 00:18:33 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:cee64bf279e2ca8e924884a10ecb98bfa79c7f0cc8d25e73039b9aeb940815b6`  
		Size: 826.4 MB (826398623 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3c428406510f0a47ed60f28060a7d625d42344a95fdcb7c4f5746fb8857c3328`  
		Last Modified: Wed, 14 Sep 2022 15:42:13 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf4bba85c5cc970a66b01ed6f4cabffa7705a0bdbc18907894f94c09b5ee2618`  
		Last Modified: Wed, 14 Sep 2022 15:42:12 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a29319534b1836908aab29077ce165236693f20e5abbb69a70639c6cce19223b`  
		Last Modified: Fri, 30 Sep 2022 00:19:24 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d34f7b3a98b75cbb6f21f33118a7f43b9efe7d7d8ef5d9f47b5ca73470abd339`  
		Last Modified: Fri, 30 Sep 2022 00:19:24 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2119397eb3051d4784ced2882a1c0f1d2995cec67f5954fd5f33fde4b6ab4c3a`  
		Last Modified: Fri, 30 Sep 2022 00:19:24 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cdecf001ef7e4a9db54aa1a639bf5036f69cfc71a2d6b1b9089c1a3810373aa`  
		Last Modified: Fri, 30 Sep 2022 00:19:24 GMT  
		Size: 358.1 KB (358089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4a5a2ffe352520814f5794422903ec9e717d37294931ca81f856257a419ee1f`  
		Last Modified: Fri, 30 Sep 2022 00:19:23 GMT  
		Size: 5.3 MB (5300456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b80c11ae75a170747a9206d993fe059c9cda9f34c08c9f2eb90bedaef90f322e`  
		Last Modified: Fri, 30 Sep 2022 00:19:22 GMT  
		Size: 2.0 KB (2012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e8020be63ec6ec39f4443bc78e114caf9c24c5686fcf3f84a8c74f38f61b864`  
		Last Modified: Fri, 30 Sep 2022 00:19:22 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50d3d068429b4966cc13e153bdbf220b0259eb72a6a3f507fc5172a963499566`  
		Last Modified: Fri, 30 Sep 2022 00:19:22 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f588edee9a48a943744711d7d4dea00d9e842180f05a759c2edf3e50ee10e06c`  
		Last Modified: Fri, 30 Sep 2022 00:19:22 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9`

```console
$ docker pull nats@sha256:2a333e9f7d50ba4dd450e435b65a5b038af6988ab4c19c858cf85c6733667c28
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.3406; amd64

### `nats:2.9` - linux; amd64

```console
$ docker pull nats@sha256:73a511425369d8e883fc5784023028b7ed02c252e6db030e776b2e6a76bb90ca
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4907513 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf3ba31eb02c938f2ab28c2b60358ef903503ce4a2fb5e2df6f4714d04e74619`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 30 Sep 2022 00:25:01 GMT
COPY file:ef7d265008705c7f8da964d29a2883d21303aab4d4520c3327ca6ce57348e137 in /nats-server 
# Fri, 30 Sep 2022 00:25:01 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 30 Sep 2022 00:25:01 GMT
EXPOSE 4222 6222 8222
# Fri, 30 Sep 2022 00:25:01 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 30 Sep 2022 00:25:01 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 30 Sep 2022 00:25:01 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:325d5a714be1f0303eebb8d34c9b23e1b15c5e7e46eb29d0f90511112fb86894`  
		Last Modified: Fri, 30 Sep 2022 00:25:50 GMT  
		Size: 4.9 MB (4907005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06b03a363308e84c4fc60d5ac2d5b9374e811456edecdb1e302e59198bfb1ca4`  
		Last Modified: Fri, 30 Sep 2022 00:25:49 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9` - linux; arm variant v6

```console
$ docker pull nats@sha256:22be654fd606d7db5e28383ce35794c881f25b77908c6f981c2442b117d7df19
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4671534 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1eeeee00c7520737eb3766018dde7f3dd63c971938d98ff49cca225f0e6c6990`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 30 Sep 2022 00:15:17 GMT
COPY file:2de52eed8721a4ef1e4c8adb2f046a7ffa8e689d614c704b329ef2bafc7dfe5c in /nats-server 
# Fri, 30 Sep 2022 00:15:17 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 30 Sep 2022 00:15:17 GMT
EXPOSE 4222 6222 8222
# Fri, 30 Sep 2022 00:15:18 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 30 Sep 2022 00:15:18 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 30 Sep 2022 00:15:18 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:948e55d9b8c745ce1f9007c64a6da65d66c0d554fa7e5808a04081a1d0754a6c`  
		Last Modified: Fri, 30 Sep 2022 00:16:49 GMT  
		Size: 4.7 MB (4671025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14bdee3fcf17688810034aff56b746397e799579ff11654f2a2ec59274a9e161`  
		Last Modified: Fri, 30 Sep 2022 00:16:48 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9` - linux; arm variant v7

```console
$ docker pull nats@sha256:dce0b0ef268b27c6417ee879c4f500273d8eabe0f3347ed2ac19b28a166085e2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4661683 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93f043be0120df37adc5618c50a4eb09f405d9a23f0794314f36c76be8bda597`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 30 Sep 2022 12:21:44 GMT
COPY file:e57d6f6c709cd7f891a48782c812655546ed7ed7194710fb4ff95d3225a8cb24 in /nats-server 
# Fri, 30 Sep 2022 12:21:44 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 30 Sep 2022 12:21:44 GMT
EXPOSE 4222 6222 8222
# Fri, 30 Sep 2022 12:21:44 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 30 Sep 2022 12:21:44 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 30 Sep 2022 12:21:44 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6709a2d5812e1f5aabc828977b23e9033fb28dd6d79bad682b986bfeaf468265`  
		Last Modified: Fri, 30 Sep 2022 12:23:13 GMT  
		Size: 4.7 MB (4661175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:913a6877bd39f71d19820c3493253d22c565656c7058ca6e5deb8e20280f8ad6`  
		Last Modified: Fri, 30 Sep 2022 12:23:12 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:6d0d5cfcf4b908ca419719473183dd4000ebe2e77e9fb1088f51f2195324d865
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4495540 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7069cf895c76381ff91ad174ed58ca07743ca741317f4a2c20ea3b1f1bae44ce`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 30 Sep 2022 01:50:11 GMT
COPY file:06300839e6ae56288247488999d2e96ee71c9bb64453bfa88faa4cbfc85a23e2 in /nats-server 
# Fri, 30 Sep 2022 01:50:12 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 30 Sep 2022 01:50:12 GMT
EXPOSE 4222 6222 8222
# Fri, 30 Sep 2022 01:50:13 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 30 Sep 2022 01:50:14 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 30 Sep 2022 01:50:15 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:71fcb6de35d4d1378bd805b642a59de493c8957d351b1f521d05492db21c54d6`  
		Last Modified: Fri, 30 Sep 2022 01:51:31 GMT  
		Size: 4.5 MB (4495032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3be89d1242837970f7157774c5188f9046677dfb8c676155f7b2d268758d504`  
		Last Modified: Fri, 30 Sep 2022 01:51:30 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9` - windows version 10.0.17763.3406; amd64

```console
$ docker pull nats@sha256:2861931a21dd96bdbd1686faf3a14c6927dc24203b8c04d30b2116ef4d670e64
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **108.3 MB (108299212 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc0fee332755f830a4cef70df70da46a2cb2c28daadd327e68b97dbf22b35166`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 09 Sep 2022 22:22:51 GMT
RUN Apply image 10.0.17763.3406
# Wed, 14 Sep 2022 15:41:36 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 30 Sep 2022 00:18:47 GMT
RUN cmd /S /C #(nop) COPY file:da89208003aed19cb9852334329c2f8b4dfdfe3218c3f05bba8fcb3247acc400 in C:\nats-server.exe 
# Fri, 30 Sep 2022 00:18:48 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Fri, 30 Sep 2022 00:18:49 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Fri, 30 Sep 2022 00:18:50 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 30 Sep 2022 00:18:51 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:bcd4ab6c304faa0a7f4e183705a7f6e4545b728788221d17886d2a507ea0a06d`  
		Size: 103.3 MB (103334221 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b6bda313a93b8c355d5adf6e15f4b805f705c3741b235a7e4644bbffe6a6af3d`  
		Last Modified: Wed, 14 Sep 2022 15:42:30 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c046270960bff604e9be6498c1c0ee8367958198004e91286a8252366f7185c`  
		Last Modified: Fri, 30 Sep 2022 00:19:41 GMT  
		Size: 5.0 MB (4958572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1087232c1623e24e6883cc4c33bb9ff4926cfc24df9f4909f09db53185f2fe15`  
		Last Modified: Fri, 30 Sep 2022 00:19:40 GMT  
		Size: 1.8 KB (1774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83e77ee18b12423f469199b766a08c031324d15169a9f2e690bf77ccbb796ecd`  
		Last Modified: Fri, 30 Sep 2022 00:19:40 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4549b9baa74eb7ff07539b979f0966c66afb35858810779ec9d7572da5777e49`  
		Last Modified: Fri, 30 Sep 2022 00:19:40 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ee9032ad08c565fc85469a687bbaddfa40a6066692a113da46c758c5d591e4a`  
		Last Modified: Fri, 30 Sep 2022 00:19:40 GMT  
		Size: 1.2 KB (1176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-alpine`

```console
$ docker pull nats@sha256:7b0816d59fbc8f00c834f53bc067bdbb35f27b79cef23e555ecd98496c9c9420
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9-alpine` - linux; amd64

```console
$ docker pull nats@sha256:93b6c178034659b624ec39316bec9daeb14b38f690a531eaf5687c8f9a6420f6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.0 MB (7998419 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5068a20fcd0f44c75cc992b50a0c9406d62900af1d7756407b98f67a5aff6049`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Fri, 30 Sep 2022 00:24:33 GMT
ENV NATS_SERVER=2.9.2
# Fri, 30 Sep 2022 00:24:35 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='a2c6ff2c7342198ed61136658310a8f3c336426b07062ed0a073c617ddf4b503' ;; 		armhf) natsArch='arm6'; sha256='918ee03dbc6ab17339f7510940945cdbb07fb15e5599b08961b17e732de0308e' ;; 		armv7) natsArch='arm7'; sha256='2de2669cd17d8c5ad118d7b1b45dbf84fd2ea2baad728cca971df09715086760' ;; 		x86_64) natsArch='amd64'; sha256='7f8f9397247ed5c69eb1ecee25ef5181be822eb85645451389f11dfc9680ed6e' ;; 		x86) natsArch='386'; sha256='dc8793a9778fecd44d71837ecd52174aec79d2115eb895373cc9dd7797d8b6a0' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 30 Sep 2022 00:24:35 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 30 Sep 2022 00:24:35 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 30 Sep 2022 00:24:35 GMT
EXPOSE 4222 6222 8222
# Fri, 30 Sep 2022 00:24:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 30 Sep 2022 00:24:35 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf1cfb9d9ea4605961cdb87b6f9e44cdcfdf68501e6502197a61ba80d7fa2cf3`  
		Last Modified: Fri, 30 Sep 2022 00:25:27 GMT  
		Size: 5.2 MB (5191367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f19aac431077ee9634be9f5879d95e018b853fe9f4355edfb009578928af4a8b`  
		Last Modified: Fri, 30 Sep 2022 00:25:26 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d803ce9173785ad956d0980594d07b7c002d401ec4f7038696cea1a816f8eeba`  
		Last Modified: Fri, 30 Sep 2022 00:25:26 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:1b1b13874064770ee71ee054d372744f61509858d4e2f0e728f4f7e3d0c96979
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7569288 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca1a0478849efea10188e490a19d87485a7e44be7adeb5a71abc150e21ad71b4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:22 GMT
ADD file:e8733e8cc0a81e15ca4041760b6e27392c34171512d34405a9b262b1fff5c687 in / 
# Tue, 09 Aug 2022 17:49:22 GMT
CMD ["/bin/sh"]
# Fri, 30 Sep 2022 00:15:00 GMT
ENV NATS_SERVER=2.9.2
# Fri, 30 Sep 2022 00:15:03 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='a2c6ff2c7342198ed61136658310a8f3c336426b07062ed0a073c617ddf4b503' ;; 		armhf) natsArch='arm6'; sha256='918ee03dbc6ab17339f7510940945cdbb07fb15e5599b08961b17e732de0308e' ;; 		armv7) natsArch='arm7'; sha256='2de2669cd17d8c5ad118d7b1b45dbf84fd2ea2baad728cca971df09715086760' ;; 		x86_64) natsArch='amd64'; sha256='7f8f9397247ed5c69eb1ecee25ef5181be822eb85645451389f11dfc9680ed6e' ;; 		x86) natsArch='386'; sha256='dc8793a9778fecd44d71837ecd52174aec79d2115eb895373cc9dd7797d8b6a0' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 30 Sep 2022 00:15:03 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 30 Sep 2022 00:15:03 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 30 Sep 2022 00:15:03 GMT
EXPOSE 4222 6222 8222
# Fri, 30 Sep 2022 00:15:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 30 Sep 2022 00:15:03 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9506b835437abb4d8ba1683e00c500b8f77e1975e930b356fbb72f2dbdc274d9`  
		Last Modified: Tue, 09 Aug 2022 17:50:33 GMT  
		Size: 2.6 MB (2613965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70e3a299d439ca160a2da5bc72a2fbdfe0d669e0251c6c9ca166ab1f6572234f`  
		Last Modified: Fri, 30 Sep 2022 00:16:18 GMT  
		Size: 5.0 MB (4954323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c2c24ad6cbf82b17aa717ce52a3630fce897bdc317f1cd90fa28a0b18ec0132`  
		Last Modified: Fri, 30 Sep 2022 00:16:17 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8569952349d4aaee564b407fc4a769f8afee1973b746dbc535f7ec1d82ee711f`  
		Last Modified: Fri, 30 Sep 2022 00:16:17 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:2acfd2cdc64cbd116f1f26fd834f476761f9bd485105fc5e9bf4e56596077414
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.4 MB (7369328 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:71027a1b3accd3e7e548dd995f0f20adb3aac785ca9a3f8e122b085367eef6be`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 16:57:44 GMT
ADD file:75521fe16320b193092588f6f31052c85e736965ceb11673de18bd14965a45e6 in / 
# Tue, 09 Aug 2022 16:57:44 GMT
CMD ["/bin/sh"]
# Fri, 30 Sep 2022 12:21:21 GMT
ENV NATS_SERVER=2.9.2
# Fri, 30 Sep 2022 12:21:23 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='a2c6ff2c7342198ed61136658310a8f3c336426b07062ed0a073c617ddf4b503' ;; 		armhf) natsArch='arm6'; sha256='918ee03dbc6ab17339f7510940945cdbb07fb15e5599b08961b17e732de0308e' ;; 		armv7) natsArch='arm7'; sha256='2de2669cd17d8c5ad118d7b1b45dbf84fd2ea2baad728cca971df09715086760' ;; 		x86_64) natsArch='amd64'; sha256='7f8f9397247ed5c69eb1ecee25ef5181be822eb85645451389f11dfc9680ed6e' ;; 		x86) natsArch='386'; sha256='dc8793a9778fecd44d71837ecd52174aec79d2115eb895373cc9dd7797d8b6a0' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 30 Sep 2022 12:21:23 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 30 Sep 2022 12:21:23 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 30 Sep 2022 12:21:23 GMT
EXPOSE 4222 6222 8222
# Fri, 30 Sep 2022 12:21:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 30 Sep 2022 12:21:23 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:c6556b3b6858c6fa1e328377cc2c4becdc9cd1bc3e7302aa7299936522cf93ba`  
		Last Modified: Tue, 09 Aug 2022 16:58:55 GMT  
		Size: 2.4 MB (2417065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce37993864155926f403118474bfe7f519e53160887c3676f0cb079b2da279fd`  
		Last Modified: Fri, 30 Sep 2022 12:22:41 GMT  
		Size: 5.0 MB (4951267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:404500b58d5dc1fd3cb248fe12df440b55e9c3ab7d8671bd898e861be2f61927`  
		Last Modified: Fri, 30 Sep 2022 12:22:40 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04c6d22f211806f08bc6bc9690b5aff62e8fd42fe73b976a1d18dee96b17d9eb`  
		Last Modified: Fri, 30 Sep 2022 12:22:40 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:63f1ff386adae53c49382ca5b6587c2dea35fc1af28e97033450cae49cfdcdab
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.5 MB (7485211 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6bf9a9bbea015857fed1ac343d2011fbc4ad3bfdc076c1963bd616875d0e0c88`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Fri, 30 Sep 2022 01:49:52 GMT
ENV NATS_SERVER=2.9.2
# Fri, 30 Sep 2022 01:49:55 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='a2c6ff2c7342198ed61136658310a8f3c336426b07062ed0a073c617ddf4b503' ;; 		armhf) natsArch='arm6'; sha256='918ee03dbc6ab17339f7510940945cdbb07fb15e5599b08961b17e732de0308e' ;; 		armv7) natsArch='arm7'; sha256='2de2669cd17d8c5ad118d7b1b45dbf84fd2ea2baad728cca971df09715086760' ;; 		x86_64) natsArch='amd64'; sha256='7f8f9397247ed5c69eb1ecee25ef5181be822eb85645451389f11dfc9680ed6e' ;; 		x86) natsArch='386'; sha256='dc8793a9778fecd44d71837ecd52174aec79d2115eb895373cc9dd7797d8b6a0' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 30 Sep 2022 01:49:57 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 30 Sep 2022 01:49:58 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 30 Sep 2022 01:49:58 GMT
EXPOSE 4222 6222 8222
# Fri, 30 Sep 2022 01:49:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 30 Sep 2022 01:50:00 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e30b79a866266b8c14d92afcced6bb4ffc32f152bafd6a4725eb24f2e5308da`  
		Last Modified: Fri, 30 Sep 2022 01:51:03 GMT  
		Size: 4.8 MB (4776577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d4ccb803f2d84c949447676b42f6b097337ce63fc73b9ff1b71715829193bb3`  
		Last Modified: Fri, 30 Sep 2022 01:51:02 GMT  
		Size: 559.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3baeeddb056b5f80c9eaf6dea17b085fd4b29d71b71ab6a68165224637f280da`  
		Last Modified: Fri, 30 Sep 2022 01:51:02 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-alpine3.16`

```console
$ docker pull nats@sha256:7b0816d59fbc8f00c834f53bc067bdbb35f27b79cef23e555ecd98496c9c9420
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9-alpine3.16` - linux; amd64

```console
$ docker pull nats@sha256:93b6c178034659b624ec39316bec9daeb14b38f690a531eaf5687c8f9a6420f6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.0 MB (7998419 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5068a20fcd0f44c75cc992b50a0c9406d62900af1d7756407b98f67a5aff6049`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Fri, 30 Sep 2022 00:24:33 GMT
ENV NATS_SERVER=2.9.2
# Fri, 30 Sep 2022 00:24:35 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='a2c6ff2c7342198ed61136658310a8f3c336426b07062ed0a073c617ddf4b503' ;; 		armhf) natsArch='arm6'; sha256='918ee03dbc6ab17339f7510940945cdbb07fb15e5599b08961b17e732de0308e' ;; 		armv7) natsArch='arm7'; sha256='2de2669cd17d8c5ad118d7b1b45dbf84fd2ea2baad728cca971df09715086760' ;; 		x86_64) natsArch='amd64'; sha256='7f8f9397247ed5c69eb1ecee25ef5181be822eb85645451389f11dfc9680ed6e' ;; 		x86) natsArch='386'; sha256='dc8793a9778fecd44d71837ecd52174aec79d2115eb895373cc9dd7797d8b6a0' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 30 Sep 2022 00:24:35 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 30 Sep 2022 00:24:35 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 30 Sep 2022 00:24:35 GMT
EXPOSE 4222 6222 8222
# Fri, 30 Sep 2022 00:24:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 30 Sep 2022 00:24:35 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf1cfb9d9ea4605961cdb87b6f9e44cdcfdf68501e6502197a61ba80d7fa2cf3`  
		Last Modified: Fri, 30 Sep 2022 00:25:27 GMT  
		Size: 5.2 MB (5191367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f19aac431077ee9634be9f5879d95e018b853fe9f4355edfb009578928af4a8b`  
		Last Modified: Fri, 30 Sep 2022 00:25:26 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d803ce9173785ad956d0980594d07b7c002d401ec4f7038696cea1a816f8eeba`  
		Last Modified: Fri, 30 Sep 2022 00:25:26 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-alpine3.16` - linux; arm variant v6

```console
$ docker pull nats@sha256:1b1b13874064770ee71ee054d372744f61509858d4e2f0e728f4f7e3d0c96979
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7569288 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca1a0478849efea10188e490a19d87485a7e44be7adeb5a71abc150e21ad71b4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:22 GMT
ADD file:e8733e8cc0a81e15ca4041760b6e27392c34171512d34405a9b262b1fff5c687 in / 
# Tue, 09 Aug 2022 17:49:22 GMT
CMD ["/bin/sh"]
# Fri, 30 Sep 2022 00:15:00 GMT
ENV NATS_SERVER=2.9.2
# Fri, 30 Sep 2022 00:15:03 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='a2c6ff2c7342198ed61136658310a8f3c336426b07062ed0a073c617ddf4b503' ;; 		armhf) natsArch='arm6'; sha256='918ee03dbc6ab17339f7510940945cdbb07fb15e5599b08961b17e732de0308e' ;; 		armv7) natsArch='arm7'; sha256='2de2669cd17d8c5ad118d7b1b45dbf84fd2ea2baad728cca971df09715086760' ;; 		x86_64) natsArch='amd64'; sha256='7f8f9397247ed5c69eb1ecee25ef5181be822eb85645451389f11dfc9680ed6e' ;; 		x86) natsArch='386'; sha256='dc8793a9778fecd44d71837ecd52174aec79d2115eb895373cc9dd7797d8b6a0' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 30 Sep 2022 00:15:03 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 30 Sep 2022 00:15:03 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 30 Sep 2022 00:15:03 GMT
EXPOSE 4222 6222 8222
# Fri, 30 Sep 2022 00:15:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 30 Sep 2022 00:15:03 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9506b835437abb4d8ba1683e00c500b8f77e1975e930b356fbb72f2dbdc274d9`  
		Last Modified: Tue, 09 Aug 2022 17:50:33 GMT  
		Size: 2.6 MB (2613965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70e3a299d439ca160a2da5bc72a2fbdfe0d669e0251c6c9ca166ab1f6572234f`  
		Last Modified: Fri, 30 Sep 2022 00:16:18 GMT  
		Size: 5.0 MB (4954323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c2c24ad6cbf82b17aa717ce52a3630fce897bdc317f1cd90fa28a0b18ec0132`  
		Last Modified: Fri, 30 Sep 2022 00:16:17 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8569952349d4aaee564b407fc4a769f8afee1973b746dbc535f7ec1d82ee711f`  
		Last Modified: Fri, 30 Sep 2022 00:16:17 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-alpine3.16` - linux; arm variant v7

```console
$ docker pull nats@sha256:2acfd2cdc64cbd116f1f26fd834f476761f9bd485105fc5e9bf4e56596077414
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.4 MB (7369328 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:71027a1b3accd3e7e548dd995f0f20adb3aac785ca9a3f8e122b085367eef6be`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 16:57:44 GMT
ADD file:75521fe16320b193092588f6f31052c85e736965ceb11673de18bd14965a45e6 in / 
# Tue, 09 Aug 2022 16:57:44 GMT
CMD ["/bin/sh"]
# Fri, 30 Sep 2022 12:21:21 GMT
ENV NATS_SERVER=2.9.2
# Fri, 30 Sep 2022 12:21:23 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='a2c6ff2c7342198ed61136658310a8f3c336426b07062ed0a073c617ddf4b503' ;; 		armhf) natsArch='arm6'; sha256='918ee03dbc6ab17339f7510940945cdbb07fb15e5599b08961b17e732de0308e' ;; 		armv7) natsArch='arm7'; sha256='2de2669cd17d8c5ad118d7b1b45dbf84fd2ea2baad728cca971df09715086760' ;; 		x86_64) natsArch='amd64'; sha256='7f8f9397247ed5c69eb1ecee25ef5181be822eb85645451389f11dfc9680ed6e' ;; 		x86) natsArch='386'; sha256='dc8793a9778fecd44d71837ecd52174aec79d2115eb895373cc9dd7797d8b6a0' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 30 Sep 2022 12:21:23 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 30 Sep 2022 12:21:23 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 30 Sep 2022 12:21:23 GMT
EXPOSE 4222 6222 8222
# Fri, 30 Sep 2022 12:21:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 30 Sep 2022 12:21:23 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:c6556b3b6858c6fa1e328377cc2c4becdc9cd1bc3e7302aa7299936522cf93ba`  
		Last Modified: Tue, 09 Aug 2022 16:58:55 GMT  
		Size: 2.4 MB (2417065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce37993864155926f403118474bfe7f519e53160887c3676f0cb079b2da279fd`  
		Last Modified: Fri, 30 Sep 2022 12:22:41 GMT  
		Size: 5.0 MB (4951267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:404500b58d5dc1fd3cb248fe12df440b55e9c3ab7d8671bd898e861be2f61927`  
		Last Modified: Fri, 30 Sep 2022 12:22:40 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04c6d22f211806f08bc6bc9690b5aff62e8fd42fe73b976a1d18dee96b17d9eb`  
		Last Modified: Fri, 30 Sep 2022 12:22:40 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-alpine3.16` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:63f1ff386adae53c49382ca5b6587c2dea35fc1af28e97033450cae49cfdcdab
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.5 MB (7485211 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6bf9a9bbea015857fed1ac343d2011fbc4ad3bfdc076c1963bd616875d0e0c88`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Fri, 30 Sep 2022 01:49:52 GMT
ENV NATS_SERVER=2.9.2
# Fri, 30 Sep 2022 01:49:55 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='a2c6ff2c7342198ed61136658310a8f3c336426b07062ed0a073c617ddf4b503' ;; 		armhf) natsArch='arm6'; sha256='918ee03dbc6ab17339f7510940945cdbb07fb15e5599b08961b17e732de0308e' ;; 		armv7) natsArch='arm7'; sha256='2de2669cd17d8c5ad118d7b1b45dbf84fd2ea2baad728cca971df09715086760' ;; 		x86_64) natsArch='amd64'; sha256='7f8f9397247ed5c69eb1ecee25ef5181be822eb85645451389f11dfc9680ed6e' ;; 		x86) natsArch='386'; sha256='dc8793a9778fecd44d71837ecd52174aec79d2115eb895373cc9dd7797d8b6a0' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 30 Sep 2022 01:49:57 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 30 Sep 2022 01:49:58 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 30 Sep 2022 01:49:58 GMT
EXPOSE 4222 6222 8222
# Fri, 30 Sep 2022 01:49:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 30 Sep 2022 01:50:00 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e30b79a866266b8c14d92afcced6bb4ffc32f152bafd6a4725eb24f2e5308da`  
		Last Modified: Fri, 30 Sep 2022 01:51:03 GMT  
		Size: 4.8 MB (4776577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d4ccb803f2d84c949447676b42f6b097337ce63fc73b9ff1b71715829193bb3`  
		Last Modified: Fri, 30 Sep 2022 01:51:02 GMT  
		Size: 559.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3baeeddb056b5f80c9eaf6dea17b085fd4b29d71b71ab6a68165224637f280da`  
		Last Modified: Fri, 30 Sep 2022 01:51:02 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-linux`

```console
$ docker pull nats@sha256:5f9faa293f743a8c78944dc1827132cc658e8ffcb2746d00e6ea69316a9fe3d9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9-linux` - linux; amd64

```console
$ docker pull nats@sha256:73a511425369d8e883fc5784023028b7ed02c252e6db030e776b2e6a76bb90ca
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4907513 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf3ba31eb02c938f2ab28c2b60358ef903503ce4a2fb5e2df6f4714d04e74619`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 30 Sep 2022 00:25:01 GMT
COPY file:ef7d265008705c7f8da964d29a2883d21303aab4d4520c3327ca6ce57348e137 in /nats-server 
# Fri, 30 Sep 2022 00:25:01 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 30 Sep 2022 00:25:01 GMT
EXPOSE 4222 6222 8222
# Fri, 30 Sep 2022 00:25:01 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 30 Sep 2022 00:25:01 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 30 Sep 2022 00:25:01 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:325d5a714be1f0303eebb8d34c9b23e1b15c5e7e46eb29d0f90511112fb86894`  
		Last Modified: Fri, 30 Sep 2022 00:25:50 GMT  
		Size: 4.9 MB (4907005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06b03a363308e84c4fc60d5ac2d5b9374e811456edecdb1e302e59198bfb1ca4`  
		Last Modified: Fri, 30 Sep 2022 00:25:49 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:22be654fd606d7db5e28383ce35794c881f25b77908c6f981c2442b117d7df19
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4671534 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1eeeee00c7520737eb3766018dde7f3dd63c971938d98ff49cca225f0e6c6990`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 30 Sep 2022 00:15:17 GMT
COPY file:2de52eed8721a4ef1e4c8adb2f046a7ffa8e689d614c704b329ef2bafc7dfe5c in /nats-server 
# Fri, 30 Sep 2022 00:15:17 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 30 Sep 2022 00:15:17 GMT
EXPOSE 4222 6222 8222
# Fri, 30 Sep 2022 00:15:18 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 30 Sep 2022 00:15:18 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 30 Sep 2022 00:15:18 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:948e55d9b8c745ce1f9007c64a6da65d66c0d554fa7e5808a04081a1d0754a6c`  
		Last Modified: Fri, 30 Sep 2022 00:16:49 GMT  
		Size: 4.7 MB (4671025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14bdee3fcf17688810034aff56b746397e799579ff11654f2a2ec59274a9e161`  
		Last Modified: Fri, 30 Sep 2022 00:16:48 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:dce0b0ef268b27c6417ee879c4f500273d8eabe0f3347ed2ac19b28a166085e2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4661683 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93f043be0120df37adc5618c50a4eb09f405d9a23f0794314f36c76be8bda597`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 30 Sep 2022 12:21:44 GMT
COPY file:e57d6f6c709cd7f891a48782c812655546ed7ed7194710fb4ff95d3225a8cb24 in /nats-server 
# Fri, 30 Sep 2022 12:21:44 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 30 Sep 2022 12:21:44 GMT
EXPOSE 4222 6222 8222
# Fri, 30 Sep 2022 12:21:44 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 30 Sep 2022 12:21:44 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 30 Sep 2022 12:21:44 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6709a2d5812e1f5aabc828977b23e9033fb28dd6d79bad682b986bfeaf468265`  
		Last Modified: Fri, 30 Sep 2022 12:23:13 GMT  
		Size: 4.7 MB (4661175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:913a6877bd39f71d19820c3493253d22c565656c7058ca6e5deb8e20280f8ad6`  
		Last Modified: Fri, 30 Sep 2022 12:23:12 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:6d0d5cfcf4b908ca419719473183dd4000ebe2e77e9fb1088f51f2195324d865
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4495540 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7069cf895c76381ff91ad174ed58ca07743ca741317f4a2c20ea3b1f1bae44ce`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 30 Sep 2022 01:50:11 GMT
COPY file:06300839e6ae56288247488999d2e96ee71c9bb64453bfa88faa4cbfc85a23e2 in /nats-server 
# Fri, 30 Sep 2022 01:50:12 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 30 Sep 2022 01:50:12 GMT
EXPOSE 4222 6222 8222
# Fri, 30 Sep 2022 01:50:13 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 30 Sep 2022 01:50:14 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 30 Sep 2022 01:50:15 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:71fcb6de35d4d1378bd805b642a59de493c8957d351b1f521d05492db21c54d6`  
		Last Modified: Fri, 30 Sep 2022 01:51:31 GMT  
		Size: 4.5 MB (4495032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3be89d1242837970f7157774c5188f9046677dfb8c676155f7b2d268758d504`  
		Last Modified: Fri, 30 Sep 2022 01:51:30 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-nanoserver`

```console
$ docker pull nats@sha256:679b0d8e5bafa2c6893078adf595ebd301d9df9258ca22d088788c40d6ca5d28
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3406; amd64

### `nats:2.9-nanoserver` - windows version 10.0.17763.3406; amd64

```console
$ docker pull nats@sha256:2861931a21dd96bdbd1686faf3a14c6927dc24203b8c04d30b2116ef4d670e64
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **108.3 MB (108299212 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc0fee332755f830a4cef70df70da46a2cb2c28daadd327e68b97dbf22b35166`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 09 Sep 2022 22:22:51 GMT
RUN Apply image 10.0.17763.3406
# Wed, 14 Sep 2022 15:41:36 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 30 Sep 2022 00:18:47 GMT
RUN cmd /S /C #(nop) COPY file:da89208003aed19cb9852334329c2f8b4dfdfe3218c3f05bba8fcb3247acc400 in C:\nats-server.exe 
# Fri, 30 Sep 2022 00:18:48 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Fri, 30 Sep 2022 00:18:49 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Fri, 30 Sep 2022 00:18:50 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 30 Sep 2022 00:18:51 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:bcd4ab6c304faa0a7f4e183705a7f6e4545b728788221d17886d2a507ea0a06d`  
		Size: 103.3 MB (103334221 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b6bda313a93b8c355d5adf6e15f4b805f705c3741b235a7e4644bbffe6a6af3d`  
		Last Modified: Wed, 14 Sep 2022 15:42:30 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c046270960bff604e9be6498c1c0ee8367958198004e91286a8252366f7185c`  
		Last Modified: Fri, 30 Sep 2022 00:19:41 GMT  
		Size: 5.0 MB (4958572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1087232c1623e24e6883cc4c33bb9ff4926cfc24df9f4909f09db53185f2fe15`  
		Last Modified: Fri, 30 Sep 2022 00:19:40 GMT  
		Size: 1.8 KB (1774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83e77ee18b12423f469199b766a08c031324d15169a9f2e690bf77ccbb796ecd`  
		Last Modified: Fri, 30 Sep 2022 00:19:40 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4549b9baa74eb7ff07539b979f0966c66afb35858810779ec9d7572da5777e49`  
		Last Modified: Fri, 30 Sep 2022 00:19:40 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ee9032ad08c565fc85469a687bbaddfa40a6066692a113da46c758c5d591e4a`  
		Last Modified: Fri, 30 Sep 2022 00:19:40 GMT  
		Size: 1.2 KB (1176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-nanoserver-1809`

```console
$ docker pull nats@sha256:679b0d8e5bafa2c6893078adf595ebd301d9df9258ca22d088788c40d6ca5d28
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3406; amd64

### `nats:2.9-nanoserver-1809` - windows version 10.0.17763.3406; amd64

```console
$ docker pull nats@sha256:2861931a21dd96bdbd1686faf3a14c6927dc24203b8c04d30b2116ef4d670e64
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **108.3 MB (108299212 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc0fee332755f830a4cef70df70da46a2cb2c28daadd327e68b97dbf22b35166`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 09 Sep 2022 22:22:51 GMT
RUN Apply image 10.0.17763.3406
# Wed, 14 Sep 2022 15:41:36 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 30 Sep 2022 00:18:47 GMT
RUN cmd /S /C #(nop) COPY file:da89208003aed19cb9852334329c2f8b4dfdfe3218c3f05bba8fcb3247acc400 in C:\nats-server.exe 
# Fri, 30 Sep 2022 00:18:48 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Fri, 30 Sep 2022 00:18:49 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Fri, 30 Sep 2022 00:18:50 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 30 Sep 2022 00:18:51 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:bcd4ab6c304faa0a7f4e183705a7f6e4545b728788221d17886d2a507ea0a06d`  
		Size: 103.3 MB (103334221 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b6bda313a93b8c355d5adf6e15f4b805f705c3741b235a7e4644bbffe6a6af3d`  
		Last Modified: Wed, 14 Sep 2022 15:42:30 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c046270960bff604e9be6498c1c0ee8367958198004e91286a8252366f7185c`  
		Last Modified: Fri, 30 Sep 2022 00:19:41 GMT  
		Size: 5.0 MB (4958572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1087232c1623e24e6883cc4c33bb9ff4926cfc24df9f4909f09db53185f2fe15`  
		Last Modified: Fri, 30 Sep 2022 00:19:40 GMT  
		Size: 1.8 KB (1774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83e77ee18b12423f469199b766a08c031324d15169a9f2e690bf77ccbb796ecd`  
		Last Modified: Fri, 30 Sep 2022 00:19:40 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4549b9baa74eb7ff07539b979f0966c66afb35858810779ec9d7572da5777e49`  
		Last Modified: Fri, 30 Sep 2022 00:19:40 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ee9032ad08c565fc85469a687bbaddfa40a6066692a113da46c758c5d591e4a`  
		Last Modified: Fri, 30 Sep 2022 00:19:40 GMT  
		Size: 1.2 KB (1176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-scratch`

```console
$ docker pull nats@sha256:5f9faa293f743a8c78944dc1827132cc658e8ffcb2746d00e6ea69316a9fe3d9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9-scratch` - linux; amd64

```console
$ docker pull nats@sha256:73a511425369d8e883fc5784023028b7ed02c252e6db030e776b2e6a76bb90ca
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4907513 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf3ba31eb02c938f2ab28c2b60358ef903503ce4a2fb5e2df6f4714d04e74619`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 30 Sep 2022 00:25:01 GMT
COPY file:ef7d265008705c7f8da964d29a2883d21303aab4d4520c3327ca6ce57348e137 in /nats-server 
# Fri, 30 Sep 2022 00:25:01 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 30 Sep 2022 00:25:01 GMT
EXPOSE 4222 6222 8222
# Fri, 30 Sep 2022 00:25:01 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 30 Sep 2022 00:25:01 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 30 Sep 2022 00:25:01 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:325d5a714be1f0303eebb8d34c9b23e1b15c5e7e46eb29d0f90511112fb86894`  
		Last Modified: Fri, 30 Sep 2022 00:25:50 GMT  
		Size: 4.9 MB (4907005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06b03a363308e84c4fc60d5ac2d5b9374e811456edecdb1e302e59198bfb1ca4`  
		Last Modified: Fri, 30 Sep 2022 00:25:49 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:22be654fd606d7db5e28383ce35794c881f25b77908c6f981c2442b117d7df19
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4671534 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1eeeee00c7520737eb3766018dde7f3dd63c971938d98ff49cca225f0e6c6990`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 30 Sep 2022 00:15:17 GMT
COPY file:2de52eed8721a4ef1e4c8adb2f046a7ffa8e689d614c704b329ef2bafc7dfe5c in /nats-server 
# Fri, 30 Sep 2022 00:15:17 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 30 Sep 2022 00:15:17 GMT
EXPOSE 4222 6222 8222
# Fri, 30 Sep 2022 00:15:18 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 30 Sep 2022 00:15:18 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 30 Sep 2022 00:15:18 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:948e55d9b8c745ce1f9007c64a6da65d66c0d554fa7e5808a04081a1d0754a6c`  
		Last Modified: Fri, 30 Sep 2022 00:16:49 GMT  
		Size: 4.7 MB (4671025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14bdee3fcf17688810034aff56b746397e799579ff11654f2a2ec59274a9e161`  
		Last Modified: Fri, 30 Sep 2022 00:16:48 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:dce0b0ef268b27c6417ee879c4f500273d8eabe0f3347ed2ac19b28a166085e2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4661683 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93f043be0120df37adc5618c50a4eb09f405d9a23f0794314f36c76be8bda597`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 30 Sep 2022 12:21:44 GMT
COPY file:e57d6f6c709cd7f891a48782c812655546ed7ed7194710fb4ff95d3225a8cb24 in /nats-server 
# Fri, 30 Sep 2022 12:21:44 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 30 Sep 2022 12:21:44 GMT
EXPOSE 4222 6222 8222
# Fri, 30 Sep 2022 12:21:44 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 30 Sep 2022 12:21:44 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 30 Sep 2022 12:21:44 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6709a2d5812e1f5aabc828977b23e9033fb28dd6d79bad682b986bfeaf468265`  
		Last Modified: Fri, 30 Sep 2022 12:23:13 GMT  
		Size: 4.7 MB (4661175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:913a6877bd39f71d19820c3493253d22c565656c7058ca6e5deb8e20280f8ad6`  
		Last Modified: Fri, 30 Sep 2022 12:23:12 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:6d0d5cfcf4b908ca419719473183dd4000ebe2e77e9fb1088f51f2195324d865
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4495540 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7069cf895c76381ff91ad174ed58ca07743ca741317f4a2c20ea3b1f1bae44ce`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 30 Sep 2022 01:50:11 GMT
COPY file:06300839e6ae56288247488999d2e96ee71c9bb64453bfa88faa4cbfc85a23e2 in /nats-server 
# Fri, 30 Sep 2022 01:50:12 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 30 Sep 2022 01:50:12 GMT
EXPOSE 4222 6222 8222
# Fri, 30 Sep 2022 01:50:13 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 30 Sep 2022 01:50:14 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 30 Sep 2022 01:50:15 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:71fcb6de35d4d1378bd805b642a59de493c8957d351b1f521d05492db21c54d6`  
		Last Modified: Fri, 30 Sep 2022 01:51:31 GMT  
		Size: 4.5 MB (4495032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3be89d1242837970f7157774c5188f9046677dfb8c676155f7b2d268758d504`  
		Last Modified: Fri, 30 Sep 2022 01:51:30 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-windowsservercore`

```console
$ docker pull nats@sha256:3357d7889ebcb10a163ba56eff66f60ff010e161b38e1f401cc136e7a6879baf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3406; amd64

### `nats:2.9-windowsservercore` - windows version 10.0.17763.3406; amd64

```console
$ docker pull nats@sha256:214e04a7dc77ff783ac336d010ba64eb98f2c8722d522260bf340c2df3d521e7
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2709236645 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:30cb30cff6676167599e8b4fd9f6b053b3e6fa2f5418a7a419e631956a014e9e`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Fri, 09 Sep 2022 22:43:02 GMT
RUN Install update 10.0.17763.3406
# Wed, 14 Sep 2022 13:39:18 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 14 Sep 2022 15:38:54 GMT
ENV NATS_DOCKERIZED=1
# Fri, 30 Sep 2022 00:15:50 GMT
ENV NATS_SERVER=2.9.2
# Fri, 30 Sep 2022 00:15:51 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.9.2/nats-server-v2.9.2-windows-amd64.zip
# Fri, 30 Sep 2022 00:15:52 GMT
ENV NATS_SERVER_SHASUM=cd3d2a9d78c235292afc27f812baee7817180fcfe5ebba662e72f0cc821d04fb
# Fri, 30 Sep 2022 00:16:59 GMT
RUN Set-PSDebug -Trace 2
# Fri, 30 Sep 2022 00:18:30 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 30 Sep 2022 00:18:31 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Fri, 30 Sep 2022 00:18:31 GMT
EXPOSE 4222 6222 8222
# Fri, 30 Sep 2022 00:18:32 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 30 Sep 2022 00:18:33 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:cee64bf279e2ca8e924884a10ecb98bfa79c7f0cc8d25e73039b9aeb940815b6`  
		Size: 826.4 MB (826398623 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3c428406510f0a47ed60f28060a7d625d42344a95fdcb7c4f5746fb8857c3328`  
		Last Modified: Wed, 14 Sep 2022 15:42:13 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf4bba85c5cc970a66b01ed6f4cabffa7705a0bdbc18907894f94c09b5ee2618`  
		Last Modified: Wed, 14 Sep 2022 15:42:12 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a29319534b1836908aab29077ce165236693f20e5abbb69a70639c6cce19223b`  
		Last Modified: Fri, 30 Sep 2022 00:19:24 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d34f7b3a98b75cbb6f21f33118a7f43b9efe7d7d8ef5d9f47b5ca73470abd339`  
		Last Modified: Fri, 30 Sep 2022 00:19:24 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2119397eb3051d4784ced2882a1c0f1d2995cec67f5954fd5f33fde4b6ab4c3a`  
		Last Modified: Fri, 30 Sep 2022 00:19:24 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cdecf001ef7e4a9db54aa1a639bf5036f69cfc71a2d6b1b9089c1a3810373aa`  
		Last Modified: Fri, 30 Sep 2022 00:19:24 GMT  
		Size: 358.1 KB (358089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4a5a2ffe352520814f5794422903ec9e717d37294931ca81f856257a419ee1f`  
		Last Modified: Fri, 30 Sep 2022 00:19:23 GMT  
		Size: 5.3 MB (5300456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b80c11ae75a170747a9206d993fe059c9cda9f34c08c9f2eb90bedaef90f322e`  
		Last Modified: Fri, 30 Sep 2022 00:19:22 GMT  
		Size: 2.0 KB (2012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e8020be63ec6ec39f4443bc78e114caf9c24c5686fcf3f84a8c74f38f61b864`  
		Last Modified: Fri, 30 Sep 2022 00:19:22 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50d3d068429b4966cc13e153bdbf220b0259eb72a6a3f507fc5172a963499566`  
		Last Modified: Fri, 30 Sep 2022 00:19:22 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f588edee9a48a943744711d7d4dea00d9e842180f05a759c2edf3e50ee10e06c`  
		Last Modified: Fri, 30 Sep 2022 00:19:22 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-windowsservercore-1809`

```console
$ docker pull nats@sha256:3357d7889ebcb10a163ba56eff66f60ff010e161b38e1f401cc136e7a6879baf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3406; amd64

### `nats:2.9-windowsservercore-1809` - windows version 10.0.17763.3406; amd64

```console
$ docker pull nats@sha256:214e04a7dc77ff783ac336d010ba64eb98f2c8722d522260bf340c2df3d521e7
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2709236645 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:30cb30cff6676167599e8b4fd9f6b053b3e6fa2f5418a7a419e631956a014e9e`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Fri, 09 Sep 2022 22:43:02 GMT
RUN Install update 10.0.17763.3406
# Wed, 14 Sep 2022 13:39:18 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 14 Sep 2022 15:38:54 GMT
ENV NATS_DOCKERIZED=1
# Fri, 30 Sep 2022 00:15:50 GMT
ENV NATS_SERVER=2.9.2
# Fri, 30 Sep 2022 00:15:51 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.9.2/nats-server-v2.9.2-windows-amd64.zip
# Fri, 30 Sep 2022 00:15:52 GMT
ENV NATS_SERVER_SHASUM=cd3d2a9d78c235292afc27f812baee7817180fcfe5ebba662e72f0cc821d04fb
# Fri, 30 Sep 2022 00:16:59 GMT
RUN Set-PSDebug -Trace 2
# Fri, 30 Sep 2022 00:18:30 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 30 Sep 2022 00:18:31 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Fri, 30 Sep 2022 00:18:31 GMT
EXPOSE 4222 6222 8222
# Fri, 30 Sep 2022 00:18:32 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 30 Sep 2022 00:18:33 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:cee64bf279e2ca8e924884a10ecb98bfa79c7f0cc8d25e73039b9aeb940815b6`  
		Size: 826.4 MB (826398623 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3c428406510f0a47ed60f28060a7d625d42344a95fdcb7c4f5746fb8857c3328`  
		Last Modified: Wed, 14 Sep 2022 15:42:13 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf4bba85c5cc970a66b01ed6f4cabffa7705a0bdbc18907894f94c09b5ee2618`  
		Last Modified: Wed, 14 Sep 2022 15:42:12 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a29319534b1836908aab29077ce165236693f20e5abbb69a70639c6cce19223b`  
		Last Modified: Fri, 30 Sep 2022 00:19:24 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d34f7b3a98b75cbb6f21f33118a7f43b9efe7d7d8ef5d9f47b5ca73470abd339`  
		Last Modified: Fri, 30 Sep 2022 00:19:24 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2119397eb3051d4784ced2882a1c0f1d2995cec67f5954fd5f33fde4b6ab4c3a`  
		Last Modified: Fri, 30 Sep 2022 00:19:24 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cdecf001ef7e4a9db54aa1a639bf5036f69cfc71a2d6b1b9089c1a3810373aa`  
		Last Modified: Fri, 30 Sep 2022 00:19:24 GMT  
		Size: 358.1 KB (358089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4a5a2ffe352520814f5794422903ec9e717d37294931ca81f856257a419ee1f`  
		Last Modified: Fri, 30 Sep 2022 00:19:23 GMT  
		Size: 5.3 MB (5300456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b80c11ae75a170747a9206d993fe059c9cda9f34c08c9f2eb90bedaef90f322e`  
		Last Modified: Fri, 30 Sep 2022 00:19:22 GMT  
		Size: 2.0 KB (2012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e8020be63ec6ec39f4443bc78e114caf9c24c5686fcf3f84a8c74f38f61b864`  
		Last Modified: Fri, 30 Sep 2022 00:19:22 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50d3d068429b4966cc13e153bdbf220b0259eb72a6a3f507fc5172a963499566`  
		Last Modified: Fri, 30 Sep 2022 00:19:22 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f588edee9a48a943744711d7d4dea00d9e842180f05a759c2edf3e50ee10e06c`  
		Last Modified: Fri, 30 Sep 2022 00:19:22 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.2`

```console
$ docker pull nats@sha256:2a333e9f7d50ba4dd450e435b65a5b038af6988ab4c19c858cf85c6733667c28
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.3406; amd64

### `nats:2.9.2` - linux; amd64

```console
$ docker pull nats@sha256:73a511425369d8e883fc5784023028b7ed02c252e6db030e776b2e6a76bb90ca
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4907513 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf3ba31eb02c938f2ab28c2b60358ef903503ce4a2fb5e2df6f4714d04e74619`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 30 Sep 2022 00:25:01 GMT
COPY file:ef7d265008705c7f8da964d29a2883d21303aab4d4520c3327ca6ce57348e137 in /nats-server 
# Fri, 30 Sep 2022 00:25:01 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 30 Sep 2022 00:25:01 GMT
EXPOSE 4222 6222 8222
# Fri, 30 Sep 2022 00:25:01 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 30 Sep 2022 00:25:01 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 30 Sep 2022 00:25:01 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:325d5a714be1f0303eebb8d34c9b23e1b15c5e7e46eb29d0f90511112fb86894`  
		Last Modified: Fri, 30 Sep 2022 00:25:50 GMT  
		Size: 4.9 MB (4907005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06b03a363308e84c4fc60d5ac2d5b9374e811456edecdb1e302e59198bfb1ca4`  
		Last Modified: Fri, 30 Sep 2022 00:25:49 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.2` - linux; arm variant v6

```console
$ docker pull nats@sha256:22be654fd606d7db5e28383ce35794c881f25b77908c6f981c2442b117d7df19
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4671534 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1eeeee00c7520737eb3766018dde7f3dd63c971938d98ff49cca225f0e6c6990`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 30 Sep 2022 00:15:17 GMT
COPY file:2de52eed8721a4ef1e4c8adb2f046a7ffa8e689d614c704b329ef2bafc7dfe5c in /nats-server 
# Fri, 30 Sep 2022 00:15:17 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 30 Sep 2022 00:15:17 GMT
EXPOSE 4222 6222 8222
# Fri, 30 Sep 2022 00:15:18 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 30 Sep 2022 00:15:18 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 30 Sep 2022 00:15:18 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:948e55d9b8c745ce1f9007c64a6da65d66c0d554fa7e5808a04081a1d0754a6c`  
		Last Modified: Fri, 30 Sep 2022 00:16:49 GMT  
		Size: 4.7 MB (4671025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14bdee3fcf17688810034aff56b746397e799579ff11654f2a2ec59274a9e161`  
		Last Modified: Fri, 30 Sep 2022 00:16:48 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.2` - linux; arm variant v7

```console
$ docker pull nats@sha256:dce0b0ef268b27c6417ee879c4f500273d8eabe0f3347ed2ac19b28a166085e2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4661683 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93f043be0120df37adc5618c50a4eb09f405d9a23f0794314f36c76be8bda597`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 30 Sep 2022 12:21:44 GMT
COPY file:e57d6f6c709cd7f891a48782c812655546ed7ed7194710fb4ff95d3225a8cb24 in /nats-server 
# Fri, 30 Sep 2022 12:21:44 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 30 Sep 2022 12:21:44 GMT
EXPOSE 4222 6222 8222
# Fri, 30 Sep 2022 12:21:44 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 30 Sep 2022 12:21:44 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 30 Sep 2022 12:21:44 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6709a2d5812e1f5aabc828977b23e9033fb28dd6d79bad682b986bfeaf468265`  
		Last Modified: Fri, 30 Sep 2022 12:23:13 GMT  
		Size: 4.7 MB (4661175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:913a6877bd39f71d19820c3493253d22c565656c7058ca6e5deb8e20280f8ad6`  
		Last Modified: Fri, 30 Sep 2022 12:23:12 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.2` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:6d0d5cfcf4b908ca419719473183dd4000ebe2e77e9fb1088f51f2195324d865
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4495540 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7069cf895c76381ff91ad174ed58ca07743ca741317f4a2c20ea3b1f1bae44ce`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 30 Sep 2022 01:50:11 GMT
COPY file:06300839e6ae56288247488999d2e96ee71c9bb64453bfa88faa4cbfc85a23e2 in /nats-server 
# Fri, 30 Sep 2022 01:50:12 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 30 Sep 2022 01:50:12 GMT
EXPOSE 4222 6222 8222
# Fri, 30 Sep 2022 01:50:13 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 30 Sep 2022 01:50:14 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 30 Sep 2022 01:50:15 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:71fcb6de35d4d1378bd805b642a59de493c8957d351b1f521d05492db21c54d6`  
		Last Modified: Fri, 30 Sep 2022 01:51:31 GMT  
		Size: 4.5 MB (4495032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3be89d1242837970f7157774c5188f9046677dfb8c676155f7b2d268758d504`  
		Last Modified: Fri, 30 Sep 2022 01:51:30 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.2` - windows version 10.0.17763.3406; amd64

```console
$ docker pull nats@sha256:2861931a21dd96bdbd1686faf3a14c6927dc24203b8c04d30b2116ef4d670e64
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **108.3 MB (108299212 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc0fee332755f830a4cef70df70da46a2cb2c28daadd327e68b97dbf22b35166`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 09 Sep 2022 22:22:51 GMT
RUN Apply image 10.0.17763.3406
# Wed, 14 Sep 2022 15:41:36 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 30 Sep 2022 00:18:47 GMT
RUN cmd /S /C #(nop) COPY file:da89208003aed19cb9852334329c2f8b4dfdfe3218c3f05bba8fcb3247acc400 in C:\nats-server.exe 
# Fri, 30 Sep 2022 00:18:48 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Fri, 30 Sep 2022 00:18:49 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Fri, 30 Sep 2022 00:18:50 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 30 Sep 2022 00:18:51 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:bcd4ab6c304faa0a7f4e183705a7f6e4545b728788221d17886d2a507ea0a06d`  
		Size: 103.3 MB (103334221 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b6bda313a93b8c355d5adf6e15f4b805f705c3741b235a7e4644bbffe6a6af3d`  
		Last Modified: Wed, 14 Sep 2022 15:42:30 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c046270960bff604e9be6498c1c0ee8367958198004e91286a8252366f7185c`  
		Last Modified: Fri, 30 Sep 2022 00:19:41 GMT  
		Size: 5.0 MB (4958572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1087232c1623e24e6883cc4c33bb9ff4926cfc24df9f4909f09db53185f2fe15`  
		Last Modified: Fri, 30 Sep 2022 00:19:40 GMT  
		Size: 1.8 KB (1774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83e77ee18b12423f469199b766a08c031324d15169a9f2e690bf77ccbb796ecd`  
		Last Modified: Fri, 30 Sep 2022 00:19:40 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4549b9baa74eb7ff07539b979f0966c66afb35858810779ec9d7572da5777e49`  
		Last Modified: Fri, 30 Sep 2022 00:19:40 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ee9032ad08c565fc85469a687bbaddfa40a6066692a113da46c758c5d591e4a`  
		Last Modified: Fri, 30 Sep 2022 00:19:40 GMT  
		Size: 1.2 KB (1176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.2-alpine`

```console
$ docker pull nats@sha256:7b0816d59fbc8f00c834f53bc067bdbb35f27b79cef23e555ecd98496c9c9420
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9.2-alpine` - linux; amd64

```console
$ docker pull nats@sha256:93b6c178034659b624ec39316bec9daeb14b38f690a531eaf5687c8f9a6420f6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.0 MB (7998419 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5068a20fcd0f44c75cc992b50a0c9406d62900af1d7756407b98f67a5aff6049`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Fri, 30 Sep 2022 00:24:33 GMT
ENV NATS_SERVER=2.9.2
# Fri, 30 Sep 2022 00:24:35 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='a2c6ff2c7342198ed61136658310a8f3c336426b07062ed0a073c617ddf4b503' ;; 		armhf) natsArch='arm6'; sha256='918ee03dbc6ab17339f7510940945cdbb07fb15e5599b08961b17e732de0308e' ;; 		armv7) natsArch='arm7'; sha256='2de2669cd17d8c5ad118d7b1b45dbf84fd2ea2baad728cca971df09715086760' ;; 		x86_64) natsArch='amd64'; sha256='7f8f9397247ed5c69eb1ecee25ef5181be822eb85645451389f11dfc9680ed6e' ;; 		x86) natsArch='386'; sha256='dc8793a9778fecd44d71837ecd52174aec79d2115eb895373cc9dd7797d8b6a0' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 30 Sep 2022 00:24:35 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 30 Sep 2022 00:24:35 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 30 Sep 2022 00:24:35 GMT
EXPOSE 4222 6222 8222
# Fri, 30 Sep 2022 00:24:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 30 Sep 2022 00:24:35 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf1cfb9d9ea4605961cdb87b6f9e44cdcfdf68501e6502197a61ba80d7fa2cf3`  
		Last Modified: Fri, 30 Sep 2022 00:25:27 GMT  
		Size: 5.2 MB (5191367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f19aac431077ee9634be9f5879d95e018b853fe9f4355edfb009578928af4a8b`  
		Last Modified: Fri, 30 Sep 2022 00:25:26 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d803ce9173785ad956d0980594d07b7c002d401ec4f7038696cea1a816f8eeba`  
		Last Modified: Fri, 30 Sep 2022 00:25:26 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.2-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:1b1b13874064770ee71ee054d372744f61509858d4e2f0e728f4f7e3d0c96979
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7569288 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca1a0478849efea10188e490a19d87485a7e44be7adeb5a71abc150e21ad71b4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:22 GMT
ADD file:e8733e8cc0a81e15ca4041760b6e27392c34171512d34405a9b262b1fff5c687 in / 
# Tue, 09 Aug 2022 17:49:22 GMT
CMD ["/bin/sh"]
# Fri, 30 Sep 2022 00:15:00 GMT
ENV NATS_SERVER=2.9.2
# Fri, 30 Sep 2022 00:15:03 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='a2c6ff2c7342198ed61136658310a8f3c336426b07062ed0a073c617ddf4b503' ;; 		armhf) natsArch='arm6'; sha256='918ee03dbc6ab17339f7510940945cdbb07fb15e5599b08961b17e732de0308e' ;; 		armv7) natsArch='arm7'; sha256='2de2669cd17d8c5ad118d7b1b45dbf84fd2ea2baad728cca971df09715086760' ;; 		x86_64) natsArch='amd64'; sha256='7f8f9397247ed5c69eb1ecee25ef5181be822eb85645451389f11dfc9680ed6e' ;; 		x86) natsArch='386'; sha256='dc8793a9778fecd44d71837ecd52174aec79d2115eb895373cc9dd7797d8b6a0' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 30 Sep 2022 00:15:03 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 30 Sep 2022 00:15:03 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 30 Sep 2022 00:15:03 GMT
EXPOSE 4222 6222 8222
# Fri, 30 Sep 2022 00:15:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 30 Sep 2022 00:15:03 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9506b835437abb4d8ba1683e00c500b8f77e1975e930b356fbb72f2dbdc274d9`  
		Last Modified: Tue, 09 Aug 2022 17:50:33 GMT  
		Size: 2.6 MB (2613965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70e3a299d439ca160a2da5bc72a2fbdfe0d669e0251c6c9ca166ab1f6572234f`  
		Last Modified: Fri, 30 Sep 2022 00:16:18 GMT  
		Size: 5.0 MB (4954323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c2c24ad6cbf82b17aa717ce52a3630fce897bdc317f1cd90fa28a0b18ec0132`  
		Last Modified: Fri, 30 Sep 2022 00:16:17 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8569952349d4aaee564b407fc4a769f8afee1973b746dbc535f7ec1d82ee711f`  
		Last Modified: Fri, 30 Sep 2022 00:16:17 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.2-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:2acfd2cdc64cbd116f1f26fd834f476761f9bd485105fc5e9bf4e56596077414
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.4 MB (7369328 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:71027a1b3accd3e7e548dd995f0f20adb3aac785ca9a3f8e122b085367eef6be`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 16:57:44 GMT
ADD file:75521fe16320b193092588f6f31052c85e736965ceb11673de18bd14965a45e6 in / 
# Tue, 09 Aug 2022 16:57:44 GMT
CMD ["/bin/sh"]
# Fri, 30 Sep 2022 12:21:21 GMT
ENV NATS_SERVER=2.9.2
# Fri, 30 Sep 2022 12:21:23 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='a2c6ff2c7342198ed61136658310a8f3c336426b07062ed0a073c617ddf4b503' ;; 		armhf) natsArch='arm6'; sha256='918ee03dbc6ab17339f7510940945cdbb07fb15e5599b08961b17e732de0308e' ;; 		armv7) natsArch='arm7'; sha256='2de2669cd17d8c5ad118d7b1b45dbf84fd2ea2baad728cca971df09715086760' ;; 		x86_64) natsArch='amd64'; sha256='7f8f9397247ed5c69eb1ecee25ef5181be822eb85645451389f11dfc9680ed6e' ;; 		x86) natsArch='386'; sha256='dc8793a9778fecd44d71837ecd52174aec79d2115eb895373cc9dd7797d8b6a0' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 30 Sep 2022 12:21:23 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 30 Sep 2022 12:21:23 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 30 Sep 2022 12:21:23 GMT
EXPOSE 4222 6222 8222
# Fri, 30 Sep 2022 12:21:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 30 Sep 2022 12:21:23 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:c6556b3b6858c6fa1e328377cc2c4becdc9cd1bc3e7302aa7299936522cf93ba`  
		Last Modified: Tue, 09 Aug 2022 16:58:55 GMT  
		Size: 2.4 MB (2417065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce37993864155926f403118474bfe7f519e53160887c3676f0cb079b2da279fd`  
		Last Modified: Fri, 30 Sep 2022 12:22:41 GMT  
		Size: 5.0 MB (4951267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:404500b58d5dc1fd3cb248fe12df440b55e9c3ab7d8671bd898e861be2f61927`  
		Last Modified: Fri, 30 Sep 2022 12:22:40 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04c6d22f211806f08bc6bc9690b5aff62e8fd42fe73b976a1d18dee96b17d9eb`  
		Last Modified: Fri, 30 Sep 2022 12:22:40 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.2-alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:63f1ff386adae53c49382ca5b6587c2dea35fc1af28e97033450cae49cfdcdab
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.5 MB (7485211 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6bf9a9bbea015857fed1ac343d2011fbc4ad3bfdc076c1963bd616875d0e0c88`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Fri, 30 Sep 2022 01:49:52 GMT
ENV NATS_SERVER=2.9.2
# Fri, 30 Sep 2022 01:49:55 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='a2c6ff2c7342198ed61136658310a8f3c336426b07062ed0a073c617ddf4b503' ;; 		armhf) natsArch='arm6'; sha256='918ee03dbc6ab17339f7510940945cdbb07fb15e5599b08961b17e732de0308e' ;; 		armv7) natsArch='arm7'; sha256='2de2669cd17d8c5ad118d7b1b45dbf84fd2ea2baad728cca971df09715086760' ;; 		x86_64) natsArch='amd64'; sha256='7f8f9397247ed5c69eb1ecee25ef5181be822eb85645451389f11dfc9680ed6e' ;; 		x86) natsArch='386'; sha256='dc8793a9778fecd44d71837ecd52174aec79d2115eb895373cc9dd7797d8b6a0' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 30 Sep 2022 01:49:57 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 30 Sep 2022 01:49:58 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 30 Sep 2022 01:49:58 GMT
EXPOSE 4222 6222 8222
# Fri, 30 Sep 2022 01:49:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 30 Sep 2022 01:50:00 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e30b79a866266b8c14d92afcced6bb4ffc32f152bafd6a4725eb24f2e5308da`  
		Last Modified: Fri, 30 Sep 2022 01:51:03 GMT  
		Size: 4.8 MB (4776577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d4ccb803f2d84c949447676b42f6b097337ce63fc73b9ff1b71715829193bb3`  
		Last Modified: Fri, 30 Sep 2022 01:51:02 GMT  
		Size: 559.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3baeeddb056b5f80c9eaf6dea17b085fd4b29d71b71ab6a68165224637f280da`  
		Last Modified: Fri, 30 Sep 2022 01:51:02 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.2-alpine3.16`

```console
$ docker pull nats@sha256:7b0816d59fbc8f00c834f53bc067bdbb35f27b79cef23e555ecd98496c9c9420
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9.2-alpine3.16` - linux; amd64

```console
$ docker pull nats@sha256:93b6c178034659b624ec39316bec9daeb14b38f690a531eaf5687c8f9a6420f6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.0 MB (7998419 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5068a20fcd0f44c75cc992b50a0c9406d62900af1d7756407b98f67a5aff6049`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Fri, 30 Sep 2022 00:24:33 GMT
ENV NATS_SERVER=2.9.2
# Fri, 30 Sep 2022 00:24:35 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='a2c6ff2c7342198ed61136658310a8f3c336426b07062ed0a073c617ddf4b503' ;; 		armhf) natsArch='arm6'; sha256='918ee03dbc6ab17339f7510940945cdbb07fb15e5599b08961b17e732de0308e' ;; 		armv7) natsArch='arm7'; sha256='2de2669cd17d8c5ad118d7b1b45dbf84fd2ea2baad728cca971df09715086760' ;; 		x86_64) natsArch='amd64'; sha256='7f8f9397247ed5c69eb1ecee25ef5181be822eb85645451389f11dfc9680ed6e' ;; 		x86) natsArch='386'; sha256='dc8793a9778fecd44d71837ecd52174aec79d2115eb895373cc9dd7797d8b6a0' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 30 Sep 2022 00:24:35 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 30 Sep 2022 00:24:35 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 30 Sep 2022 00:24:35 GMT
EXPOSE 4222 6222 8222
# Fri, 30 Sep 2022 00:24:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 30 Sep 2022 00:24:35 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf1cfb9d9ea4605961cdb87b6f9e44cdcfdf68501e6502197a61ba80d7fa2cf3`  
		Last Modified: Fri, 30 Sep 2022 00:25:27 GMT  
		Size: 5.2 MB (5191367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f19aac431077ee9634be9f5879d95e018b853fe9f4355edfb009578928af4a8b`  
		Last Modified: Fri, 30 Sep 2022 00:25:26 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d803ce9173785ad956d0980594d07b7c002d401ec4f7038696cea1a816f8eeba`  
		Last Modified: Fri, 30 Sep 2022 00:25:26 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.2-alpine3.16` - linux; arm variant v6

```console
$ docker pull nats@sha256:1b1b13874064770ee71ee054d372744f61509858d4e2f0e728f4f7e3d0c96979
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7569288 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca1a0478849efea10188e490a19d87485a7e44be7adeb5a71abc150e21ad71b4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:22 GMT
ADD file:e8733e8cc0a81e15ca4041760b6e27392c34171512d34405a9b262b1fff5c687 in / 
# Tue, 09 Aug 2022 17:49:22 GMT
CMD ["/bin/sh"]
# Fri, 30 Sep 2022 00:15:00 GMT
ENV NATS_SERVER=2.9.2
# Fri, 30 Sep 2022 00:15:03 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='a2c6ff2c7342198ed61136658310a8f3c336426b07062ed0a073c617ddf4b503' ;; 		armhf) natsArch='arm6'; sha256='918ee03dbc6ab17339f7510940945cdbb07fb15e5599b08961b17e732de0308e' ;; 		armv7) natsArch='arm7'; sha256='2de2669cd17d8c5ad118d7b1b45dbf84fd2ea2baad728cca971df09715086760' ;; 		x86_64) natsArch='amd64'; sha256='7f8f9397247ed5c69eb1ecee25ef5181be822eb85645451389f11dfc9680ed6e' ;; 		x86) natsArch='386'; sha256='dc8793a9778fecd44d71837ecd52174aec79d2115eb895373cc9dd7797d8b6a0' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 30 Sep 2022 00:15:03 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 30 Sep 2022 00:15:03 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 30 Sep 2022 00:15:03 GMT
EXPOSE 4222 6222 8222
# Fri, 30 Sep 2022 00:15:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 30 Sep 2022 00:15:03 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9506b835437abb4d8ba1683e00c500b8f77e1975e930b356fbb72f2dbdc274d9`  
		Last Modified: Tue, 09 Aug 2022 17:50:33 GMT  
		Size: 2.6 MB (2613965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70e3a299d439ca160a2da5bc72a2fbdfe0d669e0251c6c9ca166ab1f6572234f`  
		Last Modified: Fri, 30 Sep 2022 00:16:18 GMT  
		Size: 5.0 MB (4954323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c2c24ad6cbf82b17aa717ce52a3630fce897bdc317f1cd90fa28a0b18ec0132`  
		Last Modified: Fri, 30 Sep 2022 00:16:17 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8569952349d4aaee564b407fc4a769f8afee1973b746dbc535f7ec1d82ee711f`  
		Last Modified: Fri, 30 Sep 2022 00:16:17 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.2-alpine3.16` - linux; arm variant v7

```console
$ docker pull nats@sha256:2acfd2cdc64cbd116f1f26fd834f476761f9bd485105fc5e9bf4e56596077414
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.4 MB (7369328 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:71027a1b3accd3e7e548dd995f0f20adb3aac785ca9a3f8e122b085367eef6be`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 16:57:44 GMT
ADD file:75521fe16320b193092588f6f31052c85e736965ceb11673de18bd14965a45e6 in / 
# Tue, 09 Aug 2022 16:57:44 GMT
CMD ["/bin/sh"]
# Fri, 30 Sep 2022 12:21:21 GMT
ENV NATS_SERVER=2.9.2
# Fri, 30 Sep 2022 12:21:23 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='a2c6ff2c7342198ed61136658310a8f3c336426b07062ed0a073c617ddf4b503' ;; 		armhf) natsArch='arm6'; sha256='918ee03dbc6ab17339f7510940945cdbb07fb15e5599b08961b17e732de0308e' ;; 		armv7) natsArch='arm7'; sha256='2de2669cd17d8c5ad118d7b1b45dbf84fd2ea2baad728cca971df09715086760' ;; 		x86_64) natsArch='amd64'; sha256='7f8f9397247ed5c69eb1ecee25ef5181be822eb85645451389f11dfc9680ed6e' ;; 		x86) natsArch='386'; sha256='dc8793a9778fecd44d71837ecd52174aec79d2115eb895373cc9dd7797d8b6a0' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 30 Sep 2022 12:21:23 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 30 Sep 2022 12:21:23 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 30 Sep 2022 12:21:23 GMT
EXPOSE 4222 6222 8222
# Fri, 30 Sep 2022 12:21:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 30 Sep 2022 12:21:23 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:c6556b3b6858c6fa1e328377cc2c4becdc9cd1bc3e7302aa7299936522cf93ba`  
		Last Modified: Tue, 09 Aug 2022 16:58:55 GMT  
		Size: 2.4 MB (2417065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce37993864155926f403118474bfe7f519e53160887c3676f0cb079b2da279fd`  
		Last Modified: Fri, 30 Sep 2022 12:22:41 GMT  
		Size: 5.0 MB (4951267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:404500b58d5dc1fd3cb248fe12df440b55e9c3ab7d8671bd898e861be2f61927`  
		Last Modified: Fri, 30 Sep 2022 12:22:40 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04c6d22f211806f08bc6bc9690b5aff62e8fd42fe73b976a1d18dee96b17d9eb`  
		Last Modified: Fri, 30 Sep 2022 12:22:40 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.2-alpine3.16` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:63f1ff386adae53c49382ca5b6587c2dea35fc1af28e97033450cae49cfdcdab
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.5 MB (7485211 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6bf9a9bbea015857fed1ac343d2011fbc4ad3bfdc076c1963bd616875d0e0c88`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Fri, 30 Sep 2022 01:49:52 GMT
ENV NATS_SERVER=2.9.2
# Fri, 30 Sep 2022 01:49:55 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='a2c6ff2c7342198ed61136658310a8f3c336426b07062ed0a073c617ddf4b503' ;; 		armhf) natsArch='arm6'; sha256='918ee03dbc6ab17339f7510940945cdbb07fb15e5599b08961b17e732de0308e' ;; 		armv7) natsArch='arm7'; sha256='2de2669cd17d8c5ad118d7b1b45dbf84fd2ea2baad728cca971df09715086760' ;; 		x86_64) natsArch='amd64'; sha256='7f8f9397247ed5c69eb1ecee25ef5181be822eb85645451389f11dfc9680ed6e' ;; 		x86) natsArch='386'; sha256='dc8793a9778fecd44d71837ecd52174aec79d2115eb895373cc9dd7797d8b6a0' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 30 Sep 2022 01:49:57 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 30 Sep 2022 01:49:58 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 30 Sep 2022 01:49:58 GMT
EXPOSE 4222 6222 8222
# Fri, 30 Sep 2022 01:49:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 30 Sep 2022 01:50:00 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e30b79a866266b8c14d92afcced6bb4ffc32f152bafd6a4725eb24f2e5308da`  
		Last Modified: Fri, 30 Sep 2022 01:51:03 GMT  
		Size: 4.8 MB (4776577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d4ccb803f2d84c949447676b42f6b097337ce63fc73b9ff1b71715829193bb3`  
		Last Modified: Fri, 30 Sep 2022 01:51:02 GMT  
		Size: 559.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3baeeddb056b5f80c9eaf6dea17b085fd4b29d71b71ab6a68165224637f280da`  
		Last Modified: Fri, 30 Sep 2022 01:51:02 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.2-linux`

```console
$ docker pull nats@sha256:5f9faa293f743a8c78944dc1827132cc658e8ffcb2746d00e6ea69316a9fe3d9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9.2-linux` - linux; amd64

```console
$ docker pull nats@sha256:73a511425369d8e883fc5784023028b7ed02c252e6db030e776b2e6a76bb90ca
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4907513 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf3ba31eb02c938f2ab28c2b60358ef903503ce4a2fb5e2df6f4714d04e74619`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 30 Sep 2022 00:25:01 GMT
COPY file:ef7d265008705c7f8da964d29a2883d21303aab4d4520c3327ca6ce57348e137 in /nats-server 
# Fri, 30 Sep 2022 00:25:01 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 30 Sep 2022 00:25:01 GMT
EXPOSE 4222 6222 8222
# Fri, 30 Sep 2022 00:25:01 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 30 Sep 2022 00:25:01 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 30 Sep 2022 00:25:01 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:325d5a714be1f0303eebb8d34c9b23e1b15c5e7e46eb29d0f90511112fb86894`  
		Last Modified: Fri, 30 Sep 2022 00:25:50 GMT  
		Size: 4.9 MB (4907005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06b03a363308e84c4fc60d5ac2d5b9374e811456edecdb1e302e59198bfb1ca4`  
		Last Modified: Fri, 30 Sep 2022 00:25:49 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.2-linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:22be654fd606d7db5e28383ce35794c881f25b77908c6f981c2442b117d7df19
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4671534 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1eeeee00c7520737eb3766018dde7f3dd63c971938d98ff49cca225f0e6c6990`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 30 Sep 2022 00:15:17 GMT
COPY file:2de52eed8721a4ef1e4c8adb2f046a7ffa8e689d614c704b329ef2bafc7dfe5c in /nats-server 
# Fri, 30 Sep 2022 00:15:17 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 30 Sep 2022 00:15:17 GMT
EXPOSE 4222 6222 8222
# Fri, 30 Sep 2022 00:15:18 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 30 Sep 2022 00:15:18 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 30 Sep 2022 00:15:18 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:948e55d9b8c745ce1f9007c64a6da65d66c0d554fa7e5808a04081a1d0754a6c`  
		Last Modified: Fri, 30 Sep 2022 00:16:49 GMT  
		Size: 4.7 MB (4671025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14bdee3fcf17688810034aff56b746397e799579ff11654f2a2ec59274a9e161`  
		Last Modified: Fri, 30 Sep 2022 00:16:48 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.2-linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:dce0b0ef268b27c6417ee879c4f500273d8eabe0f3347ed2ac19b28a166085e2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4661683 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93f043be0120df37adc5618c50a4eb09f405d9a23f0794314f36c76be8bda597`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 30 Sep 2022 12:21:44 GMT
COPY file:e57d6f6c709cd7f891a48782c812655546ed7ed7194710fb4ff95d3225a8cb24 in /nats-server 
# Fri, 30 Sep 2022 12:21:44 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 30 Sep 2022 12:21:44 GMT
EXPOSE 4222 6222 8222
# Fri, 30 Sep 2022 12:21:44 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 30 Sep 2022 12:21:44 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 30 Sep 2022 12:21:44 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6709a2d5812e1f5aabc828977b23e9033fb28dd6d79bad682b986bfeaf468265`  
		Last Modified: Fri, 30 Sep 2022 12:23:13 GMT  
		Size: 4.7 MB (4661175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:913a6877bd39f71d19820c3493253d22c565656c7058ca6e5deb8e20280f8ad6`  
		Last Modified: Fri, 30 Sep 2022 12:23:12 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.2-linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:6d0d5cfcf4b908ca419719473183dd4000ebe2e77e9fb1088f51f2195324d865
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4495540 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7069cf895c76381ff91ad174ed58ca07743ca741317f4a2c20ea3b1f1bae44ce`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 30 Sep 2022 01:50:11 GMT
COPY file:06300839e6ae56288247488999d2e96ee71c9bb64453bfa88faa4cbfc85a23e2 in /nats-server 
# Fri, 30 Sep 2022 01:50:12 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 30 Sep 2022 01:50:12 GMT
EXPOSE 4222 6222 8222
# Fri, 30 Sep 2022 01:50:13 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 30 Sep 2022 01:50:14 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 30 Sep 2022 01:50:15 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:71fcb6de35d4d1378bd805b642a59de493c8957d351b1f521d05492db21c54d6`  
		Last Modified: Fri, 30 Sep 2022 01:51:31 GMT  
		Size: 4.5 MB (4495032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3be89d1242837970f7157774c5188f9046677dfb8c676155f7b2d268758d504`  
		Last Modified: Fri, 30 Sep 2022 01:51:30 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.2-nanoserver`

```console
$ docker pull nats@sha256:679b0d8e5bafa2c6893078adf595ebd301d9df9258ca22d088788c40d6ca5d28
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3406; amd64

### `nats:2.9.2-nanoserver` - windows version 10.0.17763.3406; amd64

```console
$ docker pull nats@sha256:2861931a21dd96bdbd1686faf3a14c6927dc24203b8c04d30b2116ef4d670e64
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **108.3 MB (108299212 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc0fee332755f830a4cef70df70da46a2cb2c28daadd327e68b97dbf22b35166`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 09 Sep 2022 22:22:51 GMT
RUN Apply image 10.0.17763.3406
# Wed, 14 Sep 2022 15:41:36 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 30 Sep 2022 00:18:47 GMT
RUN cmd /S /C #(nop) COPY file:da89208003aed19cb9852334329c2f8b4dfdfe3218c3f05bba8fcb3247acc400 in C:\nats-server.exe 
# Fri, 30 Sep 2022 00:18:48 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Fri, 30 Sep 2022 00:18:49 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Fri, 30 Sep 2022 00:18:50 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 30 Sep 2022 00:18:51 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:bcd4ab6c304faa0a7f4e183705a7f6e4545b728788221d17886d2a507ea0a06d`  
		Size: 103.3 MB (103334221 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b6bda313a93b8c355d5adf6e15f4b805f705c3741b235a7e4644bbffe6a6af3d`  
		Last Modified: Wed, 14 Sep 2022 15:42:30 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c046270960bff604e9be6498c1c0ee8367958198004e91286a8252366f7185c`  
		Last Modified: Fri, 30 Sep 2022 00:19:41 GMT  
		Size: 5.0 MB (4958572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1087232c1623e24e6883cc4c33bb9ff4926cfc24df9f4909f09db53185f2fe15`  
		Last Modified: Fri, 30 Sep 2022 00:19:40 GMT  
		Size: 1.8 KB (1774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83e77ee18b12423f469199b766a08c031324d15169a9f2e690bf77ccbb796ecd`  
		Last Modified: Fri, 30 Sep 2022 00:19:40 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4549b9baa74eb7ff07539b979f0966c66afb35858810779ec9d7572da5777e49`  
		Last Modified: Fri, 30 Sep 2022 00:19:40 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ee9032ad08c565fc85469a687bbaddfa40a6066692a113da46c758c5d591e4a`  
		Last Modified: Fri, 30 Sep 2022 00:19:40 GMT  
		Size: 1.2 KB (1176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.2-nanoserver-1809`

```console
$ docker pull nats@sha256:679b0d8e5bafa2c6893078adf595ebd301d9df9258ca22d088788c40d6ca5d28
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3406; amd64

### `nats:2.9.2-nanoserver-1809` - windows version 10.0.17763.3406; amd64

```console
$ docker pull nats@sha256:2861931a21dd96bdbd1686faf3a14c6927dc24203b8c04d30b2116ef4d670e64
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **108.3 MB (108299212 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc0fee332755f830a4cef70df70da46a2cb2c28daadd327e68b97dbf22b35166`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 09 Sep 2022 22:22:51 GMT
RUN Apply image 10.0.17763.3406
# Wed, 14 Sep 2022 15:41:36 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 30 Sep 2022 00:18:47 GMT
RUN cmd /S /C #(nop) COPY file:da89208003aed19cb9852334329c2f8b4dfdfe3218c3f05bba8fcb3247acc400 in C:\nats-server.exe 
# Fri, 30 Sep 2022 00:18:48 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Fri, 30 Sep 2022 00:18:49 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Fri, 30 Sep 2022 00:18:50 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 30 Sep 2022 00:18:51 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:bcd4ab6c304faa0a7f4e183705a7f6e4545b728788221d17886d2a507ea0a06d`  
		Size: 103.3 MB (103334221 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b6bda313a93b8c355d5adf6e15f4b805f705c3741b235a7e4644bbffe6a6af3d`  
		Last Modified: Wed, 14 Sep 2022 15:42:30 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c046270960bff604e9be6498c1c0ee8367958198004e91286a8252366f7185c`  
		Last Modified: Fri, 30 Sep 2022 00:19:41 GMT  
		Size: 5.0 MB (4958572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1087232c1623e24e6883cc4c33bb9ff4926cfc24df9f4909f09db53185f2fe15`  
		Last Modified: Fri, 30 Sep 2022 00:19:40 GMT  
		Size: 1.8 KB (1774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83e77ee18b12423f469199b766a08c031324d15169a9f2e690bf77ccbb796ecd`  
		Last Modified: Fri, 30 Sep 2022 00:19:40 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4549b9baa74eb7ff07539b979f0966c66afb35858810779ec9d7572da5777e49`  
		Last Modified: Fri, 30 Sep 2022 00:19:40 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ee9032ad08c565fc85469a687bbaddfa40a6066692a113da46c758c5d591e4a`  
		Last Modified: Fri, 30 Sep 2022 00:19:40 GMT  
		Size: 1.2 KB (1176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.2-scratch`

```console
$ docker pull nats@sha256:5f9faa293f743a8c78944dc1827132cc658e8ffcb2746d00e6ea69316a9fe3d9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9.2-scratch` - linux; amd64

```console
$ docker pull nats@sha256:73a511425369d8e883fc5784023028b7ed02c252e6db030e776b2e6a76bb90ca
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4907513 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf3ba31eb02c938f2ab28c2b60358ef903503ce4a2fb5e2df6f4714d04e74619`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 30 Sep 2022 00:25:01 GMT
COPY file:ef7d265008705c7f8da964d29a2883d21303aab4d4520c3327ca6ce57348e137 in /nats-server 
# Fri, 30 Sep 2022 00:25:01 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 30 Sep 2022 00:25:01 GMT
EXPOSE 4222 6222 8222
# Fri, 30 Sep 2022 00:25:01 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 30 Sep 2022 00:25:01 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 30 Sep 2022 00:25:01 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:325d5a714be1f0303eebb8d34c9b23e1b15c5e7e46eb29d0f90511112fb86894`  
		Last Modified: Fri, 30 Sep 2022 00:25:50 GMT  
		Size: 4.9 MB (4907005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06b03a363308e84c4fc60d5ac2d5b9374e811456edecdb1e302e59198bfb1ca4`  
		Last Modified: Fri, 30 Sep 2022 00:25:49 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.2-scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:22be654fd606d7db5e28383ce35794c881f25b77908c6f981c2442b117d7df19
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4671534 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1eeeee00c7520737eb3766018dde7f3dd63c971938d98ff49cca225f0e6c6990`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 30 Sep 2022 00:15:17 GMT
COPY file:2de52eed8721a4ef1e4c8adb2f046a7ffa8e689d614c704b329ef2bafc7dfe5c in /nats-server 
# Fri, 30 Sep 2022 00:15:17 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 30 Sep 2022 00:15:17 GMT
EXPOSE 4222 6222 8222
# Fri, 30 Sep 2022 00:15:18 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 30 Sep 2022 00:15:18 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 30 Sep 2022 00:15:18 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:948e55d9b8c745ce1f9007c64a6da65d66c0d554fa7e5808a04081a1d0754a6c`  
		Last Modified: Fri, 30 Sep 2022 00:16:49 GMT  
		Size: 4.7 MB (4671025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14bdee3fcf17688810034aff56b746397e799579ff11654f2a2ec59274a9e161`  
		Last Modified: Fri, 30 Sep 2022 00:16:48 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.2-scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:dce0b0ef268b27c6417ee879c4f500273d8eabe0f3347ed2ac19b28a166085e2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4661683 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93f043be0120df37adc5618c50a4eb09f405d9a23f0794314f36c76be8bda597`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 30 Sep 2022 12:21:44 GMT
COPY file:e57d6f6c709cd7f891a48782c812655546ed7ed7194710fb4ff95d3225a8cb24 in /nats-server 
# Fri, 30 Sep 2022 12:21:44 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 30 Sep 2022 12:21:44 GMT
EXPOSE 4222 6222 8222
# Fri, 30 Sep 2022 12:21:44 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 30 Sep 2022 12:21:44 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 30 Sep 2022 12:21:44 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6709a2d5812e1f5aabc828977b23e9033fb28dd6d79bad682b986bfeaf468265`  
		Last Modified: Fri, 30 Sep 2022 12:23:13 GMT  
		Size: 4.7 MB (4661175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:913a6877bd39f71d19820c3493253d22c565656c7058ca6e5deb8e20280f8ad6`  
		Last Modified: Fri, 30 Sep 2022 12:23:12 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.2-scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:6d0d5cfcf4b908ca419719473183dd4000ebe2e77e9fb1088f51f2195324d865
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4495540 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7069cf895c76381ff91ad174ed58ca07743ca741317f4a2c20ea3b1f1bae44ce`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 30 Sep 2022 01:50:11 GMT
COPY file:06300839e6ae56288247488999d2e96ee71c9bb64453bfa88faa4cbfc85a23e2 in /nats-server 
# Fri, 30 Sep 2022 01:50:12 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 30 Sep 2022 01:50:12 GMT
EXPOSE 4222 6222 8222
# Fri, 30 Sep 2022 01:50:13 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 30 Sep 2022 01:50:14 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 30 Sep 2022 01:50:15 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:71fcb6de35d4d1378bd805b642a59de493c8957d351b1f521d05492db21c54d6`  
		Last Modified: Fri, 30 Sep 2022 01:51:31 GMT  
		Size: 4.5 MB (4495032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3be89d1242837970f7157774c5188f9046677dfb8c676155f7b2d268758d504`  
		Last Modified: Fri, 30 Sep 2022 01:51:30 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.2-windowsservercore`

```console
$ docker pull nats@sha256:3357d7889ebcb10a163ba56eff66f60ff010e161b38e1f401cc136e7a6879baf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3406; amd64

### `nats:2.9.2-windowsservercore` - windows version 10.0.17763.3406; amd64

```console
$ docker pull nats@sha256:214e04a7dc77ff783ac336d010ba64eb98f2c8722d522260bf340c2df3d521e7
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2709236645 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:30cb30cff6676167599e8b4fd9f6b053b3e6fa2f5418a7a419e631956a014e9e`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Fri, 09 Sep 2022 22:43:02 GMT
RUN Install update 10.0.17763.3406
# Wed, 14 Sep 2022 13:39:18 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 14 Sep 2022 15:38:54 GMT
ENV NATS_DOCKERIZED=1
# Fri, 30 Sep 2022 00:15:50 GMT
ENV NATS_SERVER=2.9.2
# Fri, 30 Sep 2022 00:15:51 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.9.2/nats-server-v2.9.2-windows-amd64.zip
# Fri, 30 Sep 2022 00:15:52 GMT
ENV NATS_SERVER_SHASUM=cd3d2a9d78c235292afc27f812baee7817180fcfe5ebba662e72f0cc821d04fb
# Fri, 30 Sep 2022 00:16:59 GMT
RUN Set-PSDebug -Trace 2
# Fri, 30 Sep 2022 00:18:30 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 30 Sep 2022 00:18:31 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Fri, 30 Sep 2022 00:18:31 GMT
EXPOSE 4222 6222 8222
# Fri, 30 Sep 2022 00:18:32 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 30 Sep 2022 00:18:33 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:cee64bf279e2ca8e924884a10ecb98bfa79c7f0cc8d25e73039b9aeb940815b6`  
		Size: 826.4 MB (826398623 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3c428406510f0a47ed60f28060a7d625d42344a95fdcb7c4f5746fb8857c3328`  
		Last Modified: Wed, 14 Sep 2022 15:42:13 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf4bba85c5cc970a66b01ed6f4cabffa7705a0bdbc18907894f94c09b5ee2618`  
		Last Modified: Wed, 14 Sep 2022 15:42:12 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a29319534b1836908aab29077ce165236693f20e5abbb69a70639c6cce19223b`  
		Last Modified: Fri, 30 Sep 2022 00:19:24 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d34f7b3a98b75cbb6f21f33118a7f43b9efe7d7d8ef5d9f47b5ca73470abd339`  
		Last Modified: Fri, 30 Sep 2022 00:19:24 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2119397eb3051d4784ced2882a1c0f1d2995cec67f5954fd5f33fde4b6ab4c3a`  
		Last Modified: Fri, 30 Sep 2022 00:19:24 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cdecf001ef7e4a9db54aa1a639bf5036f69cfc71a2d6b1b9089c1a3810373aa`  
		Last Modified: Fri, 30 Sep 2022 00:19:24 GMT  
		Size: 358.1 KB (358089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4a5a2ffe352520814f5794422903ec9e717d37294931ca81f856257a419ee1f`  
		Last Modified: Fri, 30 Sep 2022 00:19:23 GMT  
		Size: 5.3 MB (5300456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b80c11ae75a170747a9206d993fe059c9cda9f34c08c9f2eb90bedaef90f322e`  
		Last Modified: Fri, 30 Sep 2022 00:19:22 GMT  
		Size: 2.0 KB (2012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e8020be63ec6ec39f4443bc78e114caf9c24c5686fcf3f84a8c74f38f61b864`  
		Last Modified: Fri, 30 Sep 2022 00:19:22 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50d3d068429b4966cc13e153bdbf220b0259eb72a6a3f507fc5172a963499566`  
		Last Modified: Fri, 30 Sep 2022 00:19:22 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f588edee9a48a943744711d7d4dea00d9e842180f05a759c2edf3e50ee10e06c`  
		Last Modified: Fri, 30 Sep 2022 00:19:22 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.2-windowsservercore-1809`

```console
$ docker pull nats@sha256:3357d7889ebcb10a163ba56eff66f60ff010e161b38e1f401cc136e7a6879baf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3406; amd64

### `nats:2.9.2-windowsservercore-1809` - windows version 10.0.17763.3406; amd64

```console
$ docker pull nats@sha256:214e04a7dc77ff783ac336d010ba64eb98f2c8722d522260bf340c2df3d521e7
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2709236645 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:30cb30cff6676167599e8b4fd9f6b053b3e6fa2f5418a7a419e631956a014e9e`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Fri, 09 Sep 2022 22:43:02 GMT
RUN Install update 10.0.17763.3406
# Wed, 14 Sep 2022 13:39:18 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 14 Sep 2022 15:38:54 GMT
ENV NATS_DOCKERIZED=1
# Fri, 30 Sep 2022 00:15:50 GMT
ENV NATS_SERVER=2.9.2
# Fri, 30 Sep 2022 00:15:51 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.9.2/nats-server-v2.9.2-windows-amd64.zip
# Fri, 30 Sep 2022 00:15:52 GMT
ENV NATS_SERVER_SHASUM=cd3d2a9d78c235292afc27f812baee7817180fcfe5ebba662e72f0cc821d04fb
# Fri, 30 Sep 2022 00:16:59 GMT
RUN Set-PSDebug -Trace 2
# Fri, 30 Sep 2022 00:18:30 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 30 Sep 2022 00:18:31 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Fri, 30 Sep 2022 00:18:31 GMT
EXPOSE 4222 6222 8222
# Fri, 30 Sep 2022 00:18:32 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 30 Sep 2022 00:18:33 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:cee64bf279e2ca8e924884a10ecb98bfa79c7f0cc8d25e73039b9aeb940815b6`  
		Size: 826.4 MB (826398623 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3c428406510f0a47ed60f28060a7d625d42344a95fdcb7c4f5746fb8857c3328`  
		Last Modified: Wed, 14 Sep 2022 15:42:13 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf4bba85c5cc970a66b01ed6f4cabffa7705a0bdbc18907894f94c09b5ee2618`  
		Last Modified: Wed, 14 Sep 2022 15:42:12 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a29319534b1836908aab29077ce165236693f20e5abbb69a70639c6cce19223b`  
		Last Modified: Fri, 30 Sep 2022 00:19:24 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d34f7b3a98b75cbb6f21f33118a7f43b9efe7d7d8ef5d9f47b5ca73470abd339`  
		Last Modified: Fri, 30 Sep 2022 00:19:24 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2119397eb3051d4784ced2882a1c0f1d2995cec67f5954fd5f33fde4b6ab4c3a`  
		Last Modified: Fri, 30 Sep 2022 00:19:24 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cdecf001ef7e4a9db54aa1a639bf5036f69cfc71a2d6b1b9089c1a3810373aa`  
		Last Modified: Fri, 30 Sep 2022 00:19:24 GMT  
		Size: 358.1 KB (358089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4a5a2ffe352520814f5794422903ec9e717d37294931ca81f856257a419ee1f`  
		Last Modified: Fri, 30 Sep 2022 00:19:23 GMT  
		Size: 5.3 MB (5300456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b80c11ae75a170747a9206d993fe059c9cda9f34c08c9f2eb90bedaef90f322e`  
		Last Modified: Fri, 30 Sep 2022 00:19:22 GMT  
		Size: 2.0 KB (2012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e8020be63ec6ec39f4443bc78e114caf9c24c5686fcf3f84a8c74f38f61b864`  
		Last Modified: Fri, 30 Sep 2022 00:19:22 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50d3d068429b4966cc13e153bdbf220b0259eb72a6a3f507fc5172a963499566`  
		Last Modified: Fri, 30 Sep 2022 00:19:22 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f588edee9a48a943744711d7d4dea00d9e842180f05a759c2edf3e50ee10e06c`  
		Last Modified: Fri, 30 Sep 2022 00:19:22 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:alpine`

```console
$ docker pull nats@sha256:7b0816d59fbc8f00c834f53bc067bdbb35f27b79cef23e555ecd98496c9c9420
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:alpine` - linux; amd64

```console
$ docker pull nats@sha256:93b6c178034659b624ec39316bec9daeb14b38f690a531eaf5687c8f9a6420f6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.0 MB (7998419 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5068a20fcd0f44c75cc992b50a0c9406d62900af1d7756407b98f67a5aff6049`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Fri, 30 Sep 2022 00:24:33 GMT
ENV NATS_SERVER=2.9.2
# Fri, 30 Sep 2022 00:24:35 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='a2c6ff2c7342198ed61136658310a8f3c336426b07062ed0a073c617ddf4b503' ;; 		armhf) natsArch='arm6'; sha256='918ee03dbc6ab17339f7510940945cdbb07fb15e5599b08961b17e732de0308e' ;; 		armv7) natsArch='arm7'; sha256='2de2669cd17d8c5ad118d7b1b45dbf84fd2ea2baad728cca971df09715086760' ;; 		x86_64) natsArch='amd64'; sha256='7f8f9397247ed5c69eb1ecee25ef5181be822eb85645451389f11dfc9680ed6e' ;; 		x86) natsArch='386'; sha256='dc8793a9778fecd44d71837ecd52174aec79d2115eb895373cc9dd7797d8b6a0' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 30 Sep 2022 00:24:35 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 30 Sep 2022 00:24:35 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 30 Sep 2022 00:24:35 GMT
EXPOSE 4222 6222 8222
# Fri, 30 Sep 2022 00:24:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 30 Sep 2022 00:24:35 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf1cfb9d9ea4605961cdb87b6f9e44cdcfdf68501e6502197a61ba80d7fa2cf3`  
		Last Modified: Fri, 30 Sep 2022 00:25:27 GMT  
		Size: 5.2 MB (5191367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f19aac431077ee9634be9f5879d95e018b853fe9f4355edfb009578928af4a8b`  
		Last Modified: Fri, 30 Sep 2022 00:25:26 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d803ce9173785ad956d0980594d07b7c002d401ec4f7038696cea1a816f8eeba`  
		Last Modified: Fri, 30 Sep 2022 00:25:26 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:1b1b13874064770ee71ee054d372744f61509858d4e2f0e728f4f7e3d0c96979
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7569288 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca1a0478849efea10188e490a19d87485a7e44be7adeb5a71abc150e21ad71b4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:22 GMT
ADD file:e8733e8cc0a81e15ca4041760b6e27392c34171512d34405a9b262b1fff5c687 in / 
# Tue, 09 Aug 2022 17:49:22 GMT
CMD ["/bin/sh"]
# Fri, 30 Sep 2022 00:15:00 GMT
ENV NATS_SERVER=2.9.2
# Fri, 30 Sep 2022 00:15:03 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='a2c6ff2c7342198ed61136658310a8f3c336426b07062ed0a073c617ddf4b503' ;; 		armhf) natsArch='arm6'; sha256='918ee03dbc6ab17339f7510940945cdbb07fb15e5599b08961b17e732de0308e' ;; 		armv7) natsArch='arm7'; sha256='2de2669cd17d8c5ad118d7b1b45dbf84fd2ea2baad728cca971df09715086760' ;; 		x86_64) natsArch='amd64'; sha256='7f8f9397247ed5c69eb1ecee25ef5181be822eb85645451389f11dfc9680ed6e' ;; 		x86) natsArch='386'; sha256='dc8793a9778fecd44d71837ecd52174aec79d2115eb895373cc9dd7797d8b6a0' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 30 Sep 2022 00:15:03 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 30 Sep 2022 00:15:03 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 30 Sep 2022 00:15:03 GMT
EXPOSE 4222 6222 8222
# Fri, 30 Sep 2022 00:15:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 30 Sep 2022 00:15:03 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9506b835437abb4d8ba1683e00c500b8f77e1975e930b356fbb72f2dbdc274d9`  
		Last Modified: Tue, 09 Aug 2022 17:50:33 GMT  
		Size: 2.6 MB (2613965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70e3a299d439ca160a2da5bc72a2fbdfe0d669e0251c6c9ca166ab1f6572234f`  
		Last Modified: Fri, 30 Sep 2022 00:16:18 GMT  
		Size: 5.0 MB (4954323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c2c24ad6cbf82b17aa717ce52a3630fce897bdc317f1cd90fa28a0b18ec0132`  
		Last Modified: Fri, 30 Sep 2022 00:16:17 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8569952349d4aaee564b407fc4a769f8afee1973b746dbc535f7ec1d82ee711f`  
		Last Modified: Fri, 30 Sep 2022 00:16:17 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:2acfd2cdc64cbd116f1f26fd834f476761f9bd485105fc5e9bf4e56596077414
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.4 MB (7369328 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:71027a1b3accd3e7e548dd995f0f20adb3aac785ca9a3f8e122b085367eef6be`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 16:57:44 GMT
ADD file:75521fe16320b193092588f6f31052c85e736965ceb11673de18bd14965a45e6 in / 
# Tue, 09 Aug 2022 16:57:44 GMT
CMD ["/bin/sh"]
# Fri, 30 Sep 2022 12:21:21 GMT
ENV NATS_SERVER=2.9.2
# Fri, 30 Sep 2022 12:21:23 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='a2c6ff2c7342198ed61136658310a8f3c336426b07062ed0a073c617ddf4b503' ;; 		armhf) natsArch='arm6'; sha256='918ee03dbc6ab17339f7510940945cdbb07fb15e5599b08961b17e732de0308e' ;; 		armv7) natsArch='arm7'; sha256='2de2669cd17d8c5ad118d7b1b45dbf84fd2ea2baad728cca971df09715086760' ;; 		x86_64) natsArch='amd64'; sha256='7f8f9397247ed5c69eb1ecee25ef5181be822eb85645451389f11dfc9680ed6e' ;; 		x86) natsArch='386'; sha256='dc8793a9778fecd44d71837ecd52174aec79d2115eb895373cc9dd7797d8b6a0' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 30 Sep 2022 12:21:23 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 30 Sep 2022 12:21:23 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 30 Sep 2022 12:21:23 GMT
EXPOSE 4222 6222 8222
# Fri, 30 Sep 2022 12:21:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 30 Sep 2022 12:21:23 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:c6556b3b6858c6fa1e328377cc2c4becdc9cd1bc3e7302aa7299936522cf93ba`  
		Last Modified: Tue, 09 Aug 2022 16:58:55 GMT  
		Size: 2.4 MB (2417065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce37993864155926f403118474bfe7f519e53160887c3676f0cb079b2da279fd`  
		Last Modified: Fri, 30 Sep 2022 12:22:41 GMT  
		Size: 5.0 MB (4951267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:404500b58d5dc1fd3cb248fe12df440b55e9c3ab7d8671bd898e861be2f61927`  
		Last Modified: Fri, 30 Sep 2022 12:22:40 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04c6d22f211806f08bc6bc9690b5aff62e8fd42fe73b976a1d18dee96b17d9eb`  
		Last Modified: Fri, 30 Sep 2022 12:22:40 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:63f1ff386adae53c49382ca5b6587c2dea35fc1af28e97033450cae49cfdcdab
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.5 MB (7485211 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6bf9a9bbea015857fed1ac343d2011fbc4ad3bfdc076c1963bd616875d0e0c88`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Fri, 30 Sep 2022 01:49:52 GMT
ENV NATS_SERVER=2.9.2
# Fri, 30 Sep 2022 01:49:55 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='a2c6ff2c7342198ed61136658310a8f3c336426b07062ed0a073c617ddf4b503' ;; 		armhf) natsArch='arm6'; sha256='918ee03dbc6ab17339f7510940945cdbb07fb15e5599b08961b17e732de0308e' ;; 		armv7) natsArch='arm7'; sha256='2de2669cd17d8c5ad118d7b1b45dbf84fd2ea2baad728cca971df09715086760' ;; 		x86_64) natsArch='amd64'; sha256='7f8f9397247ed5c69eb1ecee25ef5181be822eb85645451389f11dfc9680ed6e' ;; 		x86) natsArch='386'; sha256='dc8793a9778fecd44d71837ecd52174aec79d2115eb895373cc9dd7797d8b6a0' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 30 Sep 2022 01:49:57 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 30 Sep 2022 01:49:58 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 30 Sep 2022 01:49:58 GMT
EXPOSE 4222 6222 8222
# Fri, 30 Sep 2022 01:49:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 30 Sep 2022 01:50:00 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e30b79a866266b8c14d92afcced6bb4ffc32f152bafd6a4725eb24f2e5308da`  
		Last Modified: Fri, 30 Sep 2022 01:51:03 GMT  
		Size: 4.8 MB (4776577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d4ccb803f2d84c949447676b42f6b097337ce63fc73b9ff1b71715829193bb3`  
		Last Modified: Fri, 30 Sep 2022 01:51:02 GMT  
		Size: 559.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3baeeddb056b5f80c9eaf6dea17b085fd4b29d71b71ab6a68165224637f280da`  
		Last Modified: Fri, 30 Sep 2022 01:51:02 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:alpine3.16`

```console
$ docker pull nats@sha256:7b0816d59fbc8f00c834f53bc067bdbb35f27b79cef23e555ecd98496c9c9420
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:alpine3.16` - linux; amd64

```console
$ docker pull nats@sha256:93b6c178034659b624ec39316bec9daeb14b38f690a531eaf5687c8f9a6420f6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.0 MB (7998419 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5068a20fcd0f44c75cc992b50a0c9406d62900af1d7756407b98f67a5aff6049`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Fri, 30 Sep 2022 00:24:33 GMT
ENV NATS_SERVER=2.9.2
# Fri, 30 Sep 2022 00:24:35 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='a2c6ff2c7342198ed61136658310a8f3c336426b07062ed0a073c617ddf4b503' ;; 		armhf) natsArch='arm6'; sha256='918ee03dbc6ab17339f7510940945cdbb07fb15e5599b08961b17e732de0308e' ;; 		armv7) natsArch='arm7'; sha256='2de2669cd17d8c5ad118d7b1b45dbf84fd2ea2baad728cca971df09715086760' ;; 		x86_64) natsArch='amd64'; sha256='7f8f9397247ed5c69eb1ecee25ef5181be822eb85645451389f11dfc9680ed6e' ;; 		x86) natsArch='386'; sha256='dc8793a9778fecd44d71837ecd52174aec79d2115eb895373cc9dd7797d8b6a0' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 30 Sep 2022 00:24:35 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 30 Sep 2022 00:24:35 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 30 Sep 2022 00:24:35 GMT
EXPOSE 4222 6222 8222
# Fri, 30 Sep 2022 00:24:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 30 Sep 2022 00:24:35 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf1cfb9d9ea4605961cdb87b6f9e44cdcfdf68501e6502197a61ba80d7fa2cf3`  
		Last Modified: Fri, 30 Sep 2022 00:25:27 GMT  
		Size: 5.2 MB (5191367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f19aac431077ee9634be9f5879d95e018b853fe9f4355edfb009578928af4a8b`  
		Last Modified: Fri, 30 Sep 2022 00:25:26 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d803ce9173785ad956d0980594d07b7c002d401ec4f7038696cea1a816f8eeba`  
		Last Modified: Fri, 30 Sep 2022 00:25:26 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.16` - linux; arm variant v6

```console
$ docker pull nats@sha256:1b1b13874064770ee71ee054d372744f61509858d4e2f0e728f4f7e3d0c96979
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7569288 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca1a0478849efea10188e490a19d87485a7e44be7adeb5a71abc150e21ad71b4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:22 GMT
ADD file:e8733e8cc0a81e15ca4041760b6e27392c34171512d34405a9b262b1fff5c687 in / 
# Tue, 09 Aug 2022 17:49:22 GMT
CMD ["/bin/sh"]
# Fri, 30 Sep 2022 00:15:00 GMT
ENV NATS_SERVER=2.9.2
# Fri, 30 Sep 2022 00:15:03 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='a2c6ff2c7342198ed61136658310a8f3c336426b07062ed0a073c617ddf4b503' ;; 		armhf) natsArch='arm6'; sha256='918ee03dbc6ab17339f7510940945cdbb07fb15e5599b08961b17e732de0308e' ;; 		armv7) natsArch='arm7'; sha256='2de2669cd17d8c5ad118d7b1b45dbf84fd2ea2baad728cca971df09715086760' ;; 		x86_64) natsArch='amd64'; sha256='7f8f9397247ed5c69eb1ecee25ef5181be822eb85645451389f11dfc9680ed6e' ;; 		x86) natsArch='386'; sha256='dc8793a9778fecd44d71837ecd52174aec79d2115eb895373cc9dd7797d8b6a0' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 30 Sep 2022 00:15:03 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 30 Sep 2022 00:15:03 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 30 Sep 2022 00:15:03 GMT
EXPOSE 4222 6222 8222
# Fri, 30 Sep 2022 00:15:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 30 Sep 2022 00:15:03 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9506b835437abb4d8ba1683e00c500b8f77e1975e930b356fbb72f2dbdc274d9`  
		Last Modified: Tue, 09 Aug 2022 17:50:33 GMT  
		Size: 2.6 MB (2613965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70e3a299d439ca160a2da5bc72a2fbdfe0d669e0251c6c9ca166ab1f6572234f`  
		Last Modified: Fri, 30 Sep 2022 00:16:18 GMT  
		Size: 5.0 MB (4954323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c2c24ad6cbf82b17aa717ce52a3630fce897bdc317f1cd90fa28a0b18ec0132`  
		Last Modified: Fri, 30 Sep 2022 00:16:17 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8569952349d4aaee564b407fc4a769f8afee1973b746dbc535f7ec1d82ee711f`  
		Last Modified: Fri, 30 Sep 2022 00:16:17 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.16` - linux; arm variant v7

```console
$ docker pull nats@sha256:2acfd2cdc64cbd116f1f26fd834f476761f9bd485105fc5e9bf4e56596077414
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.4 MB (7369328 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:71027a1b3accd3e7e548dd995f0f20adb3aac785ca9a3f8e122b085367eef6be`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 16:57:44 GMT
ADD file:75521fe16320b193092588f6f31052c85e736965ceb11673de18bd14965a45e6 in / 
# Tue, 09 Aug 2022 16:57:44 GMT
CMD ["/bin/sh"]
# Fri, 30 Sep 2022 12:21:21 GMT
ENV NATS_SERVER=2.9.2
# Fri, 30 Sep 2022 12:21:23 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='a2c6ff2c7342198ed61136658310a8f3c336426b07062ed0a073c617ddf4b503' ;; 		armhf) natsArch='arm6'; sha256='918ee03dbc6ab17339f7510940945cdbb07fb15e5599b08961b17e732de0308e' ;; 		armv7) natsArch='arm7'; sha256='2de2669cd17d8c5ad118d7b1b45dbf84fd2ea2baad728cca971df09715086760' ;; 		x86_64) natsArch='amd64'; sha256='7f8f9397247ed5c69eb1ecee25ef5181be822eb85645451389f11dfc9680ed6e' ;; 		x86) natsArch='386'; sha256='dc8793a9778fecd44d71837ecd52174aec79d2115eb895373cc9dd7797d8b6a0' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 30 Sep 2022 12:21:23 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 30 Sep 2022 12:21:23 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 30 Sep 2022 12:21:23 GMT
EXPOSE 4222 6222 8222
# Fri, 30 Sep 2022 12:21:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 30 Sep 2022 12:21:23 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:c6556b3b6858c6fa1e328377cc2c4becdc9cd1bc3e7302aa7299936522cf93ba`  
		Last Modified: Tue, 09 Aug 2022 16:58:55 GMT  
		Size: 2.4 MB (2417065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce37993864155926f403118474bfe7f519e53160887c3676f0cb079b2da279fd`  
		Last Modified: Fri, 30 Sep 2022 12:22:41 GMT  
		Size: 5.0 MB (4951267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:404500b58d5dc1fd3cb248fe12df440b55e9c3ab7d8671bd898e861be2f61927`  
		Last Modified: Fri, 30 Sep 2022 12:22:40 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04c6d22f211806f08bc6bc9690b5aff62e8fd42fe73b976a1d18dee96b17d9eb`  
		Last Modified: Fri, 30 Sep 2022 12:22:40 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.16` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:63f1ff386adae53c49382ca5b6587c2dea35fc1af28e97033450cae49cfdcdab
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.5 MB (7485211 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6bf9a9bbea015857fed1ac343d2011fbc4ad3bfdc076c1963bd616875d0e0c88`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Fri, 30 Sep 2022 01:49:52 GMT
ENV NATS_SERVER=2.9.2
# Fri, 30 Sep 2022 01:49:55 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='a2c6ff2c7342198ed61136658310a8f3c336426b07062ed0a073c617ddf4b503' ;; 		armhf) natsArch='arm6'; sha256='918ee03dbc6ab17339f7510940945cdbb07fb15e5599b08961b17e732de0308e' ;; 		armv7) natsArch='arm7'; sha256='2de2669cd17d8c5ad118d7b1b45dbf84fd2ea2baad728cca971df09715086760' ;; 		x86_64) natsArch='amd64'; sha256='7f8f9397247ed5c69eb1ecee25ef5181be822eb85645451389f11dfc9680ed6e' ;; 		x86) natsArch='386'; sha256='dc8793a9778fecd44d71837ecd52174aec79d2115eb895373cc9dd7797d8b6a0' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 30 Sep 2022 01:49:57 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 30 Sep 2022 01:49:58 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 30 Sep 2022 01:49:58 GMT
EXPOSE 4222 6222 8222
# Fri, 30 Sep 2022 01:49:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 30 Sep 2022 01:50:00 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e30b79a866266b8c14d92afcced6bb4ffc32f152bafd6a4725eb24f2e5308da`  
		Last Modified: Fri, 30 Sep 2022 01:51:03 GMT  
		Size: 4.8 MB (4776577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d4ccb803f2d84c949447676b42f6b097337ce63fc73b9ff1b71715829193bb3`  
		Last Modified: Fri, 30 Sep 2022 01:51:02 GMT  
		Size: 559.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3baeeddb056b5f80c9eaf6dea17b085fd4b29d71b71ab6a68165224637f280da`  
		Last Modified: Fri, 30 Sep 2022 01:51:02 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:latest`

```console
$ docker pull nats@sha256:2a333e9f7d50ba4dd450e435b65a5b038af6988ab4c19c858cf85c6733667c28
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.3406; amd64

### `nats:latest` - linux; amd64

```console
$ docker pull nats@sha256:73a511425369d8e883fc5784023028b7ed02c252e6db030e776b2e6a76bb90ca
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4907513 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf3ba31eb02c938f2ab28c2b60358ef903503ce4a2fb5e2df6f4714d04e74619`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 30 Sep 2022 00:25:01 GMT
COPY file:ef7d265008705c7f8da964d29a2883d21303aab4d4520c3327ca6ce57348e137 in /nats-server 
# Fri, 30 Sep 2022 00:25:01 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 30 Sep 2022 00:25:01 GMT
EXPOSE 4222 6222 8222
# Fri, 30 Sep 2022 00:25:01 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 30 Sep 2022 00:25:01 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 30 Sep 2022 00:25:01 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:325d5a714be1f0303eebb8d34c9b23e1b15c5e7e46eb29d0f90511112fb86894`  
		Last Modified: Fri, 30 Sep 2022 00:25:50 GMT  
		Size: 4.9 MB (4907005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06b03a363308e84c4fc60d5ac2d5b9374e811456edecdb1e302e59198bfb1ca4`  
		Last Modified: Fri, 30 Sep 2022 00:25:49 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm variant v6

```console
$ docker pull nats@sha256:22be654fd606d7db5e28383ce35794c881f25b77908c6f981c2442b117d7df19
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4671534 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1eeeee00c7520737eb3766018dde7f3dd63c971938d98ff49cca225f0e6c6990`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 30 Sep 2022 00:15:17 GMT
COPY file:2de52eed8721a4ef1e4c8adb2f046a7ffa8e689d614c704b329ef2bafc7dfe5c in /nats-server 
# Fri, 30 Sep 2022 00:15:17 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 30 Sep 2022 00:15:17 GMT
EXPOSE 4222 6222 8222
# Fri, 30 Sep 2022 00:15:18 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 30 Sep 2022 00:15:18 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 30 Sep 2022 00:15:18 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:948e55d9b8c745ce1f9007c64a6da65d66c0d554fa7e5808a04081a1d0754a6c`  
		Last Modified: Fri, 30 Sep 2022 00:16:49 GMT  
		Size: 4.7 MB (4671025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14bdee3fcf17688810034aff56b746397e799579ff11654f2a2ec59274a9e161`  
		Last Modified: Fri, 30 Sep 2022 00:16:48 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm variant v7

```console
$ docker pull nats@sha256:dce0b0ef268b27c6417ee879c4f500273d8eabe0f3347ed2ac19b28a166085e2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4661683 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93f043be0120df37adc5618c50a4eb09f405d9a23f0794314f36c76be8bda597`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 30 Sep 2022 12:21:44 GMT
COPY file:e57d6f6c709cd7f891a48782c812655546ed7ed7194710fb4ff95d3225a8cb24 in /nats-server 
# Fri, 30 Sep 2022 12:21:44 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 30 Sep 2022 12:21:44 GMT
EXPOSE 4222 6222 8222
# Fri, 30 Sep 2022 12:21:44 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 30 Sep 2022 12:21:44 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 30 Sep 2022 12:21:44 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6709a2d5812e1f5aabc828977b23e9033fb28dd6d79bad682b986bfeaf468265`  
		Last Modified: Fri, 30 Sep 2022 12:23:13 GMT  
		Size: 4.7 MB (4661175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:913a6877bd39f71d19820c3493253d22c565656c7058ca6e5deb8e20280f8ad6`  
		Last Modified: Fri, 30 Sep 2022 12:23:12 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:6d0d5cfcf4b908ca419719473183dd4000ebe2e77e9fb1088f51f2195324d865
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4495540 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7069cf895c76381ff91ad174ed58ca07743ca741317f4a2c20ea3b1f1bae44ce`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 30 Sep 2022 01:50:11 GMT
COPY file:06300839e6ae56288247488999d2e96ee71c9bb64453bfa88faa4cbfc85a23e2 in /nats-server 
# Fri, 30 Sep 2022 01:50:12 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 30 Sep 2022 01:50:12 GMT
EXPOSE 4222 6222 8222
# Fri, 30 Sep 2022 01:50:13 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 30 Sep 2022 01:50:14 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 30 Sep 2022 01:50:15 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:71fcb6de35d4d1378bd805b642a59de493c8957d351b1f521d05492db21c54d6`  
		Last Modified: Fri, 30 Sep 2022 01:51:31 GMT  
		Size: 4.5 MB (4495032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3be89d1242837970f7157774c5188f9046677dfb8c676155f7b2d268758d504`  
		Last Modified: Fri, 30 Sep 2022 01:51:30 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - windows version 10.0.17763.3406; amd64

```console
$ docker pull nats@sha256:2861931a21dd96bdbd1686faf3a14c6927dc24203b8c04d30b2116ef4d670e64
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **108.3 MB (108299212 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc0fee332755f830a4cef70df70da46a2cb2c28daadd327e68b97dbf22b35166`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 09 Sep 2022 22:22:51 GMT
RUN Apply image 10.0.17763.3406
# Wed, 14 Sep 2022 15:41:36 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 30 Sep 2022 00:18:47 GMT
RUN cmd /S /C #(nop) COPY file:da89208003aed19cb9852334329c2f8b4dfdfe3218c3f05bba8fcb3247acc400 in C:\nats-server.exe 
# Fri, 30 Sep 2022 00:18:48 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Fri, 30 Sep 2022 00:18:49 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Fri, 30 Sep 2022 00:18:50 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 30 Sep 2022 00:18:51 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:bcd4ab6c304faa0a7f4e183705a7f6e4545b728788221d17886d2a507ea0a06d`  
		Size: 103.3 MB (103334221 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b6bda313a93b8c355d5adf6e15f4b805f705c3741b235a7e4644bbffe6a6af3d`  
		Last Modified: Wed, 14 Sep 2022 15:42:30 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c046270960bff604e9be6498c1c0ee8367958198004e91286a8252366f7185c`  
		Last Modified: Fri, 30 Sep 2022 00:19:41 GMT  
		Size: 5.0 MB (4958572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1087232c1623e24e6883cc4c33bb9ff4926cfc24df9f4909f09db53185f2fe15`  
		Last Modified: Fri, 30 Sep 2022 00:19:40 GMT  
		Size: 1.8 KB (1774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83e77ee18b12423f469199b766a08c031324d15169a9f2e690bf77ccbb796ecd`  
		Last Modified: Fri, 30 Sep 2022 00:19:40 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4549b9baa74eb7ff07539b979f0966c66afb35858810779ec9d7572da5777e49`  
		Last Modified: Fri, 30 Sep 2022 00:19:40 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ee9032ad08c565fc85469a687bbaddfa40a6066692a113da46c758c5d591e4a`  
		Last Modified: Fri, 30 Sep 2022 00:19:40 GMT  
		Size: 1.2 KB (1176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:linux`

```console
$ docker pull nats@sha256:5f9faa293f743a8c78944dc1827132cc658e8ffcb2746d00e6ea69316a9fe3d9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:linux` - linux; amd64

```console
$ docker pull nats@sha256:73a511425369d8e883fc5784023028b7ed02c252e6db030e776b2e6a76bb90ca
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4907513 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf3ba31eb02c938f2ab28c2b60358ef903503ce4a2fb5e2df6f4714d04e74619`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 30 Sep 2022 00:25:01 GMT
COPY file:ef7d265008705c7f8da964d29a2883d21303aab4d4520c3327ca6ce57348e137 in /nats-server 
# Fri, 30 Sep 2022 00:25:01 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 30 Sep 2022 00:25:01 GMT
EXPOSE 4222 6222 8222
# Fri, 30 Sep 2022 00:25:01 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 30 Sep 2022 00:25:01 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 30 Sep 2022 00:25:01 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:325d5a714be1f0303eebb8d34c9b23e1b15c5e7e46eb29d0f90511112fb86894`  
		Last Modified: Fri, 30 Sep 2022 00:25:50 GMT  
		Size: 4.9 MB (4907005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06b03a363308e84c4fc60d5ac2d5b9374e811456edecdb1e302e59198bfb1ca4`  
		Last Modified: Fri, 30 Sep 2022 00:25:49 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:22be654fd606d7db5e28383ce35794c881f25b77908c6f981c2442b117d7df19
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4671534 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1eeeee00c7520737eb3766018dde7f3dd63c971938d98ff49cca225f0e6c6990`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 30 Sep 2022 00:15:17 GMT
COPY file:2de52eed8721a4ef1e4c8adb2f046a7ffa8e689d614c704b329ef2bafc7dfe5c in /nats-server 
# Fri, 30 Sep 2022 00:15:17 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 30 Sep 2022 00:15:17 GMT
EXPOSE 4222 6222 8222
# Fri, 30 Sep 2022 00:15:18 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 30 Sep 2022 00:15:18 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 30 Sep 2022 00:15:18 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:948e55d9b8c745ce1f9007c64a6da65d66c0d554fa7e5808a04081a1d0754a6c`  
		Last Modified: Fri, 30 Sep 2022 00:16:49 GMT  
		Size: 4.7 MB (4671025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14bdee3fcf17688810034aff56b746397e799579ff11654f2a2ec59274a9e161`  
		Last Modified: Fri, 30 Sep 2022 00:16:48 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:dce0b0ef268b27c6417ee879c4f500273d8eabe0f3347ed2ac19b28a166085e2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4661683 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93f043be0120df37adc5618c50a4eb09f405d9a23f0794314f36c76be8bda597`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 30 Sep 2022 12:21:44 GMT
COPY file:e57d6f6c709cd7f891a48782c812655546ed7ed7194710fb4ff95d3225a8cb24 in /nats-server 
# Fri, 30 Sep 2022 12:21:44 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 30 Sep 2022 12:21:44 GMT
EXPOSE 4222 6222 8222
# Fri, 30 Sep 2022 12:21:44 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 30 Sep 2022 12:21:44 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 30 Sep 2022 12:21:44 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6709a2d5812e1f5aabc828977b23e9033fb28dd6d79bad682b986bfeaf468265`  
		Last Modified: Fri, 30 Sep 2022 12:23:13 GMT  
		Size: 4.7 MB (4661175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:913a6877bd39f71d19820c3493253d22c565656c7058ca6e5deb8e20280f8ad6`  
		Last Modified: Fri, 30 Sep 2022 12:23:12 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:6d0d5cfcf4b908ca419719473183dd4000ebe2e77e9fb1088f51f2195324d865
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4495540 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7069cf895c76381ff91ad174ed58ca07743ca741317f4a2c20ea3b1f1bae44ce`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 30 Sep 2022 01:50:11 GMT
COPY file:06300839e6ae56288247488999d2e96ee71c9bb64453bfa88faa4cbfc85a23e2 in /nats-server 
# Fri, 30 Sep 2022 01:50:12 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 30 Sep 2022 01:50:12 GMT
EXPOSE 4222 6222 8222
# Fri, 30 Sep 2022 01:50:13 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 30 Sep 2022 01:50:14 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 30 Sep 2022 01:50:15 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:71fcb6de35d4d1378bd805b642a59de493c8957d351b1f521d05492db21c54d6`  
		Last Modified: Fri, 30 Sep 2022 01:51:31 GMT  
		Size: 4.5 MB (4495032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3be89d1242837970f7157774c5188f9046677dfb8c676155f7b2d268758d504`  
		Last Modified: Fri, 30 Sep 2022 01:51:30 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:nanoserver`

```console
$ docker pull nats@sha256:679b0d8e5bafa2c6893078adf595ebd301d9df9258ca22d088788c40d6ca5d28
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3406; amd64

### `nats:nanoserver` - windows version 10.0.17763.3406; amd64

```console
$ docker pull nats@sha256:2861931a21dd96bdbd1686faf3a14c6927dc24203b8c04d30b2116ef4d670e64
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **108.3 MB (108299212 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc0fee332755f830a4cef70df70da46a2cb2c28daadd327e68b97dbf22b35166`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 09 Sep 2022 22:22:51 GMT
RUN Apply image 10.0.17763.3406
# Wed, 14 Sep 2022 15:41:36 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 30 Sep 2022 00:18:47 GMT
RUN cmd /S /C #(nop) COPY file:da89208003aed19cb9852334329c2f8b4dfdfe3218c3f05bba8fcb3247acc400 in C:\nats-server.exe 
# Fri, 30 Sep 2022 00:18:48 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Fri, 30 Sep 2022 00:18:49 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Fri, 30 Sep 2022 00:18:50 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 30 Sep 2022 00:18:51 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:bcd4ab6c304faa0a7f4e183705a7f6e4545b728788221d17886d2a507ea0a06d`  
		Size: 103.3 MB (103334221 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b6bda313a93b8c355d5adf6e15f4b805f705c3741b235a7e4644bbffe6a6af3d`  
		Last Modified: Wed, 14 Sep 2022 15:42:30 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c046270960bff604e9be6498c1c0ee8367958198004e91286a8252366f7185c`  
		Last Modified: Fri, 30 Sep 2022 00:19:41 GMT  
		Size: 5.0 MB (4958572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1087232c1623e24e6883cc4c33bb9ff4926cfc24df9f4909f09db53185f2fe15`  
		Last Modified: Fri, 30 Sep 2022 00:19:40 GMT  
		Size: 1.8 KB (1774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83e77ee18b12423f469199b766a08c031324d15169a9f2e690bf77ccbb796ecd`  
		Last Modified: Fri, 30 Sep 2022 00:19:40 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4549b9baa74eb7ff07539b979f0966c66afb35858810779ec9d7572da5777e49`  
		Last Modified: Fri, 30 Sep 2022 00:19:40 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ee9032ad08c565fc85469a687bbaddfa40a6066692a113da46c758c5d591e4a`  
		Last Modified: Fri, 30 Sep 2022 00:19:40 GMT  
		Size: 1.2 KB (1176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:nanoserver-1809`

```console
$ docker pull nats@sha256:679b0d8e5bafa2c6893078adf595ebd301d9df9258ca22d088788c40d6ca5d28
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3406; amd64

### `nats:nanoserver-1809` - windows version 10.0.17763.3406; amd64

```console
$ docker pull nats@sha256:2861931a21dd96bdbd1686faf3a14c6927dc24203b8c04d30b2116ef4d670e64
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **108.3 MB (108299212 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc0fee332755f830a4cef70df70da46a2cb2c28daadd327e68b97dbf22b35166`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 09 Sep 2022 22:22:51 GMT
RUN Apply image 10.0.17763.3406
# Wed, 14 Sep 2022 15:41:36 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 30 Sep 2022 00:18:47 GMT
RUN cmd /S /C #(nop) COPY file:da89208003aed19cb9852334329c2f8b4dfdfe3218c3f05bba8fcb3247acc400 in C:\nats-server.exe 
# Fri, 30 Sep 2022 00:18:48 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Fri, 30 Sep 2022 00:18:49 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Fri, 30 Sep 2022 00:18:50 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 30 Sep 2022 00:18:51 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:bcd4ab6c304faa0a7f4e183705a7f6e4545b728788221d17886d2a507ea0a06d`  
		Size: 103.3 MB (103334221 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b6bda313a93b8c355d5adf6e15f4b805f705c3741b235a7e4644bbffe6a6af3d`  
		Last Modified: Wed, 14 Sep 2022 15:42:30 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c046270960bff604e9be6498c1c0ee8367958198004e91286a8252366f7185c`  
		Last Modified: Fri, 30 Sep 2022 00:19:41 GMT  
		Size: 5.0 MB (4958572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1087232c1623e24e6883cc4c33bb9ff4926cfc24df9f4909f09db53185f2fe15`  
		Last Modified: Fri, 30 Sep 2022 00:19:40 GMT  
		Size: 1.8 KB (1774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83e77ee18b12423f469199b766a08c031324d15169a9f2e690bf77ccbb796ecd`  
		Last Modified: Fri, 30 Sep 2022 00:19:40 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4549b9baa74eb7ff07539b979f0966c66afb35858810779ec9d7572da5777e49`  
		Last Modified: Fri, 30 Sep 2022 00:19:40 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ee9032ad08c565fc85469a687bbaddfa40a6066692a113da46c758c5d591e4a`  
		Last Modified: Fri, 30 Sep 2022 00:19:40 GMT  
		Size: 1.2 KB (1176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:scratch`

```console
$ docker pull nats@sha256:5f9faa293f743a8c78944dc1827132cc658e8ffcb2746d00e6ea69316a9fe3d9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:scratch` - linux; amd64

```console
$ docker pull nats@sha256:73a511425369d8e883fc5784023028b7ed02c252e6db030e776b2e6a76bb90ca
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4907513 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf3ba31eb02c938f2ab28c2b60358ef903503ce4a2fb5e2df6f4714d04e74619`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 30 Sep 2022 00:25:01 GMT
COPY file:ef7d265008705c7f8da964d29a2883d21303aab4d4520c3327ca6ce57348e137 in /nats-server 
# Fri, 30 Sep 2022 00:25:01 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 30 Sep 2022 00:25:01 GMT
EXPOSE 4222 6222 8222
# Fri, 30 Sep 2022 00:25:01 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 30 Sep 2022 00:25:01 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 30 Sep 2022 00:25:01 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:325d5a714be1f0303eebb8d34c9b23e1b15c5e7e46eb29d0f90511112fb86894`  
		Last Modified: Fri, 30 Sep 2022 00:25:50 GMT  
		Size: 4.9 MB (4907005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06b03a363308e84c4fc60d5ac2d5b9374e811456edecdb1e302e59198bfb1ca4`  
		Last Modified: Fri, 30 Sep 2022 00:25:49 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:22be654fd606d7db5e28383ce35794c881f25b77908c6f981c2442b117d7df19
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4671534 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1eeeee00c7520737eb3766018dde7f3dd63c971938d98ff49cca225f0e6c6990`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 30 Sep 2022 00:15:17 GMT
COPY file:2de52eed8721a4ef1e4c8adb2f046a7ffa8e689d614c704b329ef2bafc7dfe5c in /nats-server 
# Fri, 30 Sep 2022 00:15:17 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 30 Sep 2022 00:15:17 GMT
EXPOSE 4222 6222 8222
# Fri, 30 Sep 2022 00:15:18 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 30 Sep 2022 00:15:18 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 30 Sep 2022 00:15:18 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:948e55d9b8c745ce1f9007c64a6da65d66c0d554fa7e5808a04081a1d0754a6c`  
		Last Modified: Fri, 30 Sep 2022 00:16:49 GMT  
		Size: 4.7 MB (4671025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14bdee3fcf17688810034aff56b746397e799579ff11654f2a2ec59274a9e161`  
		Last Modified: Fri, 30 Sep 2022 00:16:48 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:dce0b0ef268b27c6417ee879c4f500273d8eabe0f3347ed2ac19b28a166085e2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4661683 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93f043be0120df37adc5618c50a4eb09f405d9a23f0794314f36c76be8bda597`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 30 Sep 2022 12:21:44 GMT
COPY file:e57d6f6c709cd7f891a48782c812655546ed7ed7194710fb4ff95d3225a8cb24 in /nats-server 
# Fri, 30 Sep 2022 12:21:44 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 30 Sep 2022 12:21:44 GMT
EXPOSE 4222 6222 8222
# Fri, 30 Sep 2022 12:21:44 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 30 Sep 2022 12:21:44 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 30 Sep 2022 12:21:44 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6709a2d5812e1f5aabc828977b23e9033fb28dd6d79bad682b986bfeaf468265`  
		Last Modified: Fri, 30 Sep 2022 12:23:13 GMT  
		Size: 4.7 MB (4661175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:913a6877bd39f71d19820c3493253d22c565656c7058ca6e5deb8e20280f8ad6`  
		Last Modified: Fri, 30 Sep 2022 12:23:12 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:6d0d5cfcf4b908ca419719473183dd4000ebe2e77e9fb1088f51f2195324d865
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4495540 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7069cf895c76381ff91ad174ed58ca07743ca741317f4a2c20ea3b1f1bae44ce`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 30 Sep 2022 01:50:11 GMT
COPY file:06300839e6ae56288247488999d2e96ee71c9bb64453bfa88faa4cbfc85a23e2 in /nats-server 
# Fri, 30 Sep 2022 01:50:12 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 30 Sep 2022 01:50:12 GMT
EXPOSE 4222 6222 8222
# Fri, 30 Sep 2022 01:50:13 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 30 Sep 2022 01:50:14 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 30 Sep 2022 01:50:15 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:71fcb6de35d4d1378bd805b642a59de493c8957d351b1f521d05492db21c54d6`  
		Last Modified: Fri, 30 Sep 2022 01:51:31 GMT  
		Size: 4.5 MB (4495032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3be89d1242837970f7157774c5188f9046677dfb8c676155f7b2d268758d504`  
		Last Modified: Fri, 30 Sep 2022 01:51:30 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:windowsservercore`

```console
$ docker pull nats@sha256:3357d7889ebcb10a163ba56eff66f60ff010e161b38e1f401cc136e7a6879baf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3406; amd64

### `nats:windowsservercore` - windows version 10.0.17763.3406; amd64

```console
$ docker pull nats@sha256:214e04a7dc77ff783ac336d010ba64eb98f2c8722d522260bf340c2df3d521e7
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2709236645 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:30cb30cff6676167599e8b4fd9f6b053b3e6fa2f5418a7a419e631956a014e9e`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Fri, 09 Sep 2022 22:43:02 GMT
RUN Install update 10.0.17763.3406
# Wed, 14 Sep 2022 13:39:18 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 14 Sep 2022 15:38:54 GMT
ENV NATS_DOCKERIZED=1
# Fri, 30 Sep 2022 00:15:50 GMT
ENV NATS_SERVER=2.9.2
# Fri, 30 Sep 2022 00:15:51 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.9.2/nats-server-v2.9.2-windows-amd64.zip
# Fri, 30 Sep 2022 00:15:52 GMT
ENV NATS_SERVER_SHASUM=cd3d2a9d78c235292afc27f812baee7817180fcfe5ebba662e72f0cc821d04fb
# Fri, 30 Sep 2022 00:16:59 GMT
RUN Set-PSDebug -Trace 2
# Fri, 30 Sep 2022 00:18:30 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 30 Sep 2022 00:18:31 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Fri, 30 Sep 2022 00:18:31 GMT
EXPOSE 4222 6222 8222
# Fri, 30 Sep 2022 00:18:32 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 30 Sep 2022 00:18:33 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:cee64bf279e2ca8e924884a10ecb98bfa79c7f0cc8d25e73039b9aeb940815b6`  
		Size: 826.4 MB (826398623 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3c428406510f0a47ed60f28060a7d625d42344a95fdcb7c4f5746fb8857c3328`  
		Last Modified: Wed, 14 Sep 2022 15:42:13 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf4bba85c5cc970a66b01ed6f4cabffa7705a0bdbc18907894f94c09b5ee2618`  
		Last Modified: Wed, 14 Sep 2022 15:42:12 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a29319534b1836908aab29077ce165236693f20e5abbb69a70639c6cce19223b`  
		Last Modified: Fri, 30 Sep 2022 00:19:24 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d34f7b3a98b75cbb6f21f33118a7f43b9efe7d7d8ef5d9f47b5ca73470abd339`  
		Last Modified: Fri, 30 Sep 2022 00:19:24 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2119397eb3051d4784ced2882a1c0f1d2995cec67f5954fd5f33fde4b6ab4c3a`  
		Last Modified: Fri, 30 Sep 2022 00:19:24 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cdecf001ef7e4a9db54aa1a639bf5036f69cfc71a2d6b1b9089c1a3810373aa`  
		Last Modified: Fri, 30 Sep 2022 00:19:24 GMT  
		Size: 358.1 KB (358089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4a5a2ffe352520814f5794422903ec9e717d37294931ca81f856257a419ee1f`  
		Last Modified: Fri, 30 Sep 2022 00:19:23 GMT  
		Size: 5.3 MB (5300456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b80c11ae75a170747a9206d993fe059c9cda9f34c08c9f2eb90bedaef90f322e`  
		Last Modified: Fri, 30 Sep 2022 00:19:22 GMT  
		Size: 2.0 KB (2012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e8020be63ec6ec39f4443bc78e114caf9c24c5686fcf3f84a8c74f38f61b864`  
		Last Modified: Fri, 30 Sep 2022 00:19:22 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50d3d068429b4966cc13e153bdbf220b0259eb72a6a3f507fc5172a963499566`  
		Last Modified: Fri, 30 Sep 2022 00:19:22 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f588edee9a48a943744711d7d4dea00d9e842180f05a759c2edf3e50ee10e06c`  
		Last Modified: Fri, 30 Sep 2022 00:19:22 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:windowsservercore-1809`

```console
$ docker pull nats@sha256:3357d7889ebcb10a163ba56eff66f60ff010e161b38e1f401cc136e7a6879baf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3406; amd64

### `nats:windowsservercore-1809` - windows version 10.0.17763.3406; amd64

```console
$ docker pull nats@sha256:214e04a7dc77ff783ac336d010ba64eb98f2c8722d522260bf340c2df3d521e7
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2709236645 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:30cb30cff6676167599e8b4fd9f6b053b3e6fa2f5418a7a419e631956a014e9e`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Fri, 09 Sep 2022 22:43:02 GMT
RUN Install update 10.0.17763.3406
# Wed, 14 Sep 2022 13:39:18 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 14 Sep 2022 15:38:54 GMT
ENV NATS_DOCKERIZED=1
# Fri, 30 Sep 2022 00:15:50 GMT
ENV NATS_SERVER=2.9.2
# Fri, 30 Sep 2022 00:15:51 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.9.2/nats-server-v2.9.2-windows-amd64.zip
# Fri, 30 Sep 2022 00:15:52 GMT
ENV NATS_SERVER_SHASUM=cd3d2a9d78c235292afc27f812baee7817180fcfe5ebba662e72f0cc821d04fb
# Fri, 30 Sep 2022 00:16:59 GMT
RUN Set-PSDebug -Trace 2
# Fri, 30 Sep 2022 00:18:30 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 30 Sep 2022 00:18:31 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Fri, 30 Sep 2022 00:18:31 GMT
EXPOSE 4222 6222 8222
# Fri, 30 Sep 2022 00:18:32 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 30 Sep 2022 00:18:33 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:cee64bf279e2ca8e924884a10ecb98bfa79c7f0cc8d25e73039b9aeb940815b6`  
		Size: 826.4 MB (826398623 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3c428406510f0a47ed60f28060a7d625d42344a95fdcb7c4f5746fb8857c3328`  
		Last Modified: Wed, 14 Sep 2022 15:42:13 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf4bba85c5cc970a66b01ed6f4cabffa7705a0bdbc18907894f94c09b5ee2618`  
		Last Modified: Wed, 14 Sep 2022 15:42:12 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a29319534b1836908aab29077ce165236693f20e5abbb69a70639c6cce19223b`  
		Last Modified: Fri, 30 Sep 2022 00:19:24 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d34f7b3a98b75cbb6f21f33118a7f43b9efe7d7d8ef5d9f47b5ca73470abd339`  
		Last Modified: Fri, 30 Sep 2022 00:19:24 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2119397eb3051d4784ced2882a1c0f1d2995cec67f5954fd5f33fde4b6ab4c3a`  
		Last Modified: Fri, 30 Sep 2022 00:19:24 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cdecf001ef7e4a9db54aa1a639bf5036f69cfc71a2d6b1b9089c1a3810373aa`  
		Last Modified: Fri, 30 Sep 2022 00:19:24 GMT  
		Size: 358.1 KB (358089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4a5a2ffe352520814f5794422903ec9e717d37294931ca81f856257a419ee1f`  
		Last Modified: Fri, 30 Sep 2022 00:19:23 GMT  
		Size: 5.3 MB (5300456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b80c11ae75a170747a9206d993fe059c9cda9f34c08c9f2eb90bedaef90f322e`  
		Last Modified: Fri, 30 Sep 2022 00:19:22 GMT  
		Size: 2.0 KB (2012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e8020be63ec6ec39f4443bc78e114caf9c24c5686fcf3f84a8c74f38f61b864`  
		Last Modified: Fri, 30 Sep 2022 00:19:22 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50d3d068429b4966cc13e153bdbf220b0259eb72a6a3f507fc5172a963499566`  
		Last Modified: Fri, 30 Sep 2022 00:19:22 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f588edee9a48a943744711d7d4dea00d9e842180f05a759c2edf3e50ee10e06c`  
		Last Modified: Fri, 30 Sep 2022 00:19:22 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
