<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `nats-streaming`

-	[`nats-streaming:0.25`](#nats-streaming025)
-	[`nats-streaming:0.25-alpine`](#nats-streaming025-alpine)
-	[`nats-streaming:0.25-alpine3.18`](#nats-streaming025-alpine318)
-	[`nats-streaming:0.25-linux`](#nats-streaming025-linux)
-	[`nats-streaming:0.25-nanoserver`](#nats-streaming025-nanoserver)
-	[`nats-streaming:0.25-nanoserver-1809`](#nats-streaming025-nanoserver-1809)
-	[`nats-streaming:0.25-scratch`](#nats-streaming025-scratch)
-	[`nats-streaming:0.25-windowsservercore`](#nats-streaming025-windowsservercore)
-	[`nats-streaming:0.25-windowsservercore-1809`](#nats-streaming025-windowsservercore-1809)
-	[`nats-streaming:0.25.5`](#nats-streaming0255)
-	[`nats-streaming:0.25.5-alpine`](#nats-streaming0255-alpine)
-	[`nats-streaming:0.25.5-alpine3.18`](#nats-streaming0255-alpine318)
-	[`nats-streaming:0.25.5-linux`](#nats-streaming0255-linux)
-	[`nats-streaming:0.25.5-nanoserver`](#nats-streaming0255-nanoserver)
-	[`nats-streaming:0.25.5-nanoserver-1809`](#nats-streaming0255-nanoserver-1809)
-	[`nats-streaming:0.25.5-scratch`](#nats-streaming0255-scratch)
-	[`nats-streaming:0.25.5-windowsservercore`](#nats-streaming0255-windowsservercore)
-	[`nats-streaming:0.25.5-windowsservercore-1809`](#nats-streaming0255-windowsservercore-1809)
-	[`nats-streaming:alpine`](#nats-streamingalpine)
-	[`nats-streaming:alpine3.18`](#nats-streamingalpine318)
-	[`nats-streaming:latest`](#nats-streaminglatest)
-	[`nats-streaming:linux`](#nats-streaminglinux)
-	[`nats-streaming:nanoserver`](#nats-streamingnanoserver)
-	[`nats-streaming:nanoserver-1809`](#nats-streamingnanoserver-1809)
-	[`nats-streaming:scratch`](#nats-streamingscratch)
-	[`nats-streaming:windowsservercore`](#nats-streamingwindowsservercore)
-	[`nats-streaming:windowsservercore-1809`](#nats-streamingwindowsservercore-1809)

## `nats-streaming:0.25`

```console
$ docker pull nats-streaming@sha256:1eed8c2ef0f8b6e0c7264013e3f64f7f2a75195827fce558fde4d277bfcb4b7a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.4645; amd64

### `nats-streaming:0.25` - linux; amd64

```console
$ docker pull nats-streaming@sha256:0963a4d0a1504acf8b8f5b99fa1f119639a1caff31850eefe83a685fac6820fb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.7 MB (7659749 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:32ad867a381275ce803cc7a4e3007d375908b15c83a75444af3352cfdc72d2eb`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Wed, 21 Jun 2023 01:10:50 GMT
COPY file:670c17c233c7999d9f7b72c2962b221cab4e00da471a75e8679840c939143cfb in /nats-streaming-server 
# Wed, 21 Jun 2023 01:10:50 GMT
EXPOSE 4222 8222
# Wed, 21 Jun 2023 01:10:51 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Wed, 21 Jun 2023 01:10:51 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:b7ff958d406306840566ff165f0c34c6017d44a13d4355d5eb8c6cd152c57d64`  
		Last Modified: Wed, 21 Jun 2023 01:11:25 GMT  
		Size: 7.7 MB (7659749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.25` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:c6adf4bdcf4ca4548a1331f9a5b78accb38369508960b70058ae6f3cfe00ed5d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7311545 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7763bb2699d3b947f45691cca3c382801ad1c0a91b829831fd0999aa54245f66`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Wed, 21 Jun 2023 00:59:07 GMT
COPY file:9bc2f7015ff72f7e91556a01075e89ef8a85a404228874028f7a356e8142e169 in /nats-streaming-server 
# Wed, 21 Jun 2023 00:59:07 GMT
EXPOSE 4222 8222
# Wed, 21 Jun 2023 00:59:07 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Wed, 21 Jun 2023 00:59:08 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:ee4a78724efc3390679e6118a2f2c5993c9075f378bd6a2f0b7f99b50579fb2b`  
		Last Modified: Wed, 21 Jun 2023 00:59:42 GMT  
		Size: 7.3 MB (7311545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.25` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:3ae971fd2fa4bc0a898567aa6a6ea4d4dbae8d4459d81e59a2fab244b4d9c5b0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7304325 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:825e70124556ec89714458bdec5da1ee59baa724df73fa420db3005bfad56c45`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Wed, 21 Jun 2023 01:31:21 GMT
COPY file:07846c068b31699c9c9fe9b535ec7c1dcfbda7a16d7d178a50de1f9541deeebf in /nats-streaming-server 
# Wed, 21 Jun 2023 01:31:21 GMT
EXPOSE 4222 8222
# Wed, 21 Jun 2023 01:31:21 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Wed, 21 Jun 2023 01:31:21 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:039446f9a794527f7060ddd5b9b8a071ffe8816fa5aae791c4bbf01db3656057`  
		Last Modified: Wed, 21 Jun 2023 01:31:55 GMT  
		Size: 7.3 MB (7304325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.25` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:04ef4025a7de920cc90464848b402755e5da72e57bc969aff8859af5429c00a7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.0 MB (7011458 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1627cfd9fc66597d5484a918e734f0595b380583577fd3a532f6228b72db740a`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Wed, 21 Jun 2023 01:11:52 GMT
COPY file:8237d0d59fd3c6b32e52dbff50861a8848f846505c0303e7975e4a5f48ce8de9 in /nats-streaming-server 
# Wed, 21 Jun 2023 01:11:52 GMT
EXPOSE 4222 8222
# Wed, 21 Jun 2023 01:11:52 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Wed, 21 Jun 2023 01:11:52 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:c3b4c14668a8e32e87c6ea3dce4a99716b527ba7f0f4608cbab27184c89832ee`  
		Last Modified: Wed, 21 Jun 2023 01:12:24 GMT  
		Size: 7.0 MB (7011458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.25` - windows version 10.0.17763.4645; amd64

```console
$ docker pull nats-streaming@sha256:5c39267b2e159ad82e792287b1086208f57dbf20ef18e40b553f3b377b337545
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.2 MB (112198939 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ef72ff049bb8cd1e4d7c65b5e46d477eccc664570d1a61e14b52bfc1faaa98f`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Fri, 07 Jul 2023 07:42:59 GMT
RUN Apply image 10.0.17763.4645
# Fri, 14 Jul 2023 00:03:16 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 14 Jul 2023 00:07:54 GMT
RUN cmd /S /C #(nop) COPY file:0e2c8ba21e47adc90962b46928c928315462bcddaefcbc01f98113f4f66cda4a in C:\nats-streaming-server.exe 
# Fri, 14 Jul 2023 00:07:55 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Fri, 14 Jul 2023 00:07:56 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Fri, 14 Jul 2023 00:07:57 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:5c5b06ba65934bcf850a1a54ecf4b3da34d3e6d6c8e90dbc897719c3ea377c8a`  
		Last Modified: Tue, 11 Jul 2023 17:31:37 GMT  
		Size: 104.4 MB (104408241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff4bad9bf846d07362d8295a4479f8f2965dfb5934a9a032b335ce3cb086bdf7`  
		Last Modified: Fri, 14 Jul 2023 00:04:06 GMT  
		Size: 1.2 KB (1161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f94b9b520f177b081bf712ba074ba66cad6139b8164f8e18de5be8ebd3ae7382`  
		Last Modified: Fri, 14 Jul 2023 00:08:34 GMT  
		Size: 7.8 MB (7786370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c03838a3679d351be263b09d3a5c6b9c44c73bd67df1a32d00364b15614d8b4c`  
		Last Modified: Fri, 14 Jul 2023 00:08:32 GMT  
		Size: 1.1 KB (1058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3a7169624bc074e90056b7387038bd434dc1bc770b6ac612f0d295d8db6b10f`  
		Last Modified: Fri, 14 Jul 2023 00:08:31 GMT  
		Size: 1.0 KB (1035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30ef31773aef63c527f320ae07bc5b102bd9f4f448f3b8d21c3e339e30db10e1`  
		Last Modified: Fri, 14 Jul 2023 00:08:32 GMT  
		Size: 1.1 KB (1074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.25-alpine`

```console
$ docker pull nats-streaming@sha256:c9e97ca2eb081301837053ea04e6a1dfc4fedacacf21a10b540693546de6c733
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.25-alpine` - linux; amd64

```console
$ docker pull nats-streaming@sha256:6abf524d6062038a5c5c66c0733592ac2d3151abbd8b423facb5f4f575fbabda
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.3 MB (11344002 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:259306c401d301ff49ceac471b001513aeb8ec5ce27d8e92b4a6c0c4a7be30f3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 14 Jun 2023 20:41:58 GMT
ADD file:1da756d12551a0e3e793e02ef87432d69d4968937bd11bed0af215db19dd94cd in / 
# Wed, 14 Jun 2023 20:41:59 GMT
CMD ["/bin/sh"]
# Wed, 21 Jun 2023 01:10:41 GMT
ENV NATS_STREAMING_SERVER=0.25.5
# Wed, 21 Jun 2023 01:10:43 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='937af3f9cdbfe3cb4648cf8c8f505dded2cc175d59ba10e13ec71d1c04e61bf2' ;; 		armhf) natsArch='arm6'; sha256='5bd3a0456054505741b05e5d03acb9f7a5de97cf3ea20cd52d31edbae1c387ea' ;; 		armv7) natsArch='arm7'; sha256='0e643e9881cf3acf3313f84853451d1c4a1e731bc8599d223a40042f9c0c7285' ;; 		x86_64) natsArch='amd64'; sha256='22762f4d0ccfc75947096a14e09566b816113e125a3d39f7914a0c332bee25a7' ;; 		x86) natsArch='386'; sha256='92d8d4460f538883c78e67a334b23b2317e4fe58d46e4fdbbef8b4c09c7b97ae' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Wed, 21 Jun 2023 01:10:43 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Wed, 21 Jun 2023 01:10:44 GMT
EXPOSE 4222 8222
# Wed, 21 Jun 2023 01:10:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Jun 2023 01:10:44 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:31e352740f534f9ad170f75378a84fe453d6156e40700b882d737a8f4a6988a3`  
		Last Modified: Wed, 14 Jun 2023 20:42:26 GMT  
		Size: 3.4 MB (3397879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0ccb9db0d77fa25becf9aa3c73f0a091378e47d9a8c0d87114fe3ca75b17483`  
		Last Modified: Wed, 21 Jun 2023 01:11:09 GMT  
		Size: 7.9 MB (7945701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56d62dc9de67132e108b1f8b40907849093f018255907030abdb3fc7b94904a9`  
		Last Modified: Wed, 21 Jun 2023 01:11:07 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.25-alpine` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:df08adb5a35cd347a0f1d96e733b0ba3b963a100fe08534f0e3a7a739f7453d2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.7 MB (10745511 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e879e367a39ad7817ae00eaf4a01036cc223cf63db3d0b10455e54a4fcf76bc3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Mon, 07 Aug 2023 19:49:14 GMT
ADD file:9882e99e5f94ab2db05c029648ac5be7cf0f063a8701394fcbb543a7ef5d4b90 in / 
# Mon, 07 Aug 2023 19:49:15 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 20:44:50 GMT
ENV NATS_STREAMING_SERVER=0.25.5
# Tue, 08 Aug 2023 20:44:52 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='937af3f9cdbfe3cb4648cf8c8f505dded2cc175d59ba10e13ec71d1c04e61bf2' ;; 		armhf) natsArch='arm6'; sha256='5bd3a0456054505741b05e5d03acb9f7a5de97cf3ea20cd52d31edbae1c387ea' ;; 		armv7) natsArch='arm7'; sha256='0e643e9881cf3acf3313f84853451d1c4a1e731bc8599d223a40042f9c0c7285' ;; 		x86_64) natsArch='amd64'; sha256='22762f4d0ccfc75947096a14e09566b816113e125a3d39f7914a0c332bee25a7' ;; 		x86) natsArch='386'; sha256='92d8d4460f538883c78e67a334b23b2317e4fe58d46e4fdbbef8b4c09c7b97ae' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Tue, 08 Aug 2023 20:44:53 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Tue, 08 Aug 2023 20:44:53 GMT
EXPOSE 4222 8222
# Tue, 08 Aug 2023 20:44:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 08 Aug 2023 20:44:53 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:af09961d4a43b504efc76e38b50918977c28be73eeb8b926247783a00e8b9f2f`  
		Last Modified: Mon, 07 Aug 2023 19:49:38 GMT  
		Size: 3.1 MB (3144809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db57a023cb1e641cc4e410d847ed348704fa48f194e6e04feb97859ea8263399`  
		Last Modified: Tue, 08 Aug 2023 20:45:13 GMT  
		Size: 7.6 MB (7600282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d00d13e6c7ccee53d63384bf85378713efa9cd84cb8817b81ddcb19ab83106e3`  
		Last Modified: Tue, 08 Aug 2023 20:45:11 GMT  
		Size: 420.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.25-alpine` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:8b69faa2f13f8bb2769c9ca014cfb884a6f581175bf1ad9baaa59b914ef3a7fe
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.5 MB (10488008 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6b906477dbd127990b39bdff954cd4495c0027ae495dad6ab5c740cff11c8a4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Mon, 07 Aug 2023 19:57:25 GMT
ADD file:e3f56488d3d3bb67729714db13ddadf6652e7efb5281cfc7010d3e71f9d6607f in / 
# Mon, 07 Aug 2023 19:57:25 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 02:15:20 GMT
ENV NATS_STREAMING_SERVER=0.25.5
# Tue, 08 Aug 2023 02:15:23 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='937af3f9cdbfe3cb4648cf8c8f505dded2cc175d59ba10e13ec71d1c04e61bf2' ;; 		armhf) natsArch='arm6'; sha256='5bd3a0456054505741b05e5d03acb9f7a5de97cf3ea20cd52d31edbae1c387ea' ;; 		armv7) natsArch='arm7'; sha256='0e643e9881cf3acf3313f84853451d1c4a1e731bc8599d223a40042f9c0c7285' ;; 		x86_64) natsArch='amd64'; sha256='22762f4d0ccfc75947096a14e09566b816113e125a3d39f7914a0c332bee25a7' ;; 		x86) natsArch='386'; sha256='92d8d4460f538883c78e67a334b23b2317e4fe58d46e4fdbbef8b4c09c7b97ae' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Tue, 08 Aug 2023 02:15:23 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Tue, 08 Aug 2023 02:15:23 GMT
EXPOSE 4222 8222
# Tue, 08 Aug 2023 02:15:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 08 Aug 2023 02:15:24 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:f8dec92eec42224ef9e6ca9c6207ea6b9195dcf93d06bd5ceff0f814b62bf064`  
		Last Modified: Mon, 07 Aug 2023 19:57:55 GMT  
		Size: 2.9 MB (2899480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e18324f789c9a02a3fb3992cee161f01f2d80d6396a0eb54b83956b93f18e24b`  
		Last Modified: Tue, 08 Aug 2023 02:15:50 GMT  
		Size: 7.6 MB (7588109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bff0b4480470ca012849b4227c612a9a456bed7a67117efc5fb5c5a737d17e9`  
		Last Modified: Tue, 08 Aug 2023 02:15:48 GMT  
		Size: 419.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.25-alpine` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:9f7fa008b1524911fee4a485f955408c7b911611179fdf120a2bb89f3323cdfa
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.6 MB (10629737 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5be4dd1beeb3895e9906e2866ca807b53f3b5cbc33598ed378b76126ded32d8d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 14 Jun 2023 20:48:58 GMT
ADD file:289c2fac17119508ced527225d445747cd177111b4a0018a6b04948ecb3b5e29 in / 
# Wed, 14 Jun 2023 20:48:58 GMT
CMD ["/bin/sh"]
# Wed, 21 Jun 2023 01:11:44 GMT
ENV NATS_STREAMING_SERVER=0.25.5
# Wed, 21 Jun 2023 01:11:46 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='937af3f9cdbfe3cb4648cf8c8f505dded2cc175d59ba10e13ec71d1c04e61bf2' ;; 		armhf) natsArch='arm6'; sha256='5bd3a0456054505741b05e5d03acb9f7a5de97cf3ea20cd52d31edbae1c387ea' ;; 		armv7) natsArch='arm7'; sha256='0e643e9881cf3acf3313f84853451d1c4a1e731bc8599d223a40042f9c0c7285' ;; 		x86_64) natsArch='amd64'; sha256='22762f4d0ccfc75947096a14e09566b816113e125a3d39f7914a0c332bee25a7' ;; 		x86) natsArch='386'; sha256='92d8d4460f538883c78e67a334b23b2317e4fe58d46e4fdbbef8b4c09c7b97ae' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Wed, 21 Jun 2023 01:11:46 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Wed, 21 Jun 2023 01:11:46 GMT
EXPOSE 4222 8222
# Wed, 21 Jun 2023 01:11:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Jun 2023 01:11:46 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:8c6d1654570f041603f4cef49c320c8f6f3e401324913009d92a19132cbf1ac0`  
		Last Modified: Wed, 14 Jun 2023 20:49:23 GMT  
		Size: 3.3 MB (3329251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3146f74e4cb95e61d4f251594c3330ad0f9c85345a1b97bce44ab0446ee59269`  
		Last Modified: Wed, 21 Jun 2023 01:12:08 GMT  
		Size: 7.3 MB (7300064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:775fc9bc0a0519e7fe2cd9656617079a95fd7919b285649d10cf4f76b7e89b49`  
		Last Modified: Wed, 21 Jun 2023 01:12:07 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.25-alpine3.18`

```console
$ docker pull nats-streaming@sha256:c9e97ca2eb081301837053ea04e6a1dfc4fedacacf21a10b540693546de6c733
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.25-alpine3.18` - linux; amd64

```console
$ docker pull nats-streaming@sha256:6abf524d6062038a5c5c66c0733592ac2d3151abbd8b423facb5f4f575fbabda
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.3 MB (11344002 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:259306c401d301ff49ceac471b001513aeb8ec5ce27d8e92b4a6c0c4a7be30f3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 14 Jun 2023 20:41:58 GMT
ADD file:1da756d12551a0e3e793e02ef87432d69d4968937bd11bed0af215db19dd94cd in / 
# Wed, 14 Jun 2023 20:41:59 GMT
CMD ["/bin/sh"]
# Wed, 21 Jun 2023 01:10:41 GMT
ENV NATS_STREAMING_SERVER=0.25.5
# Wed, 21 Jun 2023 01:10:43 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='937af3f9cdbfe3cb4648cf8c8f505dded2cc175d59ba10e13ec71d1c04e61bf2' ;; 		armhf) natsArch='arm6'; sha256='5bd3a0456054505741b05e5d03acb9f7a5de97cf3ea20cd52d31edbae1c387ea' ;; 		armv7) natsArch='arm7'; sha256='0e643e9881cf3acf3313f84853451d1c4a1e731bc8599d223a40042f9c0c7285' ;; 		x86_64) natsArch='amd64'; sha256='22762f4d0ccfc75947096a14e09566b816113e125a3d39f7914a0c332bee25a7' ;; 		x86) natsArch='386'; sha256='92d8d4460f538883c78e67a334b23b2317e4fe58d46e4fdbbef8b4c09c7b97ae' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Wed, 21 Jun 2023 01:10:43 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Wed, 21 Jun 2023 01:10:44 GMT
EXPOSE 4222 8222
# Wed, 21 Jun 2023 01:10:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Jun 2023 01:10:44 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:31e352740f534f9ad170f75378a84fe453d6156e40700b882d737a8f4a6988a3`  
		Last Modified: Wed, 14 Jun 2023 20:42:26 GMT  
		Size: 3.4 MB (3397879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0ccb9db0d77fa25becf9aa3c73f0a091378e47d9a8c0d87114fe3ca75b17483`  
		Last Modified: Wed, 21 Jun 2023 01:11:09 GMT  
		Size: 7.9 MB (7945701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56d62dc9de67132e108b1f8b40907849093f018255907030abdb3fc7b94904a9`  
		Last Modified: Wed, 21 Jun 2023 01:11:07 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.25-alpine3.18` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:df08adb5a35cd347a0f1d96e733b0ba3b963a100fe08534f0e3a7a739f7453d2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.7 MB (10745511 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e879e367a39ad7817ae00eaf4a01036cc223cf63db3d0b10455e54a4fcf76bc3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Mon, 07 Aug 2023 19:49:14 GMT
ADD file:9882e99e5f94ab2db05c029648ac5be7cf0f063a8701394fcbb543a7ef5d4b90 in / 
# Mon, 07 Aug 2023 19:49:15 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 20:44:50 GMT
ENV NATS_STREAMING_SERVER=0.25.5
# Tue, 08 Aug 2023 20:44:52 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='937af3f9cdbfe3cb4648cf8c8f505dded2cc175d59ba10e13ec71d1c04e61bf2' ;; 		armhf) natsArch='arm6'; sha256='5bd3a0456054505741b05e5d03acb9f7a5de97cf3ea20cd52d31edbae1c387ea' ;; 		armv7) natsArch='arm7'; sha256='0e643e9881cf3acf3313f84853451d1c4a1e731bc8599d223a40042f9c0c7285' ;; 		x86_64) natsArch='amd64'; sha256='22762f4d0ccfc75947096a14e09566b816113e125a3d39f7914a0c332bee25a7' ;; 		x86) natsArch='386'; sha256='92d8d4460f538883c78e67a334b23b2317e4fe58d46e4fdbbef8b4c09c7b97ae' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Tue, 08 Aug 2023 20:44:53 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Tue, 08 Aug 2023 20:44:53 GMT
EXPOSE 4222 8222
# Tue, 08 Aug 2023 20:44:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 08 Aug 2023 20:44:53 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:af09961d4a43b504efc76e38b50918977c28be73eeb8b926247783a00e8b9f2f`  
		Last Modified: Mon, 07 Aug 2023 19:49:38 GMT  
		Size: 3.1 MB (3144809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db57a023cb1e641cc4e410d847ed348704fa48f194e6e04feb97859ea8263399`  
		Last Modified: Tue, 08 Aug 2023 20:45:13 GMT  
		Size: 7.6 MB (7600282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d00d13e6c7ccee53d63384bf85378713efa9cd84cb8817b81ddcb19ab83106e3`  
		Last Modified: Tue, 08 Aug 2023 20:45:11 GMT  
		Size: 420.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.25-alpine3.18` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:8b69faa2f13f8bb2769c9ca014cfb884a6f581175bf1ad9baaa59b914ef3a7fe
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.5 MB (10488008 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6b906477dbd127990b39bdff954cd4495c0027ae495dad6ab5c740cff11c8a4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Mon, 07 Aug 2023 19:57:25 GMT
ADD file:e3f56488d3d3bb67729714db13ddadf6652e7efb5281cfc7010d3e71f9d6607f in / 
# Mon, 07 Aug 2023 19:57:25 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 02:15:20 GMT
ENV NATS_STREAMING_SERVER=0.25.5
# Tue, 08 Aug 2023 02:15:23 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='937af3f9cdbfe3cb4648cf8c8f505dded2cc175d59ba10e13ec71d1c04e61bf2' ;; 		armhf) natsArch='arm6'; sha256='5bd3a0456054505741b05e5d03acb9f7a5de97cf3ea20cd52d31edbae1c387ea' ;; 		armv7) natsArch='arm7'; sha256='0e643e9881cf3acf3313f84853451d1c4a1e731bc8599d223a40042f9c0c7285' ;; 		x86_64) natsArch='amd64'; sha256='22762f4d0ccfc75947096a14e09566b816113e125a3d39f7914a0c332bee25a7' ;; 		x86) natsArch='386'; sha256='92d8d4460f538883c78e67a334b23b2317e4fe58d46e4fdbbef8b4c09c7b97ae' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Tue, 08 Aug 2023 02:15:23 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Tue, 08 Aug 2023 02:15:23 GMT
EXPOSE 4222 8222
# Tue, 08 Aug 2023 02:15:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 08 Aug 2023 02:15:24 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:f8dec92eec42224ef9e6ca9c6207ea6b9195dcf93d06bd5ceff0f814b62bf064`  
		Last Modified: Mon, 07 Aug 2023 19:57:55 GMT  
		Size: 2.9 MB (2899480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e18324f789c9a02a3fb3992cee161f01f2d80d6396a0eb54b83956b93f18e24b`  
		Last Modified: Tue, 08 Aug 2023 02:15:50 GMT  
		Size: 7.6 MB (7588109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bff0b4480470ca012849b4227c612a9a456bed7a67117efc5fb5c5a737d17e9`  
		Last Modified: Tue, 08 Aug 2023 02:15:48 GMT  
		Size: 419.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.25-alpine3.18` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:9f7fa008b1524911fee4a485f955408c7b911611179fdf120a2bb89f3323cdfa
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.6 MB (10629737 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5be4dd1beeb3895e9906e2866ca807b53f3b5cbc33598ed378b76126ded32d8d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 14 Jun 2023 20:48:58 GMT
ADD file:289c2fac17119508ced527225d445747cd177111b4a0018a6b04948ecb3b5e29 in / 
# Wed, 14 Jun 2023 20:48:58 GMT
CMD ["/bin/sh"]
# Wed, 21 Jun 2023 01:11:44 GMT
ENV NATS_STREAMING_SERVER=0.25.5
# Wed, 21 Jun 2023 01:11:46 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='937af3f9cdbfe3cb4648cf8c8f505dded2cc175d59ba10e13ec71d1c04e61bf2' ;; 		armhf) natsArch='arm6'; sha256='5bd3a0456054505741b05e5d03acb9f7a5de97cf3ea20cd52d31edbae1c387ea' ;; 		armv7) natsArch='arm7'; sha256='0e643e9881cf3acf3313f84853451d1c4a1e731bc8599d223a40042f9c0c7285' ;; 		x86_64) natsArch='amd64'; sha256='22762f4d0ccfc75947096a14e09566b816113e125a3d39f7914a0c332bee25a7' ;; 		x86) natsArch='386'; sha256='92d8d4460f538883c78e67a334b23b2317e4fe58d46e4fdbbef8b4c09c7b97ae' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Wed, 21 Jun 2023 01:11:46 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Wed, 21 Jun 2023 01:11:46 GMT
EXPOSE 4222 8222
# Wed, 21 Jun 2023 01:11:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Jun 2023 01:11:46 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:8c6d1654570f041603f4cef49c320c8f6f3e401324913009d92a19132cbf1ac0`  
		Last Modified: Wed, 14 Jun 2023 20:49:23 GMT  
		Size: 3.3 MB (3329251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3146f74e4cb95e61d4f251594c3330ad0f9c85345a1b97bce44ab0446ee59269`  
		Last Modified: Wed, 21 Jun 2023 01:12:08 GMT  
		Size: 7.3 MB (7300064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:775fc9bc0a0519e7fe2cd9656617079a95fd7919b285649d10cf4f76b7e89b49`  
		Last Modified: Wed, 21 Jun 2023 01:12:07 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.25-linux`

```console
$ docker pull nats-streaming@sha256:2b8205e7d3a87aacdc19ec7b71e3316a44380ef15ab834060826911876394dac
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.25-linux` - linux; amd64

```console
$ docker pull nats-streaming@sha256:0963a4d0a1504acf8b8f5b99fa1f119639a1caff31850eefe83a685fac6820fb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.7 MB (7659749 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:32ad867a381275ce803cc7a4e3007d375908b15c83a75444af3352cfdc72d2eb`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Wed, 21 Jun 2023 01:10:50 GMT
COPY file:670c17c233c7999d9f7b72c2962b221cab4e00da471a75e8679840c939143cfb in /nats-streaming-server 
# Wed, 21 Jun 2023 01:10:50 GMT
EXPOSE 4222 8222
# Wed, 21 Jun 2023 01:10:51 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Wed, 21 Jun 2023 01:10:51 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:b7ff958d406306840566ff165f0c34c6017d44a13d4355d5eb8c6cd152c57d64`  
		Last Modified: Wed, 21 Jun 2023 01:11:25 GMT  
		Size: 7.7 MB (7659749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.25-linux` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:c6adf4bdcf4ca4548a1331f9a5b78accb38369508960b70058ae6f3cfe00ed5d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7311545 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7763bb2699d3b947f45691cca3c382801ad1c0a91b829831fd0999aa54245f66`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Wed, 21 Jun 2023 00:59:07 GMT
COPY file:9bc2f7015ff72f7e91556a01075e89ef8a85a404228874028f7a356e8142e169 in /nats-streaming-server 
# Wed, 21 Jun 2023 00:59:07 GMT
EXPOSE 4222 8222
# Wed, 21 Jun 2023 00:59:07 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Wed, 21 Jun 2023 00:59:08 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:ee4a78724efc3390679e6118a2f2c5993c9075f378bd6a2f0b7f99b50579fb2b`  
		Last Modified: Wed, 21 Jun 2023 00:59:42 GMT  
		Size: 7.3 MB (7311545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.25-linux` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:3ae971fd2fa4bc0a898567aa6a6ea4d4dbae8d4459d81e59a2fab244b4d9c5b0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7304325 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:825e70124556ec89714458bdec5da1ee59baa724df73fa420db3005bfad56c45`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Wed, 21 Jun 2023 01:31:21 GMT
COPY file:07846c068b31699c9c9fe9b535ec7c1dcfbda7a16d7d178a50de1f9541deeebf in /nats-streaming-server 
# Wed, 21 Jun 2023 01:31:21 GMT
EXPOSE 4222 8222
# Wed, 21 Jun 2023 01:31:21 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Wed, 21 Jun 2023 01:31:21 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:039446f9a794527f7060ddd5b9b8a071ffe8816fa5aae791c4bbf01db3656057`  
		Last Modified: Wed, 21 Jun 2023 01:31:55 GMT  
		Size: 7.3 MB (7304325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.25-linux` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:04ef4025a7de920cc90464848b402755e5da72e57bc969aff8859af5429c00a7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.0 MB (7011458 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1627cfd9fc66597d5484a918e734f0595b380583577fd3a532f6228b72db740a`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Wed, 21 Jun 2023 01:11:52 GMT
COPY file:8237d0d59fd3c6b32e52dbff50861a8848f846505c0303e7975e4a5f48ce8de9 in /nats-streaming-server 
# Wed, 21 Jun 2023 01:11:52 GMT
EXPOSE 4222 8222
# Wed, 21 Jun 2023 01:11:52 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Wed, 21 Jun 2023 01:11:52 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:c3b4c14668a8e32e87c6ea3dce4a99716b527ba7f0f4608cbab27184c89832ee`  
		Last Modified: Wed, 21 Jun 2023 01:12:24 GMT  
		Size: 7.0 MB (7011458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.25-nanoserver`

```console
$ docker pull nats-streaming@sha256:2ea85a60361e0774ce1913ef12baa8fc87bfa4a837a811e89a0a32988b40ed14
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4645; amd64

### `nats-streaming:0.25-nanoserver` - windows version 10.0.17763.4645; amd64

```console
$ docker pull nats-streaming@sha256:5c39267b2e159ad82e792287b1086208f57dbf20ef18e40b553f3b377b337545
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.2 MB (112198939 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ef72ff049bb8cd1e4d7c65b5e46d477eccc664570d1a61e14b52bfc1faaa98f`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Fri, 07 Jul 2023 07:42:59 GMT
RUN Apply image 10.0.17763.4645
# Fri, 14 Jul 2023 00:03:16 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 14 Jul 2023 00:07:54 GMT
RUN cmd /S /C #(nop) COPY file:0e2c8ba21e47adc90962b46928c928315462bcddaefcbc01f98113f4f66cda4a in C:\nats-streaming-server.exe 
# Fri, 14 Jul 2023 00:07:55 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Fri, 14 Jul 2023 00:07:56 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Fri, 14 Jul 2023 00:07:57 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:5c5b06ba65934bcf850a1a54ecf4b3da34d3e6d6c8e90dbc897719c3ea377c8a`  
		Last Modified: Tue, 11 Jul 2023 17:31:37 GMT  
		Size: 104.4 MB (104408241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff4bad9bf846d07362d8295a4479f8f2965dfb5934a9a032b335ce3cb086bdf7`  
		Last Modified: Fri, 14 Jul 2023 00:04:06 GMT  
		Size: 1.2 KB (1161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f94b9b520f177b081bf712ba074ba66cad6139b8164f8e18de5be8ebd3ae7382`  
		Last Modified: Fri, 14 Jul 2023 00:08:34 GMT  
		Size: 7.8 MB (7786370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c03838a3679d351be263b09d3a5c6b9c44c73bd67df1a32d00364b15614d8b4c`  
		Last Modified: Fri, 14 Jul 2023 00:08:32 GMT  
		Size: 1.1 KB (1058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3a7169624bc074e90056b7387038bd434dc1bc770b6ac612f0d295d8db6b10f`  
		Last Modified: Fri, 14 Jul 2023 00:08:31 GMT  
		Size: 1.0 KB (1035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30ef31773aef63c527f320ae07bc5b102bd9f4f448f3b8d21c3e339e30db10e1`  
		Last Modified: Fri, 14 Jul 2023 00:08:32 GMT  
		Size: 1.1 KB (1074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.25-nanoserver-1809`

```console
$ docker pull nats-streaming@sha256:2ea85a60361e0774ce1913ef12baa8fc87bfa4a837a811e89a0a32988b40ed14
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4645; amd64

### `nats-streaming:0.25-nanoserver-1809` - windows version 10.0.17763.4645; amd64

```console
$ docker pull nats-streaming@sha256:5c39267b2e159ad82e792287b1086208f57dbf20ef18e40b553f3b377b337545
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.2 MB (112198939 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ef72ff049bb8cd1e4d7c65b5e46d477eccc664570d1a61e14b52bfc1faaa98f`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Fri, 07 Jul 2023 07:42:59 GMT
RUN Apply image 10.0.17763.4645
# Fri, 14 Jul 2023 00:03:16 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 14 Jul 2023 00:07:54 GMT
RUN cmd /S /C #(nop) COPY file:0e2c8ba21e47adc90962b46928c928315462bcddaefcbc01f98113f4f66cda4a in C:\nats-streaming-server.exe 
# Fri, 14 Jul 2023 00:07:55 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Fri, 14 Jul 2023 00:07:56 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Fri, 14 Jul 2023 00:07:57 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:5c5b06ba65934bcf850a1a54ecf4b3da34d3e6d6c8e90dbc897719c3ea377c8a`  
		Last Modified: Tue, 11 Jul 2023 17:31:37 GMT  
		Size: 104.4 MB (104408241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff4bad9bf846d07362d8295a4479f8f2965dfb5934a9a032b335ce3cb086bdf7`  
		Last Modified: Fri, 14 Jul 2023 00:04:06 GMT  
		Size: 1.2 KB (1161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f94b9b520f177b081bf712ba074ba66cad6139b8164f8e18de5be8ebd3ae7382`  
		Last Modified: Fri, 14 Jul 2023 00:08:34 GMT  
		Size: 7.8 MB (7786370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c03838a3679d351be263b09d3a5c6b9c44c73bd67df1a32d00364b15614d8b4c`  
		Last Modified: Fri, 14 Jul 2023 00:08:32 GMT  
		Size: 1.1 KB (1058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3a7169624bc074e90056b7387038bd434dc1bc770b6ac612f0d295d8db6b10f`  
		Last Modified: Fri, 14 Jul 2023 00:08:31 GMT  
		Size: 1.0 KB (1035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30ef31773aef63c527f320ae07bc5b102bd9f4f448f3b8d21c3e339e30db10e1`  
		Last Modified: Fri, 14 Jul 2023 00:08:32 GMT  
		Size: 1.1 KB (1074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.25-scratch`

```console
$ docker pull nats-streaming@sha256:2b8205e7d3a87aacdc19ec7b71e3316a44380ef15ab834060826911876394dac
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.25-scratch` - linux; amd64

```console
$ docker pull nats-streaming@sha256:0963a4d0a1504acf8b8f5b99fa1f119639a1caff31850eefe83a685fac6820fb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.7 MB (7659749 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:32ad867a381275ce803cc7a4e3007d375908b15c83a75444af3352cfdc72d2eb`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Wed, 21 Jun 2023 01:10:50 GMT
COPY file:670c17c233c7999d9f7b72c2962b221cab4e00da471a75e8679840c939143cfb in /nats-streaming-server 
# Wed, 21 Jun 2023 01:10:50 GMT
EXPOSE 4222 8222
# Wed, 21 Jun 2023 01:10:51 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Wed, 21 Jun 2023 01:10:51 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:b7ff958d406306840566ff165f0c34c6017d44a13d4355d5eb8c6cd152c57d64`  
		Last Modified: Wed, 21 Jun 2023 01:11:25 GMT  
		Size: 7.7 MB (7659749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.25-scratch` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:c6adf4bdcf4ca4548a1331f9a5b78accb38369508960b70058ae6f3cfe00ed5d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7311545 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7763bb2699d3b947f45691cca3c382801ad1c0a91b829831fd0999aa54245f66`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Wed, 21 Jun 2023 00:59:07 GMT
COPY file:9bc2f7015ff72f7e91556a01075e89ef8a85a404228874028f7a356e8142e169 in /nats-streaming-server 
# Wed, 21 Jun 2023 00:59:07 GMT
EXPOSE 4222 8222
# Wed, 21 Jun 2023 00:59:07 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Wed, 21 Jun 2023 00:59:08 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:ee4a78724efc3390679e6118a2f2c5993c9075f378bd6a2f0b7f99b50579fb2b`  
		Last Modified: Wed, 21 Jun 2023 00:59:42 GMT  
		Size: 7.3 MB (7311545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.25-scratch` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:3ae971fd2fa4bc0a898567aa6a6ea4d4dbae8d4459d81e59a2fab244b4d9c5b0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7304325 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:825e70124556ec89714458bdec5da1ee59baa724df73fa420db3005bfad56c45`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Wed, 21 Jun 2023 01:31:21 GMT
COPY file:07846c068b31699c9c9fe9b535ec7c1dcfbda7a16d7d178a50de1f9541deeebf in /nats-streaming-server 
# Wed, 21 Jun 2023 01:31:21 GMT
EXPOSE 4222 8222
# Wed, 21 Jun 2023 01:31:21 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Wed, 21 Jun 2023 01:31:21 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:039446f9a794527f7060ddd5b9b8a071ffe8816fa5aae791c4bbf01db3656057`  
		Last Modified: Wed, 21 Jun 2023 01:31:55 GMT  
		Size: 7.3 MB (7304325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.25-scratch` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:04ef4025a7de920cc90464848b402755e5da72e57bc969aff8859af5429c00a7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.0 MB (7011458 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1627cfd9fc66597d5484a918e734f0595b380583577fd3a532f6228b72db740a`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Wed, 21 Jun 2023 01:11:52 GMT
COPY file:8237d0d59fd3c6b32e52dbff50861a8848f846505c0303e7975e4a5f48ce8de9 in /nats-streaming-server 
# Wed, 21 Jun 2023 01:11:52 GMT
EXPOSE 4222 8222
# Wed, 21 Jun 2023 01:11:52 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Wed, 21 Jun 2023 01:11:52 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:c3b4c14668a8e32e87c6ea3dce4a99716b527ba7f0f4608cbab27184c89832ee`  
		Last Modified: Wed, 21 Jun 2023 01:12:24 GMT  
		Size: 7.0 MB (7011458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.25-windowsservercore`

```console
$ docker pull nats-streaming@sha256:f8f306c1324a747d5f42fbd66e59d90ef995c1f82d95a07af46ec637a8fa29ee
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4645; amd64

### `nats-streaming:0.25-windowsservercore` - windows version 10.0.17763.4645; amd64

```console
$ docker pull nats-streaming@sha256:e3600f1ee85431963c7c2e4ba9dd422516b7c89203680e9098086f8eee913396
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1948162918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba9d6571d5a398539f54f2d4eb7bbdc753472d33dfb4fa5905ed6a249a5ec33c`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Fri, 07 Jul 2023 08:17:39 GMT
RUN Install update 10.0.17763.4645
# Thu, 13 Jul 2023 22:38:00 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Fri, 14 Jul 2023 00:00:18 GMT
ENV NATS_DOCKERIZED=1
# Fri, 14 Jul 2023 00:04:55 GMT
ENV NATS_STREAMING_SERVER=0.25.5
# Fri, 14 Jul 2023 00:04:56 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.25.5/nats-streaming-server-v0.25.5-windows-amd64.zip
# Fri, 14 Jul 2023 00:04:56 GMT
ENV NATS_STREAMING_SERVER_SHASUM=709b481bfa3537dc7941490365e065554f19c7029830d765ef49e8cd16657b75
# Fri, 14 Jul 2023 00:05:52 GMT
RUN Set-PSDebug -Trace 2
# Fri, 14 Jul 2023 00:07:33 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Fri, 14 Jul 2023 00:07:34 GMT
EXPOSE 4222 8222
# Fri, 14 Jul 2023 00:07:35 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Fri, 14 Jul 2023 00:07:36 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e36dba1ee29cd36713c8785a5de7dd2a487244d734ed4c5e7b0a6890bffb806e`  
		Last Modified: Tue, 11 Jul 2023 18:27:38 GMT  
		Size: 289.1 MB (289068746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48b452db6d50a62b6e0e8dadb19715cfcf62cf73e54b5d3bac96621c1093673c`  
		Last Modified: Thu, 13 Jul 2023 23:25:18 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20f8ca4b8d322e27c827c0ba667217bc04a39b69f5f483d5f2f9726e6d42522e`  
		Last Modified: Fri, 14 Jul 2023 00:03:50 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18679ad5f87511b5572cc2ff53e239532dca4c70a413dcf8fc9f8aca97bf4f96`  
		Last Modified: Fri, 14 Jul 2023 00:08:19 GMT  
		Size: 1.3 KB (1279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9c5202984226bceb34a191f9e86a9b84106eebcd4c6a4e47314b707ac610f38`  
		Last Modified: Fri, 14 Jul 2023 00:08:19 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bca3f1baea6a69d419c0fce9341dfac5cbe256fdb7eb9415fe4f1c4edf1a7b93`  
		Last Modified: Fri, 14 Jul 2023 00:08:18 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4631c84b931d3f1ee529f0423fa3188ea9e48d8af0089a9887fa992becd65312`  
		Last Modified: Fri, 14 Jul 2023 00:08:17 GMT  
		Size: 226.1 KB (226123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a195df7f50ec1e109468319f7e85f27d494af37f9eceb4586c2abd45b7798ec9`  
		Last Modified: Fri, 14 Jul 2023 00:08:19 GMT  
		Size: 8.2 MB (8237038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7271bd8c5599f12857ee3ed75550b08dc3638819425f32fd3ab0b104dda1e0d8`  
		Last Modified: Fri, 14 Jul 2023 00:08:17 GMT  
		Size: 1.3 KB (1324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2001f0adacd1483a7214db132b80267a2d9a728c9099b49a73bffec74f4c4c47`  
		Last Modified: Fri, 14 Jul 2023 00:08:17 GMT  
		Size: 1.3 KB (1313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:076f3743d3f1ac915066251cf19292b7e95d2b21d98f6d6fa723ced8cf864026`  
		Last Modified: Fri, 14 Jul 2023 00:08:17 GMT  
		Size: 1.3 KB (1335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.25-windowsservercore-1809`

```console
$ docker pull nats-streaming@sha256:f8f306c1324a747d5f42fbd66e59d90ef995c1f82d95a07af46ec637a8fa29ee
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4645; amd64

### `nats-streaming:0.25-windowsservercore-1809` - windows version 10.0.17763.4645; amd64

```console
$ docker pull nats-streaming@sha256:e3600f1ee85431963c7c2e4ba9dd422516b7c89203680e9098086f8eee913396
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1948162918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba9d6571d5a398539f54f2d4eb7bbdc753472d33dfb4fa5905ed6a249a5ec33c`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Fri, 07 Jul 2023 08:17:39 GMT
RUN Install update 10.0.17763.4645
# Thu, 13 Jul 2023 22:38:00 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Fri, 14 Jul 2023 00:00:18 GMT
ENV NATS_DOCKERIZED=1
# Fri, 14 Jul 2023 00:04:55 GMT
ENV NATS_STREAMING_SERVER=0.25.5
# Fri, 14 Jul 2023 00:04:56 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.25.5/nats-streaming-server-v0.25.5-windows-amd64.zip
# Fri, 14 Jul 2023 00:04:56 GMT
ENV NATS_STREAMING_SERVER_SHASUM=709b481bfa3537dc7941490365e065554f19c7029830d765ef49e8cd16657b75
# Fri, 14 Jul 2023 00:05:52 GMT
RUN Set-PSDebug -Trace 2
# Fri, 14 Jul 2023 00:07:33 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Fri, 14 Jul 2023 00:07:34 GMT
EXPOSE 4222 8222
# Fri, 14 Jul 2023 00:07:35 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Fri, 14 Jul 2023 00:07:36 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e36dba1ee29cd36713c8785a5de7dd2a487244d734ed4c5e7b0a6890bffb806e`  
		Last Modified: Tue, 11 Jul 2023 18:27:38 GMT  
		Size: 289.1 MB (289068746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48b452db6d50a62b6e0e8dadb19715cfcf62cf73e54b5d3bac96621c1093673c`  
		Last Modified: Thu, 13 Jul 2023 23:25:18 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20f8ca4b8d322e27c827c0ba667217bc04a39b69f5f483d5f2f9726e6d42522e`  
		Last Modified: Fri, 14 Jul 2023 00:03:50 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18679ad5f87511b5572cc2ff53e239532dca4c70a413dcf8fc9f8aca97bf4f96`  
		Last Modified: Fri, 14 Jul 2023 00:08:19 GMT  
		Size: 1.3 KB (1279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9c5202984226bceb34a191f9e86a9b84106eebcd4c6a4e47314b707ac610f38`  
		Last Modified: Fri, 14 Jul 2023 00:08:19 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bca3f1baea6a69d419c0fce9341dfac5cbe256fdb7eb9415fe4f1c4edf1a7b93`  
		Last Modified: Fri, 14 Jul 2023 00:08:18 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4631c84b931d3f1ee529f0423fa3188ea9e48d8af0089a9887fa992becd65312`  
		Last Modified: Fri, 14 Jul 2023 00:08:17 GMT  
		Size: 226.1 KB (226123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a195df7f50ec1e109468319f7e85f27d494af37f9eceb4586c2abd45b7798ec9`  
		Last Modified: Fri, 14 Jul 2023 00:08:19 GMT  
		Size: 8.2 MB (8237038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7271bd8c5599f12857ee3ed75550b08dc3638819425f32fd3ab0b104dda1e0d8`  
		Last Modified: Fri, 14 Jul 2023 00:08:17 GMT  
		Size: 1.3 KB (1324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2001f0adacd1483a7214db132b80267a2d9a728c9099b49a73bffec74f4c4c47`  
		Last Modified: Fri, 14 Jul 2023 00:08:17 GMT  
		Size: 1.3 KB (1313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:076f3743d3f1ac915066251cf19292b7e95d2b21d98f6d6fa723ced8cf864026`  
		Last Modified: Fri, 14 Jul 2023 00:08:17 GMT  
		Size: 1.3 KB (1335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.25.5`

```console
$ docker pull nats-streaming@sha256:1eed8c2ef0f8b6e0c7264013e3f64f7f2a75195827fce558fde4d277bfcb4b7a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.4645; amd64

### `nats-streaming:0.25.5` - linux; amd64

```console
$ docker pull nats-streaming@sha256:0963a4d0a1504acf8b8f5b99fa1f119639a1caff31850eefe83a685fac6820fb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.7 MB (7659749 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:32ad867a381275ce803cc7a4e3007d375908b15c83a75444af3352cfdc72d2eb`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Wed, 21 Jun 2023 01:10:50 GMT
COPY file:670c17c233c7999d9f7b72c2962b221cab4e00da471a75e8679840c939143cfb in /nats-streaming-server 
# Wed, 21 Jun 2023 01:10:50 GMT
EXPOSE 4222 8222
# Wed, 21 Jun 2023 01:10:51 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Wed, 21 Jun 2023 01:10:51 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:b7ff958d406306840566ff165f0c34c6017d44a13d4355d5eb8c6cd152c57d64`  
		Last Modified: Wed, 21 Jun 2023 01:11:25 GMT  
		Size: 7.7 MB (7659749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.25.5` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:c6adf4bdcf4ca4548a1331f9a5b78accb38369508960b70058ae6f3cfe00ed5d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7311545 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7763bb2699d3b947f45691cca3c382801ad1c0a91b829831fd0999aa54245f66`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Wed, 21 Jun 2023 00:59:07 GMT
COPY file:9bc2f7015ff72f7e91556a01075e89ef8a85a404228874028f7a356e8142e169 in /nats-streaming-server 
# Wed, 21 Jun 2023 00:59:07 GMT
EXPOSE 4222 8222
# Wed, 21 Jun 2023 00:59:07 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Wed, 21 Jun 2023 00:59:08 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:ee4a78724efc3390679e6118a2f2c5993c9075f378bd6a2f0b7f99b50579fb2b`  
		Last Modified: Wed, 21 Jun 2023 00:59:42 GMT  
		Size: 7.3 MB (7311545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.25.5` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:3ae971fd2fa4bc0a898567aa6a6ea4d4dbae8d4459d81e59a2fab244b4d9c5b0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7304325 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:825e70124556ec89714458bdec5da1ee59baa724df73fa420db3005bfad56c45`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Wed, 21 Jun 2023 01:31:21 GMT
COPY file:07846c068b31699c9c9fe9b535ec7c1dcfbda7a16d7d178a50de1f9541deeebf in /nats-streaming-server 
# Wed, 21 Jun 2023 01:31:21 GMT
EXPOSE 4222 8222
# Wed, 21 Jun 2023 01:31:21 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Wed, 21 Jun 2023 01:31:21 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:039446f9a794527f7060ddd5b9b8a071ffe8816fa5aae791c4bbf01db3656057`  
		Last Modified: Wed, 21 Jun 2023 01:31:55 GMT  
		Size: 7.3 MB (7304325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.25.5` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:04ef4025a7de920cc90464848b402755e5da72e57bc969aff8859af5429c00a7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.0 MB (7011458 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1627cfd9fc66597d5484a918e734f0595b380583577fd3a532f6228b72db740a`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Wed, 21 Jun 2023 01:11:52 GMT
COPY file:8237d0d59fd3c6b32e52dbff50861a8848f846505c0303e7975e4a5f48ce8de9 in /nats-streaming-server 
# Wed, 21 Jun 2023 01:11:52 GMT
EXPOSE 4222 8222
# Wed, 21 Jun 2023 01:11:52 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Wed, 21 Jun 2023 01:11:52 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:c3b4c14668a8e32e87c6ea3dce4a99716b527ba7f0f4608cbab27184c89832ee`  
		Last Modified: Wed, 21 Jun 2023 01:12:24 GMT  
		Size: 7.0 MB (7011458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.25.5` - windows version 10.0.17763.4645; amd64

```console
$ docker pull nats-streaming@sha256:5c39267b2e159ad82e792287b1086208f57dbf20ef18e40b553f3b377b337545
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.2 MB (112198939 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ef72ff049bb8cd1e4d7c65b5e46d477eccc664570d1a61e14b52bfc1faaa98f`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Fri, 07 Jul 2023 07:42:59 GMT
RUN Apply image 10.0.17763.4645
# Fri, 14 Jul 2023 00:03:16 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 14 Jul 2023 00:07:54 GMT
RUN cmd /S /C #(nop) COPY file:0e2c8ba21e47adc90962b46928c928315462bcddaefcbc01f98113f4f66cda4a in C:\nats-streaming-server.exe 
# Fri, 14 Jul 2023 00:07:55 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Fri, 14 Jul 2023 00:07:56 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Fri, 14 Jul 2023 00:07:57 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:5c5b06ba65934bcf850a1a54ecf4b3da34d3e6d6c8e90dbc897719c3ea377c8a`  
		Last Modified: Tue, 11 Jul 2023 17:31:37 GMT  
		Size: 104.4 MB (104408241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff4bad9bf846d07362d8295a4479f8f2965dfb5934a9a032b335ce3cb086bdf7`  
		Last Modified: Fri, 14 Jul 2023 00:04:06 GMT  
		Size: 1.2 KB (1161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f94b9b520f177b081bf712ba074ba66cad6139b8164f8e18de5be8ebd3ae7382`  
		Last Modified: Fri, 14 Jul 2023 00:08:34 GMT  
		Size: 7.8 MB (7786370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c03838a3679d351be263b09d3a5c6b9c44c73bd67df1a32d00364b15614d8b4c`  
		Last Modified: Fri, 14 Jul 2023 00:08:32 GMT  
		Size: 1.1 KB (1058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3a7169624bc074e90056b7387038bd434dc1bc770b6ac612f0d295d8db6b10f`  
		Last Modified: Fri, 14 Jul 2023 00:08:31 GMT  
		Size: 1.0 KB (1035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30ef31773aef63c527f320ae07bc5b102bd9f4f448f3b8d21c3e339e30db10e1`  
		Last Modified: Fri, 14 Jul 2023 00:08:32 GMT  
		Size: 1.1 KB (1074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.25.5-alpine`

```console
$ docker pull nats-streaming@sha256:c9e97ca2eb081301837053ea04e6a1dfc4fedacacf21a10b540693546de6c733
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.25.5-alpine` - linux; amd64

```console
$ docker pull nats-streaming@sha256:6abf524d6062038a5c5c66c0733592ac2d3151abbd8b423facb5f4f575fbabda
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.3 MB (11344002 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:259306c401d301ff49ceac471b001513aeb8ec5ce27d8e92b4a6c0c4a7be30f3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 14 Jun 2023 20:41:58 GMT
ADD file:1da756d12551a0e3e793e02ef87432d69d4968937bd11bed0af215db19dd94cd in / 
# Wed, 14 Jun 2023 20:41:59 GMT
CMD ["/bin/sh"]
# Wed, 21 Jun 2023 01:10:41 GMT
ENV NATS_STREAMING_SERVER=0.25.5
# Wed, 21 Jun 2023 01:10:43 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='937af3f9cdbfe3cb4648cf8c8f505dded2cc175d59ba10e13ec71d1c04e61bf2' ;; 		armhf) natsArch='arm6'; sha256='5bd3a0456054505741b05e5d03acb9f7a5de97cf3ea20cd52d31edbae1c387ea' ;; 		armv7) natsArch='arm7'; sha256='0e643e9881cf3acf3313f84853451d1c4a1e731bc8599d223a40042f9c0c7285' ;; 		x86_64) natsArch='amd64'; sha256='22762f4d0ccfc75947096a14e09566b816113e125a3d39f7914a0c332bee25a7' ;; 		x86) natsArch='386'; sha256='92d8d4460f538883c78e67a334b23b2317e4fe58d46e4fdbbef8b4c09c7b97ae' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Wed, 21 Jun 2023 01:10:43 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Wed, 21 Jun 2023 01:10:44 GMT
EXPOSE 4222 8222
# Wed, 21 Jun 2023 01:10:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Jun 2023 01:10:44 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:31e352740f534f9ad170f75378a84fe453d6156e40700b882d737a8f4a6988a3`  
		Last Modified: Wed, 14 Jun 2023 20:42:26 GMT  
		Size: 3.4 MB (3397879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0ccb9db0d77fa25becf9aa3c73f0a091378e47d9a8c0d87114fe3ca75b17483`  
		Last Modified: Wed, 21 Jun 2023 01:11:09 GMT  
		Size: 7.9 MB (7945701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56d62dc9de67132e108b1f8b40907849093f018255907030abdb3fc7b94904a9`  
		Last Modified: Wed, 21 Jun 2023 01:11:07 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.25.5-alpine` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:df08adb5a35cd347a0f1d96e733b0ba3b963a100fe08534f0e3a7a739f7453d2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.7 MB (10745511 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e879e367a39ad7817ae00eaf4a01036cc223cf63db3d0b10455e54a4fcf76bc3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Mon, 07 Aug 2023 19:49:14 GMT
ADD file:9882e99e5f94ab2db05c029648ac5be7cf0f063a8701394fcbb543a7ef5d4b90 in / 
# Mon, 07 Aug 2023 19:49:15 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 20:44:50 GMT
ENV NATS_STREAMING_SERVER=0.25.5
# Tue, 08 Aug 2023 20:44:52 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='937af3f9cdbfe3cb4648cf8c8f505dded2cc175d59ba10e13ec71d1c04e61bf2' ;; 		armhf) natsArch='arm6'; sha256='5bd3a0456054505741b05e5d03acb9f7a5de97cf3ea20cd52d31edbae1c387ea' ;; 		armv7) natsArch='arm7'; sha256='0e643e9881cf3acf3313f84853451d1c4a1e731bc8599d223a40042f9c0c7285' ;; 		x86_64) natsArch='amd64'; sha256='22762f4d0ccfc75947096a14e09566b816113e125a3d39f7914a0c332bee25a7' ;; 		x86) natsArch='386'; sha256='92d8d4460f538883c78e67a334b23b2317e4fe58d46e4fdbbef8b4c09c7b97ae' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Tue, 08 Aug 2023 20:44:53 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Tue, 08 Aug 2023 20:44:53 GMT
EXPOSE 4222 8222
# Tue, 08 Aug 2023 20:44:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 08 Aug 2023 20:44:53 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:af09961d4a43b504efc76e38b50918977c28be73eeb8b926247783a00e8b9f2f`  
		Last Modified: Mon, 07 Aug 2023 19:49:38 GMT  
		Size: 3.1 MB (3144809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db57a023cb1e641cc4e410d847ed348704fa48f194e6e04feb97859ea8263399`  
		Last Modified: Tue, 08 Aug 2023 20:45:13 GMT  
		Size: 7.6 MB (7600282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d00d13e6c7ccee53d63384bf85378713efa9cd84cb8817b81ddcb19ab83106e3`  
		Last Modified: Tue, 08 Aug 2023 20:45:11 GMT  
		Size: 420.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.25.5-alpine` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:8b69faa2f13f8bb2769c9ca014cfb884a6f581175bf1ad9baaa59b914ef3a7fe
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.5 MB (10488008 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6b906477dbd127990b39bdff954cd4495c0027ae495dad6ab5c740cff11c8a4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Mon, 07 Aug 2023 19:57:25 GMT
ADD file:e3f56488d3d3bb67729714db13ddadf6652e7efb5281cfc7010d3e71f9d6607f in / 
# Mon, 07 Aug 2023 19:57:25 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 02:15:20 GMT
ENV NATS_STREAMING_SERVER=0.25.5
# Tue, 08 Aug 2023 02:15:23 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='937af3f9cdbfe3cb4648cf8c8f505dded2cc175d59ba10e13ec71d1c04e61bf2' ;; 		armhf) natsArch='arm6'; sha256='5bd3a0456054505741b05e5d03acb9f7a5de97cf3ea20cd52d31edbae1c387ea' ;; 		armv7) natsArch='arm7'; sha256='0e643e9881cf3acf3313f84853451d1c4a1e731bc8599d223a40042f9c0c7285' ;; 		x86_64) natsArch='amd64'; sha256='22762f4d0ccfc75947096a14e09566b816113e125a3d39f7914a0c332bee25a7' ;; 		x86) natsArch='386'; sha256='92d8d4460f538883c78e67a334b23b2317e4fe58d46e4fdbbef8b4c09c7b97ae' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Tue, 08 Aug 2023 02:15:23 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Tue, 08 Aug 2023 02:15:23 GMT
EXPOSE 4222 8222
# Tue, 08 Aug 2023 02:15:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 08 Aug 2023 02:15:24 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:f8dec92eec42224ef9e6ca9c6207ea6b9195dcf93d06bd5ceff0f814b62bf064`  
		Last Modified: Mon, 07 Aug 2023 19:57:55 GMT  
		Size: 2.9 MB (2899480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e18324f789c9a02a3fb3992cee161f01f2d80d6396a0eb54b83956b93f18e24b`  
		Last Modified: Tue, 08 Aug 2023 02:15:50 GMT  
		Size: 7.6 MB (7588109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bff0b4480470ca012849b4227c612a9a456bed7a67117efc5fb5c5a737d17e9`  
		Last Modified: Tue, 08 Aug 2023 02:15:48 GMT  
		Size: 419.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.25.5-alpine` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:9f7fa008b1524911fee4a485f955408c7b911611179fdf120a2bb89f3323cdfa
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.6 MB (10629737 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5be4dd1beeb3895e9906e2866ca807b53f3b5cbc33598ed378b76126ded32d8d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 14 Jun 2023 20:48:58 GMT
ADD file:289c2fac17119508ced527225d445747cd177111b4a0018a6b04948ecb3b5e29 in / 
# Wed, 14 Jun 2023 20:48:58 GMT
CMD ["/bin/sh"]
# Wed, 21 Jun 2023 01:11:44 GMT
ENV NATS_STREAMING_SERVER=0.25.5
# Wed, 21 Jun 2023 01:11:46 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='937af3f9cdbfe3cb4648cf8c8f505dded2cc175d59ba10e13ec71d1c04e61bf2' ;; 		armhf) natsArch='arm6'; sha256='5bd3a0456054505741b05e5d03acb9f7a5de97cf3ea20cd52d31edbae1c387ea' ;; 		armv7) natsArch='arm7'; sha256='0e643e9881cf3acf3313f84853451d1c4a1e731bc8599d223a40042f9c0c7285' ;; 		x86_64) natsArch='amd64'; sha256='22762f4d0ccfc75947096a14e09566b816113e125a3d39f7914a0c332bee25a7' ;; 		x86) natsArch='386'; sha256='92d8d4460f538883c78e67a334b23b2317e4fe58d46e4fdbbef8b4c09c7b97ae' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Wed, 21 Jun 2023 01:11:46 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Wed, 21 Jun 2023 01:11:46 GMT
EXPOSE 4222 8222
# Wed, 21 Jun 2023 01:11:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Jun 2023 01:11:46 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:8c6d1654570f041603f4cef49c320c8f6f3e401324913009d92a19132cbf1ac0`  
		Last Modified: Wed, 14 Jun 2023 20:49:23 GMT  
		Size: 3.3 MB (3329251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3146f74e4cb95e61d4f251594c3330ad0f9c85345a1b97bce44ab0446ee59269`  
		Last Modified: Wed, 21 Jun 2023 01:12:08 GMT  
		Size: 7.3 MB (7300064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:775fc9bc0a0519e7fe2cd9656617079a95fd7919b285649d10cf4f76b7e89b49`  
		Last Modified: Wed, 21 Jun 2023 01:12:07 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.25.5-alpine3.18`

```console
$ docker pull nats-streaming@sha256:c9e97ca2eb081301837053ea04e6a1dfc4fedacacf21a10b540693546de6c733
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.25.5-alpine3.18` - linux; amd64

```console
$ docker pull nats-streaming@sha256:6abf524d6062038a5c5c66c0733592ac2d3151abbd8b423facb5f4f575fbabda
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.3 MB (11344002 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:259306c401d301ff49ceac471b001513aeb8ec5ce27d8e92b4a6c0c4a7be30f3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 14 Jun 2023 20:41:58 GMT
ADD file:1da756d12551a0e3e793e02ef87432d69d4968937bd11bed0af215db19dd94cd in / 
# Wed, 14 Jun 2023 20:41:59 GMT
CMD ["/bin/sh"]
# Wed, 21 Jun 2023 01:10:41 GMT
ENV NATS_STREAMING_SERVER=0.25.5
# Wed, 21 Jun 2023 01:10:43 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='937af3f9cdbfe3cb4648cf8c8f505dded2cc175d59ba10e13ec71d1c04e61bf2' ;; 		armhf) natsArch='arm6'; sha256='5bd3a0456054505741b05e5d03acb9f7a5de97cf3ea20cd52d31edbae1c387ea' ;; 		armv7) natsArch='arm7'; sha256='0e643e9881cf3acf3313f84853451d1c4a1e731bc8599d223a40042f9c0c7285' ;; 		x86_64) natsArch='amd64'; sha256='22762f4d0ccfc75947096a14e09566b816113e125a3d39f7914a0c332bee25a7' ;; 		x86) natsArch='386'; sha256='92d8d4460f538883c78e67a334b23b2317e4fe58d46e4fdbbef8b4c09c7b97ae' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Wed, 21 Jun 2023 01:10:43 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Wed, 21 Jun 2023 01:10:44 GMT
EXPOSE 4222 8222
# Wed, 21 Jun 2023 01:10:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Jun 2023 01:10:44 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:31e352740f534f9ad170f75378a84fe453d6156e40700b882d737a8f4a6988a3`  
		Last Modified: Wed, 14 Jun 2023 20:42:26 GMT  
		Size: 3.4 MB (3397879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0ccb9db0d77fa25becf9aa3c73f0a091378e47d9a8c0d87114fe3ca75b17483`  
		Last Modified: Wed, 21 Jun 2023 01:11:09 GMT  
		Size: 7.9 MB (7945701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56d62dc9de67132e108b1f8b40907849093f018255907030abdb3fc7b94904a9`  
		Last Modified: Wed, 21 Jun 2023 01:11:07 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.25.5-alpine3.18` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:df08adb5a35cd347a0f1d96e733b0ba3b963a100fe08534f0e3a7a739f7453d2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.7 MB (10745511 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e879e367a39ad7817ae00eaf4a01036cc223cf63db3d0b10455e54a4fcf76bc3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Mon, 07 Aug 2023 19:49:14 GMT
ADD file:9882e99e5f94ab2db05c029648ac5be7cf0f063a8701394fcbb543a7ef5d4b90 in / 
# Mon, 07 Aug 2023 19:49:15 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 20:44:50 GMT
ENV NATS_STREAMING_SERVER=0.25.5
# Tue, 08 Aug 2023 20:44:52 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='937af3f9cdbfe3cb4648cf8c8f505dded2cc175d59ba10e13ec71d1c04e61bf2' ;; 		armhf) natsArch='arm6'; sha256='5bd3a0456054505741b05e5d03acb9f7a5de97cf3ea20cd52d31edbae1c387ea' ;; 		armv7) natsArch='arm7'; sha256='0e643e9881cf3acf3313f84853451d1c4a1e731bc8599d223a40042f9c0c7285' ;; 		x86_64) natsArch='amd64'; sha256='22762f4d0ccfc75947096a14e09566b816113e125a3d39f7914a0c332bee25a7' ;; 		x86) natsArch='386'; sha256='92d8d4460f538883c78e67a334b23b2317e4fe58d46e4fdbbef8b4c09c7b97ae' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Tue, 08 Aug 2023 20:44:53 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Tue, 08 Aug 2023 20:44:53 GMT
EXPOSE 4222 8222
# Tue, 08 Aug 2023 20:44:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 08 Aug 2023 20:44:53 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:af09961d4a43b504efc76e38b50918977c28be73eeb8b926247783a00e8b9f2f`  
		Last Modified: Mon, 07 Aug 2023 19:49:38 GMT  
		Size: 3.1 MB (3144809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db57a023cb1e641cc4e410d847ed348704fa48f194e6e04feb97859ea8263399`  
		Last Modified: Tue, 08 Aug 2023 20:45:13 GMT  
		Size: 7.6 MB (7600282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d00d13e6c7ccee53d63384bf85378713efa9cd84cb8817b81ddcb19ab83106e3`  
		Last Modified: Tue, 08 Aug 2023 20:45:11 GMT  
		Size: 420.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.25.5-alpine3.18` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:8b69faa2f13f8bb2769c9ca014cfb884a6f581175bf1ad9baaa59b914ef3a7fe
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.5 MB (10488008 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6b906477dbd127990b39bdff954cd4495c0027ae495dad6ab5c740cff11c8a4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Mon, 07 Aug 2023 19:57:25 GMT
ADD file:e3f56488d3d3bb67729714db13ddadf6652e7efb5281cfc7010d3e71f9d6607f in / 
# Mon, 07 Aug 2023 19:57:25 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 02:15:20 GMT
ENV NATS_STREAMING_SERVER=0.25.5
# Tue, 08 Aug 2023 02:15:23 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='937af3f9cdbfe3cb4648cf8c8f505dded2cc175d59ba10e13ec71d1c04e61bf2' ;; 		armhf) natsArch='arm6'; sha256='5bd3a0456054505741b05e5d03acb9f7a5de97cf3ea20cd52d31edbae1c387ea' ;; 		armv7) natsArch='arm7'; sha256='0e643e9881cf3acf3313f84853451d1c4a1e731bc8599d223a40042f9c0c7285' ;; 		x86_64) natsArch='amd64'; sha256='22762f4d0ccfc75947096a14e09566b816113e125a3d39f7914a0c332bee25a7' ;; 		x86) natsArch='386'; sha256='92d8d4460f538883c78e67a334b23b2317e4fe58d46e4fdbbef8b4c09c7b97ae' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Tue, 08 Aug 2023 02:15:23 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Tue, 08 Aug 2023 02:15:23 GMT
EXPOSE 4222 8222
# Tue, 08 Aug 2023 02:15:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 08 Aug 2023 02:15:24 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:f8dec92eec42224ef9e6ca9c6207ea6b9195dcf93d06bd5ceff0f814b62bf064`  
		Last Modified: Mon, 07 Aug 2023 19:57:55 GMT  
		Size: 2.9 MB (2899480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e18324f789c9a02a3fb3992cee161f01f2d80d6396a0eb54b83956b93f18e24b`  
		Last Modified: Tue, 08 Aug 2023 02:15:50 GMT  
		Size: 7.6 MB (7588109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bff0b4480470ca012849b4227c612a9a456bed7a67117efc5fb5c5a737d17e9`  
		Last Modified: Tue, 08 Aug 2023 02:15:48 GMT  
		Size: 419.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.25.5-alpine3.18` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:9f7fa008b1524911fee4a485f955408c7b911611179fdf120a2bb89f3323cdfa
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.6 MB (10629737 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5be4dd1beeb3895e9906e2866ca807b53f3b5cbc33598ed378b76126ded32d8d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 14 Jun 2023 20:48:58 GMT
ADD file:289c2fac17119508ced527225d445747cd177111b4a0018a6b04948ecb3b5e29 in / 
# Wed, 14 Jun 2023 20:48:58 GMT
CMD ["/bin/sh"]
# Wed, 21 Jun 2023 01:11:44 GMT
ENV NATS_STREAMING_SERVER=0.25.5
# Wed, 21 Jun 2023 01:11:46 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='937af3f9cdbfe3cb4648cf8c8f505dded2cc175d59ba10e13ec71d1c04e61bf2' ;; 		armhf) natsArch='arm6'; sha256='5bd3a0456054505741b05e5d03acb9f7a5de97cf3ea20cd52d31edbae1c387ea' ;; 		armv7) natsArch='arm7'; sha256='0e643e9881cf3acf3313f84853451d1c4a1e731bc8599d223a40042f9c0c7285' ;; 		x86_64) natsArch='amd64'; sha256='22762f4d0ccfc75947096a14e09566b816113e125a3d39f7914a0c332bee25a7' ;; 		x86) natsArch='386'; sha256='92d8d4460f538883c78e67a334b23b2317e4fe58d46e4fdbbef8b4c09c7b97ae' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Wed, 21 Jun 2023 01:11:46 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Wed, 21 Jun 2023 01:11:46 GMT
EXPOSE 4222 8222
# Wed, 21 Jun 2023 01:11:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Jun 2023 01:11:46 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:8c6d1654570f041603f4cef49c320c8f6f3e401324913009d92a19132cbf1ac0`  
		Last Modified: Wed, 14 Jun 2023 20:49:23 GMT  
		Size: 3.3 MB (3329251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3146f74e4cb95e61d4f251594c3330ad0f9c85345a1b97bce44ab0446ee59269`  
		Last Modified: Wed, 21 Jun 2023 01:12:08 GMT  
		Size: 7.3 MB (7300064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:775fc9bc0a0519e7fe2cd9656617079a95fd7919b285649d10cf4f76b7e89b49`  
		Last Modified: Wed, 21 Jun 2023 01:12:07 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.25.5-linux`

```console
$ docker pull nats-streaming@sha256:2b8205e7d3a87aacdc19ec7b71e3316a44380ef15ab834060826911876394dac
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.25.5-linux` - linux; amd64

```console
$ docker pull nats-streaming@sha256:0963a4d0a1504acf8b8f5b99fa1f119639a1caff31850eefe83a685fac6820fb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.7 MB (7659749 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:32ad867a381275ce803cc7a4e3007d375908b15c83a75444af3352cfdc72d2eb`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Wed, 21 Jun 2023 01:10:50 GMT
COPY file:670c17c233c7999d9f7b72c2962b221cab4e00da471a75e8679840c939143cfb in /nats-streaming-server 
# Wed, 21 Jun 2023 01:10:50 GMT
EXPOSE 4222 8222
# Wed, 21 Jun 2023 01:10:51 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Wed, 21 Jun 2023 01:10:51 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:b7ff958d406306840566ff165f0c34c6017d44a13d4355d5eb8c6cd152c57d64`  
		Last Modified: Wed, 21 Jun 2023 01:11:25 GMT  
		Size: 7.7 MB (7659749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.25.5-linux` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:c6adf4bdcf4ca4548a1331f9a5b78accb38369508960b70058ae6f3cfe00ed5d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7311545 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7763bb2699d3b947f45691cca3c382801ad1c0a91b829831fd0999aa54245f66`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Wed, 21 Jun 2023 00:59:07 GMT
COPY file:9bc2f7015ff72f7e91556a01075e89ef8a85a404228874028f7a356e8142e169 in /nats-streaming-server 
# Wed, 21 Jun 2023 00:59:07 GMT
EXPOSE 4222 8222
# Wed, 21 Jun 2023 00:59:07 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Wed, 21 Jun 2023 00:59:08 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:ee4a78724efc3390679e6118a2f2c5993c9075f378bd6a2f0b7f99b50579fb2b`  
		Last Modified: Wed, 21 Jun 2023 00:59:42 GMT  
		Size: 7.3 MB (7311545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.25.5-linux` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:3ae971fd2fa4bc0a898567aa6a6ea4d4dbae8d4459d81e59a2fab244b4d9c5b0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7304325 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:825e70124556ec89714458bdec5da1ee59baa724df73fa420db3005bfad56c45`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Wed, 21 Jun 2023 01:31:21 GMT
COPY file:07846c068b31699c9c9fe9b535ec7c1dcfbda7a16d7d178a50de1f9541deeebf in /nats-streaming-server 
# Wed, 21 Jun 2023 01:31:21 GMT
EXPOSE 4222 8222
# Wed, 21 Jun 2023 01:31:21 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Wed, 21 Jun 2023 01:31:21 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:039446f9a794527f7060ddd5b9b8a071ffe8816fa5aae791c4bbf01db3656057`  
		Last Modified: Wed, 21 Jun 2023 01:31:55 GMT  
		Size: 7.3 MB (7304325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.25.5-linux` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:04ef4025a7de920cc90464848b402755e5da72e57bc969aff8859af5429c00a7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.0 MB (7011458 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1627cfd9fc66597d5484a918e734f0595b380583577fd3a532f6228b72db740a`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Wed, 21 Jun 2023 01:11:52 GMT
COPY file:8237d0d59fd3c6b32e52dbff50861a8848f846505c0303e7975e4a5f48ce8de9 in /nats-streaming-server 
# Wed, 21 Jun 2023 01:11:52 GMT
EXPOSE 4222 8222
# Wed, 21 Jun 2023 01:11:52 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Wed, 21 Jun 2023 01:11:52 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:c3b4c14668a8e32e87c6ea3dce4a99716b527ba7f0f4608cbab27184c89832ee`  
		Last Modified: Wed, 21 Jun 2023 01:12:24 GMT  
		Size: 7.0 MB (7011458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.25.5-nanoserver`

```console
$ docker pull nats-streaming@sha256:2ea85a60361e0774ce1913ef12baa8fc87bfa4a837a811e89a0a32988b40ed14
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4645; amd64

### `nats-streaming:0.25.5-nanoserver` - windows version 10.0.17763.4645; amd64

```console
$ docker pull nats-streaming@sha256:5c39267b2e159ad82e792287b1086208f57dbf20ef18e40b553f3b377b337545
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.2 MB (112198939 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ef72ff049bb8cd1e4d7c65b5e46d477eccc664570d1a61e14b52bfc1faaa98f`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Fri, 07 Jul 2023 07:42:59 GMT
RUN Apply image 10.0.17763.4645
# Fri, 14 Jul 2023 00:03:16 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 14 Jul 2023 00:07:54 GMT
RUN cmd /S /C #(nop) COPY file:0e2c8ba21e47adc90962b46928c928315462bcddaefcbc01f98113f4f66cda4a in C:\nats-streaming-server.exe 
# Fri, 14 Jul 2023 00:07:55 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Fri, 14 Jul 2023 00:07:56 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Fri, 14 Jul 2023 00:07:57 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:5c5b06ba65934bcf850a1a54ecf4b3da34d3e6d6c8e90dbc897719c3ea377c8a`  
		Last Modified: Tue, 11 Jul 2023 17:31:37 GMT  
		Size: 104.4 MB (104408241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff4bad9bf846d07362d8295a4479f8f2965dfb5934a9a032b335ce3cb086bdf7`  
		Last Modified: Fri, 14 Jul 2023 00:04:06 GMT  
		Size: 1.2 KB (1161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f94b9b520f177b081bf712ba074ba66cad6139b8164f8e18de5be8ebd3ae7382`  
		Last Modified: Fri, 14 Jul 2023 00:08:34 GMT  
		Size: 7.8 MB (7786370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c03838a3679d351be263b09d3a5c6b9c44c73bd67df1a32d00364b15614d8b4c`  
		Last Modified: Fri, 14 Jul 2023 00:08:32 GMT  
		Size: 1.1 KB (1058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3a7169624bc074e90056b7387038bd434dc1bc770b6ac612f0d295d8db6b10f`  
		Last Modified: Fri, 14 Jul 2023 00:08:31 GMT  
		Size: 1.0 KB (1035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30ef31773aef63c527f320ae07bc5b102bd9f4f448f3b8d21c3e339e30db10e1`  
		Last Modified: Fri, 14 Jul 2023 00:08:32 GMT  
		Size: 1.1 KB (1074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.25.5-nanoserver-1809`

```console
$ docker pull nats-streaming@sha256:2ea85a60361e0774ce1913ef12baa8fc87bfa4a837a811e89a0a32988b40ed14
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4645; amd64

### `nats-streaming:0.25.5-nanoserver-1809` - windows version 10.0.17763.4645; amd64

```console
$ docker pull nats-streaming@sha256:5c39267b2e159ad82e792287b1086208f57dbf20ef18e40b553f3b377b337545
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.2 MB (112198939 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ef72ff049bb8cd1e4d7c65b5e46d477eccc664570d1a61e14b52bfc1faaa98f`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Fri, 07 Jul 2023 07:42:59 GMT
RUN Apply image 10.0.17763.4645
# Fri, 14 Jul 2023 00:03:16 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 14 Jul 2023 00:07:54 GMT
RUN cmd /S /C #(nop) COPY file:0e2c8ba21e47adc90962b46928c928315462bcddaefcbc01f98113f4f66cda4a in C:\nats-streaming-server.exe 
# Fri, 14 Jul 2023 00:07:55 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Fri, 14 Jul 2023 00:07:56 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Fri, 14 Jul 2023 00:07:57 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:5c5b06ba65934bcf850a1a54ecf4b3da34d3e6d6c8e90dbc897719c3ea377c8a`  
		Last Modified: Tue, 11 Jul 2023 17:31:37 GMT  
		Size: 104.4 MB (104408241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff4bad9bf846d07362d8295a4479f8f2965dfb5934a9a032b335ce3cb086bdf7`  
		Last Modified: Fri, 14 Jul 2023 00:04:06 GMT  
		Size: 1.2 KB (1161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f94b9b520f177b081bf712ba074ba66cad6139b8164f8e18de5be8ebd3ae7382`  
		Last Modified: Fri, 14 Jul 2023 00:08:34 GMT  
		Size: 7.8 MB (7786370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c03838a3679d351be263b09d3a5c6b9c44c73bd67df1a32d00364b15614d8b4c`  
		Last Modified: Fri, 14 Jul 2023 00:08:32 GMT  
		Size: 1.1 KB (1058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3a7169624bc074e90056b7387038bd434dc1bc770b6ac612f0d295d8db6b10f`  
		Last Modified: Fri, 14 Jul 2023 00:08:31 GMT  
		Size: 1.0 KB (1035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30ef31773aef63c527f320ae07bc5b102bd9f4f448f3b8d21c3e339e30db10e1`  
		Last Modified: Fri, 14 Jul 2023 00:08:32 GMT  
		Size: 1.1 KB (1074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.25.5-scratch`

```console
$ docker pull nats-streaming@sha256:2b8205e7d3a87aacdc19ec7b71e3316a44380ef15ab834060826911876394dac
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.25.5-scratch` - linux; amd64

```console
$ docker pull nats-streaming@sha256:0963a4d0a1504acf8b8f5b99fa1f119639a1caff31850eefe83a685fac6820fb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.7 MB (7659749 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:32ad867a381275ce803cc7a4e3007d375908b15c83a75444af3352cfdc72d2eb`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Wed, 21 Jun 2023 01:10:50 GMT
COPY file:670c17c233c7999d9f7b72c2962b221cab4e00da471a75e8679840c939143cfb in /nats-streaming-server 
# Wed, 21 Jun 2023 01:10:50 GMT
EXPOSE 4222 8222
# Wed, 21 Jun 2023 01:10:51 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Wed, 21 Jun 2023 01:10:51 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:b7ff958d406306840566ff165f0c34c6017d44a13d4355d5eb8c6cd152c57d64`  
		Last Modified: Wed, 21 Jun 2023 01:11:25 GMT  
		Size: 7.7 MB (7659749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.25.5-scratch` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:c6adf4bdcf4ca4548a1331f9a5b78accb38369508960b70058ae6f3cfe00ed5d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7311545 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7763bb2699d3b947f45691cca3c382801ad1c0a91b829831fd0999aa54245f66`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Wed, 21 Jun 2023 00:59:07 GMT
COPY file:9bc2f7015ff72f7e91556a01075e89ef8a85a404228874028f7a356e8142e169 in /nats-streaming-server 
# Wed, 21 Jun 2023 00:59:07 GMT
EXPOSE 4222 8222
# Wed, 21 Jun 2023 00:59:07 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Wed, 21 Jun 2023 00:59:08 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:ee4a78724efc3390679e6118a2f2c5993c9075f378bd6a2f0b7f99b50579fb2b`  
		Last Modified: Wed, 21 Jun 2023 00:59:42 GMT  
		Size: 7.3 MB (7311545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.25.5-scratch` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:3ae971fd2fa4bc0a898567aa6a6ea4d4dbae8d4459d81e59a2fab244b4d9c5b0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7304325 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:825e70124556ec89714458bdec5da1ee59baa724df73fa420db3005bfad56c45`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Wed, 21 Jun 2023 01:31:21 GMT
COPY file:07846c068b31699c9c9fe9b535ec7c1dcfbda7a16d7d178a50de1f9541deeebf in /nats-streaming-server 
# Wed, 21 Jun 2023 01:31:21 GMT
EXPOSE 4222 8222
# Wed, 21 Jun 2023 01:31:21 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Wed, 21 Jun 2023 01:31:21 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:039446f9a794527f7060ddd5b9b8a071ffe8816fa5aae791c4bbf01db3656057`  
		Last Modified: Wed, 21 Jun 2023 01:31:55 GMT  
		Size: 7.3 MB (7304325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.25.5-scratch` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:04ef4025a7de920cc90464848b402755e5da72e57bc969aff8859af5429c00a7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.0 MB (7011458 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1627cfd9fc66597d5484a918e734f0595b380583577fd3a532f6228b72db740a`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Wed, 21 Jun 2023 01:11:52 GMT
COPY file:8237d0d59fd3c6b32e52dbff50861a8848f846505c0303e7975e4a5f48ce8de9 in /nats-streaming-server 
# Wed, 21 Jun 2023 01:11:52 GMT
EXPOSE 4222 8222
# Wed, 21 Jun 2023 01:11:52 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Wed, 21 Jun 2023 01:11:52 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:c3b4c14668a8e32e87c6ea3dce4a99716b527ba7f0f4608cbab27184c89832ee`  
		Last Modified: Wed, 21 Jun 2023 01:12:24 GMT  
		Size: 7.0 MB (7011458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.25.5-windowsservercore`

```console
$ docker pull nats-streaming@sha256:f8f306c1324a747d5f42fbd66e59d90ef995c1f82d95a07af46ec637a8fa29ee
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4645; amd64

### `nats-streaming:0.25.5-windowsservercore` - windows version 10.0.17763.4645; amd64

```console
$ docker pull nats-streaming@sha256:e3600f1ee85431963c7c2e4ba9dd422516b7c89203680e9098086f8eee913396
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1948162918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba9d6571d5a398539f54f2d4eb7bbdc753472d33dfb4fa5905ed6a249a5ec33c`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Fri, 07 Jul 2023 08:17:39 GMT
RUN Install update 10.0.17763.4645
# Thu, 13 Jul 2023 22:38:00 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Fri, 14 Jul 2023 00:00:18 GMT
ENV NATS_DOCKERIZED=1
# Fri, 14 Jul 2023 00:04:55 GMT
ENV NATS_STREAMING_SERVER=0.25.5
# Fri, 14 Jul 2023 00:04:56 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.25.5/nats-streaming-server-v0.25.5-windows-amd64.zip
# Fri, 14 Jul 2023 00:04:56 GMT
ENV NATS_STREAMING_SERVER_SHASUM=709b481bfa3537dc7941490365e065554f19c7029830d765ef49e8cd16657b75
# Fri, 14 Jul 2023 00:05:52 GMT
RUN Set-PSDebug -Trace 2
# Fri, 14 Jul 2023 00:07:33 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Fri, 14 Jul 2023 00:07:34 GMT
EXPOSE 4222 8222
# Fri, 14 Jul 2023 00:07:35 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Fri, 14 Jul 2023 00:07:36 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e36dba1ee29cd36713c8785a5de7dd2a487244d734ed4c5e7b0a6890bffb806e`  
		Last Modified: Tue, 11 Jul 2023 18:27:38 GMT  
		Size: 289.1 MB (289068746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48b452db6d50a62b6e0e8dadb19715cfcf62cf73e54b5d3bac96621c1093673c`  
		Last Modified: Thu, 13 Jul 2023 23:25:18 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20f8ca4b8d322e27c827c0ba667217bc04a39b69f5f483d5f2f9726e6d42522e`  
		Last Modified: Fri, 14 Jul 2023 00:03:50 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18679ad5f87511b5572cc2ff53e239532dca4c70a413dcf8fc9f8aca97bf4f96`  
		Last Modified: Fri, 14 Jul 2023 00:08:19 GMT  
		Size: 1.3 KB (1279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9c5202984226bceb34a191f9e86a9b84106eebcd4c6a4e47314b707ac610f38`  
		Last Modified: Fri, 14 Jul 2023 00:08:19 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bca3f1baea6a69d419c0fce9341dfac5cbe256fdb7eb9415fe4f1c4edf1a7b93`  
		Last Modified: Fri, 14 Jul 2023 00:08:18 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4631c84b931d3f1ee529f0423fa3188ea9e48d8af0089a9887fa992becd65312`  
		Last Modified: Fri, 14 Jul 2023 00:08:17 GMT  
		Size: 226.1 KB (226123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a195df7f50ec1e109468319f7e85f27d494af37f9eceb4586c2abd45b7798ec9`  
		Last Modified: Fri, 14 Jul 2023 00:08:19 GMT  
		Size: 8.2 MB (8237038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7271bd8c5599f12857ee3ed75550b08dc3638819425f32fd3ab0b104dda1e0d8`  
		Last Modified: Fri, 14 Jul 2023 00:08:17 GMT  
		Size: 1.3 KB (1324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2001f0adacd1483a7214db132b80267a2d9a728c9099b49a73bffec74f4c4c47`  
		Last Modified: Fri, 14 Jul 2023 00:08:17 GMT  
		Size: 1.3 KB (1313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:076f3743d3f1ac915066251cf19292b7e95d2b21d98f6d6fa723ced8cf864026`  
		Last Modified: Fri, 14 Jul 2023 00:08:17 GMT  
		Size: 1.3 KB (1335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.25.5-windowsservercore-1809`

```console
$ docker pull nats-streaming@sha256:f8f306c1324a747d5f42fbd66e59d90ef995c1f82d95a07af46ec637a8fa29ee
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4645; amd64

### `nats-streaming:0.25.5-windowsservercore-1809` - windows version 10.0.17763.4645; amd64

```console
$ docker pull nats-streaming@sha256:e3600f1ee85431963c7c2e4ba9dd422516b7c89203680e9098086f8eee913396
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1948162918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba9d6571d5a398539f54f2d4eb7bbdc753472d33dfb4fa5905ed6a249a5ec33c`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Fri, 07 Jul 2023 08:17:39 GMT
RUN Install update 10.0.17763.4645
# Thu, 13 Jul 2023 22:38:00 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Fri, 14 Jul 2023 00:00:18 GMT
ENV NATS_DOCKERIZED=1
# Fri, 14 Jul 2023 00:04:55 GMT
ENV NATS_STREAMING_SERVER=0.25.5
# Fri, 14 Jul 2023 00:04:56 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.25.5/nats-streaming-server-v0.25.5-windows-amd64.zip
# Fri, 14 Jul 2023 00:04:56 GMT
ENV NATS_STREAMING_SERVER_SHASUM=709b481bfa3537dc7941490365e065554f19c7029830d765ef49e8cd16657b75
# Fri, 14 Jul 2023 00:05:52 GMT
RUN Set-PSDebug -Trace 2
# Fri, 14 Jul 2023 00:07:33 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Fri, 14 Jul 2023 00:07:34 GMT
EXPOSE 4222 8222
# Fri, 14 Jul 2023 00:07:35 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Fri, 14 Jul 2023 00:07:36 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e36dba1ee29cd36713c8785a5de7dd2a487244d734ed4c5e7b0a6890bffb806e`  
		Last Modified: Tue, 11 Jul 2023 18:27:38 GMT  
		Size: 289.1 MB (289068746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48b452db6d50a62b6e0e8dadb19715cfcf62cf73e54b5d3bac96621c1093673c`  
		Last Modified: Thu, 13 Jul 2023 23:25:18 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20f8ca4b8d322e27c827c0ba667217bc04a39b69f5f483d5f2f9726e6d42522e`  
		Last Modified: Fri, 14 Jul 2023 00:03:50 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18679ad5f87511b5572cc2ff53e239532dca4c70a413dcf8fc9f8aca97bf4f96`  
		Last Modified: Fri, 14 Jul 2023 00:08:19 GMT  
		Size: 1.3 KB (1279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9c5202984226bceb34a191f9e86a9b84106eebcd4c6a4e47314b707ac610f38`  
		Last Modified: Fri, 14 Jul 2023 00:08:19 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bca3f1baea6a69d419c0fce9341dfac5cbe256fdb7eb9415fe4f1c4edf1a7b93`  
		Last Modified: Fri, 14 Jul 2023 00:08:18 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4631c84b931d3f1ee529f0423fa3188ea9e48d8af0089a9887fa992becd65312`  
		Last Modified: Fri, 14 Jul 2023 00:08:17 GMT  
		Size: 226.1 KB (226123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a195df7f50ec1e109468319f7e85f27d494af37f9eceb4586c2abd45b7798ec9`  
		Last Modified: Fri, 14 Jul 2023 00:08:19 GMT  
		Size: 8.2 MB (8237038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7271bd8c5599f12857ee3ed75550b08dc3638819425f32fd3ab0b104dda1e0d8`  
		Last Modified: Fri, 14 Jul 2023 00:08:17 GMT  
		Size: 1.3 KB (1324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2001f0adacd1483a7214db132b80267a2d9a728c9099b49a73bffec74f4c4c47`  
		Last Modified: Fri, 14 Jul 2023 00:08:17 GMT  
		Size: 1.3 KB (1313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:076f3743d3f1ac915066251cf19292b7e95d2b21d98f6d6fa723ced8cf864026`  
		Last Modified: Fri, 14 Jul 2023 00:08:17 GMT  
		Size: 1.3 KB (1335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:alpine`

```console
$ docker pull nats-streaming@sha256:c9e97ca2eb081301837053ea04e6a1dfc4fedacacf21a10b540693546de6c733
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:alpine` - linux; amd64

```console
$ docker pull nats-streaming@sha256:6abf524d6062038a5c5c66c0733592ac2d3151abbd8b423facb5f4f575fbabda
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.3 MB (11344002 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:259306c401d301ff49ceac471b001513aeb8ec5ce27d8e92b4a6c0c4a7be30f3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 14 Jun 2023 20:41:58 GMT
ADD file:1da756d12551a0e3e793e02ef87432d69d4968937bd11bed0af215db19dd94cd in / 
# Wed, 14 Jun 2023 20:41:59 GMT
CMD ["/bin/sh"]
# Wed, 21 Jun 2023 01:10:41 GMT
ENV NATS_STREAMING_SERVER=0.25.5
# Wed, 21 Jun 2023 01:10:43 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='937af3f9cdbfe3cb4648cf8c8f505dded2cc175d59ba10e13ec71d1c04e61bf2' ;; 		armhf) natsArch='arm6'; sha256='5bd3a0456054505741b05e5d03acb9f7a5de97cf3ea20cd52d31edbae1c387ea' ;; 		armv7) natsArch='arm7'; sha256='0e643e9881cf3acf3313f84853451d1c4a1e731bc8599d223a40042f9c0c7285' ;; 		x86_64) natsArch='amd64'; sha256='22762f4d0ccfc75947096a14e09566b816113e125a3d39f7914a0c332bee25a7' ;; 		x86) natsArch='386'; sha256='92d8d4460f538883c78e67a334b23b2317e4fe58d46e4fdbbef8b4c09c7b97ae' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Wed, 21 Jun 2023 01:10:43 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Wed, 21 Jun 2023 01:10:44 GMT
EXPOSE 4222 8222
# Wed, 21 Jun 2023 01:10:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Jun 2023 01:10:44 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:31e352740f534f9ad170f75378a84fe453d6156e40700b882d737a8f4a6988a3`  
		Last Modified: Wed, 14 Jun 2023 20:42:26 GMT  
		Size: 3.4 MB (3397879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0ccb9db0d77fa25becf9aa3c73f0a091378e47d9a8c0d87114fe3ca75b17483`  
		Last Modified: Wed, 21 Jun 2023 01:11:09 GMT  
		Size: 7.9 MB (7945701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56d62dc9de67132e108b1f8b40907849093f018255907030abdb3fc7b94904a9`  
		Last Modified: Wed, 21 Jun 2023 01:11:07 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:df08adb5a35cd347a0f1d96e733b0ba3b963a100fe08534f0e3a7a739f7453d2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.7 MB (10745511 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e879e367a39ad7817ae00eaf4a01036cc223cf63db3d0b10455e54a4fcf76bc3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Mon, 07 Aug 2023 19:49:14 GMT
ADD file:9882e99e5f94ab2db05c029648ac5be7cf0f063a8701394fcbb543a7ef5d4b90 in / 
# Mon, 07 Aug 2023 19:49:15 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 20:44:50 GMT
ENV NATS_STREAMING_SERVER=0.25.5
# Tue, 08 Aug 2023 20:44:52 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='937af3f9cdbfe3cb4648cf8c8f505dded2cc175d59ba10e13ec71d1c04e61bf2' ;; 		armhf) natsArch='arm6'; sha256='5bd3a0456054505741b05e5d03acb9f7a5de97cf3ea20cd52d31edbae1c387ea' ;; 		armv7) natsArch='arm7'; sha256='0e643e9881cf3acf3313f84853451d1c4a1e731bc8599d223a40042f9c0c7285' ;; 		x86_64) natsArch='amd64'; sha256='22762f4d0ccfc75947096a14e09566b816113e125a3d39f7914a0c332bee25a7' ;; 		x86) natsArch='386'; sha256='92d8d4460f538883c78e67a334b23b2317e4fe58d46e4fdbbef8b4c09c7b97ae' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Tue, 08 Aug 2023 20:44:53 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Tue, 08 Aug 2023 20:44:53 GMT
EXPOSE 4222 8222
# Tue, 08 Aug 2023 20:44:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 08 Aug 2023 20:44:53 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:af09961d4a43b504efc76e38b50918977c28be73eeb8b926247783a00e8b9f2f`  
		Last Modified: Mon, 07 Aug 2023 19:49:38 GMT  
		Size: 3.1 MB (3144809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db57a023cb1e641cc4e410d847ed348704fa48f194e6e04feb97859ea8263399`  
		Last Modified: Tue, 08 Aug 2023 20:45:13 GMT  
		Size: 7.6 MB (7600282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d00d13e6c7ccee53d63384bf85378713efa9cd84cb8817b81ddcb19ab83106e3`  
		Last Modified: Tue, 08 Aug 2023 20:45:11 GMT  
		Size: 420.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:8b69faa2f13f8bb2769c9ca014cfb884a6f581175bf1ad9baaa59b914ef3a7fe
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.5 MB (10488008 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6b906477dbd127990b39bdff954cd4495c0027ae495dad6ab5c740cff11c8a4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Mon, 07 Aug 2023 19:57:25 GMT
ADD file:e3f56488d3d3bb67729714db13ddadf6652e7efb5281cfc7010d3e71f9d6607f in / 
# Mon, 07 Aug 2023 19:57:25 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 02:15:20 GMT
ENV NATS_STREAMING_SERVER=0.25.5
# Tue, 08 Aug 2023 02:15:23 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='937af3f9cdbfe3cb4648cf8c8f505dded2cc175d59ba10e13ec71d1c04e61bf2' ;; 		armhf) natsArch='arm6'; sha256='5bd3a0456054505741b05e5d03acb9f7a5de97cf3ea20cd52d31edbae1c387ea' ;; 		armv7) natsArch='arm7'; sha256='0e643e9881cf3acf3313f84853451d1c4a1e731bc8599d223a40042f9c0c7285' ;; 		x86_64) natsArch='amd64'; sha256='22762f4d0ccfc75947096a14e09566b816113e125a3d39f7914a0c332bee25a7' ;; 		x86) natsArch='386'; sha256='92d8d4460f538883c78e67a334b23b2317e4fe58d46e4fdbbef8b4c09c7b97ae' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Tue, 08 Aug 2023 02:15:23 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Tue, 08 Aug 2023 02:15:23 GMT
EXPOSE 4222 8222
# Tue, 08 Aug 2023 02:15:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 08 Aug 2023 02:15:24 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:f8dec92eec42224ef9e6ca9c6207ea6b9195dcf93d06bd5ceff0f814b62bf064`  
		Last Modified: Mon, 07 Aug 2023 19:57:55 GMT  
		Size: 2.9 MB (2899480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e18324f789c9a02a3fb3992cee161f01f2d80d6396a0eb54b83956b93f18e24b`  
		Last Modified: Tue, 08 Aug 2023 02:15:50 GMT  
		Size: 7.6 MB (7588109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bff0b4480470ca012849b4227c612a9a456bed7a67117efc5fb5c5a737d17e9`  
		Last Modified: Tue, 08 Aug 2023 02:15:48 GMT  
		Size: 419.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:9f7fa008b1524911fee4a485f955408c7b911611179fdf120a2bb89f3323cdfa
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.6 MB (10629737 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5be4dd1beeb3895e9906e2866ca807b53f3b5cbc33598ed378b76126ded32d8d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 14 Jun 2023 20:48:58 GMT
ADD file:289c2fac17119508ced527225d445747cd177111b4a0018a6b04948ecb3b5e29 in / 
# Wed, 14 Jun 2023 20:48:58 GMT
CMD ["/bin/sh"]
# Wed, 21 Jun 2023 01:11:44 GMT
ENV NATS_STREAMING_SERVER=0.25.5
# Wed, 21 Jun 2023 01:11:46 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='937af3f9cdbfe3cb4648cf8c8f505dded2cc175d59ba10e13ec71d1c04e61bf2' ;; 		armhf) natsArch='arm6'; sha256='5bd3a0456054505741b05e5d03acb9f7a5de97cf3ea20cd52d31edbae1c387ea' ;; 		armv7) natsArch='arm7'; sha256='0e643e9881cf3acf3313f84853451d1c4a1e731bc8599d223a40042f9c0c7285' ;; 		x86_64) natsArch='amd64'; sha256='22762f4d0ccfc75947096a14e09566b816113e125a3d39f7914a0c332bee25a7' ;; 		x86) natsArch='386'; sha256='92d8d4460f538883c78e67a334b23b2317e4fe58d46e4fdbbef8b4c09c7b97ae' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Wed, 21 Jun 2023 01:11:46 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Wed, 21 Jun 2023 01:11:46 GMT
EXPOSE 4222 8222
# Wed, 21 Jun 2023 01:11:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Jun 2023 01:11:46 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:8c6d1654570f041603f4cef49c320c8f6f3e401324913009d92a19132cbf1ac0`  
		Last Modified: Wed, 14 Jun 2023 20:49:23 GMT  
		Size: 3.3 MB (3329251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3146f74e4cb95e61d4f251594c3330ad0f9c85345a1b97bce44ab0446ee59269`  
		Last Modified: Wed, 21 Jun 2023 01:12:08 GMT  
		Size: 7.3 MB (7300064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:775fc9bc0a0519e7fe2cd9656617079a95fd7919b285649d10cf4f76b7e89b49`  
		Last Modified: Wed, 21 Jun 2023 01:12:07 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:alpine3.18`

```console
$ docker pull nats-streaming@sha256:c9e97ca2eb081301837053ea04e6a1dfc4fedacacf21a10b540693546de6c733
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:alpine3.18` - linux; amd64

```console
$ docker pull nats-streaming@sha256:6abf524d6062038a5c5c66c0733592ac2d3151abbd8b423facb5f4f575fbabda
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.3 MB (11344002 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:259306c401d301ff49ceac471b001513aeb8ec5ce27d8e92b4a6c0c4a7be30f3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 14 Jun 2023 20:41:58 GMT
ADD file:1da756d12551a0e3e793e02ef87432d69d4968937bd11bed0af215db19dd94cd in / 
# Wed, 14 Jun 2023 20:41:59 GMT
CMD ["/bin/sh"]
# Wed, 21 Jun 2023 01:10:41 GMT
ENV NATS_STREAMING_SERVER=0.25.5
# Wed, 21 Jun 2023 01:10:43 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='937af3f9cdbfe3cb4648cf8c8f505dded2cc175d59ba10e13ec71d1c04e61bf2' ;; 		armhf) natsArch='arm6'; sha256='5bd3a0456054505741b05e5d03acb9f7a5de97cf3ea20cd52d31edbae1c387ea' ;; 		armv7) natsArch='arm7'; sha256='0e643e9881cf3acf3313f84853451d1c4a1e731bc8599d223a40042f9c0c7285' ;; 		x86_64) natsArch='amd64'; sha256='22762f4d0ccfc75947096a14e09566b816113e125a3d39f7914a0c332bee25a7' ;; 		x86) natsArch='386'; sha256='92d8d4460f538883c78e67a334b23b2317e4fe58d46e4fdbbef8b4c09c7b97ae' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Wed, 21 Jun 2023 01:10:43 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Wed, 21 Jun 2023 01:10:44 GMT
EXPOSE 4222 8222
# Wed, 21 Jun 2023 01:10:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Jun 2023 01:10:44 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:31e352740f534f9ad170f75378a84fe453d6156e40700b882d737a8f4a6988a3`  
		Last Modified: Wed, 14 Jun 2023 20:42:26 GMT  
		Size: 3.4 MB (3397879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0ccb9db0d77fa25becf9aa3c73f0a091378e47d9a8c0d87114fe3ca75b17483`  
		Last Modified: Wed, 21 Jun 2023 01:11:09 GMT  
		Size: 7.9 MB (7945701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56d62dc9de67132e108b1f8b40907849093f018255907030abdb3fc7b94904a9`  
		Last Modified: Wed, 21 Jun 2023 01:11:07 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine3.18` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:df08adb5a35cd347a0f1d96e733b0ba3b963a100fe08534f0e3a7a739f7453d2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.7 MB (10745511 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e879e367a39ad7817ae00eaf4a01036cc223cf63db3d0b10455e54a4fcf76bc3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Mon, 07 Aug 2023 19:49:14 GMT
ADD file:9882e99e5f94ab2db05c029648ac5be7cf0f063a8701394fcbb543a7ef5d4b90 in / 
# Mon, 07 Aug 2023 19:49:15 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 20:44:50 GMT
ENV NATS_STREAMING_SERVER=0.25.5
# Tue, 08 Aug 2023 20:44:52 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='937af3f9cdbfe3cb4648cf8c8f505dded2cc175d59ba10e13ec71d1c04e61bf2' ;; 		armhf) natsArch='arm6'; sha256='5bd3a0456054505741b05e5d03acb9f7a5de97cf3ea20cd52d31edbae1c387ea' ;; 		armv7) natsArch='arm7'; sha256='0e643e9881cf3acf3313f84853451d1c4a1e731bc8599d223a40042f9c0c7285' ;; 		x86_64) natsArch='amd64'; sha256='22762f4d0ccfc75947096a14e09566b816113e125a3d39f7914a0c332bee25a7' ;; 		x86) natsArch='386'; sha256='92d8d4460f538883c78e67a334b23b2317e4fe58d46e4fdbbef8b4c09c7b97ae' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Tue, 08 Aug 2023 20:44:53 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Tue, 08 Aug 2023 20:44:53 GMT
EXPOSE 4222 8222
# Tue, 08 Aug 2023 20:44:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 08 Aug 2023 20:44:53 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:af09961d4a43b504efc76e38b50918977c28be73eeb8b926247783a00e8b9f2f`  
		Last Modified: Mon, 07 Aug 2023 19:49:38 GMT  
		Size: 3.1 MB (3144809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db57a023cb1e641cc4e410d847ed348704fa48f194e6e04feb97859ea8263399`  
		Last Modified: Tue, 08 Aug 2023 20:45:13 GMT  
		Size: 7.6 MB (7600282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d00d13e6c7ccee53d63384bf85378713efa9cd84cb8817b81ddcb19ab83106e3`  
		Last Modified: Tue, 08 Aug 2023 20:45:11 GMT  
		Size: 420.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine3.18` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:8b69faa2f13f8bb2769c9ca014cfb884a6f581175bf1ad9baaa59b914ef3a7fe
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.5 MB (10488008 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6b906477dbd127990b39bdff954cd4495c0027ae495dad6ab5c740cff11c8a4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Mon, 07 Aug 2023 19:57:25 GMT
ADD file:e3f56488d3d3bb67729714db13ddadf6652e7efb5281cfc7010d3e71f9d6607f in / 
# Mon, 07 Aug 2023 19:57:25 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 02:15:20 GMT
ENV NATS_STREAMING_SERVER=0.25.5
# Tue, 08 Aug 2023 02:15:23 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='937af3f9cdbfe3cb4648cf8c8f505dded2cc175d59ba10e13ec71d1c04e61bf2' ;; 		armhf) natsArch='arm6'; sha256='5bd3a0456054505741b05e5d03acb9f7a5de97cf3ea20cd52d31edbae1c387ea' ;; 		armv7) natsArch='arm7'; sha256='0e643e9881cf3acf3313f84853451d1c4a1e731bc8599d223a40042f9c0c7285' ;; 		x86_64) natsArch='amd64'; sha256='22762f4d0ccfc75947096a14e09566b816113e125a3d39f7914a0c332bee25a7' ;; 		x86) natsArch='386'; sha256='92d8d4460f538883c78e67a334b23b2317e4fe58d46e4fdbbef8b4c09c7b97ae' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Tue, 08 Aug 2023 02:15:23 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Tue, 08 Aug 2023 02:15:23 GMT
EXPOSE 4222 8222
# Tue, 08 Aug 2023 02:15:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 08 Aug 2023 02:15:24 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:f8dec92eec42224ef9e6ca9c6207ea6b9195dcf93d06bd5ceff0f814b62bf064`  
		Last Modified: Mon, 07 Aug 2023 19:57:55 GMT  
		Size: 2.9 MB (2899480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e18324f789c9a02a3fb3992cee161f01f2d80d6396a0eb54b83956b93f18e24b`  
		Last Modified: Tue, 08 Aug 2023 02:15:50 GMT  
		Size: 7.6 MB (7588109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bff0b4480470ca012849b4227c612a9a456bed7a67117efc5fb5c5a737d17e9`  
		Last Modified: Tue, 08 Aug 2023 02:15:48 GMT  
		Size: 419.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine3.18` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:9f7fa008b1524911fee4a485f955408c7b911611179fdf120a2bb89f3323cdfa
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.6 MB (10629737 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5be4dd1beeb3895e9906e2866ca807b53f3b5cbc33598ed378b76126ded32d8d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 14 Jun 2023 20:48:58 GMT
ADD file:289c2fac17119508ced527225d445747cd177111b4a0018a6b04948ecb3b5e29 in / 
# Wed, 14 Jun 2023 20:48:58 GMT
CMD ["/bin/sh"]
# Wed, 21 Jun 2023 01:11:44 GMT
ENV NATS_STREAMING_SERVER=0.25.5
# Wed, 21 Jun 2023 01:11:46 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='937af3f9cdbfe3cb4648cf8c8f505dded2cc175d59ba10e13ec71d1c04e61bf2' ;; 		armhf) natsArch='arm6'; sha256='5bd3a0456054505741b05e5d03acb9f7a5de97cf3ea20cd52d31edbae1c387ea' ;; 		armv7) natsArch='arm7'; sha256='0e643e9881cf3acf3313f84853451d1c4a1e731bc8599d223a40042f9c0c7285' ;; 		x86_64) natsArch='amd64'; sha256='22762f4d0ccfc75947096a14e09566b816113e125a3d39f7914a0c332bee25a7' ;; 		x86) natsArch='386'; sha256='92d8d4460f538883c78e67a334b23b2317e4fe58d46e4fdbbef8b4c09c7b97ae' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Wed, 21 Jun 2023 01:11:46 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Wed, 21 Jun 2023 01:11:46 GMT
EXPOSE 4222 8222
# Wed, 21 Jun 2023 01:11:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Jun 2023 01:11:46 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:8c6d1654570f041603f4cef49c320c8f6f3e401324913009d92a19132cbf1ac0`  
		Last Modified: Wed, 14 Jun 2023 20:49:23 GMT  
		Size: 3.3 MB (3329251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3146f74e4cb95e61d4f251594c3330ad0f9c85345a1b97bce44ab0446ee59269`  
		Last Modified: Wed, 21 Jun 2023 01:12:08 GMT  
		Size: 7.3 MB (7300064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:775fc9bc0a0519e7fe2cd9656617079a95fd7919b285649d10cf4f76b7e89b49`  
		Last Modified: Wed, 21 Jun 2023 01:12:07 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:latest`

```console
$ docker pull nats-streaming@sha256:1eed8c2ef0f8b6e0c7264013e3f64f7f2a75195827fce558fde4d277bfcb4b7a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.4645; amd64

### `nats-streaming:latest` - linux; amd64

```console
$ docker pull nats-streaming@sha256:0963a4d0a1504acf8b8f5b99fa1f119639a1caff31850eefe83a685fac6820fb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.7 MB (7659749 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:32ad867a381275ce803cc7a4e3007d375908b15c83a75444af3352cfdc72d2eb`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Wed, 21 Jun 2023 01:10:50 GMT
COPY file:670c17c233c7999d9f7b72c2962b221cab4e00da471a75e8679840c939143cfb in /nats-streaming-server 
# Wed, 21 Jun 2023 01:10:50 GMT
EXPOSE 4222 8222
# Wed, 21 Jun 2023 01:10:51 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Wed, 21 Jun 2023 01:10:51 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:b7ff958d406306840566ff165f0c34c6017d44a13d4355d5eb8c6cd152c57d64`  
		Last Modified: Wed, 21 Jun 2023 01:11:25 GMT  
		Size: 7.7 MB (7659749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:latest` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:c6adf4bdcf4ca4548a1331f9a5b78accb38369508960b70058ae6f3cfe00ed5d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7311545 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7763bb2699d3b947f45691cca3c382801ad1c0a91b829831fd0999aa54245f66`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Wed, 21 Jun 2023 00:59:07 GMT
COPY file:9bc2f7015ff72f7e91556a01075e89ef8a85a404228874028f7a356e8142e169 in /nats-streaming-server 
# Wed, 21 Jun 2023 00:59:07 GMT
EXPOSE 4222 8222
# Wed, 21 Jun 2023 00:59:07 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Wed, 21 Jun 2023 00:59:08 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:ee4a78724efc3390679e6118a2f2c5993c9075f378bd6a2f0b7f99b50579fb2b`  
		Last Modified: Wed, 21 Jun 2023 00:59:42 GMT  
		Size: 7.3 MB (7311545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:latest` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:3ae971fd2fa4bc0a898567aa6a6ea4d4dbae8d4459d81e59a2fab244b4d9c5b0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7304325 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:825e70124556ec89714458bdec5da1ee59baa724df73fa420db3005bfad56c45`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Wed, 21 Jun 2023 01:31:21 GMT
COPY file:07846c068b31699c9c9fe9b535ec7c1dcfbda7a16d7d178a50de1f9541deeebf in /nats-streaming-server 
# Wed, 21 Jun 2023 01:31:21 GMT
EXPOSE 4222 8222
# Wed, 21 Jun 2023 01:31:21 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Wed, 21 Jun 2023 01:31:21 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:039446f9a794527f7060ddd5b9b8a071ffe8816fa5aae791c4bbf01db3656057`  
		Last Modified: Wed, 21 Jun 2023 01:31:55 GMT  
		Size: 7.3 MB (7304325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:latest` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:04ef4025a7de920cc90464848b402755e5da72e57bc969aff8859af5429c00a7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.0 MB (7011458 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1627cfd9fc66597d5484a918e734f0595b380583577fd3a532f6228b72db740a`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Wed, 21 Jun 2023 01:11:52 GMT
COPY file:8237d0d59fd3c6b32e52dbff50861a8848f846505c0303e7975e4a5f48ce8de9 in /nats-streaming-server 
# Wed, 21 Jun 2023 01:11:52 GMT
EXPOSE 4222 8222
# Wed, 21 Jun 2023 01:11:52 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Wed, 21 Jun 2023 01:11:52 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:c3b4c14668a8e32e87c6ea3dce4a99716b527ba7f0f4608cbab27184c89832ee`  
		Last Modified: Wed, 21 Jun 2023 01:12:24 GMT  
		Size: 7.0 MB (7011458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:latest` - windows version 10.0.17763.4645; amd64

```console
$ docker pull nats-streaming@sha256:5c39267b2e159ad82e792287b1086208f57dbf20ef18e40b553f3b377b337545
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.2 MB (112198939 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ef72ff049bb8cd1e4d7c65b5e46d477eccc664570d1a61e14b52bfc1faaa98f`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Fri, 07 Jul 2023 07:42:59 GMT
RUN Apply image 10.0.17763.4645
# Fri, 14 Jul 2023 00:03:16 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 14 Jul 2023 00:07:54 GMT
RUN cmd /S /C #(nop) COPY file:0e2c8ba21e47adc90962b46928c928315462bcddaefcbc01f98113f4f66cda4a in C:\nats-streaming-server.exe 
# Fri, 14 Jul 2023 00:07:55 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Fri, 14 Jul 2023 00:07:56 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Fri, 14 Jul 2023 00:07:57 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:5c5b06ba65934bcf850a1a54ecf4b3da34d3e6d6c8e90dbc897719c3ea377c8a`  
		Last Modified: Tue, 11 Jul 2023 17:31:37 GMT  
		Size: 104.4 MB (104408241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff4bad9bf846d07362d8295a4479f8f2965dfb5934a9a032b335ce3cb086bdf7`  
		Last Modified: Fri, 14 Jul 2023 00:04:06 GMT  
		Size: 1.2 KB (1161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f94b9b520f177b081bf712ba074ba66cad6139b8164f8e18de5be8ebd3ae7382`  
		Last Modified: Fri, 14 Jul 2023 00:08:34 GMT  
		Size: 7.8 MB (7786370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c03838a3679d351be263b09d3a5c6b9c44c73bd67df1a32d00364b15614d8b4c`  
		Last Modified: Fri, 14 Jul 2023 00:08:32 GMT  
		Size: 1.1 KB (1058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3a7169624bc074e90056b7387038bd434dc1bc770b6ac612f0d295d8db6b10f`  
		Last Modified: Fri, 14 Jul 2023 00:08:31 GMT  
		Size: 1.0 KB (1035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30ef31773aef63c527f320ae07bc5b102bd9f4f448f3b8d21c3e339e30db10e1`  
		Last Modified: Fri, 14 Jul 2023 00:08:32 GMT  
		Size: 1.1 KB (1074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:linux`

```console
$ docker pull nats-streaming@sha256:2b8205e7d3a87aacdc19ec7b71e3316a44380ef15ab834060826911876394dac
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:linux` - linux; amd64

```console
$ docker pull nats-streaming@sha256:0963a4d0a1504acf8b8f5b99fa1f119639a1caff31850eefe83a685fac6820fb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.7 MB (7659749 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:32ad867a381275ce803cc7a4e3007d375908b15c83a75444af3352cfdc72d2eb`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Wed, 21 Jun 2023 01:10:50 GMT
COPY file:670c17c233c7999d9f7b72c2962b221cab4e00da471a75e8679840c939143cfb in /nats-streaming-server 
# Wed, 21 Jun 2023 01:10:50 GMT
EXPOSE 4222 8222
# Wed, 21 Jun 2023 01:10:51 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Wed, 21 Jun 2023 01:10:51 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:b7ff958d406306840566ff165f0c34c6017d44a13d4355d5eb8c6cd152c57d64`  
		Last Modified: Wed, 21 Jun 2023 01:11:25 GMT  
		Size: 7.7 MB (7659749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:linux` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:c6adf4bdcf4ca4548a1331f9a5b78accb38369508960b70058ae6f3cfe00ed5d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7311545 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7763bb2699d3b947f45691cca3c382801ad1c0a91b829831fd0999aa54245f66`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Wed, 21 Jun 2023 00:59:07 GMT
COPY file:9bc2f7015ff72f7e91556a01075e89ef8a85a404228874028f7a356e8142e169 in /nats-streaming-server 
# Wed, 21 Jun 2023 00:59:07 GMT
EXPOSE 4222 8222
# Wed, 21 Jun 2023 00:59:07 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Wed, 21 Jun 2023 00:59:08 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:ee4a78724efc3390679e6118a2f2c5993c9075f378bd6a2f0b7f99b50579fb2b`  
		Last Modified: Wed, 21 Jun 2023 00:59:42 GMT  
		Size: 7.3 MB (7311545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:linux` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:3ae971fd2fa4bc0a898567aa6a6ea4d4dbae8d4459d81e59a2fab244b4d9c5b0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7304325 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:825e70124556ec89714458bdec5da1ee59baa724df73fa420db3005bfad56c45`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Wed, 21 Jun 2023 01:31:21 GMT
COPY file:07846c068b31699c9c9fe9b535ec7c1dcfbda7a16d7d178a50de1f9541deeebf in /nats-streaming-server 
# Wed, 21 Jun 2023 01:31:21 GMT
EXPOSE 4222 8222
# Wed, 21 Jun 2023 01:31:21 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Wed, 21 Jun 2023 01:31:21 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:039446f9a794527f7060ddd5b9b8a071ffe8816fa5aae791c4bbf01db3656057`  
		Last Modified: Wed, 21 Jun 2023 01:31:55 GMT  
		Size: 7.3 MB (7304325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:linux` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:04ef4025a7de920cc90464848b402755e5da72e57bc969aff8859af5429c00a7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.0 MB (7011458 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1627cfd9fc66597d5484a918e734f0595b380583577fd3a532f6228b72db740a`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Wed, 21 Jun 2023 01:11:52 GMT
COPY file:8237d0d59fd3c6b32e52dbff50861a8848f846505c0303e7975e4a5f48ce8de9 in /nats-streaming-server 
# Wed, 21 Jun 2023 01:11:52 GMT
EXPOSE 4222 8222
# Wed, 21 Jun 2023 01:11:52 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Wed, 21 Jun 2023 01:11:52 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:c3b4c14668a8e32e87c6ea3dce4a99716b527ba7f0f4608cbab27184c89832ee`  
		Last Modified: Wed, 21 Jun 2023 01:12:24 GMT  
		Size: 7.0 MB (7011458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:nanoserver`

```console
$ docker pull nats-streaming@sha256:2ea85a60361e0774ce1913ef12baa8fc87bfa4a837a811e89a0a32988b40ed14
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4645; amd64

### `nats-streaming:nanoserver` - windows version 10.0.17763.4645; amd64

```console
$ docker pull nats-streaming@sha256:5c39267b2e159ad82e792287b1086208f57dbf20ef18e40b553f3b377b337545
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.2 MB (112198939 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ef72ff049bb8cd1e4d7c65b5e46d477eccc664570d1a61e14b52bfc1faaa98f`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Fri, 07 Jul 2023 07:42:59 GMT
RUN Apply image 10.0.17763.4645
# Fri, 14 Jul 2023 00:03:16 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 14 Jul 2023 00:07:54 GMT
RUN cmd /S /C #(nop) COPY file:0e2c8ba21e47adc90962b46928c928315462bcddaefcbc01f98113f4f66cda4a in C:\nats-streaming-server.exe 
# Fri, 14 Jul 2023 00:07:55 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Fri, 14 Jul 2023 00:07:56 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Fri, 14 Jul 2023 00:07:57 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:5c5b06ba65934bcf850a1a54ecf4b3da34d3e6d6c8e90dbc897719c3ea377c8a`  
		Last Modified: Tue, 11 Jul 2023 17:31:37 GMT  
		Size: 104.4 MB (104408241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff4bad9bf846d07362d8295a4479f8f2965dfb5934a9a032b335ce3cb086bdf7`  
		Last Modified: Fri, 14 Jul 2023 00:04:06 GMT  
		Size: 1.2 KB (1161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f94b9b520f177b081bf712ba074ba66cad6139b8164f8e18de5be8ebd3ae7382`  
		Last Modified: Fri, 14 Jul 2023 00:08:34 GMT  
		Size: 7.8 MB (7786370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c03838a3679d351be263b09d3a5c6b9c44c73bd67df1a32d00364b15614d8b4c`  
		Last Modified: Fri, 14 Jul 2023 00:08:32 GMT  
		Size: 1.1 KB (1058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3a7169624bc074e90056b7387038bd434dc1bc770b6ac612f0d295d8db6b10f`  
		Last Modified: Fri, 14 Jul 2023 00:08:31 GMT  
		Size: 1.0 KB (1035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30ef31773aef63c527f320ae07bc5b102bd9f4f448f3b8d21c3e339e30db10e1`  
		Last Modified: Fri, 14 Jul 2023 00:08:32 GMT  
		Size: 1.1 KB (1074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:nanoserver-1809`

```console
$ docker pull nats-streaming@sha256:2ea85a60361e0774ce1913ef12baa8fc87bfa4a837a811e89a0a32988b40ed14
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4645; amd64

### `nats-streaming:nanoserver-1809` - windows version 10.0.17763.4645; amd64

```console
$ docker pull nats-streaming@sha256:5c39267b2e159ad82e792287b1086208f57dbf20ef18e40b553f3b377b337545
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.2 MB (112198939 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ef72ff049bb8cd1e4d7c65b5e46d477eccc664570d1a61e14b52bfc1faaa98f`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Fri, 07 Jul 2023 07:42:59 GMT
RUN Apply image 10.0.17763.4645
# Fri, 14 Jul 2023 00:03:16 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 14 Jul 2023 00:07:54 GMT
RUN cmd /S /C #(nop) COPY file:0e2c8ba21e47adc90962b46928c928315462bcddaefcbc01f98113f4f66cda4a in C:\nats-streaming-server.exe 
# Fri, 14 Jul 2023 00:07:55 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Fri, 14 Jul 2023 00:07:56 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Fri, 14 Jul 2023 00:07:57 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:5c5b06ba65934bcf850a1a54ecf4b3da34d3e6d6c8e90dbc897719c3ea377c8a`  
		Last Modified: Tue, 11 Jul 2023 17:31:37 GMT  
		Size: 104.4 MB (104408241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff4bad9bf846d07362d8295a4479f8f2965dfb5934a9a032b335ce3cb086bdf7`  
		Last Modified: Fri, 14 Jul 2023 00:04:06 GMT  
		Size: 1.2 KB (1161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f94b9b520f177b081bf712ba074ba66cad6139b8164f8e18de5be8ebd3ae7382`  
		Last Modified: Fri, 14 Jul 2023 00:08:34 GMT  
		Size: 7.8 MB (7786370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c03838a3679d351be263b09d3a5c6b9c44c73bd67df1a32d00364b15614d8b4c`  
		Last Modified: Fri, 14 Jul 2023 00:08:32 GMT  
		Size: 1.1 KB (1058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3a7169624bc074e90056b7387038bd434dc1bc770b6ac612f0d295d8db6b10f`  
		Last Modified: Fri, 14 Jul 2023 00:08:31 GMT  
		Size: 1.0 KB (1035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30ef31773aef63c527f320ae07bc5b102bd9f4f448f3b8d21c3e339e30db10e1`  
		Last Modified: Fri, 14 Jul 2023 00:08:32 GMT  
		Size: 1.1 KB (1074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:scratch`

```console
$ docker pull nats-streaming@sha256:2b8205e7d3a87aacdc19ec7b71e3316a44380ef15ab834060826911876394dac
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:scratch` - linux; amd64

```console
$ docker pull nats-streaming@sha256:0963a4d0a1504acf8b8f5b99fa1f119639a1caff31850eefe83a685fac6820fb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.7 MB (7659749 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:32ad867a381275ce803cc7a4e3007d375908b15c83a75444af3352cfdc72d2eb`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Wed, 21 Jun 2023 01:10:50 GMT
COPY file:670c17c233c7999d9f7b72c2962b221cab4e00da471a75e8679840c939143cfb in /nats-streaming-server 
# Wed, 21 Jun 2023 01:10:50 GMT
EXPOSE 4222 8222
# Wed, 21 Jun 2023 01:10:51 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Wed, 21 Jun 2023 01:10:51 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:b7ff958d406306840566ff165f0c34c6017d44a13d4355d5eb8c6cd152c57d64`  
		Last Modified: Wed, 21 Jun 2023 01:11:25 GMT  
		Size: 7.7 MB (7659749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:scratch` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:c6adf4bdcf4ca4548a1331f9a5b78accb38369508960b70058ae6f3cfe00ed5d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7311545 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7763bb2699d3b947f45691cca3c382801ad1c0a91b829831fd0999aa54245f66`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Wed, 21 Jun 2023 00:59:07 GMT
COPY file:9bc2f7015ff72f7e91556a01075e89ef8a85a404228874028f7a356e8142e169 in /nats-streaming-server 
# Wed, 21 Jun 2023 00:59:07 GMT
EXPOSE 4222 8222
# Wed, 21 Jun 2023 00:59:07 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Wed, 21 Jun 2023 00:59:08 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:ee4a78724efc3390679e6118a2f2c5993c9075f378bd6a2f0b7f99b50579fb2b`  
		Last Modified: Wed, 21 Jun 2023 00:59:42 GMT  
		Size: 7.3 MB (7311545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:scratch` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:3ae971fd2fa4bc0a898567aa6a6ea4d4dbae8d4459d81e59a2fab244b4d9c5b0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7304325 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:825e70124556ec89714458bdec5da1ee59baa724df73fa420db3005bfad56c45`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Wed, 21 Jun 2023 01:31:21 GMT
COPY file:07846c068b31699c9c9fe9b535ec7c1dcfbda7a16d7d178a50de1f9541deeebf in /nats-streaming-server 
# Wed, 21 Jun 2023 01:31:21 GMT
EXPOSE 4222 8222
# Wed, 21 Jun 2023 01:31:21 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Wed, 21 Jun 2023 01:31:21 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:039446f9a794527f7060ddd5b9b8a071ffe8816fa5aae791c4bbf01db3656057`  
		Last Modified: Wed, 21 Jun 2023 01:31:55 GMT  
		Size: 7.3 MB (7304325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:scratch` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:04ef4025a7de920cc90464848b402755e5da72e57bc969aff8859af5429c00a7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.0 MB (7011458 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1627cfd9fc66597d5484a918e734f0595b380583577fd3a532f6228b72db740a`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Wed, 21 Jun 2023 01:11:52 GMT
COPY file:8237d0d59fd3c6b32e52dbff50861a8848f846505c0303e7975e4a5f48ce8de9 in /nats-streaming-server 
# Wed, 21 Jun 2023 01:11:52 GMT
EXPOSE 4222 8222
# Wed, 21 Jun 2023 01:11:52 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Wed, 21 Jun 2023 01:11:52 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:c3b4c14668a8e32e87c6ea3dce4a99716b527ba7f0f4608cbab27184c89832ee`  
		Last Modified: Wed, 21 Jun 2023 01:12:24 GMT  
		Size: 7.0 MB (7011458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:windowsservercore`

```console
$ docker pull nats-streaming@sha256:f8f306c1324a747d5f42fbd66e59d90ef995c1f82d95a07af46ec637a8fa29ee
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4645; amd64

### `nats-streaming:windowsservercore` - windows version 10.0.17763.4645; amd64

```console
$ docker pull nats-streaming@sha256:e3600f1ee85431963c7c2e4ba9dd422516b7c89203680e9098086f8eee913396
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1948162918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba9d6571d5a398539f54f2d4eb7bbdc753472d33dfb4fa5905ed6a249a5ec33c`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Fri, 07 Jul 2023 08:17:39 GMT
RUN Install update 10.0.17763.4645
# Thu, 13 Jul 2023 22:38:00 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Fri, 14 Jul 2023 00:00:18 GMT
ENV NATS_DOCKERIZED=1
# Fri, 14 Jul 2023 00:04:55 GMT
ENV NATS_STREAMING_SERVER=0.25.5
# Fri, 14 Jul 2023 00:04:56 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.25.5/nats-streaming-server-v0.25.5-windows-amd64.zip
# Fri, 14 Jul 2023 00:04:56 GMT
ENV NATS_STREAMING_SERVER_SHASUM=709b481bfa3537dc7941490365e065554f19c7029830d765ef49e8cd16657b75
# Fri, 14 Jul 2023 00:05:52 GMT
RUN Set-PSDebug -Trace 2
# Fri, 14 Jul 2023 00:07:33 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Fri, 14 Jul 2023 00:07:34 GMT
EXPOSE 4222 8222
# Fri, 14 Jul 2023 00:07:35 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Fri, 14 Jul 2023 00:07:36 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e36dba1ee29cd36713c8785a5de7dd2a487244d734ed4c5e7b0a6890bffb806e`  
		Last Modified: Tue, 11 Jul 2023 18:27:38 GMT  
		Size: 289.1 MB (289068746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48b452db6d50a62b6e0e8dadb19715cfcf62cf73e54b5d3bac96621c1093673c`  
		Last Modified: Thu, 13 Jul 2023 23:25:18 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20f8ca4b8d322e27c827c0ba667217bc04a39b69f5f483d5f2f9726e6d42522e`  
		Last Modified: Fri, 14 Jul 2023 00:03:50 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18679ad5f87511b5572cc2ff53e239532dca4c70a413dcf8fc9f8aca97bf4f96`  
		Last Modified: Fri, 14 Jul 2023 00:08:19 GMT  
		Size: 1.3 KB (1279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9c5202984226bceb34a191f9e86a9b84106eebcd4c6a4e47314b707ac610f38`  
		Last Modified: Fri, 14 Jul 2023 00:08:19 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bca3f1baea6a69d419c0fce9341dfac5cbe256fdb7eb9415fe4f1c4edf1a7b93`  
		Last Modified: Fri, 14 Jul 2023 00:08:18 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4631c84b931d3f1ee529f0423fa3188ea9e48d8af0089a9887fa992becd65312`  
		Last Modified: Fri, 14 Jul 2023 00:08:17 GMT  
		Size: 226.1 KB (226123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a195df7f50ec1e109468319f7e85f27d494af37f9eceb4586c2abd45b7798ec9`  
		Last Modified: Fri, 14 Jul 2023 00:08:19 GMT  
		Size: 8.2 MB (8237038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7271bd8c5599f12857ee3ed75550b08dc3638819425f32fd3ab0b104dda1e0d8`  
		Last Modified: Fri, 14 Jul 2023 00:08:17 GMT  
		Size: 1.3 KB (1324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2001f0adacd1483a7214db132b80267a2d9a728c9099b49a73bffec74f4c4c47`  
		Last Modified: Fri, 14 Jul 2023 00:08:17 GMT  
		Size: 1.3 KB (1313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:076f3743d3f1ac915066251cf19292b7e95d2b21d98f6d6fa723ced8cf864026`  
		Last Modified: Fri, 14 Jul 2023 00:08:17 GMT  
		Size: 1.3 KB (1335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:windowsservercore-1809`

```console
$ docker pull nats-streaming@sha256:f8f306c1324a747d5f42fbd66e59d90ef995c1f82d95a07af46ec637a8fa29ee
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4645; amd64

### `nats-streaming:windowsservercore-1809` - windows version 10.0.17763.4645; amd64

```console
$ docker pull nats-streaming@sha256:e3600f1ee85431963c7c2e4ba9dd422516b7c89203680e9098086f8eee913396
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1948162918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba9d6571d5a398539f54f2d4eb7bbdc753472d33dfb4fa5905ed6a249a5ec33c`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Fri, 07 Jul 2023 08:17:39 GMT
RUN Install update 10.0.17763.4645
# Thu, 13 Jul 2023 22:38:00 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Fri, 14 Jul 2023 00:00:18 GMT
ENV NATS_DOCKERIZED=1
# Fri, 14 Jul 2023 00:04:55 GMT
ENV NATS_STREAMING_SERVER=0.25.5
# Fri, 14 Jul 2023 00:04:56 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.25.5/nats-streaming-server-v0.25.5-windows-amd64.zip
# Fri, 14 Jul 2023 00:04:56 GMT
ENV NATS_STREAMING_SERVER_SHASUM=709b481bfa3537dc7941490365e065554f19c7029830d765ef49e8cd16657b75
# Fri, 14 Jul 2023 00:05:52 GMT
RUN Set-PSDebug -Trace 2
# Fri, 14 Jul 2023 00:07:33 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Fri, 14 Jul 2023 00:07:34 GMT
EXPOSE 4222 8222
# Fri, 14 Jul 2023 00:07:35 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Fri, 14 Jul 2023 00:07:36 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e36dba1ee29cd36713c8785a5de7dd2a487244d734ed4c5e7b0a6890bffb806e`  
		Last Modified: Tue, 11 Jul 2023 18:27:38 GMT  
		Size: 289.1 MB (289068746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48b452db6d50a62b6e0e8dadb19715cfcf62cf73e54b5d3bac96621c1093673c`  
		Last Modified: Thu, 13 Jul 2023 23:25:18 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20f8ca4b8d322e27c827c0ba667217bc04a39b69f5f483d5f2f9726e6d42522e`  
		Last Modified: Fri, 14 Jul 2023 00:03:50 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18679ad5f87511b5572cc2ff53e239532dca4c70a413dcf8fc9f8aca97bf4f96`  
		Last Modified: Fri, 14 Jul 2023 00:08:19 GMT  
		Size: 1.3 KB (1279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9c5202984226bceb34a191f9e86a9b84106eebcd4c6a4e47314b707ac610f38`  
		Last Modified: Fri, 14 Jul 2023 00:08:19 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bca3f1baea6a69d419c0fce9341dfac5cbe256fdb7eb9415fe4f1c4edf1a7b93`  
		Last Modified: Fri, 14 Jul 2023 00:08:18 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4631c84b931d3f1ee529f0423fa3188ea9e48d8af0089a9887fa992becd65312`  
		Last Modified: Fri, 14 Jul 2023 00:08:17 GMT  
		Size: 226.1 KB (226123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a195df7f50ec1e109468319f7e85f27d494af37f9eceb4586c2abd45b7798ec9`  
		Last Modified: Fri, 14 Jul 2023 00:08:19 GMT  
		Size: 8.2 MB (8237038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7271bd8c5599f12857ee3ed75550b08dc3638819425f32fd3ab0b104dda1e0d8`  
		Last Modified: Fri, 14 Jul 2023 00:08:17 GMT  
		Size: 1.3 KB (1324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2001f0adacd1483a7214db132b80267a2d9a728c9099b49a73bffec74f4c4c47`  
		Last Modified: Fri, 14 Jul 2023 00:08:17 GMT  
		Size: 1.3 KB (1313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:076f3743d3f1ac915066251cf19292b7e95d2b21d98f6d6fa723ced8cf864026`  
		Last Modified: Fri, 14 Jul 2023 00:08:17 GMT  
		Size: 1.3 KB (1335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
