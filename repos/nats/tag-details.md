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
-	[`nats:2.9.18`](#nats2918)
-	[`nats:2.9.18-alpine`](#nats2918-alpine)
-	[`nats:2.9.18-alpine3.18`](#nats2918-alpine318)
-	[`nats:2.9.18-linux`](#nats2918-linux)
-	[`nats:2.9.18-nanoserver`](#nats2918-nanoserver)
-	[`nats:2.9.18-nanoserver-1809`](#nats2918-nanoserver-1809)
-	[`nats:2.9.18-scratch`](#nats2918-scratch)
-	[`nats:2.9.18-windowsservercore`](#nats2918-windowsservercore)
-	[`nats:2.9.18-windowsservercore-1809`](#nats2918-windowsservercore-1809)
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
$ docker pull nats@sha256:a600ddb07ea351ff9a7d0a49f7cc8fcd930c232d55f7c18f17378c3b4f7a83e7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.4377; amd64

### `nats:2` - linux; amd64

```console
$ docker pull nats@sha256:d7a57514cf7a0949ab8e63985f040f1fbaa01aa70aa50d8485f796a9a8dead08
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5117129 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4bd1a8b681814e86af7f1b07aa7178abd74163b5101ad1f855420c25d4afae5e`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 18 May 2023 21:19:59 GMT
COPY file:a3e4cfa40e3f87cbc1a2427fe9e77a182eed251b7a2f3037b894ac919acda56d in /nats-server 
# Thu, 18 May 2023 21:19:59 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 18 May 2023 21:19:59 GMT
EXPOSE 4222 6222 8222
# Thu, 18 May 2023 21:19:59 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 18 May 2023 21:19:59 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 18 May 2023 21:19:59 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:e7f86c5b152db9b1815749cb2d298d36014c2905070ae66128b67029b4b31780`  
		Last Modified: Thu, 18 May 2023 21:20:38 GMT  
		Size: 5.1 MB (5116621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:623ce2c40f365197112db5bf1e3ed9b09b631da2058b456f99a50a5890fdda44`  
		Last Modified: Thu, 18 May 2023 21:20:37 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - linux; arm variant v6

```console
$ docker pull nats@sha256:f26f23aad2feedaeaca9df38eca5559b431fbb8ed841789b1e6b2c3c84ffa79b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4884857 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8ae95e37599ef924cfe3d5890b3af209e09951179f6672d35af6811876e61253`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 13 Jun 2023 21:49:33 GMT
COPY file:e5bb5e8247a1c4bdb92d70dc84443f615728207816f4c76763893029e98fe987 in /nats-server 
# Tue, 13 Jun 2023 21:49:33 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 13 Jun 2023 21:49:33 GMT
EXPOSE 4222 6222 8222
# Tue, 13 Jun 2023 21:49:33 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 13 Jun 2023 21:49:33 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 13 Jun 2023 21:49:33 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:7f1a7a7f3e313c163918678d53d48af6476087e63070356ad38ff1c041606bca`  
		Last Modified: Tue, 13 Jun 2023 21:50:13 GMT  
		Size: 4.9 MB (4884348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9af05a149bcbd29ea7705539c8b49e2c00b5883848519f3929bf4c4dc424022e`  
		Last Modified: Tue, 13 Jun 2023 21:50:12 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - linux; arm variant v7

```console
$ docker pull nats@sha256:94bf4a62f52fd647adb621d2d584e9c48aea06b124fb81cd59afed50252071bd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4874864 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a8b8de1397d0af96648a1d02610dc54a066633c75eb548fc6be7e0d15497c3c`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 18 May 2023 21:57:50 GMT
COPY file:31e26234e2abf1c16cd5869033f07320118e6dc458af341f37a27a3d12ffbc65 in /nats-server 
# Thu, 18 May 2023 21:57:50 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 18 May 2023 21:57:51 GMT
EXPOSE 4222 6222 8222
# Thu, 18 May 2023 21:57:51 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 18 May 2023 21:57:51 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 18 May 2023 21:57:51 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b6209c6f59228d4816baef6c05a38f68693937e6c86969581c57a1c7b68ccb40`  
		Last Modified: Thu, 18 May 2023 21:58:28 GMT  
		Size: 4.9 MB (4874355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c69c5a4696da201d78c2dae749a6bce01c3a924afbdfa7e87c6797b8db238d4d`  
		Last Modified: Thu, 18 May 2023 21:58:27 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:edbf69c3a8dab18af6eefffc70fcea84205a4397632e23fbde4cca5fe03446ff
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4688025 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b395b40ae1ff951faa10f8f5c05810b77b0a03c2ef5a8eaa8bc443497b52348d`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 13 Jun 2023 22:34:13 GMT
COPY file:0fec8537fba7c573dbe20b854a6b32d8b0940e46f9e81c41611d447b82a034bc in /nats-server 
# Tue, 13 Jun 2023 22:34:13 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 13 Jun 2023 22:34:13 GMT
EXPOSE 4222 6222 8222
# Tue, 13 Jun 2023 22:34:14 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 13 Jun 2023 22:34:14 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 13 Jun 2023 22:34:14 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:2cce796fcd5a4e60d6ca871c71b29485d80a6babd1c43a056db0b52aa6e904b6`  
		Last Modified: Tue, 13 Jun 2023 22:34:58 GMT  
		Size: 4.7 MB (4687516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22153c0efa275cbe62c344213d16db73c5732467534b2a316e379bdd77324d29`  
		Last Modified: Tue, 13 Jun 2023 22:34:57 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - windows version 10.0.17763.4377; amd64

```console
$ docker pull nats@sha256:ffdbc972ae083180acdcc8d74756ed6c94b032bce6d7ec4c224f8343919f232d
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.6 MB (109564530 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b23b2cb10135235e109abd0ca99d3cf4027f72a1c246c873707190f54bffec4`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 05 May 2023 11:29:01 GMT
RUN Apply image 10.0.17763.4377
# Wed, 10 May 2023 02:43:57 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Tue, 13 Jun 2023 22:18:13 GMT
RUN cmd /S /C #(nop) COPY file:e92fb324fb1e715aaa4f213ef42afe80c4a76690e3b2d439bee510cb2ae47cd5 in C:\nats-server.exe 
# Tue, 13 Jun 2023 22:18:14 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Tue, 13 Jun 2023 22:18:15 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Tue, 13 Jun 2023 22:18:15 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 13 Jun 2023 22:18:16 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:f7885e3a2dfeae5eea125d00da688c29930a05e4d904884fe43e093ce6223664`  
		Last Modified: Wed, 10 May 2023 01:49:01 GMT  
		Size: 104.4 MB (104383998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9af27dd7e62b7d94fa31a7c9efd9a532c42db89ec01fdb7fe430043ceabc5b4`  
		Last Modified: Wed, 10 May 2023 02:49:27 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74147f1370eb575d5bc03ac650054b5dcc36d7b40bf7706dde9d9d159d10e1a8`  
		Last Modified: Tue, 13 Jun 2023 22:19:04 GMT  
		Size: 5.2 MB (5174125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c441087537bf6a2963fdc58d12d836350044355df07fa9d696fe6e61819cc0ea`  
		Last Modified: Tue, 13 Jun 2023 22:19:02 GMT  
		Size: 1.8 KB (1803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94f7788277dc1622146a19b5407e20fc8eb003cd62b331460221d930e9154d31`  
		Last Modified: Tue, 13 Jun 2023 22:19:02 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b991262b6e730687a02c0d68ac25bc2dcf4dff69f1e9db5315f654387aab754`  
		Last Modified: Tue, 13 Jun 2023 22:19:02 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c322d11690204cb63afb856a65f1fdd8016ebd23989de8952a6ecb7f6737f17e`  
		Last Modified: Tue, 13 Jun 2023 22:19:02 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-alpine`

```console
$ docker pull nats@sha256:d2647f1f7552973967b5b974d098c290c62dcf29eedfed515917ded32afe4a94
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-alpine` - linux; amd64

```console
$ docker pull nats@sha256:7544f1dfe4b270789a68e2056135467d525da411f331f43640150b0642dee693
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.8 MB (8802768 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:04ada7bbdb360a5406551ced3593bc48e57c6cea5ee5d502e1a0df2437156d06`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 May 2023 23:11:10 GMT
ADD file:7625ddfd589fb824ee39f1b1eb387b98f3676420ff52f26eb9d975151e889667 in / 
# Tue, 09 May 2023 23:11:10 GMT
CMD ["/bin/sh"]
# Thu, 18 May 2023 21:19:49 GMT
ENV NATS_SERVER=2.9.17
# Thu, 18 May 2023 21:19:51 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='c7cf7bf8c029500d1b51773132ecc13a1fc89f2e080faa6b505da8cb95aa2a0c' ;; 		armhf) natsArch='arm6'; sha256='b09812858f1c957fd1869e21d4b8d64b3b0d6cdf3abb34502167120640f1d5e1' ;; 		armv7) natsArch='arm7'; sha256='970649306f45c78404c42dc5c0ab37fa6d5149501e47a68bef7841a06730a654' ;; 		x86_64) natsArch='amd64'; sha256='4ad2d83dd2fb9cc44a7e078d2e400f37c188b8515100f5de0f10f0eefbeb6b23' ;; 		x86) natsArch='386'; sha256='59c42f21bb6e8a5ef6e101ce6e3c29692b2cc9b1eb28465e67edeb391450626c' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 18 May 2023 21:19:52 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 18 May 2023 21:19:52 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 18 May 2023 21:19:52 GMT
EXPOSE 4222 6222 8222
# Thu, 18 May 2023 21:19:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 18 May 2023 21:19:52 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:8a49fdb3b6a5ff2bd8ec6a86c05b2922a0f7454579ecc07637e94dfd1d0639b6`  
		Last Modified: Tue, 09 May 2023 23:11:26 GMT  
		Size: 3.4 MB (3397490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ba69a821f226517d8763fd5007b51eeb8a68e40f7fb32dec75e13297ea1cb49`  
		Last Modified: Thu, 18 May 2023 21:20:19 GMT  
		Size: 5.4 MB (5404276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11ad2f9c9076c4ccedf3a056bf6e996a658fa5ece8cc35913e4728d58617e8b3`  
		Last Modified: Thu, 18 May 2023 21:20:18 GMT  
		Size: 588.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bb3c123b7bd114e7897ddf602c16bcd18f034abda3ee53d91a108b71c624faa`  
		Last Modified: Thu, 18 May 2023 21:20:18 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:957b9d5d12d8d9df6fea32822bd03a00b514635d8ede3f04c8fe3a2a0e8c436f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.3 MB (8326824 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9512db9e4ee16375a3bc31274c1b7a0480263800e5c7cfd91f794674b53e15a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 May 2023 23:11:04 GMT
ADD file:f87a991e2e9f185fd4a88569d86a9b8e5bc07182e7fa613b95acab25986f2a6c in / 
# Tue, 09 May 2023 23:11:04 GMT
CMD ["/bin/sh"]
# Tue, 13 Jun 2023 21:49:21 GMT
ENV NATS_SERVER=2.9.18
# Tue, 13 Jun 2023 21:49:24 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f5ea0ace65873cf81dde2951d9130f6ecad3f96e80a59badb259a66fc3294579' ;; 		armhf) natsArch='arm6'; sha256='f7dd549c09bac2adcc3260868bf5f182645c8e59e7b9cb868feff244017998b0' ;; 		armv7) natsArch='arm7'; sha256='bb1015887864e7eeeeb8bef4c9e06bd20d865b01a67bab8bab802ef5483bb6ad' ;; 		x86_64) natsArch='amd64'; sha256='c61c5dd662ed0836d752ed98508d5a7328d85e6126d2cf9784a0d546a64c961c' ;; 		x86) natsArch='386'; sha256='68467b7d83a96a554257b84464bdff34de956af93971e43faa711e1cb29249c8' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 13 Jun 2023 21:49:24 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 13 Jun 2023 21:49:24 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 13 Jun 2023 21:49:24 GMT
EXPOSE 4222 6222 8222
# Tue, 13 Jun 2023 21:49:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Jun 2023 21:49:25 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:015ee8d9fb3dca1b18815f1e4ee0d325d1f40cde6f2df4dd307918f7b69167d7`  
		Last Modified: Tue, 09 May 2023 23:11:20 GMT  
		Size: 3.2 MB (3155679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21a6505f5ff97d93b3e5451bb54fc64eea5680c617ce8cc7501394caf032f27f`  
		Last Modified: Tue, 13 Jun 2023 21:49:52 GMT  
		Size: 5.2 MB (5170145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43d0bff33a6560b8efd5c213b10cd3176703757ba35859a5ec499ca24abb1139`  
		Last Modified: Tue, 13 Jun 2023 21:49:51 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea53aff73c749d762e22ffbd5e9caecadeb064790877afe9c0b536284c9e4c59`  
		Last Modified: Tue, 13 Jun 2023 21:49:51 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:882066add3894dc13cfadaeec8af9f9fce5b9c3fee92e377a13f0997a88a121f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.1 MB (8071388 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:574536f22d8de67b2c2f0962d9e7d108bb4b41d07cb13a05ebab5e3b82fe6d63`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 May 2023 22:57:32 GMT
ADD file:eb6b6a885e8ac9bccbf44a5c673b8542c8144bba927376688240446c2f413b10 in / 
# Tue, 09 May 2023 22:57:32 GMT
CMD ["/bin/sh"]
# Thu, 18 May 2023 21:57:27 GMT
ENV NATS_SERVER=2.9.17
# Thu, 18 May 2023 21:57:29 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='c7cf7bf8c029500d1b51773132ecc13a1fc89f2e080faa6b505da8cb95aa2a0c' ;; 		armhf) natsArch='arm6'; sha256='b09812858f1c957fd1869e21d4b8d64b3b0d6cdf3abb34502167120640f1d5e1' ;; 		armv7) natsArch='arm7'; sha256='970649306f45c78404c42dc5c0ab37fa6d5149501e47a68bef7841a06730a654' ;; 		x86_64) natsArch='amd64'; sha256='4ad2d83dd2fb9cc44a7e078d2e400f37c188b8515100f5de0f10f0eefbeb6b23' ;; 		x86) natsArch='386'; sha256='59c42f21bb6e8a5ef6e101ce6e3c29692b2cc9b1eb28465e67edeb391450626c' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 18 May 2023 21:57:29 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 18 May 2023 21:57:29 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 18 May 2023 21:57:29 GMT
EXPOSE 4222 6222 8222
# Thu, 18 May 2023 21:57:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 18 May 2023 21:57:30 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:e14425cf8fb9304b9ad4a9d1250e0d4c22e507a334ff747fa69b804500afc113`  
		Last Modified: Tue, 09 May 2023 22:57:50 GMT  
		Size: 2.9 MB (2911117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:213de106e11b3e7261faf48da426167af8702e8a56ab0237f786ba0eb864a38d`  
		Last Modified: Thu, 18 May 2023 21:58:08 GMT  
		Size: 5.2 MB (5159272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5535f74851ba24bbb57849b9f7085eb8441d584ea938b19bdd027f5ccf52a193`  
		Last Modified: Thu, 18 May 2023 21:58:07 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2518eda2d1b2ce9ae4c75acdccc0d3bbe028cfbdf30d7e173dfa82e489af6ec`  
		Last Modified: Thu, 18 May 2023 21:58:08 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:ce87b1ebec8a22151ac8ae437db42293e4293bfecd5045752d86f661b0547b26
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.3 MB (8315499 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bdbca1cbb72621a6502190ab58418aee769fffb9d66712c9ea805d56d3fb46fc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 May 2023 23:11:08 GMT
ADD file:df7fccc3453b6ec1401d27a1295b0882a83e731fde8f23db9d3f687a2b6b4e70 in / 
# Tue, 09 May 2023 23:11:08 GMT
CMD ["/bin/sh"]
# Tue, 13 Jun 2023 22:33:21 GMT
ENV NATS_SERVER=2.9.18
# Tue, 13 Jun 2023 22:33:23 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f5ea0ace65873cf81dde2951d9130f6ecad3f96e80a59badb259a66fc3294579' ;; 		armhf) natsArch='arm6'; sha256='f7dd549c09bac2adcc3260868bf5f182645c8e59e7b9cb868feff244017998b0' ;; 		armv7) natsArch='arm7'; sha256='bb1015887864e7eeeeb8bef4c9e06bd20d865b01a67bab8bab802ef5483bb6ad' ;; 		x86_64) natsArch='amd64'; sha256='c61c5dd662ed0836d752ed98508d5a7328d85e6126d2cf9784a0d546a64c961c' ;; 		x86) natsArch='386'; sha256='68467b7d83a96a554257b84464bdff34de956af93971e43faa711e1cb29249c8' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 13 Jun 2023 22:33:23 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 13 Jun 2023 22:33:23 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 13 Jun 2023 22:33:23 GMT
EXPOSE 4222 6222 8222
# Tue, 13 Jun 2023 22:33:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Jun 2023 22:33:23 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:08409d4172603f40b56eb6b76240a1e6bd78baa0e96590dc7ff76c5f1a093af2`  
		Last Modified: Tue, 09 May 2023 23:11:23 GMT  
		Size: 3.3 MB (3342848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf2d0fd688338eb8ef69b776354053dd65c78ae5e4c3cc2e15fc586f51942d89`  
		Last Modified: Tue, 13 Jun 2023 22:34:38 GMT  
		Size: 5.0 MB (4971650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee9d7fff35b08386d1a65e0e1fa0a81bcc5877d1024bd16ca00f0af62137cdc4`  
		Last Modified: Tue, 13 Jun 2023 22:34:37 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63543f616abdbde1673d999e8e046e0f59aa734ab23d6acabdf42a9756f8c357`  
		Last Modified: Tue, 13 Jun 2023 22:34:37 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-alpine3.18`

```console
$ docker pull nats@sha256:d2647f1f7552973967b5b974d098c290c62dcf29eedfed515917ded32afe4a94
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-alpine3.18` - linux; amd64

```console
$ docker pull nats@sha256:7544f1dfe4b270789a68e2056135467d525da411f331f43640150b0642dee693
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.8 MB (8802768 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:04ada7bbdb360a5406551ced3593bc48e57c6cea5ee5d502e1a0df2437156d06`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 May 2023 23:11:10 GMT
ADD file:7625ddfd589fb824ee39f1b1eb387b98f3676420ff52f26eb9d975151e889667 in / 
# Tue, 09 May 2023 23:11:10 GMT
CMD ["/bin/sh"]
# Thu, 18 May 2023 21:19:49 GMT
ENV NATS_SERVER=2.9.17
# Thu, 18 May 2023 21:19:51 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='c7cf7bf8c029500d1b51773132ecc13a1fc89f2e080faa6b505da8cb95aa2a0c' ;; 		armhf) natsArch='arm6'; sha256='b09812858f1c957fd1869e21d4b8d64b3b0d6cdf3abb34502167120640f1d5e1' ;; 		armv7) natsArch='arm7'; sha256='970649306f45c78404c42dc5c0ab37fa6d5149501e47a68bef7841a06730a654' ;; 		x86_64) natsArch='amd64'; sha256='4ad2d83dd2fb9cc44a7e078d2e400f37c188b8515100f5de0f10f0eefbeb6b23' ;; 		x86) natsArch='386'; sha256='59c42f21bb6e8a5ef6e101ce6e3c29692b2cc9b1eb28465e67edeb391450626c' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 18 May 2023 21:19:52 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 18 May 2023 21:19:52 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 18 May 2023 21:19:52 GMT
EXPOSE 4222 6222 8222
# Thu, 18 May 2023 21:19:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 18 May 2023 21:19:52 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:8a49fdb3b6a5ff2bd8ec6a86c05b2922a0f7454579ecc07637e94dfd1d0639b6`  
		Last Modified: Tue, 09 May 2023 23:11:26 GMT  
		Size: 3.4 MB (3397490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ba69a821f226517d8763fd5007b51eeb8a68e40f7fb32dec75e13297ea1cb49`  
		Last Modified: Thu, 18 May 2023 21:20:19 GMT  
		Size: 5.4 MB (5404276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11ad2f9c9076c4ccedf3a056bf6e996a658fa5ece8cc35913e4728d58617e8b3`  
		Last Modified: Thu, 18 May 2023 21:20:18 GMT  
		Size: 588.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bb3c123b7bd114e7897ddf602c16bcd18f034abda3ee53d91a108b71c624faa`  
		Last Modified: Thu, 18 May 2023 21:20:18 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.18` - linux; arm variant v6

```console
$ docker pull nats@sha256:957b9d5d12d8d9df6fea32822bd03a00b514635d8ede3f04c8fe3a2a0e8c436f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.3 MB (8326824 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9512db9e4ee16375a3bc31274c1b7a0480263800e5c7cfd91f794674b53e15a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 May 2023 23:11:04 GMT
ADD file:f87a991e2e9f185fd4a88569d86a9b8e5bc07182e7fa613b95acab25986f2a6c in / 
# Tue, 09 May 2023 23:11:04 GMT
CMD ["/bin/sh"]
# Tue, 13 Jun 2023 21:49:21 GMT
ENV NATS_SERVER=2.9.18
# Tue, 13 Jun 2023 21:49:24 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f5ea0ace65873cf81dde2951d9130f6ecad3f96e80a59badb259a66fc3294579' ;; 		armhf) natsArch='arm6'; sha256='f7dd549c09bac2adcc3260868bf5f182645c8e59e7b9cb868feff244017998b0' ;; 		armv7) natsArch='arm7'; sha256='bb1015887864e7eeeeb8bef4c9e06bd20d865b01a67bab8bab802ef5483bb6ad' ;; 		x86_64) natsArch='amd64'; sha256='c61c5dd662ed0836d752ed98508d5a7328d85e6126d2cf9784a0d546a64c961c' ;; 		x86) natsArch='386'; sha256='68467b7d83a96a554257b84464bdff34de956af93971e43faa711e1cb29249c8' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 13 Jun 2023 21:49:24 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 13 Jun 2023 21:49:24 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 13 Jun 2023 21:49:24 GMT
EXPOSE 4222 6222 8222
# Tue, 13 Jun 2023 21:49:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Jun 2023 21:49:25 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:015ee8d9fb3dca1b18815f1e4ee0d325d1f40cde6f2df4dd307918f7b69167d7`  
		Last Modified: Tue, 09 May 2023 23:11:20 GMT  
		Size: 3.2 MB (3155679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21a6505f5ff97d93b3e5451bb54fc64eea5680c617ce8cc7501394caf032f27f`  
		Last Modified: Tue, 13 Jun 2023 21:49:52 GMT  
		Size: 5.2 MB (5170145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43d0bff33a6560b8efd5c213b10cd3176703757ba35859a5ec499ca24abb1139`  
		Last Modified: Tue, 13 Jun 2023 21:49:51 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea53aff73c749d762e22ffbd5e9caecadeb064790877afe9c0b536284c9e4c59`  
		Last Modified: Tue, 13 Jun 2023 21:49:51 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.18` - linux; arm variant v7

```console
$ docker pull nats@sha256:882066add3894dc13cfadaeec8af9f9fce5b9c3fee92e377a13f0997a88a121f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.1 MB (8071388 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:574536f22d8de67b2c2f0962d9e7d108bb4b41d07cb13a05ebab5e3b82fe6d63`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 May 2023 22:57:32 GMT
ADD file:eb6b6a885e8ac9bccbf44a5c673b8542c8144bba927376688240446c2f413b10 in / 
# Tue, 09 May 2023 22:57:32 GMT
CMD ["/bin/sh"]
# Thu, 18 May 2023 21:57:27 GMT
ENV NATS_SERVER=2.9.17
# Thu, 18 May 2023 21:57:29 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='c7cf7bf8c029500d1b51773132ecc13a1fc89f2e080faa6b505da8cb95aa2a0c' ;; 		armhf) natsArch='arm6'; sha256='b09812858f1c957fd1869e21d4b8d64b3b0d6cdf3abb34502167120640f1d5e1' ;; 		armv7) natsArch='arm7'; sha256='970649306f45c78404c42dc5c0ab37fa6d5149501e47a68bef7841a06730a654' ;; 		x86_64) natsArch='amd64'; sha256='4ad2d83dd2fb9cc44a7e078d2e400f37c188b8515100f5de0f10f0eefbeb6b23' ;; 		x86) natsArch='386'; sha256='59c42f21bb6e8a5ef6e101ce6e3c29692b2cc9b1eb28465e67edeb391450626c' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 18 May 2023 21:57:29 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 18 May 2023 21:57:29 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 18 May 2023 21:57:29 GMT
EXPOSE 4222 6222 8222
# Thu, 18 May 2023 21:57:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 18 May 2023 21:57:30 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:e14425cf8fb9304b9ad4a9d1250e0d4c22e507a334ff747fa69b804500afc113`  
		Last Modified: Tue, 09 May 2023 22:57:50 GMT  
		Size: 2.9 MB (2911117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:213de106e11b3e7261faf48da426167af8702e8a56ab0237f786ba0eb864a38d`  
		Last Modified: Thu, 18 May 2023 21:58:08 GMT  
		Size: 5.2 MB (5159272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5535f74851ba24bbb57849b9f7085eb8441d584ea938b19bdd027f5ccf52a193`  
		Last Modified: Thu, 18 May 2023 21:58:07 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2518eda2d1b2ce9ae4c75acdccc0d3bbe028cfbdf30d7e173dfa82e489af6ec`  
		Last Modified: Thu, 18 May 2023 21:58:08 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.18` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:ce87b1ebec8a22151ac8ae437db42293e4293bfecd5045752d86f661b0547b26
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.3 MB (8315499 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bdbca1cbb72621a6502190ab58418aee769fffb9d66712c9ea805d56d3fb46fc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 May 2023 23:11:08 GMT
ADD file:df7fccc3453b6ec1401d27a1295b0882a83e731fde8f23db9d3f687a2b6b4e70 in / 
# Tue, 09 May 2023 23:11:08 GMT
CMD ["/bin/sh"]
# Tue, 13 Jun 2023 22:33:21 GMT
ENV NATS_SERVER=2.9.18
# Tue, 13 Jun 2023 22:33:23 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f5ea0ace65873cf81dde2951d9130f6ecad3f96e80a59badb259a66fc3294579' ;; 		armhf) natsArch='arm6'; sha256='f7dd549c09bac2adcc3260868bf5f182645c8e59e7b9cb868feff244017998b0' ;; 		armv7) natsArch='arm7'; sha256='bb1015887864e7eeeeb8bef4c9e06bd20d865b01a67bab8bab802ef5483bb6ad' ;; 		x86_64) natsArch='amd64'; sha256='c61c5dd662ed0836d752ed98508d5a7328d85e6126d2cf9784a0d546a64c961c' ;; 		x86) natsArch='386'; sha256='68467b7d83a96a554257b84464bdff34de956af93971e43faa711e1cb29249c8' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 13 Jun 2023 22:33:23 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 13 Jun 2023 22:33:23 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 13 Jun 2023 22:33:23 GMT
EXPOSE 4222 6222 8222
# Tue, 13 Jun 2023 22:33:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Jun 2023 22:33:23 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:08409d4172603f40b56eb6b76240a1e6bd78baa0e96590dc7ff76c5f1a093af2`  
		Last Modified: Tue, 09 May 2023 23:11:23 GMT  
		Size: 3.3 MB (3342848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf2d0fd688338eb8ef69b776354053dd65c78ae5e4c3cc2e15fc586f51942d89`  
		Last Modified: Tue, 13 Jun 2023 22:34:38 GMT  
		Size: 5.0 MB (4971650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee9d7fff35b08386d1a65e0e1fa0a81bcc5877d1024bd16ca00f0af62137cdc4`  
		Last Modified: Tue, 13 Jun 2023 22:34:37 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63543f616abdbde1673d999e8e046e0f59aa734ab23d6acabdf42a9756f8c357`  
		Last Modified: Tue, 13 Jun 2023 22:34:37 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-linux`

```console
$ docker pull nats@sha256:451705c3735c55b4f7659f8690159fb8f4eb3138e0d4e1b921e4ae325fe46788
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-linux` - linux; amd64

```console
$ docker pull nats@sha256:d7a57514cf7a0949ab8e63985f040f1fbaa01aa70aa50d8485f796a9a8dead08
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5117129 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4bd1a8b681814e86af7f1b07aa7178abd74163b5101ad1f855420c25d4afae5e`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 18 May 2023 21:19:59 GMT
COPY file:a3e4cfa40e3f87cbc1a2427fe9e77a182eed251b7a2f3037b894ac919acda56d in /nats-server 
# Thu, 18 May 2023 21:19:59 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 18 May 2023 21:19:59 GMT
EXPOSE 4222 6222 8222
# Thu, 18 May 2023 21:19:59 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 18 May 2023 21:19:59 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 18 May 2023 21:19:59 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:e7f86c5b152db9b1815749cb2d298d36014c2905070ae66128b67029b4b31780`  
		Last Modified: Thu, 18 May 2023 21:20:38 GMT  
		Size: 5.1 MB (5116621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:623ce2c40f365197112db5bf1e3ed9b09b631da2058b456f99a50a5890fdda44`  
		Last Modified: Thu, 18 May 2023 21:20:37 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:f26f23aad2feedaeaca9df38eca5559b431fbb8ed841789b1e6b2c3c84ffa79b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4884857 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8ae95e37599ef924cfe3d5890b3af209e09951179f6672d35af6811876e61253`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 13 Jun 2023 21:49:33 GMT
COPY file:e5bb5e8247a1c4bdb92d70dc84443f615728207816f4c76763893029e98fe987 in /nats-server 
# Tue, 13 Jun 2023 21:49:33 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 13 Jun 2023 21:49:33 GMT
EXPOSE 4222 6222 8222
# Tue, 13 Jun 2023 21:49:33 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 13 Jun 2023 21:49:33 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 13 Jun 2023 21:49:33 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:7f1a7a7f3e313c163918678d53d48af6476087e63070356ad38ff1c041606bca`  
		Last Modified: Tue, 13 Jun 2023 21:50:13 GMT  
		Size: 4.9 MB (4884348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9af05a149bcbd29ea7705539c8b49e2c00b5883848519f3929bf4c4dc424022e`  
		Last Modified: Tue, 13 Jun 2023 21:50:12 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:94bf4a62f52fd647adb621d2d584e9c48aea06b124fb81cd59afed50252071bd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4874864 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a8b8de1397d0af96648a1d02610dc54a066633c75eb548fc6be7e0d15497c3c`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 18 May 2023 21:57:50 GMT
COPY file:31e26234e2abf1c16cd5869033f07320118e6dc458af341f37a27a3d12ffbc65 in /nats-server 
# Thu, 18 May 2023 21:57:50 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 18 May 2023 21:57:51 GMT
EXPOSE 4222 6222 8222
# Thu, 18 May 2023 21:57:51 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 18 May 2023 21:57:51 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 18 May 2023 21:57:51 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b6209c6f59228d4816baef6c05a38f68693937e6c86969581c57a1c7b68ccb40`  
		Last Modified: Thu, 18 May 2023 21:58:28 GMT  
		Size: 4.9 MB (4874355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c69c5a4696da201d78c2dae749a6bce01c3a924afbdfa7e87c6797b8db238d4d`  
		Last Modified: Thu, 18 May 2023 21:58:27 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:edbf69c3a8dab18af6eefffc70fcea84205a4397632e23fbde4cca5fe03446ff
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4688025 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b395b40ae1ff951faa10f8f5c05810b77b0a03c2ef5a8eaa8bc443497b52348d`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 13 Jun 2023 22:34:13 GMT
COPY file:0fec8537fba7c573dbe20b854a6b32d8b0940e46f9e81c41611d447b82a034bc in /nats-server 
# Tue, 13 Jun 2023 22:34:13 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 13 Jun 2023 22:34:13 GMT
EXPOSE 4222 6222 8222
# Tue, 13 Jun 2023 22:34:14 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 13 Jun 2023 22:34:14 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 13 Jun 2023 22:34:14 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:2cce796fcd5a4e60d6ca871c71b29485d80a6babd1c43a056db0b52aa6e904b6`  
		Last Modified: Tue, 13 Jun 2023 22:34:58 GMT  
		Size: 4.7 MB (4687516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22153c0efa275cbe62c344213d16db73c5732467534b2a316e379bdd77324d29`  
		Last Modified: Tue, 13 Jun 2023 22:34:57 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-nanoserver`

```console
$ docker pull nats@sha256:0a384e9a7d76bb1288a9b091976b9fa61e78c22143d6a07415707fdd6123219c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4377; amd64

### `nats:2-nanoserver` - windows version 10.0.17763.4377; amd64

```console
$ docker pull nats@sha256:ffdbc972ae083180acdcc8d74756ed6c94b032bce6d7ec4c224f8343919f232d
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.6 MB (109564530 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b23b2cb10135235e109abd0ca99d3cf4027f72a1c246c873707190f54bffec4`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 05 May 2023 11:29:01 GMT
RUN Apply image 10.0.17763.4377
# Wed, 10 May 2023 02:43:57 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Tue, 13 Jun 2023 22:18:13 GMT
RUN cmd /S /C #(nop) COPY file:e92fb324fb1e715aaa4f213ef42afe80c4a76690e3b2d439bee510cb2ae47cd5 in C:\nats-server.exe 
# Tue, 13 Jun 2023 22:18:14 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Tue, 13 Jun 2023 22:18:15 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Tue, 13 Jun 2023 22:18:15 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 13 Jun 2023 22:18:16 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:f7885e3a2dfeae5eea125d00da688c29930a05e4d904884fe43e093ce6223664`  
		Last Modified: Wed, 10 May 2023 01:49:01 GMT  
		Size: 104.4 MB (104383998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9af27dd7e62b7d94fa31a7c9efd9a532c42db89ec01fdb7fe430043ceabc5b4`  
		Last Modified: Wed, 10 May 2023 02:49:27 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74147f1370eb575d5bc03ac650054b5dcc36d7b40bf7706dde9d9d159d10e1a8`  
		Last Modified: Tue, 13 Jun 2023 22:19:04 GMT  
		Size: 5.2 MB (5174125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c441087537bf6a2963fdc58d12d836350044355df07fa9d696fe6e61819cc0ea`  
		Last Modified: Tue, 13 Jun 2023 22:19:02 GMT  
		Size: 1.8 KB (1803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94f7788277dc1622146a19b5407e20fc8eb003cd62b331460221d930e9154d31`  
		Last Modified: Tue, 13 Jun 2023 22:19:02 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b991262b6e730687a02c0d68ac25bc2dcf4dff69f1e9db5315f654387aab754`  
		Last Modified: Tue, 13 Jun 2023 22:19:02 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c322d11690204cb63afb856a65f1fdd8016ebd23989de8952a6ecb7f6737f17e`  
		Last Modified: Tue, 13 Jun 2023 22:19:02 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-nanoserver-1809`

```console
$ docker pull nats@sha256:0a384e9a7d76bb1288a9b091976b9fa61e78c22143d6a07415707fdd6123219c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4377; amd64

### `nats:2-nanoserver-1809` - windows version 10.0.17763.4377; amd64

```console
$ docker pull nats@sha256:ffdbc972ae083180acdcc8d74756ed6c94b032bce6d7ec4c224f8343919f232d
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.6 MB (109564530 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b23b2cb10135235e109abd0ca99d3cf4027f72a1c246c873707190f54bffec4`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 05 May 2023 11:29:01 GMT
RUN Apply image 10.0.17763.4377
# Wed, 10 May 2023 02:43:57 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Tue, 13 Jun 2023 22:18:13 GMT
RUN cmd /S /C #(nop) COPY file:e92fb324fb1e715aaa4f213ef42afe80c4a76690e3b2d439bee510cb2ae47cd5 in C:\nats-server.exe 
# Tue, 13 Jun 2023 22:18:14 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Tue, 13 Jun 2023 22:18:15 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Tue, 13 Jun 2023 22:18:15 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 13 Jun 2023 22:18:16 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:f7885e3a2dfeae5eea125d00da688c29930a05e4d904884fe43e093ce6223664`  
		Last Modified: Wed, 10 May 2023 01:49:01 GMT  
		Size: 104.4 MB (104383998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9af27dd7e62b7d94fa31a7c9efd9a532c42db89ec01fdb7fe430043ceabc5b4`  
		Last Modified: Wed, 10 May 2023 02:49:27 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74147f1370eb575d5bc03ac650054b5dcc36d7b40bf7706dde9d9d159d10e1a8`  
		Last Modified: Tue, 13 Jun 2023 22:19:04 GMT  
		Size: 5.2 MB (5174125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c441087537bf6a2963fdc58d12d836350044355df07fa9d696fe6e61819cc0ea`  
		Last Modified: Tue, 13 Jun 2023 22:19:02 GMT  
		Size: 1.8 KB (1803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94f7788277dc1622146a19b5407e20fc8eb003cd62b331460221d930e9154d31`  
		Last Modified: Tue, 13 Jun 2023 22:19:02 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b991262b6e730687a02c0d68ac25bc2dcf4dff69f1e9db5315f654387aab754`  
		Last Modified: Tue, 13 Jun 2023 22:19:02 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c322d11690204cb63afb856a65f1fdd8016ebd23989de8952a6ecb7f6737f17e`  
		Last Modified: Tue, 13 Jun 2023 22:19:02 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-scratch`

```console
$ docker pull nats@sha256:451705c3735c55b4f7659f8690159fb8f4eb3138e0d4e1b921e4ae325fe46788
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-scratch` - linux; amd64

```console
$ docker pull nats@sha256:d7a57514cf7a0949ab8e63985f040f1fbaa01aa70aa50d8485f796a9a8dead08
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5117129 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4bd1a8b681814e86af7f1b07aa7178abd74163b5101ad1f855420c25d4afae5e`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 18 May 2023 21:19:59 GMT
COPY file:a3e4cfa40e3f87cbc1a2427fe9e77a182eed251b7a2f3037b894ac919acda56d in /nats-server 
# Thu, 18 May 2023 21:19:59 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 18 May 2023 21:19:59 GMT
EXPOSE 4222 6222 8222
# Thu, 18 May 2023 21:19:59 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 18 May 2023 21:19:59 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 18 May 2023 21:19:59 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:e7f86c5b152db9b1815749cb2d298d36014c2905070ae66128b67029b4b31780`  
		Last Modified: Thu, 18 May 2023 21:20:38 GMT  
		Size: 5.1 MB (5116621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:623ce2c40f365197112db5bf1e3ed9b09b631da2058b456f99a50a5890fdda44`  
		Last Modified: Thu, 18 May 2023 21:20:37 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:f26f23aad2feedaeaca9df38eca5559b431fbb8ed841789b1e6b2c3c84ffa79b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4884857 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8ae95e37599ef924cfe3d5890b3af209e09951179f6672d35af6811876e61253`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 13 Jun 2023 21:49:33 GMT
COPY file:e5bb5e8247a1c4bdb92d70dc84443f615728207816f4c76763893029e98fe987 in /nats-server 
# Tue, 13 Jun 2023 21:49:33 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 13 Jun 2023 21:49:33 GMT
EXPOSE 4222 6222 8222
# Tue, 13 Jun 2023 21:49:33 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 13 Jun 2023 21:49:33 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 13 Jun 2023 21:49:33 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:7f1a7a7f3e313c163918678d53d48af6476087e63070356ad38ff1c041606bca`  
		Last Modified: Tue, 13 Jun 2023 21:50:13 GMT  
		Size: 4.9 MB (4884348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9af05a149bcbd29ea7705539c8b49e2c00b5883848519f3929bf4c4dc424022e`  
		Last Modified: Tue, 13 Jun 2023 21:50:12 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:94bf4a62f52fd647adb621d2d584e9c48aea06b124fb81cd59afed50252071bd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4874864 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a8b8de1397d0af96648a1d02610dc54a066633c75eb548fc6be7e0d15497c3c`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 18 May 2023 21:57:50 GMT
COPY file:31e26234e2abf1c16cd5869033f07320118e6dc458af341f37a27a3d12ffbc65 in /nats-server 
# Thu, 18 May 2023 21:57:50 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 18 May 2023 21:57:51 GMT
EXPOSE 4222 6222 8222
# Thu, 18 May 2023 21:57:51 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 18 May 2023 21:57:51 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 18 May 2023 21:57:51 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b6209c6f59228d4816baef6c05a38f68693937e6c86969581c57a1c7b68ccb40`  
		Last Modified: Thu, 18 May 2023 21:58:28 GMT  
		Size: 4.9 MB (4874355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c69c5a4696da201d78c2dae749a6bce01c3a924afbdfa7e87c6797b8db238d4d`  
		Last Modified: Thu, 18 May 2023 21:58:27 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:edbf69c3a8dab18af6eefffc70fcea84205a4397632e23fbde4cca5fe03446ff
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4688025 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b395b40ae1ff951faa10f8f5c05810b77b0a03c2ef5a8eaa8bc443497b52348d`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 13 Jun 2023 22:34:13 GMT
COPY file:0fec8537fba7c573dbe20b854a6b32d8b0940e46f9e81c41611d447b82a034bc in /nats-server 
# Tue, 13 Jun 2023 22:34:13 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 13 Jun 2023 22:34:13 GMT
EXPOSE 4222 6222 8222
# Tue, 13 Jun 2023 22:34:14 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 13 Jun 2023 22:34:14 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 13 Jun 2023 22:34:14 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:2cce796fcd5a4e60d6ca871c71b29485d80a6babd1c43a056db0b52aa6e904b6`  
		Last Modified: Tue, 13 Jun 2023 22:34:58 GMT  
		Size: 4.7 MB (4687516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22153c0efa275cbe62c344213d16db73c5732467534b2a316e379bdd77324d29`  
		Last Modified: Tue, 13 Jun 2023 22:34:57 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-windowsservercore`

```console
$ docker pull nats@sha256:85d1368e7f6f675346e070014b558c792541dfc94c5bd2d9f919736ddaa90dee
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4377; amd64

### `nats:2-windowsservercore` - windows version 10.0.17763.4377; amd64

```console
$ docker pull nats@sha256:6116850a9313d0b910b0db095a33e7297f06b633f1e1fb386db4fd023e23985e
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2077962593 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d0359af1b68ffc80fd1b560b7235f9eb6d3562810001343595480a3f55a0e043`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Fri, 05 May 2023 12:05:28 GMT
RUN Install update 10.0.17763.4377
# Wed, 10 May 2023 01:56:29 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 May 2023 02:40:26 GMT
ENV NATS_DOCKERIZED=1
# Tue, 13 Jun 2023 22:15:14 GMT
ENV NATS_SERVER=2.9.18
# Tue, 13 Jun 2023 22:15:15 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.9.18/nats-server-v2.9.18-windows-amd64.zip
# Tue, 13 Jun 2023 22:15:16 GMT
ENV NATS_SERVER_SHASUM=139c2d63193d7df39894b144fb08a40e15548f89087e1932617239d36ab0c901
# Tue, 13 Jun 2023 22:16:20 GMT
RUN Set-PSDebug -Trace 2
# Tue, 13 Jun 2023 22:17:54 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Tue, 13 Jun 2023 22:17:54 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Tue, 13 Jun 2023 22:17:55 GMT
EXPOSE 4222 6222 8222
# Tue, 13 Jun 2023 22:17:56 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 13 Jun 2023 22:17:57 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e01de39a0c44e24aa1912078d32ee54389b71154e509138cc4f5d1de42e7a32a`  
		Last Modified: Wed, 10 May 2023 01:47:41 GMT  
		Size: 364.1 MB (364091294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2a89be60a77cd8d520ec5f03d703ddbc15675dd1df4d95e041032cf08960af5`  
		Last Modified: Wed, 10 May 2023 02:23:36 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:446cee93ab2781cfc08e135a3a7ab166e5342ee6817c34fb47e0662c085bbc29`  
		Last Modified: Wed, 10 May 2023 02:49:15 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a057529e52e0e6010038d1fe4fc95821b317ee7379ce74a6ccdaeb4397c6580`  
		Last Modified: Tue, 13 Jun 2023 22:18:48 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c741cf7b9012d8cb23e39f90427fded64f0e4de03039ddf48b77f15ef89d7ae0`  
		Last Modified: Tue, 13 Jun 2023 22:18:48 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:208c61957253b4017f86095081c6827718ad7b858e26d20a163e66ab10ed6a92`  
		Last Modified: Tue, 13 Jun 2023 22:18:48 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3e815afe033119fccd2887c2236ea581cbab8d6d5f4b146e2f03a35c99e150c`  
		Last Modified: Tue, 13 Jun 2023 22:18:48 GMT  
		Size: 448.8 KB (448805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c786064ca9923a9e7e6f5d6e0b3a08cb4c345cb8b37053a51ffe1ed92baa434f`  
		Last Modified: Tue, 13 Jun 2023 22:18:47 GMT  
		Size: 5.5 MB (5465263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ca1ecd70300344a64c5b09e7e0ef4325d7d434f3aee3b1d7845b33db7c8b8c6`  
		Last Modified: Tue, 13 Jun 2023 22:18:46 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8b2ae653f72ce5dc355f193098cdcdeb2cd780c78bed2991512625ead60fe16`  
		Last Modified: Tue, 13 Jun 2023 22:18:46 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d20c4caf3b063c53361edeec4547495178a5ee257f0afb5d83edb3a4d0b55bf`  
		Last Modified: Tue, 13 Jun 2023 22:18:46 GMT  
		Size: 1.4 KB (1374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6cf54e3a0a4a7d1916f3634aa394fdee5078f370ce0f19f05621468dbb0e6f4`  
		Last Modified: Tue, 13 Jun 2023 22:18:46 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-windowsservercore-1809`

```console
$ docker pull nats@sha256:85d1368e7f6f675346e070014b558c792541dfc94c5bd2d9f919736ddaa90dee
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4377; amd64

### `nats:2-windowsservercore-1809` - windows version 10.0.17763.4377; amd64

```console
$ docker pull nats@sha256:6116850a9313d0b910b0db095a33e7297f06b633f1e1fb386db4fd023e23985e
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2077962593 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d0359af1b68ffc80fd1b560b7235f9eb6d3562810001343595480a3f55a0e043`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Fri, 05 May 2023 12:05:28 GMT
RUN Install update 10.0.17763.4377
# Wed, 10 May 2023 01:56:29 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 May 2023 02:40:26 GMT
ENV NATS_DOCKERIZED=1
# Tue, 13 Jun 2023 22:15:14 GMT
ENV NATS_SERVER=2.9.18
# Tue, 13 Jun 2023 22:15:15 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.9.18/nats-server-v2.9.18-windows-amd64.zip
# Tue, 13 Jun 2023 22:15:16 GMT
ENV NATS_SERVER_SHASUM=139c2d63193d7df39894b144fb08a40e15548f89087e1932617239d36ab0c901
# Tue, 13 Jun 2023 22:16:20 GMT
RUN Set-PSDebug -Trace 2
# Tue, 13 Jun 2023 22:17:54 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Tue, 13 Jun 2023 22:17:54 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Tue, 13 Jun 2023 22:17:55 GMT
EXPOSE 4222 6222 8222
# Tue, 13 Jun 2023 22:17:56 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 13 Jun 2023 22:17:57 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e01de39a0c44e24aa1912078d32ee54389b71154e509138cc4f5d1de42e7a32a`  
		Last Modified: Wed, 10 May 2023 01:47:41 GMT  
		Size: 364.1 MB (364091294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2a89be60a77cd8d520ec5f03d703ddbc15675dd1df4d95e041032cf08960af5`  
		Last Modified: Wed, 10 May 2023 02:23:36 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:446cee93ab2781cfc08e135a3a7ab166e5342ee6817c34fb47e0662c085bbc29`  
		Last Modified: Wed, 10 May 2023 02:49:15 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a057529e52e0e6010038d1fe4fc95821b317ee7379ce74a6ccdaeb4397c6580`  
		Last Modified: Tue, 13 Jun 2023 22:18:48 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c741cf7b9012d8cb23e39f90427fded64f0e4de03039ddf48b77f15ef89d7ae0`  
		Last Modified: Tue, 13 Jun 2023 22:18:48 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:208c61957253b4017f86095081c6827718ad7b858e26d20a163e66ab10ed6a92`  
		Last Modified: Tue, 13 Jun 2023 22:18:48 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3e815afe033119fccd2887c2236ea581cbab8d6d5f4b146e2f03a35c99e150c`  
		Last Modified: Tue, 13 Jun 2023 22:18:48 GMT  
		Size: 448.8 KB (448805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c786064ca9923a9e7e6f5d6e0b3a08cb4c345cb8b37053a51ffe1ed92baa434f`  
		Last Modified: Tue, 13 Jun 2023 22:18:47 GMT  
		Size: 5.5 MB (5465263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ca1ecd70300344a64c5b09e7e0ef4325d7d434f3aee3b1d7845b33db7c8b8c6`  
		Last Modified: Tue, 13 Jun 2023 22:18:46 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8b2ae653f72ce5dc355f193098cdcdeb2cd780c78bed2991512625ead60fe16`  
		Last Modified: Tue, 13 Jun 2023 22:18:46 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d20c4caf3b063c53361edeec4547495178a5ee257f0afb5d83edb3a4d0b55bf`  
		Last Modified: Tue, 13 Jun 2023 22:18:46 GMT  
		Size: 1.4 KB (1374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6cf54e3a0a4a7d1916f3634aa394fdee5078f370ce0f19f05621468dbb0e6f4`  
		Last Modified: Tue, 13 Jun 2023 22:18:46 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9`

```console
$ docker pull nats@sha256:a600ddb07ea351ff9a7d0a49f7cc8fcd930c232d55f7c18f17378c3b4f7a83e7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.4377; amd64

### `nats:2.9` - linux; amd64

```console
$ docker pull nats@sha256:d7a57514cf7a0949ab8e63985f040f1fbaa01aa70aa50d8485f796a9a8dead08
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5117129 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4bd1a8b681814e86af7f1b07aa7178abd74163b5101ad1f855420c25d4afae5e`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 18 May 2023 21:19:59 GMT
COPY file:a3e4cfa40e3f87cbc1a2427fe9e77a182eed251b7a2f3037b894ac919acda56d in /nats-server 
# Thu, 18 May 2023 21:19:59 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 18 May 2023 21:19:59 GMT
EXPOSE 4222 6222 8222
# Thu, 18 May 2023 21:19:59 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 18 May 2023 21:19:59 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 18 May 2023 21:19:59 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:e7f86c5b152db9b1815749cb2d298d36014c2905070ae66128b67029b4b31780`  
		Last Modified: Thu, 18 May 2023 21:20:38 GMT  
		Size: 5.1 MB (5116621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:623ce2c40f365197112db5bf1e3ed9b09b631da2058b456f99a50a5890fdda44`  
		Last Modified: Thu, 18 May 2023 21:20:37 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9` - linux; arm variant v6

```console
$ docker pull nats@sha256:f26f23aad2feedaeaca9df38eca5559b431fbb8ed841789b1e6b2c3c84ffa79b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4884857 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8ae95e37599ef924cfe3d5890b3af209e09951179f6672d35af6811876e61253`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 13 Jun 2023 21:49:33 GMT
COPY file:e5bb5e8247a1c4bdb92d70dc84443f615728207816f4c76763893029e98fe987 in /nats-server 
# Tue, 13 Jun 2023 21:49:33 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 13 Jun 2023 21:49:33 GMT
EXPOSE 4222 6222 8222
# Tue, 13 Jun 2023 21:49:33 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 13 Jun 2023 21:49:33 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 13 Jun 2023 21:49:33 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:7f1a7a7f3e313c163918678d53d48af6476087e63070356ad38ff1c041606bca`  
		Last Modified: Tue, 13 Jun 2023 21:50:13 GMT  
		Size: 4.9 MB (4884348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9af05a149bcbd29ea7705539c8b49e2c00b5883848519f3929bf4c4dc424022e`  
		Last Modified: Tue, 13 Jun 2023 21:50:12 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9` - linux; arm variant v7

```console
$ docker pull nats@sha256:94bf4a62f52fd647adb621d2d584e9c48aea06b124fb81cd59afed50252071bd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4874864 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a8b8de1397d0af96648a1d02610dc54a066633c75eb548fc6be7e0d15497c3c`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 18 May 2023 21:57:50 GMT
COPY file:31e26234e2abf1c16cd5869033f07320118e6dc458af341f37a27a3d12ffbc65 in /nats-server 
# Thu, 18 May 2023 21:57:50 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 18 May 2023 21:57:51 GMT
EXPOSE 4222 6222 8222
# Thu, 18 May 2023 21:57:51 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 18 May 2023 21:57:51 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 18 May 2023 21:57:51 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b6209c6f59228d4816baef6c05a38f68693937e6c86969581c57a1c7b68ccb40`  
		Last Modified: Thu, 18 May 2023 21:58:28 GMT  
		Size: 4.9 MB (4874355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c69c5a4696da201d78c2dae749a6bce01c3a924afbdfa7e87c6797b8db238d4d`  
		Last Modified: Thu, 18 May 2023 21:58:27 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:edbf69c3a8dab18af6eefffc70fcea84205a4397632e23fbde4cca5fe03446ff
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4688025 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b395b40ae1ff951faa10f8f5c05810b77b0a03c2ef5a8eaa8bc443497b52348d`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 13 Jun 2023 22:34:13 GMT
COPY file:0fec8537fba7c573dbe20b854a6b32d8b0940e46f9e81c41611d447b82a034bc in /nats-server 
# Tue, 13 Jun 2023 22:34:13 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 13 Jun 2023 22:34:13 GMT
EXPOSE 4222 6222 8222
# Tue, 13 Jun 2023 22:34:14 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 13 Jun 2023 22:34:14 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 13 Jun 2023 22:34:14 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:2cce796fcd5a4e60d6ca871c71b29485d80a6babd1c43a056db0b52aa6e904b6`  
		Last Modified: Tue, 13 Jun 2023 22:34:58 GMT  
		Size: 4.7 MB (4687516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22153c0efa275cbe62c344213d16db73c5732467534b2a316e379bdd77324d29`  
		Last Modified: Tue, 13 Jun 2023 22:34:57 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9` - windows version 10.0.17763.4377; amd64

```console
$ docker pull nats@sha256:ffdbc972ae083180acdcc8d74756ed6c94b032bce6d7ec4c224f8343919f232d
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.6 MB (109564530 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b23b2cb10135235e109abd0ca99d3cf4027f72a1c246c873707190f54bffec4`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 05 May 2023 11:29:01 GMT
RUN Apply image 10.0.17763.4377
# Wed, 10 May 2023 02:43:57 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Tue, 13 Jun 2023 22:18:13 GMT
RUN cmd /S /C #(nop) COPY file:e92fb324fb1e715aaa4f213ef42afe80c4a76690e3b2d439bee510cb2ae47cd5 in C:\nats-server.exe 
# Tue, 13 Jun 2023 22:18:14 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Tue, 13 Jun 2023 22:18:15 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Tue, 13 Jun 2023 22:18:15 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 13 Jun 2023 22:18:16 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:f7885e3a2dfeae5eea125d00da688c29930a05e4d904884fe43e093ce6223664`  
		Last Modified: Wed, 10 May 2023 01:49:01 GMT  
		Size: 104.4 MB (104383998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9af27dd7e62b7d94fa31a7c9efd9a532c42db89ec01fdb7fe430043ceabc5b4`  
		Last Modified: Wed, 10 May 2023 02:49:27 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74147f1370eb575d5bc03ac650054b5dcc36d7b40bf7706dde9d9d159d10e1a8`  
		Last Modified: Tue, 13 Jun 2023 22:19:04 GMT  
		Size: 5.2 MB (5174125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c441087537bf6a2963fdc58d12d836350044355df07fa9d696fe6e61819cc0ea`  
		Last Modified: Tue, 13 Jun 2023 22:19:02 GMT  
		Size: 1.8 KB (1803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94f7788277dc1622146a19b5407e20fc8eb003cd62b331460221d930e9154d31`  
		Last Modified: Tue, 13 Jun 2023 22:19:02 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b991262b6e730687a02c0d68ac25bc2dcf4dff69f1e9db5315f654387aab754`  
		Last Modified: Tue, 13 Jun 2023 22:19:02 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c322d11690204cb63afb856a65f1fdd8016ebd23989de8952a6ecb7f6737f17e`  
		Last Modified: Tue, 13 Jun 2023 22:19:02 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-alpine`

```console
$ docker pull nats@sha256:d2647f1f7552973967b5b974d098c290c62dcf29eedfed515917ded32afe4a94
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9-alpine` - linux; amd64

```console
$ docker pull nats@sha256:7544f1dfe4b270789a68e2056135467d525da411f331f43640150b0642dee693
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.8 MB (8802768 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:04ada7bbdb360a5406551ced3593bc48e57c6cea5ee5d502e1a0df2437156d06`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 May 2023 23:11:10 GMT
ADD file:7625ddfd589fb824ee39f1b1eb387b98f3676420ff52f26eb9d975151e889667 in / 
# Tue, 09 May 2023 23:11:10 GMT
CMD ["/bin/sh"]
# Thu, 18 May 2023 21:19:49 GMT
ENV NATS_SERVER=2.9.17
# Thu, 18 May 2023 21:19:51 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='c7cf7bf8c029500d1b51773132ecc13a1fc89f2e080faa6b505da8cb95aa2a0c' ;; 		armhf) natsArch='arm6'; sha256='b09812858f1c957fd1869e21d4b8d64b3b0d6cdf3abb34502167120640f1d5e1' ;; 		armv7) natsArch='arm7'; sha256='970649306f45c78404c42dc5c0ab37fa6d5149501e47a68bef7841a06730a654' ;; 		x86_64) natsArch='amd64'; sha256='4ad2d83dd2fb9cc44a7e078d2e400f37c188b8515100f5de0f10f0eefbeb6b23' ;; 		x86) natsArch='386'; sha256='59c42f21bb6e8a5ef6e101ce6e3c29692b2cc9b1eb28465e67edeb391450626c' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 18 May 2023 21:19:52 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 18 May 2023 21:19:52 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 18 May 2023 21:19:52 GMT
EXPOSE 4222 6222 8222
# Thu, 18 May 2023 21:19:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 18 May 2023 21:19:52 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:8a49fdb3b6a5ff2bd8ec6a86c05b2922a0f7454579ecc07637e94dfd1d0639b6`  
		Last Modified: Tue, 09 May 2023 23:11:26 GMT  
		Size: 3.4 MB (3397490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ba69a821f226517d8763fd5007b51eeb8a68e40f7fb32dec75e13297ea1cb49`  
		Last Modified: Thu, 18 May 2023 21:20:19 GMT  
		Size: 5.4 MB (5404276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11ad2f9c9076c4ccedf3a056bf6e996a658fa5ece8cc35913e4728d58617e8b3`  
		Last Modified: Thu, 18 May 2023 21:20:18 GMT  
		Size: 588.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bb3c123b7bd114e7897ddf602c16bcd18f034abda3ee53d91a108b71c624faa`  
		Last Modified: Thu, 18 May 2023 21:20:18 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:957b9d5d12d8d9df6fea32822bd03a00b514635d8ede3f04c8fe3a2a0e8c436f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.3 MB (8326824 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9512db9e4ee16375a3bc31274c1b7a0480263800e5c7cfd91f794674b53e15a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 May 2023 23:11:04 GMT
ADD file:f87a991e2e9f185fd4a88569d86a9b8e5bc07182e7fa613b95acab25986f2a6c in / 
# Tue, 09 May 2023 23:11:04 GMT
CMD ["/bin/sh"]
# Tue, 13 Jun 2023 21:49:21 GMT
ENV NATS_SERVER=2.9.18
# Tue, 13 Jun 2023 21:49:24 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f5ea0ace65873cf81dde2951d9130f6ecad3f96e80a59badb259a66fc3294579' ;; 		armhf) natsArch='arm6'; sha256='f7dd549c09bac2adcc3260868bf5f182645c8e59e7b9cb868feff244017998b0' ;; 		armv7) natsArch='arm7'; sha256='bb1015887864e7eeeeb8bef4c9e06bd20d865b01a67bab8bab802ef5483bb6ad' ;; 		x86_64) natsArch='amd64'; sha256='c61c5dd662ed0836d752ed98508d5a7328d85e6126d2cf9784a0d546a64c961c' ;; 		x86) natsArch='386'; sha256='68467b7d83a96a554257b84464bdff34de956af93971e43faa711e1cb29249c8' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 13 Jun 2023 21:49:24 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 13 Jun 2023 21:49:24 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 13 Jun 2023 21:49:24 GMT
EXPOSE 4222 6222 8222
# Tue, 13 Jun 2023 21:49:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Jun 2023 21:49:25 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:015ee8d9fb3dca1b18815f1e4ee0d325d1f40cde6f2df4dd307918f7b69167d7`  
		Last Modified: Tue, 09 May 2023 23:11:20 GMT  
		Size: 3.2 MB (3155679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21a6505f5ff97d93b3e5451bb54fc64eea5680c617ce8cc7501394caf032f27f`  
		Last Modified: Tue, 13 Jun 2023 21:49:52 GMT  
		Size: 5.2 MB (5170145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43d0bff33a6560b8efd5c213b10cd3176703757ba35859a5ec499ca24abb1139`  
		Last Modified: Tue, 13 Jun 2023 21:49:51 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea53aff73c749d762e22ffbd5e9caecadeb064790877afe9c0b536284c9e4c59`  
		Last Modified: Tue, 13 Jun 2023 21:49:51 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:882066add3894dc13cfadaeec8af9f9fce5b9c3fee92e377a13f0997a88a121f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.1 MB (8071388 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:574536f22d8de67b2c2f0962d9e7d108bb4b41d07cb13a05ebab5e3b82fe6d63`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 May 2023 22:57:32 GMT
ADD file:eb6b6a885e8ac9bccbf44a5c673b8542c8144bba927376688240446c2f413b10 in / 
# Tue, 09 May 2023 22:57:32 GMT
CMD ["/bin/sh"]
# Thu, 18 May 2023 21:57:27 GMT
ENV NATS_SERVER=2.9.17
# Thu, 18 May 2023 21:57:29 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='c7cf7bf8c029500d1b51773132ecc13a1fc89f2e080faa6b505da8cb95aa2a0c' ;; 		armhf) natsArch='arm6'; sha256='b09812858f1c957fd1869e21d4b8d64b3b0d6cdf3abb34502167120640f1d5e1' ;; 		armv7) natsArch='arm7'; sha256='970649306f45c78404c42dc5c0ab37fa6d5149501e47a68bef7841a06730a654' ;; 		x86_64) natsArch='amd64'; sha256='4ad2d83dd2fb9cc44a7e078d2e400f37c188b8515100f5de0f10f0eefbeb6b23' ;; 		x86) natsArch='386'; sha256='59c42f21bb6e8a5ef6e101ce6e3c29692b2cc9b1eb28465e67edeb391450626c' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 18 May 2023 21:57:29 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 18 May 2023 21:57:29 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 18 May 2023 21:57:29 GMT
EXPOSE 4222 6222 8222
# Thu, 18 May 2023 21:57:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 18 May 2023 21:57:30 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:e14425cf8fb9304b9ad4a9d1250e0d4c22e507a334ff747fa69b804500afc113`  
		Last Modified: Tue, 09 May 2023 22:57:50 GMT  
		Size: 2.9 MB (2911117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:213de106e11b3e7261faf48da426167af8702e8a56ab0237f786ba0eb864a38d`  
		Last Modified: Thu, 18 May 2023 21:58:08 GMT  
		Size: 5.2 MB (5159272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5535f74851ba24bbb57849b9f7085eb8441d584ea938b19bdd027f5ccf52a193`  
		Last Modified: Thu, 18 May 2023 21:58:07 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2518eda2d1b2ce9ae4c75acdccc0d3bbe028cfbdf30d7e173dfa82e489af6ec`  
		Last Modified: Thu, 18 May 2023 21:58:08 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:ce87b1ebec8a22151ac8ae437db42293e4293bfecd5045752d86f661b0547b26
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.3 MB (8315499 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bdbca1cbb72621a6502190ab58418aee769fffb9d66712c9ea805d56d3fb46fc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 May 2023 23:11:08 GMT
ADD file:df7fccc3453b6ec1401d27a1295b0882a83e731fde8f23db9d3f687a2b6b4e70 in / 
# Tue, 09 May 2023 23:11:08 GMT
CMD ["/bin/sh"]
# Tue, 13 Jun 2023 22:33:21 GMT
ENV NATS_SERVER=2.9.18
# Tue, 13 Jun 2023 22:33:23 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f5ea0ace65873cf81dde2951d9130f6ecad3f96e80a59badb259a66fc3294579' ;; 		armhf) natsArch='arm6'; sha256='f7dd549c09bac2adcc3260868bf5f182645c8e59e7b9cb868feff244017998b0' ;; 		armv7) natsArch='arm7'; sha256='bb1015887864e7eeeeb8bef4c9e06bd20d865b01a67bab8bab802ef5483bb6ad' ;; 		x86_64) natsArch='amd64'; sha256='c61c5dd662ed0836d752ed98508d5a7328d85e6126d2cf9784a0d546a64c961c' ;; 		x86) natsArch='386'; sha256='68467b7d83a96a554257b84464bdff34de956af93971e43faa711e1cb29249c8' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 13 Jun 2023 22:33:23 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 13 Jun 2023 22:33:23 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 13 Jun 2023 22:33:23 GMT
EXPOSE 4222 6222 8222
# Tue, 13 Jun 2023 22:33:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Jun 2023 22:33:23 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:08409d4172603f40b56eb6b76240a1e6bd78baa0e96590dc7ff76c5f1a093af2`  
		Last Modified: Tue, 09 May 2023 23:11:23 GMT  
		Size: 3.3 MB (3342848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf2d0fd688338eb8ef69b776354053dd65c78ae5e4c3cc2e15fc586f51942d89`  
		Last Modified: Tue, 13 Jun 2023 22:34:38 GMT  
		Size: 5.0 MB (4971650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee9d7fff35b08386d1a65e0e1fa0a81bcc5877d1024bd16ca00f0af62137cdc4`  
		Last Modified: Tue, 13 Jun 2023 22:34:37 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63543f616abdbde1673d999e8e046e0f59aa734ab23d6acabdf42a9756f8c357`  
		Last Modified: Tue, 13 Jun 2023 22:34:37 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-alpine3.18`

```console
$ docker pull nats@sha256:d2647f1f7552973967b5b974d098c290c62dcf29eedfed515917ded32afe4a94
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9-alpine3.18` - linux; amd64

```console
$ docker pull nats@sha256:7544f1dfe4b270789a68e2056135467d525da411f331f43640150b0642dee693
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.8 MB (8802768 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:04ada7bbdb360a5406551ced3593bc48e57c6cea5ee5d502e1a0df2437156d06`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 May 2023 23:11:10 GMT
ADD file:7625ddfd589fb824ee39f1b1eb387b98f3676420ff52f26eb9d975151e889667 in / 
# Tue, 09 May 2023 23:11:10 GMT
CMD ["/bin/sh"]
# Thu, 18 May 2023 21:19:49 GMT
ENV NATS_SERVER=2.9.17
# Thu, 18 May 2023 21:19:51 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='c7cf7bf8c029500d1b51773132ecc13a1fc89f2e080faa6b505da8cb95aa2a0c' ;; 		armhf) natsArch='arm6'; sha256='b09812858f1c957fd1869e21d4b8d64b3b0d6cdf3abb34502167120640f1d5e1' ;; 		armv7) natsArch='arm7'; sha256='970649306f45c78404c42dc5c0ab37fa6d5149501e47a68bef7841a06730a654' ;; 		x86_64) natsArch='amd64'; sha256='4ad2d83dd2fb9cc44a7e078d2e400f37c188b8515100f5de0f10f0eefbeb6b23' ;; 		x86) natsArch='386'; sha256='59c42f21bb6e8a5ef6e101ce6e3c29692b2cc9b1eb28465e67edeb391450626c' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 18 May 2023 21:19:52 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 18 May 2023 21:19:52 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 18 May 2023 21:19:52 GMT
EXPOSE 4222 6222 8222
# Thu, 18 May 2023 21:19:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 18 May 2023 21:19:52 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:8a49fdb3b6a5ff2bd8ec6a86c05b2922a0f7454579ecc07637e94dfd1d0639b6`  
		Last Modified: Tue, 09 May 2023 23:11:26 GMT  
		Size: 3.4 MB (3397490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ba69a821f226517d8763fd5007b51eeb8a68e40f7fb32dec75e13297ea1cb49`  
		Last Modified: Thu, 18 May 2023 21:20:19 GMT  
		Size: 5.4 MB (5404276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11ad2f9c9076c4ccedf3a056bf6e996a658fa5ece8cc35913e4728d58617e8b3`  
		Last Modified: Thu, 18 May 2023 21:20:18 GMT  
		Size: 588.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bb3c123b7bd114e7897ddf602c16bcd18f034abda3ee53d91a108b71c624faa`  
		Last Modified: Thu, 18 May 2023 21:20:18 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-alpine3.18` - linux; arm variant v6

```console
$ docker pull nats@sha256:957b9d5d12d8d9df6fea32822bd03a00b514635d8ede3f04c8fe3a2a0e8c436f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.3 MB (8326824 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9512db9e4ee16375a3bc31274c1b7a0480263800e5c7cfd91f794674b53e15a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 May 2023 23:11:04 GMT
ADD file:f87a991e2e9f185fd4a88569d86a9b8e5bc07182e7fa613b95acab25986f2a6c in / 
# Tue, 09 May 2023 23:11:04 GMT
CMD ["/bin/sh"]
# Tue, 13 Jun 2023 21:49:21 GMT
ENV NATS_SERVER=2.9.18
# Tue, 13 Jun 2023 21:49:24 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f5ea0ace65873cf81dde2951d9130f6ecad3f96e80a59badb259a66fc3294579' ;; 		armhf) natsArch='arm6'; sha256='f7dd549c09bac2adcc3260868bf5f182645c8e59e7b9cb868feff244017998b0' ;; 		armv7) natsArch='arm7'; sha256='bb1015887864e7eeeeb8bef4c9e06bd20d865b01a67bab8bab802ef5483bb6ad' ;; 		x86_64) natsArch='amd64'; sha256='c61c5dd662ed0836d752ed98508d5a7328d85e6126d2cf9784a0d546a64c961c' ;; 		x86) natsArch='386'; sha256='68467b7d83a96a554257b84464bdff34de956af93971e43faa711e1cb29249c8' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 13 Jun 2023 21:49:24 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 13 Jun 2023 21:49:24 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 13 Jun 2023 21:49:24 GMT
EXPOSE 4222 6222 8222
# Tue, 13 Jun 2023 21:49:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Jun 2023 21:49:25 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:015ee8d9fb3dca1b18815f1e4ee0d325d1f40cde6f2df4dd307918f7b69167d7`  
		Last Modified: Tue, 09 May 2023 23:11:20 GMT  
		Size: 3.2 MB (3155679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21a6505f5ff97d93b3e5451bb54fc64eea5680c617ce8cc7501394caf032f27f`  
		Last Modified: Tue, 13 Jun 2023 21:49:52 GMT  
		Size: 5.2 MB (5170145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43d0bff33a6560b8efd5c213b10cd3176703757ba35859a5ec499ca24abb1139`  
		Last Modified: Tue, 13 Jun 2023 21:49:51 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea53aff73c749d762e22ffbd5e9caecadeb064790877afe9c0b536284c9e4c59`  
		Last Modified: Tue, 13 Jun 2023 21:49:51 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-alpine3.18` - linux; arm variant v7

```console
$ docker pull nats@sha256:882066add3894dc13cfadaeec8af9f9fce5b9c3fee92e377a13f0997a88a121f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.1 MB (8071388 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:574536f22d8de67b2c2f0962d9e7d108bb4b41d07cb13a05ebab5e3b82fe6d63`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 May 2023 22:57:32 GMT
ADD file:eb6b6a885e8ac9bccbf44a5c673b8542c8144bba927376688240446c2f413b10 in / 
# Tue, 09 May 2023 22:57:32 GMT
CMD ["/bin/sh"]
# Thu, 18 May 2023 21:57:27 GMT
ENV NATS_SERVER=2.9.17
# Thu, 18 May 2023 21:57:29 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='c7cf7bf8c029500d1b51773132ecc13a1fc89f2e080faa6b505da8cb95aa2a0c' ;; 		armhf) natsArch='arm6'; sha256='b09812858f1c957fd1869e21d4b8d64b3b0d6cdf3abb34502167120640f1d5e1' ;; 		armv7) natsArch='arm7'; sha256='970649306f45c78404c42dc5c0ab37fa6d5149501e47a68bef7841a06730a654' ;; 		x86_64) natsArch='amd64'; sha256='4ad2d83dd2fb9cc44a7e078d2e400f37c188b8515100f5de0f10f0eefbeb6b23' ;; 		x86) natsArch='386'; sha256='59c42f21bb6e8a5ef6e101ce6e3c29692b2cc9b1eb28465e67edeb391450626c' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 18 May 2023 21:57:29 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 18 May 2023 21:57:29 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 18 May 2023 21:57:29 GMT
EXPOSE 4222 6222 8222
# Thu, 18 May 2023 21:57:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 18 May 2023 21:57:30 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:e14425cf8fb9304b9ad4a9d1250e0d4c22e507a334ff747fa69b804500afc113`  
		Last Modified: Tue, 09 May 2023 22:57:50 GMT  
		Size: 2.9 MB (2911117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:213de106e11b3e7261faf48da426167af8702e8a56ab0237f786ba0eb864a38d`  
		Last Modified: Thu, 18 May 2023 21:58:08 GMT  
		Size: 5.2 MB (5159272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5535f74851ba24bbb57849b9f7085eb8441d584ea938b19bdd027f5ccf52a193`  
		Last Modified: Thu, 18 May 2023 21:58:07 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2518eda2d1b2ce9ae4c75acdccc0d3bbe028cfbdf30d7e173dfa82e489af6ec`  
		Last Modified: Thu, 18 May 2023 21:58:08 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-alpine3.18` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:ce87b1ebec8a22151ac8ae437db42293e4293bfecd5045752d86f661b0547b26
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.3 MB (8315499 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bdbca1cbb72621a6502190ab58418aee769fffb9d66712c9ea805d56d3fb46fc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 May 2023 23:11:08 GMT
ADD file:df7fccc3453b6ec1401d27a1295b0882a83e731fde8f23db9d3f687a2b6b4e70 in / 
# Tue, 09 May 2023 23:11:08 GMT
CMD ["/bin/sh"]
# Tue, 13 Jun 2023 22:33:21 GMT
ENV NATS_SERVER=2.9.18
# Tue, 13 Jun 2023 22:33:23 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f5ea0ace65873cf81dde2951d9130f6ecad3f96e80a59badb259a66fc3294579' ;; 		armhf) natsArch='arm6'; sha256='f7dd549c09bac2adcc3260868bf5f182645c8e59e7b9cb868feff244017998b0' ;; 		armv7) natsArch='arm7'; sha256='bb1015887864e7eeeeb8bef4c9e06bd20d865b01a67bab8bab802ef5483bb6ad' ;; 		x86_64) natsArch='amd64'; sha256='c61c5dd662ed0836d752ed98508d5a7328d85e6126d2cf9784a0d546a64c961c' ;; 		x86) natsArch='386'; sha256='68467b7d83a96a554257b84464bdff34de956af93971e43faa711e1cb29249c8' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 13 Jun 2023 22:33:23 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 13 Jun 2023 22:33:23 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 13 Jun 2023 22:33:23 GMT
EXPOSE 4222 6222 8222
# Tue, 13 Jun 2023 22:33:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Jun 2023 22:33:23 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:08409d4172603f40b56eb6b76240a1e6bd78baa0e96590dc7ff76c5f1a093af2`  
		Last Modified: Tue, 09 May 2023 23:11:23 GMT  
		Size: 3.3 MB (3342848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf2d0fd688338eb8ef69b776354053dd65c78ae5e4c3cc2e15fc586f51942d89`  
		Last Modified: Tue, 13 Jun 2023 22:34:38 GMT  
		Size: 5.0 MB (4971650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee9d7fff35b08386d1a65e0e1fa0a81bcc5877d1024bd16ca00f0af62137cdc4`  
		Last Modified: Tue, 13 Jun 2023 22:34:37 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63543f616abdbde1673d999e8e046e0f59aa734ab23d6acabdf42a9756f8c357`  
		Last Modified: Tue, 13 Jun 2023 22:34:37 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-linux`

```console
$ docker pull nats@sha256:451705c3735c55b4f7659f8690159fb8f4eb3138e0d4e1b921e4ae325fe46788
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9-linux` - linux; amd64

```console
$ docker pull nats@sha256:d7a57514cf7a0949ab8e63985f040f1fbaa01aa70aa50d8485f796a9a8dead08
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5117129 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4bd1a8b681814e86af7f1b07aa7178abd74163b5101ad1f855420c25d4afae5e`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 18 May 2023 21:19:59 GMT
COPY file:a3e4cfa40e3f87cbc1a2427fe9e77a182eed251b7a2f3037b894ac919acda56d in /nats-server 
# Thu, 18 May 2023 21:19:59 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 18 May 2023 21:19:59 GMT
EXPOSE 4222 6222 8222
# Thu, 18 May 2023 21:19:59 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 18 May 2023 21:19:59 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 18 May 2023 21:19:59 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:e7f86c5b152db9b1815749cb2d298d36014c2905070ae66128b67029b4b31780`  
		Last Modified: Thu, 18 May 2023 21:20:38 GMT  
		Size: 5.1 MB (5116621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:623ce2c40f365197112db5bf1e3ed9b09b631da2058b456f99a50a5890fdda44`  
		Last Modified: Thu, 18 May 2023 21:20:37 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:f26f23aad2feedaeaca9df38eca5559b431fbb8ed841789b1e6b2c3c84ffa79b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4884857 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8ae95e37599ef924cfe3d5890b3af209e09951179f6672d35af6811876e61253`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 13 Jun 2023 21:49:33 GMT
COPY file:e5bb5e8247a1c4bdb92d70dc84443f615728207816f4c76763893029e98fe987 in /nats-server 
# Tue, 13 Jun 2023 21:49:33 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 13 Jun 2023 21:49:33 GMT
EXPOSE 4222 6222 8222
# Tue, 13 Jun 2023 21:49:33 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 13 Jun 2023 21:49:33 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 13 Jun 2023 21:49:33 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:7f1a7a7f3e313c163918678d53d48af6476087e63070356ad38ff1c041606bca`  
		Last Modified: Tue, 13 Jun 2023 21:50:13 GMT  
		Size: 4.9 MB (4884348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9af05a149bcbd29ea7705539c8b49e2c00b5883848519f3929bf4c4dc424022e`  
		Last Modified: Tue, 13 Jun 2023 21:50:12 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:94bf4a62f52fd647adb621d2d584e9c48aea06b124fb81cd59afed50252071bd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4874864 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a8b8de1397d0af96648a1d02610dc54a066633c75eb548fc6be7e0d15497c3c`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 18 May 2023 21:57:50 GMT
COPY file:31e26234e2abf1c16cd5869033f07320118e6dc458af341f37a27a3d12ffbc65 in /nats-server 
# Thu, 18 May 2023 21:57:50 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 18 May 2023 21:57:51 GMT
EXPOSE 4222 6222 8222
# Thu, 18 May 2023 21:57:51 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 18 May 2023 21:57:51 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 18 May 2023 21:57:51 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b6209c6f59228d4816baef6c05a38f68693937e6c86969581c57a1c7b68ccb40`  
		Last Modified: Thu, 18 May 2023 21:58:28 GMT  
		Size: 4.9 MB (4874355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c69c5a4696da201d78c2dae749a6bce01c3a924afbdfa7e87c6797b8db238d4d`  
		Last Modified: Thu, 18 May 2023 21:58:27 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:edbf69c3a8dab18af6eefffc70fcea84205a4397632e23fbde4cca5fe03446ff
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4688025 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b395b40ae1ff951faa10f8f5c05810b77b0a03c2ef5a8eaa8bc443497b52348d`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 13 Jun 2023 22:34:13 GMT
COPY file:0fec8537fba7c573dbe20b854a6b32d8b0940e46f9e81c41611d447b82a034bc in /nats-server 
# Tue, 13 Jun 2023 22:34:13 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 13 Jun 2023 22:34:13 GMT
EXPOSE 4222 6222 8222
# Tue, 13 Jun 2023 22:34:14 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 13 Jun 2023 22:34:14 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 13 Jun 2023 22:34:14 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:2cce796fcd5a4e60d6ca871c71b29485d80a6babd1c43a056db0b52aa6e904b6`  
		Last Modified: Tue, 13 Jun 2023 22:34:58 GMT  
		Size: 4.7 MB (4687516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22153c0efa275cbe62c344213d16db73c5732467534b2a316e379bdd77324d29`  
		Last Modified: Tue, 13 Jun 2023 22:34:57 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-nanoserver`

```console
$ docker pull nats@sha256:0a384e9a7d76bb1288a9b091976b9fa61e78c22143d6a07415707fdd6123219c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4377; amd64

### `nats:2.9-nanoserver` - windows version 10.0.17763.4377; amd64

```console
$ docker pull nats@sha256:ffdbc972ae083180acdcc8d74756ed6c94b032bce6d7ec4c224f8343919f232d
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.6 MB (109564530 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b23b2cb10135235e109abd0ca99d3cf4027f72a1c246c873707190f54bffec4`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 05 May 2023 11:29:01 GMT
RUN Apply image 10.0.17763.4377
# Wed, 10 May 2023 02:43:57 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Tue, 13 Jun 2023 22:18:13 GMT
RUN cmd /S /C #(nop) COPY file:e92fb324fb1e715aaa4f213ef42afe80c4a76690e3b2d439bee510cb2ae47cd5 in C:\nats-server.exe 
# Tue, 13 Jun 2023 22:18:14 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Tue, 13 Jun 2023 22:18:15 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Tue, 13 Jun 2023 22:18:15 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 13 Jun 2023 22:18:16 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:f7885e3a2dfeae5eea125d00da688c29930a05e4d904884fe43e093ce6223664`  
		Last Modified: Wed, 10 May 2023 01:49:01 GMT  
		Size: 104.4 MB (104383998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9af27dd7e62b7d94fa31a7c9efd9a532c42db89ec01fdb7fe430043ceabc5b4`  
		Last Modified: Wed, 10 May 2023 02:49:27 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74147f1370eb575d5bc03ac650054b5dcc36d7b40bf7706dde9d9d159d10e1a8`  
		Last Modified: Tue, 13 Jun 2023 22:19:04 GMT  
		Size: 5.2 MB (5174125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c441087537bf6a2963fdc58d12d836350044355df07fa9d696fe6e61819cc0ea`  
		Last Modified: Tue, 13 Jun 2023 22:19:02 GMT  
		Size: 1.8 KB (1803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94f7788277dc1622146a19b5407e20fc8eb003cd62b331460221d930e9154d31`  
		Last Modified: Tue, 13 Jun 2023 22:19:02 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b991262b6e730687a02c0d68ac25bc2dcf4dff69f1e9db5315f654387aab754`  
		Last Modified: Tue, 13 Jun 2023 22:19:02 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c322d11690204cb63afb856a65f1fdd8016ebd23989de8952a6ecb7f6737f17e`  
		Last Modified: Tue, 13 Jun 2023 22:19:02 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-nanoserver-1809`

```console
$ docker pull nats@sha256:0a384e9a7d76bb1288a9b091976b9fa61e78c22143d6a07415707fdd6123219c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4377; amd64

### `nats:2.9-nanoserver-1809` - windows version 10.0.17763.4377; amd64

```console
$ docker pull nats@sha256:ffdbc972ae083180acdcc8d74756ed6c94b032bce6d7ec4c224f8343919f232d
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.6 MB (109564530 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b23b2cb10135235e109abd0ca99d3cf4027f72a1c246c873707190f54bffec4`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 05 May 2023 11:29:01 GMT
RUN Apply image 10.0.17763.4377
# Wed, 10 May 2023 02:43:57 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Tue, 13 Jun 2023 22:18:13 GMT
RUN cmd /S /C #(nop) COPY file:e92fb324fb1e715aaa4f213ef42afe80c4a76690e3b2d439bee510cb2ae47cd5 in C:\nats-server.exe 
# Tue, 13 Jun 2023 22:18:14 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Tue, 13 Jun 2023 22:18:15 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Tue, 13 Jun 2023 22:18:15 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 13 Jun 2023 22:18:16 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:f7885e3a2dfeae5eea125d00da688c29930a05e4d904884fe43e093ce6223664`  
		Last Modified: Wed, 10 May 2023 01:49:01 GMT  
		Size: 104.4 MB (104383998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9af27dd7e62b7d94fa31a7c9efd9a532c42db89ec01fdb7fe430043ceabc5b4`  
		Last Modified: Wed, 10 May 2023 02:49:27 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74147f1370eb575d5bc03ac650054b5dcc36d7b40bf7706dde9d9d159d10e1a8`  
		Last Modified: Tue, 13 Jun 2023 22:19:04 GMT  
		Size: 5.2 MB (5174125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c441087537bf6a2963fdc58d12d836350044355df07fa9d696fe6e61819cc0ea`  
		Last Modified: Tue, 13 Jun 2023 22:19:02 GMT  
		Size: 1.8 KB (1803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94f7788277dc1622146a19b5407e20fc8eb003cd62b331460221d930e9154d31`  
		Last Modified: Tue, 13 Jun 2023 22:19:02 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b991262b6e730687a02c0d68ac25bc2dcf4dff69f1e9db5315f654387aab754`  
		Last Modified: Tue, 13 Jun 2023 22:19:02 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c322d11690204cb63afb856a65f1fdd8016ebd23989de8952a6ecb7f6737f17e`  
		Last Modified: Tue, 13 Jun 2023 22:19:02 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-scratch`

```console
$ docker pull nats@sha256:451705c3735c55b4f7659f8690159fb8f4eb3138e0d4e1b921e4ae325fe46788
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9-scratch` - linux; amd64

```console
$ docker pull nats@sha256:d7a57514cf7a0949ab8e63985f040f1fbaa01aa70aa50d8485f796a9a8dead08
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5117129 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4bd1a8b681814e86af7f1b07aa7178abd74163b5101ad1f855420c25d4afae5e`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 18 May 2023 21:19:59 GMT
COPY file:a3e4cfa40e3f87cbc1a2427fe9e77a182eed251b7a2f3037b894ac919acda56d in /nats-server 
# Thu, 18 May 2023 21:19:59 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 18 May 2023 21:19:59 GMT
EXPOSE 4222 6222 8222
# Thu, 18 May 2023 21:19:59 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 18 May 2023 21:19:59 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 18 May 2023 21:19:59 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:e7f86c5b152db9b1815749cb2d298d36014c2905070ae66128b67029b4b31780`  
		Last Modified: Thu, 18 May 2023 21:20:38 GMT  
		Size: 5.1 MB (5116621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:623ce2c40f365197112db5bf1e3ed9b09b631da2058b456f99a50a5890fdda44`  
		Last Modified: Thu, 18 May 2023 21:20:37 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:f26f23aad2feedaeaca9df38eca5559b431fbb8ed841789b1e6b2c3c84ffa79b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4884857 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8ae95e37599ef924cfe3d5890b3af209e09951179f6672d35af6811876e61253`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 13 Jun 2023 21:49:33 GMT
COPY file:e5bb5e8247a1c4bdb92d70dc84443f615728207816f4c76763893029e98fe987 in /nats-server 
# Tue, 13 Jun 2023 21:49:33 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 13 Jun 2023 21:49:33 GMT
EXPOSE 4222 6222 8222
# Tue, 13 Jun 2023 21:49:33 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 13 Jun 2023 21:49:33 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 13 Jun 2023 21:49:33 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:7f1a7a7f3e313c163918678d53d48af6476087e63070356ad38ff1c041606bca`  
		Last Modified: Tue, 13 Jun 2023 21:50:13 GMT  
		Size: 4.9 MB (4884348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9af05a149bcbd29ea7705539c8b49e2c00b5883848519f3929bf4c4dc424022e`  
		Last Modified: Tue, 13 Jun 2023 21:50:12 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:94bf4a62f52fd647adb621d2d584e9c48aea06b124fb81cd59afed50252071bd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4874864 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a8b8de1397d0af96648a1d02610dc54a066633c75eb548fc6be7e0d15497c3c`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 18 May 2023 21:57:50 GMT
COPY file:31e26234e2abf1c16cd5869033f07320118e6dc458af341f37a27a3d12ffbc65 in /nats-server 
# Thu, 18 May 2023 21:57:50 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 18 May 2023 21:57:51 GMT
EXPOSE 4222 6222 8222
# Thu, 18 May 2023 21:57:51 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 18 May 2023 21:57:51 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 18 May 2023 21:57:51 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b6209c6f59228d4816baef6c05a38f68693937e6c86969581c57a1c7b68ccb40`  
		Last Modified: Thu, 18 May 2023 21:58:28 GMT  
		Size: 4.9 MB (4874355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c69c5a4696da201d78c2dae749a6bce01c3a924afbdfa7e87c6797b8db238d4d`  
		Last Modified: Thu, 18 May 2023 21:58:27 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:edbf69c3a8dab18af6eefffc70fcea84205a4397632e23fbde4cca5fe03446ff
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4688025 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b395b40ae1ff951faa10f8f5c05810b77b0a03c2ef5a8eaa8bc443497b52348d`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 13 Jun 2023 22:34:13 GMT
COPY file:0fec8537fba7c573dbe20b854a6b32d8b0940e46f9e81c41611d447b82a034bc in /nats-server 
# Tue, 13 Jun 2023 22:34:13 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 13 Jun 2023 22:34:13 GMT
EXPOSE 4222 6222 8222
# Tue, 13 Jun 2023 22:34:14 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 13 Jun 2023 22:34:14 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 13 Jun 2023 22:34:14 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:2cce796fcd5a4e60d6ca871c71b29485d80a6babd1c43a056db0b52aa6e904b6`  
		Last Modified: Tue, 13 Jun 2023 22:34:58 GMT  
		Size: 4.7 MB (4687516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22153c0efa275cbe62c344213d16db73c5732467534b2a316e379bdd77324d29`  
		Last Modified: Tue, 13 Jun 2023 22:34:57 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-windowsservercore`

```console
$ docker pull nats@sha256:85d1368e7f6f675346e070014b558c792541dfc94c5bd2d9f919736ddaa90dee
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4377; amd64

### `nats:2.9-windowsservercore` - windows version 10.0.17763.4377; amd64

```console
$ docker pull nats@sha256:6116850a9313d0b910b0db095a33e7297f06b633f1e1fb386db4fd023e23985e
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2077962593 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d0359af1b68ffc80fd1b560b7235f9eb6d3562810001343595480a3f55a0e043`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Fri, 05 May 2023 12:05:28 GMT
RUN Install update 10.0.17763.4377
# Wed, 10 May 2023 01:56:29 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 May 2023 02:40:26 GMT
ENV NATS_DOCKERIZED=1
# Tue, 13 Jun 2023 22:15:14 GMT
ENV NATS_SERVER=2.9.18
# Tue, 13 Jun 2023 22:15:15 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.9.18/nats-server-v2.9.18-windows-amd64.zip
# Tue, 13 Jun 2023 22:15:16 GMT
ENV NATS_SERVER_SHASUM=139c2d63193d7df39894b144fb08a40e15548f89087e1932617239d36ab0c901
# Tue, 13 Jun 2023 22:16:20 GMT
RUN Set-PSDebug -Trace 2
# Tue, 13 Jun 2023 22:17:54 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Tue, 13 Jun 2023 22:17:54 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Tue, 13 Jun 2023 22:17:55 GMT
EXPOSE 4222 6222 8222
# Tue, 13 Jun 2023 22:17:56 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 13 Jun 2023 22:17:57 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e01de39a0c44e24aa1912078d32ee54389b71154e509138cc4f5d1de42e7a32a`  
		Last Modified: Wed, 10 May 2023 01:47:41 GMT  
		Size: 364.1 MB (364091294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2a89be60a77cd8d520ec5f03d703ddbc15675dd1df4d95e041032cf08960af5`  
		Last Modified: Wed, 10 May 2023 02:23:36 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:446cee93ab2781cfc08e135a3a7ab166e5342ee6817c34fb47e0662c085bbc29`  
		Last Modified: Wed, 10 May 2023 02:49:15 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a057529e52e0e6010038d1fe4fc95821b317ee7379ce74a6ccdaeb4397c6580`  
		Last Modified: Tue, 13 Jun 2023 22:18:48 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c741cf7b9012d8cb23e39f90427fded64f0e4de03039ddf48b77f15ef89d7ae0`  
		Last Modified: Tue, 13 Jun 2023 22:18:48 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:208c61957253b4017f86095081c6827718ad7b858e26d20a163e66ab10ed6a92`  
		Last Modified: Tue, 13 Jun 2023 22:18:48 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3e815afe033119fccd2887c2236ea581cbab8d6d5f4b146e2f03a35c99e150c`  
		Last Modified: Tue, 13 Jun 2023 22:18:48 GMT  
		Size: 448.8 KB (448805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c786064ca9923a9e7e6f5d6e0b3a08cb4c345cb8b37053a51ffe1ed92baa434f`  
		Last Modified: Tue, 13 Jun 2023 22:18:47 GMT  
		Size: 5.5 MB (5465263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ca1ecd70300344a64c5b09e7e0ef4325d7d434f3aee3b1d7845b33db7c8b8c6`  
		Last Modified: Tue, 13 Jun 2023 22:18:46 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8b2ae653f72ce5dc355f193098cdcdeb2cd780c78bed2991512625ead60fe16`  
		Last Modified: Tue, 13 Jun 2023 22:18:46 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d20c4caf3b063c53361edeec4547495178a5ee257f0afb5d83edb3a4d0b55bf`  
		Last Modified: Tue, 13 Jun 2023 22:18:46 GMT  
		Size: 1.4 KB (1374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6cf54e3a0a4a7d1916f3634aa394fdee5078f370ce0f19f05621468dbb0e6f4`  
		Last Modified: Tue, 13 Jun 2023 22:18:46 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-windowsservercore-1809`

```console
$ docker pull nats@sha256:85d1368e7f6f675346e070014b558c792541dfc94c5bd2d9f919736ddaa90dee
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4377; amd64

### `nats:2.9-windowsservercore-1809` - windows version 10.0.17763.4377; amd64

```console
$ docker pull nats@sha256:6116850a9313d0b910b0db095a33e7297f06b633f1e1fb386db4fd023e23985e
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2077962593 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d0359af1b68ffc80fd1b560b7235f9eb6d3562810001343595480a3f55a0e043`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Fri, 05 May 2023 12:05:28 GMT
RUN Install update 10.0.17763.4377
# Wed, 10 May 2023 01:56:29 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 May 2023 02:40:26 GMT
ENV NATS_DOCKERIZED=1
# Tue, 13 Jun 2023 22:15:14 GMT
ENV NATS_SERVER=2.9.18
# Tue, 13 Jun 2023 22:15:15 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.9.18/nats-server-v2.9.18-windows-amd64.zip
# Tue, 13 Jun 2023 22:15:16 GMT
ENV NATS_SERVER_SHASUM=139c2d63193d7df39894b144fb08a40e15548f89087e1932617239d36ab0c901
# Tue, 13 Jun 2023 22:16:20 GMT
RUN Set-PSDebug -Trace 2
# Tue, 13 Jun 2023 22:17:54 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Tue, 13 Jun 2023 22:17:54 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Tue, 13 Jun 2023 22:17:55 GMT
EXPOSE 4222 6222 8222
# Tue, 13 Jun 2023 22:17:56 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 13 Jun 2023 22:17:57 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e01de39a0c44e24aa1912078d32ee54389b71154e509138cc4f5d1de42e7a32a`  
		Last Modified: Wed, 10 May 2023 01:47:41 GMT  
		Size: 364.1 MB (364091294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2a89be60a77cd8d520ec5f03d703ddbc15675dd1df4d95e041032cf08960af5`  
		Last Modified: Wed, 10 May 2023 02:23:36 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:446cee93ab2781cfc08e135a3a7ab166e5342ee6817c34fb47e0662c085bbc29`  
		Last Modified: Wed, 10 May 2023 02:49:15 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a057529e52e0e6010038d1fe4fc95821b317ee7379ce74a6ccdaeb4397c6580`  
		Last Modified: Tue, 13 Jun 2023 22:18:48 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c741cf7b9012d8cb23e39f90427fded64f0e4de03039ddf48b77f15ef89d7ae0`  
		Last Modified: Tue, 13 Jun 2023 22:18:48 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:208c61957253b4017f86095081c6827718ad7b858e26d20a163e66ab10ed6a92`  
		Last Modified: Tue, 13 Jun 2023 22:18:48 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3e815afe033119fccd2887c2236ea581cbab8d6d5f4b146e2f03a35c99e150c`  
		Last Modified: Tue, 13 Jun 2023 22:18:48 GMT  
		Size: 448.8 KB (448805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c786064ca9923a9e7e6f5d6e0b3a08cb4c345cb8b37053a51ffe1ed92baa434f`  
		Last Modified: Tue, 13 Jun 2023 22:18:47 GMT  
		Size: 5.5 MB (5465263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ca1ecd70300344a64c5b09e7e0ef4325d7d434f3aee3b1d7845b33db7c8b8c6`  
		Last Modified: Tue, 13 Jun 2023 22:18:46 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8b2ae653f72ce5dc355f193098cdcdeb2cd780c78bed2991512625ead60fe16`  
		Last Modified: Tue, 13 Jun 2023 22:18:46 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d20c4caf3b063c53361edeec4547495178a5ee257f0afb5d83edb3a4d0b55bf`  
		Last Modified: Tue, 13 Jun 2023 22:18:46 GMT  
		Size: 1.4 KB (1374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6cf54e3a0a4a7d1916f3634aa394fdee5078f370ce0f19f05621468dbb0e6f4`  
		Last Modified: Tue, 13 Jun 2023 22:18:46 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.18`

```console
$ docker pull nats@sha256:bec70d3c576d9d47c112ba92489b19b35da4b1b7beb32009ca6b9564ef86c625
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.4377; amd64

### `nats:2.9.18` - linux; arm variant v6

```console
$ docker pull nats@sha256:f26f23aad2feedaeaca9df38eca5559b431fbb8ed841789b1e6b2c3c84ffa79b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4884857 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8ae95e37599ef924cfe3d5890b3af209e09951179f6672d35af6811876e61253`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 13 Jun 2023 21:49:33 GMT
COPY file:e5bb5e8247a1c4bdb92d70dc84443f615728207816f4c76763893029e98fe987 in /nats-server 
# Tue, 13 Jun 2023 21:49:33 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 13 Jun 2023 21:49:33 GMT
EXPOSE 4222 6222 8222
# Tue, 13 Jun 2023 21:49:33 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 13 Jun 2023 21:49:33 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 13 Jun 2023 21:49:33 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:7f1a7a7f3e313c163918678d53d48af6476087e63070356ad38ff1c041606bca`  
		Last Modified: Tue, 13 Jun 2023 21:50:13 GMT  
		Size: 4.9 MB (4884348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9af05a149bcbd29ea7705539c8b49e2c00b5883848519f3929bf4c4dc424022e`  
		Last Modified: Tue, 13 Jun 2023 21:50:12 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.18` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:edbf69c3a8dab18af6eefffc70fcea84205a4397632e23fbde4cca5fe03446ff
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4688025 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b395b40ae1ff951faa10f8f5c05810b77b0a03c2ef5a8eaa8bc443497b52348d`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 13 Jun 2023 22:34:13 GMT
COPY file:0fec8537fba7c573dbe20b854a6b32d8b0940e46f9e81c41611d447b82a034bc in /nats-server 
# Tue, 13 Jun 2023 22:34:13 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 13 Jun 2023 22:34:13 GMT
EXPOSE 4222 6222 8222
# Tue, 13 Jun 2023 22:34:14 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 13 Jun 2023 22:34:14 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 13 Jun 2023 22:34:14 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:2cce796fcd5a4e60d6ca871c71b29485d80a6babd1c43a056db0b52aa6e904b6`  
		Last Modified: Tue, 13 Jun 2023 22:34:58 GMT  
		Size: 4.7 MB (4687516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22153c0efa275cbe62c344213d16db73c5732467534b2a316e379bdd77324d29`  
		Last Modified: Tue, 13 Jun 2023 22:34:57 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.18` - windows version 10.0.17763.4377; amd64

```console
$ docker pull nats@sha256:ffdbc972ae083180acdcc8d74756ed6c94b032bce6d7ec4c224f8343919f232d
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.6 MB (109564530 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b23b2cb10135235e109abd0ca99d3cf4027f72a1c246c873707190f54bffec4`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 05 May 2023 11:29:01 GMT
RUN Apply image 10.0.17763.4377
# Wed, 10 May 2023 02:43:57 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Tue, 13 Jun 2023 22:18:13 GMT
RUN cmd /S /C #(nop) COPY file:e92fb324fb1e715aaa4f213ef42afe80c4a76690e3b2d439bee510cb2ae47cd5 in C:\nats-server.exe 
# Tue, 13 Jun 2023 22:18:14 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Tue, 13 Jun 2023 22:18:15 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Tue, 13 Jun 2023 22:18:15 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 13 Jun 2023 22:18:16 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:f7885e3a2dfeae5eea125d00da688c29930a05e4d904884fe43e093ce6223664`  
		Last Modified: Wed, 10 May 2023 01:49:01 GMT  
		Size: 104.4 MB (104383998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9af27dd7e62b7d94fa31a7c9efd9a532c42db89ec01fdb7fe430043ceabc5b4`  
		Last Modified: Wed, 10 May 2023 02:49:27 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74147f1370eb575d5bc03ac650054b5dcc36d7b40bf7706dde9d9d159d10e1a8`  
		Last Modified: Tue, 13 Jun 2023 22:19:04 GMT  
		Size: 5.2 MB (5174125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c441087537bf6a2963fdc58d12d836350044355df07fa9d696fe6e61819cc0ea`  
		Last Modified: Tue, 13 Jun 2023 22:19:02 GMT  
		Size: 1.8 KB (1803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94f7788277dc1622146a19b5407e20fc8eb003cd62b331460221d930e9154d31`  
		Last Modified: Tue, 13 Jun 2023 22:19:02 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b991262b6e730687a02c0d68ac25bc2dcf4dff69f1e9db5315f654387aab754`  
		Last Modified: Tue, 13 Jun 2023 22:19:02 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c322d11690204cb63afb856a65f1fdd8016ebd23989de8952a6ecb7f6737f17e`  
		Last Modified: Tue, 13 Jun 2023 22:19:02 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.18-alpine`

```console
$ docker pull nats@sha256:d52d61660934c995489d5df46b8733f8f045b823921c90e850f1586241b807b2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `nats:2.9.18-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:957b9d5d12d8d9df6fea32822bd03a00b514635d8ede3f04c8fe3a2a0e8c436f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.3 MB (8326824 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9512db9e4ee16375a3bc31274c1b7a0480263800e5c7cfd91f794674b53e15a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 May 2023 23:11:04 GMT
ADD file:f87a991e2e9f185fd4a88569d86a9b8e5bc07182e7fa613b95acab25986f2a6c in / 
# Tue, 09 May 2023 23:11:04 GMT
CMD ["/bin/sh"]
# Tue, 13 Jun 2023 21:49:21 GMT
ENV NATS_SERVER=2.9.18
# Tue, 13 Jun 2023 21:49:24 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f5ea0ace65873cf81dde2951d9130f6ecad3f96e80a59badb259a66fc3294579' ;; 		armhf) natsArch='arm6'; sha256='f7dd549c09bac2adcc3260868bf5f182645c8e59e7b9cb868feff244017998b0' ;; 		armv7) natsArch='arm7'; sha256='bb1015887864e7eeeeb8bef4c9e06bd20d865b01a67bab8bab802ef5483bb6ad' ;; 		x86_64) natsArch='amd64'; sha256='c61c5dd662ed0836d752ed98508d5a7328d85e6126d2cf9784a0d546a64c961c' ;; 		x86) natsArch='386'; sha256='68467b7d83a96a554257b84464bdff34de956af93971e43faa711e1cb29249c8' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 13 Jun 2023 21:49:24 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 13 Jun 2023 21:49:24 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 13 Jun 2023 21:49:24 GMT
EXPOSE 4222 6222 8222
# Tue, 13 Jun 2023 21:49:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Jun 2023 21:49:25 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:015ee8d9fb3dca1b18815f1e4ee0d325d1f40cde6f2df4dd307918f7b69167d7`  
		Last Modified: Tue, 09 May 2023 23:11:20 GMT  
		Size: 3.2 MB (3155679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21a6505f5ff97d93b3e5451bb54fc64eea5680c617ce8cc7501394caf032f27f`  
		Last Modified: Tue, 13 Jun 2023 21:49:52 GMT  
		Size: 5.2 MB (5170145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43d0bff33a6560b8efd5c213b10cd3176703757ba35859a5ec499ca24abb1139`  
		Last Modified: Tue, 13 Jun 2023 21:49:51 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea53aff73c749d762e22ffbd5e9caecadeb064790877afe9c0b536284c9e4c59`  
		Last Modified: Tue, 13 Jun 2023 21:49:51 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.18-alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:ce87b1ebec8a22151ac8ae437db42293e4293bfecd5045752d86f661b0547b26
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.3 MB (8315499 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bdbca1cbb72621a6502190ab58418aee769fffb9d66712c9ea805d56d3fb46fc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 May 2023 23:11:08 GMT
ADD file:df7fccc3453b6ec1401d27a1295b0882a83e731fde8f23db9d3f687a2b6b4e70 in / 
# Tue, 09 May 2023 23:11:08 GMT
CMD ["/bin/sh"]
# Tue, 13 Jun 2023 22:33:21 GMT
ENV NATS_SERVER=2.9.18
# Tue, 13 Jun 2023 22:33:23 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f5ea0ace65873cf81dde2951d9130f6ecad3f96e80a59badb259a66fc3294579' ;; 		armhf) natsArch='arm6'; sha256='f7dd549c09bac2adcc3260868bf5f182645c8e59e7b9cb868feff244017998b0' ;; 		armv7) natsArch='arm7'; sha256='bb1015887864e7eeeeb8bef4c9e06bd20d865b01a67bab8bab802ef5483bb6ad' ;; 		x86_64) natsArch='amd64'; sha256='c61c5dd662ed0836d752ed98508d5a7328d85e6126d2cf9784a0d546a64c961c' ;; 		x86) natsArch='386'; sha256='68467b7d83a96a554257b84464bdff34de956af93971e43faa711e1cb29249c8' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 13 Jun 2023 22:33:23 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 13 Jun 2023 22:33:23 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 13 Jun 2023 22:33:23 GMT
EXPOSE 4222 6222 8222
# Tue, 13 Jun 2023 22:33:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Jun 2023 22:33:23 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:08409d4172603f40b56eb6b76240a1e6bd78baa0e96590dc7ff76c5f1a093af2`  
		Last Modified: Tue, 09 May 2023 23:11:23 GMT  
		Size: 3.3 MB (3342848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf2d0fd688338eb8ef69b776354053dd65c78ae5e4c3cc2e15fc586f51942d89`  
		Last Modified: Tue, 13 Jun 2023 22:34:38 GMT  
		Size: 5.0 MB (4971650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee9d7fff35b08386d1a65e0e1fa0a81bcc5877d1024bd16ca00f0af62137cdc4`  
		Last Modified: Tue, 13 Jun 2023 22:34:37 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63543f616abdbde1673d999e8e046e0f59aa734ab23d6acabdf42a9756f8c357`  
		Last Modified: Tue, 13 Jun 2023 22:34:37 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.18-alpine3.18`

```console
$ docker pull nats@sha256:d52d61660934c995489d5df46b8733f8f045b823921c90e850f1586241b807b2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `nats:2.9.18-alpine3.18` - linux; arm variant v6

```console
$ docker pull nats@sha256:957b9d5d12d8d9df6fea32822bd03a00b514635d8ede3f04c8fe3a2a0e8c436f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.3 MB (8326824 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9512db9e4ee16375a3bc31274c1b7a0480263800e5c7cfd91f794674b53e15a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 May 2023 23:11:04 GMT
ADD file:f87a991e2e9f185fd4a88569d86a9b8e5bc07182e7fa613b95acab25986f2a6c in / 
# Tue, 09 May 2023 23:11:04 GMT
CMD ["/bin/sh"]
# Tue, 13 Jun 2023 21:49:21 GMT
ENV NATS_SERVER=2.9.18
# Tue, 13 Jun 2023 21:49:24 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f5ea0ace65873cf81dde2951d9130f6ecad3f96e80a59badb259a66fc3294579' ;; 		armhf) natsArch='arm6'; sha256='f7dd549c09bac2adcc3260868bf5f182645c8e59e7b9cb868feff244017998b0' ;; 		armv7) natsArch='arm7'; sha256='bb1015887864e7eeeeb8bef4c9e06bd20d865b01a67bab8bab802ef5483bb6ad' ;; 		x86_64) natsArch='amd64'; sha256='c61c5dd662ed0836d752ed98508d5a7328d85e6126d2cf9784a0d546a64c961c' ;; 		x86) natsArch='386'; sha256='68467b7d83a96a554257b84464bdff34de956af93971e43faa711e1cb29249c8' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 13 Jun 2023 21:49:24 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 13 Jun 2023 21:49:24 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 13 Jun 2023 21:49:24 GMT
EXPOSE 4222 6222 8222
# Tue, 13 Jun 2023 21:49:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Jun 2023 21:49:25 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:015ee8d9fb3dca1b18815f1e4ee0d325d1f40cde6f2df4dd307918f7b69167d7`  
		Last Modified: Tue, 09 May 2023 23:11:20 GMT  
		Size: 3.2 MB (3155679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21a6505f5ff97d93b3e5451bb54fc64eea5680c617ce8cc7501394caf032f27f`  
		Last Modified: Tue, 13 Jun 2023 21:49:52 GMT  
		Size: 5.2 MB (5170145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43d0bff33a6560b8efd5c213b10cd3176703757ba35859a5ec499ca24abb1139`  
		Last Modified: Tue, 13 Jun 2023 21:49:51 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea53aff73c749d762e22ffbd5e9caecadeb064790877afe9c0b536284c9e4c59`  
		Last Modified: Tue, 13 Jun 2023 21:49:51 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.18-alpine3.18` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:ce87b1ebec8a22151ac8ae437db42293e4293bfecd5045752d86f661b0547b26
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.3 MB (8315499 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bdbca1cbb72621a6502190ab58418aee769fffb9d66712c9ea805d56d3fb46fc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 May 2023 23:11:08 GMT
ADD file:df7fccc3453b6ec1401d27a1295b0882a83e731fde8f23db9d3f687a2b6b4e70 in / 
# Tue, 09 May 2023 23:11:08 GMT
CMD ["/bin/sh"]
# Tue, 13 Jun 2023 22:33:21 GMT
ENV NATS_SERVER=2.9.18
# Tue, 13 Jun 2023 22:33:23 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f5ea0ace65873cf81dde2951d9130f6ecad3f96e80a59badb259a66fc3294579' ;; 		armhf) natsArch='arm6'; sha256='f7dd549c09bac2adcc3260868bf5f182645c8e59e7b9cb868feff244017998b0' ;; 		armv7) natsArch='arm7'; sha256='bb1015887864e7eeeeb8bef4c9e06bd20d865b01a67bab8bab802ef5483bb6ad' ;; 		x86_64) natsArch='amd64'; sha256='c61c5dd662ed0836d752ed98508d5a7328d85e6126d2cf9784a0d546a64c961c' ;; 		x86) natsArch='386'; sha256='68467b7d83a96a554257b84464bdff34de956af93971e43faa711e1cb29249c8' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 13 Jun 2023 22:33:23 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 13 Jun 2023 22:33:23 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 13 Jun 2023 22:33:23 GMT
EXPOSE 4222 6222 8222
# Tue, 13 Jun 2023 22:33:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Jun 2023 22:33:23 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:08409d4172603f40b56eb6b76240a1e6bd78baa0e96590dc7ff76c5f1a093af2`  
		Last Modified: Tue, 09 May 2023 23:11:23 GMT  
		Size: 3.3 MB (3342848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf2d0fd688338eb8ef69b776354053dd65c78ae5e4c3cc2e15fc586f51942d89`  
		Last Modified: Tue, 13 Jun 2023 22:34:38 GMT  
		Size: 5.0 MB (4971650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee9d7fff35b08386d1a65e0e1fa0a81bcc5877d1024bd16ca00f0af62137cdc4`  
		Last Modified: Tue, 13 Jun 2023 22:34:37 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63543f616abdbde1673d999e8e046e0f59aa734ab23d6acabdf42a9756f8c357`  
		Last Modified: Tue, 13 Jun 2023 22:34:37 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.18-linux`

```console
$ docker pull nats@sha256:841b57508206cdc313e22842e3c4c15e66d31d7d4a1c465cd603337368a7705a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `nats:2.9.18-linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:f26f23aad2feedaeaca9df38eca5559b431fbb8ed841789b1e6b2c3c84ffa79b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4884857 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8ae95e37599ef924cfe3d5890b3af209e09951179f6672d35af6811876e61253`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 13 Jun 2023 21:49:33 GMT
COPY file:e5bb5e8247a1c4bdb92d70dc84443f615728207816f4c76763893029e98fe987 in /nats-server 
# Tue, 13 Jun 2023 21:49:33 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 13 Jun 2023 21:49:33 GMT
EXPOSE 4222 6222 8222
# Tue, 13 Jun 2023 21:49:33 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 13 Jun 2023 21:49:33 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 13 Jun 2023 21:49:33 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:7f1a7a7f3e313c163918678d53d48af6476087e63070356ad38ff1c041606bca`  
		Last Modified: Tue, 13 Jun 2023 21:50:13 GMT  
		Size: 4.9 MB (4884348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9af05a149bcbd29ea7705539c8b49e2c00b5883848519f3929bf4c4dc424022e`  
		Last Modified: Tue, 13 Jun 2023 21:50:12 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.18-linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:edbf69c3a8dab18af6eefffc70fcea84205a4397632e23fbde4cca5fe03446ff
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4688025 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b395b40ae1ff951faa10f8f5c05810b77b0a03c2ef5a8eaa8bc443497b52348d`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 13 Jun 2023 22:34:13 GMT
COPY file:0fec8537fba7c573dbe20b854a6b32d8b0940e46f9e81c41611d447b82a034bc in /nats-server 
# Tue, 13 Jun 2023 22:34:13 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 13 Jun 2023 22:34:13 GMT
EXPOSE 4222 6222 8222
# Tue, 13 Jun 2023 22:34:14 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 13 Jun 2023 22:34:14 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 13 Jun 2023 22:34:14 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:2cce796fcd5a4e60d6ca871c71b29485d80a6babd1c43a056db0b52aa6e904b6`  
		Last Modified: Tue, 13 Jun 2023 22:34:58 GMT  
		Size: 4.7 MB (4687516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22153c0efa275cbe62c344213d16db73c5732467534b2a316e379bdd77324d29`  
		Last Modified: Tue, 13 Jun 2023 22:34:57 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.18-nanoserver`

```console
$ docker pull nats@sha256:0a384e9a7d76bb1288a9b091976b9fa61e78c22143d6a07415707fdd6123219c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4377; amd64

### `nats:2.9.18-nanoserver` - windows version 10.0.17763.4377; amd64

```console
$ docker pull nats@sha256:ffdbc972ae083180acdcc8d74756ed6c94b032bce6d7ec4c224f8343919f232d
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.6 MB (109564530 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b23b2cb10135235e109abd0ca99d3cf4027f72a1c246c873707190f54bffec4`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 05 May 2023 11:29:01 GMT
RUN Apply image 10.0.17763.4377
# Wed, 10 May 2023 02:43:57 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Tue, 13 Jun 2023 22:18:13 GMT
RUN cmd /S /C #(nop) COPY file:e92fb324fb1e715aaa4f213ef42afe80c4a76690e3b2d439bee510cb2ae47cd5 in C:\nats-server.exe 
# Tue, 13 Jun 2023 22:18:14 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Tue, 13 Jun 2023 22:18:15 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Tue, 13 Jun 2023 22:18:15 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 13 Jun 2023 22:18:16 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:f7885e3a2dfeae5eea125d00da688c29930a05e4d904884fe43e093ce6223664`  
		Last Modified: Wed, 10 May 2023 01:49:01 GMT  
		Size: 104.4 MB (104383998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9af27dd7e62b7d94fa31a7c9efd9a532c42db89ec01fdb7fe430043ceabc5b4`  
		Last Modified: Wed, 10 May 2023 02:49:27 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74147f1370eb575d5bc03ac650054b5dcc36d7b40bf7706dde9d9d159d10e1a8`  
		Last Modified: Tue, 13 Jun 2023 22:19:04 GMT  
		Size: 5.2 MB (5174125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c441087537bf6a2963fdc58d12d836350044355df07fa9d696fe6e61819cc0ea`  
		Last Modified: Tue, 13 Jun 2023 22:19:02 GMT  
		Size: 1.8 KB (1803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94f7788277dc1622146a19b5407e20fc8eb003cd62b331460221d930e9154d31`  
		Last Modified: Tue, 13 Jun 2023 22:19:02 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b991262b6e730687a02c0d68ac25bc2dcf4dff69f1e9db5315f654387aab754`  
		Last Modified: Tue, 13 Jun 2023 22:19:02 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c322d11690204cb63afb856a65f1fdd8016ebd23989de8952a6ecb7f6737f17e`  
		Last Modified: Tue, 13 Jun 2023 22:19:02 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.18-nanoserver-1809`

```console
$ docker pull nats@sha256:0a384e9a7d76bb1288a9b091976b9fa61e78c22143d6a07415707fdd6123219c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4377; amd64

### `nats:2.9.18-nanoserver-1809` - windows version 10.0.17763.4377; amd64

```console
$ docker pull nats@sha256:ffdbc972ae083180acdcc8d74756ed6c94b032bce6d7ec4c224f8343919f232d
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.6 MB (109564530 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b23b2cb10135235e109abd0ca99d3cf4027f72a1c246c873707190f54bffec4`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 05 May 2023 11:29:01 GMT
RUN Apply image 10.0.17763.4377
# Wed, 10 May 2023 02:43:57 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Tue, 13 Jun 2023 22:18:13 GMT
RUN cmd /S /C #(nop) COPY file:e92fb324fb1e715aaa4f213ef42afe80c4a76690e3b2d439bee510cb2ae47cd5 in C:\nats-server.exe 
# Tue, 13 Jun 2023 22:18:14 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Tue, 13 Jun 2023 22:18:15 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Tue, 13 Jun 2023 22:18:15 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 13 Jun 2023 22:18:16 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:f7885e3a2dfeae5eea125d00da688c29930a05e4d904884fe43e093ce6223664`  
		Last Modified: Wed, 10 May 2023 01:49:01 GMT  
		Size: 104.4 MB (104383998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9af27dd7e62b7d94fa31a7c9efd9a532c42db89ec01fdb7fe430043ceabc5b4`  
		Last Modified: Wed, 10 May 2023 02:49:27 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74147f1370eb575d5bc03ac650054b5dcc36d7b40bf7706dde9d9d159d10e1a8`  
		Last Modified: Tue, 13 Jun 2023 22:19:04 GMT  
		Size: 5.2 MB (5174125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c441087537bf6a2963fdc58d12d836350044355df07fa9d696fe6e61819cc0ea`  
		Last Modified: Tue, 13 Jun 2023 22:19:02 GMT  
		Size: 1.8 KB (1803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94f7788277dc1622146a19b5407e20fc8eb003cd62b331460221d930e9154d31`  
		Last Modified: Tue, 13 Jun 2023 22:19:02 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b991262b6e730687a02c0d68ac25bc2dcf4dff69f1e9db5315f654387aab754`  
		Last Modified: Tue, 13 Jun 2023 22:19:02 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c322d11690204cb63afb856a65f1fdd8016ebd23989de8952a6ecb7f6737f17e`  
		Last Modified: Tue, 13 Jun 2023 22:19:02 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.18-scratch`

```console
$ docker pull nats@sha256:841b57508206cdc313e22842e3c4c15e66d31d7d4a1c465cd603337368a7705a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `nats:2.9.18-scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:f26f23aad2feedaeaca9df38eca5559b431fbb8ed841789b1e6b2c3c84ffa79b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4884857 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8ae95e37599ef924cfe3d5890b3af209e09951179f6672d35af6811876e61253`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 13 Jun 2023 21:49:33 GMT
COPY file:e5bb5e8247a1c4bdb92d70dc84443f615728207816f4c76763893029e98fe987 in /nats-server 
# Tue, 13 Jun 2023 21:49:33 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 13 Jun 2023 21:49:33 GMT
EXPOSE 4222 6222 8222
# Tue, 13 Jun 2023 21:49:33 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 13 Jun 2023 21:49:33 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 13 Jun 2023 21:49:33 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:7f1a7a7f3e313c163918678d53d48af6476087e63070356ad38ff1c041606bca`  
		Last Modified: Tue, 13 Jun 2023 21:50:13 GMT  
		Size: 4.9 MB (4884348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9af05a149bcbd29ea7705539c8b49e2c00b5883848519f3929bf4c4dc424022e`  
		Last Modified: Tue, 13 Jun 2023 21:50:12 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.18-scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:edbf69c3a8dab18af6eefffc70fcea84205a4397632e23fbde4cca5fe03446ff
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4688025 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b395b40ae1ff951faa10f8f5c05810b77b0a03c2ef5a8eaa8bc443497b52348d`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 13 Jun 2023 22:34:13 GMT
COPY file:0fec8537fba7c573dbe20b854a6b32d8b0940e46f9e81c41611d447b82a034bc in /nats-server 
# Tue, 13 Jun 2023 22:34:13 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 13 Jun 2023 22:34:13 GMT
EXPOSE 4222 6222 8222
# Tue, 13 Jun 2023 22:34:14 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 13 Jun 2023 22:34:14 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 13 Jun 2023 22:34:14 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:2cce796fcd5a4e60d6ca871c71b29485d80a6babd1c43a056db0b52aa6e904b6`  
		Last Modified: Tue, 13 Jun 2023 22:34:58 GMT  
		Size: 4.7 MB (4687516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22153c0efa275cbe62c344213d16db73c5732467534b2a316e379bdd77324d29`  
		Last Modified: Tue, 13 Jun 2023 22:34:57 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.18-windowsservercore`

```console
$ docker pull nats@sha256:85d1368e7f6f675346e070014b558c792541dfc94c5bd2d9f919736ddaa90dee
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4377; amd64

### `nats:2.9.18-windowsservercore` - windows version 10.0.17763.4377; amd64

```console
$ docker pull nats@sha256:6116850a9313d0b910b0db095a33e7297f06b633f1e1fb386db4fd023e23985e
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2077962593 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d0359af1b68ffc80fd1b560b7235f9eb6d3562810001343595480a3f55a0e043`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Fri, 05 May 2023 12:05:28 GMT
RUN Install update 10.0.17763.4377
# Wed, 10 May 2023 01:56:29 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 May 2023 02:40:26 GMT
ENV NATS_DOCKERIZED=1
# Tue, 13 Jun 2023 22:15:14 GMT
ENV NATS_SERVER=2.9.18
# Tue, 13 Jun 2023 22:15:15 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.9.18/nats-server-v2.9.18-windows-amd64.zip
# Tue, 13 Jun 2023 22:15:16 GMT
ENV NATS_SERVER_SHASUM=139c2d63193d7df39894b144fb08a40e15548f89087e1932617239d36ab0c901
# Tue, 13 Jun 2023 22:16:20 GMT
RUN Set-PSDebug -Trace 2
# Tue, 13 Jun 2023 22:17:54 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Tue, 13 Jun 2023 22:17:54 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Tue, 13 Jun 2023 22:17:55 GMT
EXPOSE 4222 6222 8222
# Tue, 13 Jun 2023 22:17:56 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 13 Jun 2023 22:17:57 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e01de39a0c44e24aa1912078d32ee54389b71154e509138cc4f5d1de42e7a32a`  
		Last Modified: Wed, 10 May 2023 01:47:41 GMT  
		Size: 364.1 MB (364091294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2a89be60a77cd8d520ec5f03d703ddbc15675dd1df4d95e041032cf08960af5`  
		Last Modified: Wed, 10 May 2023 02:23:36 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:446cee93ab2781cfc08e135a3a7ab166e5342ee6817c34fb47e0662c085bbc29`  
		Last Modified: Wed, 10 May 2023 02:49:15 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a057529e52e0e6010038d1fe4fc95821b317ee7379ce74a6ccdaeb4397c6580`  
		Last Modified: Tue, 13 Jun 2023 22:18:48 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c741cf7b9012d8cb23e39f90427fded64f0e4de03039ddf48b77f15ef89d7ae0`  
		Last Modified: Tue, 13 Jun 2023 22:18:48 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:208c61957253b4017f86095081c6827718ad7b858e26d20a163e66ab10ed6a92`  
		Last Modified: Tue, 13 Jun 2023 22:18:48 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3e815afe033119fccd2887c2236ea581cbab8d6d5f4b146e2f03a35c99e150c`  
		Last Modified: Tue, 13 Jun 2023 22:18:48 GMT  
		Size: 448.8 KB (448805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c786064ca9923a9e7e6f5d6e0b3a08cb4c345cb8b37053a51ffe1ed92baa434f`  
		Last Modified: Tue, 13 Jun 2023 22:18:47 GMT  
		Size: 5.5 MB (5465263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ca1ecd70300344a64c5b09e7e0ef4325d7d434f3aee3b1d7845b33db7c8b8c6`  
		Last Modified: Tue, 13 Jun 2023 22:18:46 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8b2ae653f72ce5dc355f193098cdcdeb2cd780c78bed2991512625ead60fe16`  
		Last Modified: Tue, 13 Jun 2023 22:18:46 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d20c4caf3b063c53361edeec4547495178a5ee257f0afb5d83edb3a4d0b55bf`  
		Last Modified: Tue, 13 Jun 2023 22:18:46 GMT  
		Size: 1.4 KB (1374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6cf54e3a0a4a7d1916f3634aa394fdee5078f370ce0f19f05621468dbb0e6f4`  
		Last Modified: Tue, 13 Jun 2023 22:18:46 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.18-windowsservercore-1809`

```console
$ docker pull nats@sha256:85d1368e7f6f675346e070014b558c792541dfc94c5bd2d9f919736ddaa90dee
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4377; amd64

### `nats:2.9.18-windowsservercore-1809` - windows version 10.0.17763.4377; amd64

```console
$ docker pull nats@sha256:6116850a9313d0b910b0db095a33e7297f06b633f1e1fb386db4fd023e23985e
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2077962593 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d0359af1b68ffc80fd1b560b7235f9eb6d3562810001343595480a3f55a0e043`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Fri, 05 May 2023 12:05:28 GMT
RUN Install update 10.0.17763.4377
# Wed, 10 May 2023 01:56:29 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 May 2023 02:40:26 GMT
ENV NATS_DOCKERIZED=1
# Tue, 13 Jun 2023 22:15:14 GMT
ENV NATS_SERVER=2.9.18
# Tue, 13 Jun 2023 22:15:15 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.9.18/nats-server-v2.9.18-windows-amd64.zip
# Tue, 13 Jun 2023 22:15:16 GMT
ENV NATS_SERVER_SHASUM=139c2d63193d7df39894b144fb08a40e15548f89087e1932617239d36ab0c901
# Tue, 13 Jun 2023 22:16:20 GMT
RUN Set-PSDebug -Trace 2
# Tue, 13 Jun 2023 22:17:54 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Tue, 13 Jun 2023 22:17:54 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Tue, 13 Jun 2023 22:17:55 GMT
EXPOSE 4222 6222 8222
# Tue, 13 Jun 2023 22:17:56 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 13 Jun 2023 22:17:57 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e01de39a0c44e24aa1912078d32ee54389b71154e509138cc4f5d1de42e7a32a`  
		Last Modified: Wed, 10 May 2023 01:47:41 GMT  
		Size: 364.1 MB (364091294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2a89be60a77cd8d520ec5f03d703ddbc15675dd1df4d95e041032cf08960af5`  
		Last Modified: Wed, 10 May 2023 02:23:36 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:446cee93ab2781cfc08e135a3a7ab166e5342ee6817c34fb47e0662c085bbc29`  
		Last Modified: Wed, 10 May 2023 02:49:15 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a057529e52e0e6010038d1fe4fc95821b317ee7379ce74a6ccdaeb4397c6580`  
		Last Modified: Tue, 13 Jun 2023 22:18:48 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c741cf7b9012d8cb23e39f90427fded64f0e4de03039ddf48b77f15ef89d7ae0`  
		Last Modified: Tue, 13 Jun 2023 22:18:48 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:208c61957253b4017f86095081c6827718ad7b858e26d20a163e66ab10ed6a92`  
		Last Modified: Tue, 13 Jun 2023 22:18:48 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3e815afe033119fccd2887c2236ea581cbab8d6d5f4b146e2f03a35c99e150c`  
		Last Modified: Tue, 13 Jun 2023 22:18:48 GMT  
		Size: 448.8 KB (448805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c786064ca9923a9e7e6f5d6e0b3a08cb4c345cb8b37053a51ffe1ed92baa434f`  
		Last Modified: Tue, 13 Jun 2023 22:18:47 GMT  
		Size: 5.5 MB (5465263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ca1ecd70300344a64c5b09e7e0ef4325d7d434f3aee3b1d7845b33db7c8b8c6`  
		Last Modified: Tue, 13 Jun 2023 22:18:46 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8b2ae653f72ce5dc355f193098cdcdeb2cd780c78bed2991512625ead60fe16`  
		Last Modified: Tue, 13 Jun 2023 22:18:46 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d20c4caf3b063c53361edeec4547495178a5ee257f0afb5d83edb3a4d0b55bf`  
		Last Modified: Tue, 13 Jun 2023 22:18:46 GMT  
		Size: 1.4 KB (1374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6cf54e3a0a4a7d1916f3634aa394fdee5078f370ce0f19f05621468dbb0e6f4`  
		Last Modified: Tue, 13 Jun 2023 22:18:46 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:alpine`

```console
$ docker pull nats@sha256:d2647f1f7552973967b5b974d098c290c62dcf29eedfed515917ded32afe4a94
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:alpine` - linux; amd64

```console
$ docker pull nats@sha256:7544f1dfe4b270789a68e2056135467d525da411f331f43640150b0642dee693
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.8 MB (8802768 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:04ada7bbdb360a5406551ced3593bc48e57c6cea5ee5d502e1a0df2437156d06`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 May 2023 23:11:10 GMT
ADD file:7625ddfd589fb824ee39f1b1eb387b98f3676420ff52f26eb9d975151e889667 in / 
# Tue, 09 May 2023 23:11:10 GMT
CMD ["/bin/sh"]
# Thu, 18 May 2023 21:19:49 GMT
ENV NATS_SERVER=2.9.17
# Thu, 18 May 2023 21:19:51 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='c7cf7bf8c029500d1b51773132ecc13a1fc89f2e080faa6b505da8cb95aa2a0c' ;; 		armhf) natsArch='arm6'; sha256='b09812858f1c957fd1869e21d4b8d64b3b0d6cdf3abb34502167120640f1d5e1' ;; 		armv7) natsArch='arm7'; sha256='970649306f45c78404c42dc5c0ab37fa6d5149501e47a68bef7841a06730a654' ;; 		x86_64) natsArch='amd64'; sha256='4ad2d83dd2fb9cc44a7e078d2e400f37c188b8515100f5de0f10f0eefbeb6b23' ;; 		x86) natsArch='386'; sha256='59c42f21bb6e8a5ef6e101ce6e3c29692b2cc9b1eb28465e67edeb391450626c' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 18 May 2023 21:19:52 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 18 May 2023 21:19:52 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 18 May 2023 21:19:52 GMT
EXPOSE 4222 6222 8222
# Thu, 18 May 2023 21:19:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 18 May 2023 21:19:52 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:8a49fdb3b6a5ff2bd8ec6a86c05b2922a0f7454579ecc07637e94dfd1d0639b6`  
		Last Modified: Tue, 09 May 2023 23:11:26 GMT  
		Size: 3.4 MB (3397490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ba69a821f226517d8763fd5007b51eeb8a68e40f7fb32dec75e13297ea1cb49`  
		Last Modified: Thu, 18 May 2023 21:20:19 GMT  
		Size: 5.4 MB (5404276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11ad2f9c9076c4ccedf3a056bf6e996a658fa5ece8cc35913e4728d58617e8b3`  
		Last Modified: Thu, 18 May 2023 21:20:18 GMT  
		Size: 588.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bb3c123b7bd114e7897ddf602c16bcd18f034abda3ee53d91a108b71c624faa`  
		Last Modified: Thu, 18 May 2023 21:20:18 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:957b9d5d12d8d9df6fea32822bd03a00b514635d8ede3f04c8fe3a2a0e8c436f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.3 MB (8326824 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9512db9e4ee16375a3bc31274c1b7a0480263800e5c7cfd91f794674b53e15a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 May 2023 23:11:04 GMT
ADD file:f87a991e2e9f185fd4a88569d86a9b8e5bc07182e7fa613b95acab25986f2a6c in / 
# Tue, 09 May 2023 23:11:04 GMT
CMD ["/bin/sh"]
# Tue, 13 Jun 2023 21:49:21 GMT
ENV NATS_SERVER=2.9.18
# Tue, 13 Jun 2023 21:49:24 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f5ea0ace65873cf81dde2951d9130f6ecad3f96e80a59badb259a66fc3294579' ;; 		armhf) natsArch='arm6'; sha256='f7dd549c09bac2adcc3260868bf5f182645c8e59e7b9cb868feff244017998b0' ;; 		armv7) natsArch='arm7'; sha256='bb1015887864e7eeeeb8bef4c9e06bd20d865b01a67bab8bab802ef5483bb6ad' ;; 		x86_64) natsArch='amd64'; sha256='c61c5dd662ed0836d752ed98508d5a7328d85e6126d2cf9784a0d546a64c961c' ;; 		x86) natsArch='386'; sha256='68467b7d83a96a554257b84464bdff34de956af93971e43faa711e1cb29249c8' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 13 Jun 2023 21:49:24 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 13 Jun 2023 21:49:24 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 13 Jun 2023 21:49:24 GMT
EXPOSE 4222 6222 8222
# Tue, 13 Jun 2023 21:49:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Jun 2023 21:49:25 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:015ee8d9fb3dca1b18815f1e4ee0d325d1f40cde6f2df4dd307918f7b69167d7`  
		Last Modified: Tue, 09 May 2023 23:11:20 GMT  
		Size: 3.2 MB (3155679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21a6505f5ff97d93b3e5451bb54fc64eea5680c617ce8cc7501394caf032f27f`  
		Last Modified: Tue, 13 Jun 2023 21:49:52 GMT  
		Size: 5.2 MB (5170145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43d0bff33a6560b8efd5c213b10cd3176703757ba35859a5ec499ca24abb1139`  
		Last Modified: Tue, 13 Jun 2023 21:49:51 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea53aff73c749d762e22ffbd5e9caecadeb064790877afe9c0b536284c9e4c59`  
		Last Modified: Tue, 13 Jun 2023 21:49:51 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:882066add3894dc13cfadaeec8af9f9fce5b9c3fee92e377a13f0997a88a121f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.1 MB (8071388 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:574536f22d8de67b2c2f0962d9e7d108bb4b41d07cb13a05ebab5e3b82fe6d63`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 May 2023 22:57:32 GMT
ADD file:eb6b6a885e8ac9bccbf44a5c673b8542c8144bba927376688240446c2f413b10 in / 
# Tue, 09 May 2023 22:57:32 GMT
CMD ["/bin/sh"]
# Thu, 18 May 2023 21:57:27 GMT
ENV NATS_SERVER=2.9.17
# Thu, 18 May 2023 21:57:29 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='c7cf7bf8c029500d1b51773132ecc13a1fc89f2e080faa6b505da8cb95aa2a0c' ;; 		armhf) natsArch='arm6'; sha256='b09812858f1c957fd1869e21d4b8d64b3b0d6cdf3abb34502167120640f1d5e1' ;; 		armv7) natsArch='arm7'; sha256='970649306f45c78404c42dc5c0ab37fa6d5149501e47a68bef7841a06730a654' ;; 		x86_64) natsArch='amd64'; sha256='4ad2d83dd2fb9cc44a7e078d2e400f37c188b8515100f5de0f10f0eefbeb6b23' ;; 		x86) natsArch='386'; sha256='59c42f21bb6e8a5ef6e101ce6e3c29692b2cc9b1eb28465e67edeb391450626c' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 18 May 2023 21:57:29 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 18 May 2023 21:57:29 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 18 May 2023 21:57:29 GMT
EXPOSE 4222 6222 8222
# Thu, 18 May 2023 21:57:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 18 May 2023 21:57:30 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:e14425cf8fb9304b9ad4a9d1250e0d4c22e507a334ff747fa69b804500afc113`  
		Last Modified: Tue, 09 May 2023 22:57:50 GMT  
		Size: 2.9 MB (2911117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:213de106e11b3e7261faf48da426167af8702e8a56ab0237f786ba0eb864a38d`  
		Last Modified: Thu, 18 May 2023 21:58:08 GMT  
		Size: 5.2 MB (5159272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5535f74851ba24bbb57849b9f7085eb8441d584ea938b19bdd027f5ccf52a193`  
		Last Modified: Thu, 18 May 2023 21:58:07 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2518eda2d1b2ce9ae4c75acdccc0d3bbe028cfbdf30d7e173dfa82e489af6ec`  
		Last Modified: Thu, 18 May 2023 21:58:08 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:ce87b1ebec8a22151ac8ae437db42293e4293bfecd5045752d86f661b0547b26
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.3 MB (8315499 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bdbca1cbb72621a6502190ab58418aee769fffb9d66712c9ea805d56d3fb46fc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 May 2023 23:11:08 GMT
ADD file:df7fccc3453b6ec1401d27a1295b0882a83e731fde8f23db9d3f687a2b6b4e70 in / 
# Tue, 09 May 2023 23:11:08 GMT
CMD ["/bin/sh"]
# Tue, 13 Jun 2023 22:33:21 GMT
ENV NATS_SERVER=2.9.18
# Tue, 13 Jun 2023 22:33:23 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f5ea0ace65873cf81dde2951d9130f6ecad3f96e80a59badb259a66fc3294579' ;; 		armhf) natsArch='arm6'; sha256='f7dd549c09bac2adcc3260868bf5f182645c8e59e7b9cb868feff244017998b0' ;; 		armv7) natsArch='arm7'; sha256='bb1015887864e7eeeeb8bef4c9e06bd20d865b01a67bab8bab802ef5483bb6ad' ;; 		x86_64) natsArch='amd64'; sha256='c61c5dd662ed0836d752ed98508d5a7328d85e6126d2cf9784a0d546a64c961c' ;; 		x86) natsArch='386'; sha256='68467b7d83a96a554257b84464bdff34de956af93971e43faa711e1cb29249c8' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 13 Jun 2023 22:33:23 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 13 Jun 2023 22:33:23 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 13 Jun 2023 22:33:23 GMT
EXPOSE 4222 6222 8222
# Tue, 13 Jun 2023 22:33:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Jun 2023 22:33:23 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:08409d4172603f40b56eb6b76240a1e6bd78baa0e96590dc7ff76c5f1a093af2`  
		Last Modified: Tue, 09 May 2023 23:11:23 GMT  
		Size: 3.3 MB (3342848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf2d0fd688338eb8ef69b776354053dd65c78ae5e4c3cc2e15fc586f51942d89`  
		Last Modified: Tue, 13 Jun 2023 22:34:38 GMT  
		Size: 5.0 MB (4971650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee9d7fff35b08386d1a65e0e1fa0a81bcc5877d1024bd16ca00f0af62137cdc4`  
		Last Modified: Tue, 13 Jun 2023 22:34:37 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63543f616abdbde1673d999e8e046e0f59aa734ab23d6acabdf42a9756f8c357`  
		Last Modified: Tue, 13 Jun 2023 22:34:37 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:alpine3.18`

```console
$ docker pull nats@sha256:d2647f1f7552973967b5b974d098c290c62dcf29eedfed515917ded32afe4a94
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:alpine3.18` - linux; amd64

```console
$ docker pull nats@sha256:7544f1dfe4b270789a68e2056135467d525da411f331f43640150b0642dee693
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.8 MB (8802768 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:04ada7bbdb360a5406551ced3593bc48e57c6cea5ee5d502e1a0df2437156d06`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 May 2023 23:11:10 GMT
ADD file:7625ddfd589fb824ee39f1b1eb387b98f3676420ff52f26eb9d975151e889667 in / 
# Tue, 09 May 2023 23:11:10 GMT
CMD ["/bin/sh"]
# Thu, 18 May 2023 21:19:49 GMT
ENV NATS_SERVER=2.9.17
# Thu, 18 May 2023 21:19:51 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='c7cf7bf8c029500d1b51773132ecc13a1fc89f2e080faa6b505da8cb95aa2a0c' ;; 		armhf) natsArch='arm6'; sha256='b09812858f1c957fd1869e21d4b8d64b3b0d6cdf3abb34502167120640f1d5e1' ;; 		armv7) natsArch='arm7'; sha256='970649306f45c78404c42dc5c0ab37fa6d5149501e47a68bef7841a06730a654' ;; 		x86_64) natsArch='amd64'; sha256='4ad2d83dd2fb9cc44a7e078d2e400f37c188b8515100f5de0f10f0eefbeb6b23' ;; 		x86) natsArch='386'; sha256='59c42f21bb6e8a5ef6e101ce6e3c29692b2cc9b1eb28465e67edeb391450626c' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 18 May 2023 21:19:52 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 18 May 2023 21:19:52 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 18 May 2023 21:19:52 GMT
EXPOSE 4222 6222 8222
# Thu, 18 May 2023 21:19:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 18 May 2023 21:19:52 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:8a49fdb3b6a5ff2bd8ec6a86c05b2922a0f7454579ecc07637e94dfd1d0639b6`  
		Last Modified: Tue, 09 May 2023 23:11:26 GMT  
		Size: 3.4 MB (3397490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ba69a821f226517d8763fd5007b51eeb8a68e40f7fb32dec75e13297ea1cb49`  
		Last Modified: Thu, 18 May 2023 21:20:19 GMT  
		Size: 5.4 MB (5404276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11ad2f9c9076c4ccedf3a056bf6e996a658fa5ece8cc35913e4728d58617e8b3`  
		Last Modified: Thu, 18 May 2023 21:20:18 GMT  
		Size: 588.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bb3c123b7bd114e7897ddf602c16bcd18f034abda3ee53d91a108b71c624faa`  
		Last Modified: Thu, 18 May 2023 21:20:18 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.18` - linux; arm variant v6

```console
$ docker pull nats@sha256:957b9d5d12d8d9df6fea32822bd03a00b514635d8ede3f04c8fe3a2a0e8c436f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.3 MB (8326824 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9512db9e4ee16375a3bc31274c1b7a0480263800e5c7cfd91f794674b53e15a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 May 2023 23:11:04 GMT
ADD file:f87a991e2e9f185fd4a88569d86a9b8e5bc07182e7fa613b95acab25986f2a6c in / 
# Tue, 09 May 2023 23:11:04 GMT
CMD ["/bin/sh"]
# Tue, 13 Jun 2023 21:49:21 GMT
ENV NATS_SERVER=2.9.18
# Tue, 13 Jun 2023 21:49:24 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f5ea0ace65873cf81dde2951d9130f6ecad3f96e80a59badb259a66fc3294579' ;; 		armhf) natsArch='arm6'; sha256='f7dd549c09bac2adcc3260868bf5f182645c8e59e7b9cb868feff244017998b0' ;; 		armv7) natsArch='arm7'; sha256='bb1015887864e7eeeeb8bef4c9e06bd20d865b01a67bab8bab802ef5483bb6ad' ;; 		x86_64) natsArch='amd64'; sha256='c61c5dd662ed0836d752ed98508d5a7328d85e6126d2cf9784a0d546a64c961c' ;; 		x86) natsArch='386'; sha256='68467b7d83a96a554257b84464bdff34de956af93971e43faa711e1cb29249c8' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 13 Jun 2023 21:49:24 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 13 Jun 2023 21:49:24 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 13 Jun 2023 21:49:24 GMT
EXPOSE 4222 6222 8222
# Tue, 13 Jun 2023 21:49:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Jun 2023 21:49:25 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:015ee8d9fb3dca1b18815f1e4ee0d325d1f40cde6f2df4dd307918f7b69167d7`  
		Last Modified: Tue, 09 May 2023 23:11:20 GMT  
		Size: 3.2 MB (3155679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21a6505f5ff97d93b3e5451bb54fc64eea5680c617ce8cc7501394caf032f27f`  
		Last Modified: Tue, 13 Jun 2023 21:49:52 GMT  
		Size: 5.2 MB (5170145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43d0bff33a6560b8efd5c213b10cd3176703757ba35859a5ec499ca24abb1139`  
		Last Modified: Tue, 13 Jun 2023 21:49:51 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea53aff73c749d762e22ffbd5e9caecadeb064790877afe9c0b536284c9e4c59`  
		Last Modified: Tue, 13 Jun 2023 21:49:51 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.18` - linux; arm variant v7

```console
$ docker pull nats@sha256:882066add3894dc13cfadaeec8af9f9fce5b9c3fee92e377a13f0997a88a121f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.1 MB (8071388 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:574536f22d8de67b2c2f0962d9e7d108bb4b41d07cb13a05ebab5e3b82fe6d63`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 May 2023 22:57:32 GMT
ADD file:eb6b6a885e8ac9bccbf44a5c673b8542c8144bba927376688240446c2f413b10 in / 
# Tue, 09 May 2023 22:57:32 GMT
CMD ["/bin/sh"]
# Thu, 18 May 2023 21:57:27 GMT
ENV NATS_SERVER=2.9.17
# Thu, 18 May 2023 21:57:29 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='c7cf7bf8c029500d1b51773132ecc13a1fc89f2e080faa6b505da8cb95aa2a0c' ;; 		armhf) natsArch='arm6'; sha256='b09812858f1c957fd1869e21d4b8d64b3b0d6cdf3abb34502167120640f1d5e1' ;; 		armv7) natsArch='arm7'; sha256='970649306f45c78404c42dc5c0ab37fa6d5149501e47a68bef7841a06730a654' ;; 		x86_64) natsArch='amd64'; sha256='4ad2d83dd2fb9cc44a7e078d2e400f37c188b8515100f5de0f10f0eefbeb6b23' ;; 		x86) natsArch='386'; sha256='59c42f21bb6e8a5ef6e101ce6e3c29692b2cc9b1eb28465e67edeb391450626c' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 18 May 2023 21:57:29 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 18 May 2023 21:57:29 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 18 May 2023 21:57:29 GMT
EXPOSE 4222 6222 8222
# Thu, 18 May 2023 21:57:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 18 May 2023 21:57:30 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:e14425cf8fb9304b9ad4a9d1250e0d4c22e507a334ff747fa69b804500afc113`  
		Last Modified: Tue, 09 May 2023 22:57:50 GMT  
		Size: 2.9 MB (2911117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:213de106e11b3e7261faf48da426167af8702e8a56ab0237f786ba0eb864a38d`  
		Last Modified: Thu, 18 May 2023 21:58:08 GMT  
		Size: 5.2 MB (5159272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5535f74851ba24bbb57849b9f7085eb8441d584ea938b19bdd027f5ccf52a193`  
		Last Modified: Thu, 18 May 2023 21:58:07 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2518eda2d1b2ce9ae4c75acdccc0d3bbe028cfbdf30d7e173dfa82e489af6ec`  
		Last Modified: Thu, 18 May 2023 21:58:08 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.18` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:ce87b1ebec8a22151ac8ae437db42293e4293bfecd5045752d86f661b0547b26
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.3 MB (8315499 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bdbca1cbb72621a6502190ab58418aee769fffb9d66712c9ea805d56d3fb46fc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 May 2023 23:11:08 GMT
ADD file:df7fccc3453b6ec1401d27a1295b0882a83e731fde8f23db9d3f687a2b6b4e70 in / 
# Tue, 09 May 2023 23:11:08 GMT
CMD ["/bin/sh"]
# Tue, 13 Jun 2023 22:33:21 GMT
ENV NATS_SERVER=2.9.18
# Tue, 13 Jun 2023 22:33:23 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f5ea0ace65873cf81dde2951d9130f6ecad3f96e80a59badb259a66fc3294579' ;; 		armhf) natsArch='arm6'; sha256='f7dd549c09bac2adcc3260868bf5f182645c8e59e7b9cb868feff244017998b0' ;; 		armv7) natsArch='arm7'; sha256='bb1015887864e7eeeeb8bef4c9e06bd20d865b01a67bab8bab802ef5483bb6ad' ;; 		x86_64) natsArch='amd64'; sha256='c61c5dd662ed0836d752ed98508d5a7328d85e6126d2cf9784a0d546a64c961c' ;; 		x86) natsArch='386'; sha256='68467b7d83a96a554257b84464bdff34de956af93971e43faa711e1cb29249c8' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 13 Jun 2023 22:33:23 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 13 Jun 2023 22:33:23 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 13 Jun 2023 22:33:23 GMT
EXPOSE 4222 6222 8222
# Tue, 13 Jun 2023 22:33:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Jun 2023 22:33:23 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:08409d4172603f40b56eb6b76240a1e6bd78baa0e96590dc7ff76c5f1a093af2`  
		Last Modified: Tue, 09 May 2023 23:11:23 GMT  
		Size: 3.3 MB (3342848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf2d0fd688338eb8ef69b776354053dd65c78ae5e4c3cc2e15fc586f51942d89`  
		Last Modified: Tue, 13 Jun 2023 22:34:38 GMT  
		Size: 5.0 MB (4971650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee9d7fff35b08386d1a65e0e1fa0a81bcc5877d1024bd16ca00f0af62137cdc4`  
		Last Modified: Tue, 13 Jun 2023 22:34:37 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63543f616abdbde1673d999e8e046e0f59aa734ab23d6acabdf42a9756f8c357`  
		Last Modified: Tue, 13 Jun 2023 22:34:37 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:latest`

```console
$ docker pull nats@sha256:a600ddb07ea351ff9a7d0a49f7cc8fcd930c232d55f7c18f17378c3b4f7a83e7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.4377; amd64

### `nats:latest` - linux; amd64

```console
$ docker pull nats@sha256:d7a57514cf7a0949ab8e63985f040f1fbaa01aa70aa50d8485f796a9a8dead08
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5117129 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4bd1a8b681814e86af7f1b07aa7178abd74163b5101ad1f855420c25d4afae5e`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 18 May 2023 21:19:59 GMT
COPY file:a3e4cfa40e3f87cbc1a2427fe9e77a182eed251b7a2f3037b894ac919acda56d in /nats-server 
# Thu, 18 May 2023 21:19:59 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 18 May 2023 21:19:59 GMT
EXPOSE 4222 6222 8222
# Thu, 18 May 2023 21:19:59 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 18 May 2023 21:19:59 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 18 May 2023 21:19:59 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:e7f86c5b152db9b1815749cb2d298d36014c2905070ae66128b67029b4b31780`  
		Last Modified: Thu, 18 May 2023 21:20:38 GMT  
		Size: 5.1 MB (5116621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:623ce2c40f365197112db5bf1e3ed9b09b631da2058b456f99a50a5890fdda44`  
		Last Modified: Thu, 18 May 2023 21:20:37 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm variant v6

```console
$ docker pull nats@sha256:f26f23aad2feedaeaca9df38eca5559b431fbb8ed841789b1e6b2c3c84ffa79b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4884857 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8ae95e37599ef924cfe3d5890b3af209e09951179f6672d35af6811876e61253`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 13 Jun 2023 21:49:33 GMT
COPY file:e5bb5e8247a1c4bdb92d70dc84443f615728207816f4c76763893029e98fe987 in /nats-server 
# Tue, 13 Jun 2023 21:49:33 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 13 Jun 2023 21:49:33 GMT
EXPOSE 4222 6222 8222
# Tue, 13 Jun 2023 21:49:33 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 13 Jun 2023 21:49:33 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 13 Jun 2023 21:49:33 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:7f1a7a7f3e313c163918678d53d48af6476087e63070356ad38ff1c041606bca`  
		Last Modified: Tue, 13 Jun 2023 21:50:13 GMT  
		Size: 4.9 MB (4884348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9af05a149bcbd29ea7705539c8b49e2c00b5883848519f3929bf4c4dc424022e`  
		Last Modified: Tue, 13 Jun 2023 21:50:12 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm variant v7

```console
$ docker pull nats@sha256:94bf4a62f52fd647adb621d2d584e9c48aea06b124fb81cd59afed50252071bd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4874864 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a8b8de1397d0af96648a1d02610dc54a066633c75eb548fc6be7e0d15497c3c`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 18 May 2023 21:57:50 GMT
COPY file:31e26234e2abf1c16cd5869033f07320118e6dc458af341f37a27a3d12ffbc65 in /nats-server 
# Thu, 18 May 2023 21:57:50 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 18 May 2023 21:57:51 GMT
EXPOSE 4222 6222 8222
# Thu, 18 May 2023 21:57:51 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 18 May 2023 21:57:51 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 18 May 2023 21:57:51 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b6209c6f59228d4816baef6c05a38f68693937e6c86969581c57a1c7b68ccb40`  
		Last Modified: Thu, 18 May 2023 21:58:28 GMT  
		Size: 4.9 MB (4874355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c69c5a4696da201d78c2dae749a6bce01c3a924afbdfa7e87c6797b8db238d4d`  
		Last Modified: Thu, 18 May 2023 21:58:27 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:edbf69c3a8dab18af6eefffc70fcea84205a4397632e23fbde4cca5fe03446ff
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4688025 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b395b40ae1ff951faa10f8f5c05810b77b0a03c2ef5a8eaa8bc443497b52348d`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 13 Jun 2023 22:34:13 GMT
COPY file:0fec8537fba7c573dbe20b854a6b32d8b0940e46f9e81c41611d447b82a034bc in /nats-server 
# Tue, 13 Jun 2023 22:34:13 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 13 Jun 2023 22:34:13 GMT
EXPOSE 4222 6222 8222
# Tue, 13 Jun 2023 22:34:14 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 13 Jun 2023 22:34:14 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 13 Jun 2023 22:34:14 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:2cce796fcd5a4e60d6ca871c71b29485d80a6babd1c43a056db0b52aa6e904b6`  
		Last Modified: Tue, 13 Jun 2023 22:34:58 GMT  
		Size: 4.7 MB (4687516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22153c0efa275cbe62c344213d16db73c5732467534b2a316e379bdd77324d29`  
		Last Modified: Tue, 13 Jun 2023 22:34:57 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - windows version 10.0.17763.4377; amd64

```console
$ docker pull nats@sha256:ffdbc972ae083180acdcc8d74756ed6c94b032bce6d7ec4c224f8343919f232d
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.6 MB (109564530 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b23b2cb10135235e109abd0ca99d3cf4027f72a1c246c873707190f54bffec4`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 05 May 2023 11:29:01 GMT
RUN Apply image 10.0.17763.4377
# Wed, 10 May 2023 02:43:57 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Tue, 13 Jun 2023 22:18:13 GMT
RUN cmd /S /C #(nop) COPY file:e92fb324fb1e715aaa4f213ef42afe80c4a76690e3b2d439bee510cb2ae47cd5 in C:\nats-server.exe 
# Tue, 13 Jun 2023 22:18:14 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Tue, 13 Jun 2023 22:18:15 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Tue, 13 Jun 2023 22:18:15 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 13 Jun 2023 22:18:16 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:f7885e3a2dfeae5eea125d00da688c29930a05e4d904884fe43e093ce6223664`  
		Last Modified: Wed, 10 May 2023 01:49:01 GMT  
		Size: 104.4 MB (104383998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9af27dd7e62b7d94fa31a7c9efd9a532c42db89ec01fdb7fe430043ceabc5b4`  
		Last Modified: Wed, 10 May 2023 02:49:27 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74147f1370eb575d5bc03ac650054b5dcc36d7b40bf7706dde9d9d159d10e1a8`  
		Last Modified: Tue, 13 Jun 2023 22:19:04 GMT  
		Size: 5.2 MB (5174125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c441087537bf6a2963fdc58d12d836350044355df07fa9d696fe6e61819cc0ea`  
		Last Modified: Tue, 13 Jun 2023 22:19:02 GMT  
		Size: 1.8 KB (1803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94f7788277dc1622146a19b5407e20fc8eb003cd62b331460221d930e9154d31`  
		Last Modified: Tue, 13 Jun 2023 22:19:02 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b991262b6e730687a02c0d68ac25bc2dcf4dff69f1e9db5315f654387aab754`  
		Last Modified: Tue, 13 Jun 2023 22:19:02 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c322d11690204cb63afb856a65f1fdd8016ebd23989de8952a6ecb7f6737f17e`  
		Last Modified: Tue, 13 Jun 2023 22:19:02 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:linux`

```console
$ docker pull nats@sha256:451705c3735c55b4f7659f8690159fb8f4eb3138e0d4e1b921e4ae325fe46788
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:linux` - linux; amd64

```console
$ docker pull nats@sha256:d7a57514cf7a0949ab8e63985f040f1fbaa01aa70aa50d8485f796a9a8dead08
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5117129 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4bd1a8b681814e86af7f1b07aa7178abd74163b5101ad1f855420c25d4afae5e`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 18 May 2023 21:19:59 GMT
COPY file:a3e4cfa40e3f87cbc1a2427fe9e77a182eed251b7a2f3037b894ac919acda56d in /nats-server 
# Thu, 18 May 2023 21:19:59 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 18 May 2023 21:19:59 GMT
EXPOSE 4222 6222 8222
# Thu, 18 May 2023 21:19:59 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 18 May 2023 21:19:59 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 18 May 2023 21:19:59 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:e7f86c5b152db9b1815749cb2d298d36014c2905070ae66128b67029b4b31780`  
		Last Modified: Thu, 18 May 2023 21:20:38 GMT  
		Size: 5.1 MB (5116621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:623ce2c40f365197112db5bf1e3ed9b09b631da2058b456f99a50a5890fdda44`  
		Last Modified: Thu, 18 May 2023 21:20:37 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:f26f23aad2feedaeaca9df38eca5559b431fbb8ed841789b1e6b2c3c84ffa79b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4884857 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8ae95e37599ef924cfe3d5890b3af209e09951179f6672d35af6811876e61253`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 13 Jun 2023 21:49:33 GMT
COPY file:e5bb5e8247a1c4bdb92d70dc84443f615728207816f4c76763893029e98fe987 in /nats-server 
# Tue, 13 Jun 2023 21:49:33 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 13 Jun 2023 21:49:33 GMT
EXPOSE 4222 6222 8222
# Tue, 13 Jun 2023 21:49:33 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 13 Jun 2023 21:49:33 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 13 Jun 2023 21:49:33 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:7f1a7a7f3e313c163918678d53d48af6476087e63070356ad38ff1c041606bca`  
		Last Modified: Tue, 13 Jun 2023 21:50:13 GMT  
		Size: 4.9 MB (4884348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9af05a149bcbd29ea7705539c8b49e2c00b5883848519f3929bf4c4dc424022e`  
		Last Modified: Tue, 13 Jun 2023 21:50:12 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:94bf4a62f52fd647adb621d2d584e9c48aea06b124fb81cd59afed50252071bd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4874864 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a8b8de1397d0af96648a1d02610dc54a066633c75eb548fc6be7e0d15497c3c`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 18 May 2023 21:57:50 GMT
COPY file:31e26234e2abf1c16cd5869033f07320118e6dc458af341f37a27a3d12ffbc65 in /nats-server 
# Thu, 18 May 2023 21:57:50 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 18 May 2023 21:57:51 GMT
EXPOSE 4222 6222 8222
# Thu, 18 May 2023 21:57:51 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 18 May 2023 21:57:51 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 18 May 2023 21:57:51 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b6209c6f59228d4816baef6c05a38f68693937e6c86969581c57a1c7b68ccb40`  
		Last Modified: Thu, 18 May 2023 21:58:28 GMT  
		Size: 4.9 MB (4874355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c69c5a4696da201d78c2dae749a6bce01c3a924afbdfa7e87c6797b8db238d4d`  
		Last Modified: Thu, 18 May 2023 21:58:27 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:edbf69c3a8dab18af6eefffc70fcea84205a4397632e23fbde4cca5fe03446ff
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4688025 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b395b40ae1ff951faa10f8f5c05810b77b0a03c2ef5a8eaa8bc443497b52348d`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 13 Jun 2023 22:34:13 GMT
COPY file:0fec8537fba7c573dbe20b854a6b32d8b0940e46f9e81c41611d447b82a034bc in /nats-server 
# Tue, 13 Jun 2023 22:34:13 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 13 Jun 2023 22:34:13 GMT
EXPOSE 4222 6222 8222
# Tue, 13 Jun 2023 22:34:14 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 13 Jun 2023 22:34:14 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 13 Jun 2023 22:34:14 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:2cce796fcd5a4e60d6ca871c71b29485d80a6babd1c43a056db0b52aa6e904b6`  
		Last Modified: Tue, 13 Jun 2023 22:34:58 GMT  
		Size: 4.7 MB (4687516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22153c0efa275cbe62c344213d16db73c5732467534b2a316e379bdd77324d29`  
		Last Modified: Tue, 13 Jun 2023 22:34:57 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:nanoserver`

```console
$ docker pull nats@sha256:0a384e9a7d76bb1288a9b091976b9fa61e78c22143d6a07415707fdd6123219c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4377; amd64

### `nats:nanoserver` - windows version 10.0.17763.4377; amd64

```console
$ docker pull nats@sha256:ffdbc972ae083180acdcc8d74756ed6c94b032bce6d7ec4c224f8343919f232d
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.6 MB (109564530 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b23b2cb10135235e109abd0ca99d3cf4027f72a1c246c873707190f54bffec4`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 05 May 2023 11:29:01 GMT
RUN Apply image 10.0.17763.4377
# Wed, 10 May 2023 02:43:57 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Tue, 13 Jun 2023 22:18:13 GMT
RUN cmd /S /C #(nop) COPY file:e92fb324fb1e715aaa4f213ef42afe80c4a76690e3b2d439bee510cb2ae47cd5 in C:\nats-server.exe 
# Tue, 13 Jun 2023 22:18:14 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Tue, 13 Jun 2023 22:18:15 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Tue, 13 Jun 2023 22:18:15 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 13 Jun 2023 22:18:16 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:f7885e3a2dfeae5eea125d00da688c29930a05e4d904884fe43e093ce6223664`  
		Last Modified: Wed, 10 May 2023 01:49:01 GMT  
		Size: 104.4 MB (104383998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9af27dd7e62b7d94fa31a7c9efd9a532c42db89ec01fdb7fe430043ceabc5b4`  
		Last Modified: Wed, 10 May 2023 02:49:27 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74147f1370eb575d5bc03ac650054b5dcc36d7b40bf7706dde9d9d159d10e1a8`  
		Last Modified: Tue, 13 Jun 2023 22:19:04 GMT  
		Size: 5.2 MB (5174125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c441087537bf6a2963fdc58d12d836350044355df07fa9d696fe6e61819cc0ea`  
		Last Modified: Tue, 13 Jun 2023 22:19:02 GMT  
		Size: 1.8 KB (1803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94f7788277dc1622146a19b5407e20fc8eb003cd62b331460221d930e9154d31`  
		Last Modified: Tue, 13 Jun 2023 22:19:02 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b991262b6e730687a02c0d68ac25bc2dcf4dff69f1e9db5315f654387aab754`  
		Last Modified: Tue, 13 Jun 2023 22:19:02 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c322d11690204cb63afb856a65f1fdd8016ebd23989de8952a6ecb7f6737f17e`  
		Last Modified: Tue, 13 Jun 2023 22:19:02 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:nanoserver-1809`

```console
$ docker pull nats@sha256:0a384e9a7d76bb1288a9b091976b9fa61e78c22143d6a07415707fdd6123219c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4377; amd64

### `nats:nanoserver-1809` - windows version 10.0.17763.4377; amd64

```console
$ docker pull nats@sha256:ffdbc972ae083180acdcc8d74756ed6c94b032bce6d7ec4c224f8343919f232d
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.6 MB (109564530 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b23b2cb10135235e109abd0ca99d3cf4027f72a1c246c873707190f54bffec4`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 05 May 2023 11:29:01 GMT
RUN Apply image 10.0.17763.4377
# Wed, 10 May 2023 02:43:57 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Tue, 13 Jun 2023 22:18:13 GMT
RUN cmd /S /C #(nop) COPY file:e92fb324fb1e715aaa4f213ef42afe80c4a76690e3b2d439bee510cb2ae47cd5 in C:\nats-server.exe 
# Tue, 13 Jun 2023 22:18:14 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Tue, 13 Jun 2023 22:18:15 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Tue, 13 Jun 2023 22:18:15 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 13 Jun 2023 22:18:16 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:f7885e3a2dfeae5eea125d00da688c29930a05e4d904884fe43e093ce6223664`  
		Last Modified: Wed, 10 May 2023 01:49:01 GMT  
		Size: 104.4 MB (104383998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9af27dd7e62b7d94fa31a7c9efd9a532c42db89ec01fdb7fe430043ceabc5b4`  
		Last Modified: Wed, 10 May 2023 02:49:27 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74147f1370eb575d5bc03ac650054b5dcc36d7b40bf7706dde9d9d159d10e1a8`  
		Last Modified: Tue, 13 Jun 2023 22:19:04 GMT  
		Size: 5.2 MB (5174125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c441087537bf6a2963fdc58d12d836350044355df07fa9d696fe6e61819cc0ea`  
		Last Modified: Tue, 13 Jun 2023 22:19:02 GMT  
		Size: 1.8 KB (1803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94f7788277dc1622146a19b5407e20fc8eb003cd62b331460221d930e9154d31`  
		Last Modified: Tue, 13 Jun 2023 22:19:02 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b991262b6e730687a02c0d68ac25bc2dcf4dff69f1e9db5315f654387aab754`  
		Last Modified: Tue, 13 Jun 2023 22:19:02 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c322d11690204cb63afb856a65f1fdd8016ebd23989de8952a6ecb7f6737f17e`  
		Last Modified: Tue, 13 Jun 2023 22:19:02 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:scratch`

```console
$ docker pull nats@sha256:451705c3735c55b4f7659f8690159fb8f4eb3138e0d4e1b921e4ae325fe46788
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:scratch` - linux; amd64

```console
$ docker pull nats@sha256:d7a57514cf7a0949ab8e63985f040f1fbaa01aa70aa50d8485f796a9a8dead08
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5117129 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4bd1a8b681814e86af7f1b07aa7178abd74163b5101ad1f855420c25d4afae5e`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 18 May 2023 21:19:59 GMT
COPY file:a3e4cfa40e3f87cbc1a2427fe9e77a182eed251b7a2f3037b894ac919acda56d in /nats-server 
# Thu, 18 May 2023 21:19:59 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 18 May 2023 21:19:59 GMT
EXPOSE 4222 6222 8222
# Thu, 18 May 2023 21:19:59 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 18 May 2023 21:19:59 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 18 May 2023 21:19:59 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:e7f86c5b152db9b1815749cb2d298d36014c2905070ae66128b67029b4b31780`  
		Last Modified: Thu, 18 May 2023 21:20:38 GMT  
		Size: 5.1 MB (5116621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:623ce2c40f365197112db5bf1e3ed9b09b631da2058b456f99a50a5890fdda44`  
		Last Modified: Thu, 18 May 2023 21:20:37 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:f26f23aad2feedaeaca9df38eca5559b431fbb8ed841789b1e6b2c3c84ffa79b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4884857 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8ae95e37599ef924cfe3d5890b3af209e09951179f6672d35af6811876e61253`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 13 Jun 2023 21:49:33 GMT
COPY file:e5bb5e8247a1c4bdb92d70dc84443f615728207816f4c76763893029e98fe987 in /nats-server 
# Tue, 13 Jun 2023 21:49:33 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 13 Jun 2023 21:49:33 GMT
EXPOSE 4222 6222 8222
# Tue, 13 Jun 2023 21:49:33 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 13 Jun 2023 21:49:33 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 13 Jun 2023 21:49:33 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:7f1a7a7f3e313c163918678d53d48af6476087e63070356ad38ff1c041606bca`  
		Last Modified: Tue, 13 Jun 2023 21:50:13 GMT  
		Size: 4.9 MB (4884348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9af05a149bcbd29ea7705539c8b49e2c00b5883848519f3929bf4c4dc424022e`  
		Last Modified: Tue, 13 Jun 2023 21:50:12 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:94bf4a62f52fd647adb621d2d584e9c48aea06b124fb81cd59afed50252071bd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4874864 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a8b8de1397d0af96648a1d02610dc54a066633c75eb548fc6be7e0d15497c3c`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 18 May 2023 21:57:50 GMT
COPY file:31e26234e2abf1c16cd5869033f07320118e6dc458af341f37a27a3d12ffbc65 in /nats-server 
# Thu, 18 May 2023 21:57:50 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 18 May 2023 21:57:51 GMT
EXPOSE 4222 6222 8222
# Thu, 18 May 2023 21:57:51 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 18 May 2023 21:57:51 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 18 May 2023 21:57:51 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b6209c6f59228d4816baef6c05a38f68693937e6c86969581c57a1c7b68ccb40`  
		Last Modified: Thu, 18 May 2023 21:58:28 GMT  
		Size: 4.9 MB (4874355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c69c5a4696da201d78c2dae749a6bce01c3a924afbdfa7e87c6797b8db238d4d`  
		Last Modified: Thu, 18 May 2023 21:58:27 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:edbf69c3a8dab18af6eefffc70fcea84205a4397632e23fbde4cca5fe03446ff
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4688025 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b395b40ae1ff951faa10f8f5c05810b77b0a03c2ef5a8eaa8bc443497b52348d`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 13 Jun 2023 22:34:13 GMT
COPY file:0fec8537fba7c573dbe20b854a6b32d8b0940e46f9e81c41611d447b82a034bc in /nats-server 
# Tue, 13 Jun 2023 22:34:13 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 13 Jun 2023 22:34:13 GMT
EXPOSE 4222 6222 8222
# Tue, 13 Jun 2023 22:34:14 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 13 Jun 2023 22:34:14 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 13 Jun 2023 22:34:14 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:2cce796fcd5a4e60d6ca871c71b29485d80a6babd1c43a056db0b52aa6e904b6`  
		Last Modified: Tue, 13 Jun 2023 22:34:58 GMT  
		Size: 4.7 MB (4687516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22153c0efa275cbe62c344213d16db73c5732467534b2a316e379bdd77324d29`  
		Last Modified: Tue, 13 Jun 2023 22:34:57 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:windowsservercore`

```console
$ docker pull nats@sha256:85d1368e7f6f675346e070014b558c792541dfc94c5bd2d9f919736ddaa90dee
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4377; amd64

### `nats:windowsservercore` - windows version 10.0.17763.4377; amd64

```console
$ docker pull nats@sha256:6116850a9313d0b910b0db095a33e7297f06b633f1e1fb386db4fd023e23985e
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2077962593 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d0359af1b68ffc80fd1b560b7235f9eb6d3562810001343595480a3f55a0e043`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Fri, 05 May 2023 12:05:28 GMT
RUN Install update 10.0.17763.4377
# Wed, 10 May 2023 01:56:29 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 May 2023 02:40:26 GMT
ENV NATS_DOCKERIZED=1
# Tue, 13 Jun 2023 22:15:14 GMT
ENV NATS_SERVER=2.9.18
# Tue, 13 Jun 2023 22:15:15 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.9.18/nats-server-v2.9.18-windows-amd64.zip
# Tue, 13 Jun 2023 22:15:16 GMT
ENV NATS_SERVER_SHASUM=139c2d63193d7df39894b144fb08a40e15548f89087e1932617239d36ab0c901
# Tue, 13 Jun 2023 22:16:20 GMT
RUN Set-PSDebug -Trace 2
# Tue, 13 Jun 2023 22:17:54 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Tue, 13 Jun 2023 22:17:54 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Tue, 13 Jun 2023 22:17:55 GMT
EXPOSE 4222 6222 8222
# Tue, 13 Jun 2023 22:17:56 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 13 Jun 2023 22:17:57 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e01de39a0c44e24aa1912078d32ee54389b71154e509138cc4f5d1de42e7a32a`  
		Last Modified: Wed, 10 May 2023 01:47:41 GMT  
		Size: 364.1 MB (364091294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2a89be60a77cd8d520ec5f03d703ddbc15675dd1df4d95e041032cf08960af5`  
		Last Modified: Wed, 10 May 2023 02:23:36 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:446cee93ab2781cfc08e135a3a7ab166e5342ee6817c34fb47e0662c085bbc29`  
		Last Modified: Wed, 10 May 2023 02:49:15 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a057529e52e0e6010038d1fe4fc95821b317ee7379ce74a6ccdaeb4397c6580`  
		Last Modified: Tue, 13 Jun 2023 22:18:48 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c741cf7b9012d8cb23e39f90427fded64f0e4de03039ddf48b77f15ef89d7ae0`  
		Last Modified: Tue, 13 Jun 2023 22:18:48 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:208c61957253b4017f86095081c6827718ad7b858e26d20a163e66ab10ed6a92`  
		Last Modified: Tue, 13 Jun 2023 22:18:48 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3e815afe033119fccd2887c2236ea581cbab8d6d5f4b146e2f03a35c99e150c`  
		Last Modified: Tue, 13 Jun 2023 22:18:48 GMT  
		Size: 448.8 KB (448805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c786064ca9923a9e7e6f5d6e0b3a08cb4c345cb8b37053a51ffe1ed92baa434f`  
		Last Modified: Tue, 13 Jun 2023 22:18:47 GMT  
		Size: 5.5 MB (5465263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ca1ecd70300344a64c5b09e7e0ef4325d7d434f3aee3b1d7845b33db7c8b8c6`  
		Last Modified: Tue, 13 Jun 2023 22:18:46 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8b2ae653f72ce5dc355f193098cdcdeb2cd780c78bed2991512625ead60fe16`  
		Last Modified: Tue, 13 Jun 2023 22:18:46 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d20c4caf3b063c53361edeec4547495178a5ee257f0afb5d83edb3a4d0b55bf`  
		Last Modified: Tue, 13 Jun 2023 22:18:46 GMT  
		Size: 1.4 KB (1374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6cf54e3a0a4a7d1916f3634aa394fdee5078f370ce0f19f05621468dbb0e6f4`  
		Last Modified: Tue, 13 Jun 2023 22:18:46 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:windowsservercore-1809`

```console
$ docker pull nats@sha256:85d1368e7f6f675346e070014b558c792541dfc94c5bd2d9f919736ddaa90dee
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4377; amd64

### `nats:windowsservercore-1809` - windows version 10.0.17763.4377; amd64

```console
$ docker pull nats@sha256:6116850a9313d0b910b0db095a33e7297f06b633f1e1fb386db4fd023e23985e
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2077962593 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d0359af1b68ffc80fd1b560b7235f9eb6d3562810001343595480a3f55a0e043`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Fri, 05 May 2023 12:05:28 GMT
RUN Install update 10.0.17763.4377
# Wed, 10 May 2023 01:56:29 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 May 2023 02:40:26 GMT
ENV NATS_DOCKERIZED=1
# Tue, 13 Jun 2023 22:15:14 GMT
ENV NATS_SERVER=2.9.18
# Tue, 13 Jun 2023 22:15:15 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.9.18/nats-server-v2.9.18-windows-amd64.zip
# Tue, 13 Jun 2023 22:15:16 GMT
ENV NATS_SERVER_SHASUM=139c2d63193d7df39894b144fb08a40e15548f89087e1932617239d36ab0c901
# Tue, 13 Jun 2023 22:16:20 GMT
RUN Set-PSDebug -Trace 2
# Tue, 13 Jun 2023 22:17:54 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Tue, 13 Jun 2023 22:17:54 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Tue, 13 Jun 2023 22:17:55 GMT
EXPOSE 4222 6222 8222
# Tue, 13 Jun 2023 22:17:56 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 13 Jun 2023 22:17:57 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e01de39a0c44e24aa1912078d32ee54389b71154e509138cc4f5d1de42e7a32a`  
		Last Modified: Wed, 10 May 2023 01:47:41 GMT  
		Size: 364.1 MB (364091294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2a89be60a77cd8d520ec5f03d703ddbc15675dd1df4d95e041032cf08960af5`  
		Last Modified: Wed, 10 May 2023 02:23:36 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:446cee93ab2781cfc08e135a3a7ab166e5342ee6817c34fb47e0662c085bbc29`  
		Last Modified: Wed, 10 May 2023 02:49:15 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a057529e52e0e6010038d1fe4fc95821b317ee7379ce74a6ccdaeb4397c6580`  
		Last Modified: Tue, 13 Jun 2023 22:18:48 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c741cf7b9012d8cb23e39f90427fded64f0e4de03039ddf48b77f15ef89d7ae0`  
		Last Modified: Tue, 13 Jun 2023 22:18:48 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:208c61957253b4017f86095081c6827718ad7b858e26d20a163e66ab10ed6a92`  
		Last Modified: Tue, 13 Jun 2023 22:18:48 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3e815afe033119fccd2887c2236ea581cbab8d6d5f4b146e2f03a35c99e150c`  
		Last Modified: Tue, 13 Jun 2023 22:18:48 GMT  
		Size: 448.8 KB (448805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c786064ca9923a9e7e6f5d6e0b3a08cb4c345cb8b37053a51ffe1ed92baa434f`  
		Last Modified: Tue, 13 Jun 2023 22:18:47 GMT  
		Size: 5.5 MB (5465263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ca1ecd70300344a64c5b09e7e0ef4325d7d434f3aee3b1d7845b33db7c8b8c6`  
		Last Modified: Tue, 13 Jun 2023 22:18:46 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8b2ae653f72ce5dc355f193098cdcdeb2cd780c78bed2991512625ead60fe16`  
		Last Modified: Tue, 13 Jun 2023 22:18:46 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d20c4caf3b063c53361edeec4547495178a5ee257f0afb5d83edb3a4d0b55bf`  
		Last Modified: Tue, 13 Jun 2023 22:18:46 GMT  
		Size: 1.4 KB (1374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6cf54e3a0a4a7d1916f3634aa394fdee5078f370ce0f19f05621468dbb0e6f4`  
		Last Modified: Tue, 13 Jun 2023 22:18:46 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
