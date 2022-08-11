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
-	[`nats:2.8`](#nats28)
-	[`nats:2.8-alpine`](#nats28-alpine)
-	[`nats:2.8-alpine3.15`](#nats28-alpine315)
-	[`nats:2.8-linux`](#nats28-linux)
-	[`nats:2.8-nanoserver`](#nats28-nanoserver)
-	[`nats:2.8-nanoserver-1809`](#nats28-nanoserver-1809)
-	[`nats:2.8-scratch`](#nats28-scratch)
-	[`nats:2.8-windowsservercore`](#nats28-windowsservercore)
-	[`nats:2.8-windowsservercore-1809`](#nats28-windowsservercore-1809)
-	[`nats:2.8.4`](#nats284)
-	[`nats:2.8.4-alpine`](#nats284-alpine)
-	[`nats:2.8.4-alpine3.15`](#nats284-alpine315)
-	[`nats:2.8.4-linux`](#nats284-linux)
-	[`nats:2.8.4-nanoserver`](#nats284-nanoserver)
-	[`nats:2.8.4-nanoserver-1809`](#nats284-nanoserver-1809)
-	[`nats:2.8.4-scratch`](#nats284-scratch)
-	[`nats:2.8.4-windowsservercore`](#nats284-windowsservercore)
-	[`nats:2.8.4-windowsservercore-1809`](#nats284-windowsservercore-1809)
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
$ docker pull nats@sha256:8f0cdcbc4c3597443fce869e75a759edb0d5a93fe98078f470a43204a6d7a729
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.3287; amd64

### `nats:2` - linux; amd64

```console
$ docker pull nats@sha256:796298f636925dedbbdfa537f42423dffd3a69b70c3a9bf4fd0982886a4b745d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4591595 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:842c053e15bdb38e697668b1f0721313203f7c2297eb6d79000f20858dc97854`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 27 May 2022 00:38:26 GMT
COPY file:c866dea678e8cec7cbd0798a1dbdefc45e992d9df374709f6000bac517589a1b in /nats-server 
# Fri, 27 May 2022 00:38:26 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 27 May 2022 00:38:27 GMT
EXPOSE 4222 6222 8222
# Fri, 27 May 2022 00:38:27 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 27 May 2022 00:38:27 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 27 May 2022 00:38:27 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:5e5797f39fa0527a3dd0a137353b40f97c71134e7eb38373d9791c5f1392885b`  
		Last Modified: Fri, 27 May 2022 00:39:15 GMT  
		Size: 4.6 MB (4591087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28c3b732adf61929b0b23ca08934cd89923e9cd9d7061544e76bbce57a9fa1e4`  
		Last Modified: Fri, 27 May 2022 00:39:14 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - linux; arm variant v6

```console
$ docker pull nats@sha256:e0c28a95cdf6dd8a566d5c2394d09e6141dffb9107fe49f9385d6f19048bd955
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4245827 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cef47371f249bc862484ca7bd4dde2d7f77dc41bcb49cc49cceb17dfb2d4471f`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 11 Aug 2022 01:12:06 GMT
COPY file:8de8b0cf8e6edf54e413c112cd66aed537abed387a26ba749a9293d43cdf6594 in /nats-server 
# Thu, 11 Aug 2022 01:12:06 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 11 Aug 2022 01:12:06 GMT
EXPOSE 4222 6222 8222
# Thu, 11 Aug 2022 01:12:06 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 11 Aug 2022 01:12:06 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 11 Aug 2022 01:12:06 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:770fa9c168613edbe7aa7007d2cf8492c6570efc1ddab217fa32772c6b72dd48`  
		Last Modified: Thu, 26 May 2022 23:58:21 GMT  
		Size: 4.2 MB (4245317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bde47aae170f9c7e50b7bbea164ec0e0d02b9c05b603e7f7554e163183c02cd9`  
		Last Modified: Thu, 11 Aug 2022 01:13:30 GMT  
		Size: 510.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - linux; arm variant v7

```console
$ docker pull nats@sha256:453c8fea5d37abc60f034f80bdb668a48c8e4f0900fce8b55fdb6ae7f2908d07
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4242795 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:508b00336aa0fc72bd1c3d33e5f447d1411e47221dfa1fa6085d6986b27045d7`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 22:36:22 GMT
COPY file:2841d6664b8897473f39b595b9aa4b28e749f587dc1afa4a0027ae507f37ee1f in /nats-server 
# Tue, 09 Aug 2022 22:36:22 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 09 Aug 2022 22:36:22 GMT
EXPOSE 4222 6222 8222
# Tue, 09 Aug 2022 22:36:22 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 09 Aug 2022 22:36:23 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 09 Aug 2022 22:36:23 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:f533e6e439ee51f1cf94458f821a20ed162b542d356340957091882ad881d5c1`  
		Last Modified: Fri, 27 May 2022 00:28:16 GMT  
		Size: 4.2 MB (4242287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:274ba9becbe1086958e9d56ab9452ec01f7fad6e3e68a34c49f1f299a5eab1ac`  
		Last Modified: Tue, 09 Aug 2022 22:38:14 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:87b1afbd78a75ee48cb6b37a8522bbb01f5e9b5047b095b16cc4f241774a48d1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4227885 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9bce5ae01237736c7e0447d8cd1b2dbe252eab3ab5ac3b05d98b646b2575cee`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 26 May 2022 23:53:56 GMT
COPY file:2dbd94c6c11f89ceba3241f1efe469d0a06f0aae91abb77f3d79756676d0be57 in /nats-server 
# Thu, 26 May 2022 23:53:57 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 26 May 2022 23:53:57 GMT
EXPOSE 4222 6222 8222
# Thu, 26 May 2022 23:53:58 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 26 May 2022 23:53:59 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 26 May 2022 23:54:00 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:1c74770da2ea808362085edd6dead652091b3e3d34c1e32c50015a6a5bb36c02`  
		Last Modified: Thu, 26 May 2022 23:55:21 GMT  
		Size: 4.2 MB (4227378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:988af7458b707048622e497d5ae818b77d3a24ed0295a7897ced8f003179f7f9`  
		Last Modified: Thu, 26 May 2022 23:55:21 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - windows version 10.0.17763.3287; amd64

```console
$ docker pull nats@sha256:1cedf48ffc2053a99d48b9d25a25aafa92106fbeeb92fe41aeb237d72e722664
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.8 MB (107843136 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:68f300c81963c2298e1d161245bcc24caccb02bc76fa1f665acbb465b70ff518`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 06 Aug 2022 18:08:38 GMT
RUN Apply image 10.0.17763.3287
# Wed, 10 Aug 2022 15:30:21 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 10 Aug 2022 15:30:22 GMT
RUN cmd /S /C #(nop) COPY file:88c957e774978b3592c1072a38fbf2d578a30b42e89604bf16828cccd9f86b17 in C:\nats-server.exe 
# Wed, 10 Aug 2022 15:30:23 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 10 Aug 2022 15:30:24 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 10 Aug 2022 15:30:25 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 10 Aug 2022 15:30:25 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:5c9d6483dab113d2d9b50fdf3156622aa2ec3d6faaed5664d15a5568032d1714`  
		Size: 103.2 MB (103204200 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:0a5df16ce106b092b5399678da04735c18584e4f99ea301691eb433072953e9a`  
		Last Modified: Wed, 10 Aug 2022 15:31:14 GMT  
		Size: 1.0 KB (1025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0da7ec45038de57bb4ae201762e54193e71ffc21892b700c1942bd3b85a10ac`  
		Last Modified: Wed, 10 Aug 2022 15:31:13 GMT  
		Size: 4.6 MB (4633133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d561d8a7d904db478c9c1e66aae419bb3d5333483d2d9f39f39e7bc62c02c56d`  
		Last Modified: Wed, 10 Aug 2022 15:31:12 GMT  
		Size: 1.7 KB (1653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f34e9538ca1cb2f704590a6fdaaef3b512b5ac93696534421be5f67017ffe8b9`  
		Last Modified: Wed, 10 Aug 2022 15:31:12 GMT  
		Size: 1.0 KB (1033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:660c54f5d2b9ddc91667f920a6f2103c75527be0b892d65aa55dd5bfa8afd3fe`  
		Last Modified: Wed, 10 Aug 2022 15:31:12 GMT  
		Size: 1.1 KB (1056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9356123a2a1af8afcf36b9979e254c522e7759fba29e96837a9d80c3a723f12c`  
		Last Modified: Wed, 10 Aug 2022 15:31:12 GMT  
		Size: 1.0 KB (1036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-alpine`

```console
$ docker pull nats@sha256:988010f74b61749cfb82c28b50b47d26d0b972860ce6e9325a5afcde97713da2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-alpine` - linux; amd64

```console
$ docker pull nats@sha256:f67ef794683ba4fcddc40bf871ad70eb258221443adcf1927b0270f257e73a74
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.7 MB (7701879 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57eb300f225ba4543fcd1c479ef7191723cf877d51078fa0d82de48cdff5c640`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:00 GMT
ADD file:f77e3f51f020890d22997e6c2ca98968b75b8bc8c463341a2010ff0655d4c88f in / 
# Tue, 09 Aug 2022 17:20:01 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 01:29:02 GMT
ENV NATS_SERVER=2.8.4
# Wed, 10 Aug 2022 01:29:04 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='75a53e10c640c8348bafe43300785d5147c91f60cd721c21ec896bc50727270a' ;; 		armhf) natsArch='arm6'; sha256='993a0d02ff9d0c74be31dc9e7ac1066659637c4897cc94ced2e0dc982fb428f3' ;; 		armv7) natsArch='arm7'; sha256='89e4191a0bc15c2196f2e6c1b2a3c4200576f6e8ec1176060b2a191c5e588b0d' ;; 		x86_64) natsArch='amd64'; sha256='da8c999ab0da5881fde68cba55238748d7310f28022fb78b9c07b420572a4b45' ;; 		x86) natsArch='386'; sha256='e94e5ec1076122e782527f4a98937c60c9eed4d04c6ba0364986cc58cd3ff8f8' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 10 Aug 2022 01:29:04 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 10 Aug 2022 01:29:04 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 10 Aug 2022 01:29:04 GMT
EXPOSE 4222 6222 8222
# Wed, 10 Aug 2022 01:29:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 10 Aug 2022 01:29:04 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9621f1afde84053b2f9b6ff34fc7f7460712247c01cbab483c5fa7132cf782ca`  
		Last Modified: Tue, 09 Aug 2022 17:20:52 GMT  
		Size: 2.8 MB (2823512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21c1a3defde00a6a87bb6d1f724a28b2cc109a3d0e6b086dc01265ecf07abf3b`  
		Last Modified: Wed, 10 Aug 2022 01:29:38 GMT  
		Size: 4.9 MB (4877365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d5c2bde7b7ca5bd606ae2db561e93e1addd87b05802f031fa6ec7a82f2828b0`  
		Last Modified: Wed, 10 Aug 2022 01:29:37 GMT  
		Size: 589.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a153c5b56febe9e8cc9d9df0925d160671c9aaffc633a61bdd7f368d42a1b96f`  
		Last Modified: Wed, 10 Aug 2022 01:29:37 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:91a3c5bbf8c80536df0dc91bebe4a3dbcf2901cdebb612e239a224e198e42c70
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7168331 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:87fc1a9a79541b69ed4655f072cef3d05408ecb373ad11d3a0f4c802831f0fa4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:29 GMT
ADD file:89cb25f97e17bed5c56311280efe5cfa78422d8ffbe36232195d13f94d67417e in / 
# Tue, 09 Aug 2022 17:49:29 GMT
CMD ["/bin/sh"]
# Thu, 11 Aug 2022 01:11:51 GMT
ENV NATS_SERVER=2.8.4
# Thu, 11 Aug 2022 01:11:53 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='75a53e10c640c8348bafe43300785d5147c91f60cd721c21ec896bc50727270a' ;; 		armhf) natsArch='arm6'; sha256='993a0d02ff9d0c74be31dc9e7ac1066659637c4897cc94ced2e0dc982fb428f3' ;; 		armv7) natsArch='arm7'; sha256='89e4191a0bc15c2196f2e6c1b2a3c4200576f6e8ec1176060b2a191c5e588b0d' ;; 		x86_64) natsArch='amd64'; sha256='da8c999ab0da5881fde68cba55238748d7310f28022fb78b9c07b420572a4b45' ;; 		x86) natsArch='386'; sha256='e94e5ec1076122e782527f4a98937c60c9eed4d04c6ba0364986cc58cd3ff8f8' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 11 Aug 2022 01:11:53 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 11 Aug 2022 01:11:54 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 11 Aug 2022 01:11:54 GMT
EXPOSE 4222 6222 8222
# Thu, 11 Aug 2022 01:11:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 Aug 2022 01:11:54 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:293b708aa6fb80967f27727d5c9c53ac9ba9cac376bed2ad02c17a5cca317b35`  
		Last Modified: Tue, 09 Aug 2022 17:50:52 GMT  
		Size: 2.6 MB (2631127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4efb85326bdd0b14d348830449cbdd93250414456c1d970d673f4002e8fdf93`  
		Last Modified: Thu, 11 Aug 2022 01:13:00 GMT  
		Size: 4.5 MB (4536202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef98b89db7bb29b263ede5d92c245cef1ed1dd56776120239a54f5f7692b2ff3`  
		Last Modified: Thu, 11 Aug 2022 01:13:00 GMT  
		Size: 589.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7a526f2148801e4c48011a6d1aa6ed5894b02339d145fbb462dae4f1692faa2`  
		Last Modified: Thu, 11 Aug 2022 01:13:00 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:a86957d0ea21981ed74f78c988f8b5202243dab5a43f68f0cd4d09be0e03acf7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.0 MB (6963329 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:02a19e2d0d29009797ec24843b88e7a35ebb4ca64c9a7b624b6be3290ec5f730`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 16:57:52 GMT
ADD file:0bd18306f21937a9572e68c768f05f4a9d8341b40c2379a7bfcb857c77734a14 in / 
# Tue, 09 Aug 2022 16:57:52 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 22:35:52 GMT
ENV NATS_SERVER=2.8.4
# Tue, 09 Aug 2022 22:35:55 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='75a53e10c640c8348bafe43300785d5147c91f60cd721c21ec896bc50727270a' ;; 		armhf) natsArch='arm6'; sha256='993a0d02ff9d0c74be31dc9e7ac1066659637c4897cc94ced2e0dc982fb428f3' ;; 		armv7) natsArch='arm7'; sha256='89e4191a0bc15c2196f2e6c1b2a3c4200576f6e8ec1176060b2a191c5e588b0d' ;; 		x86_64) natsArch='amd64'; sha256='da8c999ab0da5881fde68cba55238748d7310f28022fb78b9c07b420572a4b45' ;; 		x86) natsArch='386'; sha256='e94e5ec1076122e782527f4a98937c60c9eed4d04c6ba0364986cc58cd3ff8f8' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 09 Aug 2022 22:35:55 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 09 Aug 2022 22:35:55 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 09 Aug 2022 22:35:56 GMT
EXPOSE 4222 6222 8222
# Tue, 09 Aug 2022 22:35:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 09 Aug 2022 22:35:56 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:59775c20a906b1a49edcdc41a700a795998979d6ecf8f8d9cd7cbdf45e686d81`  
		Last Modified: Tue, 09 Aug 2022 16:59:12 GMT  
		Size: 2.4 MB (2435092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b55d1d06353a20f9de5b52fd408cb1d36cb23aea75e779350590565a5a4dea90`  
		Last Modified: Tue, 09 Aug 2022 22:37:42 GMT  
		Size: 4.5 MB (4527236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52e8be9dffb2c65f4e861ee01ddc4ec8362d0a2ca4ac53ad84fa5baf7b28b2d3`  
		Last Modified: Tue, 09 Aug 2022 22:37:41 GMT  
		Size: 589.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de94a2ef272b2e3ef327e7dbc685dfc8c6b58775169e3ec47a94fd5407841bf1`  
		Last Modified: Tue, 09 Aug 2022 22:37:41 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:1d7154e4491475ff8fb864a26874ba8b4b250864ad515419c96432134b79a03a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7234771 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ff14469067b8205c1030c0740c47b13a4cd70a4cb3cd3e3f02472b056353df3b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:51 GMT
ADD file:4b51a9d40f20d2beb29d0759b161d2b9403493453beb509de4e86a5d98513f16 in / 
# Tue, 09 Aug 2022 17:39:51 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 20:52:27 GMT
ENV NATS_SERVER=2.8.4
# Tue, 09 Aug 2022 20:52:29 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='75a53e10c640c8348bafe43300785d5147c91f60cd721c21ec896bc50727270a' ;; 		armhf) natsArch='arm6'; sha256='993a0d02ff9d0c74be31dc9e7ac1066659637c4897cc94ced2e0dc982fb428f3' ;; 		armv7) natsArch='arm7'; sha256='89e4191a0bc15c2196f2e6c1b2a3c4200576f6e8ec1176060b2a191c5e588b0d' ;; 		x86_64) natsArch='amd64'; sha256='da8c999ab0da5881fde68cba55238748d7310f28022fb78b9c07b420572a4b45' ;; 		x86) natsArch='386'; sha256='e94e5ec1076122e782527f4a98937c60c9eed4d04c6ba0364986cc58cd3ff8f8' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 09 Aug 2022 20:52:31 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 09 Aug 2022 20:52:32 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 09 Aug 2022 20:52:32 GMT
EXPOSE 4222 6222 8222
# Tue, 09 Aug 2022 20:52:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 09 Aug 2022 20:52:34 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:47517142f6ba87eca6b7bdca1e0df160b74671c81e4b9605dad38c1862a43be3`  
		Last Modified: Tue, 09 Aug 2022 17:40:55 GMT  
		Size: 2.7 MB (2718439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf0beb1bc3611827acd1326750497c2cc98b9160ed5aec13a1112ad88b6ba136`  
		Last Modified: Tue, 09 Aug 2022 20:53:33 GMT  
		Size: 4.5 MB (4515360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a20f9bb5cbf9bb42bf80058089fa2cc11fe7eaad0e4342ef69340f9421360e9`  
		Last Modified: Tue, 09 Aug 2022 20:53:31 GMT  
		Size: 560.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b065ba618e0c23dec2ae44bb9555ee098a0827cf44bc5f30ae1d9448e11f668`  
		Last Modified: Tue, 09 Aug 2022 20:53:31 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-alpine3.15`

```console
$ docker pull nats@sha256:988010f74b61749cfb82c28b50b47d26d0b972860ce6e9325a5afcde97713da2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-alpine3.15` - linux; amd64

```console
$ docker pull nats@sha256:f67ef794683ba4fcddc40bf871ad70eb258221443adcf1927b0270f257e73a74
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.7 MB (7701879 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57eb300f225ba4543fcd1c479ef7191723cf877d51078fa0d82de48cdff5c640`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:00 GMT
ADD file:f77e3f51f020890d22997e6c2ca98968b75b8bc8c463341a2010ff0655d4c88f in / 
# Tue, 09 Aug 2022 17:20:01 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 01:29:02 GMT
ENV NATS_SERVER=2.8.4
# Wed, 10 Aug 2022 01:29:04 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='75a53e10c640c8348bafe43300785d5147c91f60cd721c21ec896bc50727270a' ;; 		armhf) natsArch='arm6'; sha256='993a0d02ff9d0c74be31dc9e7ac1066659637c4897cc94ced2e0dc982fb428f3' ;; 		armv7) natsArch='arm7'; sha256='89e4191a0bc15c2196f2e6c1b2a3c4200576f6e8ec1176060b2a191c5e588b0d' ;; 		x86_64) natsArch='amd64'; sha256='da8c999ab0da5881fde68cba55238748d7310f28022fb78b9c07b420572a4b45' ;; 		x86) natsArch='386'; sha256='e94e5ec1076122e782527f4a98937c60c9eed4d04c6ba0364986cc58cd3ff8f8' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 10 Aug 2022 01:29:04 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 10 Aug 2022 01:29:04 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 10 Aug 2022 01:29:04 GMT
EXPOSE 4222 6222 8222
# Wed, 10 Aug 2022 01:29:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 10 Aug 2022 01:29:04 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9621f1afde84053b2f9b6ff34fc7f7460712247c01cbab483c5fa7132cf782ca`  
		Last Modified: Tue, 09 Aug 2022 17:20:52 GMT  
		Size: 2.8 MB (2823512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21c1a3defde00a6a87bb6d1f724a28b2cc109a3d0e6b086dc01265ecf07abf3b`  
		Last Modified: Wed, 10 Aug 2022 01:29:38 GMT  
		Size: 4.9 MB (4877365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d5c2bde7b7ca5bd606ae2db561e93e1addd87b05802f031fa6ec7a82f2828b0`  
		Last Modified: Wed, 10 Aug 2022 01:29:37 GMT  
		Size: 589.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a153c5b56febe9e8cc9d9df0925d160671c9aaffc633a61bdd7f368d42a1b96f`  
		Last Modified: Wed, 10 Aug 2022 01:29:37 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.15` - linux; arm variant v6

```console
$ docker pull nats@sha256:91a3c5bbf8c80536df0dc91bebe4a3dbcf2901cdebb612e239a224e198e42c70
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7168331 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:87fc1a9a79541b69ed4655f072cef3d05408ecb373ad11d3a0f4c802831f0fa4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:29 GMT
ADD file:89cb25f97e17bed5c56311280efe5cfa78422d8ffbe36232195d13f94d67417e in / 
# Tue, 09 Aug 2022 17:49:29 GMT
CMD ["/bin/sh"]
# Thu, 11 Aug 2022 01:11:51 GMT
ENV NATS_SERVER=2.8.4
# Thu, 11 Aug 2022 01:11:53 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='75a53e10c640c8348bafe43300785d5147c91f60cd721c21ec896bc50727270a' ;; 		armhf) natsArch='arm6'; sha256='993a0d02ff9d0c74be31dc9e7ac1066659637c4897cc94ced2e0dc982fb428f3' ;; 		armv7) natsArch='arm7'; sha256='89e4191a0bc15c2196f2e6c1b2a3c4200576f6e8ec1176060b2a191c5e588b0d' ;; 		x86_64) natsArch='amd64'; sha256='da8c999ab0da5881fde68cba55238748d7310f28022fb78b9c07b420572a4b45' ;; 		x86) natsArch='386'; sha256='e94e5ec1076122e782527f4a98937c60c9eed4d04c6ba0364986cc58cd3ff8f8' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 11 Aug 2022 01:11:53 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 11 Aug 2022 01:11:54 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 11 Aug 2022 01:11:54 GMT
EXPOSE 4222 6222 8222
# Thu, 11 Aug 2022 01:11:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 Aug 2022 01:11:54 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:293b708aa6fb80967f27727d5c9c53ac9ba9cac376bed2ad02c17a5cca317b35`  
		Last Modified: Tue, 09 Aug 2022 17:50:52 GMT  
		Size: 2.6 MB (2631127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4efb85326bdd0b14d348830449cbdd93250414456c1d970d673f4002e8fdf93`  
		Last Modified: Thu, 11 Aug 2022 01:13:00 GMT  
		Size: 4.5 MB (4536202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef98b89db7bb29b263ede5d92c245cef1ed1dd56776120239a54f5f7692b2ff3`  
		Last Modified: Thu, 11 Aug 2022 01:13:00 GMT  
		Size: 589.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7a526f2148801e4c48011a6d1aa6ed5894b02339d145fbb462dae4f1692faa2`  
		Last Modified: Thu, 11 Aug 2022 01:13:00 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.15` - linux; arm variant v7

```console
$ docker pull nats@sha256:a86957d0ea21981ed74f78c988f8b5202243dab5a43f68f0cd4d09be0e03acf7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.0 MB (6963329 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:02a19e2d0d29009797ec24843b88e7a35ebb4ca64c9a7b624b6be3290ec5f730`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 16:57:52 GMT
ADD file:0bd18306f21937a9572e68c768f05f4a9d8341b40c2379a7bfcb857c77734a14 in / 
# Tue, 09 Aug 2022 16:57:52 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 22:35:52 GMT
ENV NATS_SERVER=2.8.4
# Tue, 09 Aug 2022 22:35:55 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='75a53e10c640c8348bafe43300785d5147c91f60cd721c21ec896bc50727270a' ;; 		armhf) natsArch='arm6'; sha256='993a0d02ff9d0c74be31dc9e7ac1066659637c4897cc94ced2e0dc982fb428f3' ;; 		armv7) natsArch='arm7'; sha256='89e4191a0bc15c2196f2e6c1b2a3c4200576f6e8ec1176060b2a191c5e588b0d' ;; 		x86_64) natsArch='amd64'; sha256='da8c999ab0da5881fde68cba55238748d7310f28022fb78b9c07b420572a4b45' ;; 		x86) natsArch='386'; sha256='e94e5ec1076122e782527f4a98937c60c9eed4d04c6ba0364986cc58cd3ff8f8' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 09 Aug 2022 22:35:55 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 09 Aug 2022 22:35:55 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 09 Aug 2022 22:35:56 GMT
EXPOSE 4222 6222 8222
# Tue, 09 Aug 2022 22:35:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 09 Aug 2022 22:35:56 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:59775c20a906b1a49edcdc41a700a795998979d6ecf8f8d9cd7cbdf45e686d81`  
		Last Modified: Tue, 09 Aug 2022 16:59:12 GMT  
		Size: 2.4 MB (2435092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b55d1d06353a20f9de5b52fd408cb1d36cb23aea75e779350590565a5a4dea90`  
		Last Modified: Tue, 09 Aug 2022 22:37:42 GMT  
		Size: 4.5 MB (4527236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52e8be9dffb2c65f4e861ee01ddc4ec8362d0a2ca4ac53ad84fa5baf7b28b2d3`  
		Last Modified: Tue, 09 Aug 2022 22:37:41 GMT  
		Size: 589.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de94a2ef272b2e3ef327e7dbc685dfc8c6b58775169e3ec47a94fd5407841bf1`  
		Last Modified: Tue, 09 Aug 2022 22:37:41 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.15` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:1d7154e4491475ff8fb864a26874ba8b4b250864ad515419c96432134b79a03a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7234771 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ff14469067b8205c1030c0740c47b13a4cd70a4cb3cd3e3f02472b056353df3b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:51 GMT
ADD file:4b51a9d40f20d2beb29d0759b161d2b9403493453beb509de4e86a5d98513f16 in / 
# Tue, 09 Aug 2022 17:39:51 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 20:52:27 GMT
ENV NATS_SERVER=2.8.4
# Tue, 09 Aug 2022 20:52:29 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='75a53e10c640c8348bafe43300785d5147c91f60cd721c21ec896bc50727270a' ;; 		armhf) natsArch='arm6'; sha256='993a0d02ff9d0c74be31dc9e7ac1066659637c4897cc94ced2e0dc982fb428f3' ;; 		armv7) natsArch='arm7'; sha256='89e4191a0bc15c2196f2e6c1b2a3c4200576f6e8ec1176060b2a191c5e588b0d' ;; 		x86_64) natsArch='amd64'; sha256='da8c999ab0da5881fde68cba55238748d7310f28022fb78b9c07b420572a4b45' ;; 		x86) natsArch='386'; sha256='e94e5ec1076122e782527f4a98937c60c9eed4d04c6ba0364986cc58cd3ff8f8' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 09 Aug 2022 20:52:31 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 09 Aug 2022 20:52:32 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 09 Aug 2022 20:52:32 GMT
EXPOSE 4222 6222 8222
# Tue, 09 Aug 2022 20:52:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 09 Aug 2022 20:52:34 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:47517142f6ba87eca6b7bdca1e0df160b74671c81e4b9605dad38c1862a43be3`  
		Last Modified: Tue, 09 Aug 2022 17:40:55 GMT  
		Size: 2.7 MB (2718439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf0beb1bc3611827acd1326750497c2cc98b9160ed5aec13a1112ad88b6ba136`  
		Last Modified: Tue, 09 Aug 2022 20:53:33 GMT  
		Size: 4.5 MB (4515360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a20f9bb5cbf9bb42bf80058089fa2cc11fe7eaad0e4342ef69340f9421360e9`  
		Last Modified: Tue, 09 Aug 2022 20:53:31 GMT  
		Size: 560.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b065ba618e0c23dec2ae44bb9555ee098a0827cf44bc5f30ae1d9448e11f668`  
		Last Modified: Tue, 09 Aug 2022 20:53:31 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-linux`

```console
$ docker pull nats@sha256:95b20a1c366e503cd8c0b97a45f2b00d70adfa53f7482237d1ef8fa2e792d2cf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-linux` - linux; amd64

```console
$ docker pull nats@sha256:796298f636925dedbbdfa537f42423dffd3a69b70c3a9bf4fd0982886a4b745d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4591595 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:842c053e15bdb38e697668b1f0721313203f7c2297eb6d79000f20858dc97854`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 27 May 2022 00:38:26 GMT
COPY file:c866dea678e8cec7cbd0798a1dbdefc45e992d9df374709f6000bac517589a1b in /nats-server 
# Fri, 27 May 2022 00:38:26 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 27 May 2022 00:38:27 GMT
EXPOSE 4222 6222 8222
# Fri, 27 May 2022 00:38:27 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 27 May 2022 00:38:27 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 27 May 2022 00:38:27 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:5e5797f39fa0527a3dd0a137353b40f97c71134e7eb38373d9791c5f1392885b`  
		Last Modified: Fri, 27 May 2022 00:39:15 GMT  
		Size: 4.6 MB (4591087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28c3b732adf61929b0b23ca08934cd89923e9cd9d7061544e76bbce57a9fa1e4`  
		Last Modified: Fri, 27 May 2022 00:39:14 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:e0c28a95cdf6dd8a566d5c2394d09e6141dffb9107fe49f9385d6f19048bd955
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4245827 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cef47371f249bc862484ca7bd4dde2d7f77dc41bcb49cc49cceb17dfb2d4471f`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 11 Aug 2022 01:12:06 GMT
COPY file:8de8b0cf8e6edf54e413c112cd66aed537abed387a26ba749a9293d43cdf6594 in /nats-server 
# Thu, 11 Aug 2022 01:12:06 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 11 Aug 2022 01:12:06 GMT
EXPOSE 4222 6222 8222
# Thu, 11 Aug 2022 01:12:06 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 11 Aug 2022 01:12:06 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 11 Aug 2022 01:12:06 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:770fa9c168613edbe7aa7007d2cf8492c6570efc1ddab217fa32772c6b72dd48`  
		Last Modified: Thu, 26 May 2022 23:58:21 GMT  
		Size: 4.2 MB (4245317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bde47aae170f9c7e50b7bbea164ec0e0d02b9c05b603e7f7554e163183c02cd9`  
		Last Modified: Thu, 11 Aug 2022 01:13:30 GMT  
		Size: 510.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:453c8fea5d37abc60f034f80bdb668a48c8e4f0900fce8b55fdb6ae7f2908d07
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4242795 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:508b00336aa0fc72bd1c3d33e5f447d1411e47221dfa1fa6085d6986b27045d7`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 22:36:22 GMT
COPY file:2841d6664b8897473f39b595b9aa4b28e749f587dc1afa4a0027ae507f37ee1f in /nats-server 
# Tue, 09 Aug 2022 22:36:22 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 09 Aug 2022 22:36:22 GMT
EXPOSE 4222 6222 8222
# Tue, 09 Aug 2022 22:36:22 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 09 Aug 2022 22:36:23 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 09 Aug 2022 22:36:23 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:f533e6e439ee51f1cf94458f821a20ed162b542d356340957091882ad881d5c1`  
		Last Modified: Fri, 27 May 2022 00:28:16 GMT  
		Size: 4.2 MB (4242287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:274ba9becbe1086958e9d56ab9452ec01f7fad6e3e68a34c49f1f299a5eab1ac`  
		Last Modified: Tue, 09 Aug 2022 22:38:14 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:87b1afbd78a75ee48cb6b37a8522bbb01f5e9b5047b095b16cc4f241774a48d1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4227885 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9bce5ae01237736c7e0447d8cd1b2dbe252eab3ab5ac3b05d98b646b2575cee`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 26 May 2022 23:53:56 GMT
COPY file:2dbd94c6c11f89ceba3241f1efe469d0a06f0aae91abb77f3d79756676d0be57 in /nats-server 
# Thu, 26 May 2022 23:53:57 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 26 May 2022 23:53:57 GMT
EXPOSE 4222 6222 8222
# Thu, 26 May 2022 23:53:58 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 26 May 2022 23:53:59 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 26 May 2022 23:54:00 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:1c74770da2ea808362085edd6dead652091b3e3d34c1e32c50015a6a5bb36c02`  
		Last Modified: Thu, 26 May 2022 23:55:21 GMT  
		Size: 4.2 MB (4227378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:988af7458b707048622e497d5ae818b77d3a24ed0295a7897ced8f003179f7f9`  
		Last Modified: Thu, 26 May 2022 23:55:21 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-nanoserver`

```console
$ docker pull nats@sha256:92865bb073a2a8994aa5a8428fb857b4885c97d5c4af51ea7bdc5a56a93d4c69
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3287; amd64

### `nats:2-nanoserver` - windows version 10.0.17763.3287; amd64

```console
$ docker pull nats@sha256:1cedf48ffc2053a99d48b9d25a25aafa92106fbeeb92fe41aeb237d72e722664
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.8 MB (107843136 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:68f300c81963c2298e1d161245bcc24caccb02bc76fa1f665acbb465b70ff518`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 06 Aug 2022 18:08:38 GMT
RUN Apply image 10.0.17763.3287
# Wed, 10 Aug 2022 15:30:21 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 10 Aug 2022 15:30:22 GMT
RUN cmd /S /C #(nop) COPY file:88c957e774978b3592c1072a38fbf2d578a30b42e89604bf16828cccd9f86b17 in C:\nats-server.exe 
# Wed, 10 Aug 2022 15:30:23 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 10 Aug 2022 15:30:24 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 10 Aug 2022 15:30:25 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 10 Aug 2022 15:30:25 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:5c9d6483dab113d2d9b50fdf3156622aa2ec3d6faaed5664d15a5568032d1714`  
		Size: 103.2 MB (103204200 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:0a5df16ce106b092b5399678da04735c18584e4f99ea301691eb433072953e9a`  
		Last Modified: Wed, 10 Aug 2022 15:31:14 GMT  
		Size: 1.0 KB (1025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0da7ec45038de57bb4ae201762e54193e71ffc21892b700c1942bd3b85a10ac`  
		Last Modified: Wed, 10 Aug 2022 15:31:13 GMT  
		Size: 4.6 MB (4633133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d561d8a7d904db478c9c1e66aae419bb3d5333483d2d9f39f39e7bc62c02c56d`  
		Last Modified: Wed, 10 Aug 2022 15:31:12 GMT  
		Size: 1.7 KB (1653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f34e9538ca1cb2f704590a6fdaaef3b512b5ac93696534421be5f67017ffe8b9`  
		Last Modified: Wed, 10 Aug 2022 15:31:12 GMT  
		Size: 1.0 KB (1033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:660c54f5d2b9ddc91667f920a6f2103c75527be0b892d65aa55dd5bfa8afd3fe`  
		Last Modified: Wed, 10 Aug 2022 15:31:12 GMT  
		Size: 1.1 KB (1056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9356123a2a1af8afcf36b9979e254c522e7759fba29e96837a9d80c3a723f12c`  
		Last Modified: Wed, 10 Aug 2022 15:31:12 GMT  
		Size: 1.0 KB (1036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-nanoserver-1809`

```console
$ docker pull nats@sha256:92865bb073a2a8994aa5a8428fb857b4885c97d5c4af51ea7bdc5a56a93d4c69
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3287; amd64

### `nats:2-nanoserver-1809` - windows version 10.0.17763.3287; amd64

```console
$ docker pull nats@sha256:1cedf48ffc2053a99d48b9d25a25aafa92106fbeeb92fe41aeb237d72e722664
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.8 MB (107843136 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:68f300c81963c2298e1d161245bcc24caccb02bc76fa1f665acbb465b70ff518`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 06 Aug 2022 18:08:38 GMT
RUN Apply image 10.0.17763.3287
# Wed, 10 Aug 2022 15:30:21 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 10 Aug 2022 15:30:22 GMT
RUN cmd /S /C #(nop) COPY file:88c957e774978b3592c1072a38fbf2d578a30b42e89604bf16828cccd9f86b17 in C:\nats-server.exe 
# Wed, 10 Aug 2022 15:30:23 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 10 Aug 2022 15:30:24 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 10 Aug 2022 15:30:25 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 10 Aug 2022 15:30:25 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:5c9d6483dab113d2d9b50fdf3156622aa2ec3d6faaed5664d15a5568032d1714`  
		Size: 103.2 MB (103204200 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:0a5df16ce106b092b5399678da04735c18584e4f99ea301691eb433072953e9a`  
		Last Modified: Wed, 10 Aug 2022 15:31:14 GMT  
		Size: 1.0 KB (1025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0da7ec45038de57bb4ae201762e54193e71ffc21892b700c1942bd3b85a10ac`  
		Last Modified: Wed, 10 Aug 2022 15:31:13 GMT  
		Size: 4.6 MB (4633133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d561d8a7d904db478c9c1e66aae419bb3d5333483d2d9f39f39e7bc62c02c56d`  
		Last Modified: Wed, 10 Aug 2022 15:31:12 GMT  
		Size: 1.7 KB (1653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f34e9538ca1cb2f704590a6fdaaef3b512b5ac93696534421be5f67017ffe8b9`  
		Last Modified: Wed, 10 Aug 2022 15:31:12 GMT  
		Size: 1.0 KB (1033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:660c54f5d2b9ddc91667f920a6f2103c75527be0b892d65aa55dd5bfa8afd3fe`  
		Last Modified: Wed, 10 Aug 2022 15:31:12 GMT  
		Size: 1.1 KB (1056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9356123a2a1af8afcf36b9979e254c522e7759fba29e96837a9d80c3a723f12c`  
		Last Modified: Wed, 10 Aug 2022 15:31:12 GMT  
		Size: 1.0 KB (1036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-scratch`

```console
$ docker pull nats@sha256:95b20a1c366e503cd8c0b97a45f2b00d70adfa53f7482237d1ef8fa2e792d2cf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-scratch` - linux; amd64

```console
$ docker pull nats@sha256:796298f636925dedbbdfa537f42423dffd3a69b70c3a9bf4fd0982886a4b745d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4591595 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:842c053e15bdb38e697668b1f0721313203f7c2297eb6d79000f20858dc97854`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 27 May 2022 00:38:26 GMT
COPY file:c866dea678e8cec7cbd0798a1dbdefc45e992d9df374709f6000bac517589a1b in /nats-server 
# Fri, 27 May 2022 00:38:26 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 27 May 2022 00:38:27 GMT
EXPOSE 4222 6222 8222
# Fri, 27 May 2022 00:38:27 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 27 May 2022 00:38:27 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 27 May 2022 00:38:27 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:5e5797f39fa0527a3dd0a137353b40f97c71134e7eb38373d9791c5f1392885b`  
		Last Modified: Fri, 27 May 2022 00:39:15 GMT  
		Size: 4.6 MB (4591087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28c3b732adf61929b0b23ca08934cd89923e9cd9d7061544e76bbce57a9fa1e4`  
		Last Modified: Fri, 27 May 2022 00:39:14 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:e0c28a95cdf6dd8a566d5c2394d09e6141dffb9107fe49f9385d6f19048bd955
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4245827 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cef47371f249bc862484ca7bd4dde2d7f77dc41bcb49cc49cceb17dfb2d4471f`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 11 Aug 2022 01:12:06 GMT
COPY file:8de8b0cf8e6edf54e413c112cd66aed537abed387a26ba749a9293d43cdf6594 in /nats-server 
# Thu, 11 Aug 2022 01:12:06 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 11 Aug 2022 01:12:06 GMT
EXPOSE 4222 6222 8222
# Thu, 11 Aug 2022 01:12:06 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 11 Aug 2022 01:12:06 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 11 Aug 2022 01:12:06 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:770fa9c168613edbe7aa7007d2cf8492c6570efc1ddab217fa32772c6b72dd48`  
		Last Modified: Thu, 26 May 2022 23:58:21 GMT  
		Size: 4.2 MB (4245317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bde47aae170f9c7e50b7bbea164ec0e0d02b9c05b603e7f7554e163183c02cd9`  
		Last Modified: Thu, 11 Aug 2022 01:13:30 GMT  
		Size: 510.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:453c8fea5d37abc60f034f80bdb668a48c8e4f0900fce8b55fdb6ae7f2908d07
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4242795 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:508b00336aa0fc72bd1c3d33e5f447d1411e47221dfa1fa6085d6986b27045d7`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 22:36:22 GMT
COPY file:2841d6664b8897473f39b595b9aa4b28e749f587dc1afa4a0027ae507f37ee1f in /nats-server 
# Tue, 09 Aug 2022 22:36:22 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 09 Aug 2022 22:36:22 GMT
EXPOSE 4222 6222 8222
# Tue, 09 Aug 2022 22:36:22 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 09 Aug 2022 22:36:23 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 09 Aug 2022 22:36:23 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:f533e6e439ee51f1cf94458f821a20ed162b542d356340957091882ad881d5c1`  
		Last Modified: Fri, 27 May 2022 00:28:16 GMT  
		Size: 4.2 MB (4242287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:274ba9becbe1086958e9d56ab9452ec01f7fad6e3e68a34c49f1f299a5eab1ac`  
		Last Modified: Tue, 09 Aug 2022 22:38:14 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:87b1afbd78a75ee48cb6b37a8522bbb01f5e9b5047b095b16cc4f241774a48d1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4227885 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9bce5ae01237736c7e0447d8cd1b2dbe252eab3ab5ac3b05d98b646b2575cee`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 26 May 2022 23:53:56 GMT
COPY file:2dbd94c6c11f89ceba3241f1efe469d0a06f0aae91abb77f3d79756676d0be57 in /nats-server 
# Thu, 26 May 2022 23:53:57 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 26 May 2022 23:53:57 GMT
EXPOSE 4222 6222 8222
# Thu, 26 May 2022 23:53:58 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 26 May 2022 23:53:59 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 26 May 2022 23:54:00 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:1c74770da2ea808362085edd6dead652091b3e3d34c1e32c50015a6a5bb36c02`  
		Last Modified: Thu, 26 May 2022 23:55:21 GMT  
		Size: 4.2 MB (4227378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:988af7458b707048622e497d5ae818b77d3a24ed0295a7897ced8f003179f7f9`  
		Last Modified: Thu, 26 May 2022 23:55:21 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-windowsservercore`

```console
$ docker pull nats@sha256:01e61321ee0c2a556640c7b04f8aaf24a2e46524bdec3c3b451c81dd170d0825
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3287; amd64

### `nats:2-windowsservercore` - windows version 10.0.17763.3287; amd64

```console
$ docker pull nats@sha256:9d7b29f769b82966a826e9eebcbff7022824cb343278b2c9dd87014b310f6bc2
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2683024603 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db44bc7e8ad93293de37107a4b87601bb8241a7d0762deac86c4a40d5ef262f0`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 06 Aug 2022 18:30:32 GMT
RUN Install update 10.0.17763.3287
# Wed, 10 Aug 2022 13:44:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Aug 2022 15:27:50 GMT
ENV NATS_DOCKERIZED=1
# Wed, 10 Aug 2022 15:27:51 GMT
ENV NATS_SERVER=2.8.4
# Wed, 10 Aug 2022 15:27:52 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.8.4/nats-server-v2.8.4-windows-amd64.zip
# Wed, 10 Aug 2022 15:27:53 GMT
ENV NATS_SERVER_SHASUM=911e8b77cf288c6e0997891d1400e5cc59dedd928e8f1685650c468674b52dc8
# Wed, 10 Aug 2022 15:28:46 GMT
RUN Set-PSDebug -Trace 2
# Wed, 10 Aug 2022 15:30:06 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 10 Aug 2022 15:30:07 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 10 Aug 2022 15:30:08 GMT
EXPOSE 4222 6222 8222
# Wed, 10 Aug 2022 15:30:09 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 10 Aug 2022 15:30:09 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:294d77ac553d7210b662d07674ef9e39a6c2e88dc15b9d2788d51e509bc8b54e`  
		Size: 800.5 MB (800546641 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:da71148bcd96afa7027d6172acee93aad6002bfbe87cadf468260667c09b3a89`  
		Last Modified: Wed, 10 Aug 2022 15:05:54 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26dc1c1069568772f0068cef343e37284e5f5e488dbfc15e037d95bce032d917`  
		Last Modified: Wed, 10 Aug 2022 15:30:56 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:890750ec51eb48085268f820e86c5b7ff873ff61875ed2b5df77150e4f667aff`  
		Last Modified: Wed, 10 Aug 2022 15:30:55 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da392874ede7ff085d580701bc4800047c2c07531b8dfb625241622eaba1995c`  
		Last Modified: Wed, 10 Aug 2022 15:30:55 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5a137a2c60ae08a2536eb110f4f21b9c80f33a03ab2d732da15f5f3de36c588`  
		Last Modified: Wed, 10 Aug 2022 15:30:55 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94cf94feb41446a9b0f0b35e7d386675c5b6256a8123327795d03d29f60b9400`  
		Last Modified: Wed, 10 Aug 2022 15:30:55 GMT  
		Size: 340.8 KB (340788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ab22594d9c79ecf05870151796e0c4df02facc4a9c10e99fcbea268fcbe9886`  
		Last Modified: Wed, 10 Aug 2022 15:30:53 GMT  
		Size: 5.0 MB (4957679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:143ae888a3c2d7c0f27e7935a85c8a25ef108bb2421c597eea07c8283cf18cbd`  
		Last Modified: Wed, 10 Aug 2022 15:30:52 GMT  
		Size: 2.0 KB (1996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b16fcb36242a120d1667323616c739921e5e2ccd627ea85b09d12df62368dc62`  
		Last Modified: Wed, 10 Aug 2022 15:30:53 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:478c487cdfd4835865c12e472c096f810ceb98ae9fa4d8a77c2080b01e22f095`  
		Last Modified: Wed, 10 Aug 2022 15:30:52 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2414c1290a3b460fc321c6c8630ddd4386a1f7192c489baca687f6ce4bd010e`  
		Last Modified: Wed, 10 Aug 2022 15:30:52 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-windowsservercore-1809`

```console
$ docker pull nats@sha256:01e61321ee0c2a556640c7b04f8aaf24a2e46524bdec3c3b451c81dd170d0825
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3287; amd64

### `nats:2-windowsservercore-1809` - windows version 10.0.17763.3287; amd64

```console
$ docker pull nats@sha256:9d7b29f769b82966a826e9eebcbff7022824cb343278b2c9dd87014b310f6bc2
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2683024603 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db44bc7e8ad93293de37107a4b87601bb8241a7d0762deac86c4a40d5ef262f0`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 06 Aug 2022 18:30:32 GMT
RUN Install update 10.0.17763.3287
# Wed, 10 Aug 2022 13:44:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Aug 2022 15:27:50 GMT
ENV NATS_DOCKERIZED=1
# Wed, 10 Aug 2022 15:27:51 GMT
ENV NATS_SERVER=2.8.4
# Wed, 10 Aug 2022 15:27:52 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.8.4/nats-server-v2.8.4-windows-amd64.zip
# Wed, 10 Aug 2022 15:27:53 GMT
ENV NATS_SERVER_SHASUM=911e8b77cf288c6e0997891d1400e5cc59dedd928e8f1685650c468674b52dc8
# Wed, 10 Aug 2022 15:28:46 GMT
RUN Set-PSDebug -Trace 2
# Wed, 10 Aug 2022 15:30:06 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 10 Aug 2022 15:30:07 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 10 Aug 2022 15:30:08 GMT
EXPOSE 4222 6222 8222
# Wed, 10 Aug 2022 15:30:09 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 10 Aug 2022 15:30:09 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:294d77ac553d7210b662d07674ef9e39a6c2e88dc15b9d2788d51e509bc8b54e`  
		Size: 800.5 MB (800546641 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:da71148bcd96afa7027d6172acee93aad6002bfbe87cadf468260667c09b3a89`  
		Last Modified: Wed, 10 Aug 2022 15:05:54 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26dc1c1069568772f0068cef343e37284e5f5e488dbfc15e037d95bce032d917`  
		Last Modified: Wed, 10 Aug 2022 15:30:56 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:890750ec51eb48085268f820e86c5b7ff873ff61875ed2b5df77150e4f667aff`  
		Last Modified: Wed, 10 Aug 2022 15:30:55 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da392874ede7ff085d580701bc4800047c2c07531b8dfb625241622eaba1995c`  
		Last Modified: Wed, 10 Aug 2022 15:30:55 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5a137a2c60ae08a2536eb110f4f21b9c80f33a03ab2d732da15f5f3de36c588`  
		Last Modified: Wed, 10 Aug 2022 15:30:55 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94cf94feb41446a9b0f0b35e7d386675c5b6256a8123327795d03d29f60b9400`  
		Last Modified: Wed, 10 Aug 2022 15:30:55 GMT  
		Size: 340.8 KB (340788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ab22594d9c79ecf05870151796e0c4df02facc4a9c10e99fcbea268fcbe9886`  
		Last Modified: Wed, 10 Aug 2022 15:30:53 GMT  
		Size: 5.0 MB (4957679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:143ae888a3c2d7c0f27e7935a85c8a25ef108bb2421c597eea07c8283cf18cbd`  
		Last Modified: Wed, 10 Aug 2022 15:30:52 GMT  
		Size: 2.0 KB (1996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b16fcb36242a120d1667323616c739921e5e2ccd627ea85b09d12df62368dc62`  
		Last Modified: Wed, 10 Aug 2022 15:30:53 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:478c487cdfd4835865c12e472c096f810ceb98ae9fa4d8a77c2080b01e22f095`  
		Last Modified: Wed, 10 Aug 2022 15:30:52 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2414c1290a3b460fc321c6c8630ddd4386a1f7192c489baca687f6ce4bd010e`  
		Last Modified: Wed, 10 Aug 2022 15:30:52 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.8`

```console
$ docker pull nats@sha256:8f0cdcbc4c3597443fce869e75a759edb0d5a93fe98078f470a43204a6d7a729
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.3287; amd64

### `nats:2.8` - linux; amd64

```console
$ docker pull nats@sha256:796298f636925dedbbdfa537f42423dffd3a69b70c3a9bf4fd0982886a4b745d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4591595 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:842c053e15bdb38e697668b1f0721313203f7c2297eb6d79000f20858dc97854`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 27 May 2022 00:38:26 GMT
COPY file:c866dea678e8cec7cbd0798a1dbdefc45e992d9df374709f6000bac517589a1b in /nats-server 
# Fri, 27 May 2022 00:38:26 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 27 May 2022 00:38:27 GMT
EXPOSE 4222 6222 8222
# Fri, 27 May 2022 00:38:27 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 27 May 2022 00:38:27 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 27 May 2022 00:38:27 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:5e5797f39fa0527a3dd0a137353b40f97c71134e7eb38373d9791c5f1392885b`  
		Last Modified: Fri, 27 May 2022 00:39:15 GMT  
		Size: 4.6 MB (4591087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28c3b732adf61929b0b23ca08934cd89923e9cd9d7061544e76bbce57a9fa1e4`  
		Last Modified: Fri, 27 May 2022 00:39:14 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.8` - linux; arm variant v6

```console
$ docker pull nats@sha256:e0c28a95cdf6dd8a566d5c2394d09e6141dffb9107fe49f9385d6f19048bd955
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4245827 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cef47371f249bc862484ca7bd4dde2d7f77dc41bcb49cc49cceb17dfb2d4471f`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 11 Aug 2022 01:12:06 GMT
COPY file:8de8b0cf8e6edf54e413c112cd66aed537abed387a26ba749a9293d43cdf6594 in /nats-server 
# Thu, 11 Aug 2022 01:12:06 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 11 Aug 2022 01:12:06 GMT
EXPOSE 4222 6222 8222
# Thu, 11 Aug 2022 01:12:06 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 11 Aug 2022 01:12:06 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 11 Aug 2022 01:12:06 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:770fa9c168613edbe7aa7007d2cf8492c6570efc1ddab217fa32772c6b72dd48`  
		Last Modified: Thu, 26 May 2022 23:58:21 GMT  
		Size: 4.2 MB (4245317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bde47aae170f9c7e50b7bbea164ec0e0d02b9c05b603e7f7554e163183c02cd9`  
		Last Modified: Thu, 11 Aug 2022 01:13:30 GMT  
		Size: 510.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.8` - linux; arm variant v7

```console
$ docker pull nats@sha256:453c8fea5d37abc60f034f80bdb668a48c8e4f0900fce8b55fdb6ae7f2908d07
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4242795 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:508b00336aa0fc72bd1c3d33e5f447d1411e47221dfa1fa6085d6986b27045d7`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 22:36:22 GMT
COPY file:2841d6664b8897473f39b595b9aa4b28e749f587dc1afa4a0027ae507f37ee1f in /nats-server 
# Tue, 09 Aug 2022 22:36:22 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 09 Aug 2022 22:36:22 GMT
EXPOSE 4222 6222 8222
# Tue, 09 Aug 2022 22:36:22 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 09 Aug 2022 22:36:23 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 09 Aug 2022 22:36:23 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:f533e6e439ee51f1cf94458f821a20ed162b542d356340957091882ad881d5c1`  
		Last Modified: Fri, 27 May 2022 00:28:16 GMT  
		Size: 4.2 MB (4242287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:274ba9becbe1086958e9d56ab9452ec01f7fad6e3e68a34c49f1f299a5eab1ac`  
		Last Modified: Tue, 09 Aug 2022 22:38:14 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.8` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:87b1afbd78a75ee48cb6b37a8522bbb01f5e9b5047b095b16cc4f241774a48d1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4227885 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9bce5ae01237736c7e0447d8cd1b2dbe252eab3ab5ac3b05d98b646b2575cee`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 26 May 2022 23:53:56 GMT
COPY file:2dbd94c6c11f89ceba3241f1efe469d0a06f0aae91abb77f3d79756676d0be57 in /nats-server 
# Thu, 26 May 2022 23:53:57 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 26 May 2022 23:53:57 GMT
EXPOSE 4222 6222 8222
# Thu, 26 May 2022 23:53:58 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 26 May 2022 23:53:59 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 26 May 2022 23:54:00 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:1c74770da2ea808362085edd6dead652091b3e3d34c1e32c50015a6a5bb36c02`  
		Last Modified: Thu, 26 May 2022 23:55:21 GMT  
		Size: 4.2 MB (4227378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:988af7458b707048622e497d5ae818b77d3a24ed0295a7897ced8f003179f7f9`  
		Last Modified: Thu, 26 May 2022 23:55:21 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.8` - windows version 10.0.17763.3287; amd64

```console
$ docker pull nats@sha256:1cedf48ffc2053a99d48b9d25a25aafa92106fbeeb92fe41aeb237d72e722664
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.8 MB (107843136 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:68f300c81963c2298e1d161245bcc24caccb02bc76fa1f665acbb465b70ff518`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 06 Aug 2022 18:08:38 GMT
RUN Apply image 10.0.17763.3287
# Wed, 10 Aug 2022 15:30:21 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 10 Aug 2022 15:30:22 GMT
RUN cmd /S /C #(nop) COPY file:88c957e774978b3592c1072a38fbf2d578a30b42e89604bf16828cccd9f86b17 in C:\nats-server.exe 
# Wed, 10 Aug 2022 15:30:23 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 10 Aug 2022 15:30:24 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 10 Aug 2022 15:30:25 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 10 Aug 2022 15:30:25 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:5c9d6483dab113d2d9b50fdf3156622aa2ec3d6faaed5664d15a5568032d1714`  
		Size: 103.2 MB (103204200 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:0a5df16ce106b092b5399678da04735c18584e4f99ea301691eb433072953e9a`  
		Last Modified: Wed, 10 Aug 2022 15:31:14 GMT  
		Size: 1.0 KB (1025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0da7ec45038de57bb4ae201762e54193e71ffc21892b700c1942bd3b85a10ac`  
		Last Modified: Wed, 10 Aug 2022 15:31:13 GMT  
		Size: 4.6 MB (4633133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d561d8a7d904db478c9c1e66aae419bb3d5333483d2d9f39f39e7bc62c02c56d`  
		Last Modified: Wed, 10 Aug 2022 15:31:12 GMT  
		Size: 1.7 KB (1653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f34e9538ca1cb2f704590a6fdaaef3b512b5ac93696534421be5f67017ffe8b9`  
		Last Modified: Wed, 10 Aug 2022 15:31:12 GMT  
		Size: 1.0 KB (1033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:660c54f5d2b9ddc91667f920a6f2103c75527be0b892d65aa55dd5bfa8afd3fe`  
		Last Modified: Wed, 10 Aug 2022 15:31:12 GMT  
		Size: 1.1 KB (1056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9356123a2a1af8afcf36b9979e254c522e7759fba29e96837a9d80c3a723f12c`  
		Last Modified: Wed, 10 Aug 2022 15:31:12 GMT  
		Size: 1.0 KB (1036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.8-alpine`

```console
$ docker pull nats@sha256:988010f74b61749cfb82c28b50b47d26d0b972860ce6e9325a5afcde97713da2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.8-alpine` - linux; amd64

```console
$ docker pull nats@sha256:f67ef794683ba4fcddc40bf871ad70eb258221443adcf1927b0270f257e73a74
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.7 MB (7701879 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57eb300f225ba4543fcd1c479ef7191723cf877d51078fa0d82de48cdff5c640`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:00 GMT
ADD file:f77e3f51f020890d22997e6c2ca98968b75b8bc8c463341a2010ff0655d4c88f in / 
# Tue, 09 Aug 2022 17:20:01 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 01:29:02 GMT
ENV NATS_SERVER=2.8.4
# Wed, 10 Aug 2022 01:29:04 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='75a53e10c640c8348bafe43300785d5147c91f60cd721c21ec896bc50727270a' ;; 		armhf) natsArch='arm6'; sha256='993a0d02ff9d0c74be31dc9e7ac1066659637c4897cc94ced2e0dc982fb428f3' ;; 		armv7) natsArch='arm7'; sha256='89e4191a0bc15c2196f2e6c1b2a3c4200576f6e8ec1176060b2a191c5e588b0d' ;; 		x86_64) natsArch='amd64'; sha256='da8c999ab0da5881fde68cba55238748d7310f28022fb78b9c07b420572a4b45' ;; 		x86) natsArch='386'; sha256='e94e5ec1076122e782527f4a98937c60c9eed4d04c6ba0364986cc58cd3ff8f8' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 10 Aug 2022 01:29:04 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 10 Aug 2022 01:29:04 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 10 Aug 2022 01:29:04 GMT
EXPOSE 4222 6222 8222
# Wed, 10 Aug 2022 01:29:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 10 Aug 2022 01:29:04 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9621f1afde84053b2f9b6ff34fc7f7460712247c01cbab483c5fa7132cf782ca`  
		Last Modified: Tue, 09 Aug 2022 17:20:52 GMT  
		Size: 2.8 MB (2823512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21c1a3defde00a6a87bb6d1f724a28b2cc109a3d0e6b086dc01265ecf07abf3b`  
		Last Modified: Wed, 10 Aug 2022 01:29:38 GMT  
		Size: 4.9 MB (4877365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d5c2bde7b7ca5bd606ae2db561e93e1addd87b05802f031fa6ec7a82f2828b0`  
		Last Modified: Wed, 10 Aug 2022 01:29:37 GMT  
		Size: 589.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a153c5b56febe9e8cc9d9df0925d160671c9aaffc633a61bdd7f368d42a1b96f`  
		Last Modified: Wed, 10 Aug 2022 01:29:37 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.8-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:91a3c5bbf8c80536df0dc91bebe4a3dbcf2901cdebb612e239a224e198e42c70
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7168331 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:87fc1a9a79541b69ed4655f072cef3d05408ecb373ad11d3a0f4c802831f0fa4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:29 GMT
ADD file:89cb25f97e17bed5c56311280efe5cfa78422d8ffbe36232195d13f94d67417e in / 
# Tue, 09 Aug 2022 17:49:29 GMT
CMD ["/bin/sh"]
# Thu, 11 Aug 2022 01:11:51 GMT
ENV NATS_SERVER=2.8.4
# Thu, 11 Aug 2022 01:11:53 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='75a53e10c640c8348bafe43300785d5147c91f60cd721c21ec896bc50727270a' ;; 		armhf) natsArch='arm6'; sha256='993a0d02ff9d0c74be31dc9e7ac1066659637c4897cc94ced2e0dc982fb428f3' ;; 		armv7) natsArch='arm7'; sha256='89e4191a0bc15c2196f2e6c1b2a3c4200576f6e8ec1176060b2a191c5e588b0d' ;; 		x86_64) natsArch='amd64'; sha256='da8c999ab0da5881fde68cba55238748d7310f28022fb78b9c07b420572a4b45' ;; 		x86) natsArch='386'; sha256='e94e5ec1076122e782527f4a98937c60c9eed4d04c6ba0364986cc58cd3ff8f8' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 11 Aug 2022 01:11:53 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 11 Aug 2022 01:11:54 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 11 Aug 2022 01:11:54 GMT
EXPOSE 4222 6222 8222
# Thu, 11 Aug 2022 01:11:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 Aug 2022 01:11:54 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:293b708aa6fb80967f27727d5c9c53ac9ba9cac376bed2ad02c17a5cca317b35`  
		Last Modified: Tue, 09 Aug 2022 17:50:52 GMT  
		Size: 2.6 MB (2631127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4efb85326bdd0b14d348830449cbdd93250414456c1d970d673f4002e8fdf93`  
		Last Modified: Thu, 11 Aug 2022 01:13:00 GMT  
		Size: 4.5 MB (4536202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef98b89db7bb29b263ede5d92c245cef1ed1dd56776120239a54f5f7692b2ff3`  
		Last Modified: Thu, 11 Aug 2022 01:13:00 GMT  
		Size: 589.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7a526f2148801e4c48011a6d1aa6ed5894b02339d145fbb462dae4f1692faa2`  
		Last Modified: Thu, 11 Aug 2022 01:13:00 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.8-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:a86957d0ea21981ed74f78c988f8b5202243dab5a43f68f0cd4d09be0e03acf7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.0 MB (6963329 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:02a19e2d0d29009797ec24843b88e7a35ebb4ca64c9a7b624b6be3290ec5f730`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 16:57:52 GMT
ADD file:0bd18306f21937a9572e68c768f05f4a9d8341b40c2379a7bfcb857c77734a14 in / 
# Tue, 09 Aug 2022 16:57:52 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 22:35:52 GMT
ENV NATS_SERVER=2.8.4
# Tue, 09 Aug 2022 22:35:55 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='75a53e10c640c8348bafe43300785d5147c91f60cd721c21ec896bc50727270a' ;; 		armhf) natsArch='arm6'; sha256='993a0d02ff9d0c74be31dc9e7ac1066659637c4897cc94ced2e0dc982fb428f3' ;; 		armv7) natsArch='arm7'; sha256='89e4191a0bc15c2196f2e6c1b2a3c4200576f6e8ec1176060b2a191c5e588b0d' ;; 		x86_64) natsArch='amd64'; sha256='da8c999ab0da5881fde68cba55238748d7310f28022fb78b9c07b420572a4b45' ;; 		x86) natsArch='386'; sha256='e94e5ec1076122e782527f4a98937c60c9eed4d04c6ba0364986cc58cd3ff8f8' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 09 Aug 2022 22:35:55 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 09 Aug 2022 22:35:55 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 09 Aug 2022 22:35:56 GMT
EXPOSE 4222 6222 8222
# Tue, 09 Aug 2022 22:35:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 09 Aug 2022 22:35:56 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:59775c20a906b1a49edcdc41a700a795998979d6ecf8f8d9cd7cbdf45e686d81`  
		Last Modified: Tue, 09 Aug 2022 16:59:12 GMT  
		Size: 2.4 MB (2435092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b55d1d06353a20f9de5b52fd408cb1d36cb23aea75e779350590565a5a4dea90`  
		Last Modified: Tue, 09 Aug 2022 22:37:42 GMT  
		Size: 4.5 MB (4527236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52e8be9dffb2c65f4e861ee01ddc4ec8362d0a2ca4ac53ad84fa5baf7b28b2d3`  
		Last Modified: Tue, 09 Aug 2022 22:37:41 GMT  
		Size: 589.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de94a2ef272b2e3ef327e7dbc685dfc8c6b58775169e3ec47a94fd5407841bf1`  
		Last Modified: Tue, 09 Aug 2022 22:37:41 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.8-alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:1d7154e4491475ff8fb864a26874ba8b4b250864ad515419c96432134b79a03a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7234771 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ff14469067b8205c1030c0740c47b13a4cd70a4cb3cd3e3f02472b056353df3b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:51 GMT
ADD file:4b51a9d40f20d2beb29d0759b161d2b9403493453beb509de4e86a5d98513f16 in / 
# Tue, 09 Aug 2022 17:39:51 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 20:52:27 GMT
ENV NATS_SERVER=2.8.4
# Tue, 09 Aug 2022 20:52:29 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='75a53e10c640c8348bafe43300785d5147c91f60cd721c21ec896bc50727270a' ;; 		armhf) natsArch='arm6'; sha256='993a0d02ff9d0c74be31dc9e7ac1066659637c4897cc94ced2e0dc982fb428f3' ;; 		armv7) natsArch='arm7'; sha256='89e4191a0bc15c2196f2e6c1b2a3c4200576f6e8ec1176060b2a191c5e588b0d' ;; 		x86_64) natsArch='amd64'; sha256='da8c999ab0da5881fde68cba55238748d7310f28022fb78b9c07b420572a4b45' ;; 		x86) natsArch='386'; sha256='e94e5ec1076122e782527f4a98937c60c9eed4d04c6ba0364986cc58cd3ff8f8' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 09 Aug 2022 20:52:31 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 09 Aug 2022 20:52:32 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 09 Aug 2022 20:52:32 GMT
EXPOSE 4222 6222 8222
# Tue, 09 Aug 2022 20:52:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 09 Aug 2022 20:52:34 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:47517142f6ba87eca6b7bdca1e0df160b74671c81e4b9605dad38c1862a43be3`  
		Last Modified: Tue, 09 Aug 2022 17:40:55 GMT  
		Size: 2.7 MB (2718439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf0beb1bc3611827acd1326750497c2cc98b9160ed5aec13a1112ad88b6ba136`  
		Last Modified: Tue, 09 Aug 2022 20:53:33 GMT  
		Size: 4.5 MB (4515360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a20f9bb5cbf9bb42bf80058089fa2cc11fe7eaad0e4342ef69340f9421360e9`  
		Last Modified: Tue, 09 Aug 2022 20:53:31 GMT  
		Size: 560.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b065ba618e0c23dec2ae44bb9555ee098a0827cf44bc5f30ae1d9448e11f668`  
		Last Modified: Tue, 09 Aug 2022 20:53:31 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.8-alpine3.15`

```console
$ docker pull nats@sha256:988010f74b61749cfb82c28b50b47d26d0b972860ce6e9325a5afcde97713da2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.8-alpine3.15` - linux; amd64

```console
$ docker pull nats@sha256:f67ef794683ba4fcddc40bf871ad70eb258221443adcf1927b0270f257e73a74
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.7 MB (7701879 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57eb300f225ba4543fcd1c479ef7191723cf877d51078fa0d82de48cdff5c640`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:00 GMT
ADD file:f77e3f51f020890d22997e6c2ca98968b75b8bc8c463341a2010ff0655d4c88f in / 
# Tue, 09 Aug 2022 17:20:01 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 01:29:02 GMT
ENV NATS_SERVER=2.8.4
# Wed, 10 Aug 2022 01:29:04 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='75a53e10c640c8348bafe43300785d5147c91f60cd721c21ec896bc50727270a' ;; 		armhf) natsArch='arm6'; sha256='993a0d02ff9d0c74be31dc9e7ac1066659637c4897cc94ced2e0dc982fb428f3' ;; 		armv7) natsArch='arm7'; sha256='89e4191a0bc15c2196f2e6c1b2a3c4200576f6e8ec1176060b2a191c5e588b0d' ;; 		x86_64) natsArch='amd64'; sha256='da8c999ab0da5881fde68cba55238748d7310f28022fb78b9c07b420572a4b45' ;; 		x86) natsArch='386'; sha256='e94e5ec1076122e782527f4a98937c60c9eed4d04c6ba0364986cc58cd3ff8f8' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 10 Aug 2022 01:29:04 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 10 Aug 2022 01:29:04 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 10 Aug 2022 01:29:04 GMT
EXPOSE 4222 6222 8222
# Wed, 10 Aug 2022 01:29:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 10 Aug 2022 01:29:04 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9621f1afde84053b2f9b6ff34fc7f7460712247c01cbab483c5fa7132cf782ca`  
		Last Modified: Tue, 09 Aug 2022 17:20:52 GMT  
		Size: 2.8 MB (2823512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21c1a3defde00a6a87bb6d1f724a28b2cc109a3d0e6b086dc01265ecf07abf3b`  
		Last Modified: Wed, 10 Aug 2022 01:29:38 GMT  
		Size: 4.9 MB (4877365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d5c2bde7b7ca5bd606ae2db561e93e1addd87b05802f031fa6ec7a82f2828b0`  
		Last Modified: Wed, 10 Aug 2022 01:29:37 GMT  
		Size: 589.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a153c5b56febe9e8cc9d9df0925d160671c9aaffc633a61bdd7f368d42a1b96f`  
		Last Modified: Wed, 10 Aug 2022 01:29:37 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.8-alpine3.15` - linux; arm variant v6

```console
$ docker pull nats@sha256:91a3c5bbf8c80536df0dc91bebe4a3dbcf2901cdebb612e239a224e198e42c70
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7168331 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:87fc1a9a79541b69ed4655f072cef3d05408ecb373ad11d3a0f4c802831f0fa4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:29 GMT
ADD file:89cb25f97e17bed5c56311280efe5cfa78422d8ffbe36232195d13f94d67417e in / 
# Tue, 09 Aug 2022 17:49:29 GMT
CMD ["/bin/sh"]
# Thu, 11 Aug 2022 01:11:51 GMT
ENV NATS_SERVER=2.8.4
# Thu, 11 Aug 2022 01:11:53 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='75a53e10c640c8348bafe43300785d5147c91f60cd721c21ec896bc50727270a' ;; 		armhf) natsArch='arm6'; sha256='993a0d02ff9d0c74be31dc9e7ac1066659637c4897cc94ced2e0dc982fb428f3' ;; 		armv7) natsArch='arm7'; sha256='89e4191a0bc15c2196f2e6c1b2a3c4200576f6e8ec1176060b2a191c5e588b0d' ;; 		x86_64) natsArch='amd64'; sha256='da8c999ab0da5881fde68cba55238748d7310f28022fb78b9c07b420572a4b45' ;; 		x86) natsArch='386'; sha256='e94e5ec1076122e782527f4a98937c60c9eed4d04c6ba0364986cc58cd3ff8f8' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 11 Aug 2022 01:11:53 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 11 Aug 2022 01:11:54 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 11 Aug 2022 01:11:54 GMT
EXPOSE 4222 6222 8222
# Thu, 11 Aug 2022 01:11:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 Aug 2022 01:11:54 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:293b708aa6fb80967f27727d5c9c53ac9ba9cac376bed2ad02c17a5cca317b35`  
		Last Modified: Tue, 09 Aug 2022 17:50:52 GMT  
		Size: 2.6 MB (2631127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4efb85326bdd0b14d348830449cbdd93250414456c1d970d673f4002e8fdf93`  
		Last Modified: Thu, 11 Aug 2022 01:13:00 GMT  
		Size: 4.5 MB (4536202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef98b89db7bb29b263ede5d92c245cef1ed1dd56776120239a54f5f7692b2ff3`  
		Last Modified: Thu, 11 Aug 2022 01:13:00 GMT  
		Size: 589.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7a526f2148801e4c48011a6d1aa6ed5894b02339d145fbb462dae4f1692faa2`  
		Last Modified: Thu, 11 Aug 2022 01:13:00 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.8-alpine3.15` - linux; arm variant v7

```console
$ docker pull nats@sha256:a86957d0ea21981ed74f78c988f8b5202243dab5a43f68f0cd4d09be0e03acf7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.0 MB (6963329 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:02a19e2d0d29009797ec24843b88e7a35ebb4ca64c9a7b624b6be3290ec5f730`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 16:57:52 GMT
ADD file:0bd18306f21937a9572e68c768f05f4a9d8341b40c2379a7bfcb857c77734a14 in / 
# Tue, 09 Aug 2022 16:57:52 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 22:35:52 GMT
ENV NATS_SERVER=2.8.4
# Tue, 09 Aug 2022 22:35:55 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='75a53e10c640c8348bafe43300785d5147c91f60cd721c21ec896bc50727270a' ;; 		armhf) natsArch='arm6'; sha256='993a0d02ff9d0c74be31dc9e7ac1066659637c4897cc94ced2e0dc982fb428f3' ;; 		armv7) natsArch='arm7'; sha256='89e4191a0bc15c2196f2e6c1b2a3c4200576f6e8ec1176060b2a191c5e588b0d' ;; 		x86_64) natsArch='amd64'; sha256='da8c999ab0da5881fde68cba55238748d7310f28022fb78b9c07b420572a4b45' ;; 		x86) natsArch='386'; sha256='e94e5ec1076122e782527f4a98937c60c9eed4d04c6ba0364986cc58cd3ff8f8' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 09 Aug 2022 22:35:55 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 09 Aug 2022 22:35:55 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 09 Aug 2022 22:35:56 GMT
EXPOSE 4222 6222 8222
# Tue, 09 Aug 2022 22:35:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 09 Aug 2022 22:35:56 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:59775c20a906b1a49edcdc41a700a795998979d6ecf8f8d9cd7cbdf45e686d81`  
		Last Modified: Tue, 09 Aug 2022 16:59:12 GMT  
		Size: 2.4 MB (2435092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b55d1d06353a20f9de5b52fd408cb1d36cb23aea75e779350590565a5a4dea90`  
		Last Modified: Tue, 09 Aug 2022 22:37:42 GMT  
		Size: 4.5 MB (4527236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52e8be9dffb2c65f4e861ee01ddc4ec8362d0a2ca4ac53ad84fa5baf7b28b2d3`  
		Last Modified: Tue, 09 Aug 2022 22:37:41 GMT  
		Size: 589.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de94a2ef272b2e3ef327e7dbc685dfc8c6b58775169e3ec47a94fd5407841bf1`  
		Last Modified: Tue, 09 Aug 2022 22:37:41 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.8-alpine3.15` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:1d7154e4491475ff8fb864a26874ba8b4b250864ad515419c96432134b79a03a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7234771 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ff14469067b8205c1030c0740c47b13a4cd70a4cb3cd3e3f02472b056353df3b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:51 GMT
ADD file:4b51a9d40f20d2beb29d0759b161d2b9403493453beb509de4e86a5d98513f16 in / 
# Tue, 09 Aug 2022 17:39:51 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 20:52:27 GMT
ENV NATS_SERVER=2.8.4
# Tue, 09 Aug 2022 20:52:29 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='75a53e10c640c8348bafe43300785d5147c91f60cd721c21ec896bc50727270a' ;; 		armhf) natsArch='arm6'; sha256='993a0d02ff9d0c74be31dc9e7ac1066659637c4897cc94ced2e0dc982fb428f3' ;; 		armv7) natsArch='arm7'; sha256='89e4191a0bc15c2196f2e6c1b2a3c4200576f6e8ec1176060b2a191c5e588b0d' ;; 		x86_64) natsArch='amd64'; sha256='da8c999ab0da5881fde68cba55238748d7310f28022fb78b9c07b420572a4b45' ;; 		x86) natsArch='386'; sha256='e94e5ec1076122e782527f4a98937c60c9eed4d04c6ba0364986cc58cd3ff8f8' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 09 Aug 2022 20:52:31 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 09 Aug 2022 20:52:32 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 09 Aug 2022 20:52:32 GMT
EXPOSE 4222 6222 8222
# Tue, 09 Aug 2022 20:52:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 09 Aug 2022 20:52:34 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:47517142f6ba87eca6b7bdca1e0df160b74671c81e4b9605dad38c1862a43be3`  
		Last Modified: Tue, 09 Aug 2022 17:40:55 GMT  
		Size: 2.7 MB (2718439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf0beb1bc3611827acd1326750497c2cc98b9160ed5aec13a1112ad88b6ba136`  
		Last Modified: Tue, 09 Aug 2022 20:53:33 GMT  
		Size: 4.5 MB (4515360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a20f9bb5cbf9bb42bf80058089fa2cc11fe7eaad0e4342ef69340f9421360e9`  
		Last Modified: Tue, 09 Aug 2022 20:53:31 GMT  
		Size: 560.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b065ba618e0c23dec2ae44bb9555ee098a0827cf44bc5f30ae1d9448e11f668`  
		Last Modified: Tue, 09 Aug 2022 20:53:31 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.8-linux`

```console
$ docker pull nats@sha256:95b20a1c366e503cd8c0b97a45f2b00d70adfa53f7482237d1ef8fa2e792d2cf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.8-linux` - linux; amd64

```console
$ docker pull nats@sha256:796298f636925dedbbdfa537f42423dffd3a69b70c3a9bf4fd0982886a4b745d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4591595 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:842c053e15bdb38e697668b1f0721313203f7c2297eb6d79000f20858dc97854`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 27 May 2022 00:38:26 GMT
COPY file:c866dea678e8cec7cbd0798a1dbdefc45e992d9df374709f6000bac517589a1b in /nats-server 
# Fri, 27 May 2022 00:38:26 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 27 May 2022 00:38:27 GMT
EXPOSE 4222 6222 8222
# Fri, 27 May 2022 00:38:27 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 27 May 2022 00:38:27 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 27 May 2022 00:38:27 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:5e5797f39fa0527a3dd0a137353b40f97c71134e7eb38373d9791c5f1392885b`  
		Last Modified: Fri, 27 May 2022 00:39:15 GMT  
		Size: 4.6 MB (4591087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28c3b732adf61929b0b23ca08934cd89923e9cd9d7061544e76bbce57a9fa1e4`  
		Last Modified: Fri, 27 May 2022 00:39:14 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.8-linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:e0c28a95cdf6dd8a566d5c2394d09e6141dffb9107fe49f9385d6f19048bd955
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4245827 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cef47371f249bc862484ca7bd4dde2d7f77dc41bcb49cc49cceb17dfb2d4471f`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 11 Aug 2022 01:12:06 GMT
COPY file:8de8b0cf8e6edf54e413c112cd66aed537abed387a26ba749a9293d43cdf6594 in /nats-server 
# Thu, 11 Aug 2022 01:12:06 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 11 Aug 2022 01:12:06 GMT
EXPOSE 4222 6222 8222
# Thu, 11 Aug 2022 01:12:06 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 11 Aug 2022 01:12:06 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 11 Aug 2022 01:12:06 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:770fa9c168613edbe7aa7007d2cf8492c6570efc1ddab217fa32772c6b72dd48`  
		Last Modified: Thu, 26 May 2022 23:58:21 GMT  
		Size: 4.2 MB (4245317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bde47aae170f9c7e50b7bbea164ec0e0d02b9c05b603e7f7554e163183c02cd9`  
		Last Modified: Thu, 11 Aug 2022 01:13:30 GMT  
		Size: 510.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.8-linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:453c8fea5d37abc60f034f80bdb668a48c8e4f0900fce8b55fdb6ae7f2908d07
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4242795 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:508b00336aa0fc72bd1c3d33e5f447d1411e47221dfa1fa6085d6986b27045d7`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 22:36:22 GMT
COPY file:2841d6664b8897473f39b595b9aa4b28e749f587dc1afa4a0027ae507f37ee1f in /nats-server 
# Tue, 09 Aug 2022 22:36:22 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 09 Aug 2022 22:36:22 GMT
EXPOSE 4222 6222 8222
# Tue, 09 Aug 2022 22:36:22 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 09 Aug 2022 22:36:23 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 09 Aug 2022 22:36:23 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:f533e6e439ee51f1cf94458f821a20ed162b542d356340957091882ad881d5c1`  
		Last Modified: Fri, 27 May 2022 00:28:16 GMT  
		Size: 4.2 MB (4242287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:274ba9becbe1086958e9d56ab9452ec01f7fad6e3e68a34c49f1f299a5eab1ac`  
		Last Modified: Tue, 09 Aug 2022 22:38:14 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.8-linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:87b1afbd78a75ee48cb6b37a8522bbb01f5e9b5047b095b16cc4f241774a48d1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4227885 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9bce5ae01237736c7e0447d8cd1b2dbe252eab3ab5ac3b05d98b646b2575cee`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 26 May 2022 23:53:56 GMT
COPY file:2dbd94c6c11f89ceba3241f1efe469d0a06f0aae91abb77f3d79756676d0be57 in /nats-server 
# Thu, 26 May 2022 23:53:57 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 26 May 2022 23:53:57 GMT
EXPOSE 4222 6222 8222
# Thu, 26 May 2022 23:53:58 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 26 May 2022 23:53:59 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 26 May 2022 23:54:00 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:1c74770da2ea808362085edd6dead652091b3e3d34c1e32c50015a6a5bb36c02`  
		Last Modified: Thu, 26 May 2022 23:55:21 GMT  
		Size: 4.2 MB (4227378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:988af7458b707048622e497d5ae818b77d3a24ed0295a7897ced8f003179f7f9`  
		Last Modified: Thu, 26 May 2022 23:55:21 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.8-nanoserver`

```console
$ docker pull nats@sha256:92865bb073a2a8994aa5a8428fb857b4885c97d5c4af51ea7bdc5a56a93d4c69
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3287; amd64

### `nats:2.8-nanoserver` - windows version 10.0.17763.3287; amd64

```console
$ docker pull nats@sha256:1cedf48ffc2053a99d48b9d25a25aafa92106fbeeb92fe41aeb237d72e722664
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.8 MB (107843136 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:68f300c81963c2298e1d161245bcc24caccb02bc76fa1f665acbb465b70ff518`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 06 Aug 2022 18:08:38 GMT
RUN Apply image 10.0.17763.3287
# Wed, 10 Aug 2022 15:30:21 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 10 Aug 2022 15:30:22 GMT
RUN cmd /S /C #(nop) COPY file:88c957e774978b3592c1072a38fbf2d578a30b42e89604bf16828cccd9f86b17 in C:\nats-server.exe 
# Wed, 10 Aug 2022 15:30:23 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 10 Aug 2022 15:30:24 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 10 Aug 2022 15:30:25 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 10 Aug 2022 15:30:25 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:5c9d6483dab113d2d9b50fdf3156622aa2ec3d6faaed5664d15a5568032d1714`  
		Size: 103.2 MB (103204200 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:0a5df16ce106b092b5399678da04735c18584e4f99ea301691eb433072953e9a`  
		Last Modified: Wed, 10 Aug 2022 15:31:14 GMT  
		Size: 1.0 KB (1025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0da7ec45038de57bb4ae201762e54193e71ffc21892b700c1942bd3b85a10ac`  
		Last Modified: Wed, 10 Aug 2022 15:31:13 GMT  
		Size: 4.6 MB (4633133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d561d8a7d904db478c9c1e66aae419bb3d5333483d2d9f39f39e7bc62c02c56d`  
		Last Modified: Wed, 10 Aug 2022 15:31:12 GMT  
		Size: 1.7 KB (1653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f34e9538ca1cb2f704590a6fdaaef3b512b5ac93696534421be5f67017ffe8b9`  
		Last Modified: Wed, 10 Aug 2022 15:31:12 GMT  
		Size: 1.0 KB (1033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:660c54f5d2b9ddc91667f920a6f2103c75527be0b892d65aa55dd5bfa8afd3fe`  
		Last Modified: Wed, 10 Aug 2022 15:31:12 GMT  
		Size: 1.1 KB (1056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9356123a2a1af8afcf36b9979e254c522e7759fba29e96837a9d80c3a723f12c`  
		Last Modified: Wed, 10 Aug 2022 15:31:12 GMT  
		Size: 1.0 KB (1036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.8-nanoserver-1809`

```console
$ docker pull nats@sha256:92865bb073a2a8994aa5a8428fb857b4885c97d5c4af51ea7bdc5a56a93d4c69
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3287; amd64

### `nats:2.8-nanoserver-1809` - windows version 10.0.17763.3287; amd64

```console
$ docker pull nats@sha256:1cedf48ffc2053a99d48b9d25a25aafa92106fbeeb92fe41aeb237d72e722664
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.8 MB (107843136 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:68f300c81963c2298e1d161245bcc24caccb02bc76fa1f665acbb465b70ff518`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 06 Aug 2022 18:08:38 GMT
RUN Apply image 10.0.17763.3287
# Wed, 10 Aug 2022 15:30:21 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 10 Aug 2022 15:30:22 GMT
RUN cmd /S /C #(nop) COPY file:88c957e774978b3592c1072a38fbf2d578a30b42e89604bf16828cccd9f86b17 in C:\nats-server.exe 
# Wed, 10 Aug 2022 15:30:23 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 10 Aug 2022 15:30:24 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 10 Aug 2022 15:30:25 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 10 Aug 2022 15:30:25 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:5c9d6483dab113d2d9b50fdf3156622aa2ec3d6faaed5664d15a5568032d1714`  
		Size: 103.2 MB (103204200 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:0a5df16ce106b092b5399678da04735c18584e4f99ea301691eb433072953e9a`  
		Last Modified: Wed, 10 Aug 2022 15:31:14 GMT  
		Size: 1.0 KB (1025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0da7ec45038de57bb4ae201762e54193e71ffc21892b700c1942bd3b85a10ac`  
		Last Modified: Wed, 10 Aug 2022 15:31:13 GMT  
		Size: 4.6 MB (4633133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d561d8a7d904db478c9c1e66aae419bb3d5333483d2d9f39f39e7bc62c02c56d`  
		Last Modified: Wed, 10 Aug 2022 15:31:12 GMT  
		Size: 1.7 KB (1653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f34e9538ca1cb2f704590a6fdaaef3b512b5ac93696534421be5f67017ffe8b9`  
		Last Modified: Wed, 10 Aug 2022 15:31:12 GMT  
		Size: 1.0 KB (1033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:660c54f5d2b9ddc91667f920a6f2103c75527be0b892d65aa55dd5bfa8afd3fe`  
		Last Modified: Wed, 10 Aug 2022 15:31:12 GMT  
		Size: 1.1 KB (1056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9356123a2a1af8afcf36b9979e254c522e7759fba29e96837a9d80c3a723f12c`  
		Last Modified: Wed, 10 Aug 2022 15:31:12 GMT  
		Size: 1.0 KB (1036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.8-scratch`

```console
$ docker pull nats@sha256:95b20a1c366e503cd8c0b97a45f2b00d70adfa53f7482237d1ef8fa2e792d2cf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.8-scratch` - linux; amd64

```console
$ docker pull nats@sha256:796298f636925dedbbdfa537f42423dffd3a69b70c3a9bf4fd0982886a4b745d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4591595 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:842c053e15bdb38e697668b1f0721313203f7c2297eb6d79000f20858dc97854`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 27 May 2022 00:38:26 GMT
COPY file:c866dea678e8cec7cbd0798a1dbdefc45e992d9df374709f6000bac517589a1b in /nats-server 
# Fri, 27 May 2022 00:38:26 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 27 May 2022 00:38:27 GMT
EXPOSE 4222 6222 8222
# Fri, 27 May 2022 00:38:27 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 27 May 2022 00:38:27 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 27 May 2022 00:38:27 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:5e5797f39fa0527a3dd0a137353b40f97c71134e7eb38373d9791c5f1392885b`  
		Last Modified: Fri, 27 May 2022 00:39:15 GMT  
		Size: 4.6 MB (4591087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28c3b732adf61929b0b23ca08934cd89923e9cd9d7061544e76bbce57a9fa1e4`  
		Last Modified: Fri, 27 May 2022 00:39:14 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.8-scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:e0c28a95cdf6dd8a566d5c2394d09e6141dffb9107fe49f9385d6f19048bd955
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4245827 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cef47371f249bc862484ca7bd4dde2d7f77dc41bcb49cc49cceb17dfb2d4471f`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 11 Aug 2022 01:12:06 GMT
COPY file:8de8b0cf8e6edf54e413c112cd66aed537abed387a26ba749a9293d43cdf6594 in /nats-server 
# Thu, 11 Aug 2022 01:12:06 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 11 Aug 2022 01:12:06 GMT
EXPOSE 4222 6222 8222
# Thu, 11 Aug 2022 01:12:06 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 11 Aug 2022 01:12:06 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 11 Aug 2022 01:12:06 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:770fa9c168613edbe7aa7007d2cf8492c6570efc1ddab217fa32772c6b72dd48`  
		Last Modified: Thu, 26 May 2022 23:58:21 GMT  
		Size: 4.2 MB (4245317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bde47aae170f9c7e50b7bbea164ec0e0d02b9c05b603e7f7554e163183c02cd9`  
		Last Modified: Thu, 11 Aug 2022 01:13:30 GMT  
		Size: 510.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.8-scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:453c8fea5d37abc60f034f80bdb668a48c8e4f0900fce8b55fdb6ae7f2908d07
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4242795 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:508b00336aa0fc72bd1c3d33e5f447d1411e47221dfa1fa6085d6986b27045d7`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 22:36:22 GMT
COPY file:2841d6664b8897473f39b595b9aa4b28e749f587dc1afa4a0027ae507f37ee1f in /nats-server 
# Tue, 09 Aug 2022 22:36:22 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 09 Aug 2022 22:36:22 GMT
EXPOSE 4222 6222 8222
# Tue, 09 Aug 2022 22:36:22 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 09 Aug 2022 22:36:23 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 09 Aug 2022 22:36:23 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:f533e6e439ee51f1cf94458f821a20ed162b542d356340957091882ad881d5c1`  
		Last Modified: Fri, 27 May 2022 00:28:16 GMT  
		Size: 4.2 MB (4242287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:274ba9becbe1086958e9d56ab9452ec01f7fad6e3e68a34c49f1f299a5eab1ac`  
		Last Modified: Tue, 09 Aug 2022 22:38:14 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.8-scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:87b1afbd78a75ee48cb6b37a8522bbb01f5e9b5047b095b16cc4f241774a48d1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4227885 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9bce5ae01237736c7e0447d8cd1b2dbe252eab3ab5ac3b05d98b646b2575cee`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 26 May 2022 23:53:56 GMT
COPY file:2dbd94c6c11f89ceba3241f1efe469d0a06f0aae91abb77f3d79756676d0be57 in /nats-server 
# Thu, 26 May 2022 23:53:57 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 26 May 2022 23:53:57 GMT
EXPOSE 4222 6222 8222
# Thu, 26 May 2022 23:53:58 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 26 May 2022 23:53:59 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 26 May 2022 23:54:00 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:1c74770da2ea808362085edd6dead652091b3e3d34c1e32c50015a6a5bb36c02`  
		Last Modified: Thu, 26 May 2022 23:55:21 GMT  
		Size: 4.2 MB (4227378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:988af7458b707048622e497d5ae818b77d3a24ed0295a7897ced8f003179f7f9`  
		Last Modified: Thu, 26 May 2022 23:55:21 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.8-windowsservercore`

```console
$ docker pull nats@sha256:01e61321ee0c2a556640c7b04f8aaf24a2e46524bdec3c3b451c81dd170d0825
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3287; amd64

### `nats:2.8-windowsservercore` - windows version 10.0.17763.3287; amd64

```console
$ docker pull nats@sha256:9d7b29f769b82966a826e9eebcbff7022824cb343278b2c9dd87014b310f6bc2
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2683024603 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db44bc7e8ad93293de37107a4b87601bb8241a7d0762deac86c4a40d5ef262f0`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 06 Aug 2022 18:30:32 GMT
RUN Install update 10.0.17763.3287
# Wed, 10 Aug 2022 13:44:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Aug 2022 15:27:50 GMT
ENV NATS_DOCKERIZED=1
# Wed, 10 Aug 2022 15:27:51 GMT
ENV NATS_SERVER=2.8.4
# Wed, 10 Aug 2022 15:27:52 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.8.4/nats-server-v2.8.4-windows-amd64.zip
# Wed, 10 Aug 2022 15:27:53 GMT
ENV NATS_SERVER_SHASUM=911e8b77cf288c6e0997891d1400e5cc59dedd928e8f1685650c468674b52dc8
# Wed, 10 Aug 2022 15:28:46 GMT
RUN Set-PSDebug -Trace 2
# Wed, 10 Aug 2022 15:30:06 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 10 Aug 2022 15:30:07 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 10 Aug 2022 15:30:08 GMT
EXPOSE 4222 6222 8222
# Wed, 10 Aug 2022 15:30:09 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 10 Aug 2022 15:30:09 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:294d77ac553d7210b662d07674ef9e39a6c2e88dc15b9d2788d51e509bc8b54e`  
		Size: 800.5 MB (800546641 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:da71148bcd96afa7027d6172acee93aad6002bfbe87cadf468260667c09b3a89`  
		Last Modified: Wed, 10 Aug 2022 15:05:54 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26dc1c1069568772f0068cef343e37284e5f5e488dbfc15e037d95bce032d917`  
		Last Modified: Wed, 10 Aug 2022 15:30:56 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:890750ec51eb48085268f820e86c5b7ff873ff61875ed2b5df77150e4f667aff`  
		Last Modified: Wed, 10 Aug 2022 15:30:55 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da392874ede7ff085d580701bc4800047c2c07531b8dfb625241622eaba1995c`  
		Last Modified: Wed, 10 Aug 2022 15:30:55 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5a137a2c60ae08a2536eb110f4f21b9c80f33a03ab2d732da15f5f3de36c588`  
		Last Modified: Wed, 10 Aug 2022 15:30:55 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94cf94feb41446a9b0f0b35e7d386675c5b6256a8123327795d03d29f60b9400`  
		Last Modified: Wed, 10 Aug 2022 15:30:55 GMT  
		Size: 340.8 KB (340788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ab22594d9c79ecf05870151796e0c4df02facc4a9c10e99fcbea268fcbe9886`  
		Last Modified: Wed, 10 Aug 2022 15:30:53 GMT  
		Size: 5.0 MB (4957679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:143ae888a3c2d7c0f27e7935a85c8a25ef108bb2421c597eea07c8283cf18cbd`  
		Last Modified: Wed, 10 Aug 2022 15:30:52 GMT  
		Size: 2.0 KB (1996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b16fcb36242a120d1667323616c739921e5e2ccd627ea85b09d12df62368dc62`  
		Last Modified: Wed, 10 Aug 2022 15:30:53 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:478c487cdfd4835865c12e472c096f810ceb98ae9fa4d8a77c2080b01e22f095`  
		Last Modified: Wed, 10 Aug 2022 15:30:52 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2414c1290a3b460fc321c6c8630ddd4386a1f7192c489baca687f6ce4bd010e`  
		Last Modified: Wed, 10 Aug 2022 15:30:52 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.8-windowsservercore-1809`

```console
$ docker pull nats@sha256:01e61321ee0c2a556640c7b04f8aaf24a2e46524bdec3c3b451c81dd170d0825
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3287; amd64

### `nats:2.8-windowsservercore-1809` - windows version 10.0.17763.3287; amd64

```console
$ docker pull nats@sha256:9d7b29f769b82966a826e9eebcbff7022824cb343278b2c9dd87014b310f6bc2
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2683024603 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db44bc7e8ad93293de37107a4b87601bb8241a7d0762deac86c4a40d5ef262f0`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 06 Aug 2022 18:30:32 GMT
RUN Install update 10.0.17763.3287
# Wed, 10 Aug 2022 13:44:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Aug 2022 15:27:50 GMT
ENV NATS_DOCKERIZED=1
# Wed, 10 Aug 2022 15:27:51 GMT
ENV NATS_SERVER=2.8.4
# Wed, 10 Aug 2022 15:27:52 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.8.4/nats-server-v2.8.4-windows-amd64.zip
# Wed, 10 Aug 2022 15:27:53 GMT
ENV NATS_SERVER_SHASUM=911e8b77cf288c6e0997891d1400e5cc59dedd928e8f1685650c468674b52dc8
# Wed, 10 Aug 2022 15:28:46 GMT
RUN Set-PSDebug -Trace 2
# Wed, 10 Aug 2022 15:30:06 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 10 Aug 2022 15:30:07 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 10 Aug 2022 15:30:08 GMT
EXPOSE 4222 6222 8222
# Wed, 10 Aug 2022 15:30:09 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 10 Aug 2022 15:30:09 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:294d77ac553d7210b662d07674ef9e39a6c2e88dc15b9d2788d51e509bc8b54e`  
		Size: 800.5 MB (800546641 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:da71148bcd96afa7027d6172acee93aad6002bfbe87cadf468260667c09b3a89`  
		Last Modified: Wed, 10 Aug 2022 15:05:54 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26dc1c1069568772f0068cef343e37284e5f5e488dbfc15e037d95bce032d917`  
		Last Modified: Wed, 10 Aug 2022 15:30:56 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:890750ec51eb48085268f820e86c5b7ff873ff61875ed2b5df77150e4f667aff`  
		Last Modified: Wed, 10 Aug 2022 15:30:55 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da392874ede7ff085d580701bc4800047c2c07531b8dfb625241622eaba1995c`  
		Last Modified: Wed, 10 Aug 2022 15:30:55 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5a137a2c60ae08a2536eb110f4f21b9c80f33a03ab2d732da15f5f3de36c588`  
		Last Modified: Wed, 10 Aug 2022 15:30:55 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94cf94feb41446a9b0f0b35e7d386675c5b6256a8123327795d03d29f60b9400`  
		Last Modified: Wed, 10 Aug 2022 15:30:55 GMT  
		Size: 340.8 KB (340788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ab22594d9c79ecf05870151796e0c4df02facc4a9c10e99fcbea268fcbe9886`  
		Last Modified: Wed, 10 Aug 2022 15:30:53 GMT  
		Size: 5.0 MB (4957679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:143ae888a3c2d7c0f27e7935a85c8a25ef108bb2421c597eea07c8283cf18cbd`  
		Last Modified: Wed, 10 Aug 2022 15:30:52 GMT  
		Size: 2.0 KB (1996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b16fcb36242a120d1667323616c739921e5e2ccd627ea85b09d12df62368dc62`  
		Last Modified: Wed, 10 Aug 2022 15:30:53 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:478c487cdfd4835865c12e472c096f810ceb98ae9fa4d8a77c2080b01e22f095`  
		Last Modified: Wed, 10 Aug 2022 15:30:52 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2414c1290a3b460fc321c6c8630ddd4386a1f7192c489baca687f6ce4bd010e`  
		Last Modified: Wed, 10 Aug 2022 15:30:52 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.8.4`

```console
$ docker pull nats@sha256:8f0cdcbc4c3597443fce869e75a759edb0d5a93fe98078f470a43204a6d7a729
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.3287; amd64

### `nats:2.8.4` - linux; amd64

```console
$ docker pull nats@sha256:796298f636925dedbbdfa537f42423dffd3a69b70c3a9bf4fd0982886a4b745d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4591595 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:842c053e15bdb38e697668b1f0721313203f7c2297eb6d79000f20858dc97854`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 27 May 2022 00:38:26 GMT
COPY file:c866dea678e8cec7cbd0798a1dbdefc45e992d9df374709f6000bac517589a1b in /nats-server 
# Fri, 27 May 2022 00:38:26 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 27 May 2022 00:38:27 GMT
EXPOSE 4222 6222 8222
# Fri, 27 May 2022 00:38:27 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 27 May 2022 00:38:27 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 27 May 2022 00:38:27 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:5e5797f39fa0527a3dd0a137353b40f97c71134e7eb38373d9791c5f1392885b`  
		Last Modified: Fri, 27 May 2022 00:39:15 GMT  
		Size: 4.6 MB (4591087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28c3b732adf61929b0b23ca08934cd89923e9cd9d7061544e76bbce57a9fa1e4`  
		Last Modified: Fri, 27 May 2022 00:39:14 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.8.4` - linux; arm variant v6

```console
$ docker pull nats@sha256:e0c28a95cdf6dd8a566d5c2394d09e6141dffb9107fe49f9385d6f19048bd955
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4245827 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cef47371f249bc862484ca7bd4dde2d7f77dc41bcb49cc49cceb17dfb2d4471f`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 11 Aug 2022 01:12:06 GMT
COPY file:8de8b0cf8e6edf54e413c112cd66aed537abed387a26ba749a9293d43cdf6594 in /nats-server 
# Thu, 11 Aug 2022 01:12:06 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 11 Aug 2022 01:12:06 GMT
EXPOSE 4222 6222 8222
# Thu, 11 Aug 2022 01:12:06 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 11 Aug 2022 01:12:06 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 11 Aug 2022 01:12:06 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:770fa9c168613edbe7aa7007d2cf8492c6570efc1ddab217fa32772c6b72dd48`  
		Last Modified: Thu, 26 May 2022 23:58:21 GMT  
		Size: 4.2 MB (4245317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bde47aae170f9c7e50b7bbea164ec0e0d02b9c05b603e7f7554e163183c02cd9`  
		Last Modified: Thu, 11 Aug 2022 01:13:30 GMT  
		Size: 510.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.8.4` - linux; arm variant v7

```console
$ docker pull nats@sha256:453c8fea5d37abc60f034f80bdb668a48c8e4f0900fce8b55fdb6ae7f2908d07
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4242795 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:508b00336aa0fc72bd1c3d33e5f447d1411e47221dfa1fa6085d6986b27045d7`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 22:36:22 GMT
COPY file:2841d6664b8897473f39b595b9aa4b28e749f587dc1afa4a0027ae507f37ee1f in /nats-server 
# Tue, 09 Aug 2022 22:36:22 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 09 Aug 2022 22:36:22 GMT
EXPOSE 4222 6222 8222
# Tue, 09 Aug 2022 22:36:22 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 09 Aug 2022 22:36:23 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 09 Aug 2022 22:36:23 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:f533e6e439ee51f1cf94458f821a20ed162b542d356340957091882ad881d5c1`  
		Last Modified: Fri, 27 May 2022 00:28:16 GMT  
		Size: 4.2 MB (4242287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:274ba9becbe1086958e9d56ab9452ec01f7fad6e3e68a34c49f1f299a5eab1ac`  
		Last Modified: Tue, 09 Aug 2022 22:38:14 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.8.4` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:87b1afbd78a75ee48cb6b37a8522bbb01f5e9b5047b095b16cc4f241774a48d1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4227885 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9bce5ae01237736c7e0447d8cd1b2dbe252eab3ab5ac3b05d98b646b2575cee`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 26 May 2022 23:53:56 GMT
COPY file:2dbd94c6c11f89ceba3241f1efe469d0a06f0aae91abb77f3d79756676d0be57 in /nats-server 
# Thu, 26 May 2022 23:53:57 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 26 May 2022 23:53:57 GMT
EXPOSE 4222 6222 8222
# Thu, 26 May 2022 23:53:58 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 26 May 2022 23:53:59 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 26 May 2022 23:54:00 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:1c74770da2ea808362085edd6dead652091b3e3d34c1e32c50015a6a5bb36c02`  
		Last Modified: Thu, 26 May 2022 23:55:21 GMT  
		Size: 4.2 MB (4227378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:988af7458b707048622e497d5ae818b77d3a24ed0295a7897ced8f003179f7f9`  
		Last Modified: Thu, 26 May 2022 23:55:21 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.8.4` - windows version 10.0.17763.3287; amd64

```console
$ docker pull nats@sha256:1cedf48ffc2053a99d48b9d25a25aafa92106fbeeb92fe41aeb237d72e722664
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.8 MB (107843136 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:68f300c81963c2298e1d161245bcc24caccb02bc76fa1f665acbb465b70ff518`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 06 Aug 2022 18:08:38 GMT
RUN Apply image 10.0.17763.3287
# Wed, 10 Aug 2022 15:30:21 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 10 Aug 2022 15:30:22 GMT
RUN cmd /S /C #(nop) COPY file:88c957e774978b3592c1072a38fbf2d578a30b42e89604bf16828cccd9f86b17 in C:\nats-server.exe 
# Wed, 10 Aug 2022 15:30:23 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 10 Aug 2022 15:30:24 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 10 Aug 2022 15:30:25 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 10 Aug 2022 15:30:25 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:5c9d6483dab113d2d9b50fdf3156622aa2ec3d6faaed5664d15a5568032d1714`  
		Size: 103.2 MB (103204200 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:0a5df16ce106b092b5399678da04735c18584e4f99ea301691eb433072953e9a`  
		Last Modified: Wed, 10 Aug 2022 15:31:14 GMT  
		Size: 1.0 KB (1025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0da7ec45038de57bb4ae201762e54193e71ffc21892b700c1942bd3b85a10ac`  
		Last Modified: Wed, 10 Aug 2022 15:31:13 GMT  
		Size: 4.6 MB (4633133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d561d8a7d904db478c9c1e66aae419bb3d5333483d2d9f39f39e7bc62c02c56d`  
		Last Modified: Wed, 10 Aug 2022 15:31:12 GMT  
		Size: 1.7 KB (1653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f34e9538ca1cb2f704590a6fdaaef3b512b5ac93696534421be5f67017ffe8b9`  
		Last Modified: Wed, 10 Aug 2022 15:31:12 GMT  
		Size: 1.0 KB (1033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:660c54f5d2b9ddc91667f920a6f2103c75527be0b892d65aa55dd5bfa8afd3fe`  
		Last Modified: Wed, 10 Aug 2022 15:31:12 GMT  
		Size: 1.1 KB (1056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9356123a2a1af8afcf36b9979e254c522e7759fba29e96837a9d80c3a723f12c`  
		Last Modified: Wed, 10 Aug 2022 15:31:12 GMT  
		Size: 1.0 KB (1036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.8.4-alpine`

```console
$ docker pull nats@sha256:988010f74b61749cfb82c28b50b47d26d0b972860ce6e9325a5afcde97713da2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.8.4-alpine` - linux; amd64

```console
$ docker pull nats@sha256:f67ef794683ba4fcddc40bf871ad70eb258221443adcf1927b0270f257e73a74
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.7 MB (7701879 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57eb300f225ba4543fcd1c479ef7191723cf877d51078fa0d82de48cdff5c640`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:00 GMT
ADD file:f77e3f51f020890d22997e6c2ca98968b75b8bc8c463341a2010ff0655d4c88f in / 
# Tue, 09 Aug 2022 17:20:01 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 01:29:02 GMT
ENV NATS_SERVER=2.8.4
# Wed, 10 Aug 2022 01:29:04 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='75a53e10c640c8348bafe43300785d5147c91f60cd721c21ec896bc50727270a' ;; 		armhf) natsArch='arm6'; sha256='993a0d02ff9d0c74be31dc9e7ac1066659637c4897cc94ced2e0dc982fb428f3' ;; 		armv7) natsArch='arm7'; sha256='89e4191a0bc15c2196f2e6c1b2a3c4200576f6e8ec1176060b2a191c5e588b0d' ;; 		x86_64) natsArch='amd64'; sha256='da8c999ab0da5881fde68cba55238748d7310f28022fb78b9c07b420572a4b45' ;; 		x86) natsArch='386'; sha256='e94e5ec1076122e782527f4a98937c60c9eed4d04c6ba0364986cc58cd3ff8f8' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 10 Aug 2022 01:29:04 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 10 Aug 2022 01:29:04 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 10 Aug 2022 01:29:04 GMT
EXPOSE 4222 6222 8222
# Wed, 10 Aug 2022 01:29:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 10 Aug 2022 01:29:04 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9621f1afde84053b2f9b6ff34fc7f7460712247c01cbab483c5fa7132cf782ca`  
		Last Modified: Tue, 09 Aug 2022 17:20:52 GMT  
		Size: 2.8 MB (2823512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21c1a3defde00a6a87bb6d1f724a28b2cc109a3d0e6b086dc01265ecf07abf3b`  
		Last Modified: Wed, 10 Aug 2022 01:29:38 GMT  
		Size: 4.9 MB (4877365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d5c2bde7b7ca5bd606ae2db561e93e1addd87b05802f031fa6ec7a82f2828b0`  
		Last Modified: Wed, 10 Aug 2022 01:29:37 GMT  
		Size: 589.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a153c5b56febe9e8cc9d9df0925d160671c9aaffc633a61bdd7f368d42a1b96f`  
		Last Modified: Wed, 10 Aug 2022 01:29:37 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.8.4-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:91a3c5bbf8c80536df0dc91bebe4a3dbcf2901cdebb612e239a224e198e42c70
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7168331 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:87fc1a9a79541b69ed4655f072cef3d05408ecb373ad11d3a0f4c802831f0fa4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:29 GMT
ADD file:89cb25f97e17bed5c56311280efe5cfa78422d8ffbe36232195d13f94d67417e in / 
# Tue, 09 Aug 2022 17:49:29 GMT
CMD ["/bin/sh"]
# Thu, 11 Aug 2022 01:11:51 GMT
ENV NATS_SERVER=2.8.4
# Thu, 11 Aug 2022 01:11:53 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='75a53e10c640c8348bafe43300785d5147c91f60cd721c21ec896bc50727270a' ;; 		armhf) natsArch='arm6'; sha256='993a0d02ff9d0c74be31dc9e7ac1066659637c4897cc94ced2e0dc982fb428f3' ;; 		armv7) natsArch='arm7'; sha256='89e4191a0bc15c2196f2e6c1b2a3c4200576f6e8ec1176060b2a191c5e588b0d' ;; 		x86_64) natsArch='amd64'; sha256='da8c999ab0da5881fde68cba55238748d7310f28022fb78b9c07b420572a4b45' ;; 		x86) natsArch='386'; sha256='e94e5ec1076122e782527f4a98937c60c9eed4d04c6ba0364986cc58cd3ff8f8' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 11 Aug 2022 01:11:53 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 11 Aug 2022 01:11:54 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 11 Aug 2022 01:11:54 GMT
EXPOSE 4222 6222 8222
# Thu, 11 Aug 2022 01:11:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 Aug 2022 01:11:54 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:293b708aa6fb80967f27727d5c9c53ac9ba9cac376bed2ad02c17a5cca317b35`  
		Last Modified: Tue, 09 Aug 2022 17:50:52 GMT  
		Size: 2.6 MB (2631127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4efb85326bdd0b14d348830449cbdd93250414456c1d970d673f4002e8fdf93`  
		Last Modified: Thu, 11 Aug 2022 01:13:00 GMT  
		Size: 4.5 MB (4536202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef98b89db7bb29b263ede5d92c245cef1ed1dd56776120239a54f5f7692b2ff3`  
		Last Modified: Thu, 11 Aug 2022 01:13:00 GMT  
		Size: 589.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7a526f2148801e4c48011a6d1aa6ed5894b02339d145fbb462dae4f1692faa2`  
		Last Modified: Thu, 11 Aug 2022 01:13:00 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.8.4-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:a86957d0ea21981ed74f78c988f8b5202243dab5a43f68f0cd4d09be0e03acf7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.0 MB (6963329 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:02a19e2d0d29009797ec24843b88e7a35ebb4ca64c9a7b624b6be3290ec5f730`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 16:57:52 GMT
ADD file:0bd18306f21937a9572e68c768f05f4a9d8341b40c2379a7bfcb857c77734a14 in / 
# Tue, 09 Aug 2022 16:57:52 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 22:35:52 GMT
ENV NATS_SERVER=2.8.4
# Tue, 09 Aug 2022 22:35:55 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='75a53e10c640c8348bafe43300785d5147c91f60cd721c21ec896bc50727270a' ;; 		armhf) natsArch='arm6'; sha256='993a0d02ff9d0c74be31dc9e7ac1066659637c4897cc94ced2e0dc982fb428f3' ;; 		armv7) natsArch='arm7'; sha256='89e4191a0bc15c2196f2e6c1b2a3c4200576f6e8ec1176060b2a191c5e588b0d' ;; 		x86_64) natsArch='amd64'; sha256='da8c999ab0da5881fde68cba55238748d7310f28022fb78b9c07b420572a4b45' ;; 		x86) natsArch='386'; sha256='e94e5ec1076122e782527f4a98937c60c9eed4d04c6ba0364986cc58cd3ff8f8' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 09 Aug 2022 22:35:55 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 09 Aug 2022 22:35:55 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 09 Aug 2022 22:35:56 GMT
EXPOSE 4222 6222 8222
# Tue, 09 Aug 2022 22:35:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 09 Aug 2022 22:35:56 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:59775c20a906b1a49edcdc41a700a795998979d6ecf8f8d9cd7cbdf45e686d81`  
		Last Modified: Tue, 09 Aug 2022 16:59:12 GMT  
		Size: 2.4 MB (2435092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b55d1d06353a20f9de5b52fd408cb1d36cb23aea75e779350590565a5a4dea90`  
		Last Modified: Tue, 09 Aug 2022 22:37:42 GMT  
		Size: 4.5 MB (4527236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52e8be9dffb2c65f4e861ee01ddc4ec8362d0a2ca4ac53ad84fa5baf7b28b2d3`  
		Last Modified: Tue, 09 Aug 2022 22:37:41 GMT  
		Size: 589.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de94a2ef272b2e3ef327e7dbc685dfc8c6b58775169e3ec47a94fd5407841bf1`  
		Last Modified: Tue, 09 Aug 2022 22:37:41 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.8.4-alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:1d7154e4491475ff8fb864a26874ba8b4b250864ad515419c96432134b79a03a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7234771 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ff14469067b8205c1030c0740c47b13a4cd70a4cb3cd3e3f02472b056353df3b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:51 GMT
ADD file:4b51a9d40f20d2beb29d0759b161d2b9403493453beb509de4e86a5d98513f16 in / 
# Tue, 09 Aug 2022 17:39:51 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 20:52:27 GMT
ENV NATS_SERVER=2.8.4
# Tue, 09 Aug 2022 20:52:29 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='75a53e10c640c8348bafe43300785d5147c91f60cd721c21ec896bc50727270a' ;; 		armhf) natsArch='arm6'; sha256='993a0d02ff9d0c74be31dc9e7ac1066659637c4897cc94ced2e0dc982fb428f3' ;; 		armv7) natsArch='arm7'; sha256='89e4191a0bc15c2196f2e6c1b2a3c4200576f6e8ec1176060b2a191c5e588b0d' ;; 		x86_64) natsArch='amd64'; sha256='da8c999ab0da5881fde68cba55238748d7310f28022fb78b9c07b420572a4b45' ;; 		x86) natsArch='386'; sha256='e94e5ec1076122e782527f4a98937c60c9eed4d04c6ba0364986cc58cd3ff8f8' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 09 Aug 2022 20:52:31 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 09 Aug 2022 20:52:32 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 09 Aug 2022 20:52:32 GMT
EXPOSE 4222 6222 8222
# Tue, 09 Aug 2022 20:52:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 09 Aug 2022 20:52:34 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:47517142f6ba87eca6b7bdca1e0df160b74671c81e4b9605dad38c1862a43be3`  
		Last Modified: Tue, 09 Aug 2022 17:40:55 GMT  
		Size: 2.7 MB (2718439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf0beb1bc3611827acd1326750497c2cc98b9160ed5aec13a1112ad88b6ba136`  
		Last Modified: Tue, 09 Aug 2022 20:53:33 GMT  
		Size: 4.5 MB (4515360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a20f9bb5cbf9bb42bf80058089fa2cc11fe7eaad0e4342ef69340f9421360e9`  
		Last Modified: Tue, 09 Aug 2022 20:53:31 GMT  
		Size: 560.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b065ba618e0c23dec2ae44bb9555ee098a0827cf44bc5f30ae1d9448e11f668`  
		Last Modified: Tue, 09 Aug 2022 20:53:31 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.8.4-alpine3.15`

```console
$ docker pull nats@sha256:988010f74b61749cfb82c28b50b47d26d0b972860ce6e9325a5afcde97713da2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.8.4-alpine3.15` - linux; amd64

```console
$ docker pull nats@sha256:f67ef794683ba4fcddc40bf871ad70eb258221443adcf1927b0270f257e73a74
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.7 MB (7701879 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57eb300f225ba4543fcd1c479ef7191723cf877d51078fa0d82de48cdff5c640`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:00 GMT
ADD file:f77e3f51f020890d22997e6c2ca98968b75b8bc8c463341a2010ff0655d4c88f in / 
# Tue, 09 Aug 2022 17:20:01 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 01:29:02 GMT
ENV NATS_SERVER=2.8.4
# Wed, 10 Aug 2022 01:29:04 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='75a53e10c640c8348bafe43300785d5147c91f60cd721c21ec896bc50727270a' ;; 		armhf) natsArch='arm6'; sha256='993a0d02ff9d0c74be31dc9e7ac1066659637c4897cc94ced2e0dc982fb428f3' ;; 		armv7) natsArch='arm7'; sha256='89e4191a0bc15c2196f2e6c1b2a3c4200576f6e8ec1176060b2a191c5e588b0d' ;; 		x86_64) natsArch='amd64'; sha256='da8c999ab0da5881fde68cba55238748d7310f28022fb78b9c07b420572a4b45' ;; 		x86) natsArch='386'; sha256='e94e5ec1076122e782527f4a98937c60c9eed4d04c6ba0364986cc58cd3ff8f8' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 10 Aug 2022 01:29:04 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 10 Aug 2022 01:29:04 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 10 Aug 2022 01:29:04 GMT
EXPOSE 4222 6222 8222
# Wed, 10 Aug 2022 01:29:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 10 Aug 2022 01:29:04 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9621f1afde84053b2f9b6ff34fc7f7460712247c01cbab483c5fa7132cf782ca`  
		Last Modified: Tue, 09 Aug 2022 17:20:52 GMT  
		Size: 2.8 MB (2823512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21c1a3defde00a6a87bb6d1f724a28b2cc109a3d0e6b086dc01265ecf07abf3b`  
		Last Modified: Wed, 10 Aug 2022 01:29:38 GMT  
		Size: 4.9 MB (4877365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d5c2bde7b7ca5bd606ae2db561e93e1addd87b05802f031fa6ec7a82f2828b0`  
		Last Modified: Wed, 10 Aug 2022 01:29:37 GMT  
		Size: 589.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a153c5b56febe9e8cc9d9df0925d160671c9aaffc633a61bdd7f368d42a1b96f`  
		Last Modified: Wed, 10 Aug 2022 01:29:37 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.8.4-alpine3.15` - linux; arm variant v6

```console
$ docker pull nats@sha256:91a3c5bbf8c80536df0dc91bebe4a3dbcf2901cdebb612e239a224e198e42c70
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7168331 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:87fc1a9a79541b69ed4655f072cef3d05408ecb373ad11d3a0f4c802831f0fa4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:29 GMT
ADD file:89cb25f97e17bed5c56311280efe5cfa78422d8ffbe36232195d13f94d67417e in / 
# Tue, 09 Aug 2022 17:49:29 GMT
CMD ["/bin/sh"]
# Thu, 11 Aug 2022 01:11:51 GMT
ENV NATS_SERVER=2.8.4
# Thu, 11 Aug 2022 01:11:53 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='75a53e10c640c8348bafe43300785d5147c91f60cd721c21ec896bc50727270a' ;; 		armhf) natsArch='arm6'; sha256='993a0d02ff9d0c74be31dc9e7ac1066659637c4897cc94ced2e0dc982fb428f3' ;; 		armv7) natsArch='arm7'; sha256='89e4191a0bc15c2196f2e6c1b2a3c4200576f6e8ec1176060b2a191c5e588b0d' ;; 		x86_64) natsArch='amd64'; sha256='da8c999ab0da5881fde68cba55238748d7310f28022fb78b9c07b420572a4b45' ;; 		x86) natsArch='386'; sha256='e94e5ec1076122e782527f4a98937c60c9eed4d04c6ba0364986cc58cd3ff8f8' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 11 Aug 2022 01:11:53 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 11 Aug 2022 01:11:54 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 11 Aug 2022 01:11:54 GMT
EXPOSE 4222 6222 8222
# Thu, 11 Aug 2022 01:11:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 Aug 2022 01:11:54 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:293b708aa6fb80967f27727d5c9c53ac9ba9cac376bed2ad02c17a5cca317b35`  
		Last Modified: Tue, 09 Aug 2022 17:50:52 GMT  
		Size: 2.6 MB (2631127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4efb85326bdd0b14d348830449cbdd93250414456c1d970d673f4002e8fdf93`  
		Last Modified: Thu, 11 Aug 2022 01:13:00 GMT  
		Size: 4.5 MB (4536202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef98b89db7bb29b263ede5d92c245cef1ed1dd56776120239a54f5f7692b2ff3`  
		Last Modified: Thu, 11 Aug 2022 01:13:00 GMT  
		Size: 589.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7a526f2148801e4c48011a6d1aa6ed5894b02339d145fbb462dae4f1692faa2`  
		Last Modified: Thu, 11 Aug 2022 01:13:00 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.8.4-alpine3.15` - linux; arm variant v7

```console
$ docker pull nats@sha256:a86957d0ea21981ed74f78c988f8b5202243dab5a43f68f0cd4d09be0e03acf7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.0 MB (6963329 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:02a19e2d0d29009797ec24843b88e7a35ebb4ca64c9a7b624b6be3290ec5f730`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 16:57:52 GMT
ADD file:0bd18306f21937a9572e68c768f05f4a9d8341b40c2379a7bfcb857c77734a14 in / 
# Tue, 09 Aug 2022 16:57:52 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 22:35:52 GMT
ENV NATS_SERVER=2.8.4
# Tue, 09 Aug 2022 22:35:55 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='75a53e10c640c8348bafe43300785d5147c91f60cd721c21ec896bc50727270a' ;; 		armhf) natsArch='arm6'; sha256='993a0d02ff9d0c74be31dc9e7ac1066659637c4897cc94ced2e0dc982fb428f3' ;; 		armv7) natsArch='arm7'; sha256='89e4191a0bc15c2196f2e6c1b2a3c4200576f6e8ec1176060b2a191c5e588b0d' ;; 		x86_64) natsArch='amd64'; sha256='da8c999ab0da5881fde68cba55238748d7310f28022fb78b9c07b420572a4b45' ;; 		x86) natsArch='386'; sha256='e94e5ec1076122e782527f4a98937c60c9eed4d04c6ba0364986cc58cd3ff8f8' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 09 Aug 2022 22:35:55 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 09 Aug 2022 22:35:55 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 09 Aug 2022 22:35:56 GMT
EXPOSE 4222 6222 8222
# Tue, 09 Aug 2022 22:35:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 09 Aug 2022 22:35:56 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:59775c20a906b1a49edcdc41a700a795998979d6ecf8f8d9cd7cbdf45e686d81`  
		Last Modified: Tue, 09 Aug 2022 16:59:12 GMT  
		Size: 2.4 MB (2435092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b55d1d06353a20f9de5b52fd408cb1d36cb23aea75e779350590565a5a4dea90`  
		Last Modified: Tue, 09 Aug 2022 22:37:42 GMT  
		Size: 4.5 MB (4527236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52e8be9dffb2c65f4e861ee01ddc4ec8362d0a2ca4ac53ad84fa5baf7b28b2d3`  
		Last Modified: Tue, 09 Aug 2022 22:37:41 GMT  
		Size: 589.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de94a2ef272b2e3ef327e7dbc685dfc8c6b58775169e3ec47a94fd5407841bf1`  
		Last Modified: Tue, 09 Aug 2022 22:37:41 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.8.4-alpine3.15` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:1d7154e4491475ff8fb864a26874ba8b4b250864ad515419c96432134b79a03a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7234771 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ff14469067b8205c1030c0740c47b13a4cd70a4cb3cd3e3f02472b056353df3b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:51 GMT
ADD file:4b51a9d40f20d2beb29d0759b161d2b9403493453beb509de4e86a5d98513f16 in / 
# Tue, 09 Aug 2022 17:39:51 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 20:52:27 GMT
ENV NATS_SERVER=2.8.4
# Tue, 09 Aug 2022 20:52:29 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='75a53e10c640c8348bafe43300785d5147c91f60cd721c21ec896bc50727270a' ;; 		armhf) natsArch='arm6'; sha256='993a0d02ff9d0c74be31dc9e7ac1066659637c4897cc94ced2e0dc982fb428f3' ;; 		armv7) natsArch='arm7'; sha256='89e4191a0bc15c2196f2e6c1b2a3c4200576f6e8ec1176060b2a191c5e588b0d' ;; 		x86_64) natsArch='amd64'; sha256='da8c999ab0da5881fde68cba55238748d7310f28022fb78b9c07b420572a4b45' ;; 		x86) natsArch='386'; sha256='e94e5ec1076122e782527f4a98937c60c9eed4d04c6ba0364986cc58cd3ff8f8' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 09 Aug 2022 20:52:31 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 09 Aug 2022 20:52:32 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 09 Aug 2022 20:52:32 GMT
EXPOSE 4222 6222 8222
# Tue, 09 Aug 2022 20:52:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 09 Aug 2022 20:52:34 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:47517142f6ba87eca6b7bdca1e0df160b74671c81e4b9605dad38c1862a43be3`  
		Last Modified: Tue, 09 Aug 2022 17:40:55 GMT  
		Size: 2.7 MB (2718439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf0beb1bc3611827acd1326750497c2cc98b9160ed5aec13a1112ad88b6ba136`  
		Last Modified: Tue, 09 Aug 2022 20:53:33 GMT  
		Size: 4.5 MB (4515360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a20f9bb5cbf9bb42bf80058089fa2cc11fe7eaad0e4342ef69340f9421360e9`  
		Last Modified: Tue, 09 Aug 2022 20:53:31 GMT  
		Size: 560.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b065ba618e0c23dec2ae44bb9555ee098a0827cf44bc5f30ae1d9448e11f668`  
		Last Modified: Tue, 09 Aug 2022 20:53:31 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.8.4-linux`

```console
$ docker pull nats@sha256:95b20a1c366e503cd8c0b97a45f2b00d70adfa53f7482237d1ef8fa2e792d2cf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.8.4-linux` - linux; amd64

```console
$ docker pull nats@sha256:796298f636925dedbbdfa537f42423dffd3a69b70c3a9bf4fd0982886a4b745d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4591595 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:842c053e15bdb38e697668b1f0721313203f7c2297eb6d79000f20858dc97854`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 27 May 2022 00:38:26 GMT
COPY file:c866dea678e8cec7cbd0798a1dbdefc45e992d9df374709f6000bac517589a1b in /nats-server 
# Fri, 27 May 2022 00:38:26 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 27 May 2022 00:38:27 GMT
EXPOSE 4222 6222 8222
# Fri, 27 May 2022 00:38:27 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 27 May 2022 00:38:27 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 27 May 2022 00:38:27 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:5e5797f39fa0527a3dd0a137353b40f97c71134e7eb38373d9791c5f1392885b`  
		Last Modified: Fri, 27 May 2022 00:39:15 GMT  
		Size: 4.6 MB (4591087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28c3b732adf61929b0b23ca08934cd89923e9cd9d7061544e76bbce57a9fa1e4`  
		Last Modified: Fri, 27 May 2022 00:39:14 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.8.4-linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:e0c28a95cdf6dd8a566d5c2394d09e6141dffb9107fe49f9385d6f19048bd955
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4245827 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cef47371f249bc862484ca7bd4dde2d7f77dc41bcb49cc49cceb17dfb2d4471f`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 11 Aug 2022 01:12:06 GMT
COPY file:8de8b0cf8e6edf54e413c112cd66aed537abed387a26ba749a9293d43cdf6594 in /nats-server 
# Thu, 11 Aug 2022 01:12:06 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 11 Aug 2022 01:12:06 GMT
EXPOSE 4222 6222 8222
# Thu, 11 Aug 2022 01:12:06 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 11 Aug 2022 01:12:06 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 11 Aug 2022 01:12:06 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:770fa9c168613edbe7aa7007d2cf8492c6570efc1ddab217fa32772c6b72dd48`  
		Last Modified: Thu, 26 May 2022 23:58:21 GMT  
		Size: 4.2 MB (4245317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bde47aae170f9c7e50b7bbea164ec0e0d02b9c05b603e7f7554e163183c02cd9`  
		Last Modified: Thu, 11 Aug 2022 01:13:30 GMT  
		Size: 510.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.8.4-linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:453c8fea5d37abc60f034f80bdb668a48c8e4f0900fce8b55fdb6ae7f2908d07
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4242795 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:508b00336aa0fc72bd1c3d33e5f447d1411e47221dfa1fa6085d6986b27045d7`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 22:36:22 GMT
COPY file:2841d6664b8897473f39b595b9aa4b28e749f587dc1afa4a0027ae507f37ee1f in /nats-server 
# Tue, 09 Aug 2022 22:36:22 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 09 Aug 2022 22:36:22 GMT
EXPOSE 4222 6222 8222
# Tue, 09 Aug 2022 22:36:22 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 09 Aug 2022 22:36:23 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 09 Aug 2022 22:36:23 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:f533e6e439ee51f1cf94458f821a20ed162b542d356340957091882ad881d5c1`  
		Last Modified: Fri, 27 May 2022 00:28:16 GMT  
		Size: 4.2 MB (4242287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:274ba9becbe1086958e9d56ab9452ec01f7fad6e3e68a34c49f1f299a5eab1ac`  
		Last Modified: Tue, 09 Aug 2022 22:38:14 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.8.4-linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:87b1afbd78a75ee48cb6b37a8522bbb01f5e9b5047b095b16cc4f241774a48d1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4227885 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9bce5ae01237736c7e0447d8cd1b2dbe252eab3ab5ac3b05d98b646b2575cee`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 26 May 2022 23:53:56 GMT
COPY file:2dbd94c6c11f89ceba3241f1efe469d0a06f0aae91abb77f3d79756676d0be57 in /nats-server 
# Thu, 26 May 2022 23:53:57 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 26 May 2022 23:53:57 GMT
EXPOSE 4222 6222 8222
# Thu, 26 May 2022 23:53:58 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 26 May 2022 23:53:59 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 26 May 2022 23:54:00 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:1c74770da2ea808362085edd6dead652091b3e3d34c1e32c50015a6a5bb36c02`  
		Last Modified: Thu, 26 May 2022 23:55:21 GMT  
		Size: 4.2 MB (4227378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:988af7458b707048622e497d5ae818b77d3a24ed0295a7897ced8f003179f7f9`  
		Last Modified: Thu, 26 May 2022 23:55:21 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.8.4-nanoserver`

```console
$ docker pull nats@sha256:92865bb073a2a8994aa5a8428fb857b4885c97d5c4af51ea7bdc5a56a93d4c69
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3287; amd64

### `nats:2.8.4-nanoserver` - windows version 10.0.17763.3287; amd64

```console
$ docker pull nats@sha256:1cedf48ffc2053a99d48b9d25a25aafa92106fbeeb92fe41aeb237d72e722664
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.8 MB (107843136 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:68f300c81963c2298e1d161245bcc24caccb02bc76fa1f665acbb465b70ff518`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 06 Aug 2022 18:08:38 GMT
RUN Apply image 10.0.17763.3287
# Wed, 10 Aug 2022 15:30:21 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 10 Aug 2022 15:30:22 GMT
RUN cmd /S /C #(nop) COPY file:88c957e774978b3592c1072a38fbf2d578a30b42e89604bf16828cccd9f86b17 in C:\nats-server.exe 
# Wed, 10 Aug 2022 15:30:23 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 10 Aug 2022 15:30:24 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 10 Aug 2022 15:30:25 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 10 Aug 2022 15:30:25 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:5c9d6483dab113d2d9b50fdf3156622aa2ec3d6faaed5664d15a5568032d1714`  
		Size: 103.2 MB (103204200 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:0a5df16ce106b092b5399678da04735c18584e4f99ea301691eb433072953e9a`  
		Last Modified: Wed, 10 Aug 2022 15:31:14 GMT  
		Size: 1.0 KB (1025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0da7ec45038de57bb4ae201762e54193e71ffc21892b700c1942bd3b85a10ac`  
		Last Modified: Wed, 10 Aug 2022 15:31:13 GMT  
		Size: 4.6 MB (4633133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d561d8a7d904db478c9c1e66aae419bb3d5333483d2d9f39f39e7bc62c02c56d`  
		Last Modified: Wed, 10 Aug 2022 15:31:12 GMT  
		Size: 1.7 KB (1653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f34e9538ca1cb2f704590a6fdaaef3b512b5ac93696534421be5f67017ffe8b9`  
		Last Modified: Wed, 10 Aug 2022 15:31:12 GMT  
		Size: 1.0 KB (1033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:660c54f5d2b9ddc91667f920a6f2103c75527be0b892d65aa55dd5bfa8afd3fe`  
		Last Modified: Wed, 10 Aug 2022 15:31:12 GMT  
		Size: 1.1 KB (1056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9356123a2a1af8afcf36b9979e254c522e7759fba29e96837a9d80c3a723f12c`  
		Last Modified: Wed, 10 Aug 2022 15:31:12 GMT  
		Size: 1.0 KB (1036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.8.4-nanoserver-1809`

```console
$ docker pull nats@sha256:92865bb073a2a8994aa5a8428fb857b4885c97d5c4af51ea7bdc5a56a93d4c69
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3287; amd64

### `nats:2.8.4-nanoserver-1809` - windows version 10.0.17763.3287; amd64

```console
$ docker pull nats@sha256:1cedf48ffc2053a99d48b9d25a25aafa92106fbeeb92fe41aeb237d72e722664
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.8 MB (107843136 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:68f300c81963c2298e1d161245bcc24caccb02bc76fa1f665acbb465b70ff518`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 06 Aug 2022 18:08:38 GMT
RUN Apply image 10.0.17763.3287
# Wed, 10 Aug 2022 15:30:21 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 10 Aug 2022 15:30:22 GMT
RUN cmd /S /C #(nop) COPY file:88c957e774978b3592c1072a38fbf2d578a30b42e89604bf16828cccd9f86b17 in C:\nats-server.exe 
# Wed, 10 Aug 2022 15:30:23 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 10 Aug 2022 15:30:24 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 10 Aug 2022 15:30:25 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 10 Aug 2022 15:30:25 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:5c9d6483dab113d2d9b50fdf3156622aa2ec3d6faaed5664d15a5568032d1714`  
		Size: 103.2 MB (103204200 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:0a5df16ce106b092b5399678da04735c18584e4f99ea301691eb433072953e9a`  
		Last Modified: Wed, 10 Aug 2022 15:31:14 GMT  
		Size: 1.0 KB (1025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0da7ec45038de57bb4ae201762e54193e71ffc21892b700c1942bd3b85a10ac`  
		Last Modified: Wed, 10 Aug 2022 15:31:13 GMT  
		Size: 4.6 MB (4633133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d561d8a7d904db478c9c1e66aae419bb3d5333483d2d9f39f39e7bc62c02c56d`  
		Last Modified: Wed, 10 Aug 2022 15:31:12 GMT  
		Size: 1.7 KB (1653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f34e9538ca1cb2f704590a6fdaaef3b512b5ac93696534421be5f67017ffe8b9`  
		Last Modified: Wed, 10 Aug 2022 15:31:12 GMT  
		Size: 1.0 KB (1033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:660c54f5d2b9ddc91667f920a6f2103c75527be0b892d65aa55dd5bfa8afd3fe`  
		Last Modified: Wed, 10 Aug 2022 15:31:12 GMT  
		Size: 1.1 KB (1056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9356123a2a1af8afcf36b9979e254c522e7759fba29e96837a9d80c3a723f12c`  
		Last Modified: Wed, 10 Aug 2022 15:31:12 GMT  
		Size: 1.0 KB (1036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.8.4-scratch`

```console
$ docker pull nats@sha256:95b20a1c366e503cd8c0b97a45f2b00d70adfa53f7482237d1ef8fa2e792d2cf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.8.4-scratch` - linux; amd64

```console
$ docker pull nats@sha256:796298f636925dedbbdfa537f42423dffd3a69b70c3a9bf4fd0982886a4b745d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4591595 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:842c053e15bdb38e697668b1f0721313203f7c2297eb6d79000f20858dc97854`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 27 May 2022 00:38:26 GMT
COPY file:c866dea678e8cec7cbd0798a1dbdefc45e992d9df374709f6000bac517589a1b in /nats-server 
# Fri, 27 May 2022 00:38:26 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 27 May 2022 00:38:27 GMT
EXPOSE 4222 6222 8222
# Fri, 27 May 2022 00:38:27 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 27 May 2022 00:38:27 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 27 May 2022 00:38:27 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:5e5797f39fa0527a3dd0a137353b40f97c71134e7eb38373d9791c5f1392885b`  
		Last Modified: Fri, 27 May 2022 00:39:15 GMT  
		Size: 4.6 MB (4591087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28c3b732adf61929b0b23ca08934cd89923e9cd9d7061544e76bbce57a9fa1e4`  
		Last Modified: Fri, 27 May 2022 00:39:14 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.8.4-scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:e0c28a95cdf6dd8a566d5c2394d09e6141dffb9107fe49f9385d6f19048bd955
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4245827 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cef47371f249bc862484ca7bd4dde2d7f77dc41bcb49cc49cceb17dfb2d4471f`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 11 Aug 2022 01:12:06 GMT
COPY file:8de8b0cf8e6edf54e413c112cd66aed537abed387a26ba749a9293d43cdf6594 in /nats-server 
# Thu, 11 Aug 2022 01:12:06 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 11 Aug 2022 01:12:06 GMT
EXPOSE 4222 6222 8222
# Thu, 11 Aug 2022 01:12:06 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 11 Aug 2022 01:12:06 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 11 Aug 2022 01:12:06 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:770fa9c168613edbe7aa7007d2cf8492c6570efc1ddab217fa32772c6b72dd48`  
		Last Modified: Thu, 26 May 2022 23:58:21 GMT  
		Size: 4.2 MB (4245317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bde47aae170f9c7e50b7bbea164ec0e0d02b9c05b603e7f7554e163183c02cd9`  
		Last Modified: Thu, 11 Aug 2022 01:13:30 GMT  
		Size: 510.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.8.4-scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:453c8fea5d37abc60f034f80bdb668a48c8e4f0900fce8b55fdb6ae7f2908d07
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4242795 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:508b00336aa0fc72bd1c3d33e5f447d1411e47221dfa1fa6085d6986b27045d7`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 22:36:22 GMT
COPY file:2841d6664b8897473f39b595b9aa4b28e749f587dc1afa4a0027ae507f37ee1f in /nats-server 
# Tue, 09 Aug 2022 22:36:22 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 09 Aug 2022 22:36:22 GMT
EXPOSE 4222 6222 8222
# Tue, 09 Aug 2022 22:36:22 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 09 Aug 2022 22:36:23 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 09 Aug 2022 22:36:23 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:f533e6e439ee51f1cf94458f821a20ed162b542d356340957091882ad881d5c1`  
		Last Modified: Fri, 27 May 2022 00:28:16 GMT  
		Size: 4.2 MB (4242287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:274ba9becbe1086958e9d56ab9452ec01f7fad6e3e68a34c49f1f299a5eab1ac`  
		Last Modified: Tue, 09 Aug 2022 22:38:14 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.8.4-scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:87b1afbd78a75ee48cb6b37a8522bbb01f5e9b5047b095b16cc4f241774a48d1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4227885 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9bce5ae01237736c7e0447d8cd1b2dbe252eab3ab5ac3b05d98b646b2575cee`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 26 May 2022 23:53:56 GMT
COPY file:2dbd94c6c11f89ceba3241f1efe469d0a06f0aae91abb77f3d79756676d0be57 in /nats-server 
# Thu, 26 May 2022 23:53:57 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 26 May 2022 23:53:57 GMT
EXPOSE 4222 6222 8222
# Thu, 26 May 2022 23:53:58 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 26 May 2022 23:53:59 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 26 May 2022 23:54:00 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:1c74770da2ea808362085edd6dead652091b3e3d34c1e32c50015a6a5bb36c02`  
		Last Modified: Thu, 26 May 2022 23:55:21 GMT  
		Size: 4.2 MB (4227378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:988af7458b707048622e497d5ae818b77d3a24ed0295a7897ced8f003179f7f9`  
		Last Modified: Thu, 26 May 2022 23:55:21 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.8.4-windowsservercore`

```console
$ docker pull nats@sha256:01e61321ee0c2a556640c7b04f8aaf24a2e46524bdec3c3b451c81dd170d0825
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3287; amd64

### `nats:2.8.4-windowsservercore` - windows version 10.0.17763.3287; amd64

```console
$ docker pull nats@sha256:9d7b29f769b82966a826e9eebcbff7022824cb343278b2c9dd87014b310f6bc2
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2683024603 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db44bc7e8ad93293de37107a4b87601bb8241a7d0762deac86c4a40d5ef262f0`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 06 Aug 2022 18:30:32 GMT
RUN Install update 10.0.17763.3287
# Wed, 10 Aug 2022 13:44:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Aug 2022 15:27:50 GMT
ENV NATS_DOCKERIZED=1
# Wed, 10 Aug 2022 15:27:51 GMT
ENV NATS_SERVER=2.8.4
# Wed, 10 Aug 2022 15:27:52 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.8.4/nats-server-v2.8.4-windows-amd64.zip
# Wed, 10 Aug 2022 15:27:53 GMT
ENV NATS_SERVER_SHASUM=911e8b77cf288c6e0997891d1400e5cc59dedd928e8f1685650c468674b52dc8
# Wed, 10 Aug 2022 15:28:46 GMT
RUN Set-PSDebug -Trace 2
# Wed, 10 Aug 2022 15:30:06 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 10 Aug 2022 15:30:07 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 10 Aug 2022 15:30:08 GMT
EXPOSE 4222 6222 8222
# Wed, 10 Aug 2022 15:30:09 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 10 Aug 2022 15:30:09 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:294d77ac553d7210b662d07674ef9e39a6c2e88dc15b9d2788d51e509bc8b54e`  
		Size: 800.5 MB (800546641 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:da71148bcd96afa7027d6172acee93aad6002bfbe87cadf468260667c09b3a89`  
		Last Modified: Wed, 10 Aug 2022 15:05:54 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26dc1c1069568772f0068cef343e37284e5f5e488dbfc15e037d95bce032d917`  
		Last Modified: Wed, 10 Aug 2022 15:30:56 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:890750ec51eb48085268f820e86c5b7ff873ff61875ed2b5df77150e4f667aff`  
		Last Modified: Wed, 10 Aug 2022 15:30:55 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da392874ede7ff085d580701bc4800047c2c07531b8dfb625241622eaba1995c`  
		Last Modified: Wed, 10 Aug 2022 15:30:55 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5a137a2c60ae08a2536eb110f4f21b9c80f33a03ab2d732da15f5f3de36c588`  
		Last Modified: Wed, 10 Aug 2022 15:30:55 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94cf94feb41446a9b0f0b35e7d386675c5b6256a8123327795d03d29f60b9400`  
		Last Modified: Wed, 10 Aug 2022 15:30:55 GMT  
		Size: 340.8 KB (340788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ab22594d9c79ecf05870151796e0c4df02facc4a9c10e99fcbea268fcbe9886`  
		Last Modified: Wed, 10 Aug 2022 15:30:53 GMT  
		Size: 5.0 MB (4957679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:143ae888a3c2d7c0f27e7935a85c8a25ef108bb2421c597eea07c8283cf18cbd`  
		Last Modified: Wed, 10 Aug 2022 15:30:52 GMT  
		Size: 2.0 KB (1996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b16fcb36242a120d1667323616c739921e5e2ccd627ea85b09d12df62368dc62`  
		Last Modified: Wed, 10 Aug 2022 15:30:53 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:478c487cdfd4835865c12e472c096f810ceb98ae9fa4d8a77c2080b01e22f095`  
		Last Modified: Wed, 10 Aug 2022 15:30:52 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2414c1290a3b460fc321c6c8630ddd4386a1f7192c489baca687f6ce4bd010e`  
		Last Modified: Wed, 10 Aug 2022 15:30:52 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.8.4-windowsservercore-1809`

```console
$ docker pull nats@sha256:01e61321ee0c2a556640c7b04f8aaf24a2e46524bdec3c3b451c81dd170d0825
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3287; amd64

### `nats:2.8.4-windowsservercore-1809` - windows version 10.0.17763.3287; amd64

```console
$ docker pull nats@sha256:9d7b29f769b82966a826e9eebcbff7022824cb343278b2c9dd87014b310f6bc2
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2683024603 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db44bc7e8ad93293de37107a4b87601bb8241a7d0762deac86c4a40d5ef262f0`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 06 Aug 2022 18:30:32 GMT
RUN Install update 10.0.17763.3287
# Wed, 10 Aug 2022 13:44:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Aug 2022 15:27:50 GMT
ENV NATS_DOCKERIZED=1
# Wed, 10 Aug 2022 15:27:51 GMT
ENV NATS_SERVER=2.8.4
# Wed, 10 Aug 2022 15:27:52 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.8.4/nats-server-v2.8.4-windows-amd64.zip
# Wed, 10 Aug 2022 15:27:53 GMT
ENV NATS_SERVER_SHASUM=911e8b77cf288c6e0997891d1400e5cc59dedd928e8f1685650c468674b52dc8
# Wed, 10 Aug 2022 15:28:46 GMT
RUN Set-PSDebug -Trace 2
# Wed, 10 Aug 2022 15:30:06 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 10 Aug 2022 15:30:07 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 10 Aug 2022 15:30:08 GMT
EXPOSE 4222 6222 8222
# Wed, 10 Aug 2022 15:30:09 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 10 Aug 2022 15:30:09 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:294d77ac553d7210b662d07674ef9e39a6c2e88dc15b9d2788d51e509bc8b54e`  
		Size: 800.5 MB (800546641 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:da71148bcd96afa7027d6172acee93aad6002bfbe87cadf468260667c09b3a89`  
		Last Modified: Wed, 10 Aug 2022 15:05:54 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26dc1c1069568772f0068cef343e37284e5f5e488dbfc15e037d95bce032d917`  
		Last Modified: Wed, 10 Aug 2022 15:30:56 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:890750ec51eb48085268f820e86c5b7ff873ff61875ed2b5df77150e4f667aff`  
		Last Modified: Wed, 10 Aug 2022 15:30:55 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da392874ede7ff085d580701bc4800047c2c07531b8dfb625241622eaba1995c`  
		Last Modified: Wed, 10 Aug 2022 15:30:55 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5a137a2c60ae08a2536eb110f4f21b9c80f33a03ab2d732da15f5f3de36c588`  
		Last Modified: Wed, 10 Aug 2022 15:30:55 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94cf94feb41446a9b0f0b35e7d386675c5b6256a8123327795d03d29f60b9400`  
		Last Modified: Wed, 10 Aug 2022 15:30:55 GMT  
		Size: 340.8 KB (340788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ab22594d9c79ecf05870151796e0c4df02facc4a9c10e99fcbea268fcbe9886`  
		Last Modified: Wed, 10 Aug 2022 15:30:53 GMT  
		Size: 5.0 MB (4957679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:143ae888a3c2d7c0f27e7935a85c8a25ef108bb2421c597eea07c8283cf18cbd`  
		Last Modified: Wed, 10 Aug 2022 15:30:52 GMT  
		Size: 2.0 KB (1996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b16fcb36242a120d1667323616c739921e5e2ccd627ea85b09d12df62368dc62`  
		Last Modified: Wed, 10 Aug 2022 15:30:53 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:478c487cdfd4835865c12e472c096f810ceb98ae9fa4d8a77c2080b01e22f095`  
		Last Modified: Wed, 10 Aug 2022 15:30:52 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2414c1290a3b460fc321c6c8630ddd4386a1f7192c489baca687f6ce4bd010e`  
		Last Modified: Wed, 10 Aug 2022 15:30:52 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:alpine`

```console
$ docker pull nats@sha256:988010f74b61749cfb82c28b50b47d26d0b972860ce6e9325a5afcde97713da2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:alpine` - linux; amd64

```console
$ docker pull nats@sha256:f67ef794683ba4fcddc40bf871ad70eb258221443adcf1927b0270f257e73a74
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.7 MB (7701879 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57eb300f225ba4543fcd1c479ef7191723cf877d51078fa0d82de48cdff5c640`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:00 GMT
ADD file:f77e3f51f020890d22997e6c2ca98968b75b8bc8c463341a2010ff0655d4c88f in / 
# Tue, 09 Aug 2022 17:20:01 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 01:29:02 GMT
ENV NATS_SERVER=2.8.4
# Wed, 10 Aug 2022 01:29:04 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='75a53e10c640c8348bafe43300785d5147c91f60cd721c21ec896bc50727270a' ;; 		armhf) natsArch='arm6'; sha256='993a0d02ff9d0c74be31dc9e7ac1066659637c4897cc94ced2e0dc982fb428f3' ;; 		armv7) natsArch='arm7'; sha256='89e4191a0bc15c2196f2e6c1b2a3c4200576f6e8ec1176060b2a191c5e588b0d' ;; 		x86_64) natsArch='amd64'; sha256='da8c999ab0da5881fde68cba55238748d7310f28022fb78b9c07b420572a4b45' ;; 		x86) natsArch='386'; sha256='e94e5ec1076122e782527f4a98937c60c9eed4d04c6ba0364986cc58cd3ff8f8' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 10 Aug 2022 01:29:04 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 10 Aug 2022 01:29:04 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 10 Aug 2022 01:29:04 GMT
EXPOSE 4222 6222 8222
# Wed, 10 Aug 2022 01:29:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 10 Aug 2022 01:29:04 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9621f1afde84053b2f9b6ff34fc7f7460712247c01cbab483c5fa7132cf782ca`  
		Last Modified: Tue, 09 Aug 2022 17:20:52 GMT  
		Size: 2.8 MB (2823512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21c1a3defde00a6a87bb6d1f724a28b2cc109a3d0e6b086dc01265ecf07abf3b`  
		Last Modified: Wed, 10 Aug 2022 01:29:38 GMT  
		Size: 4.9 MB (4877365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d5c2bde7b7ca5bd606ae2db561e93e1addd87b05802f031fa6ec7a82f2828b0`  
		Last Modified: Wed, 10 Aug 2022 01:29:37 GMT  
		Size: 589.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a153c5b56febe9e8cc9d9df0925d160671c9aaffc633a61bdd7f368d42a1b96f`  
		Last Modified: Wed, 10 Aug 2022 01:29:37 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:91a3c5bbf8c80536df0dc91bebe4a3dbcf2901cdebb612e239a224e198e42c70
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7168331 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:87fc1a9a79541b69ed4655f072cef3d05408ecb373ad11d3a0f4c802831f0fa4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:29 GMT
ADD file:89cb25f97e17bed5c56311280efe5cfa78422d8ffbe36232195d13f94d67417e in / 
# Tue, 09 Aug 2022 17:49:29 GMT
CMD ["/bin/sh"]
# Thu, 11 Aug 2022 01:11:51 GMT
ENV NATS_SERVER=2.8.4
# Thu, 11 Aug 2022 01:11:53 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='75a53e10c640c8348bafe43300785d5147c91f60cd721c21ec896bc50727270a' ;; 		armhf) natsArch='arm6'; sha256='993a0d02ff9d0c74be31dc9e7ac1066659637c4897cc94ced2e0dc982fb428f3' ;; 		armv7) natsArch='arm7'; sha256='89e4191a0bc15c2196f2e6c1b2a3c4200576f6e8ec1176060b2a191c5e588b0d' ;; 		x86_64) natsArch='amd64'; sha256='da8c999ab0da5881fde68cba55238748d7310f28022fb78b9c07b420572a4b45' ;; 		x86) natsArch='386'; sha256='e94e5ec1076122e782527f4a98937c60c9eed4d04c6ba0364986cc58cd3ff8f8' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 11 Aug 2022 01:11:53 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 11 Aug 2022 01:11:54 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 11 Aug 2022 01:11:54 GMT
EXPOSE 4222 6222 8222
# Thu, 11 Aug 2022 01:11:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 Aug 2022 01:11:54 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:293b708aa6fb80967f27727d5c9c53ac9ba9cac376bed2ad02c17a5cca317b35`  
		Last Modified: Tue, 09 Aug 2022 17:50:52 GMT  
		Size: 2.6 MB (2631127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4efb85326bdd0b14d348830449cbdd93250414456c1d970d673f4002e8fdf93`  
		Last Modified: Thu, 11 Aug 2022 01:13:00 GMT  
		Size: 4.5 MB (4536202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef98b89db7bb29b263ede5d92c245cef1ed1dd56776120239a54f5f7692b2ff3`  
		Last Modified: Thu, 11 Aug 2022 01:13:00 GMT  
		Size: 589.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7a526f2148801e4c48011a6d1aa6ed5894b02339d145fbb462dae4f1692faa2`  
		Last Modified: Thu, 11 Aug 2022 01:13:00 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:a86957d0ea21981ed74f78c988f8b5202243dab5a43f68f0cd4d09be0e03acf7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.0 MB (6963329 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:02a19e2d0d29009797ec24843b88e7a35ebb4ca64c9a7b624b6be3290ec5f730`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 16:57:52 GMT
ADD file:0bd18306f21937a9572e68c768f05f4a9d8341b40c2379a7bfcb857c77734a14 in / 
# Tue, 09 Aug 2022 16:57:52 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 22:35:52 GMT
ENV NATS_SERVER=2.8.4
# Tue, 09 Aug 2022 22:35:55 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='75a53e10c640c8348bafe43300785d5147c91f60cd721c21ec896bc50727270a' ;; 		armhf) natsArch='arm6'; sha256='993a0d02ff9d0c74be31dc9e7ac1066659637c4897cc94ced2e0dc982fb428f3' ;; 		armv7) natsArch='arm7'; sha256='89e4191a0bc15c2196f2e6c1b2a3c4200576f6e8ec1176060b2a191c5e588b0d' ;; 		x86_64) natsArch='amd64'; sha256='da8c999ab0da5881fde68cba55238748d7310f28022fb78b9c07b420572a4b45' ;; 		x86) natsArch='386'; sha256='e94e5ec1076122e782527f4a98937c60c9eed4d04c6ba0364986cc58cd3ff8f8' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 09 Aug 2022 22:35:55 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 09 Aug 2022 22:35:55 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 09 Aug 2022 22:35:56 GMT
EXPOSE 4222 6222 8222
# Tue, 09 Aug 2022 22:35:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 09 Aug 2022 22:35:56 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:59775c20a906b1a49edcdc41a700a795998979d6ecf8f8d9cd7cbdf45e686d81`  
		Last Modified: Tue, 09 Aug 2022 16:59:12 GMT  
		Size: 2.4 MB (2435092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b55d1d06353a20f9de5b52fd408cb1d36cb23aea75e779350590565a5a4dea90`  
		Last Modified: Tue, 09 Aug 2022 22:37:42 GMT  
		Size: 4.5 MB (4527236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52e8be9dffb2c65f4e861ee01ddc4ec8362d0a2ca4ac53ad84fa5baf7b28b2d3`  
		Last Modified: Tue, 09 Aug 2022 22:37:41 GMT  
		Size: 589.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de94a2ef272b2e3ef327e7dbc685dfc8c6b58775169e3ec47a94fd5407841bf1`  
		Last Modified: Tue, 09 Aug 2022 22:37:41 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:1d7154e4491475ff8fb864a26874ba8b4b250864ad515419c96432134b79a03a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7234771 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ff14469067b8205c1030c0740c47b13a4cd70a4cb3cd3e3f02472b056353df3b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:51 GMT
ADD file:4b51a9d40f20d2beb29d0759b161d2b9403493453beb509de4e86a5d98513f16 in / 
# Tue, 09 Aug 2022 17:39:51 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 20:52:27 GMT
ENV NATS_SERVER=2.8.4
# Tue, 09 Aug 2022 20:52:29 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='75a53e10c640c8348bafe43300785d5147c91f60cd721c21ec896bc50727270a' ;; 		armhf) natsArch='arm6'; sha256='993a0d02ff9d0c74be31dc9e7ac1066659637c4897cc94ced2e0dc982fb428f3' ;; 		armv7) natsArch='arm7'; sha256='89e4191a0bc15c2196f2e6c1b2a3c4200576f6e8ec1176060b2a191c5e588b0d' ;; 		x86_64) natsArch='amd64'; sha256='da8c999ab0da5881fde68cba55238748d7310f28022fb78b9c07b420572a4b45' ;; 		x86) natsArch='386'; sha256='e94e5ec1076122e782527f4a98937c60c9eed4d04c6ba0364986cc58cd3ff8f8' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 09 Aug 2022 20:52:31 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 09 Aug 2022 20:52:32 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 09 Aug 2022 20:52:32 GMT
EXPOSE 4222 6222 8222
# Tue, 09 Aug 2022 20:52:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 09 Aug 2022 20:52:34 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:47517142f6ba87eca6b7bdca1e0df160b74671c81e4b9605dad38c1862a43be3`  
		Last Modified: Tue, 09 Aug 2022 17:40:55 GMT  
		Size: 2.7 MB (2718439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf0beb1bc3611827acd1326750497c2cc98b9160ed5aec13a1112ad88b6ba136`  
		Last Modified: Tue, 09 Aug 2022 20:53:33 GMT  
		Size: 4.5 MB (4515360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a20f9bb5cbf9bb42bf80058089fa2cc11fe7eaad0e4342ef69340f9421360e9`  
		Last Modified: Tue, 09 Aug 2022 20:53:31 GMT  
		Size: 560.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b065ba618e0c23dec2ae44bb9555ee098a0827cf44bc5f30ae1d9448e11f668`  
		Last Modified: Tue, 09 Aug 2022 20:53:31 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:alpine3.15`

```console
$ docker pull nats@sha256:988010f74b61749cfb82c28b50b47d26d0b972860ce6e9325a5afcde97713da2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:alpine3.15` - linux; amd64

```console
$ docker pull nats@sha256:f67ef794683ba4fcddc40bf871ad70eb258221443adcf1927b0270f257e73a74
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.7 MB (7701879 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57eb300f225ba4543fcd1c479ef7191723cf877d51078fa0d82de48cdff5c640`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:00 GMT
ADD file:f77e3f51f020890d22997e6c2ca98968b75b8bc8c463341a2010ff0655d4c88f in / 
# Tue, 09 Aug 2022 17:20:01 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 01:29:02 GMT
ENV NATS_SERVER=2.8.4
# Wed, 10 Aug 2022 01:29:04 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='75a53e10c640c8348bafe43300785d5147c91f60cd721c21ec896bc50727270a' ;; 		armhf) natsArch='arm6'; sha256='993a0d02ff9d0c74be31dc9e7ac1066659637c4897cc94ced2e0dc982fb428f3' ;; 		armv7) natsArch='arm7'; sha256='89e4191a0bc15c2196f2e6c1b2a3c4200576f6e8ec1176060b2a191c5e588b0d' ;; 		x86_64) natsArch='amd64'; sha256='da8c999ab0da5881fde68cba55238748d7310f28022fb78b9c07b420572a4b45' ;; 		x86) natsArch='386'; sha256='e94e5ec1076122e782527f4a98937c60c9eed4d04c6ba0364986cc58cd3ff8f8' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 10 Aug 2022 01:29:04 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 10 Aug 2022 01:29:04 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 10 Aug 2022 01:29:04 GMT
EXPOSE 4222 6222 8222
# Wed, 10 Aug 2022 01:29:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 10 Aug 2022 01:29:04 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9621f1afde84053b2f9b6ff34fc7f7460712247c01cbab483c5fa7132cf782ca`  
		Last Modified: Tue, 09 Aug 2022 17:20:52 GMT  
		Size: 2.8 MB (2823512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21c1a3defde00a6a87bb6d1f724a28b2cc109a3d0e6b086dc01265ecf07abf3b`  
		Last Modified: Wed, 10 Aug 2022 01:29:38 GMT  
		Size: 4.9 MB (4877365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d5c2bde7b7ca5bd606ae2db561e93e1addd87b05802f031fa6ec7a82f2828b0`  
		Last Modified: Wed, 10 Aug 2022 01:29:37 GMT  
		Size: 589.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a153c5b56febe9e8cc9d9df0925d160671c9aaffc633a61bdd7f368d42a1b96f`  
		Last Modified: Wed, 10 Aug 2022 01:29:37 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.15` - linux; arm variant v6

```console
$ docker pull nats@sha256:91a3c5bbf8c80536df0dc91bebe4a3dbcf2901cdebb612e239a224e198e42c70
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7168331 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:87fc1a9a79541b69ed4655f072cef3d05408ecb373ad11d3a0f4c802831f0fa4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:29 GMT
ADD file:89cb25f97e17bed5c56311280efe5cfa78422d8ffbe36232195d13f94d67417e in / 
# Tue, 09 Aug 2022 17:49:29 GMT
CMD ["/bin/sh"]
# Thu, 11 Aug 2022 01:11:51 GMT
ENV NATS_SERVER=2.8.4
# Thu, 11 Aug 2022 01:11:53 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='75a53e10c640c8348bafe43300785d5147c91f60cd721c21ec896bc50727270a' ;; 		armhf) natsArch='arm6'; sha256='993a0d02ff9d0c74be31dc9e7ac1066659637c4897cc94ced2e0dc982fb428f3' ;; 		armv7) natsArch='arm7'; sha256='89e4191a0bc15c2196f2e6c1b2a3c4200576f6e8ec1176060b2a191c5e588b0d' ;; 		x86_64) natsArch='amd64'; sha256='da8c999ab0da5881fde68cba55238748d7310f28022fb78b9c07b420572a4b45' ;; 		x86) natsArch='386'; sha256='e94e5ec1076122e782527f4a98937c60c9eed4d04c6ba0364986cc58cd3ff8f8' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 11 Aug 2022 01:11:53 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 11 Aug 2022 01:11:54 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 11 Aug 2022 01:11:54 GMT
EXPOSE 4222 6222 8222
# Thu, 11 Aug 2022 01:11:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 Aug 2022 01:11:54 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:293b708aa6fb80967f27727d5c9c53ac9ba9cac376bed2ad02c17a5cca317b35`  
		Last Modified: Tue, 09 Aug 2022 17:50:52 GMT  
		Size: 2.6 MB (2631127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4efb85326bdd0b14d348830449cbdd93250414456c1d970d673f4002e8fdf93`  
		Last Modified: Thu, 11 Aug 2022 01:13:00 GMT  
		Size: 4.5 MB (4536202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef98b89db7bb29b263ede5d92c245cef1ed1dd56776120239a54f5f7692b2ff3`  
		Last Modified: Thu, 11 Aug 2022 01:13:00 GMT  
		Size: 589.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7a526f2148801e4c48011a6d1aa6ed5894b02339d145fbb462dae4f1692faa2`  
		Last Modified: Thu, 11 Aug 2022 01:13:00 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.15` - linux; arm variant v7

```console
$ docker pull nats@sha256:a86957d0ea21981ed74f78c988f8b5202243dab5a43f68f0cd4d09be0e03acf7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.0 MB (6963329 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:02a19e2d0d29009797ec24843b88e7a35ebb4ca64c9a7b624b6be3290ec5f730`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 16:57:52 GMT
ADD file:0bd18306f21937a9572e68c768f05f4a9d8341b40c2379a7bfcb857c77734a14 in / 
# Tue, 09 Aug 2022 16:57:52 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 22:35:52 GMT
ENV NATS_SERVER=2.8.4
# Tue, 09 Aug 2022 22:35:55 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='75a53e10c640c8348bafe43300785d5147c91f60cd721c21ec896bc50727270a' ;; 		armhf) natsArch='arm6'; sha256='993a0d02ff9d0c74be31dc9e7ac1066659637c4897cc94ced2e0dc982fb428f3' ;; 		armv7) natsArch='arm7'; sha256='89e4191a0bc15c2196f2e6c1b2a3c4200576f6e8ec1176060b2a191c5e588b0d' ;; 		x86_64) natsArch='amd64'; sha256='da8c999ab0da5881fde68cba55238748d7310f28022fb78b9c07b420572a4b45' ;; 		x86) natsArch='386'; sha256='e94e5ec1076122e782527f4a98937c60c9eed4d04c6ba0364986cc58cd3ff8f8' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 09 Aug 2022 22:35:55 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 09 Aug 2022 22:35:55 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 09 Aug 2022 22:35:56 GMT
EXPOSE 4222 6222 8222
# Tue, 09 Aug 2022 22:35:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 09 Aug 2022 22:35:56 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:59775c20a906b1a49edcdc41a700a795998979d6ecf8f8d9cd7cbdf45e686d81`  
		Last Modified: Tue, 09 Aug 2022 16:59:12 GMT  
		Size: 2.4 MB (2435092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b55d1d06353a20f9de5b52fd408cb1d36cb23aea75e779350590565a5a4dea90`  
		Last Modified: Tue, 09 Aug 2022 22:37:42 GMT  
		Size: 4.5 MB (4527236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52e8be9dffb2c65f4e861ee01ddc4ec8362d0a2ca4ac53ad84fa5baf7b28b2d3`  
		Last Modified: Tue, 09 Aug 2022 22:37:41 GMT  
		Size: 589.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de94a2ef272b2e3ef327e7dbc685dfc8c6b58775169e3ec47a94fd5407841bf1`  
		Last Modified: Tue, 09 Aug 2022 22:37:41 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.15` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:1d7154e4491475ff8fb864a26874ba8b4b250864ad515419c96432134b79a03a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7234771 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ff14469067b8205c1030c0740c47b13a4cd70a4cb3cd3e3f02472b056353df3b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:51 GMT
ADD file:4b51a9d40f20d2beb29d0759b161d2b9403493453beb509de4e86a5d98513f16 in / 
# Tue, 09 Aug 2022 17:39:51 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 20:52:27 GMT
ENV NATS_SERVER=2.8.4
# Tue, 09 Aug 2022 20:52:29 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='75a53e10c640c8348bafe43300785d5147c91f60cd721c21ec896bc50727270a' ;; 		armhf) natsArch='arm6'; sha256='993a0d02ff9d0c74be31dc9e7ac1066659637c4897cc94ced2e0dc982fb428f3' ;; 		armv7) natsArch='arm7'; sha256='89e4191a0bc15c2196f2e6c1b2a3c4200576f6e8ec1176060b2a191c5e588b0d' ;; 		x86_64) natsArch='amd64'; sha256='da8c999ab0da5881fde68cba55238748d7310f28022fb78b9c07b420572a4b45' ;; 		x86) natsArch='386'; sha256='e94e5ec1076122e782527f4a98937c60c9eed4d04c6ba0364986cc58cd3ff8f8' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 09 Aug 2022 20:52:31 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 09 Aug 2022 20:52:32 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 09 Aug 2022 20:52:32 GMT
EXPOSE 4222 6222 8222
# Tue, 09 Aug 2022 20:52:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 09 Aug 2022 20:52:34 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:47517142f6ba87eca6b7bdca1e0df160b74671c81e4b9605dad38c1862a43be3`  
		Last Modified: Tue, 09 Aug 2022 17:40:55 GMT  
		Size: 2.7 MB (2718439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf0beb1bc3611827acd1326750497c2cc98b9160ed5aec13a1112ad88b6ba136`  
		Last Modified: Tue, 09 Aug 2022 20:53:33 GMT  
		Size: 4.5 MB (4515360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a20f9bb5cbf9bb42bf80058089fa2cc11fe7eaad0e4342ef69340f9421360e9`  
		Last Modified: Tue, 09 Aug 2022 20:53:31 GMT  
		Size: 560.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b065ba618e0c23dec2ae44bb9555ee098a0827cf44bc5f30ae1d9448e11f668`  
		Last Modified: Tue, 09 Aug 2022 20:53:31 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:latest`

```console
$ docker pull nats@sha256:8f0cdcbc4c3597443fce869e75a759edb0d5a93fe98078f470a43204a6d7a729
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.3287; amd64

### `nats:latest` - linux; amd64

```console
$ docker pull nats@sha256:796298f636925dedbbdfa537f42423dffd3a69b70c3a9bf4fd0982886a4b745d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4591595 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:842c053e15bdb38e697668b1f0721313203f7c2297eb6d79000f20858dc97854`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 27 May 2022 00:38:26 GMT
COPY file:c866dea678e8cec7cbd0798a1dbdefc45e992d9df374709f6000bac517589a1b in /nats-server 
# Fri, 27 May 2022 00:38:26 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 27 May 2022 00:38:27 GMT
EXPOSE 4222 6222 8222
# Fri, 27 May 2022 00:38:27 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 27 May 2022 00:38:27 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 27 May 2022 00:38:27 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:5e5797f39fa0527a3dd0a137353b40f97c71134e7eb38373d9791c5f1392885b`  
		Last Modified: Fri, 27 May 2022 00:39:15 GMT  
		Size: 4.6 MB (4591087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28c3b732adf61929b0b23ca08934cd89923e9cd9d7061544e76bbce57a9fa1e4`  
		Last Modified: Fri, 27 May 2022 00:39:14 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm variant v6

```console
$ docker pull nats@sha256:e0c28a95cdf6dd8a566d5c2394d09e6141dffb9107fe49f9385d6f19048bd955
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4245827 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cef47371f249bc862484ca7bd4dde2d7f77dc41bcb49cc49cceb17dfb2d4471f`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 11 Aug 2022 01:12:06 GMT
COPY file:8de8b0cf8e6edf54e413c112cd66aed537abed387a26ba749a9293d43cdf6594 in /nats-server 
# Thu, 11 Aug 2022 01:12:06 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 11 Aug 2022 01:12:06 GMT
EXPOSE 4222 6222 8222
# Thu, 11 Aug 2022 01:12:06 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 11 Aug 2022 01:12:06 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 11 Aug 2022 01:12:06 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:770fa9c168613edbe7aa7007d2cf8492c6570efc1ddab217fa32772c6b72dd48`  
		Last Modified: Thu, 26 May 2022 23:58:21 GMT  
		Size: 4.2 MB (4245317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bde47aae170f9c7e50b7bbea164ec0e0d02b9c05b603e7f7554e163183c02cd9`  
		Last Modified: Thu, 11 Aug 2022 01:13:30 GMT  
		Size: 510.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm variant v7

```console
$ docker pull nats@sha256:453c8fea5d37abc60f034f80bdb668a48c8e4f0900fce8b55fdb6ae7f2908d07
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4242795 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:508b00336aa0fc72bd1c3d33e5f447d1411e47221dfa1fa6085d6986b27045d7`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 22:36:22 GMT
COPY file:2841d6664b8897473f39b595b9aa4b28e749f587dc1afa4a0027ae507f37ee1f in /nats-server 
# Tue, 09 Aug 2022 22:36:22 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 09 Aug 2022 22:36:22 GMT
EXPOSE 4222 6222 8222
# Tue, 09 Aug 2022 22:36:22 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 09 Aug 2022 22:36:23 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 09 Aug 2022 22:36:23 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:f533e6e439ee51f1cf94458f821a20ed162b542d356340957091882ad881d5c1`  
		Last Modified: Fri, 27 May 2022 00:28:16 GMT  
		Size: 4.2 MB (4242287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:274ba9becbe1086958e9d56ab9452ec01f7fad6e3e68a34c49f1f299a5eab1ac`  
		Last Modified: Tue, 09 Aug 2022 22:38:14 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:87b1afbd78a75ee48cb6b37a8522bbb01f5e9b5047b095b16cc4f241774a48d1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4227885 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9bce5ae01237736c7e0447d8cd1b2dbe252eab3ab5ac3b05d98b646b2575cee`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 26 May 2022 23:53:56 GMT
COPY file:2dbd94c6c11f89ceba3241f1efe469d0a06f0aae91abb77f3d79756676d0be57 in /nats-server 
# Thu, 26 May 2022 23:53:57 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 26 May 2022 23:53:57 GMT
EXPOSE 4222 6222 8222
# Thu, 26 May 2022 23:53:58 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 26 May 2022 23:53:59 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 26 May 2022 23:54:00 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:1c74770da2ea808362085edd6dead652091b3e3d34c1e32c50015a6a5bb36c02`  
		Last Modified: Thu, 26 May 2022 23:55:21 GMT  
		Size: 4.2 MB (4227378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:988af7458b707048622e497d5ae818b77d3a24ed0295a7897ced8f003179f7f9`  
		Last Modified: Thu, 26 May 2022 23:55:21 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - windows version 10.0.17763.3287; amd64

```console
$ docker pull nats@sha256:1cedf48ffc2053a99d48b9d25a25aafa92106fbeeb92fe41aeb237d72e722664
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.8 MB (107843136 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:68f300c81963c2298e1d161245bcc24caccb02bc76fa1f665acbb465b70ff518`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 06 Aug 2022 18:08:38 GMT
RUN Apply image 10.0.17763.3287
# Wed, 10 Aug 2022 15:30:21 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 10 Aug 2022 15:30:22 GMT
RUN cmd /S /C #(nop) COPY file:88c957e774978b3592c1072a38fbf2d578a30b42e89604bf16828cccd9f86b17 in C:\nats-server.exe 
# Wed, 10 Aug 2022 15:30:23 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 10 Aug 2022 15:30:24 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 10 Aug 2022 15:30:25 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 10 Aug 2022 15:30:25 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:5c9d6483dab113d2d9b50fdf3156622aa2ec3d6faaed5664d15a5568032d1714`  
		Size: 103.2 MB (103204200 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:0a5df16ce106b092b5399678da04735c18584e4f99ea301691eb433072953e9a`  
		Last Modified: Wed, 10 Aug 2022 15:31:14 GMT  
		Size: 1.0 KB (1025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0da7ec45038de57bb4ae201762e54193e71ffc21892b700c1942bd3b85a10ac`  
		Last Modified: Wed, 10 Aug 2022 15:31:13 GMT  
		Size: 4.6 MB (4633133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d561d8a7d904db478c9c1e66aae419bb3d5333483d2d9f39f39e7bc62c02c56d`  
		Last Modified: Wed, 10 Aug 2022 15:31:12 GMT  
		Size: 1.7 KB (1653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f34e9538ca1cb2f704590a6fdaaef3b512b5ac93696534421be5f67017ffe8b9`  
		Last Modified: Wed, 10 Aug 2022 15:31:12 GMT  
		Size: 1.0 KB (1033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:660c54f5d2b9ddc91667f920a6f2103c75527be0b892d65aa55dd5bfa8afd3fe`  
		Last Modified: Wed, 10 Aug 2022 15:31:12 GMT  
		Size: 1.1 KB (1056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9356123a2a1af8afcf36b9979e254c522e7759fba29e96837a9d80c3a723f12c`  
		Last Modified: Wed, 10 Aug 2022 15:31:12 GMT  
		Size: 1.0 KB (1036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:linux`

```console
$ docker pull nats@sha256:95b20a1c366e503cd8c0b97a45f2b00d70adfa53f7482237d1ef8fa2e792d2cf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:linux` - linux; amd64

```console
$ docker pull nats@sha256:796298f636925dedbbdfa537f42423dffd3a69b70c3a9bf4fd0982886a4b745d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4591595 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:842c053e15bdb38e697668b1f0721313203f7c2297eb6d79000f20858dc97854`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 27 May 2022 00:38:26 GMT
COPY file:c866dea678e8cec7cbd0798a1dbdefc45e992d9df374709f6000bac517589a1b in /nats-server 
# Fri, 27 May 2022 00:38:26 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 27 May 2022 00:38:27 GMT
EXPOSE 4222 6222 8222
# Fri, 27 May 2022 00:38:27 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 27 May 2022 00:38:27 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 27 May 2022 00:38:27 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:5e5797f39fa0527a3dd0a137353b40f97c71134e7eb38373d9791c5f1392885b`  
		Last Modified: Fri, 27 May 2022 00:39:15 GMT  
		Size: 4.6 MB (4591087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28c3b732adf61929b0b23ca08934cd89923e9cd9d7061544e76bbce57a9fa1e4`  
		Last Modified: Fri, 27 May 2022 00:39:14 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:e0c28a95cdf6dd8a566d5c2394d09e6141dffb9107fe49f9385d6f19048bd955
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4245827 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cef47371f249bc862484ca7bd4dde2d7f77dc41bcb49cc49cceb17dfb2d4471f`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 11 Aug 2022 01:12:06 GMT
COPY file:8de8b0cf8e6edf54e413c112cd66aed537abed387a26ba749a9293d43cdf6594 in /nats-server 
# Thu, 11 Aug 2022 01:12:06 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 11 Aug 2022 01:12:06 GMT
EXPOSE 4222 6222 8222
# Thu, 11 Aug 2022 01:12:06 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 11 Aug 2022 01:12:06 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 11 Aug 2022 01:12:06 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:770fa9c168613edbe7aa7007d2cf8492c6570efc1ddab217fa32772c6b72dd48`  
		Last Modified: Thu, 26 May 2022 23:58:21 GMT  
		Size: 4.2 MB (4245317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bde47aae170f9c7e50b7bbea164ec0e0d02b9c05b603e7f7554e163183c02cd9`  
		Last Modified: Thu, 11 Aug 2022 01:13:30 GMT  
		Size: 510.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:453c8fea5d37abc60f034f80bdb668a48c8e4f0900fce8b55fdb6ae7f2908d07
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4242795 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:508b00336aa0fc72bd1c3d33e5f447d1411e47221dfa1fa6085d6986b27045d7`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 22:36:22 GMT
COPY file:2841d6664b8897473f39b595b9aa4b28e749f587dc1afa4a0027ae507f37ee1f in /nats-server 
# Tue, 09 Aug 2022 22:36:22 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 09 Aug 2022 22:36:22 GMT
EXPOSE 4222 6222 8222
# Tue, 09 Aug 2022 22:36:22 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 09 Aug 2022 22:36:23 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 09 Aug 2022 22:36:23 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:f533e6e439ee51f1cf94458f821a20ed162b542d356340957091882ad881d5c1`  
		Last Modified: Fri, 27 May 2022 00:28:16 GMT  
		Size: 4.2 MB (4242287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:274ba9becbe1086958e9d56ab9452ec01f7fad6e3e68a34c49f1f299a5eab1ac`  
		Last Modified: Tue, 09 Aug 2022 22:38:14 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:87b1afbd78a75ee48cb6b37a8522bbb01f5e9b5047b095b16cc4f241774a48d1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4227885 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9bce5ae01237736c7e0447d8cd1b2dbe252eab3ab5ac3b05d98b646b2575cee`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 26 May 2022 23:53:56 GMT
COPY file:2dbd94c6c11f89ceba3241f1efe469d0a06f0aae91abb77f3d79756676d0be57 in /nats-server 
# Thu, 26 May 2022 23:53:57 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 26 May 2022 23:53:57 GMT
EXPOSE 4222 6222 8222
# Thu, 26 May 2022 23:53:58 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 26 May 2022 23:53:59 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 26 May 2022 23:54:00 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:1c74770da2ea808362085edd6dead652091b3e3d34c1e32c50015a6a5bb36c02`  
		Last Modified: Thu, 26 May 2022 23:55:21 GMT  
		Size: 4.2 MB (4227378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:988af7458b707048622e497d5ae818b77d3a24ed0295a7897ced8f003179f7f9`  
		Last Modified: Thu, 26 May 2022 23:55:21 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:nanoserver`

```console
$ docker pull nats@sha256:92865bb073a2a8994aa5a8428fb857b4885c97d5c4af51ea7bdc5a56a93d4c69
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3287; amd64

### `nats:nanoserver` - windows version 10.0.17763.3287; amd64

```console
$ docker pull nats@sha256:1cedf48ffc2053a99d48b9d25a25aafa92106fbeeb92fe41aeb237d72e722664
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.8 MB (107843136 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:68f300c81963c2298e1d161245bcc24caccb02bc76fa1f665acbb465b70ff518`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 06 Aug 2022 18:08:38 GMT
RUN Apply image 10.0.17763.3287
# Wed, 10 Aug 2022 15:30:21 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 10 Aug 2022 15:30:22 GMT
RUN cmd /S /C #(nop) COPY file:88c957e774978b3592c1072a38fbf2d578a30b42e89604bf16828cccd9f86b17 in C:\nats-server.exe 
# Wed, 10 Aug 2022 15:30:23 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 10 Aug 2022 15:30:24 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 10 Aug 2022 15:30:25 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 10 Aug 2022 15:30:25 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:5c9d6483dab113d2d9b50fdf3156622aa2ec3d6faaed5664d15a5568032d1714`  
		Size: 103.2 MB (103204200 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:0a5df16ce106b092b5399678da04735c18584e4f99ea301691eb433072953e9a`  
		Last Modified: Wed, 10 Aug 2022 15:31:14 GMT  
		Size: 1.0 KB (1025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0da7ec45038de57bb4ae201762e54193e71ffc21892b700c1942bd3b85a10ac`  
		Last Modified: Wed, 10 Aug 2022 15:31:13 GMT  
		Size: 4.6 MB (4633133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d561d8a7d904db478c9c1e66aae419bb3d5333483d2d9f39f39e7bc62c02c56d`  
		Last Modified: Wed, 10 Aug 2022 15:31:12 GMT  
		Size: 1.7 KB (1653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f34e9538ca1cb2f704590a6fdaaef3b512b5ac93696534421be5f67017ffe8b9`  
		Last Modified: Wed, 10 Aug 2022 15:31:12 GMT  
		Size: 1.0 KB (1033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:660c54f5d2b9ddc91667f920a6f2103c75527be0b892d65aa55dd5bfa8afd3fe`  
		Last Modified: Wed, 10 Aug 2022 15:31:12 GMT  
		Size: 1.1 KB (1056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9356123a2a1af8afcf36b9979e254c522e7759fba29e96837a9d80c3a723f12c`  
		Last Modified: Wed, 10 Aug 2022 15:31:12 GMT  
		Size: 1.0 KB (1036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:nanoserver-1809`

```console
$ docker pull nats@sha256:92865bb073a2a8994aa5a8428fb857b4885c97d5c4af51ea7bdc5a56a93d4c69
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3287; amd64

### `nats:nanoserver-1809` - windows version 10.0.17763.3287; amd64

```console
$ docker pull nats@sha256:1cedf48ffc2053a99d48b9d25a25aafa92106fbeeb92fe41aeb237d72e722664
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.8 MB (107843136 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:68f300c81963c2298e1d161245bcc24caccb02bc76fa1f665acbb465b70ff518`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 06 Aug 2022 18:08:38 GMT
RUN Apply image 10.0.17763.3287
# Wed, 10 Aug 2022 15:30:21 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 10 Aug 2022 15:30:22 GMT
RUN cmd /S /C #(nop) COPY file:88c957e774978b3592c1072a38fbf2d578a30b42e89604bf16828cccd9f86b17 in C:\nats-server.exe 
# Wed, 10 Aug 2022 15:30:23 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 10 Aug 2022 15:30:24 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 10 Aug 2022 15:30:25 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 10 Aug 2022 15:30:25 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:5c9d6483dab113d2d9b50fdf3156622aa2ec3d6faaed5664d15a5568032d1714`  
		Size: 103.2 MB (103204200 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:0a5df16ce106b092b5399678da04735c18584e4f99ea301691eb433072953e9a`  
		Last Modified: Wed, 10 Aug 2022 15:31:14 GMT  
		Size: 1.0 KB (1025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0da7ec45038de57bb4ae201762e54193e71ffc21892b700c1942bd3b85a10ac`  
		Last Modified: Wed, 10 Aug 2022 15:31:13 GMT  
		Size: 4.6 MB (4633133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d561d8a7d904db478c9c1e66aae419bb3d5333483d2d9f39f39e7bc62c02c56d`  
		Last Modified: Wed, 10 Aug 2022 15:31:12 GMT  
		Size: 1.7 KB (1653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f34e9538ca1cb2f704590a6fdaaef3b512b5ac93696534421be5f67017ffe8b9`  
		Last Modified: Wed, 10 Aug 2022 15:31:12 GMT  
		Size: 1.0 KB (1033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:660c54f5d2b9ddc91667f920a6f2103c75527be0b892d65aa55dd5bfa8afd3fe`  
		Last Modified: Wed, 10 Aug 2022 15:31:12 GMT  
		Size: 1.1 KB (1056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9356123a2a1af8afcf36b9979e254c522e7759fba29e96837a9d80c3a723f12c`  
		Last Modified: Wed, 10 Aug 2022 15:31:12 GMT  
		Size: 1.0 KB (1036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:scratch`

```console
$ docker pull nats@sha256:95b20a1c366e503cd8c0b97a45f2b00d70adfa53f7482237d1ef8fa2e792d2cf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:scratch` - linux; amd64

```console
$ docker pull nats@sha256:796298f636925dedbbdfa537f42423dffd3a69b70c3a9bf4fd0982886a4b745d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4591595 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:842c053e15bdb38e697668b1f0721313203f7c2297eb6d79000f20858dc97854`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 27 May 2022 00:38:26 GMT
COPY file:c866dea678e8cec7cbd0798a1dbdefc45e992d9df374709f6000bac517589a1b in /nats-server 
# Fri, 27 May 2022 00:38:26 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 27 May 2022 00:38:27 GMT
EXPOSE 4222 6222 8222
# Fri, 27 May 2022 00:38:27 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 27 May 2022 00:38:27 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 27 May 2022 00:38:27 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:5e5797f39fa0527a3dd0a137353b40f97c71134e7eb38373d9791c5f1392885b`  
		Last Modified: Fri, 27 May 2022 00:39:15 GMT  
		Size: 4.6 MB (4591087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28c3b732adf61929b0b23ca08934cd89923e9cd9d7061544e76bbce57a9fa1e4`  
		Last Modified: Fri, 27 May 2022 00:39:14 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:e0c28a95cdf6dd8a566d5c2394d09e6141dffb9107fe49f9385d6f19048bd955
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4245827 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cef47371f249bc862484ca7bd4dde2d7f77dc41bcb49cc49cceb17dfb2d4471f`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 11 Aug 2022 01:12:06 GMT
COPY file:8de8b0cf8e6edf54e413c112cd66aed537abed387a26ba749a9293d43cdf6594 in /nats-server 
# Thu, 11 Aug 2022 01:12:06 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 11 Aug 2022 01:12:06 GMT
EXPOSE 4222 6222 8222
# Thu, 11 Aug 2022 01:12:06 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 11 Aug 2022 01:12:06 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 11 Aug 2022 01:12:06 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:770fa9c168613edbe7aa7007d2cf8492c6570efc1ddab217fa32772c6b72dd48`  
		Last Modified: Thu, 26 May 2022 23:58:21 GMT  
		Size: 4.2 MB (4245317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bde47aae170f9c7e50b7bbea164ec0e0d02b9c05b603e7f7554e163183c02cd9`  
		Last Modified: Thu, 11 Aug 2022 01:13:30 GMT  
		Size: 510.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:453c8fea5d37abc60f034f80bdb668a48c8e4f0900fce8b55fdb6ae7f2908d07
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4242795 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:508b00336aa0fc72bd1c3d33e5f447d1411e47221dfa1fa6085d6986b27045d7`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 22:36:22 GMT
COPY file:2841d6664b8897473f39b595b9aa4b28e749f587dc1afa4a0027ae507f37ee1f in /nats-server 
# Tue, 09 Aug 2022 22:36:22 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 09 Aug 2022 22:36:22 GMT
EXPOSE 4222 6222 8222
# Tue, 09 Aug 2022 22:36:22 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 09 Aug 2022 22:36:23 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 09 Aug 2022 22:36:23 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:f533e6e439ee51f1cf94458f821a20ed162b542d356340957091882ad881d5c1`  
		Last Modified: Fri, 27 May 2022 00:28:16 GMT  
		Size: 4.2 MB (4242287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:274ba9becbe1086958e9d56ab9452ec01f7fad6e3e68a34c49f1f299a5eab1ac`  
		Last Modified: Tue, 09 Aug 2022 22:38:14 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:87b1afbd78a75ee48cb6b37a8522bbb01f5e9b5047b095b16cc4f241774a48d1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4227885 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9bce5ae01237736c7e0447d8cd1b2dbe252eab3ab5ac3b05d98b646b2575cee`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 26 May 2022 23:53:56 GMT
COPY file:2dbd94c6c11f89ceba3241f1efe469d0a06f0aae91abb77f3d79756676d0be57 in /nats-server 
# Thu, 26 May 2022 23:53:57 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 26 May 2022 23:53:57 GMT
EXPOSE 4222 6222 8222
# Thu, 26 May 2022 23:53:58 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 26 May 2022 23:53:59 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 26 May 2022 23:54:00 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:1c74770da2ea808362085edd6dead652091b3e3d34c1e32c50015a6a5bb36c02`  
		Last Modified: Thu, 26 May 2022 23:55:21 GMT  
		Size: 4.2 MB (4227378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:988af7458b707048622e497d5ae818b77d3a24ed0295a7897ced8f003179f7f9`  
		Last Modified: Thu, 26 May 2022 23:55:21 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:windowsservercore`

```console
$ docker pull nats@sha256:01e61321ee0c2a556640c7b04f8aaf24a2e46524bdec3c3b451c81dd170d0825
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3287; amd64

### `nats:windowsservercore` - windows version 10.0.17763.3287; amd64

```console
$ docker pull nats@sha256:9d7b29f769b82966a826e9eebcbff7022824cb343278b2c9dd87014b310f6bc2
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2683024603 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db44bc7e8ad93293de37107a4b87601bb8241a7d0762deac86c4a40d5ef262f0`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 06 Aug 2022 18:30:32 GMT
RUN Install update 10.0.17763.3287
# Wed, 10 Aug 2022 13:44:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Aug 2022 15:27:50 GMT
ENV NATS_DOCKERIZED=1
# Wed, 10 Aug 2022 15:27:51 GMT
ENV NATS_SERVER=2.8.4
# Wed, 10 Aug 2022 15:27:52 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.8.4/nats-server-v2.8.4-windows-amd64.zip
# Wed, 10 Aug 2022 15:27:53 GMT
ENV NATS_SERVER_SHASUM=911e8b77cf288c6e0997891d1400e5cc59dedd928e8f1685650c468674b52dc8
# Wed, 10 Aug 2022 15:28:46 GMT
RUN Set-PSDebug -Trace 2
# Wed, 10 Aug 2022 15:30:06 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 10 Aug 2022 15:30:07 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 10 Aug 2022 15:30:08 GMT
EXPOSE 4222 6222 8222
# Wed, 10 Aug 2022 15:30:09 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 10 Aug 2022 15:30:09 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:294d77ac553d7210b662d07674ef9e39a6c2e88dc15b9d2788d51e509bc8b54e`  
		Size: 800.5 MB (800546641 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:da71148bcd96afa7027d6172acee93aad6002bfbe87cadf468260667c09b3a89`  
		Last Modified: Wed, 10 Aug 2022 15:05:54 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26dc1c1069568772f0068cef343e37284e5f5e488dbfc15e037d95bce032d917`  
		Last Modified: Wed, 10 Aug 2022 15:30:56 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:890750ec51eb48085268f820e86c5b7ff873ff61875ed2b5df77150e4f667aff`  
		Last Modified: Wed, 10 Aug 2022 15:30:55 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da392874ede7ff085d580701bc4800047c2c07531b8dfb625241622eaba1995c`  
		Last Modified: Wed, 10 Aug 2022 15:30:55 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5a137a2c60ae08a2536eb110f4f21b9c80f33a03ab2d732da15f5f3de36c588`  
		Last Modified: Wed, 10 Aug 2022 15:30:55 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94cf94feb41446a9b0f0b35e7d386675c5b6256a8123327795d03d29f60b9400`  
		Last Modified: Wed, 10 Aug 2022 15:30:55 GMT  
		Size: 340.8 KB (340788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ab22594d9c79ecf05870151796e0c4df02facc4a9c10e99fcbea268fcbe9886`  
		Last Modified: Wed, 10 Aug 2022 15:30:53 GMT  
		Size: 5.0 MB (4957679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:143ae888a3c2d7c0f27e7935a85c8a25ef108bb2421c597eea07c8283cf18cbd`  
		Last Modified: Wed, 10 Aug 2022 15:30:52 GMT  
		Size: 2.0 KB (1996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b16fcb36242a120d1667323616c739921e5e2ccd627ea85b09d12df62368dc62`  
		Last Modified: Wed, 10 Aug 2022 15:30:53 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:478c487cdfd4835865c12e472c096f810ceb98ae9fa4d8a77c2080b01e22f095`  
		Last Modified: Wed, 10 Aug 2022 15:30:52 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2414c1290a3b460fc321c6c8630ddd4386a1f7192c489baca687f6ce4bd010e`  
		Last Modified: Wed, 10 Aug 2022 15:30:52 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:windowsservercore-1809`

```console
$ docker pull nats@sha256:01e61321ee0c2a556640c7b04f8aaf24a2e46524bdec3c3b451c81dd170d0825
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3287; amd64

### `nats:windowsservercore-1809` - windows version 10.0.17763.3287; amd64

```console
$ docker pull nats@sha256:9d7b29f769b82966a826e9eebcbff7022824cb343278b2c9dd87014b310f6bc2
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2683024603 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db44bc7e8ad93293de37107a4b87601bb8241a7d0762deac86c4a40d5ef262f0`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 06 Aug 2022 18:30:32 GMT
RUN Install update 10.0.17763.3287
# Wed, 10 Aug 2022 13:44:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Aug 2022 15:27:50 GMT
ENV NATS_DOCKERIZED=1
# Wed, 10 Aug 2022 15:27:51 GMT
ENV NATS_SERVER=2.8.4
# Wed, 10 Aug 2022 15:27:52 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.8.4/nats-server-v2.8.4-windows-amd64.zip
# Wed, 10 Aug 2022 15:27:53 GMT
ENV NATS_SERVER_SHASUM=911e8b77cf288c6e0997891d1400e5cc59dedd928e8f1685650c468674b52dc8
# Wed, 10 Aug 2022 15:28:46 GMT
RUN Set-PSDebug -Trace 2
# Wed, 10 Aug 2022 15:30:06 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 10 Aug 2022 15:30:07 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 10 Aug 2022 15:30:08 GMT
EXPOSE 4222 6222 8222
# Wed, 10 Aug 2022 15:30:09 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 10 Aug 2022 15:30:09 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:294d77ac553d7210b662d07674ef9e39a6c2e88dc15b9d2788d51e509bc8b54e`  
		Size: 800.5 MB (800546641 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:da71148bcd96afa7027d6172acee93aad6002bfbe87cadf468260667c09b3a89`  
		Last Modified: Wed, 10 Aug 2022 15:05:54 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26dc1c1069568772f0068cef343e37284e5f5e488dbfc15e037d95bce032d917`  
		Last Modified: Wed, 10 Aug 2022 15:30:56 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:890750ec51eb48085268f820e86c5b7ff873ff61875ed2b5df77150e4f667aff`  
		Last Modified: Wed, 10 Aug 2022 15:30:55 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da392874ede7ff085d580701bc4800047c2c07531b8dfb625241622eaba1995c`  
		Last Modified: Wed, 10 Aug 2022 15:30:55 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5a137a2c60ae08a2536eb110f4f21b9c80f33a03ab2d732da15f5f3de36c588`  
		Last Modified: Wed, 10 Aug 2022 15:30:55 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94cf94feb41446a9b0f0b35e7d386675c5b6256a8123327795d03d29f60b9400`  
		Last Modified: Wed, 10 Aug 2022 15:30:55 GMT  
		Size: 340.8 KB (340788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ab22594d9c79ecf05870151796e0c4df02facc4a9c10e99fcbea268fcbe9886`  
		Last Modified: Wed, 10 Aug 2022 15:30:53 GMT  
		Size: 5.0 MB (4957679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:143ae888a3c2d7c0f27e7935a85c8a25ef108bb2421c597eea07c8283cf18cbd`  
		Last Modified: Wed, 10 Aug 2022 15:30:52 GMT  
		Size: 2.0 KB (1996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b16fcb36242a120d1667323616c739921e5e2ccd627ea85b09d12df62368dc62`  
		Last Modified: Wed, 10 Aug 2022 15:30:53 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:478c487cdfd4835865c12e472c096f810ceb98ae9fa4d8a77c2080b01e22f095`  
		Last Modified: Wed, 10 Aug 2022 15:30:52 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2414c1290a3b460fc321c6c8630ddd4386a1f7192c489baca687f6ce4bd010e`  
		Last Modified: Wed, 10 Aug 2022 15:30:52 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
