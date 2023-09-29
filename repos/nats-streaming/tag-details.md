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
$ docker pull nats-streaming@sha256:87741883f95fe650defcd3154a8547810b177141b0544aec09406b956ca5c95c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.4851; amd64

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

### `nats-streaming:0.25` - windows version 10.0.17763.4851; amd64

```console
$ docker pull nats-streaming@sha256:2f645551c661a9bdfa1f098de630c345560b42b46ea4f86e4358496fdb7e2c44
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.3 MB (112283602 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6811dea88de0d1562552c6c359244361ee425743d9227dd15ab5dc36b22a88f1`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 29 Aug 2023 16:42:02 GMT
RUN Apply image 10.0.17763.4851
# Wed, 13 Sep 2023 05:08:03 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 13 Sep 2023 05:12:32 GMT
RUN cmd /S /C #(nop) COPY file:0e2c8ba21e47adc90962b46928c928315462bcddaefcbc01f98113f4f66cda4a in C:\nats-streaming-server.exe 
# Wed, 13 Sep 2023 05:12:32 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 13 Sep 2023 05:12:33 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 13 Sep 2023 05:12:34 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:17ba6b878467260559b72cb6f7e79c829eae67862a09efe87f6dc324f49fc086`  
		Last Modified: Tue, 12 Sep 2023 18:31:40 GMT  
		Size: 104.5 MB (104492504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3baa9930674eb6676a1690e63a275d0da517ab8b8aeab7ccd20591f76f7c69a5`  
		Last Modified: Wed, 13 Sep 2023 05:08:48 GMT  
		Size: 1.2 KB (1182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b636690ea2cc8ecb38fcf9cec506c8c908ffe8096160b8549693ae2b6d1aab6`  
		Last Modified: Wed, 13 Sep 2023 05:13:10 GMT  
		Size: 7.8 MB (7786448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02b0f65c350b20f8ac4d372a7e811aff70b8dbcba45d5850be6e80259d1c8544`  
		Last Modified: Wed, 13 Sep 2023 05:13:08 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:181e9541dcd4167889f09d7139f64341ad22ff535be6578fbc55b09600bf8777`  
		Last Modified: Wed, 13 Sep 2023 05:13:08 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1e99090f84ed38c5eac15db96cb5f1e79ff34ddf90739902a0e20c7c5a49280`  
		Last Modified: Wed, 13 Sep 2023 05:13:08 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.25-alpine`

```console
$ docker pull nats-streaming@sha256:9882310c6e2fe226e5f32dd9585362fd1af891a1ce4b30bcc90672569ff8243b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.25-alpine` - linux; amd64

```console
$ docker pull nats-streaming@sha256:b7c0263d4bd45bb96712677a0e1f0d3387f7134fc00cd7ea6e79418ac9c71ac3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.3 MB (11348069 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0257bac8bbcc527511fb5cb28eedd8672f09164257a648d9454dd51c15affd8f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Thu, 28 Sep 2023 21:19:27 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Thu, 28 Sep 2023 21:19:27 GMT
CMD ["/bin/sh"]
# Fri, 29 Sep 2023 00:08:58 GMT
ENV NATS_STREAMING_SERVER=0.25.5
# Fri, 29 Sep 2023 00:09:00 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='937af3f9cdbfe3cb4648cf8c8f505dded2cc175d59ba10e13ec71d1c04e61bf2' ;; 		armhf) natsArch='arm6'; sha256='5bd3a0456054505741b05e5d03acb9f7a5de97cf3ea20cd52d31edbae1c387ea' ;; 		armv7) natsArch='arm7'; sha256='0e643e9881cf3acf3313f84853451d1c4a1e731bc8599d223a40042f9c0c7285' ;; 		x86_64) natsArch='amd64'; sha256='22762f4d0ccfc75947096a14e09566b816113e125a3d39f7914a0c332bee25a7' ;; 		x86) natsArch='386'; sha256='92d8d4460f538883c78e67a334b23b2317e4fe58d46e4fdbbef8b4c09c7b97ae' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Fri, 29 Sep 2023 00:09:00 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Fri, 29 Sep 2023 00:09:00 GMT
EXPOSE 4222 8222
# Fri, 29 Sep 2023 00:09:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 29 Sep 2023 00:09:01 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b50dd55f68014712009de43839be3c41b5e61bf35a6740b5ce12c47ef53779d5`  
		Last Modified: Fri, 29 Sep 2023 00:09:23 GMT  
		Size: 7.9 MB (7945682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5816d53eb086b627f225dfc8f6ebc88fb00622e1fdd9fe878f3e0eb5cfde795b`  
		Last Modified: Fri, 29 Sep 2023 00:09:21 GMT  
		Size: 420.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.25-alpine` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:f71cd5237c12dc4014b14d5791131174fa2605a37dbb1abff7b137a728a0b513
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.7 MB (10746013 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a6de804939b3fcac9461ba70f44717298c30647aa635a03302eccbe8a0c093a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Thu, 28 Sep 2023 20:49:16 GMT
ADD file:2222b03381ff0fce22edd647f5c60529ec6a72202f8d3cb1d6e4648ebcd19a1e in / 
# Thu, 28 Sep 2023 20:49:16 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 22:10:33 GMT
ENV NATS_STREAMING_SERVER=0.25.5
# Thu, 28 Sep 2023 22:10:35 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='937af3f9cdbfe3cb4648cf8c8f505dded2cc175d59ba10e13ec71d1c04e61bf2' ;; 		armhf) natsArch='arm6'; sha256='5bd3a0456054505741b05e5d03acb9f7a5de97cf3ea20cd52d31edbae1c387ea' ;; 		armv7) natsArch='arm7'; sha256='0e643e9881cf3acf3313f84853451d1c4a1e731bc8599d223a40042f9c0c7285' ;; 		x86_64) natsArch='amd64'; sha256='22762f4d0ccfc75947096a14e09566b816113e125a3d39f7914a0c332bee25a7' ;; 		x86) natsArch='386'; sha256='92d8d4460f538883c78e67a334b23b2317e4fe58d46e4fdbbef8b4c09c7b97ae' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Thu, 28 Sep 2023 22:10:35 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Thu, 28 Sep 2023 22:10:36 GMT
EXPOSE 4222 8222
# Thu, 28 Sep 2023 22:10:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 28 Sep 2023 22:10:36 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:91cb83b91ee16f1ee0d588fccef56ab5dbb5689a64e5373caf33d7e4fe52ceb4`  
		Last Modified: Thu, 28 Sep 2023 20:51:25 GMT  
		Size: 3.1 MB (3145291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0445b5b06906bb6f0d5897ac5cec84996eb8b886638a3a482c09abe5e0e32cbe`  
		Last Modified: Thu, 28 Sep 2023 22:10:54 GMT  
		Size: 7.6 MB (7600298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed760df85f369bc55148f03fc0a8c27fef9b47457cc6916b7ef7aa8afeb081ed`  
		Last Modified: Thu, 28 Sep 2023 22:10:53 GMT  
		Size: 424.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.25-alpine` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:a77c3600f2290a15c97e8f26a243c8f40fa9fa4f5251a174ba607000b8d6fc87
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.5 MB (10488419 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d9cbce71f1ae3774c1bea17aeb3c9ebd9b29679316526697d74befebf17e391`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Thu, 28 Sep 2023 20:59:24 GMT
ADD file:61f54a318ad79861c6177783bb4c604412b5d952f45a9aa12ff97f4dccba7f73 in / 
# Thu, 28 Sep 2023 20:59:24 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 22:20:51 GMT
ENV NATS_STREAMING_SERVER=0.25.5
# Thu, 28 Sep 2023 22:20:55 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='937af3f9cdbfe3cb4648cf8c8f505dded2cc175d59ba10e13ec71d1c04e61bf2' ;; 		armhf) natsArch='arm6'; sha256='5bd3a0456054505741b05e5d03acb9f7a5de97cf3ea20cd52d31edbae1c387ea' ;; 		armv7) natsArch='arm7'; sha256='0e643e9881cf3acf3313f84853451d1c4a1e731bc8599d223a40042f9c0c7285' ;; 		x86_64) natsArch='amd64'; sha256='22762f4d0ccfc75947096a14e09566b816113e125a3d39f7914a0c332bee25a7' ;; 		x86) natsArch='386'; sha256='92d8d4460f538883c78e67a334b23b2317e4fe58d46e4fdbbef8b4c09c7b97ae' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Thu, 28 Sep 2023 22:20:55 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Thu, 28 Sep 2023 22:20:56 GMT
EXPOSE 4222 8222
# Thu, 28 Sep 2023 22:20:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 28 Sep 2023 22:20:57 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:622a0779436eb93ceea635e910268f867c2eba47d4f62f0bd45f0bd165af3572`  
		Last Modified: Thu, 28 Sep 2023 21:00:50 GMT  
		Size: 2.9 MB (2899905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0188c8c2d602e176e2f3fd95dfc4449d372745f654ecf1a15331d128a13ff308`  
		Last Modified: Thu, 28 Sep 2023 22:21:27 GMT  
		Size: 7.6 MB (7588094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0780bc6839fa58bce51e6d5d4b96f1d9cb9ac3e06e04aaedded20bdc6909fe72`  
		Last Modified: Thu, 28 Sep 2023 22:21:25 GMT  
		Size: 420.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.25-alpine` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:6d3f66596143b24da010280c677ec5454c6c9bd232e9a2f0f0361d53740e7037
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.6 MB (10632393 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb729c2a167ab94cdc8df4e6393ebd475aee993d9d22fb30b6f9b4d982e7aba8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Thu, 28 Sep 2023 20:39:33 GMT
ADD file:ff3112828967e8004a3264d7ece3f81c88e6a1d44d360b9b5613caab15b41717 in / 
# Thu, 28 Sep 2023 20:39:34 GMT
CMD ["/bin/sh"]
# Fri, 29 Sep 2023 02:07:03 GMT
ENV NATS_STREAMING_SERVER=0.25.5
# Fri, 29 Sep 2023 02:07:06 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='937af3f9cdbfe3cb4648cf8c8f505dded2cc175d59ba10e13ec71d1c04e61bf2' ;; 		armhf) natsArch='arm6'; sha256='5bd3a0456054505741b05e5d03acb9f7a5de97cf3ea20cd52d31edbae1c387ea' ;; 		armv7) natsArch='arm7'; sha256='0e643e9881cf3acf3313f84853451d1c4a1e731bc8599d223a40042f9c0c7285' ;; 		x86_64) natsArch='amd64'; sha256='22762f4d0ccfc75947096a14e09566b816113e125a3d39f7914a0c332bee25a7' ;; 		x86) natsArch='386'; sha256='92d8d4460f538883c78e67a334b23b2317e4fe58d46e4fdbbef8b4c09c7b97ae' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Fri, 29 Sep 2023 02:07:06 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Fri, 29 Sep 2023 02:07:06 GMT
EXPOSE 4222 8222
# Fri, 29 Sep 2023 02:07:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 29 Sep 2023 02:07:06 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:579b34f0a95bb83b3acd6b3249ddc52c3d80f5c84b13c944e9e324feb86dd329`  
		Last Modified: Thu, 28 Sep 2023 20:40:08 GMT  
		Size: 3.3 MB (3331831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b22a41d5f7e381035298ee771a08da6b89cf6aac2dc6bcfa7fb3d78615425edb`  
		Last Modified: Fri, 29 Sep 2023 02:07:24 GMT  
		Size: 7.3 MB (7300141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e297e142ef0e9c319179692d027cf31def6f553e423c2880e6b4d191e24a6889`  
		Last Modified: Fri, 29 Sep 2023 02:07:23 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.25-alpine3.18`

```console
$ docker pull nats-streaming@sha256:9882310c6e2fe226e5f32dd9585362fd1af891a1ce4b30bcc90672569ff8243b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.25-alpine3.18` - linux; amd64

```console
$ docker pull nats-streaming@sha256:b7c0263d4bd45bb96712677a0e1f0d3387f7134fc00cd7ea6e79418ac9c71ac3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.3 MB (11348069 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0257bac8bbcc527511fb5cb28eedd8672f09164257a648d9454dd51c15affd8f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Thu, 28 Sep 2023 21:19:27 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Thu, 28 Sep 2023 21:19:27 GMT
CMD ["/bin/sh"]
# Fri, 29 Sep 2023 00:08:58 GMT
ENV NATS_STREAMING_SERVER=0.25.5
# Fri, 29 Sep 2023 00:09:00 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='937af3f9cdbfe3cb4648cf8c8f505dded2cc175d59ba10e13ec71d1c04e61bf2' ;; 		armhf) natsArch='arm6'; sha256='5bd3a0456054505741b05e5d03acb9f7a5de97cf3ea20cd52d31edbae1c387ea' ;; 		armv7) natsArch='arm7'; sha256='0e643e9881cf3acf3313f84853451d1c4a1e731bc8599d223a40042f9c0c7285' ;; 		x86_64) natsArch='amd64'; sha256='22762f4d0ccfc75947096a14e09566b816113e125a3d39f7914a0c332bee25a7' ;; 		x86) natsArch='386'; sha256='92d8d4460f538883c78e67a334b23b2317e4fe58d46e4fdbbef8b4c09c7b97ae' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Fri, 29 Sep 2023 00:09:00 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Fri, 29 Sep 2023 00:09:00 GMT
EXPOSE 4222 8222
# Fri, 29 Sep 2023 00:09:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 29 Sep 2023 00:09:01 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b50dd55f68014712009de43839be3c41b5e61bf35a6740b5ce12c47ef53779d5`  
		Last Modified: Fri, 29 Sep 2023 00:09:23 GMT  
		Size: 7.9 MB (7945682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5816d53eb086b627f225dfc8f6ebc88fb00622e1fdd9fe878f3e0eb5cfde795b`  
		Last Modified: Fri, 29 Sep 2023 00:09:21 GMT  
		Size: 420.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.25-alpine3.18` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:f71cd5237c12dc4014b14d5791131174fa2605a37dbb1abff7b137a728a0b513
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.7 MB (10746013 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a6de804939b3fcac9461ba70f44717298c30647aa635a03302eccbe8a0c093a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Thu, 28 Sep 2023 20:49:16 GMT
ADD file:2222b03381ff0fce22edd647f5c60529ec6a72202f8d3cb1d6e4648ebcd19a1e in / 
# Thu, 28 Sep 2023 20:49:16 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 22:10:33 GMT
ENV NATS_STREAMING_SERVER=0.25.5
# Thu, 28 Sep 2023 22:10:35 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='937af3f9cdbfe3cb4648cf8c8f505dded2cc175d59ba10e13ec71d1c04e61bf2' ;; 		armhf) natsArch='arm6'; sha256='5bd3a0456054505741b05e5d03acb9f7a5de97cf3ea20cd52d31edbae1c387ea' ;; 		armv7) natsArch='arm7'; sha256='0e643e9881cf3acf3313f84853451d1c4a1e731bc8599d223a40042f9c0c7285' ;; 		x86_64) natsArch='amd64'; sha256='22762f4d0ccfc75947096a14e09566b816113e125a3d39f7914a0c332bee25a7' ;; 		x86) natsArch='386'; sha256='92d8d4460f538883c78e67a334b23b2317e4fe58d46e4fdbbef8b4c09c7b97ae' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Thu, 28 Sep 2023 22:10:35 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Thu, 28 Sep 2023 22:10:36 GMT
EXPOSE 4222 8222
# Thu, 28 Sep 2023 22:10:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 28 Sep 2023 22:10:36 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:91cb83b91ee16f1ee0d588fccef56ab5dbb5689a64e5373caf33d7e4fe52ceb4`  
		Last Modified: Thu, 28 Sep 2023 20:51:25 GMT  
		Size: 3.1 MB (3145291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0445b5b06906bb6f0d5897ac5cec84996eb8b886638a3a482c09abe5e0e32cbe`  
		Last Modified: Thu, 28 Sep 2023 22:10:54 GMT  
		Size: 7.6 MB (7600298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed760df85f369bc55148f03fc0a8c27fef9b47457cc6916b7ef7aa8afeb081ed`  
		Last Modified: Thu, 28 Sep 2023 22:10:53 GMT  
		Size: 424.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.25-alpine3.18` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:a77c3600f2290a15c97e8f26a243c8f40fa9fa4f5251a174ba607000b8d6fc87
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.5 MB (10488419 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d9cbce71f1ae3774c1bea17aeb3c9ebd9b29679316526697d74befebf17e391`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Thu, 28 Sep 2023 20:59:24 GMT
ADD file:61f54a318ad79861c6177783bb4c604412b5d952f45a9aa12ff97f4dccba7f73 in / 
# Thu, 28 Sep 2023 20:59:24 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 22:20:51 GMT
ENV NATS_STREAMING_SERVER=0.25.5
# Thu, 28 Sep 2023 22:20:55 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='937af3f9cdbfe3cb4648cf8c8f505dded2cc175d59ba10e13ec71d1c04e61bf2' ;; 		armhf) natsArch='arm6'; sha256='5bd3a0456054505741b05e5d03acb9f7a5de97cf3ea20cd52d31edbae1c387ea' ;; 		armv7) natsArch='arm7'; sha256='0e643e9881cf3acf3313f84853451d1c4a1e731bc8599d223a40042f9c0c7285' ;; 		x86_64) natsArch='amd64'; sha256='22762f4d0ccfc75947096a14e09566b816113e125a3d39f7914a0c332bee25a7' ;; 		x86) natsArch='386'; sha256='92d8d4460f538883c78e67a334b23b2317e4fe58d46e4fdbbef8b4c09c7b97ae' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Thu, 28 Sep 2023 22:20:55 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Thu, 28 Sep 2023 22:20:56 GMT
EXPOSE 4222 8222
# Thu, 28 Sep 2023 22:20:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 28 Sep 2023 22:20:57 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:622a0779436eb93ceea635e910268f867c2eba47d4f62f0bd45f0bd165af3572`  
		Last Modified: Thu, 28 Sep 2023 21:00:50 GMT  
		Size: 2.9 MB (2899905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0188c8c2d602e176e2f3fd95dfc4449d372745f654ecf1a15331d128a13ff308`  
		Last Modified: Thu, 28 Sep 2023 22:21:27 GMT  
		Size: 7.6 MB (7588094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0780bc6839fa58bce51e6d5d4b96f1d9cb9ac3e06e04aaedded20bdc6909fe72`  
		Last Modified: Thu, 28 Sep 2023 22:21:25 GMT  
		Size: 420.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.25-alpine3.18` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:6d3f66596143b24da010280c677ec5454c6c9bd232e9a2f0f0361d53740e7037
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.6 MB (10632393 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb729c2a167ab94cdc8df4e6393ebd475aee993d9d22fb30b6f9b4d982e7aba8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Thu, 28 Sep 2023 20:39:33 GMT
ADD file:ff3112828967e8004a3264d7ece3f81c88e6a1d44d360b9b5613caab15b41717 in / 
# Thu, 28 Sep 2023 20:39:34 GMT
CMD ["/bin/sh"]
# Fri, 29 Sep 2023 02:07:03 GMT
ENV NATS_STREAMING_SERVER=0.25.5
# Fri, 29 Sep 2023 02:07:06 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='937af3f9cdbfe3cb4648cf8c8f505dded2cc175d59ba10e13ec71d1c04e61bf2' ;; 		armhf) natsArch='arm6'; sha256='5bd3a0456054505741b05e5d03acb9f7a5de97cf3ea20cd52d31edbae1c387ea' ;; 		armv7) natsArch='arm7'; sha256='0e643e9881cf3acf3313f84853451d1c4a1e731bc8599d223a40042f9c0c7285' ;; 		x86_64) natsArch='amd64'; sha256='22762f4d0ccfc75947096a14e09566b816113e125a3d39f7914a0c332bee25a7' ;; 		x86) natsArch='386'; sha256='92d8d4460f538883c78e67a334b23b2317e4fe58d46e4fdbbef8b4c09c7b97ae' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Fri, 29 Sep 2023 02:07:06 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Fri, 29 Sep 2023 02:07:06 GMT
EXPOSE 4222 8222
# Fri, 29 Sep 2023 02:07:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 29 Sep 2023 02:07:06 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:579b34f0a95bb83b3acd6b3249ddc52c3d80f5c84b13c944e9e324feb86dd329`  
		Last Modified: Thu, 28 Sep 2023 20:40:08 GMT  
		Size: 3.3 MB (3331831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b22a41d5f7e381035298ee771a08da6b89cf6aac2dc6bcfa7fb3d78615425edb`  
		Last Modified: Fri, 29 Sep 2023 02:07:24 GMT  
		Size: 7.3 MB (7300141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e297e142ef0e9c319179692d027cf31def6f553e423c2880e6b4d191e24a6889`  
		Last Modified: Fri, 29 Sep 2023 02:07:23 GMT  
		Size: 421.0 B  
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
$ docker pull nats-streaming@sha256:b661b1af7d63f50e0550e23204e3a544e5c351a613a832386aee365bcce484d8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4851; amd64

### `nats-streaming:0.25-nanoserver` - windows version 10.0.17763.4851; amd64

```console
$ docker pull nats-streaming@sha256:2f645551c661a9bdfa1f098de630c345560b42b46ea4f86e4358496fdb7e2c44
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.3 MB (112283602 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6811dea88de0d1562552c6c359244361ee425743d9227dd15ab5dc36b22a88f1`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 29 Aug 2023 16:42:02 GMT
RUN Apply image 10.0.17763.4851
# Wed, 13 Sep 2023 05:08:03 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 13 Sep 2023 05:12:32 GMT
RUN cmd /S /C #(nop) COPY file:0e2c8ba21e47adc90962b46928c928315462bcddaefcbc01f98113f4f66cda4a in C:\nats-streaming-server.exe 
# Wed, 13 Sep 2023 05:12:32 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 13 Sep 2023 05:12:33 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 13 Sep 2023 05:12:34 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:17ba6b878467260559b72cb6f7e79c829eae67862a09efe87f6dc324f49fc086`  
		Last Modified: Tue, 12 Sep 2023 18:31:40 GMT  
		Size: 104.5 MB (104492504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3baa9930674eb6676a1690e63a275d0da517ab8b8aeab7ccd20591f76f7c69a5`  
		Last Modified: Wed, 13 Sep 2023 05:08:48 GMT  
		Size: 1.2 KB (1182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b636690ea2cc8ecb38fcf9cec506c8c908ffe8096160b8549693ae2b6d1aab6`  
		Last Modified: Wed, 13 Sep 2023 05:13:10 GMT  
		Size: 7.8 MB (7786448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02b0f65c350b20f8ac4d372a7e811aff70b8dbcba45d5850be6e80259d1c8544`  
		Last Modified: Wed, 13 Sep 2023 05:13:08 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:181e9541dcd4167889f09d7139f64341ad22ff535be6578fbc55b09600bf8777`  
		Last Modified: Wed, 13 Sep 2023 05:13:08 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1e99090f84ed38c5eac15db96cb5f1e79ff34ddf90739902a0e20c7c5a49280`  
		Last Modified: Wed, 13 Sep 2023 05:13:08 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.25-nanoserver-1809`

```console
$ docker pull nats-streaming@sha256:b661b1af7d63f50e0550e23204e3a544e5c351a613a832386aee365bcce484d8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4851; amd64

### `nats-streaming:0.25-nanoserver-1809` - windows version 10.0.17763.4851; amd64

```console
$ docker pull nats-streaming@sha256:2f645551c661a9bdfa1f098de630c345560b42b46ea4f86e4358496fdb7e2c44
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.3 MB (112283602 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6811dea88de0d1562552c6c359244361ee425743d9227dd15ab5dc36b22a88f1`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 29 Aug 2023 16:42:02 GMT
RUN Apply image 10.0.17763.4851
# Wed, 13 Sep 2023 05:08:03 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 13 Sep 2023 05:12:32 GMT
RUN cmd /S /C #(nop) COPY file:0e2c8ba21e47adc90962b46928c928315462bcddaefcbc01f98113f4f66cda4a in C:\nats-streaming-server.exe 
# Wed, 13 Sep 2023 05:12:32 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 13 Sep 2023 05:12:33 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 13 Sep 2023 05:12:34 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:17ba6b878467260559b72cb6f7e79c829eae67862a09efe87f6dc324f49fc086`  
		Last Modified: Tue, 12 Sep 2023 18:31:40 GMT  
		Size: 104.5 MB (104492504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3baa9930674eb6676a1690e63a275d0da517ab8b8aeab7ccd20591f76f7c69a5`  
		Last Modified: Wed, 13 Sep 2023 05:08:48 GMT  
		Size: 1.2 KB (1182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b636690ea2cc8ecb38fcf9cec506c8c908ffe8096160b8549693ae2b6d1aab6`  
		Last Modified: Wed, 13 Sep 2023 05:13:10 GMT  
		Size: 7.8 MB (7786448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02b0f65c350b20f8ac4d372a7e811aff70b8dbcba45d5850be6e80259d1c8544`  
		Last Modified: Wed, 13 Sep 2023 05:13:08 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:181e9541dcd4167889f09d7139f64341ad22ff535be6578fbc55b09600bf8777`  
		Last Modified: Wed, 13 Sep 2023 05:13:08 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1e99090f84ed38c5eac15db96cb5f1e79ff34ddf90739902a0e20c7c5a49280`  
		Last Modified: Wed, 13 Sep 2023 05:13:08 GMT  
		Size: 1.2 KB (1156 bytes)  
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
$ docker pull nats-streaming@sha256:c0663722b63c368a5244ea3a4e9fe0d1191d3d884a285ca3462b49bc6ce3e425
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4851; amd64

### `nats-streaming:0.25-windowsservercore` - windows version 10.0.17763.4851; amd64

```console
$ docker pull nats-streaming@sha256:fd7cb14102d8c704ea297bc89b1a4ed0678e61ab010244b0f10c9caf9aace084
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2024830683 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48ab6bb07050789abd05c33284cfc3969f3c0d76314409cd61493ba62f861df3`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Tue, 29 Aug 2023 17:09:18 GMT
RUN Install update 10.0.17763.4851
# Wed, 13 Sep 2023 03:56:42 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 Sep 2023 05:05:36 GMT
ENV NATS_DOCKERIZED=1
# Wed, 13 Sep 2023 05:09:31 GMT
ENV NATS_STREAMING_SERVER=0.25.5
# Wed, 13 Sep 2023 05:09:32 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.25.5/nats-streaming-server-v0.25.5-windows-amd64.zip
# Wed, 13 Sep 2023 05:09:33 GMT
ENV NATS_STREAMING_SERVER_SHASUM=709b481bfa3537dc7941490365e065554f19c7029830d765ef49e8cd16657b75
# Wed, 13 Sep 2023 05:10:31 GMT
RUN Set-PSDebug -Trace 2
# Wed, 13 Sep 2023 05:12:11 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 13 Sep 2023 05:12:11 GMT
EXPOSE 4222 8222
# Wed, 13 Sep 2023 05:12:12 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 13 Sep 2023 05:12:13 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:179757339e051b99f9a62375fed8f87ffcc4df0eeedb984d20b485bdd089ad08`  
		Last Modified: Tue, 12 Sep 2023 19:41:25 GMT  
		Size: 365.7 MB (365709508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b21bbf840142288ae2bce3465085b591133cf10f78f7dda43277db4838332d8`  
		Last Modified: Wed, 13 Sep 2023 04:36:45 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b54f616fe064e9d4e73bf2aec9a4fe9c58837ec84c2fc998a54ab7a77b52e109`  
		Last Modified: Wed, 13 Sep 2023 05:08:32 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a663613aba018dc846e9dbd32363a68699885ecfc832dd1440a60f531211b506`  
		Last Modified: Wed, 13 Sep 2023 05:12:55 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05ded5f7ebb06ada7d9bd8d7108a90abed6616e6f34c16a99b1dfa3009424fc8`  
		Last Modified: Wed, 13 Sep 2023 05:12:55 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb620195a9df9d4492561a3a9dde486cc331cad8803e7abd659b32b1fb6d88ec`  
		Last Modified: Wed, 13 Sep 2023 05:12:55 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dc7eb1b31cf8667a9011b08200a46d79e72735d944a58592cc8c497b2fba9ea`  
		Last Modified: Wed, 13 Sep 2023 05:12:54 GMT  
		Size: 243.1 KB (243050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adbeadb90f3861c1ea0865df8e6cad25d103d395df563e930d5a160cf7e2f375`  
		Last Modified: Wed, 13 Sep 2023 05:12:55 GMT  
		Size: 8.2 MB (8246481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:330d26826491947886007c6590f2fdb94adff1e5d784b065940137db990e03e1`  
		Last Modified: Wed, 13 Sep 2023 05:12:53 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03882acc2f421c5d355d6c95fa6e04e4efc0d1da2e508bdc9d79462576a7bb78`  
		Last Modified: Wed, 13 Sep 2023 05:12:53 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9218586c67df475e3efb7b40ec0e40680b7ea809104b035e378ae43af8a8680`  
		Last Modified: Wed, 13 Sep 2023 05:12:53 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.25-windowsservercore-1809`

```console
$ docker pull nats-streaming@sha256:c0663722b63c368a5244ea3a4e9fe0d1191d3d884a285ca3462b49bc6ce3e425
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4851; amd64

### `nats-streaming:0.25-windowsservercore-1809` - windows version 10.0.17763.4851; amd64

```console
$ docker pull nats-streaming@sha256:fd7cb14102d8c704ea297bc89b1a4ed0678e61ab010244b0f10c9caf9aace084
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2024830683 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48ab6bb07050789abd05c33284cfc3969f3c0d76314409cd61493ba62f861df3`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Tue, 29 Aug 2023 17:09:18 GMT
RUN Install update 10.0.17763.4851
# Wed, 13 Sep 2023 03:56:42 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 Sep 2023 05:05:36 GMT
ENV NATS_DOCKERIZED=1
# Wed, 13 Sep 2023 05:09:31 GMT
ENV NATS_STREAMING_SERVER=0.25.5
# Wed, 13 Sep 2023 05:09:32 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.25.5/nats-streaming-server-v0.25.5-windows-amd64.zip
# Wed, 13 Sep 2023 05:09:33 GMT
ENV NATS_STREAMING_SERVER_SHASUM=709b481bfa3537dc7941490365e065554f19c7029830d765ef49e8cd16657b75
# Wed, 13 Sep 2023 05:10:31 GMT
RUN Set-PSDebug -Trace 2
# Wed, 13 Sep 2023 05:12:11 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 13 Sep 2023 05:12:11 GMT
EXPOSE 4222 8222
# Wed, 13 Sep 2023 05:12:12 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 13 Sep 2023 05:12:13 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:179757339e051b99f9a62375fed8f87ffcc4df0eeedb984d20b485bdd089ad08`  
		Last Modified: Tue, 12 Sep 2023 19:41:25 GMT  
		Size: 365.7 MB (365709508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b21bbf840142288ae2bce3465085b591133cf10f78f7dda43277db4838332d8`  
		Last Modified: Wed, 13 Sep 2023 04:36:45 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b54f616fe064e9d4e73bf2aec9a4fe9c58837ec84c2fc998a54ab7a77b52e109`  
		Last Modified: Wed, 13 Sep 2023 05:08:32 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a663613aba018dc846e9dbd32363a68699885ecfc832dd1440a60f531211b506`  
		Last Modified: Wed, 13 Sep 2023 05:12:55 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05ded5f7ebb06ada7d9bd8d7108a90abed6616e6f34c16a99b1dfa3009424fc8`  
		Last Modified: Wed, 13 Sep 2023 05:12:55 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb620195a9df9d4492561a3a9dde486cc331cad8803e7abd659b32b1fb6d88ec`  
		Last Modified: Wed, 13 Sep 2023 05:12:55 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dc7eb1b31cf8667a9011b08200a46d79e72735d944a58592cc8c497b2fba9ea`  
		Last Modified: Wed, 13 Sep 2023 05:12:54 GMT  
		Size: 243.1 KB (243050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adbeadb90f3861c1ea0865df8e6cad25d103d395df563e930d5a160cf7e2f375`  
		Last Modified: Wed, 13 Sep 2023 05:12:55 GMT  
		Size: 8.2 MB (8246481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:330d26826491947886007c6590f2fdb94adff1e5d784b065940137db990e03e1`  
		Last Modified: Wed, 13 Sep 2023 05:12:53 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03882acc2f421c5d355d6c95fa6e04e4efc0d1da2e508bdc9d79462576a7bb78`  
		Last Modified: Wed, 13 Sep 2023 05:12:53 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9218586c67df475e3efb7b40ec0e40680b7ea809104b035e378ae43af8a8680`  
		Last Modified: Wed, 13 Sep 2023 05:12:53 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.25.5`

```console
$ docker pull nats-streaming@sha256:87741883f95fe650defcd3154a8547810b177141b0544aec09406b956ca5c95c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.4851; amd64

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

### `nats-streaming:0.25.5` - windows version 10.0.17763.4851; amd64

```console
$ docker pull nats-streaming@sha256:2f645551c661a9bdfa1f098de630c345560b42b46ea4f86e4358496fdb7e2c44
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.3 MB (112283602 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6811dea88de0d1562552c6c359244361ee425743d9227dd15ab5dc36b22a88f1`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 29 Aug 2023 16:42:02 GMT
RUN Apply image 10.0.17763.4851
# Wed, 13 Sep 2023 05:08:03 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 13 Sep 2023 05:12:32 GMT
RUN cmd /S /C #(nop) COPY file:0e2c8ba21e47adc90962b46928c928315462bcddaefcbc01f98113f4f66cda4a in C:\nats-streaming-server.exe 
# Wed, 13 Sep 2023 05:12:32 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 13 Sep 2023 05:12:33 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 13 Sep 2023 05:12:34 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:17ba6b878467260559b72cb6f7e79c829eae67862a09efe87f6dc324f49fc086`  
		Last Modified: Tue, 12 Sep 2023 18:31:40 GMT  
		Size: 104.5 MB (104492504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3baa9930674eb6676a1690e63a275d0da517ab8b8aeab7ccd20591f76f7c69a5`  
		Last Modified: Wed, 13 Sep 2023 05:08:48 GMT  
		Size: 1.2 KB (1182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b636690ea2cc8ecb38fcf9cec506c8c908ffe8096160b8549693ae2b6d1aab6`  
		Last Modified: Wed, 13 Sep 2023 05:13:10 GMT  
		Size: 7.8 MB (7786448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02b0f65c350b20f8ac4d372a7e811aff70b8dbcba45d5850be6e80259d1c8544`  
		Last Modified: Wed, 13 Sep 2023 05:13:08 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:181e9541dcd4167889f09d7139f64341ad22ff535be6578fbc55b09600bf8777`  
		Last Modified: Wed, 13 Sep 2023 05:13:08 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1e99090f84ed38c5eac15db96cb5f1e79ff34ddf90739902a0e20c7c5a49280`  
		Last Modified: Wed, 13 Sep 2023 05:13:08 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.25.5-alpine`

```console
$ docker pull nats-streaming@sha256:9882310c6e2fe226e5f32dd9585362fd1af891a1ce4b30bcc90672569ff8243b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.25.5-alpine` - linux; amd64

```console
$ docker pull nats-streaming@sha256:b7c0263d4bd45bb96712677a0e1f0d3387f7134fc00cd7ea6e79418ac9c71ac3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.3 MB (11348069 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0257bac8bbcc527511fb5cb28eedd8672f09164257a648d9454dd51c15affd8f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Thu, 28 Sep 2023 21:19:27 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Thu, 28 Sep 2023 21:19:27 GMT
CMD ["/bin/sh"]
# Fri, 29 Sep 2023 00:08:58 GMT
ENV NATS_STREAMING_SERVER=0.25.5
# Fri, 29 Sep 2023 00:09:00 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='937af3f9cdbfe3cb4648cf8c8f505dded2cc175d59ba10e13ec71d1c04e61bf2' ;; 		armhf) natsArch='arm6'; sha256='5bd3a0456054505741b05e5d03acb9f7a5de97cf3ea20cd52d31edbae1c387ea' ;; 		armv7) natsArch='arm7'; sha256='0e643e9881cf3acf3313f84853451d1c4a1e731bc8599d223a40042f9c0c7285' ;; 		x86_64) natsArch='amd64'; sha256='22762f4d0ccfc75947096a14e09566b816113e125a3d39f7914a0c332bee25a7' ;; 		x86) natsArch='386'; sha256='92d8d4460f538883c78e67a334b23b2317e4fe58d46e4fdbbef8b4c09c7b97ae' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Fri, 29 Sep 2023 00:09:00 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Fri, 29 Sep 2023 00:09:00 GMT
EXPOSE 4222 8222
# Fri, 29 Sep 2023 00:09:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 29 Sep 2023 00:09:01 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b50dd55f68014712009de43839be3c41b5e61bf35a6740b5ce12c47ef53779d5`  
		Last Modified: Fri, 29 Sep 2023 00:09:23 GMT  
		Size: 7.9 MB (7945682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5816d53eb086b627f225dfc8f6ebc88fb00622e1fdd9fe878f3e0eb5cfde795b`  
		Last Modified: Fri, 29 Sep 2023 00:09:21 GMT  
		Size: 420.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.25.5-alpine` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:f71cd5237c12dc4014b14d5791131174fa2605a37dbb1abff7b137a728a0b513
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.7 MB (10746013 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a6de804939b3fcac9461ba70f44717298c30647aa635a03302eccbe8a0c093a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Thu, 28 Sep 2023 20:49:16 GMT
ADD file:2222b03381ff0fce22edd647f5c60529ec6a72202f8d3cb1d6e4648ebcd19a1e in / 
# Thu, 28 Sep 2023 20:49:16 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 22:10:33 GMT
ENV NATS_STREAMING_SERVER=0.25.5
# Thu, 28 Sep 2023 22:10:35 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='937af3f9cdbfe3cb4648cf8c8f505dded2cc175d59ba10e13ec71d1c04e61bf2' ;; 		armhf) natsArch='arm6'; sha256='5bd3a0456054505741b05e5d03acb9f7a5de97cf3ea20cd52d31edbae1c387ea' ;; 		armv7) natsArch='arm7'; sha256='0e643e9881cf3acf3313f84853451d1c4a1e731bc8599d223a40042f9c0c7285' ;; 		x86_64) natsArch='amd64'; sha256='22762f4d0ccfc75947096a14e09566b816113e125a3d39f7914a0c332bee25a7' ;; 		x86) natsArch='386'; sha256='92d8d4460f538883c78e67a334b23b2317e4fe58d46e4fdbbef8b4c09c7b97ae' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Thu, 28 Sep 2023 22:10:35 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Thu, 28 Sep 2023 22:10:36 GMT
EXPOSE 4222 8222
# Thu, 28 Sep 2023 22:10:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 28 Sep 2023 22:10:36 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:91cb83b91ee16f1ee0d588fccef56ab5dbb5689a64e5373caf33d7e4fe52ceb4`  
		Last Modified: Thu, 28 Sep 2023 20:51:25 GMT  
		Size: 3.1 MB (3145291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0445b5b06906bb6f0d5897ac5cec84996eb8b886638a3a482c09abe5e0e32cbe`  
		Last Modified: Thu, 28 Sep 2023 22:10:54 GMT  
		Size: 7.6 MB (7600298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed760df85f369bc55148f03fc0a8c27fef9b47457cc6916b7ef7aa8afeb081ed`  
		Last Modified: Thu, 28 Sep 2023 22:10:53 GMT  
		Size: 424.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.25.5-alpine` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:a77c3600f2290a15c97e8f26a243c8f40fa9fa4f5251a174ba607000b8d6fc87
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.5 MB (10488419 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d9cbce71f1ae3774c1bea17aeb3c9ebd9b29679316526697d74befebf17e391`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Thu, 28 Sep 2023 20:59:24 GMT
ADD file:61f54a318ad79861c6177783bb4c604412b5d952f45a9aa12ff97f4dccba7f73 in / 
# Thu, 28 Sep 2023 20:59:24 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 22:20:51 GMT
ENV NATS_STREAMING_SERVER=0.25.5
# Thu, 28 Sep 2023 22:20:55 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='937af3f9cdbfe3cb4648cf8c8f505dded2cc175d59ba10e13ec71d1c04e61bf2' ;; 		armhf) natsArch='arm6'; sha256='5bd3a0456054505741b05e5d03acb9f7a5de97cf3ea20cd52d31edbae1c387ea' ;; 		armv7) natsArch='arm7'; sha256='0e643e9881cf3acf3313f84853451d1c4a1e731bc8599d223a40042f9c0c7285' ;; 		x86_64) natsArch='amd64'; sha256='22762f4d0ccfc75947096a14e09566b816113e125a3d39f7914a0c332bee25a7' ;; 		x86) natsArch='386'; sha256='92d8d4460f538883c78e67a334b23b2317e4fe58d46e4fdbbef8b4c09c7b97ae' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Thu, 28 Sep 2023 22:20:55 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Thu, 28 Sep 2023 22:20:56 GMT
EXPOSE 4222 8222
# Thu, 28 Sep 2023 22:20:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 28 Sep 2023 22:20:57 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:622a0779436eb93ceea635e910268f867c2eba47d4f62f0bd45f0bd165af3572`  
		Last Modified: Thu, 28 Sep 2023 21:00:50 GMT  
		Size: 2.9 MB (2899905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0188c8c2d602e176e2f3fd95dfc4449d372745f654ecf1a15331d128a13ff308`  
		Last Modified: Thu, 28 Sep 2023 22:21:27 GMT  
		Size: 7.6 MB (7588094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0780bc6839fa58bce51e6d5d4b96f1d9cb9ac3e06e04aaedded20bdc6909fe72`  
		Last Modified: Thu, 28 Sep 2023 22:21:25 GMT  
		Size: 420.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.25.5-alpine` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:6d3f66596143b24da010280c677ec5454c6c9bd232e9a2f0f0361d53740e7037
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.6 MB (10632393 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb729c2a167ab94cdc8df4e6393ebd475aee993d9d22fb30b6f9b4d982e7aba8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Thu, 28 Sep 2023 20:39:33 GMT
ADD file:ff3112828967e8004a3264d7ece3f81c88e6a1d44d360b9b5613caab15b41717 in / 
# Thu, 28 Sep 2023 20:39:34 GMT
CMD ["/bin/sh"]
# Fri, 29 Sep 2023 02:07:03 GMT
ENV NATS_STREAMING_SERVER=0.25.5
# Fri, 29 Sep 2023 02:07:06 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='937af3f9cdbfe3cb4648cf8c8f505dded2cc175d59ba10e13ec71d1c04e61bf2' ;; 		armhf) natsArch='arm6'; sha256='5bd3a0456054505741b05e5d03acb9f7a5de97cf3ea20cd52d31edbae1c387ea' ;; 		armv7) natsArch='arm7'; sha256='0e643e9881cf3acf3313f84853451d1c4a1e731bc8599d223a40042f9c0c7285' ;; 		x86_64) natsArch='amd64'; sha256='22762f4d0ccfc75947096a14e09566b816113e125a3d39f7914a0c332bee25a7' ;; 		x86) natsArch='386'; sha256='92d8d4460f538883c78e67a334b23b2317e4fe58d46e4fdbbef8b4c09c7b97ae' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Fri, 29 Sep 2023 02:07:06 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Fri, 29 Sep 2023 02:07:06 GMT
EXPOSE 4222 8222
# Fri, 29 Sep 2023 02:07:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 29 Sep 2023 02:07:06 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:579b34f0a95bb83b3acd6b3249ddc52c3d80f5c84b13c944e9e324feb86dd329`  
		Last Modified: Thu, 28 Sep 2023 20:40:08 GMT  
		Size: 3.3 MB (3331831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b22a41d5f7e381035298ee771a08da6b89cf6aac2dc6bcfa7fb3d78615425edb`  
		Last Modified: Fri, 29 Sep 2023 02:07:24 GMT  
		Size: 7.3 MB (7300141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e297e142ef0e9c319179692d027cf31def6f553e423c2880e6b4d191e24a6889`  
		Last Modified: Fri, 29 Sep 2023 02:07:23 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.25.5-alpine3.18`

```console
$ docker pull nats-streaming@sha256:9882310c6e2fe226e5f32dd9585362fd1af891a1ce4b30bcc90672569ff8243b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.25.5-alpine3.18` - linux; amd64

```console
$ docker pull nats-streaming@sha256:b7c0263d4bd45bb96712677a0e1f0d3387f7134fc00cd7ea6e79418ac9c71ac3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.3 MB (11348069 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0257bac8bbcc527511fb5cb28eedd8672f09164257a648d9454dd51c15affd8f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Thu, 28 Sep 2023 21:19:27 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Thu, 28 Sep 2023 21:19:27 GMT
CMD ["/bin/sh"]
# Fri, 29 Sep 2023 00:08:58 GMT
ENV NATS_STREAMING_SERVER=0.25.5
# Fri, 29 Sep 2023 00:09:00 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='937af3f9cdbfe3cb4648cf8c8f505dded2cc175d59ba10e13ec71d1c04e61bf2' ;; 		armhf) natsArch='arm6'; sha256='5bd3a0456054505741b05e5d03acb9f7a5de97cf3ea20cd52d31edbae1c387ea' ;; 		armv7) natsArch='arm7'; sha256='0e643e9881cf3acf3313f84853451d1c4a1e731bc8599d223a40042f9c0c7285' ;; 		x86_64) natsArch='amd64'; sha256='22762f4d0ccfc75947096a14e09566b816113e125a3d39f7914a0c332bee25a7' ;; 		x86) natsArch='386'; sha256='92d8d4460f538883c78e67a334b23b2317e4fe58d46e4fdbbef8b4c09c7b97ae' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Fri, 29 Sep 2023 00:09:00 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Fri, 29 Sep 2023 00:09:00 GMT
EXPOSE 4222 8222
# Fri, 29 Sep 2023 00:09:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 29 Sep 2023 00:09:01 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b50dd55f68014712009de43839be3c41b5e61bf35a6740b5ce12c47ef53779d5`  
		Last Modified: Fri, 29 Sep 2023 00:09:23 GMT  
		Size: 7.9 MB (7945682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5816d53eb086b627f225dfc8f6ebc88fb00622e1fdd9fe878f3e0eb5cfde795b`  
		Last Modified: Fri, 29 Sep 2023 00:09:21 GMT  
		Size: 420.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.25.5-alpine3.18` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:f71cd5237c12dc4014b14d5791131174fa2605a37dbb1abff7b137a728a0b513
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.7 MB (10746013 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a6de804939b3fcac9461ba70f44717298c30647aa635a03302eccbe8a0c093a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Thu, 28 Sep 2023 20:49:16 GMT
ADD file:2222b03381ff0fce22edd647f5c60529ec6a72202f8d3cb1d6e4648ebcd19a1e in / 
# Thu, 28 Sep 2023 20:49:16 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 22:10:33 GMT
ENV NATS_STREAMING_SERVER=0.25.5
# Thu, 28 Sep 2023 22:10:35 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='937af3f9cdbfe3cb4648cf8c8f505dded2cc175d59ba10e13ec71d1c04e61bf2' ;; 		armhf) natsArch='arm6'; sha256='5bd3a0456054505741b05e5d03acb9f7a5de97cf3ea20cd52d31edbae1c387ea' ;; 		armv7) natsArch='arm7'; sha256='0e643e9881cf3acf3313f84853451d1c4a1e731bc8599d223a40042f9c0c7285' ;; 		x86_64) natsArch='amd64'; sha256='22762f4d0ccfc75947096a14e09566b816113e125a3d39f7914a0c332bee25a7' ;; 		x86) natsArch='386'; sha256='92d8d4460f538883c78e67a334b23b2317e4fe58d46e4fdbbef8b4c09c7b97ae' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Thu, 28 Sep 2023 22:10:35 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Thu, 28 Sep 2023 22:10:36 GMT
EXPOSE 4222 8222
# Thu, 28 Sep 2023 22:10:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 28 Sep 2023 22:10:36 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:91cb83b91ee16f1ee0d588fccef56ab5dbb5689a64e5373caf33d7e4fe52ceb4`  
		Last Modified: Thu, 28 Sep 2023 20:51:25 GMT  
		Size: 3.1 MB (3145291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0445b5b06906bb6f0d5897ac5cec84996eb8b886638a3a482c09abe5e0e32cbe`  
		Last Modified: Thu, 28 Sep 2023 22:10:54 GMT  
		Size: 7.6 MB (7600298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed760df85f369bc55148f03fc0a8c27fef9b47457cc6916b7ef7aa8afeb081ed`  
		Last Modified: Thu, 28 Sep 2023 22:10:53 GMT  
		Size: 424.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.25.5-alpine3.18` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:a77c3600f2290a15c97e8f26a243c8f40fa9fa4f5251a174ba607000b8d6fc87
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.5 MB (10488419 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d9cbce71f1ae3774c1bea17aeb3c9ebd9b29679316526697d74befebf17e391`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Thu, 28 Sep 2023 20:59:24 GMT
ADD file:61f54a318ad79861c6177783bb4c604412b5d952f45a9aa12ff97f4dccba7f73 in / 
# Thu, 28 Sep 2023 20:59:24 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 22:20:51 GMT
ENV NATS_STREAMING_SERVER=0.25.5
# Thu, 28 Sep 2023 22:20:55 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='937af3f9cdbfe3cb4648cf8c8f505dded2cc175d59ba10e13ec71d1c04e61bf2' ;; 		armhf) natsArch='arm6'; sha256='5bd3a0456054505741b05e5d03acb9f7a5de97cf3ea20cd52d31edbae1c387ea' ;; 		armv7) natsArch='arm7'; sha256='0e643e9881cf3acf3313f84853451d1c4a1e731bc8599d223a40042f9c0c7285' ;; 		x86_64) natsArch='amd64'; sha256='22762f4d0ccfc75947096a14e09566b816113e125a3d39f7914a0c332bee25a7' ;; 		x86) natsArch='386'; sha256='92d8d4460f538883c78e67a334b23b2317e4fe58d46e4fdbbef8b4c09c7b97ae' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Thu, 28 Sep 2023 22:20:55 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Thu, 28 Sep 2023 22:20:56 GMT
EXPOSE 4222 8222
# Thu, 28 Sep 2023 22:20:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 28 Sep 2023 22:20:57 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:622a0779436eb93ceea635e910268f867c2eba47d4f62f0bd45f0bd165af3572`  
		Last Modified: Thu, 28 Sep 2023 21:00:50 GMT  
		Size: 2.9 MB (2899905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0188c8c2d602e176e2f3fd95dfc4449d372745f654ecf1a15331d128a13ff308`  
		Last Modified: Thu, 28 Sep 2023 22:21:27 GMT  
		Size: 7.6 MB (7588094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0780bc6839fa58bce51e6d5d4b96f1d9cb9ac3e06e04aaedded20bdc6909fe72`  
		Last Modified: Thu, 28 Sep 2023 22:21:25 GMT  
		Size: 420.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.25.5-alpine3.18` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:6d3f66596143b24da010280c677ec5454c6c9bd232e9a2f0f0361d53740e7037
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.6 MB (10632393 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb729c2a167ab94cdc8df4e6393ebd475aee993d9d22fb30b6f9b4d982e7aba8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Thu, 28 Sep 2023 20:39:33 GMT
ADD file:ff3112828967e8004a3264d7ece3f81c88e6a1d44d360b9b5613caab15b41717 in / 
# Thu, 28 Sep 2023 20:39:34 GMT
CMD ["/bin/sh"]
# Fri, 29 Sep 2023 02:07:03 GMT
ENV NATS_STREAMING_SERVER=0.25.5
# Fri, 29 Sep 2023 02:07:06 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='937af3f9cdbfe3cb4648cf8c8f505dded2cc175d59ba10e13ec71d1c04e61bf2' ;; 		armhf) natsArch='arm6'; sha256='5bd3a0456054505741b05e5d03acb9f7a5de97cf3ea20cd52d31edbae1c387ea' ;; 		armv7) natsArch='arm7'; sha256='0e643e9881cf3acf3313f84853451d1c4a1e731bc8599d223a40042f9c0c7285' ;; 		x86_64) natsArch='amd64'; sha256='22762f4d0ccfc75947096a14e09566b816113e125a3d39f7914a0c332bee25a7' ;; 		x86) natsArch='386'; sha256='92d8d4460f538883c78e67a334b23b2317e4fe58d46e4fdbbef8b4c09c7b97ae' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Fri, 29 Sep 2023 02:07:06 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Fri, 29 Sep 2023 02:07:06 GMT
EXPOSE 4222 8222
# Fri, 29 Sep 2023 02:07:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 29 Sep 2023 02:07:06 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:579b34f0a95bb83b3acd6b3249ddc52c3d80f5c84b13c944e9e324feb86dd329`  
		Last Modified: Thu, 28 Sep 2023 20:40:08 GMT  
		Size: 3.3 MB (3331831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b22a41d5f7e381035298ee771a08da6b89cf6aac2dc6bcfa7fb3d78615425edb`  
		Last Modified: Fri, 29 Sep 2023 02:07:24 GMT  
		Size: 7.3 MB (7300141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e297e142ef0e9c319179692d027cf31def6f553e423c2880e6b4d191e24a6889`  
		Last Modified: Fri, 29 Sep 2023 02:07:23 GMT  
		Size: 421.0 B  
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
$ docker pull nats-streaming@sha256:b661b1af7d63f50e0550e23204e3a544e5c351a613a832386aee365bcce484d8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4851; amd64

### `nats-streaming:0.25.5-nanoserver` - windows version 10.0.17763.4851; amd64

```console
$ docker pull nats-streaming@sha256:2f645551c661a9bdfa1f098de630c345560b42b46ea4f86e4358496fdb7e2c44
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.3 MB (112283602 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6811dea88de0d1562552c6c359244361ee425743d9227dd15ab5dc36b22a88f1`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 29 Aug 2023 16:42:02 GMT
RUN Apply image 10.0.17763.4851
# Wed, 13 Sep 2023 05:08:03 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 13 Sep 2023 05:12:32 GMT
RUN cmd /S /C #(nop) COPY file:0e2c8ba21e47adc90962b46928c928315462bcddaefcbc01f98113f4f66cda4a in C:\nats-streaming-server.exe 
# Wed, 13 Sep 2023 05:12:32 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 13 Sep 2023 05:12:33 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 13 Sep 2023 05:12:34 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:17ba6b878467260559b72cb6f7e79c829eae67862a09efe87f6dc324f49fc086`  
		Last Modified: Tue, 12 Sep 2023 18:31:40 GMT  
		Size: 104.5 MB (104492504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3baa9930674eb6676a1690e63a275d0da517ab8b8aeab7ccd20591f76f7c69a5`  
		Last Modified: Wed, 13 Sep 2023 05:08:48 GMT  
		Size: 1.2 KB (1182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b636690ea2cc8ecb38fcf9cec506c8c908ffe8096160b8549693ae2b6d1aab6`  
		Last Modified: Wed, 13 Sep 2023 05:13:10 GMT  
		Size: 7.8 MB (7786448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02b0f65c350b20f8ac4d372a7e811aff70b8dbcba45d5850be6e80259d1c8544`  
		Last Modified: Wed, 13 Sep 2023 05:13:08 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:181e9541dcd4167889f09d7139f64341ad22ff535be6578fbc55b09600bf8777`  
		Last Modified: Wed, 13 Sep 2023 05:13:08 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1e99090f84ed38c5eac15db96cb5f1e79ff34ddf90739902a0e20c7c5a49280`  
		Last Modified: Wed, 13 Sep 2023 05:13:08 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.25.5-nanoserver-1809`

```console
$ docker pull nats-streaming@sha256:b661b1af7d63f50e0550e23204e3a544e5c351a613a832386aee365bcce484d8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4851; amd64

### `nats-streaming:0.25.5-nanoserver-1809` - windows version 10.0.17763.4851; amd64

```console
$ docker pull nats-streaming@sha256:2f645551c661a9bdfa1f098de630c345560b42b46ea4f86e4358496fdb7e2c44
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.3 MB (112283602 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6811dea88de0d1562552c6c359244361ee425743d9227dd15ab5dc36b22a88f1`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 29 Aug 2023 16:42:02 GMT
RUN Apply image 10.0.17763.4851
# Wed, 13 Sep 2023 05:08:03 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 13 Sep 2023 05:12:32 GMT
RUN cmd /S /C #(nop) COPY file:0e2c8ba21e47adc90962b46928c928315462bcddaefcbc01f98113f4f66cda4a in C:\nats-streaming-server.exe 
# Wed, 13 Sep 2023 05:12:32 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 13 Sep 2023 05:12:33 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 13 Sep 2023 05:12:34 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:17ba6b878467260559b72cb6f7e79c829eae67862a09efe87f6dc324f49fc086`  
		Last Modified: Tue, 12 Sep 2023 18:31:40 GMT  
		Size: 104.5 MB (104492504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3baa9930674eb6676a1690e63a275d0da517ab8b8aeab7ccd20591f76f7c69a5`  
		Last Modified: Wed, 13 Sep 2023 05:08:48 GMT  
		Size: 1.2 KB (1182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b636690ea2cc8ecb38fcf9cec506c8c908ffe8096160b8549693ae2b6d1aab6`  
		Last Modified: Wed, 13 Sep 2023 05:13:10 GMT  
		Size: 7.8 MB (7786448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02b0f65c350b20f8ac4d372a7e811aff70b8dbcba45d5850be6e80259d1c8544`  
		Last Modified: Wed, 13 Sep 2023 05:13:08 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:181e9541dcd4167889f09d7139f64341ad22ff535be6578fbc55b09600bf8777`  
		Last Modified: Wed, 13 Sep 2023 05:13:08 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1e99090f84ed38c5eac15db96cb5f1e79ff34ddf90739902a0e20c7c5a49280`  
		Last Modified: Wed, 13 Sep 2023 05:13:08 GMT  
		Size: 1.2 KB (1156 bytes)  
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
$ docker pull nats-streaming@sha256:c0663722b63c368a5244ea3a4e9fe0d1191d3d884a285ca3462b49bc6ce3e425
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4851; amd64

### `nats-streaming:0.25.5-windowsservercore` - windows version 10.0.17763.4851; amd64

```console
$ docker pull nats-streaming@sha256:fd7cb14102d8c704ea297bc89b1a4ed0678e61ab010244b0f10c9caf9aace084
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2024830683 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48ab6bb07050789abd05c33284cfc3969f3c0d76314409cd61493ba62f861df3`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Tue, 29 Aug 2023 17:09:18 GMT
RUN Install update 10.0.17763.4851
# Wed, 13 Sep 2023 03:56:42 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 Sep 2023 05:05:36 GMT
ENV NATS_DOCKERIZED=1
# Wed, 13 Sep 2023 05:09:31 GMT
ENV NATS_STREAMING_SERVER=0.25.5
# Wed, 13 Sep 2023 05:09:32 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.25.5/nats-streaming-server-v0.25.5-windows-amd64.zip
# Wed, 13 Sep 2023 05:09:33 GMT
ENV NATS_STREAMING_SERVER_SHASUM=709b481bfa3537dc7941490365e065554f19c7029830d765ef49e8cd16657b75
# Wed, 13 Sep 2023 05:10:31 GMT
RUN Set-PSDebug -Trace 2
# Wed, 13 Sep 2023 05:12:11 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 13 Sep 2023 05:12:11 GMT
EXPOSE 4222 8222
# Wed, 13 Sep 2023 05:12:12 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 13 Sep 2023 05:12:13 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:179757339e051b99f9a62375fed8f87ffcc4df0eeedb984d20b485bdd089ad08`  
		Last Modified: Tue, 12 Sep 2023 19:41:25 GMT  
		Size: 365.7 MB (365709508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b21bbf840142288ae2bce3465085b591133cf10f78f7dda43277db4838332d8`  
		Last Modified: Wed, 13 Sep 2023 04:36:45 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b54f616fe064e9d4e73bf2aec9a4fe9c58837ec84c2fc998a54ab7a77b52e109`  
		Last Modified: Wed, 13 Sep 2023 05:08:32 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a663613aba018dc846e9dbd32363a68699885ecfc832dd1440a60f531211b506`  
		Last Modified: Wed, 13 Sep 2023 05:12:55 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05ded5f7ebb06ada7d9bd8d7108a90abed6616e6f34c16a99b1dfa3009424fc8`  
		Last Modified: Wed, 13 Sep 2023 05:12:55 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb620195a9df9d4492561a3a9dde486cc331cad8803e7abd659b32b1fb6d88ec`  
		Last Modified: Wed, 13 Sep 2023 05:12:55 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dc7eb1b31cf8667a9011b08200a46d79e72735d944a58592cc8c497b2fba9ea`  
		Last Modified: Wed, 13 Sep 2023 05:12:54 GMT  
		Size: 243.1 KB (243050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adbeadb90f3861c1ea0865df8e6cad25d103d395df563e930d5a160cf7e2f375`  
		Last Modified: Wed, 13 Sep 2023 05:12:55 GMT  
		Size: 8.2 MB (8246481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:330d26826491947886007c6590f2fdb94adff1e5d784b065940137db990e03e1`  
		Last Modified: Wed, 13 Sep 2023 05:12:53 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03882acc2f421c5d355d6c95fa6e04e4efc0d1da2e508bdc9d79462576a7bb78`  
		Last Modified: Wed, 13 Sep 2023 05:12:53 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9218586c67df475e3efb7b40ec0e40680b7ea809104b035e378ae43af8a8680`  
		Last Modified: Wed, 13 Sep 2023 05:12:53 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.25.5-windowsservercore-1809`

```console
$ docker pull nats-streaming@sha256:c0663722b63c368a5244ea3a4e9fe0d1191d3d884a285ca3462b49bc6ce3e425
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4851; amd64

### `nats-streaming:0.25.5-windowsservercore-1809` - windows version 10.0.17763.4851; amd64

```console
$ docker pull nats-streaming@sha256:fd7cb14102d8c704ea297bc89b1a4ed0678e61ab010244b0f10c9caf9aace084
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2024830683 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48ab6bb07050789abd05c33284cfc3969f3c0d76314409cd61493ba62f861df3`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Tue, 29 Aug 2023 17:09:18 GMT
RUN Install update 10.0.17763.4851
# Wed, 13 Sep 2023 03:56:42 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 Sep 2023 05:05:36 GMT
ENV NATS_DOCKERIZED=1
# Wed, 13 Sep 2023 05:09:31 GMT
ENV NATS_STREAMING_SERVER=0.25.5
# Wed, 13 Sep 2023 05:09:32 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.25.5/nats-streaming-server-v0.25.5-windows-amd64.zip
# Wed, 13 Sep 2023 05:09:33 GMT
ENV NATS_STREAMING_SERVER_SHASUM=709b481bfa3537dc7941490365e065554f19c7029830d765ef49e8cd16657b75
# Wed, 13 Sep 2023 05:10:31 GMT
RUN Set-PSDebug -Trace 2
# Wed, 13 Sep 2023 05:12:11 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 13 Sep 2023 05:12:11 GMT
EXPOSE 4222 8222
# Wed, 13 Sep 2023 05:12:12 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 13 Sep 2023 05:12:13 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:179757339e051b99f9a62375fed8f87ffcc4df0eeedb984d20b485bdd089ad08`  
		Last Modified: Tue, 12 Sep 2023 19:41:25 GMT  
		Size: 365.7 MB (365709508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b21bbf840142288ae2bce3465085b591133cf10f78f7dda43277db4838332d8`  
		Last Modified: Wed, 13 Sep 2023 04:36:45 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b54f616fe064e9d4e73bf2aec9a4fe9c58837ec84c2fc998a54ab7a77b52e109`  
		Last Modified: Wed, 13 Sep 2023 05:08:32 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a663613aba018dc846e9dbd32363a68699885ecfc832dd1440a60f531211b506`  
		Last Modified: Wed, 13 Sep 2023 05:12:55 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05ded5f7ebb06ada7d9bd8d7108a90abed6616e6f34c16a99b1dfa3009424fc8`  
		Last Modified: Wed, 13 Sep 2023 05:12:55 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb620195a9df9d4492561a3a9dde486cc331cad8803e7abd659b32b1fb6d88ec`  
		Last Modified: Wed, 13 Sep 2023 05:12:55 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dc7eb1b31cf8667a9011b08200a46d79e72735d944a58592cc8c497b2fba9ea`  
		Last Modified: Wed, 13 Sep 2023 05:12:54 GMT  
		Size: 243.1 KB (243050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adbeadb90f3861c1ea0865df8e6cad25d103d395df563e930d5a160cf7e2f375`  
		Last Modified: Wed, 13 Sep 2023 05:12:55 GMT  
		Size: 8.2 MB (8246481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:330d26826491947886007c6590f2fdb94adff1e5d784b065940137db990e03e1`  
		Last Modified: Wed, 13 Sep 2023 05:12:53 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03882acc2f421c5d355d6c95fa6e04e4efc0d1da2e508bdc9d79462576a7bb78`  
		Last Modified: Wed, 13 Sep 2023 05:12:53 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9218586c67df475e3efb7b40ec0e40680b7ea809104b035e378ae43af8a8680`  
		Last Modified: Wed, 13 Sep 2023 05:12:53 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:alpine`

```console
$ docker pull nats-streaming@sha256:9882310c6e2fe226e5f32dd9585362fd1af891a1ce4b30bcc90672569ff8243b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:alpine` - linux; amd64

```console
$ docker pull nats-streaming@sha256:b7c0263d4bd45bb96712677a0e1f0d3387f7134fc00cd7ea6e79418ac9c71ac3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.3 MB (11348069 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0257bac8bbcc527511fb5cb28eedd8672f09164257a648d9454dd51c15affd8f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Thu, 28 Sep 2023 21:19:27 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Thu, 28 Sep 2023 21:19:27 GMT
CMD ["/bin/sh"]
# Fri, 29 Sep 2023 00:08:58 GMT
ENV NATS_STREAMING_SERVER=0.25.5
# Fri, 29 Sep 2023 00:09:00 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='937af3f9cdbfe3cb4648cf8c8f505dded2cc175d59ba10e13ec71d1c04e61bf2' ;; 		armhf) natsArch='arm6'; sha256='5bd3a0456054505741b05e5d03acb9f7a5de97cf3ea20cd52d31edbae1c387ea' ;; 		armv7) natsArch='arm7'; sha256='0e643e9881cf3acf3313f84853451d1c4a1e731bc8599d223a40042f9c0c7285' ;; 		x86_64) natsArch='amd64'; sha256='22762f4d0ccfc75947096a14e09566b816113e125a3d39f7914a0c332bee25a7' ;; 		x86) natsArch='386'; sha256='92d8d4460f538883c78e67a334b23b2317e4fe58d46e4fdbbef8b4c09c7b97ae' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Fri, 29 Sep 2023 00:09:00 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Fri, 29 Sep 2023 00:09:00 GMT
EXPOSE 4222 8222
# Fri, 29 Sep 2023 00:09:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 29 Sep 2023 00:09:01 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b50dd55f68014712009de43839be3c41b5e61bf35a6740b5ce12c47ef53779d5`  
		Last Modified: Fri, 29 Sep 2023 00:09:23 GMT  
		Size: 7.9 MB (7945682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5816d53eb086b627f225dfc8f6ebc88fb00622e1fdd9fe878f3e0eb5cfde795b`  
		Last Modified: Fri, 29 Sep 2023 00:09:21 GMT  
		Size: 420.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:f71cd5237c12dc4014b14d5791131174fa2605a37dbb1abff7b137a728a0b513
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.7 MB (10746013 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a6de804939b3fcac9461ba70f44717298c30647aa635a03302eccbe8a0c093a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Thu, 28 Sep 2023 20:49:16 GMT
ADD file:2222b03381ff0fce22edd647f5c60529ec6a72202f8d3cb1d6e4648ebcd19a1e in / 
# Thu, 28 Sep 2023 20:49:16 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 22:10:33 GMT
ENV NATS_STREAMING_SERVER=0.25.5
# Thu, 28 Sep 2023 22:10:35 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='937af3f9cdbfe3cb4648cf8c8f505dded2cc175d59ba10e13ec71d1c04e61bf2' ;; 		armhf) natsArch='arm6'; sha256='5bd3a0456054505741b05e5d03acb9f7a5de97cf3ea20cd52d31edbae1c387ea' ;; 		armv7) natsArch='arm7'; sha256='0e643e9881cf3acf3313f84853451d1c4a1e731bc8599d223a40042f9c0c7285' ;; 		x86_64) natsArch='amd64'; sha256='22762f4d0ccfc75947096a14e09566b816113e125a3d39f7914a0c332bee25a7' ;; 		x86) natsArch='386'; sha256='92d8d4460f538883c78e67a334b23b2317e4fe58d46e4fdbbef8b4c09c7b97ae' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Thu, 28 Sep 2023 22:10:35 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Thu, 28 Sep 2023 22:10:36 GMT
EXPOSE 4222 8222
# Thu, 28 Sep 2023 22:10:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 28 Sep 2023 22:10:36 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:91cb83b91ee16f1ee0d588fccef56ab5dbb5689a64e5373caf33d7e4fe52ceb4`  
		Last Modified: Thu, 28 Sep 2023 20:51:25 GMT  
		Size: 3.1 MB (3145291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0445b5b06906bb6f0d5897ac5cec84996eb8b886638a3a482c09abe5e0e32cbe`  
		Last Modified: Thu, 28 Sep 2023 22:10:54 GMT  
		Size: 7.6 MB (7600298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed760df85f369bc55148f03fc0a8c27fef9b47457cc6916b7ef7aa8afeb081ed`  
		Last Modified: Thu, 28 Sep 2023 22:10:53 GMT  
		Size: 424.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:a77c3600f2290a15c97e8f26a243c8f40fa9fa4f5251a174ba607000b8d6fc87
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.5 MB (10488419 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d9cbce71f1ae3774c1bea17aeb3c9ebd9b29679316526697d74befebf17e391`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Thu, 28 Sep 2023 20:59:24 GMT
ADD file:61f54a318ad79861c6177783bb4c604412b5d952f45a9aa12ff97f4dccba7f73 in / 
# Thu, 28 Sep 2023 20:59:24 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 22:20:51 GMT
ENV NATS_STREAMING_SERVER=0.25.5
# Thu, 28 Sep 2023 22:20:55 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='937af3f9cdbfe3cb4648cf8c8f505dded2cc175d59ba10e13ec71d1c04e61bf2' ;; 		armhf) natsArch='arm6'; sha256='5bd3a0456054505741b05e5d03acb9f7a5de97cf3ea20cd52d31edbae1c387ea' ;; 		armv7) natsArch='arm7'; sha256='0e643e9881cf3acf3313f84853451d1c4a1e731bc8599d223a40042f9c0c7285' ;; 		x86_64) natsArch='amd64'; sha256='22762f4d0ccfc75947096a14e09566b816113e125a3d39f7914a0c332bee25a7' ;; 		x86) natsArch='386'; sha256='92d8d4460f538883c78e67a334b23b2317e4fe58d46e4fdbbef8b4c09c7b97ae' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Thu, 28 Sep 2023 22:20:55 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Thu, 28 Sep 2023 22:20:56 GMT
EXPOSE 4222 8222
# Thu, 28 Sep 2023 22:20:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 28 Sep 2023 22:20:57 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:622a0779436eb93ceea635e910268f867c2eba47d4f62f0bd45f0bd165af3572`  
		Last Modified: Thu, 28 Sep 2023 21:00:50 GMT  
		Size: 2.9 MB (2899905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0188c8c2d602e176e2f3fd95dfc4449d372745f654ecf1a15331d128a13ff308`  
		Last Modified: Thu, 28 Sep 2023 22:21:27 GMT  
		Size: 7.6 MB (7588094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0780bc6839fa58bce51e6d5d4b96f1d9cb9ac3e06e04aaedded20bdc6909fe72`  
		Last Modified: Thu, 28 Sep 2023 22:21:25 GMT  
		Size: 420.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:6d3f66596143b24da010280c677ec5454c6c9bd232e9a2f0f0361d53740e7037
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.6 MB (10632393 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb729c2a167ab94cdc8df4e6393ebd475aee993d9d22fb30b6f9b4d982e7aba8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Thu, 28 Sep 2023 20:39:33 GMT
ADD file:ff3112828967e8004a3264d7ece3f81c88e6a1d44d360b9b5613caab15b41717 in / 
# Thu, 28 Sep 2023 20:39:34 GMT
CMD ["/bin/sh"]
# Fri, 29 Sep 2023 02:07:03 GMT
ENV NATS_STREAMING_SERVER=0.25.5
# Fri, 29 Sep 2023 02:07:06 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='937af3f9cdbfe3cb4648cf8c8f505dded2cc175d59ba10e13ec71d1c04e61bf2' ;; 		armhf) natsArch='arm6'; sha256='5bd3a0456054505741b05e5d03acb9f7a5de97cf3ea20cd52d31edbae1c387ea' ;; 		armv7) natsArch='arm7'; sha256='0e643e9881cf3acf3313f84853451d1c4a1e731bc8599d223a40042f9c0c7285' ;; 		x86_64) natsArch='amd64'; sha256='22762f4d0ccfc75947096a14e09566b816113e125a3d39f7914a0c332bee25a7' ;; 		x86) natsArch='386'; sha256='92d8d4460f538883c78e67a334b23b2317e4fe58d46e4fdbbef8b4c09c7b97ae' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Fri, 29 Sep 2023 02:07:06 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Fri, 29 Sep 2023 02:07:06 GMT
EXPOSE 4222 8222
# Fri, 29 Sep 2023 02:07:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 29 Sep 2023 02:07:06 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:579b34f0a95bb83b3acd6b3249ddc52c3d80f5c84b13c944e9e324feb86dd329`  
		Last Modified: Thu, 28 Sep 2023 20:40:08 GMT  
		Size: 3.3 MB (3331831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b22a41d5f7e381035298ee771a08da6b89cf6aac2dc6bcfa7fb3d78615425edb`  
		Last Modified: Fri, 29 Sep 2023 02:07:24 GMT  
		Size: 7.3 MB (7300141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e297e142ef0e9c319179692d027cf31def6f553e423c2880e6b4d191e24a6889`  
		Last Modified: Fri, 29 Sep 2023 02:07:23 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:alpine3.18`

```console
$ docker pull nats-streaming@sha256:9882310c6e2fe226e5f32dd9585362fd1af891a1ce4b30bcc90672569ff8243b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:alpine3.18` - linux; amd64

```console
$ docker pull nats-streaming@sha256:b7c0263d4bd45bb96712677a0e1f0d3387f7134fc00cd7ea6e79418ac9c71ac3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.3 MB (11348069 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0257bac8bbcc527511fb5cb28eedd8672f09164257a648d9454dd51c15affd8f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Thu, 28 Sep 2023 21:19:27 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Thu, 28 Sep 2023 21:19:27 GMT
CMD ["/bin/sh"]
# Fri, 29 Sep 2023 00:08:58 GMT
ENV NATS_STREAMING_SERVER=0.25.5
# Fri, 29 Sep 2023 00:09:00 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='937af3f9cdbfe3cb4648cf8c8f505dded2cc175d59ba10e13ec71d1c04e61bf2' ;; 		armhf) natsArch='arm6'; sha256='5bd3a0456054505741b05e5d03acb9f7a5de97cf3ea20cd52d31edbae1c387ea' ;; 		armv7) natsArch='arm7'; sha256='0e643e9881cf3acf3313f84853451d1c4a1e731bc8599d223a40042f9c0c7285' ;; 		x86_64) natsArch='amd64'; sha256='22762f4d0ccfc75947096a14e09566b816113e125a3d39f7914a0c332bee25a7' ;; 		x86) natsArch='386'; sha256='92d8d4460f538883c78e67a334b23b2317e4fe58d46e4fdbbef8b4c09c7b97ae' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Fri, 29 Sep 2023 00:09:00 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Fri, 29 Sep 2023 00:09:00 GMT
EXPOSE 4222 8222
# Fri, 29 Sep 2023 00:09:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 29 Sep 2023 00:09:01 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b50dd55f68014712009de43839be3c41b5e61bf35a6740b5ce12c47ef53779d5`  
		Last Modified: Fri, 29 Sep 2023 00:09:23 GMT  
		Size: 7.9 MB (7945682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5816d53eb086b627f225dfc8f6ebc88fb00622e1fdd9fe878f3e0eb5cfde795b`  
		Last Modified: Fri, 29 Sep 2023 00:09:21 GMT  
		Size: 420.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine3.18` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:f71cd5237c12dc4014b14d5791131174fa2605a37dbb1abff7b137a728a0b513
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.7 MB (10746013 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a6de804939b3fcac9461ba70f44717298c30647aa635a03302eccbe8a0c093a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Thu, 28 Sep 2023 20:49:16 GMT
ADD file:2222b03381ff0fce22edd647f5c60529ec6a72202f8d3cb1d6e4648ebcd19a1e in / 
# Thu, 28 Sep 2023 20:49:16 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 22:10:33 GMT
ENV NATS_STREAMING_SERVER=0.25.5
# Thu, 28 Sep 2023 22:10:35 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='937af3f9cdbfe3cb4648cf8c8f505dded2cc175d59ba10e13ec71d1c04e61bf2' ;; 		armhf) natsArch='arm6'; sha256='5bd3a0456054505741b05e5d03acb9f7a5de97cf3ea20cd52d31edbae1c387ea' ;; 		armv7) natsArch='arm7'; sha256='0e643e9881cf3acf3313f84853451d1c4a1e731bc8599d223a40042f9c0c7285' ;; 		x86_64) natsArch='amd64'; sha256='22762f4d0ccfc75947096a14e09566b816113e125a3d39f7914a0c332bee25a7' ;; 		x86) natsArch='386'; sha256='92d8d4460f538883c78e67a334b23b2317e4fe58d46e4fdbbef8b4c09c7b97ae' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Thu, 28 Sep 2023 22:10:35 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Thu, 28 Sep 2023 22:10:36 GMT
EXPOSE 4222 8222
# Thu, 28 Sep 2023 22:10:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 28 Sep 2023 22:10:36 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:91cb83b91ee16f1ee0d588fccef56ab5dbb5689a64e5373caf33d7e4fe52ceb4`  
		Last Modified: Thu, 28 Sep 2023 20:51:25 GMT  
		Size: 3.1 MB (3145291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0445b5b06906bb6f0d5897ac5cec84996eb8b886638a3a482c09abe5e0e32cbe`  
		Last Modified: Thu, 28 Sep 2023 22:10:54 GMT  
		Size: 7.6 MB (7600298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed760df85f369bc55148f03fc0a8c27fef9b47457cc6916b7ef7aa8afeb081ed`  
		Last Modified: Thu, 28 Sep 2023 22:10:53 GMT  
		Size: 424.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine3.18` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:a77c3600f2290a15c97e8f26a243c8f40fa9fa4f5251a174ba607000b8d6fc87
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.5 MB (10488419 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d9cbce71f1ae3774c1bea17aeb3c9ebd9b29679316526697d74befebf17e391`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Thu, 28 Sep 2023 20:59:24 GMT
ADD file:61f54a318ad79861c6177783bb4c604412b5d952f45a9aa12ff97f4dccba7f73 in / 
# Thu, 28 Sep 2023 20:59:24 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 22:20:51 GMT
ENV NATS_STREAMING_SERVER=0.25.5
# Thu, 28 Sep 2023 22:20:55 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='937af3f9cdbfe3cb4648cf8c8f505dded2cc175d59ba10e13ec71d1c04e61bf2' ;; 		armhf) natsArch='arm6'; sha256='5bd3a0456054505741b05e5d03acb9f7a5de97cf3ea20cd52d31edbae1c387ea' ;; 		armv7) natsArch='arm7'; sha256='0e643e9881cf3acf3313f84853451d1c4a1e731bc8599d223a40042f9c0c7285' ;; 		x86_64) natsArch='amd64'; sha256='22762f4d0ccfc75947096a14e09566b816113e125a3d39f7914a0c332bee25a7' ;; 		x86) natsArch='386'; sha256='92d8d4460f538883c78e67a334b23b2317e4fe58d46e4fdbbef8b4c09c7b97ae' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Thu, 28 Sep 2023 22:20:55 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Thu, 28 Sep 2023 22:20:56 GMT
EXPOSE 4222 8222
# Thu, 28 Sep 2023 22:20:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 28 Sep 2023 22:20:57 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:622a0779436eb93ceea635e910268f867c2eba47d4f62f0bd45f0bd165af3572`  
		Last Modified: Thu, 28 Sep 2023 21:00:50 GMT  
		Size: 2.9 MB (2899905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0188c8c2d602e176e2f3fd95dfc4449d372745f654ecf1a15331d128a13ff308`  
		Last Modified: Thu, 28 Sep 2023 22:21:27 GMT  
		Size: 7.6 MB (7588094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0780bc6839fa58bce51e6d5d4b96f1d9cb9ac3e06e04aaedded20bdc6909fe72`  
		Last Modified: Thu, 28 Sep 2023 22:21:25 GMT  
		Size: 420.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine3.18` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:6d3f66596143b24da010280c677ec5454c6c9bd232e9a2f0f0361d53740e7037
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.6 MB (10632393 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb729c2a167ab94cdc8df4e6393ebd475aee993d9d22fb30b6f9b4d982e7aba8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Thu, 28 Sep 2023 20:39:33 GMT
ADD file:ff3112828967e8004a3264d7ece3f81c88e6a1d44d360b9b5613caab15b41717 in / 
# Thu, 28 Sep 2023 20:39:34 GMT
CMD ["/bin/sh"]
# Fri, 29 Sep 2023 02:07:03 GMT
ENV NATS_STREAMING_SERVER=0.25.5
# Fri, 29 Sep 2023 02:07:06 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='937af3f9cdbfe3cb4648cf8c8f505dded2cc175d59ba10e13ec71d1c04e61bf2' ;; 		armhf) natsArch='arm6'; sha256='5bd3a0456054505741b05e5d03acb9f7a5de97cf3ea20cd52d31edbae1c387ea' ;; 		armv7) natsArch='arm7'; sha256='0e643e9881cf3acf3313f84853451d1c4a1e731bc8599d223a40042f9c0c7285' ;; 		x86_64) natsArch='amd64'; sha256='22762f4d0ccfc75947096a14e09566b816113e125a3d39f7914a0c332bee25a7' ;; 		x86) natsArch='386'; sha256='92d8d4460f538883c78e67a334b23b2317e4fe58d46e4fdbbef8b4c09c7b97ae' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Fri, 29 Sep 2023 02:07:06 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Fri, 29 Sep 2023 02:07:06 GMT
EXPOSE 4222 8222
# Fri, 29 Sep 2023 02:07:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 29 Sep 2023 02:07:06 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:579b34f0a95bb83b3acd6b3249ddc52c3d80f5c84b13c944e9e324feb86dd329`  
		Last Modified: Thu, 28 Sep 2023 20:40:08 GMT  
		Size: 3.3 MB (3331831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b22a41d5f7e381035298ee771a08da6b89cf6aac2dc6bcfa7fb3d78615425edb`  
		Last Modified: Fri, 29 Sep 2023 02:07:24 GMT  
		Size: 7.3 MB (7300141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e297e142ef0e9c319179692d027cf31def6f553e423c2880e6b4d191e24a6889`  
		Last Modified: Fri, 29 Sep 2023 02:07:23 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:latest`

```console
$ docker pull nats-streaming@sha256:87741883f95fe650defcd3154a8547810b177141b0544aec09406b956ca5c95c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.4851; amd64

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

### `nats-streaming:latest` - windows version 10.0.17763.4851; amd64

```console
$ docker pull nats-streaming@sha256:2f645551c661a9bdfa1f098de630c345560b42b46ea4f86e4358496fdb7e2c44
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.3 MB (112283602 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6811dea88de0d1562552c6c359244361ee425743d9227dd15ab5dc36b22a88f1`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 29 Aug 2023 16:42:02 GMT
RUN Apply image 10.0.17763.4851
# Wed, 13 Sep 2023 05:08:03 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 13 Sep 2023 05:12:32 GMT
RUN cmd /S /C #(nop) COPY file:0e2c8ba21e47adc90962b46928c928315462bcddaefcbc01f98113f4f66cda4a in C:\nats-streaming-server.exe 
# Wed, 13 Sep 2023 05:12:32 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 13 Sep 2023 05:12:33 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 13 Sep 2023 05:12:34 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:17ba6b878467260559b72cb6f7e79c829eae67862a09efe87f6dc324f49fc086`  
		Last Modified: Tue, 12 Sep 2023 18:31:40 GMT  
		Size: 104.5 MB (104492504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3baa9930674eb6676a1690e63a275d0da517ab8b8aeab7ccd20591f76f7c69a5`  
		Last Modified: Wed, 13 Sep 2023 05:08:48 GMT  
		Size: 1.2 KB (1182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b636690ea2cc8ecb38fcf9cec506c8c908ffe8096160b8549693ae2b6d1aab6`  
		Last Modified: Wed, 13 Sep 2023 05:13:10 GMT  
		Size: 7.8 MB (7786448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02b0f65c350b20f8ac4d372a7e811aff70b8dbcba45d5850be6e80259d1c8544`  
		Last Modified: Wed, 13 Sep 2023 05:13:08 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:181e9541dcd4167889f09d7139f64341ad22ff535be6578fbc55b09600bf8777`  
		Last Modified: Wed, 13 Sep 2023 05:13:08 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1e99090f84ed38c5eac15db96cb5f1e79ff34ddf90739902a0e20c7c5a49280`  
		Last Modified: Wed, 13 Sep 2023 05:13:08 GMT  
		Size: 1.2 KB (1156 bytes)  
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
$ docker pull nats-streaming@sha256:b661b1af7d63f50e0550e23204e3a544e5c351a613a832386aee365bcce484d8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4851; amd64

### `nats-streaming:nanoserver` - windows version 10.0.17763.4851; amd64

```console
$ docker pull nats-streaming@sha256:2f645551c661a9bdfa1f098de630c345560b42b46ea4f86e4358496fdb7e2c44
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.3 MB (112283602 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6811dea88de0d1562552c6c359244361ee425743d9227dd15ab5dc36b22a88f1`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 29 Aug 2023 16:42:02 GMT
RUN Apply image 10.0.17763.4851
# Wed, 13 Sep 2023 05:08:03 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 13 Sep 2023 05:12:32 GMT
RUN cmd /S /C #(nop) COPY file:0e2c8ba21e47adc90962b46928c928315462bcddaefcbc01f98113f4f66cda4a in C:\nats-streaming-server.exe 
# Wed, 13 Sep 2023 05:12:32 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 13 Sep 2023 05:12:33 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 13 Sep 2023 05:12:34 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:17ba6b878467260559b72cb6f7e79c829eae67862a09efe87f6dc324f49fc086`  
		Last Modified: Tue, 12 Sep 2023 18:31:40 GMT  
		Size: 104.5 MB (104492504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3baa9930674eb6676a1690e63a275d0da517ab8b8aeab7ccd20591f76f7c69a5`  
		Last Modified: Wed, 13 Sep 2023 05:08:48 GMT  
		Size: 1.2 KB (1182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b636690ea2cc8ecb38fcf9cec506c8c908ffe8096160b8549693ae2b6d1aab6`  
		Last Modified: Wed, 13 Sep 2023 05:13:10 GMT  
		Size: 7.8 MB (7786448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02b0f65c350b20f8ac4d372a7e811aff70b8dbcba45d5850be6e80259d1c8544`  
		Last Modified: Wed, 13 Sep 2023 05:13:08 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:181e9541dcd4167889f09d7139f64341ad22ff535be6578fbc55b09600bf8777`  
		Last Modified: Wed, 13 Sep 2023 05:13:08 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1e99090f84ed38c5eac15db96cb5f1e79ff34ddf90739902a0e20c7c5a49280`  
		Last Modified: Wed, 13 Sep 2023 05:13:08 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:nanoserver-1809`

```console
$ docker pull nats-streaming@sha256:b661b1af7d63f50e0550e23204e3a544e5c351a613a832386aee365bcce484d8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4851; amd64

### `nats-streaming:nanoserver-1809` - windows version 10.0.17763.4851; amd64

```console
$ docker pull nats-streaming@sha256:2f645551c661a9bdfa1f098de630c345560b42b46ea4f86e4358496fdb7e2c44
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.3 MB (112283602 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6811dea88de0d1562552c6c359244361ee425743d9227dd15ab5dc36b22a88f1`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 29 Aug 2023 16:42:02 GMT
RUN Apply image 10.0.17763.4851
# Wed, 13 Sep 2023 05:08:03 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 13 Sep 2023 05:12:32 GMT
RUN cmd /S /C #(nop) COPY file:0e2c8ba21e47adc90962b46928c928315462bcddaefcbc01f98113f4f66cda4a in C:\nats-streaming-server.exe 
# Wed, 13 Sep 2023 05:12:32 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 13 Sep 2023 05:12:33 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 13 Sep 2023 05:12:34 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:17ba6b878467260559b72cb6f7e79c829eae67862a09efe87f6dc324f49fc086`  
		Last Modified: Tue, 12 Sep 2023 18:31:40 GMT  
		Size: 104.5 MB (104492504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3baa9930674eb6676a1690e63a275d0da517ab8b8aeab7ccd20591f76f7c69a5`  
		Last Modified: Wed, 13 Sep 2023 05:08:48 GMT  
		Size: 1.2 KB (1182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b636690ea2cc8ecb38fcf9cec506c8c908ffe8096160b8549693ae2b6d1aab6`  
		Last Modified: Wed, 13 Sep 2023 05:13:10 GMT  
		Size: 7.8 MB (7786448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02b0f65c350b20f8ac4d372a7e811aff70b8dbcba45d5850be6e80259d1c8544`  
		Last Modified: Wed, 13 Sep 2023 05:13:08 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:181e9541dcd4167889f09d7139f64341ad22ff535be6578fbc55b09600bf8777`  
		Last Modified: Wed, 13 Sep 2023 05:13:08 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1e99090f84ed38c5eac15db96cb5f1e79ff34ddf90739902a0e20c7c5a49280`  
		Last Modified: Wed, 13 Sep 2023 05:13:08 GMT  
		Size: 1.2 KB (1156 bytes)  
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
$ docker pull nats-streaming@sha256:c0663722b63c368a5244ea3a4e9fe0d1191d3d884a285ca3462b49bc6ce3e425
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4851; amd64

### `nats-streaming:windowsservercore` - windows version 10.0.17763.4851; amd64

```console
$ docker pull nats-streaming@sha256:fd7cb14102d8c704ea297bc89b1a4ed0678e61ab010244b0f10c9caf9aace084
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2024830683 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48ab6bb07050789abd05c33284cfc3969f3c0d76314409cd61493ba62f861df3`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Tue, 29 Aug 2023 17:09:18 GMT
RUN Install update 10.0.17763.4851
# Wed, 13 Sep 2023 03:56:42 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 Sep 2023 05:05:36 GMT
ENV NATS_DOCKERIZED=1
# Wed, 13 Sep 2023 05:09:31 GMT
ENV NATS_STREAMING_SERVER=0.25.5
# Wed, 13 Sep 2023 05:09:32 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.25.5/nats-streaming-server-v0.25.5-windows-amd64.zip
# Wed, 13 Sep 2023 05:09:33 GMT
ENV NATS_STREAMING_SERVER_SHASUM=709b481bfa3537dc7941490365e065554f19c7029830d765ef49e8cd16657b75
# Wed, 13 Sep 2023 05:10:31 GMT
RUN Set-PSDebug -Trace 2
# Wed, 13 Sep 2023 05:12:11 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 13 Sep 2023 05:12:11 GMT
EXPOSE 4222 8222
# Wed, 13 Sep 2023 05:12:12 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 13 Sep 2023 05:12:13 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:179757339e051b99f9a62375fed8f87ffcc4df0eeedb984d20b485bdd089ad08`  
		Last Modified: Tue, 12 Sep 2023 19:41:25 GMT  
		Size: 365.7 MB (365709508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b21bbf840142288ae2bce3465085b591133cf10f78f7dda43277db4838332d8`  
		Last Modified: Wed, 13 Sep 2023 04:36:45 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b54f616fe064e9d4e73bf2aec9a4fe9c58837ec84c2fc998a54ab7a77b52e109`  
		Last Modified: Wed, 13 Sep 2023 05:08:32 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a663613aba018dc846e9dbd32363a68699885ecfc832dd1440a60f531211b506`  
		Last Modified: Wed, 13 Sep 2023 05:12:55 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05ded5f7ebb06ada7d9bd8d7108a90abed6616e6f34c16a99b1dfa3009424fc8`  
		Last Modified: Wed, 13 Sep 2023 05:12:55 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb620195a9df9d4492561a3a9dde486cc331cad8803e7abd659b32b1fb6d88ec`  
		Last Modified: Wed, 13 Sep 2023 05:12:55 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dc7eb1b31cf8667a9011b08200a46d79e72735d944a58592cc8c497b2fba9ea`  
		Last Modified: Wed, 13 Sep 2023 05:12:54 GMT  
		Size: 243.1 KB (243050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adbeadb90f3861c1ea0865df8e6cad25d103d395df563e930d5a160cf7e2f375`  
		Last Modified: Wed, 13 Sep 2023 05:12:55 GMT  
		Size: 8.2 MB (8246481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:330d26826491947886007c6590f2fdb94adff1e5d784b065940137db990e03e1`  
		Last Modified: Wed, 13 Sep 2023 05:12:53 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03882acc2f421c5d355d6c95fa6e04e4efc0d1da2e508bdc9d79462576a7bb78`  
		Last Modified: Wed, 13 Sep 2023 05:12:53 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9218586c67df475e3efb7b40ec0e40680b7ea809104b035e378ae43af8a8680`  
		Last Modified: Wed, 13 Sep 2023 05:12:53 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:windowsservercore-1809`

```console
$ docker pull nats-streaming@sha256:c0663722b63c368a5244ea3a4e9fe0d1191d3d884a285ca3462b49bc6ce3e425
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4851; amd64

### `nats-streaming:windowsservercore-1809` - windows version 10.0.17763.4851; amd64

```console
$ docker pull nats-streaming@sha256:fd7cb14102d8c704ea297bc89b1a4ed0678e61ab010244b0f10c9caf9aace084
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2024830683 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48ab6bb07050789abd05c33284cfc3969f3c0d76314409cd61493ba62f861df3`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Tue, 29 Aug 2023 17:09:18 GMT
RUN Install update 10.0.17763.4851
# Wed, 13 Sep 2023 03:56:42 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 Sep 2023 05:05:36 GMT
ENV NATS_DOCKERIZED=1
# Wed, 13 Sep 2023 05:09:31 GMT
ENV NATS_STREAMING_SERVER=0.25.5
# Wed, 13 Sep 2023 05:09:32 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.25.5/nats-streaming-server-v0.25.5-windows-amd64.zip
# Wed, 13 Sep 2023 05:09:33 GMT
ENV NATS_STREAMING_SERVER_SHASUM=709b481bfa3537dc7941490365e065554f19c7029830d765ef49e8cd16657b75
# Wed, 13 Sep 2023 05:10:31 GMT
RUN Set-PSDebug -Trace 2
# Wed, 13 Sep 2023 05:12:11 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 13 Sep 2023 05:12:11 GMT
EXPOSE 4222 8222
# Wed, 13 Sep 2023 05:12:12 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 13 Sep 2023 05:12:13 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:179757339e051b99f9a62375fed8f87ffcc4df0eeedb984d20b485bdd089ad08`  
		Last Modified: Tue, 12 Sep 2023 19:41:25 GMT  
		Size: 365.7 MB (365709508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b21bbf840142288ae2bce3465085b591133cf10f78f7dda43277db4838332d8`  
		Last Modified: Wed, 13 Sep 2023 04:36:45 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b54f616fe064e9d4e73bf2aec9a4fe9c58837ec84c2fc998a54ab7a77b52e109`  
		Last Modified: Wed, 13 Sep 2023 05:08:32 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a663613aba018dc846e9dbd32363a68699885ecfc832dd1440a60f531211b506`  
		Last Modified: Wed, 13 Sep 2023 05:12:55 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05ded5f7ebb06ada7d9bd8d7108a90abed6616e6f34c16a99b1dfa3009424fc8`  
		Last Modified: Wed, 13 Sep 2023 05:12:55 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb620195a9df9d4492561a3a9dde486cc331cad8803e7abd659b32b1fb6d88ec`  
		Last Modified: Wed, 13 Sep 2023 05:12:55 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dc7eb1b31cf8667a9011b08200a46d79e72735d944a58592cc8c497b2fba9ea`  
		Last Modified: Wed, 13 Sep 2023 05:12:54 GMT  
		Size: 243.1 KB (243050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adbeadb90f3861c1ea0865df8e6cad25d103d395df563e930d5a160cf7e2f375`  
		Last Modified: Wed, 13 Sep 2023 05:12:55 GMT  
		Size: 8.2 MB (8246481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:330d26826491947886007c6590f2fdb94adff1e5d784b065940137db990e03e1`  
		Last Modified: Wed, 13 Sep 2023 05:12:53 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03882acc2f421c5d355d6c95fa6e04e4efc0d1da2e508bdc9d79462576a7bb78`  
		Last Modified: Wed, 13 Sep 2023 05:12:53 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9218586c67df475e3efb7b40ec0e40680b7ea809104b035e378ae43af8a8680`  
		Last Modified: Wed, 13 Sep 2023 05:12:53 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
