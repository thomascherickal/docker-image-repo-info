<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `nats-streaming`

-	[`nats-streaming:0.22`](#nats-streaming022)
-	[`nats-streaming:0.22-alpine`](#nats-streaming022-alpine)
-	[`nats-streaming:0.22-alpine3.14`](#nats-streaming022-alpine314)
-	[`nats-streaming:0.22-linux`](#nats-streaming022-linux)
-	[`nats-streaming:0.22-nanoserver`](#nats-streaming022-nanoserver)
-	[`nats-streaming:0.22-nanoserver-1809`](#nats-streaming022-nanoserver-1809)
-	[`nats-streaming:0.22-scratch`](#nats-streaming022-scratch)
-	[`nats-streaming:0.22-windowsservercore`](#nats-streaming022-windowsservercore)
-	[`nats-streaming:0.22-windowsservercore-1809`](#nats-streaming022-windowsservercore-1809)
-	[`nats-streaming:0.22-windowsservercore-ltsc2016`](#nats-streaming022-windowsservercore-ltsc2016)
-	[`nats-streaming:0.22.1`](#nats-streaming0221)
-	[`nats-streaming:0.22.1-alpine`](#nats-streaming0221-alpine)
-	[`nats-streaming:0.22.1-alpine3.14`](#nats-streaming0221-alpine314)
-	[`nats-streaming:0.22.1-linux`](#nats-streaming0221-linux)
-	[`nats-streaming:0.22.1-nanoserver`](#nats-streaming0221-nanoserver)
-	[`nats-streaming:0.22.1-nanoserver-1809`](#nats-streaming0221-nanoserver-1809)
-	[`nats-streaming:0.22.1-scratch`](#nats-streaming0221-scratch)
-	[`nats-streaming:0.22.1-windowsservercore`](#nats-streaming0221-windowsservercore)
-	[`nats-streaming:0.22.1-windowsservercore-1809`](#nats-streaming0221-windowsservercore-1809)
-	[`nats-streaming:0.22.1-windowsservercore-ltsc2016`](#nats-streaming0221-windowsservercore-ltsc2016)
-	[`nats-streaming:alpine`](#nats-streamingalpine)
-	[`nats-streaming:alpine3.14`](#nats-streamingalpine314)
-	[`nats-streaming:latest`](#nats-streaminglatest)
-	[`nats-streaming:linux`](#nats-streaminglinux)
-	[`nats-streaming:nanoserver`](#nats-streamingnanoserver)
-	[`nats-streaming:nanoserver-1809`](#nats-streamingnanoserver-1809)
-	[`nats-streaming:scratch`](#nats-streamingscratch)
-	[`nats-streaming:windowsservercore`](#nats-streamingwindowsservercore)
-	[`nats-streaming:windowsservercore-1809`](#nats-streamingwindowsservercore-1809)
-	[`nats-streaming:windowsservercore-ltsc2016`](#nats-streamingwindowsservercore-ltsc2016)

## `nats-streaming:0.22`

```console
$ docker pull nats-streaming@sha256:390339ceba1628352f455fe424fe32e247d88ee68536deacd17fef6c85426ef3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.2114; amd64

### `nats-streaming:0.22` - linux; amd64

```console
$ docker pull nats-streaming@sha256:3c6c9375f9e9724462e98cfb98a7abb50ceeca73b3070ce061992c4009e32157
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7168713 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:184d7920ac61dd2e84320b8040f57980a7d605d42948a520ede12d421168c4ce`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 02 Aug 2021 22:20:03 GMT
COPY file:ca9a212ccef327f9c2e91a62a908ac0cdbd39b08be331ea2b209c2d724942e18 in /nats-streaming-server 
# Mon, 02 Aug 2021 22:20:03 GMT
EXPOSE 4222 8222
# Mon, 02 Aug 2021 22:20:03 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 02 Aug 2021 22:20:03 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:f3749ab6cbfff03714b5a6a1245fa249b67d19e7358b74cbc50232b14370481a`  
		Last Modified: Mon, 02 Aug 2021 22:20:48 GMT  
		Size: 7.2 MB (7168713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.22` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:e944d0e843d59d5979d7561c06b0c0adc874ceaa0bd34d3a7b536b25e8c9704d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.7 MB (6650246 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0146bbca3802c65d86e148b1d203b3d395ca1cd8a8bb89461888570d821dc4fb`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 02 Aug 2021 22:51:34 GMT
COPY file:68ac67d86d6ac617adc181feb43580415b7fc7640a3c7577bb3753c369908da0 in /nats-streaming-server 
# Mon, 02 Aug 2021 22:51:35 GMT
EXPOSE 4222 8222
# Mon, 02 Aug 2021 22:51:35 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 02 Aug 2021 22:51:35 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:c7e1d707b6179f690f3f44212cb8c9a3fe914d91d3f1ddbac9f176aa0610c90a`  
		Last Modified: Mon, 02 Aug 2021 22:53:32 GMT  
		Size: 6.7 MB (6650246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.22` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:a5e3d56b343f9091f353634f59f688998544ccd4f2cbb80001d08ea6a3207274
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6639768 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80206ae32558812ad047d8ab67519615e98e7df68a884fc32b6d5fd8f72593b0`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 02 Aug 2021 23:11:17 GMT
COPY file:79708b5d249193a95e72c506453fd1ecd3e2738ec2ff3423c4b2bd760f426da2 in /nats-streaming-server 
# Mon, 02 Aug 2021 23:11:18 GMT
EXPOSE 4222 8222
# Mon, 02 Aug 2021 23:11:18 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 02 Aug 2021 23:11:19 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:52753762f751e166edd44e37a0ef0a06b33c337bdeb66e4134ee8479a49dae68`  
		Last Modified: Mon, 02 Aug 2021 23:13:17 GMT  
		Size: 6.6 MB (6639768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.22` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:96652223cce95275138363a54affb8663ba46bc75831c2a9535375ab6d922143
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 MB (6546324 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:952bbd74028df1debbfe0e4665b514c66a36537d0868d41bc971ddb55793c442`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 02 Aug 2021 22:40:16 GMT
COPY file:a77d9769f43cc6943be482183091d3360eaadf93bf1ef5a67f0869d5555868a6 in /nats-streaming-server 
# Mon, 02 Aug 2021 22:40:17 GMT
EXPOSE 4222 8222
# Mon, 02 Aug 2021 22:40:17 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 02 Aug 2021 22:40:17 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4dc8aa7843ed2da454d59006acb180caee3f980d12034caacd4a32ffedab3df7`  
		Last Modified: Mon, 02 Aug 2021 22:41:24 GMT  
		Size: 6.5 MB (6546324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.22` - windows version 10.0.17763.2114; amd64

```console
$ docker pull nats-streaming@sha256:8b058c3d2bf71043f26b6b58702562c13724bb5594ceebad3f49b4f539c3c227
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.0 MB (110039206 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:29bedda8d4d57688f52e1b97404c0dd1ecd0d7823e3f5e07a6f0214ee01d7853`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 05 Aug 2021 19:15:20 GMT
RUN Apply image 1809-amd64
# Wed, 11 Aug 2021 16:52:04 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 11 Aug 2021 21:19:29 GMT
RUN cmd /S /C #(nop) COPY file:9670e5d1fe5a71e47c78fde01235a0bcbcafcfdeeacf96a7669f6e49343fb03b in C:\nats-streaming-server.exe 
# Wed, 11 Aug 2021 21:19:33 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 11 Aug 2021 21:19:36 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 11 Aug 2021 21:19:39 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:bc8517709e9cfff223cb034ff5be8fcbfa5409de286cdac9ae1b8878ebea6b84`  
		Size: 102.7 MB (102741177 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3aa4a9dea1e2eabb29e2100fd699f3e3acbcabd85f360a3799b2505a5f74e5a0`  
		Last Modified: Wed, 11 Aug 2021 16:57:14 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2422c6b202cf35a718dc80ef76006199902c019414449d929f2538d72106be7`  
		Last Modified: Wed, 11 Aug 2021 21:24:43 GMT  
		Size: 7.3 MB (7293397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe1c9060adc003485accbb3848bb825c0b555a9e064d8ee4861937d781f4fb6d`  
		Last Modified: Wed, 11 Aug 2021 21:24:35 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eebb7419f921a924ca580e9c32580b82f2748e7759754b74686a3778fd920843`  
		Last Modified: Wed, 11 Aug 2021 21:24:35 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:413188a47dae1e13011a4e6d4ef5a31f5e680e350820d0b968981bc816827aaa`  
		Last Modified: Wed, 11 Aug 2021 21:24:35 GMT  
		Size: 1.2 KB (1174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.22-alpine`

```console
$ docker pull nats-streaming@sha256:e1479f281ad33982c8df81acee8d71d2049fe3535d7b1595adae6eeffd669c9e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.22-alpine` - linux; amd64

```console
$ docker pull nats-streaming@sha256:b13c3888f620e128e2324e521a59ecdae8096c67f4448233afd380feafbf565e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.3 MB (10269210 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e299437f282dcf86645a5f6e5b3a8c7345ba0e4582e60b8b76b5c06d1b5d938`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 06 Aug 2021 17:19:45 GMT
ADD file:34eb5c40aa00028921a224d1764ae1b1f3ef710d191e4dfc7df55e0594aa7217 in / 
# Fri, 06 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Sat, 07 Aug 2021 00:08:04 GMT
ENV NATS_STREAMING_SERVER=0.22.1
# Sat, 07 Aug 2021 00:08:07 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='581698d248a19ecae64e4048d153bc1021744a3da6284680a339f9f82a53a9cf' ;; 		armhf) natsArch='arm6'; sha256='438a89221bb0608e40d21e73ca27a4b70b8560730726942c0ade94a6b6013d6f' ;; 		armv7) natsArch='arm7'; sha256='4164baadd201d1374f7654d3e54a24d81ceb87a385867e31a82c1d1a69e3b1ae' ;; 		x86_64) natsArch='amd64'; sha256='f29e87ac9ff998c928aa8ebc8cf0c4d04d34a3d95b9900d92fd7dafab2bec8cc' ;; 		x86) natsArch='386'; sha256='0ca68e57babb8901d7afeb7569042730904887e718ddf860ef3ee54278753505' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Sat, 07 Aug 2021 00:08:08 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Sat, 07 Aug 2021 00:08:08 GMT
EXPOSE 4222 8222
# Sat, 07 Aug 2021 00:08:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 07 Aug 2021 00:08:08 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:29291e31a76a7e560b9b7ad3cada56e8c18d50a96cca8a2573e4f4689d7aca77`  
		Last Modified: Thu, 05 Aug 2021 15:56:25 GMT  
		Size: 2.8 MB (2813006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ded93adf1b7cd7e872edc8b55f1b6f392ee0f39c43a12ea019e39c39818d7f8f`  
		Last Modified: Sat, 07 Aug 2021 00:08:56 GMT  
		Size: 7.5 MB (7455782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:146382f94f105a2b20528c00beadcfd4783e1a1485e43b55b9bdd33fe1be714f`  
		Last Modified: Sat, 07 Aug 2021 00:08:54 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.22-alpine` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:a6cf6a518fea52b3fc47ed4572652aa0e2350898b54cdbcc0f778150de352dbd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.6 MB (9559904 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c8b625df6f0e93de9095159d166249a43a96ef9f3013e4a2c483b5ac7bc972b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 06 Aug 2021 17:49:32 GMT
ADD file:7f2c7deda009eabdcbbdccb11e854043d32c498e64e7e1ca02165d7bb4261d39 in / 
# Fri, 06 Aug 2021 17:49:32 GMT
CMD ["/bin/sh"]
# Fri, 06 Aug 2021 18:59:05 GMT
ENV NATS_STREAMING_SERVER=0.22.1
# Fri, 06 Aug 2021 18:59:10 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='581698d248a19ecae64e4048d153bc1021744a3da6284680a339f9f82a53a9cf' ;; 		armhf) natsArch='arm6'; sha256='438a89221bb0608e40d21e73ca27a4b70b8560730726942c0ade94a6b6013d6f' ;; 		armv7) natsArch='arm7'; sha256='4164baadd201d1374f7654d3e54a24d81ceb87a385867e31a82c1d1a69e3b1ae' ;; 		x86_64) natsArch='amd64'; sha256='f29e87ac9ff998c928aa8ebc8cf0c4d04d34a3d95b9900d92fd7dafab2bec8cc' ;; 		x86) natsArch='386'; sha256='0ca68e57babb8901d7afeb7569042730904887e718ddf860ef3ee54278753505' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 06 Aug 2021 18:59:10 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Fri, 06 Aug 2021 18:59:11 GMT
EXPOSE 4222 8222
# Fri, 06 Aug 2021 18:59:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 06 Aug 2021 18:59:12 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:f465bb3e9fcd0c42f936ecc566c6e40353c00f3089b2b2c2ea1663c30f89d3ab`  
		Last Modified: Fri, 06 Aug 2021 17:51:00 GMT  
		Size: 2.6 MB (2626350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:719cf2771983cbb32331cc8915e2edce30fbcb308f3504276742ffc9a3bc35fd`  
		Last Modified: Fri, 06 Aug 2021 19:00:56 GMT  
		Size: 6.9 MB (6933133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a72de2e4e74462365f574ec07048641b834163995d6b95fb88af2fca27e01883`  
		Last Modified: Fri, 06 Aug 2021 19:00:52 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.22-alpine` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:7970395d00490fad62f2a51288db47d251cab92ec7634bef6de42343f8e8eedc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.4 MB (9351328 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e19086c92b47964c105a8ed130ff7219833adab1ca8e211c1ad0b0a049866252`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 06 Aug 2021 17:57:32 GMT
ADD file:3a35ff3ac0d80289d419a4d6d8319610c38e1936d296addafb9aaf506946230f in / 
# Fri, 06 Aug 2021 17:57:32 GMT
CMD ["/bin/sh"]
# Fri, 06 Aug 2021 20:29:42 GMT
ENV NATS_STREAMING_SERVER=0.22.1
# Fri, 06 Aug 2021 20:29:48 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='581698d248a19ecae64e4048d153bc1021744a3da6284680a339f9f82a53a9cf' ;; 		armhf) natsArch='arm6'; sha256='438a89221bb0608e40d21e73ca27a4b70b8560730726942c0ade94a6b6013d6f' ;; 		armv7) natsArch='arm7'; sha256='4164baadd201d1374f7654d3e54a24d81ceb87a385867e31a82c1d1a69e3b1ae' ;; 		x86_64) natsArch='amd64'; sha256='f29e87ac9ff998c928aa8ebc8cf0c4d04d34a3d95b9900d92fd7dafab2bec8cc' ;; 		x86) natsArch='386'; sha256='0ca68e57babb8901d7afeb7569042730904887e718ddf860ef3ee54278753505' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 06 Aug 2021 20:29:48 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Fri, 06 Aug 2021 20:29:49 GMT
EXPOSE 4222 8222
# Fri, 06 Aug 2021 20:29:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 06 Aug 2021 20:29:50 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:4ee0caa23b369b04827640a4be298bf4ff7bacd030c77e915f5d7fb8f987594a`  
		Last Modified: Fri, 06 Aug 2021 17:58:57 GMT  
		Size: 2.4 MB (2429359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e14712e6c4fbdd823f35d0df7aa1345088ce3d89727133dcef4adb1105ecb5f`  
		Last Modified: Fri, 06 Aug 2021 20:31:34 GMT  
		Size: 6.9 MB (6921548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e18c45098374f86d0784e7840a2c0fd15ce636edfee6d3ebc23432fd0cc47be5`  
		Last Modified: Fri, 06 Aug 2021 20:31:30 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.22-alpine` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:c4818cc3ef0783732a51706c2f08756aad823d8829e0cd0a3e0332606b2a5851
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.5 MB (9541696 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c46cfd47aedfb2dfd2d6ede8515150bcce95d109f4180ab8d4ab95055cca9b62`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 06 Aug 2021 17:39:26 GMT
ADD file:1a8fd1066485e1261462e689c1a072f010c1d3be904b73ef2b84128fac652951 in / 
# Fri, 06 Aug 2021 17:39:27 GMT
CMD ["/bin/sh"]
# Fri, 06 Aug 2021 19:51:42 GMT
ENV NATS_STREAMING_SERVER=0.22.1
# Fri, 06 Aug 2021 19:51:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='581698d248a19ecae64e4048d153bc1021744a3da6284680a339f9f82a53a9cf' ;; 		armhf) natsArch='arm6'; sha256='438a89221bb0608e40d21e73ca27a4b70b8560730726942c0ade94a6b6013d6f' ;; 		armv7) natsArch='arm7'; sha256='4164baadd201d1374f7654d3e54a24d81ceb87a385867e31a82c1d1a69e3b1ae' ;; 		x86_64) natsArch='amd64'; sha256='f29e87ac9ff998c928aa8ebc8cf0c4d04d34a3d95b9900d92fd7dafab2bec8cc' ;; 		x86) natsArch='386'; sha256='0ca68e57babb8901d7afeb7569042730904887e718ddf860ef3ee54278753505' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 06 Aug 2021 19:51:45 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Fri, 06 Aug 2021 19:51:45 GMT
EXPOSE 4222 8222
# Fri, 06 Aug 2021 19:51:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 06 Aug 2021 19:51:45 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:fd3acdcea5682abced546ec19fb6ebee725c5184e5d91614c469c0a79e67f2d0`  
		Last Modified: Fri, 06 Aug 2021 17:40:12 GMT  
		Size: 2.7 MB (2710613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0968d8a9e4506d1c6878a0b725fc7f4f449c0ddb3f88d3704902e19db206317`  
		Last Modified: Fri, 06 Aug 2021 19:52:37 GMT  
		Size: 6.8 MB (6830662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87ab8fb5390b1c71a899984eb600e99e2ad1526c1c22bc89d0f8f52e64af17aa`  
		Last Modified: Fri, 06 Aug 2021 19:52:35 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.22-alpine3.14`

```console
$ docker pull nats-streaming@sha256:e1479f281ad33982c8df81acee8d71d2049fe3535d7b1595adae6eeffd669c9e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.22-alpine3.14` - linux; amd64

```console
$ docker pull nats-streaming@sha256:b13c3888f620e128e2324e521a59ecdae8096c67f4448233afd380feafbf565e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.3 MB (10269210 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e299437f282dcf86645a5f6e5b3a8c7345ba0e4582e60b8b76b5c06d1b5d938`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 06 Aug 2021 17:19:45 GMT
ADD file:34eb5c40aa00028921a224d1764ae1b1f3ef710d191e4dfc7df55e0594aa7217 in / 
# Fri, 06 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Sat, 07 Aug 2021 00:08:04 GMT
ENV NATS_STREAMING_SERVER=0.22.1
# Sat, 07 Aug 2021 00:08:07 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='581698d248a19ecae64e4048d153bc1021744a3da6284680a339f9f82a53a9cf' ;; 		armhf) natsArch='arm6'; sha256='438a89221bb0608e40d21e73ca27a4b70b8560730726942c0ade94a6b6013d6f' ;; 		armv7) natsArch='arm7'; sha256='4164baadd201d1374f7654d3e54a24d81ceb87a385867e31a82c1d1a69e3b1ae' ;; 		x86_64) natsArch='amd64'; sha256='f29e87ac9ff998c928aa8ebc8cf0c4d04d34a3d95b9900d92fd7dafab2bec8cc' ;; 		x86) natsArch='386'; sha256='0ca68e57babb8901d7afeb7569042730904887e718ddf860ef3ee54278753505' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Sat, 07 Aug 2021 00:08:08 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Sat, 07 Aug 2021 00:08:08 GMT
EXPOSE 4222 8222
# Sat, 07 Aug 2021 00:08:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 07 Aug 2021 00:08:08 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:29291e31a76a7e560b9b7ad3cada56e8c18d50a96cca8a2573e4f4689d7aca77`  
		Last Modified: Thu, 05 Aug 2021 15:56:25 GMT  
		Size: 2.8 MB (2813006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ded93adf1b7cd7e872edc8b55f1b6f392ee0f39c43a12ea019e39c39818d7f8f`  
		Last Modified: Sat, 07 Aug 2021 00:08:56 GMT  
		Size: 7.5 MB (7455782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:146382f94f105a2b20528c00beadcfd4783e1a1485e43b55b9bdd33fe1be714f`  
		Last Modified: Sat, 07 Aug 2021 00:08:54 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.22-alpine3.14` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:a6cf6a518fea52b3fc47ed4572652aa0e2350898b54cdbcc0f778150de352dbd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.6 MB (9559904 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c8b625df6f0e93de9095159d166249a43a96ef9f3013e4a2c483b5ac7bc972b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 06 Aug 2021 17:49:32 GMT
ADD file:7f2c7deda009eabdcbbdccb11e854043d32c498e64e7e1ca02165d7bb4261d39 in / 
# Fri, 06 Aug 2021 17:49:32 GMT
CMD ["/bin/sh"]
# Fri, 06 Aug 2021 18:59:05 GMT
ENV NATS_STREAMING_SERVER=0.22.1
# Fri, 06 Aug 2021 18:59:10 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='581698d248a19ecae64e4048d153bc1021744a3da6284680a339f9f82a53a9cf' ;; 		armhf) natsArch='arm6'; sha256='438a89221bb0608e40d21e73ca27a4b70b8560730726942c0ade94a6b6013d6f' ;; 		armv7) natsArch='arm7'; sha256='4164baadd201d1374f7654d3e54a24d81ceb87a385867e31a82c1d1a69e3b1ae' ;; 		x86_64) natsArch='amd64'; sha256='f29e87ac9ff998c928aa8ebc8cf0c4d04d34a3d95b9900d92fd7dafab2bec8cc' ;; 		x86) natsArch='386'; sha256='0ca68e57babb8901d7afeb7569042730904887e718ddf860ef3ee54278753505' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 06 Aug 2021 18:59:10 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Fri, 06 Aug 2021 18:59:11 GMT
EXPOSE 4222 8222
# Fri, 06 Aug 2021 18:59:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 06 Aug 2021 18:59:12 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:f465bb3e9fcd0c42f936ecc566c6e40353c00f3089b2b2c2ea1663c30f89d3ab`  
		Last Modified: Fri, 06 Aug 2021 17:51:00 GMT  
		Size: 2.6 MB (2626350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:719cf2771983cbb32331cc8915e2edce30fbcb308f3504276742ffc9a3bc35fd`  
		Last Modified: Fri, 06 Aug 2021 19:00:56 GMT  
		Size: 6.9 MB (6933133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a72de2e4e74462365f574ec07048641b834163995d6b95fb88af2fca27e01883`  
		Last Modified: Fri, 06 Aug 2021 19:00:52 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.22-alpine3.14` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:7970395d00490fad62f2a51288db47d251cab92ec7634bef6de42343f8e8eedc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.4 MB (9351328 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e19086c92b47964c105a8ed130ff7219833adab1ca8e211c1ad0b0a049866252`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 06 Aug 2021 17:57:32 GMT
ADD file:3a35ff3ac0d80289d419a4d6d8319610c38e1936d296addafb9aaf506946230f in / 
# Fri, 06 Aug 2021 17:57:32 GMT
CMD ["/bin/sh"]
# Fri, 06 Aug 2021 20:29:42 GMT
ENV NATS_STREAMING_SERVER=0.22.1
# Fri, 06 Aug 2021 20:29:48 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='581698d248a19ecae64e4048d153bc1021744a3da6284680a339f9f82a53a9cf' ;; 		armhf) natsArch='arm6'; sha256='438a89221bb0608e40d21e73ca27a4b70b8560730726942c0ade94a6b6013d6f' ;; 		armv7) natsArch='arm7'; sha256='4164baadd201d1374f7654d3e54a24d81ceb87a385867e31a82c1d1a69e3b1ae' ;; 		x86_64) natsArch='amd64'; sha256='f29e87ac9ff998c928aa8ebc8cf0c4d04d34a3d95b9900d92fd7dafab2bec8cc' ;; 		x86) natsArch='386'; sha256='0ca68e57babb8901d7afeb7569042730904887e718ddf860ef3ee54278753505' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 06 Aug 2021 20:29:48 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Fri, 06 Aug 2021 20:29:49 GMT
EXPOSE 4222 8222
# Fri, 06 Aug 2021 20:29:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 06 Aug 2021 20:29:50 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:4ee0caa23b369b04827640a4be298bf4ff7bacd030c77e915f5d7fb8f987594a`  
		Last Modified: Fri, 06 Aug 2021 17:58:57 GMT  
		Size: 2.4 MB (2429359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e14712e6c4fbdd823f35d0df7aa1345088ce3d89727133dcef4adb1105ecb5f`  
		Last Modified: Fri, 06 Aug 2021 20:31:34 GMT  
		Size: 6.9 MB (6921548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e18c45098374f86d0784e7840a2c0fd15ce636edfee6d3ebc23432fd0cc47be5`  
		Last Modified: Fri, 06 Aug 2021 20:31:30 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.22-alpine3.14` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:c4818cc3ef0783732a51706c2f08756aad823d8829e0cd0a3e0332606b2a5851
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.5 MB (9541696 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c46cfd47aedfb2dfd2d6ede8515150bcce95d109f4180ab8d4ab95055cca9b62`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 06 Aug 2021 17:39:26 GMT
ADD file:1a8fd1066485e1261462e689c1a072f010c1d3be904b73ef2b84128fac652951 in / 
# Fri, 06 Aug 2021 17:39:27 GMT
CMD ["/bin/sh"]
# Fri, 06 Aug 2021 19:51:42 GMT
ENV NATS_STREAMING_SERVER=0.22.1
# Fri, 06 Aug 2021 19:51:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='581698d248a19ecae64e4048d153bc1021744a3da6284680a339f9f82a53a9cf' ;; 		armhf) natsArch='arm6'; sha256='438a89221bb0608e40d21e73ca27a4b70b8560730726942c0ade94a6b6013d6f' ;; 		armv7) natsArch='arm7'; sha256='4164baadd201d1374f7654d3e54a24d81ceb87a385867e31a82c1d1a69e3b1ae' ;; 		x86_64) natsArch='amd64'; sha256='f29e87ac9ff998c928aa8ebc8cf0c4d04d34a3d95b9900d92fd7dafab2bec8cc' ;; 		x86) natsArch='386'; sha256='0ca68e57babb8901d7afeb7569042730904887e718ddf860ef3ee54278753505' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 06 Aug 2021 19:51:45 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Fri, 06 Aug 2021 19:51:45 GMT
EXPOSE 4222 8222
# Fri, 06 Aug 2021 19:51:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 06 Aug 2021 19:51:45 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:fd3acdcea5682abced546ec19fb6ebee725c5184e5d91614c469c0a79e67f2d0`  
		Last Modified: Fri, 06 Aug 2021 17:40:12 GMT  
		Size: 2.7 MB (2710613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0968d8a9e4506d1c6878a0b725fc7f4f449c0ddb3f88d3704902e19db206317`  
		Last Modified: Fri, 06 Aug 2021 19:52:37 GMT  
		Size: 6.8 MB (6830662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87ab8fb5390b1c71a899984eb600e99e2ad1526c1c22bc89d0f8f52e64af17aa`  
		Last Modified: Fri, 06 Aug 2021 19:52:35 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.22-linux`

```console
$ docker pull nats-streaming@sha256:7d3a953263095ea9d7018d32bd3483577d512550bc7890ba7743f48963cce893
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.22-linux` - linux; amd64

```console
$ docker pull nats-streaming@sha256:3c6c9375f9e9724462e98cfb98a7abb50ceeca73b3070ce061992c4009e32157
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7168713 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:184d7920ac61dd2e84320b8040f57980a7d605d42948a520ede12d421168c4ce`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 02 Aug 2021 22:20:03 GMT
COPY file:ca9a212ccef327f9c2e91a62a908ac0cdbd39b08be331ea2b209c2d724942e18 in /nats-streaming-server 
# Mon, 02 Aug 2021 22:20:03 GMT
EXPOSE 4222 8222
# Mon, 02 Aug 2021 22:20:03 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 02 Aug 2021 22:20:03 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:f3749ab6cbfff03714b5a6a1245fa249b67d19e7358b74cbc50232b14370481a`  
		Last Modified: Mon, 02 Aug 2021 22:20:48 GMT  
		Size: 7.2 MB (7168713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.22-linux` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:e944d0e843d59d5979d7561c06b0c0adc874ceaa0bd34d3a7b536b25e8c9704d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.7 MB (6650246 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0146bbca3802c65d86e148b1d203b3d395ca1cd8a8bb89461888570d821dc4fb`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 02 Aug 2021 22:51:34 GMT
COPY file:68ac67d86d6ac617adc181feb43580415b7fc7640a3c7577bb3753c369908da0 in /nats-streaming-server 
# Mon, 02 Aug 2021 22:51:35 GMT
EXPOSE 4222 8222
# Mon, 02 Aug 2021 22:51:35 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 02 Aug 2021 22:51:35 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:c7e1d707b6179f690f3f44212cb8c9a3fe914d91d3f1ddbac9f176aa0610c90a`  
		Last Modified: Mon, 02 Aug 2021 22:53:32 GMT  
		Size: 6.7 MB (6650246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.22-linux` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:a5e3d56b343f9091f353634f59f688998544ccd4f2cbb80001d08ea6a3207274
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6639768 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80206ae32558812ad047d8ab67519615e98e7df68a884fc32b6d5fd8f72593b0`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 02 Aug 2021 23:11:17 GMT
COPY file:79708b5d249193a95e72c506453fd1ecd3e2738ec2ff3423c4b2bd760f426da2 in /nats-streaming-server 
# Mon, 02 Aug 2021 23:11:18 GMT
EXPOSE 4222 8222
# Mon, 02 Aug 2021 23:11:18 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 02 Aug 2021 23:11:19 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:52753762f751e166edd44e37a0ef0a06b33c337bdeb66e4134ee8479a49dae68`  
		Last Modified: Mon, 02 Aug 2021 23:13:17 GMT  
		Size: 6.6 MB (6639768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.22-linux` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:96652223cce95275138363a54affb8663ba46bc75831c2a9535375ab6d922143
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 MB (6546324 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:952bbd74028df1debbfe0e4665b514c66a36537d0868d41bc971ddb55793c442`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 02 Aug 2021 22:40:16 GMT
COPY file:a77d9769f43cc6943be482183091d3360eaadf93bf1ef5a67f0869d5555868a6 in /nats-streaming-server 
# Mon, 02 Aug 2021 22:40:17 GMT
EXPOSE 4222 8222
# Mon, 02 Aug 2021 22:40:17 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 02 Aug 2021 22:40:17 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4dc8aa7843ed2da454d59006acb180caee3f980d12034caacd4a32ffedab3df7`  
		Last Modified: Mon, 02 Aug 2021 22:41:24 GMT  
		Size: 6.5 MB (6546324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.22-nanoserver`

```console
$ docker pull nats-streaming@sha256:8407af82564828d613edb1e65aedfa7d022699303898c4c33b02f71106e85700
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2114; amd64

### `nats-streaming:0.22-nanoserver` - windows version 10.0.17763.2114; amd64

```console
$ docker pull nats-streaming@sha256:8b058c3d2bf71043f26b6b58702562c13724bb5594ceebad3f49b4f539c3c227
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.0 MB (110039206 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:29bedda8d4d57688f52e1b97404c0dd1ecd0d7823e3f5e07a6f0214ee01d7853`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 05 Aug 2021 19:15:20 GMT
RUN Apply image 1809-amd64
# Wed, 11 Aug 2021 16:52:04 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 11 Aug 2021 21:19:29 GMT
RUN cmd /S /C #(nop) COPY file:9670e5d1fe5a71e47c78fde01235a0bcbcafcfdeeacf96a7669f6e49343fb03b in C:\nats-streaming-server.exe 
# Wed, 11 Aug 2021 21:19:33 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 11 Aug 2021 21:19:36 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 11 Aug 2021 21:19:39 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:bc8517709e9cfff223cb034ff5be8fcbfa5409de286cdac9ae1b8878ebea6b84`  
		Size: 102.7 MB (102741177 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3aa4a9dea1e2eabb29e2100fd699f3e3acbcabd85f360a3799b2505a5f74e5a0`  
		Last Modified: Wed, 11 Aug 2021 16:57:14 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2422c6b202cf35a718dc80ef76006199902c019414449d929f2538d72106be7`  
		Last Modified: Wed, 11 Aug 2021 21:24:43 GMT  
		Size: 7.3 MB (7293397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe1c9060adc003485accbb3848bb825c0b555a9e064d8ee4861937d781f4fb6d`  
		Last Modified: Wed, 11 Aug 2021 21:24:35 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eebb7419f921a924ca580e9c32580b82f2748e7759754b74686a3778fd920843`  
		Last Modified: Wed, 11 Aug 2021 21:24:35 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:413188a47dae1e13011a4e6d4ef5a31f5e680e350820d0b968981bc816827aaa`  
		Last Modified: Wed, 11 Aug 2021 21:24:35 GMT  
		Size: 1.2 KB (1174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.22-nanoserver-1809`

```console
$ docker pull nats-streaming@sha256:8407af82564828d613edb1e65aedfa7d022699303898c4c33b02f71106e85700
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2114; amd64

### `nats-streaming:0.22-nanoserver-1809` - windows version 10.0.17763.2114; amd64

```console
$ docker pull nats-streaming@sha256:8b058c3d2bf71043f26b6b58702562c13724bb5594ceebad3f49b4f539c3c227
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.0 MB (110039206 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:29bedda8d4d57688f52e1b97404c0dd1ecd0d7823e3f5e07a6f0214ee01d7853`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 05 Aug 2021 19:15:20 GMT
RUN Apply image 1809-amd64
# Wed, 11 Aug 2021 16:52:04 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 11 Aug 2021 21:19:29 GMT
RUN cmd /S /C #(nop) COPY file:9670e5d1fe5a71e47c78fde01235a0bcbcafcfdeeacf96a7669f6e49343fb03b in C:\nats-streaming-server.exe 
# Wed, 11 Aug 2021 21:19:33 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 11 Aug 2021 21:19:36 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 11 Aug 2021 21:19:39 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:bc8517709e9cfff223cb034ff5be8fcbfa5409de286cdac9ae1b8878ebea6b84`  
		Size: 102.7 MB (102741177 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3aa4a9dea1e2eabb29e2100fd699f3e3acbcabd85f360a3799b2505a5f74e5a0`  
		Last Modified: Wed, 11 Aug 2021 16:57:14 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2422c6b202cf35a718dc80ef76006199902c019414449d929f2538d72106be7`  
		Last Modified: Wed, 11 Aug 2021 21:24:43 GMT  
		Size: 7.3 MB (7293397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe1c9060adc003485accbb3848bb825c0b555a9e064d8ee4861937d781f4fb6d`  
		Last Modified: Wed, 11 Aug 2021 21:24:35 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eebb7419f921a924ca580e9c32580b82f2748e7759754b74686a3778fd920843`  
		Last Modified: Wed, 11 Aug 2021 21:24:35 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:413188a47dae1e13011a4e6d4ef5a31f5e680e350820d0b968981bc816827aaa`  
		Last Modified: Wed, 11 Aug 2021 21:24:35 GMT  
		Size: 1.2 KB (1174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.22-scratch`

```console
$ docker pull nats-streaming@sha256:7d3a953263095ea9d7018d32bd3483577d512550bc7890ba7743f48963cce893
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.22-scratch` - linux; amd64

```console
$ docker pull nats-streaming@sha256:3c6c9375f9e9724462e98cfb98a7abb50ceeca73b3070ce061992c4009e32157
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7168713 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:184d7920ac61dd2e84320b8040f57980a7d605d42948a520ede12d421168c4ce`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 02 Aug 2021 22:20:03 GMT
COPY file:ca9a212ccef327f9c2e91a62a908ac0cdbd39b08be331ea2b209c2d724942e18 in /nats-streaming-server 
# Mon, 02 Aug 2021 22:20:03 GMT
EXPOSE 4222 8222
# Mon, 02 Aug 2021 22:20:03 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 02 Aug 2021 22:20:03 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:f3749ab6cbfff03714b5a6a1245fa249b67d19e7358b74cbc50232b14370481a`  
		Last Modified: Mon, 02 Aug 2021 22:20:48 GMT  
		Size: 7.2 MB (7168713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.22-scratch` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:e944d0e843d59d5979d7561c06b0c0adc874ceaa0bd34d3a7b536b25e8c9704d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.7 MB (6650246 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0146bbca3802c65d86e148b1d203b3d395ca1cd8a8bb89461888570d821dc4fb`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 02 Aug 2021 22:51:34 GMT
COPY file:68ac67d86d6ac617adc181feb43580415b7fc7640a3c7577bb3753c369908da0 in /nats-streaming-server 
# Mon, 02 Aug 2021 22:51:35 GMT
EXPOSE 4222 8222
# Mon, 02 Aug 2021 22:51:35 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 02 Aug 2021 22:51:35 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:c7e1d707b6179f690f3f44212cb8c9a3fe914d91d3f1ddbac9f176aa0610c90a`  
		Last Modified: Mon, 02 Aug 2021 22:53:32 GMT  
		Size: 6.7 MB (6650246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.22-scratch` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:a5e3d56b343f9091f353634f59f688998544ccd4f2cbb80001d08ea6a3207274
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6639768 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80206ae32558812ad047d8ab67519615e98e7df68a884fc32b6d5fd8f72593b0`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 02 Aug 2021 23:11:17 GMT
COPY file:79708b5d249193a95e72c506453fd1ecd3e2738ec2ff3423c4b2bd760f426da2 in /nats-streaming-server 
# Mon, 02 Aug 2021 23:11:18 GMT
EXPOSE 4222 8222
# Mon, 02 Aug 2021 23:11:18 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 02 Aug 2021 23:11:19 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:52753762f751e166edd44e37a0ef0a06b33c337bdeb66e4134ee8479a49dae68`  
		Last Modified: Mon, 02 Aug 2021 23:13:17 GMT  
		Size: 6.6 MB (6639768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.22-scratch` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:96652223cce95275138363a54affb8663ba46bc75831c2a9535375ab6d922143
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 MB (6546324 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:952bbd74028df1debbfe0e4665b514c66a36537d0868d41bc971ddb55793c442`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 02 Aug 2021 22:40:16 GMT
COPY file:a77d9769f43cc6943be482183091d3360eaadf93bf1ef5a67f0869d5555868a6 in /nats-streaming-server 
# Mon, 02 Aug 2021 22:40:17 GMT
EXPOSE 4222 8222
# Mon, 02 Aug 2021 22:40:17 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 02 Aug 2021 22:40:17 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4dc8aa7843ed2da454d59006acb180caee3f980d12034caacd4a32ffedab3df7`  
		Last Modified: Mon, 02 Aug 2021 22:41:24 GMT  
		Size: 6.5 MB (6546324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.22-windowsservercore`

```console
$ docker pull nats-streaming@sha256:5f9e88c929ff89c3204d105008a059f9be67f540ff96b5bfec99e3b254351411
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.2114; amd64
	-	windows version 10.0.14393.4583; amd64

### `nats-streaming:0.22-windowsservercore` - windows version 10.0.17763.2114; amd64

```console
$ docker pull nats-streaming@sha256:75b04016fe1b2f4c6a7bef238c62f6610c86ab0baed8d1031b7f061053987a27
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2693987543 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ffc0c1be51519eff598c2d5cce32f011fcfe27c06a9651541cec6796f3f66a56`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 05 Aug 2021 19:44:34 GMT
RUN Install update 1809-amd64
# Wed, 11 Aug 2021 13:42:12 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 11 Aug 2021 16:48:51 GMT
ENV NATS_DOCKERIZED=1
# Wed, 11 Aug 2021 21:16:00 GMT
ENV NATS_STREAMING_SERVER=0.22.1
# Wed, 11 Aug 2021 21:16:03 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.22.1/nats-streaming-server-v0.22.1-windows-amd64.zip
# Wed, 11 Aug 2021 21:16:06 GMT
ENV NATS_STREAMING_SERVER_SHASUM=4516852b493111b73ec06477be4a27e66f5abc9ca1ff4dd2b970232271611264
# Wed, 11 Aug 2021 21:17:09 GMT
RUN Set-PSDebug -Trace 2
# Wed, 11 Aug 2021 21:19:07 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 11 Aug 2021 21:19:10 GMT
EXPOSE 4222 8222
# Wed, 11 Aug 2021 21:19:13 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 11 Aug 2021 21:19:15 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c67ded6868b61d392a0c096f911563fd6bc0bc3ed4fe401d077b3718a1b0cdaf`  
		Size: 967.7 MB (967665054 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c613f4c34660a122de754415a884afe6b12172ac3ce792a2e4aae831cc8b2e27`  
		Last Modified: Wed, 11 Aug 2021 16:25:11 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71d8e65d39d1b09c34e0dadad1a6b7818f430fb13ce2ff8d70c549b137f9131a`  
		Last Modified: Wed, 11 Aug 2021 16:56:54 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f48fea2e101940ffa36628a8fd4da200aa97417773d993be6df74d0bcff8dccc`  
		Last Modified: Wed, 11 Aug 2021 21:24:22 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bd10110cd94f48fce072addebc384215cfee9e902098952b29a44227fc4c19b`  
		Last Modified: Wed, 11 Aug 2021 21:24:22 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f32d77caa28f59168738bee8473e7e58d117ce711f59589f9627b0facfe620bd`  
		Last Modified: Wed, 11 Aug 2021 21:24:22 GMT  
		Size: 1.4 KB (1443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90f9d42ecbcdc48ff53122318c96640c628d9f2b33df84c887b89a1b1429091e`  
		Last Modified: Wed, 11 Aug 2021 21:24:19 GMT  
		Size: 351.7 KB (351714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfe2bf098cd0e80bd3e81951fb0f411238d63d458bcd51ecd3427a1566fd0ffc`  
		Last Modified: Wed, 11 Aug 2021 21:24:21 GMT  
		Size: 7.6 MB (7626528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e710a2acda7795374f6c855a7d81c6156b961c06f5b0f13fd31e2d8c4952fd6`  
		Last Modified: Wed, 11 Aug 2021 21:24:19 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2333773eafb1bb6c7fd6fd55fd31614ec447f3b1af48b5f63fe1ee29a4093ff2`  
		Last Modified: Wed, 11 Aug 2021 21:24:19 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:666623a49ff4c5032408abc00ae56261476eed8930351412760fedada9e6e136`  
		Last Modified: Wed, 11 Aug 2021 21:24:19 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.22-windowsservercore` - windows version 10.0.14393.4583; amd64

```console
$ docker pull nats-streaming@sha256:c2dc8bad14a0594eb6483398e8aa5f20933884855abece46d39a9aaa5ff6c0de
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6283441295 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d4dcfbb00a058925aa22ae213359605c8892f3261a0afdd6941153ff9789f841`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Sun, 01 Aug 2021 08:52:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 11 Aug 2021 13:57:45 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 11 Aug 2021 16:52:27 GMT
ENV NATS_DOCKERIZED=1
# Wed, 11 Aug 2021 21:19:47 GMT
ENV NATS_STREAMING_SERVER=0.22.1
# Wed, 11 Aug 2021 21:19:50 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.22.1/nats-streaming-server-v0.22.1-windows-amd64.zip
# Wed, 11 Aug 2021 21:19:53 GMT
ENV NATS_STREAMING_SERVER_SHASUM=4516852b493111b73ec06477be4a27e66f5abc9ca1ff4dd2b970232271611264
# Wed, 11 Aug 2021 21:21:16 GMT
RUN Set-PSDebug -Trace 2
# Wed, 11 Aug 2021 21:23:38 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 11 Aug 2021 21:23:41 GMT
EXPOSE 4222 8222
# Wed, 11 Aug 2021 21:23:43 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 11 Aug 2021 21:23:46 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c427f892fe74603ae09d4e49b25f8f7046f957054034dc9f462e0e88d7bffaa5`  
		Size: 2.2 GB (2200980134 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d6d4b60a6f3b0544427c2eb9a5e27e5f6ddca0fd7632003e11331f01c4e9c6fc`  
		Last Modified: Wed, 11 Aug 2021 16:25:34 GMT  
		Size: 1.4 KB (1442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe49d3a206649779952cc6a03fdbb4e828336501708ad40c4e1a07237199e28b`  
		Last Modified: Wed, 11 Aug 2021 16:57:38 GMT  
		Size: 1.4 KB (1380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e6e2dfe14e85c8398dc3f7c7906fb1f7c777ef6d5717fe70d978ad05718ffc2`  
		Last Modified: Wed, 11 Aug 2021 21:24:59 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f846ec4e42dc3dac55d428bcb2d57cab68f2b659b2cdbba1cad2800b22496145`  
		Last Modified: Wed, 11 Aug 2021 21:24:59 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a073e823edff403699ab0d2dff8376e1b0fb57af79842af3133c0b0c0e3c77f0`  
		Last Modified: Wed, 11 Aug 2021 21:24:59 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bedf8cee66f4f7e59aee0a000c7fe523b2994d8d7f358c994942fb8b6a9ae6c`  
		Last Modified: Wed, 11 Aug 2021 21:24:57 GMT  
		Size: 338.6 KB (338573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:275d8c5f6fbce1b85b62d1f70554f8ecf9d3ccdbfe54c86356703cc697b71e2b`  
		Last Modified: Wed, 11 Aug 2021 21:24:59 GMT  
		Size: 12.1 MB (12125382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b86e3ac00ba61bf48479b43167f3550a6c8ed7af7da7dd5c0b86441e7d8f662`  
		Last Modified: Wed, 11 Aug 2021 21:24:56 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f45154e30184ba145c5239532f29c91a714e1e6be10588ab43f2dfc69986775e`  
		Last Modified: Wed, 11 Aug 2021 21:24:56 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:254423fab1337576ad61d5fdd3942f86d494a694b38f8c0f779f9239789684b3`  
		Last Modified: Wed, 11 Aug 2021 21:24:56 GMT  
		Size: 1.4 KB (1443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.22-windowsservercore-1809`

```console
$ docker pull nats-streaming@sha256:17e69850495ccb3a8a86278c37ad940698ed0da3f3c08f6de694456dbb989c25
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2114; amd64

### `nats-streaming:0.22-windowsservercore-1809` - windows version 10.0.17763.2114; amd64

```console
$ docker pull nats-streaming@sha256:75b04016fe1b2f4c6a7bef238c62f6610c86ab0baed8d1031b7f061053987a27
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2693987543 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ffc0c1be51519eff598c2d5cce32f011fcfe27c06a9651541cec6796f3f66a56`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 05 Aug 2021 19:44:34 GMT
RUN Install update 1809-amd64
# Wed, 11 Aug 2021 13:42:12 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 11 Aug 2021 16:48:51 GMT
ENV NATS_DOCKERIZED=1
# Wed, 11 Aug 2021 21:16:00 GMT
ENV NATS_STREAMING_SERVER=0.22.1
# Wed, 11 Aug 2021 21:16:03 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.22.1/nats-streaming-server-v0.22.1-windows-amd64.zip
# Wed, 11 Aug 2021 21:16:06 GMT
ENV NATS_STREAMING_SERVER_SHASUM=4516852b493111b73ec06477be4a27e66f5abc9ca1ff4dd2b970232271611264
# Wed, 11 Aug 2021 21:17:09 GMT
RUN Set-PSDebug -Trace 2
# Wed, 11 Aug 2021 21:19:07 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 11 Aug 2021 21:19:10 GMT
EXPOSE 4222 8222
# Wed, 11 Aug 2021 21:19:13 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 11 Aug 2021 21:19:15 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c67ded6868b61d392a0c096f911563fd6bc0bc3ed4fe401d077b3718a1b0cdaf`  
		Size: 967.7 MB (967665054 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c613f4c34660a122de754415a884afe6b12172ac3ce792a2e4aae831cc8b2e27`  
		Last Modified: Wed, 11 Aug 2021 16:25:11 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71d8e65d39d1b09c34e0dadad1a6b7818f430fb13ce2ff8d70c549b137f9131a`  
		Last Modified: Wed, 11 Aug 2021 16:56:54 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f48fea2e101940ffa36628a8fd4da200aa97417773d993be6df74d0bcff8dccc`  
		Last Modified: Wed, 11 Aug 2021 21:24:22 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bd10110cd94f48fce072addebc384215cfee9e902098952b29a44227fc4c19b`  
		Last Modified: Wed, 11 Aug 2021 21:24:22 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f32d77caa28f59168738bee8473e7e58d117ce711f59589f9627b0facfe620bd`  
		Last Modified: Wed, 11 Aug 2021 21:24:22 GMT  
		Size: 1.4 KB (1443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90f9d42ecbcdc48ff53122318c96640c628d9f2b33df84c887b89a1b1429091e`  
		Last Modified: Wed, 11 Aug 2021 21:24:19 GMT  
		Size: 351.7 KB (351714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfe2bf098cd0e80bd3e81951fb0f411238d63d458bcd51ecd3427a1566fd0ffc`  
		Last Modified: Wed, 11 Aug 2021 21:24:21 GMT  
		Size: 7.6 MB (7626528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e710a2acda7795374f6c855a7d81c6156b961c06f5b0f13fd31e2d8c4952fd6`  
		Last Modified: Wed, 11 Aug 2021 21:24:19 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2333773eafb1bb6c7fd6fd55fd31614ec447f3b1af48b5f63fe1ee29a4093ff2`  
		Last Modified: Wed, 11 Aug 2021 21:24:19 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:666623a49ff4c5032408abc00ae56261476eed8930351412760fedada9e6e136`  
		Last Modified: Wed, 11 Aug 2021 21:24:19 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.22-windowsservercore-ltsc2016`

```console
$ docker pull nats-streaming@sha256:9cfea454a5d6b43341f213ae8515bf3ccf36487967fc16fad686bd3bed667681
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.14393.4583; amd64

### `nats-streaming:0.22-windowsservercore-ltsc2016` - windows version 10.0.14393.4583; amd64

```console
$ docker pull nats-streaming@sha256:c2dc8bad14a0594eb6483398e8aa5f20933884855abece46d39a9aaa5ff6c0de
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6283441295 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d4dcfbb00a058925aa22ae213359605c8892f3261a0afdd6941153ff9789f841`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Sun, 01 Aug 2021 08:52:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 11 Aug 2021 13:57:45 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 11 Aug 2021 16:52:27 GMT
ENV NATS_DOCKERIZED=1
# Wed, 11 Aug 2021 21:19:47 GMT
ENV NATS_STREAMING_SERVER=0.22.1
# Wed, 11 Aug 2021 21:19:50 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.22.1/nats-streaming-server-v0.22.1-windows-amd64.zip
# Wed, 11 Aug 2021 21:19:53 GMT
ENV NATS_STREAMING_SERVER_SHASUM=4516852b493111b73ec06477be4a27e66f5abc9ca1ff4dd2b970232271611264
# Wed, 11 Aug 2021 21:21:16 GMT
RUN Set-PSDebug -Trace 2
# Wed, 11 Aug 2021 21:23:38 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 11 Aug 2021 21:23:41 GMT
EXPOSE 4222 8222
# Wed, 11 Aug 2021 21:23:43 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 11 Aug 2021 21:23:46 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c427f892fe74603ae09d4e49b25f8f7046f957054034dc9f462e0e88d7bffaa5`  
		Size: 2.2 GB (2200980134 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d6d4b60a6f3b0544427c2eb9a5e27e5f6ddca0fd7632003e11331f01c4e9c6fc`  
		Last Modified: Wed, 11 Aug 2021 16:25:34 GMT  
		Size: 1.4 KB (1442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe49d3a206649779952cc6a03fdbb4e828336501708ad40c4e1a07237199e28b`  
		Last Modified: Wed, 11 Aug 2021 16:57:38 GMT  
		Size: 1.4 KB (1380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e6e2dfe14e85c8398dc3f7c7906fb1f7c777ef6d5717fe70d978ad05718ffc2`  
		Last Modified: Wed, 11 Aug 2021 21:24:59 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f846ec4e42dc3dac55d428bcb2d57cab68f2b659b2cdbba1cad2800b22496145`  
		Last Modified: Wed, 11 Aug 2021 21:24:59 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a073e823edff403699ab0d2dff8376e1b0fb57af79842af3133c0b0c0e3c77f0`  
		Last Modified: Wed, 11 Aug 2021 21:24:59 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bedf8cee66f4f7e59aee0a000c7fe523b2994d8d7f358c994942fb8b6a9ae6c`  
		Last Modified: Wed, 11 Aug 2021 21:24:57 GMT  
		Size: 338.6 KB (338573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:275d8c5f6fbce1b85b62d1f70554f8ecf9d3ccdbfe54c86356703cc697b71e2b`  
		Last Modified: Wed, 11 Aug 2021 21:24:59 GMT  
		Size: 12.1 MB (12125382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b86e3ac00ba61bf48479b43167f3550a6c8ed7af7da7dd5c0b86441e7d8f662`  
		Last Modified: Wed, 11 Aug 2021 21:24:56 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f45154e30184ba145c5239532f29c91a714e1e6be10588ab43f2dfc69986775e`  
		Last Modified: Wed, 11 Aug 2021 21:24:56 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:254423fab1337576ad61d5fdd3942f86d494a694b38f8c0f779f9239789684b3`  
		Last Modified: Wed, 11 Aug 2021 21:24:56 GMT  
		Size: 1.4 KB (1443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.22.1`

```console
$ docker pull nats-streaming@sha256:390339ceba1628352f455fe424fe32e247d88ee68536deacd17fef6c85426ef3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.2114; amd64

### `nats-streaming:0.22.1` - linux; amd64

```console
$ docker pull nats-streaming@sha256:3c6c9375f9e9724462e98cfb98a7abb50ceeca73b3070ce061992c4009e32157
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7168713 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:184d7920ac61dd2e84320b8040f57980a7d605d42948a520ede12d421168c4ce`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 02 Aug 2021 22:20:03 GMT
COPY file:ca9a212ccef327f9c2e91a62a908ac0cdbd39b08be331ea2b209c2d724942e18 in /nats-streaming-server 
# Mon, 02 Aug 2021 22:20:03 GMT
EXPOSE 4222 8222
# Mon, 02 Aug 2021 22:20:03 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 02 Aug 2021 22:20:03 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:f3749ab6cbfff03714b5a6a1245fa249b67d19e7358b74cbc50232b14370481a`  
		Last Modified: Mon, 02 Aug 2021 22:20:48 GMT  
		Size: 7.2 MB (7168713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.22.1` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:e944d0e843d59d5979d7561c06b0c0adc874ceaa0bd34d3a7b536b25e8c9704d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.7 MB (6650246 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0146bbca3802c65d86e148b1d203b3d395ca1cd8a8bb89461888570d821dc4fb`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 02 Aug 2021 22:51:34 GMT
COPY file:68ac67d86d6ac617adc181feb43580415b7fc7640a3c7577bb3753c369908da0 in /nats-streaming-server 
# Mon, 02 Aug 2021 22:51:35 GMT
EXPOSE 4222 8222
# Mon, 02 Aug 2021 22:51:35 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 02 Aug 2021 22:51:35 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:c7e1d707b6179f690f3f44212cb8c9a3fe914d91d3f1ddbac9f176aa0610c90a`  
		Last Modified: Mon, 02 Aug 2021 22:53:32 GMT  
		Size: 6.7 MB (6650246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.22.1` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:a5e3d56b343f9091f353634f59f688998544ccd4f2cbb80001d08ea6a3207274
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6639768 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80206ae32558812ad047d8ab67519615e98e7df68a884fc32b6d5fd8f72593b0`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 02 Aug 2021 23:11:17 GMT
COPY file:79708b5d249193a95e72c506453fd1ecd3e2738ec2ff3423c4b2bd760f426da2 in /nats-streaming-server 
# Mon, 02 Aug 2021 23:11:18 GMT
EXPOSE 4222 8222
# Mon, 02 Aug 2021 23:11:18 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 02 Aug 2021 23:11:19 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:52753762f751e166edd44e37a0ef0a06b33c337bdeb66e4134ee8479a49dae68`  
		Last Modified: Mon, 02 Aug 2021 23:13:17 GMT  
		Size: 6.6 MB (6639768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.22.1` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:96652223cce95275138363a54affb8663ba46bc75831c2a9535375ab6d922143
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 MB (6546324 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:952bbd74028df1debbfe0e4665b514c66a36537d0868d41bc971ddb55793c442`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 02 Aug 2021 22:40:16 GMT
COPY file:a77d9769f43cc6943be482183091d3360eaadf93bf1ef5a67f0869d5555868a6 in /nats-streaming-server 
# Mon, 02 Aug 2021 22:40:17 GMT
EXPOSE 4222 8222
# Mon, 02 Aug 2021 22:40:17 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 02 Aug 2021 22:40:17 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4dc8aa7843ed2da454d59006acb180caee3f980d12034caacd4a32ffedab3df7`  
		Last Modified: Mon, 02 Aug 2021 22:41:24 GMT  
		Size: 6.5 MB (6546324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.22.1` - windows version 10.0.17763.2114; amd64

```console
$ docker pull nats-streaming@sha256:8b058c3d2bf71043f26b6b58702562c13724bb5594ceebad3f49b4f539c3c227
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.0 MB (110039206 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:29bedda8d4d57688f52e1b97404c0dd1ecd0d7823e3f5e07a6f0214ee01d7853`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 05 Aug 2021 19:15:20 GMT
RUN Apply image 1809-amd64
# Wed, 11 Aug 2021 16:52:04 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 11 Aug 2021 21:19:29 GMT
RUN cmd /S /C #(nop) COPY file:9670e5d1fe5a71e47c78fde01235a0bcbcafcfdeeacf96a7669f6e49343fb03b in C:\nats-streaming-server.exe 
# Wed, 11 Aug 2021 21:19:33 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 11 Aug 2021 21:19:36 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 11 Aug 2021 21:19:39 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:bc8517709e9cfff223cb034ff5be8fcbfa5409de286cdac9ae1b8878ebea6b84`  
		Size: 102.7 MB (102741177 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3aa4a9dea1e2eabb29e2100fd699f3e3acbcabd85f360a3799b2505a5f74e5a0`  
		Last Modified: Wed, 11 Aug 2021 16:57:14 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2422c6b202cf35a718dc80ef76006199902c019414449d929f2538d72106be7`  
		Last Modified: Wed, 11 Aug 2021 21:24:43 GMT  
		Size: 7.3 MB (7293397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe1c9060adc003485accbb3848bb825c0b555a9e064d8ee4861937d781f4fb6d`  
		Last Modified: Wed, 11 Aug 2021 21:24:35 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eebb7419f921a924ca580e9c32580b82f2748e7759754b74686a3778fd920843`  
		Last Modified: Wed, 11 Aug 2021 21:24:35 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:413188a47dae1e13011a4e6d4ef5a31f5e680e350820d0b968981bc816827aaa`  
		Last Modified: Wed, 11 Aug 2021 21:24:35 GMT  
		Size: 1.2 KB (1174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.22.1-alpine`

```console
$ docker pull nats-streaming@sha256:e1479f281ad33982c8df81acee8d71d2049fe3535d7b1595adae6eeffd669c9e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.22.1-alpine` - linux; amd64

```console
$ docker pull nats-streaming@sha256:b13c3888f620e128e2324e521a59ecdae8096c67f4448233afd380feafbf565e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.3 MB (10269210 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e299437f282dcf86645a5f6e5b3a8c7345ba0e4582e60b8b76b5c06d1b5d938`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 06 Aug 2021 17:19:45 GMT
ADD file:34eb5c40aa00028921a224d1764ae1b1f3ef710d191e4dfc7df55e0594aa7217 in / 
# Fri, 06 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Sat, 07 Aug 2021 00:08:04 GMT
ENV NATS_STREAMING_SERVER=0.22.1
# Sat, 07 Aug 2021 00:08:07 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='581698d248a19ecae64e4048d153bc1021744a3da6284680a339f9f82a53a9cf' ;; 		armhf) natsArch='arm6'; sha256='438a89221bb0608e40d21e73ca27a4b70b8560730726942c0ade94a6b6013d6f' ;; 		armv7) natsArch='arm7'; sha256='4164baadd201d1374f7654d3e54a24d81ceb87a385867e31a82c1d1a69e3b1ae' ;; 		x86_64) natsArch='amd64'; sha256='f29e87ac9ff998c928aa8ebc8cf0c4d04d34a3d95b9900d92fd7dafab2bec8cc' ;; 		x86) natsArch='386'; sha256='0ca68e57babb8901d7afeb7569042730904887e718ddf860ef3ee54278753505' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Sat, 07 Aug 2021 00:08:08 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Sat, 07 Aug 2021 00:08:08 GMT
EXPOSE 4222 8222
# Sat, 07 Aug 2021 00:08:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 07 Aug 2021 00:08:08 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:29291e31a76a7e560b9b7ad3cada56e8c18d50a96cca8a2573e4f4689d7aca77`  
		Last Modified: Thu, 05 Aug 2021 15:56:25 GMT  
		Size: 2.8 MB (2813006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ded93adf1b7cd7e872edc8b55f1b6f392ee0f39c43a12ea019e39c39818d7f8f`  
		Last Modified: Sat, 07 Aug 2021 00:08:56 GMT  
		Size: 7.5 MB (7455782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:146382f94f105a2b20528c00beadcfd4783e1a1485e43b55b9bdd33fe1be714f`  
		Last Modified: Sat, 07 Aug 2021 00:08:54 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.22.1-alpine` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:a6cf6a518fea52b3fc47ed4572652aa0e2350898b54cdbcc0f778150de352dbd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.6 MB (9559904 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c8b625df6f0e93de9095159d166249a43a96ef9f3013e4a2c483b5ac7bc972b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 06 Aug 2021 17:49:32 GMT
ADD file:7f2c7deda009eabdcbbdccb11e854043d32c498e64e7e1ca02165d7bb4261d39 in / 
# Fri, 06 Aug 2021 17:49:32 GMT
CMD ["/bin/sh"]
# Fri, 06 Aug 2021 18:59:05 GMT
ENV NATS_STREAMING_SERVER=0.22.1
# Fri, 06 Aug 2021 18:59:10 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='581698d248a19ecae64e4048d153bc1021744a3da6284680a339f9f82a53a9cf' ;; 		armhf) natsArch='arm6'; sha256='438a89221bb0608e40d21e73ca27a4b70b8560730726942c0ade94a6b6013d6f' ;; 		armv7) natsArch='arm7'; sha256='4164baadd201d1374f7654d3e54a24d81ceb87a385867e31a82c1d1a69e3b1ae' ;; 		x86_64) natsArch='amd64'; sha256='f29e87ac9ff998c928aa8ebc8cf0c4d04d34a3d95b9900d92fd7dafab2bec8cc' ;; 		x86) natsArch='386'; sha256='0ca68e57babb8901d7afeb7569042730904887e718ddf860ef3ee54278753505' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 06 Aug 2021 18:59:10 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Fri, 06 Aug 2021 18:59:11 GMT
EXPOSE 4222 8222
# Fri, 06 Aug 2021 18:59:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 06 Aug 2021 18:59:12 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:f465bb3e9fcd0c42f936ecc566c6e40353c00f3089b2b2c2ea1663c30f89d3ab`  
		Last Modified: Fri, 06 Aug 2021 17:51:00 GMT  
		Size: 2.6 MB (2626350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:719cf2771983cbb32331cc8915e2edce30fbcb308f3504276742ffc9a3bc35fd`  
		Last Modified: Fri, 06 Aug 2021 19:00:56 GMT  
		Size: 6.9 MB (6933133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a72de2e4e74462365f574ec07048641b834163995d6b95fb88af2fca27e01883`  
		Last Modified: Fri, 06 Aug 2021 19:00:52 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.22.1-alpine` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:7970395d00490fad62f2a51288db47d251cab92ec7634bef6de42343f8e8eedc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.4 MB (9351328 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e19086c92b47964c105a8ed130ff7219833adab1ca8e211c1ad0b0a049866252`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 06 Aug 2021 17:57:32 GMT
ADD file:3a35ff3ac0d80289d419a4d6d8319610c38e1936d296addafb9aaf506946230f in / 
# Fri, 06 Aug 2021 17:57:32 GMT
CMD ["/bin/sh"]
# Fri, 06 Aug 2021 20:29:42 GMT
ENV NATS_STREAMING_SERVER=0.22.1
# Fri, 06 Aug 2021 20:29:48 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='581698d248a19ecae64e4048d153bc1021744a3da6284680a339f9f82a53a9cf' ;; 		armhf) natsArch='arm6'; sha256='438a89221bb0608e40d21e73ca27a4b70b8560730726942c0ade94a6b6013d6f' ;; 		armv7) natsArch='arm7'; sha256='4164baadd201d1374f7654d3e54a24d81ceb87a385867e31a82c1d1a69e3b1ae' ;; 		x86_64) natsArch='amd64'; sha256='f29e87ac9ff998c928aa8ebc8cf0c4d04d34a3d95b9900d92fd7dafab2bec8cc' ;; 		x86) natsArch='386'; sha256='0ca68e57babb8901d7afeb7569042730904887e718ddf860ef3ee54278753505' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 06 Aug 2021 20:29:48 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Fri, 06 Aug 2021 20:29:49 GMT
EXPOSE 4222 8222
# Fri, 06 Aug 2021 20:29:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 06 Aug 2021 20:29:50 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:4ee0caa23b369b04827640a4be298bf4ff7bacd030c77e915f5d7fb8f987594a`  
		Last Modified: Fri, 06 Aug 2021 17:58:57 GMT  
		Size: 2.4 MB (2429359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e14712e6c4fbdd823f35d0df7aa1345088ce3d89727133dcef4adb1105ecb5f`  
		Last Modified: Fri, 06 Aug 2021 20:31:34 GMT  
		Size: 6.9 MB (6921548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e18c45098374f86d0784e7840a2c0fd15ce636edfee6d3ebc23432fd0cc47be5`  
		Last Modified: Fri, 06 Aug 2021 20:31:30 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.22.1-alpine` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:c4818cc3ef0783732a51706c2f08756aad823d8829e0cd0a3e0332606b2a5851
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.5 MB (9541696 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c46cfd47aedfb2dfd2d6ede8515150bcce95d109f4180ab8d4ab95055cca9b62`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 06 Aug 2021 17:39:26 GMT
ADD file:1a8fd1066485e1261462e689c1a072f010c1d3be904b73ef2b84128fac652951 in / 
# Fri, 06 Aug 2021 17:39:27 GMT
CMD ["/bin/sh"]
# Fri, 06 Aug 2021 19:51:42 GMT
ENV NATS_STREAMING_SERVER=0.22.1
# Fri, 06 Aug 2021 19:51:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='581698d248a19ecae64e4048d153bc1021744a3da6284680a339f9f82a53a9cf' ;; 		armhf) natsArch='arm6'; sha256='438a89221bb0608e40d21e73ca27a4b70b8560730726942c0ade94a6b6013d6f' ;; 		armv7) natsArch='arm7'; sha256='4164baadd201d1374f7654d3e54a24d81ceb87a385867e31a82c1d1a69e3b1ae' ;; 		x86_64) natsArch='amd64'; sha256='f29e87ac9ff998c928aa8ebc8cf0c4d04d34a3d95b9900d92fd7dafab2bec8cc' ;; 		x86) natsArch='386'; sha256='0ca68e57babb8901d7afeb7569042730904887e718ddf860ef3ee54278753505' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 06 Aug 2021 19:51:45 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Fri, 06 Aug 2021 19:51:45 GMT
EXPOSE 4222 8222
# Fri, 06 Aug 2021 19:51:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 06 Aug 2021 19:51:45 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:fd3acdcea5682abced546ec19fb6ebee725c5184e5d91614c469c0a79e67f2d0`  
		Last Modified: Fri, 06 Aug 2021 17:40:12 GMT  
		Size: 2.7 MB (2710613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0968d8a9e4506d1c6878a0b725fc7f4f449c0ddb3f88d3704902e19db206317`  
		Last Modified: Fri, 06 Aug 2021 19:52:37 GMT  
		Size: 6.8 MB (6830662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87ab8fb5390b1c71a899984eb600e99e2ad1526c1c22bc89d0f8f52e64af17aa`  
		Last Modified: Fri, 06 Aug 2021 19:52:35 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.22.1-alpine3.14`

```console
$ docker pull nats-streaming@sha256:e1479f281ad33982c8df81acee8d71d2049fe3535d7b1595adae6eeffd669c9e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.22.1-alpine3.14` - linux; amd64

```console
$ docker pull nats-streaming@sha256:b13c3888f620e128e2324e521a59ecdae8096c67f4448233afd380feafbf565e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.3 MB (10269210 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e299437f282dcf86645a5f6e5b3a8c7345ba0e4582e60b8b76b5c06d1b5d938`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 06 Aug 2021 17:19:45 GMT
ADD file:34eb5c40aa00028921a224d1764ae1b1f3ef710d191e4dfc7df55e0594aa7217 in / 
# Fri, 06 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Sat, 07 Aug 2021 00:08:04 GMT
ENV NATS_STREAMING_SERVER=0.22.1
# Sat, 07 Aug 2021 00:08:07 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='581698d248a19ecae64e4048d153bc1021744a3da6284680a339f9f82a53a9cf' ;; 		armhf) natsArch='arm6'; sha256='438a89221bb0608e40d21e73ca27a4b70b8560730726942c0ade94a6b6013d6f' ;; 		armv7) natsArch='arm7'; sha256='4164baadd201d1374f7654d3e54a24d81ceb87a385867e31a82c1d1a69e3b1ae' ;; 		x86_64) natsArch='amd64'; sha256='f29e87ac9ff998c928aa8ebc8cf0c4d04d34a3d95b9900d92fd7dafab2bec8cc' ;; 		x86) natsArch='386'; sha256='0ca68e57babb8901d7afeb7569042730904887e718ddf860ef3ee54278753505' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Sat, 07 Aug 2021 00:08:08 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Sat, 07 Aug 2021 00:08:08 GMT
EXPOSE 4222 8222
# Sat, 07 Aug 2021 00:08:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 07 Aug 2021 00:08:08 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:29291e31a76a7e560b9b7ad3cada56e8c18d50a96cca8a2573e4f4689d7aca77`  
		Last Modified: Thu, 05 Aug 2021 15:56:25 GMT  
		Size: 2.8 MB (2813006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ded93adf1b7cd7e872edc8b55f1b6f392ee0f39c43a12ea019e39c39818d7f8f`  
		Last Modified: Sat, 07 Aug 2021 00:08:56 GMT  
		Size: 7.5 MB (7455782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:146382f94f105a2b20528c00beadcfd4783e1a1485e43b55b9bdd33fe1be714f`  
		Last Modified: Sat, 07 Aug 2021 00:08:54 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.22.1-alpine3.14` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:a6cf6a518fea52b3fc47ed4572652aa0e2350898b54cdbcc0f778150de352dbd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.6 MB (9559904 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c8b625df6f0e93de9095159d166249a43a96ef9f3013e4a2c483b5ac7bc972b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 06 Aug 2021 17:49:32 GMT
ADD file:7f2c7deda009eabdcbbdccb11e854043d32c498e64e7e1ca02165d7bb4261d39 in / 
# Fri, 06 Aug 2021 17:49:32 GMT
CMD ["/bin/sh"]
# Fri, 06 Aug 2021 18:59:05 GMT
ENV NATS_STREAMING_SERVER=0.22.1
# Fri, 06 Aug 2021 18:59:10 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='581698d248a19ecae64e4048d153bc1021744a3da6284680a339f9f82a53a9cf' ;; 		armhf) natsArch='arm6'; sha256='438a89221bb0608e40d21e73ca27a4b70b8560730726942c0ade94a6b6013d6f' ;; 		armv7) natsArch='arm7'; sha256='4164baadd201d1374f7654d3e54a24d81ceb87a385867e31a82c1d1a69e3b1ae' ;; 		x86_64) natsArch='amd64'; sha256='f29e87ac9ff998c928aa8ebc8cf0c4d04d34a3d95b9900d92fd7dafab2bec8cc' ;; 		x86) natsArch='386'; sha256='0ca68e57babb8901d7afeb7569042730904887e718ddf860ef3ee54278753505' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 06 Aug 2021 18:59:10 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Fri, 06 Aug 2021 18:59:11 GMT
EXPOSE 4222 8222
# Fri, 06 Aug 2021 18:59:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 06 Aug 2021 18:59:12 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:f465bb3e9fcd0c42f936ecc566c6e40353c00f3089b2b2c2ea1663c30f89d3ab`  
		Last Modified: Fri, 06 Aug 2021 17:51:00 GMT  
		Size: 2.6 MB (2626350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:719cf2771983cbb32331cc8915e2edce30fbcb308f3504276742ffc9a3bc35fd`  
		Last Modified: Fri, 06 Aug 2021 19:00:56 GMT  
		Size: 6.9 MB (6933133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a72de2e4e74462365f574ec07048641b834163995d6b95fb88af2fca27e01883`  
		Last Modified: Fri, 06 Aug 2021 19:00:52 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.22.1-alpine3.14` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:7970395d00490fad62f2a51288db47d251cab92ec7634bef6de42343f8e8eedc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.4 MB (9351328 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e19086c92b47964c105a8ed130ff7219833adab1ca8e211c1ad0b0a049866252`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 06 Aug 2021 17:57:32 GMT
ADD file:3a35ff3ac0d80289d419a4d6d8319610c38e1936d296addafb9aaf506946230f in / 
# Fri, 06 Aug 2021 17:57:32 GMT
CMD ["/bin/sh"]
# Fri, 06 Aug 2021 20:29:42 GMT
ENV NATS_STREAMING_SERVER=0.22.1
# Fri, 06 Aug 2021 20:29:48 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='581698d248a19ecae64e4048d153bc1021744a3da6284680a339f9f82a53a9cf' ;; 		armhf) natsArch='arm6'; sha256='438a89221bb0608e40d21e73ca27a4b70b8560730726942c0ade94a6b6013d6f' ;; 		armv7) natsArch='arm7'; sha256='4164baadd201d1374f7654d3e54a24d81ceb87a385867e31a82c1d1a69e3b1ae' ;; 		x86_64) natsArch='amd64'; sha256='f29e87ac9ff998c928aa8ebc8cf0c4d04d34a3d95b9900d92fd7dafab2bec8cc' ;; 		x86) natsArch='386'; sha256='0ca68e57babb8901d7afeb7569042730904887e718ddf860ef3ee54278753505' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 06 Aug 2021 20:29:48 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Fri, 06 Aug 2021 20:29:49 GMT
EXPOSE 4222 8222
# Fri, 06 Aug 2021 20:29:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 06 Aug 2021 20:29:50 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:4ee0caa23b369b04827640a4be298bf4ff7bacd030c77e915f5d7fb8f987594a`  
		Last Modified: Fri, 06 Aug 2021 17:58:57 GMT  
		Size: 2.4 MB (2429359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e14712e6c4fbdd823f35d0df7aa1345088ce3d89727133dcef4adb1105ecb5f`  
		Last Modified: Fri, 06 Aug 2021 20:31:34 GMT  
		Size: 6.9 MB (6921548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e18c45098374f86d0784e7840a2c0fd15ce636edfee6d3ebc23432fd0cc47be5`  
		Last Modified: Fri, 06 Aug 2021 20:31:30 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.22.1-alpine3.14` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:c4818cc3ef0783732a51706c2f08756aad823d8829e0cd0a3e0332606b2a5851
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.5 MB (9541696 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c46cfd47aedfb2dfd2d6ede8515150bcce95d109f4180ab8d4ab95055cca9b62`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 06 Aug 2021 17:39:26 GMT
ADD file:1a8fd1066485e1261462e689c1a072f010c1d3be904b73ef2b84128fac652951 in / 
# Fri, 06 Aug 2021 17:39:27 GMT
CMD ["/bin/sh"]
# Fri, 06 Aug 2021 19:51:42 GMT
ENV NATS_STREAMING_SERVER=0.22.1
# Fri, 06 Aug 2021 19:51:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='581698d248a19ecae64e4048d153bc1021744a3da6284680a339f9f82a53a9cf' ;; 		armhf) natsArch='arm6'; sha256='438a89221bb0608e40d21e73ca27a4b70b8560730726942c0ade94a6b6013d6f' ;; 		armv7) natsArch='arm7'; sha256='4164baadd201d1374f7654d3e54a24d81ceb87a385867e31a82c1d1a69e3b1ae' ;; 		x86_64) natsArch='amd64'; sha256='f29e87ac9ff998c928aa8ebc8cf0c4d04d34a3d95b9900d92fd7dafab2bec8cc' ;; 		x86) natsArch='386'; sha256='0ca68e57babb8901d7afeb7569042730904887e718ddf860ef3ee54278753505' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 06 Aug 2021 19:51:45 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Fri, 06 Aug 2021 19:51:45 GMT
EXPOSE 4222 8222
# Fri, 06 Aug 2021 19:51:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 06 Aug 2021 19:51:45 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:fd3acdcea5682abced546ec19fb6ebee725c5184e5d91614c469c0a79e67f2d0`  
		Last Modified: Fri, 06 Aug 2021 17:40:12 GMT  
		Size: 2.7 MB (2710613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0968d8a9e4506d1c6878a0b725fc7f4f449c0ddb3f88d3704902e19db206317`  
		Last Modified: Fri, 06 Aug 2021 19:52:37 GMT  
		Size: 6.8 MB (6830662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87ab8fb5390b1c71a899984eb600e99e2ad1526c1c22bc89d0f8f52e64af17aa`  
		Last Modified: Fri, 06 Aug 2021 19:52:35 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.22.1-linux`

```console
$ docker pull nats-streaming@sha256:7d3a953263095ea9d7018d32bd3483577d512550bc7890ba7743f48963cce893
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.22.1-linux` - linux; amd64

```console
$ docker pull nats-streaming@sha256:3c6c9375f9e9724462e98cfb98a7abb50ceeca73b3070ce061992c4009e32157
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7168713 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:184d7920ac61dd2e84320b8040f57980a7d605d42948a520ede12d421168c4ce`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 02 Aug 2021 22:20:03 GMT
COPY file:ca9a212ccef327f9c2e91a62a908ac0cdbd39b08be331ea2b209c2d724942e18 in /nats-streaming-server 
# Mon, 02 Aug 2021 22:20:03 GMT
EXPOSE 4222 8222
# Mon, 02 Aug 2021 22:20:03 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 02 Aug 2021 22:20:03 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:f3749ab6cbfff03714b5a6a1245fa249b67d19e7358b74cbc50232b14370481a`  
		Last Modified: Mon, 02 Aug 2021 22:20:48 GMT  
		Size: 7.2 MB (7168713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.22.1-linux` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:e944d0e843d59d5979d7561c06b0c0adc874ceaa0bd34d3a7b536b25e8c9704d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.7 MB (6650246 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0146bbca3802c65d86e148b1d203b3d395ca1cd8a8bb89461888570d821dc4fb`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 02 Aug 2021 22:51:34 GMT
COPY file:68ac67d86d6ac617adc181feb43580415b7fc7640a3c7577bb3753c369908da0 in /nats-streaming-server 
# Mon, 02 Aug 2021 22:51:35 GMT
EXPOSE 4222 8222
# Mon, 02 Aug 2021 22:51:35 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 02 Aug 2021 22:51:35 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:c7e1d707b6179f690f3f44212cb8c9a3fe914d91d3f1ddbac9f176aa0610c90a`  
		Last Modified: Mon, 02 Aug 2021 22:53:32 GMT  
		Size: 6.7 MB (6650246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.22.1-linux` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:a5e3d56b343f9091f353634f59f688998544ccd4f2cbb80001d08ea6a3207274
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6639768 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80206ae32558812ad047d8ab67519615e98e7df68a884fc32b6d5fd8f72593b0`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 02 Aug 2021 23:11:17 GMT
COPY file:79708b5d249193a95e72c506453fd1ecd3e2738ec2ff3423c4b2bd760f426da2 in /nats-streaming-server 
# Mon, 02 Aug 2021 23:11:18 GMT
EXPOSE 4222 8222
# Mon, 02 Aug 2021 23:11:18 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 02 Aug 2021 23:11:19 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:52753762f751e166edd44e37a0ef0a06b33c337bdeb66e4134ee8479a49dae68`  
		Last Modified: Mon, 02 Aug 2021 23:13:17 GMT  
		Size: 6.6 MB (6639768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.22.1-linux` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:96652223cce95275138363a54affb8663ba46bc75831c2a9535375ab6d922143
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 MB (6546324 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:952bbd74028df1debbfe0e4665b514c66a36537d0868d41bc971ddb55793c442`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 02 Aug 2021 22:40:16 GMT
COPY file:a77d9769f43cc6943be482183091d3360eaadf93bf1ef5a67f0869d5555868a6 in /nats-streaming-server 
# Mon, 02 Aug 2021 22:40:17 GMT
EXPOSE 4222 8222
# Mon, 02 Aug 2021 22:40:17 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 02 Aug 2021 22:40:17 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4dc8aa7843ed2da454d59006acb180caee3f980d12034caacd4a32ffedab3df7`  
		Last Modified: Mon, 02 Aug 2021 22:41:24 GMT  
		Size: 6.5 MB (6546324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.22.1-nanoserver`

```console
$ docker pull nats-streaming@sha256:8407af82564828d613edb1e65aedfa7d022699303898c4c33b02f71106e85700
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2114; amd64

### `nats-streaming:0.22.1-nanoserver` - windows version 10.0.17763.2114; amd64

```console
$ docker pull nats-streaming@sha256:8b058c3d2bf71043f26b6b58702562c13724bb5594ceebad3f49b4f539c3c227
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.0 MB (110039206 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:29bedda8d4d57688f52e1b97404c0dd1ecd0d7823e3f5e07a6f0214ee01d7853`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 05 Aug 2021 19:15:20 GMT
RUN Apply image 1809-amd64
# Wed, 11 Aug 2021 16:52:04 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 11 Aug 2021 21:19:29 GMT
RUN cmd /S /C #(nop) COPY file:9670e5d1fe5a71e47c78fde01235a0bcbcafcfdeeacf96a7669f6e49343fb03b in C:\nats-streaming-server.exe 
# Wed, 11 Aug 2021 21:19:33 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 11 Aug 2021 21:19:36 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 11 Aug 2021 21:19:39 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:bc8517709e9cfff223cb034ff5be8fcbfa5409de286cdac9ae1b8878ebea6b84`  
		Size: 102.7 MB (102741177 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3aa4a9dea1e2eabb29e2100fd699f3e3acbcabd85f360a3799b2505a5f74e5a0`  
		Last Modified: Wed, 11 Aug 2021 16:57:14 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2422c6b202cf35a718dc80ef76006199902c019414449d929f2538d72106be7`  
		Last Modified: Wed, 11 Aug 2021 21:24:43 GMT  
		Size: 7.3 MB (7293397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe1c9060adc003485accbb3848bb825c0b555a9e064d8ee4861937d781f4fb6d`  
		Last Modified: Wed, 11 Aug 2021 21:24:35 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eebb7419f921a924ca580e9c32580b82f2748e7759754b74686a3778fd920843`  
		Last Modified: Wed, 11 Aug 2021 21:24:35 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:413188a47dae1e13011a4e6d4ef5a31f5e680e350820d0b968981bc816827aaa`  
		Last Modified: Wed, 11 Aug 2021 21:24:35 GMT  
		Size: 1.2 KB (1174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.22.1-nanoserver-1809`

```console
$ docker pull nats-streaming@sha256:8407af82564828d613edb1e65aedfa7d022699303898c4c33b02f71106e85700
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2114; amd64

### `nats-streaming:0.22.1-nanoserver-1809` - windows version 10.0.17763.2114; amd64

```console
$ docker pull nats-streaming@sha256:8b058c3d2bf71043f26b6b58702562c13724bb5594ceebad3f49b4f539c3c227
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.0 MB (110039206 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:29bedda8d4d57688f52e1b97404c0dd1ecd0d7823e3f5e07a6f0214ee01d7853`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 05 Aug 2021 19:15:20 GMT
RUN Apply image 1809-amd64
# Wed, 11 Aug 2021 16:52:04 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 11 Aug 2021 21:19:29 GMT
RUN cmd /S /C #(nop) COPY file:9670e5d1fe5a71e47c78fde01235a0bcbcafcfdeeacf96a7669f6e49343fb03b in C:\nats-streaming-server.exe 
# Wed, 11 Aug 2021 21:19:33 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 11 Aug 2021 21:19:36 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 11 Aug 2021 21:19:39 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:bc8517709e9cfff223cb034ff5be8fcbfa5409de286cdac9ae1b8878ebea6b84`  
		Size: 102.7 MB (102741177 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3aa4a9dea1e2eabb29e2100fd699f3e3acbcabd85f360a3799b2505a5f74e5a0`  
		Last Modified: Wed, 11 Aug 2021 16:57:14 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2422c6b202cf35a718dc80ef76006199902c019414449d929f2538d72106be7`  
		Last Modified: Wed, 11 Aug 2021 21:24:43 GMT  
		Size: 7.3 MB (7293397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe1c9060adc003485accbb3848bb825c0b555a9e064d8ee4861937d781f4fb6d`  
		Last Modified: Wed, 11 Aug 2021 21:24:35 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eebb7419f921a924ca580e9c32580b82f2748e7759754b74686a3778fd920843`  
		Last Modified: Wed, 11 Aug 2021 21:24:35 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:413188a47dae1e13011a4e6d4ef5a31f5e680e350820d0b968981bc816827aaa`  
		Last Modified: Wed, 11 Aug 2021 21:24:35 GMT  
		Size: 1.2 KB (1174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.22.1-scratch`

```console
$ docker pull nats-streaming@sha256:7d3a953263095ea9d7018d32bd3483577d512550bc7890ba7743f48963cce893
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.22.1-scratch` - linux; amd64

```console
$ docker pull nats-streaming@sha256:3c6c9375f9e9724462e98cfb98a7abb50ceeca73b3070ce061992c4009e32157
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7168713 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:184d7920ac61dd2e84320b8040f57980a7d605d42948a520ede12d421168c4ce`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 02 Aug 2021 22:20:03 GMT
COPY file:ca9a212ccef327f9c2e91a62a908ac0cdbd39b08be331ea2b209c2d724942e18 in /nats-streaming-server 
# Mon, 02 Aug 2021 22:20:03 GMT
EXPOSE 4222 8222
# Mon, 02 Aug 2021 22:20:03 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 02 Aug 2021 22:20:03 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:f3749ab6cbfff03714b5a6a1245fa249b67d19e7358b74cbc50232b14370481a`  
		Last Modified: Mon, 02 Aug 2021 22:20:48 GMT  
		Size: 7.2 MB (7168713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.22.1-scratch` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:e944d0e843d59d5979d7561c06b0c0adc874ceaa0bd34d3a7b536b25e8c9704d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.7 MB (6650246 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0146bbca3802c65d86e148b1d203b3d395ca1cd8a8bb89461888570d821dc4fb`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 02 Aug 2021 22:51:34 GMT
COPY file:68ac67d86d6ac617adc181feb43580415b7fc7640a3c7577bb3753c369908da0 in /nats-streaming-server 
# Mon, 02 Aug 2021 22:51:35 GMT
EXPOSE 4222 8222
# Mon, 02 Aug 2021 22:51:35 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 02 Aug 2021 22:51:35 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:c7e1d707b6179f690f3f44212cb8c9a3fe914d91d3f1ddbac9f176aa0610c90a`  
		Last Modified: Mon, 02 Aug 2021 22:53:32 GMT  
		Size: 6.7 MB (6650246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.22.1-scratch` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:a5e3d56b343f9091f353634f59f688998544ccd4f2cbb80001d08ea6a3207274
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6639768 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80206ae32558812ad047d8ab67519615e98e7df68a884fc32b6d5fd8f72593b0`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 02 Aug 2021 23:11:17 GMT
COPY file:79708b5d249193a95e72c506453fd1ecd3e2738ec2ff3423c4b2bd760f426da2 in /nats-streaming-server 
# Mon, 02 Aug 2021 23:11:18 GMT
EXPOSE 4222 8222
# Mon, 02 Aug 2021 23:11:18 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 02 Aug 2021 23:11:19 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:52753762f751e166edd44e37a0ef0a06b33c337bdeb66e4134ee8479a49dae68`  
		Last Modified: Mon, 02 Aug 2021 23:13:17 GMT  
		Size: 6.6 MB (6639768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.22.1-scratch` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:96652223cce95275138363a54affb8663ba46bc75831c2a9535375ab6d922143
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 MB (6546324 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:952bbd74028df1debbfe0e4665b514c66a36537d0868d41bc971ddb55793c442`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 02 Aug 2021 22:40:16 GMT
COPY file:a77d9769f43cc6943be482183091d3360eaadf93bf1ef5a67f0869d5555868a6 in /nats-streaming-server 
# Mon, 02 Aug 2021 22:40:17 GMT
EXPOSE 4222 8222
# Mon, 02 Aug 2021 22:40:17 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 02 Aug 2021 22:40:17 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4dc8aa7843ed2da454d59006acb180caee3f980d12034caacd4a32ffedab3df7`  
		Last Modified: Mon, 02 Aug 2021 22:41:24 GMT  
		Size: 6.5 MB (6546324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.22.1-windowsservercore`

```console
$ docker pull nats-streaming@sha256:5f9e88c929ff89c3204d105008a059f9be67f540ff96b5bfec99e3b254351411
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.2114; amd64
	-	windows version 10.0.14393.4583; amd64

### `nats-streaming:0.22.1-windowsservercore` - windows version 10.0.17763.2114; amd64

```console
$ docker pull nats-streaming@sha256:75b04016fe1b2f4c6a7bef238c62f6610c86ab0baed8d1031b7f061053987a27
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2693987543 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ffc0c1be51519eff598c2d5cce32f011fcfe27c06a9651541cec6796f3f66a56`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 05 Aug 2021 19:44:34 GMT
RUN Install update 1809-amd64
# Wed, 11 Aug 2021 13:42:12 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 11 Aug 2021 16:48:51 GMT
ENV NATS_DOCKERIZED=1
# Wed, 11 Aug 2021 21:16:00 GMT
ENV NATS_STREAMING_SERVER=0.22.1
# Wed, 11 Aug 2021 21:16:03 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.22.1/nats-streaming-server-v0.22.1-windows-amd64.zip
# Wed, 11 Aug 2021 21:16:06 GMT
ENV NATS_STREAMING_SERVER_SHASUM=4516852b493111b73ec06477be4a27e66f5abc9ca1ff4dd2b970232271611264
# Wed, 11 Aug 2021 21:17:09 GMT
RUN Set-PSDebug -Trace 2
# Wed, 11 Aug 2021 21:19:07 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 11 Aug 2021 21:19:10 GMT
EXPOSE 4222 8222
# Wed, 11 Aug 2021 21:19:13 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 11 Aug 2021 21:19:15 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c67ded6868b61d392a0c096f911563fd6bc0bc3ed4fe401d077b3718a1b0cdaf`  
		Size: 967.7 MB (967665054 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c613f4c34660a122de754415a884afe6b12172ac3ce792a2e4aae831cc8b2e27`  
		Last Modified: Wed, 11 Aug 2021 16:25:11 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71d8e65d39d1b09c34e0dadad1a6b7818f430fb13ce2ff8d70c549b137f9131a`  
		Last Modified: Wed, 11 Aug 2021 16:56:54 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f48fea2e101940ffa36628a8fd4da200aa97417773d993be6df74d0bcff8dccc`  
		Last Modified: Wed, 11 Aug 2021 21:24:22 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bd10110cd94f48fce072addebc384215cfee9e902098952b29a44227fc4c19b`  
		Last Modified: Wed, 11 Aug 2021 21:24:22 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f32d77caa28f59168738bee8473e7e58d117ce711f59589f9627b0facfe620bd`  
		Last Modified: Wed, 11 Aug 2021 21:24:22 GMT  
		Size: 1.4 KB (1443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90f9d42ecbcdc48ff53122318c96640c628d9f2b33df84c887b89a1b1429091e`  
		Last Modified: Wed, 11 Aug 2021 21:24:19 GMT  
		Size: 351.7 KB (351714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfe2bf098cd0e80bd3e81951fb0f411238d63d458bcd51ecd3427a1566fd0ffc`  
		Last Modified: Wed, 11 Aug 2021 21:24:21 GMT  
		Size: 7.6 MB (7626528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e710a2acda7795374f6c855a7d81c6156b961c06f5b0f13fd31e2d8c4952fd6`  
		Last Modified: Wed, 11 Aug 2021 21:24:19 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2333773eafb1bb6c7fd6fd55fd31614ec447f3b1af48b5f63fe1ee29a4093ff2`  
		Last Modified: Wed, 11 Aug 2021 21:24:19 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:666623a49ff4c5032408abc00ae56261476eed8930351412760fedada9e6e136`  
		Last Modified: Wed, 11 Aug 2021 21:24:19 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.22.1-windowsservercore` - windows version 10.0.14393.4583; amd64

```console
$ docker pull nats-streaming@sha256:c2dc8bad14a0594eb6483398e8aa5f20933884855abece46d39a9aaa5ff6c0de
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6283441295 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d4dcfbb00a058925aa22ae213359605c8892f3261a0afdd6941153ff9789f841`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Sun, 01 Aug 2021 08:52:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 11 Aug 2021 13:57:45 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 11 Aug 2021 16:52:27 GMT
ENV NATS_DOCKERIZED=1
# Wed, 11 Aug 2021 21:19:47 GMT
ENV NATS_STREAMING_SERVER=0.22.1
# Wed, 11 Aug 2021 21:19:50 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.22.1/nats-streaming-server-v0.22.1-windows-amd64.zip
# Wed, 11 Aug 2021 21:19:53 GMT
ENV NATS_STREAMING_SERVER_SHASUM=4516852b493111b73ec06477be4a27e66f5abc9ca1ff4dd2b970232271611264
# Wed, 11 Aug 2021 21:21:16 GMT
RUN Set-PSDebug -Trace 2
# Wed, 11 Aug 2021 21:23:38 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 11 Aug 2021 21:23:41 GMT
EXPOSE 4222 8222
# Wed, 11 Aug 2021 21:23:43 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 11 Aug 2021 21:23:46 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c427f892fe74603ae09d4e49b25f8f7046f957054034dc9f462e0e88d7bffaa5`  
		Size: 2.2 GB (2200980134 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d6d4b60a6f3b0544427c2eb9a5e27e5f6ddca0fd7632003e11331f01c4e9c6fc`  
		Last Modified: Wed, 11 Aug 2021 16:25:34 GMT  
		Size: 1.4 KB (1442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe49d3a206649779952cc6a03fdbb4e828336501708ad40c4e1a07237199e28b`  
		Last Modified: Wed, 11 Aug 2021 16:57:38 GMT  
		Size: 1.4 KB (1380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e6e2dfe14e85c8398dc3f7c7906fb1f7c777ef6d5717fe70d978ad05718ffc2`  
		Last Modified: Wed, 11 Aug 2021 21:24:59 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f846ec4e42dc3dac55d428bcb2d57cab68f2b659b2cdbba1cad2800b22496145`  
		Last Modified: Wed, 11 Aug 2021 21:24:59 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a073e823edff403699ab0d2dff8376e1b0fb57af79842af3133c0b0c0e3c77f0`  
		Last Modified: Wed, 11 Aug 2021 21:24:59 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bedf8cee66f4f7e59aee0a000c7fe523b2994d8d7f358c994942fb8b6a9ae6c`  
		Last Modified: Wed, 11 Aug 2021 21:24:57 GMT  
		Size: 338.6 KB (338573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:275d8c5f6fbce1b85b62d1f70554f8ecf9d3ccdbfe54c86356703cc697b71e2b`  
		Last Modified: Wed, 11 Aug 2021 21:24:59 GMT  
		Size: 12.1 MB (12125382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b86e3ac00ba61bf48479b43167f3550a6c8ed7af7da7dd5c0b86441e7d8f662`  
		Last Modified: Wed, 11 Aug 2021 21:24:56 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f45154e30184ba145c5239532f29c91a714e1e6be10588ab43f2dfc69986775e`  
		Last Modified: Wed, 11 Aug 2021 21:24:56 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:254423fab1337576ad61d5fdd3942f86d494a694b38f8c0f779f9239789684b3`  
		Last Modified: Wed, 11 Aug 2021 21:24:56 GMT  
		Size: 1.4 KB (1443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.22.1-windowsservercore-1809`

```console
$ docker pull nats-streaming@sha256:17e69850495ccb3a8a86278c37ad940698ed0da3f3c08f6de694456dbb989c25
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2114; amd64

### `nats-streaming:0.22.1-windowsservercore-1809` - windows version 10.0.17763.2114; amd64

```console
$ docker pull nats-streaming@sha256:75b04016fe1b2f4c6a7bef238c62f6610c86ab0baed8d1031b7f061053987a27
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2693987543 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ffc0c1be51519eff598c2d5cce32f011fcfe27c06a9651541cec6796f3f66a56`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 05 Aug 2021 19:44:34 GMT
RUN Install update 1809-amd64
# Wed, 11 Aug 2021 13:42:12 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 11 Aug 2021 16:48:51 GMT
ENV NATS_DOCKERIZED=1
# Wed, 11 Aug 2021 21:16:00 GMT
ENV NATS_STREAMING_SERVER=0.22.1
# Wed, 11 Aug 2021 21:16:03 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.22.1/nats-streaming-server-v0.22.1-windows-amd64.zip
# Wed, 11 Aug 2021 21:16:06 GMT
ENV NATS_STREAMING_SERVER_SHASUM=4516852b493111b73ec06477be4a27e66f5abc9ca1ff4dd2b970232271611264
# Wed, 11 Aug 2021 21:17:09 GMT
RUN Set-PSDebug -Trace 2
# Wed, 11 Aug 2021 21:19:07 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 11 Aug 2021 21:19:10 GMT
EXPOSE 4222 8222
# Wed, 11 Aug 2021 21:19:13 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 11 Aug 2021 21:19:15 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c67ded6868b61d392a0c096f911563fd6bc0bc3ed4fe401d077b3718a1b0cdaf`  
		Size: 967.7 MB (967665054 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c613f4c34660a122de754415a884afe6b12172ac3ce792a2e4aae831cc8b2e27`  
		Last Modified: Wed, 11 Aug 2021 16:25:11 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71d8e65d39d1b09c34e0dadad1a6b7818f430fb13ce2ff8d70c549b137f9131a`  
		Last Modified: Wed, 11 Aug 2021 16:56:54 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f48fea2e101940ffa36628a8fd4da200aa97417773d993be6df74d0bcff8dccc`  
		Last Modified: Wed, 11 Aug 2021 21:24:22 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bd10110cd94f48fce072addebc384215cfee9e902098952b29a44227fc4c19b`  
		Last Modified: Wed, 11 Aug 2021 21:24:22 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f32d77caa28f59168738bee8473e7e58d117ce711f59589f9627b0facfe620bd`  
		Last Modified: Wed, 11 Aug 2021 21:24:22 GMT  
		Size: 1.4 KB (1443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90f9d42ecbcdc48ff53122318c96640c628d9f2b33df84c887b89a1b1429091e`  
		Last Modified: Wed, 11 Aug 2021 21:24:19 GMT  
		Size: 351.7 KB (351714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfe2bf098cd0e80bd3e81951fb0f411238d63d458bcd51ecd3427a1566fd0ffc`  
		Last Modified: Wed, 11 Aug 2021 21:24:21 GMT  
		Size: 7.6 MB (7626528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e710a2acda7795374f6c855a7d81c6156b961c06f5b0f13fd31e2d8c4952fd6`  
		Last Modified: Wed, 11 Aug 2021 21:24:19 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2333773eafb1bb6c7fd6fd55fd31614ec447f3b1af48b5f63fe1ee29a4093ff2`  
		Last Modified: Wed, 11 Aug 2021 21:24:19 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:666623a49ff4c5032408abc00ae56261476eed8930351412760fedada9e6e136`  
		Last Modified: Wed, 11 Aug 2021 21:24:19 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.22.1-windowsservercore-ltsc2016`

```console
$ docker pull nats-streaming@sha256:9cfea454a5d6b43341f213ae8515bf3ccf36487967fc16fad686bd3bed667681
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.14393.4583; amd64

### `nats-streaming:0.22.1-windowsservercore-ltsc2016` - windows version 10.0.14393.4583; amd64

```console
$ docker pull nats-streaming@sha256:c2dc8bad14a0594eb6483398e8aa5f20933884855abece46d39a9aaa5ff6c0de
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6283441295 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d4dcfbb00a058925aa22ae213359605c8892f3261a0afdd6941153ff9789f841`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Sun, 01 Aug 2021 08:52:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 11 Aug 2021 13:57:45 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 11 Aug 2021 16:52:27 GMT
ENV NATS_DOCKERIZED=1
# Wed, 11 Aug 2021 21:19:47 GMT
ENV NATS_STREAMING_SERVER=0.22.1
# Wed, 11 Aug 2021 21:19:50 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.22.1/nats-streaming-server-v0.22.1-windows-amd64.zip
# Wed, 11 Aug 2021 21:19:53 GMT
ENV NATS_STREAMING_SERVER_SHASUM=4516852b493111b73ec06477be4a27e66f5abc9ca1ff4dd2b970232271611264
# Wed, 11 Aug 2021 21:21:16 GMT
RUN Set-PSDebug -Trace 2
# Wed, 11 Aug 2021 21:23:38 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 11 Aug 2021 21:23:41 GMT
EXPOSE 4222 8222
# Wed, 11 Aug 2021 21:23:43 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 11 Aug 2021 21:23:46 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c427f892fe74603ae09d4e49b25f8f7046f957054034dc9f462e0e88d7bffaa5`  
		Size: 2.2 GB (2200980134 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d6d4b60a6f3b0544427c2eb9a5e27e5f6ddca0fd7632003e11331f01c4e9c6fc`  
		Last Modified: Wed, 11 Aug 2021 16:25:34 GMT  
		Size: 1.4 KB (1442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe49d3a206649779952cc6a03fdbb4e828336501708ad40c4e1a07237199e28b`  
		Last Modified: Wed, 11 Aug 2021 16:57:38 GMT  
		Size: 1.4 KB (1380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e6e2dfe14e85c8398dc3f7c7906fb1f7c777ef6d5717fe70d978ad05718ffc2`  
		Last Modified: Wed, 11 Aug 2021 21:24:59 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f846ec4e42dc3dac55d428bcb2d57cab68f2b659b2cdbba1cad2800b22496145`  
		Last Modified: Wed, 11 Aug 2021 21:24:59 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a073e823edff403699ab0d2dff8376e1b0fb57af79842af3133c0b0c0e3c77f0`  
		Last Modified: Wed, 11 Aug 2021 21:24:59 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bedf8cee66f4f7e59aee0a000c7fe523b2994d8d7f358c994942fb8b6a9ae6c`  
		Last Modified: Wed, 11 Aug 2021 21:24:57 GMT  
		Size: 338.6 KB (338573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:275d8c5f6fbce1b85b62d1f70554f8ecf9d3ccdbfe54c86356703cc697b71e2b`  
		Last Modified: Wed, 11 Aug 2021 21:24:59 GMT  
		Size: 12.1 MB (12125382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b86e3ac00ba61bf48479b43167f3550a6c8ed7af7da7dd5c0b86441e7d8f662`  
		Last Modified: Wed, 11 Aug 2021 21:24:56 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f45154e30184ba145c5239532f29c91a714e1e6be10588ab43f2dfc69986775e`  
		Last Modified: Wed, 11 Aug 2021 21:24:56 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:254423fab1337576ad61d5fdd3942f86d494a694b38f8c0f779f9239789684b3`  
		Last Modified: Wed, 11 Aug 2021 21:24:56 GMT  
		Size: 1.4 KB (1443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:alpine`

```console
$ docker pull nats-streaming@sha256:e1479f281ad33982c8df81acee8d71d2049fe3535d7b1595adae6eeffd669c9e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:alpine` - linux; amd64

```console
$ docker pull nats-streaming@sha256:b13c3888f620e128e2324e521a59ecdae8096c67f4448233afd380feafbf565e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.3 MB (10269210 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e299437f282dcf86645a5f6e5b3a8c7345ba0e4582e60b8b76b5c06d1b5d938`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 06 Aug 2021 17:19:45 GMT
ADD file:34eb5c40aa00028921a224d1764ae1b1f3ef710d191e4dfc7df55e0594aa7217 in / 
# Fri, 06 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Sat, 07 Aug 2021 00:08:04 GMT
ENV NATS_STREAMING_SERVER=0.22.1
# Sat, 07 Aug 2021 00:08:07 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='581698d248a19ecae64e4048d153bc1021744a3da6284680a339f9f82a53a9cf' ;; 		armhf) natsArch='arm6'; sha256='438a89221bb0608e40d21e73ca27a4b70b8560730726942c0ade94a6b6013d6f' ;; 		armv7) natsArch='arm7'; sha256='4164baadd201d1374f7654d3e54a24d81ceb87a385867e31a82c1d1a69e3b1ae' ;; 		x86_64) natsArch='amd64'; sha256='f29e87ac9ff998c928aa8ebc8cf0c4d04d34a3d95b9900d92fd7dafab2bec8cc' ;; 		x86) natsArch='386'; sha256='0ca68e57babb8901d7afeb7569042730904887e718ddf860ef3ee54278753505' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Sat, 07 Aug 2021 00:08:08 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Sat, 07 Aug 2021 00:08:08 GMT
EXPOSE 4222 8222
# Sat, 07 Aug 2021 00:08:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 07 Aug 2021 00:08:08 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:29291e31a76a7e560b9b7ad3cada56e8c18d50a96cca8a2573e4f4689d7aca77`  
		Last Modified: Thu, 05 Aug 2021 15:56:25 GMT  
		Size: 2.8 MB (2813006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ded93adf1b7cd7e872edc8b55f1b6f392ee0f39c43a12ea019e39c39818d7f8f`  
		Last Modified: Sat, 07 Aug 2021 00:08:56 GMT  
		Size: 7.5 MB (7455782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:146382f94f105a2b20528c00beadcfd4783e1a1485e43b55b9bdd33fe1be714f`  
		Last Modified: Sat, 07 Aug 2021 00:08:54 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:a6cf6a518fea52b3fc47ed4572652aa0e2350898b54cdbcc0f778150de352dbd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.6 MB (9559904 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c8b625df6f0e93de9095159d166249a43a96ef9f3013e4a2c483b5ac7bc972b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 06 Aug 2021 17:49:32 GMT
ADD file:7f2c7deda009eabdcbbdccb11e854043d32c498e64e7e1ca02165d7bb4261d39 in / 
# Fri, 06 Aug 2021 17:49:32 GMT
CMD ["/bin/sh"]
# Fri, 06 Aug 2021 18:59:05 GMT
ENV NATS_STREAMING_SERVER=0.22.1
# Fri, 06 Aug 2021 18:59:10 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='581698d248a19ecae64e4048d153bc1021744a3da6284680a339f9f82a53a9cf' ;; 		armhf) natsArch='arm6'; sha256='438a89221bb0608e40d21e73ca27a4b70b8560730726942c0ade94a6b6013d6f' ;; 		armv7) natsArch='arm7'; sha256='4164baadd201d1374f7654d3e54a24d81ceb87a385867e31a82c1d1a69e3b1ae' ;; 		x86_64) natsArch='amd64'; sha256='f29e87ac9ff998c928aa8ebc8cf0c4d04d34a3d95b9900d92fd7dafab2bec8cc' ;; 		x86) natsArch='386'; sha256='0ca68e57babb8901d7afeb7569042730904887e718ddf860ef3ee54278753505' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 06 Aug 2021 18:59:10 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Fri, 06 Aug 2021 18:59:11 GMT
EXPOSE 4222 8222
# Fri, 06 Aug 2021 18:59:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 06 Aug 2021 18:59:12 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:f465bb3e9fcd0c42f936ecc566c6e40353c00f3089b2b2c2ea1663c30f89d3ab`  
		Last Modified: Fri, 06 Aug 2021 17:51:00 GMT  
		Size: 2.6 MB (2626350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:719cf2771983cbb32331cc8915e2edce30fbcb308f3504276742ffc9a3bc35fd`  
		Last Modified: Fri, 06 Aug 2021 19:00:56 GMT  
		Size: 6.9 MB (6933133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a72de2e4e74462365f574ec07048641b834163995d6b95fb88af2fca27e01883`  
		Last Modified: Fri, 06 Aug 2021 19:00:52 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:7970395d00490fad62f2a51288db47d251cab92ec7634bef6de42343f8e8eedc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.4 MB (9351328 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e19086c92b47964c105a8ed130ff7219833adab1ca8e211c1ad0b0a049866252`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 06 Aug 2021 17:57:32 GMT
ADD file:3a35ff3ac0d80289d419a4d6d8319610c38e1936d296addafb9aaf506946230f in / 
# Fri, 06 Aug 2021 17:57:32 GMT
CMD ["/bin/sh"]
# Fri, 06 Aug 2021 20:29:42 GMT
ENV NATS_STREAMING_SERVER=0.22.1
# Fri, 06 Aug 2021 20:29:48 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='581698d248a19ecae64e4048d153bc1021744a3da6284680a339f9f82a53a9cf' ;; 		armhf) natsArch='arm6'; sha256='438a89221bb0608e40d21e73ca27a4b70b8560730726942c0ade94a6b6013d6f' ;; 		armv7) natsArch='arm7'; sha256='4164baadd201d1374f7654d3e54a24d81ceb87a385867e31a82c1d1a69e3b1ae' ;; 		x86_64) natsArch='amd64'; sha256='f29e87ac9ff998c928aa8ebc8cf0c4d04d34a3d95b9900d92fd7dafab2bec8cc' ;; 		x86) natsArch='386'; sha256='0ca68e57babb8901d7afeb7569042730904887e718ddf860ef3ee54278753505' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 06 Aug 2021 20:29:48 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Fri, 06 Aug 2021 20:29:49 GMT
EXPOSE 4222 8222
# Fri, 06 Aug 2021 20:29:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 06 Aug 2021 20:29:50 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:4ee0caa23b369b04827640a4be298bf4ff7bacd030c77e915f5d7fb8f987594a`  
		Last Modified: Fri, 06 Aug 2021 17:58:57 GMT  
		Size: 2.4 MB (2429359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e14712e6c4fbdd823f35d0df7aa1345088ce3d89727133dcef4adb1105ecb5f`  
		Last Modified: Fri, 06 Aug 2021 20:31:34 GMT  
		Size: 6.9 MB (6921548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e18c45098374f86d0784e7840a2c0fd15ce636edfee6d3ebc23432fd0cc47be5`  
		Last Modified: Fri, 06 Aug 2021 20:31:30 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:c4818cc3ef0783732a51706c2f08756aad823d8829e0cd0a3e0332606b2a5851
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.5 MB (9541696 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c46cfd47aedfb2dfd2d6ede8515150bcce95d109f4180ab8d4ab95055cca9b62`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 06 Aug 2021 17:39:26 GMT
ADD file:1a8fd1066485e1261462e689c1a072f010c1d3be904b73ef2b84128fac652951 in / 
# Fri, 06 Aug 2021 17:39:27 GMT
CMD ["/bin/sh"]
# Fri, 06 Aug 2021 19:51:42 GMT
ENV NATS_STREAMING_SERVER=0.22.1
# Fri, 06 Aug 2021 19:51:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='581698d248a19ecae64e4048d153bc1021744a3da6284680a339f9f82a53a9cf' ;; 		armhf) natsArch='arm6'; sha256='438a89221bb0608e40d21e73ca27a4b70b8560730726942c0ade94a6b6013d6f' ;; 		armv7) natsArch='arm7'; sha256='4164baadd201d1374f7654d3e54a24d81ceb87a385867e31a82c1d1a69e3b1ae' ;; 		x86_64) natsArch='amd64'; sha256='f29e87ac9ff998c928aa8ebc8cf0c4d04d34a3d95b9900d92fd7dafab2bec8cc' ;; 		x86) natsArch='386'; sha256='0ca68e57babb8901d7afeb7569042730904887e718ddf860ef3ee54278753505' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 06 Aug 2021 19:51:45 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Fri, 06 Aug 2021 19:51:45 GMT
EXPOSE 4222 8222
# Fri, 06 Aug 2021 19:51:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 06 Aug 2021 19:51:45 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:fd3acdcea5682abced546ec19fb6ebee725c5184e5d91614c469c0a79e67f2d0`  
		Last Modified: Fri, 06 Aug 2021 17:40:12 GMT  
		Size: 2.7 MB (2710613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0968d8a9e4506d1c6878a0b725fc7f4f449c0ddb3f88d3704902e19db206317`  
		Last Modified: Fri, 06 Aug 2021 19:52:37 GMT  
		Size: 6.8 MB (6830662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87ab8fb5390b1c71a899984eb600e99e2ad1526c1c22bc89d0f8f52e64af17aa`  
		Last Modified: Fri, 06 Aug 2021 19:52:35 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:alpine3.14`

```console
$ docker pull nats-streaming@sha256:e1479f281ad33982c8df81acee8d71d2049fe3535d7b1595adae6eeffd669c9e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:alpine3.14` - linux; amd64

```console
$ docker pull nats-streaming@sha256:b13c3888f620e128e2324e521a59ecdae8096c67f4448233afd380feafbf565e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.3 MB (10269210 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e299437f282dcf86645a5f6e5b3a8c7345ba0e4582e60b8b76b5c06d1b5d938`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 06 Aug 2021 17:19:45 GMT
ADD file:34eb5c40aa00028921a224d1764ae1b1f3ef710d191e4dfc7df55e0594aa7217 in / 
# Fri, 06 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Sat, 07 Aug 2021 00:08:04 GMT
ENV NATS_STREAMING_SERVER=0.22.1
# Sat, 07 Aug 2021 00:08:07 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='581698d248a19ecae64e4048d153bc1021744a3da6284680a339f9f82a53a9cf' ;; 		armhf) natsArch='arm6'; sha256='438a89221bb0608e40d21e73ca27a4b70b8560730726942c0ade94a6b6013d6f' ;; 		armv7) natsArch='arm7'; sha256='4164baadd201d1374f7654d3e54a24d81ceb87a385867e31a82c1d1a69e3b1ae' ;; 		x86_64) natsArch='amd64'; sha256='f29e87ac9ff998c928aa8ebc8cf0c4d04d34a3d95b9900d92fd7dafab2bec8cc' ;; 		x86) natsArch='386'; sha256='0ca68e57babb8901d7afeb7569042730904887e718ddf860ef3ee54278753505' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Sat, 07 Aug 2021 00:08:08 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Sat, 07 Aug 2021 00:08:08 GMT
EXPOSE 4222 8222
# Sat, 07 Aug 2021 00:08:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 07 Aug 2021 00:08:08 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:29291e31a76a7e560b9b7ad3cada56e8c18d50a96cca8a2573e4f4689d7aca77`  
		Last Modified: Thu, 05 Aug 2021 15:56:25 GMT  
		Size: 2.8 MB (2813006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ded93adf1b7cd7e872edc8b55f1b6f392ee0f39c43a12ea019e39c39818d7f8f`  
		Last Modified: Sat, 07 Aug 2021 00:08:56 GMT  
		Size: 7.5 MB (7455782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:146382f94f105a2b20528c00beadcfd4783e1a1485e43b55b9bdd33fe1be714f`  
		Last Modified: Sat, 07 Aug 2021 00:08:54 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine3.14` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:a6cf6a518fea52b3fc47ed4572652aa0e2350898b54cdbcc0f778150de352dbd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.6 MB (9559904 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c8b625df6f0e93de9095159d166249a43a96ef9f3013e4a2c483b5ac7bc972b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 06 Aug 2021 17:49:32 GMT
ADD file:7f2c7deda009eabdcbbdccb11e854043d32c498e64e7e1ca02165d7bb4261d39 in / 
# Fri, 06 Aug 2021 17:49:32 GMT
CMD ["/bin/sh"]
# Fri, 06 Aug 2021 18:59:05 GMT
ENV NATS_STREAMING_SERVER=0.22.1
# Fri, 06 Aug 2021 18:59:10 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='581698d248a19ecae64e4048d153bc1021744a3da6284680a339f9f82a53a9cf' ;; 		armhf) natsArch='arm6'; sha256='438a89221bb0608e40d21e73ca27a4b70b8560730726942c0ade94a6b6013d6f' ;; 		armv7) natsArch='arm7'; sha256='4164baadd201d1374f7654d3e54a24d81ceb87a385867e31a82c1d1a69e3b1ae' ;; 		x86_64) natsArch='amd64'; sha256='f29e87ac9ff998c928aa8ebc8cf0c4d04d34a3d95b9900d92fd7dafab2bec8cc' ;; 		x86) natsArch='386'; sha256='0ca68e57babb8901d7afeb7569042730904887e718ddf860ef3ee54278753505' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 06 Aug 2021 18:59:10 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Fri, 06 Aug 2021 18:59:11 GMT
EXPOSE 4222 8222
# Fri, 06 Aug 2021 18:59:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 06 Aug 2021 18:59:12 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:f465bb3e9fcd0c42f936ecc566c6e40353c00f3089b2b2c2ea1663c30f89d3ab`  
		Last Modified: Fri, 06 Aug 2021 17:51:00 GMT  
		Size: 2.6 MB (2626350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:719cf2771983cbb32331cc8915e2edce30fbcb308f3504276742ffc9a3bc35fd`  
		Last Modified: Fri, 06 Aug 2021 19:00:56 GMT  
		Size: 6.9 MB (6933133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a72de2e4e74462365f574ec07048641b834163995d6b95fb88af2fca27e01883`  
		Last Modified: Fri, 06 Aug 2021 19:00:52 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine3.14` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:7970395d00490fad62f2a51288db47d251cab92ec7634bef6de42343f8e8eedc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.4 MB (9351328 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e19086c92b47964c105a8ed130ff7219833adab1ca8e211c1ad0b0a049866252`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 06 Aug 2021 17:57:32 GMT
ADD file:3a35ff3ac0d80289d419a4d6d8319610c38e1936d296addafb9aaf506946230f in / 
# Fri, 06 Aug 2021 17:57:32 GMT
CMD ["/bin/sh"]
# Fri, 06 Aug 2021 20:29:42 GMT
ENV NATS_STREAMING_SERVER=0.22.1
# Fri, 06 Aug 2021 20:29:48 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='581698d248a19ecae64e4048d153bc1021744a3da6284680a339f9f82a53a9cf' ;; 		armhf) natsArch='arm6'; sha256='438a89221bb0608e40d21e73ca27a4b70b8560730726942c0ade94a6b6013d6f' ;; 		armv7) natsArch='arm7'; sha256='4164baadd201d1374f7654d3e54a24d81ceb87a385867e31a82c1d1a69e3b1ae' ;; 		x86_64) natsArch='amd64'; sha256='f29e87ac9ff998c928aa8ebc8cf0c4d04d34a3d95b9900d92fd7dafab2bec8cc' ;; 		x86) natsArch='386'; sha256='0ca68e57babb8901d7afeb7569042730904887e718ddf860ef3ee54278753505' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 06 Aug 2021 20:29:48 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Fri, 06 Aug 2021 20:29:49 GMT
EXPOSE 4222 8222
# Fri, 06 Aug 2021 20:29:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 06 Aug 2021 20:29:50 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:4ee0caa23b369b04827640a4be298bf4ff7bacd030c77e915f5d7fb8f987594a`  
		Last Modified: Fri, 06 Aug 2021 17:58:57 GMT  
		Size: 2.4 MB (2429359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e14712e6c4fbdd823f35d0df7aa1345088ce3d89727133dcef4adb1105ecb5f`  
		Last Modified: Fri, 06 Aug 2021 20:31:34 GMT  
		Size: 6.9 MB (6921548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e18c45098374f86d0784e7840a2c0fd15ce636edfee6d3ebc23432fd0cc47be5`  
		Last Modified: Fri, 06 Aug 2021 20:31:30 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine3.14` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:c4818cc3ef0783732a51706c2f08756aad823d8829e0cd0a3e0332606b2a5851
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.5 MB (9541696 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c46cfd47aedfb2dfd2d6ede8515150bcce95d109f4180ab8d4ab95055cca9b62`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 06 Aug 2021 17:39:26 GMT
ADD file:1a8fd1066485e1261462e689c1a072f010c1d3be904b73ef2b84128fac652951 in / 
# Fri, 06 Aug 2021 17:39:27 GMT
CMD ["/bin/sh"]
# Fri, 06 Aug 2021 19:51:42 GMT
ENV NATS_STREAMING_SERVER=0.22.1
# Fri, 06 Aug 2021 19:51:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='581698d248a19ecae64e4048d153bc1021744a3da6284680a339f9f82a53a9cf' ;; 		armhf) natsArch='arm6'; sha256='438a89221bb0608e40d21e73ca27a4b70b8560730726942c0ade94a6b6013d6f' ;; 		armv7) natsArch='arm7'; sha256='4164baadd201d1374f7654d3e54a24d81ceb87a385867e31a82c1d1a69e3b1ae' ;; 		x86_64) natsArch='amd64'; sha256='f29e87ac9ff998c928aa8ebc8cf0c4d04d34a3d95b9900d92fd7dafab2bec8cc' ;; 		x86) natsArch='386'; sha256='0ca68e57babb8901d7afeb7569042730904887e718ddf860ef3ee54278753505' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 06 Aug 2021 19:51:45 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Fri, 06 Aug 2021 19:51:45 GMT
EXPOSE 4222 8222
# Fri, 06 Aug 2021 19:51:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 06 Aug 2021 19:51:45 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:fd3acdcea5682abced546ec19fb6ebee725c5184e5d91614c469c0a79e67f2d0`  
		Last Modified: Fri, 06 Aug 2021 17:40:12 GMT  
		Size: 2.7 MB (2710613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0968d8a9e4506d1c6878a0b725fc7f4f449c0ddb3f88d3704902e19db206317`  
		Last Modified: Fri, 06 Aug 2021 19:52:37 GMT  
		Size: 6.8 MB (6830662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87ab8fb5390b1c71a899984eb600e99e2ad1526c1c22bc89d0f8f52e64af17aa`  
		Last Modified: Fri, 06 Aug 2021 19:52:35 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:latest`

```console
$ docker pull nats-streaming@sha256:390339ceba1628352f455fe424fe32e247d88ee68536deacd17fef6c85426ef3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.2114; amd64

### `nats-streaming:latest` - linux; amd64

```console
$ docker pull nats-streaming@sha256:3c6c9375f9e9724462e98cfb98a7abb50ceeca73b3070ce061992c4009e32157
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7168713 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:184d7920ac61dd2e84320b8040f57980a7d605d42948a520ede12d421168c4ce`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 02 Aug 2021 22:20:03 GMT
COPY file:ca9a212ccef327f9c2e91a62a908ac0cdbd39b08be331ea2b209c2d724942e18 in /nats-streaming-server 
# Mon, 02 Aug 2021 22:20:03 GMT
EXPOSE 4222 8222
# Mon, 02 Aug 2021 22:20:03 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 02 Aug 2021 22:20:03 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:f3749ab6cbfff03714b5a6a1245fa249b67d19e7358b74cbc50232b14370481a`  
		Last Modified: Mon, 02 Aug 2021 22:20:48 GMT  
		Size: 7.2 MB (7168713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:latest` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:e944d0e843d59d5979d7561c06b0c0adc874ceaa0bd34d3a7b536b25e8c9704d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.7 MB (6650246 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0146bbca3802c65d86e148b1d203b3d395ca1cd8a8bb89461888570d821dc4fb`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 02 Aug 2021 22:51:34 GMT
COPY file:68ac67d86d6ac617adc181feb43580415b7fc7640a3c7577bb3753c369908da0 in /nats-streaming-server 
# Mon, 02 Aug 2021 22:51:35 GMT
EXPOSE 4222 8222
# Mon, 02 Aug 2021 22:51:35 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 02 Aug 2021 22:51:35 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:c7e1d707b6179f690f3f44212cb8c9a3fe914d91d3f1ddbac9f176aa0610c90a`  
		Last Modified: Mon, 02 Aug 2021 22:53:32 GMT  
		Size: 6.7 MB (6650246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:latest` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:a5e3d56b343f9091f353634f59f688998544ccd4f2cbb80001d08ea6a3207274
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6639768 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80206ae32558812ad047d8ab67519615e98e7df68a884fc32b6d5fd8f72593b0`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 02 Aug 2021 23:11:17 GMT
COPY file:79708b5d249193a95e72c506453fd1ecd3e2738ec2ff3423c4b2bd760f426da2 in /nats-streaming-server 
# Mon, 02 Aug 2021 23:11:18 GMT
EXPOSE 4222 8222
# Mon, 02 Aug 2021 23:11:18 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 02 Aug 2021 23:11:19 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:52753762f751e166edd44e37a0ef0a06b33c337bdeb66e4134ee8479a49dae68`  
		Last Modified: Mon, 02 Aug 2021 23:13:17 GMT  
		Size: 6.6 MB (6639768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:latest` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:96652223cce95275138363a54affb8663ba46bc75831c2a9535375ab6d922143
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 MB (6546324 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:952bbd74028df1debbfe0e4665b514c66a36537d0868d41bc971ddb55793c442`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 02 Aug 2021 22:40:16 GMT
COPY file:a77d9769f43cc6943be482183091d3360eaadf93bf1ef5a67f0869d5555868a6 in /nats-streaming-server 
# Mon, 02 Aug 2021 22:40:17 GMT
EXPOSE 4222 8222
# Mon, 02 Aug 2021 22:40:17 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 02 Aug 2021 22:40:17 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4dc8aa7843ed2da454d59006acb180caee3f980d12034caacd4a32ffedab3df7`  
		Last Modified: Mon, 02 Aug 2021 22:41:24 GMT  
		Size: 6.5 MB (6546324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:latest` - windows version 10.0.17763.2114; amd64

```console
$ docker pull nats-streaming@sha256:8b058c3d2bf71043f26b6b58702562c13724bb5594ceebad3f49b4f539c3c227
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.0 MB (110039206 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:29bedda8d4d57688f52e1b97404c0dd1ecd0d7823e3f5e07a6f0214ee01d7853`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 05 Aug 2021 19:15:20 GMT
RUN Apply image 1809-amd64
# Wed, 11 Aug 2021 16:52:04 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 11 Aug 2021 21:19:29 GMT
RUN cmd /S /C #(nop) COPY file:9670e5d1fe5a71e47c78fde01235a0bcbcafcfdeeacf96a7669f6e49343fb03b in C:\nats-streaming-server.exe 
# Wed, 11 Aug 2021 21:19:33 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 11 Aug 2021 21:19:36 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 11 Aug 2021 21:19:39 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:bc8517709e9cfff223cb034ff5be8fcbfa5409de286cdac9ae1b8878ebea6b84`  
		Size: 102.7 MB (102741177 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3aa4a9dea1e2eabb29e2100fd699f3e3acbcabd85f360a3799b2505a5f74e5a0`  
		Last Modified: Wed, 11 Aug 2021 16:57:14 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2422c6b202cf35a718dc80ef76006199902c019414449d929f2538d72106be7`  
		Last Modified: Wed, 11 Aug 2021 21:24:43 GMT  
		Size: 7.3 MB (7293397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe1c9060adc003485accbb3848bb825c0b555a9e064d8ee4861937d781f4fb6d`  
		Last Modified: Wed, 11 Aug 2021 21:24:35 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eebb7419f921a924ca580e9c32580b82f2748e7759754b74686a3778fd920843`  
		Last Modified: Wed, 11 Aug 2021 21:24:35 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:413188a47dae1e13011a4e6d4ef5a31f5e680e350820d0b968981bc816827aaa`  
		Last Modified: Wed, 11 Aug 2021 21:24:35 GMT  
		Size: 1.2 KB (1174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:linux`

```console
$ docker pull nats-streaming@sha256:7d3a953263095ea9d7018d32bd3483577d512550bc7890ba7743f48963cce893
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:linux` - linux; amd64

```console
$ docker pull nats-streaming@sha256:3c6c9375f9e9724462e98cfb98a7abb50ceeca73b3070ce061992c4009e32157
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7168713 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:184d7920ac61dd2e84320b8040f57980a7d605d42948a520ede12d421168c4ce`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 02 Aug 2021 22:20:03 GMT
COPY file:ca9a212ccef327f9c2e91a62a908ac0cdbd39b08be331ea2b209c2d724942e18 in /nats-streaming-server 
# Mon, 02 Aug 2021 22:20:03 GMT
EXPOSE 4222 8222
# Mon, 02 Aug 2021 22:20:03 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 02 Aug 2021 22:20:03 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:f3749ab6cbfff03714b5a6a1245fa249b67d19e7358b74cbc50232b14370481a`  
		Last Modified: Mon, 02 Aug 2021 22:20:48 GMT  
		Size: 7.2 MB (7168713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:linux` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:e944d0e843d59d5979d7561c06b0c0adc874ceaa0bd34d3a7b536b25e8c9704d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.7 MB (6650246 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0146bbca3802c65d86e148b1d203b3d395ca1cd8a8bb89461888570d821dc4fb`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 02 Aug 2021 22:51:34 GMT
COPY file:68ac67d86d6ac617adc181feb43580415b7fc7640a3c7577bb3753c369908da0 in /nats-streaming-server 
# Mon, 02 Aug 2021 22:51:35 GMT
EXPOSE 4222 8222
# Mon, 02 Aug 2021 22:51:35 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 02 Aug 2021 22:51:35 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:c7e1d707b6179f690f3f44212cb8c9a3fe914d91d3f1ddbac9f176aa0610c90a`  
		Last Modified: Mon, 02 Aug 2021 22:53:32 GMT  
		Size: 6.7 MB (6650246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:linux` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:a5e3d56b343f9091f353634f59f688998544ccd4f2cbb80001d08ea6a3207274
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6639768 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80206ae32558812ad047d8ab67519615e98e7df68a884fc32b6d5fd8f72593b0`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 02 Aug 2021 23:11:17 GMT
COPY file:79708b5d249193a95e72c506453fd1ecd3e2738ec2ff3423c4b2bd760f426da2 in /nats-streaming-server 
# Mon, 02 Aug 2021 23:11:18 GMT
EXPOSE 4222 8222
# Mon, 02 Aug 2021 23:11:18 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 02 Aug 2021 23:11:19 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:52753762f751e166edd44e37a0ef0a06b33c337bdeb66e4134ee8479a49dae68`  
		Last Modified: Mon, 02 Aug 2021 23:13:17 GMT  
		Size: 6.6 MB (6639768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:linux` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:96652223cce95275138363a54affb8663ba46bc75831c2a9535375ab6d922143
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 MB (6546324 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:952bbd74028df1debbfe0e4665b514c66a36537d0868d41bc971ddb55793c442`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 02 Aug 2021 22:40:16 GMT
COPY file:a77d9769f43cc6943be482183091d3360eaadf93bf1ef5a67f0869d5555868a6 in /nats-streaming-server 
# Mon, 02 Aug 2021 22:40:17 GMT
EXPOSE 4222 8222
# Mon, 02 Aug 2021 22:40:17 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 02 Aug 2021 22:40:17 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4dc8aa7843ed2da454d59006acb180caee3f980d12034caacd4a32ffedab3df7`  
		Last Modified: Mon, 02 Aug 2021 22:41:24 GMT  
		Size: 6.5 MB (6546324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:nanoserver`

```console
$ docker pull nats-streaming@sha256:8407af82564828d613edb1e65aedfa7d022699303898c4c33b02f71106e85700
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2114; amd64

### `nats-streaming:nanoserver` - windows version 10.0.17763.2114; amd64

```console
$ docker pull nats-streaming@sha256:8b058c3d2bf71043f26b6b58702562c13724bb5594ceebad3f49b4f539c3c227
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.0 MB (110039206 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:29bedda8d4d57688f52e1b97404c0dd1ecd0d7823e3f5e07a6f0214ee01d7853`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 05 Aug 2021 19:15:20 GMT
RUN Apply image 1809-amd64
# Wed, 11 Aug 2021 16:52:04 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 11 Aug 2021 21:19:29 GMT
RUN cmd /S /C #(nop) COPY file:9670e5d1fe5a71e47c78fde01235a0bcbcafcfdeeacf96a7669f6e49343fb03b in C:\nats-streaming-server.exe 
# Wed, 11 Aug 2021 21:19:33 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 11 Aug 2021 21:19:36 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 11 Aug 2021 21:19:39 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:bc8517709e9cfff223cb034ff5be8fcbfa5409de286cdac9ae1b8878ebea6b84`  
		Size: 102.7 MB (102741177 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3aa4a9dea1e2eabb29e2100fd699f3e3acbcabd85f360a3799b2505a5f74e5a0`  
		Last Modified: Wed, 11 Aug 2021 16:57:14 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2422c6b202cf35a718dc80ef76006199902c019414449d929f2538d72106be7`  
		Last Modified: Wed, 11 Aug 2021 21:24:43 GMT  
		Size: 7.3 MB (7293397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe1c9060adc003485accbb3848bb825c0b555a9e064d8ee4861937d781f4fb6d`  
		Last Modified: Wed, 11 Aug 2021 21:24:35 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eebb7419f921a924ca580e9c32580b82f2748e7759754b74686a3778fd920843`  
		Last Modified: Wed, 11 Aug 2021 21:24:35 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:413188a47dae1e13011a4e6d4ef5a31f5e680e350820d0b968981bc816827aaa`  
		Last Modified: Wed, 11 Aug 2021 21:24:35 GMT  
		Size: 1.2 KB (1174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:nanoserver-1809`

```console
$ docker pull nats-streaming@sha256:8407af82564828d613edb1e65aedfa7d022699303898c4c33b02f71106e85700
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2114; amd64

### `nats-streaming:nanoserver-1809` - windows version 10.0.17763.2114; amd64

```console
$ docker pull nats-streaming@sha256:8b058c3d2bf71043f26b6b58702562c13724bb5594ceebad3f49b4f539c3c227
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.0 MB (110039206 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:29bedda8d4d57688f52e1b97404c0dd1ecd0d7823e3f5e07a6f0214ee01d7853`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 05 Aug 2021 19:15:20 GMT
RUN Apply image 1809-amd64
# Wed, 11 Aug 2021 16:52:04 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 11 Aug 2021 21:19:29 GMT
RUN cmd /S /C #(nop) COPY file:9670e5d1fe5a71e47c78fde01235a0bcbcafcfdeeacf96a7669f6e49343fb03b in C:\nats-streaming-server.exe 
# Wed, 11 Aug 2021 21:19:33 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 11 Aug 2021 21:19:36 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 11 Aug 2021 21:19:39 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:bc8517709e9cfff223cb034ff5be8fcbfa5409de286cdac9ae1b8878ebea6b84`  
		Size: 102.7 MB (102741177 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3aa4a9dea1e2eabb29e2100fd699f3e3acbcabd85f360a3799b2505a5f74e5a0`  
		Last Modified: Wed, 11 Aug 2021 16:57:14 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2422c6b202cf35a718dc80ef76006199902c019414449d929f2538d72106be7`  
		Last Modified: Wed, 11 Aug 2021 21:24:43 GMT  
		Size: 7.3 MB (7293397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe1c9060adc003485accbb3848bb825c0b555a9e064d8ee4861937d781f4fb6d`  
		Last Modified: Wed, 11 Aug 2021 21:24:35 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eebb7419f921a924ca580e9c32580b82f2748e7759754b74686a3778fd920843`  
		Last Modified: Wed, 11 Aug 2021 21:24:35 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:413188a47dae1e13011a4e6d4ef5a31f5e680e350820d0b968981bc816827aaa`  
		Last Modified: Wed, 11 Aug 2021 21:24:35 GMT  
		Size: 1.2 KB (1174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:scratch`

```console
$ docker pull nats-streaming@sha256:7d3a953263095ea9d7018d32bd3483577d512550bc7890ba7743f48963cce893
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:scratch` - linux; amd64

```console
$ docker pull nats-streaming@sha256:3c6c9375f9e9724462e98cfb98a7abb50ceeca73b3070ce061992c4009e32157
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7168713 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:184d7920ac61dd2e84320b8040f57980a7d605d42948a520ede12d421168c4ce`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 02 Aug 2021 22:20:03 GMT
COPY file:ca9a212ccef327f9c2e91a62a908ac0cdbd39b08be331ea2b209c2d724942e18 in /nats-streaming-server 
# Mon, 02 Aug 2021 22:20:03 GMT
EXPOSE 4222 8222
# Mon, 02 Aug 2021 22:20:03 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 02 Aug 2021 22:20:03 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:f3749ab6cbfff03714b5a6a1245fa249b67d19e7358b74cbc50232b14370481a`  
		Last Modified: Mon, 02 Aug 2021 22:20:48 GMT  
		Size: 7.2 MB (7168713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:scratch` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:e944d0e843d59d5979d7561c06b0c0adc874ceaa0bd34d3a7b536b25e8c9704d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.7 MB (6650246 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0146bbca3802c65d86e148b1d203b3d395ca1cd8a8bb89461888570d821dc4fb`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 02 Aug 2021 22:51:34 GMT
COPY file:68ac67d86d6ac617adc181feb43580415b7fc7640a3c7577bb3753c369908da0 in /nats-streaming-server 
# Mon, 02 Aug 2021 22:51:35 GMT
EXPOSE 4222 8222
# Mon, 02 Aug 2021 22:51:35 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 02 Aug 2021 22:51:35 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:c7e1d707b6179f690f3f44212cb8c9a3fe914d91d3f1ddbac9f176aa0610c90a`  
		Last Modified: Mon, 02 Aug 2021 22:53:32 GMT  
		Size: 6.7 MB (6650246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:scratch` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:a5e3d56b343f9091f353634f59f688998544ccd4f2cbb80001d08ea6a3207274
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6639768 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80206ae32558812ad047d8ab67519615e98e7df68a884fc32b6d5fd8f72593b0`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 02 Aug 2021 23:11:17 GMT
COPY file:79708b5d249193a95e72c506453fd1ecd3e2738ec2ff3423c4b2bd760f426da2 in /nats-streaming-server 
# Mon, 02 Aug 2021 23:11:18 GMT
EXPOSE 4222 8222
# Mon, 02 Aug 2021 23:11:18 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 02 Aug 2021 23:11:19 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:52753762f751e166edd44e37a0ef0a06b33c337bdeb66e4134ee8479a49dae68`  
		Last Modified: Mon, 02 Aug 2021 23:13:17 GMT  
		Size: 6.6 MB (6639768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:scratch` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:96652223cce95275138363a54affb8663ba46bc75831c2a9535375ab6d922143
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 MB (6546324 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:952bbd74028df1debbfe0e4665b514c66a36537d0868d41bc971ddb55793c442`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 02 Aug 2021 22:40:16 GMT
COPY file:a77d9769f43cc6943be482183091d3360eaadf93bf1ef5a67f0869d5555868a6 in /nats-streaming-server 
# Mon, 02 Aug 2021 22:40:17 GMT
EXPOSE 4222 8222
# Mon, 02 Aug 2021 22:40:17 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 02 Aug 2021 22:40:17 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4dc8aa7843ed2da454d59006acb180caee3f980d12034caacd4a32ffedab3df7`  
		Last Modified: Mon, 02 Aug 2021 22:41:24 GMT  
		Size: 6.5 MB (6546324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:windowsservercore`

```console
$ docker pull nats-streaming@sha256:5f9e88c929ff89c3204d105008a059f9be67f540ff96b5bfec99e3b254351411
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.2114; amd64
	-	windows version 10.0.14393.4583; amd64

### `nats-streaming:windowsservercore` - windows version 10.0.17763.2114; amd64

```console
$ docker pull nats-streaming@sha256:75b04016fe1b2f4c6a7bef238c62f6610c86ab0baed8d1031b7f061053987a27
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2693987543 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ffc0c1be51519eff598c2d5cce32f011fcfe27c06a9651541cec6796f3f66a56`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 05 Aug 2021 19:44:34 GMT
RUN Install update 1809-amd64
# Wed, 11 Aug 2021 13:42:12 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 11 Aug 2021 16:48:51 GMT
ENV NATS_DOCKERIZED=1
# Wed, 11 Aug 2021 21:16:00 GMT
ENV NATS_STREAMING_SERVER=0.22.1
# Wed, 11 Aug 2021 21:16:03 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.22.1/nats-streaming-server-v0.22.1-windows-amd64.zip
# Wed, 11 Aug 2021 21:16:06 GMT
ENV NATS_STREAMING_SERVER_SHASUM=4516852b493111b73ec06477be4a27e66f5abc9ca1ff4dd2b970232271611264
# Wed, 11 Aug 2021 21:17:09 GMT
RUN Set-PSDebug -Trace 2
# Wed, 11 Aug 2021 21:19:07 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 11 Aug 2021 21:19:10 GMT
EXPOSE 4222 8222
# Wed, 11 Aug 2021 21:19:13 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 11 Aug 2021 21:19:15 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c67ded6868b61d392a0c096f911563fd6bc0bc3ed4fe401d077b3718a1b0cdaf`  
		Size: 967.7 MB (967665054 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c613f4c34660a122de754415a884afe6b12172ac3ce792a2e4aae831cc8b2e27`  
		Last Modified: Wed, 11 Aug 2021 16:25:11 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71d8e65d39d1b09c34e0dadad1a6b7818f430fb13ce2ff8d70c549b137f9131a`  
		Last Modified: Wed, 11 Aug 2021 16:56:54 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f48fea2e101940ffa36628a8fd4da200aa97417773d993be6df74d0bcff8dccc`  
		Last Modified: Wed, 11 Aug 2021 21:24:22 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bd10110cd94f48fce072addebc384215cfee9e902098952b29a44227fc4c19b`  
		Last Modified: Wed, 11 Aug 2021 21:24:22 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f32d77caa28f59168738bee8473e7e58d117ce711f59589f9627b0facfe620bd`  
		Last Modified: Wed, 11 Aug 2021 21:24:22 GMT  
		Size: 1.4 KB (1443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90f9d42ecbcdc48ff53122318c96640c628d9f2b33df84c887b89a1b1429091e`  
		Last Modified: Wed, 11 Aug 2021 21:24:19 GMT  
		Size: 351.7 KB (351714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfe2bf098cd0e80bd3e81951fb0f411238d63d458bcd51ecd3427a1566fd0ffc`  
		Last Modified: Wed, 11 Aug 2021 21:24:21 GMT  
		Size: 7.6 MB (7626528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e710a2acda7795374f6c855a7d81c6156b961c06f5b0f13fd31e2d8c4952fd6`  
		Last Modified: Wed, 11 Aug 2021 21:24:19 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2333773eafb1bb6c7fd6fd55fd31614ec447f3b1af48b5f63fe1ee29a4093ff2`  
		Last Modified: Wed, 11 Aug 2021 21:24:19 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:666623a49ff4c5032408abc00ae56261476eed8930351412760fedada9e6e136`  
		Last Modified: Wed, 11 Aug 2021 21:24:19 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:windowsservercore` - windows version 10.0.14393.4583; amd64

```console
$ docker pull nats-streaming@sha256:c2dc8bad14a0594eb6483398e8aa5f20933884855abece46d39a9aaa5ff6c0de
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6283441295 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d4dcfbb00a058925aa22ae213359605c8892f3261a0afdd6941153ff9789f841`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Sun, 01 Aug 2021 08:52:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 11 Aug 2021 13:57:45 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 11 Aug 2021 16:52:27 GMT
ENV NATS_DOCKERIZED=1
# Wed, 11 Aug 2021 21:19:47 GMT
ENV NATS_STREAMING_SERVER=0.22.1
# Wed, 11 Aug 2021 21:19:50 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.22.1/nats-streaming-server-v0.22.1-windows-amd64.zip
# Wed, 11 Aug 2021 21:19:53 GMT
ENV NATS_STREAMING_SERVER_SHASUM=4516852b493111b73ec06477be4a27e66f5abc9ca1ff4dd2b970232271611264
# Wed, 11 Aug 2021 21:21:16 GMT
RUN Set-PSDebug -Trace 2
# Wed, 11 Aug 2021 21:23:38 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 11 Aug 2021 21:23:41 GMT
EXPOSE 4222 8222
# Wed, 11 Aug 2021 21:23:43 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 11 Aug 2021 21:23:46 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c427f892fe74603ae09d4e49b25f8f7046f957054034dc9f462e0e88d7bffaa5`  
		Size: 2.2 GB (2200980134 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d6d4b60a6f3b0544427c2eb9a5e27e5f6ddca0fd7632003e11331f01c4e9c6fc`  
		Last Modified: Wed, 11 Aug 2021 16:25:34 GMT  
		Size: 1.4 KB (1442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe49d3a206649779952cc6a03fdbb4e828336501708ad40c4e1a07237199e28b`  
		Last Modified: Wed, 11 Aug 2021 16:57:38 GMT  
		Size: 1.4 KB (1380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e6e2dfe14e85c8398dc3f7c7906fb1f7c777ef6d5717fe70d978ad05718ffc2`  
		Last Modified: Wed, 11 Aug 2021 21:24:59 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f846ec4e42dc3dac55d428bcb2d57cab68f2b659b2cdbba1cad2800b22496145`  
		Last Modified: Wed, 11 Aug 2021 21:24:59 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a073e823edff403699ab0d2dff8376e1b0fb57af79842af3133c0b0c0e3c77f0`  
		Last Modified: Wed, 11 Aug 2021 21:24:59 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bedf8cee66f4f7e59aee0a000c7fe523b2994d8d7f358c994942fb8b6a9ae6c`  
		Last Modified: Wed, 11 Aug 2021 21:24:57 GMT  
		Size: 338.6 KB (338573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:275d8c5f6fbce1b85b62d1f70554f8ecf9d3ccdbfe54c86356703cc697b71e2b`  
		Last Modified: Wed, 11 Aug 2021 21:24:59 GMT  
		Size: 12.1 MB (12125382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b86e3ac00ba61bf48479b43167f3550a6c8ed7af7da7dd5c0b86441e7d8f662`  
		Last Modified: Wed, 11 Aug 2021 21:24:56 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f45154e30184ba145c5239532f29c91a714e1e6be10588ab43f2dfc69986775e`  
		Last Modified: Wed, 11 Aug 2021 21:24:56 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:254423fab1337576ad61d5fdd3942f86d494a694b38f8c0f779f9239789684b3`  
		Last Modified: Wed, 11 Aug 2021 21:24:56 GMT  
		Size: 1.4 KB (1443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:windowsservercore-1809`

```console
$ docker pull nats-streaming@sha256:17e69850495ccb3a8a86278c37ad940698ed0da3f3c08f6de694456dbb989c25
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2114; amd64

### `nats-streaming:windowsservercore-1809` - windows version 10.0.17763.2114; amd64

```console
$ docker pull nats-streaming@sha256:75b04016fe1b2f4c6a7bef238c62f6610c86ab0baed8d1031b7f061053987a27
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2693987543 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ffc0c1be51519eff598c2d5cce32f011fcfe27c06a9651541cec6796f3f66a56`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 05 Aug 2021 19:44:34 GMT
RUN Install update 1809-amd64
# Wed, 11 Aug 2021 13:42:12 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 11 Aug 2021 16:48:51 GMT
ENV NATS_DOCKERIZED=1
# Wed, 11 Aug 2021 21:16:00 GMT
ENV NATS_STREAMING_SERVER=0.22.1
# Wed, 11 Aug 2021 21:16:03 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.22.1/nats-streaming-server-v0.22.1-windows-amd64.zip
# Wed, 11 Aug 2021 21:16:06 GMT
ENV NATS_STREAMING_SERVER_SHASUM=4516852b493111b73ec06477be4a27e66f5abc9ca1ff4dd2b970232271611264
# Wed, 11 Aug 2021 21:17:09 GMT
RUN Set-PSDebug -Trace 2
# Wed, 11 Aug 2021 21:19:07 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 11 Aug 2021 21:19:10 GMT
EXPOSE 4222 8222
# Wed, 11 Aug 2021 21:19:13 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 11 Aug 2021 21:19:15 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c67ded6868b61d392a0c096f911563fd6bc0bc3ed4fe401d077b3718a1b0cdaf`  
		Size: 967.7 MB (967665054 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c613f4c34660a122de754415a884afe6b12172ac3ce792a2e4aae831cc8b2e27`  
		Last Modified: Wed, 11 Aug 2021 16:25:11 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71d8e65d39d1b09c34e0dadad1a6b7818f430fb13ce2ff8d70c549b137f9131a`  
		Last Modified: Wed, 11 Aug 2021 16:56:54 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f48fea2e101940ffa36628a8fd4da200aa97417773d993be6df74d0bcff8dccc`  
		Last Modified: Wed, 11 Aug 2021 21:24:22 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bd10110cd94f48fce072addebc384215cfee9e902098952b29a44227fc4c19b`  
		Last Modified: Wed, 11 Aug 2021 21:24:22 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f32d77caa28f59168738bee8473e7e58d117ce711f59589f9627b0facfe620bd`  
		Last Modified: Wed, 11 Aug 2021 21:24:22 GMT  
		Size: 1.4 KB (1443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90f9d42ecbcdc48ff53122318c96640c628d9f2b33df84c887b89a1b1429091e`  
		Last Modified: Wed, 11 Aug 2021 21:24:19 GMT  
		Size: 351.7 KB (351714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfe2bf098cd0e80bd3e81951fb0f411238d63d458bcd51ecd3427a1566fd0ffc`  
		Last Modified: Wed, 11 Aug 2021 21:24:21 GMT  
		Size: 7.6 MB (7626528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e710a2acda7795374f6c855a7d81c6156b961c06f5b0f13fd31e2d8c4952fd6`  
		Last Modified: Wed, 11 Aug 2021 21:24:19 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2333773eafb1bb6c7fd6fd55fd31614ec447f3b1af48b5f63fe1ee29a4093ff2`  
		Last Modified: Wed, 11 Aug 2021 21:24:19 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:666623a49ff4c5032408abc00ae56261476eed8930351412760fedada9e6e136`  
		Last Modified: Wed, 11 Aug 2021 21:24:19 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:windowsservercore-ltsc2016`

```console
$ docker pull nats-streaming@sha256:9cfea454a5d6b43341f213ae8515bf3ccf36487967fc16fad686bd3bed667681
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.14393.4583; amd64

### `nats-streaming:windowsservercore-ltsc2016` - windows version 10.0.14393.4583; amd64

```console
$ docker pull nats-streaming@sha256:c2dc8bad14a0594eb6483398e8aa5f20933884855abece46d39a9aaa5ff6c0de
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6283441295 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d4dcfbb00a058925aa22ae213359605c8892f3261a0afdd6941153ff9789f841`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Sun, 01 Aug 2021 08:52:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 11 Aug 2021 13:57:45 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 11 Aug 2021 16:52:27 GMT
ENV NATS_DOCKERIZED=1
# Wed, 11 Aug 2021 21:19:47 GMT
ENV NATS_STREAMING_SERVER=0.22.1
# Wed, 11 Aug 2021 21:19:50 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.22.1/nats-streaming-server-v0.22.1-windows-amd64.zip
# Wed, 11 Aug 2021 21:19:53 GMT
ENV NATS_STREAMING_SERVER_SHASUM=4516852b493111b73ec06477be4a27e66f5abc9ca1ff4dd2b970232271611264
# Wed, 11 Aug 2021 21:21:16 GMT
RUN Set-PSDebug -Trace 2
# Wed, 11 Aug 2021 21:23:38 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 11 Aug 2021 21:23:41 GMT
EXPOSE 4222 8222
# Wed, 11 Aug 2021 21:23:43 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 11 Aug 2021 21:23:46 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c427f892fe74603ae09d4e49b25f8f7046f957054034dc9f462e0e88d7bffaa5`  
		Size: 2.2 GB (2200980134 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d6d4b60a6f3b0544427c2eb9a5e27e5f6ddca0fd7632003e11331f01c4e9c6fc`  
		Last Modified: Wed, 11 Aug 2021 16:25:34 GMT  
		Size: 1.4 KB (1442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe49d3a206649779952cc6a03fdbb4e828336501708ad40c4e1a07237199e28b`  
		Last Modified: Wed, 11 Aug 2021 16:57:38 GMT  
		Size: 1.4 KB (1380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e6e2dfe14e85c8398dc3f7c7906fb1f7c777ef6d5717fe70d978ad05718ffc2`  
		Last Modified: Wed, 11 Aug 2021 21:24:59 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f846ec4e42dc3dac55d428bcb2d57cab68f2b659b2cdbba1cad2800b22496145`  
		Last Modified: Wed, 11 Aug 2021 21:24:59 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a073e823edff403699ab0d2dff8376e1b0fb57af79842af3133c0b0c0e3c77f0`  
		Last Modified: Wed, 11 Aug 2021 21:24:59 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bedf8cee66f4f7e59aee0a000c7fe523b2994d8d7f358c994942fb8b6a9ae6c`  
		Last Modified: Wed, 11 Aug 2021 21:24:57 GMT  
		Size: 338.6 KB (338573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:275d8c5f6fbce1b85b62d1f70554f8ecf9d3ccdbfe54c86356703cc697b71e2b`  
		Last Modified: Wed, 11 Aug 2021 21:24:59 GMT  
		Size: 12.1 MB (12125382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b86e3ac00ba61bf48479b43167f3550a6c8ed7af7da7dd5c0b86441e7d8f662`  
		Last Modified: Wed, 11 Aug 2021 21:24:56 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f45154e30184ba145c5239532f29c91a714e1e6be10588ab43f2dfc69986775e`  
		Last Modified: Wed, 11 Aug 2021 21:24:56 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:254423fab1337576ad61d5fdd3942f86d494a694b38f8c0f779f9239789684b3`  
		Last Modified: Wed, 11 Aug 2021 21:24:56 GMT  
		Size: 1.4 KB (1443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
