<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `nats`

-	[`nats:2`](#nats2)
-	[`nats:2-alpine`](#nats2-alpine)
-	[`nats:2-alpine3.15`](#nats2-alpine315)
-	[`nats:2-linux`](#nats2-linux)
-	[`nats:2-nanoserver`](#nats2-nanoserver)
-	[`nats:2-nanoserver-1809`](#nats2-nanoserver-1809)
-	[`nats:2-scratch`](#nats2-scratch)
-	[`nats:2-windowsservercore`](#nats2-windowsservercore)
-	[`nats:2-windowsservercore-1809`](#nats2-windowsservercore-1809)
-	[`nats:2.8`](#nats28)
-	[`nats:2.8-alpine`](#nats28-alpine)
-	[`nats:2.8-alpine3.15`](#nats28-alpine315)
-	[`nats:2.8-linux`](#nats28-linux)
-	[`nats:2.8-nanoserver`](#nats28-nanoserver)
-	[`nats:2.8-nanoserver-1809`](#nats28-nanoserver-1809)
-	[`nats:2.8-scratch`](#nats28-scratch)
-	[`nats:2.8-windowsservercore`](#nats28-windowsservercore)
-	[`nats:2.8-windowsservercore-1809`](#nats28-windowsservercore-1809)
-	[`nats:2.8.2`](#nats282)
-	[`nats:2.8.2-alpine`](#nats282-alpine)
-	[`nats:2.8.2-alpine3.15`](#nats282-alpine315)
-	[`nats:2.8.2-linux`](#nats282-linux)
-	[`nats:2.8.2-nanoserver`](#nats282-nanoserver)
-	[`nats:2.8.2-nanoserver-1809`](#nats282-nanoserver-1809)
-	[`nats:2.8.2-scratch`](#nats282-scratch)
-	[`nats:2.8.2-windowsservercore`](#nats282-windowsservercore)
-	[`nats:2.8.2-windowsservercore-1809`](#nats282-windowsservercore-1809)
-	[`nats:alpine`](#natsalpine)
-	[`nats:alpine3.15`](#natsalpine315)
-	[`nats:latest`](#natslatest)
-	[`nats:linux`](#natslinux)
-	[`nats:nanoserver`](#natsnanoserver)
-	[`nats:nanoserver-1809`](#natsnanoserver-1809)
-	[`nats:scratch`](#natsscratch)
-	[`nats:windowsservercore`](#natswindowsservercore)
-	[`nats:windowsservercore-1809`](#natswindowsservercore-1809)

## `nats:2`

```console
$ docker pull nats@sha256:78f4dc57504675513e5051ce8f64598ddede060ec74a5ff9f253143b7a081503
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.2803; amd64

### `nats:2` - linux; amd64

```console
$ docker pull nats@sha256:d7022e467f53812285667fd004413e8cb15920efbb01d1d0f7c4194a2e084959
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4580109 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:71863590dea616f7cf93b753e1e7a3baf16f89747f06004d08f65d3fa907ee9a`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 04 May 2022 21:19:54 GMT
COPY file:1b0e004de765c2bffa3154a8b1990e8a621636f4f1d7ff504c566b8ba440d227 in /nats-server 
# Wed, 04 May 2022 21:19:54 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 04 May 2022 21:19:54 GMT
EXPOSE 4222 6222 8222
# Wed, 04 May 2022 21:19:54 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 04 May 2022 21:19:54 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 04 May 2022 21:19:54 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:cf7d6008a72749fed702f25d8a1bb63636b75bf34655ba074286dc54d0db2b5b`  
		Last Modified: Wed, 04 May 2022 21:20:43 GMT  
		Size: 4.6 MB (4579600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3ef91ad4507cb0bd768e027792377ba07aaaebc8d89981a6ee648d58561273b`  
		Last Modified: Wed, 04 May 2022 21:20:43 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - linux; arm variant v6

```console
$ docker pull nats@sha256:80a268344378d95bf616b13ab6e787e5a242cadbaa9c933e6708bb8761cab22f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4238279 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d53b2041383be620a877c3c265658998b4c5a2f31c6f26d3dd2aa53cb78cf527`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 04 May 2022 22:01:42 GMT
COPY file:ed82059457db34cc43492a36d55b5f9133e36b8d203dcc971bb9feb5fb6a8528 in /nats-server 
# Wed, 04 May 2022 22:01:42 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 04 May 2022 22:01:43 GMT
EXPOSE 4222 6222 8222
# Wed, 04 May 2022 22:01:43 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 04 May 2022 22:01:44 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 04 May 2022 22:01:44 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b04b6f92c475d8e5e8cdec268c94ef3240dde7149afb05913d1099a7ae570a08`  
		Last Modified: Wed, 04 May 2022 22:04:04 GMT  
		Size: 4.2 MB (4237771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef916f73f04fb010ef2bb2bf3b7260ca2d52efb2591d966721af6b5251fd397d`  
		Last Modified: Wed, 04 May 2022 22:04:02 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - linux; arm variant v7

```console
$ docker pull nats@sha256:5faa61f14caf7dc441f38d86641bd5918d1231b40e7acd0336f57843d8ef704b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4232641 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c4caf3fcf0c7865ec8500f33783b2ba88253c0e14828b887cc8b103228346c5`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 04 May 2022 22:18:15 GMT
COPY file:2f9ffa15f39f94a4d8c8c940d7ec0b2baee22852f8f3f2c24a707b69fc8fd84f in /nats-server 
# Wed, 04 May 2022 22:18:15 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 04 May 2022 22:18:16 GMT
EXPOSE 4222 6222 8222
# Wed, 04 May 2022 22:18:16 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 04 May 2022 22:18:17 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 04 May 2022 22:18:17 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:706ff613d28c2f6958458bb4d4ce83f519f2b76bde307418fe1603aac99ac21b`  
		Last Modified: Wed, 04 May 2022 22:20:36 GMT  
		Size: 4.2 MB (4232133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb718277dd458fca567c81e0168c051df2d97f4a8eb0cb348574822d90dec67d`  
		Last Modified: Wed, 04 May 2022 22:20:33 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:009869128938685fc6fee44029ac90758f29d3fc3e33fa7d5e47a7a3905ef115
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4218329 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a787d12c02030cc31984da44a61d89f3f472271982d215d29866617891286b13`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 04 May 2022 21:48:41 GMT
COPY file:8d0405148efb3d718582f81ff5f54494a8c9789f05e85832ee98d04d228af450 in /nats-server 
# Wed, 04 May 2022 21:48:42 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 04 May 2022 21:48:42 GMT
EXPOSE 4222 6222 8222
# Wed, 04 May 2022 21:48:43 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 04 May 2022 21:48:44 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 04 May 2022 21:48:45 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:8d57fa8f4dba3b0b06e2fd0e4e7b35276d5c1078bcf1be00321d6d56bba9aa78`  
		Last Modified: Wed, 04 May 2022 21:50:01 GMT  
		Size: 4.2 MB (4217820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b388c4e085cdf26d57e7c86c2bec5f6519929e7f9ec591330158ba39d77677b4`  
		Last Modified: Wed, 04 May 2022 21:50:00 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - windows version 10.0.17763.2803; amd64

```console
$ docker pull nats@sha256:2b4914d94facbb6299c5ef2598f655a224c0f671a265bd2986f62c70b978582c
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.7 MB (107725201 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:762896cf7b68aecb4d2820c48789eeee8a8cbc7a58862c4bec5f4ad9d2ecd8f3`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 04 Apr 2022 10:52:49 GMT
RUN Apply image 1809-amd64
# Wed, 13 Apr 2022 14:45:42 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 04 May 2022 21:17:46 GMT
RUN cmd /S /C #(nop) COPY file:1e690007468fe11473f18dc8fbc8b7aa29351e71d03ca73f75d9fcfbf1fd7911 in C:\nats-server.exe 
# Wed, 04 May 2022 21:17:47 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 04 May 2022 21:17:48 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 04 May 2022 21:17:49 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 04 May 2022 21:17:49 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6fc97003d8b7f593fe071cf3ea64f3ce760cc060f3402bb6b1b849c040e222d5`  
		Size: 103.1 MB (103096169 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a6063f744e542c21ce471bdd7ff0dd6063d8d2a9670afbbc64d086813afd6385`  
		Last Modified: Wed, 13 Apr 2022 14:46:35 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c1e5f9285a324194ea2fae24594852b07a0fc1cec1388dcbc367215de23c29e`  
		Last Modified: Wed, 04 May 2022 21:18:39 GMT  
		Size: 4.6 MB (4622651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bde4044fa24dd3365cdc6ba5dff0779813bd4d34e566af1a5c4458c0a232fdc1`  
		Last Modified: Wed, 04 May 2022 21:18:38 GMT  
		Size: 1.8 KB (1791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:405a229a99882e5792c0dad43c80fb315b37c8b9c347f514baccd7d05c6c9f1c`  
		Last Modified: Wed, 04 May 2022 21:18:38 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1037a060f2ca6801837d7d720ec02ed6916e48ce1cfa49e6c7558ba04de8235`  
		Last Modified: Wed, 04 May 2022 21:18:38 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e29f6c2056586ca9353c7019499d854ba31068b682d59304ed4267576ebc5286`  
		Last Modified: Wed, 04 May 2022 21:18:38 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-alpine`

```console
$ docker pull nats@sha256:51ed1dcadcd928cbca6b4b2846491bd14667dca111ac63fdb001eef89cb9192f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-alpine` - linux; amd64

```console
$ docker pull nats@sha256:3dfa6b8def0d3c784ef7827f0c21b17afd01be56773c68d5950e9f29172ae796
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.7 MB (7667828 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3370f8d5fa5f0ea4cfdcaa60d7f568c2cf9e9752f3a75d11b0d30a257db8a51d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 05 Apr 2022 00:19:59 GMT
ADD file:5d673d25da3a14ce1f6cf66e4c7fd4f4b85a3759a9d93efb3fd9ff852b5b56e4 in / 
# Tue, 05 Apr 2022 00:19:59 GMT
CMD ["/bin/sh"]
# Wed, 04 May 2022 21:19:44 GMT
ENV NATS_SERVER=2.8.2
# Wed, 04 May 2022 21:19:47 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='3409b9dc76c0136cecded67115521d3a815f7a2f3739e81eb87a8d5d761843c3' ;; 		armhf) natsArch='arm6'; sha256='a3d474a583ca90e3577aa470335c582d4565918f500ebd28d760643fb631d8d5' ;; 		armv7) natsArch='arm7'; sha256='88fd437f7def8dbe68b17dce703c919771e64b570856bf0e6f2eb3b9459031c6' ;; 		x86_64) natsArch='amd64'; sha256='59805a464237801574ca7efdc69ebc21040e9b811fb53ed444c4808a05440719' ;; 		x86) natsArch='386'; sha256='facd3c69ee27c3e9e8654e5de95eb79de2e873bf4c066317aa9fad5c2ea26b92' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 04 May 2022 21:19:47 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 04 May 2022 21:19:47 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 04 May 2022 21:19:47 GMT
EXPOSE 4222 6222 8222
# Wed, 04 May 2022 21:19:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 04 May 2022 21:19:47 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:df9b9388f04ad6279a7410b85cedfdcb2208c0a003da7ab5613af71079148139`  
		Last Modified: Mon, 04 Apr 2022 19:10:16 GMT  
		Size: 2.8 MB (2814559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb157527e1f2e860f2700cadfdf0bed3ac0d50b8a177dd0b906431b0d46b44b5`  
		Last Modified: Wed, 04 May 2022 21:20:20 GMT  
		Size: 4.9 MB (4852271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c29bade32b2ef2ecc8325cbc5cbbf69470e5e20cc04e292244e704f68b9a6f86`  
		Last Modified: Wed, 04 May 2022 21:20:19 GMT  
		Size: 585.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dbec41bc3a042cdbf4c2e9b57c99bf99a4552e64a437be0066d42a04e3de650`  
		Last Modified: Wed, 04 May 2022 21:20:19 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:12b766cef3be0b9dc70e35a9cefcecbfad16a19e00b94a4737134ebbee24ea31
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7133599 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d1cc5ce43b7fd2c1dc34d986696c64da1a158fc067f5a4710ce475ce2f10eaec`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 04 Apr 2022 23:49:42 GMT
ADD file:159dcddaab900372df882a4e94615ed84250e9cea3e74bc0479d98280342f596 in / 
# Mon, 04 Apr 2022 23:49:42 GMT
CMD ["/bin/sh"]
# Wed, 04 May 2022 22:01:15 GMT
ENV NATS_SERVER=2.8.2
# Wed, 04 May 2022 22:01:19 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='3409b9dc76c0136cecded67115521d3a815f7a2f3739e81eb87a8d5d761843c3' ;; 		armhf) natsArch='arm6'; sha256='a3d474a583ca90e3577aa470335c582d4565918f500ebd28d760643fb631d8d5' ;; 		armv7) natsArch='arm7'; sha256='88fd437f7def8dbe68b17dce703c919771e64b570856bf0e6f2eb3b9459031c6' ;; 		x86_64) natsArch='amd64'; sha256='59805a464237801574ca7efdc69ebc21040e9b811fb53ed444c4808a05440719' ;; 		x86) natsArch='386'; sha256='facd3c69ee27c3e9e8654e5de95eb79de2e873bf4c066317aa9fad5c2ea26b92' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 04 May 2022 22:01:20 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 04 May 2022 22:01:20 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 04 May 2022 22:01:21 GMT
EXPOSE 4222 6222 8222
# Wed, 04 May 2022 22:01:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 04 May 2022 22:01:21 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:c319b1fc4ed70b8241a7ce6ac0c4015d354bf5cf8c01eb73c50b6709c0c46e49`  
		Last Modified: Mon, 04 Apr 2022 19:09:22 GMT  
		Size: 2.6 MB (2621972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3508da0a7a8c69badd89084de30d788f3c0bc57d625677ec7d68c32f18d466ba`  
		Last Modified: Wed, 04 May 2022 22:03:28 GMT  
		Size: 4.5 MB (4510625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7965b001731ee55e0b7b2c11c7ff5f851afaed57dba5ef2a08324fab5de994f7`  
		Last Modified: Wed, 04 May 2022 22:03:27 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8d031fa4afb68088db4a684f2332c5c8c3ecedb55d2aee461d64c8556afb468`  
		Last Modified: Wed, 04 May 2022 22:03:25 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:7d6c71099975b1e928511819a05612d582d412c5ed2838f04882514d0e77fff8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.9 MB (6930001 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3813055a26f58efed9d97ad053203ba493589fa6e486f3dd5810354defc6b3c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 04 Apr 2022 23:57:34 GMT
ADD file:20f8cdddc53a4a8bd78945fc32fe08e9f80ab3b16dc20a9aa4ba73b79f2bc71c in / 
# Mon, 04 Apr 2022 23:57:35 GMT
CMD ["/bin/sh"]
# Wed, 04 May 2022 22:17:46 GMT
ENV NATS_SERVER=2.8.2
# Wed, 04 May 2022 22:17:50 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='3409b9dc76c0136cecded67115521d3a815f7a2f3739e81eb87a8d5d761843c3' ;; 		armhf) natsArch='arm6'; sha256='a3d474a583ca90e3577aa470335c582d4565918f500ebd28d760643fb631d8d5' ;; 		armv7) natsArch='arm7'; sha256='88fd437f7def8dbe68b17dce703c919771e64b570856bf0e6f2eb3b9459031c6' ;; 		x86_64) natsArch='amd64'; sha256='59805a464237801574ca7efdc69ebc21040e9b811fb53ed444c4808a05440719' ;; 		x86) natsArch='386'; sha256='facd3c69ee27c3e9e8654e5de95eb79de2e873bf4c066317aa9fad5c2ea26b92' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 04 May 2022 22:17:50 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 04 May 2022 22:17:51 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 04 May 2022 22:17:51 GMT
EXPOSE 4222 6222 8222
# Wed, 04 May 2022 22:17:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 04 May 2022 22:17:52 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:57fb4b5f1a47c953ca5703f0f81ce14e5d01cf23aa79558b5adb961cc526e320`  
		Last Modified: Mon, 04 Apr 2022 19:09:36 GMT  
		Size: 2.4 MB (2424323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b49f3de3c7329a4a2fbd9e8c9cd595a837860930995c5a11d2459e045b8d2dab`  
		Last Modified: Wed, 04 May 2022 22:20:00 GMT  
		Size: 4.5 MB (4504680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51dc12ec06d594c70e53bb45c9912d27ad4869faf092615047ea9faab11d6ccb`  
		Last Modified: Wed, 04 May 2022 22:19:57 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5e0c0af17ebf42f5af072c2b71c091af0b659ac5e20a80c92ca74da9ec5353d`  
		Last Modified: Wed, 04 May 2022 22:19:57 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:81e20b06f2b5aac1ca438142975de9c05234b243fcb497ab8afd7f0bcd4a28a8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7208259 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12c2a5e86ad6fc84ed6f66fecfc26474466d0f61712b85aa012fc0b7e726019e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:31 GMT
ADD file:90e56af13188c7f0283d244a0d70b853d8bef8587a41f1da8eac3a2aba8964ef in / 
# Mon, 04 Apr 2022 23:39:31 GMT
CMD ["/bin/sh"]
# Wed, 04 May 2022 21:48:24 GMT
ENV NATS_SERVER=2.8.2
# Wed, 04 May 2022 21:48:26 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='3409b9dc76c0136cecded67115521d3a815f7a2f3739e81eb87a8d5d761843c3' ;; 		armhf) natsArch='arm6'; sha256='a3d474a583ca90e3577aa470335c582d4565918f500ebd28d760643fb631d8d5' ;; 		armv7) natsArch='arm7'; sha256='88fd437f7def8dbe68b17dce703c919771e64b570856bf0e6f2eb3b9459031c6' ;; 		x86_64) natsArch='amd64'; sha256='59805a464237801574ca7efdc69ebc21040e9b811fb53ed444c4808a05440719' ;; 		x86) natsArch='386'; sha256='facd3c69ee27c3e9e8654e5de95eb79de2e873bf4c066317aa9fad5c2ea26b92' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 04 May 2022 21:48:28 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 04 May 2022 21:48:29 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 04 May 2022 21:48:29 GMT
EXPOSE 4222 6222 8222
# Wed, 04 May 2022 21:48:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 04 May 2022 21:48:31 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9981e73032c8833e387a8f96986e560edbed12c38119e0edb0439c9c2234eac9`  
		Last Modified: Mon, 04 Apr 2022 19:09:10 GMT  
		Size: 2.7 MB (2716477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec7ea9151b15b8e90d2a0ef58393de32cefb12a7f7c7e3d7a011808b38e59565`  
		Last Modified: Wed, 04 May 2022 21:49:31 GMT  
		Size: 4.5 MB (4490808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f800447a181fc7e3f37c2e68d8374347459e1d12a8d8c8653b7da45180ae97f`  
		Last Modified: Wed, 04 May 2022 21:49:30 GMT  
		Size: 560.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:894f3b307d2ae2b261df9d763e886b3ae75f9aba6dc927eaf3f28cae9375c050`  
		Last Modified: Wed, 04 May 2022 21:49:30 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-alpine3.15`

```console
$ docker pull nats@sha256:51ed1dcadcd928cbca6b4b2846491bd14667dca111ac63fdb001eef89cb9192f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-alpine3.15` - linux; amd64

```console
$ docker pull nats@sha256:3dfa6b8def0d3c784ef7827f0c21b17afd01be56773c68d5950e9f29172ae796
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.7 MB (7667828 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3370f8d5fa5f0ea4cfdcaa60d7f568c2cf9e9752f3a75d11b0d30a257db8a51d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 05 Apr 2022 00:19:59 GMT
ADD file:5d673d25da3a14ce1f6cf66e4c7fd4f4b85a3759a9d93efb3fd9ff852b5b56e4 in / 
# Tue, 05 Apr 2022 00:19:59 GMT
CMD ["/bin/sh"]
# Wed, 04 May 2022 21:19:44 GMT
ENV NATS_SERVER=2.8.2
# Wed, 04 May 2022 21:19:47 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='3409b9dc76c0136cecded67115521d3a815f7a2f3739e81eb87a8d5d761843c3' ;; 		armhf) natsArch='arm6'; sha256='a3d474a583ca90e3577aa470335c582d4565918f500ebd28d760643fb631d8d5' ;; 		armv7) natsArch='arm7'; sha256='88fd437f7def8dbe68b17dce703c919771e64b570856bf0e6f2eb3b9459031c6' ;; 		x86_64) natsArch='amd64'; sha256='59805a464237801574ca7efdc69ebc21040e9b811fb53ed444c4808a05440719' ;; 		x86) natsArch='386'; sha256='facd3c69ee27c3e9e8654e5de95eb79de2e873bf4c066317aa9fad5c2ea26b92' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 04 May 2022 21:19:47 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 04 May 2022 21:19:47 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 04 May 2022 21:19:47 GMT
EXPOSE 4222 6222 8222
# Wed, 04 May 2022 21:19:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 04 May 2022 21:19:47 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:df9b9388f04ad6279a7410b85cedfdcb2208c0a003da7ab5613af71079148139`  
		Last Modified: Mon, 04 Apr 2022 19:10:16 GMT  
		Size: 2.8 MB (2814559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb157527e1f2e860f2700cadfdf0bed3ac0d50b8a177dd0b906431b0d46b44b5`  
		Last Modified: Wed, 04 May 2022 21:20:20 GMT  
		Size: 4.9 MB (4852271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c29bade32b2ef2ecc8325cbc5cbbf69470e5e20cc04e292244e704f68b9a6f86`  
		Last Modified: Wed, 04 May 2022 21:20:19 GMT  
		Size: 585.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dbec41bc3a042cdbf4c2e9b57c99bf99a4552e64a437be0066d42a04e3de650`  
		Last Modified: Wed, 04 May 2022 21:20:19 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.15` - linux; arm variant v6

```console
$ docker pull nats@sha256:12b766cef3be0b9dc70e35a9cefcecbfad16a19e00b94a4737134ebbee24ea31
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7133599 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d1cc5ce43b7fd2c1dc34d986696c64da1a158fc067f5a4710ce475ce2f10eaec`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 04 Apr 2022 23:49:42 GMT
ADD file:159dcddaab900372df882a4e94615ed84250e9cea3e74bc0479d98280342f596 in / 
# Mon, 04 Apr 2022 23:49:42 GMT
CMD ["/bin/sh"]
# Wed, 04 May 2022 22:01:15 GMT
ENV NATS_SERVER=2.8.2
# Wed, 04 May 2022 22:01:19 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='3409b9dc76c0136cecded67115521d3a815f7a2f3739e81eb87a8d5d761843c3' ;; 		armhf) natsArch='arm6'; sha256='a3d474a583ca90e3577aa470335c582d4565918f500ebd28d760643fb631d8d5' ;; 		armv7) natsArch='arm7'; sha256='88fd437f7def8dbe68b17dce703c919771e64b570856bf0e6f2eb3b9459031c6' ;; 		x86_64) natsArch='amd64'; sha256='59805a464237801574ca7efdc69ebc21040e9b811fb53ed444c4808a05440719' ;; 		x86) natsArch='386'; sha256='facd3c69ee27c3e9e8654e5de95eb79de2e873bf4c066317aa9fad5c2ea26b92' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 04 May 2022 22:01:20 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 04 May 2022 22:01:20 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 04 May 2022 22:01:21 GMT
EXPOSE 4222 6222 8222
# Wed, 04 May 2022 22:01:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 04 May 2022 22:01:21 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:c319b1fc4ed70b8241a7ce6ac0c4015d354bf5cf8c01eb73c50b6709c0c46e49`  
		Last Modified: Mon, 04 Apr 2022 19:09:22 GMT  
		Size: 2.6 MB (2621972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3508da0a7a8c69badd89084de30d788f3c0bc57d625677ec7d68c32f18d466ba`  
		Last Modified: Wed, 04 May 2022 22:03:28 GMT  
		Size: 4.5 MB (4510625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7965b001731ee55e0b7b2c11c7ff5f851afaed57dba5ef2a08324fab5de994f7`  
		Last Modified: Wed, 04 May 2022 22:03:27 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8d031fa4afb68088db4a684f2332c5c8c3ecedb55d2aee461d64c8556afb468`  
		Last Modified: Wed, 04 May 2022 22:03:25 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.15` - linux; arm variant v7

```console
$ docker pull nats@sha256:7d6c71099975b1e928511819a05612d582d412c5ed2838f04882514d0e77fff8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.9 MB (6930001 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3813055a26f58efed9d97ad053203ba493589fa6e486f3dd5810354defc6b3c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 04 Apr 2022 23:57:34 GMT
ADD file:20f8cdddc53a4a8bd78945fc32fe08e9f80ab3b16dc20a9aa4ba73b79f2bc71c in / 
# Mon, 04 Apr 2022 23:57:35 GMT
CMD ["/bin/sh"]
# Wed, 04 May 2022 22:17:46 GMT
ENV NATS_SERVER=2.8.2
# Wed, 04 May 2022 22:17:50 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='3409b9dc76c0136cecded67115521d3a815f7a2f3739e81eb87a8d5d761843c3' ;; 		armhf) natsArch='arm6'; sha256='a3d474a583ca90e3577aa470335c582d4565918f500ebd28d760643fb631d8d5' ;; 		armv7) natsArch='arm7'; sha256='88fd437f7def8dbe68b17dce703c919771e64b570856bf0e6f2eb3b9459031c6' ;; 		x86_64) natsArch='amd64'; sha256='59805a464237801574ca7efdc69ebc21040e9b811fb53ed444c4808a05440719' ;; 		x86) natsArch='386'; sha256='facd3c69ee27c3e9e8654e5de95eb79de2e873bf4c066317aa9fad5c2ea26b92' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 04 May 2022 22:17:50 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 04 May 2022 22:17:51 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 04 May 2022 22:17:51 GMT
EXPOSE 4222 6222 8222
# Wed, 04 May 2022 22:17:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 04 May 2022 22:17:52 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:57fb4b5f1a47c953ca5703f0f81ce14e5d01cf23aa79558b5adb961cc526e320`  
		Last Modified: Mon, 04 Apr 2022 19:09:36 GMT  
		Size: 2.4 MB (2424323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b49f3de3c7329a4a2fbd9e8c9cd595a837860930995c5a11d2459e045b8d2dab`  
		Last Modified: Wed, 04 May 2022 22:20:00 GMT  
		Size: 4.5 MB (4504680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51dc12ec06d594c70e53bb45c9912d27ad4869faf092615047ea9faab11d6ccb`  
		Last Modified: Wed, 04 May 2022 22:19:57 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5e0c0af17ebf42f5af072c2b71c091af0b659ac5e20a80c92ca74da9ec5353d`  
		Last Modified: Wed, 04 May 2022 22:19:57 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.15` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:81e20b06f2b5aac1ca438142975de9c05234b243fcb497ab8afd7f0bcd4a28a8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7208259 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12c2a5e86ad6fc84ed6f66fecfc26474466d0f61712b85aa012fc0b7e726019e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:31 GMT
ADD file:90e56af13188c7f0283d244a0d70b853d8bef8587a41f1da8eac3a2aba8964ef in / 
# Mon, 04 Apr 2022 23:39:31 GMT
CMD ["/bin/sh"]
# Wed, 04 May 2022 21:48:24 GMT
ENV NATS_SERVER=2.8.2
# Wed, 04 May 2022 21:48:26 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='3409b9dc76c0136cecded67115521d3a815f7a2f3739e81eb87a8d5d761843c3' ;; 		armhf) natsArch='arm6'; sha256='a3d474a583ca90e3577aa470335c582d4565918f500ebd28d760643fb631d8d5' ;; 		armv7) natsArch='arm7'; sha256='88fd437f7def8dbe68b17dce703c919771e64b570856bf0e6f2eb3b9459031c6' ;; 		x86_64) natsArch='amd64'; sha256='59805a464237801574ca7efdc69ebc21040e9b811fb53ed444c4808a05440719' ;; 		x86) natsArch='386'; sha256='facd3c69ee27c3e9e8654e5de95eb79de2e873bf4c066317aa9fad5c2ea26b92' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 04 May 2022 21:48:28 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 04 May 2022 21:48:29 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 04 May 2022 21:48:29 GMT
EXPOSE 4222 6222 8222
# Wed, 04 May 2022 21:48:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 04 May 2022 21:48:31 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9981e73032c8833e387a8f96986e560edbed12c38119e0edb0439c9c2234eac9`  
		Last Modified: Mon, 04 Apr 2022 19:09:10 GMT  
		Size: 2.7 MB (2716477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec7ea9151b15b8e90d2a0ef58393de32cefb12a7f7c7e3d7a011808b38e59565`  
		Last Modified: Wed, 04 May 2022 21:49:31 GMT  
		Size: 4.5 MB (4490808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f800447a181fc7e3f37c2e68d8374347459e1d12a8d8c8653b7da45180ae97f`  
		Last Modified: Wed, 04 May 2022 21:49:30 GMT  
		Size: 560.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:894f3b307d2ae2b261df9d763e886b3ae75f9aba6dc927eaf3f28cae9375c050`  
		Last Modified: Wed, 04 May 2022 21:49:30 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-linux`

```console
$ docker pull nats@sha256:dd400785e2c069158ca6a488873976cab93098904db7fcc044cfc6af0327640c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-linux` - linux; amd64

```console
$ docker pull nats@sha256:d7022e467f53812285667fd004413e8cb15920efbb01d1d0f7c4194a2e084959
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4580109 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:71863590dea616f7cf93b753e1e7a3baf16f89747f06004d08f65d3fa907ee9a`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 04 May 2022 21:19:54 GMT
COPY file:1b0e004de765c2bffa3154a8b1990e8a621636f4f1d7ff504c566b8ba440d227 in /nats-server 
# Wed, 04 May 2022 21:19:54 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 04 May 2022 21:19:54 GMT
EXPOSE 4222 6222 8222
# Wed, 04 May 2022 21:19:54 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 04 May 2022 21:19:54 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 04 May 2022 21:19:54 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:cf7d6008a72749fed702f25d8a1bb63636b75bf34655ba074286dc54d0db2b5b`  
		Last Modified: Wed, 04 May 2022 21:20:43 GMT  
		Size: 4.6 MB (4579600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3ef91ad4507cb0bd768e027792377ba07aaaebc8d89981a6ee648d58561273b`  
		Last Modified: Wed, 04 May 2022 21:20:43 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:80a268344378d95bf616b13ab6e787e5a242cadbaa9c933e6708bb8761cab22f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4238279 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d53b2041383be620a877c3c265658998b4c5a2f31c6f26d3dd2aa53cb78cf527`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 04 May 2022 22:01:42 GMT
COPY file:ed82059457db34cc43492a36d55b5f9133e36b8d203dcc971bb9feb5fb6a8528 in /nats-server 
# Wed, 04 May 2022 22:01:42 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 04 May 2022 22:01:43 GMT
EXPOSE 4222 6222 8222
# Wed, 04 May 2022 22:01:43 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 04 May 2022 22:01:44 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 04 May 2022 22:01:44 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b04b6f92c475d8e5e8cdec268c94ef3240dde7149afb05913d1099a7ae570a08`  
		Last Modified: Wed, 04 May 2022 22:04:04 GMT  
		Size: 4.2 MB (4237771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef916f73f04fb010ef2bb2bf3b7260ca2d52efb2591d966721af6b5251fd397d`  
		Last Modified: Wed, 04 May 2022 22:04:02 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:5faa61f14caf7dc441f38d86641bd5918d1231b40e7acd0336f57843d8ef704b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4232641 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c4caf3fcf0c7865ec8500f33783b2ba88253c0e14828b887cc8b103228346c5`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 04 May 2022 22:18:15 GMT
COPY file:2f9ffa15f39f94a4d8c8c940d7ec0b2baee22852f8f3f2c24a707b69fc8fd84f in /nats-server 
# Wed, 04 May 2022 22:18:15 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 04 May 2022 22:18:16 GMT
EXPOSE 4222 6222 8222
# Wed, 04 May 2022 22:18:16 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 04 May 2022 22:18:17 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 04 May 2022 22:18:17 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:706ff613d28c2f6958458bb4d4ce83f519f2b76bde307418fe1603aac99ac21b`  
		Last Modified: Wed, 04 May 2022 22:20:36 GMT  
		Size: 4.2 MB (4232133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb718277dd458fca567c81e0168c051df2d97f4a8eb0cb348574822d90dec67d`  
		Last Modified: Wed, 04 May 2022 22:20:33 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:009869128938685fc6fee44029ac90758f29d3fc3e33fa7d5e47a7a3905ef115
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4218329 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a787d12c02030cc31984da44a61d89f3f472271982d215d29866617891286b13`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 04 May 2022 21:48:41 GMT
COPY file:8d0405148efb3d718582f81ff5f54494a8c9789f05e85832ee98d04d228af450 in /nats-server 
# Wed, 04 May 2022 21:48:42 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 04 May 2022 21:48:42 GMT
EXPOSE 4222 6222 8222
# Wed, 04 May 2022 21:48:43 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 04 May 2022 21:48:44 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 04 May 2022 21:48:45 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:8d57fa8f4dba3b0b06e2fd0e4e7b35276d5c1078bcf1be00321d6d56bba9aa78`  
		Last Modified: Wed, 04 May 2022 21:50:01 GMT  
		Size: 4.2 MB (4217820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b388c4e085cdf26d57e7c86c2bec5f6519929e7f9ec591330158ba39d77677b4`  
		Last Modified: Wed, 04 May 2022 21:50:00 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-nanoserver`

```console
$ docker pull nats@sha256:f128bdd66f848762f7bb7c580b2d89e4c329ce85461597353dcbff405ddda643
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2803; amd64

### `nats:2-nanoserver` - windows version 10.0.17763.2803; amd64

```console
$ docker pull nats@sha256:2b4914d94facbb6299c5ef2598f655a224c0f671a265bd2986f62c70b978582c
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.7 MB (107725201 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:762896cf7b68aecb4d2820c48789eeee8a8cbc7a58862c4bec5f4ad9d2ecd8f3`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 04 Apr 2022 10:52:49 GMT
RUN Apply image 1809-amd64
# Wed, 13 Apr 2022 14:45:42 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 04 May 2022 21:17:46 GMT
RUN cmd /S /C #(nop) COPY file:1e690007468fe11473f18dc8fbc8b7aa29351e71d03ca73f75d9fcfbf1fd7911 in C:\nats-server.exe 
# Wed, 04 May 2022 21:17:47 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 04 May 2022 21:17:48 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 04 May 2022 21:17:49 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 04 May 2022 21:17:49 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6fc97003d8b7f593fe071cf3ea64f3ce760cc060f3402bb6b1b849c040e222d5`  
		Size: 103.1 MB (103096169 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a6063f744e542c21ce471bdd7ff0dd6063d8d2a9670afbbc64d086813afd6385`  
		Last Modified: Wed, 13 Apr 2022 14:46:35 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c1e5f9285a324194ea2fae24594852b07a0fc1cec1388dcbc367215de23c29e`  
		Last Modified: Wed, 04 May 2022 21:18:39 GMT  
		Size: 4.6 MB (4622651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bde4044fa24dd3365cdc6ba5dff0779813bd4d34e566af1a5c4458c0a232fdc1`  
		Last Modified: Wed, 04 May 2022 21:18:38 GMT  
		Size: 1.8 KB (1791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:405a229a99882e5792c0dad43c80fb315b37c8b9c347f514baccd7d05c6c9f1c`  
		Last Modified: Wed, 04 May 2022 21:18:38 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1037a060f2ca6801837d7d720ec02ed6916e48ce1cfa49e6c7558ba04de8235`  
		Last Modified: Wed, 04 May 2022 21:18:38 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e29f6c2056586ca9353c7019499d854ba31068b682d59304ed4267576ebc5286`  
		Last Modified: Wed, 04 May 2022 21:18:38 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-nanoserver-1809`

```console
$ docker pull nats@sha256:f128bdd66f848762f7bb7c580b2d89e4c329ce85461597353dcbff405ddda643
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2803; amd64

### `nats:2-nanoserver-1809` - windows version 10.0.17763.2803; amd64

```console
$ docker pull nats@sha256:2b4914d94facbb6299c5ef2598f655a224c0f671a265bd2986f62c70b978582c
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.7 MB (107725201 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:762896cf7b68aecb4d2820c48789eeee8a8cbc7a58862c4bec5f4ad9d2ecd8f3`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 04 Apr 2022 10:52:49 GMT
RUN Apply image 1809-amd64
# Wed, 13 Apr 2022 14:45:42 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 04 May 2022 21:17:46 GMT
RUN cmd /S /C #(nop) COPY file:1e690007468fe11473f18dc8fbc8b7aa29351e71d03ca73f75d9fcfbf1fd7911 in C:\nats-server.exe 
# Wed, 04 May 2022 21:17:47 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 04 May 2022 21:17:48 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 04 May 2022 21:17:49 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 04 May 2022 21:17:49 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6fc97003d8b7f593fe071cf3ea64f3ce760cc060f3402bb6b1b849c040e222d5`  
		Size: 103.1 MB (103096169 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a6063f744e542c21ce471bdd7ff0dd6063d8d2a9670afbbc64d086813afd6385`  
		Last Modified: Wed, 13 Apr 2022 14:46:35 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c1e5f9285a324194ea2fae24594852b07a0fc1cec1388dcbc367215de23c29e`  
		Last Modified: Wed, 04 May 2022 21:18:39 GMT  
		Size: 4.6 MB (4622651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bde4044fa24dd3365cdc6ba5dff0779813bd4d34e566af1a5c4458c0a232fdc1`  
		Last Modified: Wed, 04 May 2022 21:18:38 GMT  
		Size: 1.8 KB (1791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:405a229a99882e5792c0dad43c80fb315b37c8b9c347f514baccd7d05c6c9f1c`  
		Last Modified: Wed, 04 May 2022 21:18:38 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1037a060f2ca6801837d7d720ec02ed6916e48ce1cfa49e6c7558ba04de8235`  
		Last Modified: Wed, 04 May 2022 21:18:38 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e29f6c2056586ca9353c7019499d854ba31068b682d59304ed4267576ebc5286`  
		Last Modified: Wed, 04 May 2022 21:18:38 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-scratch`

```console
$ docker pull nats@sha256:dd400785e2c069158ca6a488873976cab93098904db7fcc044cfc6af0327640c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-scratch` - linux; amd64

```console
$ docker pull nats@sha256:d7022e467f53812285667fd004413e8cb15920efbb01d1d0f7c4194a2e084959
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4580109 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:71863590dea616f7cf93b753e1e7a3baf16f89747f06004d08f65d3fa907ee9a`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 04 May 2022 21:19:54 GMT
COPY file:1b0e004de765c2bffa3154a8b1990e8a621636f4f1d7ff504c566b8ba440d227 in /nats-server 
# Wed, 04 May 2022 21:19:54 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 04 May 2022 21:19:54 GMT
EXPOSE 4222 6222 8222
# Wed, 04 May 2022 21:19:54 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 04 May 2022 21:19:54 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 04 May 2022 21:19:54 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:cf7d6008a72749fed702f25d8a1bb63636b75bf34655ba074286dc54d0db2b5b`  
		Last Modified: Wed, 04 May 2022 21:20:43 GMT  
		Size: 4.6 MB (4579600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3ef91ad4507cb0bd768e027792377ba07aaaebc8d89981a6ee648d58561273b`  
		Last Modified: Wed, 04 May 2022 21:20:43 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:80a268344378d95bf616b13ab6e787e5a242cadbaa9c933e6708bb8761cab22f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4238279 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d53b2041383be620a877c3c265658998b4c5a2f31c6f26d3dd2aa53cb78cf527`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 04 May 2022 22:01:42 GMT
COPY file:ed82059457db34cc43492a36d55b5f9133e36b8d203dcc971bb9feb5fb6a8528 in /nats-server 
# Wed, 04 May 2022 22:01:42 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 04 May 2022 22:01:43 GMT
EXPOSE 4222 6222 8222
# Wed, 04 May 2022 22:01:43 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 04 May 2022 22:01:44 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 04 May 2022 22:01:44 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b04b6f92c475d8e5e8cdec268c94ef3240dde7149afb05913d1099a7ae570a08`  
		Last Modified: Wed, 04 May 2022 22:04:04 GMT  
		Size: 4.2 MB (4237771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef916f73f04fb010ef2bb2bf3b7260ca2d52efb2591d966721af6b5251fd397d`  
		Last Modified: Wed, 04 May 2022 22:04:02 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:5faa61f14caf7dc441f38d86641bd5918d1231b40e7acd0336f57843d8ef704b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4232641 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c4caf3fcf0c7865ec8500f33783b2ba88253c0e14828b887cc8b103228346c5`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 04 May 2022 22:18:15 GMT
COPY file:2f9ffa15f39f94a4d8c8c940d7ec0b2baee22852f8f3f2c24a707b69fc8fd84f in /nats-server 
# Wed, 04 May 2022 22:18:15 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 04 May 2022 22:18:16 GMT
EXPOSE 4222 6222 8222
# Wed, 04 May 2022 22:18:16 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 04 May 2022 22:18:17 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 04 May 2022 22:18:17 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:706ff613d28c2f6958458bb4d4ce83f519f2b76bde307418fe1603aac99ac21b`  
		Last Modified: Wed, 04 May 2022 22:20:36 GMT  
		Size: 4.2 MB (4232133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb718277dd458fca567c81e0168c051df2d97f4a8eb0cb348574822d90dec67d`  
		Last Modified: Wed, 04 May 2022 22:20:33 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:009869128938685fc6fee44029ac90758f29d3fc3e33fa7d5e47a7a3905ef115
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4218329 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a787d12c02030cc31984da44a61d89f3f472271982d215d29866617891286b13`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 04 May 2022 21:48:41 GMT
COPY file:8d0405148efb3d718582f81ff5f54494a8c9789f05e85832ee98d04d228af450 in /nats-server 
# Wed, 04 May 2022 21:48:42 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 04 May 2022 21:48:42 GMT
EXPOSE 4222 6222 8222
# Wed, 04 May 2022 21:48:43 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 04 May 2022 21:48:44 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 04 May 2022 21:48:45 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:8d57fa8f4dba3b0b06e2fd0e4e7b35276d5c1078bcf1be00321d6d56bba9aa78`  
		Last Modified: Wed, 04 May 2022 21:50:01 GMT  
		Size: 4.2 MB (4217820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b388c4e085cdf26d57e7c86c2bec5f6519929e7f9ec591330158ba39d77677b4`  
		Last Modified: Wed, 04 May 2022 21:50:00 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-windowsservercore`

```console
$ docker pull nats@sha256:73f511081ca198af5f5c5d1d5d609bf6cfc5a7d43f01e1c93b4b718eaa7bc1d7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2803; amd64

### `nats:2-windowsservercore` - windows version 10.0.17763.2803; amd64

```console
$ docker pull nats@sha256:6ed34062ddcdb57863540c220de7d892b2b3152ae6599e25ff1405defc63d9db
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2721253627 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:392c84a5f744aeb82235810dec31fe58510c59683d8530e1727645ae02a45a8f`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 04 Apr 2022 11:20:25 GMT
RUN Install update 1809-amd64
# Wed, 13 Apr 2022 12:43:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 Apr 2022 14:42:30 GMT
ENV NATS_DOCKERIZED=1
# Wed, 04 May 2022 21:14:48 GMT
ENV NATS_SERVER=2.8.2
# Wed, 04 May 2022 21:14:49 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.8.2/nats-server-v2.8.2-windows-amd64.zip
# Wed, 04 May 2022 21:14:50 GMT
ENV NATS_SERVER_SHASUM=300b9743afa50e02e4e8d43dc212bfde8a871617bd524829114e19ff680dde11
# Wed, 04 May 2022 21:15:50 GMT
RUN Set-PSDebug -Trace 2
# Wed, 04 May 2022 21:17:21 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 04 May 2022 21:17:22 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 04 May 2022 21:17:23 GMT
EXPOSE 4222 6222 8222
# Wed, 04 May 2022 21:17:24 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 04 May 2022 21:17:26 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ba8181afd4264392fbbf8df14fb4cddc55fbe085ab000e986b789678bc2bb171`  
		Size: 997.6 MB (997587446 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7ebb23aa64bff633cfa3c62b190d84f0e870b04fecb1910f65d0870b5c7f8981`  
		Last Modified: Wed, 13 Apr 2022 14:12:24 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d838c7a98a95bee63894bac798124e8c8572bcacc23e22d85332d453a03a7d7c`  
		Last Modified: Wed, 13 Apr 2022 14:46:17 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bba18134d0cef899134f811c0896e8003b4b03b11726200e2d4f09ff3e350d1`  
		Last Modified: Wed, 04 May 2022 21:18:21 GMT  
		Size: 1.4 KB (1382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46e1de2ac2611197cf7e3985577bdf089a2330268d7f08ad53a25b42fcf7548b`  
		Last Modified: Wed, 04 May 2022 21:18:21 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:130538769de262aeb26e810412f9ee58d5b8c1aeb653929a4607901c92363b93`  
		Last Modified: Wed, 04 May 2022 21:18:21 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1684bc7f189afcbdc72f3a0c8eab43e13bbfbe3e8fb412ac51356098cefaeb9a`  
		Last Modified: Wed, 04 May 2022 21:18:21 GMT  
		Size: 359.4 KB (359393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c1c4f2e32fa9a2920cfaeae75fe3b7e64312357d7a20b2c5e7347936eef6dc5`  
		Last Modified: Wed, 04 May 2022 21:18:24 GMT  
		Size: 5.0 MB (4960732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c18367f87433f56d999dc8c84a381afa2e8d480302ea8c78e9169557cd843606`  
		Last Modified: Wed, 04 May 2022 21:18:18 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9279a91eef9f2b4bb4964ed362b6786dc737d38e07cb0266dcbe7441930a27f0`  
		Last Modified: Wed, 04 May 2022 21:18:18 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1ff9295d7bb66afbef49bab61a76a250ae513e6acdd9a8312b8a153c2cae64c`  
		Last Modified: Wed, 04 May 2022 21:18:18 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ce0d33690a32dfd5fb8003a197bdc540ec1d876be17a42ccd82d94634514974`  
		Last Modified: Wed, 04 May 2022 21:18:18 GMT  
		Size: 1.4 KB (1363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-windowsservercore-1809`

```console
$ docker pull nats@sha256:73f511081ca198af5f5c5d1d5d609bf6cfc5a7d43f01e1c93b4b718eaa7bc1d7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2803; amd64

### `nats:2-windowsservercore-1809` - windows version 10.0.17763.2803; amd64

```console
$ docker pull nats@sha256:6ed34062ddcdb57863540c220de7d892b2b3152ae6599e25ff1405defc63d9db
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2721253627 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:392c84a5f744aeb82235810dec31fe58510c59683d8530e1727645ae02a45a8f`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 04 Apr 2022 11:20:25 GMT
RUN Install update 1809-amd64
# Wed, 13 Apr 2022 12:43:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 Apr 2022 14:42:30 GMT
ENV NATS_DOCKERIZED=1
# Wed, 04 May 2022 21:14:48 GMT
ENV NATS_SERVER=2.8.2
# Wed, 04 May 2022 21:14:49 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.8.2/nats-server-v2.8.2-windows-amd64.zip
# Wed, 04 May 2022 21:14:50 GMT
ENV NATS_SERVER_SHASUM=300b9743afa50e02e4e8d43dc212bfde8a871617bd524829114e19ff680dde11
# Wed, 04 May 2022 21:15:50 GMT
RUN Set-PSDebug -Trace 2
# Wed, 04 May 2022 21:17:21 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 04 May 2022 21:17:22 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 04 May 2022 21:17:23 GMT
EXPOSE 4222 6222 8222
# Wed, 04 May 2022 21:17:24 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 04 May 2022 21:17:26 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ba8181afd4264392fbbf8df14fb4cddc55fbe085ab000e986b789678bc2bb171`  
		Size: 997.6 MB (997587446 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7ebb23aa64bff633cfa3c62b190d84f0e870b04fecb1910f65d0870b5c7f8981`  
		Last Modified: Wed, 13 Apr 2022 14:12:24 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d838c7a98a95bee63894bac798124e8c8572bcacc23e22d85332d453a03a7d7c`  
		Last Modified: Wed, 13 Apr 2022 14:46:17 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bba18134d0cef899134f811c0896e8003b4b03b11726200e2d4f09ff3e350d1`  
		Last Modified: Wed, 04 May 2022 21:18:21 GMT  
		Size: 1.4 KB (1382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46e1de2ac2611197cf7e3985577bdf089a2330268d7f08ad53a25b42fcf7548b`  
		Last Modified: Wed, 04 May 2022 21:18:21 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:130538769de262aeb26e810412f9ee58d5b8c1aeb653929a4607901c92363b93`  
		Last Modified: Wed, 04 May 2022 21:18:21 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1684bc7f189afcbdc72f3a0c8eab43e13bbfbe3e8fb412ac51356098cefaeb9a`  
		Last Modified: Wed, 04 May 2022 21:18:21 GMT  
		Size: 359.4 KB (359393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c1c4f2e32fa9a2920cfaeae75fe3b7e64312357d7a20b2c5e7347936eef6dc5`  
		Last Modified: Wed, 04 May 2022 21:18:24 GMT  
		Size: 5.0 MB (4960732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c18367f87433f56d999dc8c84a381afa2e8d480302ea8c78e9169557cd843606`  
		Last Modified: Wed, 04 May 2022 21:18:18 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9279a91eef9f2b4bb4964ed362b6786dc737d38e07cb0266dcbe7441930a27f0`  
		Last Modified: Wed, 04 May 2022 21:18:18 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1ff9295d7bb66afbef49bab61a76a250ae513e6acdd9a8312b8a153c2cae64c`  
		Last Modified: Wed, 04 May 2022 21:18:18 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ce0d33690a32dfd5fb8003a197bdc540ec1d876be17a42ccd82d94634514974`  
		Last Modified: Wed, 04 May 2022 21:18:18 GMT  
		Size: 1.4 KB (1363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.8`

```console
$ docker pull nats@sha256:78f4dc57504675513e5051ce8f64598ddede060ec74a5ff9f253143b7a081503
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.2803; amd64

### `nats:2.8` - linux; amd64

```console
$ docker pull nats@sha256:d7022e467f53812285667fd004413e8cb15920efbb01d1d0f7c4194a2e084959
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4580109 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:71863590dea616f7cf93b753e1e7a3baf16f89747f06004d08f65d3fa907ee9a`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 04 May 2022 21:19:54 GMT
COPY file:1b0e004de765c2bffa3154a8b1990e8a621636f4f1d7ff504c566b8ba440d227 in /nats-server 
# Wed, 04 May 2022 21:19:54 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 04 May 2022 21:19:54 GMT
EXPOSE 4222 6222 8222
# Wed, 04 May 2022 21:19:54 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 04 May 2022 21:19:54 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 04 May 2022 21:19:54 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:cf7d6008a72749fed702f25d8a1bb63636b75bf34655ba074286dc54d0db2b5b`  
		Last Modified: Wed, 04 May 2022 21:20:43 GMT  
		Size: 4.6 MB (4579600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3ef91ad4507cb0bd768e027792377ba07aaaebc8d89981a6ee648d58561273b`  
		Last Modified: Wed, 04 May 2022 21:20:43 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.8` - linux; arm variant v6

```console
$ docker pull nats@sha256:80a268344378d95bf616b13ab6e787e5a242cadbaa9c933e6708bb8761cab22f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4238279 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d53b2041383be620a877c3c265658998b4c5a2f31c6f26d3dd2aa53cb78cf527`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 04 May 2022 22:01:42 GMT
COPY file:ed82059457db34cc43492a36d55b5f9133e36b8d203dcc971bb9feb5fb6a8528 in /nats-server 
# Wed, 04 May 2022 22:01:42 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 04 May 2022 22:01:43 GMT
EXPOSE 4222 6222 8222
# Wed, 04 May 2022 22:01:43 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 04 May 2022 22:01:44 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 04 May 2022 22:01:44 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b04b6f92c475d8e5e8cdec268c94ef3240dde7149afb05913d1099a7ae570a08`  
		Last Modified: Wed, 04 May 2022 22:04:04 GMT  
		Size: 4.2 MB (4237771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef916f73f04fb010ef2bb2bf3b7260ca2d52efb2591d966721af6b5251fd397d`  
		Last Modified: Wed, 04 May 2022 22:04:02 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.8` - linux; arm variant v7

```console
$ docker pull nats@sha256:5faa61f14caf7dc441f38d86641bd5918d1231b40e7acd0336f57843d8ef704b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4232641 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c4caf3fcf0c7865ec8500f33783b2ba88253c0e14828b887cc8b103228346c5`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 04 May 2022 22:18:15 GMT
COPY file:2f9ffa15f39f94a4d8c8c940d7ec0b2baee22852f8f3f2c24a707b69fc8fd84f in /nats-server 
# Wed, 04 May 2022 22:18:15 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 04 May 2022 22:18:16 GMT
EXPOSE 4222 6222 8222
# Wed, 04 May 2022 22:18:16 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 04 May 2022 22:18:17 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 04 May 2022 22:18:17 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:706ff613d28c2f6958458bb4d4ce83f519f2b76bde307418fe1603aac99ac21b`  
		Last Modified: Wed, 04 May 2022 22:20:36 GMT  
		Size: 4.2 MB (4232133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb718277dd458fca567c81e0168c051df2d97f4a8eb0cb348574822d90dec67d`  
		Last Modified: Wed, 04 May 2022 22:20:33 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.8` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:009869128938685fc6fee44029ac90758f29d3fc3e33fa7d5e47a7a3905ef115
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4218329 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a787d12c02030cc31984da44a61d89f3f472271982d215d29866617891286b13`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 04 May 2022 21:48:41 GMT
COPY file:8d0405148efb3d718582f81ff5f54494a8c9789f05e85832ee98d04d228af450 in /nats-server 
# Wed, 04 May 2022 21:48:42 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 04 May 2022 21:48:42 GMT
EXPOSE 4222 6222 8222
# Wed, 04 May 2022 21:48:43 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 04 May 2022 21:48:44 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 04 May 2022 21:48:45 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:8d57fa8f4dba3b0b06e2fd0e4e7b35276d5c1078bcf1be00321d6d56bba9aa78`  
		Last Modified: Wed, 04 May 2022 21:50:01 GMT  
		Size: 4.2 MB (4217820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b388c4e085cdf26d57e7c86c2bec5f6519929e7f9ec591330158ba39d77677b4`  
		Last Modified: Wed, 04 May 2022 21:50:00 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.8` - windows version 10.0.17763.2803; amd64

```console
$ docker pull nats@sha256:2b4914d94facbb6299c5ef2598f655a224c0f671a265bd2986f62c70b978582c
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.7 MB (107725201 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:762896cf7b68aecb4d2820c48789eeee8a8cbc7a58862c4bec5f4ad9d2ecd8f3`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 04 Apr 2022 10:52:49 GMT
RUN Apply image 1809-amd64
# Wed, 13 Apr 2022 14:45:42 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 04 May 2022 21:17:46 GMT
RUN cmd /S /C #(nop) COPY file:1e690007468fe11473f18dc8fbc8b7aa29351e71d03ca73f75d9fcfbf1fd7911 in C:\nats-server.exe 
# Wed, 04 May 2022 21:17:47 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 04 May 2022 21:17:48 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 04 May 2022 21:17:49 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 04 May 2022 21:17:49 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6fc97003d8b7f593fe071cf3ea64f3ce760cc060f3402bb6b1b849c040e222d5`  
		Size: 103.1 MB (103096169 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a6063f744e542c21ce471bdd7ff0dd6063d8d2a9670afbbc64d086813afd6385`  
		Last Modified: Wed, 13 Apr 2022 14:46:35 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c1e5f9285a324194ea2fae24594852b07a0fc1cec1388dcbc367215de23c29e`  
		Last Modified: Wed, 04 May 2022 21:18:39 GMT  
		Size: 4.6 MB (4622651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bde4044fa24dd3365cdc6ba5dff0779813bd4d34e566af1a5c4458c0a232fdc1`  
		Last Modified: Wed, 04 May 2022 21:18:38 GMT  
		Size: 1.8 KB (1791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:405a229a99882e5792c0dad43c80fb315b37c8b9c347f514baccd7d05c6c9f1c`  
		Last Modified: Wed, 04 May 2022 21:18:38 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1037a060f2ca6801837d7d720ec02ed6916e48ce1cfa49e6c7558ba04de8235`  
		Last Modified: Wed, 04 May 2022 21:18:38 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e29f6c2056586ca9353c7019499d854ba31068b682d59304ed4267576ebc5286`  
		Last Modified: Wed, 04 May 2022 21:18:38 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.8-alpine`

```console
$ docker pull nats@sha256:51ed1dcadcd928cbca6b4b2846491bd14667dca111ac63fdb001eef89cb9192f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.8-alpine` - linux; amd64

```console
$ docker pull nats@sha256:3dfa6b8def0d3c784ef7827f0c21b17afd01be56773c68d5950e9f29172ae796
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.7 MB (7667828 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3370f8d5fa5f0ea4cfdcaa60d7f568c2cf9e9752f3a75d11b0d30a257db8a51d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 05 Apr 2022 00:19:59 GMT
ADD file:5d673d25da3a14ce1f6cf66e4c7fd4f4b85a3759a9d93efb3fd9ff852b5b56e4 in / 
# Tue, 05 Apr 2022 00:19:59 GMT
CMD ["/bin/sh"]
# Wed, 04 May 2022 21:19:44 GMT
ENV NATS_SERVER=2.8.2
# Wed, 04 May 2022 21:19:47 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='3409b9dc76c0136cecded67115521d3a815f7a2f3739e81eb87a8d5d761843c3' ;; 		armhf) natsArch='arm6'; sha256='a3d474a583ca90e3577aa470335c582d4565918f500ebd28d760643fb631d8d5' ;; 		armv7) natsArch='arm7'; sha256='88fd437f7def8dbe68b17dce703c919771e64b570856bf0e6f2eb3b9459031c6' ;; 		x86_64) natsArch='amd64'; sha256='59805a464237801574ca7efdc69ebc21040e9b811fb53ed444c4808a05440719' ;; 		x86) natsArch='386'; sha256='facd3c69ee27c3e9e8654e5de95eb79de2e873bf4c066317aa9fad5c2ea26b92' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 04 May 2022 21:19:47 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 04 May 2022 21:19:47 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 04 May 2022 21:19:47 GMT
EXPOSE 4222 6222 8222
# Wed, 04 May 2022 21:19:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 04 May 2022 21:19:47 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:df9b9388f04ad6279a7410b85cedfdcb2208c0a003da7ab5613af71079148139`  
		Last Modified: Mon, 04 Apr 2022 19:10:16 GMT  
		Size: 2.8 MB (2814559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb157527e1f2e860f2700cadfdf0bed3ac0d50b8a177dd0b906431b0d46b44b5`  
		Last Modified: Wed, 04 May 2022 21:20:20 GMT  
		Size: 4.9 MB (4852271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c29bade32b2ef2ecc8325cbc5cbbf69470e5e20cc04e292244e704f68b9a6f86`  
		Last Modified: Wed, 04 May 2022 21:20:19 GMT  
		Size: 585.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dbec41bc3a042cdbf4c2e9b57c99bf99a4552e64a437be0066d42a04e3de650`  
		Last Modified: Wed, 04 May 2022 21:20:19 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.8-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:12b766cef3be0b9dc70e35a9cefcecbfad16a19e00b94a4737134ebbee24ea31
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7133599 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d1cc5ce43b7fd2c1dc34d986696c64da1a158fc067f5a4710ce475ce2f10eaec`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 04 Apr 2022 23:49:42 GMT
ADD file:159dcddaab900372df882a4e94615ed84250e9cea3e74bc0479d98280342f596 in / 
# Mon, 04 Apr 2022 23:49:42 GMT
CMD ["/bin/sh"]
# Wed, 04 May 2022 22:01:15 GMT
ENV NATS_SERVER=2.8.2
# Wed, 04 May 2022 22:01:19 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='3409b9dc76c0136cecded67115521d3a815f7a2f3739e81eb87a8d5d761843c3' ;; 		armhf) natsArch='arm6'; sha256='a3d474a583ca90e3577aa470335c582d4565918f500ebd28d760643fb631d8d5' ;; 		armv7) natsArch='arm7'; sha256='88fd437f7def8dbe68b17dce703c919771e64b570856bf0e6f2eb3b9459031c6' ;; 		x86_64) natsArch='amd64'; sha256='59805a464237801574ca7efdc69ebc21040e9b811fb53ed444c4808a05440719' ;; 		x86) natsArch='386'; sha256='facd3c69ee27c3e9e8654e5de95eb79de2e873bf4c066317aa9fad5c2ea26b92' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 04 May 2022 22:01:20 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 04 May 2022 22:01:20 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 04 May 2022 22:01:21 GMT
EXPOSE 4222 6222 8222
# Wed, 04 May 2022 22:01:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 04 May 2022 22:01:21 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:c319b1fc4ed70b8241a7ce6ac0c4015d354bf5cf8c01eb73c50b6709c0c46e49`  
		Last Modified: Mon, 04 Apr 2022 19:09:22 GMT  
		Size: 2.6 MB (2621972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3508da0a7a8c69badd89084de30d788f3c0bc57d625677ec7d68c32f18d466ba`  
		Last Modified: Wed, 04 May 2022 22:03:28 GMT  
		Size: 4.5 MB (4510625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7965b001731ee55e0b7b2c11c7ff5f851afaed57dba5ef2a08324fab5de994f7`  
		Last Modified: Wed, 04 May 2022 22:03:27 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8d031fa4afb68088db4a684f2332c5c8c3ecedb55d2aee461d64c8556afb468`  
		Last Modified: Wed, 04 May 2022 22:03:25 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.8-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:7d6c71099975b1e928511819a05612d582d412c5ed2838f04882514d0e77fff8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.9 MB (6930001 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3813055a26f58efed9d97ad053203ba493589fa6e486f3dd5810354defc6b3c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 04 Apr 2022 23:57:34 GMT
ADD file:20f8cdddc53a4a8bd78945fc32fe08e9f80ab3b16dc20a9aa4ba73b79f2bc71c in / 
# Mon, 04 Apr 2022 23:57:35 GMT
CMD ["/bin/sh"]
# Wed, 04 May 2022 22:17:46 GMT
ENV NATS_SERVER=2.8.2
# Wed, 04 May 2022 22:17:50 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='3409b9dc76c0136cecded67115521d3a815f7a2f3739e81eb87a8d5d761843c3' ;; 		armhf) natsArch='arm6'; sha256='a3d474a583ca90e3577aa470335c582d4565918f500ebd28d760643fb631d8d5' ;; 		armv7) natsArch='arm7'; sha256='88fd437f7def8dbe68b17dce703c919771e64b570856bf0e6f2eb3b9459031c6' ;; 		x86_64) natsArch='amd64'; sha256='59805a464237801574ca7efdc69ebc21040e9b811fb53ed444c4808a05440719' ;; 		x86) natsArch='386'; sha256='facd3c69ee27c3e9e8654e5de95eb79de2e873bf4c066317aa9fad5c2ea26b92' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 04 May 2022 22:17:50 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 04 May 2022 22:17:51 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 04 May 2022 22:17:51 GMT
EXPOSE 4222 6222 8222
# Wed, 04 May 2022 22:17:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 04 May 2022 22:17:52 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:57fb4b5f1a47c953ca5703f0f81ce14e5d01cf23aa79558b5adb961cc526e320`  
		Last Modified: Mon, 04 Apr 2022 19:09:36 GMT  
		Size: 2.4 MB (2424323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b49f3de3c7329a4a2fbd9e8c9cd595a837860930995c5a11d2459e045b8d2dab`  
		Last Modified: Wed, 04 May 2022 22:20:00 GMT  
		Size: 4.5 MB (4504680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51dc12ec06d594c70e53bb45c9912d27ad4869faf092615047ea9faab11d6ccb`  
		Last Modified: Wed, 04 May 2022 22:19:57 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5e0c0af17ebf42f5af072c2b71c091af0b659ac5e20a80c92ca74da9ec5353d`  
		Last Modified: Wed, 04 May 2022 22:19:57 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.8-alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:81e20b06f2b5aac1ca438142975de9c05234b243fcb497ab8afd7f0bcd4a28a8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7208259 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12c2a5e86ad6fc84ed6f66fecfc26474466d0f61712b85aa012fc0b7e726019e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:31 GMT
ADD file:90e56af13188c7f0283d244a0d70b853d8bef8587a41f1da8eac3a2aba8964ef in / 
# Mon, 04 Apr 2022 23:39:31 GMT
CMD ["/bin/sh"]
# Wed, 04 May 2022 21:48:24 GMT
ENV NATS_SERVER=2.8.2
# Wed, 04 May 2022 21:48:26 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='3409b9dc76c0136cecded67115521d3a815f7a2f3739e81eb87a8d5d761843c3' ;; 		armhf) natsArch='arm6'; sha256='a3d474a583ca90e3577aa470335c582d4565918f500ebd28d760643fb631d8d5' ;; 		armv7) natsArch='arm7'; sha256='88fd437f7def8dbe68b17dce703c919771e64b570856bf0e6f2eb3b9459031c6' ;; 		x86_64) natsArch='amd64'; sha256='59805a464237801574ca7efdc69ebc21040e9b811fb53ed444c4808a05440719' ;; 		x86) natsArch='386'; sha256='facd3c69ee27c3e9e8654e5de95eb79de2e873bf4c066317aa9fad5c2ea26b92' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 04 May 2022 21:48:28 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 04 May 2022 21:48:29 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 04 May 2022 21:48:29 GMT
EXPOSE 4222 6222 8222
# Wed, 04 May 2022 21:48:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 04 May 2022 21:48:31 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9981e73032c8833e387a8f96986e560edbed12c38119e0edb0439c9c2234eac9`  
		Last Modified: Mon, 04 Apr 2022 19:09:10 GMT  
		Size: 2.7 MB (2716477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec7ea9151b15b8e90d2a0ef58393de32cefb12a7f7c7e3d7a011808b38e59565`  
		Last Modified: Wed, 04 May 2022 21:49:31 GMT  
		Size: 4.5 MB (4490808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f800447a181fc7e3f37c2e68d8374347459e1d12a8d8c8653b7da45180ae97f`  
		Last Modified: Wed, 04 May 2022 21:49:30 GMT  
		Size: 560.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:894f3b307d2ae2b261df9d763e886b3ae75f9aba6dc927eaf3f28cae9375c050`  
		Last Modified: Wed, 04 May 2022 21:49:30 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.8-alpine3.15`

```console
$ docker pull nats@sha256:51ed1dcadcd928cbca6b4b2846491bd14667dca111ac63fdb001eef89cb9192f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.8-alpine3.15` - linux; amd64

```console
$ docker pull nats@sha256:3dfa6b8def0d3c784ef7827f0c21b17afd01be56773c68d5950e9f29172ae796
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.7 MB (7667828 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3370f8d5fa5f0ea4cfdcaa60d7f568c2cf9e9752f3a75d11b0d30a257db8a51d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 05 Apr 2022 00:19:59 GMT
ADD file:5d673d25da3a14ce1f6cf66e4c7fd4f4b85a3759a9d93efb3fd9ff852b5b56e4 in / 
# Tue, 05 Apr 2022 00:19:59 GMT
CMD ["/bin/sh"]
# Wed, 04 May 2022 21:19:44 GMT
ENV NATS_SERVER=2.8.2
# Wed, 04 May 2022 21:19:47 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='3409b9dc76c0136cecded67115521d3a815f7a2f3739e81eb87a8d5d761843c3' ;; 		armhf) natsArch='arm6'; sha256='a3d474a583ca90e3577aa470335c582d4565918f500ebd28d760643fb631d8d5' ;; 		armv7) natsArch='arm7'; sha256='88fd437f7def8dbe68b17dce703c919771e64b570856bf0e6f2eb3b9459031c6' ;; 		x86_64) natsArch='amd64'; sha256='59805a464237801574ca7efdc69ebc21040e9b811fb53ed444c4808a05440719' ;; 		x86) natsArch='386'; sha256='facd3c69ee27c3e9e8654e5de95eb79de2e873bf4c066317aa9fad5c2ea26b92' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 04 May 2022 21:19:47 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 04 May 2022 21:19:47 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 04 May 2022 21:19:47 GMT
EXPOSE 4222 6222 8222
# Wed, 04 May 2022 21:19:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 04 May 2022 21:19:47 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:df9b9388f04ad6279a7410b85cedfdcb2208c0a003da7ab5613af71079148139`  
		Last Modified: Mon, 04 Apr 2022 19:10:16 GMT  
		Size: 2.8 MB (2814559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb157527e1f2e860f2700cadfdf0bed3ac0d50b8a177dd0b906431b0d46b44b5`  
		Last Modified: Wed, 04 May 2022 21:20:20 GMT  
		Size: 4.9 MB (4852271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c29bade32b2ef2ecc8325cbc5cbbf69470e5e20cc04e292244e704f68b9a6f86`  
		Last Modified: Wed, 04 May 2022 21:20:19 GMT  
		Size: 585.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dbec41bc3a042cdbf4c2e9b57c99bf99a4552e64a437be0066d42a04e3de650`  
		Last Modified: Wed, 04 May 2022 21:20:19 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.8-alpine3.15` - linux; arm variant v6

```console
$ docker pull nats@sha256:12b766cef3be0b9dc70e35a9cefcecbfad16a19e00b94a4737134ebbee24ea31
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7133599 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d1cc5ce43b7fd2c1dc34d986696c64da1a158fc067f5a4710ce475ce2f10eaec`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 04 Apr 2022 23:49:42 GMT
ADD file:159dcddaab900372df882a4e94615ed84250e9cea3e74bc0479d98280342f596 in / 
# Mon, 04 Apr 2022 23:49:42 GMT
CMD ["/bin/sh"]
# Wed, 04 May 2022 22:01:15 GMT
ENV NATS_SERVER=2.8.2
# Wed, 04 May 2022 22:01:19 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='3409b9dc76c0136cecded67115521d3a815f7a2f3739e81eb87a8d5d761843c3' ;; 		armhf) natsArch='arm6'; sha256='a3d474a583ca90e3577aa470335c582d4565918f500ebd28d760643fb631d8d5' ;; 		armv7) natsArch='arm7'; sha256='88fd437f7def8dbe68b17dce703c919771e64b570856bf0e6f2eb3b9459031c6' ;; 		x86_64) natsArch='amd64'; sha256='59805a464237801574ca7efdc69ebc21040e9b811fb53ed444c4808a05440719' ;; 		x86) natsArch='386'; sha256='facd3c69ee27c3e9e8654e5de95eb79de2e873bf4c066317aa9fad5c2ea26b92' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 04 May 2022 22:01:20 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 04 May 2022 22:01:20 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 04 May 2022 22:01:21 GMT
EXPOSE 4222 6222 8222
# Wed, 04 May 2022 22:01:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 04 May 2022 22:01:21 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:c319b1fc4ed70b8241a7ce6ac0c4015d354bf5cf8c01eb73c50b6709c0c46e49`  
		Last Modified: Mon, 04 Apr 2022 19:09:22 GMT  
		Size: 2.6 MB (2621972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3508da0a7a8c69badd89084de30d788f3c0bc57d625677ec7d68c32f18d466ba`  
		Last Modified: Wed, 04 May 2022 22:03:28 GMT  
		Size: 4.5 MB (4510625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7965b001731ee55e0b7b2c11c7ff5f851afaed57dba5ef2a08324fab5de994f7`  
		Last Modified: Wed, 04 May 2022 22:03:27 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8d031fa4afb68088db4a684f2332c5c8c3ecedb55d2aee461d64c8556afb468`  
		Last Modified: Wed, 04 May 2022 22:03:25 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.8-alpine3.15` - linux; arm variant v7

```console
$ docker pull nats@sha256:7d6c71099975b1e928511819a05612d582d412c5ed2838f04882514d0e77fff8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.9 MB (6930001 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3813055a26f58efed9d97ad053203ba493589fa6e486f3dd5810354defc6b3c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 04 Apr 2022 23:57:34 GMT
ADD file:20f8cdddc53a4a8bd78945fc32fe08e9f80ab3b16dc20a9aa4ba73b79f2bc71c in / 
# Mon, 04 Apr 2022 23:57:35 GMT
CMD ["/bin/sh"]
# Wed, 04 May 2022 22:17:46 GMT
ENV NATS_SERVER=2.8.2
# Wed, 04 May 2022 22:17:50 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='3409b9dc76c0136cecded67115521d3a815f7a2f3739e81eb87a8d5d761843c3' ;; 		armhf) natsArch='arm6'; sha256='a3d474a583ca90e3577aa470335c582d4565918f500ebd28d760643fb631d8d5' ;; 		armv7) natsArch='arm7'; sha256='88fd437f7def8dbe68b17dce703c919771e64b570856bf0e6f2eb3b9459031c6' ;; 		x86_64) natsArch='amd64'; sha256='59805a464237801574ca7efdc69ebc21040e9b811fb53ed444c4808a05440719' ;; 		x86) natsArch='386'; sha256='facd3c69ee27c3e9e8654e5de95eb79de2e873bf4c066317aa9fad5c2ea26b92' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 04 May 2022 22:17:50 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 04 May 2022 22:17:51 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 04 May 2022 22:17:51 GMT
EXPOSE 4222 6222 8222
# Wed, 04 May 2022 22:17:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 04 May 2022 22:17:52 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:57fb4b5f1a47c953ca5703f0f81ce14e5d01cf23aa79558b5adb961cc526e320`  
		Last Modified: Mon, 04 Apr 2022 19:09:36 GMT  
		Size: 2.4 MB (2424323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b49f3de3c7329a4a2fbd9e8c9cd595a837860930995c5a11d2459e045b8d2dab`  
		Last Modified: Wed, 04 May 2022 22:20:00 GMT  
		Size: 4.5 MB (4504680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51dc12ec06d594c70e53bb45c9912d27ad4869faf092615047ea9faab11d6ccb`  
		Last Modified: Wed, 04 May 2022 22:19:57 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5e0c0af17ebf42f5af072c2b71c091af0b659ac5e20a80c92ca74da9ec5353d`  
		Last Modified: Wed, 04 May 2022 22:19:57 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.8-alpine3.15` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:81e20b06f2b5aac1ca438142975de9c05234b243fcb497ab8afd7f0bcd4a28a8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7208259 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12c2a5e86ad6fc84ed6f66fecfc26474466d0f61712b85aa012fc0b7e726019e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:31 GMT
ADD file:90e56af13188c7f0283d244a0d70b853d8bef8587a41f1da8eac3a2aba8964ef in / 
# Mon, 04 Apr 2022 23:39:31 GMT
CMD ["/bin/sh"]
# Wed, 04 May 2022 21:48:24 GMT
ENV NATS_SERVER=2.8.2
# Wed, 04 May 2022 21:48:26 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='3409b9dc76c0136cecded67115521d3a815f7a2f3739e81eb87a8d5d761843c3' ;; 		armhf) natsArch='arm6'; sha256='a3d474a583ca90e3577aa470335c582d4565918f500ebd28d760643fb631d8d5' ;; 		armv7) natsArch='arm7'; sha256='88fd437f7def8dbe68b17dce703c919771e64b570856bf0e6f2eb3b9459031c6' ;; 		x86_64) natsArch='amd64'; sha256='59805a464237801574ca7efdc69ebc21040e9b811fb53ed444c4808a05440719' ;; 		x86) natsArch='386'; sha256='facd3c69ee27c3e9e8654e5de95eb79de2e873bf4c066317aa9fad5c2ea26b92' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 04 May 2022 21:48:28 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 04 May 2022 21:48:29 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 04 May 2022 21:48:29 GMT
EXPOSE 4222 6222 8222
# Wed, 04 May 2022 21:48:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 04 May 2022 21:48:31 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9981e73032c8833e387a8f96986e560edbed12c38119e0edb0439c9c2234eac9`  
		Last Modified: Mon, 04 Apr 2022 19:09:10 GMT  
		Size: 2.7 MB (2716477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec7ea9151b15b8e90d2a0ef58393de32cefb12a7f7c7e3d7a011808b38e59565`  
		Last Modified: Wed, 04 May 2022 21:49:31 GMT  
		Size: 4.5 MB (4490808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f800447a181fc7e3f37c2e68d8374347459e1d12a8d8c8653b7da45180ae97f`  
		Last Modified: Wed, 04 May 2022 21:49:30 GMT  
		Size: 560.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:894f3b307d2ae2b261df9d763e886b3ae75f9aba6dc927eaf3f28cae9375c050`  
		Last Modified: Wed, 04 May 2022 21:49:30 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.8-linux`

```console
$ docker pull nats@sha256:dd400785e2c069158ca6a488873976cab93098904db7fcc044cfc6af0327640c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.8-linux` - linux; amd64

```console
$ docker pull nats@sha256:d7022e467f53812285667fd004413e8cb15920efbb01d1d0f7c4194a2e084959
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4580109 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:71863590dea616f7cf93b753e1e7a3baf16f89747f06004d08f65d3fa907ee9a`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 04 May 2022 21:19:54 GMT
COPY file:1b0e004de765c2bffa3154a8b1990e8a621636f4f1d7ff504c566b8ba440d227 in /nats-server 
# Wed, 04 May 2022 21:19:54 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 04 May 2022 21:19:54 GMT
EXPOSE 4222 6222 8222
# Wed, 04 May 2022 21:19:54 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 04 May 2022 21:19:54 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 04 May 2022 21:19:54 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:cf7d6008a72749fed702f25d8a1bb63636b75bf34655ba074286dc54d0db2b5b`  
		Last Modified: Wed, 04 May 2022 21:20:43 GMT  
		Size: 4.6 MB (4579600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3ef91ad4507cb0bd768e027792377ba07aaaebc8d89981a6ee648d58561273b`  
		Last Modified: Wed, 04 May 2022 21:20:43 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.8-linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:80a268344378d95bf616b13ab6e787e5a242cadbaa9c933e6708bb8761cab22f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4238279 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d53b2041383be620a877c3c265658998b4c5a2f31c6f26d3dd2aa53cb78cf527`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 04 May 2022 22:01:42 GMT
COPY file:ed82059457db34cc43492a36d55b5f9133e36b8d203dcc971bb9feb5fb6a8528 in /nats-server 
# Wed, 04 May 2022 22:01:42 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 04 May 2022 22:01:43 GMT
EXPOSE 4222 6222 8222
# Wed, 04 May 2022 22:01:43 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 04 May 2022 22:01:44 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 04 May 2022 22:01:44 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b04b6f92c475d8e5e8cdec268c94ef3240dde7149afb05913d1099a7ae570a08`  
		Last Modified: Wed, 04 May 2022 22:04:04 GMT  
		Size: 4.2 MB (4237771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef916f73f04fb010ef2bb2bf3b7260ca2d52efb2591d966721af6b5251fd397d`  
		Last Modified: Wed, 04 May 2022 22:04:02 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.8-linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:5faa61f14caf7dc441f38d86641bd5918d1231b40e7acd0336f57843d8ef704b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4232641 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c4caf3fcf0c7865ec8500f33783b2ba88253c0e14828b887cc8b103228346c5`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 04 May 2022 22:18:15 GMT
COPY file:2f9ffa15f39f94a4d8c8c940d7ec0b2baee22852f8f3f2c24a707b69fc8fd84f in /nats-server 
# Wed, 04 May 2022 22:18:15 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 04 May 2022 22:18:16 GMT
EXPOSE 4222 6222 8222
# Wed, 04 May 2022 22:18:16 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 04 May 2022 22:18:17 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 04 May 2022 22:18:17 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:706ff613d28c2f6958458bb4d4ce83f519f2b76bde307418fe1603aac99ac21b`  
		Last Modified: Wed, 04 May 2022 22:20:36 GMT  
		Size: 4.2 MB (4232133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb718277dd458fca567c81e0168c051df2d97f4a8eb0cb348574822d90dec67d`  
		Last Modified: Wed, 04 May 2022 22:20:33 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.8-linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:009869128938685fc6fee44029ac90758f29d3fc3e33fa7d5e47a7a3905ef115
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4218329 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a787d12c02030cc31984da44a61d89f3f472271982d215d29866617891286b13`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 04 May 2022 21:48:41 GMT
COPY file:8d0405148efb3d718582f81ff5f54494a8c9789f05e85832ee98d04d228af450 in /nats-server 
# Wed, 04 May 2022 21:48:42 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 04 May 2022 21:48:42 GMT
EXPOSE 4222 6222 8222
# Wed, 04 May 2022 21:48:43 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 04 May 2022 21:48:44 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 04 May 2022 21:48:45 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:8d57fa8f4dba3b0b06e2fd0e4e7b35276d5c1078bcf1be00321d6d56bba9aa78`  
		Last Modified: Wed, 04 May 2022 21:50:01 GMT  
		Size: 4.2 MB (4217820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b388c4e085cdf26d57e7c86c2bec5f6519929e7f9ec591330158ba39d77677b4`  
		Last Modified: Wed, 04 May 2022 21:50:00 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.8-nanoserver`

```console
$ docker pull nats@sha256:f128bdd66f848762f7bb7c580b2d89e4c329ce85461597353dcbff405ddda643
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2803; amd64

### `nats:2.8-nanoserver` - windows version 10.0.17763.2803; amd64

```console
$ docker pull nats@sha256:2b4914d94facbb6299c5ef2598f655a224c0f671a265bd2986f62c70b978582c
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.7 MB (107725201 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:762896cf7b68aecb4d2820c48789eeee8a8cbc7a58862c4bec5f4ad9d2ecd8f3`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 04 Apr 2022 10:52:49 GMT
RUN Apply image 1809-amd64
# Wed, 13 Apr 2022 14:45:42 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 04 May 2022 21:17:46 GMT
RUN cmd /S /C #(nop) COPY file:1e690007468fe11473f18dc8fbc8b7aa29351e71d03ca73f75d9fcfbf1fd7911 in C:\nats-server.exe 
# Wed, 04 May 2022 21:17:47 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 04 May 2022 21:17:48 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 04 May 2022 21:17:49 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 04 May 2022 21:17:49 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6fc97003d8b7f593fe071cf3ea64f3ce760cc060f3402bb6b1b849c040e222d5`  
		Size: 103.1 MB (103096169 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a6063f744e542c21ce471bdd7ff0dd6063d8d2a9670afbbc64d086813afd6385`  
		Last Modified: Wed, 13 Apr 2022 14:46:35 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c1e5f9285a324194ea2fae24594852b07a0fc1cec1388dcbc367215de23c29e`  
		Last Modified: Wed, 04 May 2022 21:18:39 GMT  
		Size: 4.6 MB (4622651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bde4044fa24dd3365cdc6ba5dff0779813bd4d34e566af1a5c4458c0a232fdc1`  
		Last Modified: Wed, 04 May 2022 21:18:38 GMT  
		Size: 1.8 KB (1791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:405a229a99882e5792c0dad43c80fb315b37c8b9c347f514baccd7d05c6c9f1c`  
		Last Modified: Wed, 04 May 2022 21:18:38 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1037a060f2ca6801837d7d720ec02ed6916e48ce1cfa49e6c7558ba04de8235`  
		Last Modified: Wed, 04 May 2022 21:18:38 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e29f6c2056586ca9353c7019499d854ba31068b682d59304ed4267576ebc5286`  
		Last Modified: Wed, 04 May 2022 21:18:38 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.8-nanoserver-1809`

```console
$ docker pull nats@sha256:f128bdd66f848762f7bb7c580b2d89e4c329ce85461597353dcbff405ddda643
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2803; amd64

### `nats:2.8-nanoserver-1809` - windows version 10.0.17763.2803; amd64

```console
$ docker pull nats@sha256:2b4914d94facbb6299c5ef2598f655a224c0f671a265bd2986f62c70b978582c
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.7 MB (107725201 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:762896cf7b68aecb4d2820c48789eeee8a8cbc7a58862c4bec5f4ad9d2ecd8f3`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 04 Apr 2022 10:52:49 GMT
RUN Apply image 1809-amd64
# Wed, 13 Apr 2022 14:45:42 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 04 May 2022 21:17:46 GMT
RUN cmd /S /C #(nop) COPY file:1e690007468fe11473f18dc8fbc8b7aa29351e71d03ca73f75d9fcfbf1fd7911 in C:\nats-server.exe 
# Wed, 04 May 2022 21:17:47 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 04 May 2022 21:17:48 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 04 May 2022 21:17:49 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 04 May 2022 21:17:49 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6fc97003d8b7f593fe071cf3ea64f3ce760cc060f3402bb6b1b849c040e222d5`  
		Size: 103.1 MB (103096169 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a6063f744e542c21ce471bdd7ff0dd6063d8d2a9670afbbc64d086813afd6385`  
		Last Modified: Wed, 13 Apr 2022 14:46:35 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c1e5f9285a324194ea2fae24594852b07a0fc1cec1388dcbc367215de23c29e`  
		Last Modified: Wed, 04 May 2022 21:18:39 GMT  
		Size: 4.6 MB (4622651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bde4044fa24dd3365cdc6ba5dff0779813bd4d34e566af1a5c4458c0a232fdc1`  
		Last Modified: Wed, 04 May 2022 21:18:38 GMT  
		Size: 1.8 KB (1791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:405a229a99882e5792c0dad43c80fb315b37c8b9c347f514baccd7d05c6c9f1c`  
		Last Modified: Wed, 04 May 2022 21:18:38 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1037a060f2ca6801837d7d720ec02ed6916e48ce1cfa49e6c7558ba04de8235`  
		Last Modified: Wed, 04 May 2022 21:18:38 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e29f6c2056586ca9353c7019499d854ba31068b682d59304ed4267576ebc5286`  
		Last Modified: Wed, 04 May 2022 21:18:38 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.8-scratch`

```console
$ docker pull nats@sha256:dd400785e2c069158ca6a488873976cab93098904db7fcc044cfc6af0327640c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.8-scratch` - linux; amd64

```console
$ docker pull nats@sha256:d7022e467f53812285667fd004413e8cb15920efbb01d1d0f7c4194a2e084959
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4580109 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:71863590dea616f7cf93b753e1e7a3baf16f89747f06004d08f65d3fa907ee9a`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 04 May 2022 21:19:54 GMT
COPY file:1b0e004de765c2bffa3154a8b1990e8a621636f4f1d7ff504c566b8ba440d227 in /nats-server 
# Wed, 04 May 2022 21:19:54 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 04 May 2022 21:19:54 GMT
EXPOSE 4222 6222 8222
# Wed, 04 May 2022 21:19:54 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 04 May 2022 21:19:54 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 04 May 2022 21:19:54 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:cf7d6008a72749fed702f25d8a1bb63636b75bf34655ba074286dc54d0db2b5b`  
		Last Modified: Wed, 04 May 2022 21:20:43 GMT  
		Size: 4.6 MB (4579600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3ef91ad4507cb0bd768e027792377ba07aaaebc8d89981a6ee648d58561273b`  
		Last Modified: Wed, 04 May 2022 21:20:43 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.8-scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:80a268344378d95bf616b13ab6e787e5a242cadbaa9c933e6708bb8761cab22f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4238279 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d53b2041383be620a877c3c265658998b4c5a2f31c6f26d3dd2aa53cb78cf527`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 04 May 2022 22:01:42 GMT
COPY file:ed82059457db34cc43492a36d55b5f9133e36b8d203dcc971bb9feb5fb6a8528 in /nats-server 
# Wed, 04 May 2022 22:01:42 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 04 May 2022 22:01:43 GMT
EXPOSE 4222 6222 8222
# Wed, 04 May 2022 22:01:43 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 04 May 2022 22:01:44 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 04 May 2022 22:01:44 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b04b6f92c475d8e5e8cdec268c94ef3240dde7149afb05913d1099a7ae570a08`  
		Last Modified: Wed, 04 May 2022 22:04:04 GMT  
		Size: 4.2 MB (4237771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef916f73f04fb010ef2bb2bf3b7260ca2d52efb2591d966721af6b5251fd397d`  
		Last Modified: Wed, 04 May 2022 22:04:02 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.8-scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:5faa61f14caf7dc441f38d86641bd5918d1231b40e7acd0336f57843d8ef704b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4232641 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c4caf3fcf0c7865ec8500f33783b2ba88253c0e14828b887cc8b103228346c5`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 04 May 2022 22:18:15 GMT
COPY file:2f9ffa15f39f94a4d8c8c940d7ec0b2baee22852f8f3f2c24a707b69fc8fd84f in /nats-server 
# Wed, 04 May 2022 22:18:15 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 04 May 2022 22:18:16 GMT
EXPOSE 4222 6222 8222
# Wed, 04 May 2022 22:18:16 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 04 May 2022 22:18:17 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 04 May 2022 22:18:17 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:706ff613d28c2f6958458bb4d4ce83f519f2b76bde307418fe1603aac99ac21b`  
		Last Modified: Wed, 04 May 2022 22:20:36 GMT  
		Size: 4.2 MB (4232133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb718277dd458fca567c81e0168c051df2d97f4a8eb0cb348574822d90dec67d`  
		Last Modified: Wed, 04 May 2022 22:20:33 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.8-scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:009869128938685fc6fee44029ac90758f29d3fc3e33fa7d5e47a7a3905ef115
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4218329 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a787d12c02030cc31984da44a61d89f3f472271982d215d29866617891286b13`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 04 May 2022 21:48:41 GMT
COPY file:8d0405148efb3d718582f81ff5f54494a8c9789f05e85832ee98d04d228af450 in /nats-server 
# Wed, 04 May 2022 21:48:42 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 04 May 2022 21:48:42 GMT
EXPOSE 4222 6222 8222
# Wed, 04 May 2022 21:48:43 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 04 May 2022 21:48:44 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 04 May 2022 21:48:45 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:8d57fa8f4dba3b0b06e2fd0e4e7b35276d5c1078bcf1be00321d6d56bba9aa78`  
		Last Modified: Wed, 04 May 2022 21:50:01 GMT  
		Size: 4.2 MB (4217820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b388c4e085cdf26d57e7c86c2bec5f6519929e7f9ec591330158ba39d77677b4`  
		Last Modified: Wed, 04 May 2022 21:50:00 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.8-windowsservercore`

```console
$ docker pull nats@sha256:73f511081ca198af5f5c5d1d5d609bf6cfc5a7d43f01e1c93b4b718eaa7bc1d7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2803; amd64

### `nats:2.8-windowsservercore` - windows version 10.0.17763.2803; amd64

```console
$ docker pull nats@sha256:6ed34062ddcdb57863540c220de7d892b2b3152ae6599e25ff1405defc63d9db
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2721253627 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:392c84a5f744aeb82235810dec31fe58510c59683d8530e1727645ae02a45a8f`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 04 Apr 2022 11:20:25 GMT
RUN Install update 1809-amd64
# Wed, 13 Apr 2022 12:43:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 Apr 2022 14:42:30 GMT
ENV NATS_DOCKERIZED=1
# Wed, 04 May 2022 21:14:48 GMT
ENV NATS_SERVER=2.8.2
# Wed, 04 May 2022 21:14:49 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.8.2/nats-server-v2.8.2-windows-amd64.zip
# Wed, 04 May 2022 21:14:50 GMT
ENV NATS_SERVER_SHASUM=300b9743afa50e02e4e8d43dc212bfde8a871617bd524829114e19ff680dde11
# Wed, 04 May 2022 21:15:50 GMT
RUN Set-PSDebug -Trace 2
# Wed, 04 May 2022 21:17:21 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 04 May 2022 21:17:22 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 04 May 2022 21:17:23 GMT
EXPOSE 4222 6222 8222
# Wed, 04 May 2022 21:17:24 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 04 May 2022 21:17:26 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ba8181afd4264392fbbf8df14fb4cddc55fbe085ab000e986b789678bc2bb171`  
		Size: 997.6 MB (997587446 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7ebb23aa64bff633cfa3c62b190d84f0e870b04fecb1910f65d0870b5c7f8981`  
		Last Modified: Wed, 13 Apr 2022 14:12:24 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d838c7a98a95bee63894bac798124e8c8572bcacc23e22d85332d453a03a7d7c`  
		Last Modified: Wed, 13 Apr 2022 14:46:17 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bba18134d0cef899134f811c0896e8003b4b03b11726200e2d4f09ff3e350d1`  
		Last Modified: Wed, 04 May 2022 21:18:21 GMT  
		Size: 1.4 KB (1382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46e1de2ac2611197cf7e3985577bdf089a2330268d7f08ad53a25b42fcf7548b`  
		Last Modified: Wed, 04 May 2022 21:18:21 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:130538769de262aeb26e810412f9ee58d5b8c1aeb653929a4607901c92363b93`  
		Last Modified: Wed, 04 May 2022 21:18:21 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1684bc7f189afcbdc72f3a0c8eab43e13bbfbe3e8fb412ac51356098cefaeb9a`  
		Last Modified: Wed, 04 May 2022 21:18:21 GMT  
		Size: 359.4 KB (359393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c1c4f2e32fa9a2920cfaeae75fe3b7e64312357d7a20b2c5e7347936eef6dc5`  
		Last Modified: Wed, 04 May 2022 21:18:24 GMT  
		Size: 5.0 MB (4960732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c18367f87433f56d999dc8c84a381afa2e8d480302ea8c78e9169557cd843606`  
		Last Modified: Wed, 04 May 2022 21:18:18 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9279a91eef9f2b4bb4964ed362b6786dc737d38e07cb0266dcbe7441930a27f0`  
		Last Modified: Wed, 04 May 2022 21:18:18 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1ff9295d7bb66afbef49bab61a76a250ae513e6acdd9a8312b8a153c2cae64c`  
		Last Modified: Wed, 04 May 2022 21:18:18 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ce0d33690a32dfd5fb8003a197bdc540ec1d876be17a42ccd82d94634514974`  
		Last Modified: Wed, 04 May 2022 21:18:18 GMT  
		Size: 1.4 KB (1363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.8-windowsservercore-1809`

```console
$ docker pull nats@sha256:73f511081ca198af5f5c5d1d5d609bf6cfc5a7d43f01e1c93b4b718eaa7bc1d7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2803; amd64

### `nats:2.8-windowsservercore-1809` - windows version 10.0.17763.2803; amd64

```console
$ docker pull nats@sha256:6ed34062ddcdb57863540c220de7d892b2b3152ae6599e25ff1405defc63d9db
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2721253627 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:392c84a5f744aeb82235810dec31fe58510c59683d8530e1727645ae02a45a8f`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 04 Apr 2022 11:20:25 GMT
RUN Install update 1809-amd64
# Wed, 13 Apr 2022 12:43:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 Apr 2022 14:42:30 GMT
ENV NATS_DOCKERIZED=1
# Wed, 04 May 2022 21:14:48 GMT
ENV NATS_SERVER=2.8.2
# Wed, 04 May 2022 21:14:49 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.8.2/nats-server-v2.8.2-windows-amd64.zip
# Wed, 04 May 2022 21:14:50 GMT
ENV NATS_SERVER_SHASUM=300b9743afa50e02e4e8d43dc212bfde8a871617bd524829114e19ff680dde11
# Wed, 04 May 2022 21:15:50 GMT
RUN Set-PSDebug -Trace 2
# Wed, 04 May 2022 21:17:21 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 04 May 2022 21:17:22 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 04 May 2022 21:17:23 GMT
EXPOSE 4222 6222 8222
# Wed, 04 May 2022 21:17:24 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 04 May 2022 21:17:26 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ba8181afd4264392fbbf8df14fb4cddc55fbe085ab000e986b789678bc2bb171`  
		Size: 997.6 MB (997587446 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7ebb23aa64bff633cfa3c62b190d84f0e870b04fecb1910f65d0870b5c7f8981`  
		Last Modified: Wed, 13 Apr 2022 14:12:24 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d838c7a98a95bee63894bac798124e8c8572bcacc23e22d85332d453a03a7d7c`  
		Last Modified: Wed, 13 Apr 2022 14:46:17 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bba18134d0cef899134f811c0896e8003b4b03b11726200e2d4f09ff3e350d1`  
		Last Modified: Wed, 04 May 2022 21:18:21 GMT  
		Size: 1.4 KB (1382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46e1de2ac2611197cf7e3985577bdf089a2330268d7f08ad53a25b42fcf7548b`  
		Last Modified: Wed, 04 May 2022 21:18:21 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:130538769de262aeb26e810412f9ee58d5b8c1aeb653929a4607901c92363b93`  
		Last Modified: Wed, 04 May 2022 21:18:21 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1684bc7f189afcbdc72f3a0c8eab43e13bbfbe3e8fb412ac51356098cefaeb9a`  
		Last Modified: Wed, 04 May 2022 21:18:21 GMT  
		Size: 359.4 KB (359393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c1c4f2e32fa9a2920cfaeae75fe3b7e64312357d7a20b2c5e7347936eef6dc5`  
		Last Modified: Wed, 04 May 2022 21:18:24 GMT  
		Size: 5.0 MB (4960732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c18367f87433f56d999dc8c84a381afa2e8d480302ea8c78e9169557cd843606`  
		Last Modified: Wed, 04 May 2022 21:18:18 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9279a91eef9f2b4bb4964ed362b6786dc737d38e07cb0266dcbe7441930a27f0`  
		Last Modified: Wed, 04 May 2022 21:18:18 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1ff9295d7bb66afbef49bab61a76a250ae513e6acdd9a8312b8a153c2cae64c`  
		Last Modified: Wed, 04 May 2022 21:18:18 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ce0d33690a32dfd5fb8003a197bdc540ec1d876be17a42ccd82d94634514974`  
		Last Modified: Wed, 04 May 2022 21:18:18 GMT  
		Size: 1.4 KB (1363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.8.2`

```console
$ docker pull nats@sha256:78f4dc57504675513e5051ce8f64598ddede060ec74a5ff9f253143b7a081503
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.2803; amd64

### `nats:2.8.2` - linux; amd64

```console
$ docker pull nats@sha256:d7022e467f53812285667fd004413e8cb15920efbb01d1d0f7c4194a2e084959
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4580109 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:71863590dea616f7cf93b753e1e7a3baf16f89747f06004d08f65d3fa907ee9a`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 04 May 2022 21:19:54 GMT
COPY file:1b0e004de765c2bffa3154a8b1990e8a621636f4f1d7ff504c566b8ba440d227 in /nats-server 
# Wed, 04 May 2022 21:19:54 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 04 May 2022 21:19:54 GMT
EXPOSE 4222 6222 8222
# Wed, 04 May 2022 21:19:54 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 04 May 2022 21:19:54 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 04 May 2022 21:19:54 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:cf7d6008a72749fed702f25d8a1bb63636b75bf34655ba074286dc54d0db2b5b`  
		Last Modified: Wed, 04 May 2022 21:20:43 GMT  
		Size: 4.6 MB (4579600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3ef91ad4507cb0bd768e027792377ba07aaaebc8d89981a6ee648d58561273b`  
		Last Modified: Wed, 04 May 2022 21:20:43 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.8.2` - linux; arm variant v6

```console
$ docker pull nats@sha256:80a268344378d95bf616b13ab6e787e5a242cadbaa9c933e6708bb8761cab22f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4238279 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d53b2041383be620a877c3c265658998b4c5a2f31c6f26d3dd2aa53cb78cf527`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 04 May 2022 22:01:42 GMT
COPY file:ed82059457db34cc43492a36d55b5f9133e36b8d203dcc971bb9feb5fb6a8528 in /nats-server 
# Wed, 04 May 2022 22:01:42 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 04 May 2022 22:01:43 GMT
EXPOSE 4222 6222 8222
# Wed, 04 May 2022 22:01:43 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 04 May 2022 22:01:44 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 04 May 2022 22:01:44 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b04b6f92c475d8e5e8cdec268c94ef3240dde7149afb05913d1099a7ae570a08`  
		Last Modified: Wed, 04 May 2022 22:04:04 GMT  
		Size: 4.2 MB (4237771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef916f73f04fb010ef2bb2bf3b7260ca2d52efb2591d966721af6b5251fd397d`  
		Last Modified: Wed, 04 May 2022 22:04:02 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.8.2` - linux; arm variant v7

```console
$ docker pull nats@sha256:5faa61f14caf7dc441f38d86641bd5918d1231b40e7acd0336f57843d8ef704b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4232641 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c4caf3fcf0c7865ec8500f33783b2ba88253c0e14828b887cc8b103228346c5`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 04 May 2022 22:18:15 GMT
COPY file:2f9ffa15f39f94a4d8c8c940d7ec0b2baee22852f8f3f2c24a707b69fc8fd84f in /nats-server 
# Wed, 04 May 2022 22:18:15 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 04 May 2022 22:18:16 GMT
EXPOSE 4222 6222 8222
# Wed, 04 May 2022 22:18:16 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 04 May 2022 22:18:17 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 04 May 2022 22:18:17 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:706ff613d28c2f6958458bb4d4ce83f519f2b76bde307418fe1603aac99ac21b`  
		Last Modified: Wed, 04 May 2022 22:20:36 GMT  
		Size: 4.2 MB (4232133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb718277dd458fca567c81e0168c051df2d97f4a8eb0cb348574822d90dec67d`  
		Last Modified: Wed, 04 May 2022 22:20:33 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.8.2` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:009869128938685fc6fee44029ac90758f29d3fc3e33fa7d5e47a7a3905ef115
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4218329 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a787d12c02030cc31984da44a61d89f3f472271982d215d29866617891286b13`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 04 May 2022 21:48:41 GMT
COPY file:8d0405148efb3d718582f81ff5f54494a8c9789f05e85832ee98d04d228af450 in /nats-server 
# Wed, 04 May 2022 21:48:42 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 04 May 2022 21:48:42 GMT
EXPOSE 4222 6222 8222
# Wed, 04 May 2022 21:48:43 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 04 May 2022 21:48:44 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 04 May 2022 21:48:45 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:8d57fa8f4dba3b0b06e2fd0e4e7b35276d5c1078bcf1be00321d6d56bba9aa78`  
		Last Modified: Wed, 04 May 2022 21:50:01 GMT  
		Size: 4.2 MB (4217820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b388c4e085cdf26d57e7c86c2bec5f6519929e7f9ec591330158ba39d77677b4`  
		Last Modified: Wed, 04 May 2022 21:50:00 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.8.2` - windows version 10.0.17763.2803; amd64

```console
$ docker pull nats@sha256:2b4914d94facbb6299c5ef2598f655a224c0f671a265bd2986f62c70b978582c
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.7 MB (107725201 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:762896cf7b68aecb4d2820c48789eeee8a8cbc7a58862c4bec5f4ad9d2ecd8f3`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 04 Apr 2022 10:52:49 GMT
RUN Apply image 1809-amd64
# Wed, 13 Apr 2022 14:45:42 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 04 May 2022 21:17:46 GMT
RUN cmd /S /C #(nop) COPY file:1e690007468fe11473f18dc8fbc8b7aa29351e71d03ca73f75d9fcfbf1fd7911 in C:\nats-server.exe 
# Wed, 04 May 2022 21:17:47 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 04 May 2022 21:17:48 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 04 May 2022 21:17:49 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 04 May 2022 21:17:49 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6fc97003d8b7f593fe071cf3ea64f3ce760cc060f3402bb6b1b849c040e222d5`  
		Size: 103.1 MB (103096169 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a6063f744e542c21ce471bdd7ff0dd6063d8d2a9670afbbc64d086813afd6385`  
		Last Modified: Wed, 13 Apr 2022 14:46:35 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c1e5f9285a324194ea2fae24594852b07a0fc1cec1388dcbc367215de23c29e`  
		Last Modified: Wed, 04 May 2022 21:18:39 GMT  
		Size: 4.6 MB (4622651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bde4044fa24dd3365cdc6ba5dff0779813bd4d34e566af1a5c4458c0a232fdc1`  
		Last Modified: Wed, 04 May 2022 21:18:38 GMT  
		Size: 1.8 KB (1791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:405a229a99882e5792c0dad43c80fb315b37c8b9c347f514baccd7d05c6c9f1c`  
		Last Modified: Wed, 04 May 2022 21:18:38 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1037a060f2ca6801837d7d720ec02ed6916e48ce1cfa49e6c7558ba04de8235`  
		Last Modified: Wed, 04 May 2022 21:18:38 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e29f6c2056586ca9353c7019499d854ba31068b682d59304ed4267576ebc5286`  
		Last Modified: Wed, 04 May 2022 21:18:38 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.8.2-alpine`

```console
$ docker pull nats@sha256:51ed1dcadcd928cbca6b4b2846491bd14667dca111ac63fdb001eef89cb9192f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.8.2-alpine` - linux; amd64

```console
$ docker pull nats@sha256:3dfa6b8def0d3c784ef7827f0c21b17afd01be56773c68d5950e9f29172ae796
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.7 MB (7667828 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3370f8d5fa5f0ea4cfdcaa60d7f568c2cf9e9752f3a75d11b0d30a257db8a51d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 05 Apr 2022 00:19:59 GMT
ADD file:5d673d25da3a14ce1f6cf66e4c7fd4f4b85a3759a9d93efb3fd9ff852b5b56e4 in / 
# Tue, 05 Apr 2022 00:19:59 GMT
CMD ["/bin/sh"]
# Wed, 04 May 2022 21:19:44 GMT
ENV NATS_SERVER=2.8.2
# Wed, 04 May 2022 21:19:47 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='3409b9dc76c0136cecded67115521d3a815f7a2f3739e81eb87a8d5d761843c3' ;; 		armhf) natsArch='arm6'; sha256='a3d474a583ca90e3577aa470335c582d4565918f500ebd28d760643fb631d8d5' ;; 		armv7) natsArch='arm7'; sha256='88fd437f7def8dbe68b17dce703c919771e64b570856bf0e6f2eb3b9459031c6' ;; 		x86_64) natsArch='amd64'; sha256='59805a464237801574ca7efdc69ebc21040e9b811fb53ed444c4808a05440719' ;; 		x86) natsArch='386'; sha256='facd3c69ee27c3e9e8654e5de95eb79de2e873bf4c066317aa9fad5c2ea26b92' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 04 May 2022 21:19:47 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 04 May 2022 21:19:47 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 04 May 2022 21:19:47 GMT
EXPOSE 4222 6222 8222
# Wed, 04 May 2022 21:19:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 04 May 2022 21:19:47 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:df9b9388f04ad6279a7410b85cedfdcb2208c0a003da7ab5613af71079148139`  
		Last Modified: Mon, 04 Apr 2022 19:10:16 GMT  
		Size: 2.8 MB (2814559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb157527e1f2e860f2700cadfdf0bed3ac0d50b8a177dd0b906431b0d46b44b5`  
		Last Modified: Wed, 04 May 2022 21:20:20 GMT  
		Size: 4.9 MB (4852271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c29bade32b2ef2ecc8325cbc5cbbf69470e5e20cc04e292244e704f68b9a6f86`  
		Last Modified: Wed, 04 May 2022 21:20:19 GMT  
		Size: 585.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dbec41bc3a042cdbf4c2e9b57c99bf99a4552e64a437be0066d42a04e3de650`  
		Last Modified: Wed, 04 May 2022 21:20:19 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.8.2-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:12b766cef3be0b9dc70e35a9cefcecbfad16a19e00b94a4737134ebbee24ea31
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7133599 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d1cc5ce43b7fd2c1dc34d986696c64da1a158fc067f5a4710ce475ce2f10eaec`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 04 Apr 2022 23:49:42 GMT
ADD file:159dcddaab900372df882a4e94615ed84250e9cea3e74bc0479d98280342f596 in / 
# Mon, 04 Apr 2022 23:49:42 GMT
CMD ["/bin/sh"]
# Wed, 04 May 2022 22:01:15 GMT
ENV NATS_SERVER=2.8.2
# Wed, 04 May 2022 22:01:19 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='3409b9dc76c0136cecded67115521d3a815f7a2f3739e81eb87a8d5d761843c3' ;; 		armhf) natsArch='arm6'; sha256='a3d474a583ca90e3577aa470335c582d4565918f500ebd28d760643fb631d8d5' ;; 		armv7) natsArch='arm7'; sha256='88fd437f7def8dbe68b17dce703c919771e64b570856bf0e6f2eb3b9459031c6' ;; 		x86_64) natsArch='amd64'; sha256='59805a464237801574ca7efdc69ebc21040e9b811fb53ed444c4808a05440719' ;; 		x86) natsArch='386'; sha256='facd3c69ee27c3e9e8654e5de95eb79de2e873bf4c066317aa9fad5c2ea26b92' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 04 May 2022 22:01:20 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 04 May 2022 22:01:20 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 04 May 2022 22:01:21 GMT
EXPOSE 4222 6222 8222
# Wed, 04 May 2022 22:01:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 04 May 2022 22:01:21 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:c319b1fc4ed70b8241a7ce6ac0c4015d354bf5cf8c01eb73c50b6709c0c46e49`  
		Last Modified: Mon, 04 Apr 2022 19:09:22 GMT  
		Size: 2.6 MB (2621972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3508da0a7a8c69badd89084de30d788f3c0bc57d625677ec7d68c32f18d466ba`  
		Last Modified: Wed, 04 May 2022 22:03:28 GMT  
		Size: 4.5 MB (4510625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7965b001731ee55e0b7b2c11c7ff5f851afaed57dba5ef2a08324fab5de994f7`  
		Last Modified: Wed, 04 May 2022 22:03:27 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8d031fa4afb68088db4a684f2332c5c8c3ecedb55d2aee461d64c8556afb468`  
		Last Modified: Wed, 04 May 2022 22:03:25 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.8.2-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:7d6c71099975b1e928511819a05612d582d412c5ed2838f04882514d0e77fff8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.9 MB (6930001 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3813055a26f58efed9d97ad053203ba493589fa6e486f3dd5810354defc6b3c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 04 Apr 2022 23:57:34 GMT
ADD file:20f8cdddc53a4a8bd78945fc32fe08e9f80ab3b16dc20a9aa4ba73b79f2bc71c in / 
# Mon, 04 Apr 2022 23:57:35 GMT
CMD ["/bin/sh"]
# Wed, 04 May 2022 22:17:46 GMT
ENV NATS_SERVER=2.8.2
# Wed, 04 May 2022 22:17:50 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='3409b9dc76c0136cecded67115521d3a815f7a2f3739e81eb87a8d5d761843c3' ;; 		armhf) natsArch='arm6'; sha256='a3d474a583ca90e3577aa470335c582d4565918f500ebd28d760643fb631d8d5' ;; 		armv7) natsArch='arm7'; sha256='88fd437f7def8dbe68b17dce703c919771e64b570856bf0e6f2eb3b9459031c6' ;; 		x86_64) natsArch='amd64'; sha256='59805a464237801574ca7efdc69ebc21040e9b811fb53ed444c4808a05440719' ;; 		x86) natsArch='386'; sha256='facd3c69ee27c3e9e8654e5de95eb79de2e873bf4c066317aa9fad5c2ea26b92' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 04 May 2022 22:17:50 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 04 May 2022 22:17:51 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 04 May 2022 22:17:51 GMT
EXPOSE 4222 6222 8222
# Wed, 04 May 2022 22:17:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 04 May 2022 22:17:52 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:57fb4b5f1a47c953ca5703f0f81ce14e5d01cf23aa79558b5adb961cc526e320`  
		Last Modified: Mon, 04 Apr 2022 19:09:36 GMT  
		Size: 2.4 MB (2424323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b49f3de3c7329a4a2fbd9e8c9cd595a837860930995c5a11d2459e045b8d2dab`  
		Last Modified: Wed, 04 May 2022 22:20:00 GMT  
		Size: 4.5 MB (4504680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51dc12ec06d594c70e53bb45c9912d27ad4869faf092615047ea9faab11d6ccb`  
		Last Modified: Wed, 04 May 2022 22:19:57 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5e0c0af17ebf42f5af072c2b71c091af0b659ac5e20a80c92ca74da9ec5353d`  
		Last Modified: Wed, 04 May 2022 22:19:57 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.8.2-alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:81e20b06f2b5aac1ca438142975de9c05234b243fcb497ab8afd7f0bcd4a28a8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7208259 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12c2a5e86ad6fc84ed6f66fecfc26474466d0f61712b85aa012fc0b7e726019e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:31 GMT
ADD file:90e56af13188c7f0283d244a0d70b853d8bef8587a41f1da8eac3a2aba8964ef in / 
# Mon, 04 Apr 2022 23:39:31 GMT
CMD ["/bin/sh"]
# Wed, 04 May 2022 21:48:24 GMT
ENV NATS_SERVER=2.8.2
# Wed, 04 May 2022 21:48:26 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='3409b9dc76c0136cecded67115521d3a815f7a2f3739e81eb87a8d5d761843c3' ;; 		armhf) natsArch='arm6'; sha256='a3d474a583ca90e3577aa470335c582d4565918f500ebd28d760643fb631d8d5' ;; 		armv7) natsArch='arm7'; sha256='88fd437f7def8dbe68b17dce703c919771e64b570856bf0e6f2eb3b9459031c6' ;; 		x86_64) natsArch='amd64'; sha256='59805a464237801574ca7efdc69ebc21040e9b811fb53ed444c4808a05440719' ;; 		x86) natsArch='386'; sha256='facd3c69ee27c3e9e8654e5de95eb79de2e873bf4c066317aa9fad5c2ea26b92' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 04 May 2022 21:48:28 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 04 May 2022 21:48:29 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 04 May 2022 21:48:29 GMT
EXPOSE 4222 6222 8222
# Wed, 04 May 2022 21:48:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 04 May 2022 21:48:31 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9981e73032c8833e387a8f96986e560edbed12c38119e0edb0439c9c2234eac9`  
		Last Modified: Mon, 04 Apr 2022 19:09:10 GMT  
		Size: 2.7 MB (2716477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec7ea9151b15b8e90d2a0ef58393de32cefb12a7f7c7e3d7a011808b38e59565`  
		Last Modified: Wed, 04 May 2022 21:49:31 GMT  
		Size: 4.5 MB (4490808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f800447a181fc7e3f37c2e68d8374347459e1d12a8d8c8653b7da45180ae97f`  
		Last Modified: Wed, 04 May 2022 21:49:30 GMT  
		Size: 560.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:894f3b307d2ae2b261df9d763e886b3ae75f9aba6dc927eaf3f28cae9375c050`  
		Last Modified: Wed, 04 May 2022 21:49:30 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.8.2-alpine3.15`

```console
$ docker pull nats@sha256:51ed1dcadcd928cbca6b4b2846491bd14667dca111ac63fdb001eef89cb9192f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.8.2-alpine3.15` - linux; amd64

```console
$ docker pull nats@sha256:3dfa6b8def0d3c784ef7827f0c21b17afd01be56773c68d5950e9f29172ae796
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.7 MB (7667828 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3370f8d5fa5f0ea4cfdcaa60d7f568c2cf9e9752f3a75d11b0d30a257db8a51d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 05 Apr 2022 00:19:59 GMT
ADD file:5d673d25da3a14ce1f6cf66e4c7fd4f4b85a3759a9d93efb3fd9ff852b5b56e4 in / 
# Tue, 05 Apr 2022 00:19:59 GMT
CMD ["/bin/sh"]
# Wed, 04 May 2022 21:19:44 GMT
ENV NATS_SERVER=2.8.2
# Wed, 04 May 2022 21:19:47 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='3409b9dc76c0136cecded67115521d3a815f7a2f3739e81eb87a8d5d761843c3' ;; 		armhf) natsArch='arm6'; sha256='a3d474a583ca90e3577aa470335c582d4565918f500ebd28d760643fb631d8d5' ;; 		armv7) natsArch='arm7'; sha256='88fd437f7def8dbe68b17dce703c919771e64b570856bf0e6f2eb3b9459031c6' ;; 		x86_64) natsArch='amd64'; sha256='59805a464237801574ca7efdc69ebc21040e9b811fb53ed444c4808a05440719' ;; 		x86) natsArch='386'; sha256='facd3c69ee27c3e9e8654e5de95eb79de2e873bf4c066317aa9fad5c2ea26b92' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 04 May 2022 21:19:47 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 04 May 2022 21:19:47 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 04 May 2022 21:19:47 GMT
EXPOSE 4222 6222 8222
# Wed, 04 May 2022 21:19:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 04 May 2022 21:19:47 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:df9b9388f04ad6279a7410b85cedfdcb2208c0a003da7ab5613af71079148139`  
		Last Modified: Mon, 04 Apr 2022 19:10:16 GMT  
		Size: 2.8 MB (2814559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb157527e1f2e860f2700cadfdf0bed3ac0d50b8a177dd0b906431b0d46b44b5`  
		Last Modified: Wed, 04 May 2022 21:20:20 GMT  
		Size: 4.9 MB (4852271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c29bade32b2ef2ecc8325cbc5cbbf69470e5e20cc04e292244e704f68b9a6f86`  
		Last Modified: Wed, 04 May 2022 21:20:19 GMT  
		Size: 585.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dbec41bc3a042cdbf4c2e9b57c99bf99a4552e64a437be0066d42a04e3de650`  
		Last Modified: Wed, 04 May 2022 21:20:19 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.8.2-alpine3.15` - linux; arm variant v6

```console
$ docker pull nats@sha256:12b766cef3be0b9dc70e35a9cefcecbfad16a19e00b94a4737134ebbee24ea31
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7133599 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d1cc5ce43b7fd2c1dc34d986696c64da1a158fc067f5a4710ce475ce2f10eaec`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 04 Apr 2022 23:49:42 GMT
ADD file:159dcddaab900372df882a4e94615ed84250e9cea3e74bc0479d98280342f596 in / 
# Mon, 04 Apr 2022 23:49:42 GMT
CMD ["/bin/sh"]
# Wed, 04 May 2022 22:01:15 GMT
ENV NATS_SERVER=2.8.2
# Wed, 04 May 2022 22:01:19 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='3409b9dc76c0136cecded67115521d3a815f7a2f3739e81eb87a8d5d761843c3' ;; 		armhf) natsArch='arm6'; sha256='a3d474a583ca90e3577aa470335c582d4565918f500ebd28d760643fb631d8d5' ;; 		armv7) natsArch='arm7'; sha256='88fd437f7def8dbe68b17dce703c919771e64b570856bf0e6f2eb3b9459031c6' ;; 		x86_64) natsArch='amd64'; sha256='59805a464237801574ca7efdc69ebc21040e9b811fb53ed444c4808a05440719' ;; 		x86) natsArch='386'; sha256='facd3c69ee27c3e9e8654e5de95eb79de2e873bf4c066317aa9fad5c2ea26b92' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 04 May 2022 22:01:20 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 04 May 2022 22:01:20 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 04 May 2022 22:01:21 GMT
EXPOSE 4222 6222 8222
# Wed, 04 May 2022 22:01:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 04 May 2022 22:01:21 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:c319b1fc4ed70b8241a7ce6ac0c4015d354bf5cf8c01eb73c50b6709c0c46e49`  
		Last Modified: Mon, 04 Apr 2022 19:09:22 GMT  
		Size: 2.6 MB (2621972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3508da0a7a8c69badd89084de30d788f3c0bc57d625677ec7d68c32f18d466ba`  
		Last Modified: Wed, 04 May 2022 22:03:28 GMT  
		Size: 4.5 MB (4510625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7965b001731ee55e0b7b2c11c7ff5f851afaed57dba5ef2a08324fab5de994f7`  
		Last Modified: Wed, 04 May 2022 22:03:27 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8d031fa4afb68088db4a684f2332c5c8c3ecedb55d2aee461d64c8556afb468`  
		Last Modified: Wed, 04 May 2022 22:03:25 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.8.2-alpine3.15` - linux; arm variant v7

```console
$ docker pull nats@sha256:7d6c71099975b1e928511819a05612d582d412c5ed2838f04882514d0e77fff8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.9 MB (6930001 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3813055a26f58efed9d97ad053203ba493589fa6e486f3dd5810354defc6b3c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 04 Apr 2022 23:57:34 GMT
ADD file:20f8cdddc53a4a8bd78945fc32fe08e9f80ab3b16dc20a9aa4ba73b79f2bc71c in / 
# Mon, 04 Apr 2022 23:57:35 GMT
CMD ["/bin/sh"]
# Wed, 04 May 2022 22:17:46 GMT
ENV NATS_SERVER=2.8.2
# Wed, 04 May 2022 22:17:50 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='3409b9dc76c0136cecded67115521d3a815f7a2f3739e81eb87a8d5d761843c3' ;; 		armhf) natsArch='arm6'; sha256='a3d474a583ca90e3577aa470335c582d4565918f500ebd28d760643fb631d8d5' ;; 		armv7) natsArch='arm7'; sha256='88fd437f7def8dbe68b17dce703c919771e64b570856bf0e6f2eb3b9459031c6' ;; 		x86_64) natsArch='amd64'; sha256='59805a464237801574ca7efdc69ebc21040e9b811fb53ed444c4808a05440719' ;; 		x86) natsArch='386'; sha256='facd3c69ee27c3e9e8654e5de95eb79de2e873bf4c066317aa9fad5c2ea26b92' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 04 May 2022 22:17:50 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 04 May 2022 22:17:51 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 04 May 2022 22:17:51 GMT
EXPOSE 4222 6222 8222
# Wed, 04 May 2022 22:17:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 04 May 2022 22:17:52 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:57fb4b5f1a47c953ca5703f0f81ce14e5d01cf23aa79558b5adb961cc526e320`  
		Last Modified: Mon, 04 Apr 2022 19:09:36 GMT  
		Size: 2.4 MB (2424323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b49f3de3c7329a4a2fbd9e8c9cd595a837860930995c5a11d2459e045b8d2dab`  
		Last Modified: Wed, 04 May 2022 22:20:00 GMT  
		Size: 4.5 MB (4504680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51dc12ec06d594c70e53bb45c9912d27ad4869faf092615047ea9faab11d6ccb`  
		Last Modified: Wed, 04 May 2022 22:19:57 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5e0c0af17ebf42f5af072c2b71c091af0b659ac5e20a80c92ca74da9ec5353d`  
		Last Modified: Wed, 04 May 2022 22:19:57 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.8.2-alpine3.15` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:81e20b06f2b5aac1ca438142975de9c05234b243fcb497ab8afd7f0bcd4a28a8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7208259 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12c2a5e86ad6fc84ed6f66fecfc26474466d0f61712b85aa012fc0b7e726019e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:31 GMT
ADD file:90e56af13188c7f0283d244a0d70b853d8bef8587a41f1da8eac3a2aba8964ef in / 
# Mon, 04 Apr 2022 23:39:31 GMT
CMD ["/bin/sh"]
# Wed, 04 May 2022 21:48:24 GMT
ENV NATS_SERVER=2.8.2
# Wed, 04 May 2022 21:48:26 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='3409b9dc76c0136cecded67115521d3a815f7a2f3739e81eb87a8d5d761843c3' ;; 		armhf) natsArch='arm6'; sha256='a3d474a583ca90e3577aa470335c582d4565918f500ebd28d760643fb631d8d5' ;; 		armv7) natsArch='arm7'; sha256='88fd437f7def8dbe68b17dce703c919771e64b570856bf0e6f2eb3b9459031c6' ;; 		x86_64) natsArch='amd64'; sha256='59805a464237801574ca7efdc69ebc21040e9b811fb53ed444c4808a05440719' ;; 		x86) natsArch='386'; sha256='facd3c69ee27c3e9e8654e5de95eb79de2e873bf4c066317aa9fad5c2ea26b92' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 04 May 2022 21:48:28 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 04 May 2022 21:48:29 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 04 May 2022 21:48:29 GMT
EXPOSE 4222 6222 8222
# Wed, 04 May 2022 21:48:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 04 May 2022 21:48:31 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9981e73032c8833e387a8f96986e560edbed12c38119e0edb0439c9c2234eac9`  
		Last Modified: Mon, 04 Apr 2022 19:09:10 GMT  
		Size: 2.7 MB (2716477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec7ea9151b15b8e90d2a0ef58393de32cefb12a7f7c7e3d7a011808b38e59565`  
		Last Modified: Wed, 04 May 2022 21:49:31 GMT  
		Size: 4.5 MB (4490808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f800447a181fc7e3f37c2e68d8374347459e1d12a8d8c8653b7da45180ae97f`  
		Last Modified: Wed, 04 May 2022 21:49:30 GMT  
		Size: 560.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:894f3b307d2ae2b261df9d763e886b3ae75f9aba6dc927eaf3f28cae9375c050`  
		Last Modified: Wed, 04 May 2022 21:49:30 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.8.2-linux`

```console
$ docker pull nats@sha256:dd400785e2c069158ca6a488873976cab93098904db7fcc044cfc6af0327640c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.8.2-linux` - linux; amd64

```console
$ docker pull nats@sha256:d7022e467f53812285667fd004413e8cb15920efbb01d1d0f7c4194a2e084959
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4580109 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:71863590dea616f7cf93b753e1e7a3baf16f89747f06004d08f65d3fa907ee9a`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 04 May 2022 21:19:54 GMT
COPY file:1b0e004de765c2bffa3154a8b1990e8a621636f4f1d7ff504c566b8ba440d227 in /nats-server 
# Wed, 04 May 2022 21:19:54 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 04 May 2022 21:19:54 GMT
EXPOSE 4222 6222 8222
# Wed, 04 May 2022 21:19:54 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 04 May 2022 21:19:54 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 04 May 2022 21:19:54 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:cf7d6008a72749fed702f25d8a1bb63636b75bf34655ba074286dc54d0db2b5b`  
		Last Modified: Wed, 04 May 2022 21:20:43 GMT  
		Size: 4.6 MB (4579600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3ef91ad4507cb0bd768e027792377ba07aaaebc8d89981a6ee648d58561273b`  
		Last Modified: Wed, 04 May 2022 21:20:43 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.8.2-linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:80a268344378d95bf616b13ab6e787e5a242cadbaa9c933e6708bb8761cab22f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4238279 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d53b2041383be620a877c3c265658998b4c5a2f31c6f26d3dd2aa53cb78cf527`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 04 May 2022 22:01:42 GMT
COPY file:ed82059457db34cc43492a36d55b5f9133e36b8d203dcc971bb9feb5fb6a8528 in /nats-server 
# Wed, 04 May 2022 22:01:42 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 04 May 2022 22:01:43 GMT
EXPOSE 4222 6222 8222
# Wed, 04 May 2022 22:01:43 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 04 May 2022 22:01:44 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 04 May 2022 22:01:44 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b04b6f92c475d8e5e8cdec268c94ef3240dde7149afb05913d1099a7ae570a08`  
		Last Modified: Wed, 04 May 2022 22:04:04 GMT  
		Size: 4.2 MB (4237771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef916f73f04fb010ef2bb2bf3b7260ca2d52efb2591d966721af6b5251fd397d`  
		Last Modified: Wed, 04 May 2022 22:04:02 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.8.2-linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:5faa61f14caf7dc441f38d86641bd5918d1231b40e7acd0336f57843d8ef704b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4232641 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c4caf3fcf0c7865ec8500f33783b2ba88253c0e14828b887cc8b103228346c5`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 04 May 2022 22:18:15 GMT
COPY file:2f9ffa15f39f94a4d8c8c940d7ec0b2baee22852f8f3f2c24a707b69fc8fd84f in /nats-server 
# Wed, 04 May 2022 22:18:15 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 04 May 2022 22:18:16 GMT
EXPOSE 4222 6222 8222
# Wed, 04 May 2022 22:18:16 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 04 May 2022 22:18:17 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 04 May 2022 22:18:17 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:706ff613d28c2f6958458bb4d4ce83f519f2b76bde307418fe1603aac99ac21b`  
		Last Modified: Wed, 04 May 2022 22:20:36 GMT  
		Size: 4.2 MB (4232133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb718277dd458fca567c81e0168c051df2d97f4a8eb0cb348574822d90dec67d`  
		Last Modified: Wed, 04 May 2022 22:20:33 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.8.2-linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:009869128938685fc6fee44029ac90758f29d3fc3e33fa7d5e47a7a3905ef115
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4218329 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a787d12c02030cc31984da44a61d89f3f472271982d215d29866617891286b13`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 04 May 2022 21:48:41 GMT
COPY file:8d0405148efb3d718582f81ff5f54494a8c9789f05e85832ee98d04d228af450 in /nats-server 
# Wed, 04 May 2022 21:48:42 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 04 May 2022 21:48:42 GMT
EXPOSE 4222 6222 8222
# Wed, 04 May 2022 21:48:43 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 04 May 2022 21:48:44 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 04 May 2022 21:48:45 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:8d57fa8f4dba3b0b06e2fd0e4e7b35276d5c1078bcf1be00321d6d56bba9aa78`  
		Last Modified: Wed, 04 May 2022 21:50:01 GMT  
		Size: 4.2 MB (4217820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b388c4e085cdf26d57e7c86c2bec5f6519929e7f9ec591330158ba39d77677b4`  
		Last Modified: Wed, 04 May 2022 21:50:00 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.8.2-nanoserver`

```console
$ docker pull nats@sha256:f128bdd66f848762f7bb7c580b2d89e4c329ce85461597353dcbff405ddda643
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2803; amd64

### `nats:2.8.2-nanoserver` - windows version 10.0.17763.2803; amd64

```console
$ docker pull nats@sha256:2b4914d94facbb6299c5ef2598f655a224c0f671a265bd2986f62c70b978582c
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.7 MB (107725201 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:762896cf7b68aecb4d2820c48789eeee8a8cbc7a58862c4bec5f4ad9d2ecd8f3`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 04 Apr 2022 10:52:49 GMT
RUN Apply image 1809-amd64
# Wed, 13 Apr 2022 14:45:42 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 04 May 2022 21:17:46 GMT
RUN cmd /S /C #(nop) COPY file:1e690007468fe11473f18dc8fbc8b7aa29351e71d03ca73f75d9fcfbf1fd7911 in C:\nats-server.exe 
# Wed, 04 May 2022 21:17:47 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 04 May 2022 21:17:48 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 04 May 2022 21:17:49 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 04 May 2022 21:17:49 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6fc97003d8b7f593fe071cf3ea64f3ce760cc060f3402bb6b1b849c040e222d5`  
		Size: 103.1 MB (103096169 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a6063f744e542c21ce471bdd7ff0dd6063d8d2a9670afbbc64d086813afd6385`  
		Last Modified: Wed, 13 Apr 2022 14:46:35 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c1e5f9285a324194ea2fae24594852b07a0fc1cec1388dcbc367215de23c29e`  
		Last Modified: Wed, 04 May 2022 21:18:39 GMT  
		Size: 4.6 MB (4622651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bde4044fa24dd3365cdc6ba5dff0779813bd4d34e566af1a5c4458c0a232fdc1`  
		Last Modified: Wed, 04 May 2022 21:18:38 GMT  
		Size: 1.8 KB (1791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:405a229a99882e5792c0dad43c80fb315b37c8b9c347f514baccd7d05c6c9f1c`  
		Last Modified: Wed, 04 May 2022 21:18:38 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1037a060f2ca6801837d7d720ec02ed6916e48ce1cfa49e6c7558ba04de8235`  
		Last Modified: Wed, 04 May 2022 21:18:38 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e29f6c2056586ca9353c7019499d854ba31068b682d59304ed4267576ebc5286`  
		Last Modified: Wed, 04 May 2022 21:18:38 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.8.2-nanoserver-1809`

```console
$ docker pull nats@sha256:f128bdd66f848762f7bb7c580b2d89e4c329ce85461597353dcbff405ddda643
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2803; amd64

### `nats:2.8.2-nanoserver-1809` - windows version 10.0.17763.2803; amd64

```console
$ docker pull nats@sha256:2b4914d94facbb6299c5ef2598f655a224c0f671a265bd2986f62c70b978582c
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.7 MB (107725201 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:762896cf7b68aecb4d2820c48789eeee8a8cbc7a58862c4bec5f4ad9d2ecd8f3`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 04 Apr 2022 10:52:49 GMT
RUN Apply image 1809-amd64
# Wed, 13 Apr 2022 14:45:42 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 04 May 2022 21:17:46 GMT
RUN cmd /S /C #(nop) COPY file:1e690007468fe11473f18dc8fbc8b7aa29351e71d03ca73f75d9fcfbf1fd7911 in C:\nats-server.exe 
# Wed, 04 May 2022 21:17:47 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 04 May 2022 21:17:48 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 04 May 2022 21:17:49 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 04 May 2022 21:17:49 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6fc97003d8b7f593fe071cf3ea64f3ce760cc060f3402bb6b1b849c040e222d5`  
		Size: 103.1 MB (103096169 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a6063f744e542c21ce471bdd7ff0dd6063d8d2a9670afbbc64d086813afd6385`  
		Last Modified: Wed, 13 Apr 2022 14:46:35 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c1e5f9285a324194ea2fae24594852b07a0fc1cec1388dcbc367215de23c29e`  
		Last Modified: Wed, 04 May 2022 21:18:39 GMT  
		Size: 4.6 MB (4622651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bde4044fa24dd3365cdc6ba5dff0779813bd4d34e566af1a5c4458c0a232fdc1`  
		Last Modified: Wed, 04 May 2022 21:18:38 GMT  
		Size: 1.8 KB (1791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:405a229a99882e5792c0dad43c80fb315b37c8b9c347f514baccd7d05c6c9f1c`  
		Last Modified: Wed, 04 May 2022 21:18:38 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1037a060f2ca6801837d7d720ec02ed6916e48ce1cfa49e6c7558ba04de8235`  
		Last Modified: Wed, 04 May 2022 21:18:38 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e29f6c2056586ca9353c7019499d854ba31068b682d59304ed4267576ebc5286`  
		Last Modified: Wed, 04 May 2022 21:18:38 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.8.2-scratch`

```console
$ docker pull nats@sha256:dd400785e2c069158ca6a488873976cab93098904db7fcc044cfc6af0327640c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.8.2-scratch` - linux; amd64

```console
$ docker pull nats@sha256:d7022e467f53812285667fd004413e8cb15920efbb01d1d0f7c4194a2e084959
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4580109 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:71863590dea616f7cf93b753e1e7a3baf16f89747f06004d08f65d3fa907ee9a`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 04 May 2022 21:19:54 GMT
COPY file:1b0e004de765c2bffa3154a8b1990e8a621636f4f1d7ff504c566b8ba440d227 in /nats-server 
# Wed, 04 May 2022 21:19:54 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 04 May 2022 21:19:54 GMT
EXPOSE 4222 6222 8222
# Wed, 04 May 2022 21:19:54 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 04 May 2022 21:19:54 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 04 May 2022 21:19:54 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:cf7d6008a72749fed702f25d8a1bb63636b75bf34655ba074286dc54d0db2b5b`  
		Last Modified: Wed, 04 May 2022 21:20:43 GMT  
		Size: 4.6 MB (4579600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3ef91ad4507cb0bd768e027792377ba07aaaebc8d89981a6ee648d58561273b`  
		Last Modified: Wed, 04 May 2022 21:20:43 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.8.2-scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:80a268344378d95bf616b13ab6e787e5a242cadbaa9c933e6708bb8761cab22f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4238279 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d53b2041383be620a877c3c265658998b4c5a2f31c6f26d3dd2aa53cb78cf527`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 04 May 2022 22:01:42 GMT
COPY file:ed82059457db34cc43492a36d55b5f9133e36b8d203dcc971bb9feb5fb6a8528 in /nats-server 
# Wed, 04 May 2022 22:01:42 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 04 May 2022 22:01:43 GMT
EXPOSE 4222 6222 8222
# Wed, 04 May 2022 22:01:43 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 04 May 2022 22:01:44 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 04 May 2022 22:01:44 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b04b6f92c475d8e5e8cdec268c94ef3240dde7149afb05913d1099a7ae570a08`  
		Last Modified: Wed, 04 May 2022 22:04:04 GMT  
		Size: 4.2 MB (4237771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef916f73f04fb010ef2bb2bf3b7260ca2d52efb2591d966721af6b5251fd397d`  
		Last Modified: Wed, 04 May 2022 22:04:02 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.8.2-scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:5faa61f14caf7dc441f38d86641bd5918d1231b40e7acd0336f57843d8ef704b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4232641 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c4caf3fcf0c7865ec8500f33783b2ba88253c0e14828b887cc8b103228346c5`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 04 May 2022 22:18:15 GMT
COPY file:2f9ffa15f39f94a4d8c8c940d7ec0b2baee22852f8f3f2c24a707b69fc8fd84f in /nats-server 
# Wed, 04 May 2022 22:18:15 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 04 May 2022 22:18:16 GMT
EXPOSE 4222 6222 8222
# Wed, 04 May 2022 22:18:16 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 04 May 2022 22:18:17 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 04 May 2022 22:18:17 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:706ff613d28c2f6958458bb4d4ce83f519f2b76bde307418fe1603aac99ac21b`  
		Last Modified: Wed, 04 May 2022 22:20:36 GMT  
		Size: 4.2 MB (4232133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb718277dd458fca567c81e0168c051df2d97f4a8eb0cb348574822d90dec67d`  
		Last Modified: Wed, 04 May 2022 22:20:33 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.8.2-scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:009869128938685fc6fee44029ac90758f29d3fc3e33fa7d5e47a7a3905ef115
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4218329 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a787d12c02030cc31984da44a61d89f3f472271982d215d29866617891286b13`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 04 May 2022 21:48:41 GMT
COPY file:8d0405148efb3d718582f81ff5f54494a8c9789f05e85832ee98d04d228af450 in /nats-server 
# Wed, 04 May 2022 21:48:42 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 04 May 2022 21:48:42 GMT
EXPOSE 4222 6222 8222
# Wed, 04 May 2022 21:48:43 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 04 May 2022 21:48:44 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 04 May 2022 21:48:45 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:8d57fa8f4dba3b0b06e2fd0e4e7b35276d5c1078bcf1be00321d6d56bba9aa78`  
		Last Modified: Wed, 04 May 2022 21:50:01 GMT  
		Size: 4.2 MB (4217820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b388c4e085cdf26d57e7c86c2bec5f6519929e7f9ec591330158ba39d77677b4`  
		Last Modified: Wed, 04 May 2022 21:50:00 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.8.2-windowsservercore`

```console
$ docker pull nats@sha256:73f511081ca198af5f5c5d1d5d609bf6cfc5a7d43f01e1c93b4b718eaa7bc1d7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2803; amd64

### `nats:2.8.2-windowsservercore` - windows version 10.0.17763.2803; amd64

```console
$ docker pull nats@sha256:6ed34062ddcdb57863540c220de7d892b2b3152ae6599e25ff1405defc63d9db
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2721253627 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:392c84a5f744aeb82235810dec31fe58510c59683d8530e1727645ae02a45a8f`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 04 Apr 2022 11:20:25 GMT
RUN Install update 1809-amd64
# Wed, 13 Apr 2022 12:43:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 Apr 2022 14:42:30 GMT
ENV NATS_DOCKERIZED=1
# Wed, 04 May 2022 21:14:48 GMT
ENV NATS_SERVER=2.8.2
# Wed, 04 May 2022 21:14:49 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.8.2/nats-server-v2.8.2-windows-amd64.zip
# Wed, 04 May 2022 21:14:50 GMT
ENV NATS_SERVER_SHASUM=300b9743afa50e02e4e8d43dc212bfde8a871617bd524829114e19ff680dde11
# Wed, 04 May 2022 21:15:50 GMT
RUN Set-PSDebug -Trace 2
# Wed, 04 May 2022 21:17:21 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 04 May 2022 21:17:22 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 04 May 2022 21:17:23 GMT
EXPOSE 4222 6222 8222
# Wed, 04 May 2022 21:17:24 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 04 May 2022 21:17:26 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ba8181afd4264392fbbf8df14fb4cddc55fbe085ab000e986b789678bc2bb171`  
		Size: 997.6 MB (997587446 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7ebb23aa64bff633cfa3c62b190d84f0e870b04fecb1910f65d0870b5c7f8981`  
		Last Modified: Wed, 13 Apr 2022 14:12:24 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d838c7a98a95bee63894bac798124e8c8572bcacc23e22d85332d453a03a7d7c`  
		Last Modified: Wed, 13 Apr 2022 14:46:17 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bba18134d0cef899134f811c0896e8003b4b03b11726200e2d4f09ff3e350d1`  
		Last Modified: Wed, 04 May 2022 21:18:21 GMT  
		Size: 1.4 KB (1382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46e1de2ac2611197cf7e3985577bdf089a2330268d7f08ad53a25b42fcf7548b`  
		Last Modified: Wed, 04 May 2022 21:18:21 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:130538769de262aeb26e810412f9ee58d5b8c1aeb653929a4607901c92363b93`  
		Last Modified: Wed, 04 May 2022 21:18:21 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1684bc7f189afcbdc72f3a0c8eab43e13bbfbe3e8fb412ac51356098cefaeb9a`  
		Last Modified: Wed, 04 May 2022 21:18:21 GMT  
		Size: 359.4 KB (359393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c1c4f2e32fa9a2920cfaeae75fe3b7e64312357d7a20b2c5e7347936eef6dc5`  
		Last Modified: Wed, 04 May 2022 21:18:24 GMT  
		Size: 5.0 MB (4960732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c18367f87433f56d999dc8c84a381afa2e8d480302ea8c78e9169557cd843606`  
		Last Modified: Wed, 04 May 2022 21:18:18 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9279a91eef9f2b4bb4964ed362b6786dc737d38e07cb0266dcbe7441930a27f0`  
		Last Modified: Wed, 04 May 2022 21:18:18 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1ff9295d7bb66afbef49bab61a76a250ae513e6acdd9a8312b8a153c2cae64c`  
		Last Modified: Wed, 04 May 2022 21:18:18 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ce0d33690a32dfd5fb8003a197bdc540ec1d876be17a42ccd82d94634514974`  
		Last Modified: Wed, 04 May 2022 21:18:18 GMT  
		Size: 1.4 KB (1363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.8.2-windowsservercore-1809`

```console
$ docker pull nats@sha256:73f511081ca198af5f5c5d1d5d609bf6cfc5a7d43f01e1c93b4b718eaa7bc1d7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2803; amd64

### `nats:2.8.2-windowsservercore-1809` - windows version 10.0.17763.2803; amd64

```console
$ docker pull nats@sha256:6ed34062ddcdb57863540c220de7d892b2b3152ae6599e25ff1405defc63d9db
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2721253627 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:392c84a5f744aeb82235810dec31fe58510c59683d8530e1727645ae02a45a8f`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 04 Apr 2022 11:20:25 GMT
RUN Install update 1809-amd64
# Wed, 13 Apr 2022 12:43:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 Apr 2022 14:42:30 GMT
ENV NATS_DOCKERIZED=1
# Wed, 04 May 2022 21:14:48 GMT
ENV NATS_SERVER=2.8.2
# Wed, 04 May 2022 21:14:49 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.8.2/nats-server-v2.8.2-windows-amd64.zip
# Wed, 04 May 2022 21:14:50 GMT
ENV NATS_SERVER_SHASUM=300b9743afa50e02e4e8d43dc212bfde8a871617bd524829114e19ff680dde11
# Wed, 04 May 2022 21:15:50 GMT
RUN Set-PSDebug -Trace 2
# Wed, 04 May 2022 21:17:21 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 04 May 2022 21:17:22 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 04 May 2022 21:17:23 GMT
EXPOSE 4222 6222 8222
# Wed, 04 May 2022 21:17:24 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 04 May 2022 21:17:26 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ba8181afd4264392fbbf8df14fb4cddc55fbe085ab000e986b789678bc2bb171`  
		Size: 997.6 MB (997587446 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7ebb23aa64bff633cfa3c62b190d84f0e870b04fecb1910f65d0870b5c7f8981`  
		Last Modified: Wed, 13 Apr 2022 14:12:24 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d838c7a98a95bee63894bac798124e8c8572bcacc23e22d85332d453a03a7d7c`  
		Last Modified: Wed, 13 Apr 2022 14:46:17 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bba18134d0cef899134f811c0896e8003b4b03b11726200e2d4f09ff3e350d1`  
		Last Modified: Wed, 04 May 2022 21:18:21 GMT  
		Size: 1.4 KB (1382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46e1de2ac2611197cf7e3985577bdf089a2330268d7f08ad53a25b42fcf7548b`  
		Last Modified: Wed, 04 May 2022 21:18:21 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:130538769de262aeb26e810412f9ee58d5b8c1aeb653929a4607901c92363b93`  
		Last Modified: Wed, 04 May 2022 21:18:21 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1684bc7f189afcbdc72f3a0c8eab43e13bbfbe3e8fb412ac51356098cefaeb9a`  
		Last Modified: Wed, 04 May 2022 21:18:21 GMT  
		Size: 359.4 KB (359393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c1c4f2e32fa9a2920cfaeae75fe3b7e64312357d7a20b2c5e7347936eef6dc5`  
		Last Modified: Wed, 04 May 2022 21:18:24 GMT  
		Size: 5.0 MB (4960732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c18367f87433f56d999dc8c84a381afa2e8d480302ea8c78e9169557cd843606`  
		Last Modified: Wed, 04 May 2022 21:18:18 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9279a91eef9f2b4bb4964ed362b6786dc737d38e07cb0266dcbe7441930a27f0`  
		Last Modified: Wed, 04 May 2022 21:18:18 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1ff9295d7bb66afbef49bab61a76a250ae513e6acdd9a8312b8a153c2cae64c`  
		Last Modified: Wed, 04 May 2022 21:18:18 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ce0d33690a32dfd5fb8003a197bdc540ec1d876be17a42ccd82d94634514974`  
		Last Modified: Wed, 04 May 2022 21:18:18 GMT  
		Size: 1.4 KB (1363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:alpine`

```console
$ docker pull nats@sha256:51ed1dcadcd928cbca6b4b2846491bd14667dca111ac63fdb001eef89cb9192f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:alpine` - linux; amd64

```console
$ docker pull nats@sha256:3dfa6b8def0d3c784ef7827f0c21b17afd01be56773c68d5950e9f29172ae796
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.7 MB (7667828 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3370f8d5fa5f0ea4cfdcaa60d7f568c2cf9e9752f3a75d11b0d30a257db8a51d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 05 Apr 2022 00:19:59 GMT
ADD file:5d673d25da3a14ce1f6cf66e4c7fd4f4b85a3759a9d93efb3fd9ff852b5b56e4 in / 
# Tue, 05 Apr 2022 00:19:59 GMT
CMD ["/bin/sh"]
# Wed, 04 May 2022 21:19:44 GMT
ENV NATS_SERVER=2.8.2
# Wed, 04 May 2022 21:19:47 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='3409b9dc76c0136cecded67115521d3a815f7a2f3739e81eb87a8d5d761843c3' ;; 		armhf) natsArch='arm6'; sha256='a3d474a583ca90e3577aa470335c582d4565918f500ebd28d760643fb631d8d5' ;; 		armv7) natsArch='arm7'; sha256='88fd437f7def8dbe68b17dce703c919771e64b570856bf0e6f2eb3b9459031c6' ;; 		x86_64) natsArch='amd64'; sha256='59805a464237801574ca7efdc69ebc21040e9b811fb53ed444c4808a05440719' ;; 		x86) natsArch='386'; sha256='facd3c69ee27c3e9e8654e5de95eb79de2e873bf4c066317aa9fad5c2ea26b92' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 04 May 2022 21:19:47 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 04 May 2022 21:19:47 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 04 May 2022 21:19:47 GMT
EXPOSE 4222 6222 8222
# Wed, 04 May 2022 21:19:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 04 May 2022 21:19:47 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:df9b9388f04ad6279a7410b85cedfdcb2208c0a003da7ab5613af71079148139`  
		Last Modified: Mon, 04 Apr 2022 19:10:16 GMT  
		Size: 2.8 MB (2814559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb157527e1f2e860f2700cadfdf0bed3ac0d50b8a177dd0b906431b0d46b44b5`  
		Last Modified: Wed, 04 May 2022 21:20:20 GMT  
		Size: 4.9 MB (4852271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c29bade32b2ef2ecc8325cbc5cbbf69470e5e20cc04e292244e704f68b9a6f86`  
		Last Modified: Wed, 04 May 2022 21:20:19 GMT  
		Size: 585.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dbec41bc3a042cdbf4c2e9b57c99bf99a4552e64a437be0066d42a04e3de650`  
		Last Modified: Wed, 04 May 2022 21:20:19 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:12b766cef3be0b9dc70e35a9cefcecbfad16a19e00b94a4737134ebbee24ea31
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7133599 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d1cc5ce43b7fd2c1dc34d986696c64da1a158fc067f5a4710ce475ce2f10eaec`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 04 Apr 2022 23:49:42 GMT
ADD file:159dcddaab900372df882a4e94615ed84250e9cea3e74bc0479d98280342f596 in / 
# Mon, 04 Apr 2022 23:49:42 GMT
CMD ["/bin/sh"]
# Wed, 04 May 2022 22:01:15 GMT
ENV NATS_SERVER=2.8.2
# Wed, 04 May 2022 22:01:19 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='3409b9dc76c0136cecded67115521d3a815f7a2f3739e81eb87a8d5d761843c3' ;; 		armhf) natsArch='arm6'; sha256='a3d474a583ca90e3577aa470335c582d4565918f500ebd28d760643fb631d8d5' ;; 		armv7) natsArch='arm7'; sha256='88fd437f7def8dbe68b17dce703c919771e64b570856bf0e6f2eb3b9459031c6' ;; 		x86_64) natsArch='amd64'; sha256='59805a464237801574ca7efdc69ebc21040e9b811fb53ed444c4808a05440719' ;; 		x86) natsArch='386'; sha256='facd3c69ee27c3e9e8654e5de95eb79de2e873bf4c066317aa9fad5c2ea26b92' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 04 May 2022 22:01:20 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 04 May 2022 22:01:20 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 04 May 2022 22:01:21 GMT
EXPOSE 4222 6222 8222
# Wed, 04 May 2022 22:01:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 04 May 2022 22:01:21 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:c319b1fc4ed70b8241a7ce6ac0c4015d354bf5cf8c01eb73c50b6709c0c46e49`  
		Last Modified: Mon, 04 Apr 2022 19:09:22 GMT  
		Size: 2.6 MB (2621972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3508da0a7a8c69badd89084de30d788f3c0bc57d625677ec7d68c32f18d466ba`  
		Last Modified: Wed, 04 May 2022 22:03:28 GMT  
		Size: 4.5 MB (4510625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7965b001731ee55e0b7b2c11c7ff5f851afaed57dba5ef2a08324fab5de994f7`  
		Last Modified: Wed, 04 May 2022 22:03:27 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8d031fa4afb68088db4a684f2332c5c8c3ecedb55d2aee461d64c8556afb468`  
		Last Modified: Wed, 04 May 2022 22:03:25 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:7d6c71099975b1e928511819a05612d582d412c5ed2838f04882514d0e77fff8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.9 MB (6930001 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3813055a26f58efed9d97ad053203ba493589fa6e486f3dd5810354defc6b3c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 04 Apr 2022 23:57:34 GMT
ADD file:20f8cdddc53a4a8bd78945fc32fe08e9f80ab3b16dc20a9aa4ba73b79f2bc71c in / 
# Mon, 04 Apr 2022 23:57:35 GMT
CMD ["/bin/sh"]
# Wed, 04 May 2022 22:17:46 GMT
ENV NATS_SERVER=2.8.2
# Wed, 04 May 2022 22:17:50 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='3409b9dc76c0136cecded67115521d3a815f7a2f3739e81eb87a8d5d761843c3' ;; 		armhf) natsArch='arm6'; sha256='a3d474a583ca90e3577aa470335c582d4565918f500ebd28d760643fb631d8d5' ;; 		armv7) natsArch='arm7'; sha256='88fd437f7def8dbe68b17dce703c919771e64b570856bf0e6f2eb3b9459031c6' ;; 		x86_64) natsArch='amd64'; sha256='59805a464237801574ca7efdc69ebc21040e9b811fb53ed444c4808a05440719' ;; 		x86) natsArch='386'; sha256='facd3c69ee27c3e9e8654e5de95eb79de2e873bf4c066317aa9fad5c2ea26b92' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 04 May 2022 22:17:50 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 04 May 2022 22:17:51 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 04 May 2022 22:17:51 GMT
EXPOSE 4222 6222 8222
# Wed, 04 May 2022 22:17:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 04 May 2022 22:17:52 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:57fb4b5f1a47c953ca5703f0f81ce14e5d01cf23aa79558b5adb961cc526e320`  
		Last Modified: Mon, 04 Apr 2022 19:09:36 GMT  
		Size: 2.4 MB (2424323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b49f3de3c7329a4a2fbd9e8c9cd595a837860930995c5a11d2459e045b8d2dab`  
		Last Modified: Wed, 04 May 2022 22:20:00 GMT  
		Size: 4.5 MB (4504680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51dc12ec06d594c70e53bb45c9912d27ad4869faf092615047ea9faab11d6ccb`  
		Last Modified: Wed, 04 May 2022 22:19:57 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5e0c0af17ebf42f5af072c2b71c091af0b659ac5e20a80c92ca74da9ec5353d`  
		Last Modified: Wed, 04 May 2022 22:19:57 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:81e20b06f2b5aac1ca438142975de9c05234b243fcb497ab8afd7f0bcd4a28a8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7208259 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12c2a5e86ad6fc84ed6f66fecfc26474466d0f61712b85aa012fc0b7e726019e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:31 GMT
ADD file:90e56af13188c7f0283d244a0d70b853d8bef8587a41f1da8eac3a2aba8964ef in / 
# Mon, 04 Apr 2022 23:39:31 GMT
CMD ["/bin/sh"]
# Wed, 04 May 2022 21:48:24 GMT
ENV NATS_SERVER=2.8.2
# Wed, 04 May 2022 21:48:26 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='3409b9dc76c0136cecded67115521d3a815f7a2f3739e81eb87a8d5d761843c3' ;; 		armhf) natsArch='arm6'; sha256='a3d474a583ca90e3577aa470335c582d4565918f500ebd28d760643fb631d8d5' ;; 		armv7) natsArch='arm7'; sha256='88fd437f7def8dbe68b17dce703c919771e64b570856bf0e6f2eb3b9459031c6' ;; 		x86_64) natsArch='amd64'; sha256='59805a464237801574ca7efdc69ebc21040e9b811fb53ed444c4808a05440719' ;; 		x86) natsArch='386'; sha256='facd3c69ee27c3e9e8654e5de95eb79de2e873bf4c066317aa9fad5c2ea26b92' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 04 May 2022 21:48:28 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 04 May 2022 21:48:29 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 04 May 2022 21:48:29 GMT
EXPOSE 4222 6222 8222
# Wed, 04 May 2022 21:48:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 04 May 2022 21:48:31 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9981e73032c8833e387a8f96986e560edbed12c38119e0edb0439c9c2234eac9`  
		Last Modified: Mon, 04 Apr 2022 19:09:10 GMT  
		Size: 2.7 MB (2716477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec7ea9151b15b8e90d2a0ef58393de32cefb12a7f7c7e3d7a011808b38e59565`  
		Last Modified: Wed, 04 May 2022 21:49:31 GMT  
		Size: 4.5 MB (4490808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f800447a181fc7e3f37c2e68d8374347459e1d12a8d8c8653b7da45180ae97f`  
		Last Modified: Wed, 04 May 2022 21:49:30 GMT  
		Size: 560.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:894f3b307d2ae2b261df9d763e886b3ae75f9aba6dc927eaf3f28cae9375c050`  
		Last Modified: Wed, 04 May 2022 21:49:30 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:alpine3.15`

```console
$ docker pull nats@sha256:51ed1dcadcd928cbca6b4b2846491bd14667dca111ac63fdb001eef89cb9192f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:alpine3.15` - linux; amd64

```console
$ docker pull nats@sha256:3dfa6b8def0d3c784ef7827f0c21b17afd01be56773c68d5950e9f29172ae796
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.7 MB (7667828 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3370f8d5fa5f0ea4cfdcaa60d7f568c2cf9e9752f3a75d11b0d30a257db8a51d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 05 Apr 2022 00:19:59 GMT
ADD file:5d673d25da3a14ce1f6cf66e4c7fd4f4b85a3759a9d93efb3fd9ff852b5b56e4 in / 
# Tue, 05 Apr 2022 00:19:59 GMT
CMD ["/bin/sh"]
# Wed, 04 May 2022 21:19:44 GMT
ENV NATS_SERVER=2.8.2
# Wed, 04 May 2022 21:19:47 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='3409b9dc76c0136cecded67115521d3a815f7a2f3739e81eb87a8d5d761843c3' ;; 		armhf) natsArch='arm6'; sha256='a3d474a583ca90e3577aa470335c582d4565918f500ebd28d760643fb631d8d5' ;; 		armv7) natsArch='arm7'; sha256='88fd437f7def8dbe68b17dce703c919771e64b570856bf0e6f2eb3b9459031c6' ;; 		x86_64) natsArch='amd64'; sha256='59805a464237801574ca7efdc69ebc21040e9b811fb53ed444c4808a05440719' ;; 		x86) natsArch='386'; sha256='facd3c69ee27c3e9e8654e5de95eb79de2e873bf4c066317aa9fad5c2ea26b92' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 04 May 2022 21:19:47 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 04 May 2022 21:19:47 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 04 May 2022 21:19:47 GMT
EXPOSE 4222 6222 8222
# Wed, 04 May 2022 21:19:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 04 May 2022 21:19:47 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:df9b9388f04ad6279a7410b85cedfdcb2208c0a003da7ab5613af71079148139`  
		Last Modified: Mon, 04 Apr 2022 19:10:16 GMT  
		Size: 2.8 MB (2814559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb157527e1f2e860f2700cadfdf0bed3ac0d50b8a177dd0b906431b0d46b44b5`  
		Last Modified: Wed, 04 May 2022 21:20:20 GMT  
		Size: 4.9 MB (4852271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c29bade32b2ef2ecc8325cbc5cbbf69470e5e20cc04e292244e704f68b9a6f86`  
		Last Modified: Wed, 04 May 2022 21:20:19 GMT  
		Size: 585.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dbec41bc3a042cdbf4c2e9b57c99bf99a4552e64a437be0066d42a04e3de650`  
		Last Modified: Wed, 04 May 2022 21:20:19 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.15` - linux; arm variant v6

```console
$ docker pull nats@sha256:12b766cef3be0b9dc70e35a9cefcecbfad16a19e00b94a4737134ebbee24ea31
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7133599 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d1cc5ce43b7fd2c1dc34d986696c64da1a158fc067f5a4710ce475ce2f10eaec`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 04 Apr 2022 23:49:42 GMT
ADD file:159dcddaab900372df882a4e94615ed84250e9cea3e74bc0479d98280342f596 in / 
# Mon, 04 Apr 2022 23:49:42 GMT
CMD ["/bin/sh"]
# Wed, 04 May 2022 22:01:15 GMT
ENV NATS_SERVER=2.8.2
# Wed, 04 May 2022 22:01:19 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='3409b9dc76c0136cecded67115521d3a815f7a2f3739e81eb87a8d5d761843c3' ;; 		armhf) natsArch='arm6'; sha256='a3d474a583ca90e3577aa470335c582d4565918f500ebd28d760643fb631d8d5' ;; 		armv7) natsArch='arm7'; sha256='88fd437f7def8dbe68b17dce703c919771e64b570856bf0e6f2eb3b9459031c6' ;; 		x86_64) natsArch='amd64'; sha256='59805a464237801574ca7efdc69ebc21040e9b811fb53ed444c4808a05440719' ;; 		x86) natsArch='386'; sha256='facd3c69ee27c3e9e8654e5de95eb79de2e873bf4c066317aa9fad5c2ea26b92' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 04 May 2022 22:01:20 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 04 May 2022 22:01:20 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 04 May 2022 22:01:21 GMT
EXPOSE 4222 6222 8222
# Wed, 04 May 2022 22:01:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 04 May 2022 22:01:21 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:c319b1fc4ed70b8241a7ce6ac0c4015d354bf5cf8c01eb73c50b6709c0c46e49`  
		Last Modified: Mon, 04 Apr 2022 19:09:22 GMT  
		Size: 2.6 MB (2621972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3508da0a7a8c69badd89084de30d788f3c0bc57d625677ec7d68c32f18d466ba`  
		Last Modified: Wed, 04 May 2022 22:03:28 GMT  
		Size: 4.5 MB (4510625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7965b001731ee55e0b7b2c11c7ff5f851afaed57dba5ef2a08324fab5de994f7`  
		Last Modified: Wed, 04 May 2022 22:03:27 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8d031fa4afb68088db4a684f2332c5c8c3ecedb55d2aee461d64c8556afb468`  
		Last Modified: Wed, 04 May 2022 22:03:25 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.15` - linux; arm variant v7

```console
$ docker pull nats@sha256:7d6c71099975b1e928511819a05612d582d412c5ed2838f04882514d0e77fff8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.9 MB (6930001 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3813055a26f58efed9d97ad053203ba493589fa6e486f3dd5810354defc6b3c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 04 Apr 2022 23:57:34 GMT
ADD file:20f8cdddc53a4a8bd78945fc32fe08e9f80ab3b16dc20a9aa4ba73b79f2bc71c in / 
# Mon, 04 Apr 2022 23:57:35 GMT
CMD ["/bin/sh"]
# Wed, 04 May 2022 22:17:46 GMT
ENV NATS_SERVER=2.8.2
# Wed, 04 May 2022 22:17:50 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='3409b9dc76c0136cecded67115521d3a815f7a2f3739e81eb87a8d5d761843c3' ;; 		armhf) natsArch='arm6'; sha256='a3d474a583ca90e3577aa470335c582d4565918f500ebd28d760643fb631d8d5' ;; 		armv7) natsArch='arm7'; sha256='88fd437f7def8dbe68b17dce703c919771e64b570856bf0e6f2eb3b9459031c6' ;; 		x86_64) natsArch='amd64'; sha256='59805a464237801574ca7efdc69ebc21040e9b811fb53ed444c4808a05440719' ;; 		x86) natsArch='386'; sha256='facd3c69ee27c3e9e8654e5de95eb79de2e873bf4c066317aa9fad5c2ea26b92' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 04 May 2022 22:17:50 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 04 May 2022 22:17:51 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 04 May 2022 22:17:51 GMT
EXPOSE 4222 6222 8222
# Wed, 04 May 2022 22:17:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 04 May 2022 22:17:52 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:57fb4b5f1a47c953ca5703f0f81ce14e5d01cf23aa79558b5adb961cc526e320`  
		Last Modified: Mon, 04 Apr 2022 19:09:36 GMT  
		Size: 2.4 MB (2424323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b49f3de3c7329a4a2fbd9e8c9cd595a837860930995c5a11d2459e045b8d2dab`  
		Last Modified: Wed, 04 May 2022 22:20:00 GMT  
		Size: 4.5 MB (4504680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51dc12ec06d594c70e53bb45c9912d27ad4869faf092615047ea9faab11d6ccb`  
		Last Modified: Wed, 04 May 2022 22:19:57 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5e0c0af17ebf42f5af072c2b71c091af0b659ac5e20a80c92ca74da9ec5353d`  
		Last Modified: Wed, 04 May 2022 22:19:57 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.15` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:81e20b06f2b5aac1ca438142975de9c05234b243fcb497ab8afd7f0bcd4a28a8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7208259 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12c2a5e86ad6fc84ed6f66fecfc26474466d0f61712b85aa012fc0b7e726019e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:31 GMT
ADD file:90e56af13188c7f0283d244a0d70b853d8bef8587a41f1da8eac3a2aba8964ef in / 
# Mon, 04 Apr 2022 23:39:31 GMT
CMD ["/bin/sh"]
# Wed, 04 May 2022 21:48:24 GMT
ENV NATS_SERVER=2.8.2
# Wed, 04 May 2022 21:48:26 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='3409b9dc76c0136cecded67115521d3a815f7a2f3739e81eb87a8d5d761843c3' ;; 		armhf) natsArch='arm6'; sha256='a3d474a583ca90e3577aa470335c582d4565918f500ebd28d760643fb631d8d5' ;; 		armv7) natsArch='arm7'; sha256='88fd437f7def8dbe68b17dce703c919771e64b570856bf0e6f2eb3b9459031c6' ;; 		x86_64) natsArch='amd64'; sha256='59805a464237801574ca7efdc69ebc21040e9b811fb53ed444c4808a05440719' ;; 		x86) natsArch='386'; sha256='facd3c69ee27c3e9e8654e5de95eb79de2e873bf4c066317aa9fad5c2ea26b92' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 04 May 2022 21:48:28 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 04 May 2022 21:48:29 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 04 May 2022 21:48:29 GMT
EXPOSE 4222 6222 8222
# Wed, 04 May 2022 21:48:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 04 May 2022 21:48:31 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9981e73032c8833e387a8f96986e560edbed12c38119e0edb0439c9c2234eac9`  
		Last Modified: Mon, 04 Apr 2022 19:09:10 GMT  
		Size: 2.7 MB (2716477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec7ea9151b15b8e90d2a0ef58393de32cefb12a7f7c7e3d7a011808b38e59565`  
		Last Modified: Wed, 04 May 2022 21:49:31 GMT  
		Size: 4.5 MB (4490808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f800447a181fc7e3f37c2e68d8374347459e1d12a8d8c8653b7da45180ae97f`  
		Last Modified: Wed, 04 May 2022 21:49:30 GMT  
		Size: 560.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:894f3b307d2ae2b261df9d763e886b3ae75f9aba6dc927eaf3f28cae9375c050`  
		Last Modified: Wed, 04 May 2022 21:49:30 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:latest`

```console
$ docker pull nats@sha256:78f4dc57504675513e5051ce8f64598ddede060ec74a5ff9f253143b7a081503
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.2803; amd64

### `nats:latest` - linux; amd64

```console
$ docker pull nats@sha256:d7022e467f53812285667fd004413e8cb15920efbb01d1d0f7c4194a2e084959
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4580109 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:71863590dea616f7cf93b753e1e7a3baf16f89747f06004d08f65d3fa907ee9a`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 04 May 2022 21:19:54 GMT
COPY file:1b0e004de765c2bffa3154a8b1990e8a621636f4f1d7ff504c566b8ba440d227 in /nats-server 
# Wed, 04 May 2022 21:19:54 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 04 May 2022 21:19:54 GMT
EXPOSE 4222 6222 8222
# Wed, 04 May 2022 21:19:54 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 04 May 2022 21:19:54 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 04 May 2022 21:19:54 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:cf7d6008a72749fed702f25d8a1bb63636b75bf34655ba074286dc54d0db2b5b`  
		Last Modified: Wed, 04 May 2022 21:20:43 GMT  
		Size: 4.6 MB (4579600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3ef91ad4507cb0bd768e027792377ba07aaaebc8d89981a6ee648d58561273b`  
		Last Modified: Wed, 04 May 2022 21:20:43 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm variant v6

```console
$ docker pull nats@sha256:80a268344378d95bf616b13ab6e787e5a242cadbaa9c933e6708bb8761cab22f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4238279 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d53b2041383be620a877c3c265658998b4c5a2f31c6f26d3dd2aa53cb78cf527`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 04 May 2022 22:01:42 GMT
COPY file:ed82059457db34cc43492a36d55b5f9133e36b8d203dcc971bb9feb5fb6a8528 in /nats-server 
# Wed, 04 May 2022 22:01:42 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 04 May 2022 22:01:43 GMT
EXPOSE 4222 6222 8222
# Wed, 04 May 2022 22:01:43 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 04 May 2022 22:01:44 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 04 May 2022 22:01:44 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b04b6f92c475d8e5e8cdec268c94ef3240dde7149afb05913d1099a7ae570a08`  
		Last Modified: Wed, 04 May 2022 22:04:04 GMT  
		Size: 4.2 MB (4237771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef916f73f04fb010ef2bb2bf3b7260ca2d52efb2591d966721af6b5251fd397d`  
		Last Modified: Wed, 04 May 2022 22:04:02 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm variant v7

```console
$ docker pull nats@sha256:5faa61f14caf7dc441f38d86641bd5918d1231b40e7acd0336f57843d8ef704b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4232641 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c4caf3fcf0c7865ec8500f33783b2ba88253c0e14828b887cc8b103228346c5`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 04 May 2022 22:18:15 GMT
COPY file:2f9ffa15f39f94a4d8c8c940d7ec0b2baee22852f8f3f2c24a707b69fc8fd84f in /nats-server 
# Wed, 04 May 2022 22:18:15 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 04 May 2022 22:18:16 GMT
EXPOSE 4222 6222 8222
# Wed, 04 May 2022 22:18:16 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 04 May 2022 22:18:17 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 04 May 2022 22:18:17 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:706ff613d28c2f6958458bb4d4ce83f519f2b76bde307418fe1603aac99ac21b`  
		Last Modified: Wed, 04 May 2022 22:20:36 GMT  
		Size: 4.2 MB (4232133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb718277dd458fca567c81e0168c051df2d97f4a8eb0cb348574822d90dec67d`  
		Last Modified: Wed, 04 May 2022 22:20:33 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:009869128938685fc6fee44029ac90758f29d3fc3e33fa7d5e47a7a3905ef115
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4218329 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a787d12c02030cc31984da44a61d89f3f472271982d215d29866617891286b13`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 04 May 2022 21:48:41 GMT
COPY file:8d0405148efb3d718582f81ff5f54494a8c9789f05e85832ee98d04d228af450 in /nats-server 
# Wed, 04 May 2022 21:48:42 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 04 May 2022 21:48:42 GMT
EXPOSE 4222 6222 8222
# Wed, 04 May 2022 21:48:43 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 04 May 2022 21:48:44 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 04 May 2022 21:48:45 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:8d57fa8f4dba3b0b06e2fd0e4e7b35276d5c1078bcf1be00321d6d56bba9aa78`  
		Last Modified: Wed, 04 May 2022 21:50:01 GMT  
		Size: 4.2 MB (4217820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b388c4e085cdf26d57e7c86c2bec5f6519929e7f9ec591330158ba39d77677b4`  
		Last Modified: Wed, 04 May 2022 21:50:00 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - windows version 10.0.17763.2803; amd64

```console
$ docker pull nats@sha256:2b4914d94facbb6299c5ef2598f655a224c0f671a265bd2986f62c70b978582c
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.7 MB (107725201 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:762896cf7b68aecb4d2820c48789eeee8a8cbc7a58862c4bec5f4ad9d2ecd8f3`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 04 Apr 2022 10:52:49 GMT
RUN Apply image 1809-amd64
# Wed, 13 Apr 2022 14:45:42 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 04 May 2022 21:17:46 GMT
RUN cmd /S /C #(nop) COPY file:1e690007468fe11473f18dc8fbc8b7aa29351e71d03ca73f75d9fcfbf1fd7911 in C:\nats-server.exe 
# Wed, 04 May 2022 21:17:47 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 04 May 2022 21:17:48 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 04 May 2022 21:17:49 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 04 May 2022 21:17:49 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6fc97003d8b7f593fe071cf3ea64f3ce760cc060f3402bb6b1b849c040e222d5`  
		Size: 103.1 MB (103096169 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a6063f744e542c21ce471bdd7ff0dd6063d8d2a9670afbbc64d086813afd6385`  
		Last Modified: Wed, 13 Apr 2022 14:46:35 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c1e5f9285a324194ea2fae24594852b07a0fc1cec1388dcbc367215de23c29e`  
		Last Modified: Wed, 04 May 2022 21:18:39 GMT  
		Size: 4.6 MB (4622651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bde4044fa24dd3365cdc6ba5dff0779813bd4d34e566af1a5c4458c0a232fdc1`  
		Last Modified: Wed, 04 May 2022 21:18:38 GMT  
		Size: 1.8 KB (1791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:405a229a99882e5792c0dad43c80fb315b37c8b9c347f514baccd7d05c6c9f1c`  
		Last Modified: Wed, 04 May 2022 21:18:38 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1037a060f2ca6801837d7d720ec02ed6916e48ce1cfa49e6c7558ba04de8235`  
		Last Modified: Wed, 04 May 2022 21:18:38 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e29f6c2056586ca9353c7019499d854ba31068b682d59304ed4267576ebc5286`  
		Last Modified: Wed, 04 May 2022 21:18:38 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:linux`

```console
$ docker pull nats@sha256:dd400785e2c069158ca6a488873976cab93098904db7fcc044cfc6af0327640c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:linux` - linux; amd64

```console
$ docker pull nats@sha256:d7022e467f53812285667fd004413e8cb15920efbb01d1d0f7c4194a2e084959
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4580109 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:71863590dea616f7cf93b753e1e7a3baf16f89747f06004d08f65d3fa907ee9a`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 04 May 2022 21:19:54 GMT
COPY file:1b0e004de765c2bffa3154a8b1990e8a621636f4f1d7ff504c566b8ba440d227 in /nats-server 
# Wed, 04 May 2022 21:19:54 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 04 May 2022 21:19:54 GMT
EXPOSE 4222 6222 8222
# Wed, 04 May 2022 21:19:54 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 04 May 2022 21:19:54 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 04 May 2022 21:19:54 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:cf7d6008a72749fed702f25d8a1bb63636b75bf34655ba074286dc54d0db2b5b`  
		Last Modified: Wed, 04 May 2022 21:20:43 GMT  
		Size: 4.6 MB (4579600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3ef91ad4507cb0bd768e027792377ba07aaaebc8d89981a6ee648d58561273b`  
		Last Modified: Wed, 04 May 2022 21:20:43 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:80a268344378d95bf616b13ab6e787e5a242cadbaa9c933e6708bb8761cab22f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4238279 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d53b2041383be620a877c3c265658998b4c5a2f31c6f26d3dd2aa53cb78cf527`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 04 May 2022 22:01:42 GMT
COPY file:ed82059457db34cc43492a36d55b5f9133e36b8d203dcc971bb9feb5fb6a8528 in /nats-server 
# Wed, 04 May 2022 22:01:42 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 04 May 2022 22:01:43 GMT
EXPOSE 4222 6222 8222
# Wed, 04 May 2022 22:01:43 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 04 May 2022 22:01:44 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 04 May 2022 22:01:44 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b04b6f92c475d8e5e8cdec268c94ef3240dde7149afb05913d1099a7ae570a08`  
		Last Modified: Wed, 04 May 2022 22:04:04 GMT  
		Size: 4.2 MB (4237771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef916f73f04fb010ef2bb2bf3b7260ca2d52efb2591d966721af6b5251fd397d`  
		Last Modified: Wed, 04 May 2022 22:04:02 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:5faa61f14caf7dc441f38d86641bd5918d1231b40e7acd0336f57843d8ef704b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4232641 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c4caf3fcf0c7865ec8500f33783b2ba88253c0e14828b887cc8b103228346c5`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 04 May 2022 22:18:15 GMT
COPY file:2f9ffa15f39f94a4d8c8c940d7ec0b2baee22852f8f3f2c24a707b69fc8fd84f in /nats-server 
# Wed, 04 May 2022 22:18:15 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 04 May 2022 22:18:16 GMT
EXPOSE 4222 6222 8222
# Wed, 04 May 2022 22:18:16 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 04 May 2022 22:18:17 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 04 May 2022 22:18:17 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:706ff613d28c2f6958458bb4d4ce83f519f2b76bde307418fe1603aac99ac21b`  
		Last Modified: Wed, 04 May 2022 22:20:36 GMT  
		Size: 4.2 MB (4232133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb718277dd458fca567c81e0168c051df2d97f4a8eb0cb348574822d90dec67d`  
		Last Modified: Wed, 04 May 2022 22:20:33 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:009869128938685fc6fee44029ac90758f29d3fc3e33fa7d5e47a7a3905ef115
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4218329 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a787d12c02030cc31984da44a61d89f3f472271982d215d29866617891286b13`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 04 May 2022 21:48:41 GMT
COPY file:8d0405148efb3d718582f81ff5f54494a8c9789f05e85832ee98d04d228af450 in /nats-server 
# Wed, 04 May 2022 21:48:42 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 04 May 2022 21:48:42 GMT
EXPOSE 4222 6222 8222
# Wed, 04 May 2022 21:48:43 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 04 May 2022 21:48:44 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 04 May 2022 21:48:45 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:8d57fa8f4dba3b0b06e2fd0e4e7b35276d5c1078bcf1be00321d6d56bba9aa78`  
		Last Modified: Wed, 04 May 2022 21:50:01 GMT  
		Size: 4.2 MB (4217820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b388c4e085cdf26d57e7c86c2bec5f6519929e7f9ec591330158ba39d77677b4`  
		Last Modified: Wed, 04 May 2022 21:50:00 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:nanoserver`

```console
$ docker pull nats@sha256:f128bdd66f848762f7bb7c580b2d89e4c329ce85461597353dcbff405ddda643
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2803; amd64

### `nats:nanoserver` - windows version 10.0.17763.2803; amd64

```console
$ docker pull nats@sha256:2b4914d94facbb6299c5ef2598f655a224c0f671a265bd2986f62c70b978582c
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.7 MB (107725201 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:762896cf7b68aecb4d2820c48789eeee8a8cbc7a58862c4bec5f4ad9d2ecd8f3`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 04 Apr 2022 10:52:49 GMT
RUN Apply image 1809-amd64
# Wed, 13 Apr 2022 14:45:42 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 04 May 2022 21:17:46 GMT
RUN cmd /S /C #(nop) COPY file:1e690007468fe11473f18dc8fbc8b7aa29351e71d03ca73f75d9fcfbf1fd7911 in C:\nats-server.exe 
# Wed, 04 May 2022 21:17:47 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 04 May 2022 21:17:48 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 04 May 2022 21:17:49 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 04 May 2022 21:17:49 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6fc97003d8b7f593fe071cf3ea64f3ce760cc060f3402bb6b1b849c040e222d5`  
		Size: 103.1 MB (103096169 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a6063f744e542c21ce471bdd7ff0dd6063d8d2a9670afbbc64d086813afd6385`  
		Last Modified: Wed, 13 Apr 2022 14:46:35 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c1e5f9285a324194ea2fae24594852b07a0fc1cec1388dcbc367215de23c29e`  
		Last Modified: Wed, 04 May 2022 21:18:39 GMT  
		Size: 4.6 MB (4622651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bde4044fa24dd3365cdc6ba5dff0779813bd4d34e566af1a5c4458c0a232fdc1`  
		Last Modified: Wed, 04 May 2022 21:18:38 GMT  
		Size: 1.8 KB (1791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:405a229a99882e5792c0dad43c80fb315b37c8b9c347f514baccd7d05c6c9f1c`  
		Last Modified: Wed, 04 May 2022 21:18:38 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1037a060f2ca6801837d7d720ec02ed6916e48ce1cfa49e6c7558ba04de8235`  
		Last Modified: Wed, 04 May 2022 21:18:38 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e29f6c2056586ca9353c7019499d854ba31068b682d59304ed4267576ebc5286`  
		Last Modified: Wed, 04 May 2022 21:18:38 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:nanoserver-1809`

```console
$ docker pull nats@sha256:f128bdd66f848762f7bb7c580b2d89e4c329ce85461597353dcbff405ddda643
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2803; amd64

### `nats:nanoserver-1809` - windows version 10.0.17763.2803; amd64

```console
$ docker pull nats@sha256:2b4914d94facbb6299c5ef2598f655a224c0f671a265bd2986f62c70b978582c
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.7 MB (107725201 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:762896cf7b68aecb4d2820c48789eeee8a8cbc7a58862c4bec5f4ad9d2ecd8f3`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 04 Apr 2022 10:52:49 GMT
RUN Apply image 1809-amd64
# Wed, 13 Apr 2022 14:45:42 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 04 May 2022 21:17:46 GMT
RUN cmd /S /C #(nop) COPY file:1e690007468fe11473f18dc8fbc8b7aa29351e71d03ca73f75d9fcfbf1fd7911 in C:\nats-server.exe 
# Wed, 04 May 2022 21:17:47 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 04 May 2022 21:17:48 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 04 May 2022 21:17:49 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 04 May 2022 21:17:49 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6fc97003d8b7f593fe071cf3ea64f3ce760cc060f3402bb6b1b849c040e222d5`  
		Size: 103.1 MB (103096169 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a6063f744e542c21ce471bdd7ff0dd6063d8d2a9670afbbc64d086813afd6385`  
		Last Modified: Wed, 13 Apr 2022 14:46:35 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c1e5f9285a324194ea2fae24594852b07a0fc1cec1388dcbc367215de23c29e`  
		Last Modified: Wed, 04 May 2022 21:18:39 GMT  
		Size: 4.6 MB (4622651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bde4044fa24dd3365cdc6ba5dff0779813bd4d34e566af1a5c4458c0a232fdc1`  
		Last Modified: Wed, 04 May 2022 21:18:38 GMT  
		Size: 1.8 KB (1791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:405a229a99882e5792c0dad43c80fb315b37c8b9c347f514baccd7d05c6c9f1c`  
		Last Modified: Wed, 04 May 2022 21:18:38 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1037a060f2ca6801837d7d720ec02ed6916e48ce1cfa49e6c7558ba04de8235`  
		Last Modified: Wed, 04 May 2022 21:18:38 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e29f6c2056586ca9353c7019499d854ba31068b682d59304ed4267576ebc5286`  
		Last Modified: Wed, 04 May 2022 21:18:38 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:scratch`

```console
$ docker pull nats@sha256:dd400785e2c069158ca6a488873976cab93098904db7fcc044cfc6af0327640c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:scratch` - linux; amd64

```console
$ docker pull nats@sha256:d7022e467f53812285667fd004413e8cb15920efbb01d1d0f7c4194a2e084959
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4580109 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:71863590dea616f7cf93b753e1e7a3baf16f89747f06004d08f65d3fa907ee9a`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 04 May 2022 21:19:54 GMT
COPY file:1b0e004de765c2bffa3154a8b1990e8a621636f4f1d7ff504c566b8ba440d227 in /nats-server 
# Wed, 04 May 2022 21:19:54 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 04 May 2022 21:19:54 GMT
EXPOSE 4222 6222 8222
# Wed, 04 May 2022 21:19:54 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 04 May 2022 21:19:54 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 04 May 2022 21:19:54 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:cf7d6008a72749fed702f25d8a1bb63636b75bf34655ba074286dc54d0db2b5b`  
		Last Modified: Wed, 04 May 2022 21:20:43 GMT  
		Size: 4.6 MB (4579600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3ef91ad4507cb0bd768e027792377ba07aaaebc8d89981a6ee648d58561273b`  
		Last Modified: Wed, 04 May 2022 21:20:43 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:80a268344378d95bf616b13ab6e787e5a242cadbaa9c933e6708bb8761cab22f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4238279 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d53b2041383be620a877c3c265658998b4c5a2f31c6f26d3dd2aa53cb78cf527`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 04 May 2022 22:01:42 GMT
COPY file:ed82059457db34cc43492a36d55b5f9133e36b8d203dcc971bb9feb5fb6a8528 in /nats-server 
# Wed, 04 May 2022 22:01:42 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 04 May 2022 22:01:43 GMT
EXPOSE 4222 6222 8222
# Wed, 04 May 2022 22:01:43 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 04 May 2022 22:01:44 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 04 May 2022 22:01:44 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b04b6f92c475d8e5e8cdec268c94ef3240dde7149afb05913d1099a7ae570a08`  
		Last Modified: Wed, 04 May 2022 22:04:04 GMT  
		Size: 4.2 MB (4237771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef916f73f04fb010ef2bb2bf3b7260ca2d52efb2591d966721af6b5251fd397d`  
		Last Modified: Wed, 04 May 2022 22:04:02 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:5faa61f14caf7dc441f38d86641bd5918d1231b40e7acd0336f57843d8ef704b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4232641 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c4caf3fcf0c7865ec8500f33783b2ba88253c0e14828b887cc8b103228346c5`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 04 May 2022 22:18:15 GMT
COPY file:2f9ffa15f39f94a4d8c8c940d7ec0b2baee22852f8f3f2c24a707b69fc8fd84f in /nats-server 
# Wed, 04 May 2022 22:18:15 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 04 May 2022 22:18:16 GMT
EXPOSE 4222 6222 8222
# Wed, 04 May 2022 22:18:16 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 04 May 2022 22:18:17 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 04 May 2022 22:18:17 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:706ff613d28c2f6958458bb4d4ce83f519f2b76bde307418fe1603aac99ac21b`  
		Last Modified: Wed, 04 May 2022 22:20:36 GMT  
		Size: 4.2 MB (4232133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb718277dd458fca567c81e0168c051df2d97f4a8eb0cb348574822d90dec67d`  
		Last Modified: Wed, 04 May 2022 22:20:33 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:009869128938685fc6fee44029ac90758f29d3fc3e33fa7d5e47a7a3905ef115
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4218329 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a787d12c02030cc31984da44a61d89f3f472271982d215d29866617891286b13`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 04 May 2022 21:48:41 GMT
COPY file:8d0405148efb3d718582f81ff5f54494a8c9789f05e85832ee98d04d228af450 in /nats-server 
# Wed, 04 May 2022 21:48:42 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 04 May 2022 21:48:42 GMT
EXPOSE 4222 6222 8222
# Wed, 04 May 2022 21:48:43 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 04 May 2022 21:48:44 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 04 May 2022 21:48:45 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:8d57fa8f4dba3b0b06e2fd0e4e7b35276d5c1078bcf1be00321d6d56bba9aa78`  
		Last Modified: Wed, 04 May 2022 21:50:01 GMT  
		Size: 4.2 MB (4217820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b388c4e085cdf26d57e7c86c2bec5f6519929e7f9ec591330158ba39d77677b4`  
		Last Modified: Wed, 04 May 2022 21:50:00 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:windowsservercore`

```console
$ docker pull nats@sha256:73f511081ca198af5f5c5d1d5d609bf6cfc5a7d43f01e1c93b4b718eaa7bc1d7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2803; amd64

### `nats:windowsservercore` - windows version 10.0.17763.2803; amd64

```console
$ docker pull nats@sha256:6ed34062ddcdb57863540c220de7d892b2b3152ae6599e25ff1405defc63d9db
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2721253627 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:392c84a5f744aeb82235810dec31fe58510c59683d8530e1727645ae02a45a8f`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 04 Apr 2022 11:20:25 GMT
RUN Install update 1809-amd64
# Wed, 13 Apr 2022 12:43:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 Apr 2022 14:42:30 GMT
ENV NATS_DOCKERIZED=1
# Wed, 04 May 2022 21:14:48 GMT
ENV NATS_SERVER=2.8.2
# Wed, 04 May 2022 21:14:49 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.8.2/nats-server-v2.8.2-windows-amd64.zip
# Wed, 04 May 2022 21:14:50 GMT
ENV NATS_SERVER_SHASUM=300b9743afa50e02e4e8d43dc212bfde8a871617bd524829114e19ff680dde11
# Wed, 04 May 2022 21:15:50 GMT
RUN Set-PSDebug -Trace 2
# Wed, 04 May 2022 21:17:21 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 04 May 2022 21:17:22 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 04 May 2022 21:17:23 GMT
EXPOSE 4222 6222 8222
# Wed, 04 May 2022 21:17:24 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 04 May 2022 21:17:26 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ba8181afd4264392fbbf8df14fb4cddc55fbe085ab000e986b789678bc2bb171`  
		Size: 997.6 MB (997587446 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7ebb23aa64bff633cfa3c62b190d84f0e870b04fecb1910f65d0870b5c7f8981`  
		Last Modified: Wed, 13 Apr 2022 14:12:24 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d838c7a98a95bee63894bac798124e8c8572bcacc23e22d85332d453a03a7d7c`  
		Last Modified: Wed, 13 Apr 2022 14:46:17 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bba18134d0cef899134f811c0896e8003b4b03b11726200e2d4f09ff3e350d1`  
		Last Modified: Wed, 04 May 2022 21:18:21 GMT  
		Size: 1.4 KB (1382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46e1de2ac2611197cf7e3985577bdf089a2330268d7f08ad53a25b42fcf7548b`  
		Last Modified: Wed, 04 May 2022 21:18:21 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:130538769de262aeb26e810412f9ee58d5b8c1aeb653929a4607901c92363b93`  
		Last Modified: Wed, 04 May 2022 21:18:21 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1684bc7f189afcbdc72f3a0c8eab43e13bbfbe3e8fb412ac51356098cefaeb9a`  
		Last Modified: Wed, 04 May 2022 21:18:21 GMT  
		Size: 359.4 KB (359393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c1c4f2e32fa9a2920cfaeae75fe3b7e64312357d7a20b2c5e7347936eef6dc5`  
		Last Modified: Wed, 04 May 2022 21:18:24 GMT  
		Size: 5.0 MB (4960732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c18367f87433f56d999dc8c84a381afa2e8d480302ea8c78e9169557cd843606`  
		Last Modified: Wed, 04 May 2022 21:18:18 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9279a91eef9f2b4bb4964ed362b6786dc737d38e07cb0266dcbe7441930a27f0`  
		Last Modified: Wed, 04 May 2022 21:18:18 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1ff9295d7bb66afbef49bab61a76a250ae513e6acdd9a8312b8a153c2cae64c`  
		Last Modified: Wed, 04 May 2022 21:18:18 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ce0d33690a32dfd5fb8003a197bdc540ec1d876be17a42ccd82d94634514974`  
		Last Modified: Wed, 04 May 2022 21:18:18 GMT  
		Size: 1.4 KB (1363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:windowsservercore-1809`

```console
$ docker pull nats@sha256:73f511081ca198af5f5c5d1d5d609bf6cfc5a7d43f01e1c93b4b718eaa7bc1d7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2803; amd64

### `nats:windowsservercore-1809` - windows version 10.0.17763.2803; amd64

```console
$ docker pull nats@sha256:6ed34062ddcdb57863540c220de7d892b2b3152ae6599e25ff1405defc63d9db
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2721253627 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:392c84a5f744aeb82235810dec31fe58510c59683d8530e1727645ae02a45a8f`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 04 Apr 2022 11:20:25 GMT
RUN Install update 1809-amd64
# Wed, 13 Apr 2022 12:43:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 Apr 2022 14:42:30 GMT
ENV NATS_DOCKERIZED=1
# Wed, 04 May 2022 21:14:48 GMT
ENV NATS_SERVER=2.8.2
# Wed, 04 May 2022 21:14:49 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.8.2/nats-server-v2.8.2-windows-amd64.zip
# Wed, 04 May 2022 21:14:50 GMT
ENV NATS_SERVER_SHASUM=300b9743afa50e02e4e8d43dc212bfde8a871617bd524829114e19ff680dde11
# Wed, 04 May 2022 21:15:50 GMT
RUN Set-PSDebug -Trace 2
# Wed, 04 May 2022 21:17:21 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 04 May 2022 21:17:22 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 04 May 2022 21:17:23 GMT
EXPOSE 4222 6222 8222
# Wed, 04 May 2022 21:17:24 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 04 May 2022 21:17:26 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ba8181afd4264392fbbf8df14fb4cddc55fbe085ab000e986b789678bc2bb171`  
		Size: 997.6 MB (997587446 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7ebb23aa64bff633cfa3c62b190d84f0e870b04fecb1910f65d0870b5c7f8981`  
		Last Modified: Wed, 13 Apr 2022 14:12:24 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d838c7a98a95bee63894bac798124e8c8572bcacc23e22d85332d453a03a7d7c`  
		Last Modified: Wed, 13 Apr 2022 14:46:17 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bba18134d0cef899134f811c0896e8003b4b03b11726200e2d4f09ff3e350d1`  
		Last Modified: Wed, 04 May 2022 21:18:21 GMT  
		Size: 1.4 KB (1382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46e1de2ac2611197cf7e3985577bdf089a2330268d7f08ad53a25b42fcf7548b`  
		Last Modified: Wed, 04 May 2022 21:18:21 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:130538769de262aeb26e810412f9ee58d5b8c1aeb653929a4607901c92363b93`  
		Last Modified: Wed, 04 May 2022 21:18:21 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1684bc7f189afcbdc72f3a0c8eab43e13bbfbe3e8fb412ac51356098cefaeb9a`  
		Last Modified: Wed, 04 May 2022 21:18:21 GMT  
		Size: 359.4 KB (359393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c1c4f2e32fa9a2920cfaeae75fe3b7e64312357d7a20b2c5e7347936eef6dc5`  
		Last Modified: Wed, 04 May 2022 21:18:24 GMT  
		Size: 5.0 MB (4960732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c18367f87433f56d999dc8c84a381afa2e8d480302ea8c78e9169557cd843606`  
		Last Modified: Wed, 04 May 2022 21:18:18 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9279a91eef9f2b4bb4964ed362b6786dc737d38e07cb0266dcbe7441930a27f0`  
		Last Modified: Wed, 04 May 2022 21:18:18 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1ff9295d7bb66afbef49bab61a76a250ae513e6acdd9a8312b8a153c2cae64c`  
		Last Modified: Wed, 04 May 2022 21:18:18 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ce0d33690a32dfd5fb8003a197bdc540ec1d876be17a42ccd82d94634514974`  
		Last Modified: Wed, 04 May 2022 21:18:18 GMT  
		Size: 1.4 KB (1363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
