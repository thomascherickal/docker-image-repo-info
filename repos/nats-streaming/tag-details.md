<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `nats-streaming`

-	[`nats-streaming:0.21`](#nats-streaming021)
-	[`nats-streaming:0.21.1`](#nats-streaming0211)
-	[`nats-streaming:0.21.1-alpine`](#nats-streaming0211-alpine)
-	[`nats-streaming:0.21.1-alpine3.13`](#nats-streaming0211-alpine313)
-	[`nats-streaming:0.21.1-linux`](#nats-streaming0211-linux)
-	[`nats-streaming:0.21.1-nanoserver`](#nats-streaming0211-nanoserver)
-	[`nats-streaming:0.21.1-nanoserver-1809`](#nats-streaming0211-nanoserver-1809)
-	[`nats-streaming:0.21.1-scratch`](#nats-streaming0211-scratch)
-	[`nats-streaming:0.21.1-windowsservercore`](#nats-streaming0211-windowsservercore)
-	[`nats-streaming:0.21.1-windowsservercore-1809`](#nats-streaming0211-windowsservercore-1809)
-	[`nats-streaming:0.21.1-windowsservercore-ltsc2016`](#nats-streaming0211-windowsservercore-ltsc2016)
-	[`nats-streaming:0.21-alpine`](#nats-streaming021-alpine)
-	[`nats-streaming:0.21-alpine3.13`](#nats-streaming021-alpine313)
-	[`nats-streaming:0.21-linux`](#nats-streaming021-linux)
-	[`nats-streaming:0.21-nanoserver`](#nats-streaming021-nanoserver)
-	[`nats-streaming:0.21-nanoserver-1809`](#nats-streaming021-nanoserver-1809)
-	[`nats-streaming:0.21-scratch`](#nats-streaming021-scratch)
-	[`nats-streaming:0.21-windowsservercore`](#nats-streaming021-windowsservercore)
-	[`nats-streaming:0.21-windowsservercore-1809`](#nats-streaming021-windowsservercore-1809)
-	[`nats-streaming:0.21-windowsservercore-ltsc2016`](#nats-streaming021-windowsservercore-ltsc2016)
-	[`nats-streaming:alpine`](#nats-streamingalpine)
-	[`nats-streaming:alpine3.13`](#nats-streamingalpine313)
-	[`nats-streaming:latest`](#nats-streaminglatest)
-	[`nats-streaming:linux`](#nats-streaminglinux)
-	[`nats-streaming:nanoserver`](#nats-streamingnanoserver)
-	[`nats-streaming:nanoserver-1809`](#nats-streamingnanoserver-1809)
-	[`nats-streaming:scratch`](#nats-streamingscratch)
-	[`nats-streaming:windowsservercore`](#nats-streamingwindowsservercore)
-	[`nats-streaming:windowsservercore-1809`](#nats-streamingwindowsservercore-1809)
-	[`nats-streaming:windowsservercore-ltsc2016`](#nats-streamingwindowsservercore-ltsc2016)

## `nats-streaming:0.21`

```console
$ docker pull nats-streaming@sha256:b5fcf8cc22f7bc9bc8724023dfee42d39861c20760558f0a2863987ae20214c4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.1757; amd64

### `nats-streaming:0.21` - linux; amd64

```console
$ docker pull nats-streaming@sha256:3783631861947e0e679506679efc64c4875f4804205377e4311e9cdab6c17965
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.7 MB (5679887 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:699c5c09ce0b6a8314d7acec3aa4c72dbaa6a6bc44881fa83719dcf5e2e5a1e1`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 02 Mar 2021 00:25:52 GMT
COPY file:4c2a24d146429270418a17857993903d39b1fcf52d11a560abd159eff99ada8d in /nats-streaming-server 
# Tue, 02 Mar 2021 00:25:52 GMT
EXPOSE 4222 8222
# Tue, 02 Mar 2021 00:25:53 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 02 Mar 2021 00:25:53 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:7fb87f3f85e42eb0fc3d88581c0b84a8d675859dd6727be9100fa9bbaa2cffa4`  
		Last Modified: Tue, 02 Mar 2021 00:26:20 GMT  
		Size: 5.7 MB (5679887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.21` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:48598a6e49d6cdd1e0829bd4d7ead1aff8b18dd07440a20337e701a94caca26e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.3 MB (5250920 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dffd1cc2cc6030e177fe45935f0fee3c62a59fdda8b12c3276d39fa19a6928b1`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 02 Mar 2021 00:26:52 GMT
COPY file:4baaca51b76d42c66f7a4d5146b598f666c38803f36a5286ede362691d89663c in /nats-streaming-server 
# Tue, 02 Mar 2021 00:26:53 GMT
EXPOSE 4222 8222
# Tue, 02 Mar 2021 00:26:53 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 02 Mar 2021 00:26:54 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:92433c508db76d76c2073b4044b8e2a847d00a4148b85326fe4be63f691ef9af`  
		Last Modified: Tue, 02 Mar 2021 00:27:35 GMT  
		Size: 5.3 MB (5250920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.21` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:ae774aee41bd64306207d739d2290639f673c9c66c367a83f155a923fe8c13f6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5246286 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ce52186dd957f6b70b086fdcbc8212e079e5ed5e3e0013f8f72b3922535a56e`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Sat, 06 Mar 2021 01:00:25 GMT
COPY file:546c18b3e8e91d453d1a325c6e4dbc3c945564c010676da1abe89a653a0dea84 in /nats-streaming-server 
# Sat, 06 Mar 2021 01:00:27 GMT
EXPOSE 4222 8222
# Sat, 06 Mar 2021 01:00:28 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Sat, 06 Mar 2021 01:00:29 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:ed8ed2aa5d978cf51ebe3454de1832aeb40919052c5cb17d5b63865c31fc03c7`  
		Last Modified: Sat, 06 Mar 2021 01:01:07 GMT  
		Size: 5.2 MB (5246286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.21` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:bb0f75068ef5a23352dc064f1f3284e6dab1c2586e6a94e2e606778b78cb03f7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5169160 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6cebf86c02f91c34c49641b50fa91c94e4100b2fa18472ca33b362283355e4c1`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 02 Mar 2021 01:14:35 GMT
COPY file:45fcdc5032324b9c78e16535704285519687d0187fa1b424eb18143deb1dece7 in /nats-streaming-server 
# Tue, 02 Mar 2021 01:14:35 GMT
EXPOSE 4222 8222
# Tue, 02 Mar 2021 01:14:36 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 02 Mar 2021 01:14:37 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:8e9b3f150b42f0a6abecb65490e22f7a6a73c1e139f69e747ca01b46f0c4ff5d`  
		Last Modified: Tue, 02 Mar 2021 01:15:22 GMT  
		Size: 5.2 MB (5169160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.21` - windows version 10.0.17763.1757; amd64

```console
$ docker pull nats-streaming@sha256:7102fdfcfc56aff3af3af39cec63c0601b43592e56b7e64d187790b0822e9a51
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.2 MB (107219449 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a8a29d1082c9d4ea1c812a4e8d84b8d8c1228d2c1c0c1543350e44bd28b31f4f`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 02 Feb 2021 13:06:30 GMT
RUN Apply image 1809-amd64
# Wed, 10 Feb 2021 16:02:26 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Mon, 01 Mar 2021 23:39:47 GMT
RUN cmd /S /C #(nop) COPY file:24ef21e1be266c0481785b3d2cebe511e1bb8a8c20c99795a9e7fa85b0d7aa50 in C:\nats-streaming-server.exe 
# Mon, 01 Mar 2021 23:39:48 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Mon, 01 Mar 2021 23:39:49 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Mon, 01 Mar 2021 23:39:50 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:ba17af31b9276ee11fdf859681b442db50979a39eff4cea2a559a5755cedbe01`  
		Size: 101.4 MB (101406193 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:23b613036f8aee9066e712b3aa58f10f2fde093623511a5658867f53a6d01b18`  
		Last Modified: Wed, 10 Feb 2021 16:06:34 GMT  
		Size: 1.1 KB (1071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:698ae4ae8df313350ab9792ea25a077b988b965eec472e98f4770b8f5b16ed33`  
		Last Modified: Mon, 01 Mar 2021 23:44:05 GMT  
		Size: 5.8 MB (5808961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec3f2e5ff2ba6f6a9881c98155b50d51c881cd77ced1ed2d75b60867bbc96e65`  
		Last Modified: Mon, 01 Mar 2021 23:43:57 GMT  
		Size: 1.1 KB (1064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aa08ef55ec2e1a3c6b2f7f88cf21aa125c7f3356775287b4f3d83372278cb4e`  
		Last Modified: Mon, 01 Mar 2021 23:43:58 GMT  
		Size: 1.0 KB (1033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af33a16b15f810a8bdb3cfe7c2387d435251d11cd9af0a3d5bf3ee30410ccc51`  
		Last Modified: Mon, 01 Mar 2021 23:43:58 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.21.1`

```console
$ docker pull nats-streaming@sha256:14ace5b780a3e1e3e843bace9214da6c6e6412067aac18835876671d534fe421
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; arm variant v7

### `nats-streaming:0.21.1` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:ae774aee41bd64306207d739d2290639f673c9c66c367a83f155a923fe8c13f6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5246286 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ce52186dd957f6b70b086fdcbc8212e079e5ed5e3e0013f8f72b3922535a56e`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Sat, 06 Mar 2021 01:00:25 GMT
COPY file:546c18b3e8e91d453d1a325c6e4dbc3c945564c010676da1abe89a653a0dea84 in /nats-streaming-server 
# Sat, 06 Mar 2021 01:00:27 GMT
EXPOSE 4222 8222
# Sat, 06 Mar 2021 01:00:28 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Sat, 06 Mar 2021 01:00:29 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:ed8ed2aa5d978cf51ebe3454de1832aeb40919052c5cb17d5b63865c31fc03c7`  
		Last Modified: Sat, 06 Mar 2021 01:01:07 GMT  
		Size: 5.2 MB (5246286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.21.1-alpine`

```console
$ docker pull nats-streaming@sha256:4dce5b202dfeec0f447edd96c2f50a78b3dcbcdecd3f0a766c96f1a5a3139cbf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; arm variant v7

### `nats-streaming:0.21.1-alpine` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:782e4290f2c50dd5e8a0714f8cfa35d8575577910ff3252c757d3a64e6bd4d47
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.0 MB (7951510 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a88cdb45d1d7d80ee678f8f1ca18f6c67822632552ea1ceb8a6a91ecc72503f4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 17 Feb 2021 20:57:36 GMT
ADD file:efdd39e5243eaf378f12ad5a85d2222b44930850a90263e5f17e8a6b5e9bc9b8 in / 
# Wed, 17 Feb 2021 20:57:37 GMT
CMD ["/bin/sh"]
# Sat, 06 Mar 2021 00:59:37 GMT
ENV NATS_STREAMING_SERVER=0.21.1
# Sat, 06 Mar 2021 00:59:41 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='06d591a61084aab1046e818486c2ee7c3936214c92dc257084693d6ffe06342b' ;; 		armhf) natsArch='arm6'; sha256='085375782abe1bacbd6fc609ce6a6721f029cba312733479204c89bf92f1e188' ;; 		armv7) natsArch='arm7'; sha256='947d91512b47ba98198bef7f799670c40cf6949f2ba2e98b5c133e6166e9b97c' ;; 		x86_64) natsArch='amd64'; sha256='85fd7fd3c7b71cbc9043900f9110b028f1fdc042c6500eed065e6e2c3331f62e' ;; 		x86) natsArch='386'; sha256='475b0f015726af99c9ea779c8bbbeaa729ef90f43dd2715273fea81fb90ea63a' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Sat, 06 Mar 2021 00:59:43 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Sat, 06 Mar 2021 00:59:43 GMT
EXPOSE 4222 8222
# Sat, 06 Mar 2021 00:59:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 06 Mar 2021 00:59:44 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:f55b840e27d3dbe27e44497103a4397f043749f933eb0433d29e2f104b3435ef`  
		Last Modified: Wed, 17 Feb 2021 20:58:14 GMT  
		Size: 2.4 MB (2423892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b550ac0781e9d06a2d5602aa128b8085d9808f31821df0db0fdb3378e4beb64`  
		Last Modified: Sat, 06 Mar 2021 01:00:55 GMT  
		Size: 5.5 MB (5527196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c9fcc13222a0356f1399ed180350034d92d18fa5262cd34421cb52915ca14df`  
		Last Modified: Sat, 06 Mar 2021 01:00:53 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.21.1-alpine3.13`

```console
$ docker pull nats-streaming@sha256:4dce5b202dfeec0f447edd96c2f50a78b3dcbcdecd3f0a766c96f1a5a3139cbf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; arm variant v7

### `nats-streaming:0.21.1-alpine3.13` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:782e4290f2c50dd5e8a0714f8cfa35d8575577910ff3252c757d3a64e6bd4d47
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.0 MB (7951510 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a88cdb45d1d7d80ee678f8f1ca18f6c67822632552ea1ceb8a6a91ecc72503f4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 17 Feb 2021 20:57:36 GMT
ADD file:efdd39e5243eaf378f12ad5a85d2222b44930850a90263e5f17e8a6b5e9bc9b8 in / 
# Wed, 17 Feb 2021 20:57:37 GMT
CMD ["/bin/sh"]
# Sat, 06 Mar 2021 00:59:37 GMT
ENV NATS_STREAMING_SERVER=0.21.1
# Sat, 06 Mar 2021 00:59:41 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='06d591a61084aab1046e818486c2ee7c3936214c92dc257084693d6ffe06342b' ;; 		armhf) natsArch='arm6'; sha256='085375782abe1bacbd6fc609ce6a6721f029cba312733479204c89bf92f1e188' ;; 		armv7) natsArch='arm7'; sha256='947d91512b47ba98198bef7f799670c40cf6949f2ba2e98b5c133e6166e9b97c' ;; 		x86_64) natsArch='amd64'; sha256='85fd7fd3c7b71cbc9043900f9110b028f1fdc042c6500eed065e6e2c3331f62e' ;; 		x86) natsArch='386'; sha256='475b0f015726af99c9ea779c8bbbeaa729ef90f43dd2715273fea81fb90ea63a' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Sat, 06 Mar 2021 00:59:43 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Sat, 06 Mar 2021 00:59:43 GMT
EXPOSE 4222 8222
# Sat, 06 Mar 2021 00:59:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 06 Mar 2021 00:59:44 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:f55b840e27d3dbe27e44497103a4397f043749f933eb0433d29e2f104b3435ef`  
		Last Modified: Wed, 17 Feb 2021 20:58:14 GMT  
		Size: 2.4 MB (2423892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b550ac0781e9d06a2d5602aa128b8085d9808f31821df0db0fdb3378e4beb64`  
		Last Modified: Sat, 06 Mar 2021 01:00:55 GMT  
		Size: 5.5 MB (5527196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c9fcc13222a0356f1399ed180350034d92d18fa5262cd34421cb52915ca14df`  
		Last Modified: Sat, 06 Mar 2021 01:00:53 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.21.1-linux`

```console
$ docker pull nats-streaming@sha256:14ace5b780a3e1e3e843bace9214da6c6e6412067aac18835876671d534fe421
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; arm variant v7

### `nats-streaming:0.21.1-linux` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:ae774aee41bd64306207d739d2290639f673c9c66c367a83f155a923fe8c13f6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5246286 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ce52186dd957f6b70b086fdcbc8212e079e5ed5e3e0013f8f72b3922535a56e`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Sat, 06 Mar 2021 01:00:25 GMT
COPY file:546c18b3e8e91d453d1a325c6e4dbc3c945564c010676da1abe89a653a0dea84 in /nats-streaming-server 
# Sat, 06 Mar 2021 01:00:27 GMT
EXPOSE 4222 8222
# Sat, 06 Mar 2021 01:00:28 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Sat, 06 Mar 2021 01:00:29 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:ed8ed2aa5d978cf51ebe3454de1832aeb40919052c5cb17d5b63865c31fc03c7`  
		Last Modified: Sat, 06 Mar 2021 01:01:07 GMT  
		Size: 5.2 MB (5246286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.21.1-nanoserver`

```console
$ docker pull nats-streaming@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:

## `nats-streaming:0.21.1-nanoserver-1809`

```console
$ docker pull nats-streaming@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:

## `nats-streaming:0.21.1-scratch`

```console
$ docker pull nats-streaming@sha256:14ace5b780a3e1e3e843bace9214da6c6e6412067aac18835876671d534fe421
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; arm variant v7

### `nats-streaming:0.21.1-scratch` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:ae774aee41bd64306207d739d2290639f673c9c66c367a83f155a923fe8c13f6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5246286 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ce52186dd957f6b70b086fdcbc8212e079e5ed5e3e0013f8f72b3922535a56e`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Sat, 06 Mar 2021 01:00:25 GMT
COPY file:546c18b3e8e91d453d1a325c6e4dbc3c945564c010676da1abe89a653a0dea84 in /nats-streaming-server 
# Sat, 06 Mar 2021 01:00:27 GMT
EXPOSE 4222 8222
# Sat, 06 Mar 2021 01:00:28 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Sat, 06 Mar 2021 01:00:29 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:ed8ed2aa5d978cf51ebe3454de1832aeb40919052c5cb17d5b63865c31fc03c7`  
		Last Modified: Sat, 06 Mar 2021 01:01:07 GMT  
		Size: 5.2 MB (5246286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.21.1-windowsservercore`

```console
$ docker pull nats-streaming@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:

## `nats-streaming:0.21.1-windowsservercore-1809`

```console
$ docker pull nats-streaming@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:

## `nats-streaming:0.21.1-windowsservercore-ltsc2016`

```console
$ docker pull nats-streaming@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:

## `nats-streaming:0.21-alpine`

```console
$ docker pull nats-streaming@sha256:17ee27f3d8f547400a952dcb9ddc3fade80fb324a17fd7e674fdf893cb8a21f4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.21-alpine` - linux; amd64

```console
$ docker pull nats-streaming@sha256:f6662c1e1e718f3d9fcb6bdb60e804f2713ab87d3d79e87867aad686c1bf26f9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.8 MB (8772720 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:040b7462b8eea20a68c23764a3d2155ba5c5c77fee37f82ac9bd0a08fd88004a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 17 Feb 2021 21:19:54 GMT
ADD file:80bf8bd014071345b1c0364eeb0a5e48f3fb0d87f9c31cb990e57caa652b59b8 in / 
# Wed, 17 Feb 2021 21:19:54 GMT
CMD ["/bin/sh"]
# Tue, 02 Mar 2021 00:25:25 GMT
ENV NATS_STREAMING_SERVER=0.21.0
# Tue, 02 Mar 2021 00:25:28 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='ace8ba06da52ca4254236c3385f07a0270bb0155139c71f853a8ca97c816880e' ;; 		armhf) natsArch='arm6'; sha256='769cab28925287d6ce3d67912799273c2ca417684adc09db2529d3e64ffdc10f' ;; 		armv7) natsArch='arm7'; sha256='f4adcefd1f9e1d6d6e9b9fb437b25ef245851b9a26d5cd29def3afff6db4b896' ;; 		x86_64) natsArch='amd64'; sha256='b259633f4f6680b0f6af96b856b648b28970e5d0f2cfc38a439ea07b9bbe2a1d' ;; 		x86) natsArch='386'; sha256='cfb14ae3ab52e66d85e83b2a35f3daee7b9e8fee031a24aeef801f128398e57a' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Tue, 02 Mar 2021 00:25:28 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Tue, 02 Mar 2021 00:25:29 GMT
EXPOSE 4222 8222
# Tue, 02 Mar 2021 00:25:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 02 Mar 2021 00:25:29 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:ba3557a56b150f9b813f9d02274d62914fd8fce120dd374d9ee17b87cf1d277d`  
		Last Modified: Wed, 17 Feb 2021 21:20:25 GMT  
		Size: 2.8 MB (2811657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d1fe86c18b7461fe173b47d88cd5c5dacf60a7445982cc8df67073d31ce5d59`  
		Last Modified: Tue, 02 Mar 2021 00:26:12 GMT  
		Size: 6.0 MB (5960641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b2eda78ff92213f3dfa2cf8f7843e06a7cd05c95b0b51247ca95152fd3ef6c8`  
		Last Modified: Tue, 02 Mar 2021 00:26:11 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.21-alpine` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:7c20fa0d0dbabb6bae2cd97d317f128827a248bc562d6d9c4834c790bf4a7021
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.2 MB (8154253 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5fe07a490b2b30897bbc5fa50238530420e06b6f3e56a1bd8cbe98ac24212b3a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 17 Feb 2021 20:49:32 GMT
ADD file:c04fbd3b039001c592cfa14f8388f8934ed4223ccf274dbb926e75039e172af4 in / 
# Wed, 17 Feb 2021 20:49:33 GMT
CMD ["/bin/sh"]
# Tue, 02 Mar 2021 00:26:32 GMT
ENV NATS_STREAMING_SERVER=0.21.0
# Tue, 02 Mar 2021 00:26:36 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='ace8ba06da52ca4254236c3385f07a0270bb0155139c71f853a8ca97c816880e' ;; 		armhf) natsArch='arm6'; sha256='769cab28925287d6ce3d67912799273c2ca417684adc09db2529d3e64ffdc10f' ;; 		armv7) natsArch='arm7'; sha256='f4adcefd1f9e1d6d6e9b9fb437b25ef245851b9a26d5cd29def3afff6db4b896' ;; 		x86_64) natsArch='amd64'; sha256='b259633f4f6680b0f6af96b856b648b28970e5d0f2cfc38a439ea07b9bbe2a1d' ;; 		x86) natsArch='386'; sha256='cfb14ae3ab52e66d85e83b2a35f3daee7b9e8fee031a24aeef801f128398e57a' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Tue, 02 Mar 2021 00:26:37 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Tue, 02 Mar 2021 00:26:38 GMT
EXPOSE 4222 8222
# Tue, 02 Mar 2021 00:26:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 02 Mar 2021 00:26:39 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:1353527ebe111f9bb1e271264a3c182e909e4b36463f80d7dbde1be0713eb892`  
		Last Modified: Wed, 17 Feb 2021 20:50:06 GMT  
		Size: 2.6 MB (2622039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c13c49183b721e7bfb4ccc166dd54d945cc1db5205af3d2ac4d23532e68688d4`  
		Last Modified: Tue, 02 Mar 2021 00:27:19 GMT  
		Size: 5.5 MB (5531793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9d856ec09a697525b968975b09d200f2f6f7816f402c6883ff0ec86b6e925fa`  
		Last Modified: Tue, 02 Mar 2021 00:27:13 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.21-alpine` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:782e4290f2c50dd5e8a0714f8cfa35d8575577910ff3252c757d3a64e6bd4d47
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.0 MB (7951510 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a88cdb45d1d7d80ee678f8f1ca18f6c67822632552ea1ceb8a6a91ecc72503f4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 17 Feb 2021 20:57:36 GMT
ADD file:efdd39e5243eaf378f12ad5a85d2222b44930850a90263e5f17e8a6b5e9bc9b8 in / 
# Wed, 17 Feb 2021 20:57:37 GMT
CMD ["/bin/sh"]
# Sat, 06 Mar 2021 00:59:37 GMT
ENV NATS_STREAMING_SERVER=0.21.1
# Sat, 06 Mar 2021 00:59:41 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='06d591a61084aab1046e818486c2ee7c3936214c92dc257084693d6ffe06342b' ;; 		armhf) natsArch='arm6'; sha256='085375782abe1bacbd6fc609ce6a6721f029cba312733479204c89bf92f1e188' ;; 		armv7) natsArch='arm7'; sha256='947d91512b47ba98198bef7f799670c40cf6949f2ba2e98b5c133e6166e9b97c' ;; 		x86_64) natsArch='amd64'; sha256='85fd7fd3c7b71cbc9043900f9110b028f1fdc042c6500eed065e6e2c3331f62e' ;; 		x86) natsArch='386'; sha256='475b0f015726af99c9ea779c8bbbeaa729ef90f43dd2715273fea81fb90ea63a' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Sat, 06 Mar 2021 00:59:43 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Sat, 06 Mar 2021 00:59:43 GMT
EXPOSE 4222 8222
# Sat, 06 Mar 2021 00:59:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 06 Mar 2021 00:59:44 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:f55b840e27d3dbe27e44497103a4397f043749f933eb0433d29e2f104b3435ef`  
		Last Modified: Wed, 17 Feb 2021 20:58:14 GMT  
		Size: 2.4 MB (2423892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b550ac0781e9d06a2d5602aa128b8085d9808f31821df0db0fdb3378e4beb64`  
		Last Modified: Sat, 06 Mar 2021 01:00:55 GMT  
		Size: 5.5 MB (5527196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c9fcc13222a0356f1399ed180350034d92d18fa5262cd34421cb52915ca14df`  
		Last Modified: Sat, 06 Mar 2021 01:00:53 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.21-alpine` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:10777a97b0533815b574cb3e18f05a66ac7b41009f455c2ebcb1539d007307f8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.2 MB (8162049 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97d442b80f45600e050156b1173265cf35372b99dffd0fb8bfdad973fd77b339`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 17 Feb 2021 20:39:29 GMT
ADD file:3bf1497bd250cf7c73c12231dc4ebe3a3a67f2cd99e35bce47ef6674683aeb1d in / 
# Wed, 17 Feb 2021 20:39:30 GMT
CMD ["/bin/sh"]
# Tue, 02 Mar 2021 01:13:01 GMT
ENV NATS_STREAMING_SERVER=0.21.0
# Tue, 02 Mar 2021 01:13:05 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='ace8ba06da52ca4254236c3385f07a0270bb0155139c71f853a8ca97c816880e' ;; 		armhf) natsArch='arm6'; sha256='769cab28925287d6ce3d67912799273c2ca417684adc09db2529d3e64ffdc10f' ;; 		armv7) natsArch='arm7'; sha256='f4adcefd1f9e1d6d6e9b9fb437b25ef245851b9a26d5cd29def3afff6db4b896' ;; 		x86_64) natsArch='amd64'; sha256='b259633f4f6680b0f6af96b856b648b28970e5d0f2cfc38a439ea07b9bbe2a1d' ;; 		x86) natsArch='386'; sha256='cfb14ae3ab52e66d85e83b2a35f3daee7b9e8fee031a24aeef801f128398e57a' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Tue, 02 Mar 2021 01:13:06 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Tue, 02 Mar 2021 01:13:06 GMT
EXPOSE 4222 8222
# Tue, 02 Mar 2021 01:13:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 02 Mar 2021 01:13:08 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:069a56d6d07f6b186fbb82e4486616b9be9a37ce32a63013af6cddcb65898182`  
		Last Modified: Wed, 17 Feb 2021 20:40:04 GMT  
		Size: 2.7 MB (2711572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12c50e699e530e5249c2caf763d7dc8d6e6b7cc9c789aa8ed85de12bee5223a2`  
		Last Modified: Tue, 02 Mar 2021 01:15:04 GMT  
		Size: 5.5 MB (5450055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5ae0645459f8848b2db6912d3c7cb864e3ed29d733b3476e1f4416849d3f383`  
		Last Modified: Tue, 02 Mar 2021 01:15:01 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.21-alpine3.13`

```console
$ docker pull nats-streaming@sha256:17ee27f3d8f547400a952dcb9ddc3fade80fb324a17fd7e674fdf893cb8a21f4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.21-alpine3.13` - linux; amd64

```console
$ docker pull nats-streaming@sha256:f6662c1e1e718f3d9fcb6bdb60e804f2713ab87d3d79e87867aad686c1bf26f9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.8 MB (8772720 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:040b7462b8eea20a68c23764a3d2155ba5c5c77fee37f82ac9bd0a08fd88004a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 17 Feb 2021 21:19:54 GMT
ADD file:80bf8bd014071345b1c0364eeb0a5e48f3fb0d87f9c31cb990e57caa652b59b8 in / 
# Wed, 17 Feb 2021 21:19:54 GMT
CMD ["/bin/sh"]
# Tue, 02 Mar 2021 00:25:25 GMT
ENV NATS_STREAMING_SERVER=0.21.0
# Tue, 02 Mar 2021 00:25:28 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='ace8ba06da52ca4254236c3385f07a0270bb0155139c71f853a8ca97c816880e' ;; 		armhf) natsArch='arm6'; sha256='769cab28925287d6ce3d67912799273c2ca417684adc09db2529d3e64ffdc10f' ;; 		armv7) natsArch='arm7'; sha256='f4adcefd1f9e1d6d6e9b9fb437b25ef245851b9a26d5cd29def3afff6db4b896' ;; 		x86_64) natsArch='amd64'; sha256='b259633f4f6680b0f6af96b856b648b28970e5d0f2cfc38a439ea07b9bbe2a1d' ;; 		x86) natsArch='386'; sha256='cfb14ae3ab52e66d85e83b2a35f3daee7b9e8fee031a24aeef801f128398e57a' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Tue, 02 Mar 2021 00:25:28 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Tue, 02 Mar 2021 00:25:29 GMT
EXPOSE 4222 8222
# Tue, 02 Mar 2021 00:25:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 02 Mar 2021 00:25:29 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:ba3557a56b150f9b813f9d02274d62914fd8fce120dd374d9ee17b87cf1d277d`  
		Last Modified: Wed, 17 Feb 2021 21:20:25 GMT  
		Size: 2.8 MB (2811657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d1fe86c18b7461fe173b47d88cd5c5dacf60a7445982cc8df67073d31ce5d59`  
		Last Modified: Tue, 02 Mar 2021 00:26:12 GMT  
		Size: 6.0 MB (5960641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b2eda78ff92213f3dfa2cf8f7843e06a7cd05c95b0b51247ca95152fd3ef6c8`  
		Last Modified: Tue, 02 Mar 2021 00:26:11 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.21-alpine3.13` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:7c20fa0d0dbabb6bae2cd97d317f128827a248bc562d6d9c4834c790bf4a7021
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.2 MB (8154253 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5fe07a490b2b30897bbc5fa50238530420e06b6f3e56a1bd8cbe98ac24212b3a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 17 Feb 2021 20:49:32 GMT
ADD file:c04fbd3b039001c592cfa14f8388f8934ed4223ccf274dbb926e75039e172af4 in / 
# Wed, 17 Feb 2021 20:49:33 GMT
CMD ["/bin/sh"]
# Tue, 02 Mar 2021 00:26:32 GMT
ENV NATS_STREAMING_SERVER=0.21.0
# Tue, 02 Mar 2021 00:26:36 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='ace8ba06da52ca4254236c3385f07a0270bb0155139c71f853a8ca97c816880e' ;; 		armhf) natsArch='arm6'; sha256='769cab28925287d6ce3d67912799273c2ca417684adc09db2529d3e64ffdc10f' ;; 		armv7) natsArch='arm7'; sha256='f4adcefd1f9e1d6d6e9b9fb437b25ef245851b9a26d5cd29def3afff6db4b896' ;; 		x86_64) natsArch='amd64'; sha256='b259633f4f6680b0f6af96b856b648b28970e5d0f2cfc38a439ea07b9bbe2a1d' ;; 		x86) natsArch='386'; sha256='cfb14ae3ab52e66d85e83b2a35f3daee7b9e8fee031a24aeef801f128398e57a' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Tue, 02 Mar 2021 00:26:37 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Tue, 02 Mar 2021 00:26:38 GMT
EXPOSE 4222 8222
# Tue, 02 Mar 2021 00:26:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 02 Mar 2021 00:26:39 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:1353527ebe111f9bb1e271264a3c182e909e4b36463f80d7dbde1be0713eb892`  
		Last Modified: Wed, 17 Feb 2021 20:50:06 GMT  
		Size: 2.6 MB (2622039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c13c49183b721e7bfb4ccc166dd54d945cc1db5205af3d2ac4d23532e68688d4`  
		Last Modified: Tue, 02 Mar 2021 00:27:19 GMT  
		Size: 5.5 MB (5531793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9d856ec09a697525b968975b09d200f2f6f7816f402c6883ff0ec86b6e925fa`  
		Last Modified: Tue, 02 Mar 2021 00:27:13 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.21-alpine3.13` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:782e4290f2c50dd5e8a0714f8cfa35d8575577910ff3252c757d3a64e6bd4d47
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.0 MB (7951510 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a88cdb45d1d7d80ee678f8f1ca18f6c67822632552ea1ceb8a6a91ecc72503f4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 17 Feb 2021 20:57:36 GMT
ADD file:efdd39e5243eaf378f12ad5a85d2222b44930850a90263e5f17e8a6b5e9bc9b8 in / 
# Wed, 17 Feb 2021 20:57:37 GMT
CMD ["/bin/sh"]
# Sat, 06 Mar 2021 00:59:37 GMT
ENV NATS_STREAMING_SERVER=0.21.1
# Sat, 06 Mar 2021 00:59:41 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='06d591a61084aab1046e818486c2ee7c3936214c92dc257084693d6ffe06342b' ;; 		armhf) natsArch='arm6'; sha256='085375782abe1bacbd6fc609ce6a6721f029cba312733479204c89bf92f1e188' ;; 		armv7) natsArch='arm7'; sha256='947d91512b47ba98198bef7f799670c40cf6949f2ba2e98b5c133e6166e9b97c' ;; 		x86_64) natsArch='amd64'; sha256='85fd7fd3c7b71cbc9043900f9110b028f1fdc042c6500eed065e6e2c3331f62e' ;; 		x86) natsArch='386'; sha256='475b0f015726af99c9ea779c8bbbeaa729ef90f43dd2715273fea81fb90ea63a' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Sat, 06 Mar 2021 00:59:43 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Sat, 06 Mar 2021 00:59:43 GMT
EXPOSE 4222 8222
# Sat, 06 Mar 2021 00:59:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 06 Mar 2021 00:59:44 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:f55b840e27d3dbe27e44497103a4397f043749f933eb0433d29e2f104b3435ef`  
		Last Modified: Wed, 17 Feb 2021 20:58:14 GMT  
		Size: 2.4 MB (2423892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b550ac0781e9d06a2d5602aa128b8085d9808f31821df0db0fdb3378e4beb64`  
		Last Modified: Sat, 06 Mar 2021 01:00:55 GMT  
		Size: 5.5 MB (5527196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c9fcc13222a0356f1399ed180350034d92d18fa5262cd34421cb52915ca14df`  
		Last Modified: Sat, 06 Mar 2021 01:00:53 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.21-alpine3.13` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:10777a97b0533815b574cb3e18f05a66ac7b41009f455c2ebcb1539d007307f8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.2 MB (8162049 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97d442b80f45600e050156b1173265cf35372b99dffd0fb8bfdad973fd77b339`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 17 Feb 2021 20:39:29 GMT
ADD file:3bf1497bd250cf7c73c12231dc4ebe3a3a67f2cd99e35bce47ef6674683aeb1d in / 
# Wed, 17 Feb 2021 20:39:30 GMT
CMD ["/bin/sh"]
# Tue, 02 Mar 2021 01:13:01 GMT
ENV NATS_STREAMING_SERVER=0.21.0
# Tue, 02 Mar 2021 01:13:05 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='ace8ba06da52ca4254236c3385f07a0270bb0155139c71f853a8ca97c816880e' ;; 		armhf) natsArch='arm6'; sha256='769cab28925287d6ce3d67912799273c2ca417684adc09db2529d3e64ffdc10f' ;; 		armv7) natsArch='arm7'; sha256='f4adcefd1f9e1d6d6e9b9fb437b25ef245851b9a26d5cd29def3afff6db4b896' ;; 		x86_64) natsArch='amd64'; sha256='b259633f4f6680b0f6af96b856b648b28970e5d0f2cfc38a439ea07b9bbe2a1d' ;; 		x86) natsArch='386'; sha256='cfb14ae3ab52e66d85e83b2a35f3daee7b9e8fee031a24aeef801f128398e57a' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Tue, 02 Mar 2021 01:13:06 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Tue, 02 Mar 2021 01:13:06 GMT
EXPOSE 4222 8222
# Tue, 02 Mar 2021 01:13:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 02 Mar 2021 01:13:08 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:069a56d6d07f6b186fbb82e4486616b9be9a37ce32a63013af6cddcb65898182`  
		Last Modified: Wed, 17 Feb 2021 20:40:04 GMT  
		Size: 2.7 MB (2711572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12c50e699e530e5249c2caf763d7dc8d6e6b7cc9c789aa8ed85de12bee5223a2`  
		Last Modified: Tue, 02 Mar 2021 01:15:04 GMT  
		Size: 5.5 MB (5450055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5ae0645459f8848b2db6912d3c7cb864e3ed29d733b3476e1f4416849d3f383`  
		Last Modified: Tue, 02 Mar 2021 01:15:01 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.21-linux`

```console
$ docker pull nats-streaming@sha256:f7f7b3ef4aa648855b38e0d4096634786a01e382bd63f478733918da6e341d72
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.21-linux` - linux; amd64

```console
$ docker pull nats-streaming@sha256:3783631861947e0e679506679efc64c4875f4804205377e4311e9cdab6c17965
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.7 MB (5679887 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:699c5c09ce0b6a8314d7acec3aa4c72dbaa6a6bc44881fa83719dcf5e2e5a1e1`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 02 Mar 2021 00:25:52 GMT
COPY file:4c2a24d146429270418a17857993903d39b1fcf52d11a560abd159eff99ada8d in /nats-streaming-server 
# Tue, 02 Mar 2021 00:25:52 GMT
EXPOSE 4222 8222
# Tue, 02 Mar 2021 00:25:53 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 02 Mar 2021 00:25:53 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:7fb87f3f85e42eb0fc3d88581c0b84a8d675859dd6727be9100fa9bbaa2cffa4`  
		Last Modified: Tue, 02 Mar 2021 00:26:20 GMT  
		Size: 5.7 MB (5679887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.21-linux` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:48598a6e49d6cdd1e0829bd4d7ead1aff8b18dd07440a20337e701a94caca26e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.3 MB (5250920 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dffd1cc2cc6030e177fe45935f0fee3c62a59fdda8b12c3276d39fa19a6928b1`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 02 Mar 2021 00:26:52 GMT
COPY file:4baaca51b76d42c66f7a4d5146b598f666c38803f36a5286ede362691d89663c in /nats-streaming-server 
# Tue, 02 Mar 2021 00:26:53 GMT
EXPOSE 4222 8222
# Tue, 02 Mar 2021 00:26:53 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 02 Mar 2021 00:26:54 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:92433c508db76d76c2073b4044b8e2a847d00a4148b85326fe4be63f691ef9af`  
		Last Modified: Tue, 02 Mar 2021 00:27:35 GMT  
		Size: 5.3 MB (5250920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.21-linux` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:ae774aee41bd64306207d739d2290639f673c9c66c367a83f155a923fe8c13f6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5246286 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ce52186dd957f6b70b086fdcbc8212e079e5ed5e3e0013f8f72b3922535a56e`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Sat, 06 Mar 2021 01:00:25 GMT
COPY file:546c18b3e8e91d453d1a325c6e4dbc3c945564c010676da1abe89a653a0dea84 in /nats-streaming-server 
# Sat, 06 Mar 2021 01:00:27 GMT
EXPOSE 4222 8222
# Sat, 06 Mar 2021 01:00:28 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Sat, 06 Mar 2021 01:00:29 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:ed8ed2aa5d978cf51ebe3454de1832aeb40919052c5cb17d5b63865c31fc03c7`  
		Last Modified: Sat, 06 Mar 2021 01:01:07 GMT  
		Size: 5.2 MB (5246286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.21-linux` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:bb0f75068ef5a23352dc064f1f3284e6dab1c2586e6a94e2e606778b78cb03f7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5169160 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6cebf86c02f91c34c49641b50fa91c94e4100b2fa18472ca33b362283355e4c1`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 02 Mar 2021 01:14:35 GMT
COPY file:45fcdc5032324b9c78e16535704285519687d0187fa1b424eb18143deb1dece7 in /nats-streaming-server 
# Tue, 02 Mar 2021 01:14:35 GMT
EXPOSE 4222 8222
# Tue, 02 Mar 2021 01:14:36 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 02 Mar 2021 01:14:37 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:8e9b3f150b42f0a6abecb65490e22f7a6a73c1e139f69e747ca01b46f0c4ff5d`  
		Last Modified: Tue, 02 Mar 2021 01:15:22 GMT  
		Size: 5.2 MB (5169160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.21-nanoserver`

```console
$ docker pull nats-streaming@sha256:dda388e643ede382e981561d8783ca34024f18de31dac28bd01ba26525fc06e2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1757; amd64

### `nats-streaming:0.21-nanoserver` - windows version 10.0.17763.1757; amd64

```console
$ docker pull nats-streaming@sha256:7102fdfcfc56aff3af3af39cec63c0601b43592e56b7e64d187790b0822e9a51
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.2 MB (107219449 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a8a29d1082c9d4ea1c812a4e8d84b8d8c1228d2c1c0c1543350e44bd28b31f4f`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 02 Feb 2021 13:06:30 GMT
RUN Apply image 1809-amd64
# Wed, 10 Feb 2021 16:02:26 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Mon, 01 Mar 2021 23:39:47 GMT
RUN cmd /S /C #(nop) COPY file:24ef21e1be266c0481785b3d2cebe511e1bb8a8c20c99795a9e7fa85b0d7aa50 in C:\nats-streaming-server.exe 
# Mon, 01 Mar 2021 23:39:48 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Mon, 01 Mar 2021 23:39:49 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Mon, 01 Mar 2021 23:39:50 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:ba17af31b9276ee11fdf859681b442db50979a39eff4cea2a559a5755cedbe01`  
		Size: 101.4 MB (101406193 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:23b613036f8aee9066e712b3aa58f10f2fde093623511a5658867f53a6d01b18`  
		Last Modified: Wed, 10 Feb 2021 16:06:34 GMT  
		Size: 1.1 KB (1071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:698ae4ae8df313350ab9792ea25a077b988b965eec472e98f4770b8f5b16ed33`  
		Last Modified: Mon, 01 Mar 2021 23:44:05 GMT  
		Size: 5.8 MB (5808961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec3f2e5ff2ba6f6a9881c98155b50d51c881cd77ced1ed2d75b60867bbc96e65`  
		Last Modified: Mon, 01 Mar 2021 23:43:57 GMT  
		Size: 1.1 KB (1064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aa08ef55ec2e1a3c6b2f7f88cf21aa125c7f3356775287b4f3d83372278cb4e`  
		Last Modified: Mon, 01 Mar 2021 23:43:58 GMT  
		Size: 1.0 KB (1033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af33a16b15f810a8bdb3cfe7c2387d435251d11cd9af0a3d5bf3ee30410ccc51`  
		Last Modified: Mon, 01 Mar 2021 23:43:58 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.21-nanoserver-1809`

```console
$ docker pull nats-streaming@sha256:dda388e643ede382e981561d8783ca34024f18de31dac28bd01ba26525fc06e2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1757; amd64

### `nats-streaming:0.21-nanoserver-1809` - windows version 10.0.17763.1757; amd64

```console
$ docker pull nats-streaming@sha256:7102fdfcfc56aff3af3af39cec63c0601b43592e56b7e64d187790b0822e9a51
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.2 MB (107219449 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a8a29d1082c9d4ea1c812a4e8d84b8d8c1228d2c1c0c1543350e44bd28b31f4f`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 02 Feb 2021 13:06:30 GMT
RUN Apply image 1809-amd64
# Wed, 10 Feb 2021 16:02:26 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Mon, 01 Mar 2021 23:39:47 GMT
RUN cmd /S /C #(nop) COPY file:24ef21e1be266c0481785b3d2cebe511e1bb8a8c20c99795a9e7fa85b0d7aa50 in C:\nats-streaming-server.exe 
# Mon, 01 Mar 2021 23:39:48 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Mon, 01 Mar 2021 23:39:49 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Mon, 01 Mar 2021 23:39:50 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:ba17af31b9276ee11fdf859681b442db50979a39eff4cea2a559a5755cedbe01`  
		Size: 101.4 MB (101406193 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:23b613036f8aee9066e712b3aa58f10f2fde093623511a5658867f53a6d01b18`  
		Last Modified: Wed, 10 Feb 2021 16:06:34 GMT  
		Size: 1.1 KB (1071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:698ae4ae8df313350ab9792ea25a077b988b965eec472e98f4770b8f5b16ed33`  
		Last Modified: Mon, 01 Mar 2021 23:44:05 GMT  
		Size: 5.8 MB (5808961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec3f2e5ff2ba6f6a9881c98155b50d51c881cd77ced1ed2d75b60867bbc96e65`  
		Last Modified: Mon, 01 Mar 2021 23:43:57 GMT  
		Size: 1.1 KB (1064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aa08ef55ec2e1a3c6b2f7f88cf21aa125c7f3356775287b4f3d83372278cb4e`  
		Last Modified: Mon, 01 Mar 2021 23:43:58 GMT  
		Size: 1.0 KB (1033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af33a16b15f810a8bdb3cfe7c2387d435251d11cd9af0a3d5bf3ee30410ccc51`  
		Last Modified: Mon, 01 Mar 2021 23:43:58 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.21-scratch`

```console
$ docker pull nats-streaming@sha256:f7f7b3ef4aa648855b38e0d4096634786a01e382bd63f478733918da6e341d72
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.21-scratch` - linux; amd64

```console
$ docker pull nats-streaming@sha256:3783631861947e0e679506679efc64c4875f4804205377e4311e9cdab6c17965
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.7 MB (5679887 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:699c5c09ce0b6a8314d7acec3aa4c72dbaa6a6bc44881fa83719dcf5e2e5a1e1`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 02 Mar 2021 00:25:52 GMT
COPY file:4c2a24d146429270418a17857993903d39b1fcf52d11a560abd159eff99ada8d in /nats-streaming-server 
# Tue, 02 Mar 2021 00:25:52 GMT
EXPOSE 4222 8222
# Tue, 02 Mar 2021 00:25:53 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 02 Mar 2021 00:25:53 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:7fb87f3f85e42eb0fc3d88581c0b84a8d675859dd6727be9100fa9bbaa2cffa4`  
		Last Modified: Tue, 02 Mar 2021 00:26:20 GMT  
		Size: 5.7 MB (5679887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.21-scratch` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:48598a6e49d6cdd1e0829bd4d7ead1aff8b18dd07440a20337e701a94caca26e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.3 MB (5250920 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dffd1cc2cc6030e177fe45935f0fee3c62a59fdda8b12c3276d39fa19a6928b1`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 02 Mar 2021 00:26:52 GMT
COPY file:4baaca51b76d42c66f7a4d5146b598f666c38803f36a5286ede362691d89663c in /nats-streaming-server 
# Tue, 02 Mar 2021 00:26:53 GMT
EXPOSE 4222 8222
# Tue, 02 Mar 2021 00:26:53 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 02 Mar 2021 00:26:54 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:92433c508db76d76c2073b4044b8e2a847d00a4148b85326fe4be63f691ef9af`  
		Last Modified: Tue, 02 Mar 2021 00:27:35 GMT  
		Size: 5.3 MB (5250920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.21-scratch` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:ae774aee41bd64306207d739d2290639f673c9c66c367a83f155a923fe8c13f6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5246286 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ce52186dd957f6b70b086fdcbc8212e079e5ed5e3e0013f8f72b3922535a56e`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Sat, 06 Mar 2021 01:00:25 GMT
COPY file:546c18b3e8e91d453d1a325c6e4dbc3c945564c010676da1abe89a653a0dea84 in /nats-streaming-server 
# Sat, 06 Mar 2021 01:00:27 GMT
EXPOSE 4222 8222
# Sat, 06 Mar 2021 01:00:28 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Sat, 06 Mar 2021 01:00:29 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:ed8ed2aa5d978cf51ebe3454de1832aeb40919052c5cb17d5b63865c31fc03c7`  
		Last Modified: Sat, 06 Mar 2021 01:01:07 GMT  
		Size: 5.2 MB (5246286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.21-scratch` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:bb0f75068ef5a23352dc064f1f3284e6dab1c2586e6a94e2e606778b78cb03f7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5169160 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6cebf86c02f91c34c49641b50fa91c94e4100b2fa18472ca33b362283355e4c1`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 02 Mar 2021 01:14:35 GMT
COPY file:45fcdc5032324b9c78e16535704285519687d0187fa1b424eb18143deb1dece7 in /nats-streaming-server 
# Tue, 02 Mar 2021 01:14:35 GMT
EXPOSE 4222 8222
# Tue, 02 Mar 2021 01:14:36 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 02 Mar 2021 01:14:37 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:8e9b3f150b42f0a6abecb65490e22f7a6a73c1e139f69e747ca01b46f0c4ff5d`  
		Last Modified: Tue, 02 Mar 2021 01:15:22 GMT  
		Size: 5.2 MB (5169160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.21-windowsservercore`

```console
$ docker pull nats-streaming@sha256:0728f2a6f38b6ddc9220b714320ea805334d12ff55fe3085f54fd4c3990ffa48
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1757; amd64
	-	windows version 10.0.14393.4225; amd64

### `nats-streaming:0.21-windowsservercore` - windows version 10.0.17763.1757; amd64

```console
$ docker pull nats-streaming@sha256:f37e01c95a35e80a9ded4c68744089da72385d2b912ea64785af120e5dfac46e
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2459529339 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b413bdbbbc445bd56eec6684f454ad90530794c0c418fe4d91945d27158fd2ca`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 06 Feb 2021 05:03:14 GMT
RUN Install update 1809-amd64
# Tue, 09 Feb 2021 20:26:38 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Feb 2021 16:00:30 GMT
ENV NATS_DOCKERIZED=1
# Mon, 01 Mar 2021 23:37:33 GMT
ENV NATS_STREAMING_SERVER=0.21.0
# Mon, 01 Mar 2021 23:37:34 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.21.0/nats-streaming-server-v0.21.0-windows-amd64.zip
# Mon, 01 Mar 2021 23:37:35 GMT
ENV GIT_DOWNLOAD_SHA256=00bd52804208a52014f518836198a3ebcd513fc5029eda9de2b4ef846f5cb828
# Mon, 01 Mar 2021 23:38:06 GMT
RUN Set-PSDebug -Trace 2
# Mon, 01 Mar 2021 23:39:26 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Mon, 01 Mar 2021 23:39:27 GMT
EXPOSE 4222 8222
# Mon, 01 Mar 2021 23:39:29 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Mon, 01 Mar 2021 23:39:30 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:db4edcf0861ff3fdc41851a5a218965ecb2ab6cf4ec9448fb80cc4b6792fd46c`  
		Size: 720.9 MB (720933935 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:751b8860e89a7e6999d74a11dc393620b118057ad881cb87f1d6e3653cb2db43`  
		Last Modified: Tue, 09 Feb 2021 20:48:09 GMT  
		Size: 1.3 KB (1337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7f01e717591f83c73890556e7a4c77e53caed8daf6c9b0150f497e094a4a698`  
		Last Modified: Wed, 10 Feb 2021 16:06:05 GMT  
		Size: 1.4 KB (1361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cee7e8f68acf02f1803fbe58fd1c98e5136b5c448a9ac12d39f5a4a64ce198a8`  
		Last Modified: Mon, 01 Mar 2021 23:43:41 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16c75a51835c930004670181ad34afd7c2e90ba762a6696cfc732939750e5023`  
		Last Modified: Mon, 01 Mar 2021 23:43:42 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00d34a3454dc6e83cea274b8fd2765fef221836a6993fbe56ceac434981fb5b0`  
		Last Modified: Mon, 01 Mar 2021 23:43:41 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0dcdeb9a6756964b7928054f4f2182d16a35b34ea18396a0d4b38cf484fd9f1`  
		Last Modified: Mon, 01 Mar 2021 23:43:37 GMT  
		Size: 5.1 MB (5051217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a34eb42fac48c971f1a0135c6584d1083bb0e536911e46b1a1e389c4ffe729a8`  
		Last Modified: Mon, 01 Mar 2021 23:43:41 GMT  
		Size: 15.2 MB (15200127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f665eadac63d2ed583f4d30a7d28791f710880674a828e61d8c2105ce70655d3`  
		Last Modified: Mon, 01 Mar 2021 23:43:36 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13fe9508026c89dd38a20a05c48fc44dcb7d86441cdcb88457d74e6625ee04cc`  
		Last Modified: Mon, 01 Mar 2021 23:43:36 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:024aa4f6d5eeceaecd71aa08ba9e78ea00fd32ea15890f9d228db2fc18580407`  
		Last Modified: Mon, 01 Mar 2021 23:43:35 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.21-windowsservercore` - windows version 10.0.14393.4225; amd64

```console
$ docker pull nats-streaming@sha256:eb47ac16c5b855632476a7b18bf7e414b1bd8f550cc6076715b87e5f0b3a531b
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5816649326 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:76ab14b94a5ce8d1e02ac5175112977ea6d3a9ab5a4b1d4f23979ef50fe19563`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 27 Jan 2021 18:11:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 09 Feb 2021 20:28:50 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Feb 2021 16:02:35 GMT
ENV NATS_DOCKERIZED=1
# Mon, 01 Mar 2021 23:39:57 GMT
ENV NATS_STREAMING_SERVER=0.21.0
# Mon, 01 Mar 2021 23:39:58 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.21.0/nats-streaming-server-v0.21.0-windows-amd64.zip
# Mon, 01 Mar 2021 23:39:59 GMT
ENV GIT_DOWNLOAD_SHA256=00bd52804208a52014f518836198a3ebcd513fc5029eda9de2b4ef846f5cb828
# Mon, 01 Mar 2021 23:41:08 GMT
RUN Set-PSDebug -Trace 2
# Mon, 01 Mar 2021 23:42:59 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Mon, 01 Mar 2021 23:43:00 GMT
EXPOSE 4222 8222
# Mon, 01 Mar 2021 23:43:01 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Mon, 01 Mar 2021 23:43:02 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:62c48323ed8ac695b8cbe0ecedcc28ba185a234673ad9241df2b151dd00f9181`  
		Size: 1.7 GB (1725027107 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ac4a230905430e1aea27172a9432f576cc4a530e72bea516a2b304d2b7e9c101`  
		Last Modified: Tue, 09 Feb 2021 20:49:11 GMT  
		Size: 1.4 KB (1356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cc28e30e89dab2d0b2b2f6c3114771d9d803d5942c730de78d2dd457ad4ac40`  
		Last Modified: Wed, 10 Feb 2021 16:06:59 GMT  
		Size: 1.4 KB (1361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e865ae49ff7ab275634dd5c255d968f5f0f59d027134ad6df4133fa52d0d0af`  
		Last Modified: Mon, 01 Mar 2021 23:44:20 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:512f73566aa9bcff8499433bf39ef4bf7fbf46bcaf045cdfe4cdc3b374fd4ac3`  
		Last Modified: Mon, 01 Mar 2021 23:44:20 GMT  
		Size: 1.3 KB (1306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:322aaa185ec2b5e90cc9eb8c57ee82a54b439aafd42bb20b59e2736d28cdc8e1`  
		Last Modified: Mon, 01 Mar 2021 23:44:20 GMT  
		Size: 1.3 KB (1302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2f75278df3ba6220910463178e2fd69782bbc0c3abbbfa41ddd271358106f32`  
		Last Modified: Mon, 01 Mar 2021 23:44:21 GMT  
		Size: 5.7 MB (5657685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b36a484255a580d8cbe179712aec8211899c8500471dcd9802790090750911c0`  
		Last Modified: Mon, 01 Mar 2021 23:44:36 GMT  
		Size: 16.0 MB (15967963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d1eabaebec46e6111a59bec9221d1e0d4973de580e30a453fa7bbb2e1ad9385`  
		Last Modified: Mon, 01 Mar 2021 23:44:17 GMT  
		Size: 1.3 KB (1300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fef8d63616ebeb7cc5aa29815610700aeccd828419c232dd4b8ba2edc47f8a7`  
		Last Modified: Mon, 01 Mar 2021 23:44:17 GMT  
		Size: 1.3 KB (1334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32683573142d691c7c5ca7fbebf8c2d37bd0ab61abafdf7be2690d440dcad8c0`  
		Last Modified: Mon, 01 Mar 2021 23:44:17 GMT  
		Size: 1.3 KB (1321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.21-windowsservercore-1809`

```console
$ docker pull nats-streaming@sha256:66f478d3ebc42ecbb2578543c96ac3870f81725bef104339e705e1ab95d5ba9c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1757; amd64

### `nats-streaming:0.21-windowsservercore-1809` - windows version 10.0.17763.1757; amd64

```console
$ docker pull nats-streaming@sha256:f37e01c95a35e80a9ded4c68744089da72385d2b912ea64785af120e5dfac46e
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2459529339 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b413bdbbbc445bd56eec6684f454ad90530794c0c418fe4d91945d27158fd2ca`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 06 Feb 2021 05:03:14 GMT
RUN Install update 1809-amd64
# Tue, 09 Feb 2021 20:26:38 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Feb 2021 16:00:30 GMT
ENV NATS_DOCKERIZED=1
# Mon, 01 Mar 2021 23:37:33 GMT
ENV NATS_STREAMING_SERVER=0.21.0
# Mon, 01 Mar 2021 23:37:34 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.21.0/nats-streaming-server-v0.21.0-windows-amd64.zip
# Mon, 01 Mar 2021 23:37:35 GMT
ENV GIT_DOWNLOAD_SHA256=00bd52804208a52014f518836198a3ebcd513fc5029eda9de2b4ef846f5cb828
# Mon, 01 Mar 2021 23:38:06 GMT
RUN Set-PSDebug -Trace 2
# Mon, 01 Mar 2021 23:39:26 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Mon, 01 Mar 2021 23:39:27 GMT
EXPOSE 4222 8222
# Mon, 01 Mar 2021 23:39:29 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Mon, 01 Mar 2021 23:39:30 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:db4edcf0861ff3fdc41851a5a218965ecb2ab6cf4ec9448fb80cc4b6792fd46c`  
		Size: 720.9 MB (720933935 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:751b8860e89a7e6999d74a11dc393620b118057ad881cb87f1d6e3653cb2db43`  
		Last Modified: Tue, 09 Feb 2021 20:48:09 GMT  
		Size: 1.3 KB (1337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7f01e717591f83c73890556e7a4c77e53caed8daf6c9b0150f497e094a4a698`  
		Last Modified: Wed, 10 Feb 2021 16:06:05 GMT  
		Size: 1.4 KB (1361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cee7e8f68acf02f1803fbe58fd1c98e5136b5c448a9ac12d39f5a4a64ce198a8`  
		Last Modified: Mon, 01 Mar 2021 23:43:41 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16c75a51835c930004670181ad34afd7c2e90ba762a6696cfc732939750e5023`  
		Last Modified: Mon, 01 Mar 2021 23:43:42 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00d34a3454dc6e83cea274b8fd2765fef221836a6993fbe56ceac434981fb5b0`  
		Last Modified: Mon, 01 Mar 2021 23:43:41 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0dcdeb9a6756964b7928054f4f2182d16a35b34ea18396a0d4b38cf484fd9f1`  
		Last Modified: Mon, 01 Mar 2021 23:43:37 GMT  
		Size: 5.1 MB (5051217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a34eb42fac48c971f1a0135c6584d1083bb0e536911e46b1a1e389c4ffe729a8`  
		Last Modified: Mon, 01 Mar 2021 23:43:41 GMT  
		Size: 15.2 MB (15200127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f665eadac63d2ed583f4d30a7d28791f710880674a828e61d8c2105ce70655d3`  
		Last Modified: Mon, 01 Mar 2021 23:43:36 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13fe9508026c89dd38a20a05c48fc44dcb7d86441cdcb88457d74e6625ee04cc`  
		Last Modified: Mon, 01 Mar 2021 23:43:36 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:024aa4f6d5eeceaecd71aa08ba9e78ea00fd32ea15890f9d228db2fc18580407`  
		Last Modified: Mon, 01 Mar 2021 23:43:35 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.21-windowsservercore-ltsc2016`

```console
$ docker pull nats-streaming@sha256:915d9002166880b04fb879b327a5382eb1d1962f95238efaa47b85bf58410a31
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4225; amd64

### `nats-streaming:0.21-windowsservercore-ltsc2016` - windows version 10.0.14393.4225; amd64

```console
$ docker pull nats-streaming@sha256:eb47ac16c5b855632476a7b18bf7e414b1bd8f550cc6076715b87e5f0b3a531b
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5816649326 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:76ab14b94a5ce8d1e02ac5175112977ea6d3a9ab5a4b1d4f23979ef50fe19563`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 27 Jan 2021 18:11:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 09 Feb 2021 20:28:50 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Feb 2021 16:02:35 GMT
ENV NATS_DOCKERIZED=1
# Mon, 01 Mar 2021 23:39:57 GMT
ENV NATS_STREAMING_SERVER=0.21.0
# Mon, 01 Mar 2021 23:39:58 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.21.0/nats-streaming-server-v0.21.0-windows-amd64.zip
# Mon, 01 Mar 2021 23:39:59 GMT
ENV GIT_DOWNLOAD_SHA256=00bd52804208a52014f518836198a3ebcd513fc5029eda9de2b4ef846f5cb828
# Mon, 01 Mar 2021 23:41:08 GMT
RUN Set-PSDebug -Trace 2
# Mon, 01 Mar 2021 23:42:59 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Mon, 01 Mar 2021 23:43:00 GMT
EXPOSE 4222 8222
# Mon, 01 Mar 2021 23:43:01 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Mon, 01 Mar 2021 23:43:02 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:62c48323ed8ac695b8cbe0ecedcc28ba185a234673ad9241df2b151dd00f9181`  
		Size: 1.7 GB (1725027107 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ac4a230905430e1aea27172a9432f576cc4a530e72bea516a2b304d2b7e9c101`  
		Last Modified: Tue, 09 Feb 2021 20:49:11 GMT  
		Size: 1.4 KB (1356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cc28e30e89dab2d0b2b2f6c3114771d9d803d5942c730de78d2dd457ad4ac40`  
		Last Modified: Wed, 10 Feb 2021 16:06:59 GMT  
		Size: 1.4 KB (1361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e865ae49ff7ab275634dd5c255d968f5f0f59d027134ad6df4133fa52d0d0af`  
		Last Modified: Mon, 01 Mar 2021 23:44:20 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:512f73566aa9bcff8499433bf39ef4bf7fbf46bcaf045cdfe4cdc3b374fd4ac3`  
		Last Modified: Mon, 01 Mar 2021 23:44:20 GMT  
		Size: 1.3 KB (1306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:322aaa185ec2b5e90cc9eb8c57ee82a54b439aafd42bb20b59e2736d28cdc8e1`  
		Last Modified: Mon, 01 Mar 2021 23:44:20 GMT  
		Size: 1.3 KB (1302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2f75278df3ba6220910463178e2fd69782bbc0c3abbbfa41ddd271358106f32`  
		Last Modified: Mon, 01 Mar 2021 23:44:21 GMT  
		Size: 5.7 MB (5657685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b36a484255a580d8cbe179712aec8211899c8500471dcd9802790090750911c0`  
		Last Modified: Mon, 01 Mar 2021 23:44:36 GMT  
		Size: 16.0 MB (15967963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d1eabaebec46e6111a59bec9221d1e0d4973de580e30a453fa7bbb2e1ad9385`  
		Last Modified: Mon, 01 Mar 2021 23:44:17 GMT  
		Size: 1.3 KB (1300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fef8d63616ebeb7cc5aa29815610700aeccd828419c232dd4b8ba2edc47f8a7`  
		Last Modified: Mon, 01 Mar 2021 23:44:17 GMT  
		Size: 1.3 KB (1334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32683573142d691c7c5ca7fbebf8c2d37bd0ab61abafdf7be2690d440dcad8c0`  
		Last Modified: Mon, 01 Mar 2021 23:44:17 GMT  
		Size: 1.3 KB (1321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:alpine`

```console
$ docker pull nats-streaming@sha256:17ee27f3d8f547400a952dcb9ddc3fade80fb324a17fd7e674fdf893cb8a21f4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:alpine` - linux; amd64

```console
$ docker pull nats-streaming@sha256:f6662c1e1e718f3d9fcb6bdb60e804f2713ab87d3d79e87867aad686c1bf26f9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.8 MB (8772720 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:040b7462b8eea20a68c23764a3d2155ba5c5c77fee37f82ac9bd0a08fd88004a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 17 Feb 2021 21:19:54 GMT
ADD file:80bf8bd014071345b1c0364eeb0a5e48f3fb0d87f9c31cb990e57caa652b59b8 in / 
# Wed, 17 Feb 2021 21:19:54 GMT
CMD ["/bin/sh"]
# Tue, 02 Mar 2021 00:25:25 GMT
ENV NATS_STREAMING_SERVER=0.21.0
# Tue, 02 Mar 2021 00:25:28 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='ace8ba06da52ca4254236c3385f07a0270bb0155139c71f853a8ca97c816880e' ;; 		armhf) natsArch='arm6'; sha256='769cab28925287d6ce3d67912799273c2ca417684adc09db2529d3e64ffdc10f' ;; 		armv7) natsArch='arm7'; sha256='f4adcefd1f9e1d6d6e9b9fb437b25ef245851b9a26d5cd29def3afff6db4b896' ;; 		x86_64) natsArch='amd64'; sha256='b259633f4f6680b0f6af96b856b648b28970e5d0f2cfc38a439ea07b9bbe2a1d' ;; 		x86) natsArch='386'; sha256='cfb14ae3ab52e66d85e83b2a35f3daee7b9e8fee031a24aeef801f128398e57a' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Tue, 02 Mar 2021 00:25:28 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Tue, 02 Mar 2021 00:25:29 GMT
EXPOSE 4222 8222
# Tue, 02 Mar 2021 00:25:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 02 Mar 2021 00:25:29 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:ba3557a56b150f9b813f9d02274d62914fd8fce120dd374d9ee17b87cf1d277d`  
		Last Modified: Wed, 17 Feb 2021 21:20:25 GMT  
		Size: 2.8 MB (2811657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d1fe86c18b7461fe173b47d88cd5c5dacf60a7445982cc8df67073d31ce5d59`  
		Last Modified: Tue, 02 Mar 2021 00:26:12 GMT  
		Size: 6.0 MB (5960641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b2eda78ff92213f3dfa2cf8f7843e06a7cd05c95b0b51247ca95152fd3ef6c8`  
		Last Modified: Tue, 02 Mar 2021 00:26:11 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:7c20fa0d0dbabb6bae2cd97d317f128827a248bc562d6d9c4834c790bf4a7021
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.2 MB (8154253 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5fe07a490b2b30897bbc5fa50238530420e06b6f3e56a1bd8cbe98ac24212b3a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 17 Feb 2021 20:49:32 GMT
ADD file:c04fbd3b039001c592cfa14f8388f8934ed4223ccf274dbb926e75039e172af4 in / 
# Wed, 17 Feb 2021 20:49:33 GMT
CMD ["/bin/sh"]
# Tue, 02 Mar 2021 00:26:32 GMT
ENV NATS_STREAMING_SERVER=0.21.0
# Tue, 02 Mar 2021 00:26:36 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='ace8ba06da52ca4254236c3385f07a0270bb0155139c71f853a8ca97c816880e' ;; 		armhf) natsArch='arm6'; sha256='769cab28925287d6ce3d67912799273c2ca417684adc09db2529d3e64ffdc10f' ;; 		armv7) natsArch='arm7'; sha256='f4adcefd1f9e1d6d6e9b9fb437b25ef245851b9a26d5cd29def3afff6db4b896' ;; 		x86_64) natsArch='amd64'; sha256='b259633f4f6680b0f6af96b856b648b28970e5d0f2cfc38a439ea07b9bbe2a1d' ;; 		x86) natsArch='386'; sha256='cfb14ae3ab52e66d85e83b2a35f3daee7b9e8fee031a24aeef801f128398e57a' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Tue, 02 Mar 2021 00:26:37 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Tue, 02 Mar 2021 00:26:38 GMT
EXPOSE 4222 8222
# Tue, 02 Mar 2021 00:26:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 02 Mar 2021 00:26:39 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:1353527ebe111f9bb1e271264a3c182e909e4b36463f80d7dbde1be0713eb892`  
		Last Modified: Wed, 17 Feb 2021 20:50:06 GMT  
		Size: 2.6 MB (2622039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c13c49183b721e7bfb4ccc166dd54d945cc1db5205af3d2ac4d23532e68688d4`  
		Last Modified: Tue, 02 Mar 2021 00:27:19 GMT  
		Size: 5.5 MB (5531793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9d856ec09a697525b968975b09d200f2f6f7816f402c6883ff0ec86b6e925fa`  
		Last Modified: Tue, 02 Mar 2021 00:27:13 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:782e4290f2c50dd5e8a0714f8cfa35d8575577910ff3252c757d3a64e6bd4d47
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.0 MB (7951510 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a88cdb45d1d7d80ee678f8f1ca18f6c67822632552ea1ceb8a6a91ecc72503f4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 17 Feb 2021 20:57:36 GMT
ADD file:efdd39e5243eaf378f12ad5a85d2222b44930850a90263e5f17e8a6b5e9bc9b8 in / 
# Wed, 17 Feb 2021 20:57:37 GMT
CMD ["/bin/sh"]
# Sat, 06 Mar 2021 00:59:37 GMT
ENV NATS_STREAMING_SERVER=0.21.1
# Sat, 06 Mar 2021 00:59:41 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='06d591a61084aab1046e818486c2ee7c3936214c92dc257084693d6ffe06342b' ;; 		armhf) natsArch='arm6'; sha256='085375782abe1bacbd6fc609ce6a6721f029cba312733479204c89bf92f1e188' ;; 		armv7) natsArch='arm7'; sha256='947d91512b47ba98198bef7f799670c40cf6949f2ba2e98b5c133e6166e9b97c' ;; 		x86_64) natsArch='amd64'; sha256='85fd7fd3c7b71cbc9043900f9110b028f1fdc042c6500eed065e6e2c3331f62e' ;; 		x86) natsArch='386'; sha256='475b0f015726af99c9ea779c8bbbeaa729ef90f43dd2715273fea81fb90ea63a' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Sat, 06 Mar 2021 00:59:43 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Sat, 06 Mar 2021 00:59:43 GMT
EXPOSE 4222 8222
# Sat, 06 Mar 2021 00:59:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 06 Mar 2021 00:59:44 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:f55b840e27d3dbe27e44497103a4397f043749f933eb0433d29e2f104b3435ef`  
		Last Modified: Wed, 17 Feb 2021 20:58:14 GMT  
		Size: 2.4 MB (2423892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b550ac0781e9d06a2d5602aa128b8085d9808f31821df0db0fdb3378e4beb64`  
		Last Modified: Sat, 06 Mar 2021 01:00:55 GMT  
		Size: 5.5 MB (5527196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c9fcc13222a0356f1399ed180350034d92d18fa5262cd34421cb52915ca14df`  
		Last Modified: Sat, 06 Mar 2021 01:00:53 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:10777a97b0533815b574cb3e18f05a66ac7b41009f455c2ebcb1539d007307f8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.2 MB (8162049 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97d442b80f45600e050156b1173265cf35372b99dffd0fb8bfdad973fd77b339`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 17 Feb 2021 20:39:29 GMT
ADD file:3bf1497bd250cf7c73c12231dc4ebe3a3a67f2cd99e35bce47ef6674683aeb1d in / 
# Wed, 17 Feb 2021 20:39:30 GMT
CMD ["/bin/sh"]
# Tue, 02 Mar 2021 01:13:01 GMT
ENV NATS_STREAMING_SERVER=0.21.0
# Tue, 02 Mar 2021 01:13:05 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='ace8ba06da52ca4254236c3385f07a0270bb0155139c71f853a8ca97c816880e' ;; 		armhf) natsArch='arm6'; sha256='769cab28925287d6ce3d67912799273c2ca417684adc09db2529d3e64ffdc10f' ;; 		armv7) natsArch='arm7'; sha256='f4adcefd1f9e1d6d6e9b9fb437b25ef245851b9a26d5cd29def3afff6db4b896' ;; 		x86_64) natsArch='amd64'; sha256='b259633f4f6680b0f6af96b856b648b28970e5d0f2cfc38a439ea07b9bbe2a1d' ;; 		x86) natsArch='386'; sha256='cfb14ae3ab52e66d85e83b2a35f3daee7b9e8fee031a24aeef801f128398e57a' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Tue, 02 Mar 2021 01:13:06 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Tue, 02 Mar 2021 01:13:06 GMT
EXPOSE 4222 8222
# Tue, 02 Mar 2021 01:13:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 02 Mar 2021 01:13:08 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:069a56d6d07f6b186fbb82e4486616b9be9a37ce32a63013af6cddcb65898182`  
		Last Modified: Wed, 17 Feb 2021 20:40:04 GMT  
		Size: 2.7 MB (2711572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12c50e699e530e5249c2caf763d7dc8d6e6b7cc9c789aa8ed85de12bee5223a2`  
		Last Modified: Tue, 02 Mar 2021 01:15:04 GMT  
		Size: 5.5 MB (5450055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5ae0645459f8848b2db6912d3c7cb864e3ed29d733b3476e1f4416849d3f383`  
		Last Modified: Tue, 02 Mar 2021 01:15:01 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:alpine3.13`

```console
$ docker pull nats-streaming@sha256:17ee27f3d8f547400a952dcb9ddc3fade80fb324a17fd7e674fdf893cb8a21f4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:alpine3.13` - linux; amd64

```console
$ docker pull nats-streaming@sha256:f6662c1e1e718f3d9fcb6bdb60e804f2713ab87d3d79e87867aad686c1bf26f9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.8 MB (8772720 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:040b7462b8eea20a68c23764a3d2155ba5c5c77fee37f82ac9bd0a08fd88004a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 17 Feb 2021 21:19:54 GMT
ADD file:80bf8bd014071345b1c0364eeb0a5e48f3fb0d87f9c31cb990e57caa652b59b8 in / 
# Wed, 17 Feb 2021 21:19:54 GMT
CMD ["/bin/sh"]
# Tue, 02 Mar 2021 00:25:25 GMT
ENV NATS_STREAMING_SERVER=0.21.0
# Tue, 02 Mar 2021 00:25:28 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='ace8ba06da52ca4254236c3385f07a0270bb0155139c71f853a8ca97c816880e' ;; 		armhf) natsArch='arm6'; sha256='769cab28925287d6ce3d67912799273c2ca417684adc09db2529d3e64ffdc10f' ;; 		armv7) natsArch='arm7'; sha256='f4adcefd1f9e1d6d6e9b9fb437b25ef245851b9a26d5cd29def3afff6db4b896' ;; 		x86_64) natsArch='amd64'; sha256='b259633f4f6680b0f6af96b856b648b28970e5d0f2cfc38a439ea07b9bbe2a1d' ;; 		x86) natsArch='386'; sha256='cfb14ae3ab52e66d85e83b2a35f3daee7b9e8fee031a24aeef801f128398e57a' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Tue, 02 Mar 2021 00:25:28 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Tue, 02 Mar 2021 00:25:29 GMT
EXPOSE 4222 8222
# Tue, 02 Mar 2021 00:25:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 02 Mar 2021 00:25:29 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:ba3557a56b150f9b813f9d02274d62914fd8fce120dd374d9ee17b87cf1d277d`  
		Last Modified: Wed, 17 Feb 2021 21:20:25 GMT  
		Size: 2.8 MB (2811657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d1fe86c18b7461fe173b47d88cd5c5dacf60a7445982cc8df67073d31ce5d59`  
		Last Modified: Tue, 02 Mar 2021 00:26:12 GMT  
		Size: 6.0 MB (5960641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b2eda78ff92213f3dfa2cf8f7843e06a7cd05c95b0b51247ca95152fd3ef6c8`  
		Last Modified: Tue, 02 Mar 2021 00:26:11 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine3.13` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:7c20fa0d0dbabb6bae2cd97d317f128827a248bc562d6d9c4834c790bf4a7021
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.2 MB (8154253 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5fe07a490b2b30897bbc5fa50238530420e06b6f3e56a1bd8cbe98ac24212b3a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 17 Feb 2021 20:49:32 GMT
ADD file:c04fbd3b039001c592cfa14f8388f8934ed4223ccf274dbb926e75039e172af4 in / 
# Wed, 17 Feb 2021 20:49:33 GMT
CMD ["/bin/sh"]
# Tue, 02 Mar 2021 00:26:32 GMT
ENV NATS_STREAMING_SERVER=0.21.0
# Tue, 02 Mar 2021 00:26:36 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='ace8ba06da52ca4254236c3385f07a0270bb0155139c71f853a8ca97c816880e' ;; 		armhf) natsArch='arm6'; sha256='769cab28925287d6ce3d67912799273c2ca417684adc09db2529d3e64ffdc10f' ;; 		armv7) natsArch='arm7'; sha256='f4adcefd1f9e1d6d6e9b9fb437b25ef245851b9a26d5cd29def3afff6db4b896' ;; 		x86_64) natsArch='amd64'; sha256='b259633f4f6680b0f6af96b856b648b28970e5d0f2cfc38a439ea07b9bbe2a1d' ;; 		x86) natsArch='386'; sha256='cfb14ae3ab52e66d85e83b2a35f3daee7b9e8fee031a24aeef801f128398e57a' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Tue, 02 Mar 2021 00:26:37 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Tue, 02 Mar 2021 00:26:38 GMT
EXPOSE 4222 8222
# Tue, 02 Mar 2021 00:26:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 02 Mar 2021 00:26:39 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:1353527ebe111f9bb1e271264a3c182e909e4b36463f80d7dbde1be0713eb892`  
		Last Modified: Wed, 17 Feb 2021 20:50:06 GMT  
		Size: 2.6 MB (2622039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c13c49183b721e7bfb4ccc166dd54d945cc1db5205af3d2ac4d23532e68688d4`  
		Last Modified: Tue, 02 Mar 2021 00:27:19 GMT  
		Size: 5.5 MB (5531793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9d856ec09a697525b968975b09d200f2f6f7816f402c6883ff0ec86b6e925fa`  
		Last Modified: Tue, 02 Mar 2021 00:27:13 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine3.13` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:782e4290f2c50dd5e8a0714f8cfa35d8575577910ff3252c757d3a64e6bd4d47
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.0 MB (7951510 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a88cdb45d1d7d80ee678f8f1ca18f6c67822632552ea1ceb8a6a91ecc72503f4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 17 Feb 2021 20:57:36 GMT
ADD file:efdd39e5243eaf378f12ad5a85d2222b44930850a90263e5f17e8a6b5e9bc9b8 in / 
# Wed, 17 Feb 2021 20:57:37 GMT
CMD ["/bin/sh"]
# Sat, 06 Mar 2021 00:59:37 GMT
ENV NATS_STREAMING_SERVER=0.21.1
# Sat, 06 Mar 2021 00:59:41 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='06d591a61084aab1046e818486c2ee7c3936214c92dc257084693d6ffe06342b' ;; 		armhf) natsArch='arm6'; sha256='085375782abe1bacbd6fc609ce6a6721f029cba312733479204c89bf92f1e188' ;; 		armv7) natsArch='arm7'; sha256='947d91512b47ba98198bef7f799670c40cf6949f2ba2e98b5c133e6166e9b97c' ;; 		x86_64) natsArch='amd64'; sha256='85fd7fd3c7b71cbc9043900f9110b028f1fdc042c6500eed065e6e2c3331f62e' ;; 		x86) natsArch='386'; sha256='475b0f015726af99c9ea779c8bbbeaa729ef90f43dd2715273fea81fb90ea63a' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Sat, 06 Mar 2021 00:59:43 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Sat, 06 Mar 2021 00:59:43 GMT
EXPOSE 4222 8222
# Sat, 06 Mar 2021 00:59:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 06 Mar 2021 00:59:44 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:f55b840e27d3dbe27e44497103a4397f043749f933eb0433d29e2f104b3435ef`  
		Last Modified: Wed, 17 Feb 2021 20:58:14 GMT  
		Size: 2.4 MB (2423892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b550ac0781e9d06a2d5602aa128b8085d9808f31821df0db0fdb3378e4beb64`  
		Last Modified: Sat, 06 Mar 2021 01:00:55 GMT  
		Size: 5.5 MB (5527196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c9fcc13222a0356f1399ed180350034d92d18fa5262cd34421cb52915ca14df`  
		Last Modified: Sat, 06 Mar 2021 01:00:53 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine3.13` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:10777a97b0533815b574cb3e18f05a66ac7b41009f455c2ebcb1539d007307f8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.2 MB (8162049 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97d442b80f45600e050156b1173265cf35372b99dffd0fb8bfdad973fd77b339`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 17 Feb 2021 20:39:29 GMT
ADD file:3bf1497bd250cf7c73c12231dc4ebe3a3a67f2cd99e35bce47ef6674683aeb1d in / 
# Wed, 17 Feb 2021 20:39:30 GMT
CMD ["/bin/sh"]
# Tue, 02 Mar 2021 01:13:01 GMT
ENV NATS_STREAMING_SERVER=0.21.0
# Tue, 02 Mar 2021 01:13:05 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='ace8ba06da52ca4254236c3385f07a0270bb0155139c71f853a8ca97c816880e' ;; 		armhf) natsArch='arm6'; sha256='769cab28925287d6ce3d67912799273c2ca417684adc09db2529d3e64ffdc10f' ;; 		armv7) natsArch='arm7'; sha256='f4adcefd1f9e1d6d6e9b9fb437b25ef245851b9a26d5cd29def3afff6db4b896' ;; 		x86_64) natsArch='amd64'; sha256='b259633f4f6680b0f6af96b856b648b28970e5d0f2cfc38a439ea07b9bbe2a1d' ;; 		x86) natsArch='386'; sha256='cfb14ae3ab52e66d85e83b2a35f3daee7b9e8fee031a24aeef801f128398e57a' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Tue, 02 Mar 2021 01:13:06 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Tue, 02 Mar 2021 01:13:06 GMT
EXPOSE 4222 8222
# Tue, 02 Mar 2021 01:13:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 02 Mar 2021 01:13:08 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:069a56d6d07f6b186fbb82e4486616b9be9a37ce32a63013af6cddcb65898182`  
		Last Modified: Wed, 17 Feb 2021 20:40:04 GMT  
		Size: 2.7 MB (2711572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12c50e699e530e5249c2caf763d7dc8d6e6b7cc9c789aa8ed85de12bee5223a2`  
		Last Modified: Tue, 02 Mar 2021 01:15:04 GMT  
		Size: 5.5 MB (5450055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5ae0645459f8848b2db6912d3c7cb864e3ed29d733b3476e1f4416849d3f383`  
		Last Modified: Tue, 02 Mar 2021 01:15:01 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:latest`

```console
$ docker pull nats-streaming@sha256:b5fcf8cc22f7bc9bc8724023dfee42d39861c20760558f0a2863987ae20214c4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.1757; amd64

### `nats-streaming:latest` - linux; amd64

```console
$ docker pull nats-streaming@sha256:3783631861947e0e679506679efc64c4875f4804205377e4311e9cdab6c17965
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.7 MB (5679887 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:699c5c09ce0b6a8314d7acec3aa4c72dbaa6a6bc44881fa83719dcf5e2e5a1e1`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 02 Mar 2021 00:25:52 GMT
COPY file:4c2a24d146429270418a17857993903d39b1fcf52d11a560abd159eff99ada8d in /nats-streaming-server 
# Tue, 02 Mar 2021 00:25:52 GMT
EXPOSE 4222 8222
# Tue, 02 Mar 2021 00:25:53 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 02 Mar 2021 00:25:53 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:7fb87f3f85e42eb0fc3d88581c0b84a8d675859dd6727be9100fa9bbaa2cffa4`  
		Last Modified: Tue, 02 Mar 2021 00:26:20 GMT  
		Size: 5.7 MB (5679887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:latest` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:48598a6e49d6cdd1e0829bd4d7ead1aff8b18dd07440a20337e701a94caca26e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.3 MB (5250920 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dffd1cc2cc6030e177fe45935f0fee3c62a59fdda8b12c3276d39fa19a6928b1`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 02 Mar 2021 00:26:52 GMT
COPY file:4baaca51b76d42c66f7a4d5146b598f666c38803f36a5286ede362691d89663c in /nats-streaming-server 
# Tue, 02 Mar 2021 00:26:53 GMT
EXPOSE 4222 8222
# Tue, 02 Mar 2021 00:26:53 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 02 Mar 2021 00:26:54 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:92433c508db76d76c2073b4044b8e2a847d00a4148b85326fe4be63f691ef9af`  
		Last Modified: Tue, 02 Mar 2021 00:27:35 GMT  
		Size: 5.3 MB (5250920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:latest` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:ae774aee41bd64306207d739d2290639f673c9c66c367a83f155a923fe8c13f6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5246286 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ce52186dd957f6b70b086fdcbc8212e079e5ed5e3e0013f8f72b3922535a56e`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Sat, 06 Mar 2021 01:00:25 GMT
COPY file:546c18b3e8e91d453d1a325c6e4dbc3c945564c010676da1abe89a653a0dea84 in /nats-streaming-server 
# Sat, 06 Mar 2021 01:00:27 GMT
EXPOSE 4222 8222
# Sat, 06 Mar 2021 01:00:28 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Sat, 06 Mar 2021 01:00:29 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:ed8ed2aa5d978cf51ebe3454de1832aeb40919052c5cb17d5b63865c31fc03c7`  
		Last Modified: Sat, 06 Mar 2021 01:01:07 GMT  
		Size: 5.2 MB (5246286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:latest` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:bb0f75068ef5a23352dc064f1f3284e6dab1c2586e6a94e2e606778b78cb03f7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5169160 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6cebf86c02f91c34c49641b50fa91c94e4100b2fa18472ca33b362283355e4c1`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 02 Mar 2021 01:14:35 GMT
COPY file:45fcdc5032324b9c78e16535704285519687d0187fa1b424eb18143deb1dece7 in /nats-streaming-server 
# Tue, 02 Mar 2021 01:14:35 GMT
EXPOSE 4222 8222
# Tue, 02 Mar 2021 01:14:36 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 02 Mar 2021 01:14:37 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:8e9b3f150b42f0a6abecb65490e22f7a6a73c1e139f69e747ca01b46f0c4ff5d`  
		Last Modified: Tue, 02 Mar 2021 01:15:22 GMT  
		Size: 5.2 MB (5169160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:latest` - windows version 10.0.17763.1757; amd64

```console
$ docker pull nats-streaming@sha256:7102fdfcfc56aff3af3af39cec63c0601b43592e56b7e64d187790b0822e9a51
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.2 MB (107219449 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a8a29d1082c9d4ea1c812a4e8d84b8d8c1228d2c1c0c1543350e44bd28b31f4f`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 02 Feb 2021 13:06:30 GMT
RUN Apply image 1809-amd64
# Wed, 10 Feb 2021 16:02:26 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Mon, 01 Mar 2021 23:39:47 GMT
RUN cmd /S /C #(nop) COPY file:24ef21e1be266c0481785b3d2cebe511e1bb8a8c20c99795a9e7fa85b0d7aa50 in C:\nats-streaming-server.exe 
# Mon, 01 Mar 2021 23:39:48 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Mon, 01 Mar 2021 23:39:49 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Mon, 01 Mar 2021 23:39:50 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:ba17af31b9276ee11fdf859681b442db50979a39eff4cea2a559a5755cedbe01`  
		Size: 101.4 MB (101406193 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:23b613036f8aee9066e712b3aa58f10f2fde093623511a5658867f53a6d01b18`  
		Last Modified: Wed, 10 Feb 2021 16:06:34 GMT  
		Size: 1.1 KB (1071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:698ae4ae8df313350ab9792ea25a077b988b965eec472e98f4770b8f5b16ed33`  
		Last Modified: Mon, 01 Mar 2021 23:44:05 GMT  
		Size: 5.8 MB (5808961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec3f2e5ff2ba6f6a9881c98155b50d51c881cd77ced1ed2d75b60867bbc96e65`  
		Last Modified: Mon, 01 Mar 2021 23:43:57 GMT  
		Size: 1.1 KB (1064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aa08ef55ec2e1a3c6b2f7f88cf21aa125c7f3356775287b4f3d83372278cb4e`  
		Last Modified: Mon, 01 Mar 2021 23:43:58 GMT  
		Size: 1.0 KB (1033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af33a16b15f810a8bdb3cfe7c2387d435251d11cd9af0a3d5bf3ee30410ccc51`  
		Last Modified: Mon, 01 Mar 2021 23:43:58 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:linux`

```console
$ docker pull nats-streaming@sha256:f7f7b3ef4aa648855b38e0d4096634786a01e382bd63f478733918da6e341d72
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:linux` - linux; amd64

```console
$ docker pull nats-streaming@sha256:3783631861947e0e679506679efc64c4875f4804205377e4311e9cdab6c17965
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.7 MB (5679887 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:699c5c09ce0b6a8314d7acec3aa4c72dbaa6a6bc44881fa83719dcf5e2e5a1e1`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 02 Mar 2021 00:25:52 GMT
COPY file:4c2a24d146429270418a17857993903d39b1fcf52d11a560abd159eff99ada8d in /nats-streaming-server 
# Tue, 02 Mar 2021 00:25:52 GMT
EXPOSE 4222 8222
# Tue, 02 Mar 2021 00:25:53 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 02 Mar 2021 00:25:53 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:7fb87f3f85e42eb0fc3d88581c0b84a8d675859dd6727be9100fa9bbaa2cffa4`  
		Last Modified: Tue, 02 Mar 2021 00:26:20 GMT  
		Size: 5.7 MB (5679887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:linux` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:48598a6e49d6cdd1e0829bd4d7ead1aff8b18dd07440a20337e701a94caca26e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.3 MB (5250920 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dffd1cc2cc6030e177fe45935f0fee3c62a59fdda8b12c3276d39fa19a6928b1`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 02 Mar 2021 00:26:52 GMT
COPY file:4baaca51b76d42c66f7a4d5146b598f666c38803f36a5286ede362691d89663c in /nats-streaming-server 
# Tue, 02 Mar 2021 00:26:53 GMT
EXPOSE 4222 8222
# Tue, 02 Mar 2021 00:26:53 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 02 Mar 2021 00:26:54 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:92433c508db76d76c2073b4044b8e2a847d00a4148b85326fe4be63f691ef9af`  
		Last Modified: Tue, 02 Mar 2021 00:27:35 GMT  
		Size: 5.3 MB (5250920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:linux` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:ae774aee41bd64306207d739d2290639f673c9c66c367a83f155a923fe8c13f6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5246286 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ce52186dd957f6b70b086fdcbc8212e079e5ed5e3e0013f8f72b3922535a56e`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Sat, 06 Mar 2021 01:00:25 GMT
COPY file:546c18b3e8e91d453d1a325c6e4dbc3c945564c010676da1abe89a653a0dea84 in /nats-streaming-server 
# Sat, 06 Mar 2021 01:00:27 GMT
EXPOSE 4222 8222
# Sat, 06 Mar 2021 01:00:28 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Sat, 06 Mar 2021 01:00:29 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:ed8ed2aa5d978cf51ebe3454de1832aeb40919052c5cb17d5b63865c31fc03c7`  
		Last Modified: Sat, 06 Mar 2021 01:01:07 GMT  
		Size: 5.2 MB (5246286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:linux` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:bb0f75068ef5a23352dc064f1f3284e6dab1c2586e6a94e2e606778b78cb03f7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5169160 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6cebf86c02f91c34c49641b50fa91c94e4100b2fa18472ca33b362283355e4c1`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 02 Mar 2021 01:14:35 GMT
COPY file:45fcdc5032324b9c78e16535704285519687d0187fa1b424eb18143deb1dece7 in /nats-streaming-server 
# Tue, 02 Mar 2021 01:14:35 GMT
EXPOSE 4222 8222
# Tue, 02 Mar 2021 01:14:36 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 02 Mar 2021 01:14:37 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:8e9b3f150b42f0a6abecb65490e22f7a6a73c1e139f69e747ca01b46f0c4ff5d`  
		Last Modified: Tue, 02 Mar 2021 01:15:22 GMT  
		Size: 5.2 MB (5169160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:nanoserver`

```console
$ docker pull nats-streaming@sha256:dda388e643ede382e981561d8783ca34024f18de31dac28bd01ba26525fc06e2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1757; amd64

### `nats-streaming:nanoserver` - windows version 10.0.17763.1757; amd64

```console
$ docker pull nats-streaming@sha256:7102fdfcfc56aff3af3af39cec63c0601b43592e56b7e64d187790b0822e9a51
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.2 MB (107219449 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a8a29d1082c9d4ea1c812a4e8d84b8d8c1228d2c1c0c1543350e44bd28b31f4f`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 02 Feb 2021 13:06:30 GMT
RUN Apply image 1809-amd64
# Wed, 10 Feb 2021 16:02:26 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Mon, 01 Mar 2021 23:39:47 GMT
RUN cmd /S /C #(nop) COPY file:24ef21e1be266c0481785b3d2cebe511e1bb8a8c20c99795a9e7fa85b0d7aa50 in C:\nats-streaming-server.exe 
# Mon, 01 Mar 2021 23:39:48 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Mon, 01 Mar 2021 23:39:49 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Mon, 01 Mar 2021 23:39:50 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:ba17af31b9276ee11fdf859681b442db50979a39eff4cea2a559a5755cedbe01`  
		Size: 101.4 MB (101406193 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:23b613036f8aee9066e712b3aa58f10f2fde093623511a5658867f53a6d01b18`  
		Last Modified: Wed, 10 Feb 2021 16:06:34 GMT  
		Size: 1.1 KB (1071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:698ae4ae8df313350ab9792ea25a077b988b965eec472e98f4770b8f5b16ed33`  
		Last Modified: Mon, 01 Mar 2021 23:44:05 GMT  
		Size: 5.8 MB (5808961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec3f2e5ff2ba6f6a9881c98155b50d51c881cd77ced1ed2d75b60867bbc96e65`  
		Last Modified: Mon, 01 Mar 2021 23:43:57 GMT  
		Size: 1.1 KB (1064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aa08ef55ec2e1a3c6b2f7f88cf21aa125c7f3356775287b4f3d83372278cb4e`  
		Last Modified: Mon, 01 Mar 2021 23:43:58 GMT  
		Size: 1.0 KB (1033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af33a16b15f810a8bdb3cfe7c2387d435251d11cd9af0a3d5bf3ee30410ccc51`  
		Last Modified: Mon, 01 Mar 2021 23:43:58 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:nanoserver-1809`

```console
$ docker pull nats-streaming@sha256:dda388e643ede382e981561d8783ca34024f18de31dac28bd01ba26525fc06e2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1757; amd64

### `nats-streaming:nanoserver-1809` - windows version 10.0.17763.1757; amd64

```console
$ docker pull nats-streaming@sha256:7102fdfcfc56aff3af3af39cec63c0601b43592e56b7e64d187790b0822e9a51
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.2 MB (107219449 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a8a29d1082c9d4ea1c812a4e8d84b8d8c1228d2c1c0c1543350e44bd28b31f4f`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 02 Feb 2021 13:06:30 GMT
RUN Apply image 1809-amd64
# Wed, 10 Feb 2021 16:02:26 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Mon, 01 Mar 2021 23:39:47 GMT
RUN cmd /S /C #(nop) COPY file:24ef21e1be266c0481785b3d2cebe511e1bb8a8c20c99795a9e7fa85b0d7aa50 in C:\nats-streaming-server.exe 
# Mon, 01 Mar 2021 23:39:48 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Mon, 01 Mar 2021 23:39:49 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Mon, 01 Mar 2021 23:39:50 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:ba17af31b9276ee11fdf859681b442db50979a39eff4cea2a559a5755cedbe01`  
		Size: 101.4 MB (101406193 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:23b613036f8aee9066e712b3aa58f10f2fde093623511a5658867f53a6d01b18`  
		Last Modified: Wed, 10 Feb 2021 16:06:34 GMT  
		Size: 1.1 KB (1071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:698ae4ae8df313350ab9792ea25a077b988b965eec472e98f4770b8f5b16ed33`  
		Last Modified: Mon, 01 Mar 2021 23:44:05 GMT  
		Size: 5.8 MB (5808961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec3f2e5ff2ba6f6a9881c98155b50d51c881cd77ced1ed2d75b60867bbc96e65`  
		Last Modified: Mon, 01 Mar 2021 23:43:57 GMT  
		Size: 1.1 KB (1064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aa08ef55ec2e1a3c6b2f7f88cf21aa125c7f3356775287b4f3d83372278cb4e`  
		Last Modified: Mon, 01 Mar 2021 23:43:58 GMT  
		Size: 1.0 KB (1033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af33a16b15f810a8bdb3cfe7c2387d435251d11cd9af0a3d5bf3ee30410ccc51`  
		Last Modified: Mon, 01 Mar 2021 23:43:58 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:scratch`

```console
$ docker pull nats-streaming@sha256:f7f7b3ef4aa648855b38e0d4096634786a01e382bd63f478733918da6e341d72
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:scratch` - linux; amd64

```console
$ docker pull nats-streaming@sha256:3783631861947e0e679506679efc64c4875f4804205377e4311e9cdab6c17965
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.7 MB (5679887 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:699c5c09ce0b6a8314d7acec3aa4c72dbaa6a6bc44881fa83719dcf5e2e5a1e1`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 02 Mar 2021 00:25:52 GMT
COPY file:4c2a24d146429270418a17857993903d39b1fcf52d11a560abd159eff99ada8d in /nats-streaming-server 
# Tue, 02 Mar 2021 00:25:52 GMT
EXPOSE 4222 8222
# Tue, 02 Mar 2021 00:25:53 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 02 Mar 2021 00:25:53 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:7fb87f3f85e42eb0fc3d88581c0b84a8d675859dd6727be9100fa9bbaa2cffa4`  
		Last Modified: Tue, 02 Mar 2021 00:26:20 GMT  
		Size: 5.7 MB (5679887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:scratch` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:48598a6e49d6cdd1e0829bd4d7ead1aff8b18dd07440a20337e701a94caca26e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.3 MB (5250920 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dffd1cc2cc6030e177fe45935f0fee3c62a59fdda8b12c3276d39fa19a6928b1`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 02 Mar 2021 00:26:52 GMT
COPY file:4baaca51b76d42c66f7a4d5146b598f666c38803f36a5286ede362691d89663c in /nats-streaming-server 
# Tue, 02 Mar 2021 00:26:53 GMT
EXPOSE 4222 8222
# Tue, 02 Mar 2021 00:26:53 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 02 Mar 2021 00:26:54 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:92433c508db76d76c2073b4044b8e2a847d00a4148b85326fe4be63f691ef9af`  
		Last Modified: Tue, 02 Mar 2021 00:27:35 GMT  
		Size: 5.3 MB (5250920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:scratch` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:ae774aee41bd64306207d739d2290639f673c9c66c367a83f155a923fe8c13f6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5246286 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ce52186dd957f6b70b086fdcbc8212e079e5ed5e3e0013f8f72b3922535a56e`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Sat, 06 Mar 2021 01:00:25 GMT
COPY file:546c18b3e8e91d453d1a325c6e4dbc3c945564c010676da1abe89a653a0dea84 in /nats-streaming-server 
# Sat, 06 Mar 2021 01:00:27 GMT
EXPOSE 4222 8222
# Sat, 06 Mar 2021 01:00:28 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Sat, 06 Mar 2021 01:00:29 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:ed8ed2aa5d978cf51ebe3454de1832aeb40919052c5cb17d5b63865c31fc03c7`  
		Last Modified: Sat, 06 Mar 2021 01:01:07 GMT  
		Size: 5.2 MB (5246286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:scratch` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:bb0f75068ef5a23352dc064f1f3284e6dab1c2586e6a94e2e606778b78cb03f7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5169160 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6cebf86c02f91c34c49641b50fa91c94e4100b2fa18472ca33b362283355e4c1`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 02 Mar 2021 01:14:35 GMT
COPY file:45fcdc5032324b9c78e16535704285519687d0187fa1b424eb18143deb1dece7 in /nats-streaming-server 
# Tue, 02 Mar 2021 01:14:35 GMT
EXPOSE 4222 8222
# Tue, 02 Mar 2021 01:14:36 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 02 Mar 2021 01:14:37 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:8e9b3f150b42f0a6abecb65490e22f7a6a73c1e139f69e747ca01b46f0c4ff5d`  
		Last Modified: Tue, 02 Mar 2021 01:15:22 GMT  
		Size: 5.2 MB (5169160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:windowsservercore`

```console
$ docker pull nats-streaming@sha256:0728f2a6f38b6ddc9220b714320ea805334d12ff55fe3085f54fd4c3990ffa48
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1757; amd64
	-	windows version 10.0.14393.4225; amd64

### `nats-streaming:windowsservercore` - windows version 10.0.17763.1757; amd64

```console
$ docker pull nats-streaming@sha256:f37e01c95a35e80a9ded4c68744089da72385d2b912ea64785af120e5dfac46e
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2459529339 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b413bdbbbc445bd56eec6684f454ad90530794c0c418fe4d91945d27158fd2ca`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 06 Feb 2021 05:03:14 GMT
RUN Install update 1809-amd64
# Tue, 09 Feb 2021 20:26:38 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Feb 2021 16:00:30 GMT
ENV NATS_DOCKERIZED=1
# Mon, 01 Mar 2021 23:37:33 GMT
ENV NATS_STREAMING_SERVER=0.21.0
# Mon, 01 Mar 2021 23:37:34 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.21.0/nats-streaming-server-v0.21.0-windows-amd64.zip
# Mon, 01 Mar 2021 23:37:35 GMT
ENV GIT_DOWNLOAD_SHA256=00bd52804208a52014f518836198a3ebcd513fc5029eda9de2b4ef846f5cb828
# Mon, 01 Mar 2021 23:38:06 GMT
RUN Set-PSDebug -Trace 2
# Mon, 01 Mar 2021 23:39:26 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Mon, 01 Mar 2021 23:39:27 GMT
EXPOSE 4222 8222
# Mon, 01 Mar 2021 23:39:29 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Mon, 01 Mar 2021 23:39:30 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:db4edcf0861ff3fdc41851a5a218965ecb2ab6cf4ec9448fb80cc4b6792fd46c`  
		Size: 720.9 MB (720933935 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:751b8860e89a7e6999d74a11dc393620b118057ad881cb87f1d6e3653cb2db43`  
		Last Modified: Tue, 09 Feb 2021 20:48:09 GMT  
		Size: 1.3 KB (1337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7f01e717591f83c73890556e7a4c77e53caed8daf6c9b0150f497e094a4a698`  
		Last Modified: Wed, 10 Feb 2021 16:06:05 GMT  
		Size: 1.4 KB (1361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cee7e8f68acf02f1803fbe58fd1c98e5136b5c448a9ac12d39f5a4a64ce198a8`  
		Last Modified: Mon, 01 Mar 2021 23:43:41 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16c75a51835c930004670181ad34afd7c2e90ba762a6696cfc732939750e5023`  
		Last Modified: Mon, 01 Mar 2021 23:43:42 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00d34a3454dc6e83cea274b8fd2765fef221836a6993fbe56ceac434981fb5b0`  
		Last Modified: Mon, 01 Mar 2021 23:43:41 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0dcdeb9a6756964b7928054f4f2182d16a35b34ea18396a0d4b38cf484fd9f1`  
		Last Modified: Mon, 01 Mar 2021 23:43:37 GMT  
		Size: 5.1 MB (5051217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a34eb42fac48c971f1a0135c6584d1083bb0e536911e46b1a1e389c4ffe729a8`  
		Last Modified: Mon, 01 Mar 2021 23:43:41 GMT  
		Size: 15.2 MB (15200127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f665eadac63d2ed583f4d30a7d28791f710880674a828e61d8c2105ce70655d3`  
		Last Modified: Mon, 01 Mar 2021 23:43:36 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13fe9508026c89dd38a20a05c48fc44dcb7d86441cdcb88457d74e6625ee04cc`  
		Last Modified: Mon, 01 Mar 2021 23:43:36 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:024aa4f6d5eeceaecd71aa08ba9e78ea00fd32ea15890f9d228db2fc18580407`  
		Last Modified: Mon, 01 Mar 2021 23:43:35 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:windowsservercore` - windows version 10.0.14393.4225; amd64

```console
$ docker pull nats-streaming@sha256:eb47ac16c5b855632476a7b18bf7e414b1bd8f550cc6076715b87e5f0b3a531b
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5816649326 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:76ab14b94a5ce8d1e02ac5175112977ea6d3a9ab5a4b1d4f23979ef50fe19563`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 27 Jan 2021 18:11:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 09 Feb 2021 20:28:50 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Feb 2021 16:02:35 GMT
ENV NATS_DOCKERIZED=1
# Mon, 01 Mar 2021 23:39:57 GMT
ENV NATS_STREAMING_SERVER=0.21.0
# Mon, 01 Mar 2021 23:39:58 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.21.0/nats-streaming-server-v0.21.0-windows-amd64.zip
# Mon, 01 Mar 2021 23:39:59 GMT
ENV GIT_DOWNLOAD_SHA256=00bd52804208a52014f518836198a3ebcd513fc5029eda9de2b4ef846f5cb828
# Mon, 01 Mar 2021 23:41:08 GMT
RUN Set-PSDebug -Trace 2
# Mon, 01 Mar 2021 23:42:59 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Mon, 01 Mar 2021 23:43:00 GMT
EXPOSE 4222 8222
# Mon, 01 Mar 2021 23:43:01 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Mon, 01 Mar 2021 23:43:02 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:62c48323ed8ac695b8cbe0ecedcc28ba185a234673ad9241df2b151dd00f9181`  
		Size: 1.7 GB (1725027107 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ac4a230905430e1aea27172a9432f576cc4a530e72bea516a2b304d2b7e9c101`  
		Last Modified: Tue, 09 Feb 2021 20:49:11 GMT  
		Size: 1.4 KB (1356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cc28e30e89dab2d0b2b2f6c3114771d9d803d5942c730de78d2dd457ad4ac40`  
		Last Modified: Wed, 10 Feb 2021 16:06:59 GMT  
		Size: 1.4 KB (1361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e865ae49ff7ab275634dd5c255d968f5f0f59d027134ad6df4133fa52d0d0af`  
		Last Modified: Mon, 01 Mar 2021 23:44:20 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:512f73566aa9bcff8499433bf39ef4bf7fbf46bcaf045cdfe4cdc3b374fd4ac3`  
		Last Modified: Mon, 01 Mar 2021 23:44:20 GMT  
		Size: 1.3 KB (1306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:322aaa185ec2b5e90cc9eb8c57ee82a54b439aafd42bb20b59e2736d28cdc8e1`  
		Last Modified: Mon, 01 Mar 2021 23:44:20 GMT  
		Size: 1.3 KB (1302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2f75278df3ba6220910463178e2fd69782bbc0c3abbbfa41ddd271358106f32`  
		Last Modified: Mon, 01 Mar 2021 23:44:21 GMT  
		Size: 5.7 MB (5657685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b36a484255a580d8cbe179712aec8211899c8500471dcd9802790090750911c0`  
		Last Modified: Mon, 01 Mar 2021 23:44:36 GMT  
		Size: 16.0 MB (15967963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d1eabaebec46e6111a59bec9221d1e0d4973de580e30a453fa7bbb2e1ad9385`  
		Last Modified: Mon, 01 Mar 2021 23:44:17 GMT  
		Size: 1.3 KB (1300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fef8d63616ebeb7cc5aa29815610700aeccd828419c232dd4b8ba2edc47f8a7`  
		Last Modified: Mon, 01 Mar 2021 23:44:17 GMT  
		Size: 1.3 KB (1334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32683573142d691c7c5ca7fbebf8c2d37bd0ab61abafdf7be2690d440dcad8c0`  
		Last Modified: Mon, 01 Mar 2021 23:44:17 GMT  
		Size: 1.3 KB (1321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:windowsservercore-1809`

```console
$ docker pull nats-streaming@sha256:66f478d3ebc42ecbb2578543c96ac3870f81725bef104339e705e1ab95d5ba9c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1757; amd64

### `nats-streaming:windowsservercore-1809` - windows version 10.0.17763.1757; amd64

```console
$ docker pull nats-streaming@sha256:f37e01c95a35e80a9ded4c68744089da72385d2b912ea64785af120e5dfac46e
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2459529339 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b413bdbbbc445bd56eec6684f454ad90530794c0c418fe4d91945d27158fd2ca`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 06 Feb 2021 05:03:14 GMT
RUN Install update 1809-amd64
# Tue, 09 Feb 2021 20:26:38 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Feb 2021 16:00:30 GMT
ENV NATS_DOCKERIZED=1
# Mon, 01 Mar 2021 23:37:33 GMT
ENV NATS_STREAMING_SERVER=0.21.0
# Mon, 01 Mar 2021 23:37:34 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.21.0/nats-streaming-server-v0.21.0-windows-amd64.zip
# Mon, 01 Mar 2021 23:37:35 GMT
ENV GIT_DOWNLOAD_SHA256=00bd52804208a52014f518836198a3ebcd513fc5029eda9de2b4ef846f5cb828
# Mon, 01 Mar 2021 23:38:06 GMT
RUN Set-PSDebug -Trace 2
# Mon, 01 Mar 2021 23:39:26 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Mon, 01 Mar 2021 23:39:27 GMT
EXPOSE 4222 8222
# Mon, 01 Mar 2021 23:39:29 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Mon, 01 Mar 2021 23:39:30 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:db4edcf0861ff3fdc41851a5a218965ecb2ab6cf4ec9448fb80cc4b6792fd46c`  
		Size: 720.9 MB (720933935 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:751b8860e89a7e6999d74a11dc393620b118057ad881cb87f1d6e3653cb2db43`  
		Last Modified: Tue, 09 Feb 2021 20:48:09 GMT  
		Size: 1.3 KB (1337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7f01e717591f83c73890556e7a4c77e53caed8daf6c9b0150f497e094a4a698`  
		Last Modified: Wed, 10 Feb 2021 16:06:05 GMT  
		Size: 1.4 KB (1361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cee7e8f68acf02f1803fbe58fd1c98e5136b5c448a9ac12d39f5a4a64ce198a8`  
		Last Modified: Mon, 01 Mar 2021 23:43:41 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16c75a51835c930004670181ad34afd7c2e90ba762a6696cfc732939750e5023`  
		Last Modified: Mon, 01 Mar 2021 23:43:42 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00d34a3454dc6e83cea274b8fd2765fef221836a6993fbe56ceac434981fb5b0`  
		Last Modified: Mon, 01 Mar 2021 23:43:41 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0dcdeb9a6756964b7928054f4f2182d16a35b34ea18396a0d4b38cf484fd9f1`  
		Last Modified: Mon, 01 Mar 2021 23:43:37 GMT  
		Size: 5.1 MB (5051217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a34eb42fac48c971f1a0135c6584d1083bb0e536911e46b1a1e389c4ffe729a8`  
		Last Modified: Mon, 01 Mar 2021 23:43:41 GMT  
		Size: 15.2 MB (15200127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f665eadac63d2ed583f4d30a7d28791f710880674a828e61d8c2105ce70655d3`  
		Last Modified: Mon, 01 Mar 2021 23:43:36 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13fe9508026c89dd38a20a05c48fc44dcb7d86441cdcb88457d74e6625ee04cc`  
		Last Modified: Mon, 01 Mar 2021 23:43:36 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:024aa4f6d5eeceaecd71aa08ba9e78ea00fd32ea15890f9d228db2fc18580407`  
		Last Modified: Mon, 01 Mar 2021 23:43:35 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:windowsservercore-ltsc2016`

```console
$ docker pull nats-streaming@sha256:915d9002166880b04fb879b327a5382eb1d1962f95238efaa47b85bf58410a31
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4225; amd64

### `nats-streaming:windowsservercore-ltsc2016` - windows version 10.0.14393.4225; amd64

```console
$ docker pull nats-streaming@sha256:eb47ac16c5b855632476a7b18bf7e414b1bd8f550cc6076715b87e5f0b3a531b
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5816649326 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:76ab14b94a5ce8d1e02ac5175112977ea6d3a9ab5a4b1d4f23979ef50fe19563`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 27 Jan 2021 18:11:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 09 Feb 2021 20:28:50 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Feb 2021 16:02:35 GMT
ENV NATS_DOCKERIZED=1
# Mon, 01 Mar 2021 23:39:57 GMT
ENV NATS_STREAMING_SERVER=0.21.0
# Mon, 01 Mar 2021 23:39:58 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.21.0/nats-streaming-server-v0.21.0-windows-amd64.zip
# Mon, 01 Mar 2021 23:39:59 GMT
ENV GIT_DOWNLOAD_SHA256=00bd52804208a52014f518836198a3ebcd513fc5029eda9de2b4ef846f5cb828
# Mon, 01 Mar 2021 23:41:08 GMT
RUN Set-PSDebug -Trace 2
# Mon, 01 Mar 2021 23:42:59 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Mon, 01 Mar 2021 23:43:00 GMT
EXPOSE 4222 8222
# Mon, 01 Mar 2021 23:43:01 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Mon, 01 Mar 2021 23:43:02 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:62c48323ed8ac695b8cbe0ecedcc28ba185a234673ad9241df2b151dd00f9181`  
		Size: 1.7 GB (1725027107 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ac4a230905430e1aea27172a9432f576cc4a530e72bea516a2b304d2b7e9c101`  
		Last Modified: Tue, 09 Feb 2021 20:49:11 GMT  
		Size: 1.4 KB (1356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cc28e30e89dab2d0b2b2f6c3114771d9d803d5942c730de78d2dd457ad4ac40`  
		Last Modified: Wed, 10 Feb 2021 16:06:59 GMT  
		Size: 1.4 KB (1361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e865ae49ff7ab275634dd5c255d968f5f0f59d027134ad6df4133fa52d0d0af`  
		Last Modified: Mon, 01 Mar 2021 23:44:20 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:512f73566aa9bcff8499433bf39ef4bf7fbf46bcaf045cdfe4cdc3b374fd4ac3`  
		Last Modified: Mon, 01 Mar 2021 23:44:20 GMT  
		Size: 1.3 KB (1306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:322aaa185ec2b5e90cc9eb8c57ee82a54b439aafd42bb20b59e2736d28cdc8e1`  
		Last Modified: Mon, 01 Mar 2021 23:44:20 GMT  
		Size: 1.3 KB (1302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2f75278df3ba6220910463178e2fd69782bbc0c3abbbfa41ddd271358106f32`  
		Last Modified: Mon, 01 Mar 2021 23:44:21 GMT  
		Size: 5.7 MB (5657685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b36a484255a580d8cbe179712aec8211899c8500471dcd9802790090750911c0`  
		Last Modified: Mon, 01 Mar 2021 23:44:36 GMT  
		Size: 16.0 MB (15967963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d1eabaebec46e6111a59bec9221d1e0d4973de580e30a453fa7bbb2e1ad9385`  
		Last Modified: Mon, 01 Mar 2021 23:44:17 GMT  
		Size: 1.3 KB (1300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fef8d63616ebeb7cc5aa29815610700aeccd828419c232dd4b8ba2edc47f8a7`  
		Last Modified: Mon, 01 Mar 2021 23:44:17 GMT  
		Size: 1.3 KB (1334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32683573142d691c7c5ca7fbebf8c2d37bd0ab61abafdf7be2690d440dcad8c0`  
		Last Modified: Mon, 01 Mar 2021 23:44:17 GMT  
		Size: 1.3 KB (1321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
