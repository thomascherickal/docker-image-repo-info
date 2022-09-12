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
-	[`nats:2.9.0`](#nats290)
-	[`nats:2.9.0-alpine`](#nats290-alpine)
-	[`nats:2.9.0-alpine3.16`](#nats290-alpine316)
-	[`nats:2.9.0-linux`](#nats290-linux)
-	[`nats:2.9.0-nanoserver`](#nats290-nanoserver)
-	[`nats:2.9.0-nanoserver-1809`](#nats290-nanoserver-1809)
-	[`nats:2.9.0-scratch`](#nats290-scratch)
-	[`nats:2.9.0-windowsservercore`](#nats290-windowsservercore)
-	[`nats:2.9.0-windowsservercore-1809`](#nats290-windowsservercore-1809)
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
$ docker pull nats@sha256:0a52cec30c1dfc97dd7c6da084a8ca41cbb186c05091494c842e3eddaed6abba
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
$ docker pull nats@sha256:118585c5efc972b7af723b603811e3146ee914a26b54bcb892c506e8080d2fac
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4665258 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dcd239e963a20ee15d599802357bd7485cbf652b2c7a5d9c77d6485c07168bce`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 12 Sep 2022 18:49:48 GMT
COPY file:37e0cdc4ef3cae050b7a622e477f07fea2b89f2849c5c229803b12157182aa73 in /nats-server 
# Mon, 12 Sep 2022 18:49:48 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 12 Sep 2022 18:49:48 GMT
EXPOSE 4222 6222 8222
# Mon, 12 Sep 2022 18:49:48 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 12 Sep 2022 18:49:49 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 12 Sep 2022 18:49:49 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:5a54d3866fde0d65a287b5e00b2251f84936c27eed638ecef0fa1e8f95134bd6`  
		Last Modified: Mon, 12 Sep 2022 18:51:17 GMT  
		Size: 4.7 MB (4664750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2846c8f5d71bd80327105a167594ce9f72272f7c6a141cf378e206141a075ab`  
		Last Modified: Mon, 12 Sep 2022 18:51:15 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - linux; arm variant v7

```console
$ docker pull nats@sha256:a48ca64c022b50e4612f11b7b0bdf380e886ad449c8eb5a48624b2df386ceab4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4658073 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d43328d44a144020547148c52c8b0e257f2553339a66f15912b23f9b377d646d`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 12 Sep 2022 19:04:24 GMT
COPY file:88b07716d72d7b053cbf196c5562712b60f9d8875ee610f10839774e5aa8fd5e in /nats-server 
# Mon, 12 Sep 2022 19:04:24 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 12 Sep 2022 19:04:24 GMT
EXPOSE 4222 6222 8222
# Mon, 12 Sep 2022 19:04:24 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 12 Sep 2022 19:04:24 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 12 Sep 2022 19:04:25 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:fdc81c83bc1df58c4e224556b8224d1e7425add4047736a641d435c2097b7c10`  
		Last Modified: Mon, 12 Sep 2022 19:05:53 GMT  
		Size: 4.7 MB (4657565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:012d019d0dd61d6f41306e0a2009771e9b75625f46458973bd5db00d964d0d28`  
		Last Modified: Mon, 12 Sep 2022 19:05:52 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:09ddfc36cc0a08d6c04828f085c33c72e9641c712d6a0f1a78126e3267a10699
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4492569 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f28d3ca7b6670d9a7ef545dae9da4b8dfb8cb06b7f35b0a1fb9db72eb9327038`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 12 Sep 2022 18:50:22 GMT
COPY file:2793f903eadf963d049d95e6645a7fc0e41632a84eff5d1055bd4de285218751 in /nats-server 
# Mon, 12 Sep 2022 18:50:23 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 12 Sep 2022 18:50:23 GMT
EXPOSE 4222 6222 8222
# Mon, 12 Sep 2022 18:50:24 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 12 Sep 2022 18:50:25 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 12 Sep 2022 18:50:26 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:29ad82f04593c429e1ee6bf6c0c2687549bee49e553052bf5b67eec17de00f9b`  
		Last Modified: Mon, 12 Sep 2022 18:51:40 GMT  
		Size: 4.5 MB (4492060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:138da13517dd9cec8dbf0a87e0ce1dc5c15dbde69247362fc9895c07830e7f72`  
		Last Modified: Mon, 12 Sep 2022 18:51:39 GMT  
		Size: 509.0 B  
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
$ docker pull nats@sha256:b11d821dbbfdfc45b8c6ef3c2b284247161c786c84968f6582478043adce5b07
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
$ docker pull nats@sha256:085e2d3603a5ffeb96a5e784f11532c03a4f0840b6d68974c49981ff00ae2403
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7567312 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9cc82d17b5c2168901fc2938dbcf28eb4107996ab8bc9eb7f577b8561f959058`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:22 GMT
ADD file:e8733e8cc0a81e15ca4041760b6e27392c34171512d34405a9b262b1fff5c687 in / 
# Tue, 09 Aug 2022 17:49:22 GMT
CMD ["/bin/sh"]
# Mon, 12 Sep 2022 18:49:32 GMT
ENV NATS_SERVER=2.9.0
# Mon, 12 Sep 2022 18:49:34 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='b82c2910819bbf9350a5040ba2145b5e17d0faf8fca502505a4845ce1dcba441' ;; 		armhf) natsArch='arm6'; sha256='4f5f02bd8e06e83d685f7cba76620ae76cdfb7bd94f89e3aea323bbd0bf6ab3b' ;; 		armv7) natsArch='arm7'; sha256='0af9e816fb4a47274d2f7b1d1ebebd13568f0b70d466feefdd04cf1f14a0195f' ;; 		x86_64) natsArch='amd64'; sha256='e2c678de6900dfd126ce181a1103201ac6fb4e63f7112d320932a011db64d4e0' ;; 		x86) natsArch='386'; sha256='a617f94da82e2518549d2192d336be1da09674498553d117a95e167c4f3425ca' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 12 Sep 2022 18:49:35 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 12 Sep 2022 18:49:35 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 12 Sep 2022 18:49:35 GMT
EXPOSE 4222 6222 8222
# Mon, 12 Sep 2022 18:49:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 12 Sep 2022 18:49:35 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9506b835437abb4d8ba1683e00c500b8f77e1975e930b356fbb72f2dbdc274d9`  
		Last Modified: Tue, 09 Aug 2022 17:50:33 GMT  
		Size: 2.6 MB (2613965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00fddff5163e8c58a7497154f421e89aff54a43caec19e95069cc494375041aa`  
		Last Modified: Mon, 12 Sep 2022 18:50:45 GMT  
		Size: 5.0 MB (4952345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8019ab673b790b4ed63a97187571f3d0e5f4eb16dfa17399f6a243d11ff5722b`  
		Last Modified: Mon, 12 Sep 2022 18:50:44 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5ceaa398303883b9d5e592ce9aeaccbcf4b34b99a27a67d1578a0d6de4e69d3`  
		Last Modified: Mon, 12 Sep 2022 18:50:44 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:b95fa7ad87668f84962e4ef5abed9890fb57640ad479112b7f8c119bfa45dfda
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.4 MB (7363700 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b06933b06c17a95c6cd21d33dc823a06314c6b8517ebbfaf5b76c3b3cf11b155`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 16:57:44 GMT
ADD file:75521fe16320b193092588f6f31052c85e736965ceb11673de18bd14965a45e6 in / 
# Tue, 09 Aug 2022 16:57:44 GMT
CMD ["/bin/sh"]
# Mon, 12 Sep 2022 19:03:51 GMT
ENV NATS_SERVER=2.9.0
# Mon, 12 Sep 2022 19:03:54 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='b82c2910819bbf9350a5040ba2145b5e17d0faf8fca502505a4845ce1dcba441' ;; 		armhf) natsArch='arm6'; sha256='4f5f02bd8e06e83d685f7cba76620ae76cdfb7bd94f89e3aea323bbd0bf6ab3b' ;; 		armv7) natsArch='arm7'; sha256='0af9e816fb4a47274d2f7b1d1ebebd13568f0b70d466feefdd04cf1f14a0195f' ;; 		x86_64) natsArch='amd64'; sha256='e2c678de6900dfd126ce181a1103201ac6fb4e63f7112d320932a011db64d4e0' ;; 		x86) natsArch='386'; sha256='a617f94da82e2518549d2192d336be1da09674498553d117a95e167c4f3425ca' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 12 Sep 2022 19:03:54 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 12 Sep 2022 19:03:54 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 12 Sep 2022 19:03:54 GMT
EXPOSE 4222 6222 8222
# Mon, 12 Sep 2022 19:03:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 12 Sep 2022 19:03:55 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:c6556b3b6858c6fa1e328377cc2c4becdc9cd1bc3e7302aa7299936522cf93ba`  
		Last Modified: Tue, 09 Aug 2022 16:58:55 GMT  
		Size: 2.4 MB (2417065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3571a588810a8fe42813cdd7bcdc3e7b0be7bfc9084e38508f050f9826bba19`  
		Last Modified: Mon, 12 Sep 2022 19:05:22 GMT  
		Size: 4.9 MB (4945636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b1bcd898e16c2896f273f1b98e85da9bae6f599fb25e92fcdb2cab7ba63d64d`  
		Last Modified: Mon, 12 Sep 2022 19:05:20 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21cdba5340addabedb9b0801b2c8d51c4b04c684965b7e4f9b25e8b44573fb78`  
		Last Modified: Mon, 12 Sep 2022 19:05:20 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:7869a7f7498ee46895e9948a102087841874c9ee049696fe96edc9c4c5f7b17c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.5 MB (7482302 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e7cded970df3ac075d6833bcc805ee1cd39b6de8728ce00785f95016a231117`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Mon, 12 Sep 2022 18:50:02 GMT
ENV NATS_SERVER=2.9.0
# Mon, 12 Sep 2022 18:50:04 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='b82c2910819bbf9350a5040ba2145b5e17d0faf8fca502505a4845ce1dcba441' ;; 		armhf) natsArch='arm6'; sha256='4f5f02bd8e06e83d685f7cba76620ae76cdfb7bd94f89e3aea323bbd0bf6ab3b' ;; 		armv7) natsArch='arm7'; sha256='0af9e816fb4a47274d2f7b1d1ebebd13568f0b70d466feefdd04cf1f14a0195f' ;; 		x86_64) natsArch='amd64'; sha256='e2c678de6900dfd126ce181a1103201ac6fb4e63f7112d320932a011db64d4e0' ;; 		x86) natsArch='386'; sha256='a617f94da82e2518549d2192d336be1da09674498553d117a95e167c4f3425ca' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 12 Sep 2022 18:50:06 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 12 Sep 2022 18:50:07 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 12 Sep 2022 18:50:07 GMT
EXPOSE 4222 6222 8222
# Mon, 12 Sep 2022 18:50:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 12 Sep 2022 18:50:09 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f13b8dbdcf7252f528110cd3097a32511e40b830a0e7690d5d3c7c544cbbace`  
		Last Modified: Mon, 12 Sep 2022 18:51:12 GMT  
		Size: 4.8 MB (4773665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27cb8435ac86def6a8973b25db155dbd8c3f0c407542046937eb1ab78b99276e`  
		Last Modified: Mon, 12 Sep 2022 18:51:11 GMT  
		Size: 561.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a47359896823731079e2553b7cf975eba66a0095c51b1ccffbe582b732a6d41b`  
		Last Modified: Mon, 12 Sep 2022 18:51:11 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-alpine3.16`

```console
$ docker pull nats@sha256:e5a371efe6187d5965b819b9152fbad9583f1750370a76961665837cfc97407f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-alpine3.16` - linux; arm variant v6

```console
$ docker pull nats@sha256:085e2d3603a5ffeb96a5e784f11532c03a4f0840b6d68974c49981ff00ae2403
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7567312 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9cc82d17b5c2168901fc2938dbcf28eb4107996ab8bc9eb7f577b8561f959058`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:22 GMT
ADD file:e8733e8cc0a81e15ca4041760b6e27392c34171512d34405a9b262b1fff5c687 in / 
# Tue, 09 Aug 2022 17:49:22 GMT
CMD ["/bin/sh"]
# Mon, 12 Sep 2022 18:49:32 GMT
ENV NATS_SERVER=2.9.0
# Mon, 12 Sep 2022 18:49:34 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='b82c2910819bbf9350a5040ba2145b5e17d0faf8fca502505a4845ce1dcba441' ;; 		armhf) natsArch='arm6'; sha256='4f5f02bd8e06e83d685f7cba76620ae76cdfb7bd94f89e3aea323bbd0bf6ab3b' ;; 		armv7) natsArch='arm7'; sha256='0af9e816fb4a47274d2f7b1d1ebebd13568f0b70d466feefdd04cf1f14a0195f' ;; 		x86_64) natsArch='amd64'; sha256='e2c678de6900dfd126ce181a1103201ac6fb4e63f7112d320932a011db64d4e0' ;; 		x86) natsArch='386'; sha256='a617f94da82e2518549d2192d336be1da09674498553d117a95e167c4f3425ca' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 12 Sep 2022 18:49:35 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 12 Sep 2022 18:49:35 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 12 Sep 2022 18:49:35 GMT
EXPOSE 4222 6222 8222
# Mon, 12 Sep 2022 18:49:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 12 Sep 2022 18:49:35 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9506b835437abb4d8ba1683e00c500b8f77e1975e930b356fbb72f2dbdc274d9`  
		Last Modified: Tue, 09 Aug 2022 17:50:33 GMT  
		Size: 2.6 MB (2613965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00fddff5163e8c58a7497154f421e89aff54a43caec19e95069cc494375041aa`  
		Last Modified: Mon, 12 Sep 2022 18:50:45 GMT  
		Size: 5.0 MB (4952345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8019ab673b790b4ed63a97187571f3d0e5f4eb16dfa17399f6a243d11ff5722b`  
		Last Modified: Mon, 12 Sep 2022 18:50:44 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5ceaa398303883b9d5e592ce9aeaccbcf4b34b99a27a67d1578a0d6de4e69d3`  
		Last Modified: Mon, 12 Sep 2022 18:50:44 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.16` - linux; arm variant v7

```console
$ docker pull nats@sha256:b95fa7ad87668f84962e4ef5abed9890fb57640ad479112b7f8c119bfa45dfda
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.4 MB (7363700 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b06933b06c17a95c6cd21d33dc823a06314c6b8517ebbfaf5b76c3b3cf11b155`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 16:57:44 GMT
ADD file:75521fe16320b193092588f6f31052c85e736965ceb11673de18bd14965a45e6 in / 
# Tue, 09 Aug 2022 16:57:44 GMT
CMD ["/bin/sh"]
# Mon, 12 Sep 2022 19:03:51 GMT
ENV NATS_SERVER=2.9.0
# Mon, 12 Sep 2022 19:03:54 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='b82c2910819bbf9350a5040ba2145b5e17d0faf8fca502505a4845ce1dcba441' ;; 		armhf) natsArch='arm6'; sha256='4f5f02bd8e06e83d685f7cba76620ae76cdfb7bd94f89e3aea323bbd0bf6ab3b' ;; 		armv7) natsArch='arm7'; sha256='0af9e816fb4a47274d2f7b1d1ebebd13568f0b70d466feefdd04cf1f14a0195f' ;; 		x86_64) natsArch='amd64'; sha256='e2c678de6900dfd126ce181a1103201ac6fb4e63f7112d320932a011db64d4e0' ;; 		x86) natsArch='386'; sha256='a617f94da82e2518549d2192d336be1da09674498553d117a95e167c4f3425ca' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 12 Sep 2022 19:03:54 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 12 Sep 2022 19:03:54 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 12 Sep 2022 19:03:54 GMT
EXPOSE 4222 6222 8222
# Mon, 12 Sep 2022 19:03:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 12 Sep 2022 19:03:55 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:c6556b3b6858c6fa1e328377cc2c4becdc9cd1bc3e7302aa7299936522cf93ba`  
		Last Modified: Tue, 09 Aug 2022 16:58:55 GMT  
		Size: 2.4 MB (2417065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3571a588810a8fe42813cdd7bcdc3e7b0be7bfc9084e38508f050f9826bba19`  
		Last Modified: Mon, 12 Sep 2022 19:05:22 GMT  
		Size: 4.9 MB (4945636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b1bcd898e16c2896f273f1b98e85da9bae6f599fb25e92fcdb2cab7ba63d64d`  
		Last Modified: Mon, 12 Sep 2022 19:05:20 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21cdba5340addabedb9b0801b2c8d51c4b04c684965b7e4f9b25e8b44573fb78`  
		Last Modified: Mon, 12 Sep 2022 19:05:20 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.16` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:7869a7f7498ee46895e9948a102087841874c9ee049696fe96edc9c4c5f7b17c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.5 MB (7482302 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e7cded970df3ac075d6833bcc805ee1cd39b6de8728ce00785f95016a231117`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Mon, 12 Sep 2022 18:50:02 GMT
ENV NATS_SERVER=2.9.0
# Mon, 12 Sep 2022 18:50:04 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='b82c2910819bbf9350a5040ba2145b5e17d0faf8fca502505a4845ce1dcba441' ;; 		armhf) natsArch='arm6'; sha256='4f5f02bd8e06e83d685f7cba76620ae76cdfb7bd94f89e3aea323bbd0bf6ab3b' ;; 		armv7) natsArch='arm7'; sha256='0af9e816fb4a47274d2f7b1d1ebebd13568f0b70d466feefdd04cf1f14a0195f' ;; 		x86_64) natsArch='amd64'; sha256='e2c678de6900dfd126ce181a1103201ac6fb4e63f7112d320932a011db64d4e0' ;; 		x86) natsArch='386'; sha256='a617f94da82e2518549d2192d336be1da09674498553d117a95e167c4f3425ca' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 12 Sep 2022 18:50:06 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 12 Sep 2022 18:50:07 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 12 Sep 2022 18:50:07 GMT
EXPOSE 4222 6222 8222
# Mon, 12 Sep 2022 18:50:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 12 Sep 2022 18:50:09 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f13b8dbdcf7252f528110cd3097a32511e40b830a0e7690d5d3c7c544cbbace`  
		Last Modified: Mon, 12 Sep 2022 18:51:12 GMT  
		Size: 4.8 MB (4773665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27cb8435ac86def6a8973b25db155dbd8c3f0c407542046937eb1ab78b99276e`  
		Last Modified: Mon, 12 Sep 2022 18:51:11 GMT  
		Size: 561.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a47359896823731079e2553b7cf975eba66a0095c51b1ccffbe582b732a6d41b`  
		Last Modified: Mon, 12 Sep 2022 18:51:11 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-linux`

```console
$ docker pull nats@sha256:c337fb296c26591ce6b0cb0e926f3d5f9503d8d0018ec38f3c342dd7930839b5
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
$ docker pull nats@sha256:118585c5efc972b7af723b603811e3146ee914a26b54bcb892c506e8080d2fac
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4665258 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dcd239e963a20ee15d599802357bd7485cbf652b2c7a5d9c77d6485c07168bce`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 12 Sep 2022 18:49:48 GMT
COPY file:37e0cdc4ef3cae050b7a622e477f07fea2b89f2849c5c229803b12157182aa73 in /nats-server 
# Mon, 12 Sep 2022 18:49:48 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 12 Sep 2022 18:49:48 GMT
EXPOSE 4222 6222 8222
# Mon, 12 Sep 2022 18:49:48 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 12 Sep 2022 18:49:49 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 12 Sep 2022 18:49:49 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:5a54d3866fde0d65a287b5e00b2251f84936c27eed638ecef0fa1e8f95134bd6`  
		Last Modified: Mon, 12 Sep 2022 18:51:17 GMT  
		Size: 4.7 MB (4664750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2846c8f5d71bd80327105a167594ce9f72272f7c6a141cf378e206141a075ab`  
		Last Modified: Mon, 12 Sep 2022 18:51:15 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:a48ca64c022b50e4612f11b7b0bdf380e886ad449c8eb5a48624b2df386ceab4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4658073 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d43328d44a144020547148c52c8b0e257f2553339a66f15912b23f9b377d646d`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 12 Sep 2022 19:04:24 GMT
COPY file:88b07716d72d7b053cbf196c5562712b60f9d8875ee610f10839774e5aa8fd5e in /nats-server 
# Mon, 12 Sep 2022 19:04:24 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 12 Sep 2022 19:04:24 GMT
EXPOSE 4222 6222 8222
# Mon, 12 Sep 2022 19:04:24 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 12 Sep 2022 19:04:24 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 12 Sep 2022 19:04:25 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:fdc81c83bc1df58c4e224556b8224d1e7425add4047736a641d435c2097b7c10`  
		Last Modified: Mon, 12 Sep 2022 19:05:53 GMT  
		Size: 4.7 MB (4657565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:012d019d0dd61d6f41306e0a2009771e9b75625f46458973bd5db00d964d0d28`  
		Last Modified: Mon, 12 Sep 2022 19:05:52 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:09ddfc36cc0a08d6c04828f085c33c72e9641c712d6a0f1a78126e3267a10699
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4492569 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f28d3ca7b6670d9a7ef545dae9da4b8dfb8cb06b7f35b0a1fb9db72eb9327038`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 12 Sep 2022 18:50:22 GMT
COPY file:2793f903eadf963d049d95e6645a7fc0e41632a84eff5d1055bd4de285218751 in /nats-server 
# Mon, 12 Sep 2022 18:50:23 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 12 Sep 2022 18:50:23 GMT
EXPOSE 4222 6222 8222
# Mon, 12 Sep 2022 18:50:24 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 12 Sep 2022 18:50:25 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 12 Sep 2022 18:50:26 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:29ad82f04593c429e1ee6bf6c0c2687549bee49e553052bf5b67eec17de00f9b`  
		Last Modified: Mon, 12 Sep 2022 18:51:40 GMT  
		Size: 4.5 MB (4492060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:138da13517dd9cec8dbf0a87e0ce1dc5c15dbde69247362fc9895c07830e7f72`  
		Last Modified: Mon, 12 Sep 2022 18:51:39 GMT  
		Size: 509.0 B  
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
$ docker pull nats@sha256:c337fb296c26591ce6b0cb0e926f3d5f9503d8d0018ec38f3c342dd7930839b5
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
$ docker pull nats@sha256:118585c5efc972b7af723b603811e3146ee914a26b54bcb892c506e8080d2fac
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4665258 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dcd239e963a20ee15d599802357bd7485cbf652b2c7a5d9c77d6485c07168bce`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 12 Sep 2022 18:49:48 GMT
COPY file:37e0cdc4ef3cae050b7a622e477f07fea2b89f2849c5c229803b12157182aa73 in /nats-server 
# Mon, 12 Sep 2022 18:49:48 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 12 Sep 2022 18:49:48 GMT
EXPOSE 4222 6222 8222
# Mon, 12 Sep 2022 18:49:48 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 12 Sep 2022 18:49:49 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 12 Sep 2022 18:49:49 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:5a54d3866fde0d65a287b5e00b2251f84936c27eed638ecef0fa1e8f95134bd6`  
		Last Modified: Mon, 12 Sep 2022 18:51:17 GMT  
		Size: 4.7 MB (4664750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2846c8f5d71bd80327105a167594ce9f72272f7c6a141cf378e206141a075ab`  
		Last Modified: Mon, 12 Sep 2022 18:51:15 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:a48ca64c022b50e4612f11b7b0bdf380e886ad449c8eb5a48624b2df386ceab4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4658073 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d43328d44a144020547148c52c8b0e257f2553339a66f15912b23f9b377d646d`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 12 Sep 2022 19:04:24 GMT
COPY file:88b07716d72d7b053cbf196c5562712b60f9d8875ee610f10839774e5aa8fd5e in /nats-server 
# Mon, 12 Sep 2022 19:04:24 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 12 Sep 2022 19:04:24 GMT
EXPOSE 4222 6222 8222
# Mon, 12 Sep 2022 19:04:24 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 12 Sep 2022 19:04:24 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 12 Sep 2022 19:04:25 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:fdc81c83bc1df58c4e224556b8224d1e7425add4047736a641d435c2097b7c10`  
		Last Modified: Mon, 12 Sep 2022 19:05:53 GMT  
		Size: 4.7 MB (4657565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:012d019d0dd61d6f41306e0a2009771e9b75625f46458973bd5db00d964d0d28`  
		Last Modified: Mon, 12 Sep 2022 19:05:52 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:09ddfc36cc0a08d6c04828f085c33c72e9641c712d6a0f1a78126e3267a10699
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4492569 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f28d3ca7b6670d9a7ef545dae9da4b8dfb8cb06b7f35b0a1fb9db72eb9327038`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 12 Sep 2022 18:50:22 GMT
COPY file:2793f903eadf963d049d95e6645a7fc0e41632a84eff5d1055bd4de285218751 in /nats-server 
# Mon, 12 Sep 2022 18:50:23 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 12 Sep 2022 18:50:23 GMT
EXPOSE 4222 6222 8222
# Mon, 12 Sep 2022 18:50:24 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 12 Sep 2022 18:50:25 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 12 Sep 2022 18:50:26 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:29ad82f04593c429e1ee6bf6c0c2687549bee49e553052bf5b67eec17de00f9b`  
		Last Modified: Mon, 12 Sep 2022 18:51:40 GMT  
		Size: 4.5 MB (4492060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:138da13517dd9cec8dbf0a87e0ce1dc5c15dbde69247362fc9895c07830e7f72`  
		Last Modified: Mon, 12 Sep 2022 18:51:39 GMT  
		Size: 509.0 B  
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

## `nats:2.9`

```console
$ docker pull nats@sha256:715227a167bc72698c322a7834aebbd465393b5019ec3f1e668378d43a60b32a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9` - linux; arm variant v6

```console
$ docker pull nats@sha256:118585c5efc972b7af723b603811e3146ee914a26b54bcb892c506e8080d2fac
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4665258 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dcd239e963a20ee15d599802357bd7485cbf652b2c7a5d9c77d6485c07168bce`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 12 Sep 2022 18:49:48 GMT
COPY file:37e0cdc4ef3cae050b7a622e477f07fea2b89f2849c5c229803b12157182aa73 in /nats-server 
# Mon, 12 Sep 2022 18:49:48 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 12 Sep 2022 18:49:48 GMT
EXPOSE 4222 6222 8222
# Mon, 12 Sep 2022 18:49:48 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 12 Sep 2022 18:49:49 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 12 Sep 2022 18:49:49 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:5a54d3866fde0d65a287b5e00b2251f84936c27eed638ecef0fa1e8f95134bd6`  
		Last Modified: Mon, 12 Sep 2022 18:51:17 GMT  
		Size: 4.7 MB (4664750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2846c8f5d71bd80327105a167594ce9f72272f7c6a141cf378e206141a075ab`  
		Last Modified: Mon, 12 Sep 2022 18:51:15 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9` - linux; arm variant v7

```console
$ docker pull nats@sha256:a48ca64c022b50e4612f11b7b0bdf380e886ad449c8eb5a48624b2df386ceab4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4658073 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d43328d44a144020547148c52c8b0e257f2553339a66f15912b23f9b377d646d`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 12 Sep 2022 19:04:24 GMT
COPY file:88b07716d72d7b053cbf196c5562712b60f9d8875ee610f10839774e5aa8fd5e in /nats-server 
# Mon, 12 Sep 2022 19:04:24 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 12 Sep 2022 19:04:24 GMT
EXPOSE 4222 6222 8222
# Mon, 12 Sep 2022 19:04:24 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 12 Sep 2022 19:04:24 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 12 Sep 2022 19:04:25 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:fdc81c83bc1df58c4e224556b8224d1e7425add4047736a641d435c2097b7c10`  
		Last Modified: Mon, 12 Sep 2022 19:05:53 GMT  
		Size: 4.7 MB (4657565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:012d019d0dd61d6f41306e0a2009771e9b75625f46458973bd5db00d964d0d28`  
		Last Modified: Mon, 12 Sep 2022 19:05:52 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:09ddfc36cc0a08d6c04828f085c33c72e9641c712d6a0f1a78126e3267a10699
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4492569 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f28d3ca7b6670d9a7ef545dae9da4b8dfb8cb06b7f35b0a1fb9db72eb9327038`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 12 Sep 2022 18:50:22 GMT
COPY file:2793f903eadf963d049d95e6645a7fc0e41632a84eff5d1055bd4de285218751 in /nats-server 
# Mon, 12 Sep 2022 18:50:23 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 12 Sep 2022 18:50:23 GMT
EXPOSE 4222 6222 8222
# Mon, 12 Sep 2022 18:50:24 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 12 Sep 2022 18:50:25 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 12 Sep 2022 18:50:26 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:29ad82f04593c429e1ee6bf6c0c2687549bee49e553052bf5b67eec17de00f9b`  
		Last Modified: Mon, 12 Sep 2022 18:51:40 GMT  
		Size: 4.5 MB (4492060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:138da13517dd9cec8dbf0a87e0ce1dc5c15dbde69247362fc9895c07830e7f72`  
		Last Modified: Mon, 12 Sep 2022 18:51:39 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-alpine`

```console
$ docker pull nats@sha256:e5a371efe6187d5965b819b9152fbad9583f1750370a76961665837cfc97407f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:085e2d3603a5ffeb96a5e784f11532c03a4f0840b6d68974c49981ff00ae2403
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7567312 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9cc82d17b5c2168901fc2938dbcf28eb4107996ab8bc9eb7f577b8561f959058`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:22 GMT
ADD file:e8733e8cc0a81e15ca4041760b6e27392c34171512d34405a9b262b1fff5c687 in / 
# Tue, 09 Aug 2022 17:49:22 GMT
CMD ["/bin/sh"]
# Mon, 12 Sep 2022 18:49:32 GMT
ENV NATS_SERVER=2.9.0
# Mon, 12 Sep 2022 18:49:34 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='b82c2910819bbf9350a5040ba2145b5e17d0faf8fca502505a4845ce1dcba441' ;; 		armhf) natsArch='arm6'; sha256='4f5f02bd8e06e83d685f7cba76620ae76cdfb7bd94f89e3aea323bbd0bf6ab3b' ;; 		armv7) natsArch='arm7'; sha256='0af9e816fb4a47274d2f7b1d1ebebd13568f0b70d466feefdd04cf1f14a0195f' ;; 		x86_64) natsArch='amd64'; sha256='e2c678de6900dfd126ce181a1103201ac6fb4e63f7112d320932a011db64d4e0' ;; 		x86) natsArch='386'; sha256='a617f94da82e2518549d2192d336be1da09674498553d117a95e167c4f3425ca' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 12 Sep 2022 18:49:35 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 12 Sep 2022 18:49:35 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 12 Sep 2022 18:49:35 GMT
EXPOSE 4222 6222 8222
# Mon, 12 Sep 2022 18:49:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 12 Sep 2022 18:49:35 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9506b835437abb4d8ba1683e00c500b8f77e1975e930b356fbb72f2dbdc274d9`  
		Last Modified: Tue, 09 Aug 2022 17:50:33 GMT  
		Size: 2.6 MB (2613965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00fddff5163e8c58a7497154f421e89aff54a43caec19e95069cc494375041aa`  
		Last Modified: Mon, 12 Sep 2022 18:50:45 GMT  
		Size: 5.0 MB (4952345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8019ab673b790b4ed63a97187571f3d0e5f4eb16dfa17399f6a243d11ff5722b`  
		Last Modified: Mon, 12 Sep 2022 18:50:44 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5ceaa398303883b9d5e592ce9aeaccbcf4b34b99a27a67d1578a0d6de4e69d3`  
		Last Modified: Mon, 12 Sep 2022 18:50:44 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:b95fa7ad87668f84962e4ef5abed9890fb57640ad479112b7f8c119bfa45dfda
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.4 MB (7363700 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b06933b06c17a95c6cd21d33dc823a06314c6b8517ebbfaf5b76c3b3cf11b155`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 16:57:44 GMT
ADD file:75521fe16320b193092588f6f31052c85e736965ceb11673de18bd14965a45e6 in / 
# Tue, 09 Aug 2022 16:57:44 GMT
CMD ["/bin/sh"]
# Mon, 12 Sep 2022 19:03:51 GMT
ENV NATS_SERVER=2.9.0
# Mon, 12 Sep 2022 19:03:54 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='b82c2910819bbf9350a5040ba2145b5e17d0faf8fca502505a4845ce1dcba441' ;; 		armhf) natsArch='arm6'; sha256='4f5f02bd8e06e83d685f7cba76620ae76cdfb7bd94f89e3aea323bbd0bf6ab3b' ;; 		armv7) natsArch='arm7'; sha256='0af9e816fb4a47274d2f7b1d1ebebd13568f0b70d466feefdd04cf1f14a0195f' ;; 		x86_64) natsArch='amd64'; sha256='e2c678de6900dfd126ce181a1103201ac6fb4e63f7112d320932a011db64d4e0' ;; 		x86) natsArch='386'; sha256='a617f94da82e2518549d2192d336be1da09674498553d117a95e167c4f3425ca' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 12 Sep 2022 19:03:54 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 12 Sep 2022 19:03:54 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 12 Sep 2022 19:03:54 GMT
EXPOSE 4222 6222 8222
# Mon, 12 Sep 2022 19:03:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 12 Sep 2022 19:03:55 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:c6556b3b6858c6fa1e328377cc2c4becdc9cd1bc3e7302aa7299936522cf93ba`  
		Last Modified: Tue, 09 Aug 2022 16:58:55 GMT  
		Size: 2.4 MB (2417065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3571a588810a8fe42813cdd7bcdc3e7b0be7bfc9084e38508f050f9826bba19`  
		Last Modified: Mon, 12 Sep 2022 19:05:22 GMT  
		Size: 4.9 MB (4945636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b1bcd898e16c2896f273f1b98e85da9bae6f599fb25e92fcdb2cab7ba63d64d`  
		Last Modified: Mon, 12 Sep 2022 19:05:20 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21cdba5340addabedb9b0801b2c8d51c4b04c684965b7e4f9b25e8b44573fb78`  
		Last Modified: Mon, 12 Sep 2022 19:05:20 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:7869a7f7498ee46895e9948a102087841874c9ee049696fe96edc9c4c5f7b17c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.5 MB (7482302 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e7cded970df3ac075d6833bcc805ee1cd39b6de8728ce00785f95016a231117`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Mon, 12 Sep 2022 18:50:02 GMT
ENV NATS_SERVER=2.9.0
# Mon, 12 Sep 2022 18:50:04 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='b82c2910819bbf9350a5040ba2145b5e17d0faf8fca502505a4845ce1dcba441' ;; 		armhf) natsArch='arm6'; sha256='4f5f02bd8e06e83d685f7cba76620ae76cdfb7bd94f89e3aea323bbd0bf6ab3b' ;; 		armv7) natsArch='arm7'; sha256='0af9e816fb4a47274d2f7b1d1ebebd13568f0b70d466feefdd04cf1f14a0195f' ;; 		x86_64) natsArch='amd64'; sha256='e2c678de6900dfd126ce181a1103201ac6fb4e63f7112d320932a011db64d4e0' ;; 		x86) natsArch='386'; sha256='a617f94da82e2518549d2192d336be1da09674498553d117a95e167c4f3425ca' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 12 Sep 2022 18:50:06 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 12 Sep 2022 18:50:07 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 12 Sep 2022 18:50:07 GMT
EXPOSE 4222 6222 8222
# Mon, 12 Sep 2022 18:50:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 12 Sep 2022 18:50:09 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f13b8dbdcf7252f528110cd3097a32511e40b830a0e7690d5d3c7c544cbbace`  
		Last Modified: Mon, 12 Sep 2022 18:51:12 GMT  
		Size: 4.8 MB (4773665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27cb8435ac86def6a8973b25db155dbd8c3f0c407542046937eb1ab78b99276e`  
		Last Modified: Mon, 12 Sep 2022 18:51:11 GMT  
		Size: 561.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a47359896823731079e2553b7cf975eba66a0095c51b1ccffbe582b732a6d41b`  
		Last Modified: Mon, 12 Sep 2022 18:51:11 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-alpine3.16`

```console
$ docker pull nats@sha256:e5a371efe6187d5965b819b9152fbad9583f1750370a76961665837cfc97407f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9-alpine3.16` - linux; arm variant v6

```console
$ docker pull nats@sha256:085e2d3603a5ffeb96a5e784f11532c03a4f0840b6d68974c49981ff00ae2403
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7567312 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9cc82d17b5c2168901fc2938dbcf28eb4107996ab8bc9eb7f577b8561f959058`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:22 GMT
ADD file:e8733e8cc0a81e15ca4041760b6e27392c34171512d34405a9b262b1fff5c687 in / 
# Tue, 09 Aug 2022 17:49:22 GMT
CMD ["/bin/sh"]
# Mon, 12 Sep 2022 18:49:32 GMT
ENV NATS_SERVER=2.9.0
# Mon, 12 Sep 2022 18:49:34 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='b82c2910819bbf9350a5040ba2145b5e17d0faf8fca502505a4845ce1dcba441' ;; 		armhf) natsArch='arm6'; sha256='4f5f02bd8e06e83d685f7cba76620ae76cdfb7bd94f89e3aea323bbd0bf6ab3b' ;; 		armv7) natsArch='arm7'; sha256='0af9e816fb4a47274d2f7b1d1ebebd13568f0b70d466feefdd04cf1f14a0195f' ;; 		x86_64) natsArch='amd64'; sha256='e2c678de6900dfd126ce181a1103201ac6fb4e63f7112d320932a011db64d4e0' ;; 		x86) natsArch='386'; sha256='a617f94da82e2518549d2192d336be1da09674498553d117a95e167c4f3425ca' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 12 Sep 2022 18:49:35 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 12 Sep 2022 18:49:35 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 12 Sep 2022 18:49:35 GMT
EXPOSE 4222 6222 8222
# Mon, 12 Sep 2022 18:49:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 12 Sep 2022 18:49:35 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9506b835437abb4d8ba1683e00c500b8f77e1975e930b356fbb72f2dbdc274d9`  
		Last Modified: Tue, 09 Aug 2022 17:50:33 GMT  
		Size: 2.6 MB (2613965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00fddff5163e8c58a7497154f421e89aff54a43caec19e95069cc494375041aa`  
		Last Modified: Mon, 12 Sep 2022 18:50:45 GMT  
		Size: 5.0 MB (4952345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8019ab673b790b4ed63a97187571f3d0e5f4eb16dfa17399f6a243d11ff5722b`  
		Last Modified: Mon, 12 Sep 2022 18:50:44 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5ceaa398303883b9d5e592ce9aeaccbcf4b34b99a27a67d1578a0d6de4e69d3`  
		Last Modified: Mon, 12 Sep 2022 18:50:44 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-alpine3.16` - linux; arm variant v7

```console
$ docker pull nats@sha256:b95fa7ad87668f84962e4ef5abed9890fb57640ad479112b7f8c119bfa45dfda
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.4 MB (7363700 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b06933b06c17a95c6cd21d33dc823a06314c6b8517ebbfaf5b76c3b3cf11b155`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 16:57:44 GMT
ADD file:75521fe16320b193092588f6f31052c85e736965ceb11673de18bd14965a45e6 in / 
# Tue, 09 Aug 2022 16:57:44 GMT
CMD ["/bin/sh"]
# Mon, 12 Sep 2022 19:03:51 GMT
ENV NATS_SERVER=2.9.0
# Mon, 12 Sep 2022 19:03:54 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='b82c2910819bbf9350a5040ba2145b5e17d0faf8fca502505a4845ce1dcba441' ;; 		armhf) natsArch='arm6'; sha256='4f5f02bd8e06e83d685f7cba76620ae76cdfb7bd94f89e3aea323bbd0bf6ab3b' ;; 		armv7) natsArch='arm7'; sha256='0af9e816fb4a47274d2f7b1d1ebebd13568f0b70d466feefdd04cf1f14a0195f' ;; 		x86_64) natsArch='amd64'; sha256='e2c678de6900dfd126ce181a1103201ac6fb4e63f7112d320932a011db64d4e0' ;; 		x86) natsArch='386'; sha256='a617f94da82e2518549d2192d336be1da09674498553d117a95e167c4f3425ca' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 12 Sep 2022 19:03:54 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 12 Sep 2022 19:03:54 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 12 Sep 2022 19:03:54 GMT
EXPOSE 4222 6222 8222
# Mon, 12 Sep 2022 19:03:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 12 Sep 2022 19:03:55 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:c6556b3b6858c6fa1e328377cc2c4becdc9cd1bc3e7302aa7299936522cf93ba`  
		Last Modified: Tue, 09 Aug 2022 16:58:55 GMT  
		Size: 2.4 MB (2417065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3571a588810a8fe42813cdd7bcdc3e7b0be7bfc9084e38508f050f9826bba19`  
		Last Modified: Mon, 12 Sep 2022 19:05:22 GMT  
		Size: 4.9 MB (4945636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b1bcd898e16c2896f273f1b98e85da9bae6f599fb25e92fcdb2cab7ba63d64d`  
		Last Modified: Mon, 12 Sep 2022 19:05:20 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21cdba5340addabedb9b0801b2c8d51c4b04c684965b7e4f9b25e8b44573fb78`  
		Last Modified: Mon, 12 Sep 2022 19:05:20 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-alpine3.16` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:7869a7f7498ee46895e9948a102087841874c9ee049696fe96edc9c4c5f7b17c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.5 MB (7482302 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e7cded970df3ac075d6833bcc805ee1cd39b6de8728ce00785f95016a231117`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Mon, 12 Sep 2022 18:50:02 GMT
ENV NATS_SERVER=2.9.0
# Mon, 12 Sep 2022 18:50:04 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='b82c2910819bbf9350a5040ba2145b5e17d0faf8fca502505a4845ce1dcba441' ;; 		armhf) natsArch='arm6'; sha256='4f5f02bd8e06e83d685f7cba76620ae76cdfb7bd94f89e3aea323bbd0bf6ab3b' ;; 		armv7) natsArch='arm7'; sha256='0af9e816fb4a47274d2f7b1d1ebebd13568f0b70d466feefdd04cf1f14a0195f' ;; 		x86_64) natsArch='amd64'; sha256='e2c678de6900dfd126ce181a1103201ac6fb4e63f7112d320932a011db64d4e0' ;; 		x86) natsArch='386'; sha256='a617f94da82e2518549d2192d336be1da09674498553d117a95e167c4f3425ca' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 12 Sep 2022 18:50:06 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 12 Sep 2022 18:50:07 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 12 Sep 2022 18:50:07 GMT
EXPOSE 4222 6222 8222
# Mon, 12 Sep 2022 18:50:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 12 Sep 2022 18:50:09 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f13b8dbdcf7252f528110cd3097a32511e40b830a0e7690d5d3c7c544cbbace`  
		Last Modified: Mon, 12 Sep 2022 18:51:12 GMT  
		Size: 4.8 MB (4773665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27cb8435ac86def6a8973b25db155dbd8c3f0c407542046937eb1ab78b99276e`  
		Last Modified: Mon, 12 Sep 2022 18:51:11 GMT  
		Size: 561.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a47359896823731079e2553b7cf975eba66a0095c51b1ccffbe582b732a6d41b`  
		Last Modified: Mon, 12 Sep 2022 18:51:11 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-linux`

```console
$ docker pull nats@sha256:715227a167bc72698c322a7834aebbd465393b5019ec3f1e668378d43a60b32a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9-linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:118585c5efc972b7af723b603811e3146ee914a26b54bcb892c506e8080d2fac
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4665258 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dcd239e963a20ee15d599802357bd7485cbf652b2c7a5d9c77d6485c07168bce`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 12 Sep 2022 18:49:48 GMT
COPY file:37e0cdc4ef3cae050b7a622e477f07fea2b89f2849c5c229803b12157182aa73 in /nats-server 
# Mon, 12 Sep 2022 18:49:48 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 12 Sep 2022 18:49:48 GMT
EXPOSE 4222 6222 8222
# Mon, 12 Sep 2022 18:49:48 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 12 Sep 2022 18:49:49 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 12 Sep 2022 18:49:49 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:5a54d3866fde0d65a287b5e00b2251f84936c27eed638ecef0fa1e8f95134bd6`  
		Last Modified: Mon, 12 Sep 2022 18:51:17 GMT  
		Size: 4.7 MB (4664750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2846c8f5d71bd80327105a167594ce9f72272f7c6a141cf378e206141a075ab`  
		Last Modified: Mon, 12 Sep 2022 18:51:15 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:a48ca64c022b50e4612f11b7b0bdf380e886ad449c8eb5a48624b2df386ceab4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4658073 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d43328d44a144020547148c52c8b0e257f2553339a66f15912b23f9b377d646d`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 12 Sep 2022 19:04:24 GMT
COPY file:88b07716d72d7b053cbf196c5562712b60f9d8875ee610f10839774e5aa8fd5e in /nats-server 
# Mon, 12 Sep 2022 19:04:24 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 12 Sep 2022 19:04:24 GMT
EXPOSE 4222 6222 8222
# Mon, 12 Sep 2022 19:04:24 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 12 Sep 2022 19:04:24 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 12 Sep 2022 19:04:25 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:fdc81c83bc1df58c4e224556b8224d1e7425add4047736a641d435c2097b7c10`  
		Last Modified: Mon, 12 Sep 2022 19:05:53 GMT  
		Size: 4.7 MB (4657565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:012d019d0dd61d6f41306e0a2009771e9b75625f46458973bd5db00d964d0d28`  
		Last Modified: Mon, 12 Sep 2022 19:05:52 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:09ddfc36cc0a08d6c04828f085c33c72e9641c712d6a0f1a78126e3267a10699
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4492569 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f28d3ca7b6670d9a7ef545dae9da4b8dfb8cb06b7f35b0a1fb9db72eb9327038`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 12 Sep 2022 18:50:22 GMT
COPY file:2793f903eadf963d049d95e6645a7fc0e41632a84eff5d1055bd4de285218751 in /nats-server 
# Mon, 12 Sep 2022 18:50:23 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 12 Sep 2022 18:50:23 GMT
EXPOSE 4222 6222 8222
# Mon, 12 Sep 2022 18:50:24 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 12 Sep 2022 18:50:25 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 12 Sep 2022 18:50:26 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:29ad82f04593c429e1ee6bf6c0c2687549bee49e553052bf5b67eec17de00f9b`  
		Last Modified: Mon, 12 Sep 2022 18:51:40 GMT  
		Size: 4.5 MB (4492060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:138da13517dd9cec8dbf0a87e0ce1dc5c15dbde69247362fc9895c07830e7f72`  
		Last Modified: Mon, 12 Sep 2022 18:51:39 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-nanoserver`

```console
$ docker pull nats@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 0

## `nats:2.9-nanoserver-1809`

```console
$ docker pull nats@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 0

## `nats:2.9-scratch`

```console
$ docker pull nats@sha256:715227a167bc72698c322a7834aebbd465393b5019ec3f1e668378d43a60b32a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9-scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:118585c5efc972b7af723b603811e3146ee914a26b54bcb892c506e8080d2fac
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4665258 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dcd239e963a20ee15d599802357bd7485cbf652b2c7a5d9c77d6485c07168bce`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 12 Sep 2022 18:49:48 GMT
COPY file:37e0cdc4ef3cae050b7a622e477f07fea2b89f2849c5c229803b12157182aa73 in /nats-server 
# Mon, 12 Sep 2022 18:49:48 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 12 Sep 2022 18:49:48 GMT
EXPOSE 4222 6222 8222
# Mon, 12 Sep 2022 18:49:48 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 12 Sep 2022 18:49:49 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 12 Sep 2022 18:49:49 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:5a54d3866fde0d65a287b5e00b2251f84936c27eed638ecef0fa1e8f95134bd6`  
		Last Modified: Mon, 12 Sep 2022 18:51:17 GMT  
		Size: 4.7 MB (4664750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2846c8f5d71bd80327105a167594ce9f72272f7c6a141cf378e206141a075ab`  
		Last Modified: Mon, 12 Sep 2022 18:51:15 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:a48ca64c022b50e4612f11b7b0bdf380e886ad449c8eb5a48624b2df386ceab4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4658073 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d43328d44a144020547148c52c8b0e257f2553339a66f15912b23f9b377d646d`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 12 Sep 2022 19:04:24 GMT
COPY file:88b07716d72d7b053cbf196c5562712b60f9d8875ee610f10839774e5aa8fd5e in /nats-server 
# Mon, 12 Sep 2022 19:04:24 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 12 Sep 2022 19:04:24 GMT
EXPOSE 4222 6222 8222
# Mon, 12 Sep 2022 19:04:24 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 12 Sep 2022 19:04:24 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 12 Sep 2022 19:04:25 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:fdc81c83bc1df58c4e224556b8224d1e7425add4047736a641d435c2097b7c10`  
		Last Modified: Mon, 12 Sep 2022 19:05:53 GMT  
		Size: 4.7 MB (4657565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:012d019d0dd61d6f41306e0a2009771e9b75625f46458973bd5db00d964d0d28`  
		Last Modified: Mon, 12 Sep 2022 19:05:52 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:09ddfc36cc0a08d6c04828f085c33c72e9641c712d6a0f1a78126e3267a10699
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4492569 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f28d3ca7b6670d9a7ef545dae9da4b8dfb8cb06b7f35b0a1fb9db72eb9327038`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 12 Sep 2022 18:50:22 GMT
COPY file:2793f903eadf963d049d95e6645a7fc0e41632a84eff5d1055bd4de285218751 in /nats-server 
# Mon, 12 Sep 2022 18:50:23 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 12 Sep 2022 18:50:23 GMT
EXPOSE 4222 6222 8222
# Mon, 12 Sep 2022 18:50:24 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 12 Sep 2022 18:50:25 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 12 Sep 2022 18:50:26 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:29ad82f04593c429e1ee6bf6c0c2687549bee49e553052bf5b67eec17de00f9b`  
		Last Modified: Mon, 12 Sep 2022 18:51:40 GMT  
		Size: 4.5 MB (4492060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:138da13517dd9cec8dbf0a87e0ce1dc5c15dbde69247362fc9895c07830e7f72`  
		Last Modified: Mon, 12 Sep 2022 18:51:39 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-windowsservercore`

```console
$ docker pull nats@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 0

## `nats:2.9-windowsservercore-1809`

```console
$ docker pull nats@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 0

## `nats:2.9.0`

```console
$ docker pull nats@sha256:715227a167bc72698c322a7834aebbd465393b5019ec3f1e668378d43a60b32a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9.0` - linux; arm variant v6

```console
$ docker pull nats@sha256:118585c5efc972b7af723b603811e3146ee914a26b54bcb892c506e8080d2fac
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4665258 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dcd239e963a20ee15d599802357bd7485cbf652b2c7a5d9c77d6485c07168bce`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 12 Sep 2022 18:49:48 GMT
COPY file:37e0cdc4ef3cae050b7a622e477f07fea2b89f2849c5c229803b12157182aa73 in /nats-server 
# Mon, 12 Sep 2022 18:49:48 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 12 Sep 2022 18:49:48 GMT
EXPOSE 4222 6222 8222
# Mon, 12 Sep 2022 18:49:48 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 12 Sep 2022 18:49:49 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 12 Sep 2022 18:49:49 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:5a54d3866fde0d65a287b5e00b2251f84936c27eed638ecef0fa1e8f95134bd6`  
		Last Modified: Mon, 12 Sep 2022 18:51:17 GMT  
		Size: 4.7 MB (4664750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2846c8f5d71bd80327105a167594ce9f72272f7c6a141cf378e206141a075ab`  
		Last Modified: Mon, 12 Sep 2022 18:51:15 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.0` - linux; arm variant v7

```console
$ docker pull nats@sha256:a48ca64c022b50e4612f11b7b0bdf380e886ad449c8eb5a48624b2df386ceab4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4658073 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d43328d44a144020547148c52c8b0e257f2553339a66f15912b23f9b377d646d`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 12 Sep 2022 19:04:24 GMT
COPY file:88b07716d72d7b053cbf196c5562712b60f9d8875ee610f10839774e5aa8fd5e in /nats-server 
# Mon, 12 Sep 2022 19:04:24 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 12 Sep 2022 19:04:24 GMT
EXPOSE 4222 6222 8222
# Mon, 12 Sep 2022 19:04:24 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 12 Sep 2022 19:04:24 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 12 Sep 2022 19:04:25 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:fdc81c83bc1df58c4e224556b8224d1e7425add4047736a641d435c2097b7c10`  
		Last Modified: Mon, 12 Sep 2022 19:05:53 GMT  
		Size: 4.7 MB (4657565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:012d019d0dd61d6f41306e0a2009771e9b75625f46458973bd5db00d964d0d28`  
		Last Modified: Mon, 12 Sep 2022 19:05:52 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.0` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:09ddfc36cc0a08d6c04828f085c33c72e9641c712d6a0f1a78126e3267a10699
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4492569 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f28d3ca7b6670d9a7ef545dae9da4b8dfb8cb06b7f35b0a1fb9db72eb9327038`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 12 Sep 2022 18:50:22 GMT
COPY file:2793f903eadf963d049d95e6645a7fc0e41632a84eff5d1055bd4de285218751 in /nats-server 
# Mon, 12 Sep 2022 18:50:23 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 12 Sep 2022 18:50:23 GMT
EXPOSE 4222 6222 8222
# Mon, 12 Sep 2022 18:50:24 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 12 Sep 2022 18:50:25 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 12 Sep 2022 18:50:26 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:29ad82f04593c429e1ee6bf6c0c2687549bee49e553052bf5b67eec17de00f9b`  
		Last Modified: Mon, 12 Sep 2022 18:51:40 GMT  
		Size: 4.5 MB (4492060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:138da13517dd9cec8dbf0a87e0ce1dc5c15dbde69247362fc9895c07830e7f72`  
		Last Modified: Mon, 12 Sep 2022 18:51:39 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.0-alpine`

```console
$ docker pull nats@sha256:e5a371efe6187d5965b819b9152fbad9583f1750370a76961665837cfc97407f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9.0-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:085e2d3603a5ffeb96a5e784f11532c03a4f0840b6d68974c49981ff00ae2403
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7567312 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9cc82d17b5c2168901fc2938dbcf28eb4107996ab8bc9eb7f577b8561f959058`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:22 GMT
ADD file:e8733e8cc0a81e15ca4041760b6e27392c34171512d34405a9b262b1fff5c687 in / 
# Tue, 09 Aug 2022 17:49:22 GMT
CMD ["/bin/sh"]
# Mon, 12 Sep 2022 18:49:32 GMT
ENV NATS_SERVER=2.9.0
# Mon, 12 Sep 2022 18:49:34 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='b82c2910819bbf9350a5040ba2145b5e17d0faf8fca502505a4845ce1dcba441' ;; 		armhf) natsArch='arm6'; sha256='4f5f02bd8e06e83d685f7cba76620ae76cdfb7bd94f89e3aea323bbd0bf6ab3b' ;; 		armv7) natsArch='arm7'; sha256='0af9e816fb4a47274d2f7b1d1ebebd13568f0b70d466feefdd04cf1f14a0195f' ;; 		x86_64) natsArch='amd64'; sha256='e2c678de6900dfd126ce181a1103201ac6fb4e63f7112d320932a011db64d4e0' ;; 		x86) natsArch='386'; sha256='a617f94da82e2518549d2192d336be1da09674498553d117a95e167c4f3425ca' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 12 Sep 2022 18:49:35 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 12 Sep 2022 18:49:35 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 12 Sep 2022 18:49:35 GMT
EXPOSE 4222 6222 8222
# Mon, 12 Sep 2022 18:49:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 12 Sep 2022 18:49:35 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9506b835437abb4d8ba1683e00c500b8f77e1975e930b356fbb72f2dbdc274d9`  
		Last Modified: Tue, 09 Aug 2022 17:50:33 GMT  
		Size: 2.6 MB (2613965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00fddff5163e8c58a7497154f421e89aff54a43caec19e95069cc494375041aa`  
		Last Modified: Mon, 12 Sep 2022 18:50:45 GMT  
		Size: 5.0 MB (4952345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8019ab673b790b4ed63a97187571f3d0e5f4eb16dfa17399f6a243d11ff5722b`  
		Last Modified: Mon, 12 Sep 2022 18:50:44 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5ceaa398303883b9d5e592ce9aeaccbcf4b34b99a27a67d1578a0d6de4e69d3`  
		Last Modified: Mon, 12 Sep 2022 18:50:44 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.0-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:b95fa7ad87668f84962e4ef5abed9890fb57640ad479112b7f8c119bfa45dfda
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.4 MB (7363700 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b06933b06c17a95c6cd21d33dc823a06314c6b8517ebbfaf5b76c3b3cf11b155`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 16:57:44 GMT
ADD file:75521fe16320b193092588f6f31052c85e736965ceb11673de18bd14965a45e6 in / 
# Tue, 09 Aug 2022 16:57:44 GMT
CMD ["/bin/sh"]
# Mon, 12 Sep 2022 19:03:51 GMT
ENV NATS_SERVER=2.9.0
# Mon, 12 Sep 2022 19:03:54 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='b82c2910819bbf9350a5040ba2145b5e17d0faf8fca502505a4845ce1dcba441' ;; 		armhf) natsArch='arm6'; sha256='4f5f02bd8e06e83d685f7cba76620ae76cdfb7bd94f89e3aea323bbd0bf6ab3b' ;; 		armv7) natsArch='arm7'; sha256='0af9e816fb4a47274d2f7b1d1ebebd13568f0b70d466feefdd04cf1f14a0195f' ;; 		x86_64) natsArch='amd64'; sha256='e2c678de6900dfd126ce181a1103201ac6fb4e63f7112d320932a011db64d4e0' ;; 		x86) natsArch='386'; sha256='a617f94da82e2518549d2192d336be1da09674498553d117a95e167c4f3425ca' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 12 Sep 2022 19:03:54 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 12 Sep 2022 19:03:54 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 12 Sep 2022 19:03:54 GMT
EXPOSE 4222 6222 8222
# Mon, 12 Sep 2022 19:03:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 12 Sep 2022 19:03:55 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:c6556b3b6858c6fa1e328377cc2c4becdc9cd1bc3e7302aa7299936522cf93ba`  
		Last Modified: Tue, 09 Aug 2022 16:58:55 GMT  
		Size: 2.4 MB (2417065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3571a588810a8fe42813cdd7bcdc3e7b0be7bfc9084e38508f050f9826bba19`  
		Last Modified: Mon, 12 Sep 2022 19:05:22 GMT  
		Size: 4.9 MB (4945636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b1bcd898e16c2896f273f1b98e85da9bae6f599fb25e92fcdb2cab7ba63d64d`  
		Last Modified: Mon, 12 Sep 2022 19:05:20 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21cdba5340addabedb9b0801b2c8d51c4b04c684965b7e4f9b25e8b44573fb78`  
		Last Modified: Mon, 12 Sep 2022 19:05:20 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.0-alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:7869a7f7498ee46895e9948a102087841874c9ee049696fe96edc9c4c5f7b17c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.5 MB (7482302 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e7cded970df3ac075d6833bcc805ee1cd39b6de8728ce00785f95016a231117`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Mon, 12 Sep 2022 18:50:02 GMT
ENV NATS_SERVER=2.9.0
# Mon, 12 Sep 2022 18:50:04 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='b82c2910819bbf9350a5040ba2145b5e17d0faf8fca502505a4845ce1dcba441' ;; 		armhf) natsArch='arm6'; sha256='4f5f02bd8e06e83d685f7cba76620ae76cdfb7bd94f89e3aea323bbd0bf6ab3b' ;; 		armv7) natsArch='arm7'; sha256='0af9e816fb4a47274d2f7b1d1ebebd13568f0b70d466feefdd04cf1f14a0195f' ;; 		x86_64) natsArch='amd64'; sha256='e2c678de6900dfd126ce181a1103201ac6fb4e63f7112d320932a011db64d4e0' ;; 		x86) natsArch='386'; sha256='a617f94da82e2518549d2192d336be1da09674498553d117a95e167c4f3425ca' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 12 Sep 2022 18:50:06 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 12 Sep 2022 18:50:07 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 12 Sep 2022 18:50:07 GMT
EXPOSE 4222 6222 8222
# Mon, 12 Sep 2022 18:50:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 12 Sep 2022 18:50:09 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f13b8dbdcf7252f528110cd3097a32511e40b830a0e7690d5d3c7c544cbbace`  
		Last Modified: Mon, 12 Sep 2022 18:51:12 GMT  
		Size: 4.8 MB (4773665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27cb8435ac86def6a8973b25db155dbd8c3f0c407542046937eb1ab78b99276e`  
		Last Modified: Mon, 12 Sep 2022 18:51:11 GMT  
		Size: 561.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a47359896823731079e2553b7cf975eba66a0095c51b1ccffbe582b732a6d41b`  
		Last Modified: Mon, 12 Sep 2022 18:51:11 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.0-alpine3.16`

```console
$ docker pull nats@sha256:e5a371efe6187d5965b819b9152fbad9583f1750370a76961665837cfc97407f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9.0-alpine3.16` - linux; arm variant v6

```console
$ docker pull nats@sha256:085e2d3603a5ffeb96a5e784f11532c03a4f0840b6d68974c49981ff00ae2403
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7567312 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9cc82d17b5c2168901fc2938dbcf28eb4107996ab8bc9eb7f577b8561f959058`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:22 GMT
ADD file:e8733e8cc0a81e15ca4041760b6e27392c34171512d34405a9b262b1fff5c687 in / 
# Tue, 09 Aug 2022 17:49:22 GMT
CMD ["/bin/sh"]
# Mon, 12 Sep 2022 18:49:32 GMT
ENV NATS_SERVER=2.9.0
# Mon, 12 Sep 2022 18:49:34 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='b82c2910819bbf9350a5040ba2145b5e17d0faf8fca502505a4845ce1dcba441' ;; 		armhf) natsArch='arm6'; sha256='4f5f02bd8e06e83d685f7cba76620ae76cdfb7bd94f89e3aea323bbd0bf6ab3b' ;; 		armv7) natsArch='arm7'; sha256='0af9e816fb4a47274d2f7b1d1ebebd13568f0b70d466feefdd04cf1f14a0195f' ;; 		x86_64) natsArch='amd64'; sha256='e2c678de6900dfd126ce181a1103201ac6fb4e63f7112d320932a011db64d4e0' ;; 		x86) natsArch='386'; sha256='a617f94da82e2518549d2192d336be1da09674498553d117a95e167c4f3425ca' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 12 Sep 2022 18:49:35 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 12 Sep 2022 18:49:35 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 12 Sep 2022 18:49:35 GMT
EXPOSE 4222 6222 8222
# Mon, 12 Sep 2022 18:49:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 12 Sep 2022 18:49:35 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9506b835437abb4d8ba1683e00c500b8f77e1975e930b356fbb72f2dbdc274d9`  
		Last Modified: Tue, 09 Aug 2022 17:50:33 GMT  
		Size: 2.6 MB (2613965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00fddff5163e8c58a7497154f421e89aff54a43caec19e95069cc494375041aa`  
		Last Modified: Mon, 12 Sep 2022 18:50:45 GMT  
		Size: 5.0 MB (4952345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8019ab673b790b4ed63a97187571f3d0e5f4eb16dfa17399f6a243d11ff5722b`  
		Last Modified: Mon, 12 Sep 2022 18:50:44 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5ceaa398303883b9d5e592ce9aeaccbcf4b34b99a27a67d1578a0d6de4e69d3`  
		Last Modified: Mon, 12 Sep 2022 18:50:44 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.0-alpine3.16` - linux; arm variant v7

```console
$ docker pull nats@sha256:b95fa7ad87668f84962e4ef5abed9890fb57640ad479112b7f8c119bfa45dfda
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.4 MB (7363700 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b06933b06c17a95c6cd21d33dc823a06314c6b8517ebbfaf5b76c3b3cf11b155`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 16:57:44 GMT
ADD file:75521fe16320b193092588f6f31052c85e736965ceb11673de18bd14965a45e6 in / 
# Tue, 09 Aug 2022 16:57:44 GMT
CMD ["/bin/sh"]
# Mon, 12 Sep 2022 19:03:51 GMT
ENV NATS_SERVER=2.9.0
# Mon, 12 Sep 2022 19:03:54 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='b82c2910819bbf9350a5040ba2145b5e17d0faf8fca502505a4845ce1dcba441' ;; 		armhf) natsArch='arm6'; sha256='4f5f02bd8e06e83d685f7cba76620ae76cdfb7bd94f89e3aea323bbd0bf6ab3b' ;; 		armv7) natsArch='arm7'; sha256='0af9e816fb4a47274d2f7b1d1ebebd13568f0b70d466feefdd04cf1f14a0195f' ;; 		x86_64) natsArch='amd64'; sha256='e2c678de6900dfd126ce181a1103201ac6fb4e63f7112d320932a011db64d4e0' ;; 		x86) natsArch='386'; sha256='a617f94da82e2518549d2192d336be1da09674498553d117a95e167c4f3425ca' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 12 Sep 2022 19:03:54 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 12 Sep 2022 19:03:54 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 12 Sep 2022 19:03:54 GMT
EXPOSE 4222 6222 8222
# Mon, 12 Sep 2022 19:03:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 12 Sep 2022 19:03:55 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:c6556b3b6858c6fa1e328377cc2c4becdc9cd1bc3e7302aa7299936522cf93ba`  
		Last Modified: Tue, 09 Aug 2022 16:58:55 GMT  
		Size: 2.4 MB (2417065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3571a588810a8fe42813cdd7bcdc3e7b0be7bfc9084e38508f050f9826bba19`  
		Last Modified: Mon, 12 Sep 2022 19:05:22 GMT  
		Size: 4.9 MB (4945636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b1bcd898e16c2896f273f1b98e85da9bae6f599fb25e92fcdb2cab7ba63d64d`  
		Last Modified: Mon, 12 Sep 2022 19:05:20 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21cdba5340addabedb9b0801b2c8d51c4b04c684965b7e4f9b25e8b44573fb78`  
		Last Modified: Mon, 12 Sep 2022 19:05:20 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.0-alpine3.16` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:7869a7f7498ee46895e9948a102087841874c9ee049696fe96edc9c4c5f7b17c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.5 MB (7482302 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e7cded970df3ac075d6833bcc805ee1cd39b6de8728ce00785f95016a231117`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Mon, 12 Sep 2022 18:50:02 GMT
ENV NATS_SERVER=2.9.0
# Mon, 12 Sep 2022 18:50:04 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='b82c2910819bbf9350a5040ba2145b5e17d0faf8fca502505a4845ce1dcba441' ;; 		armhf) natsArch='arm6'; sha256='4f5f02bd8e06e83d685f7cba76620ae76cdfb7bd94f89e3aea323bbd0bf6ab3b' ;; 		armv7) natsArch='arm7'; sha256='0af9e816fb4a47274d2f7b1d1ebebd13568f0b70d466feefdd04cf1f14a0195f' ;; 		x86_64) natsArch='amd64'; sha256='e2c678de6900dfd126ce181a1103201ac6fb4e63f7112d320932a011db64d4e0' ;; 		x86) natsArch='386'; sha256='a617f94da82e2518549d2192d336be1da09674498553d117a95e167c4f3425ca' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 12 Sep 2022 18:50:06 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 12 Sep 2022 18:50:07 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 12 Sep 2022 18:50:07 GMT
EXPOSE 4222 6222 8222
# Mon, 12 Sep 2022 18:50:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 12 Sep 2022 18:50:09 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f13b8dbdcf7252f528110cd3097a32511e40b830a0e7690d5d3c7c544cbbace`  
		Last Modified: Mon, 12 Sep 2022 18:51:12 GMT  
		Size: 4.8 MB (4773665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27cb8435ac86def6a8973b25db155dbd8c3f0c407542046937eb1ab78b99276e`  
		Last Modified: Mon, 12 Sep 2022 18:51:11 GMT  
		Size: 561.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a47359896823731079e2553b7cf975eba66a0095c51b1ccffbe582b732a6d41b`  
		Last Modified: Mon, 12 Sep 2022 18:51:11 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.0-linux`

```console
$ docker pull nats@sha256:715227a167bc72698c322a7834aebbd465393b5019ec3f1e668378d43a60b32a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9.0-linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:118585c5efc972b7af723b603811e3146ee914a26b54bcb892c506e8080d2fac
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4665258 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dcd239e963a20ee15d599802357bd7485cbf652b2c7a5d9c77d6485c07168bce`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 12 Sep 2022 18:49:48 GMT
COPY file:37e0cdc4ef3cae050b7a622e477f07fea2b89f2849c5c229803b12157182aa73 in /nats-server 
# Mon, 12 Sep 2022 18:49:48 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 12 Sep 2022 18:49:48 GMT
EXPOSE 4222 6222 8222
# Mon, 12 Sep 2022 18:49:48 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 12 Sep 2022 18:49:49 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 12 Sep 2022 18:49:49 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:5a54d3866fde0d65a287b5e00b2251f84936c27eed638ecef0fa1e8f95134bd6`  
		Last Modified: Mon, 12 Sep 2022 18:51:17 GMT  
		Size: 4.7 MB (4664750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2846c8f5d71bd80327105a167594ce9f72272f7c6a141cf378e206141a075ab`  
		Last Modified: Mon, 12 Sep 2022 18:51:15 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.0-linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:a48ca64c022b50e4612f11b7b0bdf380e886ad449c8eb5a48624b2df386ceab4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4658073 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d43328d44a144020547148c52c8b0e257f2553339a66f15912b23f9b377d646d`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 12 Sep 2022 19:04:24 GMT
COPY file:88b07716d72d7b053cbf196c5562712b60f9d8875ee610f10839774e5aa8fd5e in /nats-server 
# Mon, 12 Sep 2022 19:04:24 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 12 Sep 2022 19:04:24 GMT
EXPOSE 4222 6222 8222
# Mon, 12 Sep 2022 19:04:24 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 12 Sep 2022 19:04:24 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 12 Sep 2022 19:04:25 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:fdc81c83bc1df58c4e224556b8224d1e7425add4047736a641d435c2097b7c10`  
		Last Modified: Mon, 12 Sep 2022 19:05:53 GMT  
		Size: 4.7 MB (4657565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:012d019d0dd61d6f41306e0a2009771e9b75625f46458973bd5db00d964d0d28`  
		Last Modified: Mon, 12 Sep 2022 19:05:52 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.0-linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:09ddfc36cc0a08d6c04828f085c33c72e9641c712d6a0f1a78126e3267a10699
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4492569 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f28d3ca7b6670d9a7ef545dae9da4b8dfb8cb06b7f35b0a1fb9db72eb9327038`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 12 Sep 2022 18:50:22 GMT
COPY file:2793f903eadf963d049d95e6645a7fc0e41632a84eff5d1055bd4de285218751 in /nats-server 
# Mon, 12 Sep 2022 18:50:23 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 12 Sep 2022 18:50:23 GMT
EXPOSE 4222 6222 8222
# Mon, 12 Sep 2022 18:50:24 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 12 Sep 2022 18:50:25 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 12 Sep 2022 18:50:26 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:29ad82f04593c429e1ee6bf6c0c2687549bee49e553052bf5b67eec17de00f9b`  
		Last Modified: Mon, 12 Sep 2022 18:51:40 GMT  
		Size: 4.5 MB (4492060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:138da13517dd9cec8dbf0a87e0ce1dc5c15dbde69247362fc9895c07830e7f72`  
		Last Modified: Mon, 12 Sep 2022 18:51:39 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.0-nanoserver`

```console
$ docker pull nats@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 0

## `nats:2.9.0-nanoserver-1809`

```console
$ docker pull nats@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 0

## `nats:2.9.0-scratch`

```console
$ docker pull nats@sha256:715227a167bc72698c322a7834aebbd465393b5019ec3f1e668378d43a60b32a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9.0-scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:118585c5efc972b7af723b603811e3146ee914a26b54bcb892c506e8080d2fac
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4665258 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dcd239e963a20ee15d599802357bd7485cbf652b2c7a5d9c77d6485c07168bce`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 12 Sep 2022 18:49:48 GMT
COPY file:37e0cdc4ef3cae050b7a622e477f07fea2b89f2849c5c229803b12157182aa73 in /nats-server 
# Mon, 12 Sep 2022 18:49:48 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 12 Sep 2022 18:49:48 GMT
EXPOSE 4222 6222 8222
# Mon, 12 Sep 2022 18:49:48 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 12 Sep 2022 18:49:49 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 12 Sep 2022 18:49:49 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:5a54d3866fde0d65a287b5e00b2251f84936c27eed638ecef0fa1e8f95134bd6`  
		Last Modified: Mon, 12 Sep 2022 18:51:17 GMT  
		Size: 4.7 MB (4664750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2846c8f5d71bd80327105a167594ce9f72272f7c6a141cf378e206141a075ab`  
		Last Modified: Mon, 12 Sep 2022 18:51:15 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.0-scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:a48ca64c022b50e4612f11b7b0bdf380e886ad449c8eb5a48624b2df386ceab4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4658073 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d43328d44a144020547148c52c8b0e257f2553339a66f15912b23f9b377d646d`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 12 Sep 2022 19:04:24 GMT
COPY file:88b07716d72d7b053cbf196c5562712b60f9d8875ee610f10839774e5aa8fd5e in /nats-server 
# Mon, 12 Sep 2022 19:04:24 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 12 Sep 2022 19:04:24 GMT
EXPOSE 4222 6222 8222
# Mon, 12 Sep 2022 19:04:24 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 12 Sep 2022 19:04:24 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 12 Sep 2022 19:04:25 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:fdc81c83bc1df58c4e224556b8224d1e7425add4047736a641d435c2097b7c10`  
		Last Modified: Mon, 12 Sep 2022 19:05:53 GMT  
		Size: 4.7 MB (4657565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:012d019d0dd61d6f41306e0a2009771e9b75625f46458973bd5db00d964d0d28`  
		Last Modified: Mon, 12 Sep 2022 19:05:52 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.0-scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:09ddfc36cc0a08d6c04828f085c33c72e9641c712d6a0f1a78126e3267a10699
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4492569 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f28d3ca7b6670d9a7ef545dae9da4b8dfb8cb06b7f35b0a1fb9db72eb9327038`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 12 Sep 2022 18:50:22 GMT
COPY file:2793f903eadf963d049d95e6645a7fc0e41632a84eff5d1055bd4de285218751 in /nats-server 
# Mon, 12 Sep 2022 18:50:23 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 12 Sep 2022 18:50:23 GMT
EXPOSE 4222 6222 8222
# Mon, 12 Sep 2022 18:50:24 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 12 Sep 2022 18:50:25 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 12 Sep 2022 18:50:26 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:29ad82f04593c429e1ee6bf6c0c2687549bee49e553052bf5b67eec17de00f9b`  
		Last Modified: Mon, 12 Sep 2022 18:51:40 GMT  
		Size: 4.5 MB (4492060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:138da13517dd9cec8dbf0a87e0ce1dc5c15dbde69247362fc9895c07830e7f72`  
		Last Modified: Mon, 12 Sep 2022 18:51:39 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.0-windowsservercore`

```console
$ docker pull nats@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 0

## `nats:2.9.0-windowsservercore-1809`

```console
$ docker pull nats@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 0

## `nats:alpine`

```console
$ docker pull nats@sha256:b11d821dbbfdfc45b8c6ef3c2b284247161c786c84968f6582478043adce5b07
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
$ docker pull nats@sha256:085e2d3603a5ffeb96a5e784f11532c03a4f0840b6d68974c49981ff00ae2403
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7567312 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9cc82d17b5c2168901fc2938dbcf28eb4107996ab8bc9eb7f577b8561f959058`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:22 GMT
ADD file:e8733e8cc0a81e15ca4041760b6e27392c34171512d34405a9b262b1fff5c687 in / 
# Tue, 09 Aug 2022 17:49:22 GMT
CMD ["/bin/sh"]
# Mon, 12 Sep 2022 18:49:32 GMT
ENV NATS_SERVER=2.9.0
# Mon, 12 Sep 2022 18:49:34 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='b82c2910819bbf9350a5040ba2145b5e17d0faf8fca502505a4845ce1dcba441' ;; 		armhf) natsArch='arm6'; sha256='4f5f02bd8e06e83d685f7cba76620ae76cdfb7bd94f89e3aea323bbd0bf6ab3b' ;; 		armv7) natsArch='arm7'; sha256='0af9e816fb4a47274d2f7b1d1ebebd13568f0b70d466feefdd04cf1f14a0195f' ;; 		x86_64) natsArch='amd64'; sha256='e2c678de6900dfd126ce181a1103201ac6fb4e63f7112d320932a011db64d4e0' ;; 		x86) natsArch='386'; sha256='a617f94da82e2518549d2192d336be1da09674498553d117a95e167c4f3425ca' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 12 Sep 2022 18:49:35 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 12 Sep 2022 18:49:35 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 12 Sep 2022 18:49:35 GMT
EXPOSE 4222 6222 8222
# Mon, 12 Sep 2022 18:49:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 12 Sep 2022 18:49:35 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9506b835437abb4d8ba1683e00c500b8f77e1975e930b356fbb72f2dbdc274d9`  
		Last Modified: Tue, 09 Aug 2022 17:50:33 GMT  
		Size: 2.6 MB (2613965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00fddff5163e8c58a7497154f421e89aff54a43caec19e95069cc494375041aa`  
		Last Modified: Mon, 12 Sep 2022 18:50:45 GMT  
		Size: 5.0 MB (4952345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8019ab673b790b4ed63a97187571f3d0e5f4eb16dfa17399f6a243d11ff5722b`  
		Last Modified: Mon, 12 Sep 2022 18:50:44 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5ceaa398303883b9d5e592ce9aeaccbcf4b34b99a27a67d1578a0d6de4e69d3`  
		Last Modified: Mon, 12 Sep 2022 18:50:44 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:b95fa7ad87668f84962e4ef5abed9890fb57640ad479112b7f8c119bfa45dfda
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.4 MB (7363700 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b06933b06c17a95c6cd21d33dc823a06314c6b8517ebbfaf5b76c3b3cf11b155`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 16:57:44 GMT
ADD file:75521fe16320b193092588f6f31052c85e736965ceb11673de18bd14965a45e6 in / 
# Tue, 09 Aug 2022 16:57:44 GMT
CMD ["/bin/sh"]
# Mon, 12 Sep 2022 19:03:51 GMT
ENV NATS_SERVER=2.9.0
# Mon, 12 Sep 2022 19:03:54 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='b82c2910819bbf9350a5040ba2145b5e17d0faf8fca502505a4845ce1dcba441' ;; 		armhf) natsArch='arm6'; sha256='4f5f02bd8e06e83d685f7cba76620ae76cdfb7bd94f89e3aea323bbd0bf6ab3b' ;; 		armv7) natsArch='arm7'; sha256='0af9e816fb4a47274d2f7b1d1ebebd13568f0b70d466feefdd04cf1f14a0195f' ;; 		x86_64) natsArch='amd64'; sha256='e2c678de6900dfd126ce181a1103201ac6fb4e63f7112d320932a011db64d4e0' ;; 		x86) natsArch='386'; sha256='a617f94da82e2518549d2192d336be1da09674498553d117a95e167c4f3425ca' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 12 Sep 2022 19:03:54 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 12 Sep 2022 19:03:54 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 12 Sep 2022 19:03:54 GMT
EXPOSE 4222 6222 8222
# Mon, 12 Sep 2022 19:03:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 12 Sep 2022 19:03:55 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:c6556b3b6858c6fa1e328377cc2c4becdc9cd1bc3e7302aa7299936522cf93ba`  
		Last Modified: Tue, 09 Aug 2022 16:58:55 GMT  
		Size: 2.4 MB (2417065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3571a588810a8fe42813cdd7bcdc3e7b0be7bfc9084e38508f050f9826bba19`  
		Last Modified: Mon, 12 Sep 2022 19:05:22 GMT  
		Size: 4.9 MB (4945636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b1bcd898e16c2896f273f1b98e85da9bae6f599fb25e92fcdb2cab7ba63d64d`  
		Last Modified: Mon, 12 Sep 2022 19:05:20 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21cdba5340addabedb9b0801b2c8d51c4b04c684965b7e4f9b25e8b44573fb78`  
		Last Modified: Mon, 12 Sep 2022 19:05:20 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:7869a7f7498ee46895e9948a102087841874c9ee049696fe96edc9c4c5f7b17c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.5 MB (7482302 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e7cded970df3ac075d6833bcc805ee1cd39b6de8728ce00785f95016a231117`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Mon, 12 Sep 2022 18:50:02 GMT
ENV NATS_SERVER=2.9.0
# Mon, 12 Sep 2022 18:50:04 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='b82c2910819bbf9350a5040ba2145b5e17d0faf8fca502505a4845ce1dcba441' ;; 		armhf) natsArch='arm6'; sha256='4f5f02bd8e06e83d685f7cba76620ae76cdfb7bd94f89e3aea323bbd0bf6ab3b' ;; 		armv7) natsArch='arm7'; sha256='0af9e816fb4a47274d2f7b1d1ebebd13568f0b70d466feefdd04cf1f14a0195f' ;; 		x86_64) natsArch='amd64'; sha256='e2c678de6900dfd126ce181a1103201ac6fb4e63f7112d320932a011db64d4e0' ;; 		x86) natsArch='386'; sha256='a617f94da82e2518549d2192d336be1da09674498553d117a95e167c4f3425ca' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 12 Sep 2022 18:50:06 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 12 Sep 2022 18:50:07 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 12 Sep 2022 18:50:07 GMT
EXPOSE 4222 6222 8222
# Mon, 12 Sep 2022 18:50:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 12 Sep 2022 18:50:09 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f13b8dbdcf7252f528110cd3097a32511e40b830a0e7690d5d3c7c544cbbace`  
		Last Modified: Mon, 12 Sep 2022 18:51:12 GMT  
		Size: 4.8 MB (4773665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27cb8435ac86def6a8973b25db155dbd8c3f0c407542046937eb1ab78b99276e`  
		Last Modified: Mon, 12 Sep 2022 18:51:11 GMT  
		Size: 561.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a47359896823731079e2553b7cf975eba66a0095c51b1ccffbe582b732a6d41b`  
		Last Modified: Mon, 12 Sep 2022 18:51:11 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:alpine3.16`

```console
$ docker pull nats@sha256:e5a371efe6187d5965b819b9152fbad9583f1750370a76961665837cfc97407f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:alpine3.16` - linux; arm variant v6

```console
$ docker pull nats@sha256:085e2d3603a5ffeb96a5e784f11532c03a4f0840b6d68974c49981ff00ae2403
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7567312 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9cc82d17b5c2168901fc2938dbcf28eb4107996ab8bc9eb7f577b8561f959058`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:22 GMT
ADD file:e8733e8cc0a81e15ca4041760b6e27392c34171512d34405a9b262b1fff5c687 in / 
# Tue, 09 Aug 2022 17:49:22 GMT
CMD ["/bin/sh"]
# Mon, 12 Sep 2022 18:49:32 GMT
ENV NATS_SERVER=2.9.0
# Mon, 12 Sep 2022 18:49:34 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='b82c2910819bbf9350a5040ba2145b5e17d0faf8fca502505a4845ce1dcba441' ;; 		armhf) natsArch='arm6'; sha256='4f5f02bd8e06e83d685f7cba76620ae76cdfb7bd94f89e3aea323bbd0bf6ab3b' ;; 		armv7) natsArch='arm7'; sha256='0af9e816fb4a47274d2f7b1d1ebebd13568f0b70d466feefdd04cf1f14a0195f' ;; 		x86_64) natsArch='amd64'; sha256='e2c678de6900dfd126ce181a1103201ac6fb4e63f7112d320932a011db64d4e0' ;; 		x86) natsArch='386'; sha256='a617f94da82e2518549d2192d336be1da09674498553d117a95e167c4f3425ca' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 12 Sep 2022 18:49:35 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 12 Sep 2022 18:49:35 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 12 Sep 2022 18:49:35 GMT
EXPOSE 4222 6222 8222
# Mon, 12 Sep 2022 18:49:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 12 Sep 2022 18:49:35 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9506b835437abb4d8ba1683e00c500b8f77e1975e930b356fbb72f2dbdc274d9`  
		Last Modified: Tue, 09 Aug 2022 17:50:33 GMT  
		Size: 2.6 MB (2613965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00fddff5163e8c58a7497154f421e89aff54a43caec19e95069cc494375041aa`  
		Last Modified: Mon, 12 Sep 2022 18:50:45 GMT  
		Size: 5.0 MB (4952345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8019ab673b790b4ed63a97187571f3d0e5f4eb16dfa17399f6a243d11ff5722b`  
		Last Modified: Mon, 12 Sep 2022 18:50:44 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5ceaa398303883b9d5e592ce9aeaccbcf4b34b99a27a67d1578a0d6de4e69d3`  
		Last Modified: Mon, 12 Sep 2022 18:50:44 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.16` - linux; arm variant v7

```console
$ docker pull nats@sha256:b95fa7ad87668f84962e4ef5abed9890fb57640ad479112b7f8c119bfa45dfda
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.4 MB (7363700 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b06933b06c17a95c6cd21d33dc823a06314c6b8517ebbfaf5b76c3b3cf11b155`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 16:57:44 GMT
ADD file:75521fe16320b193092588f6f31052c85e736965ceb11673de18bd14965a45e6 in / 
# Tue, 09 Aug 2022 16:57:44 GMT
CMD ["/bin/sh"]
# Mon, 12 Sep 2022 19:03:51 GMT
ENV NATS_SERVER=2.9.0
# Mon, 12 Sep 2022 19:03:54 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='b82c2910819bbf9350a5040ba2145b5e17d0faf8fca502505a4845ce1dcba441' ;; 		armhf) natsArch='arm6'; sha256='4f5f02bd8e06e83d685f7cba76620ae76cdfb7bd94f89e3aea323bbd0bf6ab3b' ;; 		armv7) natsArch='arm7'; sha256='0af9e816fb4a47274d2f7b1d1ebebd13568f0b70d466feefdd04cf1f14a0195f' ;; 		x86_64) natsArch='amd64'; sha256='e2c678de6900dfd126ce181a1103201ac6fb4e63f7112d320932a011db64d4e0' ;; 		x86) natsArch='386'; sha256='a617f94da82e2518549d2192d336be1da09674498553d117a95e167c4f3425ca' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 12 Sep 2022 19:03:54 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 12 Sep 2022 19:03:54 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 12 Sep 2022 19:03:54 GMT
EXPOSE 4222 6222 8222
# Mon, 12 Sep 2022 19:03:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 12 Sep 2022 19:03:55 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:c6556b3b6858c6fa1e328377cc2c4becdc9cd1bc3e7302aa7299936522cf93ba`  
		Last Modified: Tue, 09 Aug 2022 16:58:55 GMT  
		Size: 2.4 MB (2417065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3571a588810a8fe42813cdd7bcdc3e7b0be7bfc9084e38508f050f9826bba19`  
		Last Modified: Mon, 12 Sep 2022 19:05:22 GMT  
		Size: 4.9 MB (4945636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b1bcd898e16c2896f273f1b98e85da9bae6f599fb25e92fcdb2cab7ba63d64d`  
		Last Modified: Mon, 12 Sep 2022 19:05:20 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21cdba5340addabedb9b0801b2c8d51c4b04c684965b7e4f9b25e8b44573fb78`  
		Last Modified: Mon, 12 Sep 2022 19:05:20 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.16` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:7869a7f7498ee46895e9948a102087841874c9ee049696fe96edc9c4c5f7b17c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.5 MB (7482302 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e7cded970df3ac075d6833bcc805ee1cd39b6de8728ce00785f95016a231117`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Mon, 12 Sep 2022 18:50:02 GMT
ENV NATS_SERVER=2.9.0
# Mon, 12 Sep 2022 18:50:04 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='b82c2910819bbf9350a5040ba2145b5e17d0faf8fca502505a4845ce1dcba441' ;; 		armhf) natsArch='arm6'; sha256='4f5f02bd8e06e83d685f7cba76620ae76cdfb7bd94f89e3aea323bbd0bf6ab3b' ;; 		armv7) natsArch='arm7'; sha256='0af9e816fb4a47274d2f7b1d1ebebd13568f0b70d466feefdd04cf1f14a0195f' ;; 		x86_64) natsArch='amd64'; sha256='e2c678de6900dfd126ce181a1103201ac6fb4e63f7112d320932a011db64d4e0' ;; 		x86) natsArch='386'; sha256='a617f94da82e2518549d2192d336be1da09674498553d117a95e167c4f3425ca' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 12 Sep 2022 18:50:06 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 12 Sep 2022 18:50:07 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 12 Sep 2022 18:50:07 GMT
EXPOSE 4222 6222 8222
# Mon, 12 Sep 2022 18:50:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 12 Sep 2022 18:50:09 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f13b8dbdcf7252f528110cd3097a32511e40b830a0e7690d5d3c7c544cbbace`  
		Last Modified: Mon, 12 Sep 2022 18:51:12 GMT  
		Size: 4.8 MB (4773665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27cb8435ac86def6a8973b25db155dbd8c3f0c407542046937eb1ab78b99276e`  
		Last Modified: Mon, 12 Sep 2022 18:51:11 GMT  
		Size: 561.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a47359896823731079e2553b7cf975eba66a0095c51b1ccffbe582b732a6d41b`  
		Last Modified: Mon, 12 Sep 2022 18:51:11 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:latest`

```console
$ docker pull nats@sha256:0a52cec30c1dfc97dd7c6da084a8ca41cbb186c05091494c842e3eddaed6abba
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
$ docker pull nats@sha256:118585c5efc972b7af723b603811e3146ee914a26b54bcb892c506e8080d2fac
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4665258 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dcd239e963a20ee15d599802357bd7485cbf652b2c7a5d9c77d6485c07168bce`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 12 Sep 2022 18:49:48 GMT
COPY file:37e0cdc4ef3cae050b7a622e477f07fea2b89f2849c5c229803b12157182aa73 in /nats-server 
# Mon, 12 Sep 2022 18:49:48 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 12 Sep 2022 18:49:48 GMT
EXPOSE 4222 6222 8222
# Mon, 12 Sep 2022 18:49:48 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 12 Sep 2022 18:49:49 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 12 Sep 2022 18:49:49 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:5a54d3866fde0d65a287b5e00b2251f84936c27eed638ecef0fa1e8f95134bd6`  
		Last Modified: Mon, 12 Sep 2022 18:51:17 GMT  
		Size: 4.7 MB (4664750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2846c8f5d71bd80327105a167594ce9f72272f7c6a141cf378e206141a075ab`  
		Last Modified: Mon, 12 Sep 2022 18:51:15 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm variant v7

```console
$ docker pull nats@sha256:a48ca64c022b50e4612f11b7b0bdf380e886ad449c8eb5a48624b2df386ceab4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4658073 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d43328d44a144020547148c52c8b0e257f2553339a66f15912b23f9b377d646d`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 12 Sep 2022 19:04:24 GMT
COPY file:88b07716d72d7b053cbf196c5562712b60f9d8875ee610f10839774e5aa8fd5e in /nats-server 
# Mon, 12 Sep 2022 19:04:24 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 12 Sep 2022 19:04:24 GMT
EXPOSE 4222 6222 8222
# Mon, 12 Sep 2022 19:04:24 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 12 Sep 2022 19:04:24 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 12 Sep 2022 19:04:25 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:fdc81c83bc1df58c4e224556b8224d1e7425add4047736a641d435c2097b7c10`  
		Last Modified: Mon, 12 Sep 2022 19:05:53 GMT  
		Size: 4.7 MB (4657565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:012d019d0dd61d6f41306e0a2009771e9b75625f46458973bd5db00d964d0d28`  
		Last Modified: Mon, 12 Sep 2022 19:05:52 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:09ddfc36cc0a08d6c04828f085c33c72e9641c712d6a0f1a78126e3267a10699
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4492569 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f28d3ca7b6670d9a7ef545dae9da4b8dfb8cb06b7f35b0a1fb9db72eb9327038`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 12 Sep 2022 18:50:22 GMT
COPY file:2793f903eadf963d049d95e6645a7fc0e41632a84eff5d1055bd4de285218751 in /nats-server 
# Mon, 12 Sep 2022 18:50:23 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 12 Sep 2022 18:50:23 GMT
EXPOSE 4222 6222 8222
# Mon, 12 Sep 2022 18:50:24 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 12 Sep 2022 18:50:25 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 12 Sep 2022 18:50:26 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:29ad82f04593c429e1ee6bf6c0c2687549bee49e553052bf5b67eec17de00f9b`  
		Last Modified: Mon, 12 Sep 2022 18:51:40 GMT  
		Size: 4.5 MB (4492060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:138da13517dd9cec8dbf0a87e0ce1dc5c15dbde69247362fc9895c07830e7f72`  
		Last Modified: Mon, 12 Sep 2022 18:51:39 GMT  
		Size: 509.0 B  
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
$ docker pull nats@sha256:c337fb296c26591ce6b0cb0e926f3d5f9503d8d0018ec38f3c342dd7930839b5
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
$ docker pull nats@sha256:118585c5efc972b7af723b603811e3146ee914a26b54bcb892c506e8080d2fac
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4665258 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dcd239e963a20ee15d599802357bd7485cbf652b2c7a5d9c77d6485c07168bce`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 12 Sep 2022 18:49:48 GMT
COPY file:37e0cdc4ef3cae050b7a622e477f07fea2b89f2849c5c229803b12157182aa73 in /nats-server 
# Mon, 12 Sep 2022 18:49:48 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 12 Sep 2022 18:49:48 GMT
EXPOSE 4222 6222 8222
# Mon, 12 Sep 2022 18:49:48 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 12 Sep 2022 18:49:49 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 12 Sep 2022 18:49:49 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:5a54d3866fde0d65a287b5e00b2251f84936c27eed638ecef0fa1e8f95134bd6`  
		Last Modified: Mon, 12 Sep 2022 18:51:17 GMT  
		Size: 4.7 MB (4664750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2846c8f5d71bd80327105a167594ce9f72272f7c6a141cf378e206141a075ab`  
		Last Modified: Mon, 12 Sep 2022 18:51:15 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:a48ca64c022b50e4612f11b7b0bdf380e886ad449c8eb5a48624b2df386ceab4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4658073 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d43328d44a144020547148c52c8b0e257f2553339a66f15912b23f9b377d646d`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 12 Sep 2022 19:04:24 GMT
COPY file:88b07716d72d7b053cbf196c5562712b60f9d8875ee610f10839774e5aa8fd5e in /nats-server 
# Mon, 12 Sep 2022 19:04:24 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 12 Sep 2022 19:04:24 GMT
EXPOSE 4222 6222 8222
# Mon, 12 Sep 2022 19:04:24 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 12 Sep 2022 19:04:24 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 12 Sep 2022 19:04:25 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:fdc81c83bc1df58c4e224556b8224d1e7425add4047736a641d435c2097b7c10`  
		Last Modified: Mon, 12 Sep 2022 19:05:53 GMT  
		Size: 4.7 MB (4657565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:012d019d0dd61d6f41306e0a2009771e9b75625f46458973bd5db00d964d0d28`  
		Last Modified: Mon, 12 Sep 2022 19:05:52 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:09ddfc36cc0a08d6c04828f085c33c72e9641c712d6a0f1a78126e3267a10699
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4492569 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f28d3ca7b6670d9a7ef545dae9da4b8dfb8cb06b7f35b0a1fb9db72eb9327038`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 12 Sep 2022 18:50:22 GMT
COPY file:2793f903eadf963d049d95e6645a7fc0e41632a84eff5d1055bd4de285218751 in /nats-server 
# Mon, 12 Sep 2022 18:50:23 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 12 Sep 2022 18:50:23 GMT
EXPOSE 4222 6222 8222
# Mon, 12 Sep 2022 18:50:24 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 12 Sep 2022 18:50:25 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 12 Sep 2022 18:50:26 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:29ad82f04593c429e1ee6bf6c0c2687549bee49e553052bf5b67eec17de00f9b`  
		Last Modified: Mon, 12 Sep 2022 18:51:40 GMT  
		Size: 4.5 MB (4492060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:138da13517dd9cec8dbf0a87e0ce1dc5c15dbde69247362fc9895c07830e7f72`  
		Last Modified: Mon, 12 Sep 2022 18:51:39 GMT  
		Size: 509.0 B  
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
$ docker pull nats@sha256:c337fb296c26591ce6b0cb0e926f3d5f9503d8d0018ec38f3c342dd7930839b5
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
$ docker pull nats@sha256:118585c5efc972b7af723b603811e3146ee914a26b54bcb892c506e8080d2fac
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4665258 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dcd239e963a20ee15d599802357bd7485cbf652b2c7a5d9c77d6485c07168bce`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 12 Sep 2022 18:49:48 GMT
COPY file:37e0cdc4ef3cae050b7a622e477f07fea2b89f2849c5c229803b12157182aa73 in /nats-server 
# Mon, 12 Sep 2022 18:49:48 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 12 Sep 2022 18:49:48 GMT
EXPOSE 4222 6222 8222
# Mon, 12 Sep 2022 18:49:48 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 12 Sep 2022 18:49:49 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 12 Sep 2022 18:49:49 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:5a54d3866fde0d65a287b5e00b2251f84936c27eed638ecef0fa1e8f95134bd6`  
		Last Modified: Mon, 12 Sep 2022 18:51:17 GMT  
		Size: 4.7 MB (4664750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2846c8f5d71bd80327105a167594ce9f72272f7c6a141cf378e206141a075ab`  
		Last Modified: Mon, 12 Sep 2022 18:51:15 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:a48ca64c022b50e4612f11b7b0bdf380e886ad449c8eb5a48624b2df386ceab4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4658073 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d43328d44a144020547148c52c8b0e257f2553339a66f15912b23f9b377d646d`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 12 Sep 2022 19:04:24 GMT
COPY file:88b07716d72d7b053cbf196c5562712b60f9d8875ee610f10839774e5aa8fd5e in /nats-server 
# Mon, 12 Sep 2022 19:04:24 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 12 Sep 2022 19:04:24 GMT
EXPOSE 4222 6222 8222
# Mon, 12 Sep 2022 19:04:24 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 12 Sep 2022 19:04:24 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 12 Sep 2022 19:04:25 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:fdc81c83bc1df58c4e224556b8224d1e7425add4047736a641d435c2097b7c10`  
		Last Modified: Mon, 12 Sep 2022 19:05:53 GMT  
		Size: 4.7 MB (4657565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:012d019d0dd61d6f41306e0a2009771e9b75625f46458973bd5db00d964d0d28`  
		Last Modified: Mon, 12 Sep 2022 19:05:52 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:09ddfc36cc0a08d6c04828f085c33c72e9641c712d6a0f1a78126e3267a10699
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4492569 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f28d3ca7b6670d9a7ef545dae9da4b8dfb8cb06b7f35b0a1fb9db72eb9327038`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 12 Sep 2022 18:50:22 GMT
COPY file:2793f903eadf963d049d95e6645a7fc0e41632a84eff5d1055bd4de285218751 in /nats-server 
# Mon, 12 Sep 2022 18:50:23 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 12 Sep 2022 18:50:23 GMT
EXPOSE 4222 6222 8222
# Mon, 12 Sep 2022 18:50:24 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 12 Sep 2022 18:50:25 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 12 Sep 2022 18:50:26 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:29ad82f04593c429e1ee6bf6c0c2687549bee49e553052bf5b67eec17de00f9b`  
		Last Modified: Mon, 12 Sep 2022 18:51:40 GMT  
		Size: 4.5 MB (4492060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:138da13517dd9cec8dbf0a87e0ce1dc5c15dbde69247362fc9895c07830e7f72`  
		Last Modified: Mon, 12 Sep 2022 18:51:39 GMT  
		Size: 509.0 B  
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
