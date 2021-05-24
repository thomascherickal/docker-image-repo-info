<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `nats-streaming`

-	[`nats-streaming:0.21`](#nats-streaming021)
-	[`nats-streaming:0.21-alpine`](#nats-streaming021-alpine)
-	[`nats-streaming:0.21-alpine3.13`](#nats-streaming021-alpine313)
-	[`nats-streaming:0.21-linux`](#nats-streaming021-linux)
-	[`nats-streaming:0.21-nanoserver`](#nats-streaming021-nanoserver)
-	[`nats-streaming:0.21-nanoserver-1809`](#nats-streaming021-nanoserver-1809)
-	[`nats-streaming:0.21-scratch`](#nats-streaming021-scratch)
-	[`nats-streaming:0.21-windowsservercore`](#nats-streaming021-windowsservercore)
-	[`nats-streaming:0.21-windowsservercore-1809`](#nats-streaming021-windowsservercore-1809)
-	[`nats-streaming:0.21-windowsservercore-ltsc2016`](#nats-streaming021-windowsservercore-ltsc2016)
-	[`nats-streaming:0.21.2`](#nats-streaming0212)
-	[`nats-streaming:0.21.2-alpine`](#nats-streaming0212-alpine)
-	[`nats-streaming:0.21.2-alpine3.13`](#nats-streaming0212-alpine313)
-	[`nats-streaming:0.21.2-linux`](#nats-streaming0212-linux)
-	[`nats-streaming:0.21.2-nanoserver`](#nats-streaming0212-nanoserver)
-	[`nats-streaming:0.21.2-nanoserver-1809`](#nats-streaming0212-nanoserver-1809)
-	[`nats-streaming:0.21.2-scratch`](#nats-streaming0212-scratch)
-	[`nats-streaming:0.21.2-windowsservercore`](#nats-streaming0212-windowsservercore)
-	[`nats-streaming:0.21.2-windowsservercore-1809`](#nats-streaming0212-windowsservercore-1809)
-	[`nats-streaming:0.21.2-windowsservercore-ltsc2016`](#nats-streaming0212-windowsservercore-ltsc2016)
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
$ docker pull nats-streaming@sha256:8e9036a7e32179bf55236241656e9555336215146d30129b5ac664f94fd73ed6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.1935; amd64

### `nats-streaming:0.21` - linux; amd64

```console
$ docker pull nats-streaming@sha256:883d4d7a47db4d1c911cf0c23dad30011b46727297d1158bede3d833455a49e4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.7 MB (5680535 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d1e123176c313a4b94f8c0fdf6cac9abdd85a1bd6edf3f7cc6e7ed61852d19a`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Fri, 16 Apr 2021 21:25:32 GMT
COPY file:aefc6cbeadb611214d28b81a278a791c774a4bbc969528522aae7abe7c4e2784 in /nats-streaming-server 
# Fri, 16 Apr 2021 21:25:32 GMT
EXPOSE 4222 8222
# Fri, 16 Apr 2021 21:25:32 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Fri, 16 Apr 2021 21:25:33 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:087a668f89c4000c166ca5a16dd40fee8206986ce9b47a92d224b78214f3db5c`  
		Last Modified: Fri, 16 Apr 2021 21:26:16 GMT  
		Size: 5.7 MB (5680535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.21` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:9dc93ca8dad040be30fe0949d19f04a6b1775750838d70d2fb12f3aa9f40b4f8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.3 MB (5253054 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba356cbd8fdcd90e529d00104791d07c50c101937487a0b8647b06226bfdef9a`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Fri, 16 Apr 2021 21:02:53 GMT
COPY file:c58b6e2180eb9d24d595f35c2205c2d9b4f80315beb0f166e20a7340cf3f2536 in /nats-streaming-server 
# Fri, 16 Apr 2021 21:03:00 GMT
EXPOSE 4222 8222
# Fri, 16 Apr 2021 21:03:04 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Fri, 16 Apr 2021 21:03:07 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:3542c02ee947256ff50165b76289b4dd90e7c82bfb7b0b983b4d66d4b1128e9a`  
		Last Modified: Fri, 16 Apr 2021 21:03:44 GMT  
		Size: 5.3 MB (5253054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.21` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:10f5838646402cebd5c40f8f02991aad0ca3767b13b3024054e5e04026d3c778
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5246280 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:409bfb98a0a11b06fb4c8a044cda742270c21f5082ef80b63e7893cb4ce2f9c3`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Fri, 16 Apr 2021 21:00:05 GMT
COPY file:7ad2a856b4d75bdc56fbd35738819610cc3c26111897fc883c3af7db16d4fa87 in /nats-streaming-server 
# Fri, 16 Apr 2021 21:00:07 GMT
EXPOSE 4222 8222
# Fri, 16 Apr 2021 21:00:09 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Fri, 16 Apr 2021 21:00:10 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:76bf01e9a89a0de09d5ab72dd4ec7e4c9f561a27756ceb73bf0365f192de2d18`  
		Last Modified: Fri, 16 Apr 2021 21:01:13 GMT  
		Size: 5.2 MB (5246280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.21` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:3bf4856546fa4657b125293b8ed701a22dd3861cd532a14281d7726210c726c9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5170831 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e4acb30c8790d9ef8af675772eda5d9f3903a662d29132ef140463453eeb717`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Fri, 16 Apr 2021 21:48:04 GMT
COPY file:b02a357b6e9250e52099dcc91c6a9a78682a192bd0850fabc93d5cdacb6fcfb3 in /nats-streaming-server 
# Fri, 16 Apr 2021 21:48:05 GMT
EXPOSE 4222 8222
# Fri, 16 Apr 2021 21:48:06 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Fri, 16 Apr 2021 21:48:07 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:fe1641db2bf227918d02728a21bd3b53989018d9c796246d3b96fcbbf75ded32`  
		Last Modified: Fri, 16 Apr 2021 21:48:50 GMT  
		Size: 5.2 MB (5170831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.21` - windows version 10.0.17763.1935; amd64

```console
$ docker pull nats-streaming@sha256:881fbff9b8ea5b5dce5d1e1fb341a4ab9a9caab12b0faf072dc89f9ab61792e9
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.2 MB (107191037 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9db19cc378f4cdf654406f9ff0a58704fbec29c0b23fa37b4919bcedd9a0a02`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Fri, 07 May 2021 11:54:57 GMT
RUN Apply image 1809-amd64
# Wed, 12 May 2021 15:44:03 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 12 May 2021 20:11:27 GMT
RUN cmd /S /C #(nop) COPY file:adacf7e54ef5a782ae37764b59883ad6a48b32c36c576816360f94cba82ba458 in C:\nats-streaming-server.exe 
# Wed, 12 May 2021 20:11:28 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 12 May 2021 20:11:29 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 12 May 2021 20:11:30 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:b9043d31610e0dfa43b1afe286f8918b6e3bf69ece50f44424b29d48f20aa662`  
		Size: 101.4 MB (101375240 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:95b58e21e5cdf4e2f9e5c87487734458885da325634d72f9c4e6583b353af06f`  
		Last Modified: Wed, 12 May 2021 15:49:02 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab3056c607d4b35216a2f74c2f849eb0c970001dc87bf45f90aea3ca4e8d9f05`  
		Last Modified: Wed, 12 May 2021 20:16:11 GMT  
		Size: 5.8 MB (5811203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:747d370e1cec130d4e6c1a20a9b8d049a93543b695b60a4fc0b5473758786920`  
		Last Modified: Wed, 12 May 2021 20:16:10 GMT  
		Size: 1.2 KB (1178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38d9d67f8ca438fa616690db8fc1087b47f11ad390d7a29761bfc08c67605c85`  
		Last Modified: Wed, 12 May 2021 20:16:10 GMT  
		Size: 1.1 KB (1105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e187a1b2446f3948440517b1cd475bdb32db16b4643b465f30313f8bbfe01d6`  
		Last Modified: Wed, 12 May 2021 20:16:10 GMT  
		Size: 1.2 KB (1161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.21-alpine`

```console
$ docker pull nats-streaming@sha256:d204ac6b58553c9632e9797984adcace87b6539d257754f1d5bdf5e4a2a8d72e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.21-alpine` - linux; amd64

```console
$ docker pull nats-streaming@sha256:402dacbb78f9bf5e9ea249c730f7905caa085ca665782e1cb4c6e7004f597689
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.8 MB (8774780 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f7ad70b17b46627026163460cce06023868f24d36a50cd9c261e7c6cba86e29`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Fri, 16 Apr 2021 21:25:11 GMT
ENV NATS_STREAMING_SERVER=0.21.2
# Fri, 16 Apr 2021 21:25:14 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='56bcfea3c3d7a232dab93ad280ce8f8df87959ac000c7d24ce03dbab2f4c4d2b' ;; 		armhf) natsArch='arm6'; sha256='34d7032ba61724ec55d78cb94a5ed244754509b8b957e1e7e4f0579292c35a7f' ;; 		armv7) natsArch='arm7'; sha256='b4869711408e3823c8818e934bf90d07ed51f350147702b80831fb4fe5a390d2' ;; 		x86_64) natsArch='amd64'; sha256='7a401a3af7eb56a0d1d3b207dc517222697b48cb7e9e524848e62bd13393d23a' ;; 		x86) natsArch='386'; sha256='58aa4cad4c75920522ec0457b79d889f9c740c248647b875254cd1313517620c' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 16 Apr 2021 21:25:14 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Fri, 16 Apr 2021 21:25:15 GMT
EXPOSE 4222 8222
# Fri, 16 Apr 2021 21:25:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Apr 2021 21:25:15 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:269577e93d92e9e558c3607d8b5e74978c939fc643895de15fd70ef06b811323`  
		Last Modified: Fri, 16 Apr 2021 21:25:54 GMT  
		Size: 6.0 MB (5962389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5fa1ca69a5dc5f7aecbfca382d45ab09423bb9d103c6567abc37af7b842073a`  
		Last Modified: Fri, 16 Apr 2021 21:25:54 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.21-alpine` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:e03de3640ce68bbb19cd2b5e8dc2a1454fbba1b369a4c236f09b6630197b6fa0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.2 MB (8156933 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a345ef8cbbe68103787d05c9dbd22742cc95b726776cbf30298c3ca98487b63`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 14 Apr 2021 18:49:39 GMT
ADD file:4479f0a51530e039edf231d87201896dcff908aa542a613cdccb015f93dda8a3 in / 
# Wed, 14 Apr 2021 18:49:40 GMT
CMD ["/bin/sh"]
# Fri, 16 Apr 2021 21:02:04 GMT
ENV NATS_STREAMING_SERVER=0.21.2
# Fri, 16 Apr 2021 21:02:23 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='56bcfea3c3d7a232dab93ad280ce8f8df87959ac000c7d24ce03dbab2f4c4d2b' ;; 		armhf) natsArch='arm6'; sha256='34d7032ba61724ec55d78cb94a5ed244754509b8b957e1e7e4f0579292c35a7f' ;; 		armv7) natsArch='arm7'; sha256='b4869711408e3823c8818e934bf90d07ed51f350147702b80831fb4fe5a390d2' ;; 		x86_64) natsArch='amd64'; sha256='7a401a3af7eb56a0d1d3b207dc517222697b48cb7e9e524848e62bd13393d23a' ;; 		x86) natsArch='386'; sha256='58aa4cad4c75920522ec0457b79d889f9c740c248647b875254cd1313517620c' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 16 Apr 2021 21:02:26 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Fri, 16 Apr 2021 21:02:27 GMT
EXPOSE 4222 8222
# Fri, 16 Apr 2021 21:02:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Apr 2021 21:02:29 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:740c950346cf39c85b52576998695c9b909c24a58a8bb1b64cce91fda3ef1d3a`  
		Last Modified: Wed, 14 Apr 2021 18:50:30 GMT  
		Size: 2.6 MB (2622131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e538f4430325ed9ef756e0e521a859c9466b9b7a45a8662e4f29f1ec5f8c3a7d`  
		Last Modified: Fri, 16 Apr 2021 21:03:32 GMT  
		Size: 5.5 MB (5534381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc165822006c8e13ee1ee6756545e0f021a059f974288d6c953febdeea6a83d3`  
		Last Modified: Fri, 16 Apr 2021 21:03:30 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.21-alpine` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:ea133d32e6510a0d1822a1ea1cfcca41e3cbd747a3d69491aee62319937e892d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.0 MB (7951606 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc13824ee86fb9d0c1609b885378ba366f3883903bfe990fb27464bce6c02686`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 14 Apr 2021 18:57:39 GMT
ADD file:028c5b473d862250586e174c5dd19b37f8fc3bffbc02d888e72df30f32fd6129 in / 
# Wed, 14 Apr 2021 18:57:39 GMT
CMD ["/bin/sh"]
# Fri, 16 Apr 2021 20:59:08 GMT
ENV NATS_STREAMING_SERVER=0.21.2
# Fri, 16 Apr 2021 20:59:12 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='56bcfea3c3d7a232dab93ad280ce8f8df87959ac000c7d24ce03dbab2f4c4d2b' ;; 		armhf) natsArch='arm6'; sha256='34d7032ba61724ec55d78cb94a5ed244754509b8b957e1e7e4f0579292c35a7f' ;; 		armv7) natsArch='arm7'; sha256='b4869711408e3823c8818e934bf90d07ed51f350147702b80831fb4fe5a390d2' ;; 		x86_64) natsArch='amd64'; sha256='7a401a3af7eb56a0d1d3b207dc517222697b48cb7e9e524848e62bd13393d23a' ;; 		x86) natsArch='386'; sha256='58aa4cad4c75920522ec0457b79d889f9c740c248647b875254cd1313517620c' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 16 Apr 2021 20:59:13 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Fri, 16 Apr 2021 20:59:14 GMT
EXPOSE 4222 8222
# Fri, 16 Apr 2021 20:59:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Apr 2021 20:59:16 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:e160e00eb35d5bc2373770873fbc9c8f5706045b0b06bfd1c364fcf69f02e9fe`  
		Last Modified: Wed, 14 Apr 2021 18:58:36 GMT  
		Size: 2.4 MB (2424145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6b86c52fd84fa988d60547be09b11af6fcac2dffa6b340e92b776a0fc89a298`  
		Last Modified: Fri, 16 Apr 2021 21:00:42 GMT  
		Size: 5.5 MB (5527039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7b279e3ce6e5cfc3967a4acbf6dc2563f1715817b059d6f320b53cbc21b74e1`  
		Last Modified: Fri, 16 Apr 2021 21:00:40 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.21-alpine` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:febf36c660fc36bcbf3da9945707f541e81665b0d21a0f1c6c8220543697a757
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.2 MB (8165113 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd79dce90e049636e2513bd55a0b3178cb59197d3dfc53cbed474dbbd5de0f1f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 14 Apr 2021 18:42:37 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Wed, 14 Apr 2021 18:42:38 GMT
CMD ["/bin/sh"]
# Fri, 16 Apr 2021 21:44:03 GMT
ENV NATS_STREAMING_SERVER=0.21.2
# Fri, 16 Apr 2021 21:44:07 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='56bcfea3c3d7a232dab93ad280ce8f8df87959ac000c7d24ce03dbab2f4c4d2b' ;; 		armhf) natsArch='arm6'; sha256='34d7032ba61724ec55d78cb94a5ed244754509b8b957e1e7e4f0579292c35a7f' ;; 		armv7) natsArch='arm7'; sha256='b4869711408e3823c8818e934bf90d07ed51f350147702b80831fb4fe5a390d2' ;; 		x86_64) natsArch='amd64'; sha256='7a401a3af7eb56a0d1d3b207dc517222697b48cb7e9e524848e62bd13393d23a' ;; 		x86) natsArch='386'; sha256='58aa4cad4c75920522ec0457b79d889f9c740c248647b875254cd1313517620c' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 16 Apr 2021 21:44:08 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Fri, 16 Apr 2021 21:44:09 GMT
EXPOSE 4222 8222
# Fri, 16 Apr 2021 21:44:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Apr 2021 21:44:10 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03a1a4dae3b1b310f0231f28f4db383d7605066343274881c5be1300ebe64f51`  
		Last Modified: Fri, 16 Apr 2021 21:48:37 GMT  
		Size: 5.5 MB (5452665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0a06774842e75925d8884fc1ea5a3e83c2c8054d4fb443ad11021c5866b0617`  
		Last Modified: Fri, 16 Apr 2021 21:48:36 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.21-alpine3.13`

```console
$ docker pull nats-streaming@sha256:d204ac6b58553c9632e9797984adcace87b6539d257754f1d5bdf5e4a2a8d72e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.21-alpine3.13` - linux; amd64

```console
$ docker pull nats-streaming@sha256:402dacbb78f9bf5e9ea249c730f7905caa085ca665782e1cb4c6e7004f597689
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.8 MB (8774780 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f7ad70b17b46627026163460cce06023868f24d36a50cd9c261e7c6cba86e29`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Fri, 16 Apr 2021 21:25:11 GMT
ENV NATS_STREAMING_SERVER=0.21.2
# Fri, 16 Apr 2021 21:25:14 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='56bcfea3c3d7a232dab93ad280ce8f8df87959ac000c7d24ce03dbab2f4c4d2b' ;; 		armhf) natsArch='arm6'; sha256='34d7032ba61724ec55d78cb94a5ed244754509b8b957e1e7e4f0579292c35a7f' ;; 		armv7) natsArch='arm7'; sha256='b4869711408e3823c8818e934bf90d07ed51f350147702b80831fb4fe5a390d2' ;; 		x86_64) natsArch='amd64'; sha256='7a401a3af7eb56a0d1d3b207dc517222697b48cb7e9e524848e62bd13393d23a' ;; 		x86) natsArch='386'; sha256='58aa4cad4c75920522ec0457b79d889f9c740c248647b875254cd1313517620c' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 16 Apr 2021 21:25:14 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Fri, 16 Apr 2021 21:25:15 GMT
EXPOSE 4222 8222
# Fri, 16 Apr 2021 21:25:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Apr 2021 21:25:15 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:269577e93d92e9e558c3607d8b5e74978c939fc643895de15fd70ef06b811323`  
		Last Modified: Fri, 16 Apr 2021 21:25:54 GMT  
		Size: 6.0 MB (5962389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5fa1ca69a5dc5f7aecbfca382d45ab09423bb9d103c6567abc37af7b842073a`  
		Last Modified: Fri, 16 Apr 2021 21:25:54 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.21-alpine3.13` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:e03de3640ce68bbb19cd2b5e8dc2a1454fbba1b369a4c236f09b6630197b6fa0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.2 MB (8156933 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a345ef8cbbe68103787d05c9dbd22742cc95b726776cbf30298c3ca98487b63`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 14 Apr 2021 18:49:39 GMT
ADD file:4479f0a51530e039edf231d87201896dcff908aa542a613cdccb015f93dda8a3 in / 
# Wed, 14 Apr 2021 18:49:40 GMT
CMD ["/bin/sh"]
# Fri, 16 Apr 2021 21:02:04 GMT
ENV NATS_STREAMING_SERVER=0.21.2
# Fri, 16 Apr 2021 21:02:23 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='56bcfea3c3d7a232dab93ad280ce8f8df87959ac000c7d24ce03dbab2f4c4d2b' ;; 		armhf) natsArch='arm6'; sha256='34d7032ba61724ec55d78cb94a5ed244754509b8b957e1e7e4f0579292c35a7f' ;; 		armv7) natsArch='arm7'; sha256='b4869711408e3823c8818e934bf90d07ed51f350147702b80831fb4fe5a390d2' ;; 		x86_64) natsArch='amd64'; sha256='7a401a3af7eb56a0d1d3b207dc517222697b48cb7e9e524848e62bd13393d23a' ;; 		x86) natsArch='386'; sha256='58aa4cad4c75920522ec0457b79d889f9c740c248647b875254cd1313517620c' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 16 Apr 2021 21:02:26 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Fri, 16 Apr 2021 21:02:27 GMT
EXPOSE 4222 8222
# Fri, 16 Apr 2021 21:02:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Apr 2021 21:02:29 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:740c950346cf39c85b52576998695c9b909c24a58a8bb1b64cce91fda3ef1d3a`  
		Last Modified: Wed, 14 Apr 2021 18:50:30 GMT  
		Size: 2.6 MB (2622131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e538f4430325ed9ef756e0e521a859c9466b9b7a45a8662e4f29f1ec5f8c3a7d`  
		Last Modified: Fri, 16 Apr 2021 21:03:32 GMT  
		Size: 5.5 MB (5534381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc165822006c8e13ee1ee6756545e0f021a059f974288d6c953febdeea6a83d3`  
		Last Modified: Fri, 16 Apr 2021 21:03:30 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.21-alpine3.13` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:ea133d32e6510a0d1822a1ea1cfcca41e3cbd747a3d69491aee62319937e892d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.0 MB (7951606 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc13824ee86fb9d0c1609b885378ba366f3883903bfe990fb27464bce6c02686`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 14 Apr 2021 18:57:39 GMT
ADD file:028c5b473d862250586e174c5dd19b37f8fc3bffbc02d888e72df30f32fd6129 in / 
# Wed, 14 Apr 2021 18:57:39 GMT
CMD ["/bin/sh"]
# Fri, 16 Apr 2021 20:59:08 GMT
ENV NATS_STREAMING_SERVER=0.21.2
# Fri, 16 Apr 2021 20:59:12 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='56bcfea3c3d7a232dab93ad280ce8f8df87959ac000c7d24ce03dbab2f4c4d2b' ;; 		armhf) natsArch='arm6'; sha256='34d7032ba61724ec55d78cb94a5ed244754509b8b957e1e7e4f0579292c35a7f' ;; 		armv7) natsArch='arm7'; sha256='b4869711408e3823c8818e934bf90d07ed51f350147702b80831fb4fe5a390d2' ;; 		x86_64) natsArch='amd64'; sha256='7a401a3af7eb56a0d1d3b207dc517222697b48cb7e9e524848e62bd13393d23a' ;; 		x86) natsArch='386'; sha256='58aa4cad4c75920522ec0457b79d889f9c740c248647b875254cd1313517620c' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 16 Apr 2021 20:59:13 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Fri, 16 Apr 2021 20:59:14 GMT
EXPOSE 4222 8222
# Fri, 16 Apr 2021 20:59:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Apr 2021 20:59:16 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:e160e00eb35d5bc2373770873fbc9c8f5706045b0b06bfd1c364fcf69f02e9fe`  
		Last Modified: Wed, 14 Apr 2021 18:58:36 GMT  
		Size: 2.4 MB (2424145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6b86c52fd84fa988d60547be09b11af6fcac2dffa6b340e92b776a0fc89a298`  
		Last Modified: Fri, 16 Apr 2021 21:00:42 GMT  
		Size: 5.5 MB (5527039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7b279e3ce6e5cfc3967a4acbf6dc2563f1715817b059d6f320b53cbc21b74e1`  
		Last Modified: Fri, 16 Apr 2021 21:00:40 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.21-alpine3.13` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:febf36c660fc36bcbf3da9945707f541e81665b0d21a0f1c6c8220543697a757
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.2 MB (8165113 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd79dce90e049636e2513bd55a0b3178cb59197d3dfc53cbed474dbbd5de0f1f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 14 Apr 2021 18:42:37 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Wed, 14 Apr 2021 18:42:38 GMT
CMD ["/bin/sh"]
# Fri, 16 Apr 2021 21:44:03 GMT
ENV NATS_STREAMING_SERVER=0.21.2
# Fri, 16 Apr 2021 21:44:07 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='56bcfea3c3d7a232dab93ad280ce8f8df87959ac000c7d24ce03dbab2f4c4d2b' ;; 		armhf) natsArch='arm6'; sha256='34d7032ba61724ec55d78cb94a5ed244754509b8b957e1e7e4f0579292c35a7f' ;; 		armv7) natsArch='arm7'; sha256='b4869711408e3823c8818e934bf90d07ed51f350147702b80831fb4fe5a390d2' ;; 		x86_64) natsArch='amd64'; sha256='7a401a3af7eb56a0d1d3b207dc517222697b48cb7e9e524848e62bd13393d23a' ;; 		x86) natsArch='386'; sha256='58aa4cad4c75920522ec0457b79d889f9c740c248647b875254cd1313517620c' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 16 Apr 2021 21:44:08 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Fri, 16 Apr 2021 21:44:09 GMT
EXPOSE 4222 8222
# Fri, 16 Apr 2021 21:44:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Apr 2021 21:44:10 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03a1a4dae3b1b310f0231f28f4db383d7605066343274881c5be1300ebe64f51`  
		Last Modified: Fri, 16 Apr 2021 21:48:37 GMT  
		Size: 5.5 MB (5452665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0a06774842e75925d8884fc1ea5a3e83c2c8054d4fb443ad11021c5866b0617`  
		Last Modified: Fri, 16 Apr 2021 21:48:36 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.21-linux`

```console
$ docker pull nats-streaming@sha256:2bf298093b69248cb6e82aa7c64d50c1a45480ad23a8ced79a5ddf588ee69102
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.21-linux` - linux; amd64

```console
$ docker pull nats-streaming@sha256:883d4d7a47db4d1c911cf0c23dad30011b46727297d1158bede3d833455a49e4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.7 MB (5680535 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d1e123176c313a4b94f8c0fdf6cac9abdd85a1bd6edf3f7cc6e7ed61852d19a`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Fri, 16 Apr 2021 21:25:32 GMT
COPY file:aefc6cbeadb611214d28b81a278a791c774a4bbc969528522aae7abe7c4e2784 in /nats-streaming-server 
# Fri, 16 Apr 2021 21:25:32 GMT
EXPOSE 4222 8222
# Fri, 16 Apr 2021 21:25:32 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Fri, 16 Apr 2021 21:25:33 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:087a668f89c4000c166ca5a16dd40fee8206986ce9b47a92d224b78214f3db5c`  
		Last Modified: Fri, 16 Apr 2021 21:26:16 GMT  
		Size: 5.7 MB (5680535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.21-linux` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:9dc93ca8dad040be30fe0949d19f04a6b1775750838d70d2fb12f3aa9f40b4f8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.3 MB (5253054 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba356cbd8fdcd90e529d00104791d07c50c101937487a0b8647b06226bfdef9a`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Fri, 16 Apr 2021 21:02:53 GMT
COPY file:c58b6e2180eb9d24d595f35c2205c2d9b4f80315beb0f166e20a7340cf3f2536 in /nats-streaming-server 
# Fri, 16 Apr 2021 21:03:00 GMT
EXPOSE 4222 8222
# Fri, 16 Apr 2021 21:03:04 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Fri, 16 Apr 2021 21:03:07 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:3542c02ee947256ff50165b76289b4dd90e7c82bfb7b0b983b4d66d4b1128e9a`  
		Last Modified: Fri, 16 Apr 2021 21:03:44 GMT  
		Size: 5.3 MB (5253054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.21-linux` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:10f5838646402cebd5c40f8f02991aad0ca3767b13b3024054e5e04026d3c778
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5246280 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:409bfb98a0a11b06fb4c8a044cda742270c21f5082ef80b63e7893cb4ce2f9c3`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Fri, 16 Apr 2021 21:00:05 GMT
COPY file:7ad2a856b4d75bdc56fbd35738819610cc3c26111897fc883c3af7db16d4fa87 in /nats-streaming-server 
# Fri, 16 Apr 2021 21:00:07 GMT
EXPOSE 4222 8222
# Fri, 16 Apr 2021 21:00:09 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Fri, 16 Apr 2021 21:00:10 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:76bf01e9a89a0de09d5ab72dd4ec7e4c9f561a27756ceb73bf0365f192de2d18`  
		Last Modified: Fri, 16 Apr 2021 21:01:13 GMT  
		Size: 5.2 MB (5246280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.21-linux` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:3bf4856546fa4657b125293b8ed701a22dd3861cd532a14281d7726210c726c9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5170831 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e4acb30c8790d9ef8af675772eda5d9f3903a662d29132ef140463453eeb717`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Fri, 16 Apr 2021 21:48:04 GMT
COPY file:b02a357b6e9250e52099dcc91c6a9a78682a192bd0850fabc93d5cdacb6fcfb3 in /nats-streaming-server 
# Fri, 16 Apr 2021 21:48:05 GMT
EXPOSE 4222 8222
# Fri, 16 Apr 2021 21:48:06 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Fri, 16 Apr 2021 21:48:07 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:fe1641db2bf227918d02728a21bd3b53989018d9c796246d3b96fcbbf75ded32`  
		Last Modified: Fri, 16 Apr 2021 21:48:50 GMT  
		Size: 5.2 MB (5170831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.21-nanoserver`

```console
$ docker pull nats-streaming@sha256:ec0aed95b5234c5cc882c7be18390dfb68a43a5285973d2264fc7cea404785ba
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1935; amd64

### `nats-streaming:0.21-nanoserver` - windows version 10.0.17763.1935; amd64

```console
$ docker pull nats-streaming@sha256:881fbff9b8ea5b5dce5d1e1fb341a4ab9a9caab12b0faf072dc89f9ab61792e9
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.2 MB (107191037 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9db19cc378f4cdf654406f9ff0a58704fbec29c0b23fa37b4919bcedd9a0a02`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Fri, 07 May 2021 11:54:57 GMT
RUN Apply image 1809-amd64
# Wed, 12 May 2021 15:44:03 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 12 May 2021 20:11:27 GMT
RUN cmd /S /C #(nop) COPY file:adacf7e54ef5a782ae37764b59883ad6a48b32c36c576816360f94cba82ba458 in C:\nats-streaming-server.exe 
# Wed, 12 May 2021 20:11:28 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 12 May 2021 20:11:29 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 12 May 2021 20:11:30 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:b9043d31610e0dfa43b1afe286f8918b6e3bf69ece50f44424b29d48f20aa662`  
		Size: 101.4 MB (101375240 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:95b58e21e5cdf4e2f9e5c87487734458885da325634d72f9c4e6583b353af06f`  
		Last Modified: Wed, 12 May 2021 15:49:02 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab3056c607d4b35216a2f74c2f849eb0c970001dc87bf45f90aea3ca4e8d9f05`  
		Last Modified: Wed, 12 May 2021 20:16:11 GMT  
		Size: 5.8 MB (5811203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:747d370e1cec130d4e6c1a20a9b8d049a93543b695b60a4fc0b5473758786920`  
		Last Modified: Wed, 12 May 2021 20:16:10 GMT  
		Size: 1.2 KB (1178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38d9d67f8ca438fa616690db8fc1087b47f11ad390d7a29761bfc08c67605c85`  
		Last Modified: Wed, 12 May 2021 20:16:10 GMT  
		Size: 1.1 KB (1105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e187a1b2446f3948440517b1cd475bdb32db16b4643b465f30313f8bbfe01d6`  
		Last Modified: Wed, 12 May 2021 20:16:10 GMT  
		Size: 1.2 KB (1161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.21-nanoserver-1809`

```console
$ docker pull nats-streaming@sha256:ec0aed95b5234c5cc882c7be18390dfb68a43a5285973d2264fc7cea404785ba
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1935; amd64

### `nats-streaming:0.21-nanoserver-1809` - windows version 10.0.17763.1935; amd64

```console
$ docker pull nats-streaming@sha256:881fbff9b8ea5b5dce5d1e1fb341a4ab9a9caab12b0faf072dc89f9ab61792e9
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.2 MB (107191037 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9db19cc378f4cdf654406f9ff0a58704fbec29c0b23fa37b4919bcedd9a0a02`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Fri, 07 May 2021 11:54:57 GMT
RUN Apply image 1809-amd64
# Wed, 12 May 2021 15:44:03 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 12 May 2021 20:11:27 GMT
RUN cmd /S /C #(nop) COPY file:adacf7e54ef5a782ae37764b59883ad6a48b32c36c576816360f94cba82ba458 in C:\nats-streaming-server.exe 
# Wed, 12 May 2021 20:11:28 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 12 May 2021 20:11:29 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 12 May 2021 20:11:30 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:b9043d31610e0dfa43b1afe286f8918b6e3bf69ece50f44424b29d48f20aa662`  
		Size: 101.4 MB (101375240 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:95b58e21e5cdf4e2f9e5c87487734458885da325634d72f9c4e6583b353af06f`  
		Last Modified: Wed, 12 May 2021 15:49:02 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab3056c607d4b35216a2f74c2f849eb0c970001dc87bf45f90aea3ca4e8d9f05`  
		Last Modified: Wed, 12 May 2021 20:16:11 GMT  
		Size: 5.8 MB (5811203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:747d370e1cec130d4e6c1a20a9b8d049a93543b695b60a4fc0b5473758786920`  
		Last Modified: Wed, 12 May 2021 20:16:10 GMT  
		Size: 1.2 KB (1178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38d9d67f8ca438fa616690db8fc1087b47f11ad390d7a29761bfc08c67605c85`  
		Last Modified: Wed, 12 May 2021 20:16:10 GMT  
		Size: 1.1 KB (1105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e187a1b2446f3948440517b1cd475bdb32db16b4643b465f30313f8bbfe01d6`  
		Last Modified: Wed, 12 May 2021 20:16:10 GMT  
		Size: 1.2 KB (1161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.21-scratch`

```console
$ docker pull nats-streaming@sha256:2bf298093b69248cb6e82aa7c64d50c1a45480ad23a8ced79a5ddf588ee69102
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.21-scratch` - linux; amd64

```console
$ docker pull nats-streaming@sha256:883d4d7a47db4d1c911cf0c23dad30011b46727297d1158bede3d833455a49e4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.7 MB (5680535 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d1e123176c313a4b94f8c0fdf6cac9abdd85a1bd6edf3f7cc6e7ed61852d19a`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Fri, 16 Apr 2021 21:25:32 GMT
COPY file:aefc6cbeadb611214d28b81a278a791c774a4bbc969528522aae7abe7c4e2784 in /nats-streaming-server 
# Fri, 16 Apr 2021 21:25:32 GMT
EXPOSE 4222 8222
# Fri, 16 Apr 2021 21:25:32 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Fri, 16 Apr 2021 21:25:33 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:087a668f89c4000c166ca5a16dd40fee8206986ce9b47a92d224b78214f3db5c`  
		Last Modified: Fri, 16 Apr 2021 21:26:16 GMT  
		Size: 5.7 MB (5680535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.21-scratch` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:9dc93ca8dad040be30fe0949d19f04a6b1775750838d70d2fb12f3aa9f40b4f8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.3 MB (5253054 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba356cbd8fdcd90e529d00104791d07c50c101937487a0b8647b06226bfdef9a`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Fri, 16 Apr 2021 21:02:53 GMT
COPY file:c58b6e2180eb9d24d595f35c2205c2d9b4f80315beb0f166e20a7340cf3f2536 in /nats-streaming-server 
# Fri, 16 Apr 2021 21:03:00 GMT
EXPOSE 4222 8222
# Fri, 16 Apr 2021 21:03:04 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Fri, 16 Apr 2021 21:03:07 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:3542c02ee947256ff50165b76289b4dd90e7c82bfb7b0b983b4d66d4b1128e9a`  
		Last Modified: Fri, 16 Apr 2021 21:03:44 GMT  
		Size: 5.3 MB (5253054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.21-scratch` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:10f5838646402cebd5c40f8f02991aad0ca3767b13b3024054e5e04026d3c778
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5246280 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:409bfb98a0a11b06fb4c8a044cda742270c21f5082ef80b63e7893cb4ce2f9c3`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Fri, 16 Apr 2021 21:00:05 GMT
COPY file:7ad2a856b4d75bdc56fbd35738819610cc3c26111897fc883c3af7db16d4fa87 in /nats-streaming-server 
# Fri, 16 Apr 2021 21:00:07 GMT
EXPOSE 4222 8222
# Fri, 16 Apr 2021 21:00:09 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Fri, 16 Apr 2021 21:00:10 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:76bf01e9a89a0de09d5ab72dd4ec7e4c9f561a27756ceb73bf0365f192de2d18`  
		Last Modified: Fri, 16 Apr 2021 21:01:13 GMT  
		Size: 5.2 MB (5246280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.21-scratch` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:3bf4856546fa4657b125293b8ed701a22dd3861cd532a14281d7726210c726c9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5170831 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e4acb30c8790d9ef8af675772eda5d9f3903a662d29132ef140463453eeb717`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Fri, 16 Apr 2021 21:48:04 GMT
COPY file:b02a357b6e9250e52099dcc91c6a9a78682a192bd0850fabc93d5cdacb6fcfb3 in /nats-streaming-server 
# Fri, 16 Apr 2021 21:48:05 GMT
EXPOSE 4222 8222
# Fri, 16 Apr 2021 21:48:06 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Fri, 16 Apr 2021 21:48:07 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:fe1641db2bf227918d02728a21bd3b53989018d9c796246d3b96fcbbf75ded32`  
		Last Modified: Fri, 16 Apr 2021 21:48:50 GMT  
		Size: 5.2 MB (5170831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.21-windowsservercore`

```console
$ docker pull nats-streaming@sha256:0befbd41f19304f5a7776ec78fae36978bd62c3f9cad17e4980b4cf886e6f64a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1935; amd64
	-	windows version 10.0.14393.4402; amd64

### `nats-streaming:0.21-windowsservercore` - windows version 10.0.17763.1935; amd64

```console
$ docker pull nats-streaming@sha256:df969179961089c2884fe95d19cab9088c89cf714b5169b76e8eaefa20d26550
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2490478060 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:87797a3af44c930235285b950723e7e38b9e69e8a60449c737a88b738c5c54e1`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 08 May 2021 09:21:48 GMT
RUN Install update 1809-amd64
# Tue, 11 May 2021 23:54:13 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 May 2021 15:41:49 GMT
ENV NATS_DOCKERIZED=1
# Wed, 12 May 2021 20:09:14 GMT
ENV NATS_STREAMING_SERVER=0.21.2
# Wed, 12 May 2021 20:09:14 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.21.2/nats-streaming-server-v0.21.2-windows-amd64.zip
# Wed, 12 May 2021 20:09:15 GMT
ENV GIT_DOWNLOAD_SHA256=5d4367fea29116fcd70c364c8e808d6bc8e74214effbde83dd9548455bd06df2
# Wed, 12 May 2021 20:09:48 GMT
RUN Set-PSDebug -Trace 2
# Wed, 12 May 2021 20:11:11 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 12 May 2021 20:11:12 GMT
EXPOSE 4222 8222
# Wed, 12 May 2021 20:11:13 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 12 May 2021 20:11:14 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8116de3c91c3f1ef2d6c09b49ef5407c9b4d672896eb3af5182a997c3c5379c9`  
		Size: 756.2 MB (756156286 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c049a65ed9206719f5c04428cb853623400e8ab1668243872b1134775f752962`  
		Last Modified: Wed, 12 May 2021 00:41:58 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:262d2305f11fe8f36ef3508b42686daac7e99da966ed02f4ded1927387b1b75b`  
		Last Modified: Wed, 12 May 2021 15:48:42 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caae5631f8d4c6cdfd8103d983810b9bfbefd01878285af9f623ac2f238f3449`  
		Last Modified: Wed, 12 May 2021 20:15:53 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d63f70b8ac38a77401cdba37ded79ef5a8565d1e0e5995c31b91f7aa4ce1b3f`  
		Last Modified: Wed, 12 May 2021 20:15:52 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0116c026836dea58f1432a034571efcf1d367ff5c6871c8f0930b7c9797602b2`  
		Last Modified: Wed, 12 May 2021 20:15:52 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7934c4e249cc275fd9d51173f09fbb985aa5c6d4314dce86d94108e3391b9bd5`  
		Last Modified: Wed, 12 May 2021 20:15:51 GMT  
		Size: 5.1 MB (5097038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:448f7480833686f3bbf6a3b41420f2f5add2aae1e35e31f4b47fe4b5e7fa441f`  
		Last Modified: Wed, 12 May 2021 20:15:53 GMT  
		Size: 10.9 MB (10880522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa234e132dde31816c466d94b40cac410cddcf081c522dbbabacbaca243f86a1`  
		Last Modified: Wed, 12 May 2021 20:15:50 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db175b165b9197d8d4b1751818e16f7c87846387f6d20a58ec01c885127fdf4d`  
		Last Modified: Wed, 12 May 2021 20:15:50 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38f8e2ba8c9a144f6620284f2697e8d0220903615e9c104d76fe384d4c5f3958`  
		Last Modified: Wed, 12 May 2021 20:15:49 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.21-windowsservercore` - windows version 10.0.14393.4402; amd64

```console
$ docker pull nats-streaming@sha256:d15f6cc0f6f200c03c249c6fa30e1d993feabdba06c9bfb4dd25a41cb75dba02
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5817500079 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:77c238ff37580c7dd07576778ab4a469bb8b538c9e3e9990a2d98c7326094ebd`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 26 Apr 2021 17:25:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 11 May 2021 23:58:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 May 2021 15:44:16 GMT
ENV NATS_DOCKERIZED=1
# Wed, 12 May 2021 20:11:37 GMT
ENV NATS_STREAMING_SERVER=0.21.2
# Wed, 12 May 2021 20:11:38 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.21.2/nats-streaming-server-v0.21.2-windows-amd64.zip
# Wed, 12 May 2021 20:11:39 GMT
ENV GIT_DOWNLOAD_SHA256=5d4367fea29116fcd70c364c8e808d6bc8e74214effbde83dd9548455bd06df2
# Wed, 12 May 2021 20:12:54 GMT
RUN Set-PSDebug -Trace 2
# Wed, 12 May 2021 20:15:02 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 12 May 2021 20:15:03 GMT
EXPOSE 4222 8222
# Wed, 12 May 2021 20:15:04 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 12 May 2021 20:15:05 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7f532f88613ca85064b055f6b93f8517bd05feba8fdce495a6ad1421573e765e`  
		Size: 1.7 GB (1725791397 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:50d0f4595a2bdc5dc0623fbee162be09d0631373eb9e82a0b1ec387ce1512c49`  
		Last Modified: Wed, 12 May 2021 00:46:32 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b7998d92dbbcfc4e6dc106e75206a3cfde70fe601eb46b0515658f23dcd53ae`  
		Last Modified: Wed, 12 May 2021 15:49:26 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f3010a7dd8667ca84982e9114e1dc65712c28bc68c365842b10a045ca612037`  
		Last Modified: Wed, 12 May 2021 20:16:28 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df06200a155b162a6be73cde9177db0ddf3ab1d3cfbd6cde1716508ea936e815`  
		Last Modified: Wed, 12 May 2021 20:16:28 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e23a0cd6171825cfd2bf6df17479e82e5845162d61bf74cf02daf44b78ba106`  
		Last Modified: Wed, 12 May 2021 20:16:28 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67048fb7884ce62e43c9c94e93c2469620bc4f1c31de0bfed360949a4856b32c`  
		Last Modified: Wed, 12 May 2021 20:16:32 GMT  
		Size: 5.7 MB (5699433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c112a8566705980bcc28d7b657abbc41bebdba6f14cc110792896e37a8ad36c0`  
		Last Modified: Wed, 12 May 2021 20:16:48 GMT  
		Size: 16.0 MB (16012020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a61d35a77f28396bd2da2e43c4fdf316968fa5dac4db17f07873ad8f2f778e54`  
		Last Modified: Wed, 12 May 2021 20:16:25 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96acafa52a9f3be44164c214903b7fffc48d9030807ce105a6c09093f4ebe1b9`  
		Last Modified: Wed, 12 May 2021 20:16:25 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b24723ae97946b0dbd5bf2b012548e33ca907518a500ca519e4bb0317bd31e0`  
		Last Modified: Wed, 12 May 2021 20:16:25 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.21-windowsservercore-1809`

```console
$ docker pull nats-streaming@sha256:ea4b6301b3365558fb705235d0e6ad5d6a3fcd989167e67831738db244d553b1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1935; amd64

### `nats-streaming:0.21-windowsservercore-1809` - windows version 10.0.17763.1935; amd64

```console
$ docker pull nats-streaming@sha256:df969179961089c2884fe95d19cab9088c89cf714b5169b76e8eaefa20d26550
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2490478060 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:87797a3af44c930235285b950723e7e38b9e69e8a60449c737a88b738c5c54e1`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 08 May 2021 09:21:48 GMT
RUN Install update 1809-amd64
# Tue, 11 May 2021 23:54:13 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 May 2021 15:41:49 GMT
ENV NATS_DOCKERIZED=1
# Wed, 12 May 2021 20:09:14 GMT
ENV NATS_STREAMING_SERVER=0.21.2
# Wed, 12 May 2021 20:09:14 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.21.2/nats-streaming-server-v0.21.2-windows-amd64.zip
# Wed, 12 May 2021 20:09:15 GMT
ENV GIT_DOWNLOAD_SHA256=5d4367fea29116fcd70c364c8e808d6bc8e74214effbde83dd9548455bd06df2
# Wed, 12 May 2021 20:09:48 GMT
RUN Set-PSDebug -Trace 2
# Wed, 12 May 2021 20:11:11 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 12 May 2021 20:11:12 GMT
EXPOSE 4222 8222
# Wed, 12 May 2021 20:11:13 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 12 May 2021 20:11:14 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8116de3c91c3f1ef2d6c09b49ef5407c9b4d672896eb3af5182a997c3c5379c9`  
		Size: 756.2 MB (756156286 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c049a65ed9206719f5c04428cb853623400e8ab1668243872b1134775f752962`  
		Last Modified: Wed, 12 May 2021 00:41:58 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:262d2305f11fe8f36ef3508b42686daac7e99da966ed02f4ded1927387b1b75b`  
		Last Modified: Wed, 12 May 2021 15:48:42 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caae5631f8d4c6cdfd8103d983810b9bfbefd01878285af9f623ac2f238f3449`  
		Last Modified: Wed, 12 May 2021 20:15:53 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d63f70b8ac38a77401cdba37ded79ef5a8565d1e0e5995c31b91f7aa4ce1b3f`  
		Last Modified: Wed, 12 May 2021 20:15:52 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0116c026836dea58f1432a034571efcf1d367ff5c6871c8f0930b7c9797602b2`  
		Last Modified: Wed, 12 May 2021 20:15:52 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7934c4e249cc275fd9d51173f09fbb985aa5c6d4314dce86d94108e3391b9bd5`  
		Last Modified: Wed, 12 May 2021 20:15:51 GMT  
		Size: 5.1 MB (5097038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:448f7480833686f3bbf6a3b41420f2f5add2aae1e35e31f4b47fe4b5e7fa441f`  
		Last Modified: Wed, 12 May 2021 20:15:53 GMT  
		Size: 10.9 MB (10880522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa234e132dde31816c466d94b40cac410cddcf081c522dbbabacbaca243f86a1`  
		Last Modified: Wed, 12 May 2021 20:15:50 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db175b165b9197d8d4b1751818e16f7c87846387f6d20a58ec01c885127fdf4d`  
		Last Modified: Wed, 12 May 2021 20:15:50 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38f8e2ba8c9a144f6620284f2697e8d0220903615e9c104d76fe384d4c5f3958`  
		Last Modified: Wed, 12 May 2021 20:15:49 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.21-windowsservercore-ltsc2016`

```console
$ docker pull nats-streaming@sha256:625ab75dea32121df296345016a44bcaa577d91d7c55b131fb28fd842ab65181
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4402; amd64

### `nats-streaming:0.21-windowsservercore-ltsc2016` - windows version 10.0.14393.4402; amd64

```console
$ docker pull nats-streaming@sha256:d15f6cc0f6f200c03c249c6fa30e1d993feabdba06c9bfb4dd25a41cb75dba02
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5817500079 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:77c238ff37580c7dd07576778ab4a469bb8b538c9e3e9990a2d98c7326094ebd`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 26 Apr 2021 17:25:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 11 May 2021 23:58:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 May 2021 15:44:16 GMT
ENV NATS_DOCKERIZED=1
# Wed, 12 May 2021 20:11:37 GMT
ENV NATS_STREAMING_SERVER=0.21.2
# Wed, 12 May 2021 20:11:38 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.21.2/nats-streaming-server-v0.21.2-windows-amd64.zip
# Wed, 12 May 2021 20:11:39 GMT
ENV GIT_DOWNLOAD_SHA256=5d4367fea29116fcd70c364c8e808d6bc8e74214effbde83dd9548455bd06df2
# Wed, 12 May 2021 20:12:54 GMT
RUN Set-PSDebug -Trace 2
# Wed, 12 May 2021 20:15:02 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 12 May 2021 20:15:03 GMT
EXPOSE 4222 8222
# Wed, 12 May 2021 20:15:04 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 12 May 2021 20:15:05 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7f532f88613ca85064b055f6b93f8517bd05feba8fdce495a6ad1421573e765e`  
		Size: 1.7 GB (1725791397 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:50d0f4595a2bdc5dc0623fbee162be09d0631373eb9e82a0b1ec387ce1512c49`  
		Last Modified: Wed, 12 May 2021 00:46:32 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b7998d92dbbcfc4e6dc106e75206a3cfde70fe601eb46b0515658f23dcd53ae`  
		Last Modified: Wed, 12 May 2021 15:49:26 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f3010a7dd8667ca84982e9114e1dc65712c28bc68c365842b10a045ca612037`  
		Last Modified: Wed, 12 May 2021 20:16:28 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df06200a155b162a6be73cde9177db0ddf3ab1d3cfbd6cde1716508ea936e815`  
		Last Modified: Wed, 12 May 2021 20:16:28 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e23a0cd6171825cfd2bf6df17479e82e5845162d61bf74cf02daf44b78ba106`  
		Last Modified: Wed, 12 May 2021 20:16:28 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67048fb7884ce62e43c9c94e93c2469620bc4f1c31de0bfed360949a4856b32c`  
		Last Modified: Wed, 12 May 2021 20:16:32 GMT  
		Size: 5.7 MB (5699433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c112a8566705980bcc28d7b657abbc41bebdba6f14cc110792896e37a8ad36c0`  
		Last Modified: Wed, 12 May 2021 20:16:48 GMT  
		Size: 16.0 MB (16012020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a61d35a77f28396bd2da2e43c4fdf316968fa5dac4db17f07873ad8f2f778e54`  
		Last Modified: Wed, 12 May 2021 20:16:25 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96acafa52a9f3be44164c214903b7fffc48d9030807ce105a6c09093f4ebe1b9`  
		Last Modified: Wed, 12 May 2021 20:16:25 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b24723ae97946b0dbd5bf2b012548e33ca907518a500ca519e4bb0317bd31e0`  
		Last Modified: Wed, 12 May 2021 20:16:25 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.21.2`

```console
$ docker pull nats-streaming@sha256:8e9036a7e32179bf55236241656e9555336215146d30129b5ac664f94fd73ed6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.1935; amd64

### `nats-streaming:0.21.2` - linux; amd64

```console
$ docker pull nats-streaming@sha256:883d4d7a47db4d1c911cf0c23dad30011b46727297d1158bede3d833455a49e4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.7 MB (5680535 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d1e123176c313a4b94f8c0fdf6cac9abdd85a1bd6edf3f7cc6e7ed61852d19a`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Fri, 16 Apr 2021 21:25:32 GMT
COPY file:aefc6cbeadb611214d28b81a278a791c774a4bbc969528522aae7abe7c4e2784 in /nats-streaming-server 
# Fri, 16 Apr 2021 21:25:32 GMT
EXPOSE 4222 8222
# Fri, 16 Apr 2021 21:25:32 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Fri, 16 Apr 2021 21:25:33 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:087a668f89c4000c166ca5a16dd40fee8206986ce9b47a92d224b78214f3db5c`  
		Last Modified: Fri, 16 Apr 2021 21:26:16 GMT  
		Size: 5.7 MB (5680535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.21.2` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:9dc93ca8dad040be30fe0949d19f04a6b1775750838d70d2fb12f3aa9f40b4f8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.3 MB (5253054 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba356cbd8fdcd90e529d00104791d07c50c101937487a0b8647b06226bfdef9a`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Fri, 16 Apr 2021 21:02:53 GMT
COPY file:c58b6e2180eb9d24d595f35c2205c2d9b4f80315beb0f166e20a7340cf3f2536 in /nats-streaming-server 
# Fri, 16 Apr 2021 21:03:00 GMT
EXPOSE 4222 8222
# Fri, 16 Apr 2021 21:03:04 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Fri, 16 Apr 2021 21:03:07 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:3542c02ee947256ff50165b76289b4dd90e7c82bfb7b0b983b4d66d4b1128e9a`  
		Last Modified: Fri, 16 Apr 2021 21:03:44 GMT  
		Size: 5.3 MB (5253054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.21.2` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:10f5838646402cebd5c40f8f02991aad0ca3767b13b3024054e5e04026d3c778
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5246280 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:409bfb98a0a11b06fb4c8a044cda742270c21f5082ef80b63e7893cb4ce2f9c3`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Fri, 16 Apr 2021 21:00:05 GMT
COPY file:7ad2a856b4d75bdc56fbd35738819610cc3c26111897fc883c3af7db16d4fa87 in /nats-streaming-server 
# Fri, 16 Apr 2021 21:00:07 GMT
EXPOSE 4222 8222
# Fri, 16 Apr 2021 21:00:09 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Fri, 16 Apr 2021 21:00:10 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:76bf01e9a89a0de09d5ab72dd4ec7e4c9f561a27756ceb73bf0365f192de2d18`  
		Last Modified: Fri, 16 Apr 2021 21:01:13 GMT  
		Size: 5.2 MB (5246280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.21.2` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:3bf4856546fa4657b125293b8ed701a22dd3861cd532a14281d7726210c726c9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5170831 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e4acb30c8790d9ef8af675772eda5d9f3903a662d29132ef140463453eeb717`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Fri, 16 Apr 2021 21:48:04 GMT
COPY file:b02a357b6e9250e52099dcc91c6a9a78682a192bd0850fabc93d5cdacb6fcfb3 in /nats-streaming-server 
# Fri, 16 Apr 2021 21:48:05 GMT
EXPOSE 4222 8222
# Fri, 16 Apr 2021 21:48:06 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Fri, 16 Apr 2021 21:48:07 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:fe1641db2bf227918d02728a21bd3b53989018d9c796246d3b96fcbbf75ded32`  
		Last Modified: Fri, 16 Apr 2021 21:48:50 GMT  
		Size: 5.2 MB (5170831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.21.2` - windows version 10.0.17763.1935; amd64

```console
$ docker pull nats-streaming@sha256:881fbff9b8ea5b5dce5d1e1fb341a4ab9a9caab12b0faf072dc89f9ab61792e9
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.2 MB (107191037 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9db19cc378f4cdf654406f9ff0a58704fbec29c0b23fa37b4919bcedd9a0a02`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Fri, 07 May 2021 11:54:57 GMT
RUN Apply image 1809-amd64
# Wed, 12 May 2021 15:44:03 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 12 May 2021 20:11:27 GMT
RUN cmd /S /C #(nop) COPY file:adacf7e54ef5a782ae37764b59883ad6a48b32c36c576816360f94cba82ba458 in C:\nats-streaming-server.exe 
# Wed, 12 May 2021 20:11:28 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 12 May 2021 20:11:29 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 12 May 2021 20:11:30 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:b9043d31610e0dfa43b1afe286f8918b6e3bf69ece50f44424b29d48f20aa662`  
		Size: 101.4 MB (101375240 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:95b58e21e5cdf4e2f9e5c87487734458885da325634d72f9c4e6583b353af06f`  
		Last Modified: Wed, 12 May 2021 15:49:02 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab3056c607d4b35216a2f74c2f849eb0c970001dc87bf45f90aea3ca4e8d9f05`  
		Last Modified: Wed, 12 May 2021 20:16:11 GMT  
		Size: 5.8 MB (5811203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:747d370e1cec130d4e6c1a20a9b8d049a93543b695b60a4fc0b5473758786920`  
		Last Modified: Wed, 12 May 2021 20:16:10 GMT  
		Size: 1.2 KB (1178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38d9d67f8ca438fa616690db8fc1087b47f11ad390d7a29761bfc08c67605c85`  
		Last Modified: Wed, 12 May 2021 20:16:10 GMT  
		Size: 1.1 KB (1105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e187a1b2446f3948440517b1cd475bdb32db16b4643b465f30313f8bbfe01d6`  
		Last Modified: Wed, 12 May 2021 20:16:10 GMT  
		Size: 1.2 KB (1161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.21.2-alpine`

```console
$ docker pull nats-streaming@sha256:d204ac6b58553c9632e9797984adcace87b6539d257754f1d5bdf5e4a2a8d72e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.21.2-alpine` - linux; amd64

```console
$ docker pull nats-streaming@sha256:402dacbb78f9bf5e9ea249c730f7905caa085ca665782e1cb4c6e7004f597689
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.8 MB (8774780 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f7ad70b17b46627026163460cce06023868f24d36a50cd9c261e7c6cba86e29`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Fri, 16 Apr 2021 21:25:11 GMT
ENV NATS_STREAMING_SERVER=0.21.2
# Fri, 16 Apr 2021 21:25:14 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='56bcfea3c3d7a232dab93ad280ce8f8df87959ac000c7d24ce03dbab2f4c4d2b' ;; 		armhf) natsArch='arm6'; sha256='34d7032ba61724ec55d78cb94a5ed244754509b8b957e1e7e4f0579292c35a7f' ;; 		armv7) natsArch='arm7'; sha256='b4869711408e3823c8818e934bf90d07ed51f350147702b80831fb4fe5a390d2' ;; 		x86_64) natsArch='amd64'; sha256='7a401a3af7eb56a0d1d3b207dc517222697b48cb7e9e524848e62bd13393d23a' ;; 		x86) natsArch='386'; sha256='58aa4cad4c75920522ec0457b79d889f9c740c248647b875254cd1313517620c' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 16 Apr 2021 21:25:14 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Fri, 16 Apr 2021 21:25:15 GMT
EXPOSE 4222 8222
# Fri, 16 Apr 2021 21:25:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Apr 2021 21:25:15 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:269577e93d92e9e558c3607d8b5e74978c939fc643895de15fd70ef06b811323`  
		Last Modified: Fri, 16 Apr 2021 21:25:54 GMT  
		Size: 6.0 MB (5962389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5fa1ca69a5dc5f7aecbfca382d45ab09423bb9d103c6567abc37af7b842073a`  
		Last Modified: Fri, 16 Apr 2021 21:25:54 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.21.2-alpine` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:e03de3640ce68bbb19cd2b5e8dc2a1454fbba1b369a4c236f09b6630197b6fa0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.2 MB (8156933 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a345ef8cbbe68103787d05c9dbd22742cc95b726776cbf30298c3ca98487b63`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 14 Apr 2021 18:49:39 GMT
ADD file:4479f0a51530e039edf231d87201896dcff908aa542a613cdccb015f93dda8a3 in / 
# Wed, 14 Apr 2021 18:49:40 GMT
CMD ["/bin/sh"]
# Fri, 16 Apr 2021 21:02:04 GMT
ENV NATS_STREAMING_SERVER=0.21.2
# Fri, 16 Apr 2021 21:02:23 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='56bcfea3c3d7a232dab93ad280ce8f8df87959ac000c7d24ce03dbab2f4c4d2b' ;; 		armhf) natsArch='arm6'; sha256='34d7032ba61724ec55d78cb94a5ed244754509b8b957e1e7e4f0579292c35a7f' ;; 		armv7) natsArch='arm7'; sha256='b4869711408e3823c8818e934bf90d07ed51f350147702b80831fb4fe5a390d2' ;; 		x86_64) natsArch='amd64'; sha256='7a401a3af7eb56a0d1d3b207dc517222697b48cb7e9e524848e62bd13393d23a' ;; 		x86) natsArch='386'; sha256='58aa4cad4c75920522ec0457b79d889f9c740c248647b875254cd1313517620c' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 16 Apr 2021 21:02:26 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Fri, 16 Apr 2021 21:02:27 GMT
EXPOSE 4222 8222
# Fri, 16 Apr 2021 21:02:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Apr 2021 21:02:29 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:740c950346cf39c85b52576998695c9b909c24a58a8bb1b64cce91fda3ef1d3a`  
		Last Modified: Wed, 14 Apr 2021 18:50:30 GMT  
		Size: 2.6 MB (2622131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e538f4430325ed9ef756e0e521a859c9466b9b7a45a8662e4f29f1ec5f8c3a7d`  
		Last Modified: Fri, 16 Apr 2021 21:03:32 GMT  
		Size: 5.5 MB (5534381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc165822006c8e13ee1ee6756545e0f021a059f974288d6c953febdeea6a83d3`  
		Last Modified: Fri, 16 Apr 2021 21:03:30 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.21.2-alpine` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:ea133d32e6510a0d1822a1ea1cfcca41e3cbd747a3d69491aee62319937e892d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.0 MB (7951606 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc13824ee86fb9d0c1609b885378ba366f3883903bfe990fb27464bce6c02686`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 14 Apr 2021 18:57:39 GMT
ADD file:028c5b473d862250586e174c5dd19b37f8fc3bffbc02d888e72df30f32fd6129 in / 
# Wed, 14 Apr 2021 18:57:39 GMT
CMD ["/bin/sh"]
# Fri, 16 Apr 2021 20:59:08 GMT
ENV NATS_STREAMING_SERVER=0.21.2
# Fri, 16 Apr 2021 20:59:12 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='56bcfea3c3d7a232dab93ad280ce8f8df87959ac000c7d24ce03dbab2f4c4d2b' ;; 		armhf) natsArch='arm6'; sha256='34d7032ba61724ec55d78cb94a5ed244754509b8b957e1e7e4f0579292c35a7f' ;; 		armv7) natsArch='arm7'; sha256='b4869711408e3823c8818e934bf90d07ed51f350147702b80831fb4fe5a390d2' ;; 		x86_64) natsArch='amd64'; sha256='7a401a3af7eb56a0d1d3b207dc517222697b48cb7e9e524848e62bd13393d23a' ;; 		x86) natsArch='386'; sha256='58aa4cad4c75920522ec0457b79d889f9c740c248647b875254cd1313517620c' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 16 Apr 2021 20:59:13 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Fri, 16 Apr 2021 20:59:14 GMT
EXPOSE 4222 8222
# Fri, 16 Apr 2021 20:59:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Apr 2021 20:59:16 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:e160e00eb35d5bc2373770873fbc9c8f5706045b0b06bfd1c364fcf69f02e9fe`  
		Last Modified: Wed, 14 Apr 2021 18:58:36 GMT  
		Size: 2.4 MB (2424145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6b86c52fd84fa988d60547be09b11af6fcac2dffa6b340e92b776a0fc89a298`  
		Last Modified: Fri, 16 Apr 2021 21:00:42 GMT  
		Size: 5.5 MB (5527039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7b279e3ce6e5cfc3967a4acbf6dc2563f1715817b059d6f320b53cbc21b74e1`  
		Last Modified: Fri, 16 Apr 2021 21:00:40 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.21.2-alpine` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:febf36c660fc36bcbf3da9945707f541e81665b0d21a0f1c6c8220543697a757
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.2 MB (8165113 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd79dce90e049636e2513bd55a0b3178cb59197d3dfc53cbed474dbbd5de0f1f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 14 Apr 2021 18:42:37 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Wed, 14 Apr 2021 18:42:38 GMT
CMD ["/bin/sh"]
# Fri, 16 Apr 2021 21:44:03 GMT
ENV NATS_STREAMING_SERVER=0.21.2
# Fri, 16 Apr 2021 21:44:07 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='56bcfea3c3d7a232dab93ad280ce8f8df87959ac000c7d24ce03dbab2f4c4d2b' ;; 		armhf) natsArch='arm6'; sha256='34d7032ba61724ec55d78cb94a5ed244754509b8b957e1e7e4f0579292c35a7f' ;; 		armv7) natsArch='arm7'; sha256='b4869711408e3823c8818e934bf90d07ed51f350147702b80831fb4fe5a390d2' ;; 		x86_64) natsArch='amd64'; sha256='7a401a3af7eb56a0d1d3b207dc517222697b48cb7e9e524848e62bd13393d23a' ;; 		x86) natsArch='386'; sha256='58aa4cad4c75920522ec0457b79d889f9c740c248647b875254cd1313517620c' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 16 Apr 2021 21:44:08 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Fri, 16 Apr 2021 21:44:09 GMT
EXPOSE 4222 8222
# Fri, 16 Apr 2021 21:44:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Apr 2021 21:44:10 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03a1a4dae3b1b310f0231f28f4db383d7605066343274881c5be1300ebe64f51`  
		Last Modified: Fri, 16 Apr 2021 21:48:37 GMT  
		Size: 5.5 MB (5452665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0a06774842e75925d8884fc1ea5a3e83c2c8054d4fb443ad11021c5866b0617`  
		Last Modified: Fri, 16 Apr 2021 21:48:36 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.21.2-alpine3.13`

```console
$ docker pull nats-streaming@sha256:d204ac6b58553c9632e9797984adcace87b6539d257754f1d5bdf5e4a2a8d72e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.21.2-alpine3.13` - linux; amd64

```console
$ docker pull nats-streaming@sha256:402dacbb78f9bf5e9ea249c730f7905caa085ca665782e1cb4c6e7004f597689
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.8 MB (8774780 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f7ad70b17b46627026163460cce06023868f24d36a50cd9c261e7c6cba86e29`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Fri, 16 Apr 2021 21:25:11 GMT
ENV NATS_STREAMING_SERVER=0.21.2
# Fri, 16 Apr 2021 21:25:14 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='56bcfea3c3d7a232dab93ad280ce8f8df87959ac000c7d24ce03dbab2f4c4d2b' ;; 		armhf) natsArch='arm6'; sha256='34d7032ba61724ec55d78cb94a5ed244754509b8b957e1e7e4f0579292c35a7f' ;; 		armv7) natsArch='arm7'; sha256='b4869711408e3823c8818e934bf90d07ed51f350147702b80831fb4fe5a390d2' ;; 		x86_64) natsArch='amd64'; sha256='7a401a3af7eb56a0d1d3b207dc517222697b48cb7e9e524848e62bd13393d23a' ;; 		x86) natsArch='386'; sha256='58aa4cad4c75920522ec0457b79d889f9c740c248647b875254cd1313517620c' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 16 Apr 2021 21:25:14 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Fri, 16 Apr 2021 21:25:15 GMT
EXPOSE 4222 8222
# Fri, 16 Apr 2021 21:25:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Apr 2021 21:25:15 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:269577e93d92e9e558c3607d8b5e74978c939fc643895de15fd70ef06b811323`  
		Last Modified: Fri, 16 Apr 2021 21:25:54 GMT  
		Size: 6.0 MB (5962389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5fa1ca69a5dc5f7aecbfca382d45ab09423bb9d103c6567abc37af7b842073a`  
		Last Modified: Fri, 16 Apr 2021 21:25:54 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.21.2-alpine3.13` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:e03de3640ce68bbb19cd2b5e8dc2a1454fbba1b369a4c236f09b6630197b6fa0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.2 MB (8156933 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a345ef8cbbe68103787d05c9dbd22742cc95b726776cbf30298c3ca98487b63`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 14 Apr 2021 18:49:39 GMT
ADD file:4479f0a51530e039edf231d87201896dcff908aa542a613cdccb015f93dda8a3 in / 
# Wed, 14 Apr 2021 18:49:40 GMT
CMD ["/bin/sh"]
# Fri, 16 Apr 2021 21:02:04 GMT
ENV NATS_STREAMING_SERVER=0.21.2
# Fri, 16 Apr 2021 21:02:23 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='56bcfea3c3d7a232dab93ad280ce8f8df87959ac000c7d24ce03dbab2f4c4d2b' ;; 		armhf) natsArch='arm6'; sha256='34d7032ba61724ec55d78cb94a5ed244754509b8b957e1e7e4f0579292c35a7f' ;; 		armv7) natsArch='arm7'; sha256='b4869711408e3823c8818e934bf90d07ed51f350147702b80831fb4fe5a390d2' ;; 		x86_64) natsArch='amd64'; sha256='7a401a3af7eb56a0d1d3b207dc517222697b48cb7e9e524848e62bd13393d23a' ;; 		x86) natsArch='386'; sha256='58aa4cad4c75920522ec0457b79d889f9c740c248647b875254cd1313517620c' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 16 Apr 2021 21:02:26 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Fri, 16 Apr 2021 21:02:27 GMT
EXPOSE 4222 8222
# Fri, 16 Apr 2021 21:02:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Apr 2021 21:02:29 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:740c950346cf39c85b52576998695c9b909c24a58a8bb1b64cce91fda3ef1d3a`  
		Last Modified: Wed, 14 Apr 2021 18:50:30 GMT  
		Size: 2.6 MB (2622131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e538f4430325ed9ef756e0e521a859c9466b9b7a45a8662e4f29f1ec5f8c3a7d`  
		Last Modified: Fri, 16 Apr 2021 21:03:32 GMT  
		Size: 5.5 MB (5534381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc165822006c8e13ee1ee6756545e0f021a059f974288d6c953febdeea6a83d3`  
		Last Modified: Fri, 16 Apr 2021 21:03:30 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.21.2-alpine3.13` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:ea133d32e6510a0d1822a1ea1cfcca41e3cbd747a3d69491aee62319937e892d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.0 MB (7951606 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc13824ee86fb9d0c1609b885378ba366f3883903bfe990fb27464bce6c02686`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 14 Apr 2021 18:57:39 GMT
ADD file:028c5b473d862250586e174c5dd19b37f8fc3bffbc02d888e72df30f32fd6129 in / 
# Wed, 14 Apr 2021 18:57:39 GMT
CMD ["/bin/sh"]
# Fri, 16 Apr 2021 20:59:08 GMT
ENV NATS_STREAMING_SERVER=0.21.2
# Fri, 16 Apr 2021 20:59:12 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='56bcfea3c3d7a232dab93ad280ce8f8df87959ac000c7d24ce03dbab2f4c4d2b' ;; 		armhf) natsArch='arm6'; sha256='34d7032ba61724ec55d78cb94a5ed244754509b8b957e1e7e4f0579292c35a7f' ;; 		armv7) natsArch='arm7'; sha256='b4869711408e3823c8818e934bf90d07ed51f350147702b80831fb4fe5a390d2' ;; 		x86_64) natsArch='amd64'; sha256='7a401a3af7eb56a0d1d3b207dc517222697b48cb7e9e524848e62bd13393d23a' ;; 		x86) natsArch='386'; sha256='58aa4cad4c75920522ec0457b79d889f9c740c248647b875254cd1313517620c' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 16 Apr 2021 20:59:13 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Fri, 16 Apr 2021 20:59:14 GMT
EXPOSE 4222 8222
# Fri, 16 Apr 2021 20:59:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Apr 2021 20:59:16 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:e160e00eb35d5bc2373770873fbc9c8f5706045b0b06bfd1c364fcf69f02e9fe`  
		Last Modified: Wed, 14 Apr 2021 18:58:36 GMT  
		Size: 2.4 MB (2424145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6b86c52fd84fa988d60547be09b11af6fcac2dffa6b340e92b776a0fc89a298`  
		Last Modified: Fri, 16 Apr 2021 21:00:42 GMT  
		Size: 5.5 MB (5527039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7b279e3ce6e5cfc3967a4acbf6dc2563f1715817b059d6f320b53cbc21b74e1`  
		Last Modified: Fri, 16 Apr 2021 21:00:40 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.21.2-alpine3.13` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:febf36c660fc36bcbf3da9945707f541e81665b0d21a0f1c6c8220543697a757
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.2 MB (8165113 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd79dce90e049636e2513bd55a0b3178cb59197d3dfc53cbed474dbbd5de0f1f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 14 Apr 2021 18:42:37 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Wed, 14 Apr 2021 18:42:38 GMT
CMD ["/bin/sh"]
# Fri, 16 Apr 2021 21:44:03 GMT
ENV NATS_STREAMING_SERVER=0.21.2
# Fri, 16 Apr 2021 21:44:07 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='56bcfea3c3d7a232dab93ad280ce8f8df87959ac000c7d24ce03dbab2f4c4d2b' ;; 		armhf) natsArch='arm6'; sha256='34d7032ba61724ec55d78cb94a5ed244754509b8b957e1e7e4f0579292c35a7f' ;; 		armv7) natsArch='arm7'; sha256='b4869711408e3823c8818e934bf90d07ed51f350147702b80831fb4fe5a390d2' ;; 		x86_64) natsArch='amd64'; sha256='7a401a3af7eb56a0d1d3b207dc517222697b48cb7e9e524848e62bd13393d23a' ;; 		x86) natsArch='386'; sha256='58aa4cad4c75920522ec0457b79d889f9c740c248647b875254cd1313517620c' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 16 Apr 2021 21:44:08 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Fri, 16 Apr 2021 21:44:09 GMT
EXPOSE 4222 8222
# Fri, 16 Apr 2021 21:44:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Apr 2021 21:44:10 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03a1a4dae3b1b310f0231f28f4db383d7605066343274881c5be1300ebe64f51`  
		Last Modified: Fri, 16 Apr 2021 21:48:37 GMT  
		Size: 5.5 MB (5452665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0a06774842e75925d8884fc1ea5a3e83c2c8054d4fb443ad11021c5866b0617`  
		Last Modified: Fri, 16 Apr 2021 21:48:36 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.21.2-linux`

```console
$ docker pull nats-streaming@sha256:2bf298093b69248cb6e82aa7c64d50c1a45480ad23a8ced79a5ddf588ee69102
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.21.2-linux` - linux; amd64

```console
$ docker pull nats-streaming@sha256:883d4d7a47db4d1c911cf0c23dad30011b46727297d1158bede3d833455a49e4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.7 MB (5680535 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d1e123176c313a4b94f8c0fdf6cac9abdd85a1bd6edf3f7cc6e7ed61852d19a`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Fri, 16 Apr 2021 21:25:32 GMT
COPY file:aefc6cbeadb611214d28b81a278a791c774a4bbc969528522aae7abe7c4e2784 in /nats-streaming-server 
# Fri, 16 Apr 2021 21:25:32 GMT
EXPOSE 4222 8222
# Fri, 16 Apr 2021 21:25:32 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Fri, 16 Apr 2021 21:25:33 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:087a668f89c4000c166ca5a16dd40fee8206986ce9b47a92d224b78214f3db5c`  
		Last Modified: Fri, 16 Apr 2021 21:26:16 GMT  
		Size: 5.7 MB (5680535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.21.2-linux` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:9dc93ca8dad040be30fe0949d19f04a6b1775750838d70d2fb12f3aa9f40b4f8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.3 MB (5253054 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba356cbd8fdcd90e529d00104791d07c50c101937487a0b8647b06226bfdef9a`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Fri, 16 Apr 2021 21:02:53 GMT
COPY file:c58b6e2180eb9d24d595f35c2205c2d9b4f80315beb0f166e20a7340cf3f2536 in /nats-streaming-server 
# Fri, 16 Apr 2021 21:03:00 GMT
EXPOSE 4222 8222
# Fri, 16 Apr 2021 21:03:04 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Fri, 16 Apr 2021 21:03:07 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:3542c02ee947256ff50165b76289b4dd90e7c82bfb7b0b983b4d66d4b1128e9a`  
		Last Modified: Fri, 16 Apr 2021 21:03:44 GMT  
		Size: 5.3 MB (5253054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.21.2-linux` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:10f5838646402cebd5c40f8f02991aad0ca3767b13b3024054e5e04026d3c778
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5246280 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:409bfb98a0a11b06fb4c8a044cda742270c21f5082ef80b63e7893cb4ce2f9c3`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Fri, 16 Apr 2021 21:00:05 GMT
COPY file:7ad2a856b4d75bdc56fbd35738819610cc3c26111897fc883c3af7db16d4fa87 in /nats-streaming-server 
# Fri, 16 Apr 2021 21:00:07 GMT
EXPOSE 4222 8222
# Fri, 16 Apr 2021 21:00:09 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Fri, 16 Apr 2021 21:00:10 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:76bf01e9a89a0de09d5ab72dd4ec7e4c9f561a27756ceb73bf0365f192de2d18`  
		Last Modified: Fri, 16 Apr 2021 21:01:13 GMT  
		Size: 5.2 MB (5246280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.21.2-linux` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:3bf4856546fa4657b125293b8ed701a22dd3861cd532a14281d7726210c726c9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5170831 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e4acb30c8790d9ef8af675772eda5d9f3903a662d29132ef140463453eeb717`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Fri, 16 Apr 2021 21:48:04 GMT
COPY file:b02a357b6e9250e52099dcc91c6a9a78682a192bd0850fabc93d5cdacb6fcfb3 in /nats-streaming-server 
# Fri, 16 Apr 2021 21:48:05 GMT
EXPOSE 4222 8222
# Fri, 16 Apr 2021 21:48:06 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Fri, 16 Apr 2021 21:48:07 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:fe1641db2bf227918d02728a21bd3b53989018d9c796246d3b96fcbbf75ded32`  
		Last Modified: Fri, 16 Apr 2021 21:48:50 GMT  
		Size: 5.2 MB (5170831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.21.2-nanoserver`

```console
$ docker pull nats-streaming@sha256:ec0aed95b5234c5cc882c7be18390dfb68a43a5285973d2264fc7cea404785ba
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1935; amd64

### `nats-streaming:0.21.2-nanoserver` - windows version 10.0.17763.1935; amd64

```console
$ docker pull nats-streaming@sha256:881fbff9b8ea5b5dce5d1e1fb341a4ab9a9caab12b0faf072dc89f9ab61792e9
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.2 MB (107191037 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9db19cc378f4cdf654406f9ff0a58704fbec29c0b23fa37b4919bcedd9a0a02`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Fri, 07 May 2021 11:54:57 GMT
RUN Apply image 1809-amd64
# Wed, 12 May 2021 15:44:03 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 12 May 2021 20:11:27 GMT
RUN cmd /S /C #(nop) COPY file:adacf7e54ef5a782ae37764b59883ad6a48b32c36c576816360f94cba82ba458 in C:\nats-streaming-server.exe 
# Wed, 12 May 2021 20:11:28 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 12 May 2021 20:11:29 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 12 May 2021 20:11:30 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:b9043d31610e0dfa43b1afe286f8918b6e3bf69ece50f44424b29d48f20aa662`  
		Size: 101.4 MB (101375240 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:95b58e21e5cdf4e2f9e5c87487734458885da325634d72f9c4e6583b353af06f`  
		Last Modified: Wed, 12 May 2021 15:49:02 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab3056c607d4b35216a2f74c2f849eb0c970001dc87bf45f90aea3ca4e8d9f05`  
		Last Modified: Wed, 12 May 2021 20:16:11 GMT  
		Size: 5.8 MB (5811203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:747d370e1cec130d4e6c1a20a9b8d049a93543b695b60a4fc0b5473758786920`  
		Last Modified: Wed, 12 May 2021 20:16:10 GMT  
		Size: 1.2 KB (1178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38d9d67f8ca438fa616690db8fc1087b47f11ad390d7a29761bfc08c67605c85`  
		Last Modified: Wed, 12 May 2021 20:16:10 GMT  
		Size: 1.1 KB (1105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e187a1b2446f3948440517b1cd475bdb32db16b4643b465f30313f8bbfe01d6`  
		Last Modified: Wed, 12 May 2021 20:16:10 GMT  
		Size: 1.2 KB (1161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.21.2-nanoserver-1809`

```console
$ docker pull nats-streaming@sha256:ec0aed95b5234c5cc882c7be18390dfb68a43a5285973d2264fc7cea404785ba
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1935; amd64

### `nats-streaming:0.21.2-nanoserver-1809` - windows version 10.0.17763.1935; amd64

```console
$ docker pull nats-streaming@sha256:881fbff9b8ea5b5dce5d1e1fb341a4ab9a9caab12b0faf072dc89f9ab61792e9
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.2 MB (107191037 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9db19cc378f4cdf654406f9ff0a58704fbec29c0b23fa37b4919bcedd9a0a02`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Fri, 07 May 2021 11:54:57 GMT
RUN Apply image 1809-amd64
# Wed, 12 May 2021 15:44:03 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 12 May 2021 20:11:27 GMT
RUN cmd /S /C #(nop) COPY file:adacf7e54ef5a782ae37764b59883ad6a48b32c36c576816360f94cba82ba458 in C:\nats-streaming-server.exe 
# Wed, 12 May 2021 20:11:28 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 12 May 2021 20:11:29 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 12 May 2021 20:11:30 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:b9043d31610e0dfa43b1afe286f8918b6e3bf69ece50f44424b29d48f20aa662`  
		Size: 101.4 MB (101375240 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:95b58e21e5cdf4e2f9e5c87487734458885da325634d72f9c4e6583b353af06f`  
		Last Modified: Wed, 12 May 2021 15:49:02 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab3056c607d4b35216a2f74c2f849eb0c970001dc87bf45f90aea3ca4e8d9f05`  
		Last Modified: Wed, 12 May 2021 20:16:11 GMT  
		Size: 5.8 MB (5811203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:747d370e1cec130d4e6c1a20a9b8d049a93543b695b60a4fc0b5473758786920`  
		Last Modified: Wed, 12 May 2021 20:16:10 GMT  
		Size: 1.2 KB (1178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38d9d67f8ca438fa616690db8fc1087b47f11ad390d7a29761bfc08c67605c85`  
		Last Modified: Wed, 12 May 2021 20:16:10 GMT  
		Size: 1.1 KB (1105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e187a1b2446f3948440517b1cd475bdb32db16b4643b465f30313f8bbfe01d6`  
		Last Modified: Wed, 12 May 2021 20:16:10 GMT  
		Size: 1.2 KB (1161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.21.2-scratch`

```console
$ docker pull nats-streaming@sha256:2bf298093b69248cb6e82aa7c64d50c1a45480ad23a8ced79a5ddf588ee69102
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.21.2-scratch` - linux; amd64

```console
$ docker pull nats-streaming@sha256:883d4d7a47db4d1c911cf0c23dad30011b46727297d1158bede3d833455a49e4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.7 MB (5680535 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d1e123176c313a4b94f8c0fdf6cac9abdd85a1bd6edf3f7cc6e7ed61852d19a`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Fri, 16 Apr 2021 21:25:32 GMT
COPY file:aefc6cbeadb611214d28b81a278a791c774a4bbc969528522aae7abe7c4e2784 in /nats-streaming-server 
# Fri, 16 Apr 2021 21:25:32 GMT
EXPOSE 4222 8222
# Fri, 16 Apr 2021 21:25:32 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Fri, 16 Apr 2021 21:25:33 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:087a668f89c4000c166ca5a16dd40fee8206986ce9b47a92d224b78214f3db5c`  
		Last Modified: Fri, 16 Apr 2021 21:26:16 GMT  
		Size: 5.7 MB (5680535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.21.2-scratch` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:9dc93ca8dad040be30fe0949d19f04a6b1775750838d70d2fb12f3aa9f40b4f8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.3 MB (5253054 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba356cbd8fdcd90e529d00104791d07c50c101937487a0b8647b06226bfdef9a`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Fri, 16 Apr 2021 21:02:53 GMT
COPY file:c58b6e2180eb9d24d595f35c2205c2d9b4f80315beb0f166e20a7340cf3f2536 in /nats-streaming-server 
# Fri, 16 Apr 2021 21:03:00 GMT
EXPOSE 4222 8222
# Fri, 16 Apr 2021 21:03:04 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Fri, 16 Apr 2021 21:03:07 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:3542c02ee947256ff50165b76289b4dd90e7c82bfb7b0b983b4d66d4b1128e9a`  
		Last Modified: Fri, 16 Apr 2021 21:03:44 GMT  
		Size: 5.3 MB (5253054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.21.2-scratch` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:10f5838646402cebd5c40f8f02991aad0ca3767b13b3024054e5e04026d3c778
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5246280 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:409bfb98a0a11b06fb4c8a044cda742270c21f5082ef80b63e7893cb4ce2f9c3`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Fri, 16 Apr 2021 21:00:05 GMT
COPY file:7ad2a856b4d75bdc56fbd35738819610cc3c26111897fc883c3af7db16d4fa87 in /nats-streaming-server 
# Fri, 16 Apr 2021 21:00:07 GMT
EXPOSE 4222 8222
# Fri, 16 Apr 2021 21:00:09 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Fri, 16 Apr 2021 21:00:10 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:76bf01e9a89a0de09d5ab72dd4ec7e4c9f561a27756ceb73bf0365f192de2d18`  
		Last Modified: Fri, 16 Apr 2021 21:01:13 GMT  
		Size: 5.2 MB (5246280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.21.2-scratch` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:3bf4856546fa4657b125293b8ed701a22dd3861cd532a14281d7726210c726c9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5170831 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e4acb30c8790d9ef8af675772eda5d9f3903a662d29132ef140463453eeb717`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Fri, 16 Apr 2021 21:48:04 GMT
COPY file:b02a357b6e9250e52099dcc91c6a9a78682a192bd0850fabc93d5cdacb6fcfb3 in /nats-streaming-server 
# Fri, 16 Apr 2021 21:48:05 GMT
EXPOSE 4222 8222
# Fri, 16 Apr 2021 21:48:06 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Fri, 16 Apr 2021 21:48:07 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:fe1641db2bf227918d02728a21bd3b53989018d9c796246d3b96fcbbf75ded32`  
		Last Modified: Fri, 16 Apr 2021 21:48:50 GMT  
		Size: 5.2 MB (5170831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.21.2-windowsservercore`

```console
$ docker pull nats-streaming@sha256:0befbd41f19304f5a7776ec78fae36978bd62c3f9cad17e4980b4cf886e6f64a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1935; amd64
	-	windows version 10.0.14393.4402; amd64

### `nats-streaming:0.21.2-windowsservercore` - windows version 10.0.17763.1935; amd64

```console
$ docker pull nats-streaming@sha256:df969179961089c2884fe95d19cab9088c89cf714b5169b76e8eaefa20d26550
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2490478060 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:87797a3af44c930235285b950723e7e38b9e69e8a60449c737a88b738c5c54e1`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 08 May 2021 09:21:48 GMT
RUN Install update 1809-amd64
# Tue, 11 May 2021 23:54:13 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 May 2021 15:41:49 GMT
ENV NATS_DOCKERIZED=1
# Wed, 12 May 2021 20:09:14 GMT
ENV NATS_STREAMING_SERVER=0.21.2
# Wed, 12 May 2021 20:09:14 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.21.2/nats-streaming-server-v0.21.2-windows-amd64.zip
# Wed, 12 May 2021 20:09:15 GMT
ENV GIT_DOWNLOAD_SHA256=5d4367fea29116fcd70c364c8e808d6bc8e74214effbde83dd9548455bd06df2
# Wed, 12 May 2021 20:09:48 GMT
RUN Set-PSDebug -Trace 2
# Wed, 12 May 2021 20:11:11 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 12 May 2021 20:11:12 GMT
EXPOSE 4222 8222
# Wed, 12 May 2021 20:11:13 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 12 May 2021 20:11:14 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8116de3c91c3f1ef2d6c09b49ef5407c9b4d672896eb3af5182a997c3c5379c9`  
		Size: 756.2 MB (756156286 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c049a65ed9206719f5c04428cb853623400e8ab1668243872b1134775f752962`  
		Last Modified: Wed, 12 May 2021 00:41:58 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:262d2305f11fe8f36ef3508b42686daac7e99da966ed02f4ded1927387b1b75b`  
		Last Modified: Wed, 12 May 2021 15:48:42 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caae5631f8d4c6cdfd8103d983810b9bfbefd01878285af9f623ac2f238f3449`  
		Last Modified: Wed, 12 May 2021 20:15:53 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d63f70b8ac38a77401cdba37ded79ef5a8565d1e0e5995c31b91f7aa4ce1b3f`  
		Last Modified: Wed, 12 May 2021 20:15:52 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0116c026836dea58f1432a034571efcf1d367ff5c6871c8f0930b7c9797602b2`  
		Last Modified: Wed, 12 May 2021 20:15:52 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7934c4e249cc275fd9d51173f09fbb985aa5c6d4314dce86d94108e3391b9bd5`  
		Last Modified: Wed, 12 May 2021 20:15:51 GMT  
		Size: 5.1 MB (5097038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:448f7480833686f3bbf6a3b41420f2f5add2aae1e35e31f4b47fe4b5e7fa441f`  
		Last Modified: Wed, 12 May 2021 20:15:53 GMT  
		Size: 10.9 MB (10880522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa234e132dde31816c466d94b40cac410cddcf081c522dbbabacbaca243f86a1`  
		Last Modified: Wed, 12 May 2021 20:15:50 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db175b165b9197d8d4b1751818e16f7c87846387f6d20a58ec01c885127fdf4d`  
		Last Modified: Wed, 12 May 2021 20:15:50 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38f8e2ba8c9a144f6620284f2697e8d0220903615e9c104d76fe384d4c5f3958`  
		Last Modified: Wed, 12 May 2021 20:15:49 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.21.2-windowsservercore` - windows version 10.0.14393.4402; amd64

```console
$ docker pull nats-streaming@sha256:d15f6cc0f6f200c03c249c6fa30e1d993feabdba06c9bfb4dd25a41cb75dba02
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5817500079 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:77c238ff37580c7dd07576778ab4a469bb8b538c9e3e9990a2d98c7326094ebd`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 26 Apr 2021 17:25:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 11 May 2021 23:58:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 May 2021 15:44:16 GMT
ENV NATS_DOCKERIZED=1
# Wed, 12 May 2021 20:11:37 GMT
ENV NATS_STREAMING_SERVER=0.21.2
# Wed, 12 May 2021 20:11:38 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.21.2/nats-streaming-server-v0.21.2-windows-amd64.zip
# Wed, 12 May 2021 20:11:39 GMT
ENV GIT_DOWNLOAD_SHA256=5d4367fea29116fcd70c364c8e808d6bc8e74214effbde83dd9548455bd06df2
# Wed, 12 May 2021 20:12:54 GMT
RUN Set-PSDebug -Trace 2
# Wed, 12 May 2021 20:15:02 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 12 May 2021 20:15:03 GMT
EXPOSE 4222 8222
# Wed, 12 May 2021 20:15:04 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 12 May 2021 20:15:05 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7f532f88613ca85064b055f6b93f8517bd05feba8fdce495a6ad1421573e765e`  
		Size: 1.7 GB (1725791397 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:50d0f4595a2bdc5dc0623fbee162be09d0631373eb9e82a0b1ec387ce1512c49`  
		Last Modified: Wed, 12 May 2021 00:46:32 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b7998d92dbbcfc4e6dc106e75206a3cfde70fe601eb46b0515658f23dcd53ae`  
		Last Modified: Wed, 12 May 2021 15:49:26 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f3010a7dd8667ca84982e9114e1dc65712c28bc68c365842b10a045ca612037`  
		Last Modified: Wed, 12 May 2021 20:16:28 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df06200a155b162a6be73cde9177db0ddf3ab1d3cfbd6cde1716508ea936e815`  
		Last Modified: Wed, 12 May 2021 20:16:28 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e23a0cd6171825cfd2bf6df17479e82e5845162d61bf74cf02daf44b78ba106`  
		Last Modified: Wed, 12 May 2021 20:16:28 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67048fb7884ce62e43c9c94e93c2469620bc4f1c31de0bfed360949a4856b32c`  
		Last Modified: Wed, 12 May 2021 20:16:32 GMT  
		Size: 5.7 MB (5699433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c112a8566705980bcc28d7b657abbc41bebdba6f14cc110792896e37a8ad36c0`  
		Last Modified: Wed, 12 May 2021 20:16:48 GMT  
		Size: 16.0 MB (16012020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a61d35a77f28396bd2da2e43c4fdf316968fa5dac4db17f07873ad8f2f778e54`  
		Last Modified: Wed, 12 May 2021 20:16:25 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96acafa52a9f3be44164c214903b7fffc48d9030807ce105a6c09093f4ebe1b9`  
		Last Modified: Wed, 12 May 2021 20:16:25 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b24723ae97946b0dbd5bf2b012548e33ca907518a500ca519e4bb0317bd31e0`  
		Last Modified: Wed, 12 May 2021 20:16:25 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.21.2-windowsservercore-1809`

```console
$ docker pull nats-streaming@sha256:ea4b6301b3365558fb705235d0e6ad5d6a3fcd989167e67831738db244d553b1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1935; amd64

### `nats-streaming:0.21.2-windowsservercore-1809` - windows version 10.0.17763.1935; amd64

```console
$ docker pull nats-streaming@sha256:df969179961089c2884fe95d19cab9088c89cf714b5169b76e8eaefa20d26550
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2490478060 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:87797a3af44c930235285b950723e7e38b9e69e8a60449c737a88b738c5c54e1`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 08 May 2021 09:21:48 GMT
RUN Install update 1809-amd64
# Tue, 11 May 2021 23:54:13 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 May 2021 15:41:49 GMT
ENV NATS_DOCKERIZED=1
# Wed, 12 May 2021 20:09:14 GMT
ENV NATS_STREAMING_SERVER=0.21.2
# Wed, 12 May 2021 20:09:14 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.21.2/nats-streaming-server-v0.21.2-windows-amd64.zip
# Wed, 12 May 2021 20:09:15 GMT
ENV GIT_DOWNLOAD_SHA256=5d4367fea29116fcd70c364c8e808d6bc8e74214effbde83dd9548455bd06df2
# Wed, 12 May 2021 20:09:48 GMT
RUN Set-PSDebug -Trace 2
# Wed, 12 May 2021 20:11:11 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 12 May 2021 20:11:12 GMT
EXPOSE 4222 8222
# Wed, 12 May 2021 20:11:13 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 12 May 2021 20:11:14 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8116de3c91c3f1ef2d6c09b49ef5407c9b4d672896eb3af5182a997c3c5379c9`  
		Size: 756.2 MB (756156286 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c049a65ed9206719f5c04428cb853623400e8ab1668243872b1134775f752962`  
		Last Modified: Wed, 12 May 2021 00:41:58 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:262d2305f11fe8f36ef3508b42686daac7e99da966ed02f4ded1927387b1b75b`  
		Last Modified: Wed, 12 May 2021 15:48:42 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caae5631f8d4c6cdfd8103d983810b9bfbefd01878285af9f623ac2f238f3449`  
		Last Modified: Wed, 12 May 2021 20:15:53 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d63f70b8ac38a77401cdba37ded79ef5a8565d1e0e5995c31b91f7aa4ce1b3f`  
		Last Modified: Wed, 12 May 2021 20:15:52 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0116c026836dea58f1432a034571efcf1d367ff5c6871c8f0930b7c9797602b2`  
		Last Modified: Wed, 12 May 2021 20:15:52 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7934c4e249cc275fd9d51173f09fbb985aa5c6d4314dce86d94108e3391b9bd5`  
		Last Modified: Wed, 12 May 2021 20:15:51 GMT  
		Size: 5.1 MB (5097038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:448f7480833686f3bbf6a3b41420f2f5add2aae1e35e31f4b47fe4b5e7fa441f`  
		Last Modified: Wed, 12 May 2021 20:15:53 GMT  
		Size: 10.9 MB (10880522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa234e132dde31816c466d94b40cac410cddcf081c522dbbabacbaca243f86a1`  
		Last Modified: Wed, 12 May 2021 20:15:50 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db175b165b9197d8d4b1751818e16f7c87846387f6d20a58ec01c885127fdf4d`  
		Last Modified: Wed, 12 May 2021 20:15:50 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38f8e2ba8c9a144f6620284f2697e8d0220903615e9c104d76fe384d4c5f3958`  
		Last Modified: Wed, 12 May 2021 20:15:49 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.21.2-windowsservercore-ltsc2016`

```console
$ docker pull nats-streaming@sha256:625ab75dea32121df296345016a44bcaa577d91d7c55b131fb28fd842ab65181
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4402; amd64

### `nats-streaming:0.21.2-windowsservercore-ltsc2016` - windows version 10.0.14393.4402; amd64

```console
$ docker pull nats-streaming@sha256:d15f6cc0f6f200c03c249c6fa30e1d993feabdba06c9bfb4dd25a41cb75dba02
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5817500079 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:77c238ff37580c7dd07576778ab4a469bb8b538c9e3e9990a2d98c7326094ebd`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 26 Apr 2021 17:25:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 11 May 2021 23:58:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 May 2021 15:44:16 GMT
ENV NATS_DOCKERIZED=1
# Wed, 12 May 2021 20:11:37 GMT
ENV NATS_STREAMING_SERVER=0.21.2
# Wed, 12 May 2021 20:11:38 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.21.2/nats-streaming-server-v0.21.2-windows-amd64.zip
# Wed, 12 May 2021 20:11:39 GMT
ENV GIT_DOWNLOAD_SHA256=5d4367fea29116fcd70c364c8e808d6bc8e74214effbde83dd9548455bd06df2
# Wed, 12 May 2021 20:12:54 GMT
RUN Set-PSDebug -Trace 2
# Wed, 12 May 2021 20:15:02 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 12 May 2021 20:15:03 GMT
EXPOSE 4222 8222
# Wed, 12 May 2021 20:15:04 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 12 May 2021 20:15:05 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7f532f88613ca85064b055f6b93f8517bd05feba8fdce495a6ad1421573e765e`  
		Size: 1.7 GB (1725791397 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:50d0f4595a2bdc5dc0623fbee162be09d0631373eb9e82a0b1ec387ce1512c49`  
		Last Modified: Wed, 12 May 2021 00:46:32 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b7998d92dbbcfc4e6dc106e75206a3cfde70fe601eb46b0515658f23dcd53ae`  
		Last Modified: Wed, 12 May 2021 15:49:26 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f3010a7dd8667ca84982e9114e1dc65712c28bc68c365842b10a045ca612037`  
		Last Modified: Wed, 12 May 2021 20:16:28 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df06200a155b162a6be73cde9177db0ddf3ab1d3cfbd6cde1716508ea936e815`  
		Last Modified: Wed, 12 May 2021 20:16:28 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e23a0cd6171825cfd2bf6df17479e82e5845162d61bf74cf02daf44b78ba106`  
		Last Modified: Wed, 12 May 2021 20:16:28 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67048fb7884ce62e43c9c94e93c2469620bc4f1c31de0bfed360949a4856b32c`  
		Last Modified: Wed, 12 May 2021 20:16:32 GMT  
		Size: 5.7 MB (5699433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c112a8566705980bcc28d7b657abbc41bebdba6f14cc110792896e37a8ad36c0`  
		Last Modified: Wed, 12 May 2021 20:16:48 GMT  
		Size: 16.0 MB (16012020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a61d35a77f28396bd2da2e43c4fdf316968fa5dac4db17f07873ad8f2f778e54`  
		Last Modified: Wed, 12 May 2021 20:16:25 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96acafa52a9f3be44164c214903b7fffc48d9030807ce105a6c09093f4ebe1b9`  
		Last Modified: Wed, 12 May 2021 20:16:25 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b24723ae97946b0dbd5bf2b012548e33ca907518a500ca519e4bb0317bd31e0`  
		Last Modified: Wed, 12 May 2021 20:16:25 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:alpine`

```console
$ docker pull nats-streaming@sha256:d204ac6b58553c9632e9797984adcace87b6539d257754f1d5bdf5e4a2a8d72e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:alpine` - linux; amd64

```console
$ docker pull nats-streaming@sha256:402dacbb78f9bf5e9ea249c730f7905caa085ca665782e1cb4c6e7004f597689
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.8 MB (8774780 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f7ad70b17b46627026163460cce06023868f24d36a50cd9c261e7c6cba86e29`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Fri, 16 Apr 2021 21:25:11 GMT
ENV NATS_STREAMING_SERVER=0.21.2
# Fri, 16 Apr 2021 21:25:14 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='56bcfea3c3d7a232dab93ad280ce8f8df87959ac000c7d24ce03dbab2f4c4d2b' ;; 		armhf) natsArch='arm6'; sha256='34d7032ba61724ec55d78cb94a5ed244754509b8b957e1e7e4f0579292c35a7f' ;; 		armv7) natsArch='arm7'; sha256='b4869711408e3823c8818e934bf90d07ed51f350147702b80831fb4fe5a390d2' ;; 		x86_64) natsArch='amd64'; sha256='7a401a3af7eb56a0d1d3b207dc517222697b48cb7e9e524848e62bd13393d23a' ;; 		x86) natsArch='386'; sha256='58aa4cad4c75920522ec0457b79d889f9c740c248647b875254cd1313517620c' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 16 Apr 2021 21:25:14 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Fri, 16 Apr 2021 21:25:15 GMT
EXPOSE 4222 8222
# Fri, 16 Apr 2021 21:25:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Apr 2021 21:25:15 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:269577e93d92e9e558c3607d8b5e74978c939fc643895de15fd70ef06b811323`  
		Last Modified: Fri, 16 Apr 2021 21:25:54 GMT  
		Size: 6.0 MB (5962389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5fa1ca69a5dc5f7aecbfca382d45ab09423bb9d103c6567abc37af7b842073a`  
		Last Modified: Fri, 16 Apr 2021 21:25:54 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:e03de3640ce68bbb19cd2b5e8dc2a1454fbba1b369a4c236f09b6630197b6fa0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.2 MB (8156933 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a345ef8cbbe68103787d05c9dbd22742cc95b726776cbf30298c3ca98487b63`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 14 Apr 2021 18:49:39 GMT
ADD file:4479f0a51530e039edf231d87201896dcff908aa542a613cdccb015f93dda8a3 in / 
# Wed, 14 Apr 2021 18:49:40 GMT
CMD ["/bin/sh"]
# Fri, 16 Apr 2021 21:02:04 GMT
ENV NATS_STREAMING_SERVER=0.21.2
# Fri, 16 Apr 2021 21:02:23 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='56bcfea3c3d7a232dab93ad280ce8f8df87959ac000c7d24ce03dbab2f4c4d2b' ;; 		armhf) natsArch='arm6'; sha256='34d7032ba61724ec55d78cb94a5ed244754509b8b957e1e7e4f0579292c35a7f' ;; 		armv7) natsArch='arm7'; sha256='b4869711408e3823c8818e934bf90d07ed51f350147702b80831fb4fe5a390d2' ;; 		x86_64) natsArch='amd64'; sha256='7a401a3af7eb56a0d1d3b207dc517222697b48cb7e9e524848e62bd13393d23a' ;; 		x86) natsArch='386'; sha256='58aa4cad4c75920522ec0457b79d889f9c740c248647b875254cd1313517620c' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 16 Apr 2021 21:02:26 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Fri, 16 Apr 2021 21:02:27 GMT
EXPOSE 4222 8222
# Fri, 16 Apr 2021 21:02:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Apr 2021 21:02:29 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:740c950346cf39c85b52576998695c9b909c24a58a8bb1b64cce91fda3ef1d3a`  
		Last Modified: Wed, 14 Apr 2021 18:50:30 GMT  
		Size: 2.6 MB (2622131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e538f4430325ed9ef756e0e521a859c9466b9b7a45a8662e4f29f1ec5f8c3a7d`  
		Last Modified: Fri, 16 Apr 2021 21:03:32 GMT  
		Size: 5.5 MB (5534381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc165822006c8e13ee1ee6756545e0f021a059f974288d6c953febdeea6a83d3`  
		Last Modified: Fri, 16 Apr 2021 21:03:30 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:ea133d32e6510a0d1822a1ea1cfcca41e3cbd747a3d69491aee62319937e892d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.0 MB (7951606 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc13824ee86fb9d0c1609b885378ba366f3883903bfe990fb27464bce6c02686`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 14 Apr 2021 18:57:39 GMT
ADD file:028c5b473d862250586e174c5dd19b37f8fc3bffbc02d888e72df30f32fd6129 in / 
# Wed, 14 Apr 2021 18:57:39 GMT
CMD ["/bin/sh"]
# Fri, 16 Apr 2021 20:59:08 GMT
ENV NATS_STREAMING_SERVER=0.21.2
# Fri, 16 Apr 2021 20:59:12 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='56bcfea3c3d7a232dab93ad280ce8f8df87959ac000c7d24ce03dbab2f4c4d2b' ;; 		armhf) natsArch='arm6'; sha256='34d7032ba61724ec55d78cb94a5ed244754509b8b957e1e7e4f0579292c35a7f' ;; 		armv7) natsArch='arm7'; sha256='b4869711408e3823c8818e934bf90d07ed51f350147702b80831fb4fe5a390d2' ;; 		x86_64) natsArch='amd64'; sha256='7a401a3af7eb56a0d1d3b207dc517222697b48cb7e9e524848e62bd13393d23a' ;; 		x86) natsArch='386'; sha256='58aa4cad4c75920522ec0457b79d889f9c740c248647b875254cd1313517620c' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 16 Apr 2021 20:59:13 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Fri, 16 Apr 2021 20:59:14 GMT
EXPOSE 4222 8222
# Fri, 16 Apr 2021 20:59:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Apr 2021 20:59:16 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:e160e00eb35d5bc2373770873fbc9c8f5706045b0b06bfd1c364fcf69f02e9fe`  
		Last Modified: Wed, 14 Apr 2021 18:58:36 GMT  
		Size: 2.4 MB (2424145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6b86c52fd84fa988d60547be09b11af6fcac2dffa6b340e92b776a0fc89a298`  
		Last Modified: Fri, 16 Apr 2021 21:00:42 GMT  
		Size: 5.5 MB (5527039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7b279e3ce6e5cfc3967a4acbf6dc2563f1715817b059d6f320b53cbc21b74e1`  
		Last Modified: Fri, 16 Apr 2021 21:00:40 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:febf36c660fc36bcbf3da9945707f541e81665b0d21a0f1c6c8220543697a757
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.2 MB (8165113 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd79dce90e049636e2513bd55a0b3178cb59197d3dfc53cbed474dbbd5de0f1f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 14 Apr 2021 18:42:37 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Wed, 14 Apr 2021 18:42:38 GMT
CMD ["/bin/sh"]
# Fri, 16 Apr 2021 21:44:03 GMT
ENV NATS_STREAMING_SERVER=0.21.2
# Fri, 16 Apr 2021 21:44:07 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='56bcfea3c3d7a232dab93ad280ce8f8df87959ac000c7d24ce03dbab2f4c4d2b' ;; 		armhf) natsArch='arm6'; sha256='34d7032ba61724ec55d78cb94a5ed244754509b8b957e1e7e4f0579292c35a7f' ;; 		armv7) natsArch='arm7'; sha256='b4869711408e3823c8818e934bf90d07ed51f350147702b80831fb4fe5a390d2' ;; 		x86_64) natsArch='amd64'; sha256='7a401a3af7eb56a0d1d3b207dc517222697b48cb7e9e524848e62bd13393d23a' ;; 		x86) natsArch='386'; sha256='58aa4cad4c75920522ec0457b79d889f9c740c248647b875254cd1313517620c' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 16 Apr 2021 21:44:08 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Fri, 16 Apr 2021 21:44:09 GMT
EXPOSE 4222 8222
# Fri, 16 Apr 2021 21:44:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Apr 2021 21:44:10 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03a1a4dae3b1b310f0231f28f4db383d7605066343274881c5be1300ebe64f51`  
		Last Modified: Fri, 16 Apr 2021 21:48:37 GMT  
		Size: 5.5 MB (5452665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0a06774842e75925d8884fc1ea5a3e83c2c8054d4fb443ad11021c5866b0617`  
		Last Modified: Fri, 16 Apr 2021 21:48:36 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:alpine3.13`

```console
$ docker pull nats-streaming@sha256:d204ac6b58553c9632e9797984adcace87b6539d257754f1d5bdf5e4a2a8d72e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:alpine3.13` - linux; amd64

```console
$ docker pull nats-streaming@sha256:402dacbb78f9bf5e9ea249c730f7905caa085ca665782e1cb4c6e7004f597689
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.8 MB (8774780 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f7ad70b17b46627026163460cce06023868f24d36a50cd9c261e7c6cba86e29`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Fri, 16 Apr 2021 21:25:11 GMT
ENV NATS_STREAMING_SERVER=0.21.2
# Fri, 16 Apr 2021 21:25:14 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='56bcfea3c3d7a232dab93ad280ce8f8df87959ac000c7d24ce03dbab2f4c4d2b' ;; 		armhf) natsArch='arm6'; sha256='34d7032ba61724ec55d78cb94a5ed244754509b8b957e1e7e4f0579292c35a7f' ;; 		armv7) natsArch='arm7'; sha256='b4869711408e3823c8818e934bf90d07ed51f350147702b80831fb4fe5a390d2' ;; 		x86_64) natsArch='amd64'; sha256='7a401a3af7eb56a0d1d3b207dc517222697b48cb7e9e524848e62bd13393d23a' ;; 		x86) natsArch='386'; sha256='58aa4cad4c75920522ec0457b79d889f9c740c248647b875254cd1313517620c' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 16 Apr 2021 21:25:14 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Fri, 16 Apr 2021 21:25:15 GMT
EXPOSE 4222 8222
# Fri, 16 Apr 2021 21:25:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Apr 2021 21:25:15 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:269577e93d92e9e558c3607d8b5e74978c939fc643895de15fd70ef06b811323`  
		Last Modified: Fri, 16 Apr 2021 21:25:54 GMT  
		Size: 6.0 MB (5962389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5fa1ca69a5dc5f7aecbfca382d45ab09423bb9d103c6567abc37af7b842073a`  
		Last Modified: Fri, 16 Apr 2021 21:25:54 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine3.13` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:e03de3640ce68bbb19cd2b5e8dc2a1454fbba1b369a4c236f09b6630197b6fa0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.2 MB (8156933 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a345ef8cbbe68103787d05c9dbd22742cc95b726776cbf30298c3ca98487b63`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 14 Apr 2021 18:49:39 GMT
ADD file:4479f0a51530e039edf231d87201896dcff908aa542a613cdccb015f93dda8a3 in / 
# Wed, 14 Apr 2021 18:49:40 GMT
CMD ["/bin/sh"]
# Fri, 16 Apr 2021 21:02:04 GMT
ENV NATS_STREAMING_SERVER=0.21.2
# Fri, 16 Apr 2021 21:02:23 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='56bcfea3c3d7a232dab93ad280ce8f8df87959ac000c7d24ce03dbab2f4c4d2b' ;; 		armhf) natsArch='arm6'; sha256='34d7032ba61724ec55d78cb94a5ed244754509b8b957e1e7e4f0579292c35a7f' ;; 		armv7) natsArch='arm7'; sha256='b4869711408e3823c8818e934bf90d07ed51f350147702b80831fb4fe5a390d2' ;; 		x86_64) natsArch='amd64'; sha256='7a401a3af7eb56a0d1d3b207dc517222697b48cb7e9e524848e62bd13393d23a' ;; 		x86) natsArch='386'; sha256='58aa4cad4c75920522ec0457b79d889f9c740c248647b875254cd1313517620c' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 16 Apr 2021 21:02:26 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Fri, 16 Apr 2021 21:02:27 GMT
EXPOSE 4222 8222
# Fri, 16 Apr 2021 21:02:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Apr 2021 21:02:29 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:740c950346cf39c85b52576998695c9b909c24a58a8bb1b64cce91fda3ef1d3a`  
		Last Modified: Wed, 14 Apr 2021 18:50:30 GMT  
		Size: 2.6 MB (2622131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e538f4430325ed9ef756e0e521a859c9466b9b7a45a8662e4f29f1ec5f8c3a7d`  
		Last Modified: Fri, 16 Apr 2021 21:03:32 GMT  
		Size: 5.5 MB (5534381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc165822006c8e13ee1ee6756545e0f021a059f974288d6c953febdeea6a83d3`  
		Last Modified: Fri, 16 Apr 2021 21:03:30 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine3.13` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:ea133d32e6510a0d1822a1ea1cfcca41e3cbd747a3d69491aee62319937e892d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.0 MB (7951606 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc13824ee86fb9d0c1609b885378ba366f3883903bfe990fb27464bce6c02686`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 14 Apr 2021 18:57:39 GMT
ADD file:028c5b473d862250586e174c5dd19b37f8fc3bffbc02d888e72df30f32fd6129 in / 
# Wed, 14 Apr 2021 18:57:39 GMT
CMD ["/bin/sh"]
# Fri, 16 Apr 2021 20:59:08 GMT
ENV NATS_STREAMING_SERVER=0.21.2
# Fri, 16 Apr 2021 20:59:12 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='56bcfea3c3d7a232dab93ad280ce8f8df87959ac000c7d24ce03dbab2f4c4d2b' ;; 		armhf) natsArch='arm6'; sha256='34d7032ba61724ec55d78cb94a5ed244754509b8b957e1e7e4f0579292c35a7f' ;; 		armv7) natsArch='arm7'; sha256='b4869711408e3823c8818e934bf90d07ed51f350147702b80831fb4fe5a390d2' ;; 		x86_64) natsArch='amd64'; sha256='7a401a3af7eb56a0d1d3b207dc517222697b48cb7e9e524848e62bd13393d23a' ;; 		x86) natsArch='386'; sha256='58aa4cad4c75920522ec0457b79d889f9c740c248647b875254cd1313517620c' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 16 Apr 2021 20:59:13 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Fri, 16 Apr 2021 20:59:14 GMT
EXPOSE 4222 8222
# Fri, 16 Apr 2021 20:59:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Apr 2021 20:59:16 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:e160e00eb35d5bc2373770873fbc9c8f5706045b0b06bfd1c364fcf69f02e9fe`  
		Last Modified: Wed, 14 Apr 2021 18:58:36 GMT  
		Size: 2.4 MB (2424145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6b86c52fd84fa988d60547be09b11af6fcac2dffa6b340e92b776a0fc89a298`  
		Last Modified: Fri, 16 Apr 2021 21:00:42 GMT  
		Size: 5.5 MB (5527039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7b279e3ce6e5cfc3967a4acbf6dc2563f1715817b059d6f320b53cbc21b74e1`  
		Last Modified: Fri, 16 Apr 2021 21:00:40 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine3.13` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:febf36c660fc36bcbf3da9945707f541e81665b0d21a0f1c6c8220543697a757
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.2 MB (8165113 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd79dce90e049636e2513bd55a0b3178cb59197d3dfc53cbed474dbbd5de0f1f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 14 Apr 2021 18:42:37 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Wed, 14 Apr 2021 18:42:38 GMT
CMD ["/bin/sh"]
# Fri, 16 Apr 2021 21:44:03 GMT
ENV NATS_STREAMING_SERVER=0.21.2
# Fri, 16 Apr 2021 21:44:07 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='56bcfea3c3d7a232dab93ad280ce8f8df87959ac000c7d24ce03dbab2f4c4d2b' ;; 		armhf) natsArch='arm6'; sha256='34d7032ba61724ec55d78cb94a5ed244754509b8b957e1e7e4f0579292c35a7f' ;; 		armv7) natsArch='arm7'; sha256='b4869711408e3823c8818e934bf90d07ed51f350147702b80831fb4fe5a390d2' ;; 		x86_64) natsArch='amd64'; sha256='7a401a3af7eb56a0d1d3b207dc517222697b48cb7e9e524848e62bd13393d23a' ;; 		x86) natsArch='386'; sha256='58aa4cad4c75920522ec0457b79d889f9c740c248647b875254cd1313517620c' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 16 Apr 2021 21:44:08 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Fri, 16 Apr 2021 21:44:09 GMT
EXPOSE 4222 8222
# Fri, 16 Apr 2021 21:44:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Apr 2021 21:44:10 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03a1a4dae3b1b310f0231f28f4db383d7605066343274881c5be1300ebe64f51`  
		Last Modified: Fri, 16 Apr 2021 21:48:37 GMT  
		Size: 5.5 MB (5452665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0a06774842e75925d8884fc1ea5a3e83c2c8054d4fb443ad11021c5866b0617`  
		Last Modified: Fri, 16 Apr 2021 21:48:36 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:latest`

```console
$ docker pull nats-streaming@sha256:8e9036a7e32179bf55236241656e9555336215146d30129b5ac664f94fd73ed6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.1935; amd64

### `nats-streaming:latest` - linux; amd64

```console
$ docker pull nats-streaming@sha256:883d4d7a47db4d1c911cf0c23dad30011b46727297d1158bede3d833455a49e4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.7 MB (5680535 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d1e123176c313a4b94f8c0fdf6cac9abdd85a1bd6edf3f7cc6e7ed61852d19a`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Fri, 16 Apr 2021 21:25:32 GMT
COPY file:aefc6cbeadb611214d28b81a278a791c774a4bbc969528522aae7abe7c4e2784 in /nats-streaming-server 
# Fri, 16 Apr 2021 21:25:32 GMT
EXPOSE 4222 8222
# Fri, 16 Apr 2021 21:25:32 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Fri, 16 Apr 2021 21:25:33 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:087a668f89c4000c166ca5a16dd40fee8206986ce9b47a92d224b78214f3db5c`  
		Last Modified: Fri, 16 Apr 2021 21:26:16 GMT  
		Size: 5.7 MB (5680535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:latest` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:9dc93ca8dad040be30fe0949d19f04a6b1775750838d70d2fb12f3aa9f40b4f8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.3 MB (5253054 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba356cbd8fdcd90e529d00104791d07c50c101937487a0b8647b06226bfdef9a`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Fri, 16 Apr 2021 21:02:53 GMT
COPY file:c58b6e2180eb9d24d595f35c2205c2d9b4f80315beb0f166e20a7340cf3f2536 in /nats-streaming-server 
# Fri, 16 Apr 2021 21:03:00 GMT
EXPOSE 4222 8222
# Fri, 16 Apr 2021 21:03:04 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Fri, 16 Apr 2021 21:03:07 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:3542c02ee947256ff50165b76289b4dd90e7c82bfb7b0b983b4d66d4b1128e9a`  
		Last Modified: Fri, 16 Apr 2021 21:03:44 GMT  
		Size: 5.3 MB (5253054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:latest` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:10f5838646402cebd5c40f8f02991aad0ca3767b13b3024054e5e04026d3c778
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5246280 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:409bfb98a0a11b06fb4c8a044cda742270c21f5082ef80b63e7893cb4ce2f9c3`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Fri, 16 Apr 2021 21:00:05 GMT
COPY file:7ad2a856b4d75bdc56fbd35738819610cc3c26111897fc883c3af7db16d4fa87 in /nats-streaming-server 
# Fri, 16 Apr 2021 21:00:07 GMT
EXPOSE 4222 8222
# Fri, 16 Apr 2021 21:00:09 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Fri, 16 Apr 2021 21:00:10 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:76bf01e9a89a0de09d5ab72dd4ec7e4c9f561a27756ceb73bf0365f192de2d18`  
		Last Modified: Fri, 16 Apr 2021 21:01:13 GMT  
		Size: 5.2 MB (5246280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:latest` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:3bf4856546fa4657b125293b8ed701a22dd3861cd532a14281d7726210c726c9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5170831 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e4acb30c8790d9ef8af675772eda5d9f3903a662d29132ef140463453eeb717`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Fri, 16 Apr 2021 21:48:04 GMT
COPY file:b02a357b6e9250e52099dcc91c6a9a78682a192bd0850fabc93d5cdacb6fcfb3 in /nats-streaming-server 
# Fri, 16 Apr 2021 21:48:05 GMT
EXPOSE 4222 8222
# Fri, 16 Apr 2021 21:48:06 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Fri, 16 Apr 2021 21:48:07 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:fe1641db2bf227918d02728a21bd3b53989018d9c796246d3b96fcbbf75ded32`  
		Last Modified: Fri, 16 Apr 2021 21:48:50 GMT  
		Size: 5.2 MB (5170831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:latest` - windows version 10.0.17763.1935; amd64

```console
$ docker pull nats-streaming@sha256:881fbff9b8ea5b5dce5d1e1fb341a4ab9a9caab12b0faf072dc89f9ab61792e9
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.2 MB (107191037 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9db19cc378f4cdf654406f9ff0a58704fbec29c0b23fa37b4919bcedd9a0a02`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Fri, 07 May 2021 11:54:57 GMT
RUN Apply image 1809-amd64
# Wed, 12 May 2021 15:44:03 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 12 May 2021 20:11:27 GMT
RUN cmd /S /C #(nop) COPY file:adacf7e54ef5a782ae37764b59883ad6a48b32c36c576816360f94cba82ba458 in C:\nats-streaming-server.exe 
# Wed, 12 May 2021 20:11:28 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 12 May 2021 20:11:29 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 12 May 2021 20:11:30 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:b9043d31610e0dfa43b1afe286f8918b6e3bf69ece50f44424b29d48f20aa662`  
		Size: 101.4 MB (101375240 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:95b58e21e5cdf4e2f9e5c87487734458885da325634d72f9c4e6583b353af06f`  
		Last Modified: Wed, 12 May 2021 15:49:02 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab3056c607d4b35216a2f74c2f849eb0c970001dc87bf45f90aea3ca4e8d9f05`  
		Last Modified: Wed, 12 May 2021 20:16:11 GMT  
		Size: 5.8 MB (5811203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:747d370e1cec130d4e6c1a20a9b8d049a93543b695b60a4fc0b5473758786920`  
		Last Modified: Wed, 12 May 2021 20:16:10 GMT  
		Size: 1.2 KB (1178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38d9d67f8ca438fa616690db8fc1087b47f11ad390d7a29761bfc08c67605c85`  
		Last Modified: Wed, 12 May 2021 20:16:10 GMT  
		Size: 1.1 KB (1105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e187a1b2446f3948440517b1cd475bdb32db16b4643b465f30313f8bbfe01d6`  
		Last Modified: Wed, 12 May 2021 20:16:10 GMT  
		Size: 1.2 KB (1161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:linux`

```console
$ docker pull nats-streaming@sha256:2bf298093b69248cb6e82aa7c64d50c1a45480ad23a8ced79a5ddf588ee69102
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:linux` - linux; amd64

```console
$ docker pull nats-streaming@sha256:883d4d7a47db4d1c911cf0c23dad30011b46727297d1158bede3d833455a49e4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.7 MB (5680535 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d1e123176c313a4b94f8c0fdf6cac9abdd85a1bd6edf3f7cc6e7ed61852d19a`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Fri, 16 Apr 2021 21:25:32 GMT
COPY file:aefc6cbeadb611214d28b81a278a791c774a4bbc969528522aae7abe7c4e2784 in /nats-streaming-server 
# Fri, 16 Apr 2021 21:25:32 GMT
EXPOSE 4222 8222
# Fri, 16 Apr 2021 21:25:32 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Fri, 16 Apr 2021 21:25:33 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:087a668f89c4000c166ca5a16dd40fee8206986ce9b47a92d224b78214f3db5c`  
		Last Modified: Fri, 16 Apr 2021 21:26:16 GMT  
		Size: 5.7 MB (5680535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:linux` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:9dc93ca8dad040be30fe0949d19f04a6b1775750838d70d2fb12f3aa9f40b4f8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.3 MB (5253054 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba356cbd8fdcd90e529d00104791d07c50c101937487a0b8647b06226bfdef9a`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Fri, 16 Apr 2021 21:02:53 GMT
COPY file:c58b6e2180eb9d24d595f35c2205c2d9b4f80315beb0f166e20a7340cf3f2536 in /nats-streaming-server 
# Fri, 16 Apr 2021 21:03:00 GMT
EXPOSE 4222 8222
# Fri, 16 Apr 2021 21:03:04 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Fri, 16 Apr 2021 21:03:07 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:3542c02ee947256ff50165b76289b4dd90e7c82bfb7b0b983b4d66d4b1128e9a`  
		Last Modified: Fri, 16 Apr 2021 21:03:44 GMT  
		Size: 5.3 MB (5253054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:linux` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:10f5838646402cebd5c40f8f02991aad0ca3767b13b3024054e5e04026d3c778
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5246280 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:409bfb98a0a11b06fb4c8a044cda742270c21f5082ef80b63e7893cb4ce2f9c3`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Fri, 16 Apr 2021 21:00:05 GMT
COPY file:7ad2a856b4d75bdc56fbd35738819610cc3c26111897fc883c3af7db16d4fa87 in /nats-streaming-server 
# Fri, 16 Apr 2021 21:00:07 GMT
EXPOSE 4222 8222
# Fri, 16 Apr 2021 21:00:09 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Fri, 16 Apr 2021 21:00:10 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:76bf01e9a89a0de09d5ab72dd4ec7e4c9f561a27756ceb73bf0365f192de2d18`  
		Last Modified: Fri, 16 Apr 2021 21:01:13 GMT  
		Size: 5.2 MB (5246280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:linux` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:3bf4856546fa4657b125293b8ed701a22dd3861cd532a14281d7726210c726c9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5170831 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e4acb30c8790d9ef8af675772eda5d9f3903a662d29132ef140463453eeb717`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Fri, 16 Apr 2021 21:48:04 GMT
COPY file:b02a357b6e9250e52099dcc91c6a9a78682a192bd0850fabc93d5cdacb6fcfb3 in /nats-streaming-server 
# Fri, 16 Apr 2021 21:48:05 GMT
EXPOSE 4222 8222
# Fri, 16 Apr 2021 21:48:06 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Fri, 16 Apr 2021 21:48:07 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:fe1641db2bf227918d02728a21bd3b53989018d9c796246d3b96fcbbf75ded32`  
		Last Modified: Fri, 16 Apr 2021 21:48:50 GMT  
		Size: 5.2 MB (5170831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:nanoserver`

```console
$ docker pull nats-streaming@sha256:ec0aed95b5234c5cc882c7be18390dfb68a43a5285973d2264fc7cea404785ba
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1935; amd64

### `nats-streaming:nanoserver` - windows version 10.0.17763.1935; amd64

```console
$ docker pull nats-streaming@sha256:881fbff9b8ea5b5dce5d1e1fb341a4ab9a9caab12b0faf072dc89f9ab61792e9
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.2 MB (107191037 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9db19cc378f4cdf654406f9ff0a58704fbec29c0b23fa37b4919bcedd9a0a02`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Fri, 07 May 2021 11:54:57 GMT
RUN Apply image 1809-amd64
# Wed, 12 May 2021 15:44:03 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 12 May 2021 20:11:27 GMT
RUN cmd /S /C #(nop) COPY file:adacf7e54ef5a782ae37764b59883ad6a48b32c36c576816360f94cba82ba458 in C:\nats-streaming-server.exe 
# Wed, 12 May 2021 20:11:28 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 12 May 2021 20:11:29 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 12 May 2021 20:11:30 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:b9043d31610e0dfa43b1afe286f8918b6e3bf69ece50f44424b29d48f20aa662`  
		Size: 101.4 MB (101375240 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:95b58e21e5cdf4e2f9e5c87487734458885da325634d72f9c4e6583b353af06f`  
		Last Modified: Wed, 12 May 2021 15:49:02 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab3056c607d4b35216a2f74c2f849eb0c970001dc87bf45f90aea3ca4e8d9f05`  
		Last Modified: Wed, 12 May 2021 20:16:11 GMT  
		Size: 5.8 MB (5811203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:747d370e1cec130d4e6c1a20a9b8d049a93543b695b60a4fc0b5473758786920`  
		Last Modified: Wed, 12 May 2021 20:16:10 GMT  
		Size: 1.2 KB (1178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38d9d67f8ca438fa616690db8fc1087b47f11ad390d7a29761bfc08c67605c85`  
		Last Modified: Wed, 12 May 2021 20:16:10 GMT  
		Size: 1.1 KB (1105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e187a1b2446f3948440517b1cd475bdb32db16b4643b465f30313f8bbfe01d6`  
		Last Modified: Wed, 12 May 2021 20:16:10 GMT  
		Size: 1.2 KB (1161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:nanoserver-1809`

```console
$ docker pull nats-streaming@sha256:ec0aed95b5234c5cc882c7be18390dfb68a43a5285973d2264fc7cea404785ba
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1935; amd64

### `nats-streaming:nanoserver-1809` - windows version 10.0.17763.1935; amd64

```console
$ docker pull nats-streaming@sha256:881fbff9b8ea5b5dce5d1e1fb341a4ab9a9caab12b0faf072dc89f9ab61792e9
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.2 MB (107191037 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9db19cc378f4cdf654406f9ff0a58704fbec29c0b23fa37b4919bcedd9a0a02`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Fri, 07 May 2021 11:54:57 GMT
RUN Apply image 1809-amd64
# Wed, 12 May 2021 15:44:03 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 12 May 2021 20:11:27 GMT
RUN cmd /S /C #(nop) COPY file:adacf7e54ef5a782ae37764b59883ad6a48b32c36c576816360f94cba82ba458 in C:\nats-streaming-server.exe 
# Wed, 12 May 2021 20:11:28 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 12 May 2021 20:11:29 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 12 May 2021 20:11:30 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:b9043d31610e0dfa43b1afe286f8918b6e3bf69ece50f44424b29d48f20aa662`  
		Size: 101.4 MB (101375240 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:95b58e21e5cdf4e2f9e5c87487734458885da325634d72f9c4e6583b353af06f`  
		Last Modified: Wed, 12 May 2021 15:49:02 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab3056c607d4b35216a2f74c2f849eb0c970001dc87bf45f90aea3ca4e8d9f05`  
		Last Modified: Wed, 12 May 2021 20:16:11 GMT  
		Size: 5.8 MB (5811203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:747d370e1cec130d4e6c1a20a9b8d049a93543b695b60a4fc0b5473758786920`  
		Last Modified: Wed, 12 May 2021 20:16:10 GMT  
		Size: 1.2 KB (1178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38d9d67f8ca438fa616690db8fc1087b47f11ad390d7a29761bfc08c67605c85`  
		Last Modified: Wed, 12 May 2021 20:16:10 GMT  
		Size: 1.1 KB (1105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e187a1b2446f3948440517b1cd475bdb32db16b4643b465f30313f8bbfe01d6`  
		Last Modified: Wed, 12 May 2021 20:16:10 GMT  
		Size: 1.2 KB (1161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:scratch`

```console
$ docker pull nats-streaming@sha256:2bf298093b69248cb6e82aa7c64d50c1a45480ad23a8ced79a5ddf588ee69102
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:scratch` - linux; amd64

```console
$ docker pull nats-streaming@sha256:883d4d7a47db4d1c911cf0c23dad30011b46727297d1158bede3d833455a49e4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.7 MB (5680535 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d1e123176c313a4b94f8c0fdf6cac9abdd85a1bd6edf3f7cc6e7ed61852d19a`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Fri, 16 Apr 2021 21:25:32 GMT
COPY file:aefc6cbeadb611214d28b81a278a791c774a4bbc969528522aae7abe7c4e2784 in /nats-streaming-server 
# Fri, 16 Apr 2021 21:25:32 GMT
EXPOSE 4222 8222
# Fri, 16 Apr 2021 21:25:32 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Fri, 16 Apr 2021 21:25:33 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:087a668f89c4000c166ca5a16dd40fee8206986ce9b47a92d224b78214f3db5c`  
		Last Modified: Fri, 16 Apr 2021 21:26:16 GMT  
		Size: 5.7 MB (5680535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:scratch` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:9dc93ca8dad040be30fe0949d19f04a6b1775750838d70d2fb12f3aa9f40b4f8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.3 MB (5253054 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba356cbd8fdcd90e529d00104791d07c50c101937487a0b8647b06226bfdef9a`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Fri, 16 Apr 2021 21:02:53 GMT
COPY file:c58b6e2180eb9d24d595f35c2205c2d9b4f80315beb0f166e20a7340cf3f2536 in /nats-streaming-server 
# Fri, 16 Apr 2021 21:03:00 GMT
EXPOSE 4222 8222
# Fri, 16 Apr 2021 21:03:04 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Fri, 16 Apr 2021 21:03:07 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:3542c02ee947256ff50165b76289b4dd90e7c82bfb7b0b983b4d66d4b1128e9a`  
		Last Modified: Fri, 16 Apr 2021 21:03:44 GMT  
		Size: 5.3 MB (5253054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:scratch` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:10f5838646402cebd5c40f8f02991aad0ca3767b13b3024054e5e04026d3c778
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5246280 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:409bfb98a0a11b06fb4c8a044cda742270c21f5082ef80b63e7893cb4ce2f9c3`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Fri, 16 Apr 2021 21:00:05 GMT
COPY file:7ad2a856b4d75bdc56fbd35738819610cc3c26111897fc883c3af7db16d4fa87 in /nats-streaming-server 
# Fri, 16 Apr 2021 21:00:07 GMT
EXPOSE 4222 8222
# Fri, 16 Apr 2021 21:00:09 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Fri, 16 Apr 2021 21:00:10 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:76bf01e9a89a0de09d5ab72dd4ec7e4c9f561a27756ceb73bf0365f192de2d18`  
		Last Modified: Fri, 16 Apr 2021 21:01:13 GMT  
		Size: 5.2 MB (5246280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:scratch` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:3bf4856546fa4657b125293b8ed701a22dd3861cd532a14281d7726210c726c9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5170831 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e4acb30c8790d9ef8af675772eda5d9f3903a662d29132ef140463453eeb717`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Fri, 16 Apr 2021 21:48:04 GMT
COPY file:b02a357b6e9250e52099dcc91c6a9a78682a192bd0850fabc93d5cdacb6fcfb3 in /nats-streaming-server 
# Fri, 16 Apr 2021 21:48:05 GMT
EXPOSE 4222 8222
# Fri, 16 Apr 2021 21:48:06 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Fri, 16 Apr 2021 21:48:07 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:fe1641db2bf227918d02728a21bd3b53989018d9c796246d3b96fcbbf75ded32`  
		Last Modified: Fri, 16 Apr 2021 21:48:50 GMT  
		Size: 5.2 MB (5170831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:windowsservercore`

```console
$ docker pull nats-streaming@sha256:0befbd41f19304f5a7776ec78fae36978bd62c3f9cad17e4980b4cf886e6f64a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1935; amd64
	-	windows version 10.0.14393.4402; amd64

### `nats-streaming:windowsservercore` - windows version 10.0.17763.1935; amd64

```console
$ docker pull nats-streaming@sha256:df969179961089c2884fe95d19cab9088c89cf714b5169b76e8eaefa20d26550
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2490478060 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:87797a3af44c930235285b950723e7e38b9e69e8a60449c737a88b738c5c54e1`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 08 May 2021 09:21:48 GMT
RUN Install update 1809-amd64
# Tue, 11 May 2021 23:54:13 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 May 2021 15:41:49 GMT
ENV NATS_DOCKERIZED=1
# Wed, 12 May 2021 20:09:14 GMT
ENV NATS_STREAMING_SERVER=0.21.2
# Wed, 12 May 2021 20:09:14 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.21.2/nats-streaming-server-v0.21.2-windows-amd64.zip
# Wed, 12 May 2021 20:09:15 GMT
ENV GIT_DOWNLOAD_SHA256=5d4367fea29116fcd70c364c8e808d6bc8e74214effbde83dd9548455bd06df2
# Wed, 12 May 2021 20:09:48 GMT
RUN Set-PSDebug -Trace 2
# Wed, 12 May 2021 20:11:11 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 12 May 2021 20:11:12 GMT
EXPOSE 4222 8222
# Wed, 12 May 2021 20:11:13 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 12 May 2021 20:11:14 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8116de3c91c3f1ef2d6c09b49ef5407c9b4d672896eb3af5182a997c3c5379c9`  
		Size: 756.2 MB (756156286 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c049a65ed9206719f5c04428cb853623400e8ab1668243872b1134775f752962`  
		Last Modified: Wed, 12 May 2021 00:41:58 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:262d2305f11fe8f36ef3508b42686daac7e99da966ed02f4ded1927387b1b75b`  
		Last Modified: Wed, 12 May 2021 15:48:42 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caae5631f8d4c6cdfd8103d983810b9bfbefd01878285af9f623ac2f238f3449`  
		Last Modified: Wed, 12 May 2021 20:15:53 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d63f70b8ac38a77401cdba37ded79ef5a8565d1e0e5995c31b91f7aa4ce1b3f`  
		Last Modified: Wed, 12 May 2021 20:15:52 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0116c026836dea58f1432a034571efcf1d367ff5c6871c8f0930b7c9797602b2`  
		Last Modified: Wed, 12 May 2021 20:15:52 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7934c4e249cc275fd9d51173f09fbb985aa5c6d4314dce86d94108e3391b9bd5`  
		Last Modified: Wed, 12 May 2021 20:15:51 GMT  
		Size: 5.1 MB (5097038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:448f7480833686f3bbf6a3b41420f2f5add2aae1e35e31f4b47fe4b5e7fa441f`  
		Last Modified: Wed, 12 May 2021 20:15:53 GMT  
		Size: 10.9 MB (10880522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa234e132dde31816c466d94b40cac410cddcf081c522dbbabacbaca243f86a1`  
		Last Modified: Wed, 12 May 2021 20:15:50 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db175b165b9197d8d4b1751818e16f7c87846387f6d20a58ec01c885127fdf4d`  
		Last Modified: Wed, 12 May 2021 20:15:50 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38f8e2ba8c9a144f6620284f2697e8d0220903615e9c104d76fe384d4c5f3958`  
		Last Modified: Wed, 12 May 2021 20:15:49 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:windowsservercore` - windows version 10.0.14393.4402; amd64

```console
$ docker pull nats-streaming@sha256:d15f6cc0f6f200c03c249c6fa30e1d993feabdba06c9bfb4dd25a41cb75dba02
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5817500079 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:77c238ff37580c7dd07576778ab4a469bb8b538c9e3e9990a2d98c7326094ebd`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 26 Apr 2021 17:25:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 11 May 2021 23:58:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 May 2021 15:44:16 GMT
ENV NATS_DOCKERIZED=1
# Wed, 12 May 2021 20:11:37 GMT
ENV NATS_STREAMING_SERVER=0.21.2
# Wed, 12 May 2021 20:11:38 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.21.2/nats-streaming-server-v0.21.2-windows-amd64.zip
# Wed, 12 May 2021 20:11:39 GMT
ENV GIT_DOWNLOAD_SHA256=5d4367fea29116fcd70c364c8e808d6bc8e74214effbde83dd9548455bd06df2
# Wed, 12 May 2021 20:12:54 GMT
RUN Set-PSDebug -Trace 2
# Wed, 12 May 2021 20:15:02 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 12 May 2021 20:15:03 GMT
EXPOSE 4222 8222
# Wed, 12 May 2021 20:15:04 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 12 May 2021 20:15:05 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7f532f88613ca85064b055f6b93f8517bd05feba8fdce495a6ad1421573e765e`  
		Size: 1.7 GB (1725791397 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:50d0f4595a2bdc5dc0623fbee162be09d0631373eb9e82a0b1ec387ce1512c49`  
		Last Modified: Wed, 12 May 2021 00:46:32 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b7998d92dbbcfc4e6dc106e75206a3cfde70fe601eb46b0515658f23dcd53ae`  
		Last Modified: Wed, 12 May 2021 15:49:26 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f3010a7dd8667ca84982e9114e1dc65712c28bc68c365842b10a045ca612037`  
		Last Modified: Wed, 12 May 2021 20:16:28 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df06200a155b162a6be73cde9177db0ddf3ab1d3cfbd6cde1716508ea936e815`  
		Last Modified: Wed, 12 May 2021 20:16:28 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e23a0cd6171825cfd2bf6df17479e82e5845162d61bf74cf02daf44b78ba106`  
		Last Modified: Wed, 12 May 2021 20:16:28 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67048fb7884ce62e43c9c94e93c2469620bc4f1c31de0bfed360949a4856b32c`  
		Last Modified: Wed, 12 May 2021 20:16:32 GMT  
		Size: 5.7 MB (5699433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c112a8566705980bcc28d7b657abbc41bebdba6f14cc110792896e37a8ad36c0`  
		Last Modified: Wed, 12 May 2021 20:16:48 GMT  
		Size: 16.0 MB (16012020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a61d35a77f28396bd2da2e43c4fdf316968fa5dac4db17f07873ad8f2f778e54`  
		Last Modified: Wed, 12 May 2021 20:16:25 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96acafa52a9f3be44164c214903b7fffc48d9030807ce105a6c09093f4ebe1b9`  
		Last Modified: Wed, 12 May 2021 20:16:25 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b24723ae97946b0dbd5bf2b012548e33ca907518a500ca519e4bb0317bd31e0`  
		Last Modified: Wed, 12 May 2021 20:16:25 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:windowsservercore-1809`

```console
$ docker pull nats-streaming@sha256:ea4b6301b3365558fb705235d0e6ad5d6a3fcd989167e67831738db244d553b1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1935; amd64

### `nats-streaming:windowsservercore-1809` - windows version 10.0.17763.1935; amd64

```console
$ docker pull nats-streaming@sha256:df969179961089c2884fe95d19cab9088c89cf714b5169b76e8eaefa20d26550
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2490478060 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:87797a3af44c930235285b950723e7e38b9e69e8a60449c737a88b738c5c54e1`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 08 May 2021 09:21:48 GMT
RUN Install update 1809-amd64
# Tue, 11 May 2021 23:54:13 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 May 2021 15:41:49 GMT
ENV NATS_DOCKERIZED=1
# Wed, 12 May 2021 20:09:14 GMT
ENV NATS_STREAMING_SERVER=0.21.2
# Wed, 12 May 2021 20:09:14 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.21.2/nats-streaming-server-v0.21.2-windows-amd64.zip
# Wed, 12 May 2021 20:09:15 GMT
ENV GIT_DOWNLOAD_SHA256=5d4367fea29116fcd70c364c8e808d6bc8e74214effbde83dd9548455bd06df2
# Wed, 12 May 2021 20:09:48 GMT
RUN Set-PSDebug -Trace 2
# Wed, 12 May 2021 20:11:11 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 12 May 2021 20:11:12 GMT
EXPOSE 4222 8222
# Wed, 12 May 2021 20:11:13 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 12 May 2021 20:11:14 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8116de3c91c3f1ef2d6c09b49ef5407c9b4d672896eb3af5182a997c3c5379c9`  
		Size: 756.2 MB (756156286 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c049a65ed9206719f5c04428cb853623400e8ab1668243872b1134775f752962`  
		Last Modified: Wed, 12 May 2021 00:41:58 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:262d2305f11fe8f36ef3508b42686daac7e99da966ed02f4ded1927387b1b75b`  
		Last Modified: Wed, 12 May 2021 15:48:42 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caae5631f8d4c6cdfd8103d983810b9bfbefd01878285af9f623ac2f238f3449`  
		Last Modified: Wed, 12 May 2021 20:15:53 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d63f70b8ac38a77401cdba37ded79ef5a8565d1e0e5995c31b91f7aa4ce1b3f`  
		Last Modified: Wed, 12 May 2021 20:15:52 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0116c026836dea58f1432a034571efcf1d367ff5c6871c8f0930b7c9797602b2`  
		Last Modified: Wed, 12 May 2021 20:15:52 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7934c4e249cc275fd9d51173f09fbb985aa5c6d4314dce86d94108e3391b9bd5`  
		Last Modified: Wed, 12 May 2021 20:15:51 GMT  
		Size: 5.1 MB (5097038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:448f7480833686f3bbf6a3b41420f2f5add2aae1e35e31f4b47fe4b5e7fa441f`  
		Last Modified: Wed, 12 May 2021 20:15:53 GMT  
		Size: 10.9 MB (10880522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa234e132dde31816c466d94b40cac410cddcf081c522dbbabacbaca243f86a1`  
		Last Modified: Wed, 12 May 2021 20:15:50 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db175b165b9197d8d4b1751818e16f7c87846387f6d20a58ec01c885127fdf4d`  
		Last Modified: Wed, 12 May 2021 20:15:50 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38f8e2ba8c9a144f6620284f2697e8d0220903615e9c104d76fe384d4c5f3958`  
		Last Modified: Wed, 12 May 2021 20:15:49 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:windowsservercore-ltsc2016`

```console
$ docker pull nats-streaming@sha256:625ab75dea32121df296345016a44bcaa577d91d7c55b131fb28fd842ab65181
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4402; amd64

### `nats-streaming:windowsservercore-ltsc2016` - windows version 10.0.14393.4402; amd64

```console
$ docker pull nats-streaming@sha256:d15f6cc0f6f200c03c249c6fa30e1d993feabdba06c9bfb4dd25a41cb75dba02
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5817500079 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:77c238ff37580c7dd07576778ab4a469bb8b538c9e3e9990a2d98c7326094ebd`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 26 Apr 2021 17:25:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 11 May 2021 23:58:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 May 2021 15:44:16 GMT
ENV NATS_DOCKERIZED=1
# Wed, 12 May 2021 20:11:37 GMT
ENV NATS_STREAMING_SERVER=0.21.2
# Wed, 12 May 2021 20:11:38 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.21.2/nats-streaming-server-v0.21.2-windows-amd64.zip
# Wed, 12 May 2021 20:11:39 GMT
ENV GIT_DOWNLOAD_SHA256=5d4367fea29116fcd70c364c8e808d6bc8e74214effbde83dd9548455bd06df2
# Wed, 12 May 2021 20:12:54 GMT
RUN Set-PSDebug -Trace 2
# Wed, 12 May 2021 20:15:02 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 12 May 2021 20:15:03 GMT
EXPOSE 4222 8222
# Wed, 12 May 2021 20:15:04 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 12 May 2021 20:15:05 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7f532f88613ca85064b055f6b93f8517bd05feba8fdce495a6ad1421573e765e`  
		Size: 1.7 GB (1725791397 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:50d0f4595a2bdc5dc0623fbee162be09d0631373eb9e82a0b1ec387ce1512c49`  
		Last Modified: Wed, 12 May 2021 00:46:32 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b7998d92dbbcfc4e6dc106e75206a3cfde70fe601eb46b0515658f23dcd53ae`  
		Last Modified: Wed, 12 May 2021 15:49:26 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f3010a7dd8667ca84982e9114e1dc65712c28bc68c365842b10a045ca612037`  
		Last Modified: Wed, 12 May 2021 20:16:28 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df06200a155b162a6be73cde9177db0ddf3ab1d3cfbd6cde1716508ea936e815`  
		Last Modified: Wed, 12 May 2021 20:16:28 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e23a0cd6171825cfd2bf6df17479e82e5845162d61bf74cf02daf44b78ba106`  
		Last Modified: Wed, 12 May 2021 20:16:28 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67048fb7884ce62e43c9c94e93c2469620bc4f1c31de0bfed360949a4856b32c`  
		Last Modified: Wed, 12 May 2021 20:16:32 GMT  
		Size: 5.7 MB (5699433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c112a8566705980bcc28d7b657abbc41bebdba6f14cc110792896e37a8ad36c0`  
		Last Modified: Wed, 12 May 2021 20:16:48 GMT  
		Size: 16.0 MB (16012020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a61d35a77f28396bd2da2e43c4fdf316968fa5dac4db17f07873ad8f2f778e54`  
		Last Modified: Wed, 12 May 2021 20:16:25 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96acafa52a9f3be44164c214903b7fffc48d9030807ce105a6c09093f4ebe1b9`  
		Last Modified: Wed, 12 May 2021 20:16:25 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b24723ae97946b0dbd5bf2b012548e33ca907518a500ca519e4bb0317bd31e0`  
		Last Modified: Wed, 12 May 2021 20:16:25 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
