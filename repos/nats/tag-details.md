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
$ docker pull nats@sha256:1fc110ad1583ad4ac948623fbaed53afec34afc4a03d60e23384a5d4479fe22d
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
$ docker pull nats@sha256:b7cd8c3270f038b671b4d55156398eec4387fff96c2de872255d30024bf6a557
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4931647 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b82b64c84efab021cd029f60c01c7e52b53b4eae18827b383f87a4393b3a7095`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 02 Feb 2023 21:33:01 GMT
COPY file:a9e60c6fbbdd9ebb5d2c4deec1df6db6d6a40a0384a5544b6c3386eea2057a54 in /nats-server 
# Thu, 02 Feb 2023 21:33:02 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 02 Feb 2023 21:33:02 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Feb 2023 21:33:02 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 02 Feb 2023 21:33:02 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 02 Feb 2023 21:33:02 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:1cd3edd838903059461e505e0f1e09d3452d5e632e2b550f4d0850b0d2f59c72`  
		Last Modified: Thu, 02 Feb 2023 21:33:50 GMT  
		Size: 4.9 MB (4931138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e56ba114f2531c68c394372ad404aeb5ac8ee8946fb17af7ac704a76697756f`  
		Last Modified: Thu, 02 Feb 2023 21:33:49 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - linux; arm variant v6

```console
$ docker pull nats@sha256:c1107d0e00f4d8dedfbf7883fbabc7b200545657e1e13495e12453d13dfde328
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4694918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c7de15c41747ca8b98deb9b16e6b45e323bf1b12bfe5ba0617911396006a4fc`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 02 Feb 2023 21:50:29 GMT
COPY file:be32648053f47b33b445bad52bed7ff3e74d1dc77100df4d672e431022428de7 in /nats-server 
# Thu, 02 Feb 2023 21:50:29 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 02 Feb 2023 21:50:29 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Feb 2023 21:50:29 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 02 Feb 2023 21:50:29 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 02 Feb 2023 21:50:29 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:eddbc6c88066991dd5810d3a3b6875ee06eecb063cccc9b0e3d9386c75c4f826`  
		Last Modified: Thu, 02 Feb 2023 21:52:00 GMT  
		Size: 4.7 MB (4694411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:795c72903a6f36672ee81a0386bff46e30e1f3598c7552f5c192f650d82c6e69`  
		Last Modified: Thu, 02 Feb 2023 21:51:59 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - linux; arm variant v7

```console
$ docker pull nats@sha256:8a3086f469fd77000e1a8618960b722ca85e5cbd69a41190e81286734c7e455a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4688297 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa7e9966ce4e992db69b98063dd7d35d6fe1239100d385115ea7031b9b65978b`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 02 Feb 2023 21:58:12 GMT
COPY file:a67f587b7b86d3c3a85687c0097c93084fb71c44966695879cd46269a36ed31d in /nats-server 
# Thu, 02 Feb 2023 21:58:12 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 02 Feb 2023 21:58:12 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Feb 2023 21:58:12 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 02 Feb 2023 21:58:12 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 02 Feb 2023 21:58:12 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:df148ca425b44984356880f1ed4c1f04d36d2e6efa76ba4043d9dd80fe9f6201`  
		Last Modified: Thu, 02 Feb 2023 21:59:43 GMT  
		Size: 4.7 MB (4687788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b679ac38b5a1c67873f0f08c522aafadecaa085bed163dcc8387ddd53c0509d2`  
		Last Modified: Thu, 02 Feb 2023 21:59:43 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:b33b08f196a8f9b3b612740d36e847c1d5bc5239bf49f768b0056cd2ff7baaf0
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4517074 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:21aad311a08f5e75bd795b33799a8a100d9eb132974428f406329a5871687f79`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 02 Feb 2023 21:47:40 GMT
COPY file:f1194fd7c754730901a7920f7db8ad6e6432e904adfe27cb3bf09f1626eb0b20 in /nats-server 
# Thu, 02 Feb 2023 21:47:40 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 02 Feb 2023 21:47:40 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Feb 2023 21:47:40 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 02 Feb 2023 21:47:40 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 02 Feb 2023 21:47:40 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:0e112ba48caecfa7e51d560718ada0f9c4e686bdc09555df0617055a883e5777`  
		Last Modified: Thu, 02 Feb 2023 21:48:28 GMT  
		Size: 4.5 MB (4516565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fce6348af8f3a9160210d4305f3a6f5c76b1b36d75df166f313f92cf3774f93f`  
		Last Modified: Thu, 02 Feb 2023 21:48:27 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - windows version 10.0.17763.3887; amd64

```console
$ docker pull nats@sha256:298b8a1b690d1d64fbd955cb251e93b63874ef7d4cb6f0eb2128cb3df82d1ecf
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.7 MB (111657511 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d6d4d57475df3d7d3cc4f4a97791acce1c9ce0aa971eff49258813b2b55ba7c`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 07 Jan 2023 05:17:01 GMT
RUN Apply image 10.0.17763.3887
# Thu, 12 Jan 2023 05:01:51 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Thu, 02 Feb 2023 21:18:29 GMT
RUN cmd /S /C #(nop) COPY file:1d619f9da4aa7d6fe4171f8e7c232a42ba0b813a50cbb3466448bbfaf0fc4a79 in C:\nats-server.exe 
# Thu, 02 Feb 2023 21:18:30 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Thu, 02 Feb 2023 21:18:31 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Thu, 02 Feb 2023 21:18:32 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 02 Feb 2023 21:18:33 GMT
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
	-	`sha256:3801c3e14f4f67451b0f8a1220428a70eeddbf9bdef73cd8b89614087bfea683`  
		Last Modified: Thu, 02 Feb 2023 21:19:24 GMT  
		Size: 5.0 MB (4985010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc3da06a2f05c3cb57b2c4406a7135beaef26938a9d48c94e9bb19f285362f19`  
		Last Modified: Thu, 02 Feb 2023 21:19:22 GMT  
		Size: 1.8 KB (1768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a28bce3ab94f882453c700042d8e7ff6aa55d92a06dad8d04be017d91ec9208`  
		Last Modified: Thu, 02 Feb 2023 21:19:22 GMT  
		Size: 1.2 KB (1173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dba391f32fd738334e9c4d766b67aa8340b1fac87188801d71faf347db92b3fb`  
		Last Modified: Thu, 02 Feb 2023 21:19:22 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d938df46930834c4903622f9028898bde90a5f21c98963408af250b41e05242c`  
		Last Modified: Thu, 02 Feb 2023 21:19:22 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-alpine`

```console
$ docker pull nats@sha256:755bdf0c9fea43659ef9485ff74a9303ac2595c1b02c807d92b53802baf808a6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-alpine` - linux; amd64

```console
$ docker pull nats@sha256:596442ede179d773ec7f08637e1347328ec3f12ed64568dd29bf8bd92259c84d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.6 MB (8589330 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:36a5b27103c778bd375b40b313ac2dd449b9123b78b3e1933ccf2c24bf0082bb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 09 Jan 2023 17:05:20 GMT
ADD file:e4d600fc4c9c293efe360be7b30ee96579925d1b4634c94332e2ec73f7d8eca1 in / 
# Mon, 09 Jan 2023 17:05:20 GMT
CMD ["/bin/sh"]
# Thu, 02 Feb 2023 21:32:50 GMT
ENV NATS_SERVER=2.9.12
# Thu, 02 Feb 2023 21:32:54 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='296075e7caa33684f0a23ac97c2a904c8f22dbc1d75da4ab443a81aa8b1b765b' ;; 		armhf) natsArch='arm6'; sha256='72af57a620de31e718131736b4ae123acd994295b2f81d1f847cdb9e1e686e63' ;; 		armv7) natsArch='arm7'; sha256='153d823e90b76457b6689cb6baa9f045b3a2152caaec787a0ad77162431949ed' ;; 		x86_64) natsArch='amd64'; sha256='cd05e53b3e1a535dd4e09a4cba3c1b0cd7c512e7f3d68d52ed8e8621dac8c925' ;; 		x86) natsArch='386'; sha256='103d89a231154708375a091dfb86ebe563f3de968a5e6ed14aba4c32e5c77925' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 02 Feb 2023 21:32:54 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 02 Feb 2023 21:32:54 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 02 Feb 2023 21:32:54 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Feb 2023 21:32:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 02 Feb 2023 21:32:54 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:8921db27df2831fa6eaa85321205a2470c669b855f3ec95d5a3c2b46de0442c9`  
		Last Modified: Mon, 09 Jan 2023 17:05:45 GMT  
		Size: 3.4 MB (3370628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90fc2d6058c164e7f06206d5ec77d1dc1a27fbde65facfb00c7be6ebd6c00c9a`  
		Last Modified: Thu, 02 Feb 2023 21:33:28 GMT  
		Size: 5.2 MB (5217701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c8da51ec4a12edfcbb65016c0ab6137e4261542c0806c198a7561573428f286`  
		Last Modified: Thu, 02 Feb 2023 21:33:28 GMT  
		Size: 588.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd8137ab539d1ca45399d4e83b217c0290e34a11f764287427ef7fa51ff209bf`  
		Last Modified: Thu, 02 Feb 2023 21:33:27 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:325775413795f10444c422d2b752494acbd407613fc1537a7cf84693283102a6
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.1 MB (8090427 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c037e626dfdaad2eb7338914f0db6020567bb99c48a7e0f01345484edfa0c7d9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 09 Jan 2023 17:04:54 GMT
ADD file:b15fd8e9f996815394e25f20c8459bfb4c2a8c4074592d6f4c75f4fe79ce537e in / 
# Mon, 09 Jan 2023 17:04:55 GMT
CMD ["/bin/sh"]
# Thu, 02 Feb 2023 21:49:33 GMT
ENV NATS_SERVER=2.9.12
# Thu, 02 Feb 2023 21:50:12 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='296075e7caa33684f0a23ac97c2a904c8f22dbc1d75da4ab443a81aa8b1b765b' ;; 		armhf) natsArch='arm6'; sha256='72af57a620de31e718131736b4ae123acd994295b2f81d1f847cdb9e1e686e63' ;; 		armv7) natsArch='arm7'; sha256='153d823e90b76457b6689cb6baa9f045b3a2152caaec787a0ad77162431949ed' ;; 		x86_64) natsArch='amd64'; sha256='cd05e53b3e1a535dd4e09a4cba3c1b0cd7c512e7f3d68d52ed8e8621dac8c925' ;; 		x86) natsArch='386'; sha256='103d89a231154708375a091dfb86ebe563f3de968a5e6ed14aba4c32e5c77925' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 02 Feb 2023 21:50:12 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 02 Feb 2023 21:50:12 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 02 Feb 2023 21:50:12 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Feb 2023 21:50:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 02 Feb 2023 21:50:13 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:0269c10e600f3a375f36ddabdbd264ce9503a455f0d0969ce8a00f24eaecc032`  
		Last Modified: Mon, 09 Jan 2023 17:05:45 GMT  
		Size: 3.1 MB (3107243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c06b18d184d344d8a89cb092274a39e8c3bf5646c1a8678e53519585c03292b`  
		Last Modified: Thu, 02 Feb 2023 21:51:28 GMT  
		Size: 5.0 MB (4982208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb35f9a15c3a5b93ea2a254cc9c9cc741a6e698dd58741a9f9af4936c2049f03`  
		Last Modified: Thu, 02 Feb 2023 21:51:27 GMT  
		Size: 561.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b92f0e4cdd97e7662fe9c94bd67aabac7172d0e0d97acf0b5c586de7b89f895`  
		Last Modified: Thu, 02 Feb 2023 21:51:27 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:6c2d2b789f9ed0c9edddd86e758373c2c2f76132958d3dec5c2a6d1e7336f9dc
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.8 MB (7841051 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d85fea070aff07d7750af4de5ce3ebb9b49a00738becb1eae53e9281e25aca5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 09 Jan 2023 17:06:27 GMT
ADD file:4696f25d0f019b27457c55b3b128b70bf153f38e3e4eb5bdfc21058543313e94 in / 
# Mon, 09 Jan 2023 17:06:27 GMT
CMD ["/bin/sh"]
# Thu, 02 Feb 2023 21:57:48 GMT
ENV NATS_SERVER=2.9.12
# Thu, 02 Feb 2023 21:57:51 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='296075e7caa33684f0a23ac97c2a904c8f22dbc1d75da4ab443a81aa8b1b765b' ;; 		armhf) natsArch='arm6'; sha256='72af57a620de31e718131736b4ae123acd994295b2f81d1f847cdb9e1e686e63' ;; 		armv7) natsArch='arm7'; sha256='153d823e90b76457b6689cb6baa9f045b3a2152caaec787a0ad77162431949ed' ;; 		x86_64) natsArch='amd64'; sha256='cd05e53b3e1a535dd4e09a4cba3c1b0cd7c512e7f3d68d52ed8e8621dac8c925' ;; 		x86) natsArch='386'; sha256='103d89a231154708375a091dfb86ebe563f3de968a5e6ed14aba4c32e5c77925' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 02 Feb 2023 21:57:51 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 02 Feb 2023 21:57:51 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 02 Feb 2023 21:57:51 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Feb 2023 21:57:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 02 Feb 2023 21:57:52 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:c527615e4ffa2d5b9b777fd469b3b5ba7c1b1e9201c065be2c43569de48a3754`  
		Last Modified: Mon, 09 Jan 2023 17:07:17 GMT  
		Size: 2.9 MB (2865208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54dcdcd84f34ebca9af1574488d3c29f20e5444ee61f4eb8688d3b5b9b1aa829`  
		Last Modified: Thu, 02 Feb 2023 21:59:11 GMT  
		Size: 5.0 MB (4974868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bebca7f9dc77dd081f1e8386b332902935be6eb718e5435056e6928dbdcded07`  
		Last Modified: Thu, 02 Feb 2023 21:59:10 GMT  
		Size: 561.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7247a73a46f57913d3042d8273753dc2524e2b7308a9b7c623043a9f83874df`  
		Last Modified: Thu, 02 Feb 2023 21:59:10 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:3b5d7a8ce580949f91c72ccb764cb0f808ca47f4a306cd2a64adef699b18c709
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.1 MB (8062087 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:72e93fab38c492847947f3360491ff675e9657ddad7fffcd6ddaf34818b3359e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 09 Jan 2023 17:04:48 GMT
ADD file:3080f19f39259a4b77cc53975de0184c78d4335ceb9ffb77a2838d0539ad6f85 in / 
# Mon, 09 Jan 2023 17:04:49 GMT
CMD ["/bin/sh"]
# Thu, 02 Feb 2023 21:47:31 GMT
ENV NATS_SERVER=2.9.12
# Thu, 02 Feb 2023 21:47:34 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='296075e7caa33684f0a23ac97c2a904c8f22dbc1d75da4ab443a81aa8b1b765b' ;; 		armhf) natsArch='arm6'; sha256='72af57a620de31e718131736b4ae123acd994295b2f81d1f847cdb9e1e686e63' ;; 		armv7) natsArch='arm7'; sha256='153d823e90b76457b6689cb6baa9f045b3a2152caaec787a0ad77162431949ed' ;; 		x86_64) natsArch='amd64'; sha256='cd05e53b3e1a535dd4e09a4cba3c1b0cd7c512e7f3d68d52ed8e8621dac8c925' ;; 		x86) natsArch='386'; sha256='103d89a231154708375a091dfb86ebe563f3de968a5e6ed14aba4c32e5c77925' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 02 Feb 2023 21:47:34 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 02 Feb 2023 21:47:34 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 02 Feb 2023 21:47:34 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Feb 2023 21:47:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 02 Feb 2023 21:47:34 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:a9eaa45ef418e883481a13c7d84fa9904f2ec56789c52a87ba5a9e6483f2b74f`  
		Last Modified: Mon, 09 Jan 2023 17:05:12 GMT  
		Size: 3.3 MB (3259241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf7882578303a0fa74c95f3a4d8ba43cb527ab5ae15db2e91420624139809c58`  
		Last Modified: Thu, 02 Feb 2023 21:48:06 GMT  
		Size: 4.8 MB (4801846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02c5fcf7cb836026cb1caf41222a5db286caad4181a1465fbc6a827e539d655f`  
		Last Modified: Thu, 02 Feb 2023 21:48:06 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c842168768b2663567de8311303dd5b2951b867f7c2228af37a24b50f24181ae`  
		Last Modified: Thu, 02 Feb 2023 21:48:05 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-alpine3.17`

```console
$ docker pull nats@sha256:755bdf0c9fea43659ef9485ff74a9303ac2595c1b02c807d92b53802baf808a6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-alpine3.17` - linux; amd64

```console
$ docker pull nats@sha256:596442ede179d773ec7f08637e1347328ec3f12ed64568dd29bf8bd92259c84d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.6 MB (8589330 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:36a5b27103c778bd375b40b313ac2dd449b9123b78b3e1933ccf2c24bf0082bb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 09 Jan 2023 17:05:20 GMT
ADD file:e4d600fc4c9c293efe360be7b30ee96579925d1b4634c94332e2ec73f7d8eca1 in / 
# Mon, 09 Jan 2023 17:05:20 GMT
CMD ["/bin/sh"]
# Thu, 02 Feb 2023 21:32:50 GMT
ENV NATS_SERVER=2.9.12
# Thu, 02 Feb 2023 21:32:54 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='296075e7caa33684f0a23ac97c2a904c8f22dbc1d75da4ab443a81aa8b1b765b' ;; 		armhf) natsArch='arm6'; sha256='72af57a620de31e718131736b4ae123acd994295b2f81d1f847cdb9e1e686e63' ;; 		armv7) natsArch='arm7'; sha256='153d823e90b76457b6689cb6baa9f045b3a2152caaec787a0ad77162431949ed' ;; 		x86_64) natsArch='amd64'; sha256='cd05e53b3e1a535dd4e09a4cba3c1b0cd7c512e7f3d68d52ed8e8621dac8c925' ;; 		x86) natsArch='386'; sha256='103d89a231154708375a091dfb86ebe563f3de968a5e6ed14aba4c32e5c77925' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 02 Feb 2023 21:32:54 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 02 Feb 2023 21:32:54 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 02 Feb 2023 21:32:54 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Feb 2023 21:32:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 02 Feb 2023 21:32:54 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:8921db27df2831fa6eaa85321205a2470c669b855f3ec95d5a3c2b46de0442c9`  
		Last Modified: Mon, 09 Jan 2023 17:05:45 GMT  
		Size: 3.4 MB (3370628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90fc2d6058c164e7f06206d5ec77d1dc1a27fbde65facfb00c7be6ebd6c00c9a`  
		Last Modified: Thu, 02 Feb 2023 21:33:28 GMT  
		Size: 5.2 MB (5217701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c8da51ec4a12edfcbb65016c0ab6137e4261542c0806c198a7561573428f286`  
		Last Modified: Thu, 02 Feb 2023 21:33:28 GMT  
		Size: 588.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd8137ab539d1ca45399d4e83b217c0290e34a11f764287427ef7fa51ff209bf`  
		Last Modified: Thu, 02 Feb 2023 21:33:27 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.17` - linux; arm variant v6

```console
$ docker pull nats@sha256:325775413795f10444c422d2b752494acbd407613fc1537a7cf84693283102a6
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.1 MB (8090427 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c037e626dfdaad2eb7338914f0db6020567bb99c48a7e0f01345484edfa0c7d9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 09 Jan 2023 17:04:54 GMT
ADD file:b15fd8e9f996815394e25f20c8459bfb4c2a8c4074592d6f4c75f4fe79ce537e in / 
# Mon, 09 Jan 2023 17:04:55 GMT
CMD ["/bin/sh"]
# Thu, 02 Feb 2023 21:49:33 GMT
ENV NATS_SERVER=2.9.12
# Thu, 02 Feb 2023 21:50:12 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='296075e7caa33684f0a23ac97c2a904c8f22dbc1d75da4ab443a81aa8b1b765b' ;; 		armhf) natsArch='arm6'; sha256='72af57a620de31e718131736b4ae123acd994295b2f81d1f847cdb9e1e686e63' ;; 		armv7) natsArch='arm7'; sha256='153d823e90b76457b6689cb6baa9f045b3a2152caaec787a0ad77162431949ed' ;; 		x86_64) natsArch='amd64'; sha256='cd05e53b3e1a535dd4e09a4cba3c1b0cd7c512e7f3d68d52ed8e8621dac8c925' ;; 		x86) natsArch='386'; sha256='103d89a231154708375a091dfb86ebe563f3de968a5e6ed14aba4c32e5c77925' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 02 Feb 2023 21:50:12 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 02 Feb 2023 21:50:12 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 02 Feb 2023 21:50:12 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Feb 2023 21:50:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 02 Feb 2023 21:50:13 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:0269c10e600f3a375f36ddabdbd264ce9503a455f0d0969ce8a00f24eaecc032`  
		Last Modified: Mon, 09 Jan 2023 17:05:45 GMT  
		Size: 3.1 MB (3107243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c06b18d184d344d8a89cb092274a39e8c3bf5646c1a8678e53519585c03292b`  
		Last Modified: Thu, 02 Feb 2023 21:51:28 GMT  
		Size: 5.0 MB (4982208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb35f9a15c3a5b93ea2a254cc9c9cc741a6e698dd58741a9f9af4936c2049f03`  
		Last Modified: Thu, 02 Feb 2023 21:51:27 GMT  
		Size: 561.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b92f0e4cdd97e7662fe9c94bd67aabac7172d0e0d97acf0b5c586de7b89f895`  
		Last Modified: Thu, 02 Feb 2023 21:51:27 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.17` - linux; arm variant v7

```console
$ docker pull nats@sha256:6c2d2b789f9ed0c9edddd86e758373c2c2f76132958d3dec5c2a6d1e7336f9dc
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.8 MB (7841051 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d85fea070aff07d7750af4de5ce3ebb9b49a00738becb1eae53e9281e25aca5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 09 Jan 2023 17:06:27 GMT
ADD file:4696f25d0f019b27457c55b3b128b70bf153f38e3e4eb5bdfc21058543313e94 in / 
# Mon, 09 Jan 2023 17:06:27 GMT
CMD ["/bin/sh"]
# Thu, 02 Feb 2023 21:57:48 GMT
ENV NATS_SERVER=2.9.12
# Thu, 02 Feb 2023 21:57:51 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='296075e7caa33684f0a23ac97c2a904c8f22dbc1d75da4ab443a81aa8b1b765b' ;; 		armhf) natsArch='arm6'; sha256='72af57a620de31e718131736b4ae123acd994295b2f81d1f847cdb9e1e686e63' ;; 		armv7) natsArch='arm7'; sha256='153d823e90b76457b6689cb6baa9f045b3a2152caaec787a0ad77162431949ed' ;; 		x86_64) natsArch='amd64'; sha256='cd05e53b3e1a535dd4e09a4cba3c1b0cd7c512e7f3d68d52ed8e8621dac8c925' ;; 		x86) natsArch='386'; sha256='103d89a231154708375a091dfb86ebe563f3de968a5e6ed14aba4c32e5c77925' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 02 Feb 2023 21:57:51 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 02 Feb 2023 21:57:51 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 02 Feb 2023 21:57:51 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Feb 2023 21:57:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 02 Feb 2023 21:57:52 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:c527615e4ffa2d5b9b777fd469b3b5ba7c1b1e9201c065be2c43569de48a3754`  
		Last Modified: Mon, 09 Jan 2023 17:07:17 GMT  
		Size: 2.9 MB (2865208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54dcdcd84f34ebca9af1574488d3c29f20e5444ee61f4eb8688d3b5b9b1aa829`  
		Last Modified: Thu, 02 Feb 2023 21:59:11 GMT  
		Size: 5.0 MB (4974868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bebca7f9dc77dd081f1e8386b332902935be6eb718e5435056e6928dbdcded07`  
		Last Modified: Thu, 02 Feb 2023 21:59:10 GMT  
		Size: 561.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7247a73a46f57913d3042d8273753dc2524e2b7308a9b7c623043a9f83874df`  
		Last Modified: Thu, 02 Feb 2023 21:59:10 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.17` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:3b5d7a8ce580949f91c72ccb764cb0f808ca47f4a306cd2a64adef699b18c709
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.1 MB (8062087 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:72e93fab38c492847947f3360491ff675e9657ddad7fffcd6ddaf34818b3359e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 09 Jan 2023 17:04:48 GMT
ADD file:3080f19f39259a4b77cc53975de0184c78d4335ceb9ffb77a2838d0539ad6f85 in / 
# Mon, 09 Jan 2023 17:04:49 GMT
CMD ["/bin/sh"]
# Thu, 02 Feb 2023 21:47:31 GMT
ENV NATS_SERVER=2.9.12
# Thu, 02 Feb 2023 21:47:34 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='296075e7caa33684f0a23ac97c2a904c8f22dbc1d75da4ab443a81aa8b1b765b' ;; 		armhf) natsArch='arm6'; sha256='72af57a620de31e718131736b4ae123acd994295b2f81d1f847cdb9e1e686e63' ;; 		armv7) natsArch='arm7'; sha256='153d823e90b76457b6689cb6baa9f045b3a2152caaec787a0ad77162431949ed' ;; 		x86_64) natsArch='amd64'; sha256='cd05e53b3e1a535dd4e09a4cba3c1b0cd7c512e7f3d68d52ed8e8621dac8c925' ;; 		x86) natsArch='386'; sha256='103d89a231154708375a091dfb86ebe563f3de968a5e6ed14aba4c32e5c77925' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 02 Feb 2023 21:47:34 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 02 Feb 2023 21:47:34 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 02 Feb 2023 21:47:34 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Feb 2023 21:47:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 02 Feb 2023 21:47:34 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:a9eaa45ef418e883481a13c7d84fa9904f2ec56789c52a87ba5a9e6483f2b74f`  
		Last Modified: Mon, 09 Jan 2023 17:05:12 GMT  
		Size: 3.3 MB (3259241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf7882578303a0fa74c95f3a4d8ba43cb527ab5ae15db2e91420624139809c58`  
		Last Modified: Thu, 02 Feb 2023 21:48:06 GMT  
		Size: 4.8 MB (4801846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02c5fcf7cb836026cb1caf41222a5db286caad4181a1465fbc6a827e539d655f`  
		Last Modified: Thu, 02 Feb 2023 21:48:06 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c842168768b2663567de8311303dd5b2951b867f7c2228af37a24b50f24181ae`  
		Last Modified: Thu, 02 Feb 2023 21:48:05 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-linux`

```console
$ docker pull nats@sha256:c926cdb68b698f2bbe658b5dac5353803f29c4cd4e7ab8bdc572077ee8a9f870
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-linux` - linux; amd64

```console
$ docker pull nats@sha256:b7cd8c3270f038b671b4d55156398eec4387fff96c2de872255d30024bf6a557
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4931647 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b82b64c84efab021cd029f60c01c7e52b53b4eae18827b383f87a4393b3a7095`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 02 Feb 2023 21:33:01 GMT
COPY file:a9e60c6fbbdd9ebb5d2c4deec1df6db6d6a40a0384a5544b6c3386eea2057a54 in /nats-server 
# Thu, 02 Feb 2023 21:33:02 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 02 Feb 2023 21:33:02 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Feb 2023 21:33:02 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 02 Feb 2023 21:33:02 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 02 Feb 2023 21:33:02 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:1cd3edd838903059461e505e0f1e09d3452d5e632e2b550f4d0850b0d2f59c72`  
		Last Modified: Thu, 02 Feb 2023 21:33:50 GMT  
		Size: 4.9 MB (4931138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e56ba114f2531c68c394372ad404aeb5ac8ee8946fb17af7ac704a76697756f`  
		Last Modified: Thu, 02 Feb 2023 21:33:49 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:c1107d0e00f4d8dedfbf7883fbabc7b200545657e1e13495e12453d13dfde328
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4694918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c7de15c41747ca8b98deb9b16e6b45e323bf1b12bfe5ba0617911396006a4fc`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 02 Feb 2023 21:50:29 GMT
COPY file:be32648053f47b33b445bad52bed7ff3e74d1dc77100df4d672e431022428de7 in /nats-server 
# Thu, 02 Feb 2023 21:50:29 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 02 Feb 2023 21:50:29 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Feb 2023 21:50:29 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 02 Feb 2023 21:50:29 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 02 Feb 2023 21:50:29 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:eddbc6c88066991dd5810d3a3b6875ee06eecb063cccc9b0e3d9386c75c4f826`  
		Last Modified: Thu, 02 Feb 2023 21:52:00 GMT  
		Size: 4.7 MB (4694411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:795c72903a6f36672ee81a0386bff46e30e1f3598c7552f5c192f650d82c6e69`  
		Last Modified: Thu, 02 Feb 2023 21:51:59 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:8a3086f469fd77000e1a8618960b722ca85e5cbd69a41190e81286734c7e455a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4688297 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa7e9966ce4e992db69b98063dd7d35d6fe1239100d385115ea7031b9b65978b`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 02 Feb 2023 21:58:12 GMT
COPY file:a67f587b7b86d3c3a85687c0097c93084fb71c44966695879cd46269a36ed31d in /nats-server 
# Thu, 02 Feb 2023 21:58:12 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 02 Feb 2023 21:58:12 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Feb 2023 21:58:12 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 02 Feb 2023 21:58:12 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 02 Feb 2023 21:58:12 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:df148ca425b44984356880f1ed4c1f04d36d2e6efa76ba4043d9dd80fe9f6201`  
		Last Modified: Thu, 02 Feb 2023 21:59:43 GMT  
		Size: 4.7 MB (4687788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b679ac38b5a1c67873f0f08c522aafadecaa085bed163dcc8387ddd53c0509d2`  
		Last Modified: Thu, 02 Feb 2023 21:59:43 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:b33b08f196a8f9b3b612740d36e847c1d5bc5239bf49f768b0056cd2ff7baaf0
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4517074 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:21aad311a08f5e75bd795b33799a8a100d9eb132974428f406329a5871687f79`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 02 Feb 2023 21:47:40 GMT
COPY file:f1194fd7c754730901a7920f7db8ad6e6432e904adfe27cb3bf09f1626eb0b20 in /nats-server 
# Thu, 02 Feb 2023 21:47:40 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 02 Feb 2023 21:47:40 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Feb 2023 21:47:40 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 02 Feb 2023 21:47:40 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 02 Feb 2023 21:47:40 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:0e112ba48caecfa7e51d560718ada0f9c4e686bdc09555df0617055a883e5777`  
		Last Modified: Thu, 02 Feb 2023 21:48:28 GMT  
		Size: 4.5 MB (4516565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fce6348af8f3a9160210d4305f3a6f5c76b1b36d75df166f313f92cf3774f93f`  
		Last Modified: Thu, 02 Feb 2023 21:48:27 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-nanoserver`

```console
$ docker pull nats@sha256:853807ebafaad1d9a9ffee4521ea63cb1f171fe4e34262749cc13a71f59c1090
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3887; amd64

### `nats:2-nanoserver` - windows version 10.0.17763.3887; amd64

```console
$ docker pull nats@sha256:298b8a1b690d1d64fbd955cb251e93b63874ef7d4cb6f0eb2128cb3df82d1ecf
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.7 MB (111657511 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d6d4d57475df3d7d3cc4f4a97791acce1c9ce0aa971eff49258813b2b55ba7c`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 07 Jan 2023 05:17:01 GMT
RUN Apply image 10.0.17763.3887
# Thu, 12 Jan 2023 05:01:51 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Thu, 02 Feb 2023 21:18:29 GMT
RUN cmd /S /C #(nop) COPY file:1d619f9da4aa7d6fe4171f8e7c232a42ba0b813a50cbb3466448bbfaf0fc4a79 in C:\nats-server.exe 
# Thu, 02 Feb 2023 21:18:30 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Thu, 02 Feb 2023 21:18:31 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Thu, 02 Feb 2023 21:18:32 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 02 Feb 2023 21:18:33 GMT
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
	-	`sha256:3801c3e14f4f67451b0f8a1220428a70eeddbf9bdef73cd8b89614087bfea683`  
		Last Modified: Thu, 02 Feb 2023 21:19:24 GMT  
		Size: 5.0 MB (4985010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc3da06a2f05c3cb57b2c4406a7135beaef26938a9d48c94e9bb19f285362f19`  
		Last Modified: Thu, 02 Feb 2023 21:19:22 GMT  
		Size: 1.8 KB (1768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a28bce3ab94f882453c700042d8e7ff6aa55d92a06dad8d04be017d91ec9208`  
		Last Modified: Thu, 02 Feb 2023 21:19:22 GMT  
		Size: 1.2 KB (1173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dba391f32fd738334e9c4d766b67aa8340b1fac87188801d71faf347db92b3fb`  
		Last Modified: Thu, 02 Feb 2023 21:19:22 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d938df46930834c4903622f9028898bde90a5f21c98963408af250b41e05242c`  
		Last Modified: Thu, 02 Feb 2023 21:19:22 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-nanoserver-1809`

```console
$ docker pull nats@sha256:853807ebafaad1d9a9ffee4521ea63cb1f171fe4e34262749cc13a71f59c1090
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3887; amd64

### `nats:2-nanoserver-1809` - windows version 10.0.17763.3887; amd64

```console
$ docker pull nats@sha256:298b8a1b690d1d64fbd955cb251e93b63874ef7d4cb6f0eb2128cb3df82d1ecf
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.7 MB (111657511 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d6d4d57475df3d7d3cc4f4a97791acce1c9ce0aa971eff49258813b2b55ba7c`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 07 Jan 2023 05:17:01 GMT
RUN Apply image 10.0.17763.3887
# Thu, 12 Jan 2023 05:01:51 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Thu, 02 Feb 2023 21:18:29 GMT
RUN cmd /S /C #(nop) COPY file:1d619f9da4aa7d6fe4171f8e7c232a42ba0b813a50cbb3466448bbfaf0fc4a79 in C:\nats-server.exe 
# Thu, 02 Feb 2023 21:18:30 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Thu, 02 Feb 2023 21:18:31 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Thu, 02 Feb 2023 21:18:32 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 02 Feb 2023 21:18:33 GMT
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
	-	`sha256:3801c3e14f4f67451b0f8a1220428a70eeddbf9bdef73cd8b89614087bfea683`  
		Last Modified: Thu, 02 Feb 2023 21:19:24 GMT  
		Size: 5.0 MB (4985010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc3da06a2f05c3cb57b2c4406a7135beaef26938a9d48c94e9bb19f285362f19`  
		Last Modified: Thu, 02 Feb 2023 21:19:22 GMT  
		Size: 1.8 KB (1768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a28bce3ab94f882453c700042d8e7ff6aa55d92a06dad8d04be017d91ec9208`  
		Last Modified: Thu, 02 Feb 2023 21:19:22 GMT  
		Size: 1.2 KB (1173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dba391f32fd738334e9c4d766b67aa8340b1fac87188801d71faf347db92b3fb`  
		Last Modified: Thu, 02 Feb 2023 21:19:22 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d938df46930834c4903622f9028898bde90a5f21c98963408af250b41e05242c`  
		Last Modified: Thu, 02 Feb 2023 21:19:22 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-scratch`

```console
$ docker pull nats@sha256:c926cdb68b698f2bbe658b5dac5353803f29c4cd4e7ab8bdc572077ee8a9f870
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-scratch` - linux; amd64

```console
$ docker pull nats@sha256:b7cd8c3270f038b671b4d55156398eec4387fff96c2de872255d30024bf6a557
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4931647 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b82b64c84efab021cd029f60c01c7e52b53b4eae18827b383f87a4393b3a7095`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 02 Feb 2023 21:33:01 GMT
COPY file:a9e60c6fbbdd9ebb5d2c4deec1df6db6d6a40a0384a5544b6c3386eea2057a54 in /nats-server 
# Thu, 02 Feb 2023 21:33:02 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 02 Feb 2023 21:33:02 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Feb 2023 21:33:02 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 02 Feb 2023 21:33:02 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 02 Feb 2023 21:33:02 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:1cd3edd838903059461e505e0f1e09d3452d5e632e2b550f4d0850b0d2f59c72`  
		Last Modified: Thu, 02 Feb 2023 21:33:50 GMT  
		Size: 4.9 MB (4931138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e56ba114f2531c68c394372ad404aeb5ac8ee8946fb17af7ac704a76697756f`  
		Last Modified: Thu, 02 Feb 2023 21:33:49 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:c1107d0e00f4d8dedfbf7883fbabc7b200545657e1e13495e12453d13dfde328
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4694918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c7de15c41747ca8b98deb9b16e6b45e323bf1b12bfe5ba0617911396006a4fc`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 02 Feb 2023 21:50:29 GMT
COPY file:be32648053f47b33b445bad52bed7ff3e74d1dc77100df4d672e431022428de7 in /nats-server 
# Thu, 02 Feb 2023 21:50:29 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 02 Feb 2023 21:50:29 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Feb 2023 21:50:29 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 02 Feb 2023 21:50:29 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 02 Feb 2023 21:50:29 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:eddbc6c88066991dd5810d3a3b6875ee06eecb063cccc9b0e3d9386c75c4f826`  
		Last Modified: Thu, 02 Feb 2023 21:52:00 GMT  
		Size: 4.7 MB (4694411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:795c72903a6f36672ee81a0386bff46e30e1f3598c7552f5c192f650d82c6e69`  
		Last Modified: Thu, 02 Feb 2023 21:51:59 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:8a3086f469fd77000e1a8618960b722ca85e5cbd69a41190e81286734c7e455a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4688297 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa7e9966ce4e992db69b98063dd7d35d6fe1239100d385115ea7031b9b65978b`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 02 Feb 2023 21:58:12 GMT
COPY file:a67f587b7b86d3c3a85687c0097c93084fb71c44966695879cd46269a36ed31d in /nats-server 
# Thu, 02 Feb 2023 21:58:12 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 02 Feb 2023 21:58:12 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Feb 2023 21:58:12 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 02 Feb 2023 21:58:12 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 02 Feb 2023 21:58:12 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:df148ca425b44984356880f1ed4c1f04d36d2e6efa76ba4043d9dd80fe9f6201`  
		Last Modified: Thu, 02 Feb 2023 21:59:43 GMT  
		Size: 4.7 MB (4687788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b679ac38b5a1c67873f0f08c522aafadecaa085bed163dcc8387ddd53c0509d2`  
		Last Modified: Thu, 02 Feb 2023 21:59:43 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:b33b08f196a8f9b3b612740d36e847c1d5bc5239bf49f768b0056cd2ff7baaf0
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4517074 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:21aad311a08f5e75bd795b33799a8a100d9eb132974428f406329a5871687f79`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 02 Feb 2023 21:47:40 GMT
COPY file:f1194fd7c754730901a7920f7db8ad6e6432e904adfe27cb3bf09f1626eb0b20 in /nats-server 
# Thu, 02 Feb 2023 21:47:40 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 02 Feb 2023 21:47:40 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Feb 2023 21:47:40 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 02 Feb 2023 21:47:40 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 02 Feb 2023 21:47:40 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:0e112ba48caecfa7e51d560718ada0f9c4e686bdc09555df0617055a883e5777`  
		Last Modified: Thu, 02 Feb 2023 21:48:28 GMT  
		Size: 4.5 MB (4516565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fce6348af8f3a9160210d4305f3a6f5c76b1b36d75df166f313f92cf3774f93f`  
		Last Modified: Thu, 02 Feb 2023 21:48:27 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-windowsservercore`

```console
$ docker pull nats@sha256:f0e699db4eb709cfad8009ccb7babc3b5f99ad75b8635428c8a1f4b968f5e1c6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3887; amd64

### `nats:2-windowsservercore` - windows version 10.0.17763.3887; amd64

```console
$ docker pull nats@sha256:21cd0fd5eed31d916b22e6bb32cfd8b17357a90504e876a650dbfe702f7ad4c3
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.7 GB (1713682302 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d6cfbec3abd0c20da1ad583cfeba37afbf93ac199cfd962df9a78badf81c44c5`
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
# Thu, 02 Feb 2023 21:16:27 GMT
ENV NATS_SERVER=2.9.12
# Thu, 02 Feb 2023 21:16:28 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.9.12/nats-server-v2.9.12-windows-amd64.zip
# Thu, 02 Feb 2023 21:16:29 GMT
ENV NATS_SERVER_SHASUM=a87b6715550f0a5f8829dd51923ce6a20c6302227e4ade76c6403f49703ad12f
# Thu, 02 Feb 2023 21:17:00 GMT
RUN Set-PSDebug -Trace 2
# Thu, 02 Feb 2023 21:18:09 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Thu, 02 Feb 2023 21:18:10 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Thu, 02 Feb 2023 21:18:11 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Feb 2023 21:18:12 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 02 Feb 2023 21:18:13 GMT
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
	-	`sha256:fe84adf024fde5f8eff638fb25641740e35f164990a89dc350e955eaac3f822d`  
		Last Modified: Thu, 02 Feb 2023 21:19:08 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3029d4bc864cb72910f78c88e54a6cd47e3ab04772b8281f529243ff7f8dd7b8`  
		Last Modified: Thu, 02 Feb 2023 21:19:08 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d08011b8eb78752d65a736ca9f99d7f77bdec75b80c52b6ebaf1986e91d27e6`  
		Last Modified: Thu, 02 Feb 2023 21:19:08 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1271e50716be60e293a328182a8014b8208316cfab34ae9ca88cca1c1d208f9`  
		Last Modified: Thu, 02 Feb 2023 21:19:08 GMT  
		Size: 382.7 KB (382745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7b8a07a3d2b9a3e07d670ef47f886c71f2dec4186a4b33fda0f4d0cf258cdeb`  
		Last Modified: Thu, 02 Feb 2023 21:19:07 GMT  
		Size: 5.3 MB (5342340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:831ce5e8c2d1c916622590fab5d1aaf7a400134a6df616daf6cfa60889de7d96`  
		Last Modified: Thu, 02 Feb 2023 21:19:06 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfc448b0cbe5f2ad0f9c72fbc2969f5bdc46b0cb3f43838d54cd9f2eb0f7a06b`  
		Last Modified: Thu, 02 Feb 2023 21:19:06 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d976be1bad16d8687a8e24c34fa6db831c074dbc26c19dc49f405a0e663d86b7`  
		Last Modified: Thu, 02 Feb 2023 21:19:06 GMT  
		Size: 1.4 KB (1386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:314a1587606bc3b0f6be6c93d6e597583050cd41304603aa4cb14447f4b6e240`  
		Last Modified: Thu, 02 Feb 2023 21:19:06 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-windowsservercore-1809`

```console
$ docker pull nats@sha256:f0e699db4eb709cfad8009ccb7babc3b5f99ad75b8635428c8a1f4b968f5e1c6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3887; amd64

### `nats:2-windowsservercore-1809` - windows version 10.0.17763.3887; amd64

```console
$ docker pull nats@sha256:21cd0fd5eed31d916b22e6bb32cfd8b17357a90504e876a650dbfe702f7ad4c3
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.7 GB (1713682302 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d6cfbec3abd0c20da1ad583cfeba37afbf93ac199cfd962df9a78badf81c44c5`
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
# Thu, 02 Feb 2023 21:16:27 GMT
ENV NATS_SERVER=2.9.12
# Thu, 02 Feb 2023 21:16:28 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.9.12/nats-server-v2.9.12-windows-amd64.zip
# Thu, 02 Feb 2023 21:16:29 GMT
ENV NATS_SERVER_SHASUM=a87b6715550f0a5f8829dd51923ce6a20c6302227e4ade76c6403f49703ad12f
# Thu, 02 Feb 2023 21:17:00 GMT
RUN Set-PSDebug -Trace 2
# Thu, 02 Feb 2023 21:18:09 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Thu, 02 Feb 2023 21:18:10 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Thu, 02 Feb 2023 21:18:11 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Feb 2023 21:18:12 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 02 Feb 2023 21:18:13 GMT
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
	-	`sha256:fe84adf024fde5f8eff638fb25641740e35f164990a89dc350e955eaac3f822d`  
		Last Modified: Thu, 02 Feb 2023 21:19:08 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3029d4bc864cb72910f78c88e54a6cd47e3ab04772b8281f529243ff7f8dd7b8`  
		Last Modified: Thu, 02 Feb 2023 21:19:08 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d08011b8eb78752d65a736ca9f99d7f77bdec75b80c52b6ebaf1986e91d27e6`  
		Last Modified: Thu, 02 Feb 2023 21:19:08 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1271e50716be60e293a328182a8014b8208316cfab34ae9ca88cca1c1d208f9`  
		Last Modified: Thu, 02 Feb 2023 21:19:08 GMT  
		Size: 382.7 KB (382745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7b8a07a3d2b9a3e07d670ef47f886c71f2dec4186a4b33fda0f4d0cf258cdeb`  
		Last Modified: Thu, 02 Feb 2023 21:19:07 GMT  
		Size: 5.3 MB (5342340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:831ce5e8c2d1c916622590fab5d1aaf7a400134a6df616daf6cfa60889de7d96`  
		Last Modified: Thu, 02 Feb 2023 21:19:06 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfc448b0cbe5f2ad0f9c72fbc2969f5bdc46b0cb3f43838d54cd9f2eb0f7a06b`  
		Last Modified: Thu, 02 Feb 2023 21:19:06 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d976be1bad16d8687a8e24c34fa6db831c074dbc26c19dc49f405a0e663d86b7`  
		Last Modified: Thu, 02 Feb 2023 21:19:06 GMT  
		Size: 1.4 KB (1386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:314a1587606bc3b0f6be6c93d6e597583050cd41304603aa4cb14447f4b6e240`  
		Last Modified: Thu, 02 Feb 2023 21:19:06 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9`

```console
$ docker pull nats@sha256:1fc110ad1583ad4ac948623fbaed53afec34afc4a03d60e23384a5d4479fe22d
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
$ docker pull nats@sha256:b7cd8c3270f038b671b4d55156398eec4387fff96c2de872255d30024bf6a557
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4931647 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b82b64c84efab021cd029f60c01c7e52b53b4eae18827b383f87a4393b3a7095`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 02 Feb 2023 21:33:01 GMT
COPY file:a9e60c6fbbdd9ebb5d2c4deec1df6db6d6a40a0384a5544b6c3386eea2057a54 in /nats-server 
# Thu, 02 Feb 2023 21:33:02 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 02 Feb 2023 21:33:02 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Feb 2023 21:33:02 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 02 Feb 2023 21:33:02 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 02 Feb 2023 21:33:02 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:1cd3edd838903059461e505e0f1e09d3452d5e632e2b550f4d0850b0d2f59c72`  
		Last Modified: Thu, 02 Feb 2023 21:33:50 GMT  
		Size: 4.9 MB (4931138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e56ba114f2531c68c394372ad404aeb5ac8ee8946fb17af7ac704a76697756f`  
		Last Modified: Thu, 02 Feb 2023 21:33:49 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9` - linux; arm variant v6

```console
$ docker pull nats@sha256:c1107d0e00f4d8dedfbf7883fbabc7b200545657e1e13495e12453d13dfde328
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4694918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c7de15c41747ca8b98deb9b16e6b45e323bf1b12bfe5ba0617911396006a4fc`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 02 Feb 2023 21:50:29 GMT
COPY file:be32648053f47b33b445bad52bed7ff3e74d1dc77100df4d672e431022428de7 in /nats-server 
# Thu, 02 Feb 2023 21:50:29 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 02 Feb 2023 21:50:29 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Feb 2023 21:50:29 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 02 Feb 2023 21:50:29 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 02 Feb 2023 21:50:29 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:eddbc6c88066991dd5810d3a3b6875ee06eecb063cccc9b0e3d9386c75c4f826`  
		Last Modified: Thu, 02 Feb 2023 21:52:00 GMT  
		Size: 4.7 MB (4694411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:795c72903a6f36672ee81a0386bff46e30e1f3598c7552f5c192f650d82c6e69`  
		Last Modified: Thu, 02 Feb 2023 21:51:59 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9` - linux; arm variant v7

```console
$ docker pull nats@sha256:8a3086f469fd77000e1a8618960b722ca85e5cbd69a41190e81286734c7e455a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4688297 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa7e9966ce4e992db69b98063dd7d35d6fe1239100d385115ea7031b9b65978b`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 02 Feb 2023 21:58:12 GMT
COPY file:a67f587b7b86d3c3a85687c0097c93084fb71c44966695879cd46269a36ed31d in /nats-server 
# Thu, 02 Feb 2023 21:58:12 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 02 Feb 2023 21:58:12 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Feb 2023 21:58:12 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 02 Feb 2023 21:58:12 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 02 Feb 2023 21:58:12 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:df148ca425b44984356880f1ed4c1f04d36d2e6efa76ba4043d9dd80fe9f6201`  
		Last Modified: Thu, 02 Feb 2023 21:59:43 GMT  
		Size: 4.7 MB (4687788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b679ac38b5a1c67873f0f08c522aafadecaa085bed163dcc8387ddd53c0509d2`  
		Last Modified: Thu, 02 Feb 2023 21:59:43 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:b33b08f196a8f9b3b612740d36e847c1d5bc5239bf49f768b0056cd2ff7baaf0
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4517074 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:21aad311a08f5e75bd795b33799a8a100d9eb132974428f406329a5871687f79`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 02 Feb 2023 21:47:40 GMT
COPY file:f1194fd7c754730901a7920f7db8ad6e6432e904adfe27cb3bf09f1626eb0b20 in /nats-server 
# Thu, 02 Feb 2023 21:47:40 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 02 Feb 2023 21:47:40 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Feb 2023 21:47:40 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 02 Feb 2023 21:47:40 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 02 Feb 2023 21:47:40 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:0e112ba48caecfa7e51d560718ada0f9c4e686bdc09555df0617055a883e5777`  
		Last Modified: Thu, 02 Feb 2023 21:48:28 GMT  
		Size: 4.5 MB (4516565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fce6348af8f3a9160210d4305f3a6f5c76b1b36d75df166f313f92cf3774f93f`  
		Last Modified: Thu, 02 Feb 2023 21:48:27 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9` - windows version 10.0.17763.3887; amd64

```console
$ docker pull nats@sha256:298b8a1b690d1d64fbd955cb251e93b63874ef7d4cb6f0eb2128cb3df82d1ecf
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.7 MB (111657511 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d6d4d57475df3d7d3cc4f4a97791acce1c9ce0aa971eff49258813b2b55ba7c`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 07 Jan 2023 05:17:01 GMT
RUN Apply image 10.0.17763.3887
# Thu, 12 Jan 2023 05:01:51 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Thu, 02 Feb 2023 21:18:29 GMT
RUN cmd /S /C #(nop) COPY file:1d619f9da4aa7d6fe4171f8e7c232a42ba0b813a50cbb3466448bbfaf0fc4a79 in C:\nats-server.exe 
# Thu, 02 Feb 2023 21:18:30 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Thu, 02 Feb 2023 21:18:31 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Thu, 02 Feb 2023 21:18:32 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 02 Feb 2023 21:18:33 GMT
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
	-	`sha256:3801c3e14f4f67451b0f8a1220428a70eeddbf9bdef73cd8b89614087bfea683`  
		Last Modified: Thu, 02 Feb 2023 21:19:24 GMT  
		Size: 5.0 MB (4985010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc3da06a2f05c3cb57b2c4406a7135beaef26938a9d48c94e9bb19f285362f19`  
		Last Modified: Thu, 02 Feb 2023 21:19:22 GMT  
		Size: 1.8 KB (1768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a28bce3ab94f882453c700042d8e7ff6aa55d92a06dad8d04be017d91ec9208`  
		Last Modified: Thu, 02 Feb 2023 21:19:22 GMT  
		Size: 1.2 KB (1173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dba391f32fd738334e9c4d766b67aa8340b1fac87188801d71faf347db92b3fb`  
		Last Modified: Thu, 02 Feb 2023 21:19:22 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d938df46930834c4903622f9028898bde90a5f21c98963408af250b41e05242c`  
		Last Modified: Thu, 02 Feb 2023 21:19:22 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-alpine`

```console
$ docker pull nats@sha256:755bdf0c9fea43659ef9485ff74a9303ac2595c1b02c807d92b53802baf808a6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9-alpine` - linux; amd64

```console
$ docker pull nats@sha256:596442ede179d773ec7f08637e1347328ec3f12ed64568dd29bf8bd92259c84d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.6 MB (8589330 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:36a5b27103c778bd375b40b313ac2dd449b9123b78b3e1933ccf2c24bf0082bb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 09 Jan 2023 17:05:20 GMT
ADD file:e4d600fc4c9c293efe360be7b30ee96579925d1b4634c94332e2ec73f7d8eca1 in / 
# Mon, 09 Jan 2023 17:05:20 GMT
CMD ["/bin/sh"]
# Thu, 02 Feb 2023 21:32:50 GMT
ENV NATS_SERVER=2.9.12
# Thu, 02 Feb 2023 21:32:54 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='296075e7caa33684f0a23ac97c2a904c8f22dbc1d75da4ab443a81aa8b1b765b' ;; 		armhf) natsArch='arm6'; sha256='72af57a620de31e718131736b4ae123acd994295b2f81d1f847cdb9e1e686e63' ;; 		armv7) natsArch='arm7'; sha256='153d823e90b76457b6689cb6baa9f045b3a2152caaec787a0ad77162431949ed' ;; 		x86_64) natsArch='amd64'; sha256='cd05e53b3e1a535dd4e09a4cba3c1b0cd7c512e7f3d68d52ed8e8621dac8c925' ;; 		x86) natsArch='386'; sha256='103d89a231154708375a091dfb86ebe563f3de968a5e6ed14aba4c32e5c77925' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 02 Feb 2023 21:32:54 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 02 Feb 2023 21:32:54 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 02 Feb 2023 21:32:54 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Feb 2023 21:32:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 02 Feb 2023 21:32:54 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:8921db27df2831fa6eaa85321205a2470c669b855f3ec95d5a3c2b46de0442c9`  
		Last Modified: Mon, 09 Jan 2023 17:05:45 GMT  
		Size: 3.4 MB (3370628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90fc2d6058c164e7f06206d5ec77d1dc1a27fbde65facfb00c7be6ebd6c00c9a`  
		Last Modified: Thu, 02 Feb 2023 21:33:28 GMT  
		Size: 5.2 MB (5217701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c8da51ec4a12edfcbb65016c0ab6137e4261542c0806c198a7561573428f286`  
		Last Modified: Thu, 02 Feb 2023 21:33:28 GMT  
		Size: 588.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd8137ab539d1ca45399d4e83b217c0290e34a11f764287427ef7fa51ff209bf`  
		Last Modified: Thu, 02 Feb 2023 21:33:27 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:325775413795f10444c422d2b752494acbd407613fc1537a7cf84693283102a6
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.1 MB (8090427 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c037e626dfdaad2eb7338914f0db6020567bb99c48a7e0f01345484edfa0c7d9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 09 Jan 2023 17:04:54 GMT
ADD file:b15fd8e9f996815394e25f20c8459bfb4c2a8c4074592d6f4c75f4fe79ce537e in / 
# Mon, 09 Jan 2023 17:04:55 GMT
CMD ["/bin/sh"]
# Thu, 02 Feb 2023 21:49:33 GMT
ENV NATS_SERVER=2.9.12
# Thu, 02 Feb 2023 21:50:12 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='296075e7caa33684f0a23ac97c2a904c8f22dbc1d75da4ab443a81aa8b1b765b' ;; 		armhf) natsArch='arm6'; sha256='72af57a620de31e718131736b4ae123acd994295b2f81d1f847cdb9e1e686e63' ;; 		armv7) natsArch='arm7'; sha256='153d823e90b76457b6689cb6baa9f045b3a2152caaec787a0ad77162431949ed' ;; 		x86_64) natsArch='amd64'; sha256='cd05e53b3e1a535dd4e09a4cba3c1b0cd7c512e7f3d68d52ed8e8621dac8c925' ;; 		x86) natsArch='386'; sha256='103d89a231154708375a091dfb86ebe563f3de968a5e6ed14aba4c32e5c77925' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 02 Feb 2023 21:50:12 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 02 Feb 2023 21:50:12 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 02 Feb 2023 21:50:12 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Feb 2023 21:50:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 02 Feb 2023 21:50:13 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:0269c10e600f3a375f36ddabdbd264ce9503a455f0d0969ce8a00f24eaecc032`  
		Last Modified: Mon, 09 Jan 2023 17:05:45 GMT  
		Size: 3.1 MB (3107243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c06b18d184d344d8a89cb092274a39e8c3bf5646c1a8678e53519585c03292b`  
		Last Modified: Thu, 02 Feb 2023 21:51:28 GMT  
		Size: 5.0 MB (4982208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb35f9a15c3a5b93ea2a254cc9c9cc741a6e698dd58741a9f9af4936c2049f03`  
		Last Modified: Thu, 02 Feb 2023 21:51:27 GMT  
		Size: 561.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b92f0e4cdd97e7662fe9c94bd67aabac7172d0e0d97acf0b5c586de7b89f895`  
		Last Modified: Thu, 02 Feb 2023 21:51:27 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:6c2d2b789f9ed0c9edddd86e758373c2c2f76132958d3dec5c2a6d1e7336f9dc
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.8 MB (7841051 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d85fea070aff07d7750af4de5ce3ebb9b49a00738becb1eae53e9281e25aca5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 09 Jan 2023 17:06:27 GMT
ADD file:4696f25d0f019b27457c55b3b128b70bf153f38e3e4eb5bdfc21058543313e94 in / 
# Mon, 09 Jan 2023 17:06:27 GMT
CMD ["/bin/sh"]
# Thu, 02 Feb 2023 21:57:48 GMT
ENV NATS_SERVER=2.9.12
# Thu, 02 Feb 2023 21:57:51 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='296075e7caa33684f0a23ac97c2a904c8f22dbc1d75da4ab443a81aa8b1b765b' ;; 		armhf) natsArch='arm6'; sha256='72af57a620de31e718131736b4ae123acd994295b2f81d1f847cdb9e1e686e63' ;; 		armv7) natsArch='arm7'; sha256='153d823e90b76457b6689cb6baa9f045b3a2152caaec787a0ad77162431949ed' ;; 		x86_64) natsArch='amd64'; sha256='cd05e53b3e1a535dd4e09a4cba3c1b0cd7c512e7f3d68d52ed8e8621dac8c925' ;; 		x86) natsArch='386'; sha256='103d89a231154708375a091dfb86ebe563f3de968a5e6ed14aba4c32e5c77925' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 02 Feb 2023 21:57:51 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 02 Feb 2023 21:57:51 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 02 Feb 2023 21:57:51 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Feb 2023 21:57:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 02 Feb 2023 21:57:52 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:c527615e4ffa2d5b9b777fd469b3b5ba7c1b1e9201c065be2c43569de48a3754`  
		Last Modified: Mon, 09 Jan 2023 17:07:17 GMT  
		Size: 2.9 MB (2865208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54dcdcd84f34ebca9af1574488d3c29f20e5444ee61f4eb8688d3b5b9b1aa829`  
		Last Modified: Thu, 02 Feb 2023 21:59:11 GMT  
		Size: 5.0 MB (4974868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bebca7f9dc77dd081f1e8386b332902935be6eb718e5435056e6928dbdcded07`  
		Last Modified: Thu, 02 Feb 2023 21:59:10 GMT  
		Size: 561.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7247a73a46f57913d3042d8273753dc2524e2b7308a9b7c623043a9f83874df`  
		Last Modified: Thu, 02 Feb 2023 21:59:10 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:3b5d7a8ce580949f91c72ccb764cb0f808ca47f4a306cd2a64adef699b18c709
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.1 MB (8062087 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:72e93fab38c492847947f3360491ff675e9657ddad7fffcd6ddaf34818b3359e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 09 Jan 2023 17:04:48 GMT
ADD file:3080f19f39259a4b77cc53975de0184c78d4335ceb9ffb77a2838d0539ad6f85 in / 
# Mon, 09 Jan 2023 17:04:49 GMT
CMD ["/bin/sh"]
# Thu, 02 Feb 2023 21:47:31 GMT
ENV NATS_SERVER=2.9.12
# Thu, 02 Feb 2023 21:47:34 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='296075e7caa33684f0a23ac97c2a904c8f22dbc1d75da4ab443a81aa8b1b765b' ;; 		armhf) natsArch='arm6'; sha256='72af57a620de31e718131736b4ae123acd994295b2f81d1f847cdb9e1e686e63' ;; 		armv7) natsArch='arm7'; sha256='153d823e90b76457b6689cb6baa9f045b3a2152caaec787a0ad77162431949ed' ;; 		x86_64) natsArch='amd64'; sha256='cd05e53b3e1a535dd4e09a4cba3c1b0cd7c512e7f3d68d52ed8e8621dac8c925' ;; 		x86) natsArch='386'; sha256='103d89a231154708375a091dfb86ebe563f3de968a5e6ed14aba4c32e5c77925' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 02 Feb 2023 21:47:34 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 02 Feb 2023 21:47:34 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 02 Feb 2023 21:47:34 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Feb 2023 21:47:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 02 Feb 2023 21:47:34 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:a9eaa45ef418e883481a13c7d84fa9904f2ec56789c52a87ba5a9e6483f2b74f`  
		Last Modified: Mon, 09 Jan 2023 17:05:12 GMT  
		Size: 3.3 MB (3259241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf7882578303a0fa74c95f3a4d8ba43cb527ab5ae15db2e91420624139809c58`  
		Last Modified: Thu, 02 Feb 2023 21:48:06 GMT  
		Size: 4.8 MB (4801846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02c5fcf7cb836026cb1caf41222a5db286caad4181a1465fbc6a827e539d655f`  
		Last Modified: Thu, 02 Feb 2023 21:48:06 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c842168768b2663567de8311303dd5b2951b867f7c2228af37a24b50f24181ae`  
		Last Modified: Thu, 02 Feb 2023 21:48:05 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-alpine3.17`

```console
$ docker pull nats@sha256:755bdf0c9fea43659ef9485ff74a9303ac2595c1b02c807d92b53802baf808a6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9-alpine3.17` - linux; amd64

```console
$ docker pull nats@sha256:596442ede179d773ec7f08637e1347328ec3f12ed64568dd29bf8bd92259c84d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.6 MB (8589330 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:36a5b27103c778bd375b40b313ac2dd449b9123b78b3e1933ccf2c24bf0082bb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 09 Jan 2023 17:05:20 GMT
ADD file:e4d600fc4c9c293efe360be7b30ee96579925d1b4634c94332e2ec73f7d8eca1 in / 
# Mon, 09 Jan 2023 17:05:20 GMT
CMD ["/bin/sh"]
# Thu, 02 Feb 2023 21:32:50 GMT
ENV NATS_SERVER=2.9.12
# Thu, 02 Feb 2023 21:32:54 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='296075e7caa33684f0a23ac97c2a904c8f22dbc1d75da4ab443a81aa8b1b765b' ;; 		armhf) natsArch='arm6'; sha256='72af57a620de31e718131736b4ae123acd994295b2f81d1f847cdb9e1e686e63' ;; 		armv7) natsArch='arm7'; sha256='153d823e90b76457b6689cb6baa9f045b3a2152caaec787a0ad77162431949ed' ;; 		x86_64) natsArch='amd64'; sha256='cd05e53b3e1a535dd4e09a4cba3c1b0cd7c512e7f3d68d52ed8e8621dac8c925' ;; 		x86) natsArch='386'; sha256='103d89a231154708375a091dfb86ebe563f3de968a5e6ed14aba4c32e5c77925' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 02 Feb 2023 21:32:54 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 02 Feb 2023 21:32:54 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 02 Feb 2023 21:32:54 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Feb 2023 21:32:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 02 Feb 2023 21:32:54 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:8921db27df2831fa6eaa85321205a2470c669b855f3ec95d5a3c2b46de0442c9`  
		Last Modified: Mon, 09 Jan 2023 17:05:45 GMT  
		Size: 3.4 MB (3370628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90fc2d6058c164e7f06206d5ec77d1dc1a27fbde65facfb00c7be6ebd6c00c9a`  
		Last Modified: Thu, 02 Feb 2023 21:33:28 GMT  
		Size: 5.2 MB (5217701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c8da51ec4a12edfcbb65016c0ab6137e4261542c0806c198a7561573428f286`  
		Last Modified: Thu, 02 Feb 2023 21:33:28 GMT  
		Size: 588.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd8137ab539d1ca45399d4e83b217c0290e34a11f764287427ef7fa51ff209bf`  
		Last Modified: Thu, 02 Feb 2023 21:33:27 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-alpine3.17` - linux; arm variant v6

```console
$ docker pull nats@sha256:325775413795f10444c422d2b752494acbd407613fc1537a7cf84693283102a6
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.1 MB (8090427 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c037e626dfdaad2eb7338914f0db6020567bb99c48a7e0f01345484edfa0c7d9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 09 Jan 2023 17:04:54 GMT
ADD file:b15fd8e9f996815394e25f20c8459bfb4c2a8c4074592d6f4c75f4fe79ce537e in / 
# Mon, 09 Jan 2023 17:04:55 GMT
CMD ["/bin/sh"]
# Thu, 02 Feb 2023 21:49:33 GMT
ENV NATS_SERVER=2.9.12
# Thu, 02 Feb 2023 21:50:12 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='296075e7caa33684f0a23ac97c2a904c8f22dbc1d75da4ab443a81aa8b1b765b' ;; 		armhf) natsArch='arm6'; sha256='72af57a620de31e718131736b4ae123acd994295b2f81d1f847cdb9e1e686e63' ;; 		armv7) natsArch='arm7'; sha256='153d823e90b76457b6689cb6baa9f045b3a2152caaec787a0ad77162431949ed' ;; 		x86_64) natsArch='amd64'; sha256='cd05e53b3e1a535dd4e09a4cba3c1b0cd7c512e7f3d68d52ed8e8621dac8c925' ;; 		x86) natsArch='386'; sha256='103d89a231154708375a091dfb86ebe563f3de968a5e6ed14aba4c32e5c77925' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 02 Feb 2023 21:50:12 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 02 Feb 2023 21:50:12 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 02 Feb 2023 21:50:12 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Feb 2023 21:50:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 02 Feb 2023 21:50:13 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:0269c10e600f3a375f36ddabdbd264ce9503a455f0d0969ce8a00f24eaecc032`  
		Last Modified: Mon, 09 Jan 2023 17:05:45 GMT  
		Size: 3.1 MB (3107243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c06b18d184d344d8a89cb092274a39e8c3bf5646c1a8678e53519585c03292b`  
		Last Modified: Thu, 02 Feb 2023 21:51:28 GMT  
		Size: 5.0 MB (4982208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb35f9a15c3a5b93ea2a254cc9c9cc741a6e698dd58741a9f9af4936c2049f03`  
		Last Modified: Thu, 02 Feb 2023 21:51:27 GMT  
		Size: 561.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b92f0e4cdd97e7662fe9c94bd67aabac7172d0e0d97acf0b5c586de7b89f895`  
		Last Modified: Thu, 02 Feb 2023 21:51:27 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-alpine3.17` - linux; arm variant v7

```console
$ docker pull nats@sha256:6c2d2b789f9ed0c9edddd86e758373c2c2f76132958d3dec5c2a6d1e7336f9dc
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.8 MB (7841051 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d85fea070aff07d7750af4de5ce3ebb9b49a00738becb1eae53e9281e25aca5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 09 Jan 2023 17:06:27 GMT
ADD file:4696f25d0f019b27457c55b3b128b70bf153f38e3e4eb5bdfc21058543313e94 in / 
# Mon, 09 Jan 2023 17:06:27 GMT
CMD ["/bin/sh"]
# Thu, 02 Feb 2023 21:57:48 GMT
ENV NATS_SERVER=2.9.12
# Thu, 02 Feb 2023 21:57:51 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='296075e7caa33684f0a23ac97c2a904c8f22dbc1d75da4ab443a81aa8b1b765b' ;; 		armhf) natsArch='arm6'; sha256='72af57a620de31e718131736b4ae123acd994295b2f81d1f847cdb9e1e686e63' ;; 		armv7) natsArch='arm7'; sha256='153d823e90b76457b6689cb6baa9f045b3a2152caaec787a0ad77162431949ed' ;; 		x86_64) natsArch='amd64'; sha256='cd05e53b3e1a535dd4e09a4cba3c1b0cd7c512e7f3d68d52ed8e8621dac8c925' ;; 		x86) natsArch='386'; sha256='103d89a231154708375a091dfb86ebe563f3de968a5e6ed14aba4c32e5c77925' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 02 Feb 2023 21:57:51 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 02 Feb 2023 21:57:51 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 02 Feb 2023 21:57:51 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Feb 2023 21:57:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 02 Feb 2023 21:57:52 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:c527615e4ffa2d5b9b777fd469b3b5ba7c1b1e9201c065be2c43569de48a3754`  
		Last Modified: Mon, 09 Jan 2023 17:07:17 GMT  
		Size: 2.9 MB (2865208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54dcdcd84f34ebca9af1574488d3c29f20e5444ee61f4eb8688d3b5b9b1aa829`  
		Last Modified: Thu, 02 Feb 2023 21:59:11 GMT  
		Size: 5.0 MB (4974868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bebca7f9dc77dd081f1e8386b332902935be6eb718e5435056e6928dbdcded07`  
		Last Modified: Thu, 02 Feb 2023 21:59:10 GMT  
		Size: 561.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7247a73a46f57913d3042d8273753dc2524e2b7308a9b7c623043a9f83874df`  
		Last Modified: Thu, 02 Feb 2023 21:59:10 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-alpine3.17` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:3b5d7a8ce580949f91c72ccb764cb0f808ca47f4a306cd2a64adef699b18c709
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.1 MB (8062087 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:72e93fab38c492847947f3360491ff675e9657ddad7fffcd6ddaf34818b3359e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 09 Jan 2023 17:04:48 GMT
ADD file:3080f19f39259a4b77cc53975de0184c78d4335ceb9ffb77a2838d0539ad6f85 in / 
# Mon, 09 Jan 2023 17:04:49 GMT
CMD ["/bin/sh"]
# Thu, 02 Feb 2023 21:47:31 GMT
ENV NATS_SERVER=2.9.12
# Thu, 02 Feb 2023 21:47:34 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='296075e7caa33684f0a23ac97c2a904c8f22dbc1d75da4ab443a81aa8b1b765b' ;; 		armhf) natsArch='arm6'; sha256='72af57a620de31e718131736b4ae123acd994295b2f81d1f847cdb9e1e686e63' ;; 		armv7) natsArch='arm7'; sha256='153d823e90b76457b6689cb6baa9f045b3a2152caaec787a0ad77162431949ed' ;; 		x86_64) natsArch='amd64'; sha256='cd05e53b3e1a535dd4e09a4cba3c1b0cd7c512e7f3d68d52ed8e8621dac8c925' ;; 		x86) natsArch='386'; sha256='103d89a231154708375a091dfb86ebe563f3de968a5e6ed14aba4c32e5c77925' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 02 Feb 2023 21:47:34 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 02 Feb 2023 21:47:34 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 02 Feb 2023 21:47:34 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Feb 2023 21:47:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 02 Feb 2023 21:47:34 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:a9eaa45ef418e883481a13c7d84fa9904f2ec56789c52a87ba5a9e6483f2b74f`  
		Last Modified: Mon, 09 Jan 2023 17:05:12 GMT  
		Size: 3.3 MB (3259241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf7882578303a0fa74c95f3a4d8ba43cb527ab5ae15db2e91420624139809c58`  
		Last Modified: Thu, 02 Feb 2023 21:48:06 GMT  
		Size: 4.8 MB (4801846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02c5fcf7cb836026cb1caf41222a5db286caad4181a1465fbc6a827e539d655f`  
		Last Modified: Thu, 02 Feb 2023 21:48:06 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c842168768b2663567de8311303dd5b2951b867f7c2228af37a24b50f24181ae`  
		Last Modified: Thu, 02 Feb 2023 21:48:05 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-linux`

```console
$ docker pull nats@sha256:c926cdb68b698f2bbe658b5dac5353803f29c4cd4e7ab8bdc572077ee8a9f870
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9-linux` - linux; amd64

```console
$ docker pull nats@sha256:b7cd8c3270f038b671b4d55156398eec4387fff96c2de872255d30024bf6a557
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4931647 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b82b64c84efab021cd029f60c01c7e52b53b4eae18827b383f87a4393b3a7095`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 02 Feb 2023 21:33:01 GMT
COPY file:a9e60c6fbbdd9ebb5d2c4deec1df6db6d6a40a0384a5544b6c3386eea2057a54 in /nats-server 
# Thu, 02 Feb 2023 21:33:02 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 02 Feb 2023 21:33:02 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Feb 2023 21:33:02 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 02 Feb 2023 21:33:02 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 02 Feb 2023 21:33:02 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:1cd3edd838903059461e505e0f1e09d3452d5e632e2b550f4d0850b0d2f59c72`  
		Last Modified: Thu, 02 Feb 2023 21:33:50 GMT  
		Size: 4.9 MB (4931138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e56ba114f2531c68c394372ad404aeb5ac8ee8946fb17af7ac704a76697756f`  
		Last Modified: Thu, 02 Feb 2023 21:33:49 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:c1107d0e00f4d8dedfbf7883fbabc7b200545657e1e13495e12453d13dfde328
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4694918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c7de15c41747ca8b98deb9b16e6b45e323bf1b12bfe5ba0617911396006a4fc`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 02 Feb 2023 21:50:29 GMT
COPY file:be32648053f47b33b445bad52bed7ff3e74d1dc77100df4d672e431022428de7 in /nats-server 
# Thu, 02 Feb 2023 21:50:29 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 02 Feb 2023 21:50:29 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Feb 2023 21:50:29 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 02 Feb 2023 21:50:29 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 02 Feb 2023 21:50:29 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:eddbc6c88066991dd5810d3a3b6875ee06eecb063cccc9b0e3d9386c75c4f826`  
		Last Modified: Thu, 02 Feb 2023 21:52:00 GMT  
		Size: 4.7 MB (4694411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:795c72903a6f36672ee81a0386bff46e30e1f3598c7552f5c192f650d82c6e69`  
		Last Modified: Thu, 02 Feb 2023 21:51:59 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:8a3086f469fd77000e1a8618960b722ca85e5cbd69a41190e81286734c7e455a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4688297 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa7e9966ce4e992db69b98063dd7d35d6fe1239100d385115ea7031b9b65978b`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 02 Feb 2023 21:58:12 GMT
COPY file:a67f587b7b86d3c3a85687c0097c93084fb71c44966695879cd46269a36ed31d in /nats-server 
# Thu, 02 Feb 2023 21:58:12 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 02 Feb 2023 21:58:12 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Feb 2023 21:58:12 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 02 Feb 2023 21:58:12 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 02 Feb 2023 21:58:12 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:df148ca425b44984356880f1ed4c1f04d36d2e6efa76ba4043d9dd80fe9f6201`  
		Last Modified: Thu, 02 Feb 2023 21:59:43 GMT  
		Size: 4.7 MB (4687788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b679ac38b5a1c67873f0f08c522aafadecaa085bed163dcc8387ddd53c0509d2`  
		Last Modified: Thu, 02 Feb 2023 21:59:43 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:b33b08f196a8f9b3b612740d36e847c1d5bc5239bf49f768b0056cd2ff7baaf0
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4517074 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:21aad311a08f5e75bd795b33799a8a100d9eb132974428f406329a5871687f79`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 02 Feb 2023 21:47:40 GMT
COPY file:f1194fd7c754730901a7920f7db8ad6e6432e904adfe27cb3bf09f1626eb0b20 in /nats-server 
# Thu, 02 Feb 2023 21:47:40 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 02 Feb 2023 21:47:40 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Feb 2023 21:47:40 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 02 Feb 2023 21:47:40 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 02 Feb 2023 21:47:40 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:0e112ba48caecfa7e51d560718ada0f9c4e686bdc09555df0617055a883e5777`  
		Last Modified: Thu, 02 Feb 2023 21:48:28 GMT  
		Size: 4.5 MB (4516565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fce6348af8f3a9160210d4305f3a6f5c76b1b36d75df166f313f92cf3774f93f`  
		Last Modified: Thu, 02 Feb 2023 21:48:27 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-nanoserver`

```console
$ docker pull nats@sha256:853807ebafaad1d9a9ffee4521ea63cb1f171fe4e34262749cc13a71f59c1090
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3887; amd64

### `nats:2.9-nanoserver` - windows version 10.0.17763.3887; amd64

```console
$ docker pull nats@sha256:298b8a1b690d1d64fbd955cb251e93b63874ef7d4cb6f0eb2128cb3df82d1ecf
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.7 MB (111657511 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d6d4d57475df3d7d3cc4f4a97791acce1c9ce0aa971eff49258813b2b55ba7c`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 07 Jan 2023 05:17:01 GMT
RUN Apply image 10.0.17763.3887
# Thu, 12 Jan 2023 05:01:51 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Thu, 02 Feb 2023 21:18:29 GMT
RUN cmd /S /C #(nop) COPY file:1d619f9da4aa7d6fe4171f8e7c232a42ba0b813a50cbb3466448bbfaf0fc4a79 in C:\nats-server.exe 
# Thu, 02 Feb 2023 21:18:30 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Thu, 02 Feb 2023 21:18:31 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Thu, 02 Feb 2023 21:18:32 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 02 Feb 2023 21:18:33 GMT
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
	-	`sha256:3801c3e14f4f67451b0f8a1220428a70eeddbf9bdef73cd8b89614087bfea683`  
		Last Modified: Thu, 02 Feb 2023 21:19:24 GMT  
		Size: 5.0 MB (4985010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc3da06a2f05c3cb57b2c4406a7135beaef26938a9d48c94e9bb19f285362f19`  
		Last Modified: Thu, 02 Feb 2023 21:19:22 GMT  
		Size: 1.8 KB (1768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a28bce3ab94f882453c700042d8e7ff6aa55d92a06dad8d04be017d91ec9208`  
		Last Modified: Thu, 02 Feb 2023 21:19:22 GMT  
		Size: 1.2 KB (1173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dba391f32fd738334e9c4d766b67aa8340b1fac87188801d71faf347db92b3fb`  
		Last Modified: Thu, 02 Feb 2023 21:19:22 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d938df46930834c4903622f9028898bde90a5f21c98963408af250b41e05242c`  
		Last Modified: Thu, 02 Feb 2023 21:19:22 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-nanoserver-1809`

```console
$ docker pull nats@sha256:853807ebafaad1d9a9ffee4521ea63cb1f171fe4e34262749cc13a71f59c1090
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3887; amd64

### `nats:2.9-nanoserver-1809` - windows version 10.0.17763.3887; amd64

```console
$ docker pull nats@sha256:298b8a1b690d1d64fbd955cb251e93b63874ef7d4cb6f0eb2128cb3df82d1ecf
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.7 MB (111657511 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d6d4d57475df3d7d3cc4f4a97791acce1c9ce0aa971eff49258813b2b55ba7c`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 07 Jan 2023 05:17:01 GMT
RUN Apply image 10.0.17763.3887
# Thu, 12 Jan 2023 05:01:51 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Thu, 02 Feb 2023 21:18:29 GMT
RUN cmd /S /C #(nop) COPY file:1d619f9da4aa7d6fe4171f8e7c232a42ba0b813a50cbb3466448bbfaf0fc4a79 in C:\nats-server.exe 
# Thu, 02 Feb 2023 21:18:30 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Thu, 02 Feb 2023 21:18:31 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Thu, 02 Feb 2023 21:18:32 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 02 Feb 2023 21:18:33 GMT
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
	-	`sha256:3801c3e14f4f67451b0f8a1220428a70eeddbf9bdef73cd8b89614087bfea683`  
		Last Modified: Thu, 02 Feb 2023 21:19:24 GMT  
		Size: 5.0 MB (4985010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc3da06a2f05c3cb57b2c4406a7135beaef26938a9d48c94e9bb19f285362f19`  
		Last Modified: Thu, 02 Feb 2023 21:19:22 GMT  
		Size: 1.8 KB (1768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a28bce3ab94f882453c700042d8e7ff6aa55d92a06dad8d04be017d91ec9208`  
		Last Modified: Thu, 02 Feb 2023 21:19:22 GMT  
		Size: 1.2 KB (1173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dba391f32fd738334e9c4d766b67aa8340b1fac87188801d71faf347db92b3fb`  
		Last Modified: Thu, 02 Feb 2023 21:19:22 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d938df46930834c4903622f9028898bde90a5f21c98963408af250b41e05242c`  
		Last Modified: Thu, 02 Feb 2023 21:19:22 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-scratch`

```console
$ docker pull nats@sha256:c926cdb68b698f2bbe658b5dac5353803f29c4cd4e7ab8bdc572077ee8a9f870
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9-scratch` - linux; amd64

```console
$ docker pull nats@sha256:b7cd8c3270f038b671b4d55156398eec4387fff96c2de872255d30024bf6a557
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4931647 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b82b64c84efab021cd029f60c01c7e52b53b4eae18827b383f87a4393b3a7095`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 02 Feb 2023 21:33:01 GMT
COPY file:a9e60c6fbbdd9ebb5d2c4deec1df6db6d6a40a0384a5544b6c3386eea2057a54 in /nats-server 
# Thu, 02 Feb 2023 21:33:02 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 02 Feb 2023 21:33:02 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Feb 2023 21:33:02 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 02 Feb 2023 21:33:02 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 02 Feb 2023 21:33:02 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:1cd3edd838903059461e505e0f1e09d3452d5e632e2b550f4d0850b0d2f59c72`  
		Last Modified: Thu, 02 Feb 2023 21:33:50 GMT  
		Size: 4.9 MB (4931138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e56ba114f2531c68c394372ad404aeb5ac8ee8946fb17af7ac704a76697756f`  
		Last Modified: Thu, 02 Feb 2023 21:33:49 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:c1107d0e00f4d8dedfbf7883fbabc7b200545657e1e13495e12453d13dfde328
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4694918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c7de15c41747ca8b98deb9b16e6b45e323bf1b12bfe5ba0617911396006a4fc`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 02 Feb 2023 21:50:29 GMT
COPY file:be32648053f47b33b445bad52bed7ff3e74d1dc77100df4d672e431022428de7 in /nats-server 
# Thu, 02 Feb 2023 21:50:29 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 02 Feb 2023 21:50:29 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Feb 2023 21:50:29 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 02 Feb 2023 21:50:29 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 02 Feb 2023 21:50:29 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:eddbc6c88066991dd5810d3a3b6875ee06eecb063cccc9b0e3d9386c75c4f826`  
		Last Modified: Thu, 02 Feb 2023 21:52:00 GMT  
		Size: 4.7 MB (4694411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:795c72903a6f36672ee81a0386bff46e30e1f3598c7552f5c192f650d82c6e69`  
		Last Modified: Thu, 02 Feb 2023 21:51:59 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:8a3086f469fd77000e1a8618960b722ca85e5cbd69a41190e81286734c7e455a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4688297 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa7e9966ce4e992db69b98063dd7d35d6fe1239100d385115ea7031b9b65978b`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 02 Feb 2023 21:58:12 GMT
COPY file:a67f587b7b86d3c3a85687c0097c93084fb71c44966695879cd46269a36ed31d in /nats-server 
# Thu, 02 Feb 2023 21:58:12 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 02 Feb 2023 21:58:12 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Feb 2023 21:58:12 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 02 Feb 2023 21:58:12 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 02 Feb 2023 21:58:12 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:df148ca425b44984356880f1ed4c1f04d36d2e6efa76ba4043d9dd80fe9f6201`  
		Last Modified: Thu, 02 Feb 2023 21:59:43 GMT  
		Size: 4.7 MB (4687788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b679ac38b5a1c67873f0f08c522aafadecaa085bed163dcc8387ddd53c0509d2`  
		Last Modified: Thu, 02 Feb 2023 21:59:43 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:b33b08f196a8f9b3b612740d36e847c1d5bc5239bf49f768b0056cd2ff7baaf0
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4517074 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:21aad311a08f5e75bd795b33799a8a100d9eb132974428f406329a5871687f79`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 02 Feb 2023 21:47:40 GMT
COPY file:f1194fd7c754730901a7920f7db8ad6e6432e904adfe27cb3bf09f1626eb0b20 in /nats-server 
# Thu, 02 Feb 2023 21:47:40 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 02 Feb 2023 21:47:40 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Feb 2023 21:47:40 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 02 Feb 2023 21:47:40 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 02 Feb 2023 21:47:40 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:0e112ba48caecfa7e51d560718ada0f9c4e686bdc09555df0617055a883e5777`  
		Last Modified: Thu, 02 Feb 2023 21:48:28 GMT  
		Size: 4.5 MB (4516565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fce6348af8f3a9160210d4305f3a6f5c76b1b36d75df166f313f92cf3774f93f`  
		Last Modified: Thu, 02 Feb 2023 21:48:27 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-windowsservercore`

```console
$ docker pull nats@sha256:f0e699db4eb709cfad8009ccb7babc3b5f99ad75b8635428c8a1f4b968f5e1c6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3887; amd64

### `nats:2.9-windowsservercore` - windows version 10.0.17763.3887; amd64

```console
$ docker pull nats@sha256:21cd0fd5eed31d916b22e6bb32cfd8b17357a90504e876a650dbfe702f7ad4c3
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.7 GB (1713682302 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d6cfbec3abd0c20da1ad583cfeba37afbf93ac199cfd962df9a78badf81c44c5`
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
# Thu, 02 Feb 2023 21:16:27 GMT
ENV NATS_SERVER=2.9.12
# Thu, 02 Feb 2023 21:16:28 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.9.12/nats-server-v2.9.12-windows-amd64.zip
# Thu, 02 Feb 2023 21:16:29 GMT
ENV NATS_SERVER_SHASUM=a87b6715550f0a5f8829dd51923ce6a20c6302227e4ade76c6403f49703ad12f
# Thu, 02 Feb 2023 21:17:00 GMT
RUN Set-PSDebug -Trace 2
# Thu, 02 Feb 2023 21:18:09 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Thu, 02 Feb 2023 21:18:10 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Thu, 02 Feb 2023 21:18:11 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Feb 2023 21:18:12 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 02 Feb 2023 21:18:13 GMT
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
	-	`sha256:fe84adf024fde5f8eff638fb25641740e35f164990a89dc350e955eaac3f822d`  
		Last Modified: Thu, 02 Feb 2023 21:19:08 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3029d4bc864cb72910f78c88e54a6cd47e3ab04772b8281f529243ff7f8dd7b8`  
		Last Modified: Thu, 02 Feb 2023 21:19:08 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d08011b8eb78752d65a736ca9f99d7f77bdec75b80c52b6ebaf1986e91d27e6`  
		Last Modified: Thu, 02 Feb 2023 21:19:08 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1271e50716be60e293a328182a8014b8208316cfab34ae9ca88cca1c1d208f9`  
		Last Modified: Thu, 02 Feb 2023 21:19:08 GMT  
		Size: 382.7 KB (382745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7b8a07a3d2b9a3e07d670ef47f886c71f2dec4186a4b33fda0f4d0cf258cdeb`  
		Last Modified: Thu, 02 Feb 2023 21:19:07 GMT  
		Size: 5.3 MB (5342340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:831ce5e8c2d1c916622590fab5d1aaf7a400134a6df616daf6cfa60889de7d96`  
		Last Modified: Thu, 02 Feb 2023 21:19:06 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfc448b0cbe5f2ad0f9c72fbc2969f5bdc46b0cb3f43838d54cd9f2eb0f7a06b`  
		Last Modified: Thu, 02 Feb 2023 21:19:06 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d976be1bad16d8687a8e24c34fa6db831c074dbc26c19dc49f405a0e663d86b7`  
		Last Modified: Thu, 02 Feb 2023 21:19:06 GMT  
		Size: 1.4 KB (1386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:314a1587606bc3b0f6be6c93d6e597583050cd41304603aa4cb14447f4b6e240`  
		Last Modified: Thu, 02 Feb 2023 21:19:06 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-windowsservercore-1809`

```console
$ docker pull nats@sha256:f0e699db4eb709cfad8009ccb7babc3b5f99ad75b8635428c8a1f4b968f5e1c6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3887; amd64

### `nats:2.9-windowsservercore-1809` - windows version 10.0.17763.3887; amd64

```console
$ docker pull nats@sha256:21cd0fd5eed31d916b22e6bb32cfd8b17357a90504e876a650dbfe702f7ad4c3
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.7 GB (1713682302 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d6cfbec3abd0c20da1ad583cfeba37afbf93ac199cfd962df9a78badf81c44c5`
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
# Thu, 02 Feb 2023 21:16:27 GMT
ENV NATS_SERVER=2.9.12
# Thu, 02 Feb 2023 21:16:28 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.9.12/nats-server-v2.9.12-windows-amd64.zip
# Thu, 02 Feb 2023 21:16:29 GMT
ENV NATS_SERVER_SHASUM=a87b6715550f0a5f8829dd51923ce6a20c6302227e4ade76c6403f49703ad12f
# Thu, 02 Feb 2023 21:17:00 GMT
RUN Set-PSDebug -Trace 2
# Thu, 02 Feb 2023 21:18:09 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Thu, 02 Feb 2023 21:18:10 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Thu, 02 Feb 2023 21:18:11 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Feb 2023 21:18:12 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 02 Feb 2023 21:18:13 GMT
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
	-	`sha256:fe84adf024fde5f8eff638fb25641740e35f164990a89dc350e955eaac3f822d`  
		Last Modified: Thu, 02 Feb 2023 21:19:08 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3029d4bc864cb72910f78c88e54a6cd47e3ab04772b8281f529243ff7f8dd7b8`  
		Last Modified: Thu, 02 Feb 2023 21:19:08 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d08011b8eb78752d65a736ca9f99d7f77bdec75b80c52b6ebaf1986e91d27e6`  
		Last Modified: Thu, 02 Feb 2023 21:19:08 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1271e50716be60e293a328182a8014b8208316cfab34ae9ca88cca1c1d208f9`  
		Last Modified: Thu, 02 Feb 2023 21:19:08 GMT  
		Size: 382.7 KB (382745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7b8a07a3d2b9a3e07d670ef47f886c71f2dec4186a4b33fda0f4d0cf258cdeb`  
		Last Modified: Thu, 02 Feb 2023 21:19:07 GMT  
		Size: 5.3 MB (5342340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:831ce5e8c2d1c916622590fab5d1aaf7a400134a6df616daf6cfa60889de7d96`  
		Last Modified: Thu, 02 Feb 2023 21:19:06 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfc448b0cbe5f2ad0f9c72fbc2969f5bdc46b0cb3f43838d54cd9f2eb0f7a06b`  
		Last Modified: Thu, 02 Feb 2023 21:19:06 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d976be1bad16d8687a8e24c34fa6db831c074dbc26c19dc49f405a0e663d86b7`  
		Last Modified: Thu, 02 Feb 2023 21:19:06 GMT  
		Size: 1.4 KB (1386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:314a1587606bc3b0f6be6c93d6e597583050cd41304603aa4cb14447f4b6e240`  
		Last Modified: Thu, 02 Feb 2023 21:19:06 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.14`

**does not exist** (yet?)

## `nats:2.9.14-alpine`

**does not exist** (yet?)

## `nats:2.9.14-alpine3.17`

**does not exist** (yet?)

## `nats:2.9.14-linux`

**does not exist** (yet?)

## `nats:2.9.14-nanoserver`

**does not exist** (yet?)

## `nats:2.9.14-nanoserver-1809`

**does not exist** (yet?)

## `nats:2.9.14-scratch`

**does not exist** (yet?)

## `nats:2.9.14-windowsservercore`

**does not exist** (yet?)

## `nats:2.9.14-windowsservercore-1809`

**does not exist** (yet?)

## `nats:alpine`

```console
$ docker pull nats@sha256:755bdf0c9fea43659ef9485ff74a9303ac2595c1b02c807d92b53802baf808a6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:alpine` - linux; amd64

```console
$ docker pull nats@sha256:596442ede179d773ec7f08637e1347328ec3f12ed64568dd29bf8bd92259c84d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.6 MB (8589330 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:36a5b27103c778bd375b40b313ac2dd449b9123b78b3e1933ccf2c24bf0082bb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 09 Jan 2023 17:05:20 GMT
ADD file:e4d600fc4c9c293efe360be7b30ee96579925d1b4634c94332e2ec73f7d8eca1 in / 
# Mon, 09 Jan 2023 17:05:20 GMT
CMD ["/bin/sh"]
# Thu, 02 Feb 2023 21:32:50 GMT
ENV NATS_SERVER=2.9.12
# Thu, 02 Feb 2023 21:32:54 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='296075e7caa33684f0a23ac97c2a904c8f22dbc1d75da4ab443a81aa8b1b765b' ;; 		armhf) natsArch='arm6'; sha256='72af57a620de31e718131736b4ae123acd994295b2f81d1f847cdb9e1e686e63' ;; 		armv7) natsArch='arm7'; sha256='153d823e90b76457b6689cb6baa9f045b3a2152caaec787a0ad77162431949ed' ;; 		x86_64) natsArch='amd64'; sha256='cd05e53b3e1a535dd4e09a4cba3c1b0cd7c512e7f3d68d52ed8e8621dac8c925' ;; 		x86) natsArch='386'; sha256='103d89a231154708375a091dfb86ebe563f3de968a5e6ed14aba4c32e5c77925' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 02 Feb 2023 21:32:54 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 02 Feb 2023 21:32:54 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 02 Feb 2023 21:32:54 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Feb 2023 21:32:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 02 Feb 2023 21:32:54 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:8921db27df2831fa6eaa85321205a2470c669b855f3ec95d5a3c2b46de0442c9`  
		Last Modified: Mon, 09 Jan 2023 17:05:45 GMT  
		Size: 3.4 MB (3370628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90fc2d6058c164e7f06206d5ec77d1dc1a27fbde65facfb00c7be6ebd6c00c9a`  
		Last Modified: Thu, 02 Feb 2023 21:33:28 GMT  
		Size: 5.2 MB (5217701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c8da51ec4a12edfcbb65016c0ab6137e4261542c0806c198a7561573428f286`  
		Last Modified: Thu, 02 Feb 2023 21:33:28 GMT  
		Size: 588.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd8137ab539d1ca45399d4e83b217c0290e34a11f764287427ef7fa51ff209bf`  
		Last Modified: Thu, 02 Feb 2023 21:33:27 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:325775413795f10444c422d2b752494acbd407613fc1537a7cf84693283102a6
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.1 MB (8090427 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c037e626dfdaad2eb7338914f0db6020567bb99c48a7e0f01345484edfa0c7d9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 09 Jan 2023 17:04:54 GMT
ADD file:b15fd8e9f996815394e25f20c8459bfb4c2a8c4074592d6f4c75f4fe79ce537e in / 
# Mon, 09 Jan 2023 17:04:55 GMT
CMD ["/bin/sh"]
# Thu, 02 Feb 2023 21:49:33 GMT
ENV NATS_SERVER=2.9.12
# Thu, 02 Feb 2023 21:50:12 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='296075e7caa33684f0a23ac97c2a904c8f22dbc1d75da4ab443a81aa8b1b765b' ;; 		armhf) natsArch='arm6'; sha256='72af57a620de31e718131736b4ae123acd994295b2f81d1f847cdb9e1e686e63' ;; 		armv7) natsArch='arm7'; sha256='153d823e90b76457b6689cb6baa9f045b3a2152caaec787a0ad77162431949ed' ;; 		x86_64) natsArch='amd64'; sha256='cd05e53b3e1a535dd4e09a4cba3c1b0cd7c512e7f3d68d52ed8e8621dac8c925' ;; 		x86) natsArch='386'; sha256='103d89a231154708375a091dfb86ebe563f3de968a5e6ed14aba4c32e5c77925' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 02 Feb 2023 21:50:12 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 02 Feb 2023 21:50:12 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 02 Feb 2023 21:50:12 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Feb 2023 21:50:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 02 Feb 2023 21:50:13 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:0269c10e600f3a375f36ddabdbd264ce9503a455f0d0969ce8a00f24eaecc032`  
		Last Modified: Mon, 09 Jan 2023 17:05:45 GMT  
		Size: 3.1 MB (3107243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c06b18d184d344d8a89cb092274a39e8c3bf5646c1a8678e53519585c03292b`  
		Last Modified: Thu, 02 Feb 2023 21:51:28 GMT  
		Size: 5.0 MB (4982208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb35f9a15c3a5b93ea2a254cc9c9cc741a6e698dd58741a9f9af4936c2049f03`  
		Last Modified: Thu, 02 Feb 2023 21:51:27 GMT  
		Size: 561.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b92f0e4cdd97e7662fe9c94bd67aabac7172d0e0d97acf0b5c586de7b89f895`  
		Last Modified: Thu, 02 Feb 2023 21:51:27 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:6c2d2b789f9ed0c9edddd86e758373c2c2f76132958d3dec5c2a6d1e7336f9dc
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.8 MB (7841051 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d85fea070aff07d7750af4de5ce3ebb9b49a00738becb1eae53e9281e25aca5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 09 Jan 2023 17:06:27 GMT
ADD file:4696f25d0f019b27457c55b3b128b70bf153f38e3e4eb5bdfc21058543313e94 in / 
# Mon, 09 Jan 2023 17:06:27 GMT
CMD ["/bin/sh"]
# Thu, 02 Feb 2023 21:57:48 GMT
ENV NATS_SERVER=2.9.12
# Thu, 02 Feb 2023 21:57:51 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='296075e7caa33684f0a23ac97c2a904c8f22dbc1d75da4ab443a81aa8b1b765b' ;; 		armhf) natsArch='arm6'; sha256='72af57a620de31e718131736b4ae123acd994295b2f81d1f847cdb9e1e686e63' ;; 		armv7) natsArch='arm7'; sha256='153d823e90b76457b6689cb6baa9f045b3a2152caaec787a0ad77162431949ed' ;; 		x86_64) natsArch='amd64'; sha256='cd05e53b3e1a535dd4e09a4cba3c1b0cd7c512e7f3d68d52ed8e8621dac8c925' ;; 		x86) natsArch='386'; sha256='103d89a231154708375a091dfb86ebe563f3de968a5e6ed14aba4c32e5c77925' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 02 Feb 2023 21:57:51 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 02 Feb 2023 21:57:51 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 02 Feb 2023 21:57:51 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Feb 2023 21:57:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 02 Feb 2023 21:57:52 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:c527615e4ffa2d5b9b777fd469b3b5ba7c1b1e9201c065be2c43569de48a3754`  
		Last Modified: Mon, 09 Jan 2023 17:07:17 GMT  
		Size: 2.9 MB (2865208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54dcdcd84f34ebca9af1574488d3c29f20e5444ee61f4eb8688d3b5b9b1aa829`  
		Last Modified: Thu, 02 Feb 2023 21:59:11 GMT  
		Size: 5.0 MB (4974868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bebca7f9dc77dd081f1e8386b332902935be6eb718e5435056e6928dbdcded07`  
		Last Modified: Thu, 02 Feb 2023 21:59:10 GMT  
		Size: 561.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7247a73a46f57913d3042d8273753dc2524e2b7308a9b7c623043a9f83874df`  
		Last Modified: Thu, 02 Feb 2023 21:59:10 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:3b5d7a8ce580949f91c72ccb764cb0f808ca47f4a306cd2a64adef699b18c709
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.1 MB (8062087 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:72e93fab38c492847947f3360491ff675e9657ddad7fffcd6ddaf34818b3359e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 09 Jan 2023 17:04:48 GMT
ADD file:3080f19f39259a4b77cc53975de0184c78d4335ceb9ffb77a2838d0539ad6f85 in / 
# Mon, 09 Jan 2023 17:04:49 GMT
CMD ["/bin/sh"]
# Thu, 02 Feb 2023 21:47:31 GMT
ENV NATS_SERVER=2.9.12
# Thu, 02 Feb 2023 21:47:34 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='296075e7caa33684f0a23ac97c2a904c8f22dbc1d75da4ab443a81aa8b1b765b' ;; 		armhf) natsArch='arm6'; sha256='72af57a620de31e718131736b4ae123acd994295b2f81d1f847cdb9e1e686e63' ;; 		armv7) natsArch='arm7'; sha256='153d823e90b76457b6689cb6baa9f045b3a2152caaec787a0ad77162431949ed' ;; 		x86_64) natsArch='amd64'; sha256='cd05e53b3e1a535dd4e09a4cba3c1b0cd7c512e7f3d68d52ed8e8621dac8c925' ;; 		x86) natsArch='386'; sha256='103d89a231154708375a091dfb86ebe563f3de968a5e6ed14aba4c32e5c77925' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 02 Feb 2023 21:47:34 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 02 Feb 2023 21:47:34 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 02 Feb 2023 21:47:34 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Feb 2023 21:47:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 02 Feb 2023 21:47:34 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:a9eaa45ef418e883481a13c7d84fa9904f2ec56789c52a87ba5a9e6483f2b74f`  
		Last Modified: Mon, 09 Jan 2023 17:05:12 GMT  
		Size: 3.3 MB (3259241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf7882578303a0fa74c95f3a4d8ba43cb527ab5ae15db2e91420624139809c58`  
		Last Modified: Thu, 02 Feb 2023 21:48:06 GMT  
		Size: 4.8 MB (4801846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02c5fcf7cb836026cb1caf41222a5db286caad4181a1465fbc6a827e539d655f`  
		Last Modified: Thu, 02 Feb 2023 21:48:06 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c842168768b2663567de8311303dd5b2951b867f7c2228af37a24b50f24181ae`  
		Last Modified: Thu, 02 Feb 2023 21:48:05 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:alpine3.17`

```console
$ docker pull nats@sha256:755bdf0c9fea43659ef9485ff74a9303ac2595c1b02c807d92b53802baf808a6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:alpine3.17` - linux; amd64

```console
$ docker pull nats@sha256:596442ede179d773ec7f08637e1347328ec3f12ed64568dd29bf8bd92259c84d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.6 MB (8589330 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:36a5b27103c778bd375b40b313ac2dd449b9123b78b3e1933ccf2c24bf0082bb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 09 Jan 2023 17:05:20 GMT
ADD file:e4d600fc4c9c293efe360be7b30ee96579925d1b4634c94332e2ec73f7d8eca1 in / 
# Mon, 09 Jan 2023 17:05:20 GMT
CMD ["/bin/sh"]
# Thu, 02 Feb 2023 21:32:50 GMT
ENV NATS_SERVER=2.9.12
# Thu, 02 Feb 2023 21:32:54 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='296075e7caa33684f0a23ac97c2a904c8f22dbc1d75da4ab443a81aa8b1b765b' ;; 		armhf) natsArch='arm6'; sha256='72af57a620de31e718131736b4ae123acd994295b2f81d1f847cdb9e1e686e63' ;; 		armv7) natsArch='arm7'; sha256='153d823e90b76457b6689cb6baa9f045b3a2152caaec787a0ad77162431949ed' ;; 		x86_64) natsArch='amd64'; sha256='cd05e53b3e1a535dd4e09a4cba3c1b0cd7c512e7f3d68d52ed8e8621dac8c925' ;; 		x86) natsArch='386'; sha256='103d89a231154708375a091dfb86ebe563f3de968a5e6ed14aba4c32e5c77925' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 02 Feb 2023 21:32:54 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 02 Feb 2023 21:32:54 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 02 Feb 2023 21:32:54 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Feb 2023 21:32:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 02 Feb 2023 21:32:54 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:8921db27df2831fa6eaa85321205a2470c669b855f3ec95d5a3c2b46de0442c9`  
		Last Modified: Mon, 09 Jan 2023 17:05:45 GMT  
		Size: 3.4 MB (3370628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90fc2d6058c164e7f06206d5ec77d1dc1a27fbde65facfb00c7be6ebd6c00c9a`  
		Last Modified: Thu, 02 Feb 2023 21:33:28 GMT  
		Size: 5.2 MB (5217701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c8da51ec4a12edfcbb65016c0ab6137e4261542c0806c198a7561573428f286`  
		Last Modified: Thu, 02 Feb 2023 21:33:28 GMT  
		Size: 588.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd8137ab539d1ca45399d4e83b217c0290e34a11f764287427ef7fa51ff209bf`  
		Last Modified: Thu, 02 Feb 2023 21:33:27 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.17` - linux; arm variant v6

```console
$ docker pull nats@sha256:325775413795f10444c422d2b752494acbd407613fc1537a7cf84693283102a6
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.1 MB (8090427 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c037e626dfdaad2eb7338914f0db6020567bb99c48a7e0f01345484edfa0c7d9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 09 Jan 2023 17:04:54 GMT
ADD file:b15fd8e9f996815394e25f20c8459bfb4c2a8c4074592d6f4c75f4fe79ce537e in / 
# Mon, 09 Jan 2023 17:04:55 GMT
CMD ["/bin/sh"]
# Thu, 02 Feb 2023 21:49:33 GMT
ENV NATS_SERVER=2.9.12
# Thu, 02 Feb 2023 21:50:12 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='296075e7caa33684f0a23ac97c2a904c8f22dbc1d75da4ab443a81aa8b1b765b' ;; 		armhf) natsArch='arm6'; sha256='72af57a620de31e718131736b4ae123acd994295b2f81d1f847cdb9e1e686e63' ;; 		armv7) natsArch='arm7'; sha256='153d823e90b76457b6689cb6baa9f045b3a2152caaec787a0ad77162431949ed' ;; 		x86_64) natsArch='amd64'; sha256='cd05e53b3e1a535dd4e09a4cba3c1b0cd7c512e7f3d68d52ed8e8621dac8c925' ;; 		x86) natsArch='386'; sha256='103d89a231154708375a091dfb86ebe563f3de968a5e6ed14aba4c32e5c77925' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 02 Feb 2023 21:50:12 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 02 Feb 2023 21:50:12 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 02 Feb 2023 21:50:12 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Feb 2023 21:50:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 02 Feb 2023 21:50:13 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:0269c10e600f3a375f36ddabdbd264ce9503a455f0d0969ce8a00f24eaecc032`  
		Last Modified: Mon, 09 Jan 2023 17:05:45 GMT  
		Size: 3.1 MB (3107243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c06b18d184d344d8a89cb092274a39e8c3bf5646c1a8678e53519585c03292b`  
		Last Modified: Thu, 02 Feb 2023 21:51:28 GMT  
		Size: 5.0 MB (4982208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb35f9a15c3a5b93ea2a254cc9c9cc741a6e698dd58741a9f9af4936c2049f03`  
		Last Modified: Thu, 02 Feb 2023 21:51:27 GMT  
		Size: 561.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b92f0e4cdd97e7662fe9c94bd67aabac7172d0e0d97acf0b5c586de7b89f895`  
		Last Modified: Thu, 02 Feb 2023 21:51:27 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.17` - linux; arm variant v7

```console
$ docker pull nats@sha256:6c2d2b789f9ed0c9edddd86e758373c2c2f76132958d3dec5c2a6d1e7336f9dc
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.8 MB (7841051 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d85fea070aff07d7750af4de5ce3ebb9b49a00738becb1eae53e9281e25aca5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 09 Jan 2023 17:06:27 GMT
ADD file:4696f25d0f019b27457c55b3b128b70bf153f38e3e4eb5bdfc21058543313e94 in / 
# Mon, 09 Jan 2023 17:06:27 GMT
CMD ["/bin/sh"]
# Thu, 02 Feb 2023 21:57:48 GMT
ENV NATS_SERVER=2.9.12
# Thu, 02 Feb 2023 21:57:51 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='296075e7caa33684f0a23ac97c2a904c8f22dbc1d75da4ab443a81aa8b1b765b' ;; 		armhf) natsArch='arm6'; sha256='72af57a620de31e718131736b4ae123acd994295b2f81d1f847cdb9e1e686e63' ;; 		armv7) natsArch='arm7'; sha256='153d823e90b76457b6689cb6baa9f045b3a2152caaec787a0ad77162431949ed' ;; 		x86_64) natsArch='amd64'; sha256='cd05e53b3e1a535dd4e09a4cba3c1b0cd7c512e7f3d68d52ed8e8621dac8c925' ;; 		x86) natsArch='386'; sha256='103d89a231154708375a091dfb86ebe563f3de968a5e6ed14aba4c32e5c77925' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 02 Feb 2023 21:57:51 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 02 Feb 2023 21:57:51 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 02 Feb 2023 21:57:51 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Feb 2023 21:57:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 02 Feb 2023 21:57:52 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:c527615e4ffa2d5b9b777fd469b3b5ba7c1b1e9201c065be2c43569de48a3754`  
		Last Modified: Mon, 09 Jan 2023 17:07:17 GMT  
		Size: 2.9 MB (2865208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54dcdcd84f34ebca9af1574488d3c29f20e5444ee61f4eb8688d3b5b9b1aa829`  
		Last Modified: Thu, 02 Feb 2023 21:59:11 GMT  
		Size: 5.0 MB (4974868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bebca7f9dc77dd081f1e8386b332902935be6eb718e5435056e6928dbdcded07`  
		Last Modified: Thu, 02 Feb 2023 21:59:10 GMT  
		Size: 561.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7247a73a46f57913d3042d8273753dc2524e2b7308a9b7c623043a9f83874df`  
		Last Modified: Thu, 02 Feb 2023 21:59:10 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.17` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:3b5d7a8ce580949f91c72ccb764cb0f808ca47f4a306cd2a64adef699b18c709
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.1 MB (8062087 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:72e93fab38c492847947f3360491ff675e9657ddad7fffcd6ddaf34818b3359e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 09 Jan 2023 17:04:48 GMT
ADD file:3080f19f39259a4b77cc53975de0184c78d4335ceb9ffb77a2838d0539ad6f85 in / 
# Mon, 09 Jan 2023 17:04:49 GMT
CMD ["/bin/sh"]
# Thu, 02 Feb 2023 21:47:31 GMT
ENV NATS_SERVER=2.9.12
# Thu, 02 Feb 2023 21:47:34 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='296075e7caa33684f0a23ac97c2a904c8f22dbc1d75da4ab443a81aa8b1b765b' ;; 		armhf) natsArch='arm6'; sha256='72af57a620de31e718131736b4ae123acd994295b2f81d1f847cdb9e1e686e63' ;; 		armv7) natsArch='arm7'; sha256='153d823e90b76457b6689cb6baa9f045b3a2152caaec787a0ad77162431949ed' ;; 		x86_64) natsArch='amd64'; sha256='cd05e53b3e1a535dd4e09a4cba3c1b0cd7c512e7f3d68d52ed8e8621dac8c925' ;; 		x86) natsArch='386'; sha256='103d89a231154708375a091dfb86ebe563f3de968a5e6ed14aba4c32e5c77925' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 02 Feb 2023 21:47:34 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 02 Feb 2023 21:47:34 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 02 Feb 2023 21:47:34 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Feb 2023 21:47:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 02 Feb 2023 21:47:34 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:a9eaa45ef418e883481a13c7d84fa9904f2ec56789c52a87ba5a9e6483f2b74f`  
		Last Modified: Mon, 09 Jan 2023 17:05:12 GMT  
		Size: 3.3 MB (3259241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf7882578303a0fa74c95f3a4d8ba43cb527ab5ae15db2e91420624139809c58`  
		Last Modified: Thu, 02 Feb 2023 21:48:06 GMT  
		Size: 4.8 MB (4801846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02c5fcf7cb836026cb1caf41222a5db286caad4181a1465fbc6a827e539d655f`  
		Last Modified: Thu, 02 Feb 2023 21:48:06 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c842168768b2663567de8311303dd5b2951b867f7c2228af37a24b50f24181ae`  
		Last Modified: Thu, 02 Feb 2023 21:48:05 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:latest`

```console
$ docker pull nats@sha256:1fc110ad1583ad4ac948623fbaed53afec34afc4a03d60e23384a5d4479fe22d
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
$ docker pull nats@sha256:b7cd8c3270f038b671b4d55156398eec4387fff96c2de872255d30024bf6a557
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4931647 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b82b64c84efab021cd029f60c01c7e52b53b4eae18827b383f87a4393b3a7095`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 02 Feb 2023 21:33:01 GMT
COPY file:a9e60c6fbbdd9ebb5d2c4deec1df6db6d6a40a0384a5544b6c3386eea2057a54 in /nats-server 
# Thu, 02 Feb 2023 21:33:02 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 02 Feb 2023 21:33:02 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Feb 2023 21:33:02 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 02 Feb 2023 21:33:02 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 02 Feb 2023 21:33:02 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:1cd3edd838903059461e505e0f1e09d3452d5e632e2b550f4d0850b0d2f59c72`  
		Last Modified: Thu, 02 Feb 2023 21:33:50 GMT  
		Size: 4.9 MB (4931138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e56ba114f2531c68c394372ad404aeb5ac8ee8946fb17af7ac704a76697756f`  
		Last Modified: Thu, 02 Feb 2023 21:33:49 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm variant v6

```console
$ docker pull nats@sha256:c1107d0e00f4d8dedfbf7883fbabc7b200545657e1e13495e12453d13dfde328
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4694918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c7de15c41747ca8b98deb9b16e6b45e323bf1b12bfe5ba0617911396006a4fc`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 02 Feb 2023 21:50:29 GMT
COPY file:be32648053f47b33b445bad52bed7ff3e74d1dc77100df4d672e431022428de7 in /nats-server 
# Thu, 02 Feb 2023 21:50:29 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 02 Feb 2023 21:50:29 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Feb 2023 21:50:29 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 02 Feb 2023 21:50:29 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 02 Feb 2023 21:50:29 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:eddbc6c88066991dd5810d3a3b6875ee06eecb063cccc9b0e3d9386c75c4f826`  
		Last Modified: Thu, 02 Feb 2023 21:52:00 GMT  
		Size: 4.7 MB (4694411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:795c72903a6f36672ee81a0386bff46e30e1f3598c7552f5c192f650d82c6e69`  
		Last Modified: Thu, 02 Feb 2023 21:51:59 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm variant v7

```console
$ docker pull nats@sha256:8a3086f469fd77000e1a8618960b722ca85e5cbd69a41190e81286734c7e455a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4688297 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa7e9966ce4e992db69b98063dd7d35d6fe1239100d385115ea7031b9b65978b`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 02 Feb 2023 21:58:12 GMT
COPY file:a67f587b7b86d3c3a85687c0097c93084fb71c44966695879cd46269a36ed31d in /nats-server 
# Thu, 02 Feb 2023 21:58:12 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 02 Feb 2023 21:58:12 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Feb 2023 21:58:12 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 02 Feb 2023 21:58:12 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 02 Feb 2023 21:58:12 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:df148ca425b44984356880f1ed4c1f04d36d2e6efa76ba4043d9dd80fe9f6201`  
		Last Modified: Thu, 02 Feb 2023 21:59:43 GMT  
		Size: 4.7 MB (4687788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b679ac38b5a1c67873f0f08c522aafadecaa085bed163dcc8387ddd53c0509d2`  
		Last Modified: Thu, 02 Feb 2023 21:59:43 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:b33b08f196a8f9b3b612740d36e847c1d5bc5239bf49f768b0056cd2ff7baaf0
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4517074 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:21aad311a08f5e75bd795b33799a8a100d9eb132974428f406329a5871687f79`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 02 Feb 2023 21:47:40 GMT
COPY file:f1194fd7c754730901a7920f7db8ad6e6432e904adfe27cb3bf09f1626eb0b20 in /nats-server 
# Thu, 02 Feb 2023 21:47:40 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 02 Feb 2023 21:47:40 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Feb 2023 21:47:40 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 02 Feb 2023 21:47:40 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 02 Feb 2023 21:47:40 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:0e112ba48caecfa7e51d560718ada0f9c4e686bdc09555df0617055a883e5777`  
		Last Modified: Thu, 02 Feb 2023 21:48:28 GMT  
		Size: 4.5 MB (4516565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fce6348af8f3a9160210d4305f3a6f5c76b1b36d75df166f313f92cf3774f93f`  
		Last Modified: Thu, 02 Feb 2023 21:48:27 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - windows version 10.0.17763.3887; amd64

```console
$ docker pull nats@sha256:298b8a1b690d1d64fbd955cb251e93b63874ef7d4cb6f0eb2128cb3df82d1ecf
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.7 MB (111657511 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d6d4d57475df3d7d3cc4f4a97791acce1c9ce0aa971eff49258813b2b55ba7c`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 07 Jan 2023 05:17:01 GMT
RUN Apply image 10.0.17763.3887
# Thu, 12 Jan 2023 05:01:51 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Thu, 02 Feb 2023 21:18:29 GMT
RUN cmd /S /C #(nop) COPY file:1d619f9da4aa7d6fe4171f8e7c232a42ba0b813a50cbb3466448bbfaf0fc4a79 in C:\nats-server.exe 
# Thu, 02 Feb 2023 21:18:30 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Thu, 02 Feb 2023 21:18:31 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Thu, 02 Feb 2023 21:18:32 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 02 Feb 2023 21:18:33 GMT
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
	-	`sha256:3801c3e14f4f67451b0f8a1220428a70eeddbf9bdef73cd8b89614087bfea683`  
		Last Modified: Thu, 02 Feb 2023 21:19:24 GMT  
		Size: 5.0 MB (4985010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc3da06a2f05c3cb57b2c4406a7135beaef26938a9d48c94e9bb19f285362f19`  
		Last Modified: Thu, 02 Feb 2023 21:19:22 GMT  
		Size: 1.8 KB (1768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a28bce3ab94f882453c700042d8e7ff6aa55d92a06dad8d04be017d91ec9208`  
		Last Modified: Thu, 02 Feb 2023 21:19:22 GMT  
		Size: 1.2 KB (1173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dba391f32fd738334e9c4d766b67aa8340b1fac87188801d71faf347db92b3fb`  
		Last Modified: Thu, 02 Feb 2023 21:19:22 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d938df46930834c4903622f9028898bde90a5f21c98963408af250b41e05242c`  
		Last Modified: Thu, 02 Feb 2023 21:19:22 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:linux`

```console
$ docker pull nats@sha256:c926cdb68b698f2bbe658b5dac5353803f29c4cd4e7ab8bdc572077ee8a9f870
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:linux` - linux; amd64

```console
$ docker pull nats@sha256:b7cd8c3270f038b671b4d55156398eec4387fff96c2de872255d30024bf6a557
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4931647 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b82b64c84efab021cd029f60c01c7e52b53b4eae18827b383f87a4393b3a7095`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 02 Feb 2023 21:33:01 GMT
COPY file:a9e60c6fbbdd9ebb5d2c4deec1df6db6d6a40a0384a5544b6c3386eea2057a54 in /nats-server 
# Thu, 02 Feb 2023 21:33:02 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 02 Feb 2023 21:33:02 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Feb 2023 21:33:02 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 02 Feb 2023 21:33:02 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 02 Feb 2023 21:33:02 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:1cd3edd838903059461e505e0f1e09d3452d5e632e2b550f4d0850b0d2f59c72`  
		Last Modified: Thu, 02 Feb 2023 21:33:50 GMT  
		Size: 4.9 MB (4931138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e56ba114f2531c68c394372ad404aeb5ac8ee8946fb17af7ac704a76697756f`  
		Last Modified: Thu, 02 Feb 2023 21:33:49 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:c1107d0e00f4d8dedfbf7883fbabc7b200545657e1e13495e12453d13dfde328
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4694918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c7de15c41747ca8b98deb9b16e6b45e323bf1b12bfe5ba0617911396006a4fc`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 02 Feb 2023 21:50:29 GMT
COPY file:be32648053f47b33b445bad52bed7ff3e74d1dc77100df4d672e431022428de7 in /nats-server 
# Thu, 02 Feb 2023 21:50:29 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 02 Feb 2023 21:50:29 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Feb 2023 21:50:29 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 02 Feb 2023 21:50:29 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 02 Feb 2023 21:50:29 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:eddbc6c88066991dd5810d3a3b6875ee06eecb063cccc9b0e3d9386c75c4f826`  
		Last Modified: Thu, 02 Feb 2023 21:52:00 GMT  
		Size: 4.7 MB (4694411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:795c72903a6f36672ee81a0386bff46e30e1f3598c7552f5c192f650d82c6e69`  
		Last Modified: Thu, 02 Feb 2023 21:51:59 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:8a3086f469fd77000e1a8618960b722ca85e5cbd69a41190e81286734c7e455a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4688297 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa7e9966ce4e992db69b98063dd7d35d6fe1239100d385115ea7031b9b65978b`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 02 Feb 2023 21:58:12 GMT
COPY file:a67f587b7b86d3c3a85687c0097c93084fb71c44966695879cd46269a36ed31d in /nats-server 
# Thu, 02 Feb 2023 21:58:12 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 02 Feb 2023 21:58:12 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Feb 2023 21:58:12 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 02 Feb 2023 21:58:12 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 02 Feb 2023 21:58:12 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:df148ca425b44984356880f1ed4c1f04d36d2e6efa76ba4043d9dd80fe9f6201`  
		Last Modified: Thu, 02 Feb 2023 21:59:43 GMT  
		Size: 4.7 MB (4687788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b679ac38b5a1c67873f0f08c522aafadecaa085bed163dcc8387ddd53c0509d2`  
		Last Modified: Thu, 02 Feb 2023 21:59:43 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:b33b08f196a8f9b3b612740d36e847c1d5bc5239bf49f768b0056cd2ff7baaf0
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4517074 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:21aad311a08f5e75bd795b33799a8a100d9eb132974428f406329a5871687f79`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 02 Feb 2023 21:47:40 GMT
COPY file:f1194fd7c754730901a7920f7db8ad6e6432e904adfe27cb3bf09f1626eb0b20 in /nats-server 
# Thu, 02 Feb 2023 21:47:40 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 02 Feb 2023 21:47:40 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Feb 2023 21:47:40 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 02 Feb 2023 21:47:40 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 02 Feb 2023 21:47:40 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:0e112ba48caecfa7e51d560718ada0f9c4e686bdc09555df0617055a883e5777`  
		Last Modified: Thu, 02 Feb 2023 21:48:28 GMT  
		Size: 4.5 MB (4516565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fce6348af8f3a9160210d4305f3a6f5c76b1b36d75df166f313f92cf3774f93f`  
		Last Modified: Thu, 02 Feb 2023 21:48:27 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:nanoserver`

```console
$ docker pull nats@sha256:853807ebafaad1d9a9ffee4521ea63cb1f171fe4e34262749cc13a71f59c1090
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3887; amd64

### `nats:nanoserver` - windows version 10.0.17763.3887; amd64

```console
$ docker pull nats@sha256:298b8a1b690d1d64fbd955cb251e93b63874ef7d4cb6f0eb2128cb3df82d1ecf
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.7 MB (111657511 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d6d4d57475df3d7d3cc4f4a97791acce1c9ce0aa971eff49258813b2b55ba7c`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 07 Jan 2023 05:17:01 GMT
RUN Apply image 10.0.17763.3887
# Thu, 12 Jan 2023 05:01:51 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Thu, 02 Feb 2023 21:18:29 GMT
RUN cmd /S /C #(nop) COPY file:1d619f9da4aa7d6fe4171f8e7c232a42ba0b813a50cbb3466448bbfaf0fc4a79 in C:\nats-server.exe 
# Thu, 02 Feb 2023 21:18:30 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Thu, 02 Feb 2023 21:18:31 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Thu, 02 Feb 2023 21:18:32 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 02 Feb 2023 21:18:33 GMT
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
	-	`sha256:3801c3e14f4f67451b0f8a1220428a70eeddbf9bdef73cd8b89614087bfea683`  
		Last Modified: Thu, 02 Feb 2023 21:19:24 GMT  
		Size: 5.0 MB (4985010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc3da06a2f05c3cb57b2c4406a7135beaef26938a9d48c94e9bb19f285362f19`  
		Last Modified: Thu, 02 Feb 2023 21:19:22 GMT  
		Size: 1.8 KB (1768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a28bce3ab94f882453c700042d8e7ff6aa55d92a06dad8d04be017d91ec9208`  
		Last Modified: Thu, 02 Feb 2023 21:19:22 GMT  
		Size: 1.2 KB (1173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dba391f32fd738334e9c4d766b67aa8340b1fac87188801d71faf347db92b3fb`  
		Last Modified: Thu, 02 Feb 2023 21:19:22 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d938df46930834c4903622f9028898bde90a5f21c98963408af250b41e05242c`  
		Last Modified: Thu, 02 Feb 2023 21:19:22 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:nanoserver-1809`

```console
$ docker pull nats@sha256:853807ebafaad1d9a9ffee4521ea63cb1f171fe4e34262749cc13a71f59c1090
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3887; amd64

### `nats:nanoserver-1809` - windows version 10.0.17763.3887; amd64

```console
$ docker pull nats@sha256:298b8a1b690d1d64fbd955cb251e93b63874ef7d4cb6f0eb2128cb3df82d1ecf
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.7 MB (111657511 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d6d4d57475df3d7d3cc4f4a97791acce1c9ce0aa971eff49258813b2b55ba7c`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 07 Jan 2023 05:17:01 GMT
RUN Apply image 10.0.17763.3887
# Thu, 12 Jan 2023 05:01:51 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Thu, 02 Feb 2023 21:18:29 GMT
RUN cmd /S /C #(nop) COPY file:1d619f9da4aa7d6fe4171f8e7c232a42ba0b813a50cbb3466448bbfaf0fc4a79 in C:\nats-server.exe 
# Thu, 02 Feb 2023 21:18:30 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Thu, 02 Feb 2023 21:18:31 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Thu, 02 Feb 2023 21:18:32 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 02 Feb 2023 21:18:33 GMT
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
	-	`sha256:3801c3e14f4f67451b0f8a1220428a70eeddbf9bdef73cd8b89614087bfea683`  
		Last Modified: Thu, 02 Feb 2023 21:19:24 GMT  
		Size: 5.0 MB (4985010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc3da06a2f05c3cb57b2c4406a7135beaef26938a9d48c94e9bb19f285362f19`  
		Last Modified: Thu, 02 Feb 2023 21:19:22 GMT  
		Size: 1.8 KB (1768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a28bce3ab94f882453c700042d8e7ff6aa55d92a06dad8d04be017d91ec9208`  
		Last Modified: Thu, 02 Feb 2023 21:19:22 GMT  
		Size: 1.2 KB (1173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dba391f32fd738334e9c4d766b67aa8340b1fac87188801d71faf347db92b3fb`  
		Last Modified: Thu, 02 Feb 2023 21:19:22 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d938df46930834c4903622f9028898bde90a5f21c98963408af250b41e05242c`  
		Last Modified: Thu, 02 Feb 2023 21:19:22 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:scratch`

```console
$ docker pull nats@sha256:c926cdb68b698f2bbe658b5dac5353803f29c4cd4e7ab8bdc572077ee8a9f870
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:scratch` - linux; amd64

```console
$ docker pull nats@sha256:b7cd8c3270f038b671b4d55156398eec4387fff96c2de872255d30024bf6a557
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4931647 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b82b64c84efab021cd029f60c01c7e52b53b4eae18827b383f87a4393b3a7095`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 02 Feb 2023 21:33:01 GMT
COPY file:a9e60c6fbbdd9ebb5d2c4deec1df6db6d6a40a0384a5544b6c3386eea2057a54 in /nats-server 
# Thu, 02 Feb 2023 21:33:02 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 02 Feb 2023 21:33:02 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Feb 2023 21:33:02 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 02 Feb 2023 21:33:02 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 02 Feb 2023 21:33:02 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:1cd3edd838903059461e505e0f1e09d3452d5e632e2b550f4d0850b0d2f59c72`  
		Last Modified: Thu, 02 Feb 2023 21:33:50 GMT  
		Size: 4.9 MB (4931138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e56ba114f2531c68c394372ad404aeb5ac8ee8946fb17af7ac704a76697756f`  
		Last Modified: Thu, 02 Feb 2023 21:33:49 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:c1107d0e00f4d8dedfbf7883fbabc7b200545657e1e13495e12453d13dfde328
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4694918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c7de15c41747ca8b98deb9b16e6b45e323bf1b12bfe5ba0617911396006a4fc`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 02 Feb 2023 21:50:29 GMT
COPY file:be32648053f47b33b445bad52bed7ff3e74d1dc77100df4d672e431022428de7 in /nats-server 
# Thu, 02 Feb 2023 21:50:29 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 02 Feb 2023 21:50:29 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Feb 2023 21:50:29 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 02 Feb 2023 21:50:29 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 02 Feb 2023 21:50:29 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:eddbc6c88066991dd5810d3a3b6875ee06eecb063cccc9b0e3d9386c75c4f826`  
		Last Modified: Thu, 02 Feb 2023 21:52:00 GMT  
		Size: 4.7 MB (4694411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:795c72903a6f36672ee81a0386bff46e30e1f3598c7552f5c192f650d82c6e69`  
		Last Modified: Thu, 02 Feb 2023 21:51:59 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:8a3086f469fd77000e1a8618960b722ca85e5cbd69a41190e81286734c7e455a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4688297 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa7e9966ce4e992db69b98063dd7d35d6fe1239100d385115ea7031b9b65978b`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 02 Feb 2023 21:58:12 GMT
COPY file:a67f587b7b86d3c3a85687c0097c93084fb71c44966695879cd46269a36ed31d in /nats-server 
# Thu, 02 Feb 2023 21:58:12 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 02 Feb 2023 21:58:12 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Feb 2023 21:58:12 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 02 Feb 2023 21:58:12 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 02 Feb 2023 21:58:12 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:df148ca425b44984356880f1ed4c1f04d36d2e6efa76ba4043d9dd80fe9f6201`  
		Last Modified: Thu, 02 Feb 2023 21:59:43 GMT  
		Size: 4.7 MB (4687788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b679ac38b5a1c67873f0f08c522aafadecaa085bed163dcc8387ddd53c0509d2`  
		Last Modified: Thu, 02 Feb 2023 21:59:43 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:b33b08f196a8f9b3b612740d36e847c1d5bc5239bf49f768b0056cd2ff7baaf0
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4517074 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:21aad311a08f5e75bd795b33799a8a100d9eb132974428f406329a5871687f79`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 02 Feb 2023 21:47:40 GMT
COPY file:f1194fd7c754730901a7920f7db8ad6e6432e904adfe27cb3bf09f1626eb0b20 in /nats-server 
# Thu, 02 Feb 2023 21:47:40 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 02 Feb 2023 21:47:40 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Feb 2023 21:47:40 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 02 Feb 2023 21:47:40 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 02 Feb 2023 21:47:40 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:0e112ba48caecfa7e51d560718ada0f9c4e686bdc09555df0617055a883e5777`  
		Last Modified: Thu, 02 Feb 2023 21:48:28 GMT  
		Size: 4.5 MB (4516565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fce6348af8f3a9160210d4305f3a6f5c76b1b36d75df166f313f92cf3774f93f`  
		Last Modified: Thu, 02 Feb 2023 21:48:27 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:windowsservercore`

```console
$ docker pull nats@sha256:f0e699db4eb709cfad8009ccb7babc3b5f99ad75b8635428c8a1f4b968f5e1c6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3887; amd64

### `nats:windowsservercore` - windows version 10.0.17763.3887; amd64

```console
$ docker pull nats@sha256:21cd0fd5eed31d916b22e6bb32cfd8b17357a90504e876a650dbfe702f7ad4c3
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.7 GB (1713682302 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d6cfbec3abd0c20da1ad583cfeba37afbf93ac199cfd962df9a78badf81c44c5`
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
# Thu, 02 Feb 2023 21:16:27 GMT
ENV NATS_SERVER=2.9.12
# Thu, 02 Feb 2023 21:16:28 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.9.12/nats-server-v2.9.12-windows-amd64.zip
# Thu, 02 Feb 2023 21:16:29 GMT
ENV NATS_SERVER_SHASUM=a87b6715550f0a5f8829dd51923ce6a20c6302227e4ade76c6403f49703ad12f
# Thu, 02 Feb 2023 21:17:00 GMT
RUN Set-PSDebug -Trace 2
# Thu, 02 Feb 2023 21:18:09 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Thu, 02 Feb 2023 21:18:10 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Thu, 02 Feb 2023 21:18:11 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Feb 2023 21:18:12 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 02 Feb 2023 21:18:13 GMT
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
	-	`sha256:fe84adf024fde5f8eff638fb25641740e35f164990a89dc350e955eaac3f822d`  
		Last Modified: Thu, 02 Feb 2023 21:19:08 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3029d4bc864cb72910f78c88e54a6cd47e3ab04772b8281f529243ff7f8dd7b8`  
		Last Modified: Thu, 02 Feb 2023 21:19:08 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d08011b8eb78752d65a736ca9f99d7f77bdec75b80c52b6ebaf1986e91d27e6`  
		Last Modified: Thu, 02 Feb 2023 21:19:08 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1271e50716be60e293a328182a8014b8208316cfab34ae9ca88cca1c1d208f9`  
		Last Modified: Thu, 02 Feb 2023 21:19:08 GMT  
		Size: 382.7 KB (382745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7b8a07a3d2b9a3e07d670ef47f886c71f2dec4186a4b33fda0f4d0cf258cdeb`  
		Last Modified: Thu, 02 Feb 2023 21:19:07 GMT  
		Size: 5.3 MB (5342340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:831ce5e8c2d1c916622590fab5d1aaf7a400134a6df616daf6cfa60889de7d96`  
		Last Modified: Thu, 02 Feb 2023 21:19:06 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfc448b0cbe5f2ad0f9c72fbc2969f5bdc46b0cb3f43838d54cd9f2eb0f7a06b`  
		Last Modified: Thu, 02 Feb 2023 21:19:06 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d976be1bad16d8687a8e24c34fa6db831c074dbc26c19dc49f405a0e663d86b7`  
		Last Modified: Thu, 02 Feb 2023 21:19:06 GMT  
		Size: 1.4 KB (1386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:314a1587606bc3b0f6be6c93d6e597583050cd41304603aa4cb14447f4b6e240`  
		Last Modified: Thu, 02 Feb 2023 21:19:06 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:windowsservercore-1809`

```console
$ docker pull nats@sha256:f0e699db4eb709cfad8009ccb7babc3b5f99ad75b8635428c8a1f4b968f5e1c6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3887; amd64

### `nats:windowsservercore-1809` - windows version 10.0.17763.3887; amd64

```console
$ docker pull nats@sha256:21cd0fd5eed31d916b22e6bb32cfd8b17357a90504e876a650dbfe702f7ad4c3
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.7 GB (1713682302 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d6cfbec3abd0c20da1ad583cfeba37afbf93ac199cfd962df9a78badf81c44c5`
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
# Thu, 02 Feb 2023 21:16:27 GMT
ENV NATS_SERVER=2.9.12
# Thu, 02 Feb 2023 21:16:28 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.9.12/nats-server-v2.9.12-windows-amd64.zip
# Thu, 02 Feb 2023 21:16:29 GMT
ENV NATS_SERVER_SHASUM=a87b6715550f0a5f8829dd51923ce6a20c6302227e4ade76c6403f49703ad12f
# Thu, 02 Feb 2023 21:17:00 GMT
RUN Set-PSDebug -Trace 2
# Thu, 02 Feb 2023 21:18:09 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Thu, 02 Feb 2023 21:18:10 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Thu, 02 Feb 2023 21:18:11 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Feb 2023 21:18:12 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 02 Feb 2023 21:18:13 GMT
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
	-	`sha256:fe84adf024fde5f8eff638fb25641740e35f164990a89dc350e955eaac3f822d`  
		Last Modified: Thu, 02 Feb 2023 21:19:08 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3029d4bc864cb72910f78c88e54a6cd47e3ab04772b8281f529243ff7f8dd7b8`  
		Last Modified: Thu, 02 Feb 2023 21:19:08 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d08011b8eb78752d65a736ca9f99d7f77bdec75b80c52b6ebaf1986e91d27e6`  
		Last Modified: Thu, 02 Feb 2023 21:19:08 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1271e50716be60e293a328182a8014b8208316cfab34ae9ca88cca1c1d208f9`  
		Last Modified: Thu, 02 Feb 2023 21:19:08 GMT  
		Size: 382.7 KB (382745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7b8a07a3d2b9a3e07d670ef47f886c71f2dec4186a4b33fda0f4d0cf258cdeb`  
		Last Modified: Thu, 02 Feb 2023 21:19:07 GMT  
		Size: 5.3 MB (5342340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:831ce5e8c2d1c916622590fab5d1aaf7a400134a6df616daf6cfa60889de7d96`  
		Last Modified: Thu, 02 Feb 2023 21:19:06 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfc448b0cbe5f2ad0f9c72fbc2969f5bdc46b0cb3f43838d54cd9f2eb0f7a06b`  
		Last Modified: Thu, 02 Feb 2023 21:19:06 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d976be1bad16d8687a8e24c34fa6db831c074dbc26c19dc49f405a0e663d86b7`  
		Last Modified: Thu, 02 Feb 2023 21:19:06 GMT  
		Size: 1.4 KB (1386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:314a1587606bc3b0f6be6c93d6e597583050cd41304603aa4cb14447f4b6e240`  
		Last Modified: Thu, 02 Feb 2023 21:19:06 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
