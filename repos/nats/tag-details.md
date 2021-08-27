<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `nats`

-	[`nats:2`](#nats2)
-	[`nats:2-alpine`](#nats2-alpine)
-	[`nats:2-alpine3.14`](#nats2-alpine314)
-	[`nats:2-linux`](#nats2-linux)
-	[`nats:2-nanoserver`](#nats2-nanoserver)
-	[`nats:2-nanoserver-1809`](#nats2-nanoserver-1809)
-	[`nats:2-scratch`](#nats2-scratch)
-	[`nats:2-windowsservercore`](#nats2-windowsservercore)
-	[`nats:2-windowsservercore-1809`](#nats2-windowsservercore-1809)
-	[`nats:2-windowsservercore-ltsc2016`](#nats2-windowsservercore-ltsc2016)
-	[`nats:2.4`](#nats24)
-	[`nats:2.4-alpine`](#nats24-alpine)
-	[`nats:2.4-alpine3.14`](#nats24-alpine314)
-	[`nats:2.4-linux`](#nats24-linux)
-	[`nats:2.4-nanoserver`](#nats24-nanoserver)
-	[`nats:2.4-nanoserver-1809`](#nats24-nanoserver-1809)
-	[`nats:2.4-scratch`](#nats24-scratch)
-	[`nats:2.4-windowsservercore`](#nats24-windowsservercore)
-	[`nats:2.4-windowsservercore-1809`](#nats24-windowsservercore-1809)
-	[`nats:2.4-windowsservercore-ltsc2016`](#nats24-windowsservercore-ltsc2016)
-	[`nats:2.4.0`](#nats240)
-	[`nats:2.4.0-alpine`](#nats240-alpine)
-	[`nats:2.4.0-alpine3.14`](#nats240-alpine314)
-	[`nats:2.4.0-linux`](#nats240-linux)
-	[`nats:2.4.0-nanoserver`](#nats240-nanoserver)
-	[`nats:2.4.0-nanoserver-1809`](#nats240-nanoserver-1809)
-	[`nats:2.4.0-scratch`](#nats240-scratch)
-	[`nats:2.4.0-windowsservercore`](#nats240-windowsservercore)
-	[`nats:2.4.0-windowsservercore-1809`](#nats240-windowsservercore-1809)
-	[`nats:2.4.0-windowsservercore-ltsc2016`](#nats240-windowsservercore-ltsc2016)
-	[`nats:alpine`](#natsalpine)
-	[`nats:alpine3.14`](#natsalpine314)
-	[`nats:latest`](#natslatest)
-	[`nats:linux`](#natslinux)
-	[`nats:nanoserver`](#natsnanoserver)
-	[`nats:nanoserver-1809`](#natsnanoserver-1809)
-	[`nats:scratch`](#natsscratch)
-	[`nats:windowsservercore`](#natswindowsservercore)
-	[`nats:windowsservercore-1809`](#natswindowsservercore-1809)
-	[`nats:windowsservercore-ltsc2016`](#natswindowsservercore-ltsc2016)

## `nats:2`

```console
$ docker pull nats@sha256:f00cc850e92427d4fc02e7090a743e9044f62755a8b06ab733ff88b8d5ff0562
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.2114; amd64

### `nats:2` - linux; amd64

```console
$ docker pull nats@sha256:acd926de12a3d1a625d13dfab262fa240b0d99ecb35c68e372e093ab466d1b0b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4506461 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5738e29b3f24028140a48fe9652afc26b4118a35427b996d591872c6dd9162ed`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 05 Aug 2021 01:20:24 GMT
COPY file:edd123fab471ca4bff1ec55ddc839aaf0defe3667b337aaec7c3c8e70e903e8d in /nats-server 
# Thu, 05 Aug 2021 01:20:24 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 05 Aug 2021 01:20:24 GMT
EXPOSE 4222 6222 8222
# Thu, 05 Aug 2021 01:20:24 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 05 Aug 2021 01:20:25 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3d02ec701f9917abde1e8953cba96577f89ebc29ced1af0d82734bde1a034361`  
		Last Modified: Thu, 05 Aug 2021 01:21:15 GMT  
		Size: 4.5 MB (4505985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6beb29f4b4e73a454d8e38755b89ed0a71bb2f1aaaaa02105c3708af114c87cc`  
		Last Modified: Thu, 05 Aug 2021 01:21:14 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - linux; arm variant v6

```console
$ docker pull nats@sha256:7201c8cd794776fa392c3a25eb89e4ee987aeaaae647caa364621d5daf5ca3c5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4201703 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc2211a135c8d5c9641c74ba5d54c3c1df4ac3f24fa70a6a57be8a2975af7854`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 02:48:56 GMT
COPY file:81d7dcb1f2223ae767ee02f3b24758797ca55a665d17dcb2054eeb097fb2eafa in /nats-server 
# Fri, 27 Aug 2021 02:48:56 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 27 Aug 2021 02:48:57 GMT
EXPOSE 4222 6222 8222
# Fri, 27 Aug 2021 02:48:57 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 27 Aug 2021 02:48:58 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a820d11a96d84195887c44533ffcad67997fcb79d52f4564709bfdbde47d578d`  
		Last Modified: Fri, 27 Aug 2021 02:51:18 GMT  
		Size: 4.2 MB (4201229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a1c4f82bf849dc3d9d18f1c560b9afd0e5237eb2f05377e6792dda2480249cb`  
		Last Modified: Fri, 27 Aug 2021 02:51:15 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - linux; arm variant v7

```console
$ docker pull nats@sha256:edbf04c6d86cc6973609fb90c099c175ba05216954d224ea93c03e862b6c0955
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4170312 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:59d59f3755a610c7ef37ce7df6d7e2a6c1a1e7e0554fd7f0dfe5a7ba96370e6f`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 05 Aug 2021 01:04:56 GMT
COPY file:f8d5a2ea993b24151d26b5967a44af43f6fa70afe6b7965767ebb48f41351935 in /nats-server 
# Thu, 05 Aug 2021 01:04:57 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 05 Aug 2021 01:04:57 GMT
EXPOSE 4222 6222 8222
# Thu, 05 Aug 2021 01:04:58 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 05 Aug 2021 01:04:58 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:0b65416c95f5f06a582f3d8ffe3f3cc9b4df10e5d724eb5167d7766bce64b77e`  
		Last Modified: Thu, 05 Aug 2021 01:07:22 GMT  
		Size: 4.2 MB (4169837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:711811fab377fd6c12391460fafc4fe011d419669f5508b086b269489ae78d22`  
		Last Modified: Thu, 05 Aug 2021 01:07:20 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:258407bfd157b748b13d824daa441eeb795b46dae0dee509189e6f215219dfc4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.1 MB (4121540 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:928fc611a3e5935a6eea2e73e72cfc121d250a608f1def1e50e9a2bca5e9e0c4`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 05 Aug 2021 01:39:59 GMT
COPY file:e2687e43e0f0627dcdfb73c8b9b66c9a86cdda6399f627b485911acbece9a3c9 in /nats-server 
# Thu, 05 Aug 2021 01:40:00 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 05 Aug 2021 01:40:00 GMT
EXPOSE 4222 6222 8222
# Thu, 05 Aug 2021 01:40:00 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 05 Aug 2021 01:40:00 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:333cb9b408ea509452b14ed5b1c9a8a6abed86e5a3177bc9ae7917d6c0c51318`  
		Last Modified: Thu, 05 Aug 2021 01:41:23 GMT  
		Size: 4.1 MB (4121065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b79f5ac7bd31304ad5fab87a7bb25e67ff6f7e8f0299806180b5bb556ea0dc9`  
		Last Modified: Thu, 05 Aug 2021 01:41:22 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - windows version 10.0.17763.2114; amd64

```console
$ docker pull nats@sha256:9c370308b1924738df19dd502a9d8d8c13066580fd1550eddbf4f70663c87fe5
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.3 MB (107338949 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e90920ed24cf8337e7f99fdd7199bff8ec7dd43cfa5063f0f373e6700f8a17a2`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 05 Aug 2021 19:15:20 GMT
RUN Apply image 1809-amd64
# Wed, 25 Aug 2021 16:07:56 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 27 Aug 2021 00:16:45 GMT
RUN cmd /S /C #(nop) COPY file:bafd3fc1559b39648f01fab1b3b19a9fc9bb95afae5b07b1d7987b376806e053 in C:\nats-server.exe 
# Fri, 27 Aug 2021 00:16:46 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 27 Aug 2021 00:16:47 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Fri, 27 Aug 2021 00:16:47 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 27 Aug 2021 00:16:48 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:bc8517709e9cfff223cb034ff5be8fcbfa5409de286cdac9ae1b8878ebea6b84`  
		Size: 102.7 MB (102741177 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ae8616c17f5cca409a4b1289387e37dc532657ba2b52bb60713ff621acccd506`  
		Last Modified: Wed, 25 Aug 2021 16:11:20 GMT  
		Size: 1.0 KB (1022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb815244c76bae445a6697a3f1b6a0643fc016be2b2da5192dc6bb4079cd0119`  
		Last Modified: Fri, 27 Aug 2021 00:20:21 GMT  
		Size: 4.6 MB (4591622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c33193ffa3c81a2ebd95cb6af96ce80ee557191a64ba47e1977479e1167530ca`  
		Last Modified: Fri, 27 Aug 2021 00:20:19 GMT  
		Size: 1.7 KB (1701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c57e2e68d87e03a37f706b01fe403fc34435b82da71d1080e11ec9df4d418a2`  
		Last Modified: Fri, 27 Aug 2021 00:20:19 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:048b1707f600e77fb06d48bd9c3759cad471944658bdfa3dd59b2852dc7983b4`  
		Last Modified: Fri, 27 Aug 2021 00:20:20 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b434e68e7546ed285144b98ef8fc3a10f1b6ee578ef2503e9f09aefab0370d0`  
		Last Modified: Fri, 27 Aug 2021 00:20:20 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-alpine`

```console
$ docker pull nats@sha256:45faf7fef5f78d815f712b8a05a2a0ded8793d777a0fb7640b0b0e6ff58e0009
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-alpine` - linux; amd64

```console
$ docker pull nats@sha256:7a1ec46ffffcc712a37d5e801e73e4cb68b22e15c842f36ab9211e1a039cb547
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7603979 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:163732450f029c457fb0826ccdbb6d69696f0d8af625ed2bef5291b807563c38`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 06 Aug 2021 17:19:45 GMT
ADD file:34eb5c40aa00028921a224d1764ae1b1f3ef710d191e4dfc7df55e0594aa7217 in / 
# Fri, 06 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Sat, 07 Aug 2021 00:12:56 GMT
ENV NATS_SERVER=2.3.4
# Sat, 07 Aug 2021 00:12:58 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='c8ba676a6c4ec9d3088e0b64ffdae36e2f2a9e1b89f030799f3efbb2923524a0' ;; 		armhf) natsArch='arm6'; sha256='d1f14441d1fbd53a7bff9623e8e572707d3e7024b42b6e925ad371d4dec0bc47' ;; 		armv7) natsArch='arm7'; sha256='2488706de91e94eba477ddbc3b293ec0b4d823509656cc101eec6a07e0319bb5' ;; 		x86_64) natsArch='amd64'; sha256='8c11abdeca4882888a8b6fbc45effe9fb4d1070eda3939b7299892c8c69a3e87' ;; 		x86) natsArch='386'; sha256='010bca73095d8a05495ef74a112dfd3919925b0ced10bc4c5f876f3858ca41f7' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Sat, 07 Aug 2021 00:12:59 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Sat, 07 Aug 2021 00:12:59 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Sat, 07 Aug 2021 00:12:59 GMT
EXPOSE 4222 6222 8222
# Sat, 07 Aug 2021 00:12:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 07 Aug 2021 00:12:59 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:29291e31a76a7e560b9b7ad3cada56e8c18d50a96cca8a2573e4f4689d7aca77`  
		Last Modified: Thu, 05 Aug 2021 15:56:25 GMT  
		Size: 2.8 MB (2813006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5b6f975cea84a1db539a70743c469f460dfd3c0e9f53362581ea5166cc6f7bb`  
		Last Modified: Sat, 07 Aug 2021 00:13:34 GMT  
		Size: 4.8 MB (4790004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:591a3df61d2af8d57d3b1b9462ef7661cf873411724688e51359600bdddd950c`  
		Last Modified: Sat, 07 Aug 2021 00:13:32 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcc7744cc9fd0f87944d530e0b43728226f13d0a9b61969249ab9b15dabd07d3`  
		Last Modified: Sat, 07 Aug 2021 00:13:32 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:e995bfdd6f9247dbf1b305adc029a95e72e8630251d8d19a9023c63dcbc47318
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7109895 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aae75c35e1d2e6f686fde0a0cfaea0aff2d58dcdf3e52a8ecba5ffc3dea3fe0b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 06 Aug 2021 17:49:32 GMT
ADD file:7f2c7deda009eabdcbbdccb11e854043d32c498e64e7e1ca02165d7bb4261d39 in / 
# Fri, 06 Aug 2021 17:49:32 GMT
CMD ["/bin/sh"]
# Fri, 27 Aug 2021 02:48:29 GMT
ENV NATS_SERVER=2.4.0
# Fri, 27 Aug 2021 02:48:34 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='eb510dd016cb1a9e9b1fae88a3471029048cb75dcc4ad83a4f5b1e3665f24a20' ;; 		armhf) natsArch='arm6'; sha256='76ac66cd86217a43bc227220eb054aac8a5744890d43c76156075d68a684d9e0' ;; 		armv7) natsArch='arm7'; sha256='e7521841d59f55fcef6172aa8f22d3af7ba1776bd67109a23c29d34d18d44bd6' ;; 		x86_64) natsArch='amd64'; sha256='f6841c89fcf99302bc7ac295ddc1e75322385f861d55abee79733976c8eb9bc7' ;; 		x86) natsArch='386'; sha256='c7e6e2b73d402e841b3abb57e26e2ef53350b44e385255bf289b08182058076a' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 27 Aug 2021 02:48:34 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 27 Aug 2021 02:48:35 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 27 Aug 2021 02:48:35 GMT
EXPOSE 4222 6222 8222
# Fri, 27 Aug 2021 02:48:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 Aug 2021 02:48:36 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:f465bb3e9fcd0c42f936ecc566c6e40353c00f3089b2b2c2ea1663c30f89d3ab`  
		Last Modified: Fri, 06 Aug 2021 17:51:00 GMT  
		Size: 2.6 MB (2626350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5abfce067d7bc34edb53d2ef3b851fb6750f2f165d88e6b7c1751a372637cf9`  
		Last Modified: Fri, 27 Aug 2021 02:50:40 GMT  
		Size: 4.5 MB (4482575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:915f8f45a2be36433373b63850ff3ca8ec9eb622ab7d74dd908284a971539307`  
		Last Modified: Fri, 27 Aug 2021 02:50:38 GMT  
		Size: 557.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dcbfc2ac16592f5503b1b3f59404245367a0082b75af6bd79a2b48e8c45a762`  
		Last Modified: Fri, 27 Aug 2021 02:50:38 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:443f504d21f3881e958e0e58c996d3e5970ff90cf970c6e41adc2542ae14e2b9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.9 MB (6880695 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:671e9b1b37b7c31f58f233286cc6ee3009ae062bfd7634d1e8e15be89ea2492e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 06 Aug 2021 17:57:32 GMT
ADD file:3a35ff3ac0d80289d419a4d6d8319610c38e1936d296addafb9aaf506946230f in / 
# Fri, 06 Aug 2021 17:57:32 GMT
CMD ["/bin/sh"]
# Fri, 06 Aug 2021 20:26:24 GMT
ENV NATS_SERVER=2.3.4
# Fri, 06 Aug 2021 20:26:28 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='c8ba676a6c4ec9d3088e0b64ffdae36e2f2a9e1b89f030799f3efbb2923524a0' ;; 		armhf) natsArch='arm6'; sha256='d1f14441d1fbd53a7bff9623e8e572707d3e7024b42b6e925ad371d4dec0bc47' ;; 		armv7) natsArch='arm7'; sha256='2488706de91e94eba477ddbc3b293ec0b4d823509656cc101eec6a07e0319bb5' ;; 		x86_64) natsArch='amd64'; sha256='8c11abdeca4882888a8b6fbc45effe9fb4d1070eda3939b7299892c8c69a3e87' ;; 		x86) natsArch='386'; sha256='010bca73095d8a05495ef74a112dfd3919925b0ced10bc4c5f876f3858ca41f7' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 06 Aug 2021 20:26:29 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 06 Aug 2021 20:26:29 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 06 Aug 2021 20:26:30 GMT
EXPOSE 4222 6222 8222
# Fri, 06 Aug 2021 20:26:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 06 Aug 2021 20:26:31 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:4ee0caa23b369b04827640a4be298bf4ff7bacd030c77e915f5d7fb8f987594a`  
		Last Modified: Fri, 06 Aug 2021 17:58:57 GMT  
		Size: 2.4 MB (2429359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54864bfc951be8b12f75e7c53f918420224b41c45520c27dc54f47006e1ace61`  
		Last Modified: Fri, 06 Aug 2021 20:28:37 GMT  
		Size: 4.5 MB (4450364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d8e3d21fd5215bd4bad28c6e61f03fe72c301544f5e535f0f618132b4bf3d90`  
		Last Modified: Fri, 06 Aug 2021 20:28:33 GMT  
		Size: 559.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e584ceff2e79dca85ab2d5589768d2243a4b7e52b7e1743785667471c73d928`  
		Last Modified: Fri, 06 Aug 2021 20:28:34 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:3ba9b8c80c1026d2a500251c07a9af099943e0291f5c381e49e6d6e496f8de8b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7115983 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:671a61b3bebfb1b125fc5ae67fc31351bc0aad1a0d1a103a21bb80895d7c09f3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 06 Aug 2021 17:39:26 GMT
ADD file:1a8fd1066485e1261462e689c1a072f010c1d3be904b73ef2b84128fac652951 in / 
# Fri, 06 Aug 2021 17:39:27 GMT
CMD ["/bin/sh"]
# Fri, 06 Aug 2021 19:49:47 GMT
ENV NATS_SERVER=2.3.4
# Fri, 06 Aug 2021 19:49:50 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='c8ba676a6c4ec9d3088e0b64ffdae36e2f2a9e1b89f030799f3efbb2923524a0' ;; 		armhf) natsArch='arm6'; sha256='d1f14441d1fbd53a7bff9623e8e572707d3e7024b42b6e925ad371d4dec0bc47' ;; 		armv7) natsArch='arm7'; sha256='2488706de91e94eba477ddbc3b293ec0b4d823509656cc101eec6a07e0319bb5' ;; 		x86_64) natsArch='amd64'; sha256='8c11abdeca4882888a8b6fbc45effe9fb4d1070eda3939b7299892c8c69a3e87' ;; 		x86) natsArch='386'; sha256='010bca73095d8a05495ef74a112dfd3919925b0ced10bc4c5f876f3858ca41f7' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 06 Aug 2021 19:49:50 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 06 Aug 2021 19:49:50 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 06 Aug 2021 19:49:50 GMT
EXPOSE 4222 6222 8222
# Fri, 06 Aug 2021 19:49:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 06 Aug 2021 19:49:50 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:fd3acdcea5682abced546ec19fb6ebee725c5184e5d91614c469c0a79e67f2d0`  
		Last Modified: Fri, 06 Aug 2021 17:40:12 GMT  
		Size: 2.7 MB (2710613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94ef6a8d5827e19307796e49f087f09097ca6784d2d680b67bf245e33eaa0417`  
		Last Modified: Fri, 06 Aug 2021 19:50:52 GMT  
		Size: 4.4 MB (4404401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc719578654cd35d6807367a487c4c618898557f046b46f894ccf6869b4d00cc`  
		Last Modified: Fri, 06 Aug 2021 19:50:52 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:742e4ce06ec6c0603f0ffe18a7788896b1ebe0f93184cba0be76177c3bb5c56b`  
		Last Modified: Fri, 06 Aug 2021 19:50:52 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-alpine3.14`

```console
$ docker pull nats@sha256:45faf7fef5f78d815f712b8a05a2a0ded8793d777a0fb7640b0b0e6ff58e0009
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-alpine3.14` - linux; amd64

```console
$ docker pull nats@sha256:7a1ec46ffffcc712a37d5e801e73e4cb68b22e15c842f36ab9211e1a039cb547
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7603979 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:163732450f029c457fb0826ccdbb6d69696f0d8af625ed2bef5291b807563c38`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 06 Aug 2021 17:19:45 GMT
ADD file:34eb5c40aa00028921a224d1764ae1b1f3ef710d191e4dfc7df55e0594aa7217 in / 
# Fri, 06 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Sat, 07 Aug 2021 00:12:56 GMT
ENV NATS_SERVER=2.3.4
# Sat, 07 Aug 2021 00:12:58 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='c8ba676a6c4ec9d3088e0b64ffdae36e2f2a9e1b89f030799f3efbb2923524a0' ;; 		armhf) natsArch='arm6'; sha256='d1f14441d1fbd53a7bff9623e8e572707d3e7024b42b6e925ad371d4dec0bc47' ;; 		armv7) natsArch='arm7'; sha256='2488706de91e94eba477ddbc3b293ec0b4d823509656cc101eec6a07e0319bb5' ;; 		x86_64) natsArch='amd64'; sha256='8c11abdeca4882888a8b6fbc45effe9fb4d1070eda3939b7299892c8c69a3e87' ;; 		x86) natsArch='386'; sha256='010bca73095d8a05495ef74a112dfd3919925b0ced10bc4c5f876f3858ca41f7' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Sat, 07 Aug 2021 00:12:59 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Sat, 07 Aug 2021 00:12:59 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Sat, 07 Aug 2021 00:12:59 GMT
EXPOSE 4222 6222 8222
# Sat, 07 Aug 2021 00:12:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 07 Aug 2021 00:12:59 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:29291e31a76a7e560b9b7ad3cada56e8c18d50a96cca8a2573e4f4689d7aca77`  
		Last Modified: Thu, 05 Aug 2021 15:56:25 GMT  
		Size: 2.8 MB (2813006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5b6f975cea84a1db539a70743c469f460dfd3c0e9f53362581ea5166cc6f7bb`  
		Last Modified: Sat, 07 Aug 2021 00:13:34 GMT  
		Size: 4.8 MB (4790004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:591a3df61d2af8d57d3b1b9462ef7661cf873411724688e51359600bdddd950c`  
		Last Modified: Sat, 07 Aug 2021 00:13:32 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcc7744cc9fd0f87944d530e0b43728226f13d0a9b61969249ab9b15dabd07d3`  
		Last Modified: Sat, 07 Aug 2021 00:13:32 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.14` - linux; arm variant v6

```console
$ docker pull nats@sha256:e995bfdd6f9247dbf1b305adc029a95e72e8630251d8d19a9023c63dcbc47318
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7109895 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aae75c35e1d2e6f686fde0a0cfaea0aff2d58dcdf3e52a8ecba5ffc3dea3fe0b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 06 Aug 2021 17:49:32 GMT
ADD file:7f2c7deda009eabdcbbdccb11e854043d32c498e64e7e1ca02165d7bb4261d39 in / 
# Fri, 06 Aug 2021 17:49:32 GMT
CMD ["/bin/sh"]
# Fri, 27 Aug 2021 02:48:29 GMT
ENV NATS_SERVER=2.4.0
# Fri, 27 Aug 2021 02:48:34 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='eb510dd016cb1a9e9b1fae88a3471029048cb75dcc4ad83a4f5b1e3665f24a20' ;; 		armhf) natsArch='arm6'; sha256='76ac66cd86217a43bc227220eb054aac8a5744890d43c76156075d68a684d9e0' ;; 		armv7) natsArch='arm7'; sha256='e7521841d59f55fcef6172aa8f22d3af7ba1776bd67109a23c29d34d18d44bd6' ;; 		x86_64) natsArch='amd64'; sha256='f6841c89fcf99302bc7ac295ddc1e75322385f861d55abee79733976c8eb9bc7' ;; 		x86) natsArch='386'; sha256='c7e6e2b73d402e841b3abb57e26e2ef53350b44e385255bf289b08182058076a' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 27 Aug 2021 02:48:34 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 27 Aug 2021 02:48:35 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 27 Aug 2021 02:48:35 GMT
EXPOSE 4222 6222 8222
# Fri, 27 Aug 2021 02:48:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 Aug 2021 02:48:36 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:f465bb3e9fcd0c42f936ecc566c6e40353c00f3089b2b2c2ea1663c30f89d3ab`  
		Last Modified: Fri, 06 Aug 2021 17:51:00 GMT  
		Size: 2.6 MB (2626350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5abfce067d7bc34edb53d2ef3b851fb6750f2f165d88e6b7c1751a372637cf9`  
		Last Modified: Fri, 27 Aug 2021 02:50:40 GMT  
		Size: 4.5 MB (4482575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:915f8f45a2be36433373b63850ff3ca8ec9eb622ab7d74dd908284a971539307`  
		Last Modified: Fri, 27 Aug 2021 02:50:38 GMT  
		Size: 557.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dcbfc2ac16592f5503b1b3f59404245367a0082b75af6bd79a2b48e8c45a762`  
		Last Modified: Fri, 27 Aug 2021 02:50:38 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.14` - linux; arm variant v7

```console
$ docker pull nats@sha256:443f504d21f3881e958e0e58c996d3e5970ff90cf970c6e41adc2542ae14e2b9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.9 MB (6880695 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:671e9b1b37b7c31f58f233286cc6ee3009ae062bfd7634d1e8e15be89ea2492e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 06 Aug 2021 17:57:32 GMT
ADD file:3a35ff3ac0d80289d419a4d6d8319610c38e1936d296addafb9aaf506946230f in / 
# Fri, 06 Aug 2021 17:57:32 GMT
CMD ["/bin/sh"]
# Fri, 06 Aug 2021 20:26:24 GMT
ENV NATS_SERVER=2.3.4
# Fri, 06 Aug 2021 20:26:28 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='c8ba676a6c4ec9d3088e0b64ffdae36e2f2a9e1b89f030799f3efbb2923524a0' ;; 		armhf) natsArch='arm6'; sha256='d1f14441d1fbd53a7bff9623e8e572707d3e7024b42b6e925ad371d4dec0bc47' ;; 		armv7) natsArch='arm7'; sha256='2488706de91e94eba477ddbc3b293ec0b4d823509656cc101eec6a07e0319bb5' ;; 		x86_64) natsArch='amd64'; sha256='8c11abdeca4882888a8b6fbc45effe9fb4d1070eda3939b7299892c8c69a3e87' ;; 		x86) natsArch='386'; sha256='010bca73095d8a05495ef74a112dfd3919925b0ced10bc4c5f876f3858ca41f7' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 06 Aug 2021 20:26:29 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 06 Aug 2021 20:26:29 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 06 Aug 2021 20:26:30 GMT
EXPOSE 4222 6222 8222
# Fri, 06 Aug 2021 20:26:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 06 Aug 2021 20:26:31 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:4ee0caa23b369b04827640a4be298bf4ff7bacd030c77e915f5d7fb8f987594a`  
		Last Modified: Fri, 06 Aug 2021 17:58:57 GMT  
		Size: 2.4 MB (2429359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54864bfc951be8b12f75e7c53f918420224b41c45520c27dc54f47006e1ace61`  
		Last Modified: Fri, 06 Aug 2021 20:28:37 GMT  
		Size: 4.5 MB (4450364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d8e3d21fd5215bd4bad28c6e61f03fe72c301544f5e535f0f618132b4bf3d90`  
		Last Modified: Fri, 06 Aug 2021 20:28:33 GMT  
		Size: 559.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e584ceff2e79dca85ab2d5589768d2243a4b7e52b7e1743785667471c73d928`  
		Last Modified: Fri, 06 Aug 2021 20:28:34 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.14` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:3ba9b8c80c1026d2a500251c07a9af099943e0291f5c381e49e6d6e496f8de8b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7115983 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:671a61b3bebfb1b125fc5ae67fc31351bc0aad1a0d1a103a21bb80895d7c09f3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 06 Aug 2021 17:39:26 GMT
ADD file:1a8fd1066485e1261462e689c1a072f010c1d3be904b73ef2b84128fac652951 in / 
# Fri, 06 Aug 2021 17:39:27 GMT
CMD ["/bin/sh"]
# Fri, 06 Aug 2021 19:49:47 GMT
ENV NATS_SERVER=2.3.4
# Fri, 06 Aug 2021 19:49:50 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='c8ba676a6c4ec9d3088e0b64ffdae36e2f2a9e1b89f030799f3efbb2923524a0' ;; 		armhf) natsArch='arm6'; sha256='d1f14441d1fbd53a7bff9623e8e572707d3e7024b42b6e925ad371d4dec0bc47' ;; 		armv7) natsArch='arm7'; sha256='2488706de91e94eba477ddbc3b293ec0b4d823509656cc101eec6a07e0319bb5' ;; 		x86_64) natsArch='amd64'; sha256='8c11abdeca4882888a8b6fbc45effe9fb4d1070eda3939b7299892c8c69a3e87' ;; 		x86) natsArch='386'; sha256='010bca73095d8a05495ef74a112dfd3919925b0ced10bc4c5f876f3858ca41f7' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 06 Aug 2021 19:49:50 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 06 Aug 2021 19:49:50 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 06 Aug 2021 19:49:50 GMT
EXPOSE 4222 6222 8222
# Fri, 06 Aug 2021 19:49:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 06 Aug 2021 19:49:50 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:fd3acdcea5682abced546ec19fb6ebee725c5184e5d91614c469c0a79e67f2d0`  
		Last Modified: Fri, 06 Aug 2021 17:40:12 GMT  
		Size: 2.7 MB (2710613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94ef6a8d5827e19307796e49f087f09097ca6784d2d680b67bf245e33eaa0417`  
		Last Modified: Fri, 06 Aug 2021 19:50:52 GMT  
		Size: 4.4 MB (4404401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc719578654cd35d6807367a487c4c618898557f046b46f894ccf6869b4d00cc`  
		Last Modified: Fri, 06 Aug 2021 19:50:52 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:742e4ce06ec6c0603f0ffe18a7788896b1ebe0f93184cba0be76177c3bb5c56b`  
		Last Modified: Fri, 06 Aug 2021 19:50:52 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-linux`

```console
$ docker pull nats@sha256:91afdbdd639c488228d39325873355953a2e8d6d579eea0d5695cea72b68e7ba
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-linux` - linux; amd64

```console
$ docker pull nats@sha256:acd926de12a3d1a625d13dfab262fa240b0d99ecb35c68e372e093ab466d1b0b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4506461 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5738e29b3f24028140a48fe9652afc26b4118a35427b996d591872c6dd9162ed`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 05 Aug 2021 01:20:24 GMT
COPY file:edd123fab471ca4bff1ec55ddc839aaf0defe3667b337aaec7c3c8e70e903e8d in /nats-server 
# Thu, 05 Aug 2021 01:20:24 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 05 Aug 2021 01:20:24 GMT
EXPOSE 4222 6222 8222
# Thu, 05 Aug 2021 01:20:24 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 05 Aug 2021 01:20:25 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3d02ec701f9917abde1e8953cba96577f89ebc29ced1af0d82734bde1a034361`  
		Last Modified: Thu, 05 Aug 2021 01:21:15 GMT  
		Size: 4.5 MB (4505985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6beb29f4b4e73a454d8e38755b89ed0a71bb2f1aaaaa02105c3708af114c87cc`  
		Last Modified: Thu, 05 Aug 2021 01:21:14 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:7201c8cd794776fa392c3a25eb89e4ee987aeaaae647caa364621d5daf5ca3c5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4201703 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc2211a135c8d5c9641c74ba5d54c3c1df4ac3f24fa70a6a57be8a2975af7854`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 02:48:56 GMT
COPY file:81d7dcb1f2223ae767ee02f3b24758797ca55a665d17dcb2054eeb097fb2eafa in /nats-server 
# Fri, 27 Aug 2021 02:48:56 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 27 Aug 2021 02:48:57 GMT
EXPOSE 4222 6222 8222
# Fri, 27 Aug 2021 02:48:57 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 27 Aug 2021 02:48:58 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a820d11a96d84195887c44533ffcad67997fcb79d52f4564709bfdbde47d578d`  
		Last Modified: Fri, 27 Aug 2021 02:51:18 GMT  
		Size: 4.2 MB (4201229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a1c4f82bf849dc3d9d18f1c560b9afd0e5237eb2f05377e6792dda2480249cb`  
		Last Modified: Fri, 27 Aug 2021 02:51:15 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:edbf04c6d86cc6973609fb90c099c175ba05216954d224ea93c03e862b6c0955
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4170312 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:59d59f3755a610c7ef37ce7df6d7e2a6c1a1e7e0554fd7f0dfe5a7ba96370e6f`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 05 Aug 2021 01:04:56 GMT
COPY file:f8d5a2ea993b24151d26b5967a44af43f6fa70afe6b7965767ebb48f41351935 in /nats-server 
# Thu, 05 Aug 2021 01:04:57 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 05 Aug 2021 01:04:57 GMT
EXPOSE 4222 6222 8222
# Thu, 05 Aug 2021 01:04:58 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 05 Aug 2021 01:04:58 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:0b65416c95f5f06a582f3d8ffe3f3cc9b4df10e5d724eb5167d7766bce64b77e`  
		Last Modified: Thu, 05 Aug 2021 01:07:22 GMT  
		Size: 4.2 MB (4169837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:711811fab377fd6c12391460fafc4fe011d419669f5508b086b269489ae78d22`  
		Last Modified: Thu, 05 Aug 2021 01:07:20 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:258407bfd157b748b13d824daa441eeb795b46dae0dee509189e6f215219dfc4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.1 MB (4121540 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:928fc611a3e5935a6eea2e73e72cfc121d250a608f1def1e50e9a2bca5e9e0c4`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 05 Aug 2021 01:39:59 GMT
COPY file:e2687e43e0f0627dcdfb73c8b9b66c9a86cdda6399f627b485911acbece9a3c9 in /nats-server 
# Thu, 05 Aug 2021 01:40:00 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 05 Aug 2021 01:40:00 GMT
EXPOSE 4222 6222 8222
# Thu, 05 Aug 2021 01:40:00 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 05 Aug 2021 01:40:00 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:333cb9b408ea509452b14ed5b1c9a8a6abed86e5a3177bc9ae7917d6c0c51318`  
		Last Modified: Thu, 05 Aug 2021 01:41:23 GMT  
		Size: 4.1 MB (4121065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b79f5ac7bd31304ad5fab87a7bb25e67ff6f7e8f0299806180b5bb556ea0dc9`  
		Last Modified: Thu, 05 Aug 2021 01:41:22 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-nanoserver`

```console
$ docker pull nats@sha256:21ff4cbb5485b408bcc030f341817018fb13a7381ca7c520960bf26bab74ddac
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2114; amd64

### `nats:2-nanoserver` - windows version 10.0.17763.2114; amd64

```console
$ docker pull nats@sha256:9c370308b1924738df19dd502a9d8d8c13066580fd1550eddbf4f70663c87fe5
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.3 MB (107338949 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e90920ed24cf8337e7f99fdd7199bff8ec7dd43cfa5063f0f373e6700f8a17a2`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 05 Aug 2021 19:15:20 GMT
RUN Apply image 1809-amd64
# Wed, 25 Aug 2021 16:07:56 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 27 Aug 2021 00:16:45 GMT
RUN cmd /S /C #(nop) COPY file:bafd3fc1559b39648f01fab1b3b19a9fc9bb95afae5b07b1d7987b376806e053 in C:\nats-server.exe 
# Fri, 27 Aug 2021 00:16:46 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 27 Aug 2021 00:16:47 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Fri, 27 Aug 2021 00:16:47 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 27 Aug 2021 00:16:48 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:bc8517709e9cfff223cb034ff5be8fcbfa5409de286cdac9ae1b8878ebea6b84`  
		Size: 102.7 MB (102741177 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ae8616c17f5cca409a4b1289387e37dc532657ba2b52bb60713ff621acccd506`  
		Last Modified: Wed, 25 Aug 2021 16:11:20 GMT  
		Size: 1.0 KB (1022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb815244c76bae445a6697a3f1b6a0643fc016be2b2da5192dc6bb4079cd0119`  
		Last Modified: Fri, 27 Aug 2021 00:20:21 GMT  
		Size: 4.6 MB (4591622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c33193ffa3c81a2ebd95cb6af96ce80ee557191a64ba47e1977479e1167530ca`  
		Last Modified: Fri, 27 Aug 2021 00:20:19 GMT  
		Size: 1.7 KB (1701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c57e2e68d87e03a37f706b01fe403fc34435b82da71d1080e11ec9df4d418a2`  
		Last Modified: Fri, 27 Aug 2021 00:20:19 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:048b1707f600e77fb06d48bd9c3759cad471944658bdfa3dd59b2852dc7983b4`  
		Last Modified: Fri, 27 Aug 2021 00:20:20 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b434e68e7546ed285144b98ef8fc3a10f1b6ee578ef2503e9f09aefab0370d0`  
		Last Modified: Fri, 27 Aug 2021 00:20:20 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-nanoserver-1809`

```console
$ docker pull nats@sha256:21ff4cbb5485b408bcc030f341817018fb13a7381ca7c520960bf26bab74ddac
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2114; amd64

### `nats:2-nanoserver-1809` - windows version 10.0.17763.2114; amd64

```console
$ docker pull nats@sha256:9c370308b1924738df19dd502a9d8d8c13066580fd1550eddbf4f70663c87fe5
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.3 MB (107338949 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e90920ed24cf8337e7f99fdd7199bff8ec7dd43cfa5063f0f373e6700f8a17a2`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 05 Aug 2021 19:15:20 GMT
RUN Apply image 1809-amd64
# Wed, 25 Aug 2021 16:07:56 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 27 Aug 2021 00:16:45 GMT
RUN cmd /S /C #(nop) COPY file:bafd3fc1559b39648f01fab1b3b19a9fc9bb95afae5b07b1d7987b376806e053 in C:\nats-server.exe 
# Fri, 27 Aug 2021 00:16:46 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 27 Aug 2021 00:16:47 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Fri, 27 Aug 2021 00:16:47 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 27 Aug 2021 00:16:48 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:bc8517709e9cfff223cb034ff5be8fcbfa5409de286cdac9ae1b8878ebea6b84`  
		Size: 102.7 MB (102741177 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ae8616c17f5cca409a4b1289387e37dc532657ba2b52bb60713ff621acccd506`  
		Last Modified: Wed, 25 Aug 2021 16:11:20 GMT  
		Size: 1.0 KB (1022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb815244c76bae445a6697a3f1b6a0643fc016be2b2da5192dc6bb4079cd0119`  
		Last Modified: Fri, 27 Aug 2021 00:20:21 GMT  
		Size: 4.6 MB (4591622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c33193ffa3c81a2ebd95cb6af96ce80ee557191a64ba47e1977479e1167530ca`  
		Last Modified: Fri, 27 Aug 2021 00:20:19 GMT  
		Size: 1.7 KB (1701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c57e2e68d87e03a37f706b01fe403fc34435b82da71d1080e11ec9df4d418a2`  
		Last Modified: Fri, 27 Aug 2021 00:20:19 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:048b1707f600e77fb06d48bd9c3759cad471944658bdfa3dd59b2852dc7983b4`  
		Last Modified: Fri, 27 Aug 2021 00:20:20 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b434e68e7546ed285144b98ef8fc3a10f1b6ee578ef2503e9f09aefab0370d0`  
		Last Modified: Fri, 27 Aug 2021 00:20:20 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-scratch`

```console
$ docker pull nats@sha256:91afdbdd639c488228d39325873355953a2e8d6d579eea0d5695cea72b68e7ba
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-scratch` - linux; amd64

```console
$ docker pull nats@sha256:acd926de12a3d1a625d13dfab262fa240b0d99ecb35c68e372e093ab466d1b0b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4506461 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5738e29b3f24028140a48fe9652afc26b4118a35427b996d591872c6dd9162ed`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 05 Aug 2021 01:20:24 GMT
COPY file:edd123fab471ca4bff1ec55ddc839aaf0defe3667b337aaec7c3c8e70e903e8d in /nats-server 
# Thu, 05 Aug 2021 01:20:24 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 05 Aug 2021 01:20:24 GMT
EXPOSE 4222 6222 8222
# Thu, 05 Aug 2021 01:20:24 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 05 Aug 2021 01:20:25 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3d02ec701f9917abde1e8953cba96577f89ebc29ced1af0d82734bde1a034361`  
		Last Modified: Thu, 05 Aug 2021 01:21:15 GMT  
		Size: 4.5 MB (4505985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6beb29f4b4e73a454d8e38755b89ed0a71bb2f1aaaaa02105c3708af114c87cc`  
		Last Modified: Thu, 05 Aug 2021 01:21:14 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:7201c8cd794776fa392c3a25eb89e4ee987aeaaae647caa364621d5daf5ca3c5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4201703 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc2211a135c8d5c9641c74ba5d54c3c1df4ac3f24fa70a6a57be8a2975af7854`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 02:48:56 GMT
COPY file:81d7dcb1f2223ae767ee02f3b24758797ca55a665d17dcb2054eeb097fb2eafa in /nats-server 
# Fri, 27 Aug 2021 02:48:56 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 27 Aug 2021 02:48:57 GMT
EXPOSE 4222 6222 8222
# Fri, 27 Aug 2021 02:48:57 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 27 Aug 2021 02:48:58 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a820d11a96d84195887c44533ffcad67997fcb79d52f4564709bfdbde47d578d`  
		Last Modified: Fri, 27 Aug 2021 02:51:18 GMT  
		Size: 4.2 MB (4201229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a1c4f82bf849dc3d9d18f1c560b9afd0e5237eb2f05377e6792dda2480249cb`  
		Last Modified: Fri, 27 Aug 2021 02:51:15 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:edbf04c6d86cc6973609fb90c099c175ba05216954d224ea93c03e862b6c0955
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4170312 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:59d59f3755a610c7ef37ce7df6d7e2a6c1a1e7e0554fd7f0dfe5a7ba96370e6f`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 05 Aug 2021 01:04:56 GMT
COPY file:f8d5a2ea993b24151d26b5967a44af43f6fa70afe6b7965767ebb48f41351935 in /nats-server 
# Thu, 05 Aug 2021 01:04:57 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 05 Aug 2021 01:04:57 GMT
EXPOSE 4222 6222 8222
# Thu, 05 Aug 2021 01:04:58 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 05 Aug 2021 01:04:58 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:0b65416c95f5f06a582f3d8ffe3f3cc9b4df10e5d724eb5167d7766bce64b77e`  
		Last Modified: Thu, 05 Aug 2021 01:07:22 GMT  
		Size: 4.2 MB (4169837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:711811fab377fd6c12391460fafc4fe011d419669f5508b086b269489ae78d22`  
		Last Modified: Thu, 05 Aug 2021 01:07:20 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:258407bfd157b748b13d824daa441eeb795b46dae0dee509189e6f215219dfc4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.1 MB (4121540 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:928fc611a3e5935a6eea2e73e72cfc121d250a608f1def1e50e9a2bca5e9e0c4`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 05 Aug 2021 01:39:59 GMT
COPY file:e2687e43e0f0627dcdfb73c8b9b66c9a86cdda6399f627b485911acbece9a3c9 in /nats-server 
# Thu, 05 Aug 2021 01:40:00 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 05 Aug 2021 01:40:00 GMT
EXPOSE 4222 6222 8222
# Thu, 05 Aug 2021 01:40:00 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 05 Aug 2021 01:40:00 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:333cb9b408ea509452b14ed5b1c9a8a6abed86e5a3177bc9ae7917d6c0c51318`  
		Last Modified: Thu, 05 Aug 2021 01:41:23 GMT  
		Size: 4.1 MB (4121065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b79f5ac7bd31304ad5fab87a7bb25e67ff6f7e8f0299806180b5bb556ea0dc9`  
		Last Modified: Thu, 05 Aug 2021 01:41:22 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-windowsservercore`

```console
$ docker pull nats@sha256:cf3aae4f841ee35ce5bfef42265fbd8025c1cff06d3f284e813cfec4cf9d6e4a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.2114; amd64
	-	windows version 10.0.14393.4583; amd64

### `nats:2-windowsservercore` - windows version 10.0.17763.2114; amd64

```console
$ docker pull nats@sha256:48cc63b49c047b98135531fccf1f7c4a418477d38def8702f6ecce6e8574923c
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2691328041 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09c3d57b266e04d58ceedd30a6c5428caa6783ca301ecc858c8aa62a8f682a3a`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 05 Aug 2021 19:44:34 GMT
RUN Install update 1809-amd64
# Wed, 25 Aug 2021 13:46:35 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 25 Aug 2021 16:05:30 GMT
ENV NATS_DOCKERIZED=1
# Fri, 27 Aug 2021 00:14:05 GMT
ENV NATS_SERVER=2.4.0
# Fri, 27 Aug 2021 00:14:06 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.4.0/nats-server-v2.4.0-windows-amd64.zip
# Fri, 27 Aug 2021 00:14:07 GMT
ENV NATS_SERVER_SHASUM=6c66acf5ed7e87a1ed9c499033c8c64c8c1365c5a95973ec57859abf1a69b032
# Fri, 27 Aug 2021 00:15:10 GMT
RUN Set-PSDebug -Trace 2
# Fri, 27 Aug 2021 00:16:22 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 27 Aug 2021 00:16:23 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 27 Aug 2021 00:16:24 GMT
EXPOSE 4222 6222 8222
# Fri, 27 Aug 2021 00:16:25 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 27 Aug 2021 00:16:26 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c67ded6868b61d392a0c096f911563fd6bc0bc3ed4fe401d077b3718a1b0cdaf`  
		Size: 967.7 MB (967665054 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:985da5cbc0735e1c422e766af23125ba345f431cb337ea43ec32298d0bb8e4ea`  
		Last Modified: Wed, 25 Aug 2021 15:45:02 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3dbdd68a4b0c278695b3e1d401d7eddfb0f0e3aa1e28aed88eb700059648f8f`  
		Last Modified: Wed, 25 Aug 2021 16:11:02 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9924833e15cbbaa8bd2d64c942c877c0765ba95d0790a5a9ea83a3d40bcaba43`  
		Last Modified: Fri, 27 Aug 2021 00:20:04 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93b8b51ab5e087ce5a5187d2967b0a82e4ce38b2151fc1b040be11a843334b1a`  
		Last Modified: Fri, 27 Aug 2021 00:20:00 GMT  
		Size: 1.4 KB (1360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73666a2686d6829048f4fa9f037f08038370c72202369f80bd4b715ead2cafe3`  
		Last Modified: Fri, 27 Aug 2021 00:20:00 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e35fdb95a7dc56c84ff744d8172574e2edd053f77affad83306be03c14fdb9fb`  
		Last Modified: Fri, 27 Aug 2021 00:20:01 GMT  
		Size: 372.5 KB (372513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3b9b9590a746c11677c6728f047f437a87645f68249b9691ed347591b850b8d`  
		Last Modified: Fri, 27 Aug 2021 00:20:00 GMT  
		Size: 4.9 MB (4944435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b629e22fb2c409b07df4f55a5b1c1d392ae3fc7110b646f46f63c8de8af0f470`  
		Last Modified: Fri, 27 Aug 2021 00:19:58 GMT  
		Size: 2.0 KB (1978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12c15056241134a8112b0c3e43493f7be7cd0421808ee5edbddb6490f355110e`  
		Last Modified: Fri, 27 Aug 2021 00:19:58 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27b1ee4ad1c87cc30317f9c2212c416f2a120923e62f8f88b8192c58d07a9dc1`  
		Last Modified: Fri, 27 Aug 2021 00:19:58 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1f840f93a8499fdb3efd112f5eedcef4290ba5edc497321ae223cdfc4dcb80e`  
		Last Modified: Fri, 27 Aug 2021 00:19:58 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-windowsservercore` - windows version 10.0.14393.4583; amd64

```console
$ docker pull nats@sha256:f6699a354c1c84d5ad72289d99c815e7bf11f983cd786684a5015745992e58e4
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6276264126 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af044355ba3348cfc4c9fb174c578e012f1a979a5d04b3681aafc9c2d9411eff`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Sun, 01 Aug 2021 08:52:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 25 Aug 2021 13:59:32 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 25 Aug 2021 16:08:06 GMT
ENV NATS_DOCKERIZED=1
# Fri, 27 Aug 2021 00:16:54 GMT
ENV NATS_SERVER=2.4.0
# Fri, 27 Aug 2021 00:16:55 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.4.0/nats-server-v2.4.0-windows-amd64.zip
# Fri, 27 Aug 2021 00:16:56 GMT
ENV NATS_SERVER_SHASUM=6c66acf5ed7e87a1ed9c499033c8c64c8c1365c5a95973ec57859abf1a69b032
# Fri, 27 Aug 2021 00:17:57 GMT
RUN Set-PSDebug -Trace 2
# Fri, 27 Aug 2021 00:19:20 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 27 Aug 2021 00:19:21 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 27 Aug 2021 00:19:21 GMT
EXPOSE 4222 6222 8222
# Fri, 27 Aug 2021 00:19:22 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 27 Aug 2021 00:19:23 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c427f892fe74603ae09d4e49b25f8f7046f957054034dc9f462e0e88d7bffaa5`  
		Size: 2.2 GB (2200980134 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a869803fc3d8292f0fe1bc6ed35e1ceedbd7c797a1486767a55f88c6c28ed4c5`  
		Last Modified: Wed, 25 Aug 2021 15:45:25 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a745f96c10790ef3a2006dbd4c116eb2f1552fd3c4a38fca179a8160e9918ac1`  
		Last Modified: Wed, 25 Aug 2021 16:11:42 GMT  
		Size: 1.3 KB (1329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ecbc2c744fbea737586b320c08b480fbd8eb2dc994300a74c6a4864ee082901`  
		Last Modified: Fri, 27 Aug 2021 00:20:37 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c530ba921538bcf67912fb5a5d6794e991501dbca08ae8137712fc58854f4f68`  
		Last Modified: Fri, 27 Aug 2021 00:20:37 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35523016d41ba152afbfa0a809770805058865f49d17d6d04d77fab412e5c29d`  
		Last Modified: Fri, 27 Aug 2021 00:20:37 GMT  
		Size: 1.4 KB (1383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:348276d7a124485ea8bc7bad9b9147c84dd20fda1da976a1542cbdb907e4ea95`  
		Last Modified: Fri, 27 Aug 2021 00:20:37 GMT  
		Size: 336.1 KB (336071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:751871e4a816cbaed81ad603047b0c9b536c2180dd5e54f7874d1ca37ef57851`  
		Last Modified: Fri, 27 Aug 2021 00:20:36 GMT  
		Size: 4.9 MB (4948899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d9507c0638be8fdbc5f10f76a31d751acfd94e02618ac7528b4856051bb3721`  
		Last Modified: Fri, 27 Aug 2021 00:20:35 GMT  
		Size: 2.0 KB (1979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:784f2e48cdd62d72893e3cf7316c3c7764e937b9ccade0cb0ce5547ee1e1a304`  
		Last Modified: Fri, 27 Aug 2021 00:20:35 GMT  
		Size: 1.4 KB (1357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc0ba660ed14d0923ea760b909e13fa4ff5bc4fe34acc4e9b0e5e072b2cd9704`  
		Last Modified: Fri, 27 Aug 2021 00:20:35 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f34329777aaf85af2b82ec6fa6640f757cc9589247f7fe67e427a4e39c19bda`  
		Last Modified: Fri, 27 Aug 2021 00:20:35 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-windowsservercore-1809`

```console
$ docker pull nats@sha256:a328e744c3a06f930890900c486761a97c2108563a63a093b1d0fc0fb9a1ad21
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2114; amd64

### `nats:2-windowsservercore-1809` - windows version 10.0.17763.2114; amd64

```console
$ docker pull nats@sha256:48cc63b49c047b98135531fccf1f7c4a418477d38def8702f6ecce6e8574923c
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2691328041 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09c3d57b266e04d58ceedd30a6c5428caa6783ca301ecc858c8aa62a8f682a3a`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 05 Aug 2021 19:44:34 GMT
RUN Install update 1809-amd64
# Wed, 25 Aug 2021 13:46:35 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 25 Aug 2021 16:05:30 GMT
ENV NATS_DOCKERIZED=1
# Fri, 27 Aug 2021 00:14:05 GMT
ENV NATS_SERVER=2.4.0
# Fri, 27 Aug 2021 00:14:06 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.4.0/nats-server-v2.4.0-windows-amd64.zip
# Fri, 27 Aug 2021 00:14:07 GMT
ENV NATS_SERVER_SHASUM=6c66acf5ed7e87a1ed9c499033c8c64c8c1365c5a95973ec57859abf1a69b032
# Fri, 27 Aug 2021 00:15:10 GMT
RUN Set-PSDebug -Trace 2
# Fri, 27 Aug 2021 00:16:22 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 27 Aug 2021 00:16:23 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 27 Aug 2021 00:16:24 GMT
EXPOSE 4222 6222 8222
# Fri, 27 Aug 2021 00:16:25 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 27 Aug 2021 00:16:26 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c67ded6868b61d392a0c096f911563fd6bc0bc3ed4fe401d077b3718a1b0cdaf`  
		Size: 967.7 MB (967665054 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:985da5cbc0735e1c422e766af23125ba345f431cb337ea43ec32298d0bb8e4ea`  
		Last Modified: Wed, 25 Aug 2021 15:45:02 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3dbdd68a4b0c278695b3e1d401d7eddfb0f0e3aa1e28aed88eb700059648f8f`  
		Last Modified: Wed, 25 Aug 2021 16:11:02 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9924833e15cbbaa8bd2d64c942c877c0765ba95d0790a5a9ea83a3d40bcaba43`  
		Last Modified: Fri, 27 Aug 2021 00:20:04 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93b8b51ab5e087ce5a5187d2967b0a82e4ce38b2151fc1b040be11a843334b1a`  
		Last Modified: Fri, 27 Aug 2021 00:20:00 GMT  
		Size: 1.4 KB (1360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73666a2686d6829048f4fa9f037f08038370c72202369f80bd4b715ead2cafe3`  
		Last Modified: Fri, 27 Aug 2021 00:20:00 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e35fdb95a7dc56c84ff744d8172574e2edd053f77affad83306be03c14fdb9fb`  
		Last Modified: Fri, 27 Aug 2021 00:20:01 GMT  
		Size: 372.5 KB (372513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3b9b9590a746c11677c6728f047f437a87645f68249b9691ed347591b850b8d`  
		Last Modified: Fri, 27 Aug 2021 00:20:00 GMT  
		Size: 4.9 MB (4944435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b629e22fb2c409b07df4f55a5b1c1d392ae3fc7110b646f46f63c8de8af0f470`  
		Last Modified: Fri, 27 Aug 2021 00:19:58 GMT  
		Size: 2.0 KB (1978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12c15056241134a8112b0c3e43493f7be7cd0421808ee5edbddb6490f355110e`  
		Last Modified: Fri, 27 Aug 2021 00:19:58 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27b1ee4ad1c87cc30317f9c2212c416f2a120923e62f8f88b8192c58d07a9dc1`  
		Last Modified: Fri, 27 Aug 2021 00:19:58 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1f840f93a8499fdb3efd112f5eedcef4290ba5edc497321ae223cdfc4dcb80e`  
		Last Modified: Fri, 27 Aug 2021 00:19:58 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-windowsservercore-ltsc2016`

```console
$ docker pull nats@sha256:7b1ad12d6c6e44e24975eb80e1111d97db29e82416a00dadd5e14a67bf6c0ae4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.14393.4583; amd64

### `nats:2-windowsservercore-ltsc2016` - windows version 10.0.14393.4583; amd64

```console
$ docker pull nats@sha256:f6699a354c1c84d5ad72289d99c815e7bf11f983cd786684a5015745992e58e4
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6276264126 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af044355ba3348cfc4c9fb174c578e012f1a979a5d04b3681aafc9c2d9411eff`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Sun, 01 Aug 2021 08:52:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 25 Aug 2021 13:59:32 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 25 Aug 2021 16:08:06 GMT
ENV NATS_DOCKERIZED=1
# Fri, 27 Aug 2021 00:16:54 GMT
ENV NATS_SERVER=2.4.0
# Fri, 27 Aug 2021 00:16:55 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.4.0/nats-server-v2.4.0-windows-amd64.zip
# Fri, 27 Aug 2021 00:16:56 GMT
ENV NATS_SERVER_SHASUM=6c66acf5ed7e87a1ed9c499033c8c64c8c1365c5a95973ec57859abf1a69b032
# Fri, 27 Aug 2021 00:17:57 GMT
RUN Set-PSDebug -Trace 2
# Fri, 27 Aug 2021 00:19:20 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 27 Aug 2021 00:19:21 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 27 Aug 2021 00:19:21 GMT
EXPOSE 4222 6222 8222
# Fri, 27 Aug 2021 00:19:22 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 27 Aug 2021 00:19:23 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c427f892fe74603ae09d4e49b25f8f7046f957054034dc9f462e0e88d7bffaa5`  
		Size: 2.2 GB (2200980134 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a869803fc3d8292f0fe1bc6ed35e1ceedbd7c797a1486767a55f88c6c28ed4c5`  
		Last Modified: Wed, 25 Aug 2021 15:45:25 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a745f96c10790ef3a2006dbd4c116eb2f1552fd3c4a38fca179a8160e9918ac1`  
		Last Modified: Wed, 25 Aug 2021 16:11:42 GMT  
		Size: 1.3 KB (1329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ecbc2c744fbea737586b320c08b480fbd8eb2dc994300a74c6a4864ee082901`  
		Last Modified: Fri, 27 Aug 2021 00:20:37 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c530ba921538bcf67912fb5a5d6794e991501dbca08ae8137712fc58854f4f68`  
		Last Modified: Fri, 27 Aug 2021 00:20:37 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35523016d41ba152afbfa0a809770805058865f49d17d6d04d77fab412e5c29d`  
		Last Modified: Fri, 27 Aug 2021 00:20:37 GMT  
		Size: 1.4 KB (1383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:348276d7a124485ea8bc7bad9b9147c84dd20fda1da976a1542cbdb907e4ea95`  
		Last Modified: Fri, 27 Aug 2021 00:20:37 GMT  
		Size: 336.1 KB (336071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:751871e4a816cbaed81ad603047b0c9b536c2180dd5e54f7874d1ca37ef57851`  
		Last Modified: Fri, 27 Aug 2021 00:20:36 GMT  
		Size: 4.9 MB (4948899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d9507c0638be8fdbc5f10f76a31d751acfd94e02618ac7528b4856051bb3721`  
		Last Modified: Fri, 27 Aug 2021 00:20:35 GMT  
		Size: 2.0 KB (1979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:784f2e48cdd62d72893e3cf7316c3c7764e937b9ccade0cb0ce5547ee1e1a304`  
		Last Modified: Fri, 27 Aug 2021 00:20:35 GMT  
		Size: 1.4 KB (1357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc0ba660ed14d0923ea760b909e13fa4ff5bc4fe34acc4e9b0e5e072b2cd9704`  
		Last Modified: Fri, 27 Aug 2021 00:20:35 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f34329777aaf85af2b82ec6fa6640f757cc9589247f7fe67e427a4e39c19bda`  
		Last Modified: Fri, 27 Aug 2021 00:20:35 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.4`

```console
$ docker pull nats@sha256:eda69a4b9a9b99aa00804bc7d0a440ff4811b9abf067e6d6bf92ddb98d3a0a7a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; arm variant v6
	-	windows version 10.0.17763.2114; amd64

### `nats:2.4` - linux; arm variant v6

```console
$ docker pull nats@sha256:7201c8cd794776fa392c3a25eb89e4ee987aeaaae647caa364621d5daf5ca3c5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4201703 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc2211a135c8d5c9641c74ba5d54c3c1df4ac3f24fa70a6a57be8a2975af7854`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 02:48:56 GMT
COPY file:81d7dcb1f2223ae767ee02f3b24758797ca55a665d17dcb2054eeb097fb2eafa in /nats-server 
# Fri, 27 Aug 2021 02:48:56 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 27 Aug 2021 02:48:57 GMT
EXPOSE 4222 6222 8222
# Fri, 27 Aug 2021 02:48:57 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 27 Aug 2021 02:48:58 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a820d11a96d84195887c44533ffcad67997fcb79d52f4564709bfdbde47d578d`  
		Last Modified: Fri, 27 Aug 2021 02:51:18 GMT  
		Size: 4.2 MB (4201229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a1c4f82bf849dc3d9d18f1c560b9afd0e5237eb2f05377e6792dda2480249cb`  
		Last Modified: Fri, 27 Aug 2021 02:51:15 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.4` - windows version 10.0.17763.2114; amd64

```console
$ docker pull nats@sha256:9c370308b1924738df19dd502a9d8d8c13066580fd1550eddbf4f70663c87fe5
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.3 MB (107338949 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e90920ed24cf8337e7f99fdd7199bff8ec7dd43cfa5063f0f373e6700f8a17a2`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 05 Aug 2021 19:15:20 GMT
RUN Apply image 1809-amd64
# Wed, 25 Aug 2021 16:07:56 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 27 Aug 2021 00:16:45 GMT
RUN cmd /S /C #(nop) COPY file:bafd3fc1559b39648f01fab1b3b19a9fc9bb95afae5b07b1d7987b376806e053 in C:\nats-server.exe 
# Fri, 27 Aug 2021 00:16:46 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 27 Aug 2021 00:16:47 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Fri, 27 Aug 2021 00:16:47 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 27 Aug 2021 00:16:48 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:bc8517709e9cfff223cb034ff5be8fcbfa5409de286cdac9ae1b8878ebea6b84`  
		Size: 102.7 MB (102741177 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ae8616c17f5cca409a4b1289387e37dc532657ba2b52bb60713ff621acccd506`  
		Last Modified: Wed, 25 Aug 2021 16:11:20 GMT  
		Size: 1.0 KB (1022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb815244c76bae445a6697a3f1b6a0643fc016be2b2da5192dc6bb4079cd0119`  
		Last Modified: Fri, 27 Aug 2021 00:20:21 GMT  
		Size: 4.6 MB (4591622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c33193ffa3c81a2ebd95cb6af96ce80ee557191a64ba47e1977479e1167530ca`  
		Last Modified: Fri, 27 Aug 2021 00:20:19 GMT  
		Size: 1.7 KB (1701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c57e2e68d87e03a37f706b01fe403fc34435b82da71d1080e11ec9df4d418a2`  
		Last Modified: Fri, 27 Aug 2021 00:20:19 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:048b1707f600e77fb06d48bd9c3759cad471944658bdfa3dd59b2852dc7983b4`  
		Last Modified: Fri, 27 Aug 2021 00:20:20 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b434e68e7546ed285144b98ef8fc3a10f1b6ee578ef2503e9f09aefab0370d0`  
		Last Modified: Fri, 27 Aug 2021 00:20:20 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.4-alpine`

```console
$ docker pull nats@sha256:22cb5ac9807b2cae3bef4c860bd2941c6fdf66eec3ddfff985666eeeffe78e39
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; arm variant v6

### `nats:2.4-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:e995bfdd6f9247dbf1b305adc029a95e72e8630251d8d19a9023c63dcbc47318
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7109895 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aae75c35e1d2e6f686fde0a0cfaea0aff2d58dcdf3e52a8ecba5ffc3dea3fe0b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 06 Aug 2021 17:49:32 GMT
ADD file:7f2c7deda009eabdcbbdccb11e854043d32c498e64e7e1ca02165d7bb4261d39 in / 
# Fri, 06 Aug 2021 17:49:32 GMT
CMD ["/bin/sh"]
# Fri, 27 Aug 2021 02:48:29 GMT
ENV NATS_SERVER=2.4.0
# Fri, 27 Aug 2021 02:48:34 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='eb510dd016cb1a9e9b1fae88a3471029048cb75dcc4ad83a4f5b1e3665f24a20' ;; 		armhf) natsArch='arm6'; sha256='76ac66cd86217a43bc227220eb054aac8a5744890d43c76156075d68a684d9e0' ;; 		armv7) natsArch='arm7'; sha256='e7521841d59f55fcef6172aa8f22d3af7ba1776bd67109a23c29d34d18d44bd6' ;; 		x86_64) natsArch='amd64'; sha256='f6841c89fcf99302bc7ac295ddc1e75322385f861d55abee79733976c8eb9bc7' ;; 		x86) natsArch='386'; sha256='c7e6e2b73d402e841b3abb57e26e2ef53350b44e385255bf289b08182058076a' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 27 Aug 2021 02:48:34 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 27 Aug 2021 02:48:35 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 27 Aug 2021 02:48:35 GMT
EXPOSE 4222 6222 8222
# Fri, 27 Aug 2021 02:48:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 Aug 2021 02:48:36 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:f465bb3e9fcd0c42f936ecc566c6e40353c00f3089b2b2c2ea1663c30f89d3ab`  
		Last Modified: Fri, 06 Aug 2021 17:51:00 GMT  
		Size: 2.6 MB (2626350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5abfce067d7bc34edb53d2ef3b851fb6750f2f165d88e6b7c1751a372637cf9`  
		Last Modified: Fri, 27 Aug 2021 02:50:40 GMT  
		Size: 4.5 MB (4482575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:915f8f45a2be36433373b63850ff3ca8ec9eb622ab7d74dd908284a971539307`  
		Last Modified: Fri, 27 Aug 2021 02:50:38 GMT  
		Size: 557.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dcbfc2ac16592f5503b1b3f59404245367a0082b75af6bd79a2b48e8c45a762`  
		Last Modified: Fri, 27 Aug 2021 02:50:38 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.4-alpine3.14`

```console
$ docker pull nats@sha256:22cb5ac9807b2cae3bef4c860bd2941c6fdf66eec3ddfff985666eeeffe78e39
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; arm variant v6

### `nats:2.4-alpine3.14` - linux; arm variant v6

```console
$ docker pull nats@sha256:e995bfdd6f9247dbf1b305adc029a95e72e8630251d8d19a9023c63dcbc47318
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7109895 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aae75c35e1d2e6f686fde0a0cfaea0aff2d58dcdf3e52a8ecba5ffc3dea3fe0b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 06 Aug 2021 17:49:32 GMT
ADD file:7f2c7deda009eabdcbbdccb11e854043d32c498e64e7e1ca02165d7bb4261d39 in / 
# Fri, 06 Aug 2021 17:49:32 GMT
CMD ["/bin/sh"]
# Fri, 27 Aug 2021 02:48:29 GMT
ENV NATS_SERVER=2.4.0
# Fri, 27 Aug 2021 02:48:34 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='eb510dd016cb1a9e9b1fae88a3471029048cb75dcc4ad83a4f5b1e3665f24a20' ;; 		armhf) natsArch='arm6'; sha256='76ac66cd86217a43bc227220eb054aac8a5744890d43c76156075d68a684d9e0' ;; 		armv7) natsArch='arm7'; sha256='e7521841d59f55fcef6172aa8f22d3af7ba1776bd67109a23c29d34d18d44bd6' ;; 		x86_64) natsArch='amd64'; sha256='f6841c89fcf99302bc7ac295ddc1e75322385f861d55abee79733976c8eb9bc7' ;; 		x86) natsArch='386'; sha256='c7e6e2b73d402e841b3abb57e26e2ef53350b44e385255bf289b08182058076a' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 27 Aug 2021 02:48:34 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 27 Aug 2021 02:48:35 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 27 Aug 2021 02:48:35 GMT
EXPOSE 4222 6222 8222
# Fri, 27 Aug 2021 02:48:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 Aug 2021 02:48:36 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:f465bb3e9fcd0c42f936ecc566c6e40353c00f3089b2b2c2ea1663c30f89d3ab`  
		Last Modified: Fri, 06 Aug 2021 17:51:00 GMT  
		Size: 2.6 MB (2626350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5abfce067d7bc34edb53d2ef3b851fb6750f2f165d88e6b7c1751a372637cf9`  
		Last Modified: Fri, 27 Aug 2021 02:50:40 GMT  
		Size: 4.5 MB (4482575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:915f8f45a2be36433373b63850ff3ca8ec9eb622ab7d74dd908284a971539307`  
		Last Modified: Fri, 27 Aug 2021 02:50:38 GMT  
		Size: 557.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dcbfc2ac16592f5503b1b3f59404245367a0082b75af6bd79a2b48e8c45a762`  
		Last Modified: Fri, 27 Aug 2021 02:50:38 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.4-linux`

```console
$ docker pull nats@sha256:fb307cc8febb00cb2c4afd02e16ee319fa13c6471c8ed6543520f2a85f1ceda1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; arm variant v6

### `nats:2.4-linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:7201c8cd794776fa392c3a25eb89e4ee987aeaaae647caa364621d5daf5ca3c5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4201703 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc2211a135c8d5c9641c74ba5d54c3c1df4ac3f24fa70a6a57be8a2975af7854`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 02:48:56 GMT
COPY file:81d7dcb1f2223ae767ee02f3b24758797ca55a665d17dcb2054eeb097fb2eafa in /nats-server 
# Fri, 27 Aug 2021 02:48:56 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 27 Aug 2021 02:48:57 GMT
EXPOSE 4222 6222 8222
# Fri, 27 Aug 2021 02:48:57 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 27 Aug 2021 02:48:58 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a820d11a96d84195887c44533ffcad67997fcb79d52f4564709bfdbde47d578d`  
		Last Modified: Fri, 27 Aug 2021 02:51:18 GMT  
		Size: 4.2 MB (4201229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a1c4f82bf849dc3d9d18f1c560b9afd0e5237eb2f05377e6792dda2480249cb`  
		Last Modified: Fri, 27 Aug 2021 02:51:15 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.4-nanoserver`

```console
$ docker pull nats@sha256:21ff4cbb5485b408bcc030f341817018fb13a7381ca7c520960bf26bab74ddac
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2114; amd64

### `nats:2.4-nanoserver` - windows version 10.0.17763.2114; amd64

```console
$ docker pull nats@sha256:9c370308b1924738df19dd502a9d8d8c13066580fd1550eddbf4f70663c87fe5
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.3 MB (107338949 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e90920ed24cf8337e7f99fdd7199bff8ec7dd43cfa5063f0f373e6700f8a17a2`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 05 Aug 2021 19:15:20 GMT
RUN Apply image 1809-amd64
# Wed, 25 Aug 2021 16:07:56 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 27 Aug 2021 00:16:45 GMT
RUN cmd /S /C #(nop) COPY file:bafd3fc1559b39648f01fab1b3b19a9fc9bb95afae5b07b1d7987b376806e053 in C:\nats-server.exe 
# Fri, 27 Aug 2021 00:16:46 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 27 Aug 2021 00:16:47 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Fri, 27 Aug 2021 00:16:47 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 27 Aug 2021 00:16:48 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:bc8517709e9cfff223cb034ff5be8fcbfa5409de286cdac9ae1b8878ebea6b84`  
		Size: 102.7 MB (102741177 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ae8616c17f5cca409a4b1289387e37dc532657ba2b52bb60713ff621acccd506`  
		Last Modified: Wed, 25 Aug 2021 16:11:20 GMT  
		Size: 1.0 KB (1022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb815244c76bae445a6697a3f1b6a0643fc016be2b2da5192dc6bb4079cd0119`  
		Last Modified: Fri, 27 Aug 2021 00:20:21 GMT  
		Size: 4.6 MB (4591622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c33193ffa3c81a2ebd95cb6af96ce80ee557191a64ba47e1977479e1167530ca`  
		Last Modified: Fri, 27 Aug 2021 00:20:19 GMT  
		Size: 1.7 KB (1701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c57e2e68d87e03a37f706b01fe403fc34435b82da71d1080e11ec9df4d418a2`  
		Last Modified: Fri, 27 Aug 2021 00:20:19 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:048b1707f600e77fb06d48bd9c3759cad471944658bdfa3dd59b2852dc7983b4`  
		Last Modified: Fri, 27 Aug 2021 00:20:20 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b434e68e7546ed285144b98ef8fc3a10f1b6ee578ef2503e9f09aefab0370d0`  
		Last Modified: Fri, 27 Aug 2021 00:20:20 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.4-nanoserver-1809`

```console
$ docker pull nats@sha256:21ff4cbb5485b408bcc030f341817018fb13a7381ca7c520960bf26bab74ddac
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2114; amd64

### `nats:2.4-nanoserver-1809` - windows version 10.0.17763.2114; amd64

```console
$ docker pull nats@sha256:9c370308b1924738df19dd502a9d8d8c13066580fd1550eddbf4f70663c87fe5
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.3 MB (107338949 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e90920ed24cf8337e7f99fdd7199bff8ec7dd43cfa5063f0f373e6700f8a17a2`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 05 Aug 2021 19:15:20 GMT
RUN Apply image 1809-amd64
# Wed, 25 Aug 2021 16:07:56 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 27 Aug 2021 00:16:45 GMT
RUN cmd /S /C #(nop) COPY file:bafd3fc1559b39648f01fab1b3b19a9fc9bb95afae5b07b1d7987b376806e053 in C:\nats-server.exe 
# Fri, 27 Aug 2021 00:16:46 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 27 Aug 2021 00:16:47 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Fri, 27 Aug 2021 00:16:47 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 27 Aug 2021 00:16:48 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:bc8517709e9cfff223cb034ff5be8fcbfa5409de286cdac9ae1b8878ebea6b84`  
		Size: 102.7 MB (102741177 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ae8616c17f5cca409a4b1289387e37dc532657ba2b52bb60713ff621acccd506`  
		Last Modified: Wed, 25 Aug 2021 16:11:20 GMT  
		Size: 1.0 KB (1022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb815244c76bae445a6697a3f1b6a0643fc016be2b2da5192dc6bb4079cd0119`  
		Last Modified: Fri, 27 Aug 2021 00:20:21 GMT  
		Size: 4.6 MB (4591622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c33193ffa3c81a2ebd95cb6af96ce80ee557191a64ba47e1977479e1167530ca`  
		Last Modified: Fri, 27 Aug 2021 00:20:19 GMT  
		Size: 1.7 KB (1701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c57e2e68d87e03a37f706b01fe403fc34435b82da71d1080e11ec9df4d418a2`  
		Last Modified: Fri, 27 Aug 2021 00:20:19 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:048b1707f600e77fb06d48bd9c3759cad471944658bdfa3dd59b2852dc7983b4`  
		Last Modified: Fri, 27 Aug 2021 00:20:20 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b434e68e7546ed285144b98ef8fc3a10f1b6ee578ef2503e9f09aefab0370d0`  
		Last Modified: Fri, 27 Aug 2021 00:20:20 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.4-scratch`

```console
$ docker pull nats@sha256:fb307cc8febb00cb2c4afd02e16ee319fa13c6471c8ed6543520f2a85f1ceda1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; arm variant v6

### `nats:2.4-scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:7201c8cd794776fa392c3a25eb89e4ee987aeaaae647caa364621d5daf5ca3c5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4201703 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc2211a135c8d5c9641c74ba5d54c3c1df4ac3f24fa70a6a57be8a2975af7854`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 02:48:56 GMT
COPY file:81d7dcb1f2223ae767ee02f3b24758797ca55a665d17dcb2054eeb097fb2eafa in /nats-server 
# Fri, 27 Aug 2021 02:48:56 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 27 Aug 2021 02:48:57 GMT
EXPOSE 4222 6222 8222
# Fri, 27 Aug 2021 02:48:57 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 27 Aug 2021 02:48:58 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a820d11a96d84195887c44533ffcad67997fcb79d52f4564709bfdbde47d578d`  
		Last Modified: Fri, 27 Aug 2021 02:51:18 GMT  
		Size: 4.2 MB (4201229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a1c4f82bf849dc3d9d18f1c560b9afd0e5237eb2f05377e6792dda2480249cb`  
		Last Modified: Fri, 27 Aug 2021 02:51:15 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.4-windowsservercore`

```console
$ docker pull nats@sha256:cf3aae4f841ee35ce5bfef42265fbd8025c1cff06d3f284e813cfec4cf9d6e4a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.2114; amd64
	-	windows version 10.0.14393.4583; amd64

### `nats:2.4-windowsservercore` - windows version 10.0.17763.2114; amd64

```console
$ docker pull nats@sha256:48cc63b49c047b98135531fccf1f7c4a418477d38def8702f6ecce6e8574923c
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2691328041 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09c3d57b266e04d58ceedd30a6c5428caa6783ca301ecc858c8aa62a8f682a3a`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 05 Aug 2021 19:44:34 GMT
RUN Install update 1809-amd64
# Wed, 25 Aug 2021 13:46:35 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 25 Aug 2021 16:05:30 GMT
ENV NATS_DOCKERIZED=1
# Fri, 27 Aug 2021 00:14:05 GMT
ENV NATS_SERVER=2.4.0
# Fri, 27 Aug 2021 00:14:06 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.4.0/nats-server-v2.4.0-windows-amd64.zip
# Fri, 27 Aug 2021 00:14:07 GMT
ENV NATS_SERVER_SHASUM=6c66acf5ed7e87a1ed9c499033c8c64c8c1365c5a95973ec57859abf1a69b032
# Fri, 27 Aug 2021 00:15:10 GMT
RUN Set-PSDebug -Trace 2
# Fri, 27 Aug 2021 00:16:22 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 27 Aug 2021 00:16:23 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 27 Aug 2021 00:16:24 GMT
EXPOSE 4222 6222 8222
# Fri, 27 Aug 2021 00:16:25 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 27 Aug 2021 00:16:26 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c67ded6868b61d392a0c096f911563fd6bc0bc3ed4fe401d077b3718a1b0cdaf`  
		Size: 967.7 MB (967665054 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:985da5cbc0735e1c422e766af23125ba345f431cb337ea43ec32298d0bb8e4ea`  
		Last Modified: Wed, 25 Aug 2021 15:45:02 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3dbdd68a4b0c278695b3e1d401d7eddfb0f0e3aa1e28aed88eb700059648f8f`  
		Last Modified: Wed, 25 Aug 2021 16:11:02 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9924833e15cbbaa8bd2d64c942c877c0765ba95d0790a5a9ea83a3d40bcaba43`  
		Last Modified: Fri, 27 Aug 2021 00:20:04 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93b8b51ab5e087ce5a5187d2967b0a82e4ce38b2151fc1b040be11a843334b1a`  
		Last Modified: Fri, 27 Aug 2021 00:20:00 GMT  
		Size: 1.4 KB (1360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73666a2686d6829048f4fa9f037f08038370c72202369f80bd4b715ead2cafe3`  
		Last Modified: Fri, 27 Aug 2021 00:20:00 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e35fdb95a7dc56c84ff744d8172574e2edd053f77affad83306be03c14fdb9fb`  
		Last Modified: Fri, 27 Aug 2021 00:20:01 GMT  
		Size: 372.5 KB (372513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3b9b9590a746c11677c6728f047f437a87645f68249b9691ed347591b850b8d`  
		Last Modified: Fri, 27 Aug 2021 00:20:00 GMT  
		Size: 4.9 MB (4944435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b629e22fb2c409b07df4f55a5b1c1d392ae3fc7110b646f46f63c8de8af0f470`  
		Last Modified: Fri, 27 Aug 2021 00:19:58 GMT  
		Size: 2.0 KB (1978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12c15056241134a8112b0c3e43493f7be7cd0421808ee5edbddb6490f355110e`  
		Last Modified: Fri, 27 Aug 2021 00:19:58 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27b1ee4ad1c87cc30317f9c2212c416f2a120923e62f8f88b8192c58d07a9dc1`  
		Last Modified: Fri, 27 Aug 2021 00:19:58 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1f840f93a8499fdb3efd112f5eedcef4290ba5edc497321ae223cdfc4dcb80e`  
		Last Modified: Fri, 27 Aug 2021 00:19:58 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.4-windowsservercore` - windows version 10.0.14393.4583; amd64

```console
$ docker pull nats@sha256:f6699a354c1c84d5ad72289d99c815e7bf11f983cd786684a5015745992e58e4
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6276264126 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af044355ba3348cfc4c9fb174c578e012f1a979a5d04b3681aafc9c2d9411eff`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Sun, 01 Aug 2021 08:52:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 25 Aug 2021 13:59:32 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 25 Aug 2021 16:08:06 GMT
ENV NATS_DOCKERIZED=1
# Fri, 27 Aug 2021 00:16:54 GMT
ENV NATS_SERVER=2.4.0
# Fri, 27 Aug 2021 00:16:55 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.4.0/nats-server-v2.4.0-windows-amd64.zip
# Fri, 27 Aug 2021 00:16:56 GMT
ENV NATS_SERVER_SHASUM=6c66acf5ed7e87a1ed9c499033c8c64c8c1365c5a95973ec57859abf1a69b032
# Fri, 27 Aug 2021 00:17:57 GMT
RUN Set-PSDebug -Trace 2
# Fri, 27 Aug 2021 00:19:20 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 27 Aug 2021 00:19:21 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 27 Aug 2021 00:19:21 GMT
EXPOSE 4222 6222 8222
# Fri, 27 Aug 2021 00:19:22 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 27 Aug 2021 00:19:23 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c427f892fe74603ae09d4e49b25f8f7046f957054034dc9f462e0e88d7bffaa5`  
		Size: 2.2 GB (2200980134 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a869803fc3d8292f0fe1bc6ed35e1ceedbd7c797a1486767a55f88c6c28ed4c5`  
		Last Modified: Wed, 25 Aug 2021 15:45:25 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a745f96c10790ef3a2006dbd4c116eb2f1552fd3c4a38fca179a8160e9918ac1`  
		Last Modified: Wed, 25 Aug 2021 16:11:42 GMT  
		Size: 1.3 KB (1329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ecbc2c744fbea737586b320c08b480fbd8eb2dc994300a74c6a4864ee082901`  
		Last Modified: Fri, 27 Aug 2021 00:20:37 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c530ba921538bcf67912fb5a5d6794e991501dbca08ae8137712fc58854f4f68`  
		Last Modified: Fri, 27 Aug 2021 00:20:37 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35523016d41ba152afbfa0a809770805058865f49d17d6d04d77fab412e5c29d`  
		Last Modified: Fri, 27 Aug 2021 00:20:37 GMT  
		Size: 1.4 KB (1383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:348276d7a124485ea8bc7bad9b9147c84dd20fda1da976a1542cbdb907e4ea95`  
		Last Modified: Fri, 27 Aug 2021 00:20:37 GMT  
		Size: 336.1 KB (336071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:751871e4a816cbaed81ad603047b0c9b536c2180dd5e54f7874d1ca37ef57851`  
		Last Modified: Fri, 27 Aug 2021 00:20:36 GMT  
		Size: 4.9 MB (4948899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d9507c0638be8fdbc5f10f76a31d751acfd94e02618ac7528b4856051bb3721`  
		Last Modified: Fri, 27 Aug 2021 00:20:35 GMT  
		Size: 2.0 KB (1979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:784f2e48cdd62d72893e3cf7316c3c7764e937b9ccade0cb0ce5547ee1e1a304`  
		Last Modified: Fri, 27 Aug 2021 00:20:35 GMT  
		Size: 1.4 KB (1357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc0ba660ed14d0923ea760b909e13fa4ff5bc4fe34acc4e9b0e5e072b2cd9704`  
		Last Modified: Fri, 27 Aug 2021 00:20:35 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f34329777aaf85af2b82ec6fa6640f757cc9589247f7fe67e427a4e39c19bda`  
		Last Modified: Fri, 27 Aug 2021 00:20:35 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.4-windowsservercore-1809`

```console
$ docker pull nats@sha256:a328e744c3a06f930890900c486761a97c2108563a63a093b1d0fc0fb9a1ad21
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2114; amd64

### `nats:2.4-windowsservercore-1809` - windows version 10.0.17763.2114; amd64

```console
$ docker pull nats@sha256:48cc63b49c047b98135531fccf1f7c4a418477d38def8702f6ecce6e8574923c
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2691328041 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09c3d57b266e04d58ceedd30a6c5428caa6783ca301ecc858c8aa62a8f682a3a`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 05 Aug 2021 19:44:34 GMT
RUN Install update 1809-amd64
# Wed, 25 Aug 2021 13:46:35 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 25 Aug 2021 16:05:30 GMT
ENV NATS_DOCKERIZED=1
# Fri, 27 Aug 2021 00:14:05 GMT
ENV NATS_SERVER=2.4.0
# Fri, 27 Aug 2021 00:14:06 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.4.0/nats-server-v2.4.0-windows-amd64.zip
# Fri, 27 Aug 2021 00:14:07 GMT
ENV NATS_SERVER_SHASUM=6c66acf5ed7e87a1ed9c499033c8c64c8c1365c5a95973ec57859abf1a69b032
# Fri, 27 Aug 2021 00:15:10 GMT
RUN Set-PSDebug -Trace 2
# Fri, 27 Aug 2021 00:16:22 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 27 Aug 2021 00:16:23 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 27 Aug 2021 00:16:24 GMT
EXPOSE 4222 6222 8222
# Fri, 27 Aug 2021 00:16:25 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 27 Aug 2021 00:16:26 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c67ded6868b61d392a0c096f911563fd6bc0bc3ed4fe401d077b3718a1b0cdaf`  
		Size: 967.7 MB (967665054 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:985da5cbc0735e1c422e766af23125ba345f431cb337ea43ec32298d0bb8e4ea`  
		Last Modified: Wed, 25 Aug 2021 15:45:02 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3dbdd68a4b0c278695b3e1d401d7eddfb0f0e3aa1e28aed88eb700059648f8f`  
		Last Modified: Wed, 25 Aug 2021 16:11:02 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9924833e15cbbaa8bd2d64c942c877c0765ba95d0790a5a9ea83a3d40bcaba43`  
		Last Modified: Fri, 27 Aug 2021 00:20:04 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93b8b51ab5e087ce5a5187d2967b0a82e4ce38b2151fc1b040be11a843334b1a`  
		Last Modified: Fri, 27 Aug 2021 00:20:00 GMT  
		Size: 1.4 KB (1360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73666a2686d6829048f4fa9f037f08038370c72202369f80bd4b715ead2cafe3`  
		Last Modified: Fri, 27 Aug 2021 00:20:00 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e35fdb95a7dc56c84ff744d8172574e2edd053f77affad83306be03c14fdb9fb`  
		Last Modified: Fri, 27 Aug 2021 00:20:01 GMT  
		Size: 372.5 KB (372513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3b9b9590a746c11677c6728f047f437a87645f68249b9691ed347591b850b8d`  
		Last Modified: Fri, 27 Aug 2021 00:20:00 GMT  
		Size: 4.9 MB (4944435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b629e22fb2c409b07df4f55a5b1c1d392ae3fc7110b646f46f63c8de8af0f470`  
		Last Modified: Fri, 27 Aug 2021 00:19:58 GMT  
		Size: 2.0 KB (1978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12c15056241134a8112b0c3e43493f7be7cd0421808ee5edbddb6490f355110e`  
		Last Modified: Fri, 27 Aug 2021 00:19:58 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27b1ee4ad1c87cc30317f9c2212c416f2a120923e62f8f88b8192c58d07a9dc1`  
		Last Modified: Fri, 27 Aug 2021 00:19:58 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1f840f93a8499fdb3efd112f5eedcef4290ba5edc497321ae223cdfc4dcb80e`  
		Last Modified: Fri, 27 Aug 2021 00:19:58 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.4-windowsservercore-ltsc2016`

```console
$ docker pull nats@sha256:7b1ad12d6c6e44e24975eb80e1111d97db29e82416a00dadd5e14a67bf6c0ae4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.14393.4583; amd64

### `nats:2.4-windowsservercore-ltsc2016` - windows version 10.0.14393.4583; amd64

```console
$ docker pull nats@sha256:f6699a354c1c84d5ad72289d99c815e7bf11f983cd786684a5015745992e58e4
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6276264126 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af044355ba3348cfc4c9fb174c578e012f1a979a5d04b3681aafc9c2d9411eff`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Sun, 01 Aug 2021 08:52:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 25 Aug 2021 13:59:32 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 25 Aug 2021 16:08:06 GMT
ENV NATS_DOCKERIZED=1
# Fri, 27 Aug 2021 00:16:54 GMT
ENV NATS_SERVER=2.4.0
# Fri, 27 Aug 2021 00:16:55 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.4.0/nats-server-v2.4.0-windows-amd64.zip
# Fri, 27 Aug 2021 00:16:56 GMT
ENV NATS_SERVER_SHASUM=6c66acf5ed7e87a1ed9c499033c8c64c8c1365c5a95973ec57859abf1a69b032
# Fri, 27 Aug 2021 00:17:57 GMT
RUN Set-PSDebug -Trace 2
# Fri, 27 Aug 2021 00:19:20 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 27 Aug 2021 00:19:21 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 27 Aug 2021 00:19:21 GMT
EXPOSE 4222 6222 8222
# Fri, 27 Aug 2021 00:19:22 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 27 Aug 2021 00:19:23 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c427f892fe74603ae09d4e49b25f8f7046f957054034dc9f462e0e88d7bffaa5`  
		Size: 2.2 GB (2200980134 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a869803fc3d8292f0fe1bc6ed35e1ceedbd7c797a1486767a55f88c6c28ed4c5`  
		Last Modified: Wed, 25 Aug 2021 15:45:25 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a745f96c10790ef3a2006dbd4c116eb2f1552fd3c4a38fca179a8160e9918ac1`  
		Last Modified: Wed, 25 Aug 2021 16:11:42 GMT  
		Size: 1.3 KB (1329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ecbc2c744fbea737586b320c08b480fbd8eb2dc994300a74c6a4864ee082901`  
		Last Modified: Fri, 27 Aug 2021 00:20:37 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c530ba921538bcf67912fb5a5d6794e991501dbca08ae8137712fc58854f4f68`  
		Last Modified: Fri, 27 Aug 2021 00:20:37 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35523016d41ba152afbfa0a809770805058865f49d17d6d04d77fab412e5c29d`  
		Last Modified: Fri, 27 Aug 2021 00:20:37 GMT  
		Size: 1.4 KB (1383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:348276d7a124485ea8bc7bad9b9147c84dd20fda1da976a1542cbdb907e4ea95`  
		Last Modified: Fri, 27 Aug 2021 00:20:37 GMT  
		Size: 336.1 KB (336071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:751871e4a816cbaed81ad603047b0c9b536c2180dd5e54f7874d1ca37ef57851`  
		Last Modified: Fri, 27 Aug 2021 00:20:36 GMT  
		Size: 4.9 MB (4948899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d9507c0638be8fdbc5f10f76a31d751acfd94e02618ac7528b4856051bb3721`  
		Last Modified: Fri, 27 Aug 2021 00:20:35 GMT  
		Size: 2.0 KB (1979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:784f2e48cdd62d72893e3cf7316c3c7764e937b9ccade0cb0ce5547ee1e1a304`  
		Last Modified: Fri, 27 Aug 2021 00:20:35 GMT  
		Size: 1.4 KB (1357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc0ba660ed14d0923ea760b909e13fa4ff5bc4fe34acc4e9b0e5e072b2cd9704`  
		Last Modified: Fri, 27 Aug 2021 00:20:35 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f34329777aaf85af2b82ec6fa6640f757cc9589247f7fe67e427a4e39c19bda`  
		Last Modified: Fri, 27 Aug 2021 00:20:35 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.4.0`

```console
$ docker pull nats@sha256:eda69a4b9a9b99aa00804bc7d0a440ff4811b9abf067e6d6bf92ddb98d3a0a7a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; arm variant v6
	-	windows version 10.0.17763.2114; amd64

### `nats:2.4.0` - linux; arm variant v6

```console
$ docker pull nats@sha256:7201c8cd794776fa392c3a25eb89e4ee987aeaaae647caa364621d5daf5ca3c5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4201703 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc2211a135c8d5c9641c74ba5d54c3c1df4ac3f24fa70a6a57be8a2975af7854`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 02:48:56 GMT
COPY file:81d7dcb1f2223ae767ee02f3b24758797ca55a665d17dcb2054eeb097fb2eafa in /nats-server 
# Fri, 27 Aug 2021 02:48:56 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 27 Aug 2021 02:48:57 GMT
EXPOSE 4222 6222 8222
# Fri, 27 Aug 2021 02:48:57 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 27 Aug 2021 02:48:58 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a820d11a96d84195887c44533ffcad67997fcb79d52f4564709bfdbde47d578d`  
		Last Modified: Fri, 27 Aug 2021 02:51:18 GMT  
		Size: 4.2 MB (4201229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a1c4f82bf849dc3d9d18f1c560b9afd0e5237eb2f05377e6792dda2480249cb`  
		Last Modified: Fri, 27 Aug 2021 02:51:15 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.4.0` - windows version 10.0.17763.2114; amd64

```console
$ docker pull nats@sha256:9c370308b1924738df19dd502a9d8d8c13066580fd1550eddbf4f70663c87fe5
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.3 MB (107338949 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e90920ed24cf8337e7f99fdd7199bff8ec7dd43cfa5063f0f373e6700f8a17a2`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 05 Aug 2021 19:15:20 GMT
RUN Apply image 1809-amd64
# Wed, 25 Aug 2021 16:07:56 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 27 Aug 2021 00:16:45 GMT
RUN cmd /S /C #(nop) COPY file:bafd3fc1559b39648f01fab1b3b19a9fc9bb95afae5b07b1d7987b376806e053 in C:\nats-server.exe 
# Fri, 27 Aug 2021 00:16:46 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 27 Aug 2021 00:16:47 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Fri, 27 Aug 2021 00:16:47 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 27 Aug 2021 00:16:48 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:bc8517709e9cfff223cb034ff5be8fcbfa5409de286cdac9ae1b8878ebea6b84`  
		Size: 102.7 MB (102741177 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ae8616c17f5cca409a4b1289387e37dc532657ba2b52bb60713ff621acccd506`  
		Last Modified: Wed, 25 Aug 2021 16:11:20 GMT  
		Size: 1.0 KB (1022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb815244c76bae445a6697a3f1b6a0643fc016be2b2da5192dc6bb4079cd0119`  
		Last Modified: Fri, 27 Aug 2021 00:20:21 GMT  
		Size: 4.6 MB (4591622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c33193ffa3c81a2ebd95cb6af96ce80ee557191a64ba47e1977479e1167530ca`  
		Last Modified: Fri, 27 Aug 2021 00:20:19 GMT  
		Size: 1.7 KB (1701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c57e2e68d87e03a37f706b01fe403fc34435b82da71d1080e11ec9df4d418a2`  
		Last Modified: Fri, 27 Aug 2021 00:20:19 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:048b1707f600e77fb06d48bd9c3759cad471944658bdfa3dd59b2852dc7983b4`  
		Last Modified: Fri, 27 Aug 2021 00:20:20 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b434e68e7546ed285144b98ef8fc3a10f1b6ee578ef2503e9f09aefab0370d0`  
		Last Modified: Fri, 27 Aug 2021 00:20:20 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.4.0-alpine`

```console
$ docker pull nats@sha256:22cb5ac9807b2cae3bef4c860bd2941c6fdf66eec3ddfff985666eeeffe78e39
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; arm variant v6

### `nats:2.4.0-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:e995bfdd6f9247dbf1b305adc029a95e72e8630251d8d19a9023c63dcbc47318
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7109895 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aae75c35e1d2e6f686fde0a0cfaea0aff2d58dcdf3e52a8ecba5ffc3dea3fe0b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 06 Aug 2021 17:49:32 GMT
ADD file:7f2c7deda009eabdcbbdccb11e854043d32c498e64e7e1ca02165d7bb4261d39 in / 
# Fri, 06 Aug 2021 17:49:32 GMT
CMD ["/bin/sh"]
# Fri, 27 Aug 2021 02:48:29 GMT
ENV NATS_SERVER=2.4.0
# Fri, 27 Aug 2021 02:48:34 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='eb510dd016cb1a9e9b1fae88a3471029048cb75dcc4ad83a4f5b1e3665f24a20' ;; 		armhf) natsArch='arm6'; sha256='76ac66cd86217a43bc227220eb054aac8a5744890d43c76156075d68a684d9e0' ;; 		armv7) natsArch='arm7'; sha256='e7521841d59f55fcef6172aa8f22d3af7ba1776bd67109a23c29d34d18d44bd6' ;; 		x86_64) natsArch='amd64'; sha256='f6841c89fcf99302bc7ac295ddc1e75322385f861d55abee79733976c8eb9bc7' ;; 		x86) natsArch='386'; sha256='c7e6e2b73d402e841b3abb57e26e2ef53350b44e385255bf289b08182058076a' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 27 Aug 2021 02:48:34 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 27 Aug 2021 02:48:35 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 27 Aug 2021 02:48:35 GMT
EXPOSE 4222 6222 8222
# Fri, 27 Aug 2021 02:48:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 Aug 2021 02:48:36 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:f465bb3e9fcd0c42f936ecc566c6e40353c00f3089b2b2c2ea1663c30f89d3ab`  
		Last Modified: Fri, 06 Aug 2021 17:51:00 GMT  
		Size: 2.6 MB (2626350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5abfce067d7bc34edb53d2ef3b851fb6750f2f165d88e6b7c1751a372637cf9`  
		Last Modified: Fri, 27 Aug 2021 02:50:40 GMT  
		Size: 4.5 MB (4482575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:915f8f45a2be36433373b63850ff3ca8ec9eb622ab7d74dd908284a971539307`  
		Last Modified: Fri, 27 Aug 2021 02:50:38 GMT  
		Size: 557.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dcbfc2ac16592f5503b1b3f59404245367a0082b75af6bd79a2b48e8c45a762`  
		Last Modified: Fri, 27 Aug 2021 02:50:38 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.4.0-alpine3.14`

```console
$ docker pull nats@sha256:22cb5ac9807b2cae3bef4c860bd2941c6fdf66eec3ddfff985666eeeffe78e39
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; arm variant v6

### `nats:2.4.0-alpine3.14` - linux; arm variant v6

```console
$ docker pull nats@sha256:e995bfdd6f9247dbf1b305adc029a95e72e8630251d8d19a9023c63dcbc47318
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7109895 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aae75c35e1d2e6f686fde0a0cfaea0aff2d58dcdf3e52a8ecba5ffc3dea3fe0b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 06 Aug 2021 17:49:32 GMT
ADD file:7f2c7deda009eabdcbbdccb11e854043d32c498e64e7e1ca02165d7bb4261d39 in / 
# Fri, 06 Aug 2021 17:49:32 GMT
CMD ["/bin/sh"]
# Fri, 27 Aug 2021 02:48:29 GMT
ENV NATS_SERVER=2.4.0
# Fri, 27 Aug 2021 02:48:34 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='eb510dd016cb1a9e9b1fae88a3471029048cb75dcc4ad83a4f5b1e3665f24a20' ;; 		armhf) natsArch='arm6'; sha256='76ac66cd86217a43bc227220eb054aac8a5744890d43c76156075d68a684d9e0' ;; 		armv7) natsArch='arm7'; sha256='e7521841d59f55fcef6172aa8f22d3af7ba1776bd67109a23c29d34d18d44bd6' ;; 		x86_64) natsArch='amd64'; sha256='f6841c89fcf99302bc7ac295ddc1e75322385f861d55abee79733976c8eb9bc7' ;; 		x86) natsArch='386'; sha256='c7e6e2b73d402e841b3abb57e26e2ef53350b44e385255bf289b08182058076a' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 27 Aug 2021 02:48:34 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 27 Aug 2021 02:48:35 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 27 Aug 2021 02:48:35 GMT
EXPOSE 4222 6222 8222
# Fri, 27 Aug 2021 02:48:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 Aug 2021 02:48:36 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:f465bb3e9fcd0c42f936ecc566c6e40353c00f3089b2b2c2ea1663c30f89d3ab`  
		Last Modified: Fri, 06 Aug 2021 17:51:00 GMT  
		Size: 2.6 MB (2626350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5abfce067d7bc34edb53d2ef3b851fb6750f2f165d88e6b7c1751a372637cf9`  
		Last Modified: Fri, 27 Aug 2021 02:50:40 GMT  
		Size: 4.5 MB (4482575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:915f8f45a2be36433373b63850ff3ca8ec9eb622ab7d74dd908284a971539307`  
		Last Modified: Fri, 27 Aug 2021 02:50:38 GMT  
		Size: 557.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dcbfc2ac16592f5503b1b3f59404245367a0082b75af6bd79a2b48e8c45a762`  
		Last Modified: Fri, 27 Aug 2021 02:50:38 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.4.0-linux`

```console
$ docker pull nats@sha256:fb307cc8febb00cb2c4afd02e16ee319fa13c6471c8ed6543520f2a85f1ceda1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; arm variant v6

### `nats:2.4.0-linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:7201c8cd794776fa392c3a25eb89e4ee987aeaaae647caa364621d5daf5ca3c5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4201703 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc2211a135c8d5c9641c74ba5d54c3c1df4ac3f24fa70a6a57be8a2975af7854`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 02:48:56 GMT
COPY file:81d7dcb1f2223ae767ee02f3b24758797ca55a665d17dcb2054eeb097fb2eafa in /nats-server 
# Fri, 27 Aug 2021 02:48:56 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 27 Aug 2021 02:48:57 GMT
EXPOSE 4222 6222 8222
# Fri, 27 Aug 2021 02:48:57 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 27 Aug 2021 02:48:58 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a820d11a96d84195887c44533ffcad67997fcb79d52f4564709bfdbde47d578d`  
		Last Modified: Fri, 27 Aug 2021 02:51:18 GMT  
		Size: 4.2 MB (4201229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a1c4f82bf849dc3d9d18f1c560b9afd0e5237eb2f05377e6792dda2480249cb`  
		Last Modified: Fri, 27 Aug 2021 02:51:15 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.4.0-nanoserver`

```console
$ docker pull nats@sha256:21ff4cbb5485b408bcc030f341817018fb13a7381ca7c520960bf26bab74ddac
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2114; amd64

### `nats:2.4.0-nanoserver` - windows version 10.0.17763.2114; amd64

```console
$ docker pull nats@sha256:9c370308b1924738df19dd502a9d8d8c13066580fd1550eddbf4f70663c87fe5
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.3 MB (107338949 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e90920ed24cf8337e7f99fdd7199bff8ec7dd43cfa5063f0f373e6700f8a17a2`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 05 Aug 2021 19:15:20 GMT
RUN Apply image 1809-amd64
# Wed, 25 Aug 2021 16:07:56 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 27 Aug 2021 00:16:45 GMT
RUN cmd /S /C #(nop) COPY file:bafd3fc1559b39648f01fab1b3b19a9fc9bb95afae5b07b1d7987b376806e053 in C:\nats-server.exe 
# Fri, 27 Aug 2021 00:16:46 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 27 Aug 2021 00:16:47 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Fri, 27 Aug 2021 00:16:47 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 27 Aug 2021 00:16:48 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:bc8517709e9cfff223cb034ff5be8fcbfa5409de286cdac9ae1b8878ebea6b84`  
		Size: 102.7 MB (102741177 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ae8616c17f5cca409a4b1289387e37dc532657ba2b52bb60713ff621acccd506`  
		Last Modified: Wed, 25 Aug 2021 16:11:20 GMT  
		Size: 1.0 KB (1022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb815244c76bae445a6697a3f1b6a0643fc016be2b2da5192dc6bb4079cd0119`  
		Last Modified: Fri, 27 Aug 2021 00:20:21 GMT  
		Size: 4.6 MB (4591622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c33193ffa3c81a2ebd95cb6af96ce80ee557191a64ba47e1977479e1167530ca`  
		Last Modified: Fri, 27 Aug 2021 00:20:19 GMT  
		Size: 1.7 KB (1701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c57e2e68d87e03a37f706b01fe403fc34435b82da71d1080e11ec9df4d418a2`  
		Last Modified: Fri, 27 Aug 2021 00:20:19 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:048b1707f600e77fb06d48bd9c3759cad471944658bdfa3dd59b2852dc7983b4`  
		Last Modified: Fri, 27 Aug 2021 00:20:20 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b434e68e7546ed285144b98ef8fc3a10f1b6ee578ef2503e9f09aefab0370d0`  
		Last Modified: Fri, 27 Aug 2021 00:20:20 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.4.0-nanoserver-1809`

```console
$ docker pull nats@sha256:21ff4cbb5485b408bcc030f341817018fb13a7381ca7c520960bf26bab74ddac
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2114; amd64

### `nats:2.4.0-nanoserver-1809` - windows version 10.0.17763.2114; amd64

```console
$ docker pull nats@sha256:9c370308b1924738df19dd502a9d8d8c13066580fd1550eddbf4f70663c87fe5
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.3 MB (107338949 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e90920ed24cf8337e7f99fdd7199bff8ec7dd43cfa5063f0f373e6700f8a17a2`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 05 Aug 2021 19:15:20 GMT
RUN Apply image 1809-amd64
# Wed, 25 Aug 2021 16:07:56 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 27 Aug 2021 00:16:45 GMT
RUN cmd /S /C #(nop) COPY file:bafd3fc1559b39648f01fab1b3b19a9fc9bb95afae5b07b1d7987b376806e053 in C:\nats-server.exe 
# Fri, 27 Aug 2021 00:16:46 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 27 Aug 2021 00:16:47 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Fri, 27 Aug 2021 00:16:47 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 27 Aug 2021 00:16:48 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:bc8517709e9cfff223cb034ff5be8fcbfa5409de286cdac9ae1b8878ebea6b84`  
		Size: 102.7 MB (102741177 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ae8616c17f5cca409a4b1289387e37dc532657ba2b52bb60713ff621acccd506`  
		Last Modified: Wed, 25 Aug 2021 16:11:20 GMT  
		Size: 1.0 KB (1022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb815244c76bae445a6697a3f1b6a0643fc016be2b2da5192dc6bb4079cd0119`  
		Last Modified: Fri, 27 Aug 2021 00:20:21 GMT  
		Size: 4.6 MB (4591622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c33193ffa3c81a2ebd95cb6af96ce80ee557191a64ba47e1977479e1167530ca`  
		Last Modified: Fri, 27 Aug 2021 00:20:19 GMT  
		Size: 1.7 KB (1701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c57e2e68d87e03a37f706b01fe403fc34435b82da71d1080e11ec9df4d418a2`  
		Last Modified: Fri, 27 Aug 2021 00:20:19 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:048b1707f600e77fb06d48bd9c3759cad471944658bdfa3dd59b2852dc7983b4`  
		Last Modified: Fri, 27 Aug 2021 00:20:20 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b434e68e7546ed285144b98ef8fc3a10f1b6ee578ef2503e9f09aefab0370d0`  
		Last Modified: Fri, 27 Aug 2021 00:20:20 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.4.0-scratch`

```console
$ docker pull nats@sha256:fb307cc8febb00cb2c4afd02e16ee319fa13c6471c8ed6543520f2a85f1ceda1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; arm variant v6

### `nats:2.4.0-scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:7201c8cd794776fa392c3a25eb89e4ee987aeaaae647caa364621d5daf5ca3c5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4201703 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc2211a135c8d5c9641c74ba5d54c3c1df4ac3f24fa70a6a57be8a2975af7854`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 02:48:56 GMT
COPY file:81d7dcb1f2223ae767ee02f3b24758797ca55a665d17dcb2054eeb097fb2eafa in /nats-server 
# Fri, 27 Aug 2021 02:48:56 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 27 Aug 2021 02:48:57 GMT
EXPOSE 4222 6222 8222
# Fri, 27 Aug 2021 02:48:57 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 27 Aug 2021 02:48:58 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a820d11a96d84195887c44533ffcad67997fcb79d52f4564709bfdbde47d578d`  
		Last Modified: Fri, 27 Aug 2021 02:51:18 GMT  
		Size: 4.2 MB (4201229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a1c4f82bf849dc3d9d18f1c560b9afd0e5237eb2f05377e6792dda2480249cb`  
		Last Modified: Fri, 27 Aug 2021 02:51:15 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.4.0-windowsservercore`

```console
$ docker pull nats@sha256:cf3aae4f841ee35ce5bfef42265fbd8025c1cff06d3f284e813cfec4cf9d6e4a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.2114; amd64
	-	windows version 10.0.14393.4583; amd64

### `nats:2.4.0-windowsservercore` - windows version 10.0.17763.2114; amd64

```console
$ docker pull nats@sha256:48cc63b49c047b98135531fccf1f7c4a418477d38def8702f6ecce6e8574923c
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2691328041 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09c3d57b266e04d58ceedd30a6c5428caa6783ca301ecc858c8aa62a8f682a3a`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 05 Aug 2021 19:44:34 GMT
RUN Install update 1809-amd64
# Wed, 25 Aug 2021 13:46:35 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 25 Aug 2021 16:05:30 GMT
ENV NATS_DOCKERIZED=1
# Fri, 27 Aug 2021 00:14:05 GMT
ENV NATS_SERVER=2.4.0
# Fri, 27 Aug 2021 00:14:06 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.4.0/nats-server-v2.4.0-windows-amd64.zip
# Fri, 27 Aug 2021 00:14:07 GMT
ENV NATS_SERVER_SHASUM=6c66acf5ed7e87a1ed9c499033c8c64c8c1365c5a95973ec57859abf1a69b032
# Fri, 27 Aug 2021 00:15:10 GMT
RUN Set-PSDebug -Trace 2
# Fri, 27 Aug 2021 00:16:22 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 27 Aug 2021 00:16:23 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 27 Aug 2021 00:16:24 GMT
EXPOSE 4222 6222 8222
# Fri, 27 Aug 2021 00:16:25 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 27 Aug 2021 00:16:26 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c67ded6868b61d392a0c096f911563fd6bc0bc3ed4fe401d077b3718a1b0cdaf`  
		Size: 967.7 MB (967665054 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:985da5cbc0735e1c422e766af23125ba345f431cb337ea43ec32298d0bb8e4ea`  
		Last Modified: Wed, 25 Aug 2021 15:45:02 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3dbdd68a4b0c278695b3e1d401d7eddfb0f0e3aa1e28aed88eb700059648f8f`  
		Last Modified: Wed, 25 Aug 2021 16:11:02 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9924833e15cbbaa8bd2d64c942c877c0765ba95d0790a5a9ea83a3d40bcaba43`  
		Last Modified: Fri, 27 Aug 2021 00:20:04 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93b8b51ab5e087ce5a5187d2967b0a82e4ce38b2151fc1b040be11a843334b1a`  
		Last Modified: Fri, 27 Aug 2021 00:20:00 GMT  
		Size: 1.4 KB (1360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73666a2686d6829048f4fa9f037f08038370c72202369f80bd4b715ead2cafe3`  
		Last Modified: Fri, 27 Aug 2021 00:20:00 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e35fdb95a7dc56c84ff744d8172574e2edd053f77affad83306be03c14fdb9fb`  
		Last Modified: Fri, 27 Aug 2021 00:20:01 GMT  
		Size: 372.5 KB (372513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3b9b9590a746c11677c6728f047f437a87645f68249b9691ed347591b850b8d`  
		Last Modified: Fri, 27 Aug 2021 00:20:00 GMT  
		Size: 4.9 MB (4944435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b629e22fb2c409b07df4f55a5b1c1d392ae3fc7110b646f46f63c8de8af0f470`  
		Last Modified: Fri, 27 Aug 2021 00:19:58 GMT  
		Size: 2.0 KB (1978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12c15056241134a8112b0c3e43493f7be7cd0421808ee5edbddb6490f355110e`  
		Last Modified: Fri, 27 Aug 2021 00:19:58 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27b1ee4ad1c87cc30317f9c2212c416f2a120923e62f8f88b8192c58d07a9dc1`  
		Last Modified: Fri, 27 Aug 2021 00:19:58 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1f840f93a8499fdb3efd112f5eedcef4290ba5edc497321ae223cdfc4dcb80e`  
		Last Modified: Fri, 27 Aug 2021 00:19:58 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.4.0-windowsservercore` - windows version 10.0.14393.4583; amd64

```console
$ docker pull nats@sha256:f6699a354c1c84d5ad72289d99c815e7bf11f983cd786684a5015745992e58e4
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6276264126 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af044355ba3348cfc4c9fb174c578e012f1a979a5d04b3681aafc9c2d9411eff`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Sun, 01 Aug 2021 08:52:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 25 Aug 2021 13:59:32 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 25 Aug 2021 16:08:06 GMT
ENV NATS_DOCKERIZED=1
# Fri, 27 Aug 2021 00:16:54 GMT
ENV NATS_SERVER=2.4.0
# Fri, 27 Aug 2021 00:16:55 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.4.0/nats-server-v2.4.0-windows-amd64.zip
# Fri, 27 Aug 2021 00:16:56 GMT
ENV NATS_SERVER_SHASUM=6c66acf5ed7e87a1ed9c499033c8c64c8c1365c5a95973ec57859abf1a69b032
# Fri, 27 Aug 2021 00:17:57 GMT
RUN Set-PSDebug -Trace 2
# Fri, 27 Aug 2021 00:19:20 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 27 Aug 2021 00:19:21 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 27 Aug 2021 00:19:21 GMT
EXPOSE 4222 6222 8222
# Fri, 27 Aug 2021 00:19:22 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 27 Aug 2021 00:19:23 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c427f892fe74603ae09d4e49b25f8f7046f957054034dc9f462e0e88d7bffaa5`  
		Size: 2.2 GB (2200980134 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a869803fc3d8292f0fe1bc6ed35e1ceedbd7c797a1486767a55f88c6c28ed4c5`  
		Last Modified: Wed, 25 Aug 2021 15:45:25 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a745f96c10790ef3a2006dbd4c116eb2f1552fd3c4a38fca179a8160e9918ac1`  
		Last Modified: Wed, 25 Aug 2021 16:11:42 GMT  
		Size: 1.3 KB (1329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ecbc2c744fbea737586b320c08b480fbd8eb2dc994300a74c6a4864ee082901`  
		Last Modified: Fri, 27 Aug 2021 00:20:37 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c530ba921538bcf67912fb5a5d6794e991501dbca08ae8137712fc58854f4f68`  
		Last Modified: Fri, 27 Aug 2021 00:20:37 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35523016d41ba152afbfa0a809770805058865f49d17d6d04d77fab412e5c29d`  
		Last Modified: Fri, 27 Aug 2021 00:20:37 GMT  
		Size: 1.4 KB (1383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:348276d7a124485ea8bc7bad9b9147c84dd20fda1da976a1542cbdb907e4ea95`  
		Last Modified: Fri, 27 Aug 2021 00:20:37 GMT  
		Size: 336.1 KB (336071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:751871e4a816cbaed81ad603047b0c9b536c2180dd5e54f7874d1ca37ef57851`  
		Last Modified: Fri, 27 Aug 2021 00:20:36 GMT  
		Size: 4.9 MB (4948899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d9507c0638be8fdbc5f10f76a31d751acfd94e02618ac7528b4856051bb3721`  
		Last Modified: Fri, 27 Aug 2021 00:20:35 GMT  
		Size: 2.0 KB (1979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:784f2e48cdd62d72893e3cf7316c3c7764e937b9ccade0cb0ce5547ee1e1a304`  
		Last Modified: Fri, 27 Aug 2021 00:20:35 GMT  
		Size: 1.4 KB (1357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc0ba660ed14d0923ea760b909e13fa4ff5bc4fe34acc4e9b0e5e072b2cd9704`  
		Last Modified: Fri, 27 Aug 2021 00:20:35 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f34329777aaf85af2b82ec6fa6640f757cc9589247f7fe67e427a4e39c19bda`  
		Last Modified: Fri, 27 Aug 2021 00:20:35 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.4.0-windowsservercore-1809`

```console
$ docker pull nats@sha256:a328e744c3a06f930890900c486761a97c2108563a63a093b1d0fc0fb9a1ad21
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2114; amd64

### `nats:2.4.0-windowsservercore-1809` - windows version 10.0.17763.2114; amd64

```console
$ docker pull nats@sha256:48cc63b49c047b98135531fccf1f7c4a418477d38def8702f6ecce6e8574923c
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2691328041 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09c3d57b266e04d58ceedd30a6c5428caa6783ca301ecc858c8aa62a8f682a3a`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 05 Aug 2021 19:44:34 GMT
RUN Install update 1809-amd64
# Wed, 25 Aug 2021 13:46:35 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 25 Aug 2021 16:05:30 GMT
ENV NATS_DOCKERIZED=1
# Fri, 27 Aug 2021 00:14:05 GMT
ENV NATS_SERVER=2.4.0
# Fri, 27 Aug 2021 00:14:06 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.4.0/nats-server-v2.4.0-windows-amd64.zip
# Fri, 27 Aug 2021 00:14:07 GMT
ENV NATS_SERVER_SHASUM=6c66acf5ed7e87a1ed9c499033c8c64c8c1365c5a95973ec57859abf1a69b032
# Fri, 27 Aug 2021 00:15:10 GMT
RUN Set-PSDebug -Trace 2
# Fri, 27 Aug 2021 00:16:22 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 27 Aug 2021 00:16:23 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 27 Aug 2021 00:16:24 GMT
EXPOSE 4222 6222 8222
# Fri, 27 Aug 2021 00:16:25 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 27 Aug 2021 00:16:26 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c67ded6868b61d392a0c096f911563fd6bc0bc3ed4fe401d077b3718a1b0cdaf`  
		Size: 967.7 MB (967665054 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:985da5cbc0735e1c422e766af23125ba345f431cb337ea43ec32298d0bb8e4ea`  
		Last Modified: Wed, 25 Aug 2021 15:45:02 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3dbdd68a4b0c278695b3e1d401d7eddfb0f0e3aa1e28aed88eb700059648f8f`  
		Last Modified: Wed, 25 Aug 2021 16:11:02 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9924833e15cbbaa8bd2d64c942c877c0765ba95d0790a5a9ea83a3d40bcaba43`  
		Last Modified: Fri, 27 Aug 2021 00:20:04 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93b8b51ab5e087ce5a5187d2967b0a82e4ce38b2151fc1b040be11a843334b1a`  
		Last Modified: Fri, 27 Aug 2021 00:20:00 GMT  
		Size: 1.4 KB (1360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73666a2686d6829048f4fa9f037f08038370c72202369f80bd4b715ead2cafe3`  
		Last Modified: Fri, 27 Aug 2021 00:20:00 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e35fdb95a7dc56c84ff744d8172574e2edd053f77affad83306be03c14fdb9fb`  
		Last Modified: Fri, 27 Aug 2021 00:20:01 GMT  
		Size: 372.5 KB (372513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3b9b9590a746c11677c6728f047f437a87645f68249b9691ed347591b850b8d`  
		Last Modified: Fri, 27 Aug 2021 00:20:00 GMT  
		Size: 4.9 MB (4944435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b629e22fb2c409b07df4f55a5b1c1d392ae3fc7110b646f46f63c8de8af0f470`  
		Last Modified: Fri, 27 Aug 2021 00:19:58 GMT  
		Size: 2.0 KB (1978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12c15056241134a8112b0c3e43493f7be7cd0421808ee5edbddb6490f355110e`  
		Last Modified: Fri, 27 Aug 2021 00:19:58 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27b1ee4ad1c87cc30317f9c2212c416f2a120923e62f8f88b8192c58d07a9dc1`  
		Last Modified: Fri, 27 Aug 2021 00:19:58 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1f840f93a8499fdb3efd112f5eedcef4290ba5edc497321ae223cdfc4dcb80e`  
		Last Modified: Fri, 27 Aug 2021 00:19:58 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.4.0-windowsservercore-ltsc2016`

```console
$ docker pull nats@sha256:7b1ad12d6c6e44e24975eb80e1111d97db29e82416a00dadd5e14a67bf6c0ae4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.14393.4583; amd64

### `nats:2.4.0-windowsservercore-ltsc2016` - windows version 10.0.14393.4583; amd64

```console
$ docker pull nats@sha256:f6699a354c1c84d5ad72289d99c815e7bf11f983cd786684a5015745992e58e4
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6276264126 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af044355ba3348cfc4c9fb174c578e012f1a979a5d04b3681aafc9c2d9411eff`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Sun, 01 Aug 2021 08:52:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 25 Aug 2021 13:59:32 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 25 Aug 2021 16:08:06 GMT
ENV NATS_DOCKERIZED=1
# Fri, 27 Aug 2021 00:16:54 GMT
ENV NATS_SERVER=2.4.0
# Fri, 27 Aug 2021 00:16:55 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.4.0/nats-server-v2.4.0-windows-amd64.zip
# Fri, 27 Aug 2021 00:16:56 GMT
ENV NATS_SERVER_SHASUM=6c66acf5ed7e87a1ed9c499033c8c64c8c1365c5a95973ec57859abf1a69b032
# Fri, 27 Aug 2021 00:17:57 GMT
RUN Set-PSDebug -Trace 2
# Fri, 27 Aug 2021 00:19:20 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 27 Aug 2021 00:19:21 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 27 Aug 2021 00:19:21 GMT
EXPOSE 4222 6222 8222
# Fri, 27 Aug 2021 00:19:22 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 27 Aug 2021 00:19:23 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c427f892fe74603ae09d4e49b25f8f7046f957054034dc9f462e0e88d7bffaa5`  
		Size: 2.2 GB (2200980134 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a869803fc3d8292f0fe1bc6ed35e1ceedbd7c797a1486767a55f88c6c28ed4c5`  
		Last Modified: Wed, 25 Aug 2021 15:45:25 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a745f96c10790ef3a2006dbd4c116eb2f1552fd3c4a38fca179a8160e9918ac1`  
		Last Modified: Wed, 25 Aug 2021 16:11:42 GMT  
		Size: 1.3 KB (1329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ecbc2c744fbea737586b320c08b480fbd8eb2dc994300a74c6a4864ee082901`  
		Last Modified: Fri, 27 Aug 2021 00:20:37 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c530ba921538bcf67912fb5a5d6794e991501dbca08ae8137712fc58854f4f68`  
		Last Modified: Fri, 27 Aug 2021 00:20:37 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35523016d41ba152afbfa0a809770805058865f49d17d6d04d77fab412e5c29d`  
		Last Modified: Fri, 27 Aug 2021 00:20:37 GMT  
		Size: 1.4 KB (1383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:348276d7a124485ea8bc7bad9b9147c84dd20fda1da976a1542cbdb907e4ea95`  
		Last Modified: Fri, 27 Aug 2021 00:20:37 GMT  
		Size: 336.1 KB (336071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:751871e4a816cbaed81ad603047b0c9b536c2180dd5e54f7874d1ca37ef57851`  
		Last Modified: Fri, 27 Aug 2021 00:20:36 GMT  
		Size: 4.9 MB (4948899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d9507c0638be8fdbc5f10f76a31d751acfd94e02618ac7528b4856051bb3721`  
		Last Modified: Fri, 27 Aug 2021 00:20:35 GMT  
		Size: 2.0 KB (1979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:784f2e48cdd62d72893e3cf7316c3c7764e937b9ccade0cb0ce5547ee1e1a304`  
		Last Modified: Fri, 27 Aug 2021 00:20:35 GMT  
		Size: 1.4 KB (1357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc0ba660ed14d0923ea760b909e13fa4ff5bc4fe34acc4e9b0e5e072b2cd9704`  
		Last Modified: Fri, 27 Aug 2021 00:20:35 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f34329777aaf85af2b82ec6fa6640f757cc9589247f7fe67e427a4e39c19bda`  
		Last Modified: Fri, 27 Aug 2021 00:20:35 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:alpine`

```console
$ docker pull nats@sha256:45faf7fef5f78d815f712b8a05a2a0ded8793d777a0fb7640b0b0e6ff58e0009
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:alpine` - linux; amd64

```console
$ docker pull nats@sha256:7a1ec46ffffcc712a37d5e801e73e4cb68b22e15c842f36ab9211e1a039cb547
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7603979 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:163732450f029c457fb0826ccdbb6d69696f0d8af625ed2bef5291b807563c38`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 06 Aug 2021 17:19:45 GMT
ADD file:34eb5c40aa00028921a224d1764ae1b1f3ef710d191e4dfc7df55e0594aa7217 in / 
# Fri, 06 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Sat, 07 Aug 2021 00:12:56 GMT
ENV NATS_SERVER=2.3.4
# Sat, 07 Aug 2021 00:12:58 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='c8ba676a6c4ec9d3088e0b64ffdae36e2f2a9e1b89f030799f3efbb2923524a0' ;; 		armhf) natsArch='arm6'; sha256='d1f14441d1fbd53a7bff9623e8e572707d3e7024b42b6e925ad371d4dec0bc47' ;; 		armv7) natsArch='arm7'; sha256='2488706de91e94eba477ddbc3b293ec0b4d823509656cc101eec6a07e0319bb5' ;; 		x86_64) natsArch='amd64'; sha256='8c11abdeca4882888a8b6fbc45effe9fb4d1070eda3939b7299892c8c69a3e87' ;; 		x86) natsArch='386'; sha256='010bca73095d8a05495ef74a112dfd3919925b0ced10bc4c5f876f3858ca41f7' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Sat, 07 Aug 2021 00:12:59 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Sat, 07 Aug 2021 00:12:59 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Sat, 07 Aug 2021 00:12:59 GMT
EXPOSE 4222 6222 8222
# Sat, 07 Aug 2021 00:12:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 07 Aug 2021 00:12:59 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:29291e31a76a7e560b9b7ad3cada56e8c18d50a96cca8a2573e4f4689d7aca77`  
		Last Modified: Thu, 05 Aug 2021 15:56:25 GMT  
		Size: 2.8 MB (2813006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5b6f975cea84a1db539a70743c469f460dfd3c0e9f53362581ea5166cc6f7bb`  
		Last Modified: Sat, 07 Aug 2021 00:13:34 GMT  
		Size: 4.8 MB (4790004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:591a3df61d2af8d57d3b1b9462ef7661cf873411724688e51359600bdddd950c`  
		Last Modified: Sat, 07 Aug 2021 00:13:32 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcc7744cc9fd0f87944d530e0b43728226f13d0a9b61969249ab9b15dabd07d3`  
		Last Modified: Sat, 07 Aug 2021 00:13:32 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:e995bfdd6f9247dbf1b305adc029a95e72e8630251d8d19a9023c63dcbc47318
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7109895 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aae75c35e1d2e6f686fde0a0cfaea0aff2d58dcdf3e52a8ecba5ffc3dea3fe0b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 06 Aug 2021 17:49:32 GMT
ADD file:7f2c7deda009eabdcbbdccb11e854043d32c498e64e7e1ca02165d7bb4261d39 in / 
# Fri, 06 Aug 2021 17:49:32 GMT
CMD ["/bin/sh"]
# Fri, 27 Aug 2021 02:48:29 GMT
ENV NATS_SERVER=2.4.0
# Fri, 27 Aug 2021 02:48:34 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='eb510dd016cb1a9e9b1fae88a3471029048cb75dcc4ad83a4f5b1e3665f24a20' ;; 		armhf) natsArch='arm6'; sha256='76ac66cd86217a43bc227220eb054aac8a5744890d43c76156075d68a684d9e0' ;; 		armv7) natsArch='arm7'; sha256='e7521841d59f55fcef6172aa8f22d3af7ba1776bd67109a23c29d34d18d44bd6' ;; 		x86_64) natsArch='amd64'; sha256='f6841c89fcf99302bc7ac295ddc1e75322385f861d55abee79733976c8eb9bc7' ;; 		x86) natsArch='386'; sha256='c7e6e2b73d402e841b3abb57e26e2ef53350b44e385255bf289b08182058076a' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 27 Aug 2021 02:48:34 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 27 Aug 2021 02:48:35 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 27 Aug 2021 02:48:35 GMT
EXPOSE 4222 6222 8222
# Fri, 27 Aug 2021 02:48:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 Aug 2021 02:48:36 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:f465bb3e9fcd0c42f936ecc566c6e40353c00f3089b2b2c2ea1663c30f89d3ab`  
		Last Modified: Fri, 06 Aug 2021 17:51:00 GMT  
		Size: 2.6 MB (2626350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5abfce067d7bc34edb53d2ef3b851fb6750f2f165d88e6b7c1751a372637cf9`  
		Last Modified: Fri, 27 Aug 2021 02:50:40 GMT  
		Size: 4.5 MB (4482575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:915f8f45a2be36433373b63850ff3ca8ec9eb622ab7d74dd908284a971539307`  
		Last Modified: Fri, 27 Aug 2021 02:50:38 GMT  
		Size: 557.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dcbfc2ac16592f5503b1b3f59404245367a0082b75af6bd79a2b48e8c45a762`  
		Last Modified: Fri, 27 Aug 2021 02:50:38 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:443f504d21f3881e958e0e58c996d3e5970ff90cf970c6e41adc2542ae14e2b9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.9 MB (6880695 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:671e9b1b37b7c31f58f233286cc6ee3009ae062bfd7634d1e8e15be89ea2492e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 06 Aug 2021 17:57:32 GMT
ADD file:3a35ff3ac0d80289d419a4d6d8319610c38e1936d296addafb9aaf506946230f in / 
# Fri, 06 Aug 2021 17:57:32 GMT
CMD ["/bin/sh"]
# Fri, 06 Aug 2021 20:26:24 GMT
ENV NATS_SERVER=2.3.4
# Fri, 06 Aug 2021 20:26:28 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='c8ba676a6c4ec9d3088e0b64ffdae36e2f2a9e1b89f030799f3efbb2923524a0' ;; 		armhf) natsArch='arm6'; sha256='d1f14441d1fbd53a7bff9623e8e572707d3e7024b42b6e925ad371d4dec0bc47' ;; 		armv7) natsArch='arm7'; sha256='2488706de91e94eba477ddbc3b293ec0b4d823509656cc101eec6a07e0319bb5' ;; 		x86_64) natsArch='amd64'; sha256='8c11abdeca4882888a8b6fbc45effe9fb4d1070eda3939b7299892c8c69a3e87' ;; 		x86) natsArch='386'; sha256='010bca73095d8a05495ef74a112dfd3919925b0ced10bc4c5f876f3858ca41f7' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 06 Aug 2021 20:26:29 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 06 Aug 2021 20:26:29 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 06 Aug 2021 20:26:30 GMT
EXPOSE 4222 6222 8222
# Fri, 06 Aug 2021 20:26:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 06 Aug 2021 20:26:31 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:4ee0caa23b369b04827640a4be298bf4ff7bacd030c77e915f5d7fb8f987594a`  
		Last Modified: Fri, 06 Aug 2021 17:58:57 GMT  
		Size: 2.4 MB (2429359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54864bfc951be8b12f75e7c53f918420224b41c45520c27dc54f47006e1ace61`  
		Last Modified: Fri, 06 Aug 2021 20:28:37 GMT  
		Size: 4.5 MB (4450364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d8e3d21fd5215bd4bad28c6e61f03fe72c301544f5e535f0f618132b4bf3d90`  
		Last Modified: Fri, 06 Aug 2021 20:28:33 GMT  
		Size: 559.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e584ceff2e79dca85ab2d5589768d2243a4b7e52b7e1743785667471c73d928`  
		Last Modified: Fri, 06 Aug 2021 20:28:34 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:3ba9b8c80c1026d2a500251c07a9af099943e0291f5c381e49e6d6e496f8de8b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7115983 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:671a61b3bebfb1b125fc5ae67fc31351bc0aad1a0d1a103a21bb80895d7c09f3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 06 Aug 2021 17:39:26 GMT
ADD file:1a8fd1066485e1261462e689c1a072f010c1d3be904b73ef2b84128fac652951 in / 
# Fri, 06 Aug 2021 17:39:27 GMT
CMD ["/bin/sh"]
# Fri, 06 Aug 2021 19:49:47 GMT
ENV NATS_SERVER=2.3.4
# Fri, 06 Aug 2021 19:49:50 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='c8ba676a6c4ec9d3088e0b64ffdae36e2f2a9e1b89f030799f3efbb2923524a0' ;; 		armhf) natsArch='arm6'; sha256='d1f14441d1fbd53a7bff9623e8e572707d3e7024b42b6e925ad371d4dec0bc47' ;; 		armv7) natsArch='arm7'; sha256='2488706de91e94eba477ddbc3b293ec0b4d823509656cc101eec6a07e0319bb5' ;; 		x86_64) natsArch='amd64'; sha256='8c11abdeca4882888a8b6fbc45effe9fb4d1070eda3939b7299892c8c69a3e87' ;; 		x86) natsArch='386'; sha256='010bca73095d8a05495ef74a112dfd3919925b0ced10bc4c5f876f3858ca41f7' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 06 Aug 2021 19:49:50 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 06 Aug 2021 19:49:50 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 06 Aug 2021 19:49:50 GMT
EXPOSE 4222 6222 8222
# Fri, 06 Aug 2021 19:49:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 06 Aug 2021 19:49:50 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:fd3acdcea5682abced546ec19fb6ebee725c5184e5d91614c469c0a79e67f2d0`  
		Last Modified: Fri, 06 Aug 2021 17:40:12 GMT  
		Size: 2.7 MB (2710613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94ef6a8d5827e19307796e49f087f09097ca6784d2d680b67bf245e33eaa0417`  
		Last Modified: Fri, 06 Aug 2021 19:50:52 GMT  
		Size: 4.4 MB (4404401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc719578654cd35d6807367a487c4c618898557f046b46f894ccf6869b4d00cc`  
		Last Modified: Fri, 06 Aug 2021 19:50:52 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:742e4ce06ec6c0603f0ffe18a7788896b1ebe0f93184cba0be76177c3bb5c56b`  
		Last Modified: Fri, 06 Aug 2021 19:50:52 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:alpine3.14`

```console
$ docker pull nats@sha256:45faf7fef5f78d815f712b8a05a2a0ded8793d777a0fb7640b0b0e6ff58e0009
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:alpine3.14` - linux; amd64

```console
$ docker pull nats@sha256:7a1ec46ffffcc712a37d5e801e73e4cb68b22e15c842f36ab9211e1a039cb547
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7603979 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:163732450f029c457fb0826ccdbb6d69696f0d8af625ed2bef5291b807563c38`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 06 Aug 2021 17:19:45 GMT
ADD file:34eb5c40aa00028921a224d1764ae1b1f3ef710d191e4dfc7df55e0594aa7217 in / 
# Fri, 06 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Sat, 07 Aug 2021 00:12:56 GMT
ENV NATS_SERVER=2.3.4
# Sat, 07 Aug 2021 00:12:58 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='c8ba676a6c4ec9d3088e0b64ffdae36e2f2a9e1b89f030799f3efbb2923524a0' ;; 		armhf) natsArch='arm6'; sha256='d1f14441d1fbd53a7bff9623e8e572707d3e7024b42b6e925ad371d4dec0bc47' ;; 		armv7) natsArch='arm7'; sha256='2488706de91e94eba477ddbc3b293ec0b4d823509656cc101eec6a07e0319bb5' ;; 		x86_64) natsArch='amd64'; sha256='8c11abdeca4882888a8b6fbc45effe9fb4d1070eda3939b7299892c8c69a3e87' ;; 		x86) natsArch='386'; sha256='010bca73095d8a05495ef74a112dfd3919925b0ced10bc4c5f876f3858ca41f7' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Sat, 07 Aug 2021 00:12:59 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Sat, 07 Aug 2021 00:12:59 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Sat, 07 Aug 2021 00:12:59 GMT
EXPOSE 4222 6222 8222
# Sat, 07 Aug 2021 00:12:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 07 Aug 2021 00:12:59 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:29291e31a76a7e560b9b7ad3cada56e8c18d50a96cca8a2573e4f4689d7aca77`  
		Last Modified: Thu, 05 Aug 2021 15:56:25 GMT  
		Size: 2.8 MB (2813006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5b6f975cea84a1db539a70743c469f460dfd3c0e9f53362581ea5166cc6f7bb`  
		Last Modified: Sat, 07 Aug 2021 00:13:34 GMT  
		Size: 4.8 MB (4790004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:591a3df61d2af8d57d3b1b9462ef7661cf873411724688e51359600bdddd950c`  
		Last Modified: Sat, 07 Aug 2021 00:13:32 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcc7744cc9fd0f87944d530e0b43728226f13d0a9b61969249ab9b15dabd07d3`  
		Last Modified: Sat, 07 Aug 2021 00:13:32 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.14` - linux; arm variant v6

```console
$ docker pull nats@sha256:e995bfdd6f9247dbf1b305adc029a95e72e8630251d8d19a9023c63dcbc47318
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7109895 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aae75c35e1d2e6f686fde0a0cfaea0aff2d58dcdf3e52a8ecba5ffc3dea3fe0b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 06 Aug 2021 17:49:32 GMT
ADD file:7f2c7deda009eabdcbbdccb11e854043d32c498e64e7e1ca02165d7bb4261d39 in / 
# Fri, 06 Aug 2021 17:49:32 GMT
CMD ["/bin/sh"]
# Fri, 27 Aug 2021 02:48:29 GMT
ENV NATS_SERVER=2.4.0
# Fri, 27 Aug 2021 02:48:34 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='eb510dd016cb1a9e9b1fae88a3471029048cb75dcc4ad83a4f5b1e3665f24a20' ;; 		armhf) natsArch='arm6'; sha256='76ac66cd86217a43bc227220eb054aac8a5744890d43c76156075d68a684d9e0' ;; 		armv7) natsArch='arm7'; sha256='e7521841d59f55fcef6172aa8f22d3af7ba1776bd67109a23c29d34d18d44bd6' ;; 		x86_64) natsArch='amd64'; sha256='f6841c89fcf99302bc7ac295ddc1e75322385f861d55abee79733976c8eb9bc7' ;; 		x86) natsArch='386'; sha256='c7e6e2b73d402e841b3abb57e26e2ef53350b44e385255bf289b08182058076a' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 27 Aug 2021 02:48:34 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 27 Aug 2021 02:48:35 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 27 Aug 2021 02:48:35 GMT
EXPOSE 4222 6222 8222
# Fri, 27 Aug 2021 02:48:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 Aug 2021 02:48:36 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:f465bb3e9fcd0c42f936ecc566c6e40353c00f3089b2b2c2ea1663c30f89d3ab`  
		Last Modified: Fri, 06 Aug 2021 17:51:00 GMT  
		Size: 2.6 MB (2626350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5abfce067d7bc34edb53d2ef3b851fb6750f2f165d88e6b7c1751a372637cf9`  
		Last Modified: Fri, 27 Aug 2021 02:50:40 GMT  
		Size: 4.5 MB (4482575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:915f8f45a2be36433373b63850ff3ca8ec9eb622ab7d74dd908284a971539307`  
		Last Modified: Fri, 27 Aug 2021 02:50:38 GMT  
		Size: 557.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dcbfc2ac16592f5503b1b3f59404245367a0082b75af6bd79a2b48e8c45a762`  
		Last Modified: Fri, 27 Aug 2021 02:50:38 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.14` - linux; arm variant v7

```console
$ docker pull nats@sha256:443f504d21f3881e958e0e58c996d3e5970ff90cf970c6e41adc2542ae14e2b9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.9 MB (6880695 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:671e9b1b37b7c31f58f233286cc6ee3009ae062bfd7634d1e8e15be89ea2492e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 06 Aug 2021 17:57:32 GMT
ADD file:3a35ff3ac0d80289d419a4d6d8319610c38e1936d296addafb9aaf506946230f in / 
# Fri, 06 Aug 2021 17:57:32 GMT
CMD ["/bin/sh"]
# Fri, 06 Aug 2021 20:26:24 GMT
ENV NATS_SERVER=2.3.4
# Fri, 06 Aug 2021 20:26:28 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='c8ba676a6c4ec9d3088e0b64ffdae36e2f2a9e1b89f030799f3efbb2923524a0' ;; 		armhf) natsArch='arm6'; sha256='d1f14441d1fbd53a7bff9623e8e572707d3e7024b42b6e925ad371d4dec0bc47' ;; 		armv7) natsArch='arm7'; sha256='2488706de91e94eba477ddbc3b293ec0b4d823509656cc101eec6a07e0319bb5' ;; 		x86_64) natsArch='amd64'; sha256='8c11abdeca4882888a8b6fbc45effe9fb4d1070eda3939b7299892c8c69a3e87' ;; 		x86) natsArch='386'; sha256='010bca73095d8a05495ef74a112dfd3919925b0ced10bc4c5f876f3858ca41f7' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 06 Aug 2021 20:26:29 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 06 Aug 2021 20:26:29 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 06 Aug 2021 20:26:30 GMT
EXPOSE 4222 6222 8222
# Fri, 06 Aug 2021 20:26:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 06 Aug 2021 20:26:31 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:4ee0caa23b369b04827640a4be298bf4ff7bacd030c77e915f5d7fb8f987594a`  
		Last Modified: Fri, 06 Aug 2021 17:58:57 GMT  
		Size: 2.4 MB (2429359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54864bfc951be8b12f75e7c53f918420224b41c45520c27dc54f47006e1ace61`  
		Last Modified: Fri, 06 Aug 2021 20:28:37 GMT  
		Size: 4.5 MB (4450364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d8e3d21fd5215bd4bad28c6e61f03fe72c301544f5e535f0f618132b4bf3d90`  
		Last Modified: Fri, 06 Aug 2021 20:28:33 GMT  
		Size: 559.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e584ceff2e79dca85ab2d5589768d2243a4b7e52b7e1743785667471c73d928`  
		Last Modified: Fri, 06 Aug 2021 20:28:34 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.14` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:3ba9b8c80c1026d2a500251c07a9af099943e0291f5c381e49e6d6e496f8de8b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7115983 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:671a61b3bebfb1b125fc5ae67fc31351bc0aad1a0d1a103a21bb80895d7c09f3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 06 Aug 2021 17:39:26 GMT
ADD file:1a8fd1066485e1261462e689c1a072f010c1d3be904b73ef2b84128fac652951 in / 
# Fri, 06 Aug 2021 17:39:27 GMT
CMD ["/bin/sh"]
# Fri, 06 Aug 2021 19:49:47 GMT
ENV NATS_SERVER=2.3.4
# Fri, 06 Aug 2021 19:49:50 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='c8ba676a6c4ec9d3088e0b64ffdae36e2f2a9e1b89f030799f3efbb2923524a0' ;; 		armhf) natsArch='arm6'; sha256='d1f14441d1fbd53a7bff9623e8e572707d3e7024b42b6e925ad371d4dec0bc47' ;; 		armv7) natsArch='arm7'; sha256='2488706de91e94eba477ddbc3b293ec0b4d823509656cc101eec6a07e0319bb5' ;; 		x86_64) natsArch='amd64'; sha256='8c11abdeca4882888a8b6fbc45effe9fb4d1070eda3939b7299892c8c69a3e87' ;; 		x86) natsArch='386'; sha256='010bca73095d8a05495ef74a112dfd3919925b0ced10bc4c5f876f3858ca41f7' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 06 Aug 2021 19:49:50 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 06 Aug 2021 19:49:50 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 06 Aug 2021 19:49:50 GMT
EXPOSE 4222 6222 8222
# Fri, 06 Aug 2021 19:49:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 06 Aug 2021 19:49:50 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:fd3acdcea5682abced546ec19fb6ebee725c5184e5d91614c469c0a79e67f2d0`  
		Last Modified: Fri, 06 Aug 2021 17:40:12 GMT  
		Size: 2.7 MB (2710613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94ef6a8d5827e19307796e49f087f09097ca6784d2d680b67bf245e33eaa0417`  
		Last Modified: Fri, 06 Aug 2021 19:50:52 GMT  
		Size: 4.4 MB (4404401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc719578654cd35d6807367a487c4c618898557f046b46f894ccf6869b4d00cc`  
		Last Modified: Fri, 06 Aug 2021 19:50:52 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:742e4ce06ec6c0603f0ffe18a7788896b1ebe0f93184cba0be76177c3bb5c56b`  
		Last Modified: Fri, 06 Aug 2021 19:50:52 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:latest`

```console
$ docker pull nats@sha256:f00cc850e92427d4fc02e7090a743e9044f62755a8b06ab733ff88b8d5ff0562
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.2114; amd64

### `nats:latest` - linux; amd64

```console
$ docker pull nats@sha256:acd926de12a3d1a625d13dfab262fa240b0d99ecb35c68e372e093ab466d1b0b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4506461 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5738e29b3f24028140a48fe9652afc26b4118a35427b996d591872c6dd9162ed`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 05 Aug 2021 01:20:24 GMT
COPY file:edd123fab471ca4bff1ec55ddc839aaf0defe3667b337aaec7c3c8e70e903e8d in /nats-server 
# Thu, 05 Aug 2021 01:20:24 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 05 Aug 2021 01:20:24 GMT
EXPOSE 4222 6222 8222
# Thu, 05 Aug 2021 01:20:24 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 05 Aug 2021 01:20:25 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3d02ec701f9917abde1e8953cba96577f89ebc29ced1af0d82734bde1a034361`  
		Last Modified: Thu, 05 Aug 2021 01:21:15 GMT  
		Size: 4.5 MB (4505985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6beb29f4b4e73a454d8e38755b89ed0a71bb2f1aaaaa02105c3708af114c87cc`  
		Last Modified: Thu, 05 Aug 2021 01:21:14 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm variant v6

```console
$ docker pull nats@sha256:7201c8cd794776fa392c3a25eb89e4ee987aeaaae647caa364621d5daf5ca3c5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4201703 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc2211a135c8d5c9641c74ba5d54c3c1df4ac3f24fa70a6a57be8a2975af7854`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 02:48:56 GMT
COPY file:81d7dcb1f2223ae767ee02f3b24758797ca55a665d17dcb2054eeb097fb2eafa in /nats-server 
# Fri, 27 Aug 2021 02:48:56 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 27 Aug 2021 02:48:57 GMT
EXPOSE 4222 6222 8222
# Fri, 27 Aug 2021 02:48:57 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 27 Aug 2021 02:48:58 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a820d11a96d84195887c44533ffcad67997fcb79d52f4564709bfdbde47d578d`  
		Last Modified: Fri, 27 Aug 2021 02:51:18 GMT  
		Size: 4.2 MB (4201229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a1c4f82bf849dc3d9d18f1c560b9afd0e5237eb2f05377e6792dda2480249cb`  
		Last Modified: Fri, 27 Aug 2021 02:51:15 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm variant v7

```console
$ docker pull nats@sha256:edbf04c6d86cc6973609fb90c099c175ba05216954d224ea93c03e862b6c0955
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4170312 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:59d59f3755a610c7ef37ce7df6d7e2a6c1a1e7e0554fd7f0dfe5a7ba96370e6f`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 05 Aug 2021 01:04:56 GMT
COPY file:f8d5a2ea993b24151d26b5967a44af43f6fa70afe6b7965767ebb48f41351935 in /nats-server 
# Thu, 05 Aug 2021 01:04:57 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 05 Aug 2021 01:04:57 GMT
EXPOSE 4222 6222 8222
# Thu, 05 Aug 2021 01:04:58 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 05 Aug 2021 01:04:58 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:0b65416c95f5f06a582f3d8ffe3f3cc9b4df10e5d724eb5167d7766bce64b77e`  
		Last Modified: Thu, 05 Aug 2021 01:07:22 GMT  
		Size: 4.2 MB (4169837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:711811fab377fd6c12391460fafc4fe011d419669f5508b086b269489ae78d22`  
		Last Modified: Thu, 05 Aug 2021 01:07:20 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:258407bfd157b748b13d824daa441eeb795b46dae0dee509189e6f215219dfc4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.1 MB (4121540 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:928fc611a3e5935a6eea2e73e72cfc121d250a608f1def1e50e9a2bca5e9e0c4`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 05 Aug 2021 01:39:59 GMT
COPY file:e2687e43e0f0627dcdfb73c8b9b66c9a86cdda6399f627b485911acbece9a3c9 in /nats-server 
# Thu, 05 Aug 2021 01:40:00 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 05 Aug 2021 01:40:00 GMT
EXPOSE 4222 6222 8222
# Thu, 05 Aug 2021 01:40:00 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 05 Aug 2021 01:40:00 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:333cb9b408ea509452b14ed5b1c9a8a6abed86e5a3177bc9ae7917d6c0c51318`  
		Last Modified: Thu, 05 Aug 2021 01:41:23 GMT  
		Size: 4.1 MB (4121065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b79f5ac7bd31304ad5fab87a7bb25e67ff6f7e8f0299806180b5bb556ea0dc9`  
		Last Modified: Thu, 05 Aug 2021 01:41:22 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - windows version 10.0.17763.2114; amd64

```console
$ docker pull nats@sha256:9c370308b1924738df19dd502a9d8d8c13066580fd1550eddbf4f70663c87fe5
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.3 MB (107338949 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e90920ed24cf8337e7f99fdd7199bff8ec7dd43cfa5063f0f373e6700f8a17a2`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 05 Aug 2021 19:15:20 GMT
RUN Apply image 1809-amd64
# Wed, 25 Aug 2021 16:07:56 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 27 Aug 2021 00:16:45 GMT
RUN cmd /S /C #(nop) COPY file:bafd3fc1559b39648f01fab1b3b19a9fc9bb95afae5b07b1d7987b376806e053 in C:\nats-server.exe 
# Fri, 27 Aug 2021 00:16:46 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 27 Aug 2021 00:16:47 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Fri, 27 Aug 2021 00:16:47 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 27 Aug 2021 00:16:48 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:bc8517709e9cfff223cb034ff5be8fcbfa5409de286cdac9ae1b8878ebea6b84`  
		Size: 102.7 MB (102741177 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ae8616c17f5cca409a4b1289387e37dc532657ba2b52bb60713ff621acccd506`  
		Last Modified: Wed, 25 Aug 2021 16:11:20 GMT  
		Size: 1.0 KB (1022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb815244c76bae445a6697a3f1b6a0643fc016be2b2da5192dc6bb4079cd0119`  
		Last Modified: Fri, 27 Aug 2021 00:20:21 GMT  
		Size: 4.6 MB (4591622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c33193ffa3c81a2ebd95cb6af96ce80ee557191a64ba47e1977479e1167530ca`  
		Last Modified: Fri, 27 Aug 2021 00:20:19 GMT  
		Size: 1.7 KB (1701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c57e2e68d87e03a37f706b01fe403fc34435b82da71d1080e11ec9df4d418a2`  
		Last Modified: Fri, 27 Aug 2021 00:20:19 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:048b1707f600e77fb06d48bd9c3759cad471944658bdfa3dd59b2852dc7983b4`  
		Last Modified: Fri, 27 Aug 2021 00:20:20 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b434e68e7546ed285144b98ef8fc3a10f1b6ee578ef2503e9f09aefab0370d0`  
		Last Modified: Fri, 27 Aug 2021 00:20:20 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:linux`

```console
$ docker pull nats@sha256:91afdbdd639c488228d39325873355953a2e8d6d579eea0d5695cea72b68e7ba
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:linux` - linux; amd64

```console
$ docker pull nats@sha256:acd926de12a3d1a625d13dfab262fa240b0d99ecb35c68e372e093ab466d1b0b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4506461 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5738e29b3f24028140a48fe9652afc26b4118a35427b996d591872c6dd9162ed`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 05 Aug 2021 01:20:24 GMT
COPY file:edd123fab471ca4bff1ec55ddc839aaf0defe3667b337aaec7c3c8e70e903e8d in /nats-server 
# Thu, 05 Aug 2021 01:20:24 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 05 Aug 2021 01:20:24 GMT
EXPOSE 4222 6222 8222
# Thu, 05 Aug 2021 01:20:24 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 05 Aug 2021 01:20:25 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3d02ec701f9917abde1e8953cba96577f89ebc29ced1af0d82734bde1a034361`  
		Last Modified: Thu, 05 Aug 2021 01:21:15 GMT  
		Size: 4.5 MB (4505985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6beb29f4b4e73a454d8e38755b89ed0a71bb2f1aaaaa02105c3708af114c87cc`  
		Last Modified: Thu, 05 Aug 2021 01:21:14 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:7201c8cd794776fa392c3a25eb89e4ee987aeaaae647caa364621d5daf5ca3c5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4201703 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc2211a135c8d5c9641c74ba5d54c3c1df4ac3f24fa70a6a57be8a2975af7854`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 02:48:56 GMT
COPY file:81d7dcb1f2223ae767ee02f3b24758797ca55a665d17dcb2054eeb097fb2eafa in /nats-server 
# Fri, 27 Aug 2021 02:48:56 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 27 Aug 2021 02:48:57 GMT
EXPOSE 4222 6222 8222
# Fri, 27 Aug 2021 02:48:57 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 27 Aug 2021 02:48:58 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a820d11a96d84195887c44533ffcad67997fcb79d52f4564709bfdbde47d578d`  
		Last Modified: Fri, 27 Aug 2021 02:51:18 GMT  
		Size: 4.2 MB (4201229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a1c4f82bf849dc3d9d18f1c560b9afd0e5237eb2f05377e6792dda2480249cb`  
		Last Modified: Fri, 27 Aug 2021 02:51:15 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:edbf04c6d86cc6973609fb90c099c175ba05216954d224ea93c03e862b6c0955
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4170312 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:59d59f3755a610c7ef37ce7df6d7e2a6c1a1e7e0554fd7f0dfe5a7ba96370e6f`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 05 Aug 2021 01:04:56 GMT
COPY file:f8d5a2ea993b24151d26b5967a44af43f6fa70afe6b7965767ebb48f41351935 in /nats-server 
# Thu, 05 Aug 2021 01:04:57 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 05 Aug 2021 01:04:57 GMT
EXPOSE 4222 6222 8222
# Thu, 05 Aug 2021 01:04:58 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 05 Aug 2021 01:04:58 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:0b65416c95f5f06a582f3d8ffe3f3cc9b4df10e5d724eb5167d7766bce64b77e`  
		Last Modified: Thu, 05 Aug 2021 01:07:22 GMT  
		Size: 4.2 MB (4169837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:711811fab377fd6c12391460fafc4fe011d419669f5508b086b269489ae78d22`  
		Last Modified: Thu, 05 Aug 2021 01:07:20 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:258407bfd157b748b13d824daa441eeb795b46dae0dee509189e6f215219dfc4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.1 MB (4121540 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:928fc611a3e5935a6eea2e73e72cfc121d250a608f1def1e50e9a2bca5e9e0c4`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 05 Aug 2021 01:39:59 GMT
COPY file:e2687e43e0f0627dcdfb73c8b9b66c9a86cdda6399f627b485911acbece9a3c9 in /nats-server 
# Thu, 05 Aug 2021 01:40:00 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 05 Aug 2021 01:40:00 GMT
EXPOSE 4222 6222 8222
# Thu, 05 Aug 2021 01:40:00 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 05 Aug 2021 01:40:00 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:333cb9b408ea509452b14ed5b1c9a8a6abed86e5a3177bc9ae7917d6c0c51318`  
		Last Modified: Thu, 05 Aug 2021 01:41:23 GMT  
		Size: 4.1 MB (4121065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b79f5ac7bd31304ad5fab87a7bb25e67ff6f7e8f0299806180b5bb556ea0dc9`  
		Last Modified: Thu, 05 Aug 2021 01:41:22 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:nanoserver`

```console
$ docker pull nats@sha256:21ff4cbb5485b408bcc030f341817018fb13a7381ca7c520960bf26bab74ddac
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2114; amd64

### `nats:nanoserver` - windows version 10.0.17763.2114; amd64

```console
$ docker pull nats@sha256:9c370308b1924738df19dd502a9d8d8c13066580fd1550eddbf4f70663c87fe5
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.3 MB (107338949 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e90920ed24cf8337e7f99fdd7199bff8ec7dd43cfa5063f0f373e6700f8a17a2`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 05 Aug 2021 19:15:20 GMT
RUN Apply image 1809-amd64
# Wed, 25 Aug 2021 16:07:56 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 27 Aug 2021 00:16:45 GMT
RUN cmd /S /C #(nop) COPY file:bafd3fc1559b39648f01fab1b3b19a9fc9bb95afae5b07b1d7987b376806e053 in C:\nats-server.exe 
# Fri, 27 Aug 2021 00:16:46 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 27 Aug 2021 00:16:47 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Fri, 27 Aug 2021 00:16:47 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 27 Aug 2021 00:16:48 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:bc8517709e9cfff223cb034ff5be8fcbfa5409de286cdac9ae1b8878ebea6b84`  
		Size: 102.7 MB (102741177 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ae8616c17f5cca409a4b1289387e37dc532657ba2b52bb60713ff621acccd506`  
		Last Modified: Wed, 25 Aug 2021 16:11:20 GMT  
		Size: 1.0 KB (1022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb815244c76bae445a6697a3f1b6a0643fc016be2b2da5192dc6bb4079cd0119`  
		Last Modified: Fri, 27 Aug 2021 00:20:21 GMT  
		Size: 4.6 MB (4591622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c33193ffa3c81a2ebd95cb6af96ce80ee557191a64ba47e1977479e1167530ca`  
		Last Modified: Fri, 27 Aug 2021 00:20:19 GMT  
		Size: 1.7 KB (1701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c57e2e68d87e03a37f706b01fe403fc34435b82da71d1080e11ec9df4d418a2`  
		Last Modified: Fri, 27 Aug 2021 00:20:19 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:048b1707f600e77fb06d48bd9c3759cad471944658bdfa3dd59b2852dc7983b4`  
		Last Modified: Fri, 27 Aug 2021 00:20:20 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b434e68e7546ed285144b98ef8fc3a10f1b6ee578ef2503e9f09aefab0370d0`  
		Last Modified: Fri, 27 Aug 2021 00:20:20 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:nanoserver-1809`

```console
$ docker pull nats@sha256:21ff4cbb5485b408bcc030f341817018fb13a7381ca7c520960bf26bab74ddac
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2114; amd64

### `nats:nanoserver-1809` - windows version 10.0.17763.2114; amd64

```console
$ docker pull nats@sha256:9c370308b1924738df19dd502a9d8d8c13066580fd1550eddbf4f70663c87fe5
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.3 MB (107338949 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e90920ed24cf8337e7f99fdd7199bff8ec7dd43cfa5063f0f373e6700f8a17a2`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 05 Aug 2021 19:15:20 GMT
RUN Apply image 1809-amd64
# Wed, 25 Aug 2021 16:07:56 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 27 Aug 2021 00:16:45 GMT
RUN cmd /S /C #(nop) COPY file:bafd3fc1559b39648f01fab1b3b19a9fc9bb95afae5b07b1d7987b376806e053 in C:\nats-server.exe 
# Fri, 27 Aug 2021 00:16:46 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 27 Aug 2021 00:16:47 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Fri, 27 Aug 2021 00:16:47 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 27 Aug 2021 00:16:48 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:bc8517709e9cfff223cb034ff5be8fcbfa5409de286cdac9ae1b8878ebea6b84`  
		Size: 102.7 MB (102741177 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ae8616c17f5cca409a4b1289387e37dc532657ba2b52bb60713ff621acccd506`  
		Last Modified: Wed, 25 Aug 2021 16:11:20 GMT  
		Size: 1.0 KB (1022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb815244c76bae445a6697a3f1b6a0643fc016be2b2da5192dc6bb4079cd0119`  
		Last Modified: Fri, 27 Aug 2021 00:20:21 GMT  
		Size: 4.6 MB (4591622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c33193ffa3c81a2ebd95cb6af96ce80ee557191a64ba47e1977479e1167530ca`  
		Last Modified: Fri, 27 Aug 2021 00:20:19 GMT  
		Size: 1.7 KB (1701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c57e2e68d87e03a37f706b01fe403fc34435b82da71d1080e11ec9df4d418a2`  
		Last Modified: Fri, 27 Aug 2021 00:20:19 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:048b1707f600e77fb06d48bd9c3759cad471944658bdfa3dd59b2852dc7983b4`  
		Last Modified: Fri, 27 Aug 2021 00:20:20 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b434e68e7546ed285144b98ef8fc3a10f1b6ee578ef2503e9f09aefab0370d0`  
		Last Modified: Fri, 27 Aug 2021 00:20:20 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:scratch`

```console
$ docker pull nats@sha256:91afdbdd639c488228d39325873355953a2e8d6d579eea0d5695cea72b68e7ba
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:scratch` - linux; amd64

```console
$ docker pull nats@sha256:acd926de12a3d1a625d13dfab262fa240b0d99ecb35c68e372e093ab466d1b0b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4506461 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5738e29b3f24028140a48fe9652afc26b4118a35427b996d591872c6dd9162ed`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 05 Aug 2021 01:20:24 GMT
COPY file:edd123fab471ca4bff1ec55ddc839aaf0defe3667b337aaec7c3c8e70e903e8d in /nats-server 
# Thu, 05 Aug 2021 01:20:24 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 05 Aug 2021 01:20:24 GMT
EXPOSE 4222 6222 8222
# Thu, 05 Aug 2021 01:20:24 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 05 Aug 2021 01:20:25 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3d02ec701f9917abde1e8953cba96577f89ebc29ced1af0d82734bde1a034361`  
		Last Modified: Thu, 05 Aug 2021 01:21:15 GMT  
		Size: 4.5 MB (4505985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6beb29f4b4e73a454d8e38755b89ed0a71bb2f1aaaaa02105c3708af114c87cc`  
		Last Modified: Thu, 05 Aug 2021 01:21:14 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:7201c8cd794776fa392c3a25eb89e4ee987aeaaae647caa364621d5daf5ca3c5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4201703 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc2211a135c8d5c9641c74ba5d54c3c1df4ac3f24fa70a6a57be8a2975af7854`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 02:48:56 GMT
COPY file:81d7dcb1f2223ae767ee02f3b24758797ca55a665d17dcb2054eeb097fb2eafa in /nats-server 
# Fri, 27 Aug 2021 02:48:56 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 27 Aug 2021 02:48:57 GMT
EXPOSE 4222 6222 8222
# Fri, 27 Aug 2021 02:48:57 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 27 Aug 2021 02:48:58 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a820d11a96d84195887c44533ffcad67997fcb79d52f4564709bfdbde47d578d`  
		Last Modified: Fri, 27 Aug 2021 02:51:18 GMT  
		Size: 4.2 MB (4201229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a1c4f82bf849dc3d9d18f1c560b9afd0e5237eb2f05377e6792dda2480249cb`  
		Last Modified: Fri, 27 Aug 2021 02:51:15 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:edbf04c6d86cc6973609fb90c099c175ba05216954d224ea93c03e862b6c0955
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4170312 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:59d59f3755a610c7ef37ce7df6d7e2a6c1a1e7e0554fd7f0dfe5a7ba96370e6f`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 05 Aug 2021 01:04:56 GMT
COPY file:f8d5a2ea993b24151d26b5967a44af43f6fa70afe6b7965767ebb48f41351935 in /nats-server 
# Thu, 05 Aug 2021 01:04:57 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 05 Aug 2021 01:04:57 GMT
EXPOSE 4222 6222 8222
# Thu, 05 Aug 2021 01:04:58 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 05 Aug 2021 01:04:58 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:0b65416c95f5f06a582f3d8ffe3f3cc9b4df10e5d724eb5167d7766bce64b77e`  
		Last Modified: Thu, 05 Aug 2021 01:07:22 GMT  
		Size: 4.2 MB (4169837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:711811fab377fd6c12391460fafc4fe011d419669f5508b086b269489ae78d22`  
		Last Modified: Thu, 05 Aug 2021 01:07:20 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:258407bfd157b748b13d824daa441eeb795b46dae0dee509189e6f215219dfc4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.1 MB (4121540 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:928fc611a3e5935a6eea2e73e72cfc121d250a608f1def1e50e9a2bca5e9e0c4`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 05 Aug 2021 01:39:59 GMT
COPY file:e2687e43e0f0627dcdfb73c8b9b66c9a86cdda6399f627b485911acbece9a3c9 in /nats-server 
# Thu, 05 Aug 2021 01:40:00 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 05 Aug 2021 01:40:00 GMT
EXPOSE 4222 6222 8222
# Thu, 05 Aug 2021 01:40:00 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 05 Aug 2021 01:40:00 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:333cb9b408ea509452b14ed5b1c9a8a6abed86e5a3177bc9ae7917d6c0c51318`  
		Last Modified: Thu, 05 Aug 2021 01:41:23 GMT  
		Size: 4.1 MB (4121065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b79f5ac7bd31304ad5fab87a7bb25e67ff6f7e8f0299806180b5bb556ea0dc9`  
		Last Modified: Thu, 05 Aug 2021 01:41:22 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:windowsservercore`

```console
$ docker pull nats@sha256:cf3aae4f841ee35ce5bfef42265fbd8025c1cff06d3f284e813cfec4cf9d6e4a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.2114; amd64
	-	windows version 10.0.14393.4583; amd64

### `nats:windowsservercore` - windows version 10.0.17763.2114; amd64

```console
$ docker pull nats@sha256:48cc63b49c047b98135531fccf1f7c4a418477d38def8702f6ecce6e8574923c
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2691328041 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09c3d57b266e04d58ceedd30a6c5428caa6783ca301ecc858c8aa62a8f682a3a`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 05 Aug 2021 19:44:34 GMT
RUN Install update 1809-amd64
# Wed, 25 Aug 2021 13:46:35 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 25 Aug 2021 16:05:30 GMT
ENV NATS_DOCKERIZED=1
# Fri, 27 Aug 2021 00:14:05 GMT
ENV NATS_SERVER=2.4.0
# Fri, 27 Aug 2021 00:14:06 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.4.0/nats-server-v2.4.0-windows-amd64.zip
# Fri, 27 Aug 2021 00:14:07 GMT
ENV NATS_SERVER_SHASUM=6c66acf5ed7e87a1ed9c499033c8c64c8c1365c5a95973ec57859abf1a69b032
# Fri, 27 Aug 2021 00:15:10 GMT
RUN Set-PSDebug -Trace 2
# Fri, 27 Aug 2021 00:16:22 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 27 Aug 2021 00:16:23 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 27 Aug 2021 00:16:24 GMT
EXPOSE 4222 6222 8222
# Fri, 27 Aug 2021 00:16:25 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 27 Aug 2021 00:16:26 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c67ded6868b61d392a0c096f911563fd6bc0bc3ed4fe401d077b3718a1b0cdaf`  
		Size: 967.7 MB (967665054 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:985da5cbc0735e1c422e766af23125ba345f431cb337ea43ec32298d0bb8e4ea`  
		Last Modified: Wed, 25 Aug 2021 15:45:02 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3dbdd68a4b0c278695b3e1d401d7eddfb0f0e3aa1e28aed88eb700059648f8f`  
		Last Modified: Wed, 25 Aug 2021 16:11:02 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9924833e15cbbaa8bd2d64c942c877c0765ba95d0790a5a9ea83a3d40bcaba43`  
		Last Modified: Fri, 27 Aug 2021 00:20:04 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93b8b51ab5e087ce5a5187d2967b0a82e4ce38b2151fc1b040be11a843334b1a`  
		Last Modified: Fri, 27 Aug 2021 00:20:00 GMT  
		Size: 1.4 KB (1360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73666a2686d6829048f4fa9f037f08038370c72202369f80bd4b715ead2cafe3`  
		Last Modified: Fri, 27 Aug 2021 00:20:00 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e35fdb95a7dc56c84ff744d8172574e2edd053f77affad83306be03c14fdb9fb`  
		Last Modified: Fri, 27 Aug 2021 00:20:01 GMT  
		Size: 372.5 KB (372513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3b9b9590a746c11677c6728f047f437a87645f68249b9691ed347591b850b8d`  
		Last Modified: Fri, 27 Aug 2021 00:20:00 GMT  
		Size: 4.9 MB (4944435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b629e22fb2c409b07df4f55a5b1c1d392ae3fc7110b646f46f63c8de8af0f470`  
		Last Modified: Fri, 27 Aug 2021 00:19:58 GMT  
		Size: 2.0 KB (1978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12c15056241134a8112b0c3e43493f7be7cd0421808ee5edbddb6490f355110e`  
		Last Modified: Fri, 27 Aug 2021 00:19:58 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27b1ee4ad1c87cc30317f9c2212c416f2a120923e62f8f88b8192c58d07a9dc1`  
		Last Modified: Fri, 27 Aug 2021 00:19:58 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1f840f93a8499fdb3efd112f5eedcef4290ba5edc497321ae223cdfc4dcb80e`  
		Last Modified: Fri, 27 Aug 2021 00:19:58 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:windowsservercore` - windows version 10.0.14393.4583; amd64

```console
$ docker pull nats@sha256:f6699a354c1c84d5ad72289d99c815e7bf11f983cd786684a5015745992e58e4
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6276264126 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af044355ba3348cfc4c9fb174c578e012f1a979a5d04b3681aafc9c2d9411eff`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Sun, 01 Aug 2021 08:52:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 25 Aug 2021 13:59:32 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 25 Aug 2021 16:08:06 GMT
ENV NATS_DOCKERIZED=1
# Fri, 27 Aug 2021 00:16:54 GMT
ENV NATS_SERVER=2.4.0
# Fri, 27 Aug 2021 00:16:55 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.4.0/nats-server-v2.4.0-windows-amd64.zip
# Fri, 27 Aug 2021 00:16:56 GMT
ENV NATS_SERVER_SHASUM=6c66acf5ed7e87a1ed9c499033c8c64c8c1365c5a95973ec57859abf1a69b032
# Fri, 27 Aug 2021 00:17:57 GMT
RUN Set-PSDebug -Trace 2
# Fri, 27 Aug 2021 00:19:20 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 27 Aug 2021 00:19:21 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 27 Aug 2021 00:19:21 GMT
EXPOSE 4222 6222 8222
# Fri, 27 Aug 2021 00:19:22 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 27 Aug 2021 00:19:23 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c427f892fe74603ae09d4e49b25f8f7046f957054034dc9f462e0e88d7bffaa5`  
		Size: 2.2 GB (2200980134 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a869803fc3d8292f0fe1bc6ed35e1ceedbd7c797a1486767a55f88c6c28ed4c5`  
		Last Modified: Wed, 25 Aug 2021 15:45:25 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a745f96c10790ef3a2006dbd4c116eb2f1552fd3c4a38fca179a8160e9918ac1`  
		Last Modified: Wed, 25 Aug 2021 16:11:42 GMT  
		Size: 1.3 KB (1329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ecbc2c744fbea737586b320c08b480fbd8eb2dc994300a74c6a4864ee082901`  
		Last Modified: Fri, 27 Aug 2021 00:20:37 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c530ba921538bcf67912fb5a5d6794e991501dbca08ae8137712fc58854f4f68`  
		Last Modified: Fri, 27 Aug 2021 00:20:37 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35523016d41ba152afbfa0a809770805058865f49d17d6d04d77fab412e5c29d`  
		Last Modified: Fri, 27 Aug 2021 00:20:37 GMT  
		Size: 1.4 KB (1383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:348276d7a124485ea8bc7bad9b9147c84dd20fda1da976a1542cbdb907e4ea95`  
		Last Modified: Fri, 27 Aug 2021 00:20:37 GMT  
		Size: 336.1 KB (336071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:751871e4a816cbaed81ad603047b0c9b536c2180dd5e54f7874d1ca37ef57851`  
		Last Modified: Fri, 27 Aug 2021 00:20:36 GMT  
		Size: 4.9 MB (4948899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d9507c0638be8fdbc5f10f76a31d751acfd94e02618ac7528b4856051bb3721`  
		Last Modified: Fri, 27 Aug 2021 00:20:35 GMT  
		Size: 2.0 KB (1979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:784f2e48cdd62d72893e3cf7316c3c7764e937b9ccade0cb0ce5547ee1e1a304`  
		Last Modified: Fri, 27 Aug 2021 00:20:35 GMT  
		Size: 1.4 KB (1357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc0ba660ed14d0923ea760b909e13fa4ff5bc4fe34acc4e9b0e5e072b2cd9704`  
		Last Modified: Fri, 27 Aug 2021 00:20:35 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f34329777aaf85af2b82ec6fa6640f757cc9589247f7fe67e427a4e39c19bda`  
		Last Modified: Fri, 27 Aug 2021 00:20:35 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:windowsservercore-1809`

```console
$ docker pull nats@sha256:a328e744c3a06f930890900c486761a97c2108563a63a093b1d0fc0fb9a1ad21
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2114; amd64

### `nats:windowsservercore-1809` - windows version 10.0.17763.2114; amd64

```console
$ docker pull nats@sha256:48cc63b49c047b98135531fccf1f7c4a418477d38def8702f6ecce6e8574923c
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2691328041 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09c3d57b266e04d58ceedd30a6c5428caa6783ca301ecc858c8aa62a8f682a3a`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 05 Aug 2021 19:44:34 GMT
RUN Install update 1809-amd64
# Wed, 25 Aug 2021 13:46:35 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 25 Aug 2021 16:05:30 GMT
ENV NATS_DOCKERIZED=1
# Fri, 27 Aug 2021 00:14:05 GMT
ENV NATS_SERVER=2.4.0
# Fri, 27 Aug 2021 00:14:06 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.4.0/nats-server-v2.4.0-windows-amd64.zip
# Fri, 27 Aug 2021 00:14:07 GMT
ENV NATS_SERVER_SHASUM=6c66acf5ed7e87a1ed9c499033c8c64c8c1365c5a95973ec57859abf1a69b032
# Fri, 27 Aug 2021 00:15:10 GMT
RUN Set-PSDebug -Trace 2
# Fri, 27 Aug 2021 00:16:22 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 27 Aug 2021 00:16:23 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 27 Aug 2021 00:16:24 GMT
EXPOSE 4222 6222 8222
# Fri, 27 Aug 2021 00:16:25 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 27 Aug 2021 00:16:26 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c67ded6868b61d392a0c096f911563fd6bc0bc3ed4fe401d077b3718a1b0cdaf`  
		Size: 967.7 MB (967665054 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:985da5cbc0735e1c422e766af23125ba345f431cb337ea43ec32298d0bb8e4ea`  
		Last Modified: Wed, 25 Aug 2021 15:45:02 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3dbdd68a4b0c278695b3e1d401d7eddfb0f0e3aa1e28aed88eb700059648f8f`  
		Last Modified: Wed, 25 Aug 2021 16:11:02 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9924833e15cbbaa8bd2d64c942c877c0765ba95d0790a5a9ea83a3d40bcaba43`  
		Last Modified: Fri, 27 Aug 2021 00:20:04 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93b8b51ab5e087ce5a5187d2967b0a82e4ce38b2151fc1b040be11a843334b1a`  
		Last Modified: Fri, 27 Aug 2021 00:20:00 GMT  
		Size: 1.4 KB (1360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73666a2686d6829048f4fa9f037f08038370c72202369f80bd4b715ead2cafe3`  
		Last Modified: Fri, 27 Aug 2021 00:20:00 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e35fdb95a7dc56c84ff744d8172574e2edd053f77affad83306be03c14fdb9fb`  
		Last Modified: Fri, 27 Aug 2021 00:20:01 GMT  
		Size: 372.5 KB (372513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3b9b9590a746c11677c6728f047f437a87645f68249b9691ed347591b850b8d`  
		Last Modified: Fri, 27 Aug 2021 00:20:00 GMT  
		Size: 4.9 MB (4944435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b629e22fb2c409b07df4f55a5b1c1d392ae3fc7110b646f46f63c8de8af0f470`  
		Last Modified: Fri, 27 Aug 2021 00:19:58 GMT  
		Size: 2.0 KB (1978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12c15056241134a8112b0c3e43493f7be7cd0421808ee5edbddb6490f355110e`  
		Last Modified: Fri, 27 Aug 2021 00:19:58 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27b1ee4ad1c87cc30317f9c2212c416f2a120923e62f8f88b8192c58d07a9dc1`  
		Last Modified: Fri, 27 Aug 2021 00:19:58 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1f840f93a8499fdb3efd112f5eedcef4290ba5edc497321ae223cdfc4dcb80e`  
		Last Modified: Fri, 27 Aug 2021 00:19:58 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:windowsservercore-ltsc2016`

```console
$ docker pull nats@sha256:7b1ad12d6c6e44e24975eb80e1111d97db29e82416a00dadd5e14a67bf6c0ae4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.14393.4583; amd64

### `nats:windowsservercore-ltsc2016` - windows version 10.0.14393.4583; amd64

```console
$ docker pull nats@sha256:f6699a354c1c84d5ad72289d99c815e7bf11f983cd786684a5015745992e58e4
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6276264126 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af044355ba3348cfc4c9fb174c578e012f1a979a5d04b3681aafc9c2d9411eff`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Sun, 01 Aug 2021 08:52:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 25 Aug 2021 13:59:32 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 25 Aug 2021 16:08:06 GMT
ENV NATS_DOCKERIZED=1
# Fri, 27 Aug 2021 00:16:54 GMT
ENV NATS_SERVER=2.4.0
# Fri, 27 Aug 2021 00:16:55 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.4.0/nats-server-v2.4.0-windows-amd64.zip
# Fri, 27 Aug 2021 00:16:56 GMT
ENV NATS_SERVER_SHASUM=6c66acf5ed7e87a1ed9c499033c8c64c8c1365c5a95973ec57859abf1a69b032
# Fri, 27 Aug 2021 00:17:57 GMT
RUN Set-PSDebug -Trace 2
# Fri, 27 Aug 2021 00:19:20 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 27 Aug 2021 00:19:21 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 27 Aug 2021 00:19:21 GMT
EXPOSE 4222 6222 8222
# Fri, 27 Aug 2021 00:19:22 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 27 Aug 2021 00:19:23 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c427f892fe74603ae09d4e49b25f8f7046f957054034dc9f462e0e88d7bffaa5`  
		Size: 2.2 GB (2200980134 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a869803fc3d8292f0fe1bc6ed35e1ceedbd7c797a1486767a55f88c6c28ed4c5`  
		Last Modified: Wed, 25 Aug 2021 15:45:25 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a745f96c10790ef3a2006dbd4c116eb2f1552fd3c4a38fca179a8160e9918ac1`  
		Last Modified: Wed, 25 Aug 2021 16:11:42 GMT  
		Size: 1.3 KB (1329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ecbc2c744fbea737586b320c08b480fbd8eb2dc994300a74c6a4864ee082901`  
		Last Modified: Fri, 27 Aug 2021 00:20:37 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c530ba921538bcf67912fb5a5d6794e991501dbca08ae8137712fc58854f4f68`  
		Last Modified: Fri, 27 Aug 2021 00:20:37 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35523016d41ba152afbfa0a809770805058865f49d17d6d04d77fab412e5c29d`  
		Last Modified: Fri, 27 Aug 2021 00:20:37 GMT  
		Size: 1.4 KB (1383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:348276d7a124485ea8bc7bad9b9147c84dd20fda1da976a1542cbdb907e4ea95`  
		Last Modified: Fri, 27 Aug 2021 00:20:37 GMT  
		Size: 336.1 KB (336071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:751871e4a816cbaed81ad603047b0c9b536c2180dd5e54f7874d1ca37ef57851`  
		Last Modified: Fri, 27 Aug 2021 00:20:36 GMT  
		Size: 4.9 MB (4948899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d9507c0638be8fdbc5f10f76a31d751acfd94e02618ac7528b4856051bb3721`  
		Last Modified: Fri, 27 Aug 2021 00:20:35 GMT  
		Size: 2.0 KB (1979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:784f2e48cdd62d72893e3cf7316c3c7764e937b9ccade0cb0ce5547ee1e1a304`  
		Last Modified: Fri, 27 Aug 2021 00:20:35 GMT  
		Size: 1.4 KB (1357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc0ba660ed14d0923ea760b909e13fa4ff5bc4fe34acc4e9b0e5e072b2cd9704`  
		Last Modified: Fri, 27 Aug 2021 00:20:35 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f34329777aaf85af2b82ec6fa6640f757cc9589247f7fe67e427a4e39c19bda`  
		Last Modified: Fri, 27 Aug 2021 00:20:35 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
