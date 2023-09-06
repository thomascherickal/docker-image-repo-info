<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `nats`

-	[`nats:2`](#nats2)
-	[`nats:2-alpine`](#nats2-alpine)
-	[`nats:2-alpine3.18`](#nats2-alpine318)
-	[`nats:2-linux`](#nats2-linux)
-	[`nats:2-nanoserver`](#nats2-nanoserver)
-	[`nats:2-nanoserver-1809`](#nats2-nanoserver-1809)
-	[`nats:2-scratch`](#nats2-scratch)
-	[`nats:2-windowsservercore`](#nats2-windowsservercore)
-	[`nats:2-windowsservercore-1809`](#nats2-windowsservercore-1809)
-	[`nats:2.9`](#nats29)
-	[`nats:2.9-alpine`](#nats29-alpine)
-	[`nats:2.9-alpine3.18`](#nats29-alpine318)
-	[`nats:2.9-linux`](#nats29-linux)
-	[`nats:2.9-nanoserver`](#nats29-nanoserver)
-	[`nats:2.9-nanoserver-1809`](#nats29-nanoserver-1809)
-	[`nats:2.9-scratch`](#nats29-scratch)
-	[`nats:2.9-windowsservercore`](#nats29-windowsservercore)
-	[`nats:2.9-windowsservercore-1809`](#nats29-windowsservercore-1809)
-	[`nats:2.9.22`](#nats2922)
-	[`nats:2.9.22-alpine`](#nats2922-alpine)
-	[`nats:2.9.22-alpine3.18`](#nats2922-alpine318)
-	[`nats:2.9.22-linux`](#nats2922-linux)
-	[`nats:2.9.22-nanoserver`](#nats2922-nanoserver)
-	[`nats:2.9.22-nanoserver-1809`](#nats2922-nanoserver-1809)
-	[`nats:2.9.22-scratch`](#nats2922-scratch)
-	[`nats:2.9.22-windowsservercore`](#nats2922-windowsservercore)
-	[`nats:2.9.22-windowsservercore-1809`](#nats2922-windowsservercore-1809)
-	[`nats:alpine`](#natsalpine)
-	[`nats:alpine3.18`](#natsalpine318)
-	[`nats:latest`](#natslatest)
-	[`nats:linux`](#natslinux)
-	[`nats:nanoserver`](#natsnanoserver)
-	[`nats:nanoserver-1809`](#natsnanoserver-1809)
-	[`nats:scratch`](#natsscratch)
-	[`nats:windowsservercore`](#natswindowsservercore)
-	[`nats:windowsservercore-1809`](#natswindowsservercore-1809)

## `nats:2`

```console
$ docker pull nats@sha256:70a536ddc540ab27ecf4ea6666bf495473a11f408d17bb694008fec41f3c4e87
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.4737; amd64

### `nats:2` - linux; amd64

```console
$ docker pull nats@sha256:841691cd373d85dfef90326ad2625e6498d8472d68d7d64b9a7d11b566729e77
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5245280 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7bfd417bdbd2f1eb2b6798d0a0fbba5ce7e3bd1d7ce50d29b8965cb174e801ed`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 06 Sep 2023 23:20:12 GMT
COPY file:acdb0e47969d6e334bcadb9c85dfef3166c764ff4ac55254185a04b1a6e8bbee in /nats-server 
# Wed, 06 Sep 2023 23:20:12 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 06 Sep 2023 23:20:12 GMT
EXPOSE 4222 6222 8222
# Wed, 06 Sep 2023 23:20:12 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 06 Sep 2023 23:20:12 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 06 Sep 2023 23:20:12 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:aac801db9a2a97942dde4494f98ce2d08c529a3af03ecb92f0b93426bbfd6419`  
		Last Modified: Wed, 06 Sep 2023 23:20:56 GMT  
		Size: 5.2 MB (5244773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f86dbe6523f83ad4a9d3f35c66bb097fad7505a3bd4de2123ea173ea21f1e38`  
		Last Modified: Wed, 06 Sep 2023 23:20:55 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - linux; arm variant v6

```console
$ docker pull nats@sha256:ec9d67b684f4605aa5fd2b86b64953bb8062a49d2916cf8e5fab437de945df15
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (4980015 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d632b911d90b9fc8ad6e2d0fd53012e9c8cc6ca17c685d2c8c2a6c4de2cb2c45`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 06 Sep 2023 23:04:49 GMT
COPY file:51aacaba9769a3f16e0467be1fc8eb86122f6f3496e89e41b61e0038083ae308 in /nats-server 
# Wed, 06 Sep 2023 23:04:49 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 06 Sep 2023 23:04:49 GMT
EXPOSE 4222 6222 8222
# Wed, 06 Sep 2023 23:04:49 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 06 Sep 2023 23:04:49 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 06 Sep 2023 23:04:50 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6a6e165fccf6da77ad3b09408162fc7daaafe266b71dd5da8679594aa110a3a5`  
		Last Modified: Wed, 06 Sep 2023 23:05:32 GMT  
		Size: 5.0 MB (4979506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1baf063892d372757ae2be4c42843e0a096826874b64519c230fd85bd65e69e8`  
		Last Modified: Wed, 06 Sep 2023 23:05:31 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - linux; arm variant v7

```console
$ docker pull nats@sha256:58dfaa80e9889d01819641e707279821d96d6f5eb7ce87e29eaa38cd4e0b5cac
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (4970850 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a2d43ddba67d73d9d9c8f19b9fbec53ca1bcb7f04349363538f7d08fd069dbd2`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 06 Sep 2023 22:57:45 GMT
COPY file:aae670bb79c659968f632ae3be388af62614010873ced2a439475906dbb769c6 in /nats-server 
# Wed, 06 Sep 2023 22:57:45 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 06 Sep 2023 22:57:45 GMT
EXPOSE 4222 6222 8222
# Wed, 06 Sep 2023 22:57:45 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 06 Sep 2023 22:57:46 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 06 Sep 2023 22:57:46 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:55b6dbad6639da13368cebb9688e8a5caaee29041e6b5e2e798201dfcf2b67ad`  
		Last Modified: Wed, 06 Sep 2023 22:58:23 GMT  
		Size: 5.0 MB (4970341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f17c52d1a9dd756c463e0590216b217bfee91f63c66217c407f1c98b1ebbc3b9`  
		Last Modified: Wed, 06 Sep 2023 22:58:22 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:dd48788f80e3925791e0dddfa44348b7df9022fbc914b20cf00e051a0b3adbf3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.8 MB (4778848 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0e35fd1c4293b595f11452fdc3e7dd6d5d9e033ecc9b1e6a35ff40577f2cba9f`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 06 Sep 2023 22:40:07 GMT
COPY file:d6eca5c67de65d1a8a30a51ea7318b044949c77108b2fdccc5aa0054c068c196 in /nats-server 
# Wed, 06 Sep 2023 22:40:07 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 06 Sep 2023 22:40:07 GMT
EXPOSE 4222 6222 8222
# Wed, 06 Sep 2023 22:40:08 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 06 Sep 2023 22:40:08 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 06 Sep 2023 22:40:08 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:88e5ff7f26ea25c6d2ab092989d9372cb32b3e60880124facfcefd7d3f0b7591`  
		Last Modified: Wed, 06 Sep 2023 22:40:49 GMT  
		Size: 4.8 MB (4778340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7795fd345dfb406d659c2502b733417a10ee85274263050ee36ab4aa021a38d9`  
		Last Modified: Wed, 06 Sep 2023 22:40:48 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - windows version 10.0.17763.4737; amd64

```console
$ docker pull nats@sha256:baec10f85f099b828313ff821f20b005907591e2f4fb414c7a240b5944f1292a
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.8 MB (109785996 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3654d1c2e7ef6e2297c519fd991a4a49b4d9928375a1142ec2af9cc55358ee84`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 02 Aug 2023 08:33:47 GMT
RUN Apply image 10.0.17763.4737
# Thu, 10 Aug 2023 02:34:52 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 06 Sep 2023 23:17:32 GMT
RUN cmd /S /C #(nop) COPY file:393d7e944d1b6697a14f19f6cb9673d95da4e1a0fc9508b238325e94beebc857 in C:\nats-server.exe 
# Wed, 06 Sep 2023 23:17:33 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 06 Sep 2023 23:17:34 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 06 Sep 2023 23:17:34 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 06 Sep 2023 23:17:35 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:86fab75eb466cadf89d853682179b3b57eba9fe28c78041dd52bced81e18a627`  
		Last Modified: Tue, 08 Aug 2023 17:55:54 GMT  
		Size: 104.5 MB (104459386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c43534c571f8fdc71038e0f4b4c33a30adb0bbc8b292454d35930557ced33408`  
		Last Modified: Thu, 10 Aug 2023 02:35:37 GMT  
		Size: 1.2 KB (1167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3eade3f0d46f534a5d639c78b1e85a1b0ea96d271fe2c3e706142d2f8d0aef7`  
		Last Modified: Wed, 06 Sep 2023 23:18:18 GMT  
		Size: 5.3 MB (5320148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4eeab0b725b185bf02913419c636eb70964ad972b883ef43006bbf75b1320ece`  
		Last Modified: Wed, 06 Sep 2023 23:18:16 GMT  
		Size: 1.8 KB (1804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c11e5f8af7811e39cecedb8bc4f4533b8f362e497bfe37a943209e0ce0d0bd5`  
		Last Modified: Wed, 06 Sep 2023 23:18:16 GMT  
		Size: 1.2 KB (1161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50806fff52469c9a918b10aa2ed383885dd30e5763ab2157c5440e425ebdccd3`  
		Last Modified: Wed, 06 Sep 2023 23:18:16 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f8c118167fb4c0339d4078748da065ff698f06d9373f7acaa5c42db51dfcdff`  
		Last Modified: Wed, 06 Sep 2023 23:18:16 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-alpine`

```console
$ docker pull nats@sha256:36d34c59ed76472d9b3caafc5e3764b7a587498808efdd5178468f4efe8b4887
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-alpine` - linux; amd64

```console
$ docker pull nats@sha256:756a55661288407f688c52224ac8b12d008f0fec9343c68281b04bb59cbcc427
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.3 MB (9270382 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dbb9252d07acfbe3ac9083449c0fef74561021019d85c2993f5bce02c7a16201`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:20 GMT
ADD file:32ff5e7a78b890996ee4681cc0a26185d3e9acdb4eb1e2aaccb2411f922fed6b in / 
# Mon, 07 Aug 2023 19:20:20 GMT
CMD ["/bin/sh"]
# Wed, 06 Sep 2023 23:19:53 GMT
ENV NATS_SERVER=2.9.22
# Wed, 06 Sep 2023 23:19:55 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='811e5a3c8187d937a753f182bd5ae2035c91604bda11a3b11023e5eea0504c41' ;; 		armhf) natsArch='arm6'; sha256='4d6f2f8ee9faf43de9fed5b43a0a5db836ad81797146065777b06a59f90cf1b0' ;; 		armv7) natsArch='arm7'; sha256='b8c83cd825b05d8d0610fc9352804fe810ae6bd9d8f0d814a39b0f152ec2ba79' ;; 		x86_64) natsArch='amd64'; sha256='9550278e34e94aebd410ec401bc145d3538e430ec2a40d5213fffdf9fdd49c27' ;; 		x86) natsArch='386'; sha256='a8ccdd37eac64b031ea96762d7f72a74445e9a708c0363549ba7e119fa79e52c' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 06 Sep 2023 23:19:55 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 06 Sep 2023 23:19:55 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 06 Sep 2023 23:19:55 GMT
EXPOSE 4222 6222 8222
# Wed, 06 Sep 2023 23:19:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 06 Sep 2023 23:19:55 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:7264a8db6415046d36d16ba98b79778e18accee6ffa71850405994cffa9be7de`  
		Last Modified: Mon, 07 Aug 2023 19:20:54 GMT  
		Size: 3.4 MB (3401613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75fdd304ec17c2cf1f7629eefc922e04fae260b6d902e4fd42c81a5e5ce9d5dc`  
		Last Modified: Wed, 06 Sep 2023 23:20:32 GMT  
		Size: 5.9 MB (5867770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2863800c65f086f618bf3df0e7855997aea26ba27f4c759cf8bfae94da866bb`  
		Last Modified: Wed, 06 Sep 2023 23:20:31 GMT  
		Size: 585.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e32a641538132ed9885ca87c473fe9ff71415289c1f5276ba1157bb0760bd04`  
		Last Modified: Wed, 06 Sep 2023 23:20:31 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:e66fcde15a5b8028aed7cdd2e03392aa10c4a51c224e964f014eddc1c821433d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.7 MB (8749092 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6e3524e57732f8e26091d551f1b5ce64405e4217d19f047345dc28a29a1b847`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:49:14 GMT
ADD file:9882e99e5f94ab2db05c029648ac5be7cf0f063a8701394fcbb543a7ef5d4b90 in / 
# Mon, 07 Aug 2023 19:49:15 GMT
CMD ["/bin/sh"]
# Wed, 06 Sep 2023 23:04:40 GMT
ENV NATS_SERVER=2.9.22
# Wed, 06 Sep 2023 23:04:43 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='811e5a3c8187d937a753f182bd5ae2035c91604bda11a3b11023e5eea0504c41' ;; 		armhf) natsArch='arm6'; sha256='4d6f2f8ee9faf43de9fed5b43a0a5db836ad81797146065777b06a59f90cf1b0' ;; 		armv7) natsArch='arm7'; sha256='b8c83cd825b05d8d0610fc9352804fe810ae6bd9d8f0d814a39b0f152ec2ba79' ;; 		x86_64) natsArch='amd64'; sha256='9550278e34e94aebd410ec401bc145d3538e430ec2a40d5213fffdf9fdd49c27' ;; 		x86) natsArch='386'; sha256='a8ccdd37eac64b031ea96762d7f72a74445e9a708c0363549ba7e119fa79e52c' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 06 Sep 2023 23:04:43 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 06 Sep 2023 23:04:43 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 06 Sep 2023 23:04:43 GMT
EXPOSE 4222 6222 8222
# Wed, 06 Sep 2023 23:04:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 06 Sep 2023 23:04:43 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:af09961d4a43b504efc76e38b50918977c28be73eeb8b926247783a00e8b9f2f`  
		Last Modified: Mon, 07 Aug 2023 19:49:38 GMT  
		Size: 3.1 MB (3144809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5a6e71bd2ab60e313e659b569f8c33e5e9dcfdb580c25af0f9c5e7eca59f92f`  
		Last Modified: Wed, 06 Sep 2023 23:05:08 GMT  
		Size: 5.6 MB (5603285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7b94c778bbad17cc9be59c68102602e2e77462672d2e045f4713e80ce1cbb1c`  
		Last Modified: Wed, 06 Sep 2023 23:05:07 GMT  
		Size: 585.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4b258e6095309f7819e72dd444d848fe600fb2e73b5bd12bd1e9a556a17bf56`  
		Last Modified: Wed, 06 Sep 2023 23:05:07 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:9ca6685d1ad99fa588f9d4dc05ffe27569ed660b735218fd38795568fe508c73
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.5 MB (8492829 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0271598ef211f3df61073ff64c769275b4bb72b68b984931c8a7af1706fe80c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:57:25 GMT
ADD file:e3f56488d3d3bb67729714db13ddadf6652e7efb5281cfc7010d3e71f9d6607f in / 
# Mon, 07 Aug 2023 19:57:25 GMT
CMD ["/bin/sh"]
# Wed, 06 Sep 2023 22:57:29 GMT
ENV NATS_SERVER=2.9.22
# Wed, 06 Sep 2023 22:57:32 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='811e5a3c8187d937a753f182bd5ae2035c91604bda11a3b11023e5eea0504c41' ;; 		armhf) natsArch='arm6'; sha256='4d6f2f8ee9faf43de9fed5b43a0a5db836ad81797146065777b06a59f90cf1b0' ;; 		armv7) natsArch='arm7'; sha256='b8c83cd825b05d8d0610fc9352804fe810ae6bd9d8f0d814a39b0f152ec2ba79' ;; 		x86_64) natsArch='amd64'; sha256='9550278e34e94aebd410ec401bc145d3538e430ec2a40d5213fffdf9fdd49c27' ;; 		x86) natsArch='386'; sha256='a8ccdd37eac64b031ea96762d7f72a74445e9a708c0363549ba7e119fa79e52c' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 06 Sep 2023 22:57:32 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 06 Sep 2023 22:57:32 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 06 Sep 2023 22:57:32 GMT
EXPOSE 4222 6222 8222
# Wed, 06 Sep 2023 22:57:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 06 Sep 2023 22:57:32 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:f8dec92eec42224ef9e6ca9c6207ea6b9195dcf93d06bd5ceff0f814b62bf064`  
		Last Modified: Mon, 07 Aug 2023 19:57:55 GMT  
		Size: 2.9 MB (2899480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1962026ec365b08ba406dd0e38e57c06dcd04f2225faffcc17883ed87716cdc8`  
		Last Modified: Wed, 06 Sep 2023 22:58:03 GMT  
		Size: 5.6 MB (5592351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:578cf75378460664df525d3b5d1412e778f7b8cdc5f3c31207b3bbc2f6c074f5`  
		Last Modified: Wed, 06 Sep 2023 22:58:01 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64bf3e24d68a6cadd0880ce3163738934bf8e5b267923da68dd6922cd6b98a31`  
		Last Modified: Wed, 06 Sep 2023 22:58:01 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:51e884da4e764cc784998e4bc69bbbefa4f39420be30021b4a1074dc40604423
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.7 MB (8734219 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c8cdff0ce493eb27f871f27f7ec452d1c36de63801fda0b331cd41067f858b9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:19 GMT
ADD file:b2e7eaa7e41f08853dbe08d84439a7f9fd32fc58c3aa1e298f3f60343b2b683a in / 
# Mon, 07 Aug 2023 19:39:19 GMT
CMD ["/bin/sh"]
# Wed, 06 Sep 2023 22:39:45 GMT
ENV NATS_SERVER=2.9.22
# Wed, 06 Sep 2023 22:39:47 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='811e5a3c8187d937a753f182bd5ae2035c91604bda11a3b11023e5eea0504c41' ;; 		armhf) natsArch='arm6'; sha256='4d6f2f8ee9faf43de9fed5b43a0a5db836ad81797146065777b06a59f90cf1b0' ;; 		armv7) natsArch='arm7'; sha256='b8c83cd825b05d8d0610fc9352804fe810ae6bd9d8f0d814a39b0f152ec2ba79' ;; 		x86_64) natsArch='amd64'; sha256='9550278e34e94aebd410ec401bc145d3538e430ec2a40d5213fffdf9fdd49c27' ;; 		x86) natsArch='386'; sha256='a8ccdd37eac64b031ea96762d7f72a74445e9a708c0363549ba7e119fa79e52c' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 06 Sep 2023 22:39:47 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 06 Sep 2023 22:39:47 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 06 Sep 2023 22:39:47 GMT
EXPOSE 4222 6222 8222
# Wed, 06 Sep 2023 22:39:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 06 Sep 2023 22:39:48 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9fda8d8052c61740409c4bea888859c141fd8cc3f58ac61943144ff6d1681b2d`  
		Last Modified: Mon, 07 Aug 2023 19:39:45 GMT  
		Size: 3.3 MB (3330767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64353667b2ee68f04c527f8dcef72789d979435b90c5b8073485e6c2fcc5c3f7`  
		Last Modified: Wed, 06 Sep 2023 22:40:28 GMT  
		Size: 5.4 MB (5402455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:540b41e481b61500ce8ed1c72cc5c0f937cabb489d0ba9de2dc2dad279696a28`  
		Last Modified: Wed, 06 Sep 2023 22:40:27 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb56160de8c01873d42326860132a0b877e470be0ff76c774c04b542515c9e4a`  
		Last Modified: Wed, 06 Sep 2023 22:40:27 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-alpine3.18`

```console
$ docker pull nats@sha256:36d34c59ed76472d9b3caafc5e3764b7a587498808efdd5178468f4efe8b4887
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-alpine3.18` - linux; amd64

```console
$ docker pull nats@sha256:756a55661288407f688c52224ac8b12d008f0fec9343c68281b04bb59cbcc427
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.3 MB (9270382 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dbb9252d07acfbe3ac9083449c0fef74561021019d85c2993f5bce02c7a16201`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:20 GMT
ADD file:32ff5e7a78b890996ee4681cc0a26185d3e9acdb4eb1e2aaccb2411f922fed6b in / 
# Mon, 07 Aug 2023 19:20:20 GMT
CMD ["/bin/sh"]
# Wed, 06 Sep 2023 23:19:53 GMT
ENV NATS_SERVER=2.9.22
# Wed, 06 Sep 2023 23:19:55 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='811e5a3c8187d937a753f182bd5ae2035c91604bda11a3b11023e5eea0504c41' ;; 		armhf) natsArch='arm6'; sha256='4d6f2f8ee9faf43de9fed5b43a0a5db836ad81797146065777b06a59f90cf1b0' ;; 		armv7) natsArch='arm7'; sha256='b8c83cd825b05d8d0610fc9352804fe810ae6bd9d8f0d814a39b0f152ec2ba79' ;; 		x86_64) natsArch='amd64'; sha256='9550278e34e94aebd410ec401bc145d3538e430ec2a40d5213fffdf9fdd49c27' ;; 		x86) natsArch='386'; sha256='a8ccdd37eac64b031ea96762d7f72a74445e9a708c0363549ba7e119fa79e52c' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 06 Sep 2023 23:19:55 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 06 Sep 2023 23:19:55 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 06 Sep 2023 23:19:55 GMT
EXPOSE 4222 6222 8222
# Wed, 06 Sep 2023 23:19:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 06 Sep 2023 23:19:55 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:7264a8db6415046d36d16ba98b79778e18accee6ffa71850405994cffa9be7de`  
		Last Modified: Mon, 07 Aug 2023 19:20:54 GMT  
		Size: 3.4 MB (3401613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75fdd304ec17c2cf1f7629eefc922e04fae260b6d902e4fd42c81a5e5ce9d5dc`  
		Last Modified: Wed, 06 Sep 2023 23:20:32 GMT  
		Size: 5.9 MB (5867770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2863800c65f086f618bf3df0e7855997aea26ba27f4c759cf8bfae94da866bb`  
		Last Modified: Wed, 06 Sep 2023 23:20:31 GMT  
		Size: 585.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e32a641538132ed9885ca87c473fe9ff71415289c1f5276ba1157bb0760bd04`  
		Last Modified: Wed, 06 Sep 2023 23:20:31 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.18` - linux; arm variant v6

```console
$ docker pull nats@sha256:e66fcde15a5b8028aed7cdd2e03392aa10c4a51c224e964f014eddc1c821433d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.7 MB (8749092 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6e3524e57732f8e26091d551f1b5ce64405e4217d19f047345dc28a29a1b847`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:49:14 GMT
ADD file:9882e99e5f94ab2db05c029648ac5be7cf0f063a8701394fcbb543a7ef5d4b90 in / 
# Mon, 07 Aug 2023 19:49:15 GMT
CMD ["/bin/sh"]
# Wed, 06 Sep 2023 23:04:40 GMT
ENV NATS_SERVER=2.9.22
# Wed, 06 Sep 2023 23:04:43 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='811e5a3c8187d937a753f182bd5ae2035c91604bda11a3b11023e5eea0504c41' ;; 		armhf) natsArch='arm6'; sha256='4d6f2f8ee9faf43de9fed5b43a0a5db836ad81797146065777b06a59f90cf1b0' ;; 		armv7) natsArch='arm7'; sha256='b8c83cd825b05d8d0610fc9352804fe810ae6bd9d8f0d814a39b0f152ec2ba79' ;; 		x86_64) natsArch='amd64'; sha256='9550278e34e94aebd410ec401bc145d3538e430ec2a40d5213fffdf9fdd49c27' ;; 		x86) natsArch='386'; sha256='a8ccdd37eac64b031ea96762d7f72a74445e9a708c0363549ba7e119fa79e52c' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 06 Sep 2023 23:04:43 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 06 Sep 2023 23:04:43 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 06 Sep 2023 23:04:43 GMT
EXPOSE 4222 6222 8222
# Wed, 06 Sep 2023 23:04:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 06 Sep 2023 23:04:43 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:af09961d4a43b504efc76e38b50918977c28be73eeb8b926247783a00e8b9f2f`  
		Last Modified: Mon, 07 Aug 2023 19:49:38 GMT  
		Size: 3.1 MB (3144809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5a6e71bd2ab60e313e659b569f8c33e5e9dcfdb580c25af0f9c5e7eca59f92f`  
		Last Modified: Wed, 06 Sep 2023 23:05:08 GMT  
		Size: 5.6 MB (5603285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7b94c778bbad17cc9be59c68102602e2e77462672d2e045f4713e80ce1cbb1c`  
		Last Modified: Wed, 06 Sep 2023 23:05:07 GMT  
		Size: 585.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4b258e6095309f7819e72dd444d848fe600fb2e73b5bd12bd1e9a556a17bf56`  
		Last Modified: Wed, 06 Sep 2023 23:05:07 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.18` - linux; arm variant v7

```console
$ docker pull nats@sha256:9ca6685d1ad99fa588f9d4dc05ffe27569ed660b735218fd38795568fe508c73
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.5 MB (8492829 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0271598ef211f3df61073ff64c769275b4bb72b68b984931c8a7af1706fe80c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:57:25 GMT
ADD file:e3f56488d3d3bb67729714db13ddadf6652e7efb5281cfc7010d3e71f9d6607f in / 
# Mon, 07 Aug 2023 19:57:25 GMT
CMD ["/bin/sh"]
# Wed, 06 Sep 2023 22:57:29 GMT
ENV NATS_SERVER=2.9.22
# Wed, 06 Sep 2023 22:57:32 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='811e5a3c8187d937a753f182bd5ae2035c91604bda11a3b11023e5eea0504c41' ;; 		armhf) natsArch='arm6'; sha256='4d6f2f8ee9faf43de9fed5b43a0a5db836ad81797146065777b06a59f90cf1b0' ;; 		armv7) natsArch='arm7'; sha256='b8c83cd825b05d8d0610fc9352804fe810ae6bd9d8f0d814a39b0f152ec2ba79' ;; 		x86_64) natsArch='amd64'; sha256='9550278e34e94aebd410ec401bc145d3538e430ec2a40d5213fffdf9fdd49c27' ;; 		x86) natsArch='386'; sha256='a8ccdd37eac64b031ea96762d7f72a74445e9a708c0363549ba7e119fa79e52c' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 06 Sep 2023 22:57:32 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 06 Sep 2023 22:57:32 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 06 Sep 2023 22:57:32 GMT
EXPOSE 4222 6222 8222
# Wed, 06 Sep 2023 22:57:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 06 Sep 2023 22:57:32 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:f8dec92eec42224ef9e6ca9c6207ea6b9195dcf93d06bd5ceff0f814b62bf064`  
		Last Modified: Mon, 07 Aug 2023 19:57:55 GMT  
		Size: 2.9 MB (2899480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1962026ec365b08ba406dd0e38e57c06dcd04f2225faffcc17883ed87716cdc8`  
		Last Modified: Wed, 06 Sep 2023 22:58:03 GMT  
		Size: 5.6 MB (5592351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:578cf75378460664df525d3b5d1412e778f7b8cdc5f3c31207b3bbc2f6c074f5`  
		Last Modified: Wed, 06 Sep 2023 22:58:01 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64bf3e24d68a6cadd0880ce3163738934bf8e5b267923da68dd6922cd6b98a31`  
		Last Modified: Wed, 06 Sep 2023 22:58:01 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.18` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:51e884da4e764cc784998e4bc69bbbefa4f39420be30021b4a1074dc40604423
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.7 MB (8734219 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c8cdff0ce493eb27f871f27f7ec452d1c36de63801fda0b331cd41067f858b9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:19 GMT
ADD file:b2e7eaa7e41f08853dbe08d84439a7f9fd32fc58c3aa1e298f3f60343b2b683a in / 
# Mon, 07 Aug 2023 19:39:19 GMT
CMD ["/bin/sh"]
# Wed, 06 Sep 2023 22:39:45 GMT
ENV NATS_SERVER=2.9.22
# Wed, 06 Sep 2023 22:39:47 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='811e5a3c8187d937a753f182bd5ae2035c91604bda11a3b11023e5eea0504c41' ;; 		armhf) natsArch='arm6'; sha256='4d6f2f8ee9faf43de9fed5b43a0a5db836ad81797146065777b06a59f90cf1b0' ;; 		armv7) natsArch='arm7'; sha256='b8c83cd825b05d8d0610fc9352804fe810ae6bd9d8f0d814a39b0f152ec2ba79' ;; 		x86_64) natsArch='amd64'; sha256='9550278e34e94aebd410ec401bc145d3538e430ec2a40d5213fffdf9fdd49c27' ;; 		x86) natsArch='386'; sha256='a8ccdd37eac64b031ea96762d7f72a74445e9a708c0363549ba7e119fa79e52c' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 06 Sep 2023 22:39:47 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 06 Sep 2023 22:39:47 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 06 Sep 2023 22:39:47 GMT
EXPOSE 4222 6222 8222
# Wed, 06 Sep 2023 22:39:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 06 Sep 2023 22:39:48 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9fda8d8052c61740409c4bea888859c141fd8cc3f58ac61943144ff6d1681b2d`  
		Last Modified: Mon, 07 Aug 2023 19:39:45 GMT  
		Size: 3.3 MB (3330767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64353667b2ee68f04c527f8dcef72789d979435b90c5b8073485e6c2fcc5c3f7`  
		Last Modified: Wed, 06 Sep 2023 22:40:28 GMT  
		Size: 5.4 MB (5402455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:540b41e481b61500ce8ed1c72cc5c0f937cabb489d0ba9de2dc2dad279696a28`  
		Last Modified: Wed, 06 Sep 2023 22:40:27 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb56160de8c01873d42326860132a0b877e470be0ff76c774c04b542515c9e4a`  
		Last Modified: Wed, 06 Sep 2023 22:40:27 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-linux`

```console
$ docker pull nats@sha256:7595e8b87b7063f28ffd3a1f0f7021f6c333fcc17377dbecccd7a6777df7754a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-linux` - linux; amd64

```console
$ docker pull nats@sha256:841691cd373d85dfef90326ad2625e6498d8472d68d7d64b9a7d11b566729e77
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5245280 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7bfd417bdbd2f1eb2b6798d0a0fbba5ce7e3bd1d7ce50d29b8965cb174e801ed`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 06 Sep 2023 23:20:12 GMT
COPY file:acdb0e47969d6e334bcadb9c85dfef3166c764ff4ac55254185a04b1a6e8bbee in /nats-server 
# Wed, 06 Sep 2023 23:20:12 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 06 Sep 2023 23:20:12 GMT
EXPOSE 4222 6222 8222
# Wed, 06 Sep 2023 23:20:12 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 06 Sep 2023 23:20:12 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 06 Sep 2023 23:20:12 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:aac801db9a2a97942dde4494f98ce2d08c529a3af03ecb92f0b93426bbfd6419`  
		Last Modified: Wed, 06 Sep 2023 23:20:56 GMT  
		Size: 5.2 MB (5244773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f86dbe6523f83ad4a9d3f35c66bb097fad7505a3bd4de2123ea173ea21f1e38`  
		Last Modified: Wed, 06 Sep 2023 23:20:55 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:ec9d67b684f4605aa5fd2b86b64953bb8062a49d2916cf8e5fab437de945df15
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (4980015 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d632b911d90b9fc8ad6e2d0fd53012e9c8cc6ca17c685d2c8c2a6c4de2cb2c45`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 06 Sep 2023 23:04:49 GMT
COPY file:51aacaba9769a3f16e0467be1fc8eb86122f6f3496e89e41b61e0038083ae308 in /nats-server 
# Wed, 06 Sep 2023 23:04:49 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 06 Sep 2023 23:04:49 GMT
EXPOSE 4222 6222 8222
# Wed, 06 Sep 2023 23:04:49 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 06 Sep 2023 23:04:49 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 06 Sep 2023 23:04:50 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6a6e165fccf6da77ad3b09408162fc7daaafe266b71dd5da8679594aa110a3a5`  
		Last Modified: Wed, 06 Sep 2023 23:05:32 GMT  
		Size: 5.0 MB (4979506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1baf063892d372757ae2be4c42843e0a096826874b64519c230fd85bd65e69e8`  
		Last Modified: Wed, 06 Sep 2023 23:05:31 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:58dfaa80e9889d01819641e707279821d96d6f5eb7ce87e29eaa38cd4e0b5cac
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (4970850 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a2d43ddba67d73d9d9c8f19b9fbec53ca1bcb7f04349363538f7d08fd069dbd2`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 06 Sep 2023 22:57:45 GMT
COPY file:aae670bb79c659968f632ae3be388af62614010873ced2a439475906dbb769c6 in /nats-server 
# Wed, 06 Sep 2023 22:57:45 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 06 Sep 2023 22:57:45 GMT
EXPOSE 4222 6222 8222
# Wed, 06 Sep 2023 22:57:45 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 06 Sep 2023 22:57:46 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 06 Sep 2023 22:57:46 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:55b6dbad6639da13368cebb9688e8a5caaee29041e6b5e2e798201dfcf2b67ad`  
		Last Modified: Wed, 06 Sep 2023 22:58:23 GMT  
		Size: 5.0 MB (4970341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f17c52d1a9dd756c463e0590216b217bfee91f63c66217c407f1c98b1ebbc3b9`  
		Last Modified: Wed, 06 Sep 2023 22:58:22 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:dd48788f80e3925791e0dddfa44348b7df9022fbc914b20cf00e051a0b3adbf3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.8 MB (4778848 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0e35fd1c4293b595f11452fdc3e7dd6d5d9e033ecc9b1e6a35ff40577f2cba9f`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 06 Sep 2023 22:40:07 GMT
COPY file:d6eca5c67de65d1a8a30a51ea7318b044949c77108b2fdccc5aa0054c068c196 in /nats-server 
# Wed, 06 Sep 2023 22:40:07 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 06 Sep 2023 22:40:07 GMT
EXPOSE 4222 6222 8222
# Wed, 06 Sep 2023 22:40:08 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 06 Sep 2023 22:40:08 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 06 Sep 2023 22:40:08 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:88e5ff7f26ea25c6d2ab092989d9372cb32b3e60880124facfcefd7d3f0b7591`  
		Last Modified: Wed, 06 Sep 2023 22:40:49 GMT  
		Size: 4.8 MB (4778340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7795fd345dfb406d659c2502b733417a10ee85274263050ee36ab4aa021a38d9`  
		Last Modified: Wed, 06 Sep 2023 22:40:48 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-nanoserver`

```console
$ docker pull nats@sha256:347c71d5b7499fda4c79d015de6e2b9da4a28374147b6901e02f8e135e482bd1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4737; amd64

### `nats:2-nanoserver` - windows version 10.0.17763.4737; amd64

```console
$ docker pull nats@sha256:baec10f85f099b828313ff821f20b005907591e2f4fb414c7a240b5944f1292a
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.8 MB (109785996 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3654d1c2e7ef6e2297c519fd991a4a49b4d9928375a1142ec2af9cc55358ee84`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 02 Aug 2023 08:33:47 GMT
RUN Apply image 10.0.17763.4737
# Thu, 10 Aug 2023 02:34:52 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 06 Sep 2023 23:17:32 GMT
RUN cmd /S /C #(nop) COPY file:393d7e944d1b6697a14f19f6cb9673d95da4e1a0fc9508b238325e94beebc857 in C:\nats-server.exe 
# Wed, 06 Sep 2023 23:17:33 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 06 Sep 2023 23:17:34 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 06 Sep 2023 23:17:34 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 06 Sep 2023 23:17:35 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:86fab75eb466cadf89d853682179b3b57eba9fe28c78041dd52bced81e18a627`  
		Last Modified: Tue, 08 Aug 2023 17:55:54 GMT  
		Size: 104.5 MB (104459386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c43534c571f8fdc71038e0f4b4c33a30adb0bbc8b292454d35930557ced33408`  
		Last Modified: Thu, 10 Aug 2023 02:35:37 GMT  
		Size: 1.2 KB (1167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3eade3f0d46f534a5d639c78b1e85a1b0ea96d271fe2c3e706142d2f8d0aef7`  
		Last Modified: Wed, 06 Sep 2023 23:18:18 GMT  
		Size: 5.3 MB (5320148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4eeab0b725b185bf02913419c636eb70964ad972b883ef43006bbf75b1320ece`  
		Last Modified: Wed, 06 Sep 2023 23:18:16 GMT  
		Size: 1.8 KB (1804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c11e5f8af7811e39cecedb8bc4f4533b8f362e497bfe37a943209e0ce0d0bd5`  
		Last Modified: Wed, 06 Sep 2023 23:18:16 GMT  
		Size: 1.2 KB (1161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50806fff52469c9a918b10aa2ed383885dd30e5763ab2157c5440e425ebdccd3`  
		Last Modified: Wed, 06 Sep 2023 23:18:16 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f8c118167fb4c0339d4078748da065ff698f06d9373f7acaa5c42db51dfcdff`  
		Last Modified: Wed, 06 Sep 2023 23:18:16 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-nanoserver-1809`

```console
$ docker pull nats@sha256:347c71d5b7499fda4c79d015de6e2b9da4a28374147b6901e02f8e135e482bd1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4737; amd64

### `nats:2-nanoserver-1809` - windows version 10.0.17763.4737; amd64

```console
$ docker pull nats@sha256:baec10f85f099b828313ff821f20b005907591e2f4fb414c7a240b5944f1292a
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.8 MB (109785996 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3654d1c2e7ef6e2297c519fd991a4a49b4d9928375a1142ec2af9cc55358ee84`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 02 Aug 2023 08:33:47 GMT
RUN Apply image 10.0.17763.4737
# Thu, 10 Aug 2023 02:34:52 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 06 Sep 2023 23:17:32 GMT
RUN cmd /S /C #(nop) COPY file:393d7e944d1b6697a14f19f6cb9673d95da4e1a0fc9508b238325e94beebc857 in C:\nats-server.exe 
# Wed, 06 Sep 2023 23:17:33 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 06 Sep 2023 23:17:34 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 06 Sep 2023 23:17:34 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 06 Sep 2023 23:17:35 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:86fab75eb466cadf89d853682179b3b57eba9fe28c78041dd52bced81e18a627`  
		Last Modified: Tue, 08 Aug 2023 17:55:54 GMT  
		Size: 104.5 MB (104459386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c43534c571f8fdc71038e0f4b4c33a30adb0bbc8b292454d35930557ced33408`  
		Last Modified: Thu, 10 Aug 2023 02:35:37 GMT  
		Size: 1.2 KB (1167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3eade3f0d46f534a5d639c78b1e85a1b0ea96d271fe2c3e706142d2f8d0aef7`  
		Last Modified: Wed, 06 Sep 2023 23:18:18 GMT  
		Size: 5.3 MB (5320148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4eeab0b725b185bf02913419c636eb70964ad972b883ef43006bbf75b1320ece`  
		Last Modified: Wed, 06 Sep 2023 23:18:16 GMT  
		Size: 1.8 KB (1804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c11e5f8af7811e39cecedb8bc4f4533b8f362e497bfe37a943209e0ce0d0bd5`  
		Last Modified: Wed, 06 Sep 2023 23:18:16 GMT  
		Size: 1.2 KB (1161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50806fff52469c9a918b10aa2ed383885dd30e5763ab2157c5440e425ebdccd3`  
		Last Modified: Wed, 06 Sep 2023 23:18:16 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f8c118167fb4c0339d4078748da065ff698f06d9373f7acaa5c42db51dfcdff`  
		Last Modified: Wed, 06 Sep 2023 23:18:16 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-scratch`

```console
$ docker pull nats@sha256:7595e8b87b7063f28ffd3a1f0f7021f6c333fcc17377dbecccd7a6777df7754a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-scratch` - linux; amd64

```console
$ docker pull nats@sha256:841691cd373d85dfef90326ad2625e6498d8472d68d7d64b9a7d11b566729e77
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5245280 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7bfd417bdbd2f1eb2b6798d0a0fbba5ce7e3bd1d7ce50d29b8965cb174e801ed`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 06 Sep 2023 23:20:12 GMT
COPY file:acdb0e47969d6e334bcadb9c85dfef3166c764ff4ac55254185a04b1a6e8bbee in /nats-server 
# Wed, 06 Sep 2023 23:20:12 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 06 Sep 2023 23:20:12 GMT
EXPOSE 4222 6222 8222
# Wed, 06 Sep 2023 23:20:12 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 06 Sep 2023 23:20:12 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 06 Sep 2023 23:20:12 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:aac801db9a2a97942dde4494f98ce2d08c529a3af03ecb92f0b93426bbfd6419`  
		Last Modified: Wed, 06 Sep 2023 23:20:56 GMT  
		Size: 5.2 MB (5244773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f86dbe6523f83ad4a9d3f35c66bb097fad7505a3bd4de2123ea173ea21f1e38`  
		Last Modified: Wed, 06 Sep 2023 23:20:55 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:ec9d67b684f4605aa5fd2b86b64953bb8062a49d2916cf8e5fab437de945df15
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (4980015 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d632b911d90b9fc8ad6e2d0fd53012e9c8cc6ca17c685d2c8c2a6c4de2cb2c45`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 06 Sep 2023 23:04:49 GMT
COPY file:51aacaba9769a3f16e0467be1fc8eb86122f6f3496e89e41b61e0038083ae308 in /nats-server 
# Wed, 06 Sep 2023 23:04:49 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 06 Sep 2023 23:04:49 GMT
EXPOSE 4222 6222 8222
# Wed, 06 Sep 2023 23:04:49 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 06 Sep 2023 23:04:49 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 06 Sep 2023 23:04:50 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6a6e165fccf6da77ad3b09408162fc7daaafe266b71dd5da8679594aa110a3a5`  
		Last Modified: Wed, 06 Sep 2023 23:05:32 GMT  
		Size: 5.0 MB (4979506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1baf063892d372757ae2be4c42843e0a096826874b64519c230fd85bd65e69e8`  
		Last Modified: Wed, 06 Sep 2023 23:05:31 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:58dfaa80e9889d01819641e707279821d96d6f5eb7ce87e29eaa38cd4e0b5cac
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (4970850 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a2d43ddba67d73d9d9c8f19b9fbec53ca1bcb7f04349363538f7d08fd069dbd2`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 06 Sep 2023 22:57:45 GMT
COPY file:aae670bb79c659968f632ae3be388af62614010873ced2a439475906dbb769c6 in /nats-server 
# Wed, 06 Sep 2023 22:57:45 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 06 Sep 2023 22:57:45 GMT
EXPOSE 4222 6222 8222
# Wed, 06 Sep 2023 22:57:45 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 06 Sep 2023 22:57:46 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 06 Sep 2023 22:57:46 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:55b6dbad6639da13368cebb9688e8a5caaee29041e6b5e2e798201dfcf2b67ad`  
		Last Modified: Wed, 06 Sep 2023 22:58:23 GMT  
		Size: 5.0 MB (4970341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f17c52d1a9dd756c463e0590216b217bfee91f63c66217c407f1c98b1ebbc3b9`  
		Last Modified: Wed, 06 Sep 2023 22:58:22 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:dd48788f80e3925791e0dddfa44348b7df9022fbc914b20cf00e051a0b3adbf3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.8 MB (4778848 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0e35fd1c4293b595f11452fdc3e7dd6d5d9e033ecc9b1e6a35ff40577f2cba9f`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 06 Sep 2023 22:40:07 GMT
COPY file:d6eca5c67de65d1a8a30a51ea7318b044949c77108b2fdccc5aa0054c068c196 in /nats-server 
# Wed, 06 Sep 2023 22:40:07 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 06 Sep 2023 22:40:07 GMT
EXPOSE 4222 6222 8222
# Wed, 06 Sep 2023 22:40:08 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 06 Sep 2023 22:40:08 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 06 Sep 2023 22:40:08 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:88e5ff7f26ea25c6d2ab092989d9372cb32b3e60880124facfcefd7d3f0b7591`  
		Last Modified: Wed, 06 Sep 2023 22:40:49 GMT  
		Size: 4.8 MB (4778340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7795fd345dfb406d659c2502b733417a10ee85274263050ee36ab4aa021a38d9`  
		Last Modified: Wed, 06 Sep 2023 22:40:48 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-windowsservercore`

```console
$ docker pull nats@sha256:df25045f4d70165b54b8b7b0ae443fd21450261550bbc1b314adf8a58053e707
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4737; amd64

### `nats:2-windowsservercore` - windows version 10.0.17763.4737; amd64

```console
$ docker pull nats@sha256:e2f9912126f4753a9e9312b5dd77a5c5e44c257f28d04ad55cef0662d24138a2
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2001990927 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3cf5f23a9d8d2eca784896bbd09d5e163b27485e7b392cd0bd92f88502dd57b7`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Wed, 02 Aug 2023 09:07:15 GMT
RUN Install update 10.0.17763.4737
# Thu, 10 Aug 2023 01:11:08 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Thu, 10 Aug 2023 02:32:08 GMT
ENV NATS_DOCKERIZED=1
# Wed, 06 Sep 2023 23:15:04 GMT
ENV NATS_SERVER=2.9.22
# Wed, 06 Sep 2023 23:15:05 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.9.22/nats-server-v2.9.22-windows-amd64.zip
# Wed, 06 Sep 2023 23:15:06 GMT
ENV NATS_SERVER_SHASUM=e91db73b02bd4dca3eb7a4bf32e29763450b08d593f73e87d0a6b70102dea0d4
# Wed, 06 Sep 2023 23:15:56 GMT
RUN Set-PSDebug -Trace 2
# Wed, 06 Sep 2023 23:17:21 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 06 Sep 2023 23:17:22 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 06 Sep 2023 23:17:23 GMT
EXPOSE 4222 6222 8222
# Wed, 06 Sep 2023 23:17:24 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 06 Sep 2023 23:17:24 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b95f433aa7d90194e65f6b08a599b3ee12292e124d47c204107baedfd71054c1`  
		Last Modified: Tue, 08 Aug 2023 18:31:16 GMT  
		Size: 345.3 MB (345334986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c5180b8f5f7c2303ba89717cfa778a2173921ca7efdc058cfd6ed951c6d5ca3`  
		Last Modified: Thu, 10 Aug 2023 01:57:18 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fed0c598ca0ae763bd83f045a0c9262bf153a47e508b736992d196e2fb47dea`  
		Last Modified: Thu, 10 Aug 2023 02:35:22 GMT  
		Size: 1.4 KB (1449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab0ebc9f46983ba56ff415cd7b99891210ab8eaad5adf4a15a8f2021de4ebdfd`  
		Last Modified: Wed, 06 Sep 2023 23:18:02 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1c4a22897bb4d3fa0ef4fff463ef850ad45e21404737f120c724fb472c77221`  
		Last Modified: Wed, 06 Sep 2023 23:18:02 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c30142424ff3f45c3c8923f1aa5d959879239599fdde6aba1101c39a168abe48`  
		Last Modified: Wed, 06 Sep 2023 23:18:02 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3723e4e864a2d241c8133b4f1c569ac4ac140d29fe8e216ecd140ebd0e2531cd`  
		Last Modified: Wed, 06 Sep 2023 23:18:02 GMT  
		Size: 242.5 KB (242470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae4c6899207e83d648ab5bf60620507d438b612cb42961f5b8b300c25fde01dd`  
		Last Modified: Wed, 06 Sep 2023 23:18:02 GMT  
		Size: 5.8 MB (5779810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bc2f6a7b18656a6539013442aa6e8c88b49fddce30025ad67ba6e4867a2860b`  
		Last Modified: Wed, 06 Sep 2023 23:18:00 GMT  
		Size: 2.0 KB (1976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ac72b596159b34e1de106133f926192bb5daac9b62301a55822162e6656b6cc`  
		Last Modified: Wed, 06 Sep 2023 23:18:00 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a11a75f33304f42224c3b832462b4497699310fd70a6cdfb322bd126be44cb32`  
		Last Modified: Wed, 06 Sep 2023 23:18:00 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c01b20cb00adae2b356c4377b9419f6a1d18d74692e89c0ee1e66d7b55ca3f3`  
		Last Modified: Wed, 06 Sep 2023 23:18:00 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-windowsservercore-1809`

```console
$ docker pull nats@sha256:df25045f4d70165b54b8b7b0ae443fd21450261550bbc1b314adf8a58053e707
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4737; amd64

### `nats:2-windowsservercore-1809` - windows version 10.0.17763.4737; amd64

```console
$ docker pull nats@sha256:e2f9912126f4753a9e9312b5dd77a5c5e44c257f28d04ad55cef0662d24138a2
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2001990927 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3cf5f23a9d8d2eca784896bbd09d5e163b27485e7b392cd0bd92f88502dd57b7`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Wed, 02 Aug 2023 09:07:15 GMT
RUN Install update 10.0.17763.4737
# Thu, 10 Aug 2023 01:11:08 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Thu, 10 Aug 2023 02:32:08 GMT
ENV NATS_DOCKERIZED=1
# Wed, 06 Sep 2023 23:15:04 GMT
ENV NATS_SERVER=2.9.22
# Wed, 06 Sep 2023 23:15:05 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.9.22/nats-server-v2.9.22-windows-amd64.zip
# Wed, 06 Sep 2023 23:15:06 GMT
ENV NATS_SERVER_SHASUM=e91db73b02bd4dca3eb7a4bf32e29763450b08d593f73e87d0a6b70102dea0d4
# Wed, 06 Sep 2023 23:15:56 GMT
RUN Set-PSDebug -Trace 2
# Wed, 06 Sep 2023 23:17:21 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 06 Sep 2023 23:17:22 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 06 Sep 2023 23:17:23 GMT
EXPOSE 4222 6222 8222
# Wed, 06 Sep 2023 23:17:24 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 06 Sep 2023 23:17:24 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b95f433aa7d90194e65f6b08a599b3ee12292e124d47c204107baedfd71054c1`  
		Last Modified: Tue, 08 Aug 2023 18:31:16 GMT  
		Size: 345.3 MB (345334986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c5180b8f5f7c2303ba89717cfa778a2173921ca7efdc058cfd6ed951c6d5ca3`  
		Last Modified: Thu, 10 Aug 2023 01:57:18 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fed0c598ca0ae763bd83f045a0c9262bf153a47e508b736992d196e2fb47dea`  
		Last Modified: Thu, 10 Aug 2023 02:35:22 GMT  
		Size: 1.4 KB (1449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab0ebc9f46983ba56ff415cd7b99891210ab8eaad5adf4a15a8f2021de4ebdfd`  
		Last Modified: Wed, 06 Sep 2023 23:18:02 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1c4a22897bb4d3fa0ef4fff463ef850ad45e21404737f120c724fb472c77221`  
		Last Modified: Wed, 06 Sep 2023 23:18:02 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c30142424ff3f45c3c8923f1aa5d959879239599fdde6aba1101c39a168abe48`  
		Last Modified: Wed, 06 Sep 2023 23:18:02 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3723e4e864a2d241c8133b4f1c569ac4ac140d29fe8e216ecd140ebd0e2531cd`  
		Last Modified: Wed, 06 Sep 2023 23:18:02 GMT  
		Size: 242.5 KB (242470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae4c6899207e83d648ab5bf60620507d438b612cb42961f5b8b300c25fde01dd`  
		Last Modified: Wed, 06 Sep 2023 23:18:02 GMT  
		Size: 5.8 MB (5779810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bc2f6a7b18656a6539013442aa6e8c88b49fddce30025ad67ba6e4867a2860b`  
		Last Modified: Wed, 06 Sep 2023 23:18:00 GMT  
		Size: 2.0 KB (1976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ac72b596159b34e1de106133f926192bb5daac9b62301a55822162e6656b6cc`  
		Last Modified: Wed, 06 Sep 2023 23:18:00 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a11a75f33304f42224c3b832462b4497699310fd70a6cdfb322bd126be44cb32`  
		Last Modified: Wed, 06 Sep 2023 23:18:00 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c01b20cb00adae2b356c4377b9419f6a1d18d74692e89c0ee1e66d7b55ca3f3`  
		Last Modified: Wed, 06 Sep 2023 23:18:00 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9`

```console
$ docker pull nats@sha256:70a536ddc540ab27ecf4ea6666bf495473a11f408d17bb694008fec41f3c4e87
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.4737; amd64

### `nats:2.9` - linux; amd64

```console
$ docker pull nats@sha256:841691cd373d85dfef90326ad2625e6498d8472d68d7d64b9a7d11b566729e77
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5245280 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7bfd417bdbd2f1eb2b6798d0a0fbba5ce7e3bd1d7ce50d29b8965cb174e801ed`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 06 Sep 2023 23:20:12 GMT
COPY file:acdb0e47969d6e334bcadb9c85dfef3166c764ff4ac55254185a04b1a6e8bbee in /nats-server 
# Wed, 06 Sep 2023 23:20:12 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 06 Sep 2023 23:20:12 GMT
EXPOSE 4222 6222 8222
# Wed, 06 Sep 2023 23:20:12 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 06 Sep 2023 23:20:12 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 06 Sep 2023 23:20:12 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:aac801db9a2a97942dde4494f98ce2d08c529a3af03ecb92f0b93426bbfd6419`  
		Last Modified: Wed, 06 Sep 2023 23:20:56 GMT  
		Size: 5.2 MB (5244773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f86dbe6523f83ad4a9d3f35c66bb097fad7505a3bd4de2123ea173ea21f1e38`  
		Last Modified: Wed, 06 Sep 2023 23:20:55 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9` - linux; arm variant v6

```console
$ docker pull nats@sha256:ec9d67b684f4605aa5fd2b86b64953bb8062a49d2916cf8e5fab437de945df15
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (4980015 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d632b911d90b9fc8ad6e2d0fd53012e9c8cc6ca17c685d2c8c2a6c4de2cb2c45`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 06 Sep 2023 23:04:49 GMT
COPY file:51aacaba9769a3f16e0467be1fc8eb86122f6f3496e89e41b61e0038083ae308 in /nats-server 
# Wed, 06 Sep 2023 23:04:49 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 06 Sep 2023 23:04:49 GMT
EXPOSE 4222 6222 8222
# Wed, 06 Sep 2023 23:04:49 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 06 Sep 2023 23:04:49 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 06 Sep 2023 23:04:50 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6a6e165fccf6da77ad3b09408162fc7daaafe266b71dd5da8679594aa110a3a5`  
		Last Modified: Wed, 06 Sep 2023 23:05:32 GMT  
		Size: 5.0 MB (4979506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1baf063892d372757ae2be4c42843e0a096826874b64519c230fd85bd65e69e8`  
		Last Modified: Wed, 06 Sep 2023 23:05:31 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9` - linux; arm variant v7

```console
$ docker pull nats@sha256:58dfaa80e9889d01819641e707279821d96d6f5eb7ce87e29eaa38cd4e0b5cac
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (4970850 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a2d43ddba67d73d9d9c8f19b9fbec53ca1bcb7f04349363538f7d08fd069dbd2`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 06 Sep 2023 22:57:45 GMT
COPY file:aae670bb79c659968f632ae3be388af62614010873ced2a439475906dbb769c6 in /nats-server 
# Wed, 06 Sep 2023 22:57:45 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 06 Sep 2023 22:57:45 GMT
EXPOSE 4222 6222 8222
# Wed, 06 Sep 2023 22:57:45 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 06 Sep 2023 22:57:46 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 06 Sep 2023 22:57:46 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:55b6dbad6639da13368cebb9688e8a5caaee29041e6b5e2e798201dfcf2b67ad`  
		Last Modified: Wed, 06 Sep 2023 22:58:23 GMT  
		Size: 5.0 MB (4970341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f17c52d1a9dd756c463e0590216b217bfee91f63c66217c407f1c98b1ebbc3b9`  
		Last Modified: Wed, 06 Sep 2023 22:58:22 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:dd48788f80e3925791e0dddfa44348b7df9022fbc914b20cf00e051a0b3adbf3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.8 MB (4778848 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0e35fd1c4293b595f11452fdc3e7dd6d5d9e033ecc9b1e6a35ff40577f2cba9f`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 06 Sep 2023 22:40:07 GMT
COPY file:d6eca5c67de65d1a8a30a51ea7318b044949c77108b2fdccc5aa0054c068c196 in /nats-server 
# Wed, 06 Sep 2023 22:40:07 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 06 Sep 2023 22:40:07 GMT
EXPOSE 4222 6222 8222
# Wed, 06 Sep 2023 22:40:08 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 06 Sep 2023 22:40:08 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 06 Sep 2023 22:40:08 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:88e5ff7f26ea25c6d2ab092989d9372cb32b3e60880124facfcefd7d3f0b7591`  
		Last Modified: Wed, 06 Sep 2023 22:40:49 GMT  
		Size: 4.8 MB (4778340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7795fd345dfb406d659c2502b733417a10ee85274263050ee36ab4aa021a38d9`  
		Last Modified: Wed, 06 Sep 2023 22:40:48 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9` - windows version 10.0.17763.4737; amd64

```console
$ docker pull nats@sha256:baec10f85f099b828313ff821f20b005907591e2f4fb414c7a240b5944f1292a
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.8 MB (109785996 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3654d1c2e7ef6e2297c519fd991a4a49b4d9928375a1142ec2af9cc55358ee84`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 02 Aug 2023 08:33:47 GMT
RUN Apply image 10.0.17763.4737
# Thu, 10 Aug 2023 02:34:52 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 06 Sep 2023 23:17:32 GMT
RUN cmd /S /C #(nop) COPY file:393d7e944d1b6697a14f19f6cb9673d95da4e1a0fc9508b238325e94beebc857 in C:\nats-server.exe 
# Wed, 06 Sep 2023 23:17:33 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 06 Sep 2023 23:17:34 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 06 Sep 2023 23:17:34 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 06 Sep 2023 23:17:35 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:86fab75eb466cadf89d853682179b3b57eba9fe28c78041dd52bced81e18a627`  
		Last Modified: Tue, 08 Aug 2023 17:55:54 GMT  
		Size: 104.5 MB (104459386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c43534c571f8fdc71038e0f4b4c33a30adb0bbc8b292454d35930557ced33408`  
		Last Modified: Thu, 10 Aug 2023 02:35:37 GMT  
		Size: 1.2 KB (1167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3eade3f0d46f534a5d639c78b1e85a1b0ea96d271fe2c3e706142d2f8d0aef7`  
		Last Modified: Wed, 06 Sep 2023 23:18:18 GMT  
		Size: 5.3 MB (5320148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4eeab0b725b185bf02913419c636eb70964ad972b883ef43006bbf75b1320ece`  
		Last Modified: Wed, 06 Sep 2023 23:18:16 GMT  
		Size: 1.8 KB (1804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c11e5f8af7811e39cecedb8bc4f4533b8f362e497bfe37a943209e0ce0d0bd5`  
		Last Modified: Wed, 06 Sep 2023 23:18:16 GMT  
		Size: 1.2 KB (1161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50806fff52469c9a918b10aa2ed383885dd30e5763ab2157c5440e425ebdccd3`  
		Last Modified: Wed, 06 Sep 2023 23:18:16 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f8c118167fb4c0339d4078748da065ff698f06d9373f7acaa5c42db51dfcdff`  
		Last Modified: Wed, 06 Sep 2023 23:18:16 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-alpine`

```console
$ docker pull nats@sha256:36d34c59ed76472d9b3caafc5e3764b7a587498808efdd5178468f4efe8b4887
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9-alpine` - linux; amd64

```console
$ docker pull nats@sha256:756a55661288407f688c52224ac8b12d008f0fec9343c68281b04bb59cbcc427
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.3 MB (9270382 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dbb9252d07acfbe3ac9083449c0fef74561021019d85c2993f5bce02c7a16201`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:20 GMT
ADD file:32ff5e7a78b890996ee4681cc0a26185d3e9acdb4eb1e2aaccb2411f922fed6b in / 
# Mon, 07 Aug 2023 19:20:20 GMT
CMD ["/bin/sh"]
# Wed, 06 Sep 2023 23:19:53 GMT
ENV NATS_SERVER=2.9.22
# Wed, 06 Sep 2023 23:19:55 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='811e5a3c8187d937a753f182bd5ae2035c91604bda11a3b11023e5eea0504c41' ;; 		armhf) natsArch='arm6'; sha256='4d6f2f8ee9faf43de9fed5b43a0a5db836ad81797146065777b06a59f90cf1b0' ;; 		armv7) natsArch='arm7'; sha256='b8c83cd825b05d8d0610fc9352804fe810ae6bd9d8f0d814a39b0f152ec2ba79' ;; 		x86_64) natsArch='amd64'; sha256='9550278e34e94aebd410ec401bc145d3538e430ec2a40d5213fffdf9fdd49c27' ;; 		x86) natsArch='386'; sha256='a8ccdd37eac64b031ea96762d7f72a74445e9a708c0363549ba7e119fa79e52c' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 06 Sep 2023 23:19:55 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 06 Sep 2023 23:19:55 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 06 Sep 2023 23:19:55 GMT
EXPOSE 4222 6222 8222
# Wed, 06 Sep 2023 23:19:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 06 Sep 2023 23:19:55 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:7264a8db6415046d36d16ba98b79778e18accee6ffa71850405994cffa9be7de`  
		Last Modified: Mon, 07 Aug 2023 19:20:54 GMT  
		Size: 3.4 MB (3401613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75fdd304ec17c2cf1f7629eefc922e04fae260b6d902e4fd42c81a5e5ce9d5dc`  
		Last Modified: Wed, 06 Sep 2023 23:20:32 GMT  
		Size: 5.9 MB (5867770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2863800c65f086f618bf3df0e7855997aea26ba27f4c759cf8bfae94da866bb`  
		Last Modified: Wed, 06 Sep 2023 23:20:31 GMT  
		Size: 585.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e32a641538132ed9885ca87c473fe9ff71415289c1f5276ba1157bb0760bd04`  
		Last Modified: Wed, 06 Sep 2023 23:20:31 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:e66fcde15a5b8028aed7cdd2e03392aa10c4a51c224e964f014eddc1c821433d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.7 MB (8749092 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6e3524e57732f8e26091d551f1b5ce64405e4217d19f047345dc28a29a1b847`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:49:14 GMT
ADD file:9882e99e5f94ab2db05c029648ac5be7cf0f063a8701394fcbb543a7ef5d4b90 in / 
# Mon, 07 Aug 2023 19:49:15 GMT
CMD ["/bin/sh"]
# Wed, 06 Sep 2023 23:04:40 GMT
ENV NATS_SERVER=2.9.22
# Wed, 06 Sep 2023 23:04:43 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='811e5a3c8187d937a753f182bd5ae2035c91604bda11a3b11023e5eea0504c41' ;; 		armhf) natsArch='arm6'; sha256='4d6f2f8ee9faf43de9fed5b43a0a5db836ad81797146065777b06a59f90cf1b0' ;; 		armv7) natsArch='arm7'; sha256='b8c83cd825b05d8d0610fc9352804fe810ae6bd9d8f0d814a39b0f152ec2ba79' ;; 		x86_64) natsArch='amd64'; sha256='9550278e34e94aebd410ec401bc145d3538e430ec2a40d5213fffdf9fdd49c27' ;; 		x86) natsArch='386'; sha256='a8ccdd37eac64b031ea96762d7f72a74445e9a708c0363549ba7e119fa79e52c' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 06 Sep 2023 23:04:43 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 06 Sep 2023 23:04:43 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 06 Sep 2023 23:04:43 GMT
EXPOSE 4222 6222 8222
# Wed, 06 Sep 2023 23:04:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 06 Sep 2023 23:04:43 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:af09961d4a43b504efc76e38b50918977c28be73eeb8b926247783a00e8b9f2f`  
		Last Modified: Mon, 07 Aug 2023 19:49:38 GMT  
		Size: 3.1 MB (3144809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5a6e71bd2ab60e313e659b569f8c33e5e9dcfdb580c25af0f9c5e7eca59f92f`  
		Last Modified: Wed, 06 Sep 2023 23:05:08 GMT  
		Size: 5.6 MB (5603285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7b94c778bbad17cc9be59c68102602e2e77462672d2e045f4713e80ce1cbb1c`  
		Last Modified: Wed, 06 Sep 2023 23:05:07 GMT  
		Size: 585.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4b258e6095309f7819e72dd444d848fe600fb2e73b5bd12bd1e9a556a17bf56`  
		Last Modified: Wed, 06 Sep 2023 23:05:07 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:9ca6685d1ad99fa588f9d4dc05ffe27569ed660b735218fd38795568fe508c73
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.5 MB (8492829 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0271598ef211f3df61073ff64c769275b4bb72b68b984931c8a7af1706fe80c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:57:25 GMT
ADD file:e3f56488d3d3bb67729714db13ddadf6652e7efb5281cfc7010d3e71f9d6607f in / 
# Mon, 07 Aug 2023 19:57:25 GMT
CMD ["/bin/sh"]
# Wed, 06 Sep 2023 22:57:29 GMT
ENV NATS_SERVER=2.9.22
# Wed, 06 Sep 2023 22:57:32 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='811e5a3c8187d937a753f182bd5ae2035c91604bda11a3b11023e5eea0504c41' ;; 		armhf) natsArch='arm6'; sha256='4d6f2f8ee9faf43de9fed5b43a0a5db836ad81797146065777b06a59f90cf1b0' ;; 		armv7) natsArch='arm7'; sha256='b8c83cd825b05d8d0610fc9352804fe810ae6bd9d8f0d814a39b0f152ec2ba79' ;; 		x86_64) natsArch='amd64'; sha256='9550278e34e94aebd410ec401bc145d3538e430ec2a40d5213fffdf9fdd49c27' ;; 		x86) natsArch='386'; sha256='a8ccdd37eac64b031ea96762d7f72a74445e9a708c0363549ba7e119fa79e52c' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 06 Sep 2023 22:57:32 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 06 Sep 2023 22:57:32 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 06 Sep 2023 22:57:32 GMT
EXPOSE 4222 6222 8222
# Wed, 06 Sep 2023 22:57:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 06 Sep 2023 22:57:32 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:f8dec92eec42224ef9e6ca9c6207ea6b9195dcf93d06bd5ceff0f814b62bf064`  
		Last Modified: Mon, 07 Aug 2023 19:57:55 GMT  
		Size: 2.9 MB (2899480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1962026ec365b08ba406dd0e38e57c06dcd04f2225faffcc17883ed87716cdc8`  
		Last Modified: Wed, 06 Sep 2023 22:58:03 GMT  
		Size: 5.6 MB (5592351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:578cf75378460664df525d3b5d1412e778f7b8cdc5f3c31207b3bbc2f6c074f5`  
		Last Modified: Wed, 06 Sep 2023 22:58:01 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64bf3e24d68a6cadd0880ce3163738934bf8e5b267923da68dd6922cd6b98a31`  
		Last Modified: Wed, 06 Sep 2023 22:58:01 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:51e884da4e764cc784998e4bc69bbbefa4f39420be30021b4a1074dc40604423
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.7 MB (8734219 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c8cdff0ce493eb27f871f27f7ec452d1c36de63801fda0b331cd41067f858b9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:19 GMT
ADD file:b2e7eaa7e41f08853dbe08d84439a7f9fd32fc58c3aa1e298f3f60343b2b683a in / 
# Mon, 07 Aug 2023 19:39:19 GMT
CMD ["/bin/sh"]
# Wed, 06 Sep 2023 22:39:45 GMT
ENV NATS_SERVER=2.9.22
# Wed, 06 Sep 2023 22:39:47 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='811e5a3c8187d937a753f182bd5ae2035c91604bda11a3b11023e5eea0504c41' ;; 		armhf) natsArch='arm6'; sha256='4d6f2f8ee9faf43de9fed5b43a0a5db836ad81797146065777b06a59f90cf1b0' ;; 		armv7) natsArch='arm7'; sha256='b8c83cd825b05d8d0610fc9352804fe810ae6bd9d8f0d814a39b0f152ec2ba79' ;; 		x86_64) natsArch='amd64'; sha256='9550278e34e94aebd410ec401bc145d3538e430ec2a40d5213fffdf9fdd49c27' ;; 		x86) natsArch='386'; sha256='a8ccdd37eac64b031ea96762d7f72a74445e9a708c0363549ba7e119fa79e52c' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 06 Sep 2023 22:39:47 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 06 Sep 2023 22:39:47 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 06 Sep 2023 22:39:47 GMT
EXPOSE 4222 6222 8222
# Wed, 06 Sep 2023 22:39:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 06 Sep 2023 22:39:48 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9fda8d8052c61740409c4bea888859c141fd8cc3f58ac61943144ff6d1681b2d`  
		Last Modified: Mon, 07 Aug 2023 19:39:45 GMT  
		Size: 3.3 MB (3330767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64353667b2ee68f04c527f8dcef72789d979435b90c5b8073485e6c2fcc5c3f7`  
		Last Modified: Wed, 06 Sep 2023 22:40:28 GMT  
		Size: 5.4 MB (5402455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:540b41e481b61500ce8ed1c72cc5c0f937cabb489d0ba9de2dc2dad279696a28`  
		Last Modified: Wed, 06 Sep 2023 22:40:27 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb56160de8c01873d42326860132a0b877e470be0ff76c774c04b542515c9e4a`  
		Last Modified: Wed, 06 Sep 2023 22:40:27 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-alpine3.18`

```console
$ docker pull nats@sha256:36d34c59ed76472d9b3caafc5e3764b7a587498808efdd5178468f4efe8b4887
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9-alpine3.18` - linux; amd64

```console
$ docker pull nats@sha256:756a55661288407f688c52224ac8b12d008f0fec9343c68281b04bb59cbcc427
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.3 MB (9270382 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dbb9252d07acfbe3ac9083449c0fef74561021019d85c2993f5bce02c7a16201`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:20 GMT
ADD file:32ff5e7a78b890996ee4681cc0a26185d3e9acdb4eb1e2aaccb2411f922fed6b in / 
# Mon, 07 Aug 2023 19:20:20 GMT
CMD ["/bin/sh"]
# Wed, 06 Sep 2023 23:19:53 GMT
ENV NATS_SERVER=2.9.22
# Wed, 06 Sep 2023 23:19:55 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='811e5a3c8187d937a753f182bd5ae2035c91604bda11a3b11023e5eea0504c41' ;; 		armhf) natsArch='arm6'; sha256='4d6f2f8ee9faf43de9fed5b43a0a5db836ad81797146065777b06a59f90cf1b0' ;; 		armv7) natsArch='arm7'; sha256='b8c83cd825b05d8d0610fc9352804fe810ae6bd9d8f0d814a39b0f152ec2ba79' ;; 		x86_64) natsArch='amd64'; sha256='9550278e34e94aebd410ec401bc145d3538e430ec2a40d5213fffdf9fdd49c27' ;; 		x86) natsArch='386'; sha256='a8ccdd37eac64b031ea96762d7f72a74445e9a708c0363549ba7e119fa79e52c' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 06 Sep 2023 23:19:55 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 06 Sep 2023 23:19:55 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 06 Sep 2023 23:19:55 GMT
EXPOSE 4222 6222 8222
# Wed, 06 Sep 2023 23:19:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 06 Sep 2023 23:19:55 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:7264a8db6415046d36d16ba98b79778e18accee6ffa71850405994cffa9be7de`  
		Last Modified: Mon, 07 Aug 2023 19:20:54 GMT  
		Size: 3.4 MB (3401613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75fdd304ec17c2cf1f7629eefc922e04fae260b6d902e4fd42c81a5e5ce9d5dc`  
		Last Modified: Wed, 06 Sep 2023 23:20:32 GMT  
		Size: 5.9 MB (5867770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2863800c65f086f618bf3df0e7855997aea26ba27f4c759cf8bfae94da866bb`  
		Last Modified: Wed, 06 Sep 2023 23:20:31 GMT  
		Size: 585.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e32a641538132ed9885ca87c473fe9ff71415289c1f5276ba1157bb0760bd04`  
		Last Modified: Wed, 06 Sep 2023 23:20:31 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-alpine3.18` - linux; arm variant v6

```console
$ docker pull nats@sha256:e66fcde15a5b8028aed7cdd2e03392aa10c4a51c224e964f014eddc1c821433d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.7 MB (8749092 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6e3524e57732f8e26091d551f1b5ce64405e4217d19f047345dc28a29a1b847`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:49:14 GMT
ADD file:9882e99e5f94ab2db05c029648ac5be7cf0f063a8701394fcbb543a7ef5d4b90 in / 
# Mon, 07 Aug 2023 19:49:15 GMT
CMD ["/bin/sh"]
# Wed, 06 Sep 2023 23:04:40 GMT
ENV NATS_SERVER=2.9.22
# Wed, 06 Sep 2023 23:04:43 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='811e5a3c8187d937a753f182bd5ae2035c91604bda11a3b11023e5eea0504c41' ;; 		armhf) natsArch='arm6'; sha256='4d6f2f8ee9faf43de9fed5b43a0a5db836ad81797146065777b06a59f90cf1b0' ;; 		armv7) natsArch='arm7'; sha256='b8c83cd825b05d8d0610fc9352804fe810ae6bd9d8f0d814a39b0f152ec2ba79' ;; 		x86_64) natsArch='amd64'; sha256='9550278e34e94aebd410ec401bc145d3538e430ec2a40d5213fffdf9fdd49c27' ;; 		x86) natsArch='386'; sha256='a8ccdd37eac64b031ea96762d7f72a74445e9a708c0363549ba7e119fa79e52c' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 06 Sep 2023 23:04:43 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 06 Sep 2023 23:04:43 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 06 Sep 2023 23:04:43 GMT
EXPOSE 4222 6222 8222
# Wed, 06 Sep 2023 23:04:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 06 Sep 2023 23:04:43 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:af09961d4a43b504efc76e38b50918977c28be73eeb8b926247783a00e8b9f2f`  
		Last Modified: Mon, 07 Aug 2023 19:49:38 GMT  
		Size: 3.1 MB (3144809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5a6e71bd2ab60e313e659b569f8c33e5e9dcfdb580c25af0f9c5e7eca59f92f`  
		Last Modified: Wed, 06 Sep 2023 23:05:08 GMT  
		Size: 5.6 MB (5603285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7b94c778bbad17cc9be59c68102602e2e77462672d2e045f4713e80ce1cbb1c`  
		Last Modified: Wed, 06 Sep 2023 23:05:07 GMT  
		Size: 585.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4b258e6095309f7819e72dd444d848fe600fb2e73b5bd12bd1e9a556a17bf56`  
		Last Modified: Wed, 06 Sep 2023 23:05:07 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-alpine3.18` - linux; arm variant v7

```console
$ docker pull nats@sha256:9ca6685d1ad99fa588f9d4dc05ffe27569ed660b735218fd38795568fe508c73
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.5 MB (8492829 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0271598ef211f3df61073ff64c769275b4bb72b68b984931c8a7af1706fe80c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:57:25 GMT
ADD file:e3f56488d3d3bb67729714db13ddadf6652e7efb5281cfc7010d3e71f9d6607f in / 
# Mon, 07 Aug 2023 19:57:25 GMT
CMD ["/bin/sh"]
# Wed, 06 Sep 2023 22:57:29 GMT
ENV NATS_SERVER=2.9.22
# Wed, 06 Sep 2023 22:57:32 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='811e5a3c8187d937a753f182bd5ae2035c91604bda11a3b11023e5eea0504c41' ;; 		armhf) natsArch='arm6'; sha256='4d6f2f8ee9faf43de9fed5b43a0a5db836ad81797146065777b06a59f90cf1b0' ;; 		armv7) natsArch='arm7'; sha256='b8c83cd825b05d8d0610fc9352804fe810ae6bd9d8f0d814a39b0f152ec2ba79' ;; 		x86_64) natsArch='amd64'; sha256='9550278e34e94aebd410ec401bc145d3538e430ec2a40d5213fffdf9fdd49c27' ;; 		x86) natsArch='386'; sha256='a8ccdd37eac64b031ea96762d7f72a74445e9a708c0363549ba7e119fa79e52c' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 06 Sep 2023 22:57:32 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 06 Sep 2023 22:57:32 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 06 Sep 2023 22:57:32 GMT
EXPOSE 4222 6222 8222
# Wed, 06 Sep 2023 22:57:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 06 Sep 2023 22:57:32 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:f8dec92eec42224ef9e6ca9c6207ea6b9195dcf93d06bd5ceff0f814b62bf064`  
		Last Modified: Mon, 07 Aug 2023 19:57:55 GMT  
		Size: 2.9 MB (2899480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1962026ec365b08ba406dd0e38e57c06dcd04f2225faffcc17883ed87716cdc8`  
		Last Modified: Wed, 06 Sep 2023 22:58:03 GMT  
		Size: 5.6 MB (5592351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:578cf75378460664df525d3b5d1412e778f7b8cdc5f3c31207b3bbc2f6c074f5`  
		Last Modified: Wed, 06 Sep 2023 22:58:01 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64bf3e24d68a6cadd0880ce3163738934bf8e5b267923da68dd6922cd6b98a31`  
		Last Modified: Wed, 06 Sep 2023 22:58:01 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-alpine3.18` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:51e884da4e764cc784998e4bc69bbbefa4f39420be30021b4a1074dc40604423
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.7 MB (8734219 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c8cdff0ce493eb27f871f27f7ec452d1c36de63801fda0b331cd41067f858b9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:19 GMT
ADD file:b2e7eaa7e41f08853dbe08d84439a7f9fd32fc58c3aa1e298f3f60343b2b683a in / 
# Mon, 07 Aug 2023 19:39:19 GMT
CMD ["/bin/sh"]
# Wed, 06 Sep 2023 22:39:45 GMT
ENV NATS_SERVER=2.9.22
# Wed, 06 Sep 2023 22:39:47 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='811e5a3c8187d937a753f182bd5ae2035c91604bda11a3b11023e5eea0504c41' ;; 		armhf) natsArch='arm6'; sha256='4d6f2f8ee9faf43de9fed5b43a0a5db836ad81797146065777b06a59f90cf1b0' ;; 		armv7) natsArch='arm7'; sha256='b8c83cd825b05d8d0610fc9352804fe810ae6bd9d8f0d814a39b0f152ec2ba79' ;; 		x86_64) natsArch='amd64'; sha256='9550278e34e94aebd410ec401bc145d3538e430ec2a40d5213fffdf9fdd49c27' ;; 		x86) natsArch='386'; sha256='a8ccdd37eac64b031ea96762d7f72a74445e9a708c0363549ba7e119fa79e52c' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 06 Sep 2023 22:39:47 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 06 Sep 2023 22:39:47 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 06 Sep 2023 22:39:47 GMT
EXPOSE 4222 6222 8222
# Wed, 06 Sep 2023 22:39:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 06 Sep 2023 22:39:48 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9fda8d8052c61740409c4bea888859c141fd8cc3f58ac61943144ff6d1681b2d`  
		Last Modified: Mon, 07 Aug 2023 19:39:45 GMT  
		Size: 3.3 MB (3330767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64353667b2ee68f04c527f8dcef72789d979435b90c5b8073485e6c2fcc5c3f7`  
		Last Modified: Wed, 06 Sep 2023 22:40:28 GMT  
		Size: 5.4 MB (5402455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:540b41e481b61500ce8ed1c72cc5c0f937cabb489d0ba9de2dc2dad279696a28`  
		Last Modified: Wed, 06 Sep 2023 22:40:27 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb56160de8c01873d42326860132a0b877e470be0ff76c774c04b542515c9e4a`  
		Last Modified: Wed, 06 Sep 2023 22:40:27 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-linux`

```console
$ docker pull nats@sha256:7595e8b87b7063f28ffd3a1f0f7021f6c333fcc17377dbecccd7a6777df7754a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9-linux` - linux; amd64

```console
$ docker pull nats@sha256:841691cd373d85dfef90326ad2625e6498d8472d68d7d64b9a7d11b566729e77
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5245280 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7bfd417bdbd2f1eb2b6798d0a0fbba5ce7e3bd1d7ce50d29b8965cb174e801ed`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 06 Sep 2023 23:20:12 GMT
COPY file:acdb0e47969d6e334bcadb9c85dfef3166c764ff4ac55254185a04b1a6e8bbee in /nats-server 
# Wed, 06 Sep 2023 23:20:12 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 06 Sep 2023 23:20:12 GMT
EXPOSE 4222 6222 8222
# Wed, 06 Sep 2023 23:20:12 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 06 Sep 2023 23:20:12 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 06 Sep 2023 23:20:12 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:aac801db9a2a97942dde4494f98ce2d08c529a3af03ecb92f0b93426bbfd6419`  
		Last Modified: Wed, 06 Sep 2023 23:20:56 GMT  
		Size: 5.2 MB (5244773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f86dbe6523f83ad4a9d3f35c66bb097fad7505a3bd4de2123ea173ea21f1e38`  
		Last Modified: Wed, 06 Sep 2023 23:20:55 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:ec9d67b684f4605aa5fd2b86b64953bb8062a49d2916cf8e5fab437de945df15
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (4980015 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d632b911d90b9fc8ad6e2d0fd53012e9c8cc6ca17c685d2c8c2a6c4de2cb2c45`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 06 Sep 2023 23:04:49 GMT
COPY file:51aacaba9769a3f16e0467be1fc8eb86122f6f3496e89e41b61e0038083ae308 in /nats-server 
# Wed, 06 Sep 2023 23:04:49 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 06 Sep 2023 23:04:49 GMT
EXPOSE 4222 6222 8222
# Wed, 06 Sep 2023 23:04:49 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 06 Sep 2023 23:04:49 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 06 Sep 2023 23:04:50 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6a6e165fccf6da77ad3b09408162fc7daaafe266b71dd5da8679594aa110a3a5`  
		Last Modified: Wed, 06 Sep 2023 23:05:32 GMT  
		Size: 5.0 MB (4979506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1baf063892d372757ae2be4c42843e0a096826874b64519c230fd85bd65e69e8`  
		Last Modified: Wed, 06 Sep 2023 23:05:31 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:58dfaa80e9889d01819641e707279821d96d6f5eb7ce87e29eaa38cd4e0b5cac
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (4970850 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a2d43ddba67d73d9d9c8f19b9fbec53ca1bcb7f04349363538f7d08fd069dbd2`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 06 Sep 2023 22:57:45 GMT
COPY file:aae670bb79c659968f632ae3be388af62614010873ced2a439475906dbb769c6 in /nats-server 
# Wed, 06 Sep 2023 22:57:45 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 06 Sep 2023 22:57:45 GMT
EXPOSE 4222 6222 8222
# Wed, 06 Sep 2023 22:57:45 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 06 Sep 2023 22:57:46 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 06 Sep 2023 22:57:46 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:55b6dbad6639da13368cebb9688e8a5caaee29041e6b5e2e798201dfcf2b67ad`  
		Last Modified: Wed, 06 Sep 2023 22:58:23 GMT  
		Size: 5.0 MB (4970341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f17c52d1a9dd756c463e0590216b217bfee91f63c66217c407f1c98b1ebbc3b9`  
		Last Modified: Wed, 06 Sep 2023 22:58:22 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:dd48788f80e3925791e0dddfa44348b7df9022fbc914b20cf00e051a0b3adbf3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.8 MB (4778848 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0e35fd1c4293b595f11452fdc3e7dd6d5d9e033ecc9b1e6a35ff40577f2cba9f`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 06 Sep 2023 22:40:07 GMT
COPY file:d6eca5c67de65d1a8a30a51ea7318b044949c77108b2fdccc5aa0054c068c196 in /nats-server 
# Wed, 06 Sep 2023 22:40:07 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 06 Sep 2023 22:40:07 GMT
EXPOSE 4222 6222 8222
# Wed, 06 Sep 2023 22:40:08 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 06 Sep 2023 22:40:08 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 06 Sep 2023 22:40:08 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:88e5ff7f26ea25c6d2ab092989d9372cb32b3e60880124facfcefd7d3f0b7591`  
		Last Modified: Wed, 06 Sep 2023 22:40:49 GMT  
		Size: 4.8 MB (4778340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7795fd345dfb406d659c2502b733417a10ee85274263050ee36ab4aa021a38d9`  
		Last Modified: Wed, 06 Sep 2023 22:40:48 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-nanoserver`

```console
$ docker pull nats@sha256:347c71d5b7499fda4c79d015de6e2b9da4a28374147b6901e02f8e135e482bd1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4737; amd64

### `nats:2.9-nanoserver` - windows version 10.0.17763.4737; amd64

```console
$ docker pull nats@sha256:baec10f85f099b828313ff821f20b005907591e2f4fb414c7a240b5944f1292a
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.8 MB (109785996 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3654d1c2e7ef6e2297c519fd991a4a49b4d9928375a1142ec2af9cc55358ee84`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 02 Aug 2023 08:33:47 GMT
RUN Apply image 10.0.17763.4737
# Thu, 10 Aug 2023 02:34:52 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 06 Sep 2023 23:17:32 GMT
RUN cmd /S /C #(nop) COPY file:393d7e944d1b6697a14f19f6cb9673d95da4e1a0fc9508b238325e94beebc857 in C:\nats-server.exe 
# Wed, 06 Sep 2023 23:17:33 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 06 Sep 2023 23:17:34 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 06 Sep 2023 23:17:34 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 06 Sep 2023 23:17:35 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:86fab75eb466cadf89d853682179b3b57eba9fe28c78041dd52bced81e18a627`  
		Last Modified: Tue, 08 Aug 2023 17:55:54 GMT  
		Size: 104.5 MB (104459386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c43534c571f8fdc71038e0f4b4c33a30adb0bbc8b292454d35930557ced33408`  
		Last Modified: Thu, 10 Aug 2023 02:35:37 GMT  
		Size: 1.2 KB (1167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3eade3f0d46f534a5d639c78b1e85a1b0ea96d271fe2c3e706142d2f8d0aef7`  
		Last Modified: Wed, 06 Sep 2023 23:18:18 GMT  
		Size: 5.3 MB (5320148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4eeab0b725b185bf02913419c636eb70964ad972b883ef43006bbf75b1320ece`  
		Last Modified: Wed, 06 Sep 2023 23:18:16 GMT  
		Size: 1.8 KB (1804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c11e5f8af7811e39cecedb8bc4f4533b8f362e497bfe37a943209e0ce0d0bd5`  
		Last Modified: Wed, 06 Sep 2023 23:18:16 GMT  
		Size: 1.2 KB (1161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50806fff52469c9a918b10aa2ed383885dd30e5763ab2157c5440e425ebdccd3`  
		Last Modified: Wed, 06 Sep 2023 23:18:16 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f8c118167fb4c0339d4078748da065ff698f06d9373f7acaa5c42db51dfcdff`  
		Last Modified: Wed, 06 Sep 2023 23:18:16 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-nanoserver-1809`

```console
$ docker pull nats@sha256:347c71d5b7499fda4c79d015de6e2b9da4a28374147b6901e02f8e135e482bd1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4737; amd64

### `nats:2.9-nanoserver-1809` - windows version 10.0.17763.4737; amd64

```console
$ docker pull nats@sha256:baec10f85f099b828313ff821f20b005907591e2f4fb414c7a240b5944f1292a
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.8 MB (109785996 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3654d1c2e7ef6e2297c519fd991a4a49b4d9928375a1142ec2af9cc55358ee84`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 02 Aug 2023 08:33:47 GMT
RUN Apply image 10.0.17763.4737
# Thu, 10 Aug 2023 02:34:52 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 06 Sep 2023 23:17:32 GMT
RUN cmd /S /C #(nop) COPY file:393d7e944d1b6697a14f19f6cb9673d95da4e1a0fc9508b238325e94beebc857 in C:\nats-server.exe 
# Wed, 06 Sep 2023 23:17:33 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 06 Sep 2023 23:17:34 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 06 Sep 2023 23:17:34 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 06 Sep 2023 23:17:35 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:86fab75eb466cadf89d853682179b3b57eba9fe28c78041dd52bced81e18a627`  
		Last Modified: Tue, 08 Aug 2023 17:55:54 GMT  
		Size: 104.5 MB (104459386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c43534c571f8fdc71038e0f4b4c33a30adb0bbc8b292454d35930557ced33408`  
		Last Modified: Thu, 10 Aug 2023 02:35:37 GMT  
		Size: 1.2 KB (1167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3eade3f0d46f534a5d639c78b1e85a1b0ea96d271fe2c3e706142d2f8d0aef7`  
		Last Modified: Wed, 06 Sep 2023 23:18:18 GMT  
		Size: 5.3 MB (5320148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4eeab0b725b185bf02913419c636eb70964ad972b883ef43006bbf75b1320ece`  
		Last Modified: Wed, 06 Sep 2023 23:18:16 GMT  
		Size: 1.8 KB (1804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c11e5f8af7811e39cecedb8bc4f4533b8f362e497bfe37a943209e0ce0d0bd5`  
		Last Modified: Wed, 06 Sep 2023 23:18:16 GMT  
		Size: 1.2 KB (1161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50806fff52469c9a918b10aa2ed383885dd30e5763ab2157c5440e425ebdccd3`  
		Last Modified: Wed, 06 Sep 2023 23:18:16 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f8c118167fb4c0339d4078748da065ff698f06d9373f7acaa5c42db51dfcdff`  
		Last Modified: Wed, 06 Sep 2023 23:18:16 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-scratch`

```console
$ docker pull nats@sha256:7595e8b87b7063f28ffd3a1f0f7021f6c333fcc17377dbecccd7a6777df7754a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9-scratch` - linux; amd64

```console
$ docker pull nats@sha256:841691cd373d85dfef90326ad2625e6498d8472d68d7d64b9a7d11b566729e77
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5245280 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7bfd417bdbd2f1eb2b6798d0a0fbba5ce7e3bd1d7ce50d29b8965cb174e801ed`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 06 Sep 2023 23:20:12 GMT
COPY file:acdb0e47969d6e334bcadb9c85dfef3166c764ff4ac55254185a04b1a6e8bbee in /nats-server 
# Wed, 06 Sep 2023 23:20:12 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 06 Sep 2023 23:20:12 GMT
EXPOSE 4222 6222 8222
# Wed, 06 Sep 2023 23:20:12 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 06 Sep 2023 23:20:12 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 06 Sep 2023 23:20:12 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:aac801db9a2a97942dde4494f98ce2d08c529a3af03ecb92f0b93426bbfd6419`  
		Last Modified: Wed, 06 Sep 2023 23:20:56 GMT  
		Size: 5.2 MB (5244773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f86dbe6523f83ad4a9d3f35c66bb097fad7505a3bd4de2123ea173ea21f1e38`  
		Last Modified: Wed, 06 Sep 2023 23:20:55 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:ec9d67b684f4605aa5fd2b86b64953bb8062a49d2916cf8e5fab437de945df15
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (4980015 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d632b911d90b9fc8ad6e2d0fd53012e9c8cc6ca17c685d2c8c2a6c4de2cb2c45`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 06 Sep 2023 23:04:49 GMT
COPY file:51aacaba9769a3f16e0467be1fc8eb86122f6f3496e89e41b61e0038083ae308 in /nats-server 
# Wed, 06 Sep 2023 23:04:49 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 06 Sep 2023 23:04:49 GMT
EXPOSE 4222 6222 8222
# Wed, 06 Sep 2023 23:04:49 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 06 Sep 2023 23:04:49 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 06 Sep 2023 23:04:50 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6a6e165fccf6da77ad3b09408162fc7daaafe266b71dd5da8679594aa110a3a5`  
		Last Modified: Wed, 06 Sep 2023 23:05:32 GMT  
		Size: 5.0 MB (4979506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1baf063892d372757ae2be4c42843e0a096826874b64519c230fd85bd65e69e8`  
		Last Modified: Wed, 06 Sep 2023 23:05:31 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:58dfaa80e9889d01819641e707279821d96d6f5eb7ce87e29eaa38cd4e0b5cac
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (4970850 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a2d43ddba67d73d9d9c8f19b9fbec53ca1bcb7f04349363538f7d08fd069dbd2`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 06 Sep 2023 22:57:45 GMT
COPY file:aae670bb79c659968f632ae3be388af62614010873ced2a439475906dbb769c6 in /nats-server 
# Wed, 06 Sep 2023 22:57:45 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 06 Sep 2023 22:57:45 GMT
EXPOSE 4222 6222 8222
# Wed, 06 Sep 2023 22:57:45 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 06 Sep 2023 22:57:46 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 06 Sep 2023 22:57:46 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:55b6dbad6639da13368cebb9688e8a5caaee29041e6b5e2e798201dfcf2b67ad`  
		Last Modified: Wed, 06 Sep 2023 22:58:23 GMT  
		Size: 5.0 MB (4970341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f17c52d1a9dd756c463e0590216b217bfee91f63c66217c407f1c98b1ebbc3b9`  
		Last Modified: Wed, 06 Sep 2023 22:58:22 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:dd48788f80e3925791e0dddfa44348b7df9022fbc914b20cf00e051a0b3adbf3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.8 MB (4778848 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0e35fd1c4293b595f11452fdc3e7dd6d5d9e033ecc9b1e6a35ff40577f2cba9f`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 06 Sep 2023 22:40:07 GMT
COPY file:d6eca5c67de65d1a8a30a51ea7318b044949c77108b2fdccc5aa0054c068c196 in /nats-server 
# Wed, 06 Sep 2023 22:40:07 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 06 Sep 2023 22:40:07 GMT
EXPOSE 4222 6222 8222
# Wed, 06 Sep 2023 22:40:08 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 06 Sep 2023 22:40:08 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 06 Sep 2023 22:40:08 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:88e5ff7f26ea25c6d2ab092989d9372cb32b3e60880124facfcefd7d3f0b7591`  
		Last Modified: Wed, 06 Sep 2023 22:40:49 GMT  
		Size: 4.8 MB (4778340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7795fd345dfb406d659c2502b733417a10ee85274263050ee36ab4aa021a38d9`  
		Last Modified: Wed, 06 Sep 2023 22:40:48 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-windowsservercore`

```console
$ docker pull nats@sha256:df25045f4d70165b54b8b7b0ae443fd21450261550bbc1b314adf8a58053e707
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4737; amd64

### `nats:2.9-windowsservercore` - windows version 10.0.17763.4737; amd64

```console
$ docker pull nats@sha256:e2f9912126f4753a9e9312b5dd77a5c5e44c257f28d04ad55cef0662d24138a2
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2001990927 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3cf5f23a9d8d2eca784896bbd09d5e163b27485e7b392cd0bd92f88502dd57b7`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Wed, 02 Aug 2023 09:07:15 GMT
RUN Install update 10.0.17763.4737
# Thu, 10 Aug 2023 01:11:08 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Thu, 10 Aug 2023 02:32:08 GMT
ENV NATS_DOCKERIZED=1
# Wed, 06 Sep 2023 23:15:04 GMT
ENV NATS_SERVER=2.9.22
# Wed, 06 Sep 2023 23:15:05 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.9.22/nats-server-v2.9.22-windows-amd64.zip
# Wed, 06 Sep 2023 23:15:06 GMT
ENV NATS_SERVER_SHASUM=e91db73b02bd4dca3eb7a4bf32e29763450b08d593f73e87d0a6b70102dea0d4
# Wed, 06 Sep 2023 23:15:56 GMT
RUN Set-PSDebug -Trace 2
# Wed, 06 Sep 2023 23:17:21 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 06 Sep 2023 23:17:22 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 06 Sep 2023 23:17:23 GMT
EXPOSE 4222 6222 8222
# Wed, 06 Sep 2023 23:17:24 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 06 Sep 2023 23:17:24 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b95f433aa7d90194e65f6b08a599b3ee12292e124d47c204107baedfd71054c1`  
		Last Modified: Tue, 08 Aug 2023 18:31:16 GMT  
		Size: 345.3 MB (345334986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c5180b8f5f7c2303ba89717cfa778a2173921ca7efdc058cfd6ed951c6d5ca3`  
		Last Modified: Thu, 10 Aug 2023 01:57:18 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fed0c598ca0ae763bd83f045a0c9262bf153a47e508b736992d196e2fb47dea`  
		Last Modified: Thu, 10 Aug 2023 02:35:22 GMT  
		Size: 1.4 KB (1449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab0ebc9f46983ba56ff415cd7b99891210ab8eaad5adf4a15a8f2021de4ebdfd`  
		Last Modified: Wed, 06 Sep 2023 23:18:02 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1c4a22897bb4d3fa0ef4fff463ef850ad45e21404737f120c724fb472c77221`  
		Last Modified: Wed, 06 Sep 2023 23:18:02 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c30142424ff3f45c3c8923f1aa5d959879239599fdde6aba1101c39a168abe48`  
		Last Modified: Wed, 06 Sep 2023 23:18:02 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3723e4e864a2d241c8133b4f1c569ac4ac140d29fe8e216ecd140ebd0e2531cd`  
		Last Modified: Wed, 06 Sep 2023 23:18:02 GMT  
		Size: 242.5 KB (242470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae4c6899207e83d648ab5bf60620507d438b612cb42961f5b8b300c25fde01dd`  
		Last Modified: Wed, 06 Sep 2023 23:18:02 GMT  
		Size: 5.8 MB (5779810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bc2f6a7b18656a6539013442aa6e8c88b49fddce30025ad67ba6e4867a2860b`  
		Last Modified: Wed, 06 Sep 2023 23:18:00 GMT  
		Size: 2.0 KB (1976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ac72b596159b34e1de106133f926192bb5daac9b62301a55822162e6656b6cc`  
		Last Modified: Wed, 06 Sep 2023 23:18:00 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a11a75f33304f42224c3b832462b4497699310fd70a6cdfb322bd126be44cb32`  
		Last Modified: Wed, 06 Sep 2023 23:18:00 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c01b20cb00adae2b356c4377b9419f6a1d18d74692e89c0ee1e66d7b55ca3f3`  
		Last Modified: Wed, 06 Sep 2023 23:18:00 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-windowsservercore-1809`

```console
$ docker pull nats@sha256:df25045f4d70165b54b8b7b0ae443fd21450261550bbc1b314adf8a58053e707
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4737; amd64

### `nats:2.9-windowsservercore-1809` - windows version 10.0.17763.4737; amd64

```console
$ docker pull nats@sha256:e2f9912126f4753a9e9312b5dd77a5c5e44c257f28d04ad55cef0662d24138a2
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2001990927 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3cf5f23a9d8d2eca784896bbd09d5e163b27485e7b392cd0bd92f88502dd57b7`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Wed, 02 Aug 2023 09:07:15 GMT
RUN Install update 10.0.17763.4737
# Thu, 10 Aug 2023 01:11:08 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Thu, 10 Aug 2023 02:32:08 GMT
ENV NATS_DOCKERIZED=1
# Wed, 06 Sep 2023 23:15:04 GMT
ENV NATS_SERVER=2.9.22
# Wed, 06 Sep 2023 23:15:05 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.9.22/nats-server-v2.9.22-windows-amd64.zip
# Wed, 06 Sep 2023 23:15:06 GMT
ENV NATS_SERVER_SHASUM=e91db73b02bd4dca3eb7a4bf32e29763450b08d593f73e87d0a6b70102dea0d4
# Wed, 06 Sep 2023 23:15:56 GMT
RUN Set-PSDebug -Trace 2
# Wed, 06 Sep 2023 23:17:21 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 06 Sep 2023 23:17:22 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 06 Sep 2023 23:17:23 GMT
EXPOSE 4222 6222 8222
# Wed, 06 Sep 2023 23:17:24 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 06 Sep 2023 23:17:24 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b95f433aa7d90194e65f6b08a599b3ee12292e124d47c204107baedfd71054c1`  
		Last Modified: Tue, 08 Aug 2023 18:31:16 GMT  
		Size: 345.3 MB (345334986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c5180b8f5f7c2303ba89717cfa778a2173921ca7efdc058cfd6ed951c6d5ca3`  
		Last Modified: Thu, 10 Aug 2023 01:57:18 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fed0c598ca0ae763bd83f045a0c9262bf153a47e508b736992d196e2fb47dea`  
		Last Modified: Thu, 10 Aug 2023 02:35:22 GMT  
		Size: 1.4 KB (1449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab0ebc9f46983ba56ff415cd7b99891210ab8eaad5adf4a15a8f2021de4ebdfd`  
		Last Modified: Wed, 06 Sep 2023 23:18:02 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1c4a22897bb4d3fa0ef4fff463ef850ad45e21404737f120c724fb472c77221`  
		Last Modified: Wed, 06 Sep 2023 23:18:02 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c30142424ff3f45c3c8923f1aa5d959879239599fdde6aba1101c39a168abe48`  
		Last Modified: Wed, 06 Sep 2023 23:18:02 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3723e4e864a2d241c8133b4f1c569ac4ac140d29fe8e216ecd140ebd0e2531cd`  
		Last Modified: Wed, 06 Sep 2023 23:18:02 GMT  
		Size: 242.5 KB (242470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae4c6899207e83d648ab5bf60620507d438b612cb42961f5b8b300c25fde01dd`  
		Last Modified: Wed, 06 Sep 2023 23:18:02 GMT  
		Size: 5.8 MB (5779810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bc2f6a7b18656a6539013442aa6e8c88b49fddce30025ad67ba6e4867a2860b`  
		Last Modified: Wed, 06 Sep 2023 23:18:00 GMT  
		Size: 2.0 KB (1976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ac72b596159b34e1de106133f926192bb5daac9b62301a55822162e6656b6cc`  
		Last Modified: Wed, 06 Sep 2023 23:18:00 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a11a75f33304f42224c3b832462b4497699310fd70a6cdfb322bd126be44cb32`  
		Last Modified: Wed, 06 Sep 2023 23:18:00 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c01b20cb00adae2b356c4377b9419f6a1d18d74692e89c0ee1e66d7b55ca3f3`  
		Last Modified: Wed, 06 Sep 2023 23:18:00 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.22`

```console
$ docker pull nats@sha256:70a536ddc540ab27ecf4ea6666bf495473a11f408d17bb694008fec41f3c4e87
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.4737; amd64

### `nats:2.9.22` - linux; amd64

```console
$ docker pull nats@sha256:841691cd373d85dfef90326ad2625e6498d8472d68d7d64b9a7d11b566729e77
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5245280 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7bfd417bdbd2f1eb2b6798d0a0fbba5ce7e3bd1d7ce50d29b8965cb174e801ed`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 06 Sep 2023 23:20:12 GMT
COPY file:acdb0e47969d6e334bcadb9c85dfef3166c764ff4ac55254185a04b1a6e8bbee in /nats-server 
# Wed, 06 Sep 2023 23:20:12 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 06 Sep 2023 23:20:12 GMT
EXPOSE 4222 6222 8222
# Wed, 06 Sep 2023 23:20:12 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 06 Sep 2023 23:20:12 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 06 Sep 2023 23:20:12 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:aac801db9a2a97942dde4494f98ce2d08c529a3af03ecb92f0b93426bbfd6419`  
		Last Modified: Wed, 06 Sep 2023 23:20:56 GMT  
		Size: 5.2 MB (5244773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f86dbe6523f83ad4a9d3f35c66bb097fad7505a3bd4de2123ea173ea21f1e38`  
		Last Modified: Wed, 06 Sep 2023 23:20:55 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.22` - linux; arm variant v6

```console
$ docker pull nats@sha256:ec9d67b684f4605aa5fd2b86b64953bb8062a49d2916cf8e5fab437de945df15
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (4980015 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d632b911d90b9fc8ad6e2d0fd53012e9c8cc6ca17c685d2c8c2a6c4de2cb2c45`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 06 Sep 2023 23:04:49 GMT
COPY file:51aacaba9769a3f16e0467be1fc8eb86122f6f3496e89e41b61e0038083ae308 in /nats-server 
# Wed, 06 Sep 2023 23:04:49 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 06 Sep 2023 23:04:49 GMT
EXPOSE 4222 6222 8222
# Wed, 06 Sep 2023 23:04:49 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 06 Sep 2023 23:04:49 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 06 Sep 2023 23:04:50 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6a6e165fccf6da77ad3b09408162fc7daaafe266b71dd5da8679594aa110a3a5`  
		Last Modified: Wed, 06 Sep 2023 23:05:32 GMT  
		Size: 5.0 MB (4979506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1baf063892d372757ae2be4c42843e0a096826874b64519c230fd85bd65e69e8`  
		Last Modified: Wed, 06 Sep 2023 23:05:31 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.22` - linux; arm variant v7

```console
$ docker pull nats@sha256:58dfaa80e9889d01819641e707279821d96d6f5eb7ce87e29eaa38cd4e0b5cac
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (4970850 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a2d43ddba67d73d9d9c8f19b9fbec53ca1bcb7f04349363538f7d08fd069dbd2`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 06 Sep 2023 22:57:45 GMT
COPY file:aae670bb79c659968f632ae3be388af62614010873ced2a439475906dbb769c6 in /nats-server 
# Wed, 06 Sep 2023 22:57:45 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 06 Sep 2023 22:57:45 GMT
EXPOSE 4222 6222 8222
# Wed, 06 Sep 2023 22:57:45 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 06 Sep 2023 22:57:46 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 06 Sep 2023 22:57:46 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:55b6dbad6639da13368cebb9688e8a5caaee29041e6b5e2e798201dfcf2b67ad`  
		Last Modified: Wed, 06 Sep 2023 22:58:23 GMT  
		Size: 5.0 MB (4970341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f17c52d1a9dd756c463e0590216b217bfee91f63c66217c407f1c98b1ebbc3b9`  
		Last Modified: Wed, 06 Sep 2023 22:58:22 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.22` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:dd48788f80e3925791e0dddfa44348b7df9022fbc914b20cf00e051a0b3adbf3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.8 MB (4778848 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0e35fd1c4293b595f11452fdc3e7dd6d5d9e033ecc9b1e6a35ff40577f2cba9f`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 06 Sep 2023 22:40:07 GMT
COPY file:d6eca5c67de65d1a8a30a51ea7318b044949c77108b2fdccc5aa0054c068c196 in /nats-server 
# Wed, 06 Sep 2023 22:40:07 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 06 Sep 2023 22:40:07 GMT
EXPOSE 4222 6222 8222
# Wed, 06 Sep 2023 22:40:08 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 06 Sep 2023 22:40:08 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 06 Sep 2023 22:40:08 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:88e5ff7f26ea25c6d2ab092989d9372cb32b3e60880124facfcefd7d3f0b7591`  
		Last Modified: Wed, 06 Sep 2023 22:40:49 GMT  
		Size: 4.8 MB (4778340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7795fd345dfb406d659c2502b733417a10ee85274263050ee36ab4aa021a38d9`  
		Last Modified: Wed, 06 Sep 2023 22:40:48 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.22` - windows version 10.0.17763.4737; amd64

```console
$ docker pull nats@sha256:baec10f85f099b828313ff821f20b005907591e2f4fb414c7a240b5944f1292a
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.8 MB (109785996 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3654d1c2e7ef6e2297c519fd991a4a49b4d9928375a1142ec2af9cc55358ee84`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 02 Aug 2023 08:33:47 GMT
RUN Apply image 10.0.17763.4737
# Thu, 10 Aug 2023 02:34:52 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 06 Sep 2023 23:17:32 GMT
RUN cmd /S /C #(nop) COPY file:393d7e944d1b6697a14f19f6cb9673d95da4e1a0fc9508b238325e94beebc857 in C:\nats-server.exe 
# Wed, 06 Sep 2023 23:17:33 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 06 Sep 2023 23:17:34 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 06 Sep 2023 23:17:34 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 06 Sep 2023 23:17:35 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:86fab75eb466cadf89d853682179b3b57eba9fe28c78041dd52bced81e18a627`  
		Last Modified: Tue, 08 Aug 2023 17:55:54 GMT  
		Size: 104.5 MB (104459386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c43534c571f8fdc71038e0f4b4c33a30adb0bbc8b292454d35930557ced33408`  
		Last Modified: Thu, 10 Aug 2023 02:35:37 GMT  
		Size: 1.2 KB (1167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3eade3f0d46f534a5d639c78b1e85a1b0ea96d271fe2c3e706142d2f8d0aef7`  
		Last Modified: Wed, 06 Sep 2023 23:18:18 GMT  
		Size: 5.3 MB (5320148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4eeab0b725b185bf02913419c636eb70964ad972b883ef43006bbf75b1320ece`  
		Last Modified: Wed, 06 Sep 2023 23:18:16 GMT  
		Size: 1.8 KB (1804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c11e5f8af7811e39cecedb8bc4f4533b8f362e497bfe37a943209e0ce0d0bd5`  
		Last Modified: Wed, 06 Sep 2023 23:18:16 GMT  
		Size: 1.2 KB (1161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50806fff52469c9a918b10aa2ed383885dd30e5763ab2157c5440e425ebdccd3`  
		Last Modified: Wed, 06 Sep 2023 23:18:16 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f8c118167fb4c0339d4078748da065ff698f06d9373f7acaa5c42db51dfcdff`  
		Last Modified: Wed, 06 Sep 2023 23:18:16 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.22-alpine`

```console
$ docker pull nats@sha256:36d34c59ed76472d9b3caafc5e3764b7a587498808efdd5178468f4efe8b4887
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9.22-alpine` - linux; amd64

```console
$ docker pull nats@sha256:756a55661288407f688c52224ac8b12d008f0fec9343c68281b04bb59cbcc427
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.3 MB (9270382 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dbb9252d07acfbe3ac9083449c0fef74561021019d85c2993f5bce02c7a16201`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:20 GMT
ADD file:32ff5e7a78b890996ee4681cc0a26185d3e9acdb4eb1e2aaccb2411f922fed6b in / 
# Mon, 07 Aug 2023 19:20:20 GMT
CMD ["/bin/sh"]
# Wed, 06 Sep 2023 23:19:53 GMT
ENV NATS_SERVER=2.9.22
# Wed, 06 Sep 2023 23:19:55 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='811e5a3c8187d937a753f182bd5ae2035c91604bda11a3b11023e5eea0504c41' ;; 		armhf) natsArch='arm6'; sha256='4d6f2f8ee9faf43de9fed5b43a0a5db836ad81797146065777b06a59f90cf1b0' ;; 		armv7) natsArch='arm7'; sha256='b8c83cd825b05d8d0610fc9352804fe810ae6bd9d8f0d814a39b0f152ec2ba79' ;; 		x86_64) natsArch='amd64'; sha256='9550278e34e94aebd410ec401bc145d3538e430ec2a40d5213fffdf9fdd49c27' ;; 		x86) natsArch='386'; sha256='a8ccdd37eac64b031ea96762d7f72a74445e9a708c0363549ba7e119fa79e52c' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 06 Sep 2023 23:19:55 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 06 Sep 2023 23:19:55 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 06 Sep 2023 23:19:55 GMT
EXPOSE 4222 6222 8222
# Wed, 06 Sep 2023 23:19:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 06 Sep 2023 23:19:55 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:7264a8db6415046d36d16ba98b79778e18accee6ffa71850405994cffa9be7de`  
		Last Modified: Mon, 07 Aug 2023 19:20:54 GMT  
		Size: 3.4 MB (3401613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75fdd304ec17c2cf1f7629eefc922e04fae260b6d902e4fd42c81a5e5ce9d5dc`  
		Last Modified: Wed, 06 Sep 2023 23:20:32 GMT  
		Size: 5.9 MB (5867770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2863800c65f086f618bf3df0e7855997aea26ba27f4c759cf8bfae94da866bb`  
		Last Modified: Wed, 06 Sep 2023 23:20:31 GMT  
		Size: 585.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e32a641538132ed9885ca87c473fe9ff71415289c1f5276ba1157bb0760bd04`  
		Last Modified: Wed, 06 Sep 2023 23:20:31 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.22-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:e66fcde15a5b8028aed7cdd2e03392aa10c4a51c224e964f014eddc1c821433d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.7 MB (8749092 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6e3524e57732f8e26091d551f1b5ce64405e4217d19f047345dc28a29a1b847`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:49:14 GMT
ADD file:9882e99e5f94ab2db05c029648ac5be7cf0f063a8701394fcbb543a7ef5d4b90 in / 
# Mon, 07 Aug 2023 19:49:15 GMT
CMD ["/bin/sh"]
# Wed, 06 Sep 2023 23:04:40 GMT
ENV NATS_SERVER=2.9.22
# Wed, 06 Sep 2023 23:04:43 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='811e5a3c8187d937a753f182bd5ae2035c91604bda11a3b11023e5eea0504c41' ;; 		armhf) natsArch='arm6'; sha256='4d6f2f8ee9faf43de9fed5b43a0a5db836ad81797146065777b06a59f90cf1b0' ;; 		armv7) natsArch='arm7'; sha256='b8c83cd825b05d8d0610fc9352804fe810ae6bd9d8f0d814a39b0f152ec2ba79' ;; 		x86_64) natsArch='amd64'; sha256='9550278e34e94aebd410ec401bc145d3538e430ec2a40d5213fffdf9fdd49c27' ;; 		x86) natsArch='386'; sha256='a8ccdd37eac64b031ea96762d7f72a74445e9a708c0363549ba7e119fa79e52c' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 06 Sep 2023 23:04:43 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 06 Sep 2023 23:04:43 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 06 Sep 2023 23:04:43 GMT
EXPOSE 4222 6222 8222
# Wed, 06 Sep 2023 23:04:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 06 Sep 2023 23:04:43 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:af09961d4a43b504efc76e38b50918977c28be73eeb8b926247783a00e8b9f2f`  
		Last Modified: Mon, 07 Aug 2023 19:49:38 GMT  
		Size: 3.1 MB (3144809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5a6e71bd2ab60e313e659b569f8c33e5e9dcfdb580c25af0f9c5e7eca59f92f`  
		Last Modified: Wed, 06 Sep 2023 23:05:08 GMT  
		Size: 5.6 MB (5603285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7b94c778bbad17cc9be59c68102602e2e77462672d2e045f4713e80ce1cbb1c`  
		Last Modified: Wed, 06 Sep 2023 23:05:07 GMT  
		Size: 585.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4b258e6095309f7819e72dd444d848fe600fb2e73b5bd12bd1e9a556a17bf56`  
		Last Modified: Wed, 06 Sep 2023 23:05:07 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.22-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:9ca6685d1ad99fa588f9d4dc05ffe27569ed660b735218fd38795568fe508c73
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.5 MB (8492829 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0271598ef211f3df61073ff64c769275b4bb72b68b984931c8a7af1706fe80c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:57:25 GMT
ADD file:e3f56488d3d3bb67729714db13ddadf6652e7efb5281cfc7010d3e71f9d6607f in / 
# Mon, 07 Aug 2023 19:57:25 GMT
CMD ["/bin/sh"]
# Wed, 06 Sep 2023 22:57:29 GMT
ENV NATS_SERVER=2.9.22
# Wed, 06 Sep 2023 22:57:32 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='811e5a3c8187d937a753f182bd5ae2035c91604bda11a3b11023e5eea0504c41' ;; 		armhf) natsArch='arm6'; sha256='4d6f2f8ee9faf43de9fed5b43a0a5db836ad81797146065777b06a59f90cf1b0' ;; 		armv7) natsArch='arm7'; sha256='b8c83cd825b05d8d0610fc9352804fe810ae6bd9d8f0d814a39b0f152ec2ba79' ;; 		x86_64) natsArch='amd64'; sha256='9550278e34e94aebd410ec401bc145d3538e430ec2a40d5213fffdf9fdd49c27' ;; 		x86) natsArch='386'; sha256='a8ccdd37eac64b031ea96762d7f72a74445e9a708c0363549ba7e119fa79e52c' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 06 Sep 2023 22:57:32 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 06 Sep 2023 22:57:32 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 06 Sep 2023 22:57:32 GMT
EXPOSE 4222 6222 8222
# Wed, 06 Sep 2023 22:57:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 06 Sep 2023 22:57:32 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:f8dec92eec42224ef9e6ca9c6207ea6b9195dcf93d06bd5ceff0f814b62bf064`  
		Last Modified: Mon, 07 Aug 2023 19:57:55 GMT  
		Size: 2.9 MB (2899480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1962026ec365b08ba406dd0e38e57c06dcd04f2225faffcc17883ed87716cdc8`  
		Last Modified: Wed, 06 Sep 2023 22:58:03 GMT  
		Size: 5.6 MB (5592351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:578cf75378460664df525d3b5d1412e778f7b8cdc5f3c31207b3bbc2f6c074f5`  
		Last Modified: Wed, 06 Sep 2023 22:58:01 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64bf3e24d68a6cadd0880ce3163738934bf8e5b267923da68dd6922cd6b98a31`  
		Last Modified: Wed, 06 Sep 2023 22:58:01 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.22-alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:51e884da4e764cc784998e4bc69bbbefa4f39420be30021b4a1074dc40604423
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.7 MB (8734219 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c8cdff0ce493eb27f871f27f7ec452d1c36de63801fda0b331cd41067f858b9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:19 GMT
ADD file:b2e7eaa7e41f08853dbe08d84439a7f9fd32fc58c3aa1e298f3f60343b2b683a in / 
# Mon, 07 Aug 2023 19:39:19 GMT
CMD ["/bin/sh"]
# Wed, 06 Sep 2023 22:39:45 GMT
ENV NATS_SERVER=2.9.22
# Wed, 06 Sep 2023 22:39:47 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='811e5a3c8187d937a753f182bd5ae2035c91604bda11a3b11023e5eea0504c41' ;; 		armhf) natsArch='arm6'; sha256='4d6f2f8ee9faf43de9fed5b43a0a5db836ad81797146065777b06a59f90cf1b0' ;; 		armv7) natsArch='arm7'; sha256='b8c83cd825b05d8d0610fc9352804fe810ae6bd9d8f0d814a39b0f152ec2ba79' ;; 		x86_64) natsArch='amd64'; sha256='9550278e34e94aebd410ec401bc145d3538e430ec2a40d5213fffdf9fdd49c27' ;; 		x86) natsArch='386'; sha256='a8ccdd37eac64b031ea96762d7f72a74445e9a708c0363549ba7e119fa79e52c' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 06 Sep 2023 22:39:47 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 06 Sep 2023 22:39:47 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 06 Sep 2023 22:39:47 GMT
EXPOSE 4222 6222 8222
# Wed, 06 Sep 2023 22:39:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 06 Sep 2023 22:39:48 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9fda8d8052c61740409c4bea888859c141fd8cc3f58ac61943144ff6d1681b2d`  
		Last Modified: Mon, 07 Aug 2023 19:39:45 GMT  
		Size: 3.3 MB (3330767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64353667b2ee68f04c527f8dcef72789d979435b90c5b8073485e6c2fcc5c3f7`  
		Last Modified: Wed, 06 Sep 2023 22:40:28 GMT  
		Size: 5.4 MB (5402455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:540b41e481b61500ce8ed1c72cc5c0f937cabb489d0ba9de2dc2dad279696a28`  
		Last Modified: Wed, 06 Sep 2023 22:40:27 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb56160de8c01873d42326860132a0b877e470be0ff76c774c04b542515c9e4a`  
		Last Modified: Wed, 06 Sep 2023 22:40:27 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.22-alpine3.18`

```console
$ docker pull nats@sha256:36d34c59ed76472d9b3caafc5e3764b7a587498808efdd5178468f4efe8b4887
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9.22-alpine3.18` - linux; amd64

```console
$ docker pull nats@sha256:756a55661288407f688c52224ac8b12d008f0fec9343c68281b04bb59cbcc427
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.3 MB (9270382 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dbb9252d07acfbe3ac9083449c0fef74561021019d85c2993f5bce02c7a16201`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:20 GMT
ADD file:32ff5e7a78b890996ee4681cc0a26185d3e9acdb4eb1e2aaccb2411f922fed6b in / 
# Mon, 07 Aug 2023 19:20:20 GMT
CMD ["/bin/sh"]
# Wed, 06 Sep 2023 23:19:53 GMT
ENV NATS_SERVER=2.9.22
# Wed, 06 Sep 2023 23:19:55 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='811e5a3c8187d937a753f182bd5ae2035c91604bda11a3b11023e5eea0504c41' ;; 		armhf) natsArch='arm6'; sha256='4d6f2f8ee9faf43de9fed5b43a0a5db836ad81797146065777b06a59f90cf1b0' ;; 		armv7) natsArch='arm7'; sha256='b8c83cd825b05d8d0610fc9352804fe810ae6bd9d8f0d814a39b0f152ec2ba79' ;; 		x86_64) natsArch='amd64'; sha256='9550278e34e94aebd410ec401bc145d3538e430ec2a40d5213fffdf9fdd49c27' ;; 		x86) natsArch='386'; sha256='a8ccdd37eac64b031ea96762d7f72a74445e9a708c0363549ba7e119fa79e52c' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 06 Sep 2023 23:19:55 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 06 Sep 2023 23:19:55 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 06 Sep 2023 23:19:55 GMT
EXPOSE 4222 6222 8222
# Wed, 06 Sep 2023 23:19:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 06 Sep 2023 23:19:55 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:7264a8db6415046d36d16ba98b79778e18accee6ffa71850405994cffa9be7de`  
		Last Modified: Mon, 07 Aug 2023 19:20:54 GMT  
		Size: 3.4 MB (3401613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75fdd304ec17c2cf1f7629eefc922e04fae260b6d902e4fd42c81a5e5ce9d5dc`  
		Last Modified: Wed, 06 Sep 2023 23:20:32 GMT  
		Size: 5.9 MB (5867770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2863800c65f086f618bf3df0e7855997aea26ba27f4c759cf8bfae94da866bb`  
		Last Modified: Wed, 06 Sep 2023 23:20:31 GMT  
		Size: 585.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e32a641538132ed9885ca87c473fe9ff71415289c1f5276ba1157bb0760bd04`  
		Last Modified: Wed, 06 Sep 2023 23:20:31 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.22-alpine3.18` - linux; arm variant v6

```console
$ docker pull nats@sha256:e66fcde15a5b8028aed7cdd2e03392aa10c4a51c224e964f014eddc1c821433d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.7 MB (8749092 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6e3524e57732f8e26091d551f1b5ce64405e4217d19f047345dc28a29a1b847`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:49:14 GMT
ADD file:9882e99e5f94ab2db05c029648ac5be7cf0f063a8701394fcbb543a7ef5d4b90 in / 
# Mon, 07 Aug 2023 19:49:15 GMT
CMD ["/bin/sh"]
# Wed, 06 Sep 2023 23:04:40 GMT
ENV NATS_SERVER=2.9.22
# Wed, 06 Sep 2023 23:04:43 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='811e5a3c8187d937a753f182bd5ae2035c91604bda11a3b11023e5eea0504c41' ;; 		armhf) natsArch='arm6'; sha256='4d6f2f8ee9faf43de9fed5b43a0a5db836ad81797146065777b06a59f90cf1b0' ;; 		armv7) natsArch='arm7'; sha256='b8c83cd825b05d8d0610fc9352804fe810ae6bd9d8f0d814a39b0f152ec2ba79' ;; 		x86_64) natsArch='amd64'; sha256='9550278e34e94aebd410ec401bc145d3538e430ec2a40d5213fffdf9fdd49c27' ;; 		x86) natsArch='386'; sha256='a8ccdd37eac64b031ea96762d7f72a74445e9a708c0363549ba7e119fa79e52c' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 06 Sep 2023 23:04:43 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 06 Sep 2023 23:04:43 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 06 Sep 2023 23:04:43 GMT
EXPOSE 4222 6222 8222
# Wed, 06 Sep 2023 23:04:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 06 Sep 2023 23:04:43 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:af09961d4a43b504efc76e38b50918977c28be73eeb8b926247783a00e8b9f2f`  
		Last Modified: Mon, 07 Aug 2023 19:49:38 GMT  
		Size: 3.1 MB (3144809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5a6e71bd2ab60e313e659b569f8c33e5e9dcfdb580c25af0f9c5e7eca59f92f`  
		Last Modified: Wed, 06 Sep 2023 23:05:08 GMT  
		Size: 5.6 MB (5603285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7b94c778bbad17cc9be59c68102602e2e77462672d2e045f4713e80ce1cbb1c`  
		Last Modified: Wed, 06 Sep 2023 23:05:07 GMT  
		Size: 585.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4b258e6095309f7819e72dd444d848fe600fb2e73b5bd12bd1e9a556a17bf56`  
		Last Modified: Wed, 06 Sep 2023 23:05:07 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.22-alpine3.18` - linux; arm variant v7

```console
$ docker pull nats@sha256:9ca6685d1ad99fa588f9d4dc05ffe27569ed660b735218fd38795568fe508c73
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.5 MB (8492829 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0271598ef211f3df61073ff64c769275b4bb72b68b984931c8a7af1706fe80c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:57:25 GMT
ADD file:e3f56488d3d3bb67729714db13ddadf6652e7efb5281cfc7010d3e71f9d6607f in / 
# Mon, 07 Aug 2023 19:57:25 GMT
CMD ["/bin/sh"]
# Wed, 06 Sep 2023 22:57:29 GMT
ENV NATS_SERVER=2.9.22
# Wed, 06 Sep 2023 22:57:32 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='811e5a3c8187d937a753f182bd5ae2035c91604bda11a3b11023e5eea0504c41' ;; 		armhf) natsArch='arm6'; sha256='4d6f2f8ee9faf43de9fed5b43a0a5db836ad81797146065777b06a59f90cf1b0' ;; 		armv7) natsArch='arm7'; sha256='b8c83cd825b05d8d0610fc9352804fe810ae6bd9d8f0d814a39b0f152ec2ba79' ;; 		x86_64) natsArch='amd64'; sha256='9550278e34e94aebd410ec401bc145d3538e430ec2a40d5213fffdf9fdd49c27' ;; 		x86) natsArch='386'; sha256='a8ccdd37eac64b031ea96762d7f72a74445e9a708c0363549ba7e119fa79e52c' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 06 Sep 2023 22:57:32 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 06 Sep 2023 22:57:32 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 06 Sep 2023 22:57:32 GMT
EXPOSE 4222 6222 8222
# Wed, 06 Sep 2023 22:57:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 06 Sep 2023 22:57:32 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:f8dec92eec42224ef9e6ca9c6207ea6b9195dcf93d06bd5ceff0f814b62bf064`  
		Last Modified: Mon, 07 Aug 2023 19:57:55 GMT  
		Size: 2.9 MB (2899480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1962026ec365b08ba406dd0e38e57c06dcd04f2225faffcc17883ed87716cdc8`  
		Last Modified: Wed, 06 Sep 2023 22:58:03 GMT  
		Size: 5.6 MB (5592351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:578cf75378460664df525d3b5d1412e778f7b8cdc5f3c31207b3bbc2f6c074f5`  
		Last Modified: Wed, 06 Sep 2023 22:58:01 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64bf3e24d68a6cadd0880ce3163738934bf8e5b267923da68dd6922cd6b98a31`  
		Last Modified: Wed, 06 Sep 2023 22:58:01 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.22-alpine3.18` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:51e884da4e764cc784998e4bc69bbbefa4f39420be30021b4a1074dc40604423
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.7 MB (8734219 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c8cdff0ce493eb27f871f27f7ec452d1c36de63801fda0b331cd41067f858b9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:19 GMT
ADD file:b2e7eaa7e41f08853dbe08d84439a7f9fd32fc58c3aa1e298f3f60343b2b683a in / 
# Mon, 07 Aug 2023 19:39:19 GMT
CMD ["/bin/sh"]
# Wed, 06 Sep 2023 22:39:45 GMT
ENV NATS_SERVER=2.9.22
# Wed, 06 Sep 2023 22:39:47 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='811e5a3c8187d937a753f182bd5ae2035c91604bda11a3b11023e5eea0504c41' ;; 		armhf) natsArch='arm6'; sha256='4d6f2f8ee9faf43de9fed5b43a0a5db836ad81797146065777b06a59f90cf1b0' ;; 		armv7) natsArch='arm7'; sha256='b8c83cd825b05d8d0610fc9352804fe810ae6bd9d8f0d814a39b0f152ec2ba79' ;; 		x86_64) natsArch='amd64'; sha256='9550278e34e94aebd410ec401bc145d3538e430ec2a40d5213fffdf9fdd49c27' ;; 		x86) natsArch='386'; sha256='a8ccdd37eac64b031ea96762d7f72a74445e9a708c0363549ba7e119fa79e52c' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 06 Sep 2023 22:39:47 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 06 Sep 2023 22:39:47 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 06 Sep 2023 22:39:47 GMT
EXPOSE 4222 6222 8222
# Wed, 06 Sep 2023 22:39:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 06 Sep 2023 22:39:48 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9fda8d8052c61740409c4bea888859c141fd8cc3f58ac61943144ff6d1681b2d`  
		Last Modified: Mon, 07 Aug 2023 19:39:45 GMT  
		Size: 3.3 MB (3330767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64353667b2ee68f04c527f8dcef72789d979435b90c5b8073485e6c2fcc5c3f7`  
		Last Modified: Wed, 06 Sep 2023 22:40:28 GMT  
		Size: 5.4 MB (5402455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:540b41e481b61500ce8ed1c72cc5c0f937cabb489d0ba9de2dc2dad279696a28`  
		Last Modified: Wed, 06 Sep 2023 22:40:27 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb56160de8c01873d42326860132a0b877e470be0ff76c774c04b542515c9e4a`  
		Last Modified: Wed, 06 Sep 2023 22:40:27 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.22-linux`

```console
$ docker pull nats@sha256:7595e8b87b7063f28ffd3a1f0f7021f6c333fcc17377dbecccd7a6777df7754a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9.22-linux` - linux; amd64

```console
$ docker pull nats@sha256:841691cd373d85dfef90326ad2625e6498d8472d68d7d64b9a7d11b566729e77
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5245280 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7bfd417bdbd2f1eb2b6798d0a0fbba5ce7e3bd1d7ce50d29b8965cb174e801ed`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 06 Sep 2023 23:20:12 GMT
COPY file:acdb0e47969d6e334bcadb9c85dfef3166c764ff4ac55254185a04b1a6e8bbee in /nats-server 
# Wed, 06 Sep 2023 23:20:12 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 06 Sep 2023 23:20:12 GMT
EXPOSE 4222 6222 8222
# Wed, 06 Sep 2023 23:20:12 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 06 Sep 2023 23:20:12 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 06 Sep 2023 23:20:12 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:aac801db9a2a97942dde4494f98ce2d08c529a3af03ecb92f0b93426bbfd6419`  
		Last Modified: Wed, 06 Sep 2023 23:20:56 GMT  
		Size: 5.2 MB (5244773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f86dbe6523f83ad4a9d3f35c66bb097fad7505a3bd4de2123ea173ea21f1e38`  
		Last Modified: Wed, 06 Sep 2023 23:20:55 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.22-linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:ec9d67b684f4605aa5fd2b86b64953bb8062a49d2916cf8e5fab437de945df15
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (4980015 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d632b911d90b9fc8ad6e2d0fd53012e9c8cc6ca17c685d2c8c2a6c4de2cb2c45`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 06 Sep 2023 23:04:49 GMT
COPY file:51aacaba9769a3f16e0467be1fc8eb86122f6f3496e89e41b61e0038083ae308 in /nats-server 
# Wed, 06 Sep 2023 23:04:49 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 06 Sep 2023 23:04:49 GMT
EXPOSE 4222 6222 8222
# Wed, 06 Sep 2023 23:04:49 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 06 Sep 2023 23:04:49 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 06 Sep 2023 23:04:50 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6a6e165fccf6da77ad3b09408162fc7daaafe266b71dd5da8679594aa110a3a5`  
		Last Modified: Wed, 06 Sep 2023 23:05:32 GMT  
		Size: 5.0 MB (4979506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1baf063892d372757ae2be4c42843e0a096826874b64519c230fd85bd65e69e8`  
		Last Modified: Wed, 06 Sep 2023 23:05:31 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.22-linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:58dfaa80e9889d01819641e707279821d96d6f5eb7ce87e29eaa38cd4e0b5cac
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (4970850 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a2d43ddba67d73d9d9c8f19b9fbec53ca1bcb7f04349363538f7d08fd069dbd2`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 06 Sep 2023 22:57:45 GMT
COPY file:aae670bb79c659968f632ae3be388af62614010873ced2a439475906dbb769c6 in /nats-server 
# Wed, 06 Sep 2023 22:57:45 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 06 Sep 2023 22:57:45 GMT
EXPOSE 4222 6222 8222
# Wed, 06 Sep 2023 22:57:45 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 06 Sep 2023 22:57:46 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 06 Sep 2023 22:57:46 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:55b6dbad6639da13368cebb9688e8a5caaee29041e6b5e2e798201dfcf2b67ad`  
		Last Modified: Wed, 06 Sep 2023 22:58:23 GMT  
		Size: 5.0 MB (4970341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f17c52d1a9dd756c463e0590216b217bfee91f63c66217c407f1c98b1ebbc3b9`  
		Last Modified: Wed, 06 Sep 2023 22:58:22 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.22-linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:dd48788f80e3925791e0dddfa44348b7df9022fbc914b20cf00e051a0b3adbf3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.8 MB (4778848 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0e35fd1c4293b595f11452fdc3e7dd6d5d9e033ecc9b1e6a35ff40577f2cba9f`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 06 Sep 2023 22:40:07 GMT
COPY file:d6eca5c67de65d1a8a30a51ea7318b044949c77108b2fdccc5aa0054c068c196 in /nats-server 
# Wed, 06 Sep 2023 22:40:07 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 06 Sep 2023 22:40:07 GMT
EXPOSE 4222 6222 8222
# Wed, 06 Sep 2023 22:40:08 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 06 Sep 2023 22:40:08 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 06 Sep 2023 22:40:08 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:88e5ff7f26ea25c6d2ab092989d9372cb32b3e60880124facfcefd7d3f0b7591`  
		Last Modified: Wed, 06 Sep 2023 22:40:49 GMT  
		Size: 4.8 MB (4778340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7795fd345dfb406d659c2502b733417a10ee85274263050ee36ab4aa021a38d9`  
		Last Modified: Wed, 06 Sep 2023 22:40:48 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.22-nanoserver`

```console
$ docker pull nats@sha256:347c71d5b7499fda4c79d015de6e2b9da4a28374147b6901e02f8e135e482bd1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4737; amd64

### `nats:2.9.22-nanoserver` - windows version 10.0.17763.4737; amd64

```console
$ docker pull nats@sha256:baec10f85f099b828313ff821f20b005907591e2f4fb414c7a240b5944f1292a
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.8 MB (109785996 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3654d1c2e7ef6e2297c519fd991a4a49b4d9928375a1142ec2af9cc55358ee84`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 02 Aug 2023 08:33:47 GMT
RUN Apply image 10.0.17763.4737
# Thu, 10 Aug 2023 02:34:52 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 06 Sep 2023 23:17:32 GMT
RUN cmd /S /C #(nop) COPY file:393d7e944d1b6697a14f19f6cb9673d95da4e1a0fc9508b238325e94beebc857 in C:\nats-server.exe 
# Wed, 06 Sep 2023 23:17:33 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 06 Sep 2023 23:17:34 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 06 Sep 2023 23:17:34 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 06 Sep 2023 23:17:35 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:86fab75eb466cadf89d853682179b3b57eba9fe28c78041dd52bced81e18a627`  
		Last Modified: Tue, 08 Aug 2023 17:55:54 GMT  
		Size: 104.5 MB (104459386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c43534c571f8fdc71038e0f4b4c33a30adb0bbc8b292454d35930557ced33408`  
		Last Modified: Thu, 10 Aug 2023 02:35:37 GMT  
		Size: 1.2 KB (1167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3eade3f0d46f534a5d639c78b1e85a1b0ea96d271fe2c3e706142d2f8d0aef7`  
		Last Modified: Wed, 06 Sep 2023 23:18:18 GMT  
		Size: 5.3 MB (5320148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4eeab0b725b185bf02913419c636eb70964ad972b883ef43006bbf75b1320ece`  
		Last Modified: Wed, 06 Sep 2023 23:18:16 GMT  
		Size: 1.8 KB (1804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c11e5f8af7811e39cecedb8bc4f4533b8f362e497bfe37a943209e0ce0d0bd5`  
		Last Modified: Wed, 06 Sep 2023 23:18:16 GMT  
		Size: 1.2 KB (1161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50806fff52469c9a918b10aa2ed383885dd30e5763ab2157c5440e425ebdccd3`  
		Last Modified: Wed, 06 Sep 2023 23:18:16 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f8c118167fb4c0339d4078748da065ff698f06d9373f7acaa5c42db51dfcdff`  
		Last Modified: Wed, 06 Sep 2023 23:18:16 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.22-nanoserver-1809`

```console
$ docker pull nats@sha256:347c71d5b7499fda4c79d015de6e2b9da4a28374147b6901e02f8e135e482bd1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4737; amd64

### `nats:2.9.22-nanoserver-1809` - windows version 10.0.17763.4737; amd64

```console
$ docker pull nats@sha256:baec10f85f099b828313ff821f20b005907591e2f4fb414c7a240b5944f1292a
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.8 MB (109785996 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3654d1c2e7ef6e2297c519fd991a4a49b4d9928375a1142ec2af9cc55358ee84`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 02 Aug 2023 08:33:47 GMT
RUN Apply image 10.0.17763.4737
# Thu, 10 Aug 2023 02:34:52 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 06 Sep 2023 23:17:32 GMT
RUN cmd /S /C #(nop) COPY file:393d7e944d1b6697a14f19f6cb9673d95da4e1a0fc9508b238325e94beebc857 in C:\nats-server.exe 
# Wed, 06 Sep 2023 23:17:33 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 06 Sep 2023 23:17:34 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 06 Sep 2023 23:17:34 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 06 Sep 2023 23:17:35 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:86fab75eb466cadf89d853682179b3b57eba9fe28c78041dd52bced81e18a627`  
		Last Modified: Tue, 08 Aug 2023 17:55:54 GMT  
		Size: 104.5 MB (104459386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c43534c571f8fdc71038e0f4b4c33a30adb0bbc8b292454d35930557ced33408`  
		Last Modified: Thu, 10 Aug 2023 02:35:37 GMT  
		Size: 1.2 KB (1167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3eade3f0d46f534a5d639c78b1e85a1b0ea96d271fe2c3e706142d2f8d0aef7`  
		Last Modified: Wed, 06 Sep 2023 23:18:18 GMT  
		Size: 5.3 MB (5320148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4eeab0b725b185bf02913419c636eb70964ad972b883ef43006bbf75b1320ece`  
		Last Modified: Wed, 06 Sep 2023 23:18:16 GMT  
		Size: 1.8 KB (1804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c11e5f8af7811e39cecedb8bc4f4533b8f362e497bfe37a943209e0ce0d0bd5`  
		Last Modified: Wed, 06 Sep 2023 23:18:16 GMT  
		Size: 1.2 KB (1161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50806fff52469c9a918b10aa2ed383885dd30e5763ab2157c5440e425ebdccd3`  
		Last Modified: Wed, 06 Sep 2023 23:18:16 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f8c118167fb4c0339d4078748da065ff698f06d9373f7acaa5c42db51dfcdff`  
		Last Modified: Wed, 06 Sep 2023 23:18:16 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.22-scratch`

```console
$ docker pull nats@sha256:7595e8b87b7063f28ffd3a1f0f7021f6c333fcc17377dbecccd7a6777df7754a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9.22-scratch` - linux; amd64

```console
$ docker pull nats@sha256:841691cd373d85dfef90326ad2625e6498d8472d68d7d64b9a7d11b566729e77
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5245280 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7bfd417bdbd2f1eb2b6798d0a0fbba5ce7e3bd1d7ce50d29b8965cb174e801ed`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 06 Sep 2023 23:20:12 GMT
COPY file:acdb0e47969d6e334bcadb9c85dfef3166c764ff4ac55254185a04b1a6e8bbee in /nats-server 
# Wed, 06 Sep 2023 23:20:12 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 06 Sep 2023 23:20:12 GMT
EXPOSE 4222 6222 8222
# Wed, 06 Sep 2023 23:20:12 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 06 Sep 2023 23:20:12 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 06 Sep 2023 23:20:12 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:aac801db9a2a97942dde4494f98ce2d08c529a3af03ecb92f0b93426bbfd6419`  
		Last Modified: Wed, 06 Sep 2023 23:20:56 GMT  
		Size: 5.2 MB (5244773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f86dbe6523f83ad4a9d3f35c66bb097fad7505a3bd4de2123ea173ea21f1e38`  
		Last Modified: Wed, 06 Sep 2023 23:20:55 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.22-scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:ec9d67b684f4605aa5fd2b86b64953bb8062a49d2916cf8e5fab437de945df15
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (4980015 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d632b911d90b9fc8ad6e2d0fd53012e9c8cc6ca17c685d2c8c2a6c4de2cb2c45`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 06 Sep 2023 23:04:49 GMT
COPY file:51aacaba9769a3f16e0467be1fc8eb86122f6f3496e89e41b61e0038083ae308 in /nats-server 
# Wed, 06 Sep 2023 23:04:49 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 06 Sep 2023 23:04:49 GMT
EXPOSE 4222 6222 8222
# Wed, 06 Sep 2023 23:04:49 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 06 Sep 2023 23:04:49 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 06 Sep 2023 23:04:50 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6a6e165fccf6da77ad3b09408162fc7daaafe266b71dd5da8679594aa110a3a5`  
		Last Modified: Wed, 06 Sep 2023 23:05:32 GMT  
		Size: 5.0 MB (4979506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1baf063892d372757ae2be4c42843e0a096826874b64519c230fd85bd65e69e8`  
		Last Modified: Wed, 06 Sep 2023 23:05:31 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.22-scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:58dfaa80e9889d01819641e707279821d96d6f5eb7ce87e29eaa38cd4e0b5cac
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (4970850 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a2d43ddba67d73d9d9c8f19b9fbec53ca1bcb7f04349363538f7d08fd069dbd2`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 06 Sep 2023 22:57:45 GMT
COPY file:aae670bb79c659968f632ae3be388af62614010873ced2a439475906dbb769c6 in /nats-server 
# Wed, 06 Sep 2023 22:57:45 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 06 Sep 2023 22:57:45 GMT
EXPOSE 4222 6222 8222
# Wed, 06 Sep 2023 22:57:45 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 06 Sep 2023 22:57:46 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 06 Sep 2023 22:57:46 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:55b6dbad6639da13368cebb9688e8a5caaee29041e6b5e2e798201dfcf2b67ad`  
		Last Modified: Wed, 06 Sep 2023 22:58:23 GMT  
		Size: 5.0 MB (4970341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f17c52d1a9dd756c463e0590216b217bfee91f63c66217c407f1c98b1ebbc3b9`  
		Last Modified: Wed, 06 Sep 2023 22:58:22 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.22-scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:dd48788f80e3925791e0dddfa44348b7df9022fbc914b20cf00e051a0b3adbf3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.8 MB (4778848 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0e35fd1c4293b595f11452fdc3e7dd6d5d9e033ecc9b1e6a35ff40577f2cba9f`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 06 Sep 2023 22:40:07 GMT
COPY file:d6eca5c67de65d1a8a30a51ea7318b044949c77108b2fdccc5aa0054c068c196 in /nats-server 
# Wed, 06 Sep 2023 22:40:07 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 06 Sep 2023 22:40:07 GMT
EXPOSE 4222 6222 8222
# Wed, 06 Sep 2023 22:40:08 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 06 Sep 2023 22:40:08 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 06 Sep 2023 22:40:08 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:88e5ff7f26ea25c6d2ab092989d9372cb32b3e60880124facfcefd7d3f0b7591`  
		Last Modified: Wed, 06 Sep 2023 22:40:49 GMT  
		Size: 4.8 MB (4778340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7795fd345dfb406d659c2502b733417a10ee85274263050ee36ab4aa021a38d9`  
		Last Modified: Wed, 06 Sep 2023 22:40:48 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.22-windowsservercore`

```console
$ docker pull nats@sha256:df25045f4d70165b54b8b7b0ae443fd21450261550bbc1b314adf8a58053e707
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4737; amd64

### `nats:2.9.22-windowsservercore` - windows version 10.0.17763.4737; amd64

```console
$ docker pull nats@sha256:e2f9912126f4753a9e9312b5dd77a5c5e44c257f28d04ad55cef0662d24138a2
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2001990927 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3cf5f23a9d8d2eca784896bbd09d5e163b27485e7b392cd0bd92f88502dd57b7`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Wed, 02 Aug 2023 09:07:15 GMT
RUN Install update 10.0.17763.4737
# Thu, 10 Aug 2023 01:11:08 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Thu, 10 Aug 2023 02:32:08 GMT
ENV NATS_DOCKERIZED=1
# Wed, 06 Sep 2023 23:15:04 GMT
ENV NATS_SERVER=2.9.22
# Wed, 06 Sep 2023 23:15:05 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.9.22/nats-server-v2.9.22-windows-amd64.zip
# Wed, 06 Sep 2023 23:15:06 GMT
ENV NATS_SERVER_SHASUM=e91db73b02bd4dca3eb7a4bf32e29763450b08d593f73e87d0a6b70102dea0d4
# Wed, 06 Sep 2023 23:15:56 GMT
RUN Set-PSDebug -Trace 2
# Wed, 06 Sep 2023 23:17:21 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 06 Sep 2023 23:17:22 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 06 Sep 2023 23:17:23 GMT
EXPOSE 4222 6222 8222
# Wed, 06 Sep 2023 23:17:24 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 06 Sep 2023 23:17:24 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b95f433aa7d90194e65f6b08a599b3ee12292e124d47c204107baedfd71054c1`  
		Last Modified: Tue, 08 Aug 2023 18:31:16 GMT  
		Size: 345.3 MB (345334986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c5180b8f5f7c2303ba89717cfa778a2173921ca7efdc058cfd6ed951c6d5ca3`  
		Last Modified: Thu, 10 Aug 2023 01:57:18 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fed0c598ca0ae763bd83f045a0c9262bf153a47e508b736992d196e2fb47dea`  
		Last Modified: Thu, 10 Aug 2023 02:35:22 GMT  
		Size: 1.4 KB (1449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab0ebc9f46983ba56ff415cd7b99891210ab8eaad5adf4a15a8f2021de4ebdfd`  
		Last Modified: Wed, 06 Sep 2023 23:18:02 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1c4a22897bb4d3fa0ef4fff463ef850ad45e21404737f120c724fb472c77221`  
		Last Modified: Wed, 06 Sep 2023 23:18:02 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c30142424ff3f45c3c8923f1aa5d959879239599fdde6aba1101c39a168abe48`  
		Last Modified: Wed, 06 Sep 2023 23:18:02 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3723e4e864a2d241c8133b4f1c569ac4ac140d29fe8e216ecd140ebd0e2531cd`  
		Last Modified: Wed, 06 Sep 2023 23:18:02 GMT  
		Size: 242.5 KB (242470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae4c6899207e83d648ab5bf60620507d438b612cb42961f5b8b300c25fde01dd`  
		Last Modified: Wed, 06 Sep 2023 23:18:02 GMT  
		Size: 5.8 MB (5779810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bc2f6a7b18656a6539013442aa6e8c88b49fddce30025ad67ba6e4867a2860b`  
		Last Modified: Wed, 06 Sep 2023 23:18:00 GMT  
		Size: 2.0 KB (1976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ac72b596159b34e1de106133f926192bb5daac9b62301a55822162e6656b6cc`  
		Last Modified: Wed, 06 Sep 2023 23:18:00 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a11a75f33304f42224c3b832462b4497699310fd70a6cdfb322bd126be44cb32`  
		Last Modified: Wed, 06 Sep 2023 23:18:00 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c01b20cb00adae2b356c4377b9419f6a1d18d74692e89c0ee1e66d7b55ca3f3`  
		Last Modified: Wed, 06 Sep 2023 23:18:00 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.22-windowsservercore-1809`

```console
$ docker pull nats@sha256:df25045f4d70165b54b8b7b0ae443fd21450261550bbc1b314adf8a58053e707
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4737; amd64

### `nats:2.9.22-windowsservercore-1809` - windows version 10.0.17763.4737; amd64

```console
$ docker pull nats@sha256:e2f9912126f4753a9e9312b5dd77a5c5e44c257f28d04ad55cef0662d24138a2
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2001990927 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3cf5f23a9d8d2eca784896bbd09d5e163b27485e7b392cd0bd92f88502dd57b7`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Wed, 02 Aug 2023 09:07:15 GMT
RUN Install update 10.0.17763.4737
# Thu, 10 Aug 2023 01:11:08 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Thu, 10 Aug 2023 02:32:08 GMT
ENV NATS_DOCKERIZED=1
# Wed, 06 Sep 2023 23:15:04 GMT
ENV NATS_SERVER=2.9.22
# Wed, 06 Sep 2023 23:15:05 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.9.22/nats-server-v2.9.22-windows-amd64.zip
# Wed, 06 Sep 2023 23:15:06 GMT
ENV NATS_SERVER_SHASUM=e91db73b02bd4dca3eb7a4bf32e29763450b08d593f73e87d0a6b70102dea0d4
# Wed, 06 Sep 2023 23:15:56 GMT
RUN Set-PSDebug -Trace 2
# Wed, 06 Sep 2023 23:17:21 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 06 Sep 2023 23:17:22 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 06 Sep 2023 23:17:23 GMT
EXPOSE 4222 6222 8222
# Wed, 06 Sep 2023 23:17:24 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 06 Sep 2023 23:17:24 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b95f433aa7d90194e65f6b08a599b3ee12292e124d47c204107baedfd71054c1`  
		Last Modified: Tue, 08 Aug 2023 18:31:16 GMT  
		Size: 345.3 MB (345334986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c5180b8f5f7c2303ba89717cfa778a2173921ca7efdc058cfd6ed951c6d5ca3`  
		Last Modified: Thu, 10 Aug 2023 01:57:18 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fed0c598ca0ae763bd83f045a0c9262bf153a47e508b736992d196e2fb47dea`  
		Last Modified: Thu, 10 Aug 2023 02:35:22 GMT  
		Size: 1.4 KB (1449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab0ebc9f46983ba56ff415cd7b99891210ab8eaad5adf4a15a8f2021de4ebdfd`  
		Last Modified: Wed, 06 Sep 2023 23:18:02 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1c4a22897bb4d3fa0ef4fff463ef850ad45e21404737f120c724fb472c77221`  
		Last Modified: Wed, 06 Sep 2023 23:18:02 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c30142424ff3f45c3c8923f1aa5d959879239599fdde6aba1101c39a168abe48`  
		Last Modified: Wed, 06 Sep 2023 23:18:02 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3723e4e864a2d241c8133b4f1c569ac4ac140d29fe8e216ecd140ebd0e2531cd`  
		Last Modified: Wed, 06 Sep 2023 23:18:02 GMT  
		Size: 242.5 KB (242470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae4c6899207e83d648ab5bf60620507d438b612cb42961f5b8b300c25fde01dd`  
		Last Modified: Wed, 06 Sep 2023 23:18:02 GMT  
		Size: 5.8 MB (5779810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bc2f6a7b18656a6539013442aa6e8c88b49fddce30025ad67ba6e4867a2860b`  
		Last Modified: Wed, 06 Sep 2023 23:18:00 GMT  
		Size: 2.0 KB (1976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ac72b596159b34e1de106133f926192bb5daac9b62301a55822162e6656b6cc`  
		Last Modified: Wed, 06 Sep 2023 23:18:00 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a11a75f33304f42224c3b832462b4497699310fd70a6cdfb322bd126be44cb32`  
		Last Modified: Wed, 06 Sep 2023 23:18:00 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c01b20cb00adae2b356c4377b9419f6a1d18d74692e89c0ee1e66d7b55ca3f3`  
		Last Modified: Wed, 06 Sep 2023 23:18:00 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:alpine`

```console
$ docker pull nats@sha256:36d34c59ed76472d9b3caafc5e3764b7a587498808efdd5178468f4efe8b4887
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:alpine` - linux; amd64

```console
$ docker pull nats@sha256:756a55661288407f688c52224ac8b12d008f0fec9343c68281b04bb59cbcc427
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.3 MB (9270382 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dbb9252d07acfbe3ac9083449c0fef74561021019d85c2993f5bce02c7a16201`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:20 GMT
ADD file:32ff5e7a78b890996ee4681cc0a26185d3e9acdb4eb1e2aaccb2411f922fed6b in / 
# Mon, 07 Aug 2023 19:20:20 GMT
CMD ["/bin/sh"]
# Wed, 06 Sep 2023 23:19:53 GMT
ENV NATS_SERVER=2.9.22
# Wed, 06 Sep 2023 23:19:55 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='811e5a3c8187d937a753f182bd5ae2035c91604bda11a3b11023e5eea0504c41' ;; 		armhf) natsArch='arm6'; sha256='4d6f2f8ee9faf43de9fed5b43a0a5db836ad81797146065777b06a59f90cf1b0' ;; 		armv7) natsArch='arm7'; sha256='b8c83cd825b05d8d0610fc9352804fe810ae6bd9d8f0d814a39b0f152ec2ba79' ;; 		x86_64) natsArch='amd64'; sha256='9550278e34e94aebd410ec401bc145d3538e430ec2a40d5213fffdf9fdd49c27' ;; 		x86) natsArch='386'; sha256='a8ccdd37eac64b031ea96762d7f72a74445e9a708c0363549ba7e119fa79e52c' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 06 Sep 2023 23:19:55 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 06 Sep 2023 23:19:55 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 06 Sep 2023 23:19:55 GMT
EXPOSE 4222 6222 8222
# Wed, 06 Sep 2023 23:19:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 06 Sep 2023 23:19:55 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:7264a8db6415046d36d16ba98b79778e18accee6ffa71850405994cffa9be7de`  
		Last Modified: Mon, 07 Aug 2023 19:20:54 GMT  
		Size: 3.4 MB (3401613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75fdd304ec17c2cf1f7629eefc922e04fae260b6d902e4fd42c81a5e5ce9d5dc`  
		Last Modified: Wed, 06 Sep 2023 23:20:32 GMT  
		Size: 5.9 MB (5867770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2863800c65f086f618bf3df0e7855997aea26ba27f4c759cf8bfae94da866bb`  
		Last Modified: Wed, 06 Sep 2023 23:20:31 GMT  
		Size: 585.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e32a641538132ed9885ca87c473fe9ff71415289c1f5276ba1157bb0760bd04`  
		Last Modified: Wed, 06 Sep 2023 23:20:31 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:e66fcde15a5b8028aed7cdd2e03392aa10c4a51c224e964f014eddc1c821433d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.7 MB (8749092 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6e3524e57732f8e26091d551f1b5ce64405e4217d19f047345dc28a29a1b847`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:49:14 GMT
ADD file:9882e99e5f94ab2db05c029648ac5be7cf0f063a8701394fcbb543a7ef5d4b90 in / 
# Mon, 07 Aug 2023 19:49:15 GMT
CMD ["/bin/sh"]
# Wed, 06 Sep 2023 23:04:40 GMT
ENV NATS_SERVER=2.9.22
# Wed, 06 Sep 2023 23:04:43 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='811e5a3c8187d937a753f182bd5ae2035c91604bda11a3b11023e5eea0504c41' ;; 		armhf) natsArch='arm6'; sha256='4d6f2f8ee9faf43de9fed5b43a0a5db836ad81797146065777b06a59f90cf1b0' ;; 		armv7) natsArch='arm7'; sha256='b8c83cd825b05d8d0610fc9352804fe810ae6bd9d8f0d814a39b0f152ec2ba79' ;; 		x86_64) natsArch='amd64'; sha256='9550278e34e94aebd410ec401bc145d3538e430ec2a40d5213fffdf9fdd49c27' ;; 		x86) natsArch='386'; sha256='a8ccdd37eac64b031ea96762d7f72a74445e9a708c0363549ba7e119fa79e52c' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 06 Sep 2023 23:04:43 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 06 Sep 2023 23:04:43 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 06 Sep 2023 23:04:43 GMT
EXPOSE 4222 6222 8222
# Wed, 06 Sep 2023 23:04:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 06 Sep 2023 23:04:43 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:af09961d4a43b504efc76e38b50918977c28be73eeb8b926247783a00e8b9f2f`  
		Last Modified: Mon, 07 Aug 2023 19:49:38 GMT  
		Size: 3.1 MB (3144809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5a6e71bd2ab60e313e659b569f8c33e5e9dcfdb580c25af0f9c5e7eca59f92f`  
		Last Modified: Wed, 06 Sep 2023 23:05:08 GMT  
		Size: 5.6 MB (5603285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7b94c778bbad17cc9be59c68102602e2e77462672d2e045f4713e80ce1cbb1c`  
		Last Modified: Wed, 06 Sep 2023 23:05:07 GMT  
		Size: 585.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4b258e6095309f7819e72dd444d848fe600fb2e73b5bd12bd1e9a556a17bf56`  
		Last Modified: Wed, 06 Sep 2023 23:05:07 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:9ca6685d1ad99fa588f9d4dc05ffe27569ed660b735218fd38795568fe508c73
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.5 MB (8492829 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0271598ef211f3df61073ff64c769275b4bb72b68b984931c8a7af1706fe80c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:57:25 GMT
ADD file:e3f56488d3d3bb67729714db13ddadf6652e7efb5281cfc7010d3e71f9d6607f in / 
# Mon, 07 Aug 2023 19:57:25 GMT
CMD ["/bin/sh"]
# Wed, 06 Sep 2023 22:57:29 GMT
ENV NATS_SERVER=2.9.22
# Wed, 06 Sep 2023 22:57:32 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='811e5a3c8187d937a753f182bd5ae2035c91604bda11a3b11023e5eea0504c41' ;; 		armhf) natsArch='arm6'; sha256='4d6f2f8ee9faf43de9fed5b43a0a5db836ad81797146065777b06a59f90cf1b0' ;; 		armv7) natsArch='arm7'; sha256='b8c83cd825b05d8d0610fc9352804fe810ae6bd9d8f0d814a39b0f152ec2ba79' ;; 		x86_64) natsArch='amd64'; sha256='9550278e34e94aebd410ec401bc145d3538e430ec2a40d5213fffdf9fdd49c27' ;; 		x86) natsArch='386'; sha256='a8ccdd37eac64b031ea96762d7f72a74445e9a708c0363549ba7e119fa79e52c' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 06 Sep 2023 22:57:32 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 06 Sep 2023 22:57:32 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 06 Sep 2023 22:57:32 GMT
EXPOSE 4222 6222 8222
# Wed, 06 Sep 2023 22:57:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 06 Sep 2023 22:57:32 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:f8dec92eec42224ef9e6ca9c6207ea6b9195dcf93d06bd5ceff0f814b62bf064`  
		Last Modified: Mon, 07 Aug 2023 19:57:55 GMT  
		Size: 2.9 MB (2899480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1962026ec365b08ba406dd0e38e57c06dcd04f2225faffcc17883ed87716cdc8`  
		Last Modified: Wed, 06 Sep 2023 22:58:03 GMT  
		Size: 5.6 MB (5592351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:578cf75378460664df525d3b5d1412e778f7b8cdc5f3c31207b3bbc2f6c074f5`  
		Last Modified: Wed, 06 Sep 2023 22:58:01 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64bf3e24d68a6cadd0880ce3163738934bf8e5b267923da68dd6922cd6b98a31`  
		Last Modified: Wed, 06 Sep 2023 22:58:01 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:51e884da4e764cc784998e4bc69bbbefa4f39420be30021b4a1074dc40604423
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.7 MB (8734219 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c8cdff0ce493eb27f871f27f7ec452d1c36de63801fda0b331cd41067f858b9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:19 GMT
ADD file:b2e7eaa7e41f08853dbe08d84439a7f9fd32fc58c3aa1e298f3f60343b2b683a in / 
# Mon, 07 Aug 2023 19:39:19 GMT
CMD ["/bin/sh"]
# Wed, 06 Sep 2023 22:39:45 GMT
ENV NATS_SERVER=2.9.22
# Wed, 06 Sep 2023 22:39:47 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='811e5a3c8187d937a753f182bd5ae2035c91604bda11a3b11023e5eea0504c41' ;; 		armhf) natsArch='arm6'; sha256='4d6f2f8ee9faf43de9fed5b43a0a5db836ad81797146065777b06a59f90cf1b0' ;; 		armv7) natsArch='arm7'; sha256='b8c83cd825b05d8d0610fc9352804fe810ae6bd9d8f0d814a39b0f152ec2ba79' ;; 		x86_64) natsArch='amd64'; sha256='9550278e34e94aebd410ec401bc145d3538e430ec2a40d5213fffdf9fdd49c27' ;; 		x86) natsArch='386'; sha256='a8ccdd37eac64b031ea96762d7f72a74445e9a708c0363549ba7e119fa79e52c' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 06 Sep 2023 22:39:47 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 06 Sep 2023 22:39:47 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 06 Sep 2023 22:39:47 GMT
EXPOSE 4222 6222 8222
# Wed, 06 Sep 2023 22:39:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 06 Sep 2023 22:39:48 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9fda8d8052c61740409c4bea888859c141fd8cc3f58ac61943144ff6d1681b2d`  
		Last Modified: Mon, 07 Aug 2023 19:39:45 GMT  
		Size: 3.3 MB (3330767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64353667b2ee68f04c527f8dcef72789d979435b90c5b8073485e6c2fcc5c3f7`  
		Last Modified: Wed, 06 Sep 2023 22:40:28 GMT  
		Size: 5.4 MB (5402455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:540b41e481b61500ce8ed1c72cc5c0f937cabb489d0ba9de2dc2dad279696a28`  
		Last Modified: Wed, 06 Sep 2023 22:40:27 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb56160de8c01873d42326860132a0b877e470be0ff76c774c04b542515c9e4a`  
		Last Modified: Wed, 06 Sep 2023 22:40:27 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:alpine3.18`

```console
$ docker pull nats@sha256:36d34c59ed76472d9b3caafc5e3764b7a587498808efdd5178468f4efe8b4887
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:alpine3.18` - linux; amd64

```console
$ docker pull nats@sha256:756a55661288407f688c52224ac8b12d008f0fec9343c68281b04bb59cbcc427
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.3 MB (9270382 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dbb9252d07acfbe3ac9083449c0fef74561021019d85c2993f5bce02c7a16201`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:20 GMT
ADD file:32ff5e7a78b890996ee4681cc0a26185d3e9acdb4eb1e2aaccb2411f922fed6b in / 
# Mon, 07 Aug 2023 19:20:20 GMT
CMD ["/bin/sh"]
# Wed, 06 Sep 2023 23:19:53 GMT
ENV NATS_SERVER=2.9.22
# Wed, 06 Sep 2023 23:19:55 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='811e5a3c8187d937a753f182bd5ae2035c91604bda11a3b11023e5eea0504c41' ;; 		armhf) natsArch='arm6'; sha256='4d6f2f8ee9faf43de9fed5b43a0a5db836ad81797146065777b06a59f90cf1b0' ;; 		armv7) natsArch='arm7'; sha256='b8c83cd825b05d8d0610fc9352804fe810ae6bd9d8f0d814a39b0f152ec2ba79' ;; 		x86_64) natsArch='amd64'; sha256='9550278e34e94aebd410ec401bc145d3538e430ec2a40d5213fffdf9fdd49c27' ;; 		x86) natsArch='386'; sha256='a8ccdd37eac64b031ea96762d7f72a74445e9a708c0363549ba7e119fa79e52c' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 06 Sep 2023 23:19:55 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 06 Sep 2023 23:19:55 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 06 Sep 2023 23:19:55 GMT
EXPOSE 4222 6222 8222
# Wed, 06 Sep 2023 23:19:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 06 Sep 2023 23:19:55 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:7264a8db6415046d36d16ba98b79778e18accee6ffa71850405994cffa9be7de`  
		Last Modified: Mon, 07 Aug 2023 19:20:54 GMT  
		Size: 3.4 MB (3401613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75fdd304ec17c2cf1f7629eefc922e04fae260b6d902e4fd42c81a5e5ce9d5dc`  
		Last Modified: Wed, 06 Sep 2023 23:20:32 GMT  
		Size: 5.9 MB (5867770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2863800c65f086f618bf3df0e7855997aea26ba27f4c759cf8bfae94da866bb`  
		Last Modified: Wed, 06 Sep 2023 23:20:31 GMT  
		Size: 585.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e32a641538132ed9885ca87c473fe9ff71415289c1f5276ba1157bb0760bd04`  
		Last Modified: Wed, 06 Sep 2023 23:20:31 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.18` - linux; arm variant v6

```console
$ docker pull nats@sha256:e66fcde15a5b8028aed7cdd2e03392aa10c4a51c224e964f014eddc1c821433d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.7 MB (8749092 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6e3524e57732f8e26091d551f1b5ce64405e4217d19f047345dc28a29a1b847`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:49:14 GMT
ADD file:9882e99e5f94ab2db05c029648ac5be7cf0f063a8701394fcbb543a7ef5d4b90 in / 
# Mon, 07 Aug 2023 19:49:15 GMT
CMD ["/bin/sh"]
# Wed, 06 Sep 2023 23:04:40 GMT
ENV NATS_SERVER=2.9.22
# Wed, 06 Sep 2023 23:04:43 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='811e5a3c8187d937a753f182bd5ae2035c91604bda11a3b11023e5eea0504c41' ;; 		armhf) natsArch='arm6'; sha256='4d6f2f8ee9faf43de9fed5b43a0a5db836ad81797146065777b06a59f90cf1b0' ;; 		armv7) natsArch='arm7'; sha256='b8c83cd825b05d8d0610fc9352804fe810ae6bd9d8f0d814a39b0f152ec2ba79' ;; 		x86_64) natsArch='amd64'; sha256='9550278e34e94aebd410ec401bc145d3538e430ec2a40d5213fffdf9fdd49c27' ;; 		x86) natsArch='386'; sha256='a8ccdd37eac64b031ea96762d7f72a74445e9a708c0363549ba7e119fa79e52c' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 06 Sep 2023 23:04:43 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 06 Sep 2023 23:04:43 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 06 Sep 2023 23:04:43 GMT
EXPOSE 4222 6222 8222
# Wed, 06 Sep 2023 23:04:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 06 Sep 2023 23:04:43 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:af09961d4a43b504efc76e38b50918977c28be73eeb8b926247783a00e8b9f2f`  
		Last Modified: Mon, 07 Aug 2023 19:49:38 GMT  
		Size: 3.1 MB (3144809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5a6e71bd2ab60e313e659b569f8c33e5e9dcfdb580c25af0f9c5e7eca59f92f`  
		Last Modified: Wed, 06 Sep 2023 23:05:08 GMT  
		Size: 5.6 MB (5603285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7b94c778bbad17cc9be59c68102602e2e77462672d2e045f4713e80ce1cbb1c`  
		Last Modified: Wed, 06 Sep 2023 23:05:07 GMT  
		Size: 585.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4b258e6095309f7819e72dd444d848fe600fb2e73b5bd12bd1e9a556a17bf56`  
		Last Modified: Wed, 06 Sep 2023 23:05:07 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.18` - linux; arm variant v7

```console
$ docker pull nats@sha256:9ca6685d1ad99fa588f9d4dc05ffe27569ed660b735218fd38795568fe508c73
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.5 MB (8492829 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0271598ef211f3df61073ff64c769275b4bb72b68b984931c8a7af1706fe80c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:57:25 GMT
ADD file:e3f56488d3d3bb67729714db13ddadf6652e7efb5281cfc7010d3e71f9d6607f in / 
# Mon, 07 Aug 2023 19:57:25 GMT
CMD ["/bin/sh"]
# Wed, 06 Sep 2023 22:57:29 GMT
ENV NATS_SERVER=2.9.22
# Wed, 06 Sep 2023 22:57:32 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='811e5a3c8187d937a753f182bd5ae2035c91604bda11a3b11023e5eea0504c41' ;; 		armhf) natsArch='arm6'; sha256='4d6f2f8ee9faf43de9fed5b43a0a5db836ad81797146065777b06a59f90cf1b0' ;; 		armv7) natsArch='arm7'; sha256='b8c83cd825b05d8d0610fc9352804fe810ae6bd9d8f0d814a39b0f152ec2ba79' ;; 		x86_64) natsArch='amd64'; sha256='9550278e34e94aebd410ec401bc145d3538e430ec2a40d5213fffdf9fdd49c27' ;; 		x86) natsArch='386'; sha256='a8ccdd37eac64b031ea96762d7f72a74445e9a708c0363549ba7e119fa79e52c' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 06 Sep 2023 22:57:32 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 06 Sep 2023 22:57:32 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 06 Sep 2023 22:57:32 GMT
EXPOSE 4222 6222 8222
# Wed, 06 Sep 2023 22:57:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 06 Sep 2023 22:57:32 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:f8dec92eec42224ef9e6ca9c6207ea6b9195dcf93d06bd5ceff0f814b62bf064`  
		Last Modified: Mon, 07 Aug 2023 19:57:55 GMT  
		Size: 2.9 MB (2899480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1962026ec365b08ba406dd0e38e57c06dcd04f2225faffcc17883ed87716cdc8`  
		Last Modified: Wed, 06 Sep 2023 22:58:03 GMT  
		Size: 5.6 MB (5592351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:578cf75378460664df525d3b5d1412e778f7b8cdc5f3c31207b3bbc2f6c074f5`  
		Last Modified: Wed, 06 Sep 2023 22:58:01 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64bf3e24d68a6cadd0880ce3163738934bf8e5b267923da68dd6922cd6b98a31`  
		Last Modified: Wed, 06 Sep 2023 22:58:01 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.18` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:51e884da4e764cc784998e4bc69bbbefa4f39420be30021b4a1074dc40604423
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.7 MB (8734219 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c8cdff0ce493eb27f871f27f7ec452d1c36de63801fda0b331cd41067f858b9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:19 GMT
ADD file:b2e7eaa7e41f08853dbe08d84439a7f9fd32fc58c3aa1e298f3f60343b2b683a in / 
# Mon, 07 Aug 2023 19:39:19 GMT
CMD ["/bin/sh"]
# Wed, 06 Sep 2023 22:39:45 GMT
ENV NATS_SERVER=2.9.22
# Wed, 06 Sep 2023 22:39:47 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='811e5a3c8187d937a753f182bd5ae2035c91604bda11a3b11023e5eea0504c41' ;; 		armhf) natsArch='arm6'; sha256='4d6f2f8ee9faf43de9fed5b43a0a5db836ad81797146065777b06a59f90cf1b0' ;; 		armv7) natsArch='arm7'; sha256='b8c83cd825b05d8d0610fc9352804fe810ae6bd9d8f0d814a39b0f152ec2ba79' ;; 		x86_64) natsArch='amd64'; sha256='9550278e34e94aebd410ec401bc145d3538e430ec2a40d5213fffdf9fdd49c27' ;; 		x86) natsArch='386'; sha256='a8ccdd37eac64b031ea96762d7f72a74445e9a708c0363549ba7e119fa79e52c' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 06 Sep 2023 22:39:47 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 06 Sep 2023 22:39:47 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 06 Sep 2023 22:39:47 GMT
EXPOSE 4222 6222 8222
# Wed, 06 Sep 2023 22:39:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 06 Sep 2023 22:39:48 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9fda8d8052c61740409c4bea888859c141fd8cc3f58ac61943144ff6d1681b2d`  
		Last Modified: Mon, 07 Aug 2023 19:39:45 GMT  
		Size: 3.3 MB (3330767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64353667b2ee68f04c527f8dcef72789d979435b90c5b8073485e6c2fcc5c3f7`  
		Last Modified: Wed, 06 Sep 2023 22:40:28 GMT  
		Size: 5.4 MB (5402455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:540b41e481b61500ce8ed1c72cc5c0f937cabb489d0ba9de2dc2dad279696a28`  
		Last Modified: Wed, 06 Sep 2023 22:40:27 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb56160de8c01873d42326860132a0b877e470be0ff76c774c04b542515c9e4a`  
		Last Modified: Wed, 06 Sep 2023 22:40:27 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:latest`

```console
$ docker pull nats@sha256:70a536ddc540ab27ecf4ea6666bf495473a11f408d17bb694008fec41f3c4e87
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.4737; amd64

### `nats:latest` - linux; amd64

```console
$ docker pull nats@sha256:841691cd373d85dfef90326ad2625e6498d8472d68d7d64b9a7d11b566729e77
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5245280 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7bfd417bdbd2f1eb2b6798d0a0fbba5ce7e3bd1d7ce50d29b8965cb174e801ed`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 06 Sep 2023 23:20:12 GMT
COPY file:acdb0e47969d6e334bcadb9c85dfef3166c764ff4ac55254185a04b1a6e8bbee in /nats-server 
# Wed, 06 Sep 2023 23:20:12 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 06 Sep 2023 23:20:12 GMT
EXPOSE 4222 6222 8222
# Wed, 06 Sep 2023 23:20:12 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 06 Sep 2023 23:20:12 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 06 Sep 2023 23:20:12 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:aac801db9a2a97942dde4494f98ce2d08c529a3af03ecb92f0b93426bbfd6419`  
		Last Modified: Wed, 06 Sep 2023 23:20:56 GMT  
		Size: 5.2 MB (5244773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f86dbe6523f83ad4a9d3f35c66bb097fad7505a3bd4de2123ea173ea21f1e38`  
		Last Modified: Wed, 06 Sep 2023 23:20:55 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm variant v6

```console
$ docker pull nats@sha256:ec9d67b684f4605aa5fd2b86b64953bb8062a49d2916cf8e5fab437de945df15
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (4980015 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d632b911d90b9fc8ad6e2d0fd53012e9c8cc6ca17c685d2c8c2a6c4de2cb2c45`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 06 Sep 2023 23:04:49 GMT
COPY file:51aacaba9769a3f16e0467be1fc8eb86122f6f3496e89e41b61e0038083ae308 in /nats-server 
# Wed, 06 Sep 2023 23:04:49 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 06 Sep 2023 23:04:49 GMT
EXPOSE 4222 6222 8222
# Wed, 06 Sep 2023 23:04:49 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 06 Sep 2023 23:04:49 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 06 Sep 2023 23:04:50 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6a6e165fccf6da77ad3b09408162fc7daaafe266b71dd5da8679594aa110a3a5`  
		Last Modified: Wed, 06 Sep 2023 23:05:32 GMT  
		Size: 5.0 MB (4979506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1baf063892d372757ae2be4c42843e0a096826874b64519c230fd85bd65e69e8`  
		Last Modified: Wed, 06 Sep 2023 23:05:31 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm variant v7

```console
$ docker pull nats@sha256:58dfaa80e9889d01819641e707279821d96d6f5eb7ce87e29eaa38cd4e0b5cac
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (4970850 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a2d43ddba67d73d9d9c8f19b9fbec53ca1bcb7f04349363538f7d08fd069dbd2`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 06 Sep 2023 22:57:45 GMT
COPY file:aae670bb79c659968f632ae3be388af62614010873ced2a439475906dbb769c6 in /nats-server 
# Wed, 06 Sep 2023 22:57:45 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 06 Sep 2023 22:57:45 GMT
EXPOSE 4222 6222 8222
# Wed, 06 Sep 2023 22:57:45 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 06 Sep 2023 22:57:46 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 06 Sep 2023 22:57:46 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:55b6dbad6639da13368cebb9688e8a5caaee29041e6b5e2e798201dfcf2b67ad`  
		Last Modified: Wed, 06 Sep 2023 22:58:23 GMT  
		Size: 5.0 MB (4970341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f17c52d1a9dd756c463e0590216b217bfee91f63c66217c407f1c98b1ebbc3b9`  
		Last Modified: Wed, 06 Sep 2023 22:58:22 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:dd48788f80e3925791e0dddfa44348b7df9022fbc914b20cf00e051a0b3adbf3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.8 MB (4778848 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0e35fd1c4293b595f11452fdc3e7dd6d5d9e033ecc9b1e6a35ff40577f2cba9f`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 06 Sep 2023 22:40:07 GMT
COPY file:d6eca5c67de65d1a8a30a51ea7318b044949c77108b2fdccc5aa0054c068c196 in /nats-server 
# Wed, 06 Sep 2023 22:40:07 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 06 Sep 2023 22:40:07 GMT
EXPOSE 4222 6222 8222
# Wed, 06 Sep 2023 22:40:08 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 06 Sep 2023 22:40:08 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 06 Sep 2023 22:40:08 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:88e5ff7f26ea25c6d2ab092989d9372cb32b3e60880124facfcefd7d3f0b7591`  
		Last Modified: Wed, 06 Sep 2023 22:40:49 GMT  
		Size: 4.8 MB (4778340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7795fd345dfb406d659c2502b733417a10ee85274263050ee36ab4aa021a38d9`  
		Last Modified: Wed, 06 Sep 2023 22:40:48 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - windows version 10.0.17763.4737; amd64

```console
$ docker pull nats@sha256:baec10f85f099b828313ff821f20b005907591e2f4fb414c7a240b5944f1292a
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.8 MB (109785996 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3654d1c2e7ef6e2297c519fd991a4a49b4d9928375a1142ec2af9cc55358ee84`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 02 Aug 2023 08:33:47 GMT
RUN Apply image 10.0.17763.4737
# Thu, 10 Aug 2023 02:34:52 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 06 Sep 2023 23:17:32 GMT
RUN cmd /S /C #(nop) COPY file:393d7e944d1b6697a14f19f6cb9673d95da4e1a0fc9508b238325e94beebc857 in C:\nats-server.exe 
# Wed, 06 Sep 2023 23:17:33 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 06 Sep 2023 23:17:34 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 06 Sep 2023 23:17:34 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 06 Sep 2023 23:17:35 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:86fab75eb466cadf89d853682179b3b57eba9fe28c78041dd52bced81e18a627`  
		Last Modified: Tue, 08 Aug 2023 17:55:54 GMT  
		Size: 104.5 MB (104459386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c43534c571f8fdc71038e0f4b4c33a30adb0bbc8b292454d35930557ced33408`  
		Last Modified: Thu, 10 Aug 2023 02:35:37 GMT  
		Size: 1.2 KB (1167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3eade3f0d46f534a5d639c78b1e85a1b0ea96d271fe2c3e706142d2f8d0aef7`  
		Last Modified: Wed, 06 Sep 2023 23:18:18 GMT  
		Size: 5.3 MB (5320148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4eeab0b725b185bf02913419c636eb70964ad972b883ef43006bbf75b1320ece`  
		Last Modified: Wed, 06 Sep 2023 23:18:16 GMT  
		Size: 1.8 KB (1804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c11e5f8af7811e39cecedb8bc4f4533b8f362e497bfe37a943209e0ce0d0bd5`  
		Last Modified: Wed, 06 Sep 2023 23:18:16 GMT  
		Size: 1.2 KB (1161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50806fff52469c9a918b10aa2ed383885dd30e5763ab2157c5440e425ebdccd3`  
		Last Modified: Wed, 06 Sep 2023 23:18:16 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f8c118167fb4c0339d4078748da065ff698f06d9373f7acaa5c42db51dfcdff`  
		Last Modified: Wed, 06 Sep 2023 23:18:16 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:linux`

```console
$ docker pull nats@sha256:7595e8b87b7063f28ffd3a1f0f7021f6c333fcc17377dbecccd7a6777df7754a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:linux` - linux; amd64

```console
$ docker pull nats@sha256:841691cd373d85dfef90326ad2625e6498d8472d68d7d64b9a7d11b566729e77
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5245280 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7bfd417bdbd2f1eb2b6798d0a0fbba5ce7e3bd1d7ce50d29b8965cb174e801ed`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 06 Sep 2023 23:20:12 GMT
COPY file:acdb0e47969d6e334bcadb9c85dfef3166c764ff4ac55254185a04b1a6e8bbee in /nats-server 
# Wed, 06 Sep 2023 23:20:12 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 06 Sep 2023 23:20:12 GMT
EXPOSE 4222 6222 8222
# Wed, 06 Sep 2023 23:20:12 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 06 Sep 2023 23:20:12 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 06 Sep 2023 23:20:12 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:aac801db9a2a97942dde4494f98ce2d08c529a3af03ecb92f0b93426bbfd6419`  
		Last Modified: Wed, 06 Sep 2023 23:20:56 GMT  
		Size: 5.2 MB (5244773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f86dbe6523f83ad4a9d3f35c66bb097fad7505a3bd4de2123ea173ea21f1e38`  
		Last Modified: Wed, 06 Sep 2023 23:20:55 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:ec9d67b684f4605aa5fd2b86b64953bb8062a49d2916cf8e5fab437de945df15
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (4980015 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d632b911d90b9fc8ad6e2d0fd53012e9c8cc6ca17c685d2c8c2a6c4de2cb2c45`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 06 Sep 2023 23:04:49 GMT
COPY file:51aacaba9769a3f16e0467be1fc8eb86122f6f3496e89e41b61e0038083ae308 in /nats-server 
# Wed, 06 Sep 2023 23:04:49 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 06 Sep 2023 23:04:49 GMT
EXPOSE 4222 6222 8222
# Wed, 06 Sep 2023 23:04:49 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 06 Sep 2023 23:04:49 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 06 Sep 2023 23:04:50 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6a6e165fccf6da77ad3b09408162fc7daaafe266b71dd5da8679594aa110a3a5`  
		Last Modified: Wed, 06 Sep 2023 23:05:32 GMT  
		Size: 5.0 MB (4979506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1baf063892d372757ae2be4c42843e0a096826874b64519c230fd85bd65e69e8`  
		Last Modified: Wed, 06 Sep 2023 23:05:31 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:58dfaa80e9889d01819641e707279821d96d6f5eb7ce87e29eaa38cd4e0b5cac
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (4970850 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a2d43ddba67d73d9d9c8f19b9fbec53ca1bcb7f04349363538f7d08fd069dbd2`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 06 Sep 2023 22:57:45 GMT
COPY file:aae670bb79c659968f632ae3be388af62614010873ced2a439475906dbb769c6 in /nats-server 
# Wed, 06 Sep 2023 22:57:45 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 06 Sep 2023 22:57:45 GMT
EXPOSE 4222 6222 8222
# Wed, 06 Sep 2023 22:57:45 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 06 Sep 2023 22:57:46 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 06 Sep 2023 22:57:46 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:55b6dbad6639da13368cebb9688e8a5caaee29041e6b5e2e798201dfcf2b67ad`  
		Last Modified: Wed, 06 Sep 2023 22:58:23 GMT  
		Size: 5.0 MB (4970341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f17c52d1a9dd756c463e0590216b217bfee91f63c66217c407f1c98b1ebbc3b9`  
		Last Modified: Wed, 06 Sep 2023 22:58:22 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:dd48788f80e3925791e0dddfa44348b7df9022fbc914b20cf00e051a0b3adbf3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.8 MB (4778848 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0e35fd1c4293b595f11452fdc3e7dd6d5d9e033ecc9b1e6a35ff40577f2cba9f`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 06 Sep 2023 22:40:07 GMT
COPY file:d6eca5c67de65d1a8a30a51ea7318b044949c77108b2fdccc5aa0054c068c196 in /nats-server 
# Wed, 06 Sep 2023 22:40:07 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 06 Sep 2023 22:40:07 GMT
EXPOSE 4222 6222 8222
# Wed, 06 Sep 2023 22:40:08 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 06 Sep 2023 22:40:08 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 06 Sep 2023 22:40:08 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:88e5ff7f26ea25c6d2ab092989d9372cb32b3e60880124facfcefd7d3f0b7591`  
		Last Modified: Wed, 06 Sep 2023 22:40:49 GMT  
		Size: 4.8 MB (4778340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7795fd345dfb406d659c2502b733417a10ee85274263050ee36ab4aa021a38d9`  
		Last Modified: Wed, 06 Sep 2023 22:40:48 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:nanoserver`

```console
$ docker pull nats@sha256:347c71d5b7499fda4c79d015de6e2b9da4a28374147b6901e02f8e135e482bd1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4737; amd64

### `nats:nanoserver` - windows version 10.0.17763.4737; amd64

```console
$ docker pull nats@sha256:baec10f85f099b828313ff821f20b005907591e2f4fb414c7a240b5944f1292a
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.8 MB (109785996 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3654d1c2e7ef6e2297c519fd991a4a49b4d9928375a1142ec2af9cc55358ee84`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 02 Aug 2023 08:33:47 GMT
RUN Apply image 10.0.17763.4737
# Thu, 10 Aug 2023 02:34:52 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 06 Sep 2023 23:17:32 GMT
RUN cmd /S /C #(nop) COPY file:393d7e944d1b6697a14f19f6cb9673d95da4e1a0fc9508b238325e94beebc857 in C:\nats-server.exe 
# Wed, 06 Sep 2023 23:17:33 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 06 Sep 2023 23:17:34 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 06 Sep 2023 23:17:34 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 06 Sep 2023 23:17:35 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:86fab75eb466cadf89d853682179b3b57eba9fe28c78041dd52bced81e18a627`  
		Last Modified: Tue, 08 Aug 2023 17:55:54 GMT  
		Size: 104.5 MB (104459386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c43534c571f8fdc71038e0f4b4c33a30adb0bbc8b292454d35930557ced33408`  
		Last Modified: Thu, 10 Aug 2023 02:35:37 GMT  
		Size: 1.2 KB (1167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3eade3f0d46f534a5d639c78b1e85a1b0ea96d271fe2c3e706142d2f8d0aef7`  
		Last Modified: Wed, 06 Sep 2023 23:18:18 GMT  
		Size: 5.3 MB (5320148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4eeab0b725b185bf02913419c636eb70964ad972b883ef43006bbf75b1320ece`  
		Last Modified: Wed, 06 Sep 2023 23:18:16 GMT  
		Size: 1.8 KB (1804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c11e5f8af7811e39cecedb8bc4f4533b8f362e497bfe37a943209e0ce0d0bd5`  
		Last Modified: Wed, 06 Sep 2023 23:18:16 GMT  
		Size: 1.2 KB (1161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50806fff52469c9a918b10aa2ed383885dd30e5763ab2157c5440e425ebdccd3`  
		Last Modified: Wed, 06 Sep 2023 23:18:16 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f8c118167fb4c0339d4078748da065ff698f06d9373f7acaa5c42db51dfcdff`  
		Last Modified: Wed, 06 Sep 2023 23:18:16 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:nanoserver-1809`

```console
$ docker pull nats@sha256:347c71d5b7499fda4c79d015de6e2b9da4a28374147b6901e02f8e135e482bd1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4737; amd64

### `nats:nanoserver-1809` - windows version 10.0.17763.4737; amd64

```console
$ docker pull nats@sha256:baec10f85f099b828313ff821f20b005907591e2f4fb414c7a240b5944f1292a
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.8 MB (109785996 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3654d1c2e7ef6e2297c519fd991a4a49b4d9928375a1142ec2af9cc55358ee84`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 02 Aug 2023 08:33:47 GMT
RUN Apply image 10.0.17763.4737
# Thu, 10 Aug 2023 02:34:52 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 06 Sep 2023 23:17:32 GMT
RUN cmd /S /C #(nop) COPY file:393d7e944d1b6697a14f19f6cb9673d95da4e1a0fc9508b238325e94beebc857 in C:\nats-server.exe 
# Wed, 06 Sep 2023 23:17:33 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 06 Sep 2023 23:17:34 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 06 Sep 2023 23:17:34 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 06 Sep 2023 23:17:35 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:86fab75eb466cadf89d853682179b3b57eba9fe28c78041dd52bced81e18a627`  
		Last Modified: Tue, 08 Aug 2023 17:55:54 GMT  
		Size: 104.5 MB (104459386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c43534c571f8fdc71038e0f4b4c33a30adb0bbc8b292454d35930557ced33408`  
		Last Modified: Thu, 10 Aug 2023 02:35:37 GMT  
		Size: 1.2 KB (1167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3eade3f0d46f534a5d639c78b1e85a1b0ea96d271fe2c3e706142d2f8d0aef7`  
		Last Modified: Wed, 06 Sep 2023 23:18:18 GMT  
		Size: 5.3 MB (5320148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4eeab0b725b185bf02913419c636eb70964ad972b883ef43006bbf75b1320ece`  
		Last Modified: Wed, 06 Sep 2023 23:18:16 GMT  
		Size: 1.8 KB (1804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c11e5f8af7811e39cecedb8bc4f4533b8f362e497bfe37a943209e0ce0d0bd5`  
		Last Modified: Wed, 06 Sep 2023 23:18:16 GMT  
		Size: 1.2 KB (1161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50806fff52469c9a918b10aa2ed383885dd30e5763ab2157c5440e425ebdccd3`  
		Last Modified: Wed, 06 Sep 2023 23:18:16 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f8c118167fb4c0339d4078748da065ff698f06d9373f7acaa5c42db51dfcdff`  
		Last Modified: Wed, 06 Sep 2023 23:18:16 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:scratch`

```console
$ docker pull nats@sha256:7595e8b87b7063f28ffd3a1f0f7021f6c333fcc17377dbecccd7a6777df7754a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:scratch` - linux; amd64

```console
$ docker pull nats@sha256:841691cd373d85dfef90326ad2625e6498d8472d68d7d64b9a7d11b566729e77
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5245280 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7bfd417bdbd2f1eb2b6798d0a0fbba5ce7e3bd1d7ce50d29b8965cb174e801ed`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 06 Sep 2023 23:20:12 GMT
COPY file:acdb0e47969d6e334bcadb9c85dfef3166c764ff4ac55254185a04b1a6e8bbee in /nats-server 
# Wed, 06 Sep 2023 23:20:12 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 06 Sep 2023 23:20:12 GMT
EXPOSE 4222 6222 8222
# Wed, 06 Sep 2023 23:20:12 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 06 Sep 2023 23:20:12 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 06 Sep 2023 23:20:12 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:aac801db9a2a97942dde4494f98ce2d08c529a3af03ecb92f0b93426bbfd6419`  
		Last Modified: Wed, 06 Sep 2023 23:20:56 GMT  
		Size: 5.2 MB (5244773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f86dbe6523f83ad4a9d3f35c66bb097fad7505a3bd4de2123ea173ea21f1e38`  
		Last Modified: Wed, 06 Sep 2023 23:20:55 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:ec9d67b684f4605aa5fd2b86b64953bb8062a49d2916cf8e5fab437de945df15
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (4980015 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d632b911d90b9fc8ad6e2d0fd53012e9c8cc6ca17c685d2c8c2a6c4de2cb2c45`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 06 Sep 2023 23:04:49 GMT
COPY file:51aacaba9769a3f16e0467be1fc8eb86122f6f3496e89e41b61e0038083ae308 in /nats-server 
# Wed, 06 Sep 2023 23:04:49 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 06 Sep 2023 23:04:49 GMT
EXPOSE 4222 6222 8222
# Wed, 06 Sep 2023 23:04:49 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 06 Sep 2023 23:04:49 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 06 Sep 2023 23:04:50 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6a6e165fccf6da77ad3b09408162fc7daaafe266b71dd5da8679594aa110a3a5`  
		Last Modified: Wed, 06 Sep 2023 23:05:32 GMT  
		Size: 5.0 MB (4979506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1baf063892d372757ae2be4c42843e0a096826874b64519c230fd85bd65e69e8`  
		Last Modified: Wed, 06 Sep 2023 23:05:31 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:58dfaa80e9889d01819641e707279821d96d6f5eb7ce87e29eaa38cd4e0b5cac
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (4970850 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a2d43ddba67d73d9d9c8f19b9fbec53ca1bcb7f04349363538f7d08fd069dbd2`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 06 Sep 2023 22:57:45 GMT
COPY file:aae670bb79c659968f632ae3be388af62614010873ced2a439475906dbb769c6 in /nats-server 
# Wed, 06 Sep 2023 22:57:45 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 06 Sep 2023 22:57:45 GMT
EXPOSE 4222 6222 8222
# Wed, 06 Sep 2023 22:57:45 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 06 Sep 2023 22:57:46 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 06 Sep 2023 22:57:46 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:55b6dbad6639da13368cebb9688e8a5caaee29041e6b5e2e798201dfcf2b67ad`  
		Last Modified: Wed, 06 Sep 2023 22:58:23 GMT  
		Size: 5.0 MB (4970341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f17c52d1a9dd756c463e0590216b217bfee91f63c66217c407f1c98b1ebbc3b9`  
		Last Modified: Wed, 06 Sep 2023 22:58:22 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:dd48788f80e3925791e0dddfa44348b7df9022fbc914b20cf00e051a0b3adbf3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.8 MB (4778848 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0e35fd1c4293b595f11452fdc3e7dd6d5d9e033ecc9b1e6a35ff40577f2cba9f`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 06 Sep 2023 22:40:07 GMT
COPY file:d6eca5c67de65d1a8a30a51ea7318b044949c77108b2fdccc5aa0054c068c196 in /nats-server 
# Wed, 06 Sep 2023 22:40:07 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 06 Sep 2023 22:40:07 GMT
EXPOSE 4222 6222 8222
# Wed, 06 Sep 2023 22:40:08 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 06 Sep 2023 22:40:08 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 06 Sep 2023 22:40:08 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:88e5ff7f26ea25c6d2ab092989d9372cb32b3e60880124facfcefd7d3f0b7591`  
		Last Modified: Wed, 06 Sep 2023 22:40:49 GMT  
		Size: 4.8 MB (4778340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7795fd345dfb406d659c2502b733417a10ee85274263050ee36ab4aa021a38d9`  
		Last Modified: Wed, 06 Sep 2023 22:40:48 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:windowsservercore`

```console
$ docker pull nats@sha256:df25045f4d70165b54b8b7b0ae443fd21450261550bbc1b314adf8a58053e707
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4737; amd64

### `nats:windowsservercore` - windows version 10.0.17763.4737; amd64

```console
$ docker pull nats@sha256:e2f9912126f4753a9e9312b5dd77a5c5e44c257f28d04ad55cef0662d24138a2
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2001990927 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3cf5f23a9d8d2eca784896bbd09d5e163b27485e7b392cd0bd92f88502dd57b7`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Wed, 02 Aug 2023 09:07:15 GMT
RUN Install update 10.0.17763.4737
# Thu, 10 Aug 2023 01:11:08 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Thu, 10 Aug 2023 02:32:08 GMT
ENV NATS_DOCKERIZED=1
# Wed, 06 Sep 2023 23:15:04 GMT
ENV NATS_SERVER=2.9.22
# Wed, 06 Sep 2023 23:15:05 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.9.22/nats-server-v2.9.22-windows-amd64.zip
# Wed, 06 Sep 2023 23:15:06 GMT
ENV NATS_SERVER_SHASUM=e91db73b02bd4dca3eb7a4bf32e29763450b08d593f73e87d0a6b70102dea0d4
# Wed, 06 Sep 2023 23:15:56 GMT
RUN Set-PSDebug -Trace 2
# Wed, 06 Sep 2023 23:17:21 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 06 Sep 2023 23:17:22 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 06 Sep 2023 23:17:23 GMT
EXPOSE 4222 6222 8222
# Wed, 06 Sep 2023 23:17:24 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 06 Sep 2023 23:17:24 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b95f433aa7d90194e65f6b08a599b3ee12292e124d47c204107baedfd71054c1`  
		Last Modified: Tue, 08 Aug 2023 18:31:16 GMT  
		Size: 345.3 MB (345334986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c5180b8f5f7c2303ba89717cfa778a2173921ca7efdc058cfd6ed951c6d5ca3`  
		Last Modified: Thu, 10 Aug 2023 01:57:18 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fed0c598ca0ae763bd83f045a0c9262bf153a47e508b736992d196e2fb47dea`  
		Last Modified: Thu, 10 Aug 2023 02:35:22 GMT  
		Size: 1.4 KB (1449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab0ebc9f46983ba56ff415cd7b99891210ab8eaad5adf4a15a8f2021de4ebdfd`  
		Last Modified: Wed, 06 Sep 2023 23:18:02 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1c4a22897bb4d3fa0ef4fff463ef850ad45e21404737f120c724fb472c77221`  
		Last Modified: Wed, 06 Sep 2023 23:18:02 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c30142424ff3f45c3c8923f1aa5d959879239599fdde6aba1101c39a168abe48`  
		Last Modified: Wed, 06 Sep 2023 23:18:02 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3723e4e864a2d241c8133b4f1c569ac4ac140d29fe8e216ecd140ebd0e2531cd`  
		Last Modified: Wed, 06 Sep 2023 23:18:02 GMT  
		Size: 242.5 KB (242470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae4c6899207e83d648ab5bf60620507d438b612cb42961f5b8b300c25fde01dd`  
		Last Modified: Wed, 06 Sep 2023 23:18:02 GMT  
		Size: 5.8 MB (5779810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bc2f6a7b18656a6539013442aa6e8c88b49fddce30025ad67ba6e4867a2860b`  
		Last Modified: Wed, 06 Sep 2023 23:18:00 GMT  
		Size: 2.0 KB (1976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ac72b596159b34e1de106133f926192bb5daac9b62301a55822162e6656b6cc`  
		Last Modified: Wed, 06 Sep 2023 23:18:00 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a11a75f33304f42224c3b832462b4497699310fd70a6cdfb322bd126be44cb32`  
		Last Modified: Wed, 06 Sep 2023 23:18:00 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c01b20cb00adae2b356c4377b9419f6a1d18d74692e89c0ee1e66d7b55ca3f3`  
		Last Modified: Wed, 06 Sep 2023 23:18:00 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:windowsservercore-1809`

```console
$ docker pull nats@sha256:df25045f4d70165b54b8b7b0ae443fd21450261550bbc1b314adf8a58053e707
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4737; amd64

### `nats:windowsservercore-1809` - windows version 10.0.17763.4737; amd64

```console
$ docker pull nats@sha256:e2f9912126f4753a9e9312b5dd77a5c5e44c257f28d04ad55cef0662d24138a2
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2001990927 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3cf5f23a9d8d2eca784896bbd09d5e163b27485e7b392cd0bd92f88502dd57b7`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Wed, 02 Aug 2023 09:07:15 GMT
RUN Install update 10.0.17763.4737
# Thu, 10 Aug 2023 01:11:08 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Thu, 10 Aug 2023 02:32:08 GMT
ENV NATS_DOCKERIZED=1
# Wed, 06 Sep 2023 23:15:04 GMT
ENV NATS_SERVER=2.9.22
# Wed, 06 Sep 2023 23:15:05 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.9.22/nats-server-v2.9.22-windows-amd64.zip
# Wed, 06 Sep 2023 23:15:06 GMT
ENV NATS_SERVER_SHASUM=e91db73b02bd4dca3eb7a4bf32e29763450b08d593f73e87d0a6b70102dea0d4
# Wed, 06 Sep 2023 23:15:56 GMT
RUN Set-PSDebug -Trace 2
# Wed, 06 Sep 2023 23:17:21 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 06 Sep 2023 23:17:22 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 06 Sep 2023 23:17:23 GMT
EXPOSE 4222 6222 8222
# Wed, 06 Sep 2023 23:17:24 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 06 Sep 2023 23:17:24 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b95f433aa7d90194e65f6b08a599b3ee12292e124d47c204107baedfd71054c1`  
		Last Modified: Tue, 08 Aug 2023 18:31:16 GMT  
		Size: 345.3 MB (345334986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c5180b8f5f7c2303ba89717cfa778a2173921ca7efdc058cfd6ed951c6d5ca3`  
		Last Modified: Thu, 10 Aug 2023 01:57:18 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fed0c598ca0ae763bd83f045a0c9262bf153a47e508b736992d196e2fb47dea`  
		Last Modified: Thu, 10 Aug 2023 02:35:22 GMT  
		Size: 1.4 KB (1449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab0ebc9f46983ba56ff415cd7b99891210ab8eaad5adf4a15a8f2021de4ebdfd`  
		Last Modified: Wed, 06 Sep 2023 23:18:02 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1c4a22897bb4d3fa0ef4fff463ef850ad45e21404737f120c724fb472c77221`  
		Last Modified: Wed, 06 Sep 2023 23:18:02 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c30142424ff3f45c3c8923f1aa5d959879239599fdde6aba1101c39a168abe48`  
		Last Modified: Wed, 06 Sep 2023 23:18:02 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3723e4e864a2d241c8133b4f1c569ac4ac140d29fe8e216ecd140ebd0e2531cd`  
		Last Modified: Wed, 06 Sep 2023 23:18:02 GMT  
		Size: 242.5 KB (242470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae4c6899207e83d648ab5bf60620507d438b612cb42961f5b8b300c25fde01dd`  
		Last Modified: Wed, 06 Sep 2023 23:18:02 GMT  
		Size: 5.8 MB (5779810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bc2f6a7b18656a6539013442aa6e8c88b49fddce30025ad67ba6e4867a2860b`  
		Last Modified: Wed, 06 Sep 2023 23:18:00 GMT  
		Size: 2.0 KB (1976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ac72b596159b34e1de106133f926192bb5daac9b62301a55822162e6656b6cc`  
		Last Modified: Wed, 06 Sep 2023 23:18:00 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a11a75f33304f42224c3b832462b4497699310fd70a6cdfb322bd126be44cb32`  
		Last Modified: Wed, 06 Sep 2023 23:18:00 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c01b20cb00adae2b356c4377b9419f6a1d18d74692e89c0ee1e66d7b55ca3f3`  
		Last Modified: Wed, 06 Sep 2023 23:18:00 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
