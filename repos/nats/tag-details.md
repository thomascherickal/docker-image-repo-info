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
-	[`nats:2.9.7`](#nats297)
-	[`nats:2.9.7-alpine`](#nats297-alpine)
-	[`nats:2.9.7-alpine3.16`](#nats297-alpine316)
-	[`nats:2.9.7-linux`](#nats297-linux)
-	[`nats:2.9.7-nanoserver`](#nats297-nanoserver)
-	[`nats:2.9.7-nanoserver-1809`](#nats297-nanoserver-1809)
-	[`nats:2.9.7-scratch`](#nats297-scratch)
-	[`nats:2.9.7-windowsservercore`](#nats297-windowsservercore)
-	[`nats:2.9.7-windowsservercore-1809`](#nats297-windowsservercore-1809)
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
$ docker pull nats@sha256:8a550ace09f524090c5399c7eab008c9f0d55a29eb1732cc4a565d4f1160346c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.3650; amd64

### `nats:2` - linux; amd64

```console
$ docker pull nats@sha256:6fc6aee58f7a448bb3bbd803f3addfa0c9512b5083376ce20781b9b635c381cf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4918825 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:974c838918842c11cbf59d7af83a073f753537c9d4b14f47231d3c1c7ba41c9e`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 17 Nov 2022 20:21:46 GMT
COPY file:88cbf98679a4e287b67a701a1fb77e0e0928e75cc0e1e669916e033ecf774fdc in /nats-server 
# Thu, 17 Nov 2022 20:21:46 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 17 Nov 2022 20:21:46 GMT
EXPOSE 4222 6222 8222
# Thu, 17 Nov 2022 20:21:46 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 17 Nov 2022 20:21:46 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 17 Nov 2022 20:21:47 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c8ce17c05ed27e7e08286a74c292d54eb2d5902af8f901dab4505ba83f7296f5`  
		Last Modified: Thu, 17 Nov 2022 20:22:33 GMT  
		Size: 4.9 MB (4918317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88c3d57c92f61ccff2db59e857c959bc11ca2ed1a6ca7f5494aa479c513196f7`  
		Last Modified: Thu, 17 Nov 2022 20:22:32 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - linux; arm variant v6

```console
$ docker pull nats@sha256:9e5158db138340db27aef59e820bafe7a09359e8910c2cef451b58348dd329ff
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4683160 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b5c60a8afd73cd47b032a2d66e4968bf12f1aed52fee0f708cf184ef6c09b960`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 17 Nov 2022 20:49:48 GMT
COPY file:75f2ce97960bd08a17d41dd00b0f977ff54641b0f3d5b35f613c50553a59e8e1 in /nats-server 
# Thu, 17 Nov 2022 20:49:48 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 17 Nov 2022 20:49:49 GMT
EXPOSE 4222 6222 8222
# Thu, 17 Nov 2022 20:49:49 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 17 Nov 2022 20:49:49 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 17 Nov 2022 20:49:49 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:e27c576ee7d0df355bb5ab346016b3a399e8048fe3f938263b3b77e343d9243f`  
		Last Modified: Thu, 17 Nov 2022 20:51:22 GMT  
		Size: 4.7 MB (4682651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:788fb9f41d9d2c69e1f5737db95b3d0e754d24cd75bdd8d94a80166b8c97d6b6`  
		Last Modified: Thu, 17 Nov 2022 20:51:21 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - linux; arm variant v7

```console
$ docker pull nats@sha256:e4c874e4f9f5eafa49bdd7fed9a022da8958f69cc70e245af8bb9ebf7cad0c0c
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4679780 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2bc64213c48245d6c2d479e5be4d5043a6d811cb9d273ae36c8dfa157accbd04`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 17 Nov 2022 20:58:06 GMT
COPY file:ebca823a5dac00609e9fb9733528840572067b84b58dcccbe67a2df698f2869e in /nats-server 
# Thu, 17 Nov 2022 20:58:06 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 17 Nov 2022 20:58:06 GMT
EXPOSE 4222 6222 8222
# Thu, 17 Nov 2022 20:58:06 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 17 Nov 2022 20:58:06 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 17 Nov 2022 20:58:06 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:2c415cfba68b644bd88b057d832ff5015af29e04439812f5bd2e6873b3d7b8fd`  
		Last Modified: Thu, 17 Nov 2022 20:59:39 GMT  
		Size: 4.7 MB (4679272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:875032eeefdff15b8e0c04ffba01805fa83a04cad983b8322b99f53b04e9c1fe`  
		Last Modified: Thu, 17 Nov 2022 20:59:38 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:6d5eefe444c9be5d4f08fd3ccf8277d186014689ef84ea0f59c59dc11acb4904
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4504058 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7ac0ab188af08ab1a9c049a3f6c349d0d2df9595cee8e6626c19a913526dcb2`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 17 Nov 2022 20:40:45 GMT
COPY file:d11c7b340550df0716193331cacb3d06f2cb3b9971e90e006a9c153aaadc50f8 in /nats-server 
# Thu, 17 Nov 2022 20:40:45 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 17 Nov 2022 20:40:45 GMT
EXPOSE 4222 6222 8222
# Thu, 17 Nov 2022 20:40:45 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 17 Nov 2022 20:40:45 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 17 Nov 2022 20:40:45 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:d3e01af3796e331721cc924f0d95499739cea560e1ac4bac35c11176033c94c8`  
		Last Modified: Thu, 17 Nov 2022 20:41:30 GMT  
		Size: 4.5 MB (4503550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e0b7a277e0d621acb2a17025b4318262de852c8be74070453c2f8c9983601ad`  
		Last Modified: Thu, 17 Nov 2022 20:41:30 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - windows version 10.0.17763.3650; amd64

```console
$ docker pull nats@sha256:b69aaf3d5200a1cb93e65a79acaa950d17ee0b0e88be899c4c3ecd6695cf9529
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.7 MB (111704287 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a82f827f381afa49f7b9d69a162222472931dd2aad1ebbac2b60a8155e798028`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 05 Nov 2022 18:06:28 GMT
RUN Apply image 10.0.17763.3650
# Wed, 09 Nov 2022 16:47:43 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Thu, 17 Nov 2022 20:19:19 GMT
RUN cmd /S /C #(nop) COPY file:d6b547504effc3514ee13384db156b8c7df287eadd44c86f4e5f5eabb6646c1d in C:\nats-server.exe 
# Thu, 17 Nov 2022 20:19:20 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Thu, 17 Nov 2022 20:19:21 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Thu, 17 Nov 2022 20:19:21 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 17 Nov 2022 20:19:22 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:35ab4104a4d9df6a0d1eac84cc8fbc13511ef6c8aef5ced04fdf63e7e20803a3`  
		Last Modified: Tue, 08 Nov 2022 19:45:20 GMT  
		Size: 106.7 MB (106723592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6708525607bc7a2985c6a423e6cb63d6175e3ad60d997873c4519fab371772fe`  
		Last Modified: Wed, 09 Nov 2022 16:48:43 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cb5d7747e73374a2c02473deb4bde157dddb2835cb5e66800cfba5842c1fd88`  
		Last Modified: Thu, 17 Nov 2022 20:20:12 GMT  
		Size: 5.0 MB (4974250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b3d427408549420b1666d1a85d3ff1bd3132f4e61dd9a7bd4e75a7c5adc32ee`  
		Last Modified: Thu, 17 Nov 2022 20:20:11 GMT  
		Size: 1.8 KB (1811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4682e51d5cc8bfadb600b57559df30d236b94223a5e9b1c3d2468f6acb1ee3f3`  
		Last Modified: Thu, 17 Nov 2022 20:20:11 GMT  
		Size: 1.2 KB (1161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8223b92ce81db067bb8ee9eacbf53e251b0dcd29dd1af6aa3a519768f0a7b44b`  
		Last Modified: Thu, 17 Nov 2022 20:20:11 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51f050378e256630049566bfcc0cf782533a8f961bcae8b6d9421ef19a8a780f`  
		Last Modified: Thu, 17 Nov 2022 20:20:11 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-alpine`

```console
$ docker pull nats@sha256:400adfffe0df7f2df0e76d34d6e25a0fb8eb68cfdc10d404afbbb31f818d0276
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-alpine` - linux; amd64

```console
$ docker pull nats@sha256:d4698031a0afeb1ed37b240a9632b22a2d0fcea5fd48af3c8b28e1eba3348033
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.0 MB (8014859 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c26ee116aa283ae59469d995e49cce15bb982559c777e32f06933e315898c54`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Sat, 12 Nov 2022 04:19:23 GMT
ADD file:ceeb6e8632fafc657116cbf3afbd522185a16963230b57881073dad22eb0e1a3 in / 
# Sat, 12 Nov 2022 04:19:23 GMT
CMD ["/bin/sh"]
# Thu, 17 Nov 2022 20:21:36 GMT
ENV NATS_SERVER=2.9.7
# Thu, 17 Nov 2022 20:21:38 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='153018a675b0e896ffbed0cbc3fe5f733fd674d2f4bf554130ae8960a6c5277c' ;; 		armhf) natsArch='arm6'; sha256='9714af72c37f0ede4465a3b0324230af74701e82414194a9c2228e7563327523' ;; 		armv7) natsArch='arm7'; sha256='804ec4f600418d4afd6a9cb94b92c306ab75c589fc5180a5c2c99cc514c0899a' ;; 		x86_64) natsArch='amd64'; sha256='d4d2ef2952a9a841ce6594a4dbd07b8a45ceea32dadb321ddebc0c56598c2085' ;; 		x86) natsArch='386'; sha256='add5a328af2cab82230f881f71f7ca4dd907b477972d14a06b77b83188863d4d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 17 Nov 2022 20:21:38 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 17 Nov 2022 20:21:38 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 17 Nov 2022 20:21:39 GMT
EXPOSE 4222 6222 8222
# Thu, 17 Nov 2022 20:21:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Nov 2022 20:21:39 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:ca7dd9ec2225f2385955c43b2379305acd51543c28cf1d4e94522b3d94cce3ce`  
		Last Modified: Sat, 12 Nov 2022 02:52:15 GMT  
		Size: 2.8 MB (2806272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94acb566bf3ae8a5a3c0747075e8b16df167a9694bfb5ac6ccdea4e5558e2a01`  
		Last Modified: Thu, 17 Nov 2022 20:22:12 GMT  
		Size: 5.2 MB (5207590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e759e667a2c2d6d67aaf3491e124f07a1afc8de774d7973958b32b81ff7a0304`  
		Last Modified: Thu, 17 Nov 2022 20:22:11 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c0e8173963a2be8b30df5827fcfc01a70e5c95ab186696e43d9f624884cee41`  
		Last Modified: Thu, 17 Nov 2022 20:22:11 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:221c14c269fed109042c154935b6cd22b270dda8b66b30e48f734f5fb50ffb87
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7586411 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b8f37497160e12532b20e7eaca7e50daa1304f46b7002848dfae699b06743ba`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Sat, 12 Nov 2022 03:49:18 GMT
ADD file:493290ed8856fa13463defe63da0d30ab3de5dde042c87ef7c0701d66ebb8892 in / 
# Sat, 12 Nov 2022 03:49:18 GMT
CMD ["/bin/sh"]
# Thu, 17 Nov 2022 20:49:34 GMT
ENV NATS_SERVER=2.9.7
# Thu, 17 Nov 2022 20:49:36 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='153018a675b0e896ffbed0cbc3fe5f733fd674d2f4bf554130ae8960a6c5277c' ;; 		armhf) natsArch='arm6'; sha256='9714af72c37f0ede4465a3b0324230af74701e82414194a9c2228e7563327523' ;; 		armv7) natsArch='arm7'; sha256='804ec4f600418d4afd6a9cb94b92c306ab75c589fc5180a5c2c99cc514c0899a' ;; 		x86_64) natsArch='amd64'; sha256='d4d2ef2952a9a841ce6594a4dbd07b8a45ceea32dadb321ddebc0c56598c2085' ;; 		x86) natsArch='386'; sha256='add5a328af2cab82230f881f71f7ca4dd907b477972d14a06b77b83188863d4d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 17 Nov 2022 20:49:36 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 17 Nov 2022 20:49:36 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 17 Nov 2022 20:49:36 GMT
EXPOSE 4222 6222 8222
# Thu, 17 Nov 2022 20:49:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Nov 2022 20:49:37 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9616ea8c1de4a90b1a50591336485e88ae5c2346e0d778bdbe69b00647bf8e39`  
		Last Modified: Sat, 12 Nov 2022 03:50:12 GMT  
		Size: 2.6 MB (2615105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d5728111a27515c16eb46117bf3339ccefc8af39e7c1508951d9286a3c3891c`  
		Last Modified: Thu, 17 Nov 2022 20:50:52 GMT  
		Size: 5.0 MB (4970331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d3e171e5c82f413b32d409f4fce9c56e3a429da91e068be34239e7c8c856576`  
		Last Modified: Thu, 17 Nov 2022 20:50:51 GMT  
		Size: 561.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:699b733f623013826c3dee6862aac2f7cb12bc97712d445dcf79191ba87875f6`  
		Last Modified: Thu, 17 Nov 2022 20:50:51 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:bf2175af45ce04af8a4d8a8c810eb98dbbdf0208010f248234803a56346e7492
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.4 MB (7380724 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af540a578654dbc22e31a00269e904f93dae199d3a57c7b588311595cd8c326c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Sat, 12 Nov 2022 03:57:24 GMT
ADD file:0b4a628f529226f5ec9d357ca63138bd2d22411a889c780ac8d395d761e07b2c in / 
# Sat, 12 Nov 2022 03:57:24 GMT
CMD ["/bin/sh"]
# Thu, 17 Nov 2022 20:57:48 GMT
ENV NATS_SERVER=2.9.7
# Thu, 17 Nov 2022 20:57:51 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='153018a675b0e896ffbed0cbc3fe5f733fd674d2f4bf554130ae8960a6c5277c' ;; 		armhf) natsArch='arm6'; sha256='9714af72c37f0ede4465a3b0324230af74701e82414194a9c2228e7563327523' ;; 		armv7) natsArch='arm7'; sha256='804ec4f600418d4afd6a9cb94b92c306ab75c589fc5180a5c2c99cc514c0899a' ;; 		x86_64) natsArch='amd64'; sha256='d4d2ef2952a9a841ce6594a4dbd07b8a45ceea32dadb321ddebc0c56598c2085' ;; 		x86) natsArch='386'; sha256='add5a328af2cab82230f881f71f7ca4dd907b477972d14a06b77b83188863d4d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 17 Nov 2022 20:57:51 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 17 Nov 2022 20:57:51 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 17 Nov 2022 20:57:52 GMT
EXPOSE 4222 6222 8222
# Thu, 17 Nov 2022 20:57:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Nov 2022 20:57:52 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:e44ba29d168a7f7c9e914f3724614df9e070aa6ef9b9ba5c9004db3c071f403a`  
		Last Modified: Sat, 12 Nov 2022 03:58:16 GMT  
		Size: 2.4 MB (2418788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c6aab4ebcc741288db0b5a719ef99f393d0fd90552b7131f9391a1f1bb37575`  
		Last Modified: Thu, 17 Nov 2022 20:59:09 GMT  
		Size: 5.0 MB (4960964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c4be9c1201790ef36f0543a1ad75a874f321b98fb2053e0b742e2f74e72338e`  
		Last Modified: Thu, 17 Nov 2022 20:59:08 GMT  
		Size: 560.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6f34e641f8406d256e755f8e058c5e957c85a985209c0e0021a18e1aab450c9`  
		Last Modified: Thu, 17 Nov 2022 20:59:08 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:173181d8057b550ed4e321336b885f0ada263273ebc6cba24563f43578c00c23
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.5 MB (7503096 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:41f949bc183512a9594a4bcf404727a905c6e76f0ac0318a03cf0e2b93ccf1de`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Sat, 12 Nov 2022 03:39:38 GMT
ADD file:57d621536158358b14d15155826ef2dd4ca034278044111ec0aaf6717016e569 in / 
# Sat, 12 Nov 2022 03:39:38 GMT
CMD ["/bin/sh"]
# Thu, 17 Nov 2022 20:40:36 GMT
ENV NATS_SERVER=2.9.7
# Thu, 17 Nov 2022 20:40:39 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='153018a675b0e896ffbed0cbc3fe5f733fd674d2f4bf554130ae8960a6c5277c' ;; 		armhf) natsArch='arm6'; sha256='9714af72c37f0ede4465a3b0324230af74701e82414194a9c2228e7563327523' ;; 		armv7) natsArch='arm7'; sha256='804ec4f600418d4afd6a9cb94b92c306ab75c589fc5180a5c2c99cc514c0899a' ;; 		x86_64) natsArch='amd64'; sha256='d4d2ef2952a9a841ce6594a4dbd07b8a45ceea32dadb321ddebc0c56598c2085' ;; 		x86) natsArch='386'; sha256='add5a328af2cab82230f881f71f7ca4dd907b477972d14a06b77b83188863d4d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 17 Nov 2022 20:40:39 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 17 Nov 2022 20:40:39 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 17 Nov 2022 20:40:39 GMT
EXPOSE 4222 6222 8222
# Thu, 17 Nov 2022 20:40:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Nov 2022 20:40:40 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:6875df1f535433e5affe18ecfde9acb7950ab5f76887980ff06c5cdd48cf98f4`  
		Last Modified: Sat, 12 Nov 2022 03:40:05 GMT  
		Size: 2.7 MB (2707756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46474a86907df61c3b68bfcfc04ccf1b583ae765e82a80c581951fb9f5e8a104`  
		Last Modified: Thu, 17 Nov 2022 20:41:10 GMT  
		Size: 4.8 MB (4794340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98cf9fbe300cc2e491de01ad75e29bc228c5e706a5140594a1c29c565216b00e`  
		Last Modified: Thu, 17 Nov 2022 20:41:09 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9323da261341d5d9bbcca4222e4b1c77ff87a4bd0aae38eb7e003bc530717bd2`  
		Last Modified: Thu, 17 Nov 2022 20:41:09 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-alpine3.16`

```console
$ docker pull nats@sha256:400adfffe0df7f2df0e76d34d6e25a0fb8eb68cfdc10d404afbbb31f818d0276
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-alpine3.16` - linux; amd64

```console
$ docker pull nats@sha256:d4698031a0afeb1ed37b240a9632b22a2d0fcea5fd48af3c8b28e1eba3348033
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.0 MB (8014859 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c26ee116aa283ae59469d995e49cce15bb982559c777e32f06933e315898c54`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Sat, 12 Nov 2022 04:19:23 GMT
ADD file:ceeb6e8632fafc657116cbf3afbd522185a16963230b57881073dad22eb0e1a3 in / 
# Sat, 12 Nov 2022 04:19:23 GMT
CMD ["/bin/sh"]
# Thu, 17 Nov 2022 20:21:36 GMT
ENV NATS_SERVER=2.9.7
# Thu, 17 Nov 2022 20:21:38 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='153018a675b0e896ffbed0cbc3fe5f733fd674d2f4bf554130ae8960a6c5277c' ;; 		armhf) natsArch='arm6'; sha256='9714af72c37f0ede4465a3b0324230af74701e82414194a9c2228e7563327523' ;; 		armv7) natsArch='arm7'; sha256='804ec4f600418d4afd6a9cb94b92c306ab75c589fc5180a5c2c99cc514c0899a' ;; 		x86_64) natsArch='amd64'; sha256='d4d2ef2952a9a841ce6594a4dbd07b8a45ceea32dadb321ddebc0c56598c2085' ;; 		x86) natsArch='386'; sha256='add5a328af2cab82230f881f71f7ca4dd907b477972d14a06b77b83188863d4d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 17 Nov 2022 20:21:38 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 17 Nov 2022 20:21:38 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 17 Nov 2022 20:21:39 GMT
EXPOSE 4222 6222 8222
# Thu, 17 Nov 2022 20:21:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Nov 2022 20:21:39 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:ca7dd9ec2225f2385955c43b2379305acd51543c28cf1d4e94522b3d94cce3ce`  
		Last Modified: Sat, 12 Nov 2022 02:52:15 GMT  
		Size: 2.8 MB (2806272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94acb566bf3ae8a5a3c0747075e8b16df167a9694bfb5ac6ccdea4e5558e2a01`  
		Last Modified: Thu, 17 Nov 2022 20:22:12 GMT  
		Size: 5.2 MB (5207590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e759e667a2c2d6d67aaf3491e124f07a1afc8de774d7973958b32b81ff7a0304`  
		Last Modified: Thu, 17 Nov 2022 20:22:11 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c0e8173963a2be8b30df5827fcfc01a70e5c95ab186696e43d9f624884cee41`  
		Last Modified: Thu, 17 Nov 2022 20:22:11 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.16` - linux; arm variant v6

```console
$ docker pull nats@sha256:221c14c269fed109042c154935b6cd22b270dda8b66b30e48f734f5fb50ffb87
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7586411 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b8f37497160e12532b20e7eaca7e50daa1304f46b7002848dfae699b06743ba`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Sat, 12 Nov 2022 03:49:18 GMT
ADD file:493290ed8856fa13463defe63da0d30ab3de5dde042c87ef7c0701d66ebb8892 in / 
# Sat, 12 Nov 2022 03:49:18 GMT
CMD ["/bin/sh"]
# Thu, 17 Nov 2022 20:49:34 GMT
ENV NATS_SERVER=2.9.7
# Thu, 17 Nov 2022 20:49:36 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='153018a675b0e896ffbed0cbc3fe5f733fd674d2f4bf554130ae8960a6c5277c' ;; 		armhf) natsArch='arm6'; sha256='9714af72c37f0ede4465a3b0324230af74701e82414194a9c2228e7563327523' ;; 		armv7) natsArch='arm7'; sha256='804ec4f600418d4afd6a9cb94b92c306ab75c589fc5180a5c2c99cc514c0899a' ;; 		x86_64) natsArch='amd64'; sha256='d4d2ef2952a9a841ce6594a4dbd07b8a45ceea32dadb321ddebc0c56598c2085' ;; 		x86) natsArch='386'; sha256='add5a328af2cab82230f881f71f7ca4dd907b477972d14a06b77b83188863d4d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 17 Nov 2022 20:49:36 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 17 Nov 2022 20:49:36 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 17 Nov 2022 20:49:36 GMT
EXPOSE 4222 6222 8222
# Thu, 17 Nov 2022 20:49:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Nov 2022 20:49:37 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9616ea8c1de4a90b1a50591336485e88ae5c2346e0d778bdbe69b00647bf8e39`  
		Last Modified: Sat, 12 Nov 2022 03:50:12 GMT  
		Size: 2.6 MB (2615105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d5728111a27515c16eb46117bf3339ccefc8af39e7c1508951d9286a3c3891c`  
		Last Modified: Thu, 17 Nov 2022 20:50:52 GMT  
		Size: 5.0 MB (4970331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d3e171e5c82f413b32d409f4fce9c56e3a429da91e068be34239e7c8c856576`  
		Last Modified: Thu, 17 Nov 2022 20:50:51 GMT  
		Size: 561.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:699b733f623013826c3dee6862aac2f7cb12bc97712d445dcf79191ba87875f6`  
		Last Modified: Thu, 17 Nov 2022 20:50:51 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.16` - linux; arm variant v7

```console
$ docker pull nats@sha256:bf2175af45ce04af8a4d8a8c810eb98dbbdf0208010f248234803a56346e7492
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.4 MB (7380724 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af540a578654dbc22e31a00269e904f93dae199d3a57c7b588311595cd8c326c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Sat, 12 Nov 2022 03:57:24 GMT
ADD file:0b4a628f529226f5ec9d357ca63138bd2d22411a889c780ac8d395d761e07b2c in / 
# Sat, 12 Nov 2022 03:57:24 GMT
CMD ["/bin/sh"]
# Thu, 17 Nov 2022 20:57:48 GMT
ENV NATS_SERVER=2.9.7
# Thu, 17 Nov 2022 20:57:51 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='153018a675b0e896ffbed0cbc3fe5f733fd674d2f4bf554130ae8960a6c5277c' ;; 		armhf) natsArch='arm6'; sha256='9714af72c37f0ede4465a3b0324230af74701e82414194a9c2228e7563327523' ;; 		armv7) natsArch='arm7'; sha256='804ec4f600418d4afd6a9cb94b92c306ab75c589fc5180a5c2c99cc514c0899a' ;; 		x86_64) natsArch='amd64'; sha256='d4d2ef2952a9a841ce6594a4dbd07b8a45ceea32dadb321ddebc0c56598c2085' ;; 		x86) natsArch='386'; sha256='add5a328af2cab82230f881f71f7ca4dd907b477972d14a06b77b83188863d4d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 17 Nov 2022 20:57:51 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 17 Nov 2022 20:57:51 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 17 Nov 2022 20:57:52 GMT
EXPOSE 4222 6222 8222
# Thu, 17 Nov 2022 20:57:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Nov 2022 20:57:52 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:e44ba29d168a7f7c9e914f3724614df9e070aa6ef9b9ba5c9004db3c071f403a`  
		Last Modified: Sat, 12 Nov 2022 03:58:16 GMT  
		Size: 2.4 MB (2418788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c6aab4ebcc741288db0b5a719ef99f393d0fd90552b7131f9391a1f1bb37575`  
		Last Modified: Thu, 17 Nov 2022 20:59:09 GMT  
		Size: 5.0 MB (4960964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c4be9c1201790ef36f0543a1ad75a874f321b98fb2053e0b742e2f74e72338e`  
		Last Modified: Thu, 17 Nov 2022 20:59:08 GMT  
		Size: 560.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6f34e641f8406d256e755f8e058c5e957c85a985209c0e0021a18e1aab450c9`  
		Last Modified: Thu, 17 Nov 2022 20:59:08 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.16` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:173181d8057b550ed4e321336b885f0ada263273ebc6cba24563f43578c00c23
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.5 MB (7503096 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:41f949bc183512a9594a4bcf404727a905c6e76f0ac0318a03cf0e2b93ccf1de`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Sat, 12 Nov 2022 03:39:38 GMT
ADD file:57d621536158358b14d15155826ef2dd4ca034278044111ec0aaf6717016e569 in / 
# Sat, 12 Nov 2022 03:39:38 GMT
CMD ["/bin/sh"]
# Thu, 17 Nov 2022 20:40:36 GMT
ENV NATS_SERVER=2.9.7
# Thu, 17 Nov 2022 20:40:39 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='153018a675b0e896ffbed0cbc3fe5f733fd674d2f4bf554130ae8960a6c5277c' ;; 		armhf) natsArch='arm6'; sha256='9714af72c37f0ede4465a3b0324230af74701e82414194a9c2228e7563327523' ;; 		armv7) natsArch='arm7'; sha256='804ec4f600418d4afd6a9cb94b92c306ab75c589fc5180a5c2c99cc514c0899a' ;; 		x86_64) natsArch='amd64'; sha256='d4d2ef2952a9a841ce6594a4dbd07b8a45ceea32dadb321ddebc0c56598c2085' ;; 		x86) natsArch='386'; sha256='add5a328af2cab82230f881f71f7ca4dd907b477972d14a06b77b83188863d4d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 17 Nov 2022 20:40:39 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 17 Nov 2022 20:40:39 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 17 Nov 2022 20:40:39 GMT
EXPOSE 4222 6222 8222
# Thu, 17 Nov 2022 20:40:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Nov 2022 20:40:40 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:6875df1f535433e5affe18ecfde9acb7950ab5f76887980ff06c5cdd48cf98f4`  
		Last Modified: Sat, 12 Nov 2022 03:40:05 GMT  
		Size: 2.7 MB (2707756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46474a86907df61c3b68bfcfc04ccf1b583ae765e82a80c581951fb9f5e8a104`  
		Last Modified: Thu, 17 Nov 2022 20:41:10 GMT  
		Size: 4.8 MB (4794340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98cf9fbe300cc2e491de01ad75e29bc228c5e706a5140594a1c29c565216b00e`  
		Last Modified: Thu, 17 Nov 2022 20:41:09 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9323da261341d5d9bbcca4222e4b1c77ff87a4bd0aae38eb7e003bc530717bd2`  
		Last Modified: Thu, 17 Nov 2022 20:41:09 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-linux`

```console
$ docker pull nats@sha256:26a7092afff4cfbdd0fc17bd33dbf3308383876690a72fd95b009500d840dce2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-linux` - linux; amd64

```console
$ docker pull nats@sha256:6fc6aee58f7a448bb3bbd803f3addfa0c9512b5083376ce20781b9b635c381cf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4918825 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:974c838918842c11cbf59d7af83a073f753537c9d4b14f47231d3c1c7ba41c9e`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 17 Nov 2022 20:21:46 GMT
COPY file:88cbf98679a4e287b67a701a1fb77e0e0928e75cc0e1e669916e033ecf774fdc in /nats-server 
# Thu, 17 Nov 2022 20:21:46 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 17 Nov 2022 20:21:46 GMT
EXPOSE 4222 6222 8222
# Thu, 17 Nov 2022 20:21:46 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 17 Nov 2022 20:21:46 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 17 Nov 2022 20:21:47 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c8ce17c05ed27e7e08286a74c292d54eb2d5902af8f901dab4505ba83f7296f5`  
		Last Modified: Thu, 17 Nov 2022 20:22:33 GMT  
		Size: 4.9 MB (4918317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88c3d57c92f61ccff2db59e857c959bc11ca2ed1a6ca7f5494aa479c513196f7`  
		Last Modified: Thu, 17 Nov 2022 20:22:32 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:9e5158db138340db27aef59e820bafe7a09359e8910c2cef451b58348dd329ff
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4683160 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b5c60a8afd73cd47b032a2d66e4968bf12f1aed52fee0f708cf184ef6c09b960`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 17 Nov 2022 20:49:48 GMT
COPY file:75f2ce97960bd08a17d41dd00b0f977ff54641b0f3d5b35f613c50553a59e8e1 in /nats-server 
# Thu, 17 Nov 2022 20:49:48 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 17 Nov 2022 20:49:49 GMT
EXPOSE 4222 6222 8222
# Thu, 17 Nov 2022 20:49:49 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 17 Nov 2022 20:49:49 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 17 Nov 2022 20:49:49 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:e27c576ee7d0df355bb5ab346016b3a399e8048fe3f938263b3b77e343d9243f`  
		Last Modified: Thu, 17 Nov 2022 20:51:22 GMT  
		Size: 4.7 MB (4682651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:788fb9f41d9d2c69e1f5737db95b3d0e754d24cd75bdd8d94a80166b8c97d6b6`  
		Last Modified: Thu, 17 Nov 2022 20:51:21 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:e4c874e4f9f5eafa49bdd7fed9a022da8958f69cc70e245af8bb9ebf7cad0c0c
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4679780 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2bc64213c48245d6c2d479e5be4d5043a6d811cb9d273ae36c8dfa157accbd04`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 17 Nov 2022 20:58:06 GMT
COPY file:ebca823a5dac00609e9fb9733528840572067b84b58dcccbe67a2df698f2869e in /nats-server 
# Thu, 17 Nov 2022 20:58:06 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 17 Nov 2022 20:58:06 GMT
EXPOSE 4222 6222 8222
# Thu, 17 Nov 2022 20:58:06 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 17 Nov 2022 20:58:06 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 17 Nov 2022 20:58:06 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:2c415cfba68b644bd88b057d832ff5015af29e04439812f5bd2e6873b3d7b8fd`  
		Last Modified: Thu, 17 Nov 2022 20:59:39 GMT  
		Size: 4.7 MB (4679272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:875032eeefdff15b8e0c04ffba01805fa83a04cad983b8322b99f53b04e9c1fe`  
		Last Modified: Thu, 17 Nov 2022 20:59:38 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:6d5eefe444c9be5d4f08fd3ccf8277d186014689ef84ea0f59c59dc11acb4904
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4504058 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7ac0ab188af08ab1a9c049a3f6c349d0d2df9595cee8e6626c19a913526dcb2`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 17 Nov 2022 20:40:45 GMT
COPY file:d11c7b340550df0716193331cacb3d06f2cb3b9971e90e006a9c153aaadc50f8 in /nats-server 
# Thu, 17 Nov 2022 20:40:45 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 17 Nov 2022 20:40:45 GMT
EXPOSE 4222 6222 8222
# Thu, 17 Nov 2022 20:40:45 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 17 Nov 2022 20:40:45 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 17 Nov 2022 20:40:45 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:d3e01af3796e331721cc924f0d95499739cea560e1ac4bac35c11176033c94c8`  
		Last Modified: Thu, 17 Nov 2022 20:41:30 GMT  
		Size: 4.5 MB (4503550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e0b7a277e0d621acb2a17025b4318262de852c8be74070453c2f8c9983601ad`  
		Last Modified: Thu, 17 Nov 2022 20:41:30 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-nanoserver`

```console
$ docker pull nats@sha256:8f26c87d964b3426a16e546857fc7873a8acc6ee97786a9366744ae849a4825d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3650; amd64

### `nats:2-nanoserver` - windows version 10.0.17763.3650; amd64

```console
$ docker pull nats@sha256:b69aaf3d5200a1cb93e65a79acaa950d17ee0b0e88be899c4c3ecd6695cf9529
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.7 MB (111704287 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a82f827f381afa49f7b9d69a162222472931dd2aad1ebbac2b60a8155e798028`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 05 Nov 2022 18:06:28 GMT
RUN Apply image 10.0.17763.3650
# Wed, 09 Nov 2022 16:47:43 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Thu, 17 Nov 2022 20:19:19 GMT
RUN cmd /S /C #(nop) COPY file:d6b547504effc3514ee13384db156b8c7df287eadd44c86f4e5f5eabb6646c1d in C:\nats-server.exe 
# Thu, 17 Nov 2022 20:19:20 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Thu, 17 Nov 2022 20:19:21 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Thu, 17 Nov 2022 20:19:21 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 17 Nov 2022 20:19:22 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:35ab4104a4d9df6a0d1eac84cc8fbc13511ef6c8aef5ced04fdf63e7e20803a3`  
		Last Modified: Tue, 08 Nov 2022 19:45:20 GMT  
		Size: 106.7 MB (106723592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6708525607bc7a2985c6a423e6cb63d6175e3ad60d997873c4519fab371772fe`  
		Last Modified: Wed, 09 Nov 2022 16:48:43 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cb5d7747e73374a2c02473deb4bde157dddb2835cb5e66800cfba5842c1fd88`  
		Last Modified: Thu, 17 Nov 2022 20:20:12 GMT  
		Size: 5.0 MB (4974250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b3d427408549420b1666d1a85d3ff1bd3132f4e61dd9a7bd4e75a7c5adc32ee`  
		Last Modified: Thu, 17 Nov 2022 20:20:11 GMT  
		Size: 1.8 KB (1811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4682e51d5cc8bfadb600b57559df30d236b94223a5e9b1c3d2468f6acb1ee3f3`  
		Last Modified: Thu, 17 Nov 2022 20:20:11 GMT  
		Size: 1.2 KB (1161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8223b92ce81db067bb8ee9eacbf53e251b0dcd29dd1af6aa3a519768f0a7b44b`  
		Last Modified: Thu, 17 Nov 2022 20:20:11 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51f050378e256630049566bfcc0cf782533a8f961bcae8b6d9421ef19a8a780f`  
		Last Modified: Thu, 17 Nov 2022 20:20:11 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-nanoserver-1809`

```console
$ docker pull nats@sha256:8f26c87d964b3426a16e546857fc7873a8acc6ee97786a9366744ae849a4825d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3650; amd64

### `nats:2-nanoserver-1809` - windows version 10.0.17763.3650; amd64

```console
$ docker pull nats@sha256:b69aaf3d5200a1cb93e65a79acaa950d17ee0b0e88be899c4c3ecd6695cf9529
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.7 MB (111704287 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a82f827f381afa49f7b9d69a162222472931dd2aad1ebbac2b60a8155e798028`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 05 Nov 2022 18:06:28 GMT
RUN Apply image 10.0.17763.3650
# Wed, 09 Nov 2022 16:47:43 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Thu, 17 Nov 2022 20:19:19 GMT
RUN cmd /S /C #(nop) COPY file:d6b547504effc3514ee13384db156b8c7df287eadd44c86f4e5f5eabb6646c1d in C:\nats-server.exe 
# Thu, 17 Nov 2022 20:19:20 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Thu, 17 Nov 2022 20:19:21 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Thu, 17 Nov 2022 20:19:21 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 17 Nov 2022 20:19:22 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:35ab4104a4d9df6a0d1eac84cc8fbc13511ef6c8aef5ced04fdf63e7e20803a3`  
		Last Modified: Tue, 08 Nov 2022 19:45:20 GMT  
		Size: 106.7 MB (106723592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6708525607bc7a2985c6a423e6cb63d6175e3ad60d997873c4519fab371772fe`  
		Last Modified: Wed, 09 Nov 2022 16:48:43 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cb5d7747e73374a2c02473deb4bde157dddb2835cb5e66800cfba5842c1fd88`  
		Last Modified: Thu, 17 Nov 2022 20:20:12 GMT  
		Size: 5.0 MB (4974250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b3d427408549420b1666d1a85d3ff1bd3132f4e61dd9a7bd4e75a7c5adc32ee`  
		Last Modified: Thu, 17 Nov 2022 20:20:11 GMT  
		Size: 1.8 KB (1811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4682e51d5cc8bfadb600b57559df30d236b94223a5e9b1c3d2468f6acb1ee3f3`  
		Last Modified: Thu, 17 Nov 2022 20:20:11 GMT  
		Size: 1.2 KB (1161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8223b92ce81db067bb8ee9eacbf53e251b0dcd29dd1af6aa3a519768f0a7b44b`  
		Last Modified: Thu, 17 Nov 2022 20:20:11 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51f050378e256630049566bfcc0cf782533a8f961bcae8b6d9421ef19a8a780f`  
		Last Modified: Thu, 17 Nov 2022 20:20:11 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-scratch`

```console
$ docker pull nats@sha256:26a7092afff4cfbdd0fc17bd33dbf3308383876690a72fd95b009500d840dce2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-scratch` - linux; amd64

```console
$ docker pull nats@sha256:6fc6aee58f7a448bb3bbd803f3addfa0c9512b5083376ce20781b9b635c381cf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4918825 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:974c838918842c11cbf59d7af83a073f753537c9d4b14f47231d3c1c7ba41c9e`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 17 Nov 2022 20:21:46 GMT
COPY file:88cbf98679a4e287b67a701a1fb77e0e0928e75cc0e1e669916e033ecf774fdc in /nats-server 
# Thu, 17 Nov 2022 20:21:46 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 17 Nov 2022 20:21:46 GMT
EXPOSE 4222 6222 8222
# Thu, 17 Nov 2022 20:21:46 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 17 Nov 2022 20:21:46 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 17 Nov 2022 20:21:47 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c8ce17c05ed27e7e08286a74c292d54eb2d5902af8f901dab4505ba83f7296f5`  
		Last Modified: Thu, 17 Nov 2022 20:22:33 GMT  
		Size: 4.9 MB (4918317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88c3d57c92f61ccff2db59e857c959bc11ca2ed1a6ca7f5494aa479c513196f7`  
		Last Modified: Thu, 17 Nov 2022 20:22:32 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:9e5158db138340db27aef59e820bafe7a09359e8910c2cef451b58348dd329ff
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4683160 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b5c60a8afd73cd47b032a2d66e4968bf12f1aed52fee0f708cf184ef6c09b960`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 17 Nov 2022 20:49:48 GMT
COPY file:75f2ce97960bd08a17d41dd00b0f977ff54641b0f3d5b35f613c50553a59e8e1 in /nats-server 
# Thu, 17 Nov 2022 20:49:48 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 17 Nov 2022 20:49:49 GMT
EXPOSE 4222 6222 8222
# Thu, 17 Nov 2022 20:49:49 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 17 Nov 2022 20:49:49 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 17 Nov 2022 20:49:49 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:e27c576ee7d0df355bb5ab346016b3a399e8048fe3f938263b3b77e343d9243f`  
		Last Modified: Thu, 17 Nov 2022 20:51:22 GMT  
		Size: 4.7 MB (4682651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:788fb9f41d9d2c69e1f5737db95b3d0e754d24cd75bdd8d94a80166b8c97d6b6`  
		Last Modified: Thu, 17 Nov 2022 20:51:21 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:e4c874e4f9f5eafa49bdd7fed9a022da8958f69cc70e245af8bb9ebf7cad0c0c
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4679780 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2bc64213c48245d6c2d479e5be4d5043a6d811cb9d273ae36c8dfa157accbd04`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 17 Nov 2022 20:58:06 GMT
COPY file:ebca823a5dac00609e9fb9733528840572067b84b58dcccbe67a2df698f2869e in /nats-server 
# Thu, 17 Nov 2022 20:58:06 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 17 Nov 2022 20:58:06 GMT
EXPOSE 4222 6222 8222
# Thu, 17 Nov 2022 20:58:06 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 17 Nov 2022 20:58:06 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 17 Nov 2022 20:58:06 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:2c415cfba68b644bd88b057d832ff5015af29e04439812f5bd2e6873b3d7b8fd`  
		Last Modified: Thu, 17 Nov 2022 20:59:39 GMT  
		Size: 4.7 MB (4679272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:875032eeefdff15b8e0c04ffba01805fa83a04cad983b8322b99f53b04e9c1fe`  
		Last Modified: Thu, 17 Nov 2022 20:59:38 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:6d5eefe444c9be5d4f08fd3ccf8277d186014689ef84ea0f59c59dc11acb4904
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4504058 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7ac0ab188af08ab1a9c049a3f6c349d0d2df9595cee8e6626c19a913526dcb2`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 17 Nov 2022 20:40:45 GMT
COPY file:d11c7b340550df0716193331cacb3d06f2cb3b9971e90e006a9c153aaadc50f8 in /nats-server 
# Thu, 17 Nov 2022 20:40:45 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 17 Nov 2022 20:40:45 GMT
EXPOSE 4222 6222 8222
# Thu, 17 Nov 2022 20:40:45 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 17 Nov 2022 20:40:45 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 17 Nov 2022 20:40:45 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:d3e01af3796e331721cc924f0d95499739cea560e1ac4bac35c11176033c94c8`  
		Last Modified: Thu, 17 Nov 2022 20:41:30 GMT  
		Size: 4.5 MB (4503550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e0b7a277e0d621acb2a17025b4318262de852c8be74070453c2f8c9983601ad`  
		Last Modified: Thu, 17 Nov 2022 20:41:30 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-windowsservercore`

```console
$ docker pull nats@sha256:a2a17b6c8e185249db8f657d5b4b5473e4627feb0a7ea39ac121544d7ab11465
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3650; amd64

### `nats:2-windowsservercore` - windows version 10.0.17763.3650; amd64

```console
$ docker pull nats@sha256:d42d0b0ee29bdd7b0ea24be91fb754a64a3da2ab070ed93e185e983132b9beec
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2784314848 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a836a477662568b8b4f2cd2ba8211273a6ae351f51fd48d29015400f42f395c`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 05 Nov 2022 18:29:26 GMT
RUN Install update 10.0.17763.3650
# Wed, 09 Nov 2022 14:50:58 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Nov 2022 16:44:45 GMT
ENV NATS_DOCKERIZED=1
# Thu, 17 Nov 2022 20:15:26 GMT
ENV NATS_SERVER=2.9.7
# Thu, 17 Nov 2022 20:15:27 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.9.7/nats-server-v2.9.7-windows-amd64.zip
# Thu, 17 Nov 2022 20:15:28 GMT
ENV NATS_SERVER_SHASUM=f1baa1646b7a499d035ebfd529644c1379988ab69703a090f9899c97067cea02
# Thu, 17 Nov 2022 20:17:00 GMT
RUN Set-PSDebug -Trace 2
# Thu, 17 Nov 2022 20:18:59 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Thu, 17 Nov 2022 20:19:00 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Thu, 17 Nov 2022 20:19:01 GMT
EXPOSE 4222 6222 8222
# Thu, 17 Nov 2022 20:19:02 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 17 Nov 2022 20:19:03 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a48a3e4ae2de839d8e99bde16eb91d113fb2cf889bba472d0c4274851b5fb402`  
		Last Modified: Tue, 21 Jun 2022 18:30:17 GMT  
		Size: 1.9 GB (1924269350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c26cc6e4f9eb1ae415a5ead6f884cac597bbd57efa6cd042c878d5b54c9d2091`  
		Last Modified: Tue, 08 Nov 2022 19:44:35 GMT  
		Size: 854.3 MB (854317461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99941fb33972e616b231a8aadd93463fdfd5de6aece4aa6c470d2feec31839be`  
		Last Modified: Wed, 09 Nov 2022 16:48:23 GMT  
		Size: 1.3 KB (1335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0f3d8a87f0a1540850986ff94131286dfa42ca116f04779e02f60b3a724641b`  
		Last Modified: Wed, 09 Nov 2022 16:48:23 GMT  
		Size: 1.3 KB (1327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69b8ead5903ee0014b1d59597e3e42c54eb9ad338e077477176b04d22ab4f291`  
		Last Modified: Thu, 17 Nov 2022 20:19:56 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd5112842b491d9aed12c373a680aa352fda7856f4dd7ae100240cda81004d10`  
		Last Modified: Thu, 17 Nov 2022 20:19:56 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27e8ac611281af798a4d5c0f0ffeca3542a44a865688ca95c3f963d0f3a2b009`  
		Last Modified: Thu, 17 Nov 2022 20:19:56 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ced45d282af98e490deb218ae7d77ad9ee20038016ea5fad600ab6363d4339fd`  
		Last Modified: Thu, 17 Nov 2022 20:19:56 GMT  
		Size: 381.6 KB (381592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d244e04b249f9171046dc315cd9c7d70aadbaa6496d85f41de583773d750a76b`  
		Last Modified: Thu, 17 Nov 2022 20:19:55 GMT  
		Size: 5.3 MB (5333250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e9dc3cf2f9c57dc6d24c7b6d3a526d97d4c7ef1de724d54dae9ad10211ba0e1`  
		Last Modified: Thu, 17 Nov 2022 20:19:54 GMT  
		Size: 2.0 KB (2001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6e0bb8f7d2e8165a51f2f77c4ee12feb907b21e4a5f2fe8c6215e6ee1c3b075`  
		Last Modified: Thu, 17 Nov 2022 20:19:54 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80326cc866c490bc13a4ead203b6b1af79320652c34f6605511671f003980078`  
		Last Modified: Thu, 17 Nov 2022 20:19:54 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7785e4126ef3eb2bac999118a556a59d9ab9474c8175a5742b4a1c7fba660efe`  
		Last Modified: Thu, 17 Nov 2022 20:19:54 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-windowsservercore-1809`

```console
$ docker pull nats@sha256:a2a17b6c8e185249db8f657d5b4b5473e4627feb0a7ea39ac121544d7ab11465
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3650; amd64

### `nats:2-windowsservercore-1809` - windows version 10.0.17763.3650; amd64

```console
$ docker pull nats@sha256:d42d0b0ee29bdd7b0ea24be91fb754a64a3da2ab070ed93e185e983132b9beec
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2784314848 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a836a477662568b8b4f2cd2ba8211273a6ae351f51fd48d29015400f42f395c`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 05 Nov 2022 18:29:26 GMT
RUN Install update 10.0.17763.3650
# Wed, 09 Nov 2022 14:50:58 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Nov 2022 16:44:45 GMT
ENV NATS_DOCKERIZED=1
# Thu, 17 Nov 2022 20:15:26 GMT
ENV NATS_SERVER=2.9.7
# Thu, 17 Nov 2022 20:15:27 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.9.7/nats-server-v2.9.7-windows-amd64.zip
# Thu, 17 Nov 2022 20:15:28 GMT
ENV NATS_SERVER_SHASUM=f1baa1646b7a499d035ebfd529644c1379988ab69703a090f9899c97067cea02
# Thu, 17 Nov 2022 20:17:00 GMT
RUN Set-PSDebug -Trace 2
# Thu, 17 Nov 2022 20:18:59 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Thu, 17 Nov 2022 20:19:00 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Thu, 17 Nov 2022 20:19:01 GMT
EXPOSE 4222 6222 8222
# Thu, 17 Nov 2022 20:19:02 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 17 Nov 2022 20:19:03 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a48a3e4ae2de839d8e99bde16eb91d113fb2cf889bba472d0c4274851b5fb402`  
		Last Modified: Tue, 21 Jun 2022 18:30:17 GMT  
		Size: 1.9 GB (1924269350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c26cc6e4f9eb1ae415a5ead6f884cac597bbd57efa6cd042c878d5b54c9d2091`  
		Last Modified: Tue, 08 Nov 2022 19:44:35 GMT  
		Size: 854.3 MB (854317461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99941fb33972e616b231a8aadd93463fdfd5de6aece4aa6c470d2feec31839be`  
		Last Modified: Wed, 09 Nov 2022 16:48:23 GMT  
		Size: 1.3 KB (1335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0f3d8a87f0a1540850986ff94131286dfa42ca116f04779e02f60b3a724641b`  
		Last Modified: Wed, 09 Nov 2022 16:48:23 GMT  
		Size: 1.3 KB (1327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69b8ead5903ee0014b1d59597e3e42c54eb9ad338e077477176b04d22ab4f291`  
		Last Modified: Thu, 17 Nov 2022 20:19:56 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd5112842b491d9aed12c373a680aa352fda7856f4dd7ae100240cda81004d10`  
		Last Modified: Thu, 17 Nov 2022 20:19:56 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27e8ac611281af798a4d5c0f0ffeca3542a44a865688ca95c3f963d0f3a2b009`  
		Last Modified: Thu, 17 Nov 2022 20:19:56 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ced45d282af98e490deb218ae7d77ad9ee20038016ea5fad600ab6363d4339fd`  
		Last Modified: Thu, 17 Nov 2022 20:19:56 GMT  
		Size: 381.6 KB (381592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d244e04b249f9171046dc315cd9c7d70aadbaa6496d85f41de583773d750a76b`  
		Last Modified: Thu, 17 Nov 2022 20:19:55 GMT  
		Size: 5.3 MB (5333250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e9dc3cf2f9c57dc6d24c7b6d3a526d97d4c7ef1de724d54dae9ad10211ba0e1`  
		Last Modified: Thu, 17 Nov 2022 20:19:54 GMT  
		Size: 2.0 KB (2001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6e0bb8f7d2e8165a51f2f77c4ee12feb907b21e4a5f2fe8c6215e6ee1c3b075`  
		Last Modified: Thu, 17 Nov 2022 20:19:54 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80326cc866c490bc13a4ead203b6b1af79320652c34f6605511671f003980078`  
		Last Modified: Thu, 17 Nov 2022 20:19:54 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7785e4126ef3eb2bac999118a556a59d9ab9474c8175a5742b4a1c7fba660efe`  
		Last Modified: Thu, 17 Nov 2022 20:19:54 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9`

```console
$ docker pull nats@sha256:8a550ace09f524090c5399c7eab008c9f0d55a29eb1732cc4a565d4f1160346c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.3650; amd64

### `nats:2.9` - linux; amd64

```console
$ docker pull nats@sha256:6fc6aee58f7a448bb3bbd803f3addfa0c9512b5083376ce20781b9b635c381cf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4918825 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:974c838918842c11cbf59d7af83a073f753537c9d4b14f47231d3c1c7ba41c9e`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 17 Nov 2022 20:21:46 GMT
COPY file:88cbf98679a4e287b67a701a1fb77e0e0928e75cc0e1e669916e033ecf774fdc in /nats-server 
# Thu, 17 Nov 2022 20:21:46 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 17 Nov 2022 20:21:46 GMT
EXPOSE 4222 6222 8222
# Thu, 17 Nov 2022 20:21:46 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 17 Nov 2022 20:21:46 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 17 Nov 2022 20:21:47 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c8ce17c05ed27e7e08286a74c292d54eb2d5902af8f901dab4505ba83f7296f5`  
		Last Modified: Thu, 17 Nov 2022 20:22:33 GMT  
		Size: 4.9 MB (4918317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88c3d57c92f61ccff2db59e857c959bc11ca2ed1a6ca7f5494aa479c513196f7`  
		Last Modified: Thu, 17 Nov 2022 20:22:32 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9` - linux; arm variant v6

```console
$ docker pull nats@sha256:9e5158db138340db27aef59e820bafe7a09359e8910c2cef451b58348dd329ff
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4683160 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b5c60a8afd73cd47b032a2d66e4968bf12f1aed52fee0f708cf184ef6c09b960`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 17 Nov 2022 20:49:48 GMT
COPY file:75f2ce97960bd08a17d41dd00b0f977ff54641b0f3d5b35f613c50553a59e8e1 in /nats-server 
# Thu, 17 Nov 2022 20:49:48 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 17 Nov 2022 20:49:49 GMT
EXPOSE 4222 6222 8222
# Thu, 17 Nov 2022 20:49:49 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 17 Nov 2022 20:49:49 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 17 Nov 2022 20:49:49 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:e27c576ee7d0df355bb5ab346016b3a399e8048fe3f938263b3b77e343d9243f`  
		Last Modified: Thu, 17 Nov 2022 20:51:22 GMT  
		Size: 4.7 MB (4682651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:788fb9f41d9d2c69e1f5737db95b3d0e754d24cd75bdd8d94a80166b8c97d6b6`  
		Last Modified: Thu, 17 Nov 2022 20:51:21 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9` - linux; arm variant v7

```console
$ docker pull nats@sha256:e4c874e4f9f5eafa49bdd7fed9a022da8958f69cc70e245af8bb9ebf7cad0c0c
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4679780 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2bc64213c48245d6c2d479e5be4d5043a6d811cb9d273ae36c8dfa157accbd04`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 17 Nov 2022 20:58:06 GMT
COPY file:ebca823a5dac00609e9fb9733528840572067b84b58dcccbe67a2df698f2869e in /nats-server 
# Thu, 17 Nov 2022 20:58:06 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 17 Nov 2022 20:58:06 GMT
EXPOSE 4222 6222 8222
# Thu, 17 Nov 2022 20:58:06 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 17 Nov 2022 20:58:06 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 17 Nov 2022 20:58:06 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:2c415cfba68b644bd88b057d832ff5015af29e04439812f5bd2e6873b3d7b8fd`  
		Last Modified: Thu, 17 Nov 2022 20:59:39 GMT  
		Size: 4.7 MB (4679272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:875032eeefdff15b8e0c04ffba01805fa83a04cad983b8322b99f53b04e9c1fe`  
		Last Modified: Thu, 17 Nov 2022 20:59:38 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:6d5eefe444c9be5d4f08fd3ccf8277d186014689ef84ea0f59c59dc11acb4904
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4504058 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7ac0ab188af08ab1a9c049a3f6c349d0d2df9595cee8e6626c19a913526dcb2`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 17 Nov 2022 20:40:45 GMT
COPY file:d11c7b340550df0716193331cacb3d06f2cb3b9971e90e006a9c153aaadc50f8 in /nats-server 
# Thu, 17 Nov 2022 20:40:45 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 17 Nov 2022 20:40:45 GMT
EXPOSE 4222 6222 8222
# Thu, 17 Nov 2022 20:40:45 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 17 Nov 2022 20:40:45 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 17 Nov 2022 20:40:45 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:d3e01af3796e331721cc924f0d95499739cea560e1ac4bac35c11176033c94c8`  
		Last Modified: Thu, 17 Nov 2022 20:41:30 GMT  
		Size: 4.5 MB (4503550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e0b7a277e0d621acb2a17025b4318262de852c8be74070453c2f8c9983601ad`  
		Last Modified: Thu, 17 Nov 2022 20:41:30 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9` - windows version 10.0.17763.3650; amd64

```console
$ docker pull nats@sha256:b69aaf3d5200a1cb93e65a79acaa950d17ee0b0e88be899c4c3ecd6695cf9529
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.7 MB (111704287 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a82f827f381afa49f7b9d69a162222472931dd2aad1ebbac2b60a8155e798028`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 05 Nov 2022 18:06:28 GMT
RUN Apply image 10.0.17763.3650
# Wed, 09 Nov 2022 16:47:43 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Thu, 17 Nov 2022 20:19:19 GMT
RUN cmd /S /C #(nop) COPY file:d6b547504effc3514ee13384db156b8c7df287eadd44c86f4e5f5eabb6646c1d in C:\nats-server.exe 
# Thu, 17 Nov 2022 20:19:20 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Thu, 17 Nov 2022 20:19:21 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Thu, 17 Nov 2022 20:19:21 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 17 Nov 2022 20:19:22 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:35ab4104a4d9df6a0d1eac84cc8fbc13511ef6c8aef5ced04fdf63e7e20803a3`  
		Last Modified: Tue, 08 Nov 2022 19:45:20 GMT  
		Size: 106.7 MB (106723592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6708525607bc7a2985c6a423e6cb63d6175e3ad60d997873c4519fab371772fe`  
		Last Modified: Wed, 09 Nov 2022 16:48:43 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cb5d7747e73374a2c02473deb4bde157dddb2835cb5e66800cfba5842c1fd88`  
		Last Modified: Thu, 17 Nov 2022 20:20:12 GMT  
		Size: 5.0 MB (4974250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b3d427408549420b1666d1a85d3ff1bd3132f4e61dd9a7bd4e75a7c5adc32ee`  
		Last Modified: Thu, 17 Nov 2022 20:20:11 GMT  
		Size: 1.8 KB (1811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4682e51d5cc8bfadb600b57559df30d236b94223a5e9b1c3d2468f6acb1ee3f3`  
		Last Modified: Thu, 17 Nov 2022 20:20:11 GMT  
		Size: 1.2 KB (1161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8223b92ce81db067bb8ee9eacbf53e251b0dcd29dd1af6aa3a519768f0a7b44b`  
		Last Modified: Thu, 17 Nov 2022 20:20:11 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51f050378e256630049566bfcc0cf782533a8f961bcae8b6d9421ef19a8a780f`  
		Last Modified: Thu, 17 Nov 2022 20:20:11 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-alpine`

```console
$ docker pull nats@sha256:400adfffe0df7f2df0e76d34d6e25a0fb8eb68cfdc10d404afbbb31f818d0276
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9-alpine` - linux; amd64

```console
$ docker pull nats@sha256:d4698031a0afeb1ed37b240a9632b22a2d0fcea5fd48af3c8b28e1eba3348033
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.0 MB (8014859 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c26ee116aa283ae59469d995e49cce15bb982559c777e32f06933e315898c54`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Sat, 12 Nov 2022 04:19:23 GMT
ADD file:ceeb6e8632fafc657116cbf3afbd522185a16963230b57881073dad22eb0e1a3 in / 
# Sat, 12 Nov 2022 04:19:23 GMT
CMD ["/bin/sh"]
# Thu, 17 Nov 2022 20:21:36 GMT
ENV NATS_SERVER=2.9.7
# Thu, 17 Nov 2022 20:21:38 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='153018a675b0e896ffbed0cbc3fe5f733fd674d2f4bf554130ae8960a6c5277c' ;; 		armhf) natsArch='arm6'; sha256='9714af72c37f0ede4465a3b0324230af74701e82414194a9c2228e7563327523' ;; 		armv7) natsArch='arm7'; sha256='804ec4f600418d4afd6a9cb94b92c306ab75c589fc5180a5c2c99cc514c0899a' ;; 		x86_64) natsArch='amd64'; sha256='d4d2ef2952a9a841ce6594a4dbd07b8a45ceea32dadb321ddebc0c56598c2085' ;; 		x86) natsArch='386'; sha256='add5a328af2cab82230f881f71f7ca4dd907b477972d14a06b77b83188863d4d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 17 Nov 2022 20:21:38 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 17 Nov 2022 20:21:38 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 17 Nov 2022 20:21:39 GMT
EXPOSE 4222 6222 8222
# Thu, 17 Nov 2022 20:21:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Nov 2022 20:21:39 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:ca7dd9ec2225f2385955c43b2379305acd51543c28cf1d4e94522b3d94cce3ce`  
		Last Modified: Sat, 12 Nov 2022 02:52:15 GMT  
		Size: 2.8 MB (2806272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94acb566bf3ae8a5a3c0747075e8b16df167a9694bfb5ac6ccdea4e5558e2a01`  
		Last Modified: Thu, 17 Nov 2022 20:22:12 GMT  
		Size: 5.2 MB (5207590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e759e667a2c2d6d67aaf3491e124f07a1afc8de774d7973958b32b81ff7a0304`  
		Last Modified: Thu, 17 Nov 2022 20:22:11 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c0e8173963a2be8b30df5827fcfc01a70e5c95ab186696e43d9f624884cee41`  
		Last Modified: Thu, 17 Nov 2022 20:22:11 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:221c14c269fed109042c154935b6cd22b270dda8b66b30e48f734f5fb50ffb87
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7586411 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b8f37497160e12532b20e7eaca7e50daa1304f46b7002848dfae699b06743ba`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Sat, 12 Nov 2022 03:49:18 GMT
ADD file:493290ed8856fa13463defe63da0d30ab3de5dde042c87ef7c0701d66ebb8892 in / 
# Sat, 12 Nov 2022 03:49:18 GMT
CMD ["/bin/sh"]
# Thu, 17 Nov 2022 20:49:34 GMT
ENV NATS_SERVER=2.9.7
# Thu, 17 Nov 2022 20:49:36 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='153018a675b0e896ffbed0cbc3fe5f733fd674d2f4bf554130ae8960a6c5277c' ;; 		armhf) natsArch='arm6'; sha256='9714af72c37f0ede4465a3b0324230af74701e82414194a9c2228e7563327523' ;; 		armv7) natsArch='arm7'; sha256='804ec4f600418d4afd6a9cb94b92c306ab75c589fc5180a5c2c99cc514c0899a' ;; 		x86_64) natsArch='amd64'; sha256='d4d2ef2952a9a841ce6594a4dbd07b8a45ceea32dadb321ddebc0c56598c2085' ;; 		x86) natsArch='386'; sha256='add5a328af2cab82230f881f71f7ca4dd907b477972d14a06b77b83188863d4d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 17 Nov 2022 20:49:36 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 17 Nov 2022 20:49:36 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 17 Nov 2022 20:49:36 GMT
EXPOSE 4222 6222 8222
# Thu, 17 Nov 2022 20:49:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Nov 2022 20:49:37 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9616ea8c1de4a90b1a50591336485e88ae5c2346e0d778bdbe69b00647bf8e39`  
		Last Modified: Sat, 12 Nov 2022 03:50:12 GMT  
		Size: 2.6 MB (2615105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d5728111a27515c16eb46117bf3339ccefc8af39e7c1508951d9286a3c3891c`  
		Last Modified: Thu, 17 Nov 2022 20:50:52 GMT  
		Size: 5.0 MB (4970331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d3e171e5c82f413b32d409f4fce9c56e3a429da91e068be34239e7c8c856576`  
		Last Modified: Thu, 17 Nov 2022 20:50:51 GMT  
		Size: 561.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:699b733f623013826c3dee6862aac2f7cb12bc97712d445dcf79191ba87875f6`  
		Last Modified: Thu, 17 Nov 2022 20:50:51 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:bf2175af45ce04af8a4d8a8c810eb98dbbdf0208010f248234803a56346e7492
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.4 MB (7380724 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af540a578654dbc22e31a00269e904f93dae199d3a57c7b588311595cd8c326c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Sat, 12 Nov 2022 03:57:24 GMT
ADD file:0b4a628f529226f5ec9d357ca63138bd2d22411a889c780ac8d395d761e07b2c in / 
# Sat, 12 Nov 2022 03:57:24 GMT
CMD ["/bin/sh"]
# Thu, 17 Nov 2022 20:57:48 GMT
ENV NATS_SERVER=2.9.7
# Thu, 17 Nov 2022 20:57:51 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='153018a675b0e896ffbed0cbc3fe5f733fd674d2f4bf554130ae8960a6c5277c' ;; 		armhf) natsArch='arm6'; sha256='9714af72c37f0ede4465a3b0324230af74701e82414194a9c2228e7563327523' ;; 		armv7) natsArch='arm7'; sha256='804ec4f600418d4afd6a9cb94b92c306ab75c589fc5180a5c2c99cc514c0899a' ;; 		x86_64) natsArch='amd64'; sha256='d4d2ef2952a9a841ce6594a4dbd07b8a45ceea32dadb321ddebc0c56598c2085' ;; 		x86) natsArch='386'; sha256='add5a328af2cab82230f881f71f7ca4dd907b477972d14a06b77b83188863d4d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 17 Nov 2022 20:57:51 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 17 Nov 2022 20:57:51 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 17 Nov 2022 20:57:52 GMT
EXPOSE 4222 6222 8222
# Thu, 17 Nov 2022 20:57:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Nov 2022 20:57:52 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:e44ba29d168a7f7c9e914f3724614df9e070aa6ef9b9ba5c9004db3c071f403a`  
		Last Modified: Sat, 12 Nov 2022 03:58:16 GMT  
		Size: 2.4 MB (2418788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c6aab4ebcc741288db0b5a719ef99f393d0fd90552b7131f9391a1f1bb37575`  
		Last Modified: Thu, 17 Nov 2022 20:59:09 GMT  
		Size: 5.0 MB (4960964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c4be9c1201790ef36f0543a1ad75a874f321b98fb2053e0b742e2f74e72338e`  
		Last Modified: Thu, 17 Nov 2022 20:59:08 GMT  
		Size: 560.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6f34e641f8406d256e755f8e058c5e957c85a985209c0e0021a18e1aab450c9`  
		Last Modified: Thu, 17 Nov 2022 20:59:08 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:173181d8057b550ed4e321336b885f0ada263273ebc6cba24563f43578c00c23
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.5 MB (7503096 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:41f949bc183512a9594a4bcf404727a905c6e76f0ac0318a03cf0e2b93ccf1de`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Sat, 12 Nov 2022 03:39:38 GMT
ADD file:57d621536158358b14d15155826ef2dd4ca034278044111ec0aaf6717016e569 in / 
# Sat, 12 Nov 2022 03:39:38 GMT
CMD ["/bin/sh"]
# Thu, 17 Nov 2022 20:40:36 GMT
ENV NATS_SERVER=2.9.7
# Thu, 17 Nov 2022 20:40:39 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='153018a675b0e896ffbed0cbc3fe5f733fd674d2f4bf554130ae8960a6c5277c' ;; 		armhf) natsArch='arm6'; sha256='9714af72c37f0ede4465a3b0324230af74701e82414194a9c2228e7563327523' ;; 		armv7) natsArch='arm7'; sha256='804ec4f600418d4afd6a9cb94b92c306ab75c589fc5180a5c2c99cc514c0899a' ;; 		x86_64) natsArch='amd64'; sha256='d4d2ef2952a9a841ce6594a4dbd07b8a45ceea32dadb321ddebc0c56598c2085' ;; 		x86) natsArch='386'; sha256='add5a328af2cab82230f881f71f7ca4dd907b477972d14a06b77b83188863d4d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 17 Nov 2022 20:40:39 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 17 Nov 2022 20:40:39 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 17 Nov 2022 20:40:39 GMT
EXPOSE 4222 6222 8222
# Thu, 17 Nov 2022 20:40:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Nov 2022 20:40:40 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:6875df1f535433e5affe18ecfde9acb7950ab5f76887980ff06c5cdd48cf98f4`  
		Last Modified: Sat, 12 Nov 2022 03:40:05 GMT  
		Size: 2.7 MB (2707756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46474a86907df61c3b68bfcfc04ccf1b583ae765e82a80c581951fb9f5e8a104`  
		Last Modified: Thu, 17 Nov 2022 20:41:10 GMT  
		Size: 4.8 MB (4794340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98cf9fbe300cc2e491de01ad75e29bc228c5e706a5140594a1c29c565216b00e`  
		Last Modified: Thu, 17 Nov 2022 20:41:09 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9323da261341d5d9bbcca4222e4b1c77ff87a4bd0aae38eb7e003bc530717bd2`  
		Last Modified: Thu, 17 Nov 2022 20:41:09 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-alpine3.16`

```console
$ docker pull nats@sha256:400adfffe0df7f2df0e76d34d6e25a0fb8eb68cfdc10d404afbbb31f818d0276
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9-alpine3.16` - linux; amd64

```console
$ docker pull nats@sha256:d4698031a0afeb1ed37b240a9632b22a2d0fcea5fd48af3c8b28e1eba3348033
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.0 MB (8014859 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c26ee116aa283ae59469d995e49cce15bb982559c777e32f06933e315898c54`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Sat, 12 Nov 2022 04:19:23 GMT
ADD file:ceeb6e8632fafc657116cbf3afbd522185a16963230b57881073dad22eb0e1a3 in / 
# Sat, 12 Nov 2022 04:19:23 GMT
CMD ["/bin/sh"]
# Thu, 17 Nov 2022 20:21:36 GMT
ENV NATS_SERVER=2.9.7
# Thu, 17 Nov 2022 20:21:38 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='153018a675b0e896ffbed0cbc3fe5f733fd674d2f4bf554130ae8960a6c5277c' ;; 		armhf) natsArch='arm6'; sha256='9714af72c37f0ede4465a3b0324230af74701e82414194a9c2228e7563327523' ;; 		armv7) natsArch='arm7'; sha256='804ec4f600418d4afd6a9cb94b92c306ab75c589fc5180a5c2c99cc514c0899a' ;; 		x86_64) natsArch='amd64'; sha256='d4d2ef2952a9a841ce6594a4dbd07b8a45ceea32dadb321ddebc0c56598c2085' ;; 		x86) natsArch='386'; sha256='add5a328af2cab82230f881f71f7ca4dd907b477972d14a06b77b83188863d4d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 17 Nov 2022 20:21:38 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 17 Nov 2022 20:21:38 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 17 Nov 2022 20:21:39 GMT
EXPOSE 4222 6222 8222
# Thu, 17 Nov 2022 20:21:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Nov 2022 20:21:39 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:ca7dd9ec2225f2385955c43b2379305acd51543c28cf1d4e94522b3d94cce3ce`  
		Last Modified: Sat, 12 Nov 2022 02:52:15 GMT  
		Size: 2.8 MB (2806272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94acb566bf3ae8a5a3c0747075e8b16df167a9694bfb5ac6ccdea4e5558e2a01`  
		Last Modified: Thu, 17 Nov 2022 20:22:12 GMT  
		Size: 5.2 MB (5207590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e759e667a2c2d6d67aaf3491e124f07a1afc8de774d7973958b32b81ff7a0304`  
		Last Modified: Thu, 17 Nov 2022 20:22:11 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c0e8173963a2be8b30df5827fcfc01a70e5c95ab186696e43d9f624884cee41`  
		Last Modified: Thu, 17 Nov 2022 20:22:11 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-alpine3.16` - linux; arm variant v6

```console
$ docker pull nats@sha256:221c14c269fed109042c154935b6cd22b270dda8b66b30e48f734f5fb50ffb87
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7586411 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b8f37497160e12532b20e7eaca7e50daa1304f46b7002848dfae699b06743ba`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Sat, 12 Nov 2022 03:49:18 GMT
ADD file:493290ed8856fa13463defe63da0d30ab3de5dde042c87ef7c0701d66ebb8892 in / 
# Sat, 12 Nov 2022 03:49:18 GMT
CMD ["/bin/sh"]
# Thu, 17 Nov 2022 20:49:34 GMT
ENV NATS_SERVER=2.9.7
# Thu, 17 Nov 2022 20:49:36 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='153018a675b0e896ffbed0cbc3fe5f733fd674d2f4bf554130ae8960a6c5277c' ;; 		armhf) natsArch='arm6'; sha256='9714af72c37f0ede4465a3b0324230af74701e82414194a9c2228e7563327523' ;; 		armv7) natsArch='arm7'; sha256='804ec4f600418d4afd6a9cb94b92c306ab75c589fc5180a5c2c99cc514c0899a' ;; 		x86_64) natsArch='amd64'; sha256='d4d2ef2952a9a841ce6594a4dbd07b8a45ceea32dadb321ddebc0c56598c2085' ;; 		x86) natsArch='386'; sha256='add5a328af2cab82230f881f71f7ca4dd907b477972d14a06b77b83188863d4d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 17 Nov 2022 20:49:36 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 17 Nov 2022 20:49:36 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 17 Nov 2022 20:49:36 GMT
EXPOSE 4222 6222 8222
# Thu, 17 Nov 2022 20:49:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Nov 2022 20:49:37 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9616ea8c1de4a90b1a50591336485e88ae5c2346e0d778bdbe69b00647bf8e39`  
		Last Modified: Sat, 12 Nov 2022 03:50:12 GMT  
		Size: 2.6 MB (2615105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d5728111a27515c16eb46117bf3339ccefc8af39e7c1508951d9286a3c3891c`  
		Last Modified: Thu, 17 Nov 2022 20:50:52 GMT  
		Size: 5.0 MB (4970331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d3e171e5c82f413b32d409f4fce9c56e3a429da91e068be34239e7c8c856576`  
		Last Modified: Thu, 17 Nov 2022 20:50:51 GMT  
		Size: 561.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:699b733f623013826c3dee6862aac2f7cb12bc97712d445dcf79191ba87875f6`  
		Last Modified: Thu, 17 Nov 2022 20:50:51 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-alpine3.16` - linux; arm variant v7

```console
$ docker pull nats@sha256:bf2175af45ce04af8a4d8a8c810eb98dbbdf0208010f248234803a56346e7492
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.4 MB (7380724 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af540a578654dbc22e31a00269e904f93dae199d3a57c7b588311595cd8c326c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Sat, 12 Nov 2022 03:57:24 GMT
ADD file:0b4a628f529226f5ec9d357ca63138bd2d22411a889c780ac8d395d761e07b2c in / 
# Sat, 12 Nov 2022 03:57:24 GMT
CMD ["/bin/sh"]
# Thu, 17 Nov 2022 20:57:48 GMT
ENV NATS_SERVER=2.9.7
# Thu, 17 Nov 2022 20:57:51 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='153018a675b0e896ffbed0cbc3fe5f733fd674d2f4bf554130ae8960a6c5277c' ;; 		armhf) natsArch='arm6'; sha256='9714af72c37f0ede4465a3b0324230af74701e82414194a9c2228e7563327523' ;; 		armv7) natsArch='arm7'; sha256='804ec4f600418d4afd6a9cb94b92c306ab75c589fc5180a5c2c99cc514c0899a' ;; 		x86_64) natsArch='amd64'; sha256='d4d2ef2952a9a841ce6594a4dbd07b8a45ceea32dadb321ddebc0c56598c2085' ;; 		x86) natsArch='386'; sha256='add5a328af2cab82230f881f71f7ca4dd907b477972d14a06b77b83188863d4d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 17 Nov 2022 20:57:51 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 17 Nov 2022 20:57:51 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 17 Nov 2022 20:57:52 GMT
EXPOSE 4222 6222 8222
# Thu, 17 Nov 2022 20:57:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Nov 2022 20:57:52 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:e44ba29d168a7f7c9e914f3724614df9e070aa6ef9b9ba5c9004db3c071f403a`  
		Last Modified: Sat, 12 Nov 2022 03:58:16 GMT  
		Size: 2.4 MB (2418788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c6aab4ebcc741288db0b5a719ef99f393d0fd90552b7131f9391a1f1bb37575`  
		Last Modified: Thu, 17 Nov 2022 20:59:09 GMT  
		Size: 5.0 MB (4960964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c4be9c1201790ef36f0543a1ad75a874f321b98fb2053e0b742e2f74e72338e`  
		Last Modified: Thu, 17 Nov 2022 20:59:08 GMT  
		Size: 560.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6f34e641f8406d256e755f8e058c5e957c85a985209c0e0021a18e1aab450c9`  
		Last Modified: Thu, 17 Nov 2022 20:59:08 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-alpine3.16` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:173181d8057b550ed4e321336b885f0ada263273ebc6cba24563f43578c00c23
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.5 MB (7503096 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:41f949bc183512a9594a4bcf404727a905c6e76f0ac0318a03cf0e2b93ccf1de`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Sat, 12 Nov 2022 03:39:38 GMT
ADD file:57d621536158358b14d15155826ef2dd4ca034278044111ec0aaf6717016e569 in / 
# Sat, 12 Nov 2022 03:39:38 GMT
CMD ["/bin/sh"]
# Thu, 17 Nov 2022 20:40:36 GMT
ENV NATS_SERVER=2.9.7
# Thu, 17 Nov 2022 20:40:39 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='153018a675b0e896ffbed0cbc3fe5f733fd674d2f4bf554130ae8960a6c5277c' ;; 		armhf) natsArch='arm6'; sha256='9714af72c37f0ede4465a3b0324230af74701e82414194a9c2228e7563327523' ;; 		armv7) natsArch='arm7'; sha256='804ec4f600418d4afd6a9cb94b92c306ab75c589fc5180a5c2c99cc514c0899a' ;; 		x86_64) natsArch='amd64'; sha256='d4d2ef2952a9a841ce6594a4dbd07b8a45ceea32dadb321ddebc0c56598c2085' ;; 		x86) natsArch='386'; sha256='add5a328af2cab82230f881f71f7ca4dd907b477972d14a06b77b83188863d4d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 17 Nov 2022 20:40:39 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 17 Nov 2022 20:40:39 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 17 Nov 2022 20:40:39 GMT
EXPOSE 4222 6222 8222
# Thu, 17 Nov 2022 20:40:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Nov 2022 20:40:40 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:6875df1f535433e5affe18ecfde9acb7950ab5f76887980ff06c5cdd48cf98f4`  
		Last Modified: Sat, 12 Nov 2022 03:40:05 GMT  
		Size: 2.7 MB (2707756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46474a86907df61c3b68bfcfc04ccf1b583ae765e82a80c581951fb9f5e8a104`  
		Last Modified: Thu, 17 Nov 2022 20:41:10 GMT  
		Size: 4.8 MB (4794340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98cf9fbe300cc2e491de01ad75e29bc228c5e706a5140594a1c29c565216b00e`  
		Last Modified: Thu, 17 Nov 2022 20:41:09 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9323da261341d5d9bbcca4222e4b1c77ff87a4bd0aae38eb7e003bc530717bd2`  
		Last Modified: Thu, 17 Nov 2022 20:41:09 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-linux`

```console
$ docker pull nats@sha256:26a7092afff4cfbdd0fc17bd33dbf3308383876690a72fd95b009500d840dce2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9-linux` - linux; amd64

```console
$ docker pull nats@sha256:6fc6aee58f7a448bb3bbd803f3addfa0c9512b5083376ce20781b9b635c381cf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4918825 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:974c838918842c11cbf59d7af83a073f753537c9d4b14f47231d3c1c7ba41c9e`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 17 Nov 2022 20:21:46 GMT
COPY file:88cbf98679a4e287b67a701a1fb77e0e0928e75cc0e1e669916e033ecf774fdc in /nats-server 
# Thu, 17 Nov 2022 20:21:46 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 17 Nov 2022 20:21:46 GMT
EXPOSE 4222 6222 8222
# Thu, 17 Nov 2022 20:21:46 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 17 Nov 2022 20:21:46 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 17 Nov 2022 20:21:47 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c8ce17c05ed27e7e08286a74c292d54eb2d5902af8f901dab4505ba83f7296f5`  
		Last Modified: Thu, 17 Nov 2022 20:22:33 GMT  
		Size: 4.9 MB (4918317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88c3d57c92f61ccff2db59e857c959bc11ca2ed1a6ca7f5494aa479c513196f7`  
		Last Modified: Thu, 17 Nov 2022 20:22:32 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:9e5158db138340db27aef59e820bafe7a09359e8910c2cef451b58348dd329ff
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4683160 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b5c60a8afd73cd47b032a2d66e4968bf12f1aed52fee0f708cf184ef6c09b960`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 17 Nov 2022 20:49:48 GMT
COPY file:75f2ce97960bd08a17d41dd00b0f977ff54641b0f3d5b35f613c50553a59e8e1 in /nats-server 
# Thu, 17 Nov 2022 20:49:48 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 17 Nov 2022 20:49:49 GMT
EXPOSE 4222 6222 8222
# Thu, 17 Nov 2022 20:49:49 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 17 Nov 2022 20:49:49 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 17 Nov 2022 20:49:49 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:e27c576ee7d0df355bb5ab346016b3a399e8048fe3f938263b3b77e343d9243f`  
		Last Modified: Thu, 17 Nov 2022 20:51:22 GMT  
		Size: 4.7 MB (4682651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:788fb9f41d9d2c69e1f5737db95b3d0e754d24cd75bdd8d94a80166b8c97d6b6`  
		Last Modified: Thu, 17 Nov 2022 20:51:21 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:e4c874e4f9f5eafa49bdd7fed9a022da8958f69cc70e245af8bb9ebf7cad0c0c
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4679780 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2bc64213c48245d6c2d479e5be4d5043a6d811cb9d273ae36c8dfa157accbd04`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 17 Nov 2022 20:58:06 GMT
COPY file:ebca823a5dac00609e9fb9733528840572067b84b58dcccbe67a2df698f2869e in /nats-server 
# Thu, 17 Nov 2022 20:58:06 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 17 Nov 2022 20:58:06 GMT
EXPOSE 4222 6222 8222
# Thu, 17 Nov 2022 20:58:06 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 17 Nov 2022 20:58:06 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 17 Nov 2022 20:58:06 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:2c415cfba68b644bd88b057d832ff5015af29e04439812f5bd2e6873b3d7b8fd`  
		Last Modified: Thu, 17 Nov 2022 20:59:39 GMT  
		Size: 4.7 MB (4679272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:875032eeefdff15b8e0c04ffba01805fa83a04cad983b8322b99f53b04e9c1fe`  
		Last Modified: Thu, 17 Nov 2022 20:59:38 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:6d5eefe444c9be5d4f08fd3ccf8277d186014689ef84ea0f59c59dc11acb4904
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4504058 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7ac0ab188af08ab1a9c049a3f6c349d0d2df9595cee8e6626c19a913526dcb2`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 17 Nov 2022 20:40:45 GMT
COPY file:d11c7b340550df0716193331cacb3d06f2cb3b9971e90e006a9c153aaadc50f8 in /nats-server 
# Thu, 17 Nov 2022 20:40:45 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 17 Nov 2022 20:40:45 GMT
EXPOSE 4222 6222 8222
# Thu, 17 Nov 2022 20:40:45 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 17 Nov 2022 20:40:45 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 17 Nov 2022 20:40:45 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:d3e01af3796e331721cc924f0d95499739cea560e1ac4bac35c11176033c94c8`  
		Last Modified: Thu, 17 Nov 2022 20:41:30 GMT  
		Size: 4.5 MB (4503550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e0b7a277e0d621acb2a17025b4318262de852c8be74070453c2f8c9983601ad`  
		Last Modified: Thu, 17 Nov 2022 20:41:30 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-nanoserver`

```console
$ docker pull nats@sha256:8f26c87d964b3426a16e546857fc7873a8acc6ee97786a9366744ae849a4825d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3650; amd64

### `nats:2.9-nanoserver` - windows version 10.0.17763.3650; amd64

```console
$ docker pull nats@sha256:b69aaf3d5200a1cb93e65a79acaa950d17ee0b0e88be899c4c3ecd6695cf9529
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.7 MB (111704287 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a82f827f381afa49f7b9d69a162222472931dd2aad1ebbac2b60a8155e798028`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 05 Nov 2022 18:06:28 GMT
RUN Apply image 10.0.17763.3650
# Wed, 09 Nov 2022 16:47:43 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Thu, 17 Nov 2022 20:19:19 GMT
RUN cmd /S /C #(nop) COPY file:d6b547504effc3514ee13384db156b8c7df287eadd44c86f4e5f5eabb6646c1d in C:\nats-server.exe 
# Thu, 17 Nov 2022 20:19:20 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Thu, 17 Nov 2022 20:19:21 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Thu, 17 Nov 2022 20:19:21 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 17 Nov 2022 20:19:22 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:35ab4104a4d9df6a0d1eac84cc8fbc13511ef6c8aef5ced04fdf63e7e20803a3`  
		Last Modified: Tue, 08 Nov 2022 19:45:20 GMT  
		Size: 106.7 MB (106723592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6708525607bc7a2985c6a423e6cb63d6175e3ad60d997873c4519fab371772fe`  
		Last Modified: Wed, 09 Nov 2022 16:48:43 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cb5d7747e73374a2c02473deb4bde157dddb2835cb5e66800cfba5842c1fd88`  
		Last Modified: Thu, 17 Nov 2022 20:20:12 GMT  
		Size: 5.0 MB (4974250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b3d427408549420b1666d1a85d3ff1bd3132f4e61dd9a7bd4e75a7c5adc32ee`  
		Last Modified: Thu, 17 Nov 2022 20:20:11 GMT  
		Size: 1.8 KB (1811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4682e51d5cc8bfadb600b57559df30d236b94223a5e9b1c3d2468f6acb1ee3f3`  
		Last Modified: Thu, 17 Nov 2022 20:20:11 GMT  
		Size: 1.2 KB (1161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8223b92ce81db067bb8ee9eacbf53e251b0dcd29dd1af6aa3a519768f0a7b44b`  
		Last Modified: Thu, 17 Nov 2022 20:20:11 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51f050378e256630049566bfcc0cf782533a8f961bcae8b6d9421ef19a8a780f`  
		Last Modified: Thu, 17 Nov 2022 20:20:11 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-nanoserver-1809`

```console
$ docker pull nats@sha256:8f26c87d964b3426a16e546857fc7873a8acc6ee97786a9366744ae849a4825d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3650; amd64

### `nats:2.9-nanoserver-1809` - windows version 10.0.17763.3650; amd64

```console
$ docker pull nats@sha256:b69aaf3d5200a1cb93e65a79acaa950d17ee0b0e88be899c4c3ecd6695cf9529
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.7 MB (111704287 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a82f827f381afa49f7b9d69a162222472931dd2aad1ebbac2b60a8155e798028`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 05 Nov 2022 18:06:28 GMT
RUN Apply image 10.0.17763.3650
# Wed, 09 Nov 2022 16:47:43 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Thu, 17 Nov 2022 20:19:19 GMT
RUN cmd /S /C #(nop) COPY file:d6b547504effc3514ee13384db156b8c7df287eadd44c86f4e5f5eabb6646c1d in C:\nats-server.exe 
# Thu, 17 Nov 2022 20:19:20 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Thu, 17 Nov 2022 20:19:21 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Thu, 17 Nov 2022 20:19:21 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 17 Nov 2022 20:19:22 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:35ab4104a4d9df6a0d1eac84cc8fbc13511ef6c8aef5ced04fdf63e7e20803a3`  
		Last Modified: Tue, 08 Nov 2022 19:45:20 GMT  
		Size: 106.7 MB (106723592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6708525607bc7a2985c6a423e6cb63d6175e3ad60d997873c4519fab371772fe`  
		Last Modified: Wed, 09 Nov 2022 16:48:43 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cb5d7747e73374a2c02473deb4bde157dddb2835cb5e66800cfba5842c1fd88`  
		Last Modified: Thu, 17 Nov 2022 20:20:12 GMT  
		Size: 5.0 MB (4974250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b3d427408549420b1666d1a85d3ff1bd3132f4e61dd9a7bd4e75a7c5adc32ee`  
		Last Modified: Thu, 17 Nov 2022 20:20:11 GMT  
		Size: 1.8 KB (1811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4682e51d5cc8bfadb600b57559df30d236b94223a5e9b1c3d2468f6acb1ee3f3`  
		Last Modified: Thu, 17 Nov 2022 20:20:11 GMT  
		Size: 1.2 KB (1161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8223b92ce81db067bb8ee9eacbf53e251b0dcd29dd1af6aa3a519768f0a7b44b`  
		Last Modified: Thu, 17 Nov 2022 20:20:11 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51f050378e256630049566bfcc0cf782533a8f961bcae8b6d9421ef19a8a780f`  
		Last Modified: Thu, 17 Nov 2022 20:20:11 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-scratch`

```console
$ docker pull nats@sha256:26a7092afff4cfbdd0fc17bd33dbf3308383876690a72fd95b009500d840dce2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9-scratch` - linux; amd64

```console
$ docker pull nats@sha256:6fc6aee58f7a448bb3bbd803f3addfa0c9512b5083376ce20781b9b635c381cf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4918825 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:974c838918842c11cbf59d7af83a073f753537c9d4b14f47231d3c1c7ba41c9e`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 17 Nov 2022 20:21:46 GMT
COPY file:88cbf98679a4e287b67a701a1fb77e0e0928e75cc0e1e669916e033ecf774fdc in /nats-server 
# Thu, 17 Nov 2022 20:21:46 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 17 Nov 2022 20:21:46 GMT
EXPOSE 4222 6222 8222
# Thu, 17 Nov 2022 20:21:46 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 17 Nov 2022 20:21:46 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 17 Nov 2022 20:21:47 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c8ce17c05ed27e7e08286a74c292d54eb2d5902af8f901dab4505ba83f7296f5`  
		Last Modified: Thu, 17 Nov 2022 20:22:33 GMT  
		Size: 4.9 MB (4918317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88c3d57c92f61ccff2db59e857c959bc11ca2ed1a6ca7f5494aa479c513196f7`  
		Last Modified: Thu, 17 Nov 2022 20:22:32 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:9e5158db138340db27aef59e820bafe7a09359e8910c2cef451b58348dd329ff
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4683160 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b5c60a8afd73cd47b032a2d66e4968bf12f1aed52fee0f708cf184ef6c09b960`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 17 Nov 2022 20:49:48 GMT
COPY file:75f2ce97960bd08a17d41dd00b0f977ff54641b0f3d5b35f613c50553a59e8e1 in /nats-server 
# Thu, 17 Nov 2022 20:49:48 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 17 Nov 2022 20:49:49 GMT
EXPOSE 4222 6222 8222
# Thu, 17 Nov 2022 20:49:49 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 17 Nov 2022 20:49:49 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 17 Nov 2022 20:49:49 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:e27c576ee7d0df355bb5ab346016b3a399e8048fe3f938263b3b77e343d9243f`  
		Last Modified: Thu, 17 Nov 2022 20:51:22 GMT  
		Size: 4.7 MB (4682651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:788fb9f41d9d2c69e1f5737db95b3d0e754d24cd75bdd8d94a80166b8c97d6b6`  
		Last Modified: Thu, 17 Nov 2022 20:51:21 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:e4c874e4f9f5eafa49bdd7fed9a022da8958f69cc70e245af8bb9ebf7cad0c0c
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4679780 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2bc64213c48245d6c2d479e5be4d5043a6d811cb9d273ae36c8dfa157accbd04`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 17 Nov 2022 20:58:06 GMT
COPY file:ebca823a5dac00609e9fb9733528840572067b84b58dcccbe67a2df698f2869e in /nats-server 
# Thu, 17 Nov 2022 20:58:06 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 17 Nov 2022 20:58:06 GMT
EXPOSE 4222 6222 8222
# Thu, 17 Nov 2022 20:58:06 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 17 Nov 2022 20:58:06 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 17 Nov 2022 20:58:06 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:2c415cfba68b644bd88b057d832ff5015af29e04439812f5bd2e6873b3d7b8fd`  
		Last Modified: Thu, 17 Nov 2022 20:59:39 GMT  
		Size: 4.7 MB (4679272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:875032eeefdff15b8e0c04ffba01805fa83a04cad983b8322b99f53b04e9c1fe`  
		Last Modified: Thu, 17 Nov 2022 20:59:38 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:6d5eefe444c9be5d4f08fd3ccf8277d186014689ef84ea0f59c59dc11acb4904
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4504058 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7ac0ab188af08ab1a9c049a3f6c349d0d2df9595cee8e6626c19a913526dcb2`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 17 Nov 2022 20:40:45 GMT
COPY file:d11c7b340550df0716193331cacb3d06f2cb3b9971e90e006a9c153aaadc50f8 in /nats-server 
# Thu, 17 Nov 2022 20:40:45 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 17 Nov 2022 20:40:45 GMT
EXPOSE 4222 6222 8222
# Thu, 17 Nov 2022 20:40:45 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 17 Nov 2022 20:40:45 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 17 Nov 2022 20:40:45 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:d3e01af3796e331721cc924f0d95499739cea560e1ac4bac35c11176033c94c8`  
		Last Modified: Thu, 17 Nov 2022 20:41:30 GMT  
		Size: 4.5 MB (4503550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e0b7a277e0d621acb2a17025b4318262de852c8be74070453c2f8c9983601ad`  
		Last Modified: Thu, 17 Nov 2022 20:41:30 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-windowsservercore`

```console
$ docker pull nats@sha256:a2a17b6c8e185249db8f657d5b4b5473e4627feb0a7ea39ac121544d7ab11465
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3650; amd64

### `nats:2.9-windowsservercore` - windows version 10.0.17763.3650; amd64

```console
$ docker pull nats@sha256:d42d0b0ee29bdd7b0ea24be91fb754a64a3da2ab070ed93e185e983132b9beec
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2784314848 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a836a477662568b8b4f2cd2ba8211273a6ae351f51fd48d29015400f42f395c`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 05 Nov 2022 18:29:26 GMT
RUN Install update 10.0.17763.3650
# Wed, 09 Nov 2022 14:50:58 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Nov 2022 16:44:45 GMT
ENV NATS_DOCKERIZED=1
# Thu, 17 Nov 2022 20:15:26 GMT
ENV NATS_SERVER=2.9.7
# Thu, 17 Nov 2022 20:15:27 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.9.7/nats-server-v2.9.7-windows-amd64.zip
# Thu, 17 Nov 2022 20:15:28 GMT
ENV NATS_SERVER_SHASUM=f1baa1646b7a499d035ebfd529644c1379988ab69703a090f9899c97067cea02
# Thu, 17 Nov 2022 20:17:00 GMT
RUN Set-PSDebug -Trace 2
# Thu, 17 Nov 2022 20:18:59 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Thu, 17 Nov 2022 20:19:00 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Thu, 17 Nov 2022 20:19:01 GMT
EXPOSE 4222 6222 8222
# Thu, 17 Nov 2022 20:19:02 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 17 Nov 2022 20:19:03 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a48a3e4ae2de839d8e99bde16eb91d113fb2cf889bba472d0c4274851b5fb402`  
		Last Modified: Tue, 21 Jun 2022 18:30:17 GMT  
		Size: 1.9 GB (1924269350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c26cc6e4f9eb1ae415a5ead6f884cac597bbd57efa6cd042c878d5b54c9d2091`  
		Last Modified: Tue, 08 Nov 2022 19:44:35 GMT  
		Size: 854.3 MB (854317461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99941fb33972e616b231a8aadd93463fdfd5de6aece4aa6c470d2feec31839be`  
		Last Modified: Wed, 09 Nov 2022 16:48:23 GMT  
		Size: 1.3 KB (1335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0f3d8a87f0a1540850986ff94131286dfa42ca116f04779e02f60b3a724641b`  
		Last Modified: Wed, 09 Nov 2022 16:48:23 GMT  
		Size: 1.3 KB (1327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69b8ead5903ee0014b1d59597e3e42c54eb9ad338e077477176b04d22ab4f291`  
		Last Modified: Thu, 17 Nov 2022 20:19:56 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd5112842b491d9aed12c373a680aa352fda7856f4dd7ae100240cda81004d10`  
		Last Modified: Thu, 17 Nov 2022 20:19:56 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27e8ac611281af798a4d5c0f0ffeca3542a44a865688ca95c3f963d0f3a2b009`  
		Last Modified: Thu, 17 Nov 2022 20:19:56 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ced45d282af98e490deb218ae7d77ad9ee20038016ea5fad600ab6363d4339fd`  
		Last Modified: Thu, 17 Nov 2022 20:19:56 GMT  
		Size: 381.6 KB (381592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d244e04b249f9171046dc315cd9c7d70aadbaa6496d85f41de583773d750a76b`  
		Last Modified: Thu, 17 Nov 2022 20:19:55 GMT  
		Size: 5.3 MB (5333250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e9dc3cf2f9c57dc6d24c7b6d3a526d97d4c7ef1de724d54dae9ad10211ba0e1`  
		Last Modified: Thu, 17 Nov 2022 20:19:54 GMT  
		Size: 2.0 KB (2001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6e0bb8f7d2e8165a51f2f77c4ee12feb907b21e4a5f2fe8c6215e6ee1c3b075`  
		Last Modified: Thu, 17 Nov 2022 20:19:54 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80326cc866c490bc13a4ead203b6b1af79320652c34f6605511671f003980078`  
		Last Modified: Thu, 17 Nov 2022 20:19:54 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7785e4126ef3eb2bac999118a556a59d9ab9474c8175a5742b4a1c7fba660efe`  
		Last Modified: Thu, 17 Nov 2022 20:19:54 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-windowsservercore-1809`

```console
$ docker pull nats@sha256:a2a17b6c8e185249db8f657d5b4b5473e4627feb0a7ea39ac121544d7ab11465
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3650; amd64

### `nats:2.9-windowsservercore-1809` - windows version 10.0.17763.3650; amd64

```console
$ docker pull nats@sha256:d42d0b0ee29bdd7b0ea24be91fb754a64a3da2ab070ed93e185e983132b9beec
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2784314848 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a836a477662568b8b4f2cd2ba8211273a6ae351f51fd48d29015400f42f395c`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 05 Nov 2022 18:29:26 GMT
RUN Install update 10.0.17763.3650
# Wed, 09 Nov 2022 14:50:58 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Nov 2022 16:44:45 GMT
ENV NATS_DOCKERIZED=1
# Thu, 17 Nov 2022 20:15:26 GMT
ENV NATS_SERVER=2.9.7
# Thu, 17 Nov 2022 20:15:27 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.9.7/nats-server-v2.9.7-windows-amd64.zip
# Thu, 17 Nov 2022 20:15:28 GMT
ENV NATS_SERVER_SHASUM=f1baa1646b7a499d035ebfd529644c1379988ab69703a090f9899c97067cea02
# Thu, 17 Nov 2022 20:17:00 GMT
RUN Set-PSDebug -Trace 2
# Thu, 17 Nov 2022 20:18:59 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Thu, 17 Nov 2022 20:19:00 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Thu, 17 Nov 2022 20:19:01 GMT
EXPOSE 4222 6222 8222
# Thu, 17 Nov 2022 20:19:02 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 17 Nov 2022 20:19:03 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a48a3e4ae2de839d8e99bde16eb91d113fb2cf889bba472d0c4274851b5fb402`  
		Last Modified: Tue, 21 Jun 2022 18:30:17 GMT  
		Size: 1.9 GB (1924269350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c26cc6e4f9eb1ae415a5ead6f884cac597bbd57efa6cd042c878d5b54c9d2091`  
		Last Modified: Tue, 08 Nov 2022 19:44:35 GMT  
		Size: 854.3 MB (854317461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99941fb33972e616b231a8aadd93463fdfd5de6aece4aa6c470d2feec31839be`  
		Last Modified: Wed, 09 Nov 2022 16:48:23 GMT  
		Size: 1.3 KB (1335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0f3d8a87f0a1540850986ff94131286dfa42ca116f04779e02f60b3a724641b`  
		Last Modified: Wed, 09 Nov 2022 16:48:23 GMT  
		Size: 1.3 KB (1327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69b8ead5903ee0014b1d59597e3e42c54eb9ad338e077477176b04d22ab4f291`  
		Last Modified: Thu, 17 Nov 2022 20:19:56 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd5112842b491d9aed12c373a680aa352fda7856f4dd7ae100240cda81004d10`  
		Last Modified: Thu, 17 Nov 2022 20:19:56 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27e8ac611281af798a4d5c0f0ffeca3542a44a865688ca95c3f963d0f3a2b009`  
		Last Modified: Thu, 17 Nov 2022 20:19:56 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ced45d282af98e490deb218ae7d77ad9ee20038016ea5fad600ab6363d4339fd`  
		Last Modified: Thu, 17 Nov 2022 20:19:56 GMT  
		Size: 381.6 KB (381592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d244e04b249f9171046dc315cd9c7d70aadbaa6496d85f41de583773d750a76b`  
		Last Modified: Thu, 17 Nov 2022 20:19:55 GMT  
		Size: 5.3 MB (5333250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e9dc3cf2f9c57dc6d24c7b6d3a526d97d4c7ef1de724d54dae9ad10211ba0e1`  
		Last Modified: Thu, 17 Nov 2022 20:19:54 GMT  
		Size: 2.0 KB (2001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6e0bb8f7d2e8165a51f2f77c4ee12feb907b21e4a5f2fe8c6215e6ee1c3b075`  
		Last Modified: Thu, 17 Nov 2022 20:19:54 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80326cc866c490bc13a4ead203b6b1af79320652c34f6605511671f003980078`  
		Last Modified: Thu, 17 Nov 2022 20:19:54 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7785e4126ef3eb2bac999118a556a59d9ab9474c8175a5742b4a1c7fba660efe`  
		Last Modified: Thu, 17 Nov 2022 20:19:54 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.7`

```console
$ docker pull nats@sha256:8a550ace09f524090c5399c7eab008c9f0d55a29eb1732cc4a565d4f1160346c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.3650; amd64

### `nats:2.9.7` - linux; amd64

```console
$ docker pull nats@sha256:6fc6aee58f7a448bb3bbd803f3addfa0c9512b5083376ce20781b9b635c381cf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4918825 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:974c838918842c11cbf59d7af83a073f753537c9d4b14f47231d3c1c7ba41c9e`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 17 Nov 2022 20:21:46 GMT
COPY file:88cbf98679a4e287b67a701a1fb77e0e0928e75cc0e1e669916e033ecf774fdc in /nats-server 
# Thu, 17 Nov 2022 20:21:46 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 17 Nov 2022 20:21:46 GMT
EXPOSE 4222 6222 8222
# Thu, 17 Nov 2022 20:21:46 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 17 Nov 2022 20:21:46 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 17 Nov 2022 20:21:47 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c8ce17c05ed27e7e08286a74c292d54eb2d5902af8f901dab4505ba83f7296f5`  
		Last Modified: Thu, 17 Nov 2022 20:22:33 GMT  
		Size: 4.9 MB (4918317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88c3d57c92f61ccff2db59e857c959bc11ca2ed1a6ca7f5494aa479c513196f7`  
		Last Modified: Thu, 17 Nov 2022 20:22:32 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.7` - linux; arm variant v6

```console
$ docker pull nats@sha256:9e5158db138340db27aef59e820bafe7a09359e8910c2cef451b58348dd329ff
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4683160 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b5c60a8afd73cd47b032a2d66e4968bf12f1aed52fee0f708cf184ef6c09b960`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 17 Nov 2022 20:49:48 GMT
COPY file:75f2ce97960bd08a17d41dd00b0f977ff54641b0f3d5b35f613c50553a59e8e1 in /nats-server 
# Thu, 17 Nov 2022 20:49:48 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 17 Nov 2022 20:49:49 GMT
EXPOSE 4222 6222 8222
# Thu, 17 Nov 2022 20:49:49 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 17 Nov 2022 20:49:49 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 17 Nov 2022 20:49:49 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:e27c576ee7d0df355bb5ab346016b3a399e8048fe3f938263b3b77e343d9243f`  
		Last Modified: Thu, 17 Nov 2022 20:51:22 GMT  
		Size: 4.7 MB (4682651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:788fb9f41d9d2c69e1f5737db95b3d0e754d24cd75bdd8d94a80166b8c97d6b6`  
		Last Modified: Thu, 17 Nov 2022 20:51:21 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.7` - linux; arm variant v7

```console
$ docker pull nats@sha256:e4c874e4f9f5eafa49bdd7fed9a022da8958f69cc70e245af8bb9ebf7cad0c0c
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4679780 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2bc64213c48245d6c2d479e5be4d5043a6d811cb9d273ae36c8dfa157accbd04`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 17 Nov 2022 20:58:06 GMT
COPY file:ebca823a5dac00609e9fb9733528840572067b84b58dcccbe67a2df698f2869e in /nats-server 
# Thu, 17 Nov 2022 20:58:06 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 17 Nov 2022 20:58:06 GMT
EXPOSE 4222 6222 8222
# Thu, 17 Nov 2022 20:58:06 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 17 Nov 2022 20:58:06 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 17 Nov 2022 20:58:06 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:2c415cfba68b644bd88b057d832ff5015af29e04439812f5bd2e6873b3d7b8fd`  
		Last Modified: Thu, 17 Nov 2022 20:59:39 GMT  
		Size: 4.7 MB (4679272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:875032eeefdff15b8e0c04ffba01805fa83a04cad983b8322b99f53b04e9c1fe`  
		Last Modified: Thu, 17 Nov 2022 20:59:38 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.7` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:6d5eefe444c9be5d4f08fd3ccf8277d186014689ef84ea0f59c59dc11acb4904
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4504058 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7ac0ab188af08ab1a9c049a3f6c349d0d2df9595cee8e6626c19a913526dcb2`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 17 Nov 2022 20:40:45 GMT
COPY file:d11c7b340550df0716193331cacb3d06f2cb3b9971e90e006a9c153aaadc50f8 in /nats-server 
# Thu, 17 Nov 2022 20:40:45 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 17 Nov 2022 20:40:45 GMT
EXPOSE 4222 6222 8222
# Thu, 17 Nov 2022 20:40:45 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 17 Nov 2022 20:40:45 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 17 Nov 2022 20:40:45 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:d3e01af3796e331721cc924f0d95499739cea560e1ac4bac35c11176033c94c8`  
		Last Modified: Thu, 17 Nov 2022 20:41:30 GMT  
		Size: 4.5 MB (4503550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e0b7a277e0d621acb2a17025b4318262de852c8be74070453c2f8c9983601ad`  
		Last Modified: Thu, 17 Nov 2022 20:41:30 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.7` - windows version 10.0.17763.3650; amd64

```console
$ docker pull nats@sha256:b69aaf3d5200a1cb93e65a79acaa950d17ee0b0e88be899c4c3ecd6695cf9529
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.7 MB (111704287 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a82f827f381afa49f7b9d69a162222472931dd2aad1ebbac2b60a8155e798028`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 05 Nov 2022 18:06:28 GMT
RUN Apply image 10.0.17763.3650
# Wed, 09 Nov 2022 16:47:43 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Thu, 17 Nov 2022 20:19:19 GMT
RUN cmd /S /C #(nop) COPY file:d6b547504effc3514ee13384db156b8c7df287eadd44c86f4e5f5eabb6646c1d in C:\nats-server.exe 
# Thu, 17 Nov 2022 20:19:20 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Thu, 17 Nov 2022 20:19:21 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Thu, 17 Nov 2022 20:19:21 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 17 Nov 2022 20:19:22 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:35ab4104a4d9df6a0d1eac84cc8fbc13511ef6c8aef5ced04fdf63e7e20803a3`  
		Last Modified: Tue, 08 Nov 2022 19:45:20 GMT  
		Size: 106.7 MB (106723592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6708525607bc7a2985c6a423e6cb63d6175e3ad60d997873c4519fab371772fe`  
		Last Modified: Wed, 09 Nov 2022 16:48:43 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cb5d7747e73374a2c02473deb4bde157dddb2835cb5e66800cfba5842c1fd88`  
		Last Modified: Thu, 17 Nov 2022 20:20:12 GMT  
		Size: 5.0 MB (4974250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b3d427408549420b1666d1a85d3ff1bd3132f4e61dd9a7bd4e75a7c5adc32ee`  
		Last Modified: Thu, 17 Nov 2022 20:20:11 GMT  
		Size: 1.8 KB (1811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4682e51d5cc8bfadb600b57559df30d236b94223a5e9b1c3d2468f6acb1ee3f3`  
		Last Modified: Thu, 17 Nov 2022 20:20:11 GMT  
		Size: 1.2 KB (1161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8223b92ce81db067bb8ee9eacbf53e251b0dcd29dd1af6aa3a519768f0a7b44b`  
		Last Modified: Thu, 17 Nov 2022 20:20:11 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51f050378e256630049566bfcc0cf782533a8f961bcae8b6d9421ef19a8a780f`  
		Last Modified: Thu, 17 Nov 2022 20:20:11 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.7-alpine`

```console
$ docker pull nats@sha256:400adfffe0df7f2df0e76d34d6e25a0fb8eb68cfdc10d404afbbb31f818d0276
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9.7-alpine` - linux; amd64

```console
$ docker pull nats@sha256:d4698031a0afeb1ed37b240a9632b22a2d0fcea5fd48af3c8b28e1eba3348033
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.0 MB (8014859 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c26ee116aa283ae59469d995e49cce15bb982559c777e32f06933e315898c54`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Sat, 12 Nov 2022 04:19:23 GMT
ADD file:ceeb6e8632fafc657116cbf3afbd522185a16963230b57881073dad22eb0e1a3 in / 
# Sat, 12 Nov 2022 04:19:23 GMT
CMD ["/bin/sh"]
# Thu, 17 Nov 2022 20:21:36 GMT
ENV NATS_SERVER=2.9.7
# Thu, 17 Nov 2022 20:21:38 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='153018a675b0e896ffbed0cbc3fe5f733fd674d2f4bf554130ae8960a6c5277c' ;; 		armhf) natsArch='arm6'; sha256='9714af72c37f0ede4465a3b0324230af74701e82414194a9c2228e7563327523' ;; 		armv7) natsArch='arm7'; sha256='804ec4f600418d4afd6a9cb94b92c306ab75c589fc5180a5c2c99cc514c0899a' ;; 		x86_64) natsArch='amd64'; sha256='d4d2ef2952a9a841ce6594a4dbd07b8a45ceea32dadb321ddebc0c56598c2085' ;; 		x86) natsArch='386'; sha256='add5a328af2cab82230f881f71f7ca4dd907b477972d14a06b77b83188863d4d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 17 Nov 2022 20:21:38 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 17 Nov 2022 20:21:38 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 17 Nov 2022 20:21:39 GMT
EXPOSE 4222 6222 8222
# Thu, 17 Nov 2022 20:21:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Nov 2022 20:21:39 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:ca7dd9ec2225f2385955c43b2379305acd51543c28cf1d4e94522b3d94cce3ce`  
		Last Modified: Sat, 12 Nov 2022 02:52:15 GMT  
		Size: 2.8 MB (2806272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94acb566bf3ae8a5a3c0747075e8b16df167a9694bfb5ac6ccdea4e5558e2a01`  
		Last Modified: Thu, 17 Nov 2022 20:22:12 GMT  
		Size: 5.2 MB (5207590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e759e667a2c2d6d67aaf3491e124f07a1afc8de774d7973958b32b81ff7a0304`  
		Last Modified: Thu, 17 Nov 2022 20:22:11 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c0e8173963a2be8b30df5827fcfc01a70e5c95ab186696e43d9f624884cee41`  
		Last Modified: Thu, 17 Nov 2022 20:22:11 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.7-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:221c14c269fed109042c154935b6cd22b270dda8b66b30e48f734f5fb50ffb87
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7586411 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b8f37497160e12532b20e7eaca7e50daa1304f46b7002848dfae699b06743ba`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Sat, 12 Nov 2022 03:49:18 GMT
ADD file:493290ed8856fa13463defe63da0d30ab3de5dde042c87ef7c0701d66ebb8892 in / 
# Sat, 12 Nov 2022 03:49:18 GMT
CMD ["/bin/sh"]
# Thu, 17 Nov 2022 20:49:34 GMT
ENV NATS_SERVER=2.9.7
# Thu, 17 Nov 2022 20:49:36 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='153018a675b0e896ffbed0cbc3fe5f733fd674d2f4bf554130ae8960a6c5277c' ;; 		armhf) natsArch='arm6'; sha256='9714af72c37f0ede4465a3b0324230af74701e82414194a9c2228e7563327523' ;; 		armv7) natsArch='arm7'; sha256='804ec4f600418d4afd6a9cb94b92c306ab75c589fc5180a5c2c99cc514c0899a' ;; 		x86_64) natsArch='amd64'; sha256='d4d2ef2952a9a841ce6594a4dbd07b8a45ceea32dadb321ddebc0c56598c2085' ;; 		x86) natsArch='386'; sha256='add5a328af2cab82230f881f71f7ca4dd907b477972d14a06b77b83188863d4d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 17 Nov 2022 20:49:36 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 17 Nov 2022 20:49:36 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 17 Nov 2022 20:49:36 GMT
EXPOSE 4222 6222 8222
# Thu, 17 Nov 2022 20:49:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Nov 2022 20:49:37 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9616ea8c1de4a90b1a50591336485e88ae5c2346e0d778bdbe69b00647bf8e39`  
		Last Modified: Sat, 12 Nov 2022 03:50:12 GMT  
		Size: 2.6 MB (2615105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d5728111a27515c16eb46117bf3339ccefc8af39e7c1508951d9286a3c3891c`  
		Last Modified: Thu, 17 Nov 2022 20:50:52 GMT  
		Size: 5.0 MB (4970331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d3e171e5c82f413b32d409f4fce9c56e3a429da91e068be34239e7c8c856576`  
		Last Modified: Thu, 17 Nov 2022 20:50:51 GMT  
		Size: 561.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:699b733f623013826c3dee6862aac2f7cb12bc97712d445dcf79191ba87875f6`  
		Last Modified: Thu, 17 Nov 2022 20:50:51 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.7-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:bf2175af45ce04af8a4d8a8c810eb98dbbdf0208010f248234803a56346e7492
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.4 MB (7380724 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af540a578654dbc22e31a00269e904f93dae199d3a57c7b588311595cd8c326c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Sat, 12 Nov 2022 03:57:24 GMT
ADD file:0b4a628f529226f5ec9d357ca63138bd2d22411a889c780ac8d395d761e07b2c in / 
# Sat, 12 Nov 2022 03:57:24 GMT
CMD ["/bin/sh"]
# Thu, 17 Nov 2022 20:57:48 GMT
ENV NATS_SERVER=2.9.7
# Thu, 17 Nov 2022 20:57:51 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='153018a675b0e896ffbed0cbc3fe5f733fd674d2f4bf554130ae8960a6c5277c' ;; 		armhf) natsArch='arm6'; sha256='9714af72c37f0ede4465a3b0324230af74701e82414194a9c2228e7563327523' ;; 		armv7) natsArch='arm7'; sha256='804ec4f600418d4afd6a9cb94b92c306ab75c589fc5180a5c2c99cc514c0899a' ;; 		x86_64) natsArch='amd64'; sha256='d4d2ef2952a9a841ce6594a4dbd07b8a45ceea32dadb321ddebc0c56598c2085' ;; 		x86) natsArch='386'; sha256='add5a328af2cab82230f881f71f7ca4dd907b477972d14a06b77b83188863d4d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 17 Nov 2022 20:57:51 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 17 Nov 2022 20:57:51 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 17 Nov 2022 20:57:52 GMT
EXPOSE 4222 6222 8222
# Thu, 17 Nov 2022 20:57:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Nov 2022 20:57:52 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:e44ba29d168a7f7c9e914f3724614df9e070aa6ef9b9ba5c9004db3c071f403a`  
		Last Modified: Sat, 12 Nov 2022 03:58:16 GMT  
		Size: 2.4 MB (2418788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c6aab4ebcc741288db0b5a719ef99f393d0fd90552b7131f9391a1f1bb37575`  
		Last Modified: Thu, 17 Nov 2022 20:59:09 GMT  
		Size: 5.0 MB (4960964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c4be9c1201790ef36f0543a1ad75a874f321b98fb2053e0b742e2f74e72338e`  
		Last Modified: Thu, 17 Nov 2022 20:59:08 GMT  
		Size: 560.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6f34e641f8406d256e755f8e058c5e957c85a985209c0e0021a18e1aab450c9`  
		Last Modified: Thu, 17 Nov 2022 20:59:08 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.7-alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:173181d8057b550ed4e321336b885f0ada263273ebc6cba24563f43578c00c23
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.5 MB (7503096 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:41f949bc183512a9594a4bcf404727a905c6e76f0ac0318a03cf0e2b93ccf1de`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Sat, 12 Nov 2022 03:39:38 GMT
ADD file:57d621536158358b14d15155826ef2dd4ca034278044111ec0aaf6717016e569 in / 
# Sat, 12 Nov 2022 03:39:38 GMT
CMD ["/bin/sh"]
# Thu, 17 Nov 2022 20:40:36 GMT
ENV NATS_SERVER=2.9.7
# Thu, 17 Nov 2022 20:40:39 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='153018a675b0e896ffbed0cbc3fe5f733fd674d2f4bf554130ae8960a6c5277c' ;; 		armhf) natsArch='arm6'; sha256='9714af72c37f0ede4465a3b0324230af74701e82414194a9c2228e7563327523' ;; 		armv7) natsArch='arm7'; sha256='804ec4f600418d4afd6a9cb94b92c306ab75c589fc5180a5c2c99cc514c0899a' ;; 		x86_64) natsArch='amd64'; sha256='d4d2ef2952a9a841ce6594a4dbd07b8a45ceea32dadb321ddebc0c56598c2085' ;; 		x86) natsArch='386'; sha256='add5a328af2cab82230f881f71f7ca4dd907b477972d14a06b77b83188863d4d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 17 Nov 2022 20:40:39 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 17 Nov 2022 20:40:39 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 17 Nov 2022 20:40:39 GMT
EXPOSE 4222 6222 8222
# Thu, 17 Nov 2022 20:40:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Nov 2022 20:40:40 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:6875df1f535433e5affe18ecfde9acb7950ab5f76887980ff06c5cdd48cf98f4`  
		Last Modified: Sat, 12 Nov 2022 03:40:05 GMT  
		Size: 2.7 MB (2707756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46474a86907df61c3b68bfcfc04ccf1b583ae765e82a80c581951fb9f5e8a104`  
		Last Modified: Thu, 17 Nov 2022 20:41:10 GMT  
		Size: 4.8 MB (4794340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98cf9fbe300cc2e491de01ad75e29bc228c5e706a5140594a1c29c565216b00e`  
		Last Modified: Thu, 17 Nov 2022 20:41:09 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9323da261341d5d9bbcca4222e4b1c77ff87a4bd0aae38eb7e003bc530717bd2`  
		Last Modified: Thu, 17 Nov 2022 20:41:09 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.7-alpine3.16`

```console
$ docker pull nats@sha256:400adfffe0df7f2df0e76d34d6e25a0fb8eb68cfdc10d404afbbb31f818d0276
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9.7-alpine3.16` - linux; amd64

```console
$ docker pull nats@sha256:d4698031a0afeb1ed37b240a9632b22a2d0fcea5fd48af3c8b28e1eba3348033
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.0 MB (8014859 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c26ee116aa283ae59469d995e49cce15bb982559c777e32f06933e315898c54`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Sat, 12 Nov 2022 04:19:23 GMT
ADD file:ceeb6e8632fafc657116cbf3afbd522185a16963230b57881073dad22eb0e1a3 in / 
# Sat, 12 Nov 2022 04:19:23 GMT
CMD ["/bin/sh"]
# Thu, 17 Nov 2022 20:21:36 GMT
ENV NATS_SERVER=2.9.7
# Thu, 17 Nov 2022 20:21:38 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='153018a675b0e896ffbed0cbc3fe5f733fd674d2f4bf554130ae8960a6c5277c' ;; 		armhf) natsArch='arm6'; sha256='9714af72c37f0ede4465a3b0324230af74701e82414194a9c2228e7563327523' ;; 		armv7) natsArch='arm7'; sha256='804ec4f600418d4afd6a9cb94b92c306ab75c589fc5180a5c2c99cc514c0899a' ;; 		x86_64) natsArch='amd64'; sha256='d4d2ef2952a9a841ce6594a4dbd07b8a45ceea32dadb321ddebc0c56598c2085' ;; 		x86) natsArch='386'; sha256='add5a328af2cab82230f881f71f7ca4dd907b477972d14a06b77b83188863d4d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 17 Nov 2022 20:21:38 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 17 Nov 2022 20:21:38 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 17 Nov 2022 20:21:39 GMT
EXPOSE 4222 6222 8222
# Thu, 17 Nov 2022 20:21:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Nov 2022 20:21:39 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:ca7dd9ec2225f2385955c43b2379305acd51543c28cf1d4e94522b3d94cce3ce`  
		Last Modified: Sat, 12 Nov 2022 02:52:15 GMT  
		Size: 2.8 MB (2806272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94acb566bf3ae8a5a3c0747075e8b16df167a9694bfb5ac6ccdea4e5558e2a01`  
		Last Modified: Thu, 17 Nov 2022 20:22:12 GMT  
		Size: 5.2 MB (5207590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e759e667a2c2d6d67aaf3491e124f07a1afc8de774d7973958b32b81ff7a0304`  
		Last Modified: Thu, 17 Nov 2022 20:22:11 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c0e8173963a2be8b30df5827fcfc01a70e5c95ab186696e43d9f624884cee41`  
		Last Modified: Thu, 17 Nov 2022 20:22:11 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.7-alpine3.16` - linux; arm variant v6

```console
$ docker pull nats@sha256:221c14c269fed109042c154935b6cd22b270dda8b66b30e48f734f5fb50ffb87
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7586411 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b8f37497160e12532b20e7eaca7e50daa1304f46b7002848dfae699b06743ba`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Sat, 12 Nov 2022 03:49:18 GMT
ADD file:493290ed8856fa13463defe63da0d30ab3de5dde042c87ef7c0701d66ebb8892 in / 
# Sat, 12 Nov 2022 03:49:18 GMT
CMD ["/bin/sh"]
# Thu, 17 Nov 2022 20:49:34 GMT
ENV NATS_SERVER=2.9.7
# Thu, 17 Nov 2022 20:49:36 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='153018a675b0e896ffbed0cbc3fe5f733fd674d2f4bf554130ae8960a6c5277c' ;; 		armhf) natsArch='arm6'; sha256='9714af72c37f0ede4465a3b0324230af74701e82414194a9c2228e7563327523' ;; 		armv7) natsArch='arm7'; sha256='804ec4f600418d4afd6a9cb94b92c306ab75c589fc5180a5c2c99cc514c0899a' ;; 		x86_64) natsArch='amd64'; sha256='d4d2ef2952a9a841ce6594a4dbd07b8a45ceea32dadb321ddebc0c56598c2085' ;; 		x86) natsArch='386'; sha256='add5a328af2cab82230f881f71f7ca4dd907b477972d14a06b77b83188863d4d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 17 Nov 2022 20:49:36 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 17 Nov 2022 20:49:36 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 17 Nov 2022 20:49:36 GMT
EXPOSE 4222 6222 8222
# Thu, 17 Nov 2022 20:49:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Nov 2022 20:49:37 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9616ea8c1de4a90b1a50591336485e88ae5c2346e0d778bdbe69b00647bf8e39`  
		Last Modified: Sat, 12 Nov 2022 03:50:12 GMT  
		Size: 2.6 MB (2615105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d5728111a27515c16eb46117bf3339ccefc8af39e7c1508951d9286a3c3891c`  
		Last Modified: Thu, 17 Nov 2022 20:50:52 GMT  
		Size: 5.0 MB (4970331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d3e171e5c82f413b32d409f4fce9c56e3a429da91e068be34239e7c8c856576`  
		Last Modified: Thu, 17 Nov 2022 20:50:51 GMT  
		Size: 561.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:699b733f623013826c3dee6862aac2f7cb12bc97712d445dcf79191ba87875f6`  
		Last Modified: Thu, 17 Nov 2022 20:50:51 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.7-alpine3.16` - linux; arm variant v7

```console
$ docker pull nats@sha256:bf2175af45ce04af8a4d8a8c810eb98dbbdf0208010f248234803a56346e7492
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.4 MB (7380724 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af540a578654dbc22e31a00269e904f93dae199d3a57c7b588311595cd8c326c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Sat, 12 Nov 2022 03:57:24 GMT
ADD file:0b4a628f529226f5ec9d357ca63138bd2d22411a889c780ac8d395d761e07b2c in / 
# Sat, 12 Nov 2022 03:57:24 GMT
CMD ["/bin/sh"]
# Thu, 17 Nov 2022 20:57:48 GMT
ENV NATS_SERVER=2.9.7
# Thu, 17 Nov 2022 20:57:51 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='153018a675b0e896ffbed0cbc3fe5f733fd674d2f4bf554130ae8960a6c5277c' ;; 		armhf) natsArch='arm6'; sha256='9714af72c37f0ede4465a3b0324230af74701e82414194a9c2228e7563327523' ;; 		armv7) natsArch='arm7'; sha256='804ec4f600418d4afd6a9cb94b92c306ab75c589fc5180a5c2c99cc514c0899a' ;; 		x86_64) natsArch='amd64'; sha256='d4d2ef2952a9a841ce6594a4dbd07b8a45ceea32dadb321ddebc0c56598c2085' ;; 		x86) natsArch='386'; sha256='add5a328af2cab82230f881f71f7ca4dd907b477972d14a06b77b83188863d4d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 17 Nov 2022 20:57:51 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 17 Nov 2022 20:57:51 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 17 Nov 2022 20:57:52 GMT
EXPOSE 4222 6222 8222
# Thu, 17 Nov 2022 20:57:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Nov 2022 20:57:52 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:e44ba29d168a7f7c9e914f3724614df9e070aa6ef9b9ba5c9004db3c071f403a`  
		Last Modified: Sat, 12 Nov 2022 03:58:16 GMT  
		Size: 2.4 MB (2418788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c6aab4ebcc741288db0b5a719ef99f393d0fd90552b7131f9391a1f1bb37575`  
		Last Modified: Thu, 17 Nov 2022 20:59:09 GMT  
		Size: 5.0 MB (4960964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c4be9c1201790ef36f0543a1ad75a874f321b98fb2053e0b742e2f74e72338e`  
		Last Modified: Thu, 17 Nov 2022 20:59:08 GMT  
		Size: 560.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6f34e641f8406d256e755f8e058c5e957c85a985209c0e0021a18e1aab450c9`  
		Last Modified: Thu, 17 Nov 2022 20:59:08 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.7-alpine3.16` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:173181d8057b550ed4e321336b885f0ada263273ebc6cba24563f43578c00c23
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.5 MB (7503096 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:41f949bc183512a9594a4bcf404727a905c6e76f0ac0318a03cf0e2b93ccf1de`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Sat, 12 Nov 2022 03:39:38 GMT
ADD file:57d621536158358b14d15155826ef2dd4ca034278044111ec0aaf6717016e569 in / 
# Sat, 12 Nov 2022 03:39:38 GMT
CMD ["/bin/sh"]
# Thu, 17 Nov 2022 20:40:36 GMT
ENV NATS_SERVER=2.9.7
# Thu, 17 Nov 2022 20:40:39 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='153018a675b0e896ffbed0cbc3fe5f733fd674d2f4bf554130ae8960a6c5277c' ;; 		armhf) natsArch='arm6'; sha256='9714af72c37f0ede4465a3b0324230af74701e82414194a9c2228e7563327523' ;; 		armv7) natsArch='arm7'; sha256='804ec4f600418d4afd6a9cb94b92c306ab75c589fc5180a5c2c99cc514c0899a' ;; 		x86_64) natsArch='amd64'; sha256='d4d2ef2952a9a841ce6594a4dbd07b8a45ceea32dadb321ddebc0c56598c2085' ;; 		x86) natsArch='386'; sha256='add5a328af2cab82230f881f71f7ca4dd907b477972d14a06b77b83188863d4d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 17 Nov 2022 20:40:39 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 17 Nov 2022 20:40:39 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 17 Nov 2022 20:40:39 GMT
EXPOSE 4222 6222 8222
# Thu, 17 Nov 2022 20:40:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Nov 2022 20:40:40 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:6875df1f535433e5affe18ecfde9acb7950ab5f76887980ff06c5cdd48cf98f4`  
		Last Modified: Sat, 12 Nov 2022 03:40:05 GMT  
		Size: 2.7 MB (2707756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46474a86907df61c3b68bfcfc04ccf1b583ae765e82a80c581951fb9f5e8a104`  
		Last Modified: Thu, 17 Nov 2022 20:41:10 GMT  
		Size: 4.8 MB (4794340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98cf9fbe300cc2e491de01ad75e29bc228c5e706a5140594a1c29c565216b00e`  
		Last Modified: Thu, 17 Nov 2022 20:41:09 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9323da261341d5d9bbcca4222e4b1c77ff87a4bd0aae38eb7e003bc530717bd2`  
		Last Modified: Thu, 17 Nov 2022 20:41:09 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.7-linux`

```console
$ docker pull nats@sha256:26a7092afff4cfbdd0fc17bd33dbf3308383876690a72fd95b009500d840dce2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9.7-linux` - linux; amd64

```console
$ docker pull nats@sha256:6fc6aee58f7a448bb3bbd803f3addfa0c9512b5083376ce20781b9b635c381cf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4918825 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:974c838918842c11cbf59d7af83a073f753537c9d4b14f47231d3c1c7ba41c9e`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 17 Nov 2022 20:21:46 GMT
COPY file:88cbf98679a4e287b67a701a1fb77e0e0928e75cc0e1e669916e033ecf774fdc in /nats-server 
# Thu, 17 Nov 2022 20:21:46 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 17 Nov 2022 20:21:46 GMT
EXPOSE 4222 6222 8222
# Thu, 17 Nov 2022 20:21:46 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 17 Nov 2022 20:21:46 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 17 Nov 2022 20:21:47 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c8ce17c05ed27e7e08286a74c292d54eb2d5902af8f901dab4505ba83f7296f5`  
		Last Modified: Thu, 17 Nov 2022 20:22:33 GMT  
		Size: 4.9 MB (4918317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88c3d57c92f61ccff2db59e857c959bc11ca2ed1a6ca7f5494aa479c513196f7`  
		Last Modified: Thu, 17 Nov 2022 20:22:32 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.7-linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:9e5158db138340db27aef59e820bafe7a09359e8910c2cef451b58348dd329ff
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4683160 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b5c60a8afd73cd47b032a2d66e4968bf12f1aed52fee0f708cf184ef6c09b960`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 17 Nov 2022 20:49:48 GMT
COPY file:75f2ce97960bd08a17d41dd00b0f977ff54641b0f3d5b35f613c50553a59e8e1 in /nats-server 
# Thu, 17 Nov 2022 20:49:48 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 17 Nov 2022 20:49:49 GMT
EXPOSE 4222 6222 8222
# Thu, 17 Nov 2022 20:49:49 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 17 Nov 2022 20:49:49 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 17 Nov 2022 20:49:49 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:e27c576ee7d0df355bb5ab346016b3a399e8048fe3f938263b3b77e343d9243f`  
		Last Modified: Thu, 17 Nov 2022 20:51:22 GMT  
		Size: 4.7 MB (4682651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:788fb9f41d9d2c69e1f5737db95b3d0e754d24cd75bdd8d94a80166b8c97d6b6`  
		Last Modified: Thu, 17 Nov 2022 20:51:21 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.7-linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:e4c874e4f9f5eafa49bdd7fed9a022da8958f69cc70e245af8bb9ebf7cad0c0c
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4679780 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2bc64213c48245d6c2d479e5be4d5043a6d811cb9d273ae36c8dfa157accbd04`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 17 Nov 2022 20:58:06 GMT
COPY file:ebca823a5dac00609e9fb9733528840572067b84b58dcccbe67a2df698f2869e in /nats-server 
# Thu, 17 Nov 2022 20:58:06 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 17 Nov 2022 20:58:06 GMT
EXPOSE 4222 6222 8222
# Thu, 17 Nov 2022 20:58:06 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 17 Nov 2022 20:58:06 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 17 Nov 2022 20:58:06 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:2c415cfba68b644bd88b057d832ff5015af29e04439812f5bd2e6873b3d7b8fd`  
		Last Modified: Thu, 17 Nov 2022 20:59:39 GMT  
		Size: 4.7 MB (4679272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:875032eeefdff15b8e0c04ffba01805fa83a04cad983b8322b99f53b04e9c1fe`  
		Last Modified: Thu, 17 Nov 2022 20:59:38 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.7-linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:6d5eefe444c9be5d4f08fd3ccf8277d186014689ef84ea0f59c59dc11acb4904
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4504058 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7ac0ab188af08ab1a9c049a3f6c349d0d2df9595cee8e6626c19a913526dcb2`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 17 Nov 2022 20:40:45 GMT
COPY file:d11c7b340550df0716193331cacb3d06f2cb3b9971e90e006a9c153aaadc50f8 in /nats-server 
# Thu, 17 Nov 2022 20:40:45 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 17 Nov 2022 20:40:45 GMT
EXPOSE 4222 6222 8222
# Thu, 17 Nov 2022 20:40:45 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 17 Nov 2022 20:40:45 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 17 Nov 2022 20:40:45 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:d3e01af3796e331721cc924f0d95499739cea560e1ac4bac35c11176033c94c8`  
		Last Modified: Thu, 17 Nov 2022 20:41:30 GMT  
		Size: 4.5 MB (4503550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e0b7a277e0d621acb2a17025b4318262de852c8be74070453c2f8c9983601ad`  
		Last Modified: Thu, 17 Nov 2022 20:41:30 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.7-nanoserver`

```console
$ docker pull nats@sha256:8f26c87d964b3426a16e546857fc7873a8acc6ee97786a9366744ae849a4825d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3650; amd64

### `nats:2.9.7-nanoserver` - windows version 10.0.17763.3650; amd64

```console
$ docker pull nats@sha256:b69aaf3d5200a1cb93e65a79acaa950d17ee0b0e88be899c4c3ecd6695cf9529
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.7 MB (111704287 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a82f827f381afa49f7b9d69a162222472931dd2aad1ebbac2b60a8155e798028`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 05 Nov 2022 18:06:28 GMT
RUN Apply image 10.0.17763.3650
# Wed, 09 Nov 2022 16:47:43 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Thu, 17 Nov 2022 20:19:19 GMT
RUN cmd /S /C #(nop) COPY file:d6b547504effc3514ee13384db156b8c7df287eadd44c86f4e5f5eabb6646c1d in C:\nats-server.exe 
# Thu, 17 Nov 2022 20:19:20 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Thu, 17 Nov 2022 20:19:21 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Thu, 17 Nov 2022 20:19:21 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 17 Nov 2022 20:19:22 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:35ab4104a4d9df6a0d1eac84cc8fbc13511ef6c8aef5ced04fdf63e7e20803a3`  
		Last Modified: Tue, 08 Nov 2022 19:45:20 GMT  
		Size: 106.7 MB (106723592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6708525607bc7a2985c6a423e6cb63d6175e3ad60d997873c4519fab371772fe`  
		Last Modified: Wed, 09 Nov 2022 16:48:43 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cb5d7747e73374a2c02473deb4bde157dddb2835cb5e66800cfba5842c1fd88`  
		Last Modified: Thu, 17 Nov 2022 20:20:12 GMT  
		Size: 5.0 MB (4974250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b3d427408549420b1666d1a85d3ff1bd3132f4e61dd9a7bd4e75a7c5adc32ee`  
		Last Modified: Thu, 17 Nov 2022 20:20:11 GMT  
		Size: 1.8 KB (1811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4682e51d5cc8bfadb600b57559df30d236b94223a5e9b1c3d2468f6acb1ee3f3`  
		Last Modified: Thu, 17 Nov 2022 20:20:11 GMT  
		Size: 1.2 KB (1161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8223b92ce81db067bb8ee9eacbf53e251b0dcd29dd1af6aa3a519768f0a7b44b`  
		Last Modified: Thu, 17 Nov 2022 20:20:11 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51f050378e256630049566bfcc0cf782533a8f961bcae8b6d9421ef19a8a780f`  
		Last Modified: Thu, 17 Nov 2022 20:20:11 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.7-nanoserver-1809`

```console
$ docker pull nats@sha256:8f26c87d964b3426a16e546857fc7873a8acc6ee97786a9366744ae849a4825d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3650; amd64

### `nats:2.9.7-nanoserver-1809` - windows version 10.0.17763.3650; amd64

```console
$ docker pull nats@sha256:b69aaf3d5200a1cb93e65a79acaa950d17ee0b0e88be899c4c3ecd6695cf9529
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.7 MB (111704287 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a82f827f381afa49f7b9d69a162222472931dd2aad1ebbac2b60a8155e798028`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 05 Nov 2022 18:06:28 GMT
RUN Apply image 10.0.17763.3650
# Wed, 09 Nov 2022 16:47:43 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Thu, 17 Nov 2022 20:19:19 GMT
RUN cmd /S /C #(nop) COPY file:d6b547504effc3514ee13384db156b8c7df287eadd44c86f4e5f5eabb6646c1d in C:\nats-server.exe 
# Thu, 17 Nov 2022 20:19:20 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Thu, 17 Nov 2022 20:19:21 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Thu, 17 Nov 2022 20:19:21 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 17 Nov 2022 20:19:22 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:35ab4104a4d9df6a0d1eac84cc8fbc13511ef6c8aef5ced04fdf63e7e20803a3`  
		Last Modified: Tue, 08 Nov 2022 19:45:20 GMT  
		Size: 106.7 MB (106723592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6708525607bc7a2985c6a423e6cb63d6175e3ad60d997873c4519fab371772fe`  
		Last Modified: Wed, 09 Nov 2022 16:48:43 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cb5d7747e73374a2c02473deb4bde157dddb2835cb5e66800cfba5842c1fd88`  
		Last Modified: Thu, 17 Nov 2022 20:20:12 GMT  
		Size: 5.0 MB (4974250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b3d427408549420b1666d1a85d3ff1bd3132f4e61dd9a7bd4e75a7c5adc32ee`  
		Last Modified: Thu, 17 Nov 2022 20:20:11 GMT  
		Size: 1.8 KB (1811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4682e51d5cc8bfadb600b57559df30d236b94223a5e9b1c3d2468f6acb1ee3f3`  
		Last Modified: Thu, 17 Nov 2022 20:20:11 GMT  
		Size: 1.2 KB (1161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8223b92ce81db067bb8ee9eacbf53e251b0dcd29dd1af6aa3a519768f0a7b44b`  
		Last Modified: Thu, 17 Nov 2022 20:20:11 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51f050378e256630049566bfcc0cf782533a8f961bcae8b6d9421ef19a8a780f`  
		Last Modified: Thu, 17 Nov 2022 20:20:11 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.7-scratch`

```console
$ docker pull nats@sha256:26a7092afff4cfbdd0fc17bd33dbf3308383876690a72fd95b009500d840dce2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9.7-scratch` - linux; amd64

```console
$ docker pull nats@sha256:6fc6aee58f7a448bb3bbd803f3addfa0c9512b5083376ce20781b9b635c381cf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4918825 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:974c838918842c11cbf59d7af83a073f753537c9d4b14f47231d3c1c7ba41c9e`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 17 Nov 2022 20:21:46 GMT
COPY file:88cbf98679a4e287b67a701a1fb77e0e0928e75cc0e1e669916e033ecf774fdc in /nats-server 
# Thu, 17 Nov 2022 20:21:46 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 17 Nov 2022 20:21:46 GMT
EXPOSE 4222 6222 8222
# Thu, 17 Nov 2022 20:21:46 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 17 Nov 2022 20:21:46 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 17 Nov 2022 20:21:47 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c8ce17c05ed27e7e08286a74c292d54eb2d5902af8f901dab4505ba83f7296f5`  
		Last Modified: Thu, 17 Nov 2022 20:22:33 GMT  
		Size: 4.9 MB (4918317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88c3d57c92f61ccff2db59e857c959bc11ca2ed1a6ca7f5494aa479c513196f7`  
		Last Modified: Thu, 17 Nov 2022 20:22:32 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.7-scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:9e5158db138340db27aef59e820bafe7a09359e8910c2cef451b58348dd329ff
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4683160 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b5c60a8afd73cd47b032a2d66e4968bf12f1aed52fee0f708cf184ef6c09b960`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 17 Nov 2022 20:49:48 GMT
COPY file:75f2ce97960bd08a17d41dd00b0f977ff54641b0f3d5b35f613c50553a59e8e1 in /nats-server 
# Thu, 17 Nov 2022 20:49:48 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 17 Nov 2022 20:49:49 GMT
EXPOSE 4222 6222 8222
# Thu, 17 Nov 2022 20:49:49 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 17 Nov 2022 20:49:49 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 17 Nov 2022 20:49:49 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:e27c576ee7d0df355bb5ab346016b3a399e8048fe3f938263b3b77e343d9243f`  
		Last Modified: Thu, 17 Nov 2022 20:51:22 GMT  
		Size: 4.7 MB (4682651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:788fb9f41d9d2c69e1f5737db95b3d0e754d24cd75bdd8d94a80166b8c97d6b6`  
		Last Modified: Thu, 17 Nov 2022 20:51:21 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.7-scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:e4c874e4f9f5eafa49bdd7fed9a022da8958f69cc70e245af8bb9ebf7cad0c0c
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4679780 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2bc64213c48245d6c2d479e5be4d5043a6d811cb9d273ae36c8dfa157accbd04`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 17 Nov 2022 20:58:06 GMT
COPY file:ebca823a5dac00609e9fb9733528840572067b84b58dcccbe67a2df698f2869e in /nats-server 
# Thu, 17 Nov 2022 20:58:06 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 17 Nov 2022 20:58:06 GMT
EXPOSE 4222 6222 8222
# Thu, 17 Nov 2022 20:58:06 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 17 Nov 2022 20:58:06 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 17 Nov 2022 20:58:06 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:2c415cfba68b644bd88b057d832ff5015af29e04439812f5bd2e6873b3d7b8fd`  
		Last Modified: Thu, 17 Nov 2022 20:59:39 GMT  
		Size: 4.7 MB (4679272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:875032eeefdff15b8e0c04ffba01805fa83a04cad983b8322b99f53b04e9c1fe`  
		Last Modified: Thu, 17 Nov 2022 20:59:38 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.7-scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:6d5eefe444c9be5d4f08fd3ccf8277d186014689ef84ea0f59c59dc11acb4904
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4504058 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7ac0ab188af08ab1a9c049a3f6c349d0d2df9595cee8e6626c19a913526dcb2`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 17 Nov 2022 20:40:45 GMT
COPY file:d11c7b340550df0716193331cacb3d06f2cb3b9971e90e006a9c153aaadc50f8 in /nats-server 
# Thu, 17 Nov 2022 20:40:45 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 17 Nov 2022 20:40:45 GMT
EXPOSE 4222 6222 8222
# Thu, 17 Nov 2022 20:40:45 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 17 Nov 2022 20:40:45 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 17 Nov 2022 20:40:45 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:d3e01af3796e331721cc924f0d95499739cea560e1ac4bac35c11176033c94c8`  
		Last Modified: Thu, 17 Nov 2022 20:41:30 GMT  
		Size: 4.5 MB (4503550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e0b7a277e0d621acb2a17025b4318262de852c8be74070453c2f8c9983601ad`  
		Last Modified: Thu, 17 Nov 2022 20:41:30 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.7-windowsservercore`

```console
$ docker pull nats@sha256:a2a17b6c8e185249db8f657d5b4b5473e4627feb0a7ea39ac121544d7ab11465
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3650; amd64

### `nats:2.9.7-windowsservercore` - windows version 10.0.17763.3650; amd64

```console
$ docker pull nats@sha256:d42d0b0ee29bdd7b0ea24be91fb754a64a3da2ab070ed93e185e983132b9beec
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2784314848 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a836a477662568b8b4f2cd2ba8211273a6ae351f51fd48d29015400f42f395c`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 05 Nov 2022 18:29:26 GMT
RUN Install update 10.0.17763.3650
# Wed, 09 Nov 2022 14:50:58 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Nov 2022 16:44:45 GMT
ENV NATS_DOCKERIZED=1
# Thu, 17 Nov 2022 20:15:26 GMT
ENV NATS_SERVER=2.9.7
# Thu, 17 Nov 2022 20:15:27 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.9.7/nats-server-v2.9.7-windows-amd64.zip
# Thu, 17 Nov 2022 20:15:28 GMT
ENV NATS_SERVER_SHASUM=f1baa1646b7a499d035ebfd529644c1379988ab69703a090f9899c97067cea02
# Thu, 17 Nov 2022 20:17:00 GMT
RUN Set-PSDebug -Trace 2
# Thu, 17 Nov 2022 20:18:59 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Thu, 17 Nov 2022 20:19:00 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Thu, 17 Nov 2022 20:19:01 GMT
EXPOSE 4222 6222 8222
# Thu, 17 Nov 2022 20:19:02 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 17 Nov 2022 20:19:03 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a48a3e4ae2de839d8e99bde16eb91d113fb2cf889bba472d0c4274851b5fb402`  
		Last Modified: Tue, 21 Jun 2022 18:30:17 GMT  
		Size: 1.9 GB (1924269350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c26cc6e4f9eb1ae415a5ead6f884cac597bbd57efa6cd042c878d5b54c9d2091`  
		Last Modified: Tue, 08 Nov 2022 19:44:35 GMT  
		Size: 854.3 MB (854317461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99941fb33972e616b231a8aadd93463fdfd5de6aece4aa6c470d2feec31839be`  
		Last Modified: Wed, 09 Nov 2022 16:48:23 GMT  
		Size: 1.3 KB (1335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0f3d8a87f0a1540850986ff94131286dfa42ca116f04779e02f60b3a724641b`  
		Last Modified: Wed, 09 Nov 2022 16:48:23 GMT  
		Size: 1.3 KB (1327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69b8ead5903ee0014b1d59597e3e42c54eb9ad338e077477176b04d22ab4f291`  
		Last Modified: Thu, 17 Nov 2022 20:19:56 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd5112842b491d9aed12c373a680aa352fda7856f4dd7ae100240cda81004d10`  
		Last Modified: Thu, 17 Nov 2022 20:19:56 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27e8ac611281af798a4d5c0f0ffeca3542a44a865688ca95c3f963d0f3a2b009`  
		Last Modified: Thu, 17 Nov 2022 20:19:56 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ced45d282af98e490deb218ae7d77ad9ee20038016ea5fad600ab6363d4339fd`  
		Last Modified: Thu, 17 Nov 2022 20:19:56 GMT  
		Size: 381.6 KB (381592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d244e04b249f9171046dc315cd9c7d70aadbaa6496d85f41de583773d750a76b`  
		Last Modified: Thu, 17 Nov 2022 20:19:55 GMT  
		Size: 5.3 MB (5333250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e9dc3cf2f9c57dc6d24c7b6d3a526d97d4c7ef1de724d54dae9ad10211ba0e1`  
		Last Modified: Thu, 17 Nov 2022 20:19:54 GMT  
		Size: 2.0 KB (2001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6e0bb8f7d2e8165a51f2f77c4ee12feb907b21e4a5f2fe8c6215e6ee1c3b075`  
		Last Modified: Thu, 17 Nov 2022 20:19:54 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80326cc866c490bc13a4ead203b6b1af79320652c34f6605511671f003980078`  
		Last Modified: Thu, 17 Nov 2022 20:19:54 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7785e4126ef3eb2bac999118a556a59d9ab9474c8175a5742b4a1c7fba660efe`  
		Last Modified: Thu, 17 Nov 2022 20:19:54 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.7-windowsservercore-1809`

```console
$ docker pull nats@sha256:a2a17b6c8e185249db8f657d5b4b5473e4627feb0a7ea39ac121544d7ab11465
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3650; amd64

### `nats:2.9.7-windowsservercore-1809` - windows version 10.0.17763.3650; amd64

```console
$ docker pull nats@sha256:d42d0b0ee29bdd7b0ea24be91fb754a64a3da2ab070ed93e185e983132b9beec
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2784314848 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a836a477662568b8b4f2cd2ba8211273a6ae351f51fd48d29015400f42f395c`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 05 Nov 2022 18:29:26 GMT
RUN Install update 10.0.17763.3650
# Wed, 09 Nov 2022 14:50:58 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Nov 2022 16:44:45 GMT
ENV NATS_DOCKERIZED=1
# Thu, 17 Nov 2022 20:15:26 GMT
ENV NATS_SERVER=2.9.7
# Thu, 17 Nov 2022 20:15:27 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.9.7/nats-server-v2.9.7-windows-amd64.zip
# Thu, 17 Nov 2022 20:15:28 GMT
ENV NATS_SERVER_SHASUM=f1baa1646b7a499d035ebfd529644c1379988ab69703a090f9899c97067cea02
# Thu, 17 Nov 2022 20:17:00 GMT
RUN Set-PSDebug -Trace 2
# Thu, 17 Nov 2022 20:18:59 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Thu, 17 Nov 2022 20:19:00 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Thu, 17 Nov 2022 20:19:01 GMT
EXPOSE 4222 6222 8222
# Thu, 17 Nov 2022 20:19:02 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 17 Nov 2022 20:19:03 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a48a3e4ae2de839d8e99bde16eb91d113fb2cf889bba472d0c4274851b5fb402`  
		Last Modified: Tue, 21 Jun 2022 18:30:17 GMT  
		Size: 1.9 GB (1924269350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c26cc6e4f9eb1ae415a5ead6f884cac597bbd57efa6cd042c878d5b54c9d2091`  
		Last Modified: Tue, 08 Nov 2022 19:44:35 GMT  
		Size: 854.3 MB (854317461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99941fb33972e616b231a8aadd93463fdfd5de6aece4aa6c470d2feec31839be`  
		Last Modified: Wed, 09 Nov 2022 16:48:23 GMT  
		Size: 1.3 KB (1335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0f3d8a87f0a1540850986ff94131286dfa42ca116f04779e02f60b3a724641b`  
		Last Modified: Wed, 09 Nov 2022 16:48:23 GMT  
		Size: 1.3 KB (1327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69b8ead5903ee0014b1d59597e3e42c54eb9ad338e077477176b04d22ab4f291`  
		Last Modified: Thu, 17 Nov 2022 20:19:56 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd5112842b491d9aed12c373a680aa352fda7856f4dd7ae100240cda81004d10`  
		Last Modified: Thu, 17 Nov 2022 20:19:56 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27e8ac611281af798a4d5c0f0ffeca3542a44a865688ca95c3f963d0f3a2b009`  
		Last Modified: Thu, 17 Nov 2022 20:19:56 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ced45d282af98e490deb218ae7d77ad9ee20038016ea5fad600ab6363d4339fd`  
		Last Modified: Thu, 17 Nov 2022 20:19:56 GMT  
		Size: 381.6 KB (381592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d244e04b249f9171046dc315cd9c7d70aadbaa6496d85f41de583773d750a76b`  
		Last Modified: Thu, 17 Nov 2022 20:19:55 GMT  
		Size: 5.3 MB (5333250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e9dc3cf2f9c57dc6d24c7b6d3a526d97d4c7ef1de724d54dae9ad10211ba0e1`  
		Last Modified: Thu, 17 Nov 2022 20:19:54 GMT  
		Size: 2.0 KB (2001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6e0bb8f7d2e8165a51f2f77c4ee12feb907b21e4a5f2fe8c6215e6ee1c3b075`  
		Last Modified: Thu, 17 Nov 2022 20:19:54 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80326cc866c490bc13a4ead203b6b1af79320652c34f6605511671f003980078`  
		Last Modified: Thu, 17 Nov 2022 20:19:54 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7785e4126ef3eb2bac999118a556a59d9ab9474c8175a5742b4a1c7fba660efe`  
		Last Modified: Thu, 17 Nov 2022 20:19:54 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:alpine`

```console
$ docker pull nats@sha256:400adfffe0df7f2df0e76d34d6e25a0fb8eb68cfdc10d404afbbb31f818d0276
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:alpine` - linux; amd64

```console
$ docker pull nats@sha256:d4698031a0afeb1ed37b240a9632b22a2d0fcea5fd48af3c8b28e1eba3348033
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.0 MB (8014859 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c26ee116aa283ae59469d995e49cce15bb982559c777e32f06933e315898c54`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Sat, 12 Nov 2022 04:19:23 GMT
ADD file:ceeb6e8632fafc657116cbf3afbd522185a16963230b57881073dad22eb0e1a3 in / 
# Sat, 12 Nov 2022 04:19:23 GMT
CMD ["/bin/sh"]
# Thu, 17 Nov 2022 20:21:36 GMT
ENV NATS_SERVER=2.9.7
# Thu, 17 Nov 2022 20:21:38 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='153018a675b0e896ffbed0cbc3fe5f733fd674d2f4bf554130ae8960a6c5277c' ;; 		armhf) natsArch='arm6'; sha256='9714af72c37f0ede4465a3b0324230af74701e82414194a9c2228e7563327523' ;; 		armv7) natsArch='arm7'; sha256='804ec4f600418d4afd6a9cb94b92c306ab75c589fc5180a5c2c99cc514c0899a' ;; 		x86_64) natsArch='amd64'; sha256='d4d2ef2952a9a841ce6594a4dbd07b8a45ceea32dadb321ddebc0c56598c2085' ;; 		x86) natsArch='386'; sha256='add5a328af2cab82230f881f71f7ca4dd907b477972d14a06b77b83188863d4d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 17 Nov 2022 20:21:38 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 17 Nov 2022 20:21:38 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 17 Nov 2022 20:21:39 GMT
EXPOSE 4222 6222 8222
# Thu, 17 Nov 2022 20:21:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Nov 2022 20:21:39 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:ca7dd9ec2225f2385955c43b2379305acd51543c28cf1d4e94522b3d94cce3ce`  
		Last Modified: Sat, 12 Nov 2022 02:52:15 GMT  
		Size: 2.8 MB (2806272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94acb566bf3ae8a5a3c0747075e8b16df167a9694bfb5ac6ccdea4e5558e2a01`  
		Last Modified: Thu, 17 Nov 2022 20:22:12 GMT  
		Size: 5.2 MB (5207590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e759e667a2c2d6d67aaf3491e124f07a1afc8de774d7973958b32b81ff7a0304`  
		Last Modified: Thu, 17 Nov 2022 20:22:11 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c0e8173963a2be8b30df5827fcfc01a70e5c95ab186696e43d9f624884cee41`  
		Last Modified: Thu, 17 Nov 2022 20:22:11 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:221c14c269fed109042c154935b6cd22b270dda8b66b30e48f734f5fb50ffb87
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7586411 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b8f37497160e12532b20e7eaca7e50daa1304f46b7002848dfae699b06743ba`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Sat, 12 Nov 2022 03:49:18 GMT
ADD file:493290ed8856fa13463defe63da0d30ab3de5dde042c87ef7c0701d66ebb8892 in / 
# Sat, 12 Nov 2022 03:49:18 GMT
CMD ["/bin/sh"]
# Thu, 17 Nov 2022 20:49:34 GMT
ENV NATS_SERVER=2.9.7
# Thu, 17 Nov 2022 20:49:36 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='153018a675b0e896ffbed0cbc3fe5f733fd674d2f4bf554130ae8960a6c5277c' ;; 		armhf) natsArch='arm6'; sha256='9714af72c37f0ede4465a3b0324230af74701e82414194a9c2228e7563327523' ;; 		armv7) natsArch='arm7'; sha256='804ec4f600418d4afd6a9cb94b92c306ab75c589fc5180a5c2c99cc514c0899a' ;; 		x86_64) natsArch='amd64'; sha256='d4d2ef2952a9a841ce6594a4dbd07b8a45ceea32dadb321ddebc0c56598c2085' ;; 		x86) natsArch='386'; sha256='add5a328af2cab82230f881f71f7ca4dd907b477972d14a06b77b83188863d4d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 17 Nov 2022 20:49:36 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 17 Nov 2022 20:49:36 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 17 Nov 2022 20:49:36 GMT
EXPOSE 4222 6222 8222
# Thu, 17 Nov 2022 20:49:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Nov 2022 20:49:37 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9616ea8c1de4a90b1a50591336485e88ae5c2346e0d778bdbe69b00647bf8e39`  
		Last Modified: Sat, 12 Nov 2022 03:50:12 GMT  
		Size: 2.6 MB (2615105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d5728111a27515c16eb46117bf3339ccefc8af39e7c1508951d9286a3c3891c`  
		Last Modified: Thu, 17 Nov 2022 20:50:52 GMT  
		Size: 5.0 MB (4970331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d3e171e5c82f413b32d409f4fce9c56e3a429da91e068be34239e7c8c856576`  
		Last Modified: Thu, 17 Nov 2022 20:50:51 GMT  
		Size: 561.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:699b733f623013826c3dee6862aac2f7cb12bc97712d445dcf79191ba87875f6`  
		Last Modified: Thu, 17 Nov 2022 20:50:51 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:bf2175af45ce04af8a4d8a8c810eb98dbbdf0208010f248234803a56346e7492
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.4 MB (7380724 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af540a578654dbc22e31a00269e904f93dae199d3a57c7b588311595cd8c326c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Sat, 12 Nov 2022 03:57:24 GMT
ADD file:0b4a628f529226f5ec9d357ca63138bd2d22411a889c780ac8d395d761e07b2c in / 
# Sat, 12 Nov 2022 03:57:24 GMT
CMD ["/bin/sh"]
# Thu, 17 Nov 2022 20:57:48 GMT
ENV NATS_SERVER=2.9.7
# Thu, 17 Nov 2022 20:57:51 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='153018a675b0e896ffbed0cbc3fe5f733fd674d2f4bf554130ae8960a6c5277c' ;; 		armhf) natsArch='arm6'; sha256='9714af72c37f0ede4465a3b0324230af74701e82414194a9c2228e7563327523' ;; 		armv7) natsArch='arm7'; sha256='804ec4f600418d4afd6a9cb94b92c306ab75c589fc5180a5c2c99cc514c0899a' ;; 		x86_64) natsArch='amd64'; sha256='d4d2ef2952a9a841ce6594a4dbd07b8a45ceea32dadb321ddebc0c56598c2085' ;; 		x86) natsArch='386'; sha256='add5a328af2cab82230f881f71f7ca4dd907b477972d14a06b77b83188863d4d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 17 Nov 2022 20:57:51 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 17 Nov 2022 20:57:51 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 17 Nov 2022 20:57:52 GMT
EXPOSE 4222 6222 8222
# Thu, 17 Nov 2022 20:57:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Nov 2022 20:57:52 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:e44ba29d168a7f7c9e914f3724614df9e070aa6ef9b9ba5c9004db3c071f403a`  
		Last Modified: Sat, 12 Nov 2022 03:58:16 GMT  
		Size: 2.4 MB (2418788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c6aab4ebcc741288db0b5a719ef99f393d0fd90552b7131f9391a1f1bb37575`  
		Last Modified: Thu, 17 Nov 2022 20:59:09 GMT  
		Size: 5.0 MB (4960964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c4be9c1201790ef36f0543a1ad75a874f321b98fb2053e0b742e2f74e72338e`  
		Last Modified: Thu, 17 Nov 2022 20:59:08 GMT  
		Size: 560.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6f34e641f8406d256e755f8e058c5e957c85a985209c0e0021a18e1aab450c9`  
		Last Modified: Thu, 17 Nov 2022 20:59:08 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:173181d8057b550ed4e321336b885f0ada263273ebc6cba24563f43578c00c23
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.5 MB (7503096 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:41f949bc183512a9594a4bcf404727a905c6e76f0ac0318a03cf0e2b93ccf1de`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Sat, 12 Nov 2022 03:39:38 GMT
ADD file:57d621536158358b14d15155826ef2dd4ca034278044111ec0aaf6717016e569 in / 
# Sat, 12 Nov 2022 03:39:38 GMT
CMD ["/bin/sh"]
# Thu, 17 Nov 2022 20:40:36 GMT
ENV NATS_SERVER=2.9.7
# Thu, 17 Nov 2022 20:40:39 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='153018a675b0e896ffbed0cbc3fe5f733fd674d2f4bf554130ae8960a6c5277c' ;; 		armhf) natsArch='arm6'; sha256='9714af72c37f0ede4465a3b0324230af74701e82414194a9c2228e7563327523' ;; 		armv7) natsArch='arm7'; sha256='804ec4f600418d4afd6a9cb94b92c306ab75c589fc5180a5c2c99cc514c0899a' ;; 		x86_64) natsArch='amd64'; sha256='d4d2ef2952a9a841ce6594a4dbd07b8a45ceea32dadb321ddebc0c56598c2085' ;; 		x86) natsArch='386'; sha256='add5a328af2cab82230f881f71f7ca4dd907b477972d14a06b77b83188863d4d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 17 Nov 2022 20:40:39 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 17 Nov 2022 20:40:39 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 17 Nov 2022 20:40:39 GMT
EXPOSE 4222 6222 8222
# Thu, 17 Nov 2022 20:40:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Nov 2022 20:40:40 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:6875df1f535433e5affe18ecfde9acb7950ab5f76887980ff06c5cdd48cf98f4`  
		Last Modified: Sat, 12 Nov 2022 03:40:05 GMT  
		Size: 2.7 MB (2707756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46474a86907df61c3b68bfcfc04ccf1b583ae765e82a80c581951fb9f5e8a104`  
		Last Modified: Thu, 17 Nov 2022 20:41:10 GMT  
		Size: 4.8 MB (4794340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98cf9fbe300cc2e491de01ad75e29bc228c5e706a5140594a1c29c565216b00e`  
		Last Modified: Thu, 17 Nov 2022 20:41:09 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9323da261341d5d9bbcca4222e4b1c77ff87a4bd0aae38eb7e003bc530717bd2`  
		Last Modified: Thu, 17 Nov 2022 20:41:09 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:alpine3.16`

```console
$ docker pull nats@sha256:400adfffe0df7f2df0e76d34d6e25a0fb8eb68cfdc10d404afbbb31f818d0276
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:alpine3.16` - linux; amd64

```console
$ docker pull nats@sha256:d4698031a0afeb1ed37b240a9632b22a2d0fcea5fd48af3c8b28e1eba3348033
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.0 MB (8014859 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c26ee116aa283ae59469d995e49cce15bb982559c777e32f06933e315898c54`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Sat, 12 Nov 2022 04:19:23 GMT
ADD file:ceeb6e8632fafc657116cbf3afbd522185a16963230b57881073dad22eb0e1a3 in / 
# Sat, 12 Nov 2022 04:19:23 GMT
CMD ["/bin/sh"]
# Thu, 17 Nov 2022 20:21:36 GMT
ENV NATS_SERVER=2.9.7
# Thu, 17 Nov 2022 20:21:38 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='153018a675b0e896ffbed0cbc3fe5f733fd674d2f4bf554130ae8960a6c5277c' ;; 		armhf) natsArch='arm6'; sha256='9714af72c37f0ede4465a3b0324230af74701e82414194a9c2228e7563327523' ;; 		armv7) natsArch='arm7'; sha256='804ec4f600418d4afd6a9cb94b92c306ab75c589fc5180a5c2c99cc514c0899a' ;; 		x86_64) natsArch='amd64'; sha256='d4d2ef2952a9a841ce6594a4dbd07b8a45ceea32dadb321ddebc0c56598c2085' ;; 		x86) natsArch='386'; sha256='add5a328af2cab82230f881f71f7ca4dd907b477972d14a06b77b83188863d4d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 17 Nov 2022 20:21:38 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 17 Nov 2022 20:21:38 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 17 Nov 2022 20:21:39 GMT
EXPOSE 4222 6222 8222
# Thu, 17 Nov 2022 20:21:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Nov 2022 20:21:39 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:ca7dd9ec2225f2385955c43b2379305acd51543c28cf1d4e94522b3d94cce3ce`  
		Last Modified: Sat, 12 Nov 2022 02:52:15 GMT  
		Size: 2.8 MB (2806272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94acb566bf3ae8a5a3c0747075e8b16df167a9694bfb5ac6ccdea4e5558e2a01`  
		Last Modified: Thu, 17 Nov 2022 20:22:12 GMT  
		Size: 5.2 MB (5207590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e759e667a2c2d6d67aaf3491e124f07a1afc8de774d7973958b32b81ff7a0304`  
		Last Modified: Thu, 17 Nov 2022 20:22:11 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c0e8173963a2be8b30df5827fcfc01a70e5c95ab186696e43d9f624884cee41`  
		Last Modified: Thu, 17 Nov 2022 20:22:11 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.16` - linux; arm variant v6

```console
$ docker pull nats@sha256:221c14c269fed109042c154935b6cd22b270dda8b66b30e48f734f5fb50ffb87
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7586411 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b8f37497160e12532b20e7eaca7e50daa1304f46b7002848dfae699b06743ba`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Sat, 12 Nov 2022 03:49:18 GMT
ADD file:493290ed8856fa13463defe63da0d30ab3de5dde042c87ef7c0701d66ebb8892 in / 
# Sat, 12 Nov 2022 03:49:18 GMT
CMD ["/bin/sh"]
# Thu, 17 Nov 2022 20:49:34 GMT
ENV NATS_SERVER=2.9.7
# Thu, 17 Nov 2022 20:49:36 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='153018a675b0e896ffbed0cbc3fe5f733fd674d2f4bf554130ae8960a6c5277c' ;; 		armhf) natsArch='arm6'; sha256='9714af72c37f0ede4465a3b0324230af74701e82414194a9c2228e7563327523' ;; 		armv7) natsArch='arm7'; sha256='804ec4f600418d4afd6a9cb94b92c306ab75c589fc5180a5c2c99cc514c0899a' ;; 		x86_64) natsArch='amd64'; sha256='d4d2ef2952a9a841ce6594a4dbd07b8a45ceea32dadb321ddebc0c56598c2085' ;; 		x86) natsArch='386'; sha256='add5a328af2cab82230f881f71f7ca4dd907b477972d14a06b77b83188863d4d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 17 Nov 2022 20:49:36 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 17 Nov 2022 20:49:36 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 17 Nov 2022 20:49:36 GMT
EXPOSE 4222 6222 8222
# Thu, 17 Nov 2022 20:49:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Nov 2022 20:49:37 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9616ea8c1de4a90b1a50591336485e88ae5c2346e0d778bdbe69b00647bf8e39`  
		Last Modified: Sat, 12 Nov 2022 03:50:12 GMT  
		Size: 2.6 MB (2615105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d5728111a27515c16eb46117bf3339ccefc8af39e7c1508951d9286a3c3891c`  
		Last Modified: Thu, 17 Nov 2022 20:50:52 GMT  
		Size: 5.0 MB (4970331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d3e171e5c82f413b32d409f4fce9c56e3a429da91e068be34239e7c8c856576`  
		Last Modified: Thu, 17 Nov 2022 20:50:51 GMT  
		Size: 561.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:699b733f623013826c3dee6862aac2f7cb12bc97712d445dcf79191ba87875f6`  
		Last Modified: Thu, 17 Nov 2022 20:50:51 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.16` - linux; arm variant v7

```console
$ docker pull nats@sha256:bf2175af45ce04af8a4d8a8c810eb98dbbdf0208010f248234803a56346e7492
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.4 MB (7380724 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af540a578654dbc22e31a00269e904f93dae199d3a57c7b588311595cd8c326c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Sat, 12 Nov 2022 03:57:24 GMT
ADD file:0b4a628f529226f5ec9d357ca63138bd2d22411a889c780ac8d395d761e07b2c in / 
# Sat, 12 Nov 2022 03:57:24 GMT
CMD ["/bin/sh"]
# Thu, 17 Nov 2022 20:57:48 GMT
ENV NATS_SERVER=2.9.7
# Thu, 17 Nov 2022 20:57:51 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='153018a675b0e896ffbed0cbc3fe5f733fd674d2f4bf554130ae8960a6c5277c' ;; 		armhf) natsArch='arm6'; sha256='9714af72c37f0ede4465a3b0324230af74701e82414194a9c2228e7563327523' ;; 		armv7) natsArch='arm7'; sha256='804ec4f600418d4afd6a9cb94b92c306ab75c589fc5180a5c2c99cc514c0899a' ;; 		x86_64) natsArch='amd64'; sha256='d4d2ef2952a9a841ce6594a4dbd07b8a45ceea32dadb321ddebc0c56598c2085' ;; 		x86) natsArch='386'; sha256='add5a328af2cab82230f881f71f7ca4dd907b477972d14a06b77b83188863d4d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 17 Nov 2022 20:57:51 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 17 Nov 2022 20:57:51 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 17 Nov 2022 20:57:52 GMT
EXPOSE 4222 6222 8222
# Thu, 17 Nov 2022 20:57:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Nov 2022 20:57:52 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:e44ba29d168a7f7c9e914f3724614df9e070aa6ef9b9ba5c9004db3c071f403a`  
		Last Modified: Sat, 12 Nov 2022 03:58:16 GMT  
		Size: 2.4 MB (2418788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c6aab4ebcc741288db0b5a719ef99f393d0fd90552b7131f9391a1f1bb37575`  
		Last Modified: Thu, 17 Nov 2022 20:59:09 GMT  
		Size: 5.0 MB (4960964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c4be9c1201790ef36f0543a1ad75a874f321b98fb2053e0b742e2f74e72338e`  
		Last Modified: Thu, 17 Nov 2022 20:59:08 GMT  
		Size: 560.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6f34e641f8406d256e755f8e058c5e957c85a985209c0e0021a18e1aab450c9`  
		Last Modified: Thu, 17 Nov 2022 20:59:08 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.16` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:173181d8057b550ed4e321336b885f0ada263273ebc6cba24563f43578c00c23
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.5 MB (7503096 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:41f949bc183512a9594a4bcf404727a905c6e76f0ac0318a03cf0e2b93ccf1de`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Sat, 12 Nov 2022 03:39:38 GMT
ADD file:57d621536158358b14d15155826ef2dd4ca034278044111ec0aaf6717016e569 in / 
# Sat, 12 Nov 2022 03:39:38 GMT
CMD ["/bin/sh"]
# Thu, 17 Nov 2022 20:40:36 GMT
ENV NATS_SERVER=2.9.7
# Thu, 17 Nov 2022 20:40:39 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='153018a675b0e896ffbed0cbc3fe5f733fd674d2f4bf554130ae8960a6c5277c' ;; 		armhf) natsArch='arm6'; sha256='9714af72c37f0ede4465a3b0324230af74701e82414194a9c2228e7563327523' ;; 		armv7) natsArch='arm7'; sha256='804ec4f600418d4afd6a9cb94b92c306ab75c589fc5180a5c2c99cc514c0899a' ;; 		x86_64) natsArch='amd64'; sha256='d4d2ef2952a9a841ce6594a4dbd07b8a45ceea32dadb321ddebc0c56598c2085' ;; 		x86) natsArch='386'; sha256='add5a328af2cab82230f881f71f7ca4dd907b477972d14a06b77b83188863d4d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 17 Nov 2022 20:40:39 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 17 Nov 2022 20:40:39 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 17 Nov 2022 20:40:39 GMT
EXPOSE 4222 6222 8222
# Thu, 17 Nov 2022 20:40:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Nov 2022 20:40:40 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:6875df1f535433e5affe18ecfde9acb7950ab5f76887980ff06c5cdd48cf98f4`  
		Last Modified: Sat, 12 Nov 2022 03:40:05 GMT  
		Size: 2.7 MB (2707756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46474a86907df61c3b68bfcfc04ccf1b583ae765e82a80c581951fb9f5e8a104`  
		Last Modified: Thu, 17 Nov 2022 20:41:10 GMT  
		Size: 4.8 MB (4794340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98cf9fbe300cc2e491de01ad75e29bc228c5e706a5140594a1c29c565216b00e`  
		Last Modified: Thu, 17 Nov 2022 20:41:09 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9323da261341d5d9bbcca4222e4b1c77ff87a4bd0aae38eb7e003bc530717bd2`  
		Last Modified: Thu, 17 Nov 2022 20:41:09 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:latest`

```console
$ docker pull nats@sha256:8a550ace09f524090c5399c7eab008c9f0d55a29eb1732cc4a565d4f1160346c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.3650; amd64

### `nats:latest` - linux; amd64

```console
$ docker pull nats@sha256:6fc6aee58f7a448bb3bbd803f3addfa0c9512b5083376ce20781b9b635c381cf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4918825 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:974c838918842c11cbf59d7af83a073f753537c9d4b14f47231d3c1c7ba41c9e`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 17 Nov 2022 20:21:46 GMT
COPY file:88cbf98679a4e287b67a701a1fb77e0e0928e75cc0e1e669916e033ecf774fdc in /nats-server 
# Thu, 17 Nov 2022 20:21:46 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 17 Nov 2022 20:21:46 GMT
EXPOSE 4222 6222 8222
# Thu, 17 Nov 2022 20:21:46 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 17 Nov 2022 20:21:46 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 17 Nov 2022 20:21:47 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c8ce17c05ed27e7e08286a74c292d54eb2d5902af8f901dab4505ba83f7296f5`  
		Last Modified: Thu, 17 Nov 2022 20:22:33 GMT  
		Size: 4.9 MB (4918317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88c3d57c92f61ccff2db59e857c959bc11ca2ed1a6ca7f5494aa479c513196f7`  
		Last Modified: Thu, 17 Nov 2022 20:22:32 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm variant v6

```console
$ docker pull nats@sha256:9e5158db138340db27aef59e820bafe7a09359e8910c2cef451b58348dd329ff
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4683160 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b5c60a8afd73cd47b032a2d66e4968bf12f1aed52fee0f708cf184ef6c09b960`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 17 Nov 2022 20:49:48 GMT
COPY file:75f2ce97960bd08a17d41dd00b0f977ff54641b0f3d5b35f613c50553a59e8e1 in /nats-server 
# Thu, 17 Nov 2022 20:49:48 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 17 Nov 2022 20:49:49 GMT
EXPOSE 4222 6222 8222
# Thu, 17 Nov 2022 20:49:49 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 17 Nov 2022 20:49:49 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 17 Nov 2022 20:49:49 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:e27c576ee7d0df355bb5ab346016b3a399e8048fe3f938263b3b77e343d9243f`  
		Last Modified: Thu, 17 Nov 2022 20:51:22 GMT  
		Size: 4.7 MB (4682651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:788fb9f41d9d2c69e1f5737db95b3d0e754d24cd75bdd8d94a80166b8c97d6b6`  
		Last Modified: Thu, 17 Nov 2022 20:51:21 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm variant v7

```console
$ docker pull nats@sha256:e4c874e4f9f5eafa49bdd7fed9a022da8958f69cc70e245af8bb9ebf7cad0c0c
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4679780 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2bc64213c48245d6c2d479e5be4d5043a6d811cb9d273ae36c8dfa157accbd04`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 17 Nov 2022 20:58:06 GMT
COPY file:ebca823a5dac00609e9fb9733528840572067b84b58dcccbe67a2df698f2869e in /nats-server 
# Thu, 17 Nov 2022 20:58:06 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 17 Nov 2022 20:58:06 GMT
EXPOSE 4222 6222 8222
# Thu, 17 Nov 2022 20:58:06 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 17 Nov 2022 20:58:06 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 17 Nov 2022 20:58:06 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:2c415cfba68b644bd88b057d832ff5015af29e04439812f5bd2e6873b3d7b8fd`  
		Last Modified: Thu, 17 Nov 2022 20:59:39 GMT  
		Size: 4.7 MB (4679272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:875032eeefdff15b8e0c04ffba01805fa83a04cad983b8322b99f53b04e9c1fe`  
		Last Modified: Thu, 17 Nov 2022 20:59:38 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:6d5eefe444c9be5d4f08fd3ccf8277d186014689ef84ea0f59c59dc11acb4904
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4504058 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7ac0ab188af08ab1a9c049a3f6c349d0d2df9595cee8e6626c19a913526dcb2`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 17 Nov 2022 20:40:45 GMT
COPY file:d11c7b340550df0716193331cacb3d06f2cb3b9971e90e006a9c153aaadc50f8 in /nats-server 
# Thu, 17 Nov 2022 20:40:45 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 17 Nov 2022 20:40:45 GMT
EXPOSE 4222 6222 8222
# Thu, 17 Nov 2022 20:40:45 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 17 Nov 2022 20:40:45 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 17 Nov 2022 20:40:45 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:d3e01af3796e331721cc924f0d95499739cea560e1ac4bac35c11176033c94c8`  
		Last Modified: Thu, 17 Nov 2022 20:41:30 GMT  
		Size: 4.5 MB (4503550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e0b7a277e0d621acb2a17025b4318262de852c8be74070453c2f8c9983601ad`  
		Last Modified: Thu, 17 Nov 2022 20:41:30 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - windows version 10.0.17763.3650; amd64

```console
$ docker pull nats@sha256:b69aaf3d5200a1cb93e65a79acaa950d17ee0b0e88be899c4c3ecd6695cf9529
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.7 MB (111704287 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a82f827f381afa49f7b9d69a162222472931dd2aad1ebbac2b60a8155e798028`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 05 Nov 2022 18:06:28 GMT
RUN Apply image 10.0.17763.3650
# Wed, 09 Nov 2022 16:47:43 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Thu, 17 Nov 2022 20:19:19 GMT
RUN cmd /S /C #(nop) COPY file:d6b547504effc3514ee13384db156b8c7df287eadd44c86f4e5f5eabb6646c1d in C:\nats-server.exe 
# Thu, 17 Nov 2022 20:19:20 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Thu, 17 Nov 2022 20:19:21 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Thu, 17 Nov 2022 20:19:21 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 17 Nov 2022 20:19:22 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:35ab4104a4d9df6a0d1eac84cc8fbc13511ef6c8aef5ced04fdf63e7e20803a3`  
		Last Modified: Tue, 08 Nov 2022 19:45:20 GMT  
		Size: 106.7 MB (106723592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6708525607bc7a2985c6a423e6cb63d6175e3ad60d997873c4519fab371772fe`  
		Last Modified: Wed, 09 Nov 2022 16:48:43 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cb5d7747e73374a2c02473deb4bde157dddb2835cb5e66800cfba5842c1fd88`  
		Last Modified: Thu, 17 Nov 2022 20:20:12 GMT  
		Size: 5.0 MB (4974250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b3d427408549420b1666d1a85d3ff1bd3132f4e61dd9a7bd4e75a7c5adc32ee`  
		Last Modified: Thu, 17 Nov 2022 20:20:11 GMT  
		Size: 1.8 KB (1811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4682e51d5cc8bfadb600b57559df30d236b94223a5e9b1c3d2468f6acb1ee3f3`  
		Last Modified: Thu, 17 Nov 2022 20:20:11 GMT  
		Size: 1.2 KB (1161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8223b92ce81db067bb8ee9eacbf53e251b0dcd29dd1af6aa3a519768f0a7b44b`  
		Last Modified: Thu, 17 Nov 2022 20:20:11 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51f050378e256630049566bfcc0cf782533a8f961bcae8b6d9421ef19a8a780f`  
		Last Modified: Thu, 17 Nov 2022 20:20:11 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:linux`

```console
$ docker pull nats@sha256:26a7092afff4cfbdd0fc17bd33dbf3308383876690a72fd95b009500d840dce2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:linux` - linux; amd64

```console
$ docker pull nats@sha256:6fc6aee58f7a448bb3bbd803f3addfa0c9512b5083376ce20781b9b635c381cf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4918825 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:974c838918842c11cbf59d7af83a073f753537c9d4b14f47231d3c1c7ba41c9e`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 17 Nov 2022 20:21:46 GMT
COPY file:88cbf98679a4e287b67a701a1fb77e0e0928e75cc0e1e669916e033ecf774fdc in /nats-server 
# Thu, 17 Nov 2022 20:21:46 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 17 Nov 2022 20:21:46 GMT
EXPOSE 4222 6222 8222
# Thu, 17 Nov 2022 20:21:46 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 17 Nov 2022 20:21:46 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 17 Nov 2022 20:21:47 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c8ce17c05ed27e7e08286a74c292d54eb2d5902af8f901dab4505ba83f7296f5`  
		Last Modified: Thu, 17 Nov 2022 20:22:33 GMT  
		Size: 4.9 MB (4918317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88c3d57c92f61ccff2db59e857c959bc11ca2ed1a6ca7f5494aa479c513196f7`  
		Last Modified: Thu, 17 Nov 2022 20:22:32 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:9e5158db138340db27aef59e820bafe7a09359e8910c2cef451b58348dd329ff
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4683160 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b5c60a8afd73cd47b032a2d66e4968bf12f1aed52fee0f708cf184ef6c09b960`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 17 Nov 2022 20:49:48 GMT
COPY file:75f2ce97960bd08a17d41dd00b0f977ff54641b0f3d5b35f613c50553a59e8e1 in /nats-server 
# Thu, 17 Nov 2022 20:49:48 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 17 Nov 2022 20:49:49 GMT
EXPOSE 4222 6222 8222
# Thu, 17 Nov 2022 20:49:49 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 17 Nov 2022 20:49:49 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 17 Nov 2022 20:49:49 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:e27c576ee7d0df355bb5ab346016b3a399e8048fe3f938263b3b77e343d9243f`  
		Last Modified: Thu, 17 Nov 2022 20:51:22 GMT  
		Size: 4.7 MB (4682651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:788fb9f41d9d2c69e1f5737db95b3d0e754d24cd75bdd8d94a80166b8c97d6b6`  
		Last Modified: Thu, 17 Nov 2022 20:51:21 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:e4c874e4f9f5eafa49bdd7fed9a022da8958f69cc70e245af8bb9ebf7cad0c0c
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4679780 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2bc64213c48245d6c2d479e5be4d5043a6d811cb9d273ae36c8dfa157accbd04`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 17 Nov 2022 20:58:06 GMT
COPY file:ebca823a5dac00609e9fb9733528840572067b84b58dcccbe67a2df698f2869e in /nats-server 
# Thu, 17 Nov 2022 20:58:06 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 17 Nov 2022 20:58:06 GMT
EXPOSE 4222 6222 8222
# Thu, 17 Nov 2022 20:58:06 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 17 Nov 2022 20:58:06 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 17 Nov 2022 20:58:06 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:2c415cfba68b644bd88b057d832ff5015af29e04439812f5bd2e6873b3d7b8fd`  
		Last Modified: Thu, 17 Nov 2022 20:59:39 GMT  
		Size: 4.7 MB (4679272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:875032eeefdff15b8e0c04ffba01805fa83a04cad983b8322b99f53b04e9c1fe`  
		Last Modified: Thu, 17 Nov 2022 20:59:38 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:6d5eefe444c9be5d4f08fd3ccf8277d186014689ef84ea0f59c59dc11acb4904
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4504058 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7ac0ab188af08ab1a9c049a3f6c349d0d2df9595cee8e6626c19a913526dcb2`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 17 Nov 2022 20:40:45 GMT
COPY file:d11c7b340550df0716193331cacb3d06f2cb3b9971e90e006a9c153aaadc50f8 in /nats-server 
# Thu, 17 Nov 2022 20:40:45 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 17 Nov 2022 20:40:45 GMT
EXPOSE 4222 6222 8222
# Thu, 17 Nov 2022 20:40:45 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 17 Nov 2022 20:40:45 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 17 Nov 2022 20:40:45 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:d3e01af3796e331721cc924f0d95499739cea560e1ac4bac35c11176033c94c8`  
		Last Modified: Thu, 17 Nov 2022 20:41:30 GMT  
		Size: 4.5 MB (4503550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e0b7a277e0d621acb2a17025b4318262de852c8be74070453c2f8c9983601ad`  
		Last Modified: Thu, 17 Nov 2022 20:41:30 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:nanoserver`

```console
$ docker pull nats@sha256:8f26c87d964b3426a16e546857fc7873a8acc6ee97786a9366744ae849a4825d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3650; amd64

### `nats:nanoserver` - windows version 10.0.17763.3650; amd64

```console
$ docker pull nats@sha256:b69aaf3d5200a1cb93e65a79acaa950d17ee0b0e88be899c4c3ecd6695cf9529
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.7 MB (111704287 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a82f827f381afa49f7b9d69a162222472931dd2aad1ebbac2b60a8155e798028`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 05 Nov 2022 18:06:28 GMT
RUN Apply image 10.0.17763.3650
# Wed, 09 Nov 2022 16:47:43 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Thu, 17 Nov 2022 20:19:19 GMT
RUN cmd /S /C #(nop) COPY file:d6b547504effc3514ee13384db156b8c7df287eadd44c86f4e5f5eabb6646c1d in C:\nats-server.exe 
# Thu, 17 Nov 2022 20:19:20 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Thu, 17 Nov 2022 20:19:21 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Thu, 17 Nov 2022 20:19:21 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 17 Nov 2022 20:19:22 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:35ab4104a4d9df6a0d1eac84cc8fbc13511ef6c8aef5ced04fdf63e7e20803a3`  
		Last Modified: Tue, 08 Nov 2022 19:45:20 GMT  
		Size: 106.7 MB (106723592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6708525607bc7a2985c6a423e6cb63d6175e3ad60d997873c4519fab371772fe`  
		Last Modified: Wed, 09 Nov 2022 16:48:43 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cb5d7747e73374a2c02473deb4bde157dddb2835cb5e66800cfba5842c1fd88`  
		Last Modified: Thu, 17 Nov 2022 20:20:12 GMT  
		Size: 5.0 MB (4974250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b3d427408549420b1666d1a85d3ff1bd3132f4e61dd9a7bd4e75a7c5adc32ee`  
		Last Modified: Thu, 17 Nov 2022 20:20:11 GMT  
		Size: 1.8 KB (1811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4682e51d5cc8bfadb600b57559df30d236b94223a5e9b1c3d2468f6acb1ee3f3`  
		Last Modified: Thu, 17 Nov 2022 20:20:11 GMT  
		Size: 1.2 KB (1161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8223b92ce81db067bb8ee9eacbf53e251b0dcd29dd1af6aa3a519768f0a7b44b`  
		Last Modified: Thu, 17 Nov 2022 20:20:11 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51f050378e256630049566bfcc0cf782533a8f961bcae8b6d9421ef19a8a780f`  
		Last Modified: Thu, 17 Nov 2022 20:20:11 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:nanoserver-1809`

```console
$ docker pull nats@sha256:8f26c87d964b3426a16e546857fc7873a8acc6ee97786a9366744ae849a4825d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3650; amd64

### `nats:nanoserver-1809` - windows version 10.0.17763.3650; amd64

```console
$ docker pull nats@sha256:b69aaf3d5200a1cb93e65a79acaa950d17ee0b0e88be899c4c3ecd6695cf9529
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.7 MB (111704287 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a82f827f381afa49f7b9d69a162222472931dd2aad1ebbac2b60a8155e798028`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 05 Nov 2022 18:06:28 GMT
RUN Apply image 10.0.17763.3650
# Wed, 09 Nov 2022 16:47:43 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Thu, 17 Nov 2022 20:19:19 GMT
RUN cmd /S /C #(nop) COPY file:d6b547504effc3514ee13384db156b8c7df287eadd44c86f4e5f5eabb6646c1d in C:\nats-server.exe 
# Thu, 17 Nov 2022 20:19:20 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Thu, 17 Nov 2022 20:19:21 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Thu, 17 Nov 2022 20:19:21 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 17 Nov 2022 20:19:22 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:35ab4104a4d9df6a0d1eac84cc8fbc13511ef6c8aef5ced04fdf63e7e20803a3`  
		Last Modified: Tue, 08 Nov 2022 19:45:20 GMT  
		Size: 106.7 MB (106723592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6708525607bc7a2985c6a423e6cb63d6175e3ad60d997873c4519fab371772fe`  
		Last Modified: Wed, 09 Nov 2022 16:48:43 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cb5d7747e73374a2c02473deb4bde157dddb2835cb5e66800cfba5842c1fd88`  
		Last Modified: Thu, 17 Nov 2022 20:20:12 GMT  
		Size: 5.0 MB (4974250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b3d427408549420b1666d1a85d3ff1bd3132f4e61dd9a7bd4e75a7c5adc32ee`  
		Last Modified: Thu, 17 Nov 2022 20:20:11 GMT  
		Size: 1.8 KB (1811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4682e51d5cc8bfadb600b57559df30d236b94223a5e9b1c3d2468f6acb1ee3f3`  
		Last Modified: Thu, 17 Nov 2022 20:20:11 GMT  
		Size: 1.2 KB (1161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8223b92ce81db067bb8ee9eacbf53e251b0dcd29dd1af6aa3a519768f0a7b44b`  
		Last Modified: Thu, 17 Nov 2022 20:20:11 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51f050378e256630049566bfcc0cf782533a8f961bcae8b6d9421ef19a8a780f`  
		Last Modified: Thu, 17 Nov 2022 20:20:11 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:scratch`

```console
$ docker pull nats@sha256:26a7092afff4cfbdd0fc17bd33dbf3308383876690a72fd95b009500d840dce2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:scratch` - linux; amd64

```console
$ docker pull nats@sha256:6fc6aee58f7a448bb3bbd803f3addfa0c9512b5083376ce20781b9b635c381cf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4918825 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:974c838918842c11cbf59d7af83a073f753537c9d4b14f47231d3c1c7ba41c9e`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 17 Nov 2022 20:21:46 GMT
COPY file:88cbf98679a4e287b67a701a1fb77e0e0928e75cc0e1e669916e033ecf774fdc in /nats-server 
# Thu, 17 Nov 2022 20:21:46 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 17 Nov 2022 20:21:46 GMT
EXPOSE 4222 6222 8222
# Thu, 17 Nov 2022 20:21:46 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 17 Nov 2022 20:21:46 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 17 Nov 2022 20:21:47 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c8ce17c05ed27e7e08286a74c292d54eb2d5902af8f901dab4505ba83f7296f5`  
		Last Modified: Thu, 17 Nov 2022 20:22:33 GMT  
		Size: 4.9 MB (4918317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88c3d57c92f61ccff2db59e857c959bc11ca2ed1a6ca7f5494aa479c513196f7`  
		Last Modified: Thu, 17 Nov 2022 20:22:32 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:9e5158db138340db27aef59e820bafe7a09359e8910c2cef451b58348dd329ff
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4683160 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b5c60a8afd73cd47b032a2d66e4968bf12f1aed52fee0f708cf184ef6c09b960`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 17 Nov 2022 20:49:48 GMT
COPY file:75f2ce97960bd08a17d41dd00b0f977ff54641b0f3d5b35f613c50553a59e8e1 in /nats-server 
# Thu, 17 Nov 2022 20:49:48 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 17 Nov 2022 20:49:49 GMT
EXPOSE 4222 6222 8222
# Thu, 17 Nov 2022 20:49:49 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 17 Nov 2022 20:49:49 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 17 Nov 2022 20:49:49 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:e27c576ee7d0df355bb5ab346016b3a399e8048fe3f938263b3b77e343d9243f`  
		Last Modified: Thu, 17 Nov 2022 20:51:22 GMT  
		Size: 4.7 MB (4682651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:788fb9f41d9d2c69e1f5737db95b3d0e754d24cd75bdd8d94a80166b8c97d6b6`  
		Last Modified: Thu, 17 Nov 2022 20:51:21 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:e4c874e4f9f5eafa49bdd7fed9a022da8958f69cc70e245af8bb9ebf7cad0c0c
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4679780 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2bc64213c48245d6c2d479e5be4d5043a6d811cb9d273ae36c8dfa157accbd04`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 17 Nov 2022 20:58:06 GMT
COPY file:ebca823a5dac00609e9fb9733528840572067b84b58dcccbe67a2df698f2869e in /nats-server 
# Thu, 17 Nov 2022 20:58:06 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 17 Nov 2022 20:58:06 GMT
EXPOSE 4222 6222 8222
# Thu, 17 Nov 2022 20:58:06 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 17 Nov 2022 20:58:06 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 17 Nov 2022 20:58:06 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:2c415cfba68b644bd88b057d832ff5015af29e04439812f5bd2e6873b3d7b8fd`  
		Last Modified: Thu, 17 Nov 2022 20:59:39 GMT  
		Size: 4.7 MB (4679272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:875032eeefdff15b8e0c04ffba01805fa83a04cad983b8322b99f53b04e9c1fe`  
		Last Modified: Thu, 17 Nov 2022 20:59:38 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:6d5eefe444c9be5d4f08fd3ccf8277d186014689ef84ea0f59c59dc11acb4904
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4504058 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7ac0ab188af08ab1a9c049a3f6c349d0d2df9595cee8e6626c19a913526dcb2`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 17 Nov 2022 20:40:45 GMT
COPY file:d11c7b340550df0716193331cacb3d06f2cb3b9971e90e006a9c153aaadc50f8 in /nats-server 
# Thu, 17 Nov 2022 20:40:45 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 17 Nov 2022 20:40:45 GMT
EXPOSE 4222 6222 8222
# Thu, 17 Nov 2022 20:40:45 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 17 Nov 2022 20:40:45 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 17 Nov 2022 20:40:45 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:d3e01af3796e331721cc924f0d95499739cea560e1ac4bac35c11176033c94c8`  
		Last Modified: Thu, 17 Nov 2022 20:41:30 GMT  
		Size: 4.5 MB (4503550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e0b7a277e0d621acb2a17025b4318262de852c8be74070453c2f8c9983601ad`  
		Last Modified: Thu, 17 Nov 2022 20:41:30 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:windowsservercore`

```console
$ docker pull nats@sha256:a2a17b6c8e185249db8f657d5b4b5473e4627feb0a7ea39ac121544d7ab11465
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3650; amd64

### `nats:windowsservercore` - windows version 10.0.17763.3650; amd64

```console
$ docker pull nats@sha256:d42d0b0ee29bdd7b0ea24be91fb754a64a3da2ab070ed93e185e983132b9beec
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2784314848 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a836a477662568b8b4f2cd2ba8211273a6ae351f51fd48d29015400f42f395c`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 05 Nov 2022 18:29:26 GMT
RUN Install update 10.0.17763.3650
# Wed, 09 Nov 2022 14:50:58 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Nov 2022 16:44:45 GMT
ENV NATS_DOCKERIZED=1
# Thu, 17 Nov 2022 20:15:26 GMT
ENV NATS_SERVER=2.9.7
# Thu, 17 Nov 2022 20:15:27 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.9.7/nats-server-v2.9.7-windows-amd64.zip
# Thu, 17 Nov 2022 20:15:28 GMT
ENV NATS_SERVER_SHASUM=f1baa1646b7a499d035ebfd529644c1379988ab69703a090f9899c97067cea02
# Thu, 17 Nov 2022 20:17:00 GMT
RUN Set-PSDebug -Trace 2
# Thu, 17 Nov 2022 20:18:59 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Thu, 17 Nov 2022 20:19:00 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Thu, 17 Nov 2022 20:19:01 GMT
EXPOSE 4222 6222 8222
# Thu, 17 Nov 2022 20:19:02 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 17 Nov 2022 20:19:03 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a48a3e4ae2de839d8e99bde16eb91d113fb2cf889bba472d0c4274851b5fb402`  
		Last Modified: Tue, 21 Jun 2022 18:30:17 GMT  
		Size: 1.9 GB (1924269350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c26cc6e4f9eb1ae415a5ead6f884cac597bbd57efa6cd042c878d5b54c9d2091`  
		Last Modified: Tue, 08 Nov 2022 19:44:35 GMT  
		Size: 854.3 MB (854317461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99941fb33972e616b231a8aadd93463fdfd5de6aece4aa6c470d2feec31839be`  
		Last Modified: Wed, 09 Nov 2022 16:48:23 GMT  
		Size: 1.3 KB (1335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0f3d8a87f0a1540850986ff94131286dfa42ca116f04779e02f60b3a724641b`  
		Last Modified: Wed, 09 Nov 2022 16:48:23 GMT  
		Size: 1.3 KB (1327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69b8ead5903ee0014b1d59597e3e42c54eb9ad338e077477176b04d22ab4f291`  
		Last Modified: Thu, 17 Nov 2022 20:19:56 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd5112842b491d9aed12c373a680aa352fda7856f4dd7ae100240cda81004d10`  
		Last Modified: Thu, 17 Nov 2022 20:19:56 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27e8ac611281af798a4d5c0f0ffeca3542a44a865688ca95c3f963d0f3a2b009`  
		Last Modified: Thu, 17 Nov 2022 20:19:56 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ced45d282af98e490deb218ae7d77ad9ee20038016ea5fad600ab6363d4339fd`  
		Last Modified: Thu, 17 Nov 2022 20:19:56 GMT  
		Size: 381.6 KB (381592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d244e04b249f9171046dc315cd9c7d70aadbaa6496d85f41de583773d750a76b`  
		Last Modified: Thu, 17 Nov 2022 20:19:55 GMT  
		Size: 5.3 MB (5333250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e9dc3cf2f9c57dc6d24c7b6d3a526d97d4c7ef1de724d54dae9ad10211ba0e1`  
		Last Modified: Thu, 17 Nov 2022 20:19:54 GMT  
		Size: 2.0 KB (2001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6e0bb8f7d2e8165a51f2f77c4ee12feb907b21e4a5f2fe8c6215e6ee1c3b075`  
		Last Modified: Thu, 17 Nov 2022 20:19:54 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80326cc866c490bc13a4ead203b6b1af79320652c34f6605511671f003980078`  
		Last Modified: Thu, 17 Nov 2022 20:19:54 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7785e4126ef3eb2bac999118a556a59d9ab9474c8175a5742b4a1c7fba660efe`  
		Last Modified: Thu, 17 Nov 2022 20:19:54 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:windowsservercore-1809`

```console
$ docker pull nats@sha256:a2a17b6c8e185249db8f657d5b4b5473e4627feb0a7ea39ac121544d7ab11465
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3650; amd64

### `nats:windowsservercore-1809` - windows version 10.0.17763.3650; amd64

```console
$ docker pull nats@sha256:d42d0b0ee29bdd7b0ea24be91fb754a64a3da2ab070ed93e185e983132b9beec
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2784314848 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a836a477662568b8b4f2cd2ba8211273a6ae351f51fd48d29015400f42f395c`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 05 Nov 2022 18:29:26 GMT
RUN Install update 10.0.17763.3650
# Wed, 09 Nov 2022 14:50:58 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Nov 2022 16:44:45 GMT
ENV NATS_DOCKERIZED=1
# Thu, 17 Nov 2022 20:15:26 GMT
ENV NATS_SERVER=2.9.7
# Thu, 17 Nov 2022 20:15:27 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.9.7/nats-server-v2.9.7-windows-amd64.zip
# Thu, 17 Nov 2022 20:15:28 GMT
ENV NATS_SERVER_SHASUM=f1baa1646b7a499d035ebfd529644c1379988ab69703a090f9899c97067cea02
# Thu, 17 Nov 2022 20:17:00 GMT
RUN Set-PSDebug -Trace 2
# Thu, 17 Nov 2022 20:18:59 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Thu, 17 Nov 2022 20:19:00 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Thu, 17 Nov 2022 20:19:01 GMT
EXPOSE 4222 6222 8222
# Thu, 17 Nov 2022 20:19:02 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 17 Nov 2022 20:19:03 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a48a3e4ae2de839d8e99bde16eb91d113fb2cf889bba472d0c4274851b5fb402`  
		Last Modified: Tue, 21 Jun 2022 18:30:17 GMT  
		Size: 1.9 GB (1924269350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c26cc6e4f9eb1ae415a5ead6f884cac597bbd57efa6cd042c878d5b54c9d2091`  
		Last Modified: Tue, 08 Nov 2022 19:44:35 GMT  
		Size: 854.3 MB (854317461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99941fb33972e616b231a8aadd93463fdfd5de6aece4aa6c470d2feec31839be`  
		Last Modified: Wed, 09 Nov 2022 16:48:23 GMT  
		Size: 1.3 KB (1335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0f3d8a87f0a1540850986ff94131286dfa42ca116f04779e02f60b3a724641b`  
		Last Modified: Wed, 09 Nov 2022 16:48:23 GMT  
		Size: 1.3 KB (1327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69b8ead5903ee0014b1d59597e3e42c54eb9ad338e077477176b04d22ab4f291`  
		Last Modified: Thu, 17 Nov 2022 20:19:56 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd5112842b491d9aed12c373a680aa352fda7856f4dd7ae100240cda81004d10`  
		Last Modified: Thu, 17 Nov 2022 20:19:56 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27e8ac611281af798a4d5c0f0ffeca3542a44a865688ca95c3f963d0f3a2b009`  
		Last Modified: Thu, 17 Nov 2022 20:19:56 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ced45d282af98e490deb218ae7d77ad9ee20038016ea5fad600ab6363d4339fd`  
		Last Modified: Thu, 17 Nov 2022 20:19:56 GMT  
		Size: 381.6 KB (381592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d244e04b249f9171046dc315cd9c7d70aadbaa6496d85f41de583773d750a76b`  
		Last Modified: Thu, 17 Nov 2022 20:19:55 GMT  
		Size: 5.3 MB (5333250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e9dc3cf2f9c57dc6d24c7b6d3a526d97d4c7ef1de724d54dae9ad10211ba0e1`  
		Last Modified: Thu, 17 Nov 2022 20:19:54 GMT  
		Size: 2.0 KB (2001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6e0bb8f7d2e8165a51f2f77c4ee12feb907b21e4a5f2fe8c6215e6ee1c3b075`  
		Last Modified: Thu, 17 Nov 2022 20:19:54 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80326cc866c490bc13a4ead203b6b1af79320652c34f6605511671f003980078`  
		Last Modified: Thu, 17 Nov 2022 20:19:54 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7785e4126ef3eb2bac999118a556a59d9ab9474c8175a5742b4a1c7fba660efe`  
		Last Modified: Thu, 17 Nov 2022 20:19:54 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
